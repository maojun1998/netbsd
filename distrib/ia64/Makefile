#	$NetBSD: Makefile,v 1.1 2016/08/05 16:18:19 scole Exp $

.include <bsd.own.mk>
.include "${NETBSDSRCDIR}/distrib/common/Makefile.distrib"

.include <bsd.kernobj.mk>

# XXX add other SUBDIR

SUBDIR=		cdroms
#SUBDIR+=	netboot ramdisk

TARGETS+=	release

# XXX sort out loader.efi
#BOOTOBJ!=	cd ${KERNSRCDIR}/arch/ia64/stand/ia64/efi && ${PRINTOBJDIR}
#EFIBOOTERS=	${BOOTOBJ}/loader.sym ${BOOTOBJ}/loader.efi

#release: check_RELEASEDIR .WAIT ${EFIBOOTERS}
#	${RELEASE_INSTALL} ${EFIBOOTERS} ${RELEASEDIR}/${RELEASEMACHINEDIR}/installation

iso_image:
	${MAKEDIRTARGET} cdroms iso_image

.include <bsd.subdir.mk>
