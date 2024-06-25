BROKEN =		i am no longer providing the unofficial source tarball or maintaining. may fixup when 1.0 is released
COMMENT =		open and free bittorrent tracker

DISTNAME =		opentracker-0.1-110868ec
PKGNAME =		opentracker-0.1

CATEGORIES =		net

HOMEPAGE =		https://erdgeist.org/arts/software/opentracker/

MAINTAINER =		"Ed <ed@i2pmail.org>"

# beerware
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBC} owfat

MASTER_SITES =		https://www.d-rine.com/pub/Software2/SRC/

COMPILER =		base-clang ports-gcc base-gcc
COMPILER_LANGS =	c

LIB_DEPENDS =		devel/libowfat

CONFIGURE_STYLE =	none

NO_TEST =		Yes

post-install:
	${INSTALL_DATA_DIR} ${PREFIX}/share/examples/opentracker
	${INSTALL_DATA} ${FILESDIR}/opentracker.conf ${PREFIX}/share/examples/opentracker/

.include <bsd.port.mk>
