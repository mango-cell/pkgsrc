# $NetBSD: Makefile,v 1.21 2017/08/01 16:47:37 wiz Exp $
#

DISTNAME=	ssam-1.9
PKGREVISION=	1
CATEGORIES=	editors
MASTER_SITES=	http://www.westley.demon.co.uk/src/

MAINTAINER=	agc@NetBSD.org
#HOMEPAGE=	http://www.alistaircrooks.co.uk/software.html
COMMENT=	UTF-8-aware stream editor like sed(1), using the sam command set

GNU_CONFIGURE=	yes
BUILD_TARGET=	ssam
TEST_TARGET=	tst

.include "../../misc/libutf/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
