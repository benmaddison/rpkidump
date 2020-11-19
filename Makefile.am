#
# Copyright (c) 2020 Ben Maddison
#
# Permission to use, copy, modify, and distribute this software for any
# purpose with or without fee is hereby granted, provided that the above
# copyright notice and this permission notice appear in all copies.
#
# THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
# WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
# MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
# ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
# WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
# ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
# OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.

AM_CPPFLAGS = -I$(top_srcdir)/include
AM_CPPFLAGS += -I$(top_srcdir)/src

ACLOCAL_AMFLAGS = -Im4

sbin_PROGRAMS = rpkidump
man_MANS = rpkidump.1

rpkidump_CFLAGS = $(AM_CFLAGS)

rpkidump_LDADD = $(PLATFORM_LDADD) $(PROG_LDADD) -lcrypto
rpkidump_LDADD += $(top_builddir)/compat/libcompat.la
rpkidump_LDADD += $(top_builddir)/compat/libcompatnoopt.la

rpkidump_SOURCES = rpkidump.c
rpkidump_SOURCES += print.c
rpkidump_SOURCES += ../as.c
rpkidump_SOURCES += ../cert.c
rpkidump_SOURCES += ../cms.c
rpkidump_SOURCES += ../io.c
rpkidump_SOURCES += ../ip.c
rpkidump_SOURCES += ../log.c
rpkidump_SOURCES += ../mft.c
rpkidump_SOURCES += ../roa.c
rpkidump_SOURCES += ../rsync.c
rpkidump_SOURCES += ../x509.c

rpkidump_DEPENDENCIES = rpkidump.1
