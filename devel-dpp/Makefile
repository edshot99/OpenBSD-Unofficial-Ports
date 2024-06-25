COMMENT =		Discord API Bot Library

# 10.0.30 fails on unit tests
V =			10.0.29
DISTNAME =		DPP-${V}

SHARED_LIBS =		dpp	0.0	# 10.0.29

CATEGORIES =		devel

HOMEPAGE =		https://dpp.dev

MAINTAINER =		"Ed <ed@i2pmail.org>"

# Apache-2.0
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBCXX} sodium opus crypto m ssl z

SITES =			https://github.com/brainboxdotcc/DPP/releases/download/v${V}/

COMPILER =		base-clang ports-gcc

MODULES =		devel/cmake

BUILD_DEPENDS =		devel/cmake
LIB_DEPENDS =		audio/opus \
			security/libsodium

CONFIGURE_ARGS =	-DRUN_LDCONFIG=OFF

NO_TEST =		Yes

.include <bsd.port.mk>
