COMMENT =		file archiver with a high compression ratio

V =			24.08
DISTNAME =		7z2408-src
PKGNAME =		7zip-${V}

CATEGORIES =		archivers

HOMEPAGE =		https://7-zip.org

MAINTAINER =		"Ed <ed@i2pmail.org>"

# LGPLv2.1
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBCXX} c m

SITES =			"https://github.com/ip7z/7zip/releases/download/${V}/"

EXTRACT_SUFX =		.tar.xz

FIX_CRLF_FILES =	CPP/7zip/7zip_gcc.mak

COMPILER =		base-clang ports-gcc

USE_GMAKE =		Yes
CONFIGURE_STYLE =	none

NO_TEST =		Yes

MAKE_FILE_base-clang = 	../../cmpl_clang.mak
MAKE_FILE_ports-gcc =	../../cmpl_gcc.mak
MAKE_FILE =		${MAKE_FILE_${CHOSEN_COMPILER}}

WRKDIST =		${WRKDIR}
WRKSRC =		${WRKDIST}/CPP/7zip/Bundles/Alone2

do-install:
	${INSTALL_PROGRAM} ${WRKSRC}/b/c/7zz ${PREFIX}/bin

.include <bsd.port.mk>
