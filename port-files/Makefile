# $FreeBSD$

PORTNAME=	trueos-desktop
PORTVERSION=	%%CHGVERSION%%
CATEGORIES=	misc
MASTER_SITES=
DISTFILES=

MAINTAINER=	jmaloney@ixsystems.com
COMMENT=	TrueOS Desktop

LICENSE=	BSD2CLAUSE

RUN_DEPENDS=	${LOCALBASE}/sbin/PCDMd:x11/pcdm \
		${LOCALBASE}/bin/pc-updatemanager:sysutils/pc-updatemanager \
		${LOCALBASE}/bin/qsudo:sysutils/qsudo \
		${LOCALBASE}/bin/pc-wificonfig:sysutils/pc-networkmanager \
		${LOCALBASE}/sbin/pc-sysinstall:sysutils/pc-sysinstall \
		${LOCALBASE}/share/trueos/scripts/functions.sh:sysutils/trueos-libsh \
		${LOCALBASE}/bin/pc-firstgui:sysutils/trueos-utils \
		${LOCALBASE}/bin/pc-firstboot:sysutils/trueos-utils-qt5 \
		${LOCALBASE}/bin/pc-mixer:audio/pc-mixer \
		${LOCALBASE}/bin/sysadm-binary:sysutils/sysadm \
		${LOCALBASE}/bin/sysadm-client:sysutils/sysadm-client \
		${LOCALBASE}/bin/lpreserver:sysutils/life-preserver \
		${LOCALBASE}/bin/personacrypt:sysutils/personacrypt \
		${LOCALBASE}/bin/pc-webkitviewer:www/pc-webkitviewer \
		${LOCALBASE}/sbin/beadm:sysutils/beadm \
		${LOCALBASE}/bin/xdg-open:devel/xdg-utils \
		${LOCALBASE}/bin/xvkbd:x11/xvkbd \
		${LOCALBASE}/sbin/anacron:sysutils/anacron \
		cups-filters>=0:print/cups-filters \
		drm-next-kmod>=g20170918:graphics/drm-next-kmod \
		trueos-handbook>=0:misc/trueos-handbook \
		lumina>=0:x11/lumina \
		foomatic-db>=0:print/foomatic-db \
		fluxbox-tenr-styles-pack>=0:x11-themes/fluxbox-tenr-styles-pack \
		xorg-minimal>=0:x11/xorg-minimal \
		xorg-drivers>=0:x11-drivers/xorg-drivers \
		nss_mdns>=0:dns/nss_mdns \
		cuse4bsd-kmod>=0:multimedia/cuse4bsd-kmod \
		webcamd>=0:multimedia/webcamd \
		pciutils>=0:sysutils/pciutils \
		pam_mkhomedir>=0:security/pam_mkhomedir \
		x11vnc>=0:net/x11vnc \
		openntpd>=0:net/openntpd \
		git:devel/git \
		xv>=0:graphics/xv \
		tor>=0:security/tor \
		socat>=0:net/socat \
		mesa-demos>=0:graphics/mesa-demos \
		dhcpcd>=0:net/dhcpcd \
		bsdstats>=0:sysutils/bsdstats

WRKSRC_SUBDIR=  xtrafiles
MAKE_ARGS=      PREFIX=${STAGEDIR}${PREFIX}

CONFLICTS=      pcbsd-utils-[0-9]* trueos-server-[0-9]*
WRKSRC_SUBDIR=	xtrafiles
MAKE_ARGS=	PREFIX=${STAGEDIR}${PREFIX}

USE_GITHUB=     yes
GH_ACCOUNT=     trueos
GH_PROJECT=     trueos-core
GH_TAGNAME=     %%GHTAG%%

.include <bsd.port.mk>
