COMMENT =		Alternative Discord client made in C++ with GTK

VERSION =		0.2.1
REVISION =		1
GH_ACCOUNT =		uowuo
GH_PROJECT =		abaddon
GH_TAGNAME =		v${VERSION}

CATEGORIES =		net

HOMEPAGE =		https://github.com/uowuo/abaddon

MAINTAINER =		"Ed <ed@i2pmail.org>"

# GPLv3
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBCXX} atk-1.0 atkmm-1.6 cairo gio-2.0
WANTLIB +=		giomm-2.4 glib-2.0 glibmm-2.4 gobject-2.0 harfbuzz opus
WANTLIB +=		rnnoise sigc-2.0 sqlite3 spdlog sodium handy-1 gdkmm-3.0

COMPILER =		base-clang ports-gcc

MODULES =		devel/cmake

BUILD_DEPENDS =		audio/miniaudio \
			devel/spdlog \
			security/libsodium \
			x11/gtk3mm \
			x11/libhandy

LIB_DEPENDS =		audio/opus \
			audio/rnnoise \
			databases/sqlite3 \
			devel/atk2mm \
			devel/glib2 \
			devel/glib2mm \
			devel/harfbuzz \
#			devel/keychain \
			devel/pango \
#			devel/qr-code-generator \
			devel/spdlog \
			graphics/cairo \
			graphics/gdk-pixbuf2 \
			net/curl \
			net/IXWebSocket \
			security/libsodium \
			textproc/nlohmann-json \
			x11/gtk+3 \
			x11/gtk3mm \
			x11/libhandy

RUN_DEPENDS =		devel/spdlog \
			security/libsodium \
			x11/gtk3mm \
			x11/libhandy

# devel/keychain requires GNOME or KDE "Secret Service" which I don't use nor want.
CONFIGURE_ARGS +=	-DUSE_KEYCHAIN=OFF

# devel/qr-code-generator has linking problem.
CONFIGURE_ARGS +=	-DENABLE_QRCODE_LOGIN=OFF

# https://github.com/uowuo/abaddon/issues/280
CXXFLAGS =		-O1 -pipe

NO_TEST =		Yes

.include <bsd.port.mk>
