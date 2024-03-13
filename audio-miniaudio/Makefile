COMMENT =		Audio playback and capture library written in C

GH_ACCOUNT =		mackron
GH_PROJECT =		miniaudio
GH_TAGNAME =		0.11.21

CATEGORIES =		audio

HOMEPAGE =		https://miniaud.io/

MAINTAINER =		"Ed <ed@i2pmail.org>"

# Public Domain or MIT
PERMIT_PACKAGE =	Yes

NO_BUILD =		Yes
NO_TEST =		Yes

PKG_ARCH =		*

do-install:
	${INSTALL_DATA_DIR} ${PREFIX}/include/
	${INSTALL_DATA} ${WRKDIR}/${GH_PROJECT}-${GH_TAGNAME}/miniaudio.h ${PREFIX}/include/

.include <bsd.port.mk>
