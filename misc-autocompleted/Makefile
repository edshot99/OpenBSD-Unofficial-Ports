COMMENT =		e621ng search bar auto completion

PKGNAME =		autocompleted-0.1.0

DIST_TUPLE +=		github e621ng autocompleted 75a53598e8f7c97f9f4afa08f33db9820768403e .

CATEGORIES =		misc

HOMEPAGE =		https://github.com/e621ng/autocompleted

MAINTAINER =		"Ed <ed@i2pmail.org>"

# BSD-2
PERMIT_PACKAGE =	Yes

MODULES =		devel/cargo

CONFIGURE_STYLE =	cargo

NO_TEST =		Yes

MODCARGO_RUSTFLAGS += -L${TRUEPREFIX}/lib
MODCARGO_RUSTFLAGS += -L${LOCALBASE}/lib

post-install:
	${INSTALL_DATA_DIR} ${PREFIX}/share/examples/autocompleted
	${INSTALL_DATA} ${FILESDIR}/autocompleted.env ${PREFIX}/share/examples/autocompleted/autocompleted.env

.include "crates.inc"

.include <bsd.port.mk>
