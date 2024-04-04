COMMENT =		Source RCON client for command line

GH_ACCOUNT =		n0la
GH_PROJECT =		rcon
GH_TAGNAME =		0.6

CATEGORIES =		net

HOMEPAGE =		https://github.com/n0la/rcon

MAINTAINER =		"Ed <ed@i2pmail.org>"

# BSD-2
PERMIT_PACKAGE =	Yes

# uses pledge()

WANTLIB =		${COMPILER_LIBC} glib-2.0 intl iconv pcre2-8

COMPILER =		base-clang ports-gcc base-gcc
COMPILER_LANGS =	c

MODULES =		devel/cmake

BUILD_DEPENDS =		devel/check \
			devel/cmake
LIB_DEPENDS =		devel/glib2

NO_TEST =		Yes

.include <bsd.port.mk>
