# Comparing `tmp/pypkgconf-0.1.0.tar.gz` & `tmp/pypkgconf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypkgconf-0.1.0.tar", last modified: Mon Aug  7 18:38:33 2023, max compression
+gzip compressed data, was "pypkgconf-0.1.1.tar", last modified: Tue Aug  8 14:32:22 2023, max compression
```

## Comparing `pypkgconf-0.1.0.tar` & `pypkgconf-0.1.1.tar`

### file list

```diff
@@ -1,197 +1,197 @@
--rw-rw-rw-   0        0        0       45 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/.gitignore
--rw-rw-rw-   0        0        0     2027 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      111 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/.gitmodules
--rw-rw-rw-   0        0        0    11549 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1742 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/README.md
--rw-rw-rw-   0        0        0     2093 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/cffibuild.py
--rw-rw-rw-   0        0        0     1514 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/meson.build
--rw-rw-rw-   0        0        0      181 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/pypkgconf/__init__.py
--rw-rw-rw-   0        0        0     3041 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/pypkgconf/callbacks.py
--rw-rw-rw-   0        0        0    28766 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/pypkgconf/clilike.py
--rw-rw-rw-   0        0        0     1514 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/pypkgconf/constants.py
--rw-rw-rw-   0        0        0      515 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/pypkgconf/logger.py
--rw-rw-rw-   0        0        0     1085 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/pypkgconf/meson.build
--rw-rw-rw-   0        0        0      450 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/pypkgconf/util.py
--rw-rw-rw-   0        0        0      677 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       40 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/.gitattributes
--rw-rw-rw-   0        0        0       53 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/.github/FUNDING.yml
--rw-rw-rw-   0        0        0     3477 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/.github/workflows/test.yml
--rw-rw-rw-   0        0        0      310 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/.gitignore
--rw-rw-rw-   0        0        0       70 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/.mailmap
--rw-rw-rw-   0        0        0     1708 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/.woodpecker.yml
--rw-rw-rw-   0        0        0     1539 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/AUTHORS
--rw-rw-rw-   0        0        0     1078 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0      519 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/COPYING
--rw-rw-rw-   0        0        0       65 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/Kyuafile.in
--rw-rw-rw-   0        0        0     6105 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/Makefile.am
--rw-rw-rw-   0        0        0     2519 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/Makefile.lite
--rw-rw-rw-   0        0        0    24928 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/NEWS
--rw-rw-rw-   0        0        0     6749 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/README.md
--rw-rw-rw-   0        0        0     1630 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/autogen.sh
--rw-rw-rw-   0        0        0    10006 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/cli/bomtool/main.c
--rw-rw-rw-   0        0        0    18626 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/cli/getopt_long.c
--rw-rw-rw-   0        0        0     2715 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/cli/getopt_long.h
--rw-rw-rw-   0        0        0    46369 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/cli/main.c
--rw-rw-rw-   0        0        0     3526 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/cli/renderer-msvc.c
--rw-rw-rw-   0        0        0      710 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/cli/renderer-msvc.h
--rw-rw-rw-   0        0        0     2553 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/configure.ac
--rw-rw-rw-   0        0        0    10129 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/conf.py
--rw-rw-rw-   0        0        0     5790 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/extract.py
--rw-rw-rw-   0        0        0      150 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/index.rst
--rw-rw-rw-   0        0        0      732 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst
--rw-rw-rw-   0        0        0     1488 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-audit.rst
--rw-rw-rw-   0        0        0     1841 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-cache.rst
--rw-rw-rw-   0        0        0    10184 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-client.rst
--rw-rw-rw-   0        0        0     4486 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-dependency.rst
--rw-rw-rw-   0        0        0     6067 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-fragment.rst
--rw-rw-rw-   0        0        0     3007 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-path.rst
--rw-rw-rw-   0        0        0      785 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-personality.rst
--rw-rw-rw-   0        0        0     8337 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-pkg.rst
--rw-rw-rw-   0        0        0     4439 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-queue.rst
--rw-rw-rw-   0        0        0     3982 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-tuple.rst
--rw-rw-rw-   0        0        0      392 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf.rst
--rw-rw-rw-   0        0        0     3224 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/argvsplit.c
--rw-rw-rw-   0        0        0     2991 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/audit.c
--rw-rw-rw-   0        0        0     4119 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/bsdstubs.c
--rw-rw-rw-   0        0        0     1110 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/bsdstubs.h
--rw-rw-rw-   0        0        0     5924 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/cache.c
--rw-rw-rw-   0        0        0    21142 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/client.c
--rw-rw-rw-   0        0        0     1951 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/config.h.meson
--rw-rw-rw-   0        0        0    14794 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/dependency.c
--rw-rw-rw-   0        0        0     2077 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/fileio.c
--rw-rw-rw-   0        0        0    19932 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/fragment.c
--rw-rw-rw-   0        0        0     2129 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/iter.h
--rw-rw-rw-   0        0        0      618 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/libpkgconf-api.h
--rw-rw-rw-   0        0        0    18820 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/libpkgconf.h
--rw-rw-rw-   0        0        0      233 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/meson.build
--rw-rw-rw-   0        0        0     3051 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/parser.c
--rw-rw-rw-   0        0        0     8382 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/path.c
--rw-rw-rw-   0        0        0     8960 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/personality.c
--rw-rw-rw-   0        0        0    54160 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/pkg.c
--rw-rw-rw-   0        0        0    12162 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/queue.c
--rw-rw-rw-   0        0        0     1682 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/stdinc.h
--rw-rw-rw-   0        0        0    13228 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/tuple.c
--rw-rw-rw-   0        0        0    24042 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/win-dirent.h
--rw-rw-rw-   0        0        0      351 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf.pc.in
--rw-rw-rw-   0        0        0     3405 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/m4/ax_check_compile_flag.m4
--rw-rw-rw-   0        0        0     6157 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/man/pc.5
--rw-rw-rw-   0        0        0     4148 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/man/pkg.m4.7
--rw-rw-rw-   0        0        0     3517 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/man/pkgconf-personality.5
--rw-rw-rw-   0        0        0     7933 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/man/pkgconf.1
--rw-rw-rw-   0        0        0     4340 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/meson.build
--rw-rw-rw-   0        0        0      113 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/meson_options.txt
--rw-rw-rw-   0        0        0    13078 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/pkg.m4
--rw-rw-rw-   0        0        0      347 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/Kyuafile.in
--rw-rw-rw-   0        0        0     7103 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/basic.sh
--rw-rw-rw-   0        0        0     1310 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/builtins.sh
--rw-rw-rw-   0        0        0      411 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/conflicts.sh
--rw-rw-rw-   0        0        0      497 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/framework.sh
--rw-rw-rw-   0        0        0      248 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib-relocatable/lib/pkgconfig/foo.pc
--rw-rw-rw-   0        0        0      219 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/argv-parse-2.pc
--rw-rw-rw-   0        0        0      223 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/argv-parse-3.pc
--rw-rw-rw-   0        0        0      216 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/argv-parse.pc
--rw-rw-rw-   0        0        0      194 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/bar.pc
--rw-rw-rw-   0        0        0      264 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/baz.pc
--rw-rw-rw-   0        0        0      579 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/billion-laughs.pc
--rw-rw-rw-   0        0        0      127 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/case-sensitivity.pc
--rw-rw-rw-   0        0        0      205 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/cflags-internal.pc
--rw-rw-rw-   0        0        0      231 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/cflags-libs-only.pc
--rw-rw-rw-   0        0        0      150 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/cflags-whitespace-trailing.pc
--rw-rw-rw-   0        0        0      146 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/cflags-whitespace.pc
--rw-rw-rw-   0        0        0      216 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/circular-1.pc
--rw-rw-rw-   0        0        0      216 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/circular-2.pc
--rw-rw-rw-   0        0        0      216 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/circular-3.pc
--rw-rw-rw-   0        0        0      215 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/comments-in-fields.pc
--rw-rw-rw-   0        0        0      128 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/comments.pc
--rw-rw-rw-   0        0        0      259 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/conflicts.pc
--rw-rw-rw-   0        0        0      282 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/depgraph-break.pc
--rw-rw-rw-   0        0        0      270 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/dos-lineendings.pc
--rw-rw-rw-   0        0        0       90 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/empty-tuple.pc
--rw-rw-rw-   0        0        0      111 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/escaped-backslash.pc
--rw-rw-rw-   0        0        0      170 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/explicit-sysroot.pc
--rw-rw-rw-   0        0        0      239 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/flag-order-1.pc
--rw-rw-rw-   0        0        0      254 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/flag-order-3.pc
--rw-rw-rw-   0        0        0      262 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/foo.pc
--rw-rw-rw-   0        0        0      119 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-collision-1.pc
--rw-rw-rw-   0        0        0      102 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-collision-2.pc
--rw-rw-rw-   0        0        0      175 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-collision-intermediary.pc
--rw-rw-rw-   0        0        0      205 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-collision.pc
--rw-rw-rw-   0        0        0       95 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-comment.pc
--rw-rw-rw-   0        0        0      120 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-escaping-1.pc
--rw-rw-rw-   0        0        0       96 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-escaping-2.pc
--rw-rw-rw-   0        0        0       96 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-escaping-3.pc
--rw-rw-rw-   0        0        0      267 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-quoting-2.pc
--rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-quoting-3.pc
--rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-quoting-5.pc
--rw-rw-rw-   0        0        0      172 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-quoting-7.pc
--rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/fragment-quoting.pc
--rw-rw-rw-   0        0        0      204 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/framework-1.pc
--rw-rw-rw-   0        0        0      227 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/framework-2.pc
--rw-rw-rw-   0        0        0      234 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/idirafter-ordering.pc
--rw-rw-rw-   0        0        0      245 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/idirafter.pc
--rw-rw-rw-   0        0        0      118 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/incomplete.pc
--rw-rw-rw-   0        0        0      220 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/intermediary-1.pc
--rw-rw-rw-   0        0        0      220 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/intermediary-2.pc
--rw-rw-rw-   0        0        0      239 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/isystem.pc
--rw-rw-rw-   0        0        0      160 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/malformed-1.pc
--rw-rw-rw-   0        0        0       74 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/malformed-quoting.pc
--rw-rw-rw-   0        0        0      100 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/malformed-version.pc
--rw-rw-rw-   0        0        0      164 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/metapackage-1.pc
--rw-rw-rw-   0        0        0      131 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/metapackage-2.pc
--rw-rw-rw-   0        0        0      120 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/metapackage.pc
--rw-rw-rw-   0        0        0      257 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/missing-require.pc
--rw-rw-rw-   0        0        0      178 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/multiline-bogus.pc
--rw-rw-rw-   0        0        0      178 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/multiline.pc
--rw-rw-rw-   0        0        0      280 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/no-trailing-newline.pc
--rw-rw-rw-   0        0        0      183 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/nocflag.pc
--rw-rw-rw-   0        0        0      193 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/nolib.pc
--rw-rw-rw-   0        0        0      242 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/omg-sysroot-uninstalled.pc
--rw-rw-rw-   0        0        0      218 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/omg-uninstalled.pc
--rw-rw-rw-   0        0        0      195 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/orphaned-requires-private.pc
--rw-rw-rw-   0        0        0      125 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/paren-quoting.pc
--rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/prefix-foo1.pc
--rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/prefix-foo2.pc
--rw-rw-rw-   0        0        0      124 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/private-libs-duplication.pc
--rw-rw-rw-   0        0        0      157 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/provides-request-simple.pc
--rw-rw-rw-   0        0        0      290 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/provides.pc
--rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/quotes.pc
--rw-rw-rw-   0        0        0      214 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/requires-internal-2.pc
--rw-rw-rw-   0        0        0      249 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/requires-internal-collision.pc
--rw-rw-rw-   0        0        0      242 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/requires-internal-missing.pc
--rw-rw-rw-   0        0        0      233 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/requires-internal.pc
--rw-rw-rw-   0        0        0      213 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/spaces-in-paths.pc
--rw-rw-rw-   0        0        0      235 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/static-archive-libs.pc
--rw-rw-rw-   0        0        0      266 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/static-libs.pc
--rw-rw-rw-   0        0        0      195 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/sysroot-dir-2.pc
--rw-rw-rw-   0        0        0      231 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/sysroot-dir-3.pc
--rw-rw-rw-   0        0        0      239 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/sysroot-dir-4.pc
--rw-rw-rw-   0        0        0      231 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/sysroot-dir-5.pc
--rw-rw-rw-   0        0        0      162 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/sysroot-dir.pc
--rw-rw-rw-   0        0        0       97 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/tilde-quoting.pc
--rw-rw-rw-   0        0        0      266 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/tilde.pc
--rw-rw-rw-   0        0        0      138 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/tuple-quoting.pc
--rw-rw-rw-   0        0        0      217 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/typelibdir.pc
--rw-rw-rw-   0        0        0      222 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/utf8.pc
--rw-rw-rw-   0        0        0      256 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/variable-whitespace.pc
--rw-rw-rw-   0        0        0      218 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib2/foo.pc
--rw-rw-rw-   0        0        0      194 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/lib3/bar.pc
--rw-rw-rw-   0        0        0      450 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/meson.build
--rw-rw-rw-   0        0        0     7070 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/parser.sh
--rw-rw-rw-   0        0        0     6726 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/provides.sh
--rw-rw-rw-   0        0        0     6757 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/regress.sh
--rw-rw-rw-   0        0        0     2670 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/requires.sh
--rw-rw-rw-   0        0        0     2451 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/sysroot.sh
--rw-rw-rw-   0        0        0     1247 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/test_env.sh.in
--rw-rw-rw-   0        0        0      638 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/subprojects/pkgconf/tests/version.sh
--rw-rw-rw-   0        0        0      717 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/conftest.py
--rw-rw-rw-   0        0        0     7055 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/test_basic.py
--rw-rw-rw-   0        0        0     1448 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/test_builtins.py
--rw-rw-rw-   0        0        0      409 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/test_conflicts.py
--rw-rw-rw-   0        0        0      582 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/test_framework.py
--rw-rw-rw-   0        0        0     7368 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/test_parser.py
--rw-rw-rw-   0        0        0     7241 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/test_provides.py
--rw-rw-rw-   0        0        0     7749 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/test_regress.py
--rw-rw-rw-   0        0        0     2898 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/test_requires.py
--rw-rw-rw-   0        0        0     2736 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/test_sysroot.py
--rw-rw-rw-   0        0        0      735 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/tests/test_version.py
--rw-r--r--   0        0        0    15077 1970-01-01 00:00:00.000000 pypkgconf-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       81 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/.gitignore
+-rw-rw-rw-   0        0        0     2099 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      111 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/.gitmodules
+-rw-rw-rw-   0        0        0    11549 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1900 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/README.md
+-rw-rw-rw-   0        0        0     2093 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/cffibuild.py
+-rw-rw-rw-   0        0        0     1514 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/meson.build
+-rw-rw-rw-   0        0        0      181 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/pypkgconf/__init__.py
+-rw-rw-rw-   0        0        0     3041 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/pypkgconf/callbacks.py
+-rw-rw-rw-   0        0        0    29793 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/pypkgconf/clilike.py
+-rw-rw-rw-   0        0        0     1514 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/pypkgconf/constants.py
+-rw-rw-rw-   0        0        0      515 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/pypkgconf/logger.py
+-rw-rw-rw-   0        0        0     1085 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/pypkgconf/meson.build
+-rw-rw-rw-   0        0        0      450 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/pypkgconf/util.py
+-rw-rw-rw-   0        0        0      677 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       40 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/.gitattributes
+-rw-rw-rw-   0        0        0       53 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/.github/FUNDING.yml
+-rw-rw-rw-   0        0        0     3477 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0      310 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/.gitignore
+-rw-rw-rw-   0        0        0       70 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/.mailmap
+-rw-rw-rw-   0        0        0     1708 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/.woodpecker.yml
+-rw-rw-rw-   0        0        0     1539 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/AUTHORS
+-rw-rw-rw-   0        0        0     1078 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0      519 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/COPYING
+-rw-rw-rw-   0        0        0       65 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/Kyuafile.in
+-rw-rw-rw-   0        0        0     6105 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/Makefile.am
+-rw-rw-rw-   0        0        0     2519 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/Makefile.lite
+-rw-rw-rw-   0        0        0    24928 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/NEWS
+-rw-rw-rw-   0        0        0     6749 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/README.md
+-rw-rw-rw-   0        0        0     1630 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/autogen.sh
+-rw-rw-rw-   0        0        0    10006 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/cli/bomtool/main.c
+-rw-rw-rw-   0        0        0    18626 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/cli/getopt_long.c
+-rw-rw-rw-   0        0        0     2715 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/cli/getopt_long.h
+-rw-rw-rw-   0        0        0    46369 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/cli/main.c
+-rw-rw-rw-   0        0        0     3526 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/cli/renderer-msvc.c
+-rw-rw-rw-   0        0        0      710 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/cli/renderer-msvc.h
+-rw-rw-rw-   0        0        0     2553 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/configure.ac
+-rw-rw-rw-   0        0        0    10129 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/conf.py
+-rw-rw-rw-   0        0        0     5790 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/extract.py
+-rw-rw-rw-   0        0        0      150 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/index.rst
+-rw-rw-rw-   0        0        0      732 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst
+-rw-rw-rw-   0        0        0     1488 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-audit.rst
+-rw-rw-rw-   0        0        0     1841 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-cache.rst
+-rw-rw-rw-   0        0        0    10184 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-client.rst
+-rw-rw-rw-   0        0        0     4486 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-dependency.rst
+-rw-rw-rw-   0        0        0     6067 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-fragment.rst
+-rw-rw-rw-   0        0        0     3007 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-path.rst
+-rw-rw-rw-   0        0        0      785 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-personality.rst
+-rw-rw-rw-   0        0        0     8337 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-pkg.rst
+-rw-rw-rw-   0        0        0     4439 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-queue.rst
+-rw-rw-rw-   0        0        0     3982 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-tuple.rst
+-rw-rw-rw-   0        0        0      392 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf.rst
+-rw-rw-rw-   0        0        0     3224 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/argvsplit.c
+-rw-rw-rw-   0        0        0     2991 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/audit.c
+-rw-rw-rw-   0        0        0     4119 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/bsdstubs.c
+-rw-rw-rw-   0        0        0     1110 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/bsdstubs.h
+-rw-rw-rw-   0        0        0     5924 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/cache.c
+-rw-rw-rw-   0        0        0    21142 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/client.c
+-rw-rw-rw-   0        0        0     1951 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/config.h.meson
+-rw-rw-rw-   0        0        0    14794 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/dependency.c
+-rw-rw-rw-   0        0        0     2077 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/fileio.c
+-rw-rw-rw-   0        0        0    19932 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/fragment.c
+-rw-rw-rw-   0        0        0     2129 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/iter.h
+-rw-rw-rw-   0        0        0      618 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/libpkgconf-api.h
+-rw-rw-rw-   0        0        0    18820 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/libpkgconf.h
+-rw-rw-rw-   0        0        0      233 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/meson.build
+-rw-rw-rw-   0        0        0     3051 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/parser.c
+-rw-rw-rw-   0        0        0     8382 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/path.c
+-rw-rw-rw-   0        0        0     8960 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/personality.c
+-rw-rw-rw-   0        0        0    54160 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/pkg.c
+-rw-rw-rw-   0        0        0    12162 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/queue.c
+-rw-rw-rw-   0        0        0     1682 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/stdinc.h
+-rw-rw-rw-   0        0        0    13228 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/tuple.c
+-rw-rw-rw-   0        0        0    24042 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/win-dirent.h
+-rw-rw-rw-   0        0        0      351 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf.pc.in
+-rw-rw-rw-   0        0        0     3405 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/m4/ax_check_compile_flag.m4
+-rw-rw-rw-   0        0        0     6157 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/man/pc.5
+-rw-rw-rw-   0        0        0     4148 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/man/pkg.m4.7
+-rw-rw-rw-   0        0        0     3517 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/man/pkgconf-personality.5
+-rw-rw-rw-   0        0        0     7933 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/man/pkgconf.1
+-rw-rw-rw-   0        0        0     4340 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/meson.build
+-rw-rw-rw-   0        0        0      113 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/meson_options.txt
+-rw-rw-rw-   0        0        0    13078 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/pkg.m4
+-rw-rw-rw-   0        0        0      347 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/Kyuafile.in
+-rw-rw-rw-   0        0        0     7103 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/basic.sh
+-rw-rw-rw-   0        0        0     1310 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/builtins.sh
+-rw-rw-rw-   0        0        0      411 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/conflicts.sh
+-rw-rw-rw-   0        0        0      497 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/framework.sh
+-rw-rw-rw-   0        0        0      248 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib-relocatable/lib/pkgconfig/foo.pc
+-rw-rw-rw-   0        0        0      219 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/argv-parse-2.pc
+-rw-rw-rw-   0        0        0      223 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/argv-parse-3.pc
+-rw-rw-rw-   0        0        0      216 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/argv-parse.pc
+-rw-rw-rw-   0        0        0      194 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/bar.pc
+-rw-rw-rw-   0        0        0      264 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/baz.pc
+-rw-rw-rw-   0        0        0      579 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/billion-laughs.pc
+-rw-rw-rw-   0        0        0      127 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/case-sensitivity.pc
+-rw-rw-rw-   0        0        0      205 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/cflags-internal.pc
+-rw-rw-rw-   0        0        0      231 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/cflags-libs-only.pc
+-rw-rw-rw-   0        0        0      150 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/cflags-whitespace-trailing.pc
+-rw-rw-rw-   0        0        0      146 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/cflags-whitespace.pc
+-rw-rw-rw-   0        0        0      216 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/circular-1.pc
+-rw-rw-rw-   0        0        0      216 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/circular-2.pc
+-rw-rw-rw-   0        0        0      216 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/circular-3.pc
+-rw-rw-rw-   0        0        0      215 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/comments-in-fields.pc
+-rw-rw-rw-   0        0        0      128 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/comments.pc
+-rw-rw-rw-   0        0        0      259 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/conflicts.pc
+-rw-rw-rw-   0        0        0      282 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/depgraph-break.pc
+-rw-rw-rw-   0        0        0      270 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/dos-lineendings.pc
+-rw-rw-rw-   0        0        0       90 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/empty-tuple.pc
+-rw-rw-rw-   0        0        0      111 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/escaped-backslash.pc
+-rw-rw-rw-   0        0        0      170 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/explicit-sysroot.pc
+-rw-rw-rw-   0        0        0      239 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/flag-order-1.pc
+-rw-rw-rw-   0        0        0      254 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/flag-order-3.pc
+-rw-rw-rw-   0        0        0      262 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/foo.pc
+-rw-rw-rw-   0        0        0      119 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-collision-1.pc
+-rw-rw-rw-   0        0        0      102 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-collision-2.pc
+-rw-rw-rw-   0        0        0      175 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-collision-intermediary.pc
+-rw-rw-rw-   0        0        0      205 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-collision.pc
+-rw-rw-rw-   0        0        0       95 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-comment.pc
+-rw-rw-rw-   0        0        0      120 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-escaping-1.pc
+-rw-rw-rw-   0        0        0       96 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-escaping-2.pc
+-rw-rw-rw-   0        0        0       96 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-escaping-3.pc
+-rw-rw-rw-   0        0        0      267 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-quoting-2.pc
+-rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-quoting-3.pc
+-rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-quoting-5.pc
+-rw-rw-rw-   0        0        0      172 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-quoting-7.pc
+-rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/fragment-quoting.pc
+-rw-rw-rw-   0        0        0      204 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/framework-1.pc
+-rw-rw-rw-   0        0        0      227 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/framework-2.pc
+-rw-rw-rw-   0        0        0      234 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/idirafter-ordering.pc
+-rw-rw-rw-   0        0        0      245 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/idirafter.pc
+-rw-rw-rw-   0        0        0      118 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/incomplete.pc
+-rw-rw-rw-   0        0        0      220 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/intermediary-1.pc
+-rw-rw-rw-   0        0        0      220 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/intermediary-2.pc
+-rw-rw-rw-   0        0        0      239 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/isystem.pc
+-rw-rw-rw-   0        0        0      160 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/malformed-1.pc
+-rw-rw-rw-   0        0        0       74 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/malformed-quoting.pc
+-rw-rw-rw-   0        0        0      100 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/malformed-version.pc
+-rw-rw-rw-   0        0        0      164 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/metapackage-1.pc
+-rw-rw-rw-   0        0        0      131 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/metapackage-2.pc
+-rw-rw-rw-   0        0        0      120 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/metapackage.pc
+-rw-rw-rw-   0        0        0      257 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/missing-require.pc
+-rw-rw-rw-   0        0        0      178 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/multiline-bogus.pc
+-rw-rw-rw-   0        0        0      178 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/multiline.pc
+-rw-rw-rw-   0        0        0      280 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/no-trailing-newline.pc
+-rw-rw-rw-   0        0        0      183 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/nocflag.pc
+-rw-rw-rw-   0        0        0      193 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/nolib.pc
+-rw-rw-rw-   0        0        0      242 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/omg-sysroot-uninstalled.pc
+-rw-rw-rw-   0        0        0      218 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/omg-uninstalled.pc
+-rw-rw-rw-   0        0        0      195 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/orphaned-requires-private.pc
+-rw-rw-rw-   0        0        0      125 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/paren-quoting.pc
+-rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/prefix-foo1.pc
+-rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/prefix-foo2.pc
+-rw-rw-rw-   0        0        0      124 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/private-libs-duplication.pc
+-rw-rw-rw-   0        0        0      157 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/provides-request-simple.pc
+-rw-rw-rw-   0        0        0      290 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/provides.pc
+-rw-rw-rw-   0        0        0      269 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/quotes.pc
+-rw-rw-rw-   0        0        0      214 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/requires-internal-2.pc
+-rw-rw-rw-   0        0        0      249 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/requires-internal-collision.pc
+-rw-rw-rw-   0        0        0      242 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/requires-internal-missing.pc
+-rw-rw-rw-   0        0        0      233 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/requires-internal.pc
+-rw-rw-rw-   0        0        0      213 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/spaces-in-paths.pc
+-rw-rw-rw-   0        0        0      235 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/static-archive-libs.pc
+-rw-rw-rw-   0        0        0      266 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/static-libs.pc
+-rw-rw-rw-   0        0        0      195 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/sysroot-dir-2.pc
+-rw-rw-rw-   0        0        0      231 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/sysroot-dir-3.pc
+-rw-rw-rw-   0        0        0      239 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/sysroot-dir-4.pc
+-rw-rw-rw-   0        0        0      231 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/sysroot-dir-5.pc
+-rw-rw-rw-   0        0        0      162 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/sysroot-dir.pc
+-rw-rw-rw-   0        0        0       97 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/tilde-quoting.pc
+-rw-rw-rw-   0        0        0      266 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/tilde.pc
+-rw-rw-rw-   0        0        0      138 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/tuple-quoting.pc
+-rw-rw-rw-   0        0        0      217 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/typelibdir.pc
+-rw-rw-rw-   0        0        0      222 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/utf8.pc
+-rw-rw-rw-   0        0        0      256 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/variable-whitespace.pc
+-rw-rw-rw-   0        0        0      218 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib2/foo.pc
+-rw-rw-rw-   0        0        0      194 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/lib3/bar.pc
+-rw-rw-rw-   0        0        0      450 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/meson.build
+-rw-rw-rw-   0        0        0     7070 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/parser.sh
+-rw-rw-rw-   0        0        0     6726 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/provides.sh
+-rw-rw-rw-   0        0        0     6757 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/regress.sh
+-rw-rw-rw-   0        0        0     2670 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/requires.sh
+-rw-rw-rw-   0        0        0     2451 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/sysroot.sh
+-rw-rw-rw-   0        0        0     1247 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/test_env.sh.in
+-rw-rw-rw-   0        0        0      638 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/subprojects/pkgconf/tests/version.sh
+-rw-rw-rw-   0        0        0      649 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     7488 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tests/test_basic.py
+-rw-rw-rw-   0        0        0      347 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tests/test_conflicts.py
+-rw-rw-rw-   0        0        0      536 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tests/test_framework.py
+-rw-rw-rw-   0        0        0     7792 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tests/test_parser.py
+-rw-rw-rw-   0        0        0     8662 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tests/test_provides.py
+-rw-rw-rw-   0        0        0     8401 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tests/test_regress.py
+-rw-rw-rw-   0        0        0     3065 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tests/test_requires.py
+-rw-rw-rw-   0        0        0     2748 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tests/test_sysroot.py
+-rw-rw-rw-   0        0        0      736 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tests/test_version.py
+-rw-rw-rw-   0        0        0      425 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/tox.ini
+-rw-r--r--   0        0        0    15233 1970-01-01 00:00:00.000000 pypkgconf-0.1.1/PKG-INFO
```

### Comparing `pypkgconf-0.1.0/.gitlab-ci.yml` & `pypkgconf-0.1.1/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,26 @@
         PRE: [""]
       # - PYTHON_VERSION: ["312"]
       #   PRE: ["--pre"]
   stage: Build
   rules:
     - if: $CI_MERGE_REQUEST_ID
     - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
+  variables:
+    TOXENV: py${PYTHON_VERSION}
   before_script:
     # https://gitlab.com/gitlab-org/ci-cd/shared-runners/images/gcp/windows-containers/-/issues/13
     - Import-Module "$env:ChocolateyInstall\helpers\chocolateyProfile.psm1"
     - choco install python${PYTHON_VERSION} ${PRE} --yes --force --no-progress
     - refreshenv
     - python -m pip install --upgrade pip
-    - pip install build meson cffi pytest
+    - pip install build meson cffi tox
   script:
     - python -m build -Csetup-args="-Ddefault_library=static" -Csetup-args="-Dbuildtype=release" -Cbuilddir=build
-    - meson test -C build
+    - tox --installpkg (get-item dist\*.whl).FullName
   artifacts:
     expire_in: 1 day
     paths:
       - dist
 
 
 # build_linux:
```

### Comparing `pypkgconf-0.1.0/LICENSE.txt` & `pypkgconf-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/README.md` & `pypkgconf-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -38,18 +38,20 @@
 This high-level API uses same arguments as the `pkgconf` executable.
 
 Results are returned as a list of string (the list may be empty).
 Errors and warnings are logger using the standard Python logging module, under
 the `pkgconf` logger.
 In case or error result, a `pypkgconf.PkgConfError` exception is raised.
 
-#### `pypkgconf.query_args(command: str) -> list[str]`
+#### `pypkgconf.query_args(command: str, env: dict[str, str] | None = None) -> list[str]`
 
 The command is just like the command line arguments (e.g.: `"--libs foo"`)
 
+If `env` is provided, pkgconf will use it for any envvar it queries.
+If `env` is `None` (default), `os.environ` is used.
 
 #### `pypkgconf.query(args: list[str] | None, **kwargs) -> list[str]`
 
 Positional arguments are given as a list of strings.
 
 Optional arguments are given either using an union of `pypkgconf.Flags`,
 or as keyword arguments, depending if it is a boolean value or not.
```

### Comparing `pypkgconf-0.1.0/cffibuild.py` & `pypkgconf-0.1.1/cffibuild.py`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/meson.build` & `pypkgconf-0.1.1/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 project('pypkgconf',
     ['c'],
     license: 'Apache-2.0',
     meson_version: '>=1.1.0',
-    version: '0.1.0',
+    version: '0.1.1',
 )
 
 
 libpkgconf = dependency('pkgconf', fallback: ['pkgconf', 'dep_libpkgconf'], version: '2.0.0')
 libpkgconf_include = libpkgconf.get_variable('includedir', default_value: meson.global_source_root() / 'subprojects' / 'pkgconf')
 
 fs = import('fs')
```

### Comparing `pypkgconf-0.1.0/pypkgconf/callbacks.py` & `pypkgconf-0.1.1/pypkgconf/callbacks.py`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/pypkgconf/clilike.py` & `pypkgconf-0.1.1/pypkgconf/clilike.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import argparse
 from enum import IntFlag
-from functools import reduce
+from functools import reduce, wraps
 import logging
 import operator
 import os
 import re
 import shlex
 import sys
 import typing as T
@@ -42,14 +42,31 @@
         if frag.merged:
             result.extend(item.split(' '))
         else:
             result.append(item)
 
     return result
 
+
+def preserve_env(fct):
+    @wraps(fct)
+    def wrapper(*args, **kwargs):
+
+        orig_env = os.environ.copy()
+
+        try:
+            return fct(*args, **kwargs)
+        
+        finally:
+            os.environ.clear()
+            os.environ.update(orig_env)
+
+    return wrapper
+
+
 def relocate_path(path: str) -> str:
     buf = path.encode()
     if len(buf) > lib.PKGCONF_BUFSIZE-1:
         buf = buf[:lib.PKGCONF_BUFSIZE-1]
     cbuf = ffi.new('char[]', buf)
 
     lib.pkgconf_path_relocate(cbuf, ffi.sizeof(cbuf))
@@ -326,31 +343,54 @@
             key, value = opt.split('=', maxsplit=1)
             dv[key] = value
         options.define_variable = dv
 
     return options
 
 
+@preserve_env
 def query(args: T.Optional[T.List[str]] = None,
           want_flags: Flags = Flags.DEFAULT,
+          env: T.Optional[T.Dict[str, str]] = None,
           required_module_version: T.Optional[str] = None,
           required_pkgconfig_version: T.Optional[str] = None,
           want_variable: T.Optional[str] = None,
           define_variable: T.Optional[T.Dict[str, str]] = None,
           maximum_traverse_depth: int = MAXIMUM_TRAVERSE_DEPTH,
           required_exact_module_version: T.Optional[str] = None,
           required_max_module_version: T.Optional[str] = None,
           logfile_arg: T.Optional[str] = None,
-          with_path: T.Optional[str] = None,
+          with_path: T.Optional[T.List[str]] = None,
           prefix_variable: T.Optional[str] = None,
           relocate: T.Optional[str] = None,
           want_env_prefix: T.Optional[str] = None,
           want_fragment_filter: T.Optional[str] = None,
           ) -> T.List[str]:
     
+    if env is None:
+        env = os.environ.copy()
+
+    else:
+        # Those env vars are accessed directly from libpkgconf
+        for k in ('PKG_CONFIG_PATH',
+                  'PKG_CONFIG_LIBDIR',
+                  'PKG_CONFIG_SYSTEM_LIBRARY_PATH',
+                  'PKG_CONFIG_SYSTEM_INCLUDE_PATH',
+                  'BELIBRARIES',
+                  'LIBRARY_PATH',
+                  'CPATH',
+                  'C_INCLUDE_PATH',
+                  'CPLUS_INCLUDE_PATH',
+                  'OBJC_INCLUDE_PATH',
+                  'INCLUDE'):
+            if k in env:
+                os.environ[k] = env[k]
+            elif k in os.environ:
+                del os.environ[k]
+    
     if relocate:
         return [relocate_path(relocate)]
 
     maximum_package_count = 0
     pkgq = ffi.new('pkgconf_list_t*')
     dir_list = ffi.new('pkgconf_list_t*')
     want_client_flags = lib.PKGCONF_PKG_PKGF_NONE
@@ -360,15 +400,15 @@
     world.id = id
     realname = ffi.new('char[]', 'virtual world package'.encode())
     world.realname = realname
     world.flags = lib.PKGCONF_PKG_PROPF_STATIC | lib.PKGCONF_PKG_PROPF_VIRTUAL
 
     pkg_client = ffi.new('pkgconf_client_t*')
 
-    # if os.environ.get('PKG_CONFIG_EARLY_TRACE'):
+    # if env.get('PKG_CONFIG_EARLY_TRACE'):
 
     if define_variable:
         for key, value in define_variable.items():
             lib.pkgconf_tuple_define_global(pkg_client, f'{key}={value}'.encode())
     for path in with_path or []:
         lib.pkgconf_path_add(path.encode(), dir_list, True)
     if prefix_variable:
@@ -393,26 +433,26 @@
     def raise_and_clean(*args) -> None:
         try:
             raise PkgConfError(*args)
         finally:
             cleanup()
 
 
-    if os.environ.get('PKG_CONFIG_MAXIMUM_TRAVERSE_DEPTH') is not None:
-        maximum_traverse_depth = int(os.environ.get('PKG_CONFIG_MAXIMUM_TRAVERSE_DEPTH'))
+    if env.get('PKG_CONFIG_MAXIMUM_TRAVERSE_DEPTH') is not None:
+        maximum_traverse_depth = int(env.get('PKG_CONFIG_MAXIMUM_TRAVERSE_DEPTH'))
     
     if Flags.PRINT_ERRORS not in want_flags:
         want_flags |= Flags.SILENCE_ERRORS
     
-    if Flags.SILENCE_ERRORS in want_flags and not os.environ.get('PKG_CONFIG_DEBUG_SPEW'):
+    if Flags.SILENCE_ERRORS in want_flags and not env.get('PKG_CONFIG_DEBUG_SPEW'):
         want_flags |= Flags.SILENCE_ERRORS
     else:
         want_flags &= ~Flags.SILENCE_ERRORS
     
-    if os.environ.get('PKG_CONFIG_DONT_RELOCATE_PATHS'):
+    if env.get('PKG_CONFIG_DONT_RELOCATE_PATHS'):
         want_flags |= Flags.DONT_RELOCATE_PATHS
 
     if Flags.VALIDATE in want_flags or Flags.DEBUG in want_flags:
         warning_level_handle = ffi.new_handle(logging.WARNING)
         lib.pkgconf_client_set_warn_handler(pkg_client, lib.error_handler, warning_level_handle)
 
     #ifndef PKGCONF_LITE
@@ -428,18 +468,18 @@
         try:
             return [version()]
         finally:
             cleanup()
 
     # if Flags.HELP in want_flags
 
-    if os.environ.get('PKG_CONFIG_FDO_SYSROOT_RULES'):
+    if env.get('PKG_CONFIG_FDO_SYSROOT_RULES'):
         want_client_flags |= lib.PKGCONF_PKG_PKGF_FDO_SYSROOT_RULES
 
-    if os.environ.get('PKG_CONFIG_PKGCONF1_SYSROOT_RULES'):
+    if env.get('PKG_CONFIG_PKGCONF1_SYSROOT_RULES'):
         want_client_flags |= lib.PKGCONF_PKG_PKGF_PKGCONF1_SYSROOT_RULES
 
     if Flags.SHORT_ERRORS in want_flags:
         want_client_flags |= lib.PKGCONF_PKG_PKGF_SIMPLIFY_ERRORS
     
     if Flags.DONT_RELOCATE_PATHS in want_flags:
         want_client_flags |= lib.PKGCONF_PKG_PKGF_DONT_RELOCATE_PATHS
@@ -447,43 +487,43 @@
     if Flags.SILENCE_ERRORS in want_flags:
         set_stream_handler(None)
     elif Flags.ERRORS_ON_STDOUT in want_flags:
         set_stream_handler(sys.stdout)
     else:
         set_stream_handler(sys.stderr)
 
-    if Flags.IGNORE_CONFLICTS in want_flags or os.environ.get('PKG_CONFIG_IGNORE_CONFLICTS'):
+    if Flags.IGNORE_CONFLICTS in want_flags or env.get('PKG_CONFIG_IGNORE_CONFLICTS'):
         want_client_flags |= lib.PKGCONF_PKG_PKGF_SKIP_CONFLICTS
     
     if Flags.STATIC in want_flags or personality.want_default_static:
         want_client_flags |= lib.PKGCONF_PKG_PKGF_SEARCH_PRIVATE | lib.PKGCONF_PKG_PKGF_MERGE_PRIVATE_FRAGMENTS
     
     if Flags.SHARED in want_flags:
         want_client_flags &= ~(lib.PKGCONF_PKG_PKGF_SEARCH_PRIVATE | lib.PKGCONF_PKG_PKGF_MERGE_PRIVATE_FRAGMENTS)
 
-    if Flags.PURE in want_flags or os.environ.get('PKG_CONFIG_PURE_DEPGRAPH') is not None or personality.want_default_pure:
+    if Flags.PURE in want_flags or env.get('PKG_CONFIG_PURE_DEPGRAPH') is not None or personality.want_default_pure:
         want_client_flags &= ~lib.PKGCONF_PKG_PKGF_MERGE_PRIVATE_FRAGMENTS
     
     if Flags.ENV_ONLY in want_flags:
         want_client_flags |= lib.PKGCONF_PKG_PKGF_ENV_ONLY
     
     if Flags.NO_CACHE in want_flags:
         want_client_flags |= lib.PKGCONF_PKG_PKGF_NO_CACHE
     
     # FIXME: only win32?
     if sys.platform in {'win32', 'cygwin', 'msys'} or Flags.DEFINE_PREFIX in want_flags:
         want_client_flags |= lib.PKGCONF_PKG_PKGF_REDEFINE_PREFIX
     
-    if Flags.NO_UNINSTALLED in want_flags or os.environ.get('PKG_CONFIG_DISABLE_UNINSTALLED') is not None:
+    if Flags.NO_UNINSTALLED in want_flags or env.get('PKG_CONFIG_DISABLE_UNINSTALLED') is not None:
         want_client_flags |= lib.PKGCONF_PKG_PKGF_NO_UNINSTALLED
     
     if Flags.NO_PROVIDES in want_flags:
         want_client_flags |= lib.PKGCONF_PKG_PKGF_SKIP_PROVIDES
     
-    if Flags.DONT_DEFINE_PREFIX in want_flags or os.environ.get('PKG_CONFIG_DONT_DEFINE_PREFIX') is not None:
+    if Flags.DONT_DEFINE_PREFIX in want_flags or env.get('PKG_CONFIG_DONT_DEFINE_PREFIX') is not None:
         want_client_flags &= ~lib.PKGCONF_PKG_PKGF_REDEFINE_PREFIX
 
     if Flags.INTERNAL_CFLAGS in want_flags:
         want_client_flags |= lib.PKGCONF_PKG_PKGF_DONT_FILTER_INTERNAL_CFLAGS
     
     if (Flags.REQUIRES in want_flags
             or Flags.REQUIRES_PRIVATE in want_flags
@@ -491,32 +531,32 @@
             or Flags.VARIABLES in want_flags
             or Flags.MODVERSION in want_flags
             or Flags.PATH in want_flags
             or want_variable):
         maximum_package_count = 1
         maximum_traverse_depth = 1
     
-    if os.environ.get('PKG_CONFIG_ALLOW_SYSTEM_CFLAGS') is not None:
+    if env.get('PKG_CONFIG_ALLOW_SYSTEM_CFLAGS') is not None:
         want_flags |= Flags.KEEP_SYSTEM_CFLAGS
     
-    if os.environ.get('PKG_CONFIG_ALLOW_SYSTEM_LIBS') is not None:
+    if env.get('PKG_CONFIG_ALLOW_SYSTEM_LIBS') is not None:
         want_flags |= Flags.KEEP_SYSTEM_LIBS
     
-    builddir = os.environ.get('PKG_CONFIG_TOP_BUILD_DIR')
+    builddir = env.get('PKG_CONFIG_TOP_BUILD_DIR')
     if builddir is not None:
         lib.pkgconf_client_set_buildroot_dir(pkg_client, builddir.encode())
     
     if Flags.REQUIRES_PRIVATE in want_flags or want_flags & Flags.CFLAGS:
         want_client_flags |= lib.PKGCONF_PKG_PKGF_SEARCH_PRIVATE
     
-    sysroot_dir = os.environ.get('PKG_CONFIG_SYSROOT_DIR')
+    sysroot_dir = env.get('PKG_CONFIG_SYSROOT_DIR')
     if sysroot_dir is not None:
         lib.pkgconf_client_set_sysroot_dir(pkg_client, sysroot_dir.encode())
 
-        destdir = os.environ.get('DESTDIR')
+        destdir = env.get('DESTDIR')
         if destdir == sysroot_dir:
             want_client_flags |= lib.PKGCONF_PKG_PKGF_FDO_SYSROOT_RULES
     
     lib.pkgconf_client_set_flags(pkg_client, want_client_flags)
     lib.pkgconf_client_dir_list_build(pkg_client, personality)
 
     if required_pkgconfig_version is not None:
@@ -678,14 +718,14 @@
         data_handle = ffi.new_handle(data)
         result.extend(apply_libs(pkg_client, world, 2, data_handle))
     
     cleanup()
     return result
         
 
-def query_args(command: str) -> T.List[str]:
+def query_args(command: str, env: T.Optional[T.Dict[str, str]] = None) -> T.List[str]:
     try:
         options = parse_args(command)
-        return query(**vars(options))
+        return query(env=env, **vars(options))
     
     except SystemExit:
         raise PkgConfError()
```

### Comparing `pypkgconf-0.1.0/pypkgconf/constants.py` & `pypkgconf-0.1.1/pypkgconf/constants.py`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/pypkgconf/logger.py` & `pypkgconf-0.1.1/pypkgconf/logger.py`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/pypkgconf/meson.build` & `pypkgconf-0.1.1/pypkgconf/meson.build`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/pyproject.toml` & `pypkgconf-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/.github/workflows/test.yml` & `pypkgconf-0.1.1/subprojects/pkgconf/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/.woodpecker.yml` & `pypkgconf-0.1.1/subprojects/pkgconf/.woodpecker.yml`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/AUTHORS` & `pypkgconf-0.1.1/subprojects/pkgconf/AUTHORS`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/CODE_OF_CONDUCT.md` & `pypkgconf-0.1.1/subprojects/pkgconf/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/COPYING` & `pypkgconf-0.1.1/subprojects/pkgconf/COPYING`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/Makefile.am` & `pypkgconf-0.1.1/subprojects/pkgconf/Makefile.am`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/Makefile.lite` & `pypkgconf-0.1.1/subprojects/pkgconf/Makefile.lite`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/NEWS` & `pypkgconf-0.1.1/subprojects/pkgconf/NEWS`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/README.md` & `pypkgconf-0.1.1/subprojects/pkgconf/README.md`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/autogen.sh` & `pypkgconf-0.1.1/subprojects/pkgconf/autogen.sh`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/cli/bomtool/main.c` & `pypkgconf-0.1.1/subprojects/pkgconf/cli/bomtool/main.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/cli/getopt_long.c` & `pypkgconf-0.1.1/subprojects/pkgconf/cli/getopt_long.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/cli/getopt_long.h` & `pypkgconf-0.1.1/subprojects/pkgconf/cli/getopt_long.h`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/cli/main.c` & `pypkgconf-0.1.1/subprojects/pkgconf/cli/main.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/cli/renderer-msvc.c` & `pypkgconf-0.1.1/subprojects/pkgconf/cli/renderer-msvc.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/cli/renderer-msvc.h` & `pypkgconf-0.1.1/subprojects/pkgconf/cli/renderer-msvc.h`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/configure.ac` & `pypkgconf-0.1.1/subprojects/pkgconf/configure.ac`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/conf.py` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/extract.py` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/extract.py`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-argvsplit.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-audit.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-audit.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-cache.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-cache.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-client.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-client.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-dependency.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-dependency.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-fragment.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-fragment.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-path.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-path.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-personality.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-personality.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-pkg.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-pkg.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-queue.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-queue.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/doc/libpkgconf-tuple.rst` & `pypkgconf-0.1.1/subprojects/pkgconf/doc/libpkgconf-tuple.rst`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/argvsplit.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/argvsplit.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/audit.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/audit.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/bsdstubs.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/bsdstubs.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/bsdstubs.h` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/bsdstubs.h`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/cache.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/cache.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/client.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/client.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/config.h.meson` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/config.h.meson`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/dependency.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/dependency.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/fileio.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/fileio.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/fragment.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/fragment.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/iter.h` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/iter.h`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/libpkgconf-api.h` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/libpkgconf-api.h`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/libpkgconf.h` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/libpkgconf.h`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/parser.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/parser.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/path.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/path.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/personality.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/personality.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/pkg.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/pkg.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/queue.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/queue.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/stdinc.h` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/stdinc.h`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/tuple.c` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/tuple.c`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/libpkgconf/win-dirent.h` & `pypkgconf-0.1.1/subprojects/pkgconf/libpkgconf/win-dirent.h`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/m4/ax_check_compile_flag.m4` & `pypkgconf-0.1.1/subprojects/pkgconf/m4/ax_check_compile_flag.m4`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/man/pc.5` & `pypkgconf-0.1.1/subprojects/pkgconf/man/pc.5`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/man/pkg.m4.7` & `pypkgconf-0.1.1/subprojects/pkgconf/man/pkg.m4.7`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/man/pkgconf-personality.5` & `pypkgconf-0.1.1/subprojects/pkgconf/man/pkgconf-personality.5`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/man/pkgconf.1` & `pypkgconf-0.1.1/subprojects/pkgconf/man/pkgconf.1`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/meson.build` & `pypkgconf-0.1.1/subprojects/pkgconf/meson.build`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/pkg.m4` & `pypkgconf-0.1.1/subprojects/pkgconf/pkg.m4`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/tests/basic.sh` & `pypkgconf-0.1.1/subprojects/pkgconf/tests/basic.sh`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/tests/builtins.sh` & `pypkgconf-0.1.1/subprojects/pkgconf/tests/builtins.sh`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/tests/lib1/billion-laughs.pc` & `pypkgconf-0.1.1/subprojects/pkgconf/tests/lib1/billion-laughs.pc`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/tests/parser.sh` & `pypkgconf-0.1.1/subprojects/pkgconf/tests/parser.sh`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/tests/provides.sh` & `pypkgconf-0.1.1/subprojects/pkgconf/tests/provides.sh`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/tests/regress.sh` & `pypkgconf-0.1.1/subprojects/pkgconf/tests/regress.sh`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/tests/requires.sh` & `pypkgconf-0.1.1/subprojects/pkgconf/tests/requires.sh`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/tests/sysroot.sh` & `pypkgconf-0.1.1/subprojects/pkgconf/tests/sysroot.sh`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/tests/test_env.sh.in` & `pypkgconf-0.1.1/subprojects/pkgconf/tests/test_env.sh.in`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/subprojects/pkgconf/tests/version.sh` & `pypkgconf-0.1.1/subprojects/pkgconf/tests/version.sh`

 * *Files identical despite different names*

### Comparing `pypkgconf-0.1.0/tests/test_basic.py` & `pypkgconf-0.1.1/tests/test_basic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,262 +1,254 @@
 import pypkgconf
 
 import pytest
 
 import shutil
 
 
-with_lib1 = pytest.mark.usefixtures('lib1_pkg_config_path')
-with_lib1lib2 = pytest.mark.usefixtures('lib1lib2_pkg_config_path')
-
-
-@with_lib1
-def test_noargs():
+def test_noargs(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('')
+        pypkgconf.query_args("", env=lib1_env)
 
 
-@with_lib1
-def test_libs():
-    result = pypkgconf.query_args('--libs foo')
+def test_libs(lib1_env):
+    result = pypkgconf.query_args("--libs foo", env=lib1_env)
 
-    assert result == ['-L/test/lib', '-lfoo']
+    assert result == ["-L/test/lib", "-lfoo"]
 
 
-@with_lib1
-def test_libs_cflags():
-    result = pypkgconf.query_args('--cflags --libs foo')
+def test_libs_cflags(lib1_env):
+    result = pypkgconf.query_args("--cflags --libs foo", env=lib1_env)
 
-    assert result == ['-fPIC', '-I/test/include/foo', '-L/test/lib', '-lfoo']
+    assert result == ["-fPIC", "-I/test/include/foo", "-L/test/lib", "-lfoo"]
 
 
-@with_lib1
-def test_libs_cflags_version():
-    result = pypkgconf.query_args('--cflags --libs "foo > 1.2"')
+def test_libs_cflags_version(lib1_env):
+    result = pypkgconf.query_args('--cflags --libs "foo > 1.2"', env=lib1_env)
 
-    assert result == ['-fPIC', '-I/test/include/foo', '-L/test/lib', '-lfoo']
+    assert result == ["-fPIC", "-I/test/include/foo", "-L/test/lib", "-lfoo"]
 
 
-@with_lib1
-def test_libs_cflags_version_multiple():
-    result = pypkgconf.query_args('--cflags --libs "foo > 1.2 bar >= 1.3"')
+def test_libs_cflags_version_multiple(lib1_env):
+    result = pypkgconf.query_args(
+        '--cflags --libs "foo > 1.2 bar >= 1.3"', env=lib1_env
+    )
 
-    assert result == ['-fPIC', '-I/test/include/foo', '-L/test/lib', '-lbar', '-lfoo']
+    assert result == ["-fPIC", "-I/test/include/foo", "-L/test/lib", "-lbar", "-lfoo"]
 
 
-@with_lib1
-def test_libs_cflags_version_multiple_coma():
-    result = pypkgconf.query_args('--cflags --libs "foo > 1.2,bar >= 1.3"')
+def test_libs_cflags_version_multiple_coma(lib1_env):
+    result = pypkgconf.query_args(
+        '--cflags --libs "foo > 1.2,bar >= 1.3"', env=lib1_env
+    )
 
-    assert result == ['-fPIC', '-I/test/include/foo', '-L/test/lib', '-lbar', '-lfoo']
+    assert result == ["-fPIC", "-I/test/include/foo", "-L/test/lib", "-lbar", "-lfoo"]
 
 
-@with_lib1
-def test_libs_cflags_version_alt():
-    result = pypkgconf.query_args('--cflags --libs "foo" ">" "1.2"')
+def test_libs_cflags_version_alt(lib1_env):
+    result = pypkgconf.query_args('--cflags --libs "foo" ">" "1.2"', env=lib1_env)
 
-    assert result == ['-fPIC', '-I/test/include/foo', '-L/test/lib', '-lfoo']
+    assert result == ["-fPIC", "-I/test/include/foo", "-L/test/lib", "-lfoo"]
 
 
-@with_lib1
-def test_libs_cflags_version_different():
-    result = pypkgconf.query_args('--cflags --libs "foo" "!=" "1.3.0"')
+def test_libs_cflags_version_different(lib1_env):
+    result = pypkgconf.query_args('--cflags --libs "foo" "!=" "1.3.0"', env=lib1_env)
 
-    assert result == ['-fPIC', '-I/test/include/foo', '-L/test/lib', '-lfoo']
+    assert result == ["-fPIC", "-I/test/include/foo", "-L/test/lib", "-lfoo"]
 
 
-@with_lib1
-def test_libs_cflags_version_different_bad(caplog):
+def test_libs_cflags_version_different_bad(caplog, lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--cflags --libs "foo" "!=" "1.2.3"')
+        pypkgconf.query_args('--cflags --libs "foo" "!=" "1.2.3"', env=lib1_env)
 
-    assert "Package dependency requirement 'foo != 1.2.3' could not be satisfied.\n" in caplog.text
-    assert "Package 'foo' has version '1.2.3', required version is '!= 1.2.3'\n" in caplog.text
+    assert (
+        "Package dependency requirement 'foo != 1.2.3' could not be satisfied.\n"
+        in caplog.text
+    )
+    assert (
+        "Package 'foo' has version '1.2.3', required version is '!= 1.2.3'\n"
+        in caplog.text
+    )
 
 
-@with_lib1
-def test_exists_nonexitent():
+def test_exists_nonexitent(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--exists nonexistant')
+        pypkgconf.query_args("--exists nonexistant", env=lib1_env)
 
 
-@with_lib1
-def test_nonexitent():
+def test_nonexitent(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('nonexistant')
+        pypkgconf.query_args("nonexistant", env=lib1_env)
 
 
-@with_lib1
-def test_exists_version():
-    assert pypkgconf.query_args('--exists "foo > 1.2"') == []
+def test_exists_version(lib1_env):
+    assert pypkgconf.query_args('--exists "foo > 1.2"', env=lib1_env) == []
 
 
-@with_lib1
-def test_exists_version_bad():
+def test_exists_version_bad(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--exists "foo > 1.2.3"')
+        pypkgconf.query_args('--exists "foo > 1.2.3"', env=lib1_env)
 
 
-@with_lib1
-def test_exists_version_bad():
-    assert pypkgconf.query_args('--exists "foo" ">" "1.2"') == []
+def test_exists_version_bad(lib1_env):
+    assert pypkgconf.query_args('--exists "foo" ">" "1.2"', env=lib1_env) == []
 
 
-@with_lib1
-def test_uninstalled_bad():
+def test_uninstalled_bad(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--uninstalled "foo"')
+        pypkgconf.query_args('--uninstalled "foo"', env=lib1_env)
 
 
-@with_lib1
-def test_uninstalled():
-    assert pypkgconf.query_args('--uninstalled "omg"') == []
+def test_uninstalled(lib1_env):
+    assert pypkgconf.query_args('--uninstalled "omg"', env=lib1_env) == []
 
 
-@with_lib1
-def test_exists_version_bad2():
+def test_exists_version_bad2(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--exists "foo >= "')
+        pypkgconf.query_args('--exists "foo >= "', env=lib1_env)
 
 
-@with_lib1
-def test_exists_version_bad3():
+def test_exists_version_bad3(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--exists "tilde >= 1.0.0"')
-
-
-@with_lib1
-def test_exists():
-    assert pypkgconf.query_args('--exists "tilde = 1.0.0~rc1"') == []
+        pypkgconf.query_args('--exists "tilde >= 1.0.0"', env=lib1_env)
 
 
-@with_lib1
-def test_exists2():
-    assert pypkgconf.query_args('--exists "tilde <= 1.0.0"') == []
+def test_exists(lib1_env):
+    assert pypkgconf.query_args('--exists "tilde = 1.0.0~rc1"', env=lib1_env) == []
 
 
-@with_lib1
-def test_exists3():
-    assert pypkgconf.query_args('--exists "" "foo"') == []
+def test_exists2(lib1_env):
+    assert pypkgconf.query_args('--exists "tilde <= 1.0.0"', env=lib1_env) == []
 
 
+def test_exists3(lib1_env):
+    assert pypkgconf.query_args('--exists "" "foo"', env=lib1_env) == []
 
-@with_lib1
-def test_libs_intermediary():
-    result = pypkgconf.query_args('--libs intermediary-1 intermediary-2')
 
-    assert result == ['-lintermediary-1', '-lintermediary-2', '-lfoo', '-lbar', '-lbaz']
+def test_libs_intermediary(lib1_env):
+    result = pypkgconf.query_args("--libs intermediary-1 intermediary-2", env=lib1_env)
 
+    assert result == ["-lintermediary-1", "-lintermediary-2", "-lfoo", "-lbar", "-lbaz"]
 
-@with_lib1
-def test_libs_circular2(caplog):
-    assert pypkgconf.query_args('circular-2 --validate') == []
-    assert 'circular-1: breaking circular reference (circular-1 -> circular-2 -> circular-1)\n' in caplog.text
 
+def test_libs_circular2(caplog, lib1_env):
+    assert pypkgconf.query_args("circular-2 --validate", env=lib1_env) == []
+    assert (
+        "circular-1: breaking circular reference (circular-1 -> circular-2 -> circular-1)\n"
+        in caplog.text
+    )
 
-@with_lib1
-def test_libs_circular1(caplog):
-    assert pypkgconf.query_args('circular-1 --validate') == []
-    assert 'circular-3: breaking circular reference (circular-3 -> circular-1 -> circular-3)\n' in caplog.text
 
+def test_libs_circular1(caplog, lib1_env):
+    assert pypkgconf.query_args("circular-1 --validate", env=lib1_env) == []
+    assert (
+        "circular-3: breaking circular reference (circular-3 -> circular-1 -> circular-3)\n"
+        in caplog.text
+    )
 
 
-@with_lib1
-def test_libs_circular_directpc(testsdir):
-    result = pypkgconf.query_args(f'--libs {testsdir.as_posix()}/lib1/circular-3.pc')
+def test_libs_circular_directpc(testsdir, lib1_env):
+    result = pypkgconf.query_args(
+        f"--libs {testsdir.as_posix()}/lib1/circular-3.pc", env=lib1_env
+    )
 
-    assert result == ['-lcircular-2', '-lcircular-3', '-lcircular-1']
+    assert result == ["-lcircular-2", "-lcircular-3", "-lcircular-1"]
 
 
-# 
-@with_lib1
-def test_libs_static():
-    result = pypkgconf.query_args('--libs static-archive-libs')
+def test_libs_static(lib1_env):
+    result = pypkgconf.query_args("--libs static-archive-libs", env=lib1_env)
 
-    assert result == ['/libfoo.a', '-pthread']
+    assert result == ["/libfoo.a", "-pthread"]
 
 
-@with_lib1
-def test_libs_static_ordering():
-    result = pypkgconf.query_args('--libs foo bar')
+def test_libs_static_ordering(lib1_env):
+    result = pypkgconf.query_args("--libs foo bar", env=lib1_env)
 
-    assert result == ['-L/test/lib', '-lbar', '-lfoo']
+    assert result == ["-L/test/lib", "-lbar", "-lfoo"]
 
 
+def test_pkg_config_path(lib1_lib2_env):
+    result = pypkgconf.query_args("--libs foo", env=lib1_lib2_env)
 
-@with_lib1lib2
-def test_pkg_config_path():
-    result = pypkgconf.query_args('--libs foo')
+    assert result == ["-L/test/lib", "-lfoo"]
 
-    assert result == ['-L/test/lib', '-lfoo']
-
-    result = pypkgconf.query_args('--libs bar')
-
-    assert result == ['-L/test/lib', '-lbar', '-lfoo']
+    result = pypkgconf.query_args("--libs bar", env=lib1_lib2_env)
 
+    assert result == ["-L/test/lib", "-lbar", "-lfoo"]
 
 
 def test_with_path(testsdir):
-    lib1_path = testsdir / 'lib1'
-    lib2_path = testsdir / 'lib2'
+    lib1_path = testsdir / "lib1"
+    lib2_path = testsdir / "lib2"
 
-    result = pypkgconf.query_args(f'--with-path={lib1_path.as_posix()} --with-path={lib2_path.as_posix()} --libs foo')
+    result = pypkgconf.query_args(
+        f"--with-path={lib1_path.as_posix()} --with-path={lib2_path.as_posix()} --libs foo"
+    )
 
-    assert result == ['-L/test/lib', '-lfoo']
+    assert result == ["-L/test/lib", "-lfoo"]
 
-    result = pypkgconf.query_args(f'--with-path={lib1_path.as_posix()} --with-path={lib2_path.as_posix()} --libs bar')
+    result = pypkgconf.query_args(
+        f"--with-path={lib1_path.as_posix()} --with-path={lib2_path.as_posix()} --libs bar"
+    )
 
-    assert result == ['-L/test/lib', '-lbar', '-lfoo']
+    assert result == ["-L/test/lib", "-lbar", "-lfoo"]
 
 
-@with_lib1
-def test_nolibs():
-    assert pypkgconf.query_args('--libs nolib') == []
+def test_nolibs(lib1_env):
+    assert pypkgconf.query_args("--libs nolib", env=lib1_env) == []
 
 
-@with_lib1
-def test_nocflags():
-    assert pypkgconf.query_args('--cflags nocflag') == []
+def test_nocflags(lib1_env):
+    assert pypkgconf.query_args("--cflags nocflag", env=lib1_env) == []
 
 
 def test_arbitary_path(testsdir, tmp_path, monkeypatch):
-    shutil.copy(testsdir / 'lib1' / 'foo.pc', tmp_path)
+    shutil.copy(testsdir / "lib1" / "foo.pc", tmp_path)
     monkeypatch.chdir(tmp_path)
 
-    result = pypkgconf.query_args('--libs foo.pc')
+    result = pypkgconf.query_args("--libs foo.pc")
 
-    assert result == ['-L/test/lib', '-lfoo']
+    assert result == ["-L/test/lib", "-lfoo"]
 
 
 def test_relocatable(testsdir):
-    basedir = pypkgconf.query_args(f'--relocate {testsdir.as_posix()}')[0]
+    basedir = pypkgconf.query_args(f"--relocate {testsdir.as_posix()}")[0]
 
-    result = pypkgconf.query_args(f'--define-prefix --variable=prefix {basedir}/lib-relocatable/lib/pkgconfig/foo.pc')
+    result = pypkgconf.query_args(
+        f"--define-prefix --variable=prefix {basedir}/lib-relocatable/lib/pkgconfig/foo.pc"
+    )
 
-    assert result == [f'{basedir}/lib-relocatable']
+    assert result == [f"{basedir}/lib-relocatable"]
 
 
-def test_single_depth_selectors(monkeypatch, testsdir):
-    monkeypatch.setenv('PKG_CONFIG_MAXIMUM_TRAVERSE_DEPTH', '1')
+def test_single_depth_selectors(testsdir):
+    env = {"PKG_CONFIG_MAXIMUM_TRAVERSE_DEPTH": "1"}
 
-    result = pypkgconf.query_args(f'--with-path={testsdir.as_posix()}/lib3 --print-requires bar')
+    result = pypkgconf.query_args(
+        f"--with-path={testsdir.as_posix()}/lib3 --print-requires bar", env=env
+    )
 
-    assert result == ['foo']
+    assert result == ["foo"]
 
 
 def test_license_isc(testsdir):
-    result = pypkgconf.query_args(f'--with-path={testsdir.as_posix()}/lib1 --license foo')
-
-    assert result == ['foo: ISC']
+    result = pypkgconf.query_args(
+        f"--with-path={testsdir.as_posix()}/lib1 --license foo"
+    )
 
+    assert result == ["foo: ISC"]
 
 
 def test_license_noassertion(testsdir):
-    result = pypkgconf.query_args(f'--with-path={testsdir.as_posix()}/lib1 --license bar')
+    result = pypkgconf.query_args(
+        f"--with-path={testsdir.as_posix()}/lib1 --license bar"
+    )
 
-    assert result == ['bar: NOASSERTION', 'foo: ISC']
+    assert result == ["bar: NOASSERTION", "foo: ISC"]
 
 
 def test_modversion_noflatten(testsdir):
-    result = pypkgconf.query_args(f'--with-path={testsdir.as_posix()}/lib1 --modversion bar')
-    
-    assert result == ['1.3']
+    result = pypkgconf.query_args(
+        f"--with-path={testsdir.as_posix()}/lib1 --modversion bar"
+    )
+
+    assert result == ["1.3"]
```

### Comparing `pypkgconf-0.1.0/tests/test_parser.py` & `pypkgconf-0.1.1/tests/test_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,262 +1,263 @@
 import pypkgconf
 
 import pytest
 
 import logging
 
 
-with_lib1 = pytest.mark.usefixtures('lib1_pkg_config_path')
+def test_comments(lib1_env):
+    result = pypkgconf.query_args("--libs comments", env=lib1_env)
 
+    assert result == ["-lfoo"]
 
-@with_lib1
-def test_comments():
-    result = pypkgconf.query_args('--libs comments')
 
-    assert result == ['-lfoo']
+def test_comments_in_fields(lib1_env):
+    result = pypkgconf.query_args("--libs comments-in-fields", env=lib1_env)
 
+    assert result == ["-lfoo"]
 
-@with_lib1
-def test_comments_in_fields():
-    result = pypkgconf.query_args('--libs comments-in-fields')
 
-    assert result == ['-lfoo']
+def test_dos(lib1_env):
+    result = pypkgconf.query_args("--libs dos-lineendings", env=lib1_env)
 
+    assert result == ["-L/test/lib/dos-lineendings", "-ldos-lineendings"]
 
-@with_lib1
-def test_dos():
-    result = pypkgconf.query_args('--libs dos-lineendings')
 
-    assert result == ['-L/test/lib/dos-lineendings' ,'-ldos-lineendings']
+def test_no_trailing_newline(lib1_env):
+    result = pypkgconf.query_args("--cflags no-trailing-newline", env=lib1_env)
 
+    assert result == ["-I/test/include/no-trailing-newline"]
 
-@with_lib1
-def test_no_trailing_newline():
-    result = pypkgconf.query_args('--cflags no-trailing-newline')
 
-    assert result == ['-I/test/include/no-trailing-newline']
+def test_parse(lib1_env):
+    result = pypkgconf.query_args("--libs argv-parse", env=lib1_env)
 
+    assert result == ["-llib-3", "-llib-1", "-llib-2", "-lpthread"]
 
-@with_lib1
-def test_parse():
-    result = pypkgconf.query_args('--libs argv-parse')
 
-    assert result == ['-llib-3', '-llib-1', '-llib-2', '-lpthread']
-
-
-@with_lib1
-def test_bad_option():
+def test_bad_option(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--exists -foo')
+        pypkgconf.query_args("--exists -foo", env=lib1_env)
 
 
-@with_lib1
-def test_argv_parse_3():
-    result = pypkgconf.query_args('--libs argv-parse-3')
+def test_argv_parse_3(lib1_env):
+    result = pypkgconf.query_args("--libs argv-parse-3", env=lib1_env)
 
-    assert result == ['-llib-1', '-pthread', '/test/lib/lib2.so']
+    assert result == ["-llib-1", "-pthread", "/test/lib/lib2.so"]
 
 
-@with_lib1
-def test_quoting():
-    result = pypkgconf.query_args('--libs tilde-quoting')
-    assert result == ['-L~', '-ltilde']
+def test_quoting(lib1_env):
+    result = pypkgconf.query_args("--libs tilde-quoting", env=lib1_env)
+    assert result == ["-L~", "-ltilde"]
 
-    result = pypkgconf.query_args('--cflags tilde-quoting')
-    assert result == ['-I~']
+    result = pypkgconf.query_args("--cflags tilde-quoting", env=lib1_env)
+    assert result == ["-I~"]
 
 
-@with_lib1
-def test_paren_quoting():
-    result = pypkgconf.query_args('--libs paren-quoting')
+def test_paren_quoting(lib1_env):
+    result = pypkgconf.query_args("--libs paren-quoting", env=lib1_env)
 
     # FIXME: escape $?
-    assert result == ['-L$(libdir)', '-ltilde']
+    assert result == ["-L$(libdir)", "-ltilde"]
 
 
-@with_lib1
-def test_multiline_field():
-    result = pypkgconf.query_args('--list-all')
+def test_multiline_field(lib1_env):
+    result = pypkgconf.query_args("--list-all", env=lib1_env)
 
-    assert 'multiline description' in '\n'.join(result)
+    assert "multiline description" in "\n".join(result)
 
 
-@with_lib1
-def test_multiline_bogus_header():
-    assert pypkgconf.query_args('--exists multiline-bogus') == []
+def test_multiline_bogus_header(lib1_env):
+    assert pypkgconf.query_args("--exists multiline-bogus", env=lib1_env) == []
 
 
 def test_escaped_backslash(testsdir):
-    selfdir = (testsdir / 'lib1').as_posix()
-    result = pypkgconf.query_args(f'--with-path={selfdir} --cflags escaped-backslash')
-
-    assert result == ['-IC:\\\\A']
-
+    selfdir = (testsdir / "lib1").as_posix()
+    result = pypkgconf.query_args(f"--with-path={selfdir} --cflags escaped-backslash")
 
-@with_lib1
-def test_quoted():
-    result = pypkgconf.query_args('--cflags quotes')
+    assert result == ["-IC:\\\\A"]
 
-    #FIXME: is it ok?
-    assert result == ['-DQUOTED=\\"bla\\"', '-DA=\\"escaped\\ string\\\'\\ literal\\"', '-DB=\\\\1$', '-DC=bla']
 
+def test_quoted(lib1_env):
+    result = pypkgconf.query_args("--cflags quotes", env=lib1_env)
 
-@with_lib1
-def test_flag_order_1():
-    result = pypkgconf.query_args('--libs flag-order-1')
+    # FIXME: is it ok?
+    assert result == [
+        '-DQUOTED=\\"bla\\"',
+        '-DA=\\"escaped\\ string\\\'\\ literal\\"',
+        "-DB=\\\\1$",
+        "-DC=bla",
+    ]
 
-    assert result == ['-L/test/lib', '-Bdynamic', '-lfoo', '-Bstatic', '-lbar']
 
+def test_flag_order_1(lib1_env):
+    result = pypkgconf.query_args("--libs flag-order-1", env=lib1_env)
 
+    assert result == ["-L/test/lib", "-Bdynamic", "-lfoo", "-Bstatic", "-lbar"]
 
-@with_lib1
-def test_flag_order_2():
-    result = pypkgconf.query_args('--libs flag-order-1 foo')
 
-    assert result == ['-L/test/lib', '-Bdynamic', '-lfoo', '-Bstatic', '-lbar', '-lfoo']
+def test_flag_order_2(lib1_env):
+    result = pypkgconf.query_args("--libs flag-order-1 foo", env=lib1_env)
 
+    assert result == ["-L/test/lib", "-Bdynamic", "-lfoo", "-Bstatic", "-lbar", "-lfoo"]
 
-@with_lib1
-def test_flag_order_3():
-    result = pypkgconf.query_args('--libs flag-order-3')
 
-    assert result == ['-L/test/lib', '-Wl,--start-group', '-lfoo', '-lbar', '-Wl,--end-group']
+def test_flag_order_3(lib1_env):
+    result = pypkgconf.query_args("--libs flag-order-3", env=lib1_env)
 
+    assert result == [
+        "-L/test/lib",
+        "-Wl,--start-group",
+        "-lfoo",
+        "-lbar",
+        "-Wl,--end-group",
+    ]
 
 
-@with_lib1
-def test_flag_order_4():
-    result = pypkgconf.query_args('--libs flag-order-3 foo')
+def test_flag_order_4(lib1_env):
+    result = pypkgconf.query_args("--libs flag-order-3 foo", env=lib1_env)
 
-    assert result == ['-L/test/lib', '-Wl,--start-group', '-lfoo', '-lbar', '-Wl,--end-group', '-lfoo']
+    assert result == [
+        "-L/test/lib",
+        "-Wl,--start-group",
+        "-lfoo",
+        "-lbar",
+        "-Wl,--end-group",
+        "-lfoo",
+    ]
 
 
-@with_lib1
-def test_variable_whitespace():
-    result = pypkgconf.query_args('--cflags variable-whitespace')
+def test_variable_whitespace(lib1_env):
+    result = pypkgconf.query_args("--cflags variable-whitespace", env=lib1_env)
 
-    assert result == ['-I/test/include']
+    assert result == ["-I/test/include"]
 
 
-@with_lib1
-def test_fragment_quoting():
-    result = pypkgconf.query_args('--cflags fragment-quoting')
+def test_fragment_quoting(lib1_env):
+    result = pypkgconf.query_args("--cflags fragment-quoting", env=lib1_env)
 
-    assert result == ['-fPIC', '-I/test/include/foo', '-DQUOTED=\\\"/test/share/doc\\\"']
+    assert result == ["-fPIC", "-I/test/include/foo", '-DQUOTED=\\"/test/share/doc\\"']
 
 
-@with_lib1
-def test_fragment_quoting_2():
-    result = pypkgconf.query_args('--cflags fragment-quoting-2')
+def test_fragment_quoting_2(lib1_env):
+    result = pypkgconf.query_args("--cflags fragment-quoting-2", env=lib1_env)
 
-    assert result == ['-fPIC', '-I/test/include/foo', '-DQUOTED=/test/share/doc']
+    assert result == ["-fPIC", "-I/test/include/foo", "-DQUOTED=/test/share/doc"]
 
 
-@with_lib1
-def test_fragment_quoting_3():
-    result = pypkgconf.query_args('--cflags fragment-quoting-3')
+def test_fragment_quoting_3(lib1_env):
+    result = pypkgconf.query_args("--cflags fragment-quoting-3", env=lib1_env)
 
-    assert result == ['-fPIC', '-I/test/include/foo', '-DQUOTED=\\\"/test/share/doc\\\"']
+    assert result == ["-fPIC", "-I/test/include/foo", '-DQUOTED=\\"/test/share/doc\\"']
 
 
-@with_lib1
-def test_fragment_quoting_5():
-    result = pypkgconf.query_args('--cflags fragment-quoting-5')
+def test_fragment_quoting_5(lib1_env):
+    result = pypkgconf.query_args("--cflags fragment-quoting-5", env=lib1_env)
 
-    assert result == ['-fPIC', '-I/test/include/foo', '-DQUOTED=/test/share/doc']
+    assert result == ["-fPIC", "-I/test/include/foo", "-DQUOTED=/test/share/doc"]
 
 
-@with_lib1
-def test_fragment_quoting_7():
-    result = pypkgconf.query_args('--cflags fragment-quoting-7')
+def test_fragment_quoting_7(lib1_env):
+    result = pypkgconf.query_args("--cflags fragment-quoting-7", env=lib1_env)
 
-    assert result == ['-Dhello=10', '-Dworld=+32', '-DDEFINED_FROM_PKG_CONFIG=hello\\ world']
+    assert result == [
+        "-Dhello=10",
+        "-Dworld=+32",
+        "-DDEFINED_FROM_PKG_CONFIG=hello\\ world",
+    ]
 
 
 def test_fragment_escaping_1(testsdir):
-    selfdir = (testsdir / 'lib1').as_posix()
-    result = pypkgconf.query_args(f'--with-path={selfdir} --cflags fragment-escaping-1')
+    selfdir = (testsdir / "lib1").as_posix()
+    result = pypkgconf.query_args(f"--with-path={selfdir} --cflags fragment-escaping-1")
 
-    assert result == ['-IC:\\\\D\\ E']
+    assert result == ["-IC:\\\\D\\ E"]
 
 
 def test_fragment_escaping_2(testsdir):
-    selfdir = (testsdir / 'lib1').as_posix()
-    result = pypkgconf.query_args(f'--with-path={selfdir} --cflags fragment-escaping-2')
+    selfdir = (testsdir / "lib1").as_posix()
+    result = pypkgconf.query_args(f"--with-path={selfdir} --cflags fragment-escaping-2")
 
-    assert result == ['-IC:\\\\D\\ E']
+    assert result == ["-IC:\\\\D\\ E"]
 
 
 def test_fragment_escaping_3(testsdir):
-    selfdir = (testsdir / 'lib1').as_posix()
-    result = pypkgconf.query_args(f'--with-path={selfdir} --cflags fragment-escaping-3')
+    selfdir = (testsdir / "lib1").as_posix()
+    result = pypkgconf.query_args(f"--with-path={selfdir} --cflags fragment-escaping-3")
 
-    assert result == ['-IC:\\\\D\\ E']
+    assert result == ["-IC:\\\\D\\ E"]
 
 
 # FIXME: how to test macro arithmetics in Python...
 # def test_fragment_quoting_7a(testsdir):
 #     selfdir = (testsdir / 'lib1').as_posix()
 #     result = pypkgconf.query_args(f'--with-path={selfdir} --cflags fragment-quoting-7')
 
 #     assert result == ['-Dhello=10', '-Dworld=+32', '-DDEFINED_FROM_PKG_CONFIG=hello\\ world']
 
-    # 	cat > test.c <<- __TESTCASE_END__
-    # 		int main(int argc, char *argv[]) { return DEFINED_FROM_PKG_CONFIG; }
-    # 	__TESTCASE_END__
-    # 	cc -o test-fragment-quoting-7 ${test_cflags} ./test.c
-    # 	atf_check -e 42 ./test-fragment-quoting-7
-    # 	rm -f test.c test-fragment-quoting-7
+# 	cat > test.c <<- __TESTCASE_END__
+# 		int main(int argc, char *argv[]) { return DEFINED_FROM_PKG_CONFIG; }
+# 	__TESTCASE_END__
+# 	cc -o test-fragment-quoting-7 ${test_cflags} ./test.c
+# 	atf_check -e 42 ./test-fragment-quoting-7
+# 	rm -f test.c test-fragment-quoting-7
 
 
 def test_fragment_comment(testsdir):
-    selfdir = (testsdir / 'lib1').as_posix()
-    result = pypkgconf.query_args(f'--with-path={selfdir} --cflags fragment-comment')
+    selfdir = (testsdir / "lib1").as_posix()
+    result = pypkgconf.query_args(f"--with-path={selfdir} --cflags fragment-comment")
 
-    assert result == ['kuku=\\#ttt']
+    assert result == ["kuku=\\#ttt"]
 
 
-@pytest.mark.skip(reason='--msvc-syntax not implemented')
-@with_lib1
-def test_msvc_fragment_quoting():
-    result = pypkgconf.query_args('--libs --msvc-syntax fragment-escaping-1')
+@pytest.mark.skip(reason="--msvc-syntax not implemented")
+def test_msvc_fragment_quoting(lib1_env):
+    result = pypkgconf.query_args(
+        "--libs --msvc-syntax fragment-escaping-1", env=lib1_env
+    )
 
-    assert result == ['/libpath:"C:\\D E"', 'E.lib']
+    assert result == ['/libpath:"C:\\D E"', "E.lib"]
 
 
-@pytest.mark.skip(reason='--msvc-syntax not implemented')
-@with_lib1
-def test_msvc_fragment_render_cflags():
-    result = pypkgconf.query_args('--cflags --static --msvc-syntax foo')
+@pytest.mark.skip(reason="--msvc-syntax not implemented")
+def test_msvc_fragment_render_cflags(lib1_env):
+    result = pypkgconf.query_args("--cflags --static --msvc-syntax foo", env=lib1_env)
 
-    assert result == ['/I/test/include/foo', '/DFOO_STATIC']
+    assert result == ["/I/test/include/foo", "/DFOO_STATIC"]
 
 
 def test_tuple_dequote(testsdir):
-    selfdir = (testsdir / 'lib1').as_posix()
-    result = pypkgconf.query_args(f'--with-path={selfdir} --libs tuple-quoting')
+    selfdir = (testsdir / "lib1").as_posix()
+    result = pypkgconf.query_args(f"--with-path={selfdir} --libs tuple-quoting")
 
-    assert result == ['-L/test/lib', '-lfoo']
+    assert result == ["-L/test/lib", "-lfoo"]
 
 
 def test_version_with_whitespace(testsdir):
-    selfdir = (testsdir / 'lib1').as_posix()
-    result = pypkgconf.query_args(f'--with-path={selfdir} --modversion malformed-version')
+    selfdir = (testsdir / "lib1").as_posix()
+    result = pypkgconf.query_args(
+        f"--with-path={selfdir} --modversion malformed-version"
+    )
 
-    assert result == ['3.922']
+    assert result == ["3.922"]
 
 
 def test_version_with_whitespace_2(testsdir):
-    selfdir = (testsdir / 'lib1').as_posix()
-    result = pypkgconf.query_args(f'--with-path={selfdir} --print-provides malformed-version')
+    selfdir = (testsdir / "lib1").as_posix()
+    result = pypkgconf.query_args(
+        f"--with-path={selfdir} --print-provides malformed-version"
+    )
 
-    assert result == ['malformed-version = 3.922']
+    assert result == ["malformed-version = 3.922"]
 
 
 def test_version_with_whitespace_diagnostic(testsdir, caplog):
-    selfdir = (testsdir / 'lib1').as_posix()
+    selfdir = (testsdir / "lib1").as_posix()
 
     with caplog.at_level(logging.WARNING):
-        result = pypkgconf.query_args(f'--with-path={selfdir} --validate malformed-version')
+        result = pypkgconf.query_args(
+            f"--with-path={selfdir} --validate malformed-version"
+        )
 
     assert result == []
-    assert any(record.levelname == 'WARNING' for record in caplog.records)
+    assert any(record.levelname == "WARNING" for record in caplog.records)
```

### Comparing `pypkgconf-0.1.0/tests/test_provides.py` & `pypkgconf-0.1.1/tests/test_provides.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,145 +1,210 @@
 import pypkgconf
 
 import pytest
 
 
-with_lib1 = pytest.mark.usefixtures('lib1_pkg_config_path')
-
-
-@with_lib1
-def test_simple():
-    result = pypkgconf.query_args('--print-provides provides')
+def test_simple(lib1_env):
+    result = pypkgconf.query_args("--print-provides provides", env=lib1_env)
     assert result == [
-        'provides-test-foo = 1.0.0',
-        'provides-test-bar > 1.1.0',
-        'provides-test-baz >= 1.1.0',
-        'provides-test-quux < 1.2.0',
-        'provides-test-moo <= 1.2.0',
-        'provides-test-meow != 1.3.0',
-        'provides = 1.2.3',
+        "provides-test-foo = 1.0.0",
+        "provides-test-bar > 1.1.0",
+        "provides-test-baz >= 1.1.0",
+        "provides-test-quux < 1.2.0",
+        "provides-test-moo <= 1.2.0",
+        "provides-test-meow != 1.3.0",
+        "provides = 1.2.3",
     ]
 
-    result = pypkgconf.query_args('--libs provides-request-simple')
-    assert result == ['-lfoo']
+    result = pypkgconf.query_args("--libs provides-request-simple", env=lib1_env)
+    assert result == ["-lfoo"]
 
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--no-provides --libs provides-request-simple')
+        pypkgconf.query_args(
+            "--no-provides --libs provides-request-simple", env=lib1_env
+        )
 
 
-@with_lib1
-def test_foo():
-    assert pypkgconf.query_args('--libs provides-test-foo') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-foo = 1.0.0"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-foo >= 1.0.0"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-foo <= 1.0.0"') == ['-lfoo']
+def test_foo(lib1_env):
+    assert pypkgconf.query_args("--libs provides-test-foo", env=lib1_env) == ["-lfoo"]
+    assert pypkgconf.query_args('--libs "provides-test-foo = 1.0.0"', env=lib1_env) == [
+        "-lfoo"
+    ]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-foo >= 1.0.0"', env=lib1_env
+    ) == ["-lfoo"]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-foo <= 1.0.0"', env=lib1_env
+    ) == ["-lfoo"]
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-foo != 1.0.0"')
+        pypkgconf.query_args('--libs "provides-test-foo != 1.0.0"', env=lib1_env)
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-foo > 1.0.0"')
+        pypkgconf.query_args('--libs "provides-test-foo > 1.0.0"', env=lib1_env)
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-foo < 1.0.0"')
+        pypkgconf.query_args('--libs "provides-test-foo < 1.0.0"', env=lib1_env)
 
 
-@with_lib1
-def test_bar():
-    assert pypkgconf.query_args('--libs provides-test-bar') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-bar = 1.1.1"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-bar >= 1.1.1"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-bar <= 1.1.1"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-bar != 1.1.0"') == ['-lfoo']
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-bar != 1.1.1"')
-    assert pypkgconf.query_args('--libs "provides-test-bar > 1.1.1"') == ['-lfoo']
+def test_bar(lib1_env):
+    assert pypkgconf.query_args("--libs provides-test-bar", env=lib1_env) == ["-lfoo"]
+    assert pypkgconf.query_args('--libs "provides-test-bar = 1.1.1"', env=lib1_env) == [
+        "-lfoo"
+    ]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-bar >= 1.1.1"', env=lib1_env
+    ) == ["-lfoo"]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-bar <= 1.1.1"', env=lib1_env
+    ) == ["-lfoo"]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-bar != 1.1.0"', env=lib1_env
+    ) == ["-lfoo"]
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-bar != 1.1.1"', env=lib1_env)
+    assert pypkgconf.query_args('--libs "provides-test-bar > 1.1.1"', env=lib1_env) == [
+        "-lfoo"
+    ]
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-bar <= 1.1.0"')
-    assert pypkgconf.query_args('--libs "provides-test-bar <= 1.2.0"') == ['-lfoo']
-    
+        pypkgconf.query_args('--libs "provides-test-bar <= 1.1.0"', env=lib1_env)
+    assert pypkgconf.query_args(
+        '--libs "provides-test-bar <= 1.2.0"', env=lib1_env
+    ) == ["-lfoo"]
 
-@with_lib1
-def test_bar():
-    assert pypkgconf.query_args('--libs provides-test-baz') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-baz = 1.1.0"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-baz >= 1.1.0"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-baz <= 1.1.0"') == ['-lfoo']
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-baz != 1.1.0"')
-    assert pypkgconf.query_args('--libs "provides-test-baz !- 1.0.0"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-baz > 1.1.1"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-baz > 1.1.0"') == ['-lfoo']
+
+def test_bar(lib1_env):
+    assert pypkgconf.query_args("--libs provides-test-baz", env=lib1_env) == ["-lfoo"]
+    assert pypkgconf.query_args('--libs "provides-test-baz = 1.1.0"', env=lib1_env) == [
+        "-lfoo"
+    ]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-baz >= 1.1.0"', env=lib1_env
+    ) == ["-lfoo"]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-baz <= 1.1.0"', env=lib1_env
+    ) == ["-lfoo"]
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-baz != 1.1.0"', env=lib1_env)
+    assert pypkgconf.query_args(
+        '--libs "provides-test-baz !- 1.0.0"', env=lib1_env
+    ) == ["-lfoo"]
+    assert pypkgconf.query_args('--libs "provides-test-baz > 1.1.1"', env=lib1_env) == [
+        "-lfoo"
+    ]
+    assert pypkgconf.query_args('--libs "provides-test-baz > 1.1.0"', env=lib1_env) == [
+        "-lfoo"
+    ]
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-baz < 1.1.0"')
-    assert pypkgconf.query_args('--libs "provides-test-baz < 1.2.0"') == ['-lfoo']
+        pypkgconf.query_args('--libs "provides-test-baz < 1.1.0"', env=lib1_env)
+    assert pypkgconf.query_args('--libs "provides-test-baz < 1.2.0"', env=lib1_env) == [
+        "-lfoo"
+    ]
 
 
-@with_lib1
-def test_quux():
-    assert pypkgconf.query_args('--libs provides-test-quux') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-quux = 1.1.9"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-quux >= 1.1.0"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-quux >= 1.1.9"') == ['-lfoo']
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-quux >= 1.2.0"')
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-quux <= 1.2.0"')
-    assert pypkgconf.query_args('--libs "provides-test-quux <= 1.1.9"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-quux != 1.2.0"') == ['-lfoo']
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-quux != 1.1.0"')
-    assert pypkgconf.query_args('--libs "provides-test-quux > 1.1.9"') == ['-lfoo']
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-quux > 1.2.0"')
-    assert pypkgconf.query_args('--libs "provides-test-quux < 1.1.0"') == ['-lfoo']
+def test_quux(lib1_env):
+    assert pypkgconf.query_args("--libs provides-test-quux", env=lib1_env) == ["-lfoo"]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-quux = 1.1.9"', env=lib1_env
+    ) == ["-lfoo"]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-quux >= 1.1.0"', env=lib1_env
+    ) == ["-lfoo"]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-quux >= 1.1.9"', env=lib1_env
+    ) == ["-lfoo"]
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-quux >= 1.2.0"', env=lib1_env)
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-quux <= 1.2.0"', env=lib1_env)
+    assert pypkgconf.query_args(
+        '--libs "provides-test-quux <= 1.1.9"', env=lib1_env
+    ) == ["-lfoo"]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-quux != 1.2.0"', env=lib1_env
+    ) == ["-lfoo"]
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-quux != 1.1.0"', env=lib1_env)
+    assert pypkgconf.query_args(
+        '--libs "provides-test-quux > 1.1.9"', env=lib1_env
+    ) == ["-lfoo"]
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-quux > 1.2.0"', env=lib1_env)
+    assert pypkgconf.query_args(
+        '--libs "provides-test-quux < 1.1.0"', env=lib1_env
+    ) == ["-lfoo"]
     # FIXME: Test duplicated...
     # with pytest.raises(pypkgconf.PkgConfError):
     #     pypkgconf.query_args('--libs "provides-test-quux > 1.2.0"')
 
 
-@with_lib1
-def test_moo():
-    assert pypkgconf.query_args('--libs provides-test-moo') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-moo = 1.2.0"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-moo >= 1.1.0"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-moo >= 1.2.0"') == ['-lfoo']
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-moo >= 1.2.1"')
-    assert pypkgconf.query_args('--libs "provides-test-moo <= 1.2.0"') == ['-lfoo']
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-moo != 1.1.0"')
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-moo != 1.0.0"')
-    assert pypkgconf.query_args('--libs "provides-test-moo > 1.1.9"') == ['-lfoo']
+def test_moo(lib1_env):
+    assert pypkgconf.query_args("--libs provides-test-moo", env=lib1_env) == ["-lfoo"]
+    assert pypkgconf.query_args('--libs "provides-test-moo = 1.2.0"', env=lib1_env) == [
+        "-lfoo"
+    ]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-moo >= 1.1.0"', env=lib1_env
+    ) == ["-lfoo"]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-moo >= 1.2.0"', env=lib1_env
+    ) == ["-lfoo"]
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-moo >= 1.2.1"', env=lib1_env)
+    assert pypkgconf.query_args(
+        '--libs "provides-test-moo <= 1.2.0"', env=lib1_env
+    ) == ["-lfoo"]
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-moo != 1.1.0"', env=lib1_env)
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-moo != 1.0.0"', env=lib1_env)
+    assert pypkgconf.query_args('--libs "provides-test-moo > 1.1.9"', env=lib1_env) == [
+        "-lfoo"
+    ]
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-moo > 1.2.0"')
-    assert pypkgconf.query_args('--libs "provides-test-moo < 1.1.0"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-moo < 1.2.0"') == ['-lfoo']
-
+        pypkgconf.query_args('--libs "provides-test-moo > 1.2.0"', env=lib1_env)
+    assert pypkgconf.query_args('--libs "provides-test-moo < 1.1.0"', env=lib1_env) == [
+        "-lfoo"
+    ]
+    assert pypkgconf.query_args('--libs "provides-test-moo < 1.2.0"', env=lib1_env) == [
+        "-lfoo"
+    ]
 
 
-@with_lib1
-def test_meow():
-    assert pypkgconf.query_args('--libs provides-test-meow') == ['-lfoo']
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-meow = 1.3.0"')
-    assert pypkgconf.query_args('--libs "provides-test-meow != 1.3.0"') == ['-lfoo']
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-meow > 1.2.0"')
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-meow < 1.3.1"')
-    assert pypkgconf.query_args('--libs "provides-test-meow < 1.3.0"') == ['-lfoo']
-    assert pypkgconf.query_args('--libs "provides-test-meow > 1.3.0"') == ['-lfoo']
-    with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-meow >= 1.3.0"')
-    assert pypkgconf.query_args('--libs "provides-test-meow >= 1.3.1"') == ['-lfoo']
+def test_meow(lib1_env):
+    assert pypkgconf.query_args("--libs provides-test-meow", env=lib1_env) == ["-lfoo"]
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--libs "provides-test-meow <= 1.3.0"')
-    assert pypkgconf.query_args('--libs "provides-test-meow < 1.2.0"') == ['-lfoo']
+        pypkgconf.query_args('--libs "provides-test-meow = 1.3.0"', env=lib1_env)
+    assert pypkgconf.query_args(
+        '--libs "provides-test-meow != 1.3.0"', env=lib1_env
+    ) == ["-lfoo"]
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-meow > 1.2.0"', env=lib1_env)
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-meow < 1.3.1"', env=lib1_env)
+    assert pypkgconf.query_args(
+        '--libs "provides-test-meow < 1.3.0"', env=lib1_env
+    ) == ["-lfoo"]
+    assert pypkgconf.query_args(
+        '--libs "provides-test-meow > 1.3.0"', env=lib1_env
+    ) == ["-lfoo"]
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-meow >= 1.3.0"', env=lib1_env)
+    assert pypkgconf.query_args(
+        '--libs "provides-test-meow >= 1.3.1"', env=lib1_env
+    ) == ["-lfoo"]
+    with pytest.raises(pypkgconf.PkgConfError):
+        pypkgconf.query_args('--libs "provides-test-meow <= 1.3.0"', env=lib1_env)
+    assert pypkgconf.query_args(
+        '--libs "provides-test-meow < 1.2.0"', env=lib1_env
+    ) == ["-lfoo"]
 
 
 def test_indirect_dependency_node(testsdir):
-    selfdir = (testsdir / 'lib1').as_posix()
+    selfdir = (testsdir / "lib1").as_posix()
 
-    result = pypkgconf.query_args(f'--with-path="{selfdir}" --modversion "provides-test-meow"')
-    assert result == ['1.2.3']
+    result = pypkgconf.query_args(
+        f'--with-path="{selfdir}" --modversion "provides-test-meow"'
+    )
+    assert result == ["1.2.3"]
 
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args(f'--with-path="{selfdir}" --modversion "provides-test-meow = 1.3.0"')
+        pypkgconf.query_args(
+            f'--with-path="{selfdir}" --modversion "provides-test-meow = 1.3.0"'
+        )
```

### Comparing `pypkgconf-0.1.0/tests/test_regress.py` & `pypkgconf-0.1.1/tests/test_regress.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,244 +3,279 @@
 import pytest
 
 import logging
 import os
 import sys
 
 
-with_lib1 = pytest.mark.usefixtures('lib1_pkg_config_path')
-with_lib2 = pytest.mark.usefixtures('lib2_pkg_config_path')
+def test_case_sensitivity(lib1_env):
+    assert pypkgconf.query_args("--variable=foo case-sensitivity", env=lib1_env) == [
+        "3"
+    ]
+    assert pypkgconf.query_args("--variable=Foo case-sensitivity", env=lib1_env) == [
+        "4"
+    ]
 
 
-@with_lib1
-def test_case_sensitivity():
-    assert pypkgconf.query_args('--variable=foo case-sensitivity') == ['3']
-    assert pypkgconf.query_args('--variable=Foo case-sensitivity') == ['4']
-
-
-@with_lib1
-def test_depgraph_break_1():
+def test_depgraph_break_1(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--exists --print-errors "foo > 0.6.0 foo < 0.8.0"')
+        pypkgconf.query_args(
+            '--exists --print-errors "foo > 0.6.0 foo < 0.8.0"', env=lib1_env
+        )
 
 
-@with_lib1
-def test_depgraph_break_2():
+def test_depgraph_break_2(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--exists --print-errors "nonexisting foo <= 3"')
+        pypkgconf.query_args(
+            '--exists --print-errors "nonexisting foo <= 3"', env=lib1_env
+        )
 
 
-@with_lib1
-def test_depgraph_break_3():
+def test_depgraph_break_3(lib1_env):
     with pytest.raises(pypkgconf.PkgConfError):
-        pypkgconf.query_args('--exists --print-errors "depgraph-break"')
-
+        pypkgconf.query_args('--exists --print-errors "depgraph-break"', env=lib1_env)
 
-@with_lib1
-def test_define_variable():
-    result = pypkgconf.query_args('--variable=typelibdir --define-variable="libdir=\\${libdir}" typelibdir')
-    assert result == ['\\${libdir}/typelibdir']
 
+def test_define_variable(lib1_env):
+    result = pypkgconf.query_args(
+        '--variable=typelibdir --define-variable="libdir=\\${libdir}" typelibdir',
+        env=lib1_env,
+    )
+    assert result == ["\\${libdir}/typelibdir"]
 
-@with_lib1
-def test_define_variable_override():
-    result = pypkgconf.query_args('--variable=prefix --define-variable="prefix=/test" typelibdir')
-    assert result == ['/test']
 
+def test_define_variable_override(lib1_env):
+    result = pypkgconf.query_args(
+        '--variable=prefix --define-variable="prefix=/test" typelibdir', env=lib1_env
+    )
+    assert result == ["/test"]
 
-@with_lib1
-def test_variable():
-    result = pypkgconf.query_args('--variable=includedir foo')
-    assert result == ['/test/include']
 
+def test_variable(lib1_env):
+    result = pypkgconf.query_args("--variable=includedir foo", env=lib1_env)
+    assert result == ["/test/include"]
 
-@with_lib1
-def test_keep_system_libs(monkeypatch):
-    monkeypatch.setenv('LIBRARY_PATH', '/test/local/lib')
 
-    assert pypkgconf.query_args('--libs-only-L cflags-libs-only') == []
+def test_keep_system_libs(lib1_env):
+    env = {"LIBRARY_PATH": "/test/local/lib"}
+    env.update(lib1_env)
 
-    result = pypkgconf.query_args('--libs-only-L --keep-system-libs cflags-libs-only')
-    assert result == ['-L/test/local/lib']
+    assert pypkgconf.query_args("--libs-only-L cflags-libs-only", env=env) == []
 
+    result = pypkgconf.query_args(
+        "--libs-only-L --keep-system-libs cflags-libs-only", env=env
+    )
+    assert result == ["-L/test/local/lib"]
 
-@with_lib1
-def test_libs():
-    result = pypkgconf.query_args('--libs cflags-libs-only')
-    assert result == ['-L/test/local/lib', '-lfoo']
 
+def test_libs(lib1_env):
+    result = pypkgconf.query_args("--libs cflags-libs-only", env=lib1_env)
+    assert result == ["-L/test/local/lib", "-lfoo"]
 
-@with_lib1
-def test_libs_only():
-    result = pypkgconf.query_args('--libs-only-L --libs-only-l cflags-libs-only')
-    assert result == ['-L/test/local/lib', '-lfoo']
 
+def test_libs_only(lib1_env):
+    result = pypkgconf.query_args(
+        "--libs-only-L --libs-only-l cflags-libs-only", env=lib1_env
+    )
+    assert result == ["-L/test/local/lib", "-lfoo"]
 
 
-@with_lib1
-def test_libs_never_mergeback():
-    result = pypkgconf.query_args('--libs prefix-foo1')
-    assert result == ['-L/test/bar/lib', '-lfoo1']
+def test_libs_never_mergeback(lib1_env):
+    result = pypkgconf.query_args("--libs prefix-foo1", env=lib1_env)
+    assert result == ["-L/test/bar/lib", "-lfoo1"]
 
-    result = pypkgconf.query_args('--libs prefix-foo1 prefix-foo2')
-    assert result == ['-L/test/bar/lib', '-lfoo1', '-lfoo2']
+    result = pypkgconf.query_args("--libs prefix-foo1 prefix-foo2", env=lib1_env)
+    assert result == ["-L/test/bar/lib", "-lfoo1", "-lfoo2"]
 
 
-@with_lib1
-def test_cflags_only():
-    result = pypkgconf.query_args('--cflags-only-I --cflags-only-other cflags-libs-only')
-    assert result == ['-I/test/local/include/foo']
+def test_cflags_only(lib1_env):
+    result = pypkgconf.query_args(
+        "--cflags-only-I --cflags-only-other cflags-libs-only", env=lib1_env
+    )
+    assert result == ["-I/test/local/include/foo"]
 
 
+def test_cflags_never_mergeback(lib1_env):
+    result = pypkgconf.query_args("--cflags prefix-foo1 prefix-foo2", env=lib1_env)
+    assert result == ["-I/test/bar/include/foo", "-DBAR", "-fPIC", "-DFOO"]
 
-@with_lib1
-def test_cflags_never_mergeback():
-    result = pypkgconf.query_args('--cflags prefix-foo1 prefix-foo2')
-    assert result == ['-I/test/bar/include/foo', '-DBAR', '-fPIC', '-DFOO']
 
-
-@with_lib1
-def test_incomplete_libs():
-    result = pypkgconf.query_args('--libs incomplete')
+def test_incomplete_libs(lib1_env):
+    result = pypkgconf.query_args("--libs incomplete", env=lib1_env)
     assert result == []
 
 
-@with_lib1
-def test_incomplete_cflags():
-    result = pypkgconf.query_args('--cflags incomplete')
+def test_incomplete_cflags(lib1_env):
+    result = pypkgconf.query_args("--cflags incomplete", env=lib1_env)
     assert result == []
 
 
-@with_lib1
-def test_isystem_munge_order():
-    result = pypkgconf.query_args('--cflags isystem')
-    assert result == ['-isystem', '/opt/bad/include', '-isystem', '/opt/bad2/include']
+def test_isystem_munge_order(lib1_env):
+    result = pypkgconf.query_args("--cflags isystem", env=lib1_env)
+    assert result == ["-isystem", "/opt/bad/include", "-isystem", "/opt/bad2/include"]
 
 
-@with_lib1
-def test_isystem_munge_sysroot(monkeypatch, testsdir):
-    monkeypatch.setenv('PKG_CONFIG_SYSROOT_DIR', testsdir.as_posix())
+def test_isystem_munge_sysroot(testsdir, lib1_env):
+    env = {"PKG_CONFIG_SYSROOT_DIR": testsdir.as_posix()}
+    env.update(lib1_env)
 
-    result = pypkgconf.query_args('--cflags isystem')
+    result = pypkgconf.query_args("--cflags isystem", env=env)
 
-    assert f'-isystem {testsdir.as_posix()}/opt/bad/include' in ' '.join(result)
+    assert f"-isystem {testsdir.as_posix()}/opt/bad/include" in " ".join(result)
 
 
-@with_lib1
-def test_idirafter_munge_order():
-    result = pypkgconf.query_args('--cflags idirafter')
-    assert result == ['-idirafter', '/opt/bad/include', '-idirafter', '/opt/bad2/include']
+def test_idirafter_munge_order(lib1_env):
+    result = pypkgconf.query_args("--cflags idirafter", env=lib1_env)
+    assert result == [
+        "-idirafter",
+        "/opt/bad/include",
+        "-idirafter",
+        "/opt/bad2/include",
+    ]
 
 
-@with_lib1
-def test_idirafter_munge_sysroot(monkeypatch, testsdir):
-    monkeypatch.setenv('PKG_CONFIG_SYSROOT_DIR', testsdir.as_posix())
+def test_idirafter_munge_sysroot(testsdir, lib1_env):
+    env = {"PKG_CONFIG_SYSROOT_DIR": testsdir.as_posix()}
+    env.update(lib1_env)
 
-    result = pypkgconf.query_args('--cflags idirafter')
-    assert f'-idirafter {testsdir.as_posix()}/opt/bad/include' in ' '.join(result)
+    result = pypkgconf.query_args("--cflags idirafter", env=env)
+    assert f"-idirafter {testsdir.as_posix()}/opt/bad/include" in " ".join(result)
 
 
-@with_lib1
-def test_idirafter_ordering():
-    result = pypkgconf.query_args('--cflags idirafter-ordering')
-    assert result == ['-I/opt/bad/include1', '-idirafter', '-I/opt/bad/include2', '-I/opt/bad/include3']
+def test_idirafter_ordering(lib1_env):
+    result = pypkgconf.query_args("--cflags idirafter-ordering", env=lib1_env)
+    assert result == [
+        "-I/opt/bad/include1",
+        "-idirafter",
+        "-I/opt/bad/include2",
+        "-I/opt/bad/include3",
+    ]
 
 
-@with_lib2
-def test_pcpath(testsdir):
+def test_pcpath(testsdir, lib2_env):
     selfdir = testsdir.as_posix()
 
-    result = pypkgconf.query_args(f'--cflags {selfdir}/lib3/bar.pc')
-    assert result == ['-fPIC', '-I/test/include/foo']
-
+    result = pypkgconf.query_args(f"--cflags {selfdir}/lib3/bar.pc", env=lib2_env)
+    assert result == ["-fPIC", "-I/test/include/foo"]
 
-def test_sysroot_munge(tmp_path, testsdir, monkeypatch):
-    contents = (testsdir / 'lib1' / 'sysroot-dir.pc').read_text(encoding='utf-8')
-    contents = contents.replace('/sysroot/', testsdir.as_posix() + '/')
 
-    (tmp_path / 'lib1').mkdir()
-    (tmp_path / 'lib1' / 'sysroot-dir-selfdir.pc').write_text(contents, encoding='utf-8')
+def test_sysroot_munge(tmp_path, testsdir):
+    contents = (testsdir / "lib1" / "sysroot-dir.pc").read_text(encoding="utf-8")
+    contents = contents.replace("/sysroot/", testsdir.as_posix() + "/")
+
+    (tmp_path / "lib1").mkdir()
+    (tmp_path / "lib1" / "sysroot-dir-selfdir.pc").write_text(
+        contents, encoding="utf-8"
+    )
+
+    env = {
+        "PKG_CONFIG_PATH": (tmp_path / "lib1").as_posix(),
+        "PKG_CONFIG_SYSROOT_DIR": testsdir.as_posix(),
+    }
 
-    monkeypatch.setenv('PKG_CONFIG_PATH', (tmp_path / 'lib1').as_posix())
-    monkeypatch.setenv('PKG_CONFIG_SYSROOT_DIR', testsdir.as_posix())
-
-    result = pypkgconf.query_args('--libs sysroot-dir-selfdir')
-    assert result == [f'-L{testsdir.as_posix()}/lib', '-lfoo']
+    result = pypkgconf.query_args("--libs sysroot-dir-selfdir", env=env)
+    assert result == [f"-L{testsdir.as_posix()}/lib", "-lfoo"]
 
 
 def test_virtual_variable():
-    assert pypkgconf.query_args('--exists pkg-config') == []
-    assert pypkgconf.query_args('--exists pkgconf') == []
+    assert pypkgconf.query_args("--exists pkg-config") == []
+    assert pypkgconf.query_args("--exists pkgconf") == []
 
-    if sys.platform in {'win32', 'cygwin', 'msys'}:
-        pcpath = '../lib/pkgconfig;../share/pkgconfig'
+    if sys.platform in {"win32", "cygwin", "msys"}:
+        pcpath = "../lib/pkgconfig;../share/pkgconfig"
     else:
-        pcpath = os.environ.get('PKG_DEFAULT_PATH')
-    result = pypkgconf.query_args('--variable=pc_path pkg-config')
+        pcpath = os.environ.get("PKG_DEFAULT_PATH")
+    result = pypkgconf.query_args("--variable=pc_path pkg-config")
     assert result == [pcpath]
 
-    result = pypkgconf.query_args('--variable=pc_path pkgconf')
+    result = pypkgconf.query_args("--variable=pc_path pkgconf")
     assert result == [pcpath]
 
 
-
 def test_fragment_collision(testsdir):
     selfdir = testsdir.as_posix()
 
-    result = pypkgconf.query_args(f'--with-path="{selfdir}/lib1" --cflags fragment-collision')
-    assert result == ['-D_BAZ', '-D_BAR', '-D_FOO', '-D_THREAD_SAFE', '-pthread']
+    result = pypkgconf.query_args(
+        f'--with-path="{selfdir}/lib1" --cflags fragment-collision'
+    )
+    assert result == ["-D_BAZ", "-D_BAR", "-D_FOO", "-D_THREAD_SAFE", "-pthread"]
 
 
 def test_malformed_1(testsdir):
     selfdir = testsdir.as_posix()
 
     with pytest.raises(pypkgconf.PkgConfError):
         pypkgconf.query_args(f'--validate --with-path="{selfdir}/lib1" malformed-1')
 
 
 def test_malformed_quoting(testsdir):
     selfdir = testsdir.as_posix()
 
-    assert pypkgconf.query_args(f'--validate --with-path="{selfdir}/lib1" malformed-quoting') == []
+    assert (
+        pypkgconf.query_args(
+            f'--validate --with-path="{selfdir}/lib1" malformed-quoting'
+        )
+        == []
+    )
 
 
 def test_explicit_sysroot(monkeypatch, testsdir):
     # FIXME: does not work with drive letter...
     selfdir = testsdir.as_posix().removeprefix(testsdir.drive)
-    monkeypatch.setenv('PKG_CONFIG_SYSROOT_DIR', selfdir)
+    monkeypatch.setenv("PKG_CONFIG_SYSROOT_DIR", selfdir)
 
-    result = pypkgconf.query_args(f'--debug --with-path="{selfdir}/lib1" --variable=pkgdatadir explicit-sysroot')
-    assert result == [f'{selfdir}/usr/share/test']
+    result = pypkgconf.query_args(
+        f'--debug --with-path="{selfdir}/lib1" --variable=pkgdatadir explicit-sysroot'
+    )
+    assert result == [f"{selfdir}/usr/share/test"]
 
 
 def test_empty_tuple(testsdir):
     selfdir = testsdir.as_posix()
 
-    assert pypkgconf.query_args(f'--with-path="{selfdir}/lib1" --cflags empty-tuple') == []
-
+    assert (
+        pypkgconf.query_args(f'--with-path="{selfdir}/lib1" --cflags empty-tuple') == []
+    )
 
 
 def test_solver_requires_private_debounce(testsdir):
     selfdir = testsdir.as_posix()
 
-    result = pypkgconf.query_args(f'--with-path="{selfdir}/lib1" --cflags --libs metapackage')
-    assert result == ['-I/metapackage-1', '-I/metapackage-2', '-lmetapackage-1', '-lmetapackage-2']
-    
+    result = pypkgconf.query_args(
+        f'--with-path="{selfdir}/lib1" --cflags --libs metapackage'
+    )
+    assert result == [
+        "-I/metapackage-1",
+        "-I/metapackage-2",
+        "-lmetapackage-1",
+        "-lmetapackage-2",
+    ]
+
 
 def test_solver_requires_private_debounce(testsdir, caplog):
     selfdir = testsdir.as_posix()
 
     with caplog.at_level(logging.WARNING):
-        assert pypkgconf.query_args(f'--with-path="{selfdir}/lib1" --validate billion-laughs') == []
+        assert (
+            pypkgconf.query_args(
+                f'--with-path="{selfdir}/lib1" --validate billion-laughs'
+            )
+            == []
+        )
 
     s = 0
     for r in caplog.records:
-        if r.levelno == logging.WARNING and r.msg == 'warning: truncating very long variable to 64KB':
+        if (
+            r.levelno == logging.WARNING
+            and r.msg == "warning: truncating very long variable to 64KB"
+        ):
             s += 1
     assert s == 5
 
 
 def test_maximum_package_depth_off_by_one(testsdir):
     selfdir = testsdir.as_posix()
 
-    result = pypkgconf.query_args(f'--with-path="{selfdir}/lib1" --modversion foo bar baz')
-    assert result == ['1.2.3']
+    result = pypkgconf.query_args(
+        f'--with-path="{selfdir}/lib1" --modversion foo bar baz'
+    )
+    assert result == ["1.2.3"]
```

### Comparing `pypkgconf-0.1.0/PKG-INFO` & `pypkgconf-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypkgconf
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python bindings to libpkgconf
 Author-Email: Charles Brunet <charles.brunet@optelgroup.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -252,18 +252,20 @@
 This high-level API uses same arguments as the `pkgconf` executable.
 
 Results are returned as a list of string (the list may be empty).
 Errors and warnings are logger using the standard Python logging module, under
 the `pkgconf` logger.
 In case or error result, a `pypkgconf.PkgConfError` exception is raised.
 
-#### `pypkgconf.query_args(command: str) -> list[str]`
+#### `pypkgconf.query_args(command: str, env: dict[str, str] | None = None) -> list[str]`
 
 The command is just like the command line arguments (e.g.: `"--libs foo"`)
 
+If `env` is provided, pkgconf will use it for any envvar it queries.
+If `env` is `None` (default), `os.environ` is used.
 
 #### `pypkgconf.query(args: list[str] | None, **kwargs) -> list[str]`
 
 Positional arguments are given as a list of strings.
 
 Optional arguments are given either using an union of `pypkgconf.Flags`,
 or as keyword arguments, depending if it is a boolean value or not.
```

