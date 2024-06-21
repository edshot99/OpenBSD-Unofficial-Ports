COMMENT =		MPEG Transport Stream Toolkit

# TODO: cannot update to 3.37-3670 without patches or support for LibreSSL
V1 =			3.36
V2 =			3528
PKGNAME =		tsduck-${V1}.${V2}

GH_ACCOUNT =		tsduck
GH_PROJECT =		tsduck
GH_TAGNAME =		v${V1}-${V2}

# tsduck Makefile needs to be hacked on for proper SHARED_LIBS
#SHARED_LIBS =		tsduck	0.0	# ???

CATEGORIES =		multimedia

HOMEPAGE =		https://tsduck.io

MAINTAINER =		"Ed <ed@i2pmail.org>"

# BSD-2
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBCXX} edit curl rist

COMPILER =		base-clang ports-gcc

LIB_DEPENDS =		multimedia/librist \
			net/curl

FAKE_FLAGS =		SYSROOT=${WRKINST}

USE_GMAKE =		Yes
CONFIGURE_STYLE =	none

NO_TEST =		Yes

ALL_TARGET =		default

.include <bsd.port.mk>
