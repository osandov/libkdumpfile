## Process this file with automake to create Makefile.in
## Configure input file for libkdumpfile.
##
## Copyright (C) 2015 Ales Novak <alnovak@suse.cz>
##
## This file is part of libkdumpfile.
##
## This file is free software; you can redistribute it and/or modify
## it under the terms of the GNU General Public License as published by
## the Free Software Foundation; either version 3 of the License, or
## (at your option) any later version.
##
## libkdumpfile is distributed in the hope that it will be useful, but
## WITHOUT ANY WARRANTY; without even the implied warranty of
## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
## GNU General Public License for more details.
##
## You should have received a copy of the GNU General Public License
## along with this program.  If not, see <http://www.gnu.org/licenses/>.
##

kdumpfiledir = $(pkgpythondir)

pyexec_LTLIBRARIES = _kdumpfile.la

_kdumpfile_la_SOURCES = kdumpfile.c
_kdumpfile_la_CPPFLAGS = $(PYTHON_CFLAGS) -I$(top_srcdir)/src
_kdumpfile_la_LDFLAGS = -module -avoid-version -export-symbols-regex init_kdumpfile
_kdumpfile_la_LIBADD = $(top_builddir)/src/libkdumpfile.la
