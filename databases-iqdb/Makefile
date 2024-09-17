COMMENT =		Image Query Database System

PKGNAME =		iqdb-0.1

DIST_TUPLE +=		github e621ng iqdb d42a65ba35523eb46152744d68d8ff302c1c9f92 .

CATEGORIES =		databases

HOMEPAGE =		https://github.com/e621ng/iqdb

MAINTAINER =		"Ed <ed@i2pmail.org>"

# GPLv2+
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBCXX} sqlite3 fmt c m z
WANTLIB +=		brotlicommon brotlidec brotlienc

COMPILER =		base-clang ports-gcc

MODULES =		devel/cmake

BUILD_DEPENDS =		devel/cmake \
			devel/cpp-httplib \
			devel/sqlite-orm \
			textproc/nlohmann-json

RUN_DEPENDS =		archivers/brotli

LIB_DEPENDS =		databases/sqlite3 \
			devel/fmt

TEST_DEPENDS =		devel/catch2

# Missing CMakeLists.txt for test/
NO_TEST =		Yes

.include <bsd.port.mk>
