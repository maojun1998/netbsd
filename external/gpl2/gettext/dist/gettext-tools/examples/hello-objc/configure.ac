dnl Example for use of GNU gettext.
dnl Copyright (C) 2003-2004, 2006 Free Software Foundation, Inc.
dnl This file is in the public domain.
dnl
dnl Configuration file - processed by autoconf.

AC_INIT
AC_CONFIG_SRCDIR(hello.m)
AM_INIT_AUTOMAKE(hello-objc, 0)

AC_PROG_CC
AC_SUBST(OBJC,["$CC"])
AC_CHECK_HEADERS([unistd.h])
AM_GNU_GETTEXT([external])
AM_GNU_GETTEXT_VERSION(0.15)

AC_CONFIG_FILES([Makefile])
AC_CONFIG_FILES([m4/Makefile])
AC_CONFIG_FILES([po/Makefile.in])
AC_OUTPUT
