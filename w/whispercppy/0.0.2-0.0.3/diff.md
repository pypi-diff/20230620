# Comparing `tmp/whispercppy-0.0.2.tar.gz` & `tmp/whispercppy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whispercppy-0.0.2.tar", last modified: Mon Apr 24 22:16:40 2023, max compression
+gzip compressed data, was "whispercppy-0.0.3.tar", last modified: Tue Jun 20 12:20:23 2023, max compression
```

## Comparing `whispercppy-0.0.2.tar` & `whispercppy-0.0.3.tar`

### file list

```diff
@@ -1,350 +1,353 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.470872 whispercppy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 22:16:31.000000 whispercppy-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 22:16:31.000000 whispercppy-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 22:16:40.470872 whispercppy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-24 22:16:31.000000 whispercppy-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.422870 whispercppy-0.0.2/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.442870 whispercppy-0.0.2/external/whisper.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-24 22:16:31.000000 whispercppy-0.0.2/external/whisper.cpp/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.422870 whispercppy-0.0.2/external/whisper.cpp/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.442870 whispercppy-0.0.2/external/whisper.cpp/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/.github/workflows/bindings-go.yml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/.github/workflows/bindings-ruby.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/.github/workflows/examples.yml
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    27042 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.442870 whispercppy-0.0.2/external/whisper.cpp/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.442870 whispercppy-0.0.2/external/whisper.cpp/bindings/go/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/doc.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.422870 whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.446871 whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-model-download/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-model-download/context.go
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-model-download/main.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.446871 whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-whisper/color.go
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-whisper/flags.go
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-whisper/main.go
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-whisper/process.go
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/go.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/go.sum
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/params.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.422870 whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.446871 whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/consts.go
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/context.go
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/context_test.go
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/doc.go
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/interface.go
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/model.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.446871 whispercppy-0.0.2/external/whisper.cpp/bindings/go/samples/
--rw-r--r--   0 runner    (1001) docker     (123)   352078 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/samples/jfk.wav
--rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/whisper.go
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/go/whisper_test.go
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.446871 whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/libwhisper.worker.js
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/package-tmpl.json
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/package.json
--rw-r--r--   0 runner    (1001) docker     (123)   744738 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/whisper.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.422870 whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.446871 whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/ext/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/ext/extconf.rb
--rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/ext/ruby_whisper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.450871 whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/tests/test_whisper.rb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.450871 whispercppy-0.0.2/external/whisper.cpp/cmake/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/cmake/BuildTypes.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/cmake/DefaultTargetOptions.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/cmake/GitVars.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.450871 whispercppy-0.0.2/external/whisper.cpp/coreml/
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-decoder-impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-decoder-impl.m
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-encoder-impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-encoder-impl.m
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-encoder.h
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-encoder.mm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.450871 whispercppy-0.0.2/external/whisper.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.450871 whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.450871 whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/__test__/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/__test__/whisper.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/addon.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.450871 whispercppy-0.0.2/external/whisper.cpp/examples/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/bench/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/bench/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/bench/bench.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.454871 whispercppy-0.0.2/external/whisper.cpp/examples/bench.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/bench.wasm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/bench.wasm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/bench.wasm/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/bench.wasm/index-tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.454871 whispercppy-0.0.2/external/whisper.cpp/examples/command/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/command/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/command/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    25615 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/command/command.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/command/commands.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.454871 whispercppy-0.0.2/external/whisper.cpp/examples/command.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/command.wasm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/command.wasm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/command.wasm/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/command.wasm/index-tmpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/common-sdl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/common-sdl.h
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/common.h
--rw-r--r--   0 runner    (1001) docker     (123)   241358 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/dr_wav.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/generate-karaoke.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/helpers.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     2955 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/livestream.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.454871 whispercppy-0.0.2/external/whisper.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/main/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/main/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    35726 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/main/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.454871 whispercppy-0.0.2/external/whisper.cpp/examples/stream/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/stream/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/stream/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/stream/stream.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.454871 whispercppy-0.0.2/external/whisper.cpp/examples/stream.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/stream.wasm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/stream.wasm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/stream.wasm/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/stream.wasm/index-tmpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.454871 whispercppy-0.0.2/external/whisper.cpp/examples/talk/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk/eleven-labs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30715 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk/gpt-2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk/gpt-2.h
--rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk/speak.sh
--rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk/talk.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/eleven-labs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64204 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/llama.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/llama.h
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/llama_internal.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    11029 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/llama_util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/speak.sh
--rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/talk-llama.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30900 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/gpt-2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/gpt-2.h
--rw-r--r--   0 runner    (1001) docker     (123)    31661 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/index-tmpl.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     2757 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/twitch.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/.idea/compiler.xml
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/.idea/gradle.xml
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/build.gradle
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/proguard-rules.pro
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.430870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.426870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/androidTest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.426870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/androidTest/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.426870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.426870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.426870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.430870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt
--rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Color.kt
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.458871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.430870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/jni/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Application.mk
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.430870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/ic_launcher.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/values/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/values/colors.xml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/values/strings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/values/themes.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/xml/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/xml/backup_rules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.430870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.430870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/test/java/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.430870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/test/java/com/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/ExampleUnitTest.kt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/build.gradle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.430870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradle/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradle/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)    59203 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.properties
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradle.properties
--rwxr-xr-x   0 runner    (1001) docker     (123)     5766 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradlew
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradlew.bat
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/settings.gradle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.nvim/
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.nvim/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.nvim/whisper.nvim
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.h
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard
--rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.h
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/main.m
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/WhisperCppDemo-Bridging-Header.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.434870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.462871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AccentColor.colorset/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AccentColor.colorset/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/Contents.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.434870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Preview Content/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Preview Content/Preview Assets.xcassets/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Preview Content/Preview Assets.xcassets/Contents.json
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/WhisperCppDemo.entitlements
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/RiffWaveUtils.swift
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/WhisperCppDemoApp.swift
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.434870 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.wasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.wasm/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.wasm/emscripten.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26310 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/whisper.wasm/index-tmpl.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     6932 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/examples/yt-wsp.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/extra/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/extra/bench-all.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/extra/bench-wts.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      297 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/extra/convert-all.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/extra/deploy-wasm.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/extra/sha-all.sh
--rw-r--r--   0 runner    (1001) docker     (123)   352108 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/ggml.c
--rw-r--r--   0 runner    (1001) docker     (123)    24659 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/ggml.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/samples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/samples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   352078 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/samples/jfk.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.466871 whispercppy-0.0.2/external/whisper.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/tests/en-0-ref.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/tests/en-1-ref.txt
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/tests/en-2-ref.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/tests/es-0-ref.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     3346 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/tests/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/tests/test-whisper.js
--rw-r--r--   0 runner    (1001) docker     (123)   178962 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/whisper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23720 2023-04-24 22:16:32.000000 whispercppy-0.0.2/external/whisper.cpp/whisper.h
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-24 22:16:31.000000 whispercppy-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:16:40.470872 whispercppy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-24 22:16:31.000000 whispercppy-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.470872 whispercppy-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-04-24 22:16:31.000000 whispercppy-0.0.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-24 22:16:31.000000 whispercppy-0.0.2/src/api_cpp2py_export.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-24 22:16:31.000000 whispercppy-0.0.2/src/api_cpp2py_export.h
--rw-r--r--   0 runner    (1001) docker     (123)    24117 2023-04-24 22:16:31.000000 whispercppy-0.0.2/src/context.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-04-24 22:16:31.000000 whispercppy-0.0.2/src/context.h
--rw-r--r--   0 runner    (1001) docker     (123)    32113 2023-04-24 22:16:31.000000 whispercppy-0.0.2/src/params.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-24 22:16:31.000000 whispercppy-0.0.2/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.470872 whispercppy-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-24 22:16:31.000000 whispercppy-0.0.2/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:16:40.470872 whispercppy-0.0.2/whispercppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 22:16:40.000000 whispercppy-0.0.2/whispercppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-04-24 22:16:40.000000 whispercppy-0.0.2/whispercppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:16:40.000000 whispercppy-0.0.2/whispercppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-24 22:16:40.000000 whispercppy-0.0.2/whispercppy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.281940 whispercppy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 12:20:14.000000 whispercppy-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 12:20:14.000000 whispercppy-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-20 12:20:23.281940 whispercppy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-20 12:20:14.000000 whispercppy-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.245939 whispercppy-0.0.3/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.253939 whispercppy-0.0.3/external/whisper.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 12:20:14.000000 whispercppy-0.0.3/external/whisper.cpp/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.245939 whispercppy-0.0.3/external/whisper.cpp/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.253939 whispercppy-0.0.3/external/whisper.cpp/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/.github/workflows/bindings-go.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/.github/workflows/bindings-ruby.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/.github/workflows/examples.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    27042 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.253939 whispercppy-0.0.3/external/whisper.cpp/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.257940 whispercppy-0.0.3/external/whisper.cpp/bindings/go/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/doc.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.245939 whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.257940 whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-model-download/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-model-download/context.go
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-model-download/main.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.257940 whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-whisper/color.go
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-whisper/flags.go
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-whisper/main.go
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-whisper/process.go
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/go.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/go.sum
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/params.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.245939 whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.257940 whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/consts.go
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/context.go
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/context_test.go
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/doc.go
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/interface.go
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/model.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.257940 whispercppy-0.0.3/external/whisper.cpp/bindings/go/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)   352078 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/samples/jfk.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    14538 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/whisper.go
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/go/whisper_test.go
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.257940 whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/libwhisper.worker.js
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/package-tmpl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)   744738 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/whisper.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.245939 whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.261940 whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/ext/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/ext/extconf.rb
+-rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/ext/ruby_whisper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.261940 whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/tests/test_whisper.rb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.261940 whispercppy-0.0.3/external/whisper.cpp/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/cmake/BuildTypes.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/cmake/DefaultTargetOptions.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/cmake/GitVars.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.261940 whispercppy-0.0.3/external/whisper.cpp/coreml/
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-decoder-impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-decoder-impl.m
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-encoder-impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-encoder-impl.m
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-encoder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-encoder.mm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.261940 whispercppy-0.0.3/external/whisper.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.261940 whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.261940 whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/__test__/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/__test__/whisper.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/addon.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.261940 whispercppy-0.0.3/external/whisper.cpp/examples/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/bench/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/bench/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/bench/bench.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.265940 whispercppy-0.0.3/external/whisper.cpp/examples/bench.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/bench.wasm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/bench.wasm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/bench.wasm/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/bench.wasm/index-tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.265940 whispercppy-0.0.3/external/whisper.cpp/examples/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/command/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/command/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    25615 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/command/command.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/command/commands.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.265940 whispercppy-0.0.3/external/whisper.cpp/examples/command.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/command.wasm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/command.wasm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/command.wasm/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/command.wasm/index-tmpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/common-sdl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/common-sdl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)   241358 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/dr_wav.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1197 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/generate-karaoke.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/helpers.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2955 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/livestream.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.265940 whispercppy-0.0.3/external/whisper.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/main/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/main/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35726 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/main/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.265940 whispercppy-0.0.3/external/whisper.cpp/examples/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/stream/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/stream/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/stream/stream.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.265940 whispercppy-0.0.3/external/whisper.cpp/examples/stream.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/stream.wasm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/stream.wasm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/stream.wasm/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/stream.wasm/index-tmpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.265940 whispercppy-0.0.3/external/whisper.cpp/examples/talk/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk/eleven-labs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30715 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk/gpt-2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk/gpt-2.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)      563 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk/speak.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk/talk.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/eleven-labs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64204 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/llama.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/llama.h
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/llama_internal.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11029 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/llama_util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/speak.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    21631 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/talk-llama.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30900 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/gpt-2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/gpt-2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31661 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/index-tmpl.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2757 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/twitch.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/.idea/compiler.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/.idea/gradle.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/build.gradle
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/proguard-rules.pro
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.245939 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/androidTest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.245939 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/androidTest/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.245939 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.269940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Color.kt
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/jni/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Application.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/mipmap-anydpi/ic_launcher.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/values/colors.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/values/strings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/values/themes.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/xml/backup_rules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/test/java/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/test/java/com/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/test/java/com/whispercppdemo/ExampleUnitTest.kt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/build.gradle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradle/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradle/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)    59203 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.properties
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradle.properties
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5766 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradlew
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradlew.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/settings.gradle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.nvim/
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.nvim/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.nvim/whisper.nvim
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AccentColor.colorset/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Assets.xcassets/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard
+-rw-r--r--   0 runner    (1001) docker     (123)     8419 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/main.m
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (123)    17120 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.273940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/WhisperCppDemo-Bridging-Header.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/models/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Resources/samples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AccentColor.colorset/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AccentColor.colorset/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/Contents.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Preview Content/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Preview Content/Preview Assets.xcassets/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Preview Content/Preview Assets.xcassets/Contents.json
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/WhisperCppDemo.entitlements
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/RiffWaveUtils.swift
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/WhisperCppDemoApp.swift
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    21447 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.249940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.wasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.wasm/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.wasm/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.wasm/emscripten.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26310 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/whisper.wasm/index-tmpl.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6932 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/examples/yt-wsp.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/extra/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1935 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/extra/bench-all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/extra/bench-wts.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      297 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/extra/convert-all.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1152 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/extra/deploy-wasm.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/extra/sha-all.sh
+-rw-r--r--   0 runner    (1001) docker     (123)   352108 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/ggml.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24659 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/ggml.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.277940 whispercppy-0.0.3/external/whisper.cpp/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/samples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/samples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   352078 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/samples/jfk.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.281940 whispercppy-0.0.3/external/whisper.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/tests/en-0-ref.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/tests/en-1-ref.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/tests/en-2-ref.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/tests/es-0-ref.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3346 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/tests/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/tests/test-whisper.js
+-rw-r--r--   0 runner    (1001) docker     (123)   178962 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/whisper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23720 2023-06-20 12:20:15.000000 whispercppy-0.0.3/external/whisper.cpp/whisper.h
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-20 12:20:14.000000 whispercppy-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:20:23.281940 whispercppy-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-20 12:20:14.000000 whispercppy-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.281940 whispercppy-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-20 12:20:14.000000 whispercppy-0.0.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-20 12:20:14.000000 whispercppy-0.0.3/src/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-06-20 12:20:14.000000 whispercppy-0.0.3/src/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-20 12:20:14.000000 whispercppy-0.0.3/src/api_cpp2py_export.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-20 12:20:14.000000 whispercppy-0.0.3/src/api_cpp2py_export.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24117 2023-06-20 12:20:14.000000 whispercppy-0.0.3/src/context.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-06-20 12:20:14.000000 whispercppy-0.0.3/src/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32113 2023-06-20 12:20:14.000000 whispercppy-0.0.3/src/params.cc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:14.000000 whispercppy-0.0.3/src/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-20 12:20:14.000000 whispercppy-0.0.3/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.281940 whispercppy-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 12:20:14.000000 whispercppy-0.0.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:20:23.281940 whispercppy-0.0.3/whispercppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-20 12:20:23.000000 whispercppy-0.0.3/whispercppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-06-20 12:20:23.000000 whispercppy-0.0.3/whispercppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:20:23.000000 whispercppy-0.0.3/whispercppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 12:20:23.000000 whispercppy-0.0.3/whispercppy.egg-info/top_level.txt
```

### Comparing `whispercppy-0.0.2/LICENSE` & `whispercppy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/.github/workflows/build.yml` & `whispercppy-0.0.3/external/whisper.cpp/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/.github/workflows/examples.yml` & `whispercppy-0.0.3/external/whisper.cpp/.github/workflows/examples.yml`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/.gitignore` & `whispercppy-0.0.3/external/whisper.cpp/.gitignore`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/LICENSE` & `whispercppy-0.0.3/external/whisper.cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/Makefile` & `whispercppy-0.0.3/external/whisper.cpp/Makefile`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/README.md` & `whispercppy-0.0.3/external/whisper.cpp/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/LICENSE` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/LICENSE`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/Makefile` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/Makefile`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/README.md` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-model-download/context.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-model-download/context.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-model-download/main.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-model-download/main.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-whisper/color.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-whisper/color.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-whisper/flags.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-whisper/flags.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-whisper/main.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-whisper/main.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/examples/go-whisper/process.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/examples/go-whisper/process.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/go.sum` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/go.sum`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/params.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/params.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/consts.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/consts.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/context.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/context.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/context_test.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/context_test.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/interface.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/interface.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/pkg/whisper/model.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/pkg/whisper/model.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/samples/jfk.wav` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/samples/jfk.wav`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/whisper.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/whisper.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/go/whisper_test.go` & `whispercppy-0.0.3/external/whisper.cpp/bindings/go/whisper_test.go`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/README.md` & `whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/emscripten.cpp` & `whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/libwhisper.worker.js` & `whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/libwhisper.worker.js`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/package-tmpl.json` & `whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/package-tmpl.json`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/package.json` & `whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/package.json`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/javascript/whisper.js` & `whispercppy-0.0.3/external/whisper.cpp/bindings/javascript/whisper.js`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/ext/extconf.rb` & `whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/ext/extconf.rb`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp` & `whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/ext/ruby_whisper.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/bindings/ruby/tests/test_whisper.rb` & `whispercppy-0.0.3/external/whisper.cpp/bindings/ruby/tests/test_whisper.rb`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/cmake/BuildTypes.cmake` & `whispercppy-0.0.3/external/whisper.cpp/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/cmake/GitVars.cmake` & `whispercppy-0.0.3/external/whisper.cpp/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-decoder-impl.h` & `whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-decoder-impl.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-decoder-impl.m` & `whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-decoder-impl.m`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-encoder-impl.h` & `whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-encoder-impl.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-encoder-impl.m` & `whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-encoder-impl.m`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-encoder.h` & `whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-encoder.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/coreml/whisper-encoder.mm` & `whispercppy-0.0.3/external/whisper.cpp/coreml/whisper-encoder.mm`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/__test__/whisper.spec.js` & `whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/__test__/whisper.spec.js`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/addon.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/addon.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/addon.node/index.js` & `whispercppy-0.0.3/external/whisper.cpp/examples/addon.node/index.js`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/bench/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/bench/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/bench/bench.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/bench/bench.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/bench.wasm/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/examples/bench.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/bench.wasm/emscripten.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/bench.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/bench.wasm/index-tmpl.html` & `whispercppy-0.0.3/external/whisper.cpp/examples/bench.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/command/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/command/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/command/command.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/command/command.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/command.wasm/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/examples/command.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/command.wasm/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/command.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/command.wasm/emscripten.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/command.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/command.wasm/index-tmpl.html` & `whispercppy-0.0.3/external/whisper.cpp/examples/command.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/common-sdl.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/common-sdl.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/common-sdl.h` & `whispercppy-0.0.3/external/whisper.cpp/examples/common-sdl.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/common.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/common.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/common.h` & `whispercppy-0.0.3/external/whisper.cpp/examples/common.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/dr_wav.h` & `whispercppy-0.0.3/external/whisper.cpp/examples/dr_wav.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/generate-karaoke.sh` & `whispercppy-0.0.3/external/whisper.cpp/examples/generate-karaoke.sh`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/helpers.js` & `whispercppy-0.0.3/external/whisper.cpp/examples/helpers.js`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/livestream.sh` & `whispercppy-0.0.3/external/whisper.cpp/examples/livestream.sh`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/main/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/main/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/main/main.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/main/main.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/stream/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/stream/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/stream/stream.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/stream/stream.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/stream.wasm/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/examples/stream.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/stream.wasm/emscripten.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/stream.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/stream.wasm/index-tmpl.html` & `whispercppy-0.0.3/external/whisper.cpp/examples/stream.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk/eleven-labs.py` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk/eleven-labs.py`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk/gpt-2.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk/gpt-2.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk/gpt-2.h` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk/gpt-2.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk/speak.sh` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk/speak.sh`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk/talk.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk/talk.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/eleven-labs.py` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/eleven-labs.py`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/llama.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/llama.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/llama.h` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/llama.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/llama_util.h` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/llama_util.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/prompts/talk-alpaca.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/speak.sh` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/speak.sh`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk-llama/talk-llama.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk-llama/talk-llama.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/emscripten.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/gpt-2.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/gpt-2.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/gpt-2.h` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/gpt-2.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/talk.wasm/index-tmpl.html` & `whispercppy-0.0.3/external/whisper.cpp/examples/talk.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/twitch.sh` & `whispercppy-0.0.3/external/whisper.cpp/examples/twitch.sh`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/.idea/gradle.xml` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/.idea/gradle.xml`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/build.gradle` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/build.gradle`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/proguard-rules.pro` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/proguard-rules.pro`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/androidTest/java/com/whispercppdemo/ExampleInstrumentedTest.kt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/AndroidManifest.xml`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/MainActivity.kt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/media/RiffWaveHelper.kt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/recorder/Recorder.kt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreen.kt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/main/MainScreenViewModel.kt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Theme.kt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/ui/theme/Type.kt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/java/com/whispercppdemo/whisper/LibWhisper.kt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Android.mk`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/Whisper.mk`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/jni/whisper/jni.c`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_background.xml`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/drawable/ic_launcher_foreground.xml`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/app/src/main/res/xml/data_extraction_rules.xml`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradle/wrapper/gradle-wrapper.jar`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradle.properties` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradle.properties`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradlew` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradlew`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.android/gradlew.bat` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.android/gradlew.bat`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.nvim/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.nvim/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.nvim/whisper.nvim` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.nvim/whisper.nvim`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/AppDelegate.m`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/LaunchScreen.storyboard`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Base.lproj/Main.storyboard`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/Info.plist`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/SceneDelegate.m`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc/ViewController.m`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.objc/whisper.objc.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.cpp.swift/LibWhisper.swift`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Models/WhisperState.swift`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/Contents.json` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Supporting files/Assets.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/UI/ContentView.swift`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.demo/Utils/Recorder.swift`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.swiftui/whisper.swiftui.xcodeproj/xcshareddata/xcschemes/WhisperCppDemo.xcscheme`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.wasm/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.wasm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.wasm/README.md` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.wasm/README.md`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.wasm/emscripten.cpp` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.wasm/emscripten.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/whisper.wasm/index-tmpl.html` & `whispercppy-0.0.3/external/whisper.cpp/examples/whisper.wasm/index-tmpl.html`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/examples/yt-wsp.sh` & `whispercppy-0.0.3/external/whisper.cpp/examples/yt-wsp.sh`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/extra/bench-all.sh` & `whispercppy-0.0.3/external/whisper.cpp/extra/bench-all.sh`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/extra/bench-wts.sh` & `whispercppy-0.0.3/external/whisper.cpp/extra/bench-wts.sh`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/extra/deploy-wasm.sh` & `whispercppy-0.0.3/external/whisper.cpp/extra/deploy-wasm.sh`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/ggml.c` & `whispercppy-0.0.3/external/whisper.cpp/ggml.c`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/ggml.h` & `whispercppy-0.0.3/external/whisper.cpp/ggml.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/samples/jfk.wav` & `whispercppy-0.0.3/external/whisper.cpp/samples/jfk.wav`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/tests/CMakeLists.txt` & `whispercppy-0.0.3/external/whisper.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/tests/en-0-ref.txt` & `whispercppy-0.0.3/external/whisper.cpp/tests/en-0-ref.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/tests/en-1-ref.txt` & `whispercppy-0.0.3/external/whisper.cpp/tests/en-1-ref.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/tests/en-2-ref.txt` & `whispercppy-0.0.3/external/whisper.cpp/tests/en-2-ref.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/tests/es-0-ref.txt` & `whispercppy-0.0.3/external/whisper.cpp/tests/es-0-ref.txt`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/tests/run-tests.sh` & `whispercppy-0.0.3/external/whisper.cpp/tests/run-tests.sh`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/tests/test-whisper.js` & `whispercppy-0.0.3/external/whisper.cpp/tests/test-whisper.js`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/whisper.cpp` & `whispercppy-0.0.3/external/whisper.cpp/whisper.cpp`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/external/whisper.cpp/whisper.h` & `whispercppy-0.0.3/external/whisper.cpp/whisper.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/setup.py` & `whispercppy-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from pybind11.setup_helpers import Pybind11Extension
 from pybind11.setup_helpers import build_ext as _build_ext
 from setuptools import Extension, setup
 
 WHISPER_ENABLE_COREML = False
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 
 class CopyWhisperDummyExtension(Extension):
     pass
 
 
 class build_ext(_build_ext):
```

### Comparing `whispercppy-0.0.2/src/__init__.py` & `whispercppy-0.0.3/src/__init__.py`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/src/api_cpp2py_export.cc` & `whispercppy-0.0.3/src/api_cpp2py_export.cc`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/src/api_cpp2py_export.h` & `whispercppy-0.0.3/src/api_cpp2py_export.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/src/context.cc` & `whispercppy-0.0.3/src/context.cc`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/src/context.h` & `whispercppy-0.0.3/src/context.h`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/src/params.cc` & `whispercppy-0.0.3/src/params.cc`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/src/utils.py` & `whispercppy-0.0.3/src/utils.py`

 * *Files identical despite different names*

### Comparing `whispercppy-0.0.2/whispercppy.egg-info/SOURCES.txt` & `whispercppy-0.0.3/whispercppy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -230,18 +230,21 @@
 external/whisper.cpp/tests/en-0-ref.txt
 external/whisper.cpp/tests/en-1-ref.txt
 external/whisper.cpp/tests/en-2-ref.txt
 external/whisper.cpp/tests/es-0-ref.txt
 external/whisper.cpp/tests/run-tests.sh
 external/whisper.cpp/tests/test-whisper.js
 src/__init__.py
+src/__init__.pyi
+src/api.pyi
 src/api_cpp2py_export.cc
 src/api_cpp2py_export.h
 src/context.cc
 src/context.h
 src/params.cc
+src/py.typed
 src/utils.py
 tests/test.py
 whispercppy.egg-info/PKG-INFO
 whispercppy.egg-info/SOURCES.txt
 whispercppy.egg-info/dependency_links.txt
 whispercppy.egg-info/top_level.txt
```

