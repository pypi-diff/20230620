# Comparing `tmp/yaramod-3.9.1.tar.gz` & `tmp/yaramod-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yaramod-3.9.1.tar", last modified: Mon Mar 29 12:58:20 2021, max compression
+gzip compressed data, was "dist/yaramod-3.9.2.tar", last modified: Fri Jun  4 12:24:43 2021, max compression
```

## Comparing `yaramod-3.9.1.tar` & `yaramod-3.9.2.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6667 2021-03-29 12:54:41.000000 yaramod-3.9.1/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2021-03-29 12:58:20.000000 yaramod-3.9.1/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/googletest/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3846 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/googletest/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/cmake/
--rw-rw-r--   0 travis    (2000) travis    (2000)      691 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/cmake/Findre2.cmake
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/cmake/fmt/
--rw-rw-r--   0 travis    (2000) travis    (2000)      703 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/cmake/fmt/Findfmt.cmake
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/re2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1907 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1516 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/utf.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4842 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/strutil.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     2882 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/logging.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1142 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/test.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4164 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/mutex.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    27527 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/pcre.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    36169 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/pcre.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     3762 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/benchmark.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      488 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/strutil.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      544 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/fuzz.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)      991 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/util.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4944 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/rune.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     2998 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/benchmark.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)      969 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/mix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      505 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/malloc_counter.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      678 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/flags.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      693 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/util/test.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     4368 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6336 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/stringpiece.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4058 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/filtered_re2.h
--rw-rw-r--   0 travis    (2000) travis    (2000)   119147 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/unicode_groups.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     7827 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/walker-inl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    37585 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/re2.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    17672 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prefilter.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     7140 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/sparse_set.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    74716 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/dfa.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     1011 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/pod_array.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4310 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/set.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     3320 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/filtered_re2.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    75452 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/parse.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    23588 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/regexp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    22863 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/onepass.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    27421 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prog.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    11974 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/sparse_array.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8710 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/tostring.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     2883 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/perl_groups.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    12466 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prefilter_tree.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     6057 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/mimics_pcre.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    25600 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/regexp.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/stringpiece.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    38500 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/compile.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    17912 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prog.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13119 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/unicode_casefold.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/set.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2562 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/unicode_casefold.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2564 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/bitmap256.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21866 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/nfa.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    11250 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/bitstate.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     5224 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prefilter_tree.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    20117 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/simplify.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     3031 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prefilter.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    37660 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/re2.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1548 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/re2/unicode_groups.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1558 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/re2/re2/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/fmt/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2085 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    93539 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/ChangeLog.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/support/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/support/cmake/
--rw-rw-r--   0 travis    (2000) travis    (2000)      299 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/support/cmake/FindSetEnv.cmake
--rw-rw-r--   0 travis    (2000) travis    (2000)      267 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/support/cmake/fmt.pc.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2343 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/support/cmake/cxx14.cmake
--rw-rw-r--   0 travis    (2000) travis    (2000)      110 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/support/cmake/fmt-config.cmake.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    19713 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2208 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/src/format.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)     6865 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/src/posix.cc
--rw-rw-r--   0 travis    (2000) travis    (2000)    10679 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    46856 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/core.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4263 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/ostream.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9297 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/ranges.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    15689 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/compile.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    25769 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/chrono.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8706 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/posix.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    36028 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/format-inl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)   117567 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/format.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9337 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/safe-duration-cast.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    21945 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/printf.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2870 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/locale.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    22863 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/color.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1408 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/deps/fmt/fmt/LICENSE.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5422 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/include/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/include/pog/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4467 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/state.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/include/pog/relations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5744 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/relations/includes.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/relations/relation.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4898 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/relations/lookback.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1653 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/errors.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8709 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/grammar.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      399 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/action.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7321 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/tokenizer.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2173 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/token.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2840 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/token_builder.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/include/pog/types/
--rw-rw-r--   0 travis    (2000) travis    (2000)      702 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/types/state_and_symbol.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      680 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/types/state_and_rule.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1773 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/utils.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/include/pog/operations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2877 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/operations/lookahead.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2080 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/operations/follow.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1230 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/operations/operation.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2387 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/operations/read.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2161 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/filter_view.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1478 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/symbol.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9149 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/html_report.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2694 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/digraph_algo.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2946 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/rule.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      764 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/precedence.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5299 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/parsing_table.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4567 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/automaton.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2651 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/parser_report.h
--rw-rw-r--   0 travis    (2000) travis    (2000)       96 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/pog.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9551 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/parser.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4125 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/rule_builder.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3529 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/include/pog/item.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     3802 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pog/share/
--rw-rw-r--   0 travis    (2000) travis    (2000)      218 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/share/pog.pc.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      889 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/share/pog-config.cmake.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1643 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pog/CHANGELOG.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      312 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pybind11/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pybind11/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 travis    (2000) travis    (2000)     9422 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 travis    (2000) travis    (2000)     8201 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 travis    (2000) travis    (2000)     4485 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6507 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pybind11/include/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21607 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/stl_bind.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7731 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    19031 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    65937 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/numpy.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/detail/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16322 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    13634 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    24766 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1429 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/detail/typeid.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    37068 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2031 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/options.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    14029 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4326 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8749 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2944 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    89483 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6616 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    56424 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/pytypes.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3865 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    29043 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5395 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    94338 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2001 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/complex.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/include/pybind11/common.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     5828 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/deps/pybind11/pybind11/
--rw-rw-r--   0 travis    (2000) travis    (2000)       77 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/pybind11/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      871 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/pybind11/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      879 2021-03-29 12:54:41.000000 yaramod-3.9.1/deps/pybind11/pybind11/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      167 2021-03-29 12:54:41.000000 yaramod-3.9.1/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/types/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1310 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/meta.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1858 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/plain_string.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/hex_string.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1864 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/token.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    15256 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/yara_file.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    12638 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/rule.cpp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/types/modules/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1143 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4561 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/dotnet_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)      863 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/magic_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    13706 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/dex_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     8078 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/cuckoo_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    11434 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/elf_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1350 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/metadata_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    19606 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/phish_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    18923 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/macho_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)      760 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/time_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2180 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/math_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1699 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/hash_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4507 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/androguard_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    22341 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/modules/pe_module.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     6257 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/literal.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     1154 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/variable.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    26009 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/types/token_stream.cpp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3078 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/utils/filesystem.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4704 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/utils/utils.cpp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/parser/
--rw-rw-r--   0 travis    (2000) travis    (2000)   110786 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/parser/parser_driver.cpp
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)      790 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/python/CMakeLists.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    44590 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/python/yaramod_python.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    28019 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/python/py_visitor.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    10209 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/python/py_visitor.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1571 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/python/yaramod_python.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/builder/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11983 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/builder/yara_hex_string_builder.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     4170 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/builder/yara_file_builder.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    24708 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/builder/yara_rule_builder.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)    42416 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/builder/yara_expression_builder.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)      922 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/yaramod.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)     2718 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/examples/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/examples/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10675 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/examples/python/dump_rules_ast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5236 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/examples/python/simplify_bools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/examples/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/examples/cpp/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/examples/cpp/simplify_bools/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5947 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/examples/cpp/simplify_bools/bool_simplifier.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1006 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/examples/cpp/simplify_bools/main.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)       86 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/examples/cpp/simplify_bools/CMakeLists.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/examples/cpp/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/src/examples/cpp/dump_rules_ast/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16657 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/examples/cpp/dump_rules_ast/dumper.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      704 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/examples/cpp/dump_rules_ast/main.cpp
--rw-rw-r--   0 travis    (2000) travis    (2000)       86 2021-03-29 12:54:41.000000 yaramod-3.9.1/src/examples/cpp/dump_rules_ast/CMakeLists.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2439 2021-03-29 12:58:20.000000 yaramod-3.9.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1260 2021-03-29 12:54:41.000000 yaramod-3.9.1/CMakeLists.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/include/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/include/yaramod/
--rw-rw-r--   0 travis    (2000) travis    (2000)      799 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/yaramod_error.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/include/yaramod/types/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5690 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/token.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/token_type.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      320 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/expression_type.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     8669 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/hex_string.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6780 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/symbols.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/symbol.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3652 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/rule.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    18065 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/regexp.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4367 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/expression.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     3361 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/yara_file.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6158 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/string_modifier.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/include/yaramod/types/modules/
--rw-rw-r--   0 travis    (2000) travis    (2000)      571 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/time_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2000 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/modules_pool.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      577 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/phish_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2046 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/dex_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      583 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/cuckoo_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      571 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/math_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      799 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/modules.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      631 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/metadata_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      565 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/elf_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      577 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/macho_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      577 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/magic_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      559 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/pe_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      607 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/androguard_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      583 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/dotnet_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      571 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/modules/hash_module.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1051 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/meta.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1185 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/plain_string.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5134 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/literal.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     7332 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/string.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/variable.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     6037 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/token_stream.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    56673 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/types/expressions.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/include/yaramod/utils/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7254 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/utils/visitor.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2669 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/utils/utils.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     9306 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/utils/trie.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/utils/filesystem.h
--rw-rw-r--   0 travis    (2000) travis    (2000)      918 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/utils/visitor_result.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    22092 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/utils/modifying_visitor.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10531 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/utils/observing_visitor.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/include/yaramod/parser/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6918 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/parser/parser_driver.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1415 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/parser/file_context.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     2898 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/parser/location.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     5035 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/parser/value.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     1783 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/yaramod.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/include/yaramod/builder/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2079 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/builder/yara_file_builder.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4671 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/builder/yara_rule_builder.h
--rw-rw-r--   0 travis    (2000) travis    (2000)    10329 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/builder/yara_expression_builder.h
--rw-rw-r--   0 travis    (2000) travis    (2000)     4855 2021-03-29 12:54:41.000000 yaramod-3.9.1/include/yaramod/builder/yara_hex_string_builder.h
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-29 12:58:20.000000 yaramod-3.9.1/yaramod.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2021-03-29 12:58:20.000000 yaramod-3.9.1/yaramod.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2439 2021-03-29 12:58:20.000000 yaramod-3.9.1/yaramod.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     9399 2021-03-29 12:58:20.000000 yaramod-3.9.1/yaramod.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-29 12:58:20.000000 yaramod-3.9.1/yaramod.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2021-03-29 12:54:41.000000 yaramod-3.9.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2021-03-29 12:54:41.000000 yaramod-3.9.1/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2021-03-29 12:54:41.000000 yaramod-3.9.1/LICENSE-THIRD-PARTY
--rw-rw-r--   0 travis    (2000) travis    (2000)    11242 2021-03-29 12:54:41.000000 yaramod-3.9.1/CHANGELOG.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6667 2021-06-04 12:21:24.000000 yaramod-3.9.2/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2021-06-04 12:24:43.000000 yaramod-3.9.2/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/googletest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3846 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/googletest/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/cmake/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      691 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/cmake/Findre2.cmake
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/cmake/fmt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      703 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/cmake/fmt/Findfmt.cmake
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/re2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1907 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1516 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/utf.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4842 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/strutil.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2882 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/logging.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1142 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/test.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4164 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/mutex.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27527 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/pcre.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36169 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/pcre.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3762 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/benchmark.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      488 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/strutil.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      544 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/fuzz.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)      991 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/util.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4944 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/rune.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2998 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/benchmark.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)      969 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/mix.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      505 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/malloc_counter.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      678 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/flags.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      693 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/util/test.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4368 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6336 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/stringpiece.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4058 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/filtered_re2.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119147 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/unicode_groups.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7827 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/walker-inl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37585 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/re2.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17672 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prefilter.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7140 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/sparse_set.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74716 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/dfa.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1011 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/pod_array.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4310 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/set.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3320 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/filtered_re2.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75452 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/parse.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23588 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/regexp.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22863 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/onepass.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27421 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prog.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11974 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/sparse_array.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8710 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/tostring.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2883 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/perl_groups.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12466 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prefilter_tree.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6057 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/mimics_pcre.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25600 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/regexp.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/stringpiece.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38500 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/compile.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17912 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prog.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13119 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/unicode_casefold.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2365 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/set.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2562 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/unicode_casefold.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2564 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/bitmap256.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21866 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/nfa.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11250 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/bitstate.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5224 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prefilter_tree.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20117 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/simplify.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3031 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prefilter.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37660 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/re2.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1548 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/re2/unicode_groups.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1558 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/re2/re2/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/fmt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2085 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    93539 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/ChangeLog.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/support/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/support/cmake/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      299 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/support/cmake/FindSetEnv.cmake
+-rw-rw-r--   0 travis    (2000) travis    (2000)      267 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/support/cmake/fmt.pc.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2343 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/support/cmake/cxx14.cmake
+-rw-rw-r--   0 travis    (2000) travis    (2000)      110 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/support/cmake/fmt-config.cmake.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19713 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/src/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2208 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/src/format.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6865 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/src/posix.cc
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10679 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46856 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/core.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4263 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/ostream.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9297 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/ranges.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15689 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/compile.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25769 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/chrono.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8706 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/posix.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36028 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/format-inl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117567 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/format.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9337 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/safe-duration-cast.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21945 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/printf.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2870 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/locale.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22863 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/color.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1408 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/deps/fmt/fmt/LICENSE.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5422 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/include/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/include/pog/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4467 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/state.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/include/pog/relations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5744 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/relations/includes.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/relations/relation.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4898 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/relations/lookback.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1653 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/errors.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8709 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/grammar.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      399 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/action.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7321 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/tokenizer.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2173 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/token.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2840 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/token_builder.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/include/pog/types/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      702 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/types/state_and_symbol.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      680 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/types/state_and_rule.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1773 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/utils.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/include/pog/operations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2877 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/operations/lookahead.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2080 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/operations/follow.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1230 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/operations/operation.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2387 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/operations/read.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2161 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/filter_view.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1478 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/symbol.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9149 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/html_report.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2694 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/digraph_algo.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2946 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/rule.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      764 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/precedence.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5299 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/parsing_table.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4567 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/automaton.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2651 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/parser_report.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)       96 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/pog.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9551 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/parser.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4125 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/rule_builder.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3529 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/include/pog/item.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3802 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pog/share/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      218 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/share/pog.pc.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      889 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/share/pog-config.cmake.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1643 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pog/CHANGELOG.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      312 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pybind11/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pybind11/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2995 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9422 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8201 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4485 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6507 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pybind11/include/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21607 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/stl_bind.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7731 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19031 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65937 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/numpy.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16322 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13634 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24766 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1429 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/detail/typeid.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37068 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2031 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14029 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4326 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8749 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2944 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89483 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6616 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56424 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/pytypes.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3865 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29043 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5395 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    94338 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2001 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/complex.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5828 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/deps/pybind11/pybind11/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       77 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/pybind11/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      871 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/pybind11/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      879 2021-06-04 12:21:24.000000 yaramod-3.9.2/deps/pybind11/pybind11/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      167 2021-06-04 12:21:24.000000 yaramod-3.9.2/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/types/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1310 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/meta.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1858 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/plain_string.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/hex_string.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1864 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/token.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15256 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/yara_file.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12638 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/rule.cpp
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/types/modules/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1143 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4561 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/dotnet_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)      863 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/magic_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13706 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/dex_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8078 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/cuckoo_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11434 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/elf_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1350 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/metadata_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19606 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/phish_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18923 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/macho_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)      760 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/time_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2180 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/math_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1699 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/hash_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4507 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/androguard_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22341 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/modules/pe_module.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6257 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/literal.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1154 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/variable.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25828 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/types/token_stream.cpp
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3078 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/utils/filesystem.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4704 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/utils/utils.cpp
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/parser/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   110786 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/parser/parser_driver.cpp
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/python/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      790 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/python/CMakeLists.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44590 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/python/yaramod_python.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28019 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/python/py_visitor.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10209 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/python/py_visitor.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1571 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/python/yaramod_python.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/builder/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11983 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/builder/yara_hex_string_builder.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4170 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/builder/yara_file_builder.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24708 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/builder/yara_rule_builder.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42416 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/builder/yara_expression_builder.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)      922 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/yaramod.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2718 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/examples/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/examples/python/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10675 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/examples/python/dump_rules_ast.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5236 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/examples/python/simplify_bools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/examples/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/examples/cpp/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/examples/cpp/simplify_bools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5947 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/examples/cpp/simplify_bools/bool_simplifier.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1006 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/examples/cpp/simplify_bools/main.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)       86 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/examples/cpp/simplify_bools/CMakeLists.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/examples/cpp/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/src/examples/cpp/dump_rules_ast/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16657 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/examples/cpp/dump_rules_ast/dumper.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      704 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/examples/cpp/dump_rules_ast/main.cpp
+-rw-rw-r--   0 travis    (2000) travis    (2000)       86 2021-06-04 12:21:24.000000 yaramod-3.9.2/src/examples/cpp/dump_rules_ast/CMakeLists.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2234 2021-06-04 12:24:43.000000 yaramod-3.9.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1260 2021-06-04 12:21:24.000000 yaramod-3.9.2/CMakeLists.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/include/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/include/yaramod/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      799 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/yaramod_error.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/include/yaramod/types/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5690 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/token.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/token_type.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      320 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/expression_type.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8669 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/hex_string.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6780 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/symbols.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/symbol.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3652 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/rule.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18065 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/regexp.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4367 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/expression.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3361 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/yara_file.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6158 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/string_modifier.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/include/yaramod/types/modules/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      571 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/time_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2000 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/modules_pool.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      577 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/phish_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2046 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      565 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/dex_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      583 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/cuckoo_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      571 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/math_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      799 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/modules.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      631 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/metadata_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      565 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/elf_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      577 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/macho_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      577 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/magic_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      559 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/pe_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      607 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/androguard_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      583 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/dotnet_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      571 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/modules/hash_module.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1051 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/meta.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1185 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/plain_string.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5134 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/literal.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7332 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/string.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/variable.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6037 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/token_stream.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56673 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/types/expressions.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/include/yaramod/utils/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7254 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/utils/visitor.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2669 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/utils/utils.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9306 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/utils/trie.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/utils/filesystem.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)      918 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/utils/visitor_result.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22092 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/utils/modifying_visitor.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10531 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/utils/observing_visitor.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/include/yaramod/parser/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6918 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/parser/parser_driver.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1415 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/parser/file_context.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2898 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/parser/location.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5035 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/parser/value.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1783 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/yaramod.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/include/yaramod/builder/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2079 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/builder/yara_file_builder.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4671 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/builder/yara_rule_builder.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10329 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/builder/yara_expression_builder.h
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4855 2021-06-04 12:21:24.000000 yaramod-3.9.2/include/yaramod/builder/yara_hex_string_builder.h
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-04 12:24:43.000000 yaramod-3.9.2/yaramod.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2021-06-04 12:24:42.000000 yaramod-3.9.2/yaramod.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2234 2021-06-04 12:24:42.000000 yaramod-3.9.2/yaramod.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9399 2021-06-04 12:24:42.000000 yaramod-3.9.2/yaramod.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-04 12:24:42.000000 yaramod-3.9.2/yaramod.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2021-06-04 12:21:24.000000 yaramod-3.9.2/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2021-06-04 12:21:24.000000 yaramod-3.9.2/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2021-06-04 12:21:24.000000 yaramod-3.9.2/LICENSE-THIRD-PARTY
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11242 2021-06-04 12:21:24.000000 yaramod-3.9.2/CHANGELOG.md
```

### Comparing `yaramod-3.9.1/setup.py` & `yaramod-3.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/googletest/CMakeLists.txt` & `yaramod-3.9.2/deps/googletest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/cmake/Findre2.cmake` & `yaramod-3.9.2/deps/pog/cmake/Findre2.cmake`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/cmake/fmt/Findfmt.cmake` & `yaramod-3.9.2/deps/pog/cmake/fmt/Findfmt.cmake`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/CMakeLists.txt` & `yaramod-3.9.2/deps/pog/deps/re2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/utf.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/utf.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/strutil.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/strutil.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/logging.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/logging.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/test.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/test.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/mutex.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/mutex.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/pcre.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/pcre.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/pcre.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/pcre.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/benchmark.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/benchmark.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/fuzz.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/fuzz.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/util.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/util.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/rune.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/rune.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/benchmark.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/benchmark.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/mix.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/mix.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/flags.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/flags.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/util/test.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/util/test.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/CMakeLists.txt` & `yaramod-3.9.2/deps/pog/deps/re2/re2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/stringpiece.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/stringpiece.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/filtered_re2.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/filtered_re2.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/unicode_groups.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/unicode_groups.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/walker-inl.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/walker-inl.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/re2.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/re2.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prefilter.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prefilter.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/sparse_set.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/sparse_set.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/dfa.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/dfa.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/pod_array.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/pod_array.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/set.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/set.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/filtered_re2.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/filtered_re2.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/parse.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/parse.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/regexp.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/regexp.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/onepass.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/onepass.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prog.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prog.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/sparse_array.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/sparse_array.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/tostring.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/tostring.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/perl_groups.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/perl_groups.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prefilter_tree.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prefilter_tree.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/mimics_pcre.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/mimics_pcre.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/regexp.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/regexp.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/stringpiece.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/compile.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/compile.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prog.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prog.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/unicode_casefold.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/unicode_casefold.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/set.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/set.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/unicode_casefold.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/unicode_casefold.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/bitmap256.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/bitmap256.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/nfa.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/nfa.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/bitstate.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/bitstate.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prefilter_tree.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prefilter_tree.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/simplify.cc` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/simplify.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/prefilter.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/prefilter.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/re2.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/re2.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/re2/unicode_groups.h` & `yaramod-3.9.2/deps/pog/deps/re2/re2/re2/unicode_groups.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/re2/re2/LICENSE` & `yaramod-3.9.2/deps/pog/deps/re2/re2/LICENSE`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/CMakeLists.txt` & `yaramod-3.9.2/deps/pog/deps/fmt/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/ChangeLog.rst` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/ChangeLog.rst`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/support/cmake/cxx14.cmake` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/support/cmake/cxx14.cmake`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/README.rst` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/README.rst`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/src/format.cc` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/src/format.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/src/posix.cc` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/src/posix.cc`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/CMakeLists.txt` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/core.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/core.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/ostream.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/ostream.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/ranges.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/ranges.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/compile.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/compile.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/chrono.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/chrono.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/posix.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/posix.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/format-inl.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/format-inl.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/format.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/format.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/safe-duration-cast.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/safe-duration-cast.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/printf.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/printf.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/locale.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/locale.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/include/fmt/color.h` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/include/fmt/color.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/deps/fmt/fmt/LICENSE.rst` & `yaramod-3.9.2/deps/pog/deps/fmt/fmt/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/CMakeLists.txt` & `yaramod-3.9.2/deps/pog/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/state.h` & `yaramod-3.9.2/deps/pog/include/pog/state.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/relations/includes.h` & `yaramod-3.9.2/deps/pog/include/pog/relations/includes.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/relations/relation.h` & `yaramod-3.9.2/deps/pog/include/pog/relations/relation.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/relations/lookback.h` & `yaramod-3.9.2/deps/pog/include/pog/relations/lookback.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/errors.h` & `yaramod-3.9.2/deps/pog/include/pog/errors.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/grammar.h` & `yaramod-3.9.2/deps/pog/include/pog/grammar.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/tokenizer.h` & `yaramod-3.9.2/deps/pog/include/pog/tokenizer.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/token.h` & `yaramod-3.9.2/deps/pog/include/pog/token.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/token_builder.h` & `yaramod-3.9.2/deps/pog/include/pog/token_builder.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/types/state_and_symbol.h` & `yaramod-3.9.2/deps/pog/include/pog/types/state_and_symbol.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/types/state_and_rule.h` & `yaramod-3.9.2/deps/pog/include/pog/types/state_and_rule.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/utils.h` & `yaramod-3.9.2/deps/pog/include/pog/utils.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/operations/lookahead.h` & `yaramod-3.9.2/deps/pog/include/pog/operations/lookahead.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/operations/follow.h` & `yaramod-3.9.2/deps/pog/include/pog/operations/follow.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/operations/operation.h` & `yaramod-3.9.2/deps/pog/include/pog/operations/operation.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/operations/read.h` & `yaramod-3.9.2/deps/pog/include/pog/operations/read.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/filter_view.h` & `yaramod-3.9.2/deps/pog/include/pog/filter_view.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/symbol.h` & `yaramod-3.9.2/deps/pog/include/pog/symbol.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/html_report.h` & `yaramod-3.9.2/deps/pog/include/pog/html_report.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/digraph_algo.h` & `yaramod-3.9.2/deps/pog/include/pog/digraph_algo.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/rule.h` & `yaramod-3.9.2/deps/pog/include/pog/rule.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/precedence.h` & `yaramod-3.9.2/deps/pog/include/pog/precedence.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/parsing_table.h` & `yaramod-3.9.2/deps/pog/include/pog/parsing_table.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/automaton.h` & `yaramod-3.9.2/deps/pog/include/pog/automaton.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/parser_report.h` & `yaramod-3.9.2/deps/pog/include/pog/parser_report.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/parser.h` & `yaramod-3.9.2/deps/pog/include/pog/parser.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/rule_builder.h` & `yaramod-3.9.2/deps/pog/include/pog/rule_builder.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/include/pog/item.h` & `yaramod-3.9.2/deps/pog/include/pog/item.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/LICENSE` & `yaramod-3.9.2/deps/pog/LICENSE`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/README.md` & `yaramod-3.9.2/deps/pog/README.md`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/share/pog-config.cmake.in` & `yaramod-3.9.2/deps/pog/share/pog-config.cmake.in`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pog/CHANGELOG.md` & `yaramod-3.9.2/deps/pog/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/tools/FindEigen3.cmake` & `yaramod-3.9.2/deps/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/tools/pybind11Tools.cmake` & `yaramod-3.9.2/deps/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/tools/FindPythonLibsNew.cmake` & `yaramod-3.9.2/deps/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/tools/FindCatch.cmake` & `yaramod-3.9.2/deps/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/setup.py` & `yaramod-3.9.2/deps/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/CMakeLists.txt` & `yaramod-3.9.2/deps/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/stl_bind.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/embed.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/attr.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/numpy.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/detail/init.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/detail/descr.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/detail/internals.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/detail/class.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/detail/typeid.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/detail/common.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/options.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/stl.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/buffer_info.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/operators.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/functional.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/cast.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/chrono.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/pytypes.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/eval.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/eigen.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/iostream.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/pybind11.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/include/pybind11/complex.h` & `yaramod-3.9.2/deps/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/LICENSE` & `yaramod-3.9.2/deps/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/README.md` & `yaramod-3.9.2/deps/pybind11/README.md`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/pybind11/__main__.py` & `yaramod-3.9.2/deps/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/deps/pybind11/pybind11/__init__.py` & `yaramod-3.9.2/deps/pybind11/pybind11/__init__.py`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/meta.cpp` & `yaramod-3.9.2/src/types/meta.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/plain_string.cpp` & `yaramod-3.9.2/src/types/plain_string.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/hex_string.cpp` & `yaramod-3.9.2/src/types/hex_string.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/token.cpp` & `yaramod-3.9.2/src/types/token.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/yara_file.cpp` & `yaramod-3.9.2/src/types/yara_file.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/rule.cpp` & `yaramod-3.9.2/src/types/rule.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/module.cpp` & `yaramod-3.9.2/src/types/modules/module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/dotnet_module.cpp` & `yaramod-3.9.2/src/types/modules/dotnet_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/magic_module.cpp` & `yaramod-3.9.2/src/types/modules/magic_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/dex_module.cpp` & `yaramod-3.9.2/src/types/modules/dex_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/cuckoo_module.cpp` & `yaramod-3.9.2/src/types/modules/cuckoo_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/elf_module.cpp` & `yaramod-3.9.2/src/types/modules/elf_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/metadata_module.cpp` & `yaramod-3.9.2/src/types/modules/metadata_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/phish_module.cpp` & `yaramod-3.9.2/src/types/modules/phish_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/macho_module.cpp` & `yaramod-3.9.2/src/types/modules/macho_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/time_module.cpp` & `yaramod-3.9.2/src/types/modules/time_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/math_module.cpp` & `yaramod-3.9.2/src/types/modules/math_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/hash_module.cpp` & `yaramod-3.9.2/src/types/modules/hash_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/androguard_module.cpp` & `yaramod-3.9.2/src/types/modules/androguard_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/modules/pe_module.cpp` & `yaramod-3.9.2/src/types/modules/pe_module.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/literal.cpp` & `yaramod-3.9.2/src/types/literal.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/variable.cpp` & `yaramod-3.9.2/src/types/variable.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/types/token_stream.cpp` & `yaramod-3.9.2/src/types/token_stream.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -762,18 +762,14 @@
 			inside_regexp = true;
 		else if (current == TokenType::REGEXP_END_SLASH)
 			inside_regexp = false;
 		else if (current == TokenType::LP_ENUMERATION)
 			inside_enumeration_brackets = true;
 		else if (current == TokenType::RP_ENUMERATION)
 			inside_enumeration_brackets = false;
-		else if (current == TokenType::LSQB_ENUMERATION)
-			inside_enumeration_brackets = true;
-		else if (current == TokenType::RSQB_ENUMERATION)
-			inside_enumeration_brackets = false;
 		else if (it->isStringModifier())
 			inside_string_modifiers = true;
 
 		if (inside_string_modifiers)
 		{
 			if (next == TokenType::LP)
 				inside_string_modifiers_arguments = true;
```

### Comparing `yaramod-3.9.1/src/utils/filesystem.cpp` & `yaramod-3.9.2/src/utils/filesystem.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/utils/utils.cpp` & `yaramod-3.9.2/src/utils/utils.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/parser/parser_driver.cpp` & `yaramod-3.9.2/src/parser/parser_driver.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1829,15 +1829,15 @@
 	if (_features & Features::AvastOnly)
 	{
 		_parser.rule("expression_iterable") // shared_ptr<IterableExpression>
 			.production("LSQB", "expression_enumeration", "RSQB", [&](auto&& args) -> Value {
 				TokenIt lsqb = args[0].getTokenIt();
 				lsqb->setType(TokenType::LSQB_ENUMERATION);
 				TokenIt rsqb = args[2].getTokenIt();
-				lsqb->setType(TokenType::RSQB_ENUMERATION);
+				rsqb->setType(TokenType::RSQB_ENUMERATION);
 				auto output = std::make_shared<IterableExpression>(lsqb, std::move(args[1].getMultipleExpressions()), rsqb);
 				output->setTokenStream(currentTokenStream());
 				return output;
 			})
 			;
 
 		_parser.rule("expression_enumeration") // vector<Expression::Ptr>
```

### Comparing `yaramod-3.9.1/src/python/CMakeLists.txt` & `yaramod-3.9.2/src/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/python/yaramod_python.cpp` & `yaramod-3.9.2/src/python/yaramod_python.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/python/py_visitor.cpp` & `yaramod-3.9.2/src/python/py_visitor.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/python/py_visitor.h` & `yaramod-3.9.2/src/python/py_visitor.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/python/yaramod_python.h` & `yaramod-3.9.2/src/python/yaramod_python.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/builder/yara_hex_string_builder.cpp` & `yaramod-3.9.2/src/builder/yara_hex_string_builder.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/builder/yara_file_builder.cpp` & `yaramod-3.9.2/src/builder/yara_file_builder.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/builder/yara_rule_builder.cpp` & `yaramod-3.9.2/src/builder/yara_rule_builder.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/builder/yara_expression_builder.cpp` & `yaramod-3.9.2/src/builder/yara_expression_builder.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/yaramod.cpp` & `yaramod-3.9.2/src/yaramod.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/CMakeLists.txt` & `yaramod-3.9.2/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/examples/python/dump_rules_ast.py` & `yaramod-3.9.2/src/examples/python/dump_rules_ast.py`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/examples/python/simplify_bools.py` & `yaramod-3.9.2/src/examples/python/simplify_bools.py`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/examples/cpp/simplify_bools/bool_simplifier.h` & `yaramod-3.9.2/src/examples/cpp/simplify_bools/bool_simplifier.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/examples/cpp/simplify_bools/main.cpp` & `yaramod-3.9.2/src/examples/cpp/simplify_bools/main.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/examples/cpp/dump_rules_ast/dumper.h` & `yaramod-3.9.2/src/examples/cpp/dump_rules_ast/dumper.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/src/examples/cpp/dump_rules_ast/main.cpp` & `yaramod-3.9.2/src/examples/cpp/dump_rules_ast/main.cpp`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/CMakeLists.txt` & `yaramod-3.9.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/yaramod_error.h` & `yaramod-3.9.2/include/yaramod/yaramod_error.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/token.h` & `yaramod-3.9.2/include/yaramod/types/token.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/token_type.h` & `yaramod-3.9.2/include/yaramod/types/token_type.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/hex_string.h` & `yaramod-3.9.2/include/yaramod/types/hex_string.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/symbols.h` & `yaramod-3.9.2/include/yaramod/types/symbols.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/symbol.h` & `yaramod-3.9.2/include/yaramod/types/symbol.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/rule.h` & `yaramod-3.9.2/include/yaramod/types/rule.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/regexp.h` & `yaramod-3.9.2/include/yaramod/types/regexp.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/expression.h` & `yaramod-3.9.2/include/yaramod/types/expression.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/yara_file.h` & `yaramod-3.9.2/include/yaramod/types/yara_file.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/string_modifier.h` & `yaramod-3.9.2/include/yaramod/types/string_modifier.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/time_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/time_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/modules_pool.h` & `yaramod-3.9.2/include/yaramod/types/modules/modules_pool.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/phish_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/phish_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/module.h` & `yaramod-3.9.2/include/yaramod/types/modules/module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/dex_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/dex_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/cuckoo_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/cuckoo_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/math_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/math_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/modules.h` & `yaramod-3.9.2/include/yaramod/types/modules/modules.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/metadata_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/metadata_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/elf_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/elf_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/macho_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/macho_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/magic_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/magic_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/pe_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/pe_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/androguard_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/androguard_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/dotnet_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/dotnet_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/modules/hash_module.h` & `yaramod-3.9.2/include/yaramod/types/modules/hash_module.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/meta.h` & `yaramod-3.9.2/include/yaramod/types/meta.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/plain_string.h` & `yaramod-3.9.2/include/yaramod/types/plain_string.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/literal.h` & `yaramod-3.9.2/include/yaramod/types/literal.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/string.h` & `yaramod-3.9.2/include/yaramod/types/string.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/variable.h` & `yaramod-3.9.2/include/yaramod/types/variable.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/token_stream.h` & `yaramod-3.9.2/include/yaramod/types/token_stream.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/types/expressions.h` & `yaramod-3.9.2/include/yaramod/types/expressions.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/utils/visitor.h` & `yaramod-3.9.2/include/yaramod/utils/visitor.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/utils/utils.h` & `yaramod-3.9.2/include/yaramod/utils/utils.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/utils/trie.h` & `yaramod-3.9.2/include/yaramod/utils/trie.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/utils/visitor_result.h` & `yaramod-3.9.2/include/yaramod/utils/visitor_result.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/utils/modifying_visitor.h` & `yaramod-3.9.2/include/yaramod/utils/modifying_visitor.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/utils/observing_visitor.h` & `yaramod-3.9.2/include/yaramod/utils/observing_visitor.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/parser/parser_driver.h` & `yaramod-3.9.2/include/yaramod/parser/parser_driver.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/parser/file_context.h` & `yaramod-3.9.2/include/yaramod/parser/file_context.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/parser/location.h` & `yaramod-3.9.2/include/yaramod/parser/location.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/parser/value.h` & `yaramod-3.9.2/include/yaramod/parser/value.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/yaramod.h` & `yaramod-3.9.2/include/yaramod/yaramod.h`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #pragma once
 
 #define STR_HELPER(x) #x
 #define STR(x) STR_HELPER(x)
 
 #define YARAMOD_VERSION_MAJOR 3
 #define YARAMOD_VERSION_MINOR 9
-#define YARAMOD_VERSION_PATCH 1
+#define YARAMOD_VERSION_PATCH 2
 #define YARAMOD_VERSION_ADDEND ""
 
 #define YARAMOD_VERSION STR(YARAMOD_VERSION_MAJOR) "." STR(YARAMOD_VERSION_MINOR) "." STR(YARAMOD_VERSION_PATCH) YARAMOD_VERSION_ADDEND
 
 #define YARA_SYNTAX_VERSION "4.0"
 
 #include <memory>
```

### Comparing `yaramod-3.9.1/include/yaramod/builder/yara_file_builder.h` & `yaramod-3.9.2/include/yaramod/builder/yara_file_builder.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/builder/yara_rule_builder.h` & `yaramod-3.9.2/include/yaramod/builder/yara_rule_builder.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/builder/yara_expression_builder.h` & `yaramod-3.9.2/include/yaramod/builder/yara_expression_builder.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/include/yaramod/builder/yara_hex_string_builder.h` & `yaramod-3.9.2/include/yaramod/builder/yara_hex_string_builder.h`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/yaramod.egg-info/SOURCES.txt` & `yaramod-3.9.2/yaramod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/LICENSE` & `yaramod-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/README.md` & `yaramod-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/LICENSE-THIRD-PARTY` & `yaramod-3.9.2/LICENSE-THIRD-PARTY`

 * *Files identical despite different names*

### Comparing `yaramod-3.9.1/CHANGELOG.md` & `yaramod-3.9.2/CHANGELOG.md`

 * *Files identical despite different names*

