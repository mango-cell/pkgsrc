# $NetBSD: Makefile,v 1.32 2016/03/05 11:28:20 jperkin Exp $

DISTNAME=	automoc4-0.9.88
PKGREVISION=	24
CATEGORIES=	devel
MASTER_SITES=	${MASTER_SITE_KDE:=automoc4/0.9.88/}
EXTRACT_SUFX=	.tar.bz2
DIST_SUBDIR=	automoc4

MAINTAINER=	markd@NetBSD.org
HOMEPAGE=	http://www.kde.org/
COMMENT=	Automatic moc for Qt 4 packages

USE_LANGUAGES=	c c++
USE_CMAKE=	yes
CMAKE_ARG_PATH=	..
CONFIGURE_DIRS=	_build
LDFLAGS.SunOS+=	-lrt

pre-configure:
	${LN} -sf ${QTDIR}/bin/qmake ${BUILDLINK_DIR}/bin/
	${MKDIR} ${WRKSRC}/_build

.include "../../x11/qt4-libs/buildlink3.mk"
.include "../../x11/qt4-tools/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
