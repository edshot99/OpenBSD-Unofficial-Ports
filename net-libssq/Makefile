COMMENT =		up-to-date Source Server Query protocol library

GH_ACCOUNT =		BinaryAlien
GH_PROJECT =		libssq
GH_TAGNAME =		v3.0.0

CATEGORIES =		net

HOMEPAGE =		https://github.com/BinaryAlien/libssq

MAINTAINER =		"Ed <ed@i2pmail.org>"

# MIT
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBC}

COMPILER =		base-clang ports-gcc base-gcc
COMPILER_LANGS =	c

MODULES =		devel/cmake

BUILD_DEPENDS =		devel/cmake

NO_TEST =		Yes

do-install:
	${INSTALL_DATA} ${WRKBUILD}/${GH_PROJECT}.a ${PREFIX}/lib/

.include <bsd.port.mk>
