COMMENT =		Media Player Classic Qute Theater

V =			23.12
GH_ACCOUNT =		mpc-qt
GH_PROJECT =		mpc-qt
GH_TAGNAME =		v${V}

CATEGORIES =		x11

HOMEPAGE =		https://mpc-qt.github.io

MAINTAINER =		"Ed <ed@i2pmail.org>"

# GPLv2
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBCXX} mpv Qt6Core
WANTLIB +=		GL Qt6DBus Qt6Gui Qt6Network Qt6OpenGL
WANTLIB +=		Qt6OpenGLWidgets Qt6Widgets c m

COMPILER =		base-clang ports-gcc

MODULES =		devel/qmake

BUILD_DEPENDS =		x11/qt6/qtsvg \
			x11/qt6/qttools
LIB_DEPENDS =		multimedia/mpv \
			x11/qt6/qtbase

MODQT_QMAKE =		qmake-qt6
MODQMAKE_ARGS +=	MPCQT_VERSION=${V}

NO_TEST =		Yes

.include <bsd.port.mk>
