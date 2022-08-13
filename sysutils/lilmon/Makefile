# $OpenBSD$

COMMENT = minimalistic monitoring application

MODGO_MODNAME =	github.com/susji/lilmon
MODGO_VERSION =	v0.10.0

DISTNAME = lilmon-${MODGO_VERSION}
PKGNAME =	lilmon-0.10.0

CATEGORIES = sysutils

HOMEPAGE = https://github.com/susji/lilmon

# GPLv3 only
PERMIT_PACKAGE = Yes

MODULES =	lang/go

post-install:
	${INSTALL_DATA_DIR} ${WRKINST}/${SYSCONFDIR}/lilmon
	${INSTALL_DATA_DIR} ${WRKINST}/${LOCALSTATEDIR}/lilmon/db
	${INSTALL_DATA_DIR} ${PREFIX}/share/examples/lilmon

	${INSTALL_DATA} ${WRKSRC}/lilmon.ini.example \
		${PREFIX}/share/examples/lilmon/lilmon.ini
	${INSTALL_DATA} ${WRKSRC}/lilmon.template.example \
		${PREFIX}/share/examples/lilmon/lilmon.template

.include "modules.inc"

.include <bsd.port.mk>
