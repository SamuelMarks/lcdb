# Makefile.am - automake file for lcdb
# Copyright (c) 2022, Christopher Jeffrey (MIT License).
# https://github.com/chjj/lcdb

AM_CPPFLAGS = $(WARN_FLAGS) -I$(top_builddir)/include
AM_LDFLAGS = -no-install
LDADD = $(top_builddir)/liblcdb.la

tests_lib = t-arena        \
            t-autocompact  \
            t-bloom        \
            t-c            \
            t-cache        \
            t-coding       \
            t-corruption   \
            t-crc32c       \
            t-db           \
            t-dbformat     \
            t-env          \
            t-filename     \
            t-filter_block \
            t-hash         \
            t-issue178     \
            t-issue200     \
            t-issue320     \
            t-log          \
            t-rbt          \
            t-recovery     \
            t-simple       \
            t-skiplist     \
            t-snappy       \
            t-status       \
            t-strutil      \
            t-table        \
            t-version_edit \
            t-version_set  \
            t-write_batch

check_PROGRAMS = $(tests_lib)

TESTS = $(check_PROGRAMS)

all-local: $(check_PROGRAMS)
