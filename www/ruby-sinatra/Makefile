# $NetBSD: Makefile,v 1.24 2018/01/08 14:34:41 taca Exp $

DISTNAME=	sinatra-2.0.0
CATEGORIES=	www

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://www.sinatrarb.com/
COMMENT=	Classy web-development dressed in a DSL
LICENSE=	mit

DEPENDS+=	${RUBY_PKGPREFIX}-rack>=2.0<3:../../www/ruby-rack
DEPENDS+=	${RUBY_PKGPREFIX}-rack-protection>=2.0.0:../../www/ruby-rack-protection
DEPENDS+=	${RUBY_PKGPREFIX}-mustermann>=1.0<2:../../www/ruby-mustermann
DEPENDS+=	${RUBY_PKGPREFIX}-tilt>=2.0<3:../../textproc/ruby-tilt

.include "../../lang/ruby/gem.mk"
.include "../../mk/bsd.pkg.mk"
