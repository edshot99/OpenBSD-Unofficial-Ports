COMMENT =		Reliable Internet Stream Transport library

VERSION =		0.2.10
DISTNAME =		librist-v${VERSION}
PKGNAME =		librist-${VERSION}

SHARED_LIBS =		rist	0.0	# 4.3.1

CATEGORIES =		multimedia

HOMEPAGE =		https://code.videolan.org/rist/librist

MAINTAINER =		"Ed <ed@i2pmail.org>"

# BSD-2
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBC} c pthread nettle hogweed gmp gnutls cjson

SITES =			https://code.videolan.org/rist/librist/-/archive/v${VERSION}/

COMPILER =		base-clang ports-gcc base-gcc
COMPILER_LANGS =	c

MODULES =		devel/meson

BUILD_DEPENDS =		devel/meson

LIB_DEPENDS =		devel/cjson \
			security/gnutls \
			security/libnettle

TEST_DEPENDS =		devel/cmocka

NO_TEST =		Yes

.include <bsd.port.mk>
