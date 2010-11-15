dnl Process this file with autoconf to produce a configure script.
dnl Created by Anjuta application wizard.

AC_INIT(pkgsrc_applet, 0.1)

AM_INIT_AUTOMAKE(AC_PACKAGE_NAME, AC_PACKAGE_VERSION)
AC_CONFIG_SRCDIR(src/main.py)
AM_MAINTAINER_MODE

AC_ISC_POSIX
AC_PROG_CC
AM_PROG_CC_STDC
AC_HEADER_STDC

# Check Python
AM_PATH_PYTHON([2.6])
if test "x$PYTHON" = "x:"; then
    AC_MSG_ERROR([Python not found])
fi

PKG_CHECK_MODULES(PKGSRC_APPLET,
    pygtk-2.0               >= 2.10
    pygobject-2.0           >= 2.10
    gnome-python-2.0        >= 2.10
)

AC_SUBST(PYGTK_CFLAGS)
AC_SUBST(PYGTK_LIBS)
PYGTK_DEFS=`$PKG_CONFIG --variable=defsdir pygtk-2.0`
AC_SUBST(PYGTK_DEFS)

GNOME_DOC_INIT

AC_OUTPUT([
Makefile
src/Makefile
])

echo
echo $PACKAGE $VERSION
echo

echo Prefix............... : $prefix

echo
echo "Now type make to compile"
echo
