# $NetBSD: Makefile,v 1.6 2017/11/23 17:19:57 wiz Exp $

DISTNAME=	paper-icon-theme-1.3.2
PKGREVISION=	5
CATEGORIES=	graphics
MASTER_SITES=	${MASTER_SITE_GITHUB:=snwh/}

MAINTAINER=	youri@NetBSD.org
HOMEPAGE=	https://github.com/snwh/paper-icon-theme/
COMMENT=	Modern freedesktop icon theme
LICENSE=	gnu-gpl-v3

GITHUB_TAG=	v${PKGVERSION_NOREV}

GNU_CONFIGURE=	yes
USE_LIBTOOL=	yes
USE_TOOLS+=	automake pkg-config

SUBST_CLASSES+=		configure
SUBST_STAGE.configure=	pre-configure
SUBST_FILES.configure=	configure.ac
SUBST_SED.configure=	-e 's,/usr/local,${PREFIX},'

pre-configure:
		cd ${WRKSRC} && ./autogen.sh

.include "../../x11/gtk2/buildlink3.mk"
.include "../../x11/gtk3/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
