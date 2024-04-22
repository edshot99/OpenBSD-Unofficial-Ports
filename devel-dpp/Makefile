COMMENT =		Discord API Bot Library

GH_ACCOUNT =		brainboxdotcc
GH_PROJECT =		DPP
GH_TAGNAME =		v10.0.29

SHARED_LIBS =		dpp	0.0	# 10.0.29

CATEGORIES =		devel

HOMEPAGE =		https://dpp.dev

MAINTAINER =		"Ed <ed@i2pmail.org>"

# Apache-2.0
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBCXX} sodium opus

COMPILER =		base-clang ports-gcc

MODULES =		devel/cmake

BUILD_DEPENDS =		devel/cmake \
			textproc/nlohmann-json
LIB_DEPENDS =		audio/opus \
			security/libsodium

CONFIGURE_ARGS =	-DRUN_LDCONFIG=OFF -DPP_USE_EXTERNAL_JSON=ON

NO_TEST =		Yes

.include <bsd.port.mk>
