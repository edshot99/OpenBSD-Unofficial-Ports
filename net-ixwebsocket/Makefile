COMMENT =		websocket and http client and server library

GH_ACCOUNT =		machinezone
GH_PROJECT =		IXWebSocket
GH_TAGNAME =		v11.4.5

# CMakeLists.txt needs to be hacked on for building both static and shared libraries
#SHARED_LIBS =		ixwebsocket	0.0	# ???

CATEGORIES =		net

HOMEPAGE =		https://github.com/machinezone/IXWebSocket

MAINTAINER =		"Ed <ed@i2pmail.org>"

# BSD3
PERMIT_PACKAGE =	Yes

COMPILER =		base-clang ports-gcc

MODULES =		devel/cmake

CONFIGURE_ARGS =	-DUSE_TLS=TRUE

NO_TEST =		Yes

.include <bsd.port.mk>
