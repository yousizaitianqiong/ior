AM_CPPFLAGS = -I$(top_srcdir)/src
AM_LDFLAGS = $(extraLDFLAGS)
LDADD    = ../libaiori.a $(extraLDADD)

if USE_NCMPI_AIORI
LDADD += -lpnetcdf
endif

TESTS = testlib testexample testrand testmdtestoutput test-summary-output.sh test-ior-exit.sh test-mdtest-summary.sh test-csv-output.sh test-byte-transfers.sh test-mmap-options.sh test-mmap-file-size.sh
check_PROGRAMS = testlib testexample testrand testsummary testmdtestoutput
testexample_SOURCES  = example.c
testlib_SOURCES  = lib.c
testrand_SOURCES = rand.c
testsummary_SOURCES = summary.c
testmdtestoutput_SOURCES = mdtest-output.c
EXTRA_DIST = test-summary-output.sh test-summary-output.py test-ior-exit.sh test-ior-exit.py test-mdtest-summary.sh test-csv-output.sh test-csv-output.py test-byte-transfers.sh test-byte-transfers.py test-mmap-options.sh test-mmap-options.py test-mmap-file-size.sh test-mmap-file-size.py
