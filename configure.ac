AC_INIT([yuma123-netconfd-module-lsi-foo], [1.0], [vladimir@lightside-instruments.com])

AC_CANONICAL_SYSTEM

AM_INIT_AUTOMAKE([-Werror foreign])
LT_INIT([disable-static])

AC_PROG_CC
AC_PROG_CXX
AM_PROG_AS
AC_PROG_LIBTOOL

netconfmoduledir="$libdir/yuma"
AC_SUBST(netconfmoduledir)

yangdir="$prefix/share/yuma/modules/lsi"
AC_SUBST(yangdir)

ncx_netconf_includedir="$includedir/yuma/ncx"
AC_SUBST(ncx_netconf_includedir)

agt_netconf_includedir="$includedir/yuma/agt"
AC_SUBST(agt_netconf_includedir)

CFLAGS="$CFLAGS -g -fPIC -DDEBUG=1 -DLINUX=1 -DGCC=1"
AC_SUBST(CFLAGS)

AM_PATH_XML2

AC_CONFIG_FILES([
        Makefile
])

AC_OUTPUT
