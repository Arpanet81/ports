# $FreeBSD$

PORTNAME=	newrelic_rpm
PORTVERSION=	4.0.0.332
CATEGORIES=	devel rubygems
MASTER_SITES=	RG

MAINTAINER=	ruby@FreeBSD.org
COMMENT=	Performance management system for Rails applications

LICENSE=	MIT NEWRELIC RUBY
LICENSE_COMB=	multi
LICENSE_NAME_NEWRELIC=	New Relic License
LICENSE_FILE_NEWRELIC=	${WRKSRC}/LICENSE
LICENSE_PERMS_NEWRELIC=	dist-mirror no-dist-sell pkg-mirror no-pkg-sell auto-accept

NO_ARCH=	yes
USE_RUBY=	yes
USES=		gem shebangfix

PLIST_FILES=	bin/mongrel_rpm bin/newrelic bin/newrelic_cmd bin/nrdebug

SHEBANG_FILES=	test/script/*.sh

.include <bsd.port.mk>
