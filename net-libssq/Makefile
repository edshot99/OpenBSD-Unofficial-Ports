COMMENT =		up-to-date Source Server Query protocol library

V =			3.0.0
REVISION =		1
GH_ACCOUNT =		BinaryAlien
GH_PROJECT =		libssq
GH_TAGNAME =		v${V}

SHARED_LIBS =		ssq	0.0

CATEGORIES =		net

HOMEPAGE =		https://github.com/BinaryAlien/libssq

MAINTAINER =		"Ed <ed@i2pmail.org>"

# MIT
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBC} c

COMPILER =		base-clang ports-gcc base-gcc
COMPILER_LANGS =	c

MODULES =		devel/cmake

BUILD_DEPENDS =		devel/cmake

NO_TEST =		Yes

.include <bsd.port.mk>
