# $OpenBSD: Makefile,v 1.6 2011/09/16 11:41:41 espie Exp $

COMMENT=		RDF Parser Toolkit for Redland
DISTNAME=		raptor2-2.0.7
PKGNAME=		${DISTNAME:C/raptor2/raptor/}
CATEGORIES=		textproc

SHARED_LIBS=		raptor2	0.0 # 0.0

HOMEPAGE=		http://librdf.org/

MASTER_SITES=		http://download.librdf.org/source/

# LGPL 2.1, GPL 2 or Apache 2
PERMIT_PACKAGE_CDROM=	Yes
PERMIT_PACKAGE_FTP=	Yes
PERMIT_DISTFILES_CDROM=	Yes
PERMIT_DISTFILES_FTP=	Yes

WANTLIB=		c crypto idn m ssl z curl>=12 xml2>=7 xslt>=1

MODULES=		devel/gettext

USE_LIBTOOL=		Yes
USE_GROFF =		Yes

LIB_DEPENDS=		net/curl \
			textproc/libxml \
			textproc/libxslt

CONFIGURE_STYLE=	gnu
CONFIGURE_ARGS=		--with-xml-parser=libxml \
			--with-www=curl

.include <bsd.port.mk>
