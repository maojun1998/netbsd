# $NetBSD: Makefile,v 1.33 2017/05/27 21:02:56 bouyer Exp $

.include <bsd.own.mk>

TESTSDIR=	${TESTSBASE}/net

TESTS_SUBDIRS=		fdpass in_cksum net sys
.if (${MKRUMP} != "no") && !defined(BSD_MK_COMPAT_FILE)
TESTS_SUBDIRS+=		arp bpf bpfilter can carp icmp if if_bridge if_gif
TESTS_SUBDIRS+=		if_l2tp if_loop if_pppoe if_tap if_tun ipsec
TESTS_SUBDIRS+=		mcast mpls ndp npf route if_vlan
.if (${MKSLJIT} != "no")
TESTS_SUBDIRS+=		bpfjit
.endif
.endif

.include <bsd.test.mk>
