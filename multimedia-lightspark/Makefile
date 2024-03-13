COMMENT =		open source flash player implementation

DISTNAME =		lightspark-92669267cef54041095dccf1511d1f5e2e7b566f
PKGNAME =		lightspark-0.8.7

GH_ACCOUNT =		lightspark
GH_PROJECT =		lightspark
GH_COMMIT =		92669267cef54041095dccf1511d1f5e2e7b566f

SHARED_LIBS =		lightspark	0.0	# 0.8.7

CATEGORIES =		multimedia

HOMEPAGE =		https://lightspark.github.io

MAINTAINER =		"Ed <ed@i2pmail.org>"

# GPLv3 LGPLv3
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBC} ${COMPILER_LIBCXX}
WANTLIB +=		lzma pango-1.0 SDL2 cairo GLEW jpeg avcodec swresample
WANTLIB +=		avformat curl

COMPILER =		base-clang ports-gcc

MODULES =		devel/cmake

BUILD_DEPENDS =		devel/cmake
LIB_DEPENDS =		archivers/xz \
			devel/pango \
			devel/sdl2 \
			graphics/cairo \
			graphics/glew \
			graphics/jpeg \
			graphics/ffmpeg \
			net/curl

CONFIGURE_ARGS =	-DCMAKE_BUILD_TYPE=Release -DENABLE_RTMP=False -DMANUAL_DIRECTORY=man
CONFIGURE_ENV =		LDFLAGS="-L/usr/lib -L/usr/local/lib -L/usr/X11R6/lib -lc -lc++ -lc++abi -lpthread"

NO_TEST =		Yes

.include <bsd.port.mk>
