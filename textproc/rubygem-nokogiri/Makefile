# $FreeBSD$

PORTNAME=	nokogiri
PORTVERSION=	1.7.1
CATEGORIES=	textproc rubygems
MASTER_SITES=	RG

MAINTAINER=	ruby@FreeBSD.org
COMMENT=	HTML, XML, SAX, and Reader parser

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE.txt

BUILD_DEPENDS=	rubygem-pkg-config>=1.1.7:devel/rubygem-pkg-config
RUN_DEPENDS=	rubygem-pkg-config>=1.1.7:devel/rubygem-pkg-config

USE_RUBY=	yes
USES=		gem pkgconfig
USE_GNOME=	libxml2 libxslt
CONFIGURE_ARGS=	--use-system-libraries

PLIST_FILES=	bin/nokogiri

post-install:
	${FIND} ${STAGEDIR}${PREFIX}/${GEMS_BASE_DIR} -name '*.o' -o -name '*.so' | ${XARGS} ${STRIP_CMD}
	${RMDIR} ${STAGEDIR}${PREFIX}/${GEM_LIB_DIR}/ports/

.include <bsd.port.mk>
