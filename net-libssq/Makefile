COMMENT =		up-to-date Source Server Query protocol library

V =			3.0.0
GH_ACCOUNT =		BinaryAlien
GH_PROJECT =		libssq
GH_TAGNAME =		v${V}

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
	${INSTALL_DATA_DIR} ${PREFIX}/include/ssq
	${INSTALL_DATA_DIR} ${PREFIX}/include/ssq/a2s
	${INSTALL_DATA_DIR} ${PREFIX}/include/ssq/server
	${INSTALL_DATA} ${WRKDIR}/${GH_PROJECT}-${V}/include/ssq/a2s/*.* ${PREFIX}/include/ssq/a2s/
	${INSTALL_DATA} ${WRKDIR}/${GH_PROJECT}-${V}/include/ssq/server/*.* ${PREFIX}/include/ssq/server/
	${INSTALL_DATA} ${WRKDIR}/${GH_PROJECT}-${V}/include/ssq/*.* ${PREFIX}/include/ssq/

.include <bsd.port.mk>
