#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([update-icon-cache],[2.24.29],[xakepa10@gmail.com])
AC_CONFIG_SRCDIR([src/updateiconcache.c])
AC_CONFIG_HEADERS([config.h])
AM_INIT_AUTOMAKE

AC_PREFIX_DEFAULT([/usr])

# Checks for programs.
AC_PROG_CC
AM_PROG_CC_C_O

# Checks for header files.
AC_CHECK_HEADERS([fcntl.h locale.h stdlib.h string.h unistd.h utime.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_C_INLINE
AC_TYPE_MODE_T
AC_TYPE_SIZE_T

# Checks for library functions.
AC_CHECK_FUNCS([setlocale strchr strrchr utime])

# Check for libraries.
PKG_CHECK_MODULES(GLIB, [glib-2.0])
AC_SUBST(GLIB_CFLAGS)
AC_SUBST(GLIB_LIBS)

PKG_CHECK_MODULES(GDK, [gdk-pixbuf-2.0])
AC_SUBST(GDK_CFLAGS)
AC_SUBST(GDK_LIBS)

AC_CONFIG_FILES([Makefile
                 src/Makefile])
AC_OUTPUT
