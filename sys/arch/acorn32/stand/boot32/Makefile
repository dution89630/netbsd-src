#	$NetBSD: Makefile,v 1.5 2006/04/01 19:08:08 bjh21 Exp $

PROG=		boot32
PROGSOURCE=	rmheader.S rmvers.c srt0.S boot32.c start.S
NEWVERSWHAT=	"RISC OS Boot"
RISCOSTYPE=	ffa

SAMISCMAKEFLAGS+= SA_USE_LOADFILE=yes SA_USE_CREAD=yes

CPPFLAGS+=	-DBOOT_MAXIMISE_MEMORY \
		-DLIBSA_NO_FS_WRITE \
		-DLIBSA_SINGLE_FILESYSTEM=riscos

rmvers.c: ${.CURDIR}/version
	${HOST_SH} ${.CURDIR}/../lib/newvers_rm.sh ${.CURDIR}/version "NetBSD Boot"
.PHONY: rmvers.c

CLEANFILES+=	rmvers.c

.include "../Makefile.buildboot"
