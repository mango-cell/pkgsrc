# $NetBSD: Makefile,v 1.10 2014/04/30 14:19:42 wiz Exp $
#

DISTNAME=		open-axiom-1.4.1
PKGNAME=		${DISTNAME:S/open-/open/}
PKGREVISION=		3
CATEGORIES=		math
MASTER_SITES=		${MASTER_SITE_SOURCEFORGE:=open-axiom/}
EXTRACT_SUFX=		.tar.bz2

MAINTAINER=		asau@inbox.ru
HOMEPAGE=		http://www.open-axiom.org/
COMMENT=		Platform for symbolic, algebraic, and numerical computations

MAKE_JOBS_SAFE=		no

USE_LANGUAGES=		c c++
GNU_CONFIGURE=		yes
USE_TOOLS+=		gmake makeinfo awk:run
BUILD_DEPENDS+=		noweb-[0-9]*:../../devel/noweb

CONFIGURE_ENV=		HOST_AWK=${TOOLS_PLATFORM.awk:Q}
BUILD_MAKE_FLAGS+=	TOOLS_PLATFORM.install=${TOOLS_PLATFORM.install:Q}

.include "options.mk"

.include "../../mk/bsd.pkg.mk"
