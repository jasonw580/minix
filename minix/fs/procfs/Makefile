# Makefile for ProcFS server
.include <bsd.own.mk>

PROG=	procfs
SRCS=	buf.c main.c pid.c root.c tree.c util.c cpuinfo.c

CPPFLAGS+= -I${NETBSDSRCDIR}/minix
CPPFLAGS+= -I${NETBSDSRCDIR}/minix/fs
CPPFLAGS+= -I${NETBSDSRCDIR}/minix/servers

DPADD+=	${LIBVTREEFS} ${LIBFSDRIVER}
LDADD+=	-lvtreefs -lfsdriver

.include <minix.service.mk>
