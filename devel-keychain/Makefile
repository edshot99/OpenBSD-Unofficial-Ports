COMMENT =		cross-platform wrapper for the OS credential storage

GH_ACCOUNT =		hrantzsch
GH_PROJECT =		keychain
GH_TAGNAME =		v1.2.1

CATEGORIES =		devel

HOMEPAGE =		https://github.com/hrantzsch/keychain

MAINTAINER =		"Ed <ed@i2pmail.org>"

# MIT
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBCXX} glib-2.0 secret-1

COMPILER =		base-clang ports-gcc base-gcc

MODULES =		devel/cmake

LIB_DEPENDS =		devel/glib2 \
			x11/gnome/libsecret

NO_TEST =		Yes

.include <bsd.port.mk>
