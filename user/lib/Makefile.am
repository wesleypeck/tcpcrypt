lib_LTLIBRARIES = libtcpcrypt.la
libtcpcrypt_ladir = $(includedir)/tcpcrypt
libtcpcrypt_la_HEADERS = $(top_srcdir)/include/tcpcrypt/tcpcrypt.h
libtcpcrypt_la_SOURCES = sockopt.c
libtcpcrypt_la_CFLAGS  = -I$(top_srcdir)/include/ -I$(top_srcdir)

TCPCRYPT_LIBRARY_VERSION = 0:0:0
libtcpcrypt_la_LDFLAGS = -version-info $(TCPCRYPT_LIBRARY_VERSION)

if OS_MINGW
libtcpcrypt_la_LIBADD = -lws2_32
endif
