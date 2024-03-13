COMMENT =		system tray as a Window Maker dock app

DISTNAME =		wmsystemtray-1.4

CATEGORIES =		x11

HOMEPAGE =		https://www.dockapps.net/wmsystemtray

MAINTAINER =		"Ed <ed@i2pmail.org>"

# GPLv2+
PERMIT_PACKAGE =	Yes

WANTLIB =		${COMPILER_LIBC}
WANTLIB +=		X11 Xext Xfixes Xmu Xmuu

MASTER_SITES =		${MASTER_SITE_SOURCEFORGE:=wmsystemtray/}

COMPILER =		base-clang ports-gcc base-gcc

CONFIGURE_STYLE =	gnu

NO_TEST =		Yes

.include <bsd.port.mk>
