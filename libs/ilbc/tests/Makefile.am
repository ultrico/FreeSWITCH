##
## iLBC - a library for the iLBC codec
##
## Makefile.am -- Process this file with automake to produce Makefile.in
##
## This program is free software; you can redistribute it and/or modify
## it under the terms of the GNU General Public License version 2, as
## published by the Free Software Foundation.
##
## This program is distributed in the hope that it will be useful,
## but WITHOUT ANY WARRANTY; without even the implied warranty of
## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
## GNU General Public License for more details.
##
## You should have received a copy of the GNU General Public License
## along with this program; if not, write to the Free Software
## Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA.
##
## $Id: Makefile.am,v 1.1.1.1 2008/02/15 12:15:55 steveu Exp $

AM_CFLAGS = $(COMP_VENDOR_CFLAGS)

LIBS += $(TESTLIBS)

EXTRA_DIST = regression_tests.sh

MAINTAINERCLEANFILES = Makefile.in

INCLUDES = -I$(top_builddir)/src -DDATADIR="\"$(pkgdatadir)\""

LIBDIR = -L$(top_builddir)/src

noinst_PROGRAMS = ilbc_tests

ilbc_tests_SOURCES = ilbc_tests.c
ilbc_tests_LDADD = $(LIBDIR) -lilbc
