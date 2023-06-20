# Comparing `tmp/pyccel-1.7.4.tar.gz` & `tmp/pyccel-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyccel-1.7.4.tar", last modified: Tue May  2 21:46:47 2023, max compression
+gzip compressed data, was "pyccel-1.8.0.tar", last modified: Tue Jun 20 10:09:40 2023, max compression
```

## Comparing `pyccel-1.7.4.tar` & `pyccel-1.8.0.tar`

### file list

```diff
@@ -1,726 +1,730 @@
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.194131 pyccel-1.7.4/
--rw-r--r--   0 yaman      (501) staff       (20)      451 2023-05-02 21:45:18.000000 pyccel-1.7.4/AUTHORS
--rw-r--r--   0 yaman      (501) staff       (20)     1081 2023-05-02 21:45:18.000000 pyccel-1.7.4/LICENSE
--rw-r--r--   0 yaman      (501) staff       (20)      293 2023-05-02 21:45:18.000000 pyccel-1.7.4/MANIFEST.in
--rw-r--r--   0 yaman      (501) staff       (20)    13504 2023-05-02 21:46:47.194320 pyccel-1.7.4/PKG-INFO
--rw-r--r--   0 yaman      (501) staff       (20)    13180 2023-05-02 21:45:18.000000 pyccel-1.7.4/README.md
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.813501 pyccel-1.7.4/pyccel/
--rw-r--r--   0 yaman      (501) staff       (20)       33 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.831474 pyccel-1.7.4/pyccel/ast/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    15604 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)    13461 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/bind_c.py
--rw-r--r--   0 yaman      (501) staff       (20)     7686 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/bitwise_operators.py
--rw-r--r--   0 yaman      (501) staff       (20)     3400 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/builtin_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)    29378 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/builtins.py
--rw-r--r--   0 yaman      (501) staff       (20)     6502 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/c_concepts.py
--rw-r--r--   0 yaman      (501) staff       (20)     6460 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/class_defs.py
--rw-r--r--   0 yaman      (501) staff       (20)   126977 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/core.py
--rw-r--r--   0 yaman      (501) staff       (20)    20054 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/cwrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)    10493 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/datatypes.py
--rw-r--r--   0 yaman      (501) staff       (20)     3715 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/functionalexpr.py
--rw-r--r--   0 yaman      (501) staff       (20)    29329 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/headers.py
--rw-r--r--   0 yaman      (501) staff       (20)     9428 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/internals.py
--rw-r--r--   0 yaman      (501) staff       (20)     2062 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/itertoolsext.py
--rw-r--r--   0 yaman      (501) staff       (20)    10766 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/literals.py
--rw-r--r--   0 yaman      (501) staff       (20)     3564 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/macros.py
--rw-r--r--   0 yaman      (501) staff       (20)    10805 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/mathext.py
--rw-r--r--   0 yaman      (501) staff       (20)    14034 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/numpy_wrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)    62314 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/numpyext.py
--rw-r--r--   0 yaman      (501) staff       (20)     7113 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/omp.py
--rw-r--r--   0 yaman      (501) staff       (20)    35482 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/operators.py
--rw-r--r--   0 yaman      (501) staff       (20)      869 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/scipyext.py
--rw-r--r--   0 yaman      (501) staff       (20)     7346 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/sympy_helper.py
--rw-r--r--   0 yaman      (501) staff       (20)     1630 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/sysext.py
--rw-r--r--   0 yaman      (501) staff       (20)    30831 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/utilities.py
--rw-r--r--   0 yaman      (501) staff       (20)    28982 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/ast/variable.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.834125 pyccel-1.7.4/pyccel/codegen/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     6587 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.835598 pyccel-1.7.4/pyccel/codegen/compiling/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/compiling/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     9200 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/compiling/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)    16711 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/compiling/compilers.py
--rw-r--r--   0 yaman      (501) staff       (20)    16095 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/pipeline.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.843133 pyccel-1.7.4/pyccel/codegen/printing/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    85613 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/ccode.py
--rw-r--r--   0 yaman      (501) staff       (20)     4722 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/codeprinter.py
--rw-r--r--   0 yaman      (501) staff       (20)    63675 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/cwrappercode.py
--rw-r--r--   0 yaman      (501) staff       (20)   121391 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/fcode.py
--rw-r--r--   0 yaman      (501) staff       (20)    20480 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/luacode.py
--rw-r--r--   0 yaman      (501) staff       (20)    38538 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/printing/pycode.py
--rw-r--r--   0 yaman      (501) staff       (20)     5941 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/python_wrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)     7452 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/codegen/utilities.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.846050 pyccel-1.7.4/pyccel/commands/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/commands/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    11032 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/commands/console.py
--rw-r--r--   0 yaman      (501) staff       (20)     3461 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/commands/pyccel_clean.py
--rw-r--r--   0 yaman      (501) staff       (20)     1144 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/commands/pyccel_init.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.847418 pyccel-1.7.4/pyccel/compilers/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/compilers/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    10742 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/compilers/default_compilers.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.849477 pyccel-1.7.4/pyccel/complexity/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/complexity/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2780 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/complexity/arithmetic.py
--rw-r--r--   0 yaman      (501) staff       (20)     1145 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/complexity/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)     7188 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/complexity/memory.py
--rw-r--r--   0 yaman      (501) staff       (20)     2358 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/decorators.py
--rw-r--r--   0 yaman      (501) staff       (20)    11778 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/epyccel.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.850786 pyccel-1.7.4/pyccel/errors/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/errors/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    11261 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/errors/errors.py
--rw-r--r--   0 yaman      (501) staff       (20)    11854 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/errors/messages.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.852404 pyccel-1.7.4/pyccel/naming/
--rw-r--r--   0 yaman      (501) staff       (20)      791 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/naming/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2980 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/naming/cnameclashchecker.py
--rw-r--r--   0 yaman      (501) staff       (20)     3572 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/naming/fortrannameclashchecker.py
--rw-r--r--   0 yaman      (501) staff       (20)     1429 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/naming/pythonnameclashchecker.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.855745 pyccel-1.7.4/pyccel/parser/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    16370 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/base.py
--rw-r--r--   0 yaman      (501) staff       (20)     9547 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/extend_tree.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.860050 pyccel-1.7.4/pyccel/parser/grammar/
--rw-r--r--   0 yaman      (501) staff       (20)     2221 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/grammar/headers.tx
--rw-r--r--   0 yaman      (501) staff       (20)      391 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/grammar/himi.tx
--rw-r--r--   0 yaman      (501) staff       (20)     6361 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/grammar/openacc.tx
--rw-r--r--   0 yaman      (501) staff       (20)     7307 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/grammar/openmp.tx
--rw-r--r--   0 yaman      (501) staff       (20)     6539 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/grammar/pyccel.tx
--rw-r--r--   0 yaman      (501) staff       (20)     7460 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/parser.py
--rw-r--r--   0 yaman      (501) staff       (20)    19696 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/scope.py
--rw-r--r--   0 yaman      (501) staff       (20)   161830 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/semantic.py
--rw-r--r--   0 yaman      (501) staff       (20)    39088 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntactic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.864222 pyccel-1.7.4/pyccel/parser/syntax/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2236 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)    19189 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/headers.py
--rw-r--r--   0 yaman      (501) staff       (20)     4144 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/himi.py
--rw-r--r--   0 yaman      (501) staff       (20)    36464 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/openacc.py
--rw-r--r--   0 yaman      (501) staff       (20)    27508 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/syntax/openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)     4079 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/parser/utilities.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.864714 pyccel-1.7.4/pyccel/stdlib/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.865543 pyccel-1.7.4/pyccel/stdlib/cwrapper/
--rw-r--r--   0 yaman      (501) staff       (20)     4529 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/cwrapper/cwrapper.c
--rw-r--r--   0 yaman      (501) staff       (20)     6528 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/cwrapper/cwrapper.h
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.866905 pyccel-1.7.4/pyccel/stdlib/cwrapper_ndarrays/
--rw-r--r--   0 yaman      (501) staff       (20)    12578 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c
--rw-r--r--   0 yaman      (501) staff       (20)     1845 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.869194 pyccel-1.7.4/pyccel/stdlib/external/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/external/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     1749 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/external/dfftpack.py
--rw-r--r--   0 yaman      (501) staff       (20)     1112 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/external/fitpack.py
--rw-r--r--   0 yaman      (501) staff       (20)     1266 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/external/lapack.py
--rw-r--r--   0 yaman      (501) staff       (20)     9467 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/external/mpi4py.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.880124 pyccel-1.7.4/pyccel/stdlib/internal/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    35216 2023-05-02 21:46:43.000000 pyccel-1.7.4/pyccel/stdlib/internal/blas.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     7825 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/blas.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     5940 2023-05-02 21:46:43.000000 pyccel-1.7.4/pyccel/stdlib/internal/dfftpack.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     1144 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/dfftpack.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     2841 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/fftw.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     2867 2023-05-02 21:46:43.000000 pyccel-1.7.4/pyccel/stdlib/internal/fitpack.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)      343 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/fitpack.pyh
--rw-r--r--   0 yaman      (501) staff       (20)    18250 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/hdf5.pyh
--rw-r--r--   0 yaman      (501) staff       (20)   354641 2023-05-02 21:46:44.000000 pyccel-1.7.4/pyccel/stdlib/internal/lapack.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)    58149 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/lapack.pyh
--rw-r--r--   0 yaman      (501) staff       (20)    25250 2023-05-02 21:46:44.000000 pyccel-1.7.4/pyccel/stdlib/internal/mpi.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     5911 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/mpi.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     1226 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/mpiext.py
--rw-r--r--   0 yaman      (501) staff       (20)    11017 2023-05-02 21:46:44.000000 pyccel-1.7.4/pyccel/stdlib/internal/openacc.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     2675 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/openacc.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     8715 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)    10053 2023-05-02 21:46:44.000000 pyccel-1.7.4/pyccel/stdlib/internal/openmp.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     2645 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/internal/openmp.pyh
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.882061 pyccel-1.7.4/pyccel/stdlib/math/
--rw-r--r--   0 yaman      (501) staff       (20)     1766 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/math/pyc_math_c.c
--rw-r--r--   0 yaman      (501) staff       (20)     1331 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/math/pyc_math_c.h
--rw-r--r--   0 yaman      (501) staff       (20)     3479 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/math/pyc_math_f90.f90
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.883523 pyccel-1.7.4/pyccel/stdlib/ndarrays/
--rw-r--r--   0 yaman      (501) staff       (20)    11346 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/ndarrays/ndarrays.c
--rw-r--r--   0 yaman      (501) staff       (20)     7152 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/ndarrays/ndarrays.h
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.885589 pyccel-1.7.4/pyccel/stdlib/numpy/
--rw-r--r--   0 yaman      (501) staff       (20)      755 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/numpy/numpy_c.c
--rw-r--r--   0 yaman      (501) staff       (20)      650 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/numpy/numpy_c.h
--rw-r--r--   0 yaman      (501) staff       (20)     4629 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/numpy/numpy_f90.f90
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.886537 pyccel-1.7.4/pyccel/stdlib/parallel/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/parallel/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     7487 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/stdlib/parallel/mpi.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.887520 pyccel-1.7.4/pyccel/symbolic/
--rw-r--r--   0 yaman      (501) staff       (20)       48 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/symbolic/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     4472 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/symbolic/lambdify.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.889491 pyccel-1.7.4/pyccel/utilities/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/utilities/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     1203 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/utilities/metaclasses.py
--rw-r--r--   0 yaman      (501) staff       (20)     1227 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/utilities/stage.py
--rw-r--r--   0 yaman      (501) staff       (20)     1796 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/utilities/strings.py
--rw-r--r--   0 yaman      (501) staff       (20)       86 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyccel/version.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.816588 pyccel-1.7.4/pyccel.egg-info/
--rw-r--r--   0 yaman      (501) staff       (20)    13504 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/PKG-INFO
--rw-r--r--   0 yaman      (501) staff       (20)    24626 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/SOURCES.txt
--rw-r--r--   0 yaman      (501) staff       (20)        1 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/dependency_links.txt
--rw-r--r--   0 yaman      (501) staff       (20)      185 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/entry_points.txt
--rw-r--r--   0 yaman      (501) staff       (20)        1 2023-05-02 21:46:44.000000 pyccel-1.7.4/pyccel.egg-info/not-zip-safe
--rw-r--r--   0 yaman      (501) staff       (20)      178 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/requires.txt
--rw-r--r--   0 yaman      (501) staff       (20)        7 2023-05-02 21:46:46.000000 pyccel-1.7.4/pyccel.egg-info/top_level.txt
--rw-r--r--   0 yaman      (501) staff       (20)      225 2023-05-02 21:45:18.000000 pyccel-1.7.4/pyproject.toml
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.891082 pyccel-1.7.4/samples/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/samples/README.rst
--rw-r--r--   0 yaman      (501) staff       (20)      385 2023-05-02 21:45:18.000000 pyccel-1.7.4/samples/mxm.py
--rw-r--r--   0 yaman      (501) staff       (20)      564 2023-05-02 21:45:18.000000 pyccel-1.7.4/samples/mxm_openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)      950 2023-05-02 21:46:47.195119 pyccel-1.7.4/setup.cfg
--rw-r--r--   0 yaman      (501) staff       (20)      628 2023-05-02 21:45:18.000000 pyccel-1.7.4/setup.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.893571 pyccel-1.7.4/tests/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.894232 pyccel-1.7.4/tests/ast/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.895557 pyccel-1.7.4/tests/ast/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      257 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ast/scripts/cyclic_dependence.py
--rw-r--r--   0 yaman      (501) staff       (20)      173 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ast/scripts/math.py
--rw-r--r--   0 yaman      (501) staff       (20)     5098 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ast/test_basic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.792333 pyccel-1.7.4/tests/codegen/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.896295 pyccel-1.7.4/tests/codegen/ccode/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.901543 pyccel-1.7.4/tests/codegen/ccode/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      771 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)     1558 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_create.py
--rw-r--r--   0 yaman      (501) staff       (20)      754 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_indexing.py
--rw-r--r--   0 yaman      (501) staff       (20)      616 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_pointers.py
--rw-r--r--   0 yaman      (501) staff       (20)     1320 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_slicing.py
--rw-r--r--   0 yaman      (501) staff       (20)      876 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      925 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)     1300 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)      378 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)     1734 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/ccode/test_ccode_codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.902104 pyccel-1.7.4/tests/codegen/fcode/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.923259 pyccel-1.7.4/tests/codegen/fcode/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)     1280 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/CommentBlock.py
--rw-r--r--   0 yaman      (501) staff       (20)      851 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/Functional_Stmts.py
--rw-r--r--   0 yaman      (501) staff       (20)      401 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/ListComprehension.py
--rw-r--r--   0 yaman      (501) staff       (20)      145 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/USELESS_EXPRESSION.py
--rw-r--r--   0 yaman      (501) staff       (20)      229 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)      101 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/calls.py
--rw-r--r--   0 yaman      (501) staff       (20)      646 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)      734 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/classes_2.py
--rw-r--r--   0 yaman      (501) staff       (20)      735 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/classes_3.py
--rw-r--r--   0 yaman      (501) staff       (20)     1388 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/classes_4.py
--rw-r--r--   0 yaman      (501) staff       (20)      295 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/complex_numbers.py
--rw-r--r--   0 yaman      (501) staff       (20)      154 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/concatenation.py
--rw-r--r--   0 yaman      (501) staff       (20)     1160 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/context.py
--rw-r--r--   0 yaman      (501) staff       (20)     1272 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/decorators.py
--rw-r--r--   0 yaman      (501) staff       (20)      294 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/decorators_elemental.py
--rw-r--r--   0 yaman      (501) staff       (20)      163 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/decorators_pure.py
--rw-r--r--   0 yaman      (501) staff       (20)     1103 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/decorators_types.py
--rw-r--r--   0 yaman      (501) staff       (20)      232 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)      574 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/functions_inout.py
--rw-r--r--   0 yaman      (501) staff       (20)      480 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/generic_methods.py
--rw-r--r--   0 yaman      (501) staff       (20)      425 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/headers.py
--rw-r--r--   0 yaman      (501) staff       (20)      980 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)      264 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      485 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/issue_177.py
--rw-r--r--   0 yaman      (501) staff       (20)      190 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/lists.py
--rw-r--r--   0 yaman      (501) staff       (20)      838 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     2002 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/macros.py
--rw-r--r--   0 yaman      (501) staff       (20)      802 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/matrix_assembly.py
--rw-r--r--   0 yaman      (501) staff       (20)      681 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/matrix_mul.py
--rw-r--r--   0 yaman      (501) staff       (20)      257 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/multiple_assign.py
--rw-r--r--   0 yaman      (501) staff       (20)     1231 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/numpyext.py
--rw-r--r--   0 yaman      (501) staff       (20)      782 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/precision.py
--rw-r--r--   0 yaman      (501) staff       (20)      761 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/recursive_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      236 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/returns.py
--rw-r--r--   0 yaman      (501) staff       (20)      359 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      381 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)     1711 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/fcode/test_fcode_codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.923902 pyccel-1.7.4/tests/codegen/pycode/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.924482 pyccel-1.7.4/tests/codegen/pycode/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)     1427 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/pycode/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     1351 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/codegen/pycode/test_pycode_codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.925108 pyccel-1.7.4/tests/complexity/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.925845 pyccel-1.7.4/tests/complexity/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/complexity/scripts/ex.py
--rw-r--r--   0 yaman      (501) staff       (20)     1053 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/complexity/test_complexity.py
--rw-r--r--   0 yaman      (501) staff       (20)     2253 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/conftest.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.957871 pyccel-1.7.4/tests/epyccel/
--rw-r--r--   0 yaman      (501) staff       (20)      240 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/Module_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      238 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/README.rst
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.980337 pyccel-1.7.4/tests/epyccel/modules/
--rw-r--r--   0 yaman      (501) staff       (20)      240 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      315 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_2.py
--rw-r--r--   0 yaman      (501) staff       (20)      247 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      338 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_4.py
--rw-r--r--   0 yaman      (501) staff       (20)     1363 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_5.py
--rw-r--r--   0 yaman      (501) staff       (20)      698 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_6.py
--rw-r--r--   0 yaman      (501) staff       (20)      771 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_7.py
--rw-r--r--   0 yaman      (501) staff       (20)      234 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/Module_8.py
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      728 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/array_consts.py
--rw-r--r--   0 yaman      (501) staff       (20)    47942 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)     2416 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/augassign.py
--rw-r--r--   0 yaman      (501) staff       (20)      234 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/awkward_names.py
--rw-r--r--   0 yaman      (501) staff       (20)     3565 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/base.py
--rw-r--r--   0 yaman      (501) staff       (20)     1497 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/bitwise.py
--rw-r--r--   0 yaman      (501) staff       (20)      845 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/call_user_defined_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)     2001 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/complex_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      222 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/consts.py
--rw-r--r--   0 yaman      (501) staff       (20)     2284 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/external_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     2092 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/functionals.py
--rw-r--r--   0 yaman      (501) staff       (20)     2227 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/generic_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     4058 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/generic_functions_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     4157 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/highorder_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     4462 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     1070 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/mpi_collective.py
--rw-r--r--   0 yaman      (501) staff       (20)      530 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/mpi_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)     2911 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/multi_rank.py
--rw-r--r--   0 yaman      (501) staff       (20)     5155 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/numpy_sign.py
--rw-r--r--   0 yaman      (501) staff       (20)    14866 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)     1198 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/pointers.py
--rw-r--r--   0 yaman      (501) staff       (20)     1101 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/python_annotations.py
--rw-r--r--   0 yaman      (501) staff       (20)      681 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/strings.py
--rw-r--r--   0 yaman      (501) staff       (20)     9815 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      632 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/modules/types.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.986185 pyccel-1.7.4/tests/epyccel/recognised_functions/
--rw-r--r--   0 yaman      (501) staff       (20)     2756 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py
--rw-r--r--   0 yaman      (501) staff       (20)    37669 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/recognised_functions/test_math_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)   247535 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/recognised_functions/test_numpy_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)    45813 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/recognised_functions/test_numpy_types.py
--rw-r--r--   0 yaman      (501) staff       (20)     4693 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_array_as_func_args.py
--rw-r--r--   0 yaman      (501) staff       (20)    95679 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)     9425 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_arrays_multiple_assignments.py
--rw-r--r--   0 yaman      (501) staff       (20)     6170 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_base.py
--rw-r--r--   0 yaman      (501) staff       (20)     5120 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_bitwise.py
--rw-r--r--   0 yaman      (501) staff       (20)     9648 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_builtins.py
--rw-r--r--   0 yaman      (501) staff       (20)     2537 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_class_expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1476 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_compare_expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)      834 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_default_precision_template.py
--rw-r--r--   0 yaman      (501) staff       (20)     1191 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_docstrings.py
--rw-r--r--   0 yaman      (501) staff       (20)     7704 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_IfTernaryOperator.py
--rw-r--r--   0 yaman      (501) staff       (20)     7921 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_augassign.py
--rw-r--r--   0 yaman      (501) staff       (20)     3817 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_complex_func.py
--rw-r--r--   0 yaman      (501) staff       (20)     3136 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_decorators.py
--rw-r--r--   0 yaman      (501) staff       (20)     2377 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_default_args.py
--rw-r--r--   0 yaman      (501) staff       (20)     8351 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_division.py
--rw-r--r--   0 yaman      (501) staff       (20)     9369 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     4662 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_generators.py
--rw-r--r--   0 yaman      (501) staff       (20)     2822 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_mod.py
--rw-r--r--   0 yaman      (501) staff       (20)     4652 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_modules.py
--rw-r--r--   0 yaman      (501) staff       (20)     5519 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_multi_rank.py
--rw-r--r--   0 yaman      (501) staff       (20)    19588 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)     5681 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_optional_args.py
--rw-r--r--   0 yaman      (501) staff       (20)     6663 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_pow.py
--rw-r--r--   0 yaman      (501) staff       (20)     3265 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_python_annotations.py
--rw-r--r--   0 yaman      (501) staff       (20)    30656 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_return_arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)    13388 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_sign.py
--rw-r--r--   0 yaman      (501) staff       (20)     5823 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_transpose.py
--rw-r--r--   0 yaman      (501) staff       (20)     3471 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_epyccel_types.py
--rw-r--r--   0 yaman      (501) staff       (20)     3306 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_external_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     2149 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_functionals.py
--rw-r--r--   0 yaman      (501) staff       (20)    14120 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_generic_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1922 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_higherorder_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1841 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)     2208 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_kind.py
--rw-r--r--   0 yaman      (501) staff       (20)     5783 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     4164 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_mpi_collective.py
--rw-r--r--   0 yaman      (501) staff       (20)     2114 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_mpi_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)     1040 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_multiple_results.py
--rw-r--r--   0 yaman      (501) staff       (20)     1735 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_parallel_epyccel.py
--rw-r--r--   0 yaman      (501) staff       (20)     1258 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_pointers.py
--rw-r--r--   0 yaman      (501) staff       (20)     7595 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_return.py
--rw-r--r--   0 yaman      (501) staff       (20)     1333 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_strings.py
--rw-r--r--   0 yaman      (501) staff       (20)     3200 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/test_tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      704 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/epyccel/utilities.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.987366 pyccel-1.7.4/tests/errors/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.795123 pyccel-1.7.4/tests/errors/codegen/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.989006 pyccel-1.7.4/tests/errors/codegen/fortran/
--rw-r--r--   0 yaman      (501) staff       (20)      108 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/codegen/fortran/FORTRAN_ALLOCATABLE_IN_EXPRESSION.py
--rw-r--r--   0 yaman      (501) staff       (20)      131 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/codegen/fortran/randint.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.995793 pyccel-1.7.4/tests/errors/known_bugs/
--rw-r--r--   0 yaman      (501) staff       (20)      236 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/cross.py
--rw-r--r--   0 yaman      (501) staff       (20)      143 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/dicts.py
--rw-r--r--   0 yaman      (501) staff       (20)      495 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/ex3.py
--rw-r--r--   0 yaman      (501) staff       (20)      796 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/ex4.py
--rw-r--r--   0 yaman      (501) staff       (20)      654 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/generic_methods.py
--rw-r--r--   0 yaman      (501) staff       (20)      579 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/header_interface.py
--rw-r--r--   0 yaman      (501) staff       (20)      928 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/inheritance.py
--rw-r--r--   0 yaman      (501) staff       (20)      180 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/known_bugs/lambdas.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.795987 pyccel-1.7.4/tests/errors/semantic/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.017946 pyccel-1.7.4/tests/errors/semantic/blocking/
--rw-r--r--   0 yaman      (501) staff       (20)      128 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_0.py
--rw-r--r--   0 yaman      (501) staff       (20)      208 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      174 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/COMPLEX_TYPE.py
--rw-r--r--   0 yaman      (501) staff       (20)      159 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT.py
--rw-r--r--   0 yaman      (501) staff       (20)      193 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT2.py
--rw-r--r--   0 yaman      (501) staff       (20)      155 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/DECORATOR_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      132 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      296 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
--rw-r--r--   0 yaman      (501) staff       (20)      114 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED.py
--rw-r--r--   0 yaman      (501) staff       (20)      145 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED2.py
--rw-r--r--   0 yaman      (501) staff       (20)      315 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED3.py
--rw-r--r--   0 yaman      (501) staff       (20)       94 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/INHOMOG_LIST.py
--rw-r--r--   0 yaman      (501) staff       (20)      124 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/INIT_NDARRAY_WITH_INHOMOG_LIST.py
--rw-r--r--   0 yaman      (501) staff       (20)      436 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/INTERFACE_WRONG_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      182 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/LIST_OF_TUPLES.py
--rw-r--r--   0 yaman      (501) staff       (20)      129 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/OPENMP_loop_check.py
--rw-r--r--   0 yaman      (501) staff       (20)      102 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/OPENMP_parallel_for_check.py
--rw-r--r--   0 yaman      (501) staff       (20)      131 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/OPENMP_simd_check.py
--rw-r--r--   0 yaman      (501) staff       (20)      263 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_decorator.py
--rw-r--r--   0 yaman      (501) staff       (20)      241 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_header.py
--rw-r--r--   0 yaman      (501) staff       (20)      493 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/TEMPLATE_WRONG_TYPE_CALL.py
--rw-r--r--   0 yaman      (501) staff       (20)      110 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/TOO_MANY_ARGS.py
--rw-r--r--   0 yaman      (501) staff       (20)       92 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_FUNCTION.py
--rw-r--r--   0 yaman      (501) staff       (20)       89 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_VARIABLE.py
--rw-r--r--   0 yaman      (501) staff       (20)      108 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/UNRECOGNISED_FUNCTION_CALL.py
--rw-r--r--   0 yaman      (501) staff       (20)      186 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)       95 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ex2.py
--rw-r--r--   0 yaman      (501) staff       (20)       97 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ex3.py
--rw-r--r--   0 yaman      (501) staff       (20)       88 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ex4.py
--rw-r--r--   0 yaman      (501) staff       (20)       92 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/ex5.py
--rw-r--r--   0 yaman      (501) staff       (20)      100 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/str_join.py
--rw-r--r--   0 yaman      (501) staff       (20)      106 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/blocking/str_join2.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.033268 pyccel-1.7.4/tests/errors/semantic/non_blocking/
--rw-r--r--   0 yaman      (501) staff       (20)      136 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT.py
--rw-r--r--   0 yaman      (501) staff       (20)      150 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT2.py
--rw-r--r--   0 yaman      (501) staff       (20)      152 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      118 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_2.py
--rw-r--r--   0 yaman      (501) staff       (20)       87 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      155 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_complex.py
--rw-r--r--   0 yaman      (501) staff       (20)      149 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_float.py
--rw-r--r--   0 yaman      (501) staff       (20)      147 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_integer.py
--rw-r--r--   0 yaman      (501) staff       (20)      163 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_string.py
--rw-r--r--   0 yaman      (501) staff       (20)      148 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_complex.py
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_float.py
--rw-r--r--   0 yaman      (501) staff       (20)      140 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_integer.py
--rw-r--r--   0 yaman      (501) staff       (20)      156 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_string.py
--rw-r--r--   0 yaman      (501) staff       (20)      220 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/PYCCEL_RESTRICTION_LIST_COMPREHENSION_LIMITS.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/TOO_FEW_ARGS.py
--rw-r--r--   0 yaman      (501) staff       (20)      118 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT.py
--rw-r--r--   0 yaman      (501) staff       (20)       97 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT2.py
--rw-r--r--   0 yaman      (501) staff       (20)      201 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/ex6.py
--rw-r--r--   0 yaman      (501) staff       (20)      143 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/is.py
--rw-r--r--   0 yaman      (501) staff       (20)      195 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/semantic/non_blocking/var_is_none.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.034559 pyccel-1.7.4/tests/errors/syntax_blockers/
--rw-r--r--   0 yaman      (501) staff       (20)      286 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_blockers/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      412 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_blockers/imports.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.043753 pyccel-1.7.4/tests/errors/syntax_errors/
--rw-r--r--   0 yaman      (501) staff       (20)      371 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/TEMPLATE_WRONG_KEY.py
--rw-r--r--   0 yaman      (501) staff       (20)      382 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/TEMPLATE_WRONG_NUMBER_ARGS.py
--rw-r--r--   0 yaman      (501) staff       (20)       91 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/dict_str_keys.py
--rw-r--r--   0 yaman      (501) staff       (20)      206 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/functions_in_template.py
--rw-r--r--   0 yaman      (501) staff       (20)      157 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/functions_in_uniontype.py
--rw-r--r--   0 yaman      (501) staff       (20)      109 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/import_star.py
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/list_comprehension_no_assign.py
--rw-r--r--   0 yaman      (501) staff       (20)       95 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/nargs.py
--rw-r--r--   0 yaman      (501) staff       (20)      125 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/not_implemented.py
--rw-r--r--   0 yaman      (501) staff       (20)      114 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/raise.py
--rw-r--r--   0 yaman      (501) staff       (20)      125 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/try.py
--rw-r--r--   0 yaman      (501) staff       (20)      156 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/types_arg.py
--rw-r--r--   0 yaman      (501) staff       (20)      137 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/types_arg_type.py
--rw-r--r--   0 yaman      (501) staff       (20)       99 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/syntax_errors/yield.py
--rw-r--r--   0 yaman      (501) staff       (20)     4383 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/errors/test_errors.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.044398 pyccel-1.7.4/tests/external/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.797285 pyccel-1.7.4/tests/external/scripts/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.045065 pyccel-1.7.4/tests/external/scripts/lapack/
--rw-r--r--   0 yaman      (501) staff       (20)     2401 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/lapack/ex1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.056787 pyccel-1.7.4/tests/external/scripts/mpi4py/
--rw-r--r--   0 yaman      (501) staff       (20)      334 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      684 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/bcast.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.058230 pyccel-1.7.4/tests/external/scripts/mpi4py/bugs/
--rw-r--r--   0 yaman      (501) staff       (20)      943 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/bugs/ex6.py
--rw-r--r--   0 yaman      (501) staff       (20)      662 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/bugs/ex8.py
--rw-r--r--   0 yaman      (501) staff       (20)      550 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/gather.py
--rw-r--r--   0 yaman      (501) staff       (20)      468 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_Allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      765 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_Bcast.py
--rw-r--r--   0 yaman      (501) staff       (20)      720 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_Gather.py
--rw-r--r--   0 yaman      (501) staff       (20)      435 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_Reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      524 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_Sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      636 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      402 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1559 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/np_point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      274 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      367 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1559 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      339 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      364 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      240 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/scripts/mpi4py/who_am_i.py
--rw-r--r--   0 yaman      (501) staff       (20)     1362 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/external/test_external.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.058935 pyccel-1.7.4/tests/internal/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.799163 pyccel-1.7.4/tests/internal/scripts/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.062314 pyccel-1.7.4/tests/internal/scripts/blas/
--rw-r--r--   0 yaman      (501) staff       (20)      559 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/blas/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      890 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/blas/ex2.py
--rw-r--r--   0 yaman      (501) staff       (20)      584 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/blas/ex3.py
--rw-r--r--   0 yaman      (501) staff       (20)      920 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/blas/ex4.py
--rw-r--r--   0 yaman      (501) staff       (20)      761 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/blas/ex5.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.062955 pyccel-1.7.4/tests/internal/scripts/lapack/
--rw-r--r--   0 yaman      (501) staff       (20)     2779 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/lapack/ex1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.072661 pyccel-1.7.4/tests/internal/scripts/mpi/
--rw-r--r--   0 yaman      (501) staff       (20)     1401 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/allgather.py
--rw-r--r--   0 yaman      (501) staff       (20)     1205 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)     1391 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/alltoall.py
--rw-r--r--   0 yaman      (501) staff       (20)     1129 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/bcast.py
--rw-r--r--   0 yaman      (501) staff       (20)     2057 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/column.py
--rw-r--r--   0 yaman      (501) staff       (20)     1477 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/gather.py
--rw-r--r--   0 yaman      (501) staff       (20)     2089 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/line.py
--rw-r--r--   0 yaman      (501) staff       (20)     1771 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/nonblocking.py
--rw-r--r--   0 yaman      (501) staff       (20)     1266 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/point_to_point_1.py
--rw-r--r--   0 yaman      (501) staff       (20)     3048 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1237 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)     1431 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/scatter.py
--rw-r--r--   0 yaman      (501) staff       (20)     1372 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)     1321 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/sendrecv_replace.py
--rw-r--r--   0 yaman      (501) staff       (20)     1740 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/split.py
--rw-r--r--   0 yaman      (501) staff       (20)      772 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/mpi/who_am_i.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.075069 pyccel-1.7.4/tests/internal/scripts/openacc/
--rw-r--r--   0 yaman      (501) staff       (20)      448 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/openacc/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      619 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/openacc/sum.py
--rw-r--r--   0 yaman      (501) staff       (20)      581 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/openacc/sum_kernels.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.076953 pyccel-1.7.4/tests/internal/scripts/openmp/
--rw-r--r--   0 yaman      (501) staff       (20)      606 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/openmp/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      412 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/scripts/openmp/ex2.py
--rw-r--r--   0 yaman      (501) staff       (20)     3507 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/internal/test_internal.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.077625 pyccel-1.7.4/tests/macro/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:46.800614 pyccel-1.7.4/tests/macro/scripts/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.089085 pyccel-1.7.4/tests/macro/scripts/MPI/
--rw-r--r--   0 yaman      (501) staff       (20)      447 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      864 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/bcast.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.090471 pyccel-1.7.4/tests/macro/scripts/MPI/bug/
--rw-r--r--   0 yaman      (501) staff       (20)     1586 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/bug/ex6.py
--rw-r--r--   0 yaman      (501) staff       (20)      662 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/bug/ex8.py
--rw-r--r--   0 yaman      (501) staff       (20)      788 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/gather.py
--rw-r--r--   0 yaman      (501) staff       (20)     7929 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/mpi4py.py
--rw-r--r--   0 yaman      (501) staff       (20)      548 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_Allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      898 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_Bcast.py
--rw-r--r--   0 yaman      (501) staff       (20)      831 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_Gather.py
--rw-r--r--   0 yaman      (501) staff       (20)      551 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_Reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      567 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_Sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      749 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      602 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1942 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      379 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      567 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1952 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      471 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      478 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      403 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/MPI/who_am_i.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.094922 pyccel-1.7.4/tests/macro/scripts/blas/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.095544 pyccel-1.7.4/tests/macro/scripts/blas/bugs/
--rw-r--r--   0 yaman      (501) staff       (20)      363 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/bugs/dnrm2.py
--rw-r--r--   0 yaman      (501) staff       (20)      681 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_daxpy.py
--rw-r--r--   0 yaman      (501) staff       (20)      467 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dcopy.py
--rw-r--r--   0 yaman      (501) staff       (20)     1148 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dgemm.py
--rw-r--r--   0 yaman      (501) staff       (20)     1186 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dgemv.py
--rw-r--r--   0 yaman      (501) staff       (20)      756 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dger.py
--rw-r--r--   0 yaman      (501) staff       (20)      482 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dscal.py
--rw-r--r--   0 yaman      (501) staff       (20)      636 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/blas/runtest_dswap.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.096229 pyccel-1.7.4/tests/macro/scripts/lapack/
--rw-r--r--   0 yaman      (501) staff       (20)      670 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/scripts/lapack/runtest_dgbtrf.py
--rw-r--r--   0 yaman      (501) staff       (20)     3214 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/macro/test_macro.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.098132 pyccel-1.7.4/tests/ndarrays/
--rw-r--r--   0 yaman      (501) staff       (20)     4723 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ndarrays/conftest.py
--rw-r--r--   0 yaman      (501) staff       (20)     1714 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ndarrays/leaks_check.py
--rw-r--r--   0 yaman      (501) staff       (20)    26585 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/ndarrays/test_ndarrays.c
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.101658 pyccel-1.7.4/tests/parser/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.102270 pyccel-1.7.4/tests/parser/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)     1074 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/scripts/comments.py
--rw-r--r--   0 yaman      (501) staff       (20)     3490 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/test_comments.py
--rw-r--r--   0 yaman      (501) staff       (20)     1468 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/test_headers.py
--rw-r--r--   0 yaman      (501) staff       (20)      304 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/test_himi.py
--rw-r--r--   0 yaman      (501) staff       (20)      358 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/test_openacc.py
--rw-r--r--   0 yaman      (501) staff       (20)      279 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/parser/test_openmp.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.102974 pyccel-1.7.4/tests/preprocess/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.103505 pyccel-1.7.4/tests/preprocess/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      943 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/preprocess/scripts/omp.py
--rw-r--r--   0 yaman      (501) staff       (20)     1017 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/preprocess/test_preprocess.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.104860 pyccel-1.7.4/tests/pyccel/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.106066 pyccel-1.7.4/tests/pyccel/project_abs_imports/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.106666 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.108019 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder1/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder1/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      305 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder1/mod1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.109561 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder2/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder2/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      227 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder2/mod2.py
--rw-r--r--   0 yaman      (501) staff       (20)      306 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/project/folder2/mod3.py
--rw-r--r--   0 yaman      (501) staff       (20)      214 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_abs_imports/runtest.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.112300 pyccel-1.7.4/tests/pyccel/project_multi_imports/
--rw-r--r--   0 yaman      (501) staff       (20)      116 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_multi_imports/file1.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_multi_imports/file2.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_multi_imports/file3.py
--rw-r--r--   0 yaman      (501) staff       (20)      179 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_multi_imports/file4.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.112985 pyccel-1.7.4/tests/pyccel/project_rel_imports/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.113684 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.114492 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder1/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder1/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      305 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder1/mod1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.116257 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder2/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder2/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      221 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder2/mod2.py
--rw-r--r--   0 yaman      (501) staff       (20)      285 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/project/folder2/mod3.py
--rw-r--r--   0 yaman      (501) staff       (20)      214 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/project_rel_imports/runtest.py
--rw-r--r--   0 yaman      (501) staff       (20)      199 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/run_import_function.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.137798 pyccel-1.7.4/tests/pyccel/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2969 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/array_binary_operation.py
--rw-r--r--   0 yaman      (501) staff       (20)     4131 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/arrays_view.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.140046 pyccel-1.7.4/tests/pyccel/scripts/asserts/
--rw-r--r--   0 yaman      (501) staff       (20)      117 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/asserts/unvalid_assert1.py
--rw-r--r--   0 yaman      (501) staff       (20)      138 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/asserts/unvalid_assert2.py
--rw-r--r--   0 yaman      (501) staff       (20)      162 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/asserts/unvalid_assert3.py
--rw-r--r--   0 yaman      (501) staff       (20)      217 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/asserts/valid_assert.py
--rw-r--r--   0 yaman      (501) staff       (20)       68 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/basic_header.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     1410 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/bool_comp.py
--rw-r--r--   0 yaman      (501) staff       (20)     2132 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/c_arrays.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.141781 pyccel-1.7.4/tests/pyccel/scripts/classes/
--rw-r--r--   0 yaman      (501) staff       (20)      726 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/classes/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)      590 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/classes/classes_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      490 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/classes/classes_5.py
--rw-r--r--   0 yaman      (501) staff       (20)      372 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/decorators_elemental.py
--rw-r--r--   0 yaman      (501) staff       (20)      821 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/decorators_inline.py
--rw-r--r--   0 yaman      (501) staff       (20)      915 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/default_args_mod.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.145918 pyccel-1.7.4/tests/pyccel/scripts/exits/
--rw-r--r--   0 yaman      (501) staff       (20)      126 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/empty_exit.py
--rw-r--r--   0 yaman      (501) staff       (20)      150 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/negative_exit1.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/negative_exit2.py
--rw-r--r--   0 yaman      (501) staff       (20)      127 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/positive_exit1.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/positive_exit2.py
--rw-r--r--   0 yaman      (501) staff       (20)      184 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/positive_exit3.py
--rw-r--r--   0 yaman      (501) staff       (20)      127 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/exits/zero_exit.py
--rw-r--r--   0 yaman      (501) staff       (20)     2236 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/expressions.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.146742 pyccel-1.7.4/tests/pyccel/scripts/folder1/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder1/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      300 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder1/folder1_funcs.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.148571 pyccel-1.7.4/tests/pyccel/scripts/folder2/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder2/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      300 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder2/folder2_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)      198 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder2/runtest_imports2.py
--rw-r--r--   0 yaman      (501) staff       (20)      189 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/folder2/runtest_rel_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      300 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)     1154 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     3617 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/generic_functions.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.152243 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/
--rw-r--r--   0 yaman      (501) staff       (20)      285 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_fib.py
--rw-r--r--   0 yaman      (501) staff       (20)      591 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py
--rw-r--r--   0 yaman      (501) staff       (20)      814 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py
--rw-r--r--   0 yaman      (501) staff       (20)      265 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_pisum.py
--rw-r--r--   0 yaman      (501) staff       (20)     1188 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      807 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/quicksort.py
--rw-r--r--   0 yaman      (501) staff       (20)      280 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/simplify.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.155001 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/
--rw-r--r--   0 yaman      (501) staff       (20)      309 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/fib.py
--rw-r--r--   0 yaman      (501) staff       (20)      583 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py
--rw-r--r--   0 yaman      (501) staff       (20)      826 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py
--rw-r--r--   0 yaman      (501) staff       (20)     1226 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      824 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py
--rw-r--r--   0 yaman      (501) staff       (20)      306 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/simplify.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.165774 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/
--rw-r--r--   0 yaman      (501) staff       (20)      182 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/collisions2.py
--rw-r--r--   0 yaman      (501) staff       (20)      201 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/collisions3.py
--rw-r--r--   0 yaman      (501) staff       (20)      218 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/collisions4.py
--rw-r--r--   0 yaman      (501) staff       (20)      187 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/collisions5.py
--rw-r--r--   0 yaman      (501) staff       (20)      922 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import.py
--rw-r--r--   0 yaman      (501) staff       (20)      993 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as.py
--rw-r--r--   0 yaman      (501) staff       (20)     1002 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      287 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      291 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      943 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      290 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      295 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      934 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod.py
--rw-r--r--   0 yaman      (501) staff       (20)      925 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as.py
--rw-r--r--   0 yaman      (501) staff       (20)     1019 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      282 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      287 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)     1001 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      284 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      288 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      190 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/user_mod.py
--rw-r--r--   0 yaman      (501) staff       (20)      174 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/import_syntax/user_mod2.py
--rw-r--r--   0 yaman      (501) staff       (20)      882 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/lapack_subroutine.py
--rw-r--r--   0 yaman      (501) staff       (20)      175 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/module_init.py
--rw-r--r--   0 yaman      (501) staff       (20)      116 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/module_init2.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.166780 pyccel-1.7.4/tests/pyccel/scripts/numpy/
--rw-r--r--   0 yaman      (501) staff       (20)     1590 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/numpy/numpy_kernels.py
--rw-r--r--   0 yaman      (501) staff       (20)     2812 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/numpy/numpy_sign.py
--rw-r--r--   0 yaman      (501) staff       (20)      812 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/print_integers.py
--rw-r--r--   0 yaman      (501) staff       (20)      885 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/print_sp_and_end.py
--rw-r--r--   0 yaman      (501) staff       (20)     2056 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/print_strings.py
--rw-r--r--   0 yaman      (501) staff       (20)      381 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/print_tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      617 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/return_numpy_arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)      418 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_decorators_inline.py
--rw-r--r--   0 yaman      (501) staff       (20)      736 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_default_args.py
--rw-r--r--   0 yaman      (501) staff       (20)      673 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_degree_in.py
--rw-r--r--   0 yaman      (501) staff       (20)      166 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_folder_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      350 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)      324 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_function_alias.py
--rw-r--r--   0 yaman      (501) staff       (20)      659 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_generic_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      150 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      427 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_inoutfunc.py
--rw-r--r--   0 yaman      (501) staff       (20)      167 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_module_init.py
--rw-r--r--   0 yaman      (501) staff       (20)      305 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_module_init2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1510 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_multiple_results.py
--rw-r--r--   0 yaman      (501) staff       (20)      412 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/scripts/runtest_type_print.py
--rw-r--r--   0 yaman      (501) staff       (20)    42226 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/pyccel/test_pyccel.py
--rw-r--r--   0 yaman      (501) staff       (20)      844 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/run_tests.bat
--rwxr-xr-x   0 yaman      (501) staff       (20)      899 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/run_tests_py3.sh
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.167188 pyccel-1.7.4/tests/semantic/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.172742 pyccel-1.7.4/tests/semantic/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      135 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/calls.py
--rw-r--r--   0 yaman      (501) staff       (20)      506 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)      825 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1171 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      128 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)      197 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      141 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/lists.py
--rw-r--r--   0 yaman      (501) staff       (20)      111 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)      307 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      163 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)      311 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/scripts/zeros.py
--rw-r--r--   0 yaman      (501) staff       (20)     1030 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/semantic/test_semantic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.173178 pyccel-1.7.4/tests/symbolic/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.174865 pyccel-1.7.4/tests/symbolic/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      958 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/symbolic/scripts/decorator.py
--rw-r--r--   0 yaman      (501) staff       (20)      283 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/symbolic/scripts/lambdas.py
--rw-r--r--   0 yaman      (501) staff       (20)      711 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/symbolic/scripts/neural_net.py
--rw-r--r--   0 yaman      (501) staff       (20)     1263 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/symbolic/test_symbolic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.175404 pyccel-1.7.4/tests/syntax/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.184461 pyccel-1.7.4/tests/syntax/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      851 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/Functional_Stmts.py
--rw-r--r--   0 yaman      (501) staff       (20)      157 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/annotated_comments.py
--rw-r--r--   0 yaman      (501) staff       (20)       86 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/asserts.py
--rw-r--r--   0 yaman      (501) staff       (20)       77 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/breaks.py
--rw-r--r--   0 yaman      (501) staff       (20)      110 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/calls.py
--rw-r--r--   0 yaman      (501) staff       (20)      796 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/class_member_index.py
--rw-r--r--   0 yaman      (501) staff       (20)      369 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)       86 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/dels.py
--rw-r--r--   0 yaman      (501) staff       (20)      190 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/dots.py
--rw-r--r--   0 yaman      (501) staff       (20)      964 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)      193 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)      288 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/lists.py
--rw-r--r--   0 yaman      (501) staff       (20)      110 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)       80 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/prints.py
--rw-r--r--   0 yaman      (501) staff       (20)      196 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/slice.py
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)       92 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)      311 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/scripts/zeros.py
--rw-r--r--   0 yaman      (501) staff       (20)     1059 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/syntax/test_syntax.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.184966 pyccel-1.7.4/tests/warnings/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.187968 pyccel-1.7.4/tests/warnings/semantic/
--rw-r--r--   0 yaman      (501) staff       (20)      155 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/DECORATOR_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      145 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/FOUND_DUPLICATED_IMPORT.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      318 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
--rw-r--r--   0 yaman      (501) staff       (20)      133 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/UNDEFINED_DECORATOR.py
--rw-r--r--   0 yaman      (501) staff       (20)      141 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/semantic/UNDEFINED_DECORATORS.py
--rw-r--r--   0 yaman      (501) staff       (20)     3007 2023-05-02 21:45:18.000000 pyccel-1.7.4/tests/warnings/test_warnings.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-05-02 21:46:47.193718 pyccel-1.7.4/tutorial/
--rw-r--r--   0 yaman      (501) staff       (20)     1667 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/builtin-functions.md
--rw-r--r--   0 yaman      (501) staff       (20)     2642 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/compiler.md
--rw-r--r--   0 yaman      (501) staff       (20)     1779 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/const_keyword.md
--rw-r--r--   0 yaman      (501) staff       (20)    15373 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/decorators.md
--rw-r--r--   0 yaman      (501) staff       (20)    10633 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/function-pointers-as-arguments.md
--rw-r--r--   0 yaman      (501) staff       (20)     3173 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/header-files.md
--rw-r--r--   0 yaman      (501) staff       (20)     8825 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/ndarrays.md
--rw-r--r--   0 yaman      (501) staff       (20)    16159 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/numpy-functions.md
--rw-r--r--   0 yaman      (501) staff       (20)    18475 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/openmp.md
--rw-r--r--   0 yaman      (501) staff       (20)    17344 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/quickstart.md
--rw-r--r--   0 yaman      (501) staff       (20)     2505 2023-05-02 21:45:18.000000 pyccel-1.7.4/tutorial/templates.md
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:40.021392 pyccel-1.8.0/
+-rw-r--r--   0 yaman      (501) staff       (20)      522 2023-06-20 10:07:44.000000 pyccel-1.8.0/AUTHORS
+-rw-r--r--   0 yaman      (501) staff       (20)     1081 2023-06-20 10:07:44.000000 pyccel-1.8.0/LICENSE
+-rw-r--r--   0 yaman      (501) staff       (20)      293 2023-06-20 10:07:44.000000 pyccel-1.8.0/MANIFEST.in
+-rw-r--r--   0 yaman      (501) staff       (20)    13504 2023-06-20 10:09:40.021618 pyccel-1.8.0/PKG-INFO
+-rw-r--r--   0 yaman      (501) staff       (20)    13180 2023-06-20 10:07:44.000000 pyccel-1.8.0/README.md
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.775745 pyccel-1.8.0/pyccel/
+-rw-r--r--   0 yaman      (501) staff       (20)       33 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/__init__.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.791304 pyccel-1.8.0/pyccel/ast/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    15604 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/basic.py
+-rw-r--r--   0 yaman      (501) staff       (20)    16812 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/bind_c.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7686 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/bitwise_operators.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3400 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/builtin_imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)    29378 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/builtins.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6502 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/c_concepts.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6460 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/class_defs.py
+-rw-r--r--   0 yaman      (501) staff       (20)   127130 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/core.py
+-rw-r--r--   0 yaman      (501) staff       (20)    20054 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/cwrapper.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9758 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/datatypes.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3715 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/functionalexpr.py
+-rw-r--r--   0 yaman      (501) staff       (20)    29329 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/headers.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9428 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/internals.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2062 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/itertoolsext.py
+-rw-r--r--   0 yaman      (501) staff       (20)    10766 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/literals.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3564 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/macros.py
+-rw-r--r--   0 yaman      (501) staff       (20)    10805 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/mathext.py
+-rw-r--r--   0 yaman      (501) staff       (20)    15073 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/numpy_wrapper.py
+-rw-r--r--   0 yaman      (501) staff       (20)    62314 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/numpyext.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7113 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/omp.py
+-rw-r--r--   0 yaman      (501) staff       (20)    35482 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/operators.py
+-rw-r--r--   0 yaman      (501) staff       (20)      869 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/scipyext.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7346 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/sympy_helper.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1630 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/sysext.py
+-rw-r--r--   0 yaman      (501) staff       (20)    30831 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/utilities.py
+-rw-r--r--   0 yaman      (501) staff       (20)    28982 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/ast/variable.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.793391 pyccel-1.8.0/pyccel/codegen/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6587 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/codegen.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.794435 pyccel-1.8.0/pyccel/codegen/compiling/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/compiling/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9200 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/compiling/basic.py
+-rw-r--r--   0 yaman      (501) staff       (20)    18032 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/compiling/compilers.py
+-rw-r--r--   0 yaman      (501) staff       (20)    16408 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/pipeline.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.797749 pyccel-1.8.0/pyccel/codegen/printing/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/printing/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    85648 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/printing/ccode.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4722 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/printing/codeprinter.py
+-rw-r--r--   0 yaman      (501) staff       (20)    69940 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/printing/cwrappercode.py
+-rw-r--r--   0 yaman      (501) staff       (20)   121337 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/printing/fcode.py
+-rw-r--r--   0 yaman      (501) staff       (20)    20480 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/printing/luacode.py
+-rw-r--r--   0 yaman      (501) staff       (20)    38538 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/printing/pycode.py
+-rw-r--r--   0 yaman      (501) staff       (20)     8082 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/python_wrapper.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7452 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/utilities.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.799020 pyccel-1.8.0/pyccel/codegen/wrapper/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/wrapper/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    20124 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/wrapper/fortran_to_c_wrapper.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3341 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/codegen/wrapper/wrapper.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.800264 pyccel-1.8.0/pyccel/commands/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/commands/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    12405 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/commands/console.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3461 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/commands/pyccel_clean.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1144 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/commands/pyccel_init.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.800753 pyccel-1.8.0/pyccel/compilers/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/compilers/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    10802 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/compilers/default_compilers.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.802230 pyccel-1.8.0/pyccel/complexity/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/complexity/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2780 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/complexity/arithmetic.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1145 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/complexity/basic.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7188 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/complexity/memory.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2358 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/decorators.py
+-rw-r--r--   0 yaman      (501) staff       (20)    13756 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/epyccel.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.803167 pyccel-1.8.0/pyccel/errors/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/errors/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    11261 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/errors/errors.py
+-rw-r--r--   0 yaman      (501) staff       (20)    11926 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/errors/messages.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.804945 pyccel-1.8.0/pyccel/naming/
+-rw-r--r--   0 yaman      (501) staff       (20)      791 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/naming/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3328 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/naming/cnameclashchecker.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4048 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/naming/fortrannameclashchecker.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1879 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/naming/languagenameclashchecker.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1810 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/naming/pythonnameclashchecker.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.807852 pyccel-1.8.0/pyccel/parser/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    16321 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/base.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9547 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/extend_tree.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.809572 pyccel-1.8.0/pyccel/parser/grammar/
+-rw-r--r--   0 yaman      (501) staff       (20)     2221 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/grammar/headers.tx
+-rw-r--r--   0 yaman      (501) staff       (20)      391 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/grammar/himi.tx
+-rw-r--r--   0 yaman      (501) staff       (20)     6361 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/grammar/openacc.tx
+-rw-r--r--   0 yaman      (501) staff       (20)     7307 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/grammar/openmp.tx
+-rw-r--r--   0 yaman      (501) staff       (20)     6539 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/grammar/pyccel.tx
+-rw-r--r--   0 yaman      (501) staff       (20)     7460 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/parser.py
+-rw-r--r--   0 yaman      (501) staff       (20)    21165 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/scope.py
+-rw-r--r--   0 yaman      (501) staff       (20)   159514 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/semantic.py
+-rw-r--r--   0 yaman      (501) staff       (20)    39500 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/syntactic.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.812335 pyccel-1.8.0/pyccel/parser/syntax/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/syntax/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2236 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/syntax/basic.py
+-rw-r--r--   0 yaman      (501) staff       (20)    19189 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/syntax/headers.py
+-rw-r--r--   0 yaman      (501) staff       (20)    36464 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/syntax/openacc.py
+-rw-r--r--   0 yaman      (501) staff       (20)    27508 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/syntax/openmp.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4079 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/parser/utilities.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.812926 pyccel-1.8.0/pyccel/stdlib/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/__init__.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.813804 pyccel-1.8.0/pyccel/stdlib/cwrapper/
+-rw-r--r--   0 yaman      (501) staff       (20)     4529 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/cwrapper/cwrapper.c
+-rw-r--r--   0 yaman      (501) staff       (20)     6528 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/cwrapper/cwrapper.h
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.814808 pyccel-1.8.0/pyccel/stdlib/cwrapper_ndarrays/
+-rw-r--r--   0 yaman      (501) staff       (20)    13567 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c
+-rw-r--r--   0 yaman      (501) staff       (20)     1927 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.817034 pyccel-1.8.0/pyccel/stdlib/external/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/external/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1749 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/external/dfftpack.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1112 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/external/fitpack.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1266 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/external/lapack.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9467 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/external/mpi4py.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.827080 pyccel-1.8.0/pyccel/stdlib/internal/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)    35216 2023-06-20 10:09:36.000000 pyccel-1.8.0/pyccel/stdlib/internal/blas.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)     7825 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/blas.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     5940 2023-06-20 10:09:36.000000 pyccel-1.8.0/pyccel/stdlib/internal/dfftpack.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)     1144 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/dfftpack.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     2841 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/fftw.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     2867 2023-06-20 10:09:36.000000 pyccel-1.8.0/pyccel/stdlib/internal/fitpack.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)      343 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/fitpack.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)    18250 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/hdf5.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)   354641 2023-06-20 10:09:37.000000 pyccel-1.8.0/pyccel/stdlib/internal/lapack.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)    58149 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/lapack.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)    25250 2023-06-20 10:09:37.000000 pyccel-1.8.0/pyccel/stdlib/internal/mpi.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)     5911 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/mpi.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     1226 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/mpiext.py
+-rw-r--r--   0 yaman      (501) staff       (20)    11017 2023-06-20 10:09:37.000000 pyccel-1.8.0/pyccel/stdlib/internal/openacc.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)     2675 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/openacc.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     8715 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/openmp.py
+-rw-r--r--   0 yaman      (501) staff       (20)    10053 2023-06-20 10:09:37.000000 pyccel-1.8.0/pyccel/stdlib/internal/openmp.pyccel
+-rw-r--r--   0 yaman      (501) staff       (20)     2645 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/internal/openmp.pyh
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.828463 pyccel-1.8.0/pyccel/stdlib/math/
+-rw-r--r--   0 yaman      (501) staff       (20)     1766 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/math/pyc_math_c.c
+-rw-r--r--   0 yaman      (501) staff       (20)     1331 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/math/pyc_math_c.h
+-rw-r--r--   0 yaman      (501) staff       (20)     3479 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/math/pyc_math_f90.f90
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.829402 pyccel-1.8.0/pyccel/stdlib/ndarrays/
+-rw-r--r--   0 yaman      (501) staff       (20)    11346 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/ndarrays/ndarrays.c
+-rw-r--r--   0 yaman      (501) staff       (20)     7152 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/ndarrays/ndarrays.h
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.831232 pyccel-1.8.0/pyccel/stdlib/numpy/
+-rw-r--r--   0 yaman      (501) staff       (20)      755 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/numpy/numpy_c.c
+-rw-r--r--   0 yaman      (501) staff       (20)      650 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/numpy/numpy_c.h
+-rw-r--r--   0 yaman      (501) staff       (20)     4629 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/numpy/numpy_f90.f90
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.832140 pyccel-1.8.0/pyccel/stdlib/parallel/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/parallel/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7487 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/stdlib/parallel/mpi.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.833033 pyccel-1.8.0/pyccel/symbolic/
+-rw-r--r--   0 yaman      (501) staff       (20)       48 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/symbolic/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4472 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/symbolic/lambdify.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.834774 pyccel-1.8.0/pyccel/utilities/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/utilities/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1350 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/utilities/metaclasses.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1227 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/utilities/stage.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2185 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/utilities/strings.py
+-rw-r--r--   0 yaman      (501) staff       (20)       86 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyccel/version.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.778818 pyccel-1.8.0/pyccel.egg-info/
+-rw-r--r--   0 yaman      (501) staff       (20)    13504 2023-06-20 10:09:39.000000 pyccel-1.8.0/pyccel.egg-info/PKG-INFO
+-rw-r--r--   0 yaman      (501) staff       (20)    24771 2023-06-20 10:09:39.000000 pyccel-1.8.0/pyccel.egg-info/SOURCES.txt
+-rw-r--r--   0 yaman      (501) staff       (20)        1 2023-06-20 10:09:39.000000 pyccel-1.8.0/pyccel.egg-info/dependency_links.txt
+-rw-r--r--   0 yaman      (501) staff       (20)      185 2023-06-20 10:09:39.000000 pyccel-1.8.0/pyccel.egg-info/entry_points.txt
+-rw-r--r--   0 yaman      (501) staff       (20)        1 2023-06-20 10:09:37.000000 pyccel-1.8.0/pyccel.egg-info/not-zip-safe
+-rw-r--r--   0 yaman      (501) staff       (20)      178 2023-06-20 10:09:39.000000 pyccel-1.8.0/pyccel.egg-info/requires.txt
+-rw-r--r--   0 yaman      (501) staff       (20)        7 2023-06-20 10:09:39.000000 pyccel-1.8.0/pyccel.egg-info/top_level.txt
+-rw-r--r--   0 yaman      (501) staff       (20)      225 2023-06-20 10:07:44.000000 pyccel-1.8.0/pyproject.toml
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.836014 pyccel-1.8.0/samples/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/samples/README.rst
+-rw-r--r--   0 yaman      (501) staff       (20)      385 2023-06-20 10:07:44.000000 pyccel-1.8.0/samples/mxm.py
+-rw-r--r--   0 yaman      (501) staff       (20)      564 2023-06-20 10:07:44.000000 pyccel-1.8.0/samples/mxm_openmp.py
+-rw-r--r--   0 yaman      (501) staff       (20)      950 2023-06-20 10:09:40.022721 pyccel-1.8.0/setup.cfg
+-rw-r--r--   0 yaman      (501) staff       (20)      628 2023-06-20 10:07:44.000000 pyccel-1.8.0/setup.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.837329 pyccel-1.8.0/tests/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.837771 pyccel-1.8.0/tests/ast/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.838713 pyccel-1.8.0/tests/ast/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      257 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/ast/scripts/cyclic_dependence.py
+-rw-r--r--   0 yaman      (501) staff       (20)      184 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/ast/scripts/math.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5580 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/ast/test_basic.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.757827 pyccel-1.8.0/tests/codegen/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.839182 pyccel-1.8.0/tests/codegen/ccode/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.842967 pyccel-1.8.0/tests/codegen/ccode/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      771 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/ccode/scripts/arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1558 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/ccode/scripts/arrays_create.py
+-rw-r--r--   0 yaman      (501) staff       (20)      754 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/ccode/scripts/arrays_indexing.py
+-rw-r--r--   0 yaman      (501) staff       (20)      616 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/ccode/scripts/arrays_pointers.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1320 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/ccode/scripts/arrays_slicing.py
+-rw-r--r--   0 yaman      (501) staff       (20)      876 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/ccode/scripts/functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      925 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/ccode/scripts/ifs.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1300 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/ccode/scripts/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)      378 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/ccode/scripts/whiles.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1734 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/ccode/test_ccode_codegen.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.843273 pyccel-1.8.0/tests/codegen/fcode/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.854785 pyccel-1.8.0/tests/codegen/fcode/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)     1280 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/CommentBlock.py
+-rw-r--r--   0 yaman      (501) staff       (20)      851 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/Functional_Stmts.py
+-rw-r--r--   0 yaman      (501) staff       (20)      401 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/ListComprehension.py
+-rw-r--r--   0 yaman      (501) staff       (20)      145 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/USELESS_EXPRESSION.py
+-rw-r--r--   0 yaman      (501) staff       (20)      229 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)      101 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/calls.py
+-rw-r--r--   0 yaman      (501) staff       (20)      646 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/classes.py
+-rw-r--r--   0 yaman      (501) staff       (20)      734 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/classes_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      735 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/classes_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1388 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/classes_4.py
+-rw-r--r--   0 yaman      (501) staff       (20)      295 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/complex_numbers.py
+-rw-r--r--   0 yaman      (501) staff       (20)      154 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/concatenation.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1160 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/context.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1272 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/decorators.py
+-rw-r--r--   0 yaman      (501) staff       (20)      294 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/decorators_elemental.py
+-rw-r--r--   0 yaman      (501) staff       (20)      163 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/decorators_pure.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1103 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/decorators_types.py
+-rw-r--r--   0 yaman      (501) staff       (20)      232 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/expressions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      574 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/functions_inout.py
+-rw-r--r--   0 yaman      (501) staff       (20)      480 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/generic_methods.py
+-rw-r--r--   0 yaman      (501) staff       (20)      425 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/headers.py
+-rw-r--r--   0 yaman      (501) staff       (20)      980 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/ifs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      264 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      485 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/issue_177.py
+-rw-r--r--   0 yaman      (501) staff       (20)      190 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/lists.py
+-rw-r--r--   0 yaman      (501) staff       (20)      838 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2002 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/macros.py
+-rw-r--r--   0 yaman      (501) staff       (20)      802 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/matrix_assembly.py
+-rw-r--r--   0 yaman      (501) staff       (20)      681 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/matrix_mul.py
+-rw-r--r--   0 yaman      (501) staff       (20)      257 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/multiple_assign.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1231 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/numpyext.py
+-rw-r--r--   0 yaman      (501) staff       (20)      782 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/precision.py
+-rw-r--r--   0 yaman      (501) staff       (20)      761 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/recursive_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      236 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/returns.py
+-rw-r--r--   0 yaman      (501) staff       (20)      359 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)      381 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/scripts/whiles.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1711 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/fcode/test_fcode_codegen.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.855089 pyccel-1.8.0/tests/codegen/pycode/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.855465 pyccel-1.8.0/tests/codegen/pycode/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)     1427 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/pycode/scripts/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1351 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/codegen/pycode/test_pycode_codegen.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.855765 pyccel-1.8.0/tests/complexity/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.856054 pyccel-1.8.0/tests/complexity/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      142 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/complexity/scripts/ex.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1053 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/complexity/test_complexity.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2253 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/conftest.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.874909 pyccel-1.8.0/tests/epyccel/
+-rw-r--r--   0 yaman      (501) staff       (20)      240 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/Module_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      238 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/README.rst
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.887069 pyccel-1.8.0/tests/epyccel/modules/
+-rw-r--r--   0 yaman      (501) staff       (20)      240 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/Module_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      315 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/Module_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      247 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/Module_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      338 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/Module_4.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1363 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/Module_5.py
+-rw-r--r--   0 yaman      (501) staff       (20)      698 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/Module_6.py
+-rw-r--r--   0 yaman      (501) staff       (20)      771 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/Module_7.py
+-rw-r--r--   0 yaman      (501) staff       (20)      234 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/Module_8.py
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      728 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/array_consts.py
+-rw-r--r--   0 yaman      (501) staff       (20)    47942 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2687 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/augassign.py
+-rw-r--r--   0 yaman      (501) staff       (20)      234 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/awkward_names.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3565 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/base.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1497 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/bitwise.py
+-rw-r--r--   0 yaman      (501) staff       (20)      845 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/call_user_defined_funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2001 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/complex_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      222 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/consts.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2284 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/external_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2092 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/functionals.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2227 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/generic_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4058 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/generic_functions_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4157 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/highorder_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4704 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1070 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/mpi_collective.py
+-rw-r--r--   0 yaman      (501) staff       (20)      530 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/mpi_point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2911 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/multi_rank.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5155 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/numpy_sign.py
+-rw-r--r--   0 yaman      (501) staff       (20)    14866 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/openmp.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1198 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/pointers.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1101 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/python_annotations.py
+-rw-r--r--   0 yaman      (501) staff       (20)      681 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/strings.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9815 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)      632 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/modules/types.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.888986 pyccel-1.8.0/tests/epyccel/recognised_functions/
+-rw-r--r--   0 yaman      (501) staff       (20)     2756 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py
+-rw-r--r--   0 yaman      (501) staff       (20)    37669 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/recognised_functions/test_math_funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)   247535 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/recognised_functions/test_numpy_funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)    45813 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/recognised_functions/test_numpy_types.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4693 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_array_as_func_args.py
+-rw-r--r--   0 yaman      (501) staff       (20)   100991 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)    10276 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_arrays_multiple_assignments.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6170 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_base.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5120 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_bitwise.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9648 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_builtins.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2537 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_class_expressions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1476 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_compare_expressions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      834 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_default_precision_template.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1191 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_docstrings.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7704 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_IfTernaryOperator.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9168 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_augassign.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3817 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_complex_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3136 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_decorators.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2377 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_default_args.py
+-rw-r--r--   0 yaman      (501) staff       (20)     8351 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_division.py
+-rw-r--r--   0 yaman      (501) staff       (20)     9369 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4662 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_generators.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2822 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_mod.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4652 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_modules.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5519 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_multi_rank.py
+-rw-r--r--   0 yaman      (501) staff       (20)    19588 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_openmp.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5681 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_optional_args.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6663 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_pow.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3265 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_python_annotations.py
+-rw-r--r--   0 yaman      (501) staff       (20)    30656 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_return_arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)    13388 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_sign.py
+-rw-r--r--   0 yaman      (501) staff       (20)     5823 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_transpose.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3471 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_epyccel_types.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3306 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_external_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2149 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_functionals.py
+-rw-r--r--   0 yaman      (501) staff       (20)    14120 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_generic_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1922 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_higherorder_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1841 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2208 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_kind.py
+-rw-r--r--   0 yaman      (501) staff       (20)     6036 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4164 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_mpi_collective.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2114 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_mpi_point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1040 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_multiple_results.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1735 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_parallel_epyccel.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1258 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_pointers.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7595 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_return.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1333 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_strings.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3200 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/test_tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)      704 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/epyccel/utilities.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.889419 pyccel-1.8.0/tests/errors/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.759995 pyccel-1.8.0/tests/errors/codegen/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.890231 pyccel-1.8.0/tests/errors/codegen/fortran/
+-rw-r--r--   0 yaman      (501) staff       (20)      108 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/codegen/fortran/FORTRAN_ALLOCATABLE_IN_EXPRESSION.py
+-rw-r--r--   0 yaman      (501) staff       (20)      131 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/codegen/fortran/randint.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.893930 pyccel-1.8.0/tests/errors/known_bugs/
+-rw-r--r--   0 yaman      (501) staff       (20)      236 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/known_bugs/cross.py
+-rw-r--r--   0 yaman      (501) staff       (20)      143 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/known_bugs/dicts.py
+-rw-r--r--   0 yaman      (501) staff       (20)      495 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/known_bugs/ex3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      796 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/known_bugs/ex4.py
+-rw-r--r--   0 yaman      (501) staff       (20)      654 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/known_bugs/generic_methods.py
+-rw-r--r--   0 yaman      (501) staff       (20)      579 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/known_bugs/header_interface.py
+-rw-r--r--   0 yaman      (501) staff       (20)      928 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/known_bugs/inheritance.py
+-rw-r--r--   0 yaman      (501) staff       (20)      180 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/known_bugs/lambdas.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.760827 pyccel-1.8.0/tests/errors/semantic/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.907095 pyccel-1.8.0/tests/errors/semantic/blocking/
+-rw-r--r--   0 yaman      (501) staff       (20)      128 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_0.py
+-rw-r--r--   0 yaman      (501) staff       (20)      208 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      174 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/COMPLEX_TYPE.py
+-rw-r--r--   0 yaman      (501) staff       (20)      159 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT.py
+-rw-r--r--   0 yaman      (501) staff       (20)      193 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      155 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/DECORATOR_WRONG_NUMBER_TYPES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      132 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      296 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
+-rw-r--r--   0 yaman      (501) staff       (20)      114 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED.py
+-rw-r--r--   0 yaman      (501) staff       (20)      145 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      315 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED3.py
+-rw-r--r--   0 yaman      (501) staff       (20)       94 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/INHOMOG_LIST.py
+-rw-r--r--   0 yaman      (501) staff       (20)      124 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/INIT_NDARRAY_WITH_INHOMOG_LIST.py
+-rw-r--r--   0 yaman      (501) staff       (20)      436 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/INTERFACE_WRONG_TYPES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      182 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/LIST_OF_TUPLES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      129 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/OPENMP_loop_check.py
+-rw-r--r--   0 yaman      (501) staff       (20)      102 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/OPENMP_parallel_for_check.py
+-rw-r--r--   0 yaman      (501) staff       (20)      131 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/OPENMP_simd_check.py
+-rw-r--r--   0 yaman      (501) staff       (20)      263 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_decorator.py
+-rw-r--r--   0 yaman      (501) staff       (20)      241 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_header.py
+-rw-r--r--   0 yaman      (501) staff       (20)      493 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/TEMPLATE_WRONG_TYPE_CALL.py
+-rw-r--r--   0 yaman      (501) staff       (20)      110 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/TOO_MANY_ARGS.py
+-rw-r--r--   0 yaman      (501) staff       (20)       92 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_FUNCTION.py
+-rw-r--r--   0 yaman      (501) staff       (20)       89 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_VARIABLE.py
+-rw-r--r--   0 yaman      (501) staff       (20)      108 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/UNRECOGNISED_FUNCTION_CALL.py
+-rw-r--r--   0 yaman      (501) staff       (20)      186 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/ex1.py
+-rw-r--r--   0 yaman      (501) staff       (20)       95 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/ex2.py
+-rw-r--r--   0 yaman      (501) staff       (20)       97 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/ex3.py
+-rw-r--r--   0 yaman      (501) staff       (20)       88 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/ex4.py
+-rw-r--r--   0 yaman      (501) staff       (20)       92 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/ex5.py
+-rw-r--r--   0 yaman      (501) staff       (20)      100 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/str_join.py
+-rw-r--r--   0 yaman      (501) staff       (20)      106 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/blocking/str_join2.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.916093 pyccel-1.8.0/tests/errors/semantic/non_blocking/
+-rw-r--r--   0 yaman      (501) staff       (20)      136 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT.py
+-rw-r--r--   0 yaman      (501) staff       (20)      150 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      152 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      118 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)       87 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      155 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_complex.py
+-rw-r--r--   0 yaman      (501) staff       (20)      149 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_float.py
+-rw-r--r--   0 yaman      (501) staff       (20)      147 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_integer.py
+-rw-r--r--   0 yaman      (501) staff       (20)      163 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_string.py
+-rw-r--r--   0 yaman      (501) staff       (20)      148 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_complex.py
+-rw-r--r--   0 yaman      (501) staff       (20)      142 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_float.py
+-rw-r--r--   0 yaman      (501) staff       (20)      140 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_integer.py
+-rw-r--r--   0 yaman      (501) staff       (20)      156 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_string.py
+-rw-r--r--   0 yaman      (501) staff       (20)      220 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/PYCCEL_RESTRICTION_LIST_COMPREHENSION_LIMITS.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/TOO_FEW_ARGS.py
+-rw-r--r--   0 yaman      (501) staff       (20)      118 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT.py
+-rw-r--r--   0 yaman      (501) staff       (20)       97 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      201 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/ex6.py
+-rw-r--r--   0 yaman      (501) staff       (20)      143 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/is.py
+-rw-r--r--   0 yaman      (501) staff       (20)      195 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/semantic/non_blocking/var_is_none.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.916794 pyccel-1.8.0/tests/errors/syntax_blockers/
+-rw-r--r--   0 yaman      (501) staff       (20)      286 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_blockers/ex1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      412 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_blockers/imports.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.922478 pyccel-1.8.0/tests/errors/syntax_errors/
+-rw-r--r--   0 yaman      (501) staff       (20)      371 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/TEMPLATE_WRONG_KEY.py
+-rw-r--r--   0 yaman      (501) staff       (20)      382 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/TEMPLATE_WRONG_NUMBER_ARGS.py
+-rw-r--r--   0 yaman      (501) staff       (20)       91 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/dict_str_keys.py
+-rw-r--r--   0 yaman      (501) staff       (20)      122 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/empty_class.py
+-rw-r--r--   0 yaman      (501) staff       (20)      206 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/functions_in_template.py
+-rw-r--r--   0 yaman      (501) staff       (20)      157 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/functions_in_uniontype.py
+-rw-r--r--   0 yaman      (501) staff       (20)      109 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/import_star.py
+-rw-r--r--   0 yaman      (501) staff       (20)      142 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/list_comprehension_no_assign.py
+-rw-r--r--   0 yaman      (501) staff       (20)       95 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/nargs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      125 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/not_implemented.py
+-rw-r--r--   0 yaman      (501) staff       (20)      114 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/raise.py
+-rw-r--r--   0 yaman      (501) staff       (20)      125 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/try.py
+-rw-r--r--   0 yaman      (501) staff       (20)      156 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/types_arg.py
+-rw-r--r--   0 yaman      (501) staff       (20)      137 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/types_arg_type.py
+-rw-r--r--   0 yaman      (501) staff       (20)       99 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/syntax_errors/yield.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4383 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/errors/test_errors.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.922916 pyccel-1.8.0/tests/external/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.761820 pyccel-1.8.0/tests/external/scripts/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.923243 pyccel-1.8.0/tests/external/scripts/lapack/
+-rw-r--r--   0 yaman      (501) staff       (20)     2401 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/lapack/ex1.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.929738 pyccel-1.8.0/tests/external/scripts/mpi4py/
+-rw-r--r--   0 yaman      (501) staff       (20)      334 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/allreduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      684 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/bcast.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.930454 pyccel-1.8.0/tests/external/scripts/mpi4py/bugs/
+-rw-r--r--   0 yaman      (501) staff       (20)      943 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/bugs/ex6.py
+-rw-r--r--   0 yaman      (501) staff       (20)      662 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/bugs/ex8.py
+-rw-r--r--   0 yaman      (501) staff       (20)      550 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/gather.py
+-rw-r--r--   0 yaman      (501) staff       (20)      468 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/np_Allreduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      765 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/np_Bcast.py
+-rw-r--r--   0 yaman      (501) staff       (20)      720 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/np_Gather.py
+-rw-r--r--   0 yaman      (501) staff       (20)      435 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/np_Reduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      524 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/np_Sendrecv.py
+-rw-r--r--   0 yaman      (501) staff       (20)      636 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/np_point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)      402 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/np_point_to_point_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1559 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/np_point_to_point_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      274 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)      367 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/point_to_point_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1559 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/point_to_point_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      339 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/reduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      364 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/sendrecv.py
+-rw-r--r--   0 yaman      (501) staff       (20)      240 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/scripts/mpi4py/who_am_i.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1362 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/external/test_external.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.930824 pyccel-1.8.0/tests/internal/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.763063 pyccel-1.8.0/tests/internal/scripts/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.933112 pyccel-1.8.0/tests/internal/scripts/blas/
+-rw-r--r--   0 yaman      (501) staff       (20)      559 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/blas/ex1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      890 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/blas/ex2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      584 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/blas/ex3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      920 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/blas/ex4.py
+-rw-r--r--   0 yaman      (501) staff       (20)      761 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/blas/ex5.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.933514 pyccel-1.8.0/tests/internal/scripts/lapack/
+-rw-r--r--   0 yaman      (501) staff       (20)     2779 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/lapack/ex1.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.938595 pyccel-1.8.0/tests/internal/scripts/mpi/
+-rw-r--r--   0 yaman      (501) staff       (20)     1401 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/allgather.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1205 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/allreduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1391 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/alltoall.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1129 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/bcast.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2057 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/column.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1477 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/gather.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2089 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/line.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1771 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/nonblocking.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1266 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/point_to_point_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3048 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/point_to_point_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1237 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/reduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1431 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/scatter.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1372 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/sendrecv.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1321 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/sendrecv_replace.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1740 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/split.py
+-rw-r--r--   0 yaman      (501) staff       (20)      772 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/mpi/who_am_i.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.939473 pyccel-1.8.0/tests/internal/scripts/openacc/
+-rw-r--r--   0 yaman      (501) staff       (20)      448 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/openacc/ex1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      619 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/openacc/sum.py
+-rw-r--r--   0 yaman      (501) staff       (20)      581 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/openacc/sum_kernels.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.940103 pyccel-1.8.0/tests/internal/scripts/openmp/
+-rw-r--r--   0 yaman      (501) staff       (20)      606 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/openmp/ex1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      412 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/scripts/openmp/ex2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3507 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/internal/test_internal.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.940397 pyccel-1.8.0/tests/macro/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.764251 pyccel-1.8.0/tests/macro/scripts/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.945780 pyccel-1.8.0/tests/macro/scripts/MPI/
+-rw-r--r--   0 yaman      (501) staff       (20)      447 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/allreduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      864 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/bcast.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.946519 pyccel-1.8.0/tests/macro/scripts/MPI/bug/
+-rw-r--r--   0 yaman      (501) staff       (20)     1586 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/bug/ex6.py
+-rw-r--r--   0 yaman      (501) staff       (20)      662 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/bug/ex8.py
+-rw-r--r--   0 yaman      (501) staff       (20)      788 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/gather.py
+-rw-r--r--   0 yaman      (501) staff       (20)     7929 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/mpi4py.py
+-rw-r--r--   0 yaman      (501) staff       (20)      548 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/np_Allreduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      898 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/np_Bcast.py
+-rw-r--r--   0 yaman      (501) staff       (20)      831 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/np_Gather.py
+-rw-r--r--   0 yaman      (501) staff       (20)      551 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/np_Reduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      567 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/np_Sendrecv.py
+-rw-r--r--   0 yaman      (501) staff       (20)      749 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/np_point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)      602 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/np_point_to_point_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1942 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/np_point_to_point_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      379 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/point_to_point.py
+-rw-r--r--   0 yaman      (501) staff       (20)      567 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/point_to_point_2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1952 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/point_to_point_3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      471 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/reduce.py
+-rw-r--r--   0 yaman      (501) staff       (20)      478 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/sendrecv.py
+-rw-r--r--   0 yaman      (501) staff       (20)      403 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/MPI/who_am_i.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.948695 pyccel-1.8.0/tests/macro/scripts/blas/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.948964 pyccel-1.8.0/tests/macro/scripts/blas/bugs/
+-rw-r--r--   0 yaman      (501) staff       (20)      363 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/blas/bugs/dnrm2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      681 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/blas/runtest_daxpy.py
+-rw-r--r--   0 yaman      (501) staff       (20)      467 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/blas/runtest_dcopy.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1148 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/blas/runtest_dgemm.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1186 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/blas/runtest_dgemv.py
+-rw-r--r--   0 yaman      (501) staff       (20)      756 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/blas/runtest_dger.py
+-rw-r--r--   0 yaman      (501) staff       (20)      482 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/blas/runtest_dscal.py
+-rw-r--r--   0 yaman      (501) staff       (20)      636 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/blas/runtest_dswap.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.949244 pyccel-1.8.0/tests/macro/scripts/lapack/
+-rw-r--r--   0 yaman      (501) staff       (20)      670 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/scripts/lapack/runtest_dgbtrf.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3214 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/macro/test_macro.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.950064 pyccel-1.8.0/tests/ndarrays/
+-rw-r--r--   0 yaman      (501) staff       (20)     4723 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/ndarrays/conftest.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1714 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/ndarrays/leaks_check.py
+-rw-r--r--   0 yaman      (501) staff       (20)    26585 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/ndarrays/test_ndarrays.c
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.951347 pyccel-1.8.0/tests/parser/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.951628 pyccel-1.8.0/tests/parser/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)     1074 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/parser/scripts/comments.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3490 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/parser/test_comments.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1468 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/parser/test_headers.py
+-rw-r--r--   0 yaman      (501) staff       (20)      358 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/parser/test_openacc.py
+-rw-r--r--   0 yaman      (501) staff       (20)      279 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/parser/test_openmp.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.951912 pyccel-1.8.0/tests/preprocess/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.952202 pyccel-1.8.0/tests/preprocess/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      943 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/preprocess/scripts/omp.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1017 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/preprocess/test_preprocess.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.952786 pyccel-1.8.0/tests/pyccel/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.953147 pyccel-1.8.0/tests/pyccel/project_abs_imports/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.953564 pyccel-1.8.0/tests/pyccel/project_abs_imports/project/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_abs_imports/project/__init__.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.953991 pyccel-1.8.0/tests/pyccel/project_abs_imports/project/folder1/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_abs_imports/project/folder1/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      305 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_abs_imports/project/folder1/mod1.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.954776 pyccel-1.8.0/tests/pyccel/project_abs_imports/project/folder2/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_abs_imports/project/folder2/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      227 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_abs_imports/project/folder2/mod2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      306 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_abs_imports/project/folder2/mod3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      214 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_abs_imports/runtest.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.956169 pyccel-1.8.0/tests/pyccel/project_multi_imports/
+-rw-r--r--   0 yaman      (501) staff       (20)      116 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_multi_imports/file1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_multi_imports/file2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_multi_imports/file3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      179 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_multi_imports/file4.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.956543 pyccel-1.8.0/tests/pyccel/project_rel_imports/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.956894 pyccel-1.8.0/tests/pyccel/project_rel_imports/project/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_rel_imports/project/__init__.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.957509 pyccel-1.8.0/tests/pyccel/project_rel_imports/project/folder1/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_rel_imports/project/folder1/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      305 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_rel_imports/project/folder1/mod1.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.958577 pyccel-1.8.0/tests/pyccel/project_rel_imports/project/folder2/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_rel_imports/project/folder2/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      221 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_rel_imports/project/folder2/mod2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      285 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_rel_imports/project/folder2/mod3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      214 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/project_rel_imports/runtest.py
+-rw-r--r--   0 yaman      (501) staff       (20)      199 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/run_import_function.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.974595 pyccel-1.8.0/tests/pyccel/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2969 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/array_binary_operation.py
+-rw-r--r--   0 yaman      (501) staff       (20)     4131 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/arrays_view.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.976410 pyccel-1.8.0/tests/pyccel/scripts/asserts/
+-rw-r--r--   0 yaman      (501) staff       (20)      117 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/asserts/unvalid_assert1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      138 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/asserts/unvalid_assert2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      162 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/asserts/unvalid_assert3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      217 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/asserts/valid_assert.py
+-rw-r--r--   0 yaman      (501) staff       (20)       68 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/basic_header.pyh
+-rw-r--r--   0 yaman      (501) staff       (20)     1410 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/bool_comp.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2132 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/c_arrays.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.977479 pyccel-1.8.0/tests/pyccel/scripts/classes/
+-rw-r--r--   0 yaman      (501) staff       (20)      726 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/classes/classes.py
+-rw-r--r--   0 yaman      (501) staff       (20)      590 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/classes/classes_1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      490 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/classes/classes_5.py
+-rw-r--r--   0 yaman      (501) staff       (20)      372 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/decorators_elemental.py
+-rw-r--r--   0 yaman      (501) staff       (20)      821 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/decorators_inline.py
+-rw-r--r--   0 yaman      (501) staff       (20)      915 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/default_args_mod.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.980491 pyccel-1.8.0/tests/pyccel/scripts/exits/
+-rw-r--r--   0 yaman      (501) staff       (20)      126 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/exits/empty_exit.py
+-rw-r--r--   0 yaman      (501) staff       (20)      150 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/exits/negative_exit1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/exits/negative_exit2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      127 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/exits/positive_exit1.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/exits/positive_exit2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      184 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/exits/positive_exit3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      127 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/exits/zero_exit.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2236 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/expressions.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.981298 pyccel-1.8.0/tests/pyccel/scripts/folder1/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/folder1/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      300 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/folder1/folder1_funcs.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.982735 pyccel-1.8.0/tests/pyccel/scripts/folder2/
+-rw-r--r--   0 yaman      (501) staff       (20)        0 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/folder2/__init__.py
+-rw-r--r--   0 yaman      (501) staff       (20)      300 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/folder2/folder2_funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      198 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/folder2/runtest_imports2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      189 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/folder2/runtest_rel_imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      300 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1154 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3617 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/generic_functions.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.985183 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/
+-rw-r--r--   0 yaman      (501) staff       (20)      285 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/hope_fib.py
+-rw-r--r--   0 yaman      (501) staff       (20)      591 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py
+-rw-r--r--   0 yaman      (501) staff       (20)      814 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py
+-rw-r--r--   0 yaman      (501) staff       (20)      265 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/hope_pisum.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1188 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      807 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/quicksort.py
+-rw-r--r--   0 yaman      (501) staff       (20)      280 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/simplify.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.987383 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/
+-rw-r--r--   0 yaman      (501) staff       (20)      309 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/fib.py
+-rw-r--r--   0 yaman      (501) staff       (20)      583 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py
+-rw-r--r--   0 yaman      (501) staff       (20)      826 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1226 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      824 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py
+-rw-r--r--   0 yaman      (501) staff       (20)      306 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/simplify.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.995375 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/
+-rw-r--r--   0 yaman      (501) staff       (20)      182 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/collisions2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      201 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/collisions3.py
+-rw-r--r--   0 yaman      (501) staff       (20)      218 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/collisions4.py
+-rw-r--r--   0 yaman      (501) staff       (20)      187 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/collisions5.py
+-rw-r--r--   0 yaman      (501) staff       (20)      922 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import.py
+-rw-r--r--   0 yaman      (501) staff       (20)      993 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import_as.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1002 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      287 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import_as_user.py
+-rw-r--r--   0 yaman      (501) staff       (20)      291 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import_as_user_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      943 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      290 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import_user.py
+-rw-r--r--   0 yaman      (501) staff       (20)      295 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import_user_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      934 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod.py
+-rw-r--r--   0 yaman      (501) staff       (20)      925 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod_as.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1019 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod_as_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      282 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod_as_user.py
+-rw-r--r--   0 yaman      (501) staff       (20)      287 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod_as_user_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1001 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      284 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod_user.py
+-rw-r--r--   0 yaman      (501) staff       (20)      288 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod_user_func.py
+-rw-r--r--   0 yaman      (501) staff       (20)      190 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/user_mod.py
+-rw-r--r--   0 yaman      (501) staff       (20)      174 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/import_syntax/user_mod2.py
+-rw-r--r--   0 yaman      (501) staff       (20)      882 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/lapack_subroutine.py
+-rw-r--r--   0 yaman      (501) staff       (20)      175 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/module_init.py
+-rw-r--r--   0 yaman      (501) staff       (20)      116 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/module_init2.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.996063 pyccel-1.8.0/tests/pyccel/scripts/numpy/
+-rw-r--r--   0 yaman      (501) staff       (20)     1590 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/numpy/numpy_kernels.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2812 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/numpy/numpy_sign.py
+-rw-r--r--   0 yaman      (501) staff       (20)      812 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/print_integers.py
+-rw-r--r--   0 yaman      (501) staff       (20)      885 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/print_sp_and_end.py
+-rw-r--r--   0 yaman      (501) staff       (20)     2056 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/print_strings.py
+-rw-r--r--   0 yaman      (501) staff       (20)      381 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/print_tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)      735 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/return_numpy_arrays.py
+-rw-r--r--   0 yaman      (501) staff       (20)      418 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_decorators_inline.py
+-rw-r--r--   0 yaman      (501) staff       (20)      736 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_default_args.py
+-rw-r--r--   0 yaman      (501) staff       (20)      673 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_degree_in.py
+-rw-r--r--   0 yaman      (501) staff       (20)      166 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_folder_imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      350 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_funcs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      324 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_function_alias.py
+-rw-r--r--   0 yaman      (501) staff       (20)      659 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_generic_functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      150 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      427 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_inoutfunc.py
+-rw-r--r--   0 yaman      (501) staff       (20)      167 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_module_init.py
+-rw-r--r--   0 yaman      (501) staff       (20)      305 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_module_init2.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1510 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_multiple_results.py
+-rw-r--r--   0 yaman      (501) staff       (20)      412 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/scripts/runtest_type_print.py
+-rw-r--r--   0 yaman      (501) staff       (20)    42779 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/pyccel/test_pyccel.py
+-rw-r--r--   0 yaman      (501) staff       (20)      844 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/run_tests.bat
+-rwxr-xr-x   0 yaman      (501) staff       (20)      899 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/run_tests_py3.sh
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:39.996405 pyccel-1.8.0/tests/semantic/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:40.000452 pyccel-1.8.0/tests/semantic/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      135 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/calls.py
+-rw-r--r--   0 yaman      (501) staff       (20)      506 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/classes.py
+-rw-r--r--   0 yaman      (501) staff       (20)      825 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/expressions.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1171 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      128 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/ifs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      197 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      141 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/lists.py
+-rw-r--r--   0 yaman      (501) staff       (20)      111 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)      307 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)      163 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/whiles.py
+-rw-r--r--   0 yaman      (501) staff       (20)      311 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/scripts/zeros.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1030 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/semantic/test_semantic.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:40.000883 pyccel-1.8.0/tests/symbolic/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:40.002488 pyccel-1.8.0/tests/symbolic/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      958 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/symbolic/scripts/decorator.py
+-rw-r--r--   0 yaman      (501) staff       (20)      283 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/symbolic/scripts/lambdas.py
+-rw-r--r--   0 yaman      (501) staff       (20)      711 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/symbolic/scripts/neural_net.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1263 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/symbolic/test_symbolic.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:40.003121 pyccel-1.8.0/tests/syntax/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:40.012479 pyccel-1.8.0/tests/syntax/scripts/
+-rw-r--r--   0 yaman      (501) staff       (20)      851 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/Functional_Stmts.py
+-rw-r--r--   0 yaman      (501) staff       (20)      157 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/annotated_comments.py
+-rw-r--r--   0 yaman      (501) staff       (20)       86 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/asserts.py
+-rw-r--r--   0 yaman      (501) staff       (20)       77 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/breaks.py
+-rw-r--r--   0 yaman      (501) staff       (20)      110 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/calls.py
+-rw-r--r--   0 yaman      (501) staff       (20)      796 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/class_member_index.py
+-rw-r--r--   0 yaman      (501) staff       (20)      369 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/classes.py
+-rw-r--r--   0 yaman      (501) staff       (20)       86 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/dels.py
+-rw-r--r--   0 yaman      (501) staff       (20)      190 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/dots.py
+-rw-r--r--   0 yaman      (501) staff       (20)      964 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/expressions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      193 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/functions.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/ifs.py
+-rw-r--r--   0 yaman      (501) staff       (20)      288 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/imports.py
+-rw-r--r--   0 yaman      (501) staff       (20)      142 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/lists.py
+-rw-r--r--   0 yaman      (501) staff       (20)      110 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/loops.py
+-rw-r--r--   0 yaman      (501) staff       (20)       80 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/prints.py
+-rw-r--r--   0 yaman      (501) staff       (20)      196 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/slice.py
+-rw-r--r--   0 yaman      (501) staff       (20)      142 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/tuples.py
+-rw-r--r--   0 yaman      (501) staff       (20)       92 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/whiles.py
+-rw-r--r--   0 yaman      (501) staff       (20)      311 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/scripts/zeros.py
+-rw-r--r--   0 yaman      (501) staff       (20)     1059 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/syntax/test_syntax.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:40.012945 pyccel-1.8.0/tests/warnings/
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:40.015922 pyccel-1.8.0/tests/warnings/semantic/
+-rw-r--r--   0 yaman      (501) staff       (20)      155 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/warnings/semantic/DECORATOR_WRONG_NUMBER_TYPES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      145 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/warnings/semantic/FOUND_DUPLICATED_IMPORT.py
+-rw-r--r--   0 yaman      (501) staff       (20)      130 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES.py
+-rw-r--r--   0 yaman      (501) staff       (20)      318 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
+-rw-r--r--   0 yaman      (501) staff       (20)      133 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/warnings/semantic/UNDEFINED_DECORATOR.py
+-rw-r--r--   0 yaman      (501) staff       (20)      141 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/warnings/semantic/UNDEFINED_DECORATORS.py
+-rw-r--r--   0 yaman      (501) staff       (20)     3007 2023-06-20 10:07:44.000000 pyccel-1.8.0/tests/warnings/test_warnings.py
+drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-06-20 10:09:40.021017 pyccel-1.8.0/tutorial/
+-rw-r--r--   0 yaman      (501) staff       (20)     1667 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/builtin-functions.md
+-rw-r--r--   0 yaman      (501) staff       (20)     3486 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/compiler.md
+-rw-r--r--   0 yaman      (501) staff       (20)     1779 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/const_keyword.md
+-rw-r--r--   0 yaman      (501) staff       (20)    15373 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/decorators.md
+-rw-r--r--   0 yaman      (501) staff       (20)    10633 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/function-pointers-as-arguments.md
+-rw-r--r--   0 yaman      (501) staff       (20)     3173 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/header-files.md
+-rw-r--r--   0 yaman      (501) staff       (20)     8825 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/ndarrays.md
+-rw-r--r--   0 yaman      (501) staff       (20)    16159 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/numpy-functions.md
+-rw-r--r--   0 yaman      (501) staff       (20)    18475 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/openmp.md
+-rw-r--r--   0 yaman      (501) staff       (20)    17344 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/quickstart.md
+-rw-r--r--   0 yaman      (501) staff       (20)     2505 2023-06-20 10:07:44.000000 pyccel-1.8.0/tutorial/templates.md
```

### Comparing `pyccel-1.7.4/LICENSE` & `pyccel-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/PKG-INFO` & `pyccel-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyccel
-Version: 1.7.4
+Version: 1.8.0
 Summary: UNKNOWN
 Home-page: https://github.com/pyccel/pyccel
 Author: Pyccel development team
 License: LICENSE
 Keywords: math
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pyccel-1.7.4/README.md` & `pyccel-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/basic.py` & `pyccel-1.8.0/pyccel/ast/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/bitwise_operators.py` & `pyccel-1.8.0/pyccel/ast/bitwise_operators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/builtin_imports.py` & `pyccel-1.8.0/pyccel/ast/builtin_imports.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/builtins.py` & `pyccel-1.8.0/pyccel/ast/builtins.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/c_concepts.py` & `pyccel-1.8.0/pyccel/ast/c_concepts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/class_defs.py` & `pyccel-1.8.0/pyccel/ast/class_defs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/core.py` & `pyccel-1.8.0/pyccel/ast/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1228,18 +1228,20 @@
         self._internal_dictionary.update({i.name:i for i in interfaces})
         self._internal_dictionary.update({c.name:c for c in classes})
         import_mods = {i.source: [t.object for t in i.target if isinstance(t.object, Module)] for i in imports}
         self._internal_dictionary.update({v:t[0] for v,t in import_mods.items() if t})
 
         if init_func:
             init_if = init_func.body.body[0]
-            init_cond = init_if.blocks[0].condition
-            init_var = init_cond.args[0]
-            self._variables.append(init_var)
-            self._variable_inits.append(LiteralFalse())
+            # The init function should always contain an If block unless it is part of a wrapper
+            if isinstance(init_if, If):
+                init_cond = init_if.blocks[0].condition
+                init_var = init_cond.args[0]
+                self._variables.append(init_var)
+                self._variable_inits.append(LiteralFalse())
 
         super().__init__(scope)
 
     @property
     def name(self):
         """ Name of the module
         """
```

### Comparing `pyccel-1.7.4/pyccel/ast/cwrapper.py` & `pyccel-1.8.0/pyccel/ast/cwrapper.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/datatypes.py` & `pyccel-1.8.0/pyccel/ast/datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,26 @@
 # NOTE: symbols not used in pyccel are commented out
 __all__ = (
 #
 # --------- CLASSES -----------
 #
     'CustomDataType',
     'DataType',
-    'FunctionType',
     'NativeBool',
     'NativeComplex',
     'NativeGeneric',
     'NativeInteger',
     'NativeTuple',
     'NativeNil',
     'NativeRange',
     'NativeFloat',
     'NativeString',
     'NativeSymbol',
     'NativeVoid',
     'UnionType',
-    'VariableType',
     'DataTypeFactory',
 #
 # --------- FUNCTIONS -----------
 #
     'datatype',
     'is_iterable_datatype',
     'is_pyccel_datatype',
@@ -192,44 +190,14 @@
     def __init__(self, name='__UNDEFINED__'):
         self._name = name
 
 class NativeGeneric(DataType):
     __slots__ = ()
     _name = 'Generic'
 
-
-# ...
-class VariableType(DataType):
-    __slots__ = ('_alias','_rhs','_name')
-
-    def __init__(self, rhs, alias):
-        self._alias = alias
-        self._rhs = rhs
-        self._name = rhs._name
-
-    @property
-    def alias(self):
-        return self._alias
-
-class FunctionType(DataType):
-    __slots__ = ('_domain','_codomain','_domains','_name')
-
-    def __init__(self, domains):
-        self._domain = domains[0]
-        self._codomain = domains[1:]
-        self._domains = domains
-        self._name = ' -> '.join('{}'.format(V) for V in self._domains)
-
-    @property
-    def domain(self):
-        return self._domain
-
-    @property
-    def codomain(self):
-        return self._codomain
 # ...
 
 
 
 Bool           = NativeBool()
 Int            = NativeInteger()
 Float          = NativeFloat()
```

### Comparing `pyccel-1.7.4/pyccel/ast/functionalexpr.py` & `pyccel-1.8.0/pyccel/ast/functionalexpr.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/headers.py` & `pyccel-1.8.0/pyccel/ast/headers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/internals.py` & `pyccel-1.8.0/pyccel/ast/internals.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/itertoolsext.py` & `pyccel-1.8.0/pyccel/ast/itertoolsext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/literals.py` & `pyccel-1.8.0/pyccel/ast/literals.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/macros.py` & `pyccel-1.8.0/pyccel/ast/macros.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/mathext.py` & `pyccel-1.8.0/pyccel/ast/mathext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/numpy_wrapper.py` & `pyccel-1.8.0/pyccel/ast/numpy_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     'pyarray_to_ndarray',
     #-------CHECK FUNCTIONS ------
     'array_type_check',
     'scalar_type_check',
     #-------HELPERS ------
     'array_get_dim',
     'array_get_data',
+    'array_get_c_step',
+    'array_get_f_step',
     #-------OTHERS--------
     'get_numpy_max_acceptable_version_file'
 )
 
 #-------------------------------------------------------------------
 #                      Numpy functions
 #-------------------------------------------------------------------
@@ -101,14 +103,26 @@
 # Return the shape of the n-th dimension : function definition in pyccel/stdlib/cwrapper/cwrapper_ndarrays.c
 array_get_dim  = FunctionDef(name    = 'nd_ndim',
                            body      = [],
                            arguments = [FunctionDefArgument(Variable(dtype=NativeVoid(), name = 'o', memory_handling='alias')),
                                         FunctionDefArgument(Variable(dtype=NativeInteger(), name = 'idx'))],
                            results   = [FunctionDefResult(Variable(dtype=NativeInteger(), name = 'd'))])
 
+# Return the stride of the n-th dimension : function definition in pyccel/stdlib/cwrapper/cwrapper_ndarrays.c
+array_get_c_step = FunctionDef(name    = 'nd_nstep_C',
+                           body      = [],
+                           arguments = [FunctionDefArgument(Variable(dtype=NativeVoid(), name = 'o', memory_handling='alias')),
+                                        FunctionDefArgument(Variable(dtype=NativeInteger(), name = 'idx'))],
+                           results   = [FunctionDefResult(Variable(dtype=NativeInteger(), name = 'd'))])
+array_get_f_step = FunctionDef(name    = 'nd_nstep_F',
+                           body      = [],
+                           arguments = [FunctionDefArgument(Variable(dtype=NativeVoid(), name = 'o', memory_handling='alias')),
+                                        FunctionDefArgument(Variable(dtype=NativeInteger(), name = 'idx'))],
+                           results   = [FunctionDefResult(Variable(dtype=NativeInteger(), name = 'd'))])
+
 # Return the data of ndarray : function definition in pyccel/stdlib/cwrapper/cwrapper_ndarrays.c
 array_get_data  = FunctionDef(name   = 'nd_data',
                            body      = [],
                            arguments = [FunctionDefArgument(Variable(dtype=NativeVoid(), name = 'o', memory_handling='alias'))],
                            results   = [FunctionDefResult(Variable(dtype=NativeVoid(), name = 'v', memory_handling='alias', rank = 1))])
 
 # Basic Array Flags
```

### Comparing `pyccel-1.7.4/pyccel/ast/numpyext.py` & `pyccel-1.8.0/pyccel/ast/numpyext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/omp.py` & `pyccel-1.8.0/pyccel/ast/omp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/operators.py` & `pyccel-1.8.0/pyccel/ast/operators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/scipyext.py` & `pyccel-1.8.0/pyccel/ast/scipyext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/sympy_helper.py` & `pyccel-1.8.0/pyccel/ast/sympy_helper.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/sysext.py` & `pyccel-1.8.0/pyccel/ast/sysext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/utilities.py` & `pyccel-1.8.0/pyccel/ast/utilities.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/ast/variable.py` & `pyccel-1.8.0/pyccel/ast/variable.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/codegen/codegen.py` & `pyccel-1.8.0/pyccel/codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/codegen/compiling/basic.py` & `pyccel-1.8.0/pyccel/codegen/compiling/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/codegen/compiling/compilers.py` & `pyccel-1.8.0/pyccel/codegen/compiling/compilers.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,26 +24,45 @@
     # https://developer.apple.com/documentation/macos-release-notes/macos-big-sur-11_0_1-release-notes#Third-Party-Apps
     p = subprocess.Popen([shutil.which("sw_vers"), "-productVersion"], stdout=subprocess.PIPE)
     result, err = p.communicate()
     mac_version_tuple = result.decode("utf-8").strip().split('.')
     mac_target = '{}.{}'.format(*mac_version_tuple[:2])
     os.environ['MACOSX_DEPLOYMENT_TARGET'] = mac_target
 
-def get_condaless_search_path():
-    """ Get the value of the PATH variable to be set when searching for the compiler.
-    This is the same as the environment PATH variable but without any conda paths
+
+def get_condaless_search_path(conda_warnings = 'basic'):
+    """
+    Get a list of paths excluding the conda paths.
+
+    Get the value of the PATH variable to be set when searching for the compiler
+    This is the same as the environment PATH variable but without any conda paths.
+
+    Parameters
+    ----------
+    conda_warnings : str, optional
+        Specify the level of Conda warnings to display (choices: off, basic, verbose), Default is 'basic'.
+
+    Returns
+    -------
+    str
+        A list of paths excluding the conda paths.
     """
     path_sep = ';' if platform.system() == 'Windows' else ':'
     current_path = os.environ['PATH']
     folders = {f: f.split(os.sep) for f in current_path.split(path_sep)}
     conda_folder_names = ('conda', 'anaconda', 'miniconda',
                           'Conda', 'Anaconda', 'Miniconda')
     conda_folders = [p for p,f in folders.items() if any(con in f for con in conda_folder_names)]
     if conda_folders:
-        warnings.warn(UserWarning("Ignoring conda paths when searching for compiler : {}".format(conda_folders)))
+        if conda_warnings in ('basic', 'verbose'):
+            message_warning = "Conda paths are ignored. See https://github.com/pyccel/pyccel/blob/devel/tutorial/compiler.md#utilising-pyccel-within-anaconda-environment for details"
+            if conda_warnings == 'verbose':
+                message_warning = message_warning + "\nConda ignored PATH:\n"
+                message_warning = message_warning + ":".join(conda_folders)
+            warnings.warn(UserWarning(message_warning))
     acceptable_search_paths = path_sep.join(p for p in folders.keys() if p not in conda_folders and os.path.exists(p))
     return acceptable_search_paths
 
 #------------------------------------------------------------
 class Compiler:
     """
     Class which handles all compiler options.
@@ -59,15 +78,15 @@
                Name of the family of compilers.
     language : str
                Language that we are translating to.
     debug : bool
                Indicates whether we are compiling in debug mode.
     """
     __slots__ = ('_debug','_info')
-    _acceptable_bin_paths = get_condaless_search_path()
+    acceptable_bin_paths = None
     def __init__(self, vendor : str, language : str, debug=False):
         if language=='python':
             return
         if vendor.endswith('.json') and os.path.exists(vendor):
             with open(vendor, encoding="utf-8") as vendor_file:
                 self._info = json.load(vendor_file)
             if language != self._info['language']:
@@ -80,20 +99,41 @@
                 self._info = available_compilers[(vendor,language)]
             except KeyError as e:
                 raise NotImplementedError("Compiler not available") from e
 
         self._debug = debug
 
     def _get_exec(self, accelerators):
+        """
+        Obtain the path of the executable based on the specified accelerators.
+
+        The `_get_exec` method is responsible for retrieving the path of the executable based on the specified accelerators.
+        It is used internally in the Pyccel module.
+
+        Parameters
+        ----------
+        accelerators : str
+            Specifies the accelerators to be used.
+
+        Returns
+        -------
+        str
+            The path of the executable corresponding to the specified accelerators.
+
+        Raises
+        ------
+        PyccelError
+            If the compiler executable cannot be found.
+        """
         # Get executable
         exec_cmd = self._info['mpi_exec'] if 'mpi' in accelerators else self._info['exec']
 
         # Clean conda paths out of the PATH variable
         current_path = os.environ['PATH']
-        os.environ['PATH'] = self._acceptable_bin_paths
+        os.environ['PATH'] = self.acceptable_bin_paths
 
         # Find the exact path of the executable
         exec_loc = shutil.which(exec_cmd)
 
         # Reset PATH variable
         os.environ['PATH'] = current_path
```

### Comparing `pyccel-1.7.4/pyccel/codegen/pipeline.py` & `pyccel-1.8.0/pyccel/codegen/pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,30 +6,32 @@
 """
 Contains the execute_pyccel function which carries out the main steps required to execute pyccel
 """
 
 import os
 import sys
 import shutil
+from pathlib import Path
 
 from pyccel.errors.errors          import Errors, PyccelError
 from pyccel.errors.errors          import PyccelSyntaxError, PyccelSemanticError, PyccelCodegenError
 from pyccel.errors.messages        import PYCCEL_RESTRICTION_TODO
 from pyccel.parser.parser          import Parser
 from pyccel.codegen.codegen        import Codegen
 from pyccel.codegen.utilities      import recompile_object
 from pyccel.codegen.utilities      import copy_internal_library
 from pyccel.codegen.utilities      import internal_libs
 from pyccel.codegen.python_wrapper import create_shared_library
 from pyccel.naming                 import name_clash_checkers
 from pyccel.utilities.stage        import PyccelStage
+from pyccel.ast.utilities          import python_builtin_libs
 from pyccel.parser.scope           import Scope
 
 from .compiling.basic     import CompileObj
-from .compiling.compilers import Compiler
+from .compiling.compilers import Compiler, get_condaless_search_path
 
 pyccel_stage = PyccelStage()
 
 __all__ = ['execute_pyccel']
 
 #==============================================================================
 # NOTE:
@@ -51,98 +53,75 @@
                    includes      = (),
                    libdirs       = (),
                    modules       = (),
                    libs          = (),
                    debug         = False,
                    accelerators  = (),
                    output_name   = None,
-                   compiler_export_file = None):
+                   compiler_export_file = None,
+                   conda_warnings = 'basic'):
     """
-    Carries out the main steps required to execute pyccel
+    Run Pyccel on the provided code.
+
+    Carry out the main steps required to execute Pyccel:
     - Parses the python file (syntactic stage)
     - Annotates the abstract syntax tree (semantic stage)
     - Generates the translated file(s) (codegen stage)
-    - Compiles the files to generate an executable and/or a shared library
+    - Compiles the files to generate an executable and/or a shared library.
 
     Parameters
     ----------
-    fname         : str
-                    Name of python file to be translated
-
-    syntax_only   : bool
-                    Boolean indicating whether the pipeline should stop
-                    after the syntax stage
-                    Default : False
-
-    semantic_only : bool
-                    Boolean indicating whether the pipeline should stop
-                    after the semantic stage
-                    Default : False
-
-    convert_only  : bool
-                    Boolean indicating whether the pipeline should stop
-                    after the codegen stage
-                    Default : False
-
-    verbose       : bool
-                    Boolean indicating whether debugging messages should be printed
-                    Default : False
-
-    folder        : str
-                    Path to the working directory
-                    Default : folder containing the file to be translated
-
-    language      : str
-                    The language which pyccel is translating to
-                    Default : fortran
-
-    compiler      : str
-                    The compiler used to compile the generated files
-                    Default : GNU
-
-    fflags        : str
-                    The flags passed to the compiler
-                    Default : provided by Compiler
-
-    wrapper_flags : str
-                    The flags passed to the compiler to compile the c wrapper
-                    Default : provided by Compiler
-
-    includes      : list
-                    list of include directories paths
-
-    libdirs       : list
-                    list of paths to directories containing the required libraries
-
-    modules       : list
-                    list of files which must also be compiled in order to compile this module
-
-    libs          : list
-                    list of required libraries
-
-    debug         : bool
-                    Boolean indicating whether the file should be compiled in debug mode
-                    (currently this only implies that the flag -fcheck=bounds is added)
-                    Default : False
-
-    accelerators  : iterable
-                    Tool used to accelerate the code (e.g. openmp openacc)
-
-    output_name   : str
-                    Name of the generated module
-                    Default : Same name as the file which was translated
-    export_compile_info : str
-                    Name of the json file to which compiler information is exported
-                    Default : None
+    fname : str
+        Name of the Python file to be translated.
+    syntax_only : bool, optional
+        Indicates whether the pipeline should stop after the syntax stage. Default is False.
+    semantic_only : bool, optional
+        Indicates whether the pipeline should stop after the semantic stage. Default is False.
+    convert_only : bool, optional
+        Indicates whether the pipeline should stop after the codegen stage. Default is False.
+    verbose : bool, optional
+        Indicates whether debugging messages should be printed. Default is False.
+    folder : str, optional
+        Path to the working directory. Default is the folder containing the file to be translated.
+    language : str, optional
+        The target language Pyccel is translating to. Default is 'fortran'.
+    compiler : str, optional
+        The compiler used to compile the generated files. Default is 'GNU'.
+    fflags : str, optional
+        The flags passed to the compiler. Default is provided by the Compiler.
+    wrapper_flags : str, optional
+        The flags passed to the compiler to compile the C wrapper. Default is provided by the Compiler.
+    includes : list, optional
+        List of include directory paths.
+    libdirs : list, optional
+        List of paths to directories containing the required libraries.
+    modules : list, optional
+        List of files that must be compiled in order to compile this module.
+    libs : list, optional
+        List of required libraries.
+    debug : bool, optional
+        Indicates whether the file should be compiled in debug mode. Default is False.
+        (Currently, this only implies that the flag -fcheck=bounds is added.).
+    accelerators : iterable, optional
+        Tool used to accelerate the code (e.g., OpenMP, OpenACC).
+    output_name : str, optional
+        Name of the generated module. Default is the same name as the translated file.
+    compiler_export_file : str, optional
+        Name of the JSON file to which compiler information is exported. Default is None.
+    conda_warnings : str, optional
+        Specify the level of Conda warnings to display (choices: off, basic, verbose), Default is 'basic'.
     """
     if fname.endswith('.pyh'):
         syntax_only = True
         if verbose:
             print("Header file recognised, stopping after syntactic stage")
 
+    if Path(fname).stem in python_builtin_libs:
+        raise ValueError(f"File called {os.path.basename(fname)} has the same name as a Python built-in package and can't be imported from Python. See #1402")
+
     # Reset Errors singleton before parsing a new file
     errors = Errors()
     errors.reset()
 
     # TODO [YG, 03.02.2020]: test validity of function arguments
 
     # Copy list arguments to local lists to avoid unexpected behavior
@@ -187,25 +166,29 @@
     os.makedirs(folder, exist_ok=True)
     if not (syntax_only or semantic_only):
         os.makedirs(pyccel_dirpath, exist_ok=True)
 
     # Change working directory to 'folder'
     os.chdir(folder)
 
+    if conda_warnings not in ('off', 'basic', 'verbose'):
+        raise ValueError("conda warnings accept {off, basic,verbose}")
+
     if language is None:
         language = 'fortran'
 
     # Choose Fortran compiler
     if compiler is None:
         compiler = 'GNU'
 
     fflags = [] if fflags is None else fflags.split()
     wrapper_flags = [] if wrapper_flags is None else wrapper_flags.split()
 
     # Get compiler object
+    Compiler.acceptable_bin_paths = get_condaless_search_path(conda_warnings)
     src_compiler = Compiler(compiler, language, debug)
     wrapper_compiler = Compiler('GNU', 'c', debug)
 
     # Export the compiler information if requested
     if compiler_export_file:
         src_compiler.export_compiler_info(compiler_export_file)
         if not fname:
```

### Comparing `pyccel-1.7.4/pyccel/codegen/printing/ccode.py` & `pyccel-1.8.0/pyccel/codegen/printing/ccode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1820,14 +1820,15 @@
     def _print_AugAssign(self, expr):
         op = expr.op
         lhs = expr.lhs
         rhs = expr.rhs
 
         if op == '%' and isinstance(lhs.dtype, NativeFloat):
             _expr = expr.to_basic_assign()
+            expr.invalidate_node()
             return self._print(_expr)
 
         lhs_code = self._print(lhs)
         rhs_code = self._print(rhs)
         return f'{lhs_code} {op}= {rhs_code};\n'
 
     def _print_Assign(self, expr):
```

### Comparing `pyccel-1.7.4/pyccel/codegen/printing/codeprinter.py` & `pyccel-1.8.0/pyccel/codegen/printing/codeprinter.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/codegen/printing/cwrappercode.py` & `pyccel-1.8.0/pyccel/codegen/printing/cwrappercode.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 
 from collections import OrderedDict
 
 from pyccel.codegen.printing.ccode import CCodePrinter
 
-from pyccel.ast.bind_c   import as_static_function, wrap_module_array_var, BindCPointer
+from pyccel.ast.bind_c   import BindCPointer
+from pyccel.ast.bind_c   import BindCModule, BindCFunctionDef, BindCFunctionDefArgument
+from pyccel.ast.bind_c   import BindCFunctionDefResult
 
 from pyccel.ast.builtins import PythonTuple, PythonType
 
 from pyccel.ast.core import Assign, AliasAssign, FunctionDef, FunctionAddress
 from pyccel.ast.core import If, IfSection, Return, FunctionCall, Deallocate
 from pyccel.ast.core import SeparatorComment, Allocate
 from pyccel.ast.core import Import, Module, Declare
@@ -32,15 +34,15 @@
 from pyccel.ast.datatypes import datatype, NativeVoid
 
 from pyccel.ast.literals  import LiteralTrue, LiteralInteger, LiteralString
 from pyccel.ast.literals  import Nil
 
 from pyccel.ast.numpy_wrapper   import array_type_check
 from pyccel.ast.numpy_wrapper   import pyarray_to_ndarray
-from pyccel.ast.numpy_wrapper   import array_get_data, array_get_dim
+from pyccel.ast.numpy_wrapper   import array_get_data, array_get_dim, array_get_c_step, array_get_f_step
 
 from pyccel.ast.operators import PyccelEq, PyccelNot, PyccelOr, PyccelAssociativeParenthesis
 from pyccel.ast.operators import PyccelIsNot, PyccelLt, PyccelUnarySub
 
 from pyccel.ast.variable  import Variable, DottedVariable
 
 from pyccel.ast.c_concepts import ObjectAddress
@@ -52,15 +54,15 @@
 errors = Errors()
 
 __all__ = ["CWrapperCodePrinter", "cwrappercode"]
 
 dtype_registry = {('pyobject'     , 0) : 'PyObject',
                   ('pyarrayobject', 0) : 'PyArrayObject',
                   ('void'         , 0) : 'void',
-                  ('bind_c_ptr'   , 0) : 'void*'}
+                  ('bind_c_ptr'   , 0) : 'void'}
 
 module_imports  = [Import('numpy_version', Module('numpy_version',(),())),
             Import('numpy/arrayobject', Module('numpy/arrayobject',(),())),
             Import('cwrapper', Module('cwrapper',(),()))]
 
 cwrapper_ndarray_import = Import('cwrapper_ndarrays', Module('cwrapper_ndarrays', (), ()))
 
@@ -120,14 +122,42 @@
         if isinstance(a.dtype, PyccelPyObject):
             return True
         elif isinstance(a, PyBuildValueNode):
             return True
         else:
             return CCodePrinter.is_c_pointer(self,a)
 
+    def get_python_name(self, scope, obj):
+        """
+        Get the name of object as defined in the original python code.
+
+        Get the name of the object as it was originally defined in the
+        Python code being translated. This name may have changed before
+        the printing stage in the case of name clashes or language interfaces.
+
+        Parameters
+        ----------
+        scope : pyccel.parser.scope.Scope
+            The scope where the object was defined.
+
+        obj : pyccel.ast.basic.Basic
+            The object whose name we wish to identify.
+
+        Returns
+        -------
+        str
+            The original name of the object.
+        """
+        if isinstance(obj, BindCFunctionDef):
+            return scope.get_python_name(obj.original_function.name)
+        elif isinstance(obj, BindCModule):
+            return obj.original_module.name
+        else:
+            return scope.get_python_name(obj.name)
+
     def function_signature(self, expr, print_arg_names = True):
         args = list(expr.arguments)
         if any([isinstance(a.var, FunctionAddress) for a in args]):
             # Functions with function addresses as arguments cannot be
             # exposed to python so there is no need to print their signature
             return ''
         else:
@@ -243,39 +273,14 @@
         elif isinstance(arg.dtype, (NativeFloat, NativeInteger, NativeBool)):
             return Assign(arg, value)
         elif isinstance(arg.dtype, PyccelPyObject):
             return AliasAssign(arg, Py_None)
         else:
             raise NotImplementedError('Default values are not implemented for this datatype : {}'.format(func_arg.dtype))
 
-    def get_static_function(self, function):
-        """
-
-        Create a static FunctionDef from the argument used for
-        C/fortran binding.
-        If target language is C return the argument function
-        If target language is Fortran, return a static function which
-        takes both the data and the shapes as arguments
-
-        Parameters
-        ----------
-        function    : FunctionDef
-            FunctionDef holding information needed to create static function
-
-        Returns   :
-        -----------
-        static_func : FunctionDef
-        """
-        if self._target_language == 'fortran':
-            static_func = as_static_function(function, mod_scope = self.scope)
-        else:
-            static_func = function
-
-        return static_func
-
     def static_function_signature(self, expr):
         """
         Get the C representation of the function signature using only basic types.
 
         Extract from the function definition `expr` all the
         information (name, input, output) needed to create the
         function signature used for C/Fortran binding and return
@@ -313,36 +318,61 @@
                         else self.get_static_declare_type(i)
                         for i in args)
 
         return f'{ret_type} {name}({arg_code})'
 
     def get_static_args(self, argument):
         """
-        Create bind_C arguments for arguments rank > 0 in fortran.
-        needed in static function call
-        func(a) ==> static_func(nd_dim(a) , nd_data(a))
-        where nd_data(a) = buffer holding data
-              nd_dim(a)  = size of array
+        Get the value(s) which should be passed for the provided argument.
+
+        Get the value(s) which should be passed to the function for the
+        specified argument. In the case of a BindCFunctionDef (when the
+        target language is Fortran) and an argument with rank > 0,
+        multiple arguments are needed:
+        - buffer holding data.
+        - shape of array in each dimension.
+        - stride for the array in each dimension.
 
         Parameters
         ----------
-        argument    : Variable
-            Variable holding information needed (rank)
+        argument : Variable
+            Variable holding information needed (rank).
 
-        Returns     : List of arguments
-            List that can contains Variables and FunctionCalls
-        -----------
+        Returns
+        -------
+        List of arguments
+            List that can contain Variables and FunctionCalls.
+
+        Examples
+        --------
+        If target language is Fortran:
+        >>> x = Variable('int', 'x', rank=2, order='c')
+        >>> self.get_static_args(x)
+        [&nd_data(x), nd_ndim(x, 0), nd_ndim(x, 1), nd_nstep_C(x, 0), nd_nstep_C(x, 1)]
+
+        If target language is C:
+        >>> x = Variable('int', 'x', rank=2, order='c')
+        >>> self.get_static_args(x)
+        [x]
         """
 
         if self._target_language == 'fortran' and argument.rank > 0:
             arg_address = ObjectAddress(argument)
-            static_args = [
+            static_args = [ObjectAddress(FunctionCall(array_get_data, [arg_address]))]
+            static_args+= [
                 FunctionCall(array_get_dim, [arg_address, i]) for i in range(argument.rank)
             ]
-            static_args.append(ObjectAddress(FunctionCall(array_get_data, [arg_address])))
+            if argument.order == 'C':
+                static_args+= [
+                    FunctionCall(array_get_c_step, [arg_address, i]) for i in range(argument.rank)
+                ]
+            else:
+                static_args+= [
+                    FunctionCall(array_get_f_step, [arg_address, i]) for i in range(argument.rank)
+                ]
         else:
             static_args = [argument]
 
         return static_args
 
     def get_static_declare_type(self, variable):
         """
@@ -363,97 +393,115 @@
         """
         dtype = self._print(variable.dtype)
         prec  = variable.precision
 
         dtype = self.find_in_dtype_registry(dtype, prec)
 
         if self.is_c_pointer(variable):
-            return '{0}*'.format(dtype)
-
-        elif self._target_language == 'fortran' and variable.rank > 0:
-            return '{0}*'.format(dtype)
+            return f'{dtype}*'
 
         else:
-            return '{0}'.format(dtype)
+            return dtype
 
     def get_static_results(self, result):
         """
-        Create bind_C results for results rank > 0 in fortran.
-        needed in static function call
-        func(a) ==> static_func(a.shape[0] , &a->raw_data)
+        Get the value(s) which should be used to collect the provided result.
+
+        Get the value(s) which should be collected from the function for the
+        specified argument. In the case of a BindCFunctionDefResult (when the
+        target language is Fortran) and an argument with rank > 0,
+        multiple outputs are needed:
+        - buffer holding data.
+        - shape of array in each dimension.
+        These must then be used to create the expected result variable.
 
         Parameters
         ----------
-        result      : Variable
-            Variable holding information needed (rank)
+        result : FunctionDefResult
+            The result of the function which we want to collect.
 
         Returns
         -------
         body : list
-            Additional instructions (allocations and pointer assignments) for function body
+            Additional instructions (allocations and pointer assignments) for function body.
 
         static_results : list
-            Expanded list of function arguments corresponding to the given result
+            Expanded list of function arguments corresponding to the given result.
+
+        Examples
+        --------
+        If target language is Fortran:
+        >>> x_res = BindCFunctionDefResult(Variable(BindCPointer(), 'x_ptr', memory_handling='alias'), Variable('int', 'x', rank=2, order='c'), scope)
+        >>> self.get_static_results(x)
+        [allocate(x, [x_shape_0, x_shape_1]), x.raw_data=>x_ptr], [&nd_data(x_ptr), x_shape_0, x_shape_1]
+
+        If target language is C:
+        >>> x_res = FunctionDefResult(Variable('int', 'x', rank=2, order='c'))
+        >>> self.get_static_args(x)
+        [], [Variable(x)]
         """
 
         body = []
+        var_name = self.scope.get_expected_name(result.var.name)
 
-        if self._target_language == 'fortran' and result.rank > 0:
-            sizes = [
-                     self.scope.get_temporary_variable(NativeInteger(),
-                         result.name+'_size') for _ in range(result.rank)
-                     ]
-            nd_var = self.scope.get_temporary_variable(dtype_or_var = NativeVoid(),
-                    name = result.name,
-                    memory_handling = 'alias')
-            body.append(Allocate(result, shape = sizes, order = result.order,
+        if isinstance(result, BindCFunctionDefResult) and result.shape:
+            shape = [self.scope.get_temporary_variable(s) for s in result.shape]
+            orig_name = result.original_function_result_variable.name
+            orig_var = self.scope.find(self.scope.get_expected_name(orig_name), category='variables')
+            nd_var = self.scope.find(var_name, category='variables')
+            body.append(Allocate(orig_var, shape = shape, order = orig_var.order,
                 status='unallocated'))
             body.append(AliasAssign(DottedVariable(NativeVoid(), 'raw_data', memory_handling = 'alias',
-                lhs=result), nd_var))
+                lhs=orig_var), nd_var))
 
-            static_results = [ObjectAddress(nd_var), *sizes]
+            static_results = [ObjectAddress(nd_var), *shape]
 
         else:
-            static_results = [result]
+            var = self.scope.find(var_name, category='variables')
+            static_results = [var]
 
         return body, static_results
 
     def _get_static_func_call_code(self, expr, static_func_args, results):
         """
-        Get all code necessary to call the wrapped function
+        Get all code necessary to call the wrapped function.
+
+        Get the function call which calls the underlying translated function
+        being wrapped. This may involve creating new variables in order to
+        call the function in a compatible way.
 
         Parameters
         ----------
-        expr             : FunctionDef
-                           The function being wrapped
+        expr : FunctionDef
+            The function being wrapped.
+
         static_func_args : List of arguments
-                           Arguments compatible with the static function
-        results          : List of results
-                           Results of the wrapped function
+            Arguments compatible with the static function.
+
+        results : List of results
+            Results of the wrapped function.
 
         Returns
         -------
-        body             : List of Basic Nodes
-                           List of nodes describing the instructions which call the
-                           wrapped function
-
+        list of pyccel.ast.basic.Basic
+            List of nodes describing the instructions which call the
+            wrapped function.
         """
         body = []
-        static_function = self.get_static_function(expr)
         if len(results) == 0:
-            body.append(FunctionCall(static_function, static_func_args))
+            body.append(FunctionCall(expr, static_func_args))
         else:
             static_func_results = []
             for r in results:
                 b, s = self.get_static_results(r)
                 body.extend(b)
                 static_func_results.extend(s)
 
             results   = static_func_results if len(static_func_results)>1 else static_func_results[0]
-            func_call = Assign(results,FunctionCall(static_function, static_func_args))
+            func_call = Assign(results,FunctionCall(expr, static_func_args))
             body.insert(0, func_call)
 
         return body
 
     def _get_check_type_statement(self, variable, collect_var, compulsory):
         """
         Check if the provided variable has the expected type.
@@ -782,36 +830,41 @@
         collect_var  = Variable(dtype = collect_type,
                             memory_handling='alias',
                             name=self.scope.get_new_name(variable.name+"_tmp"))
         self.scope.insert_variable(collect_var)
 
         return collect_var
 
-    def get_PyBuildValue(self, variable):
+    def get_PyBuildValue(self, result):
         """
+        Get the necessary objects for calling PyBuildValue.
+
         Responsible for collecting the variable required to build the result
-        and the necessary cast function
+        using the Python function PyBuildValue. Also responsible for creating
+        the necessary cast function which creates this variable.
 
         Parameters
         ----------
-        variable : Variable
-            The variable returned by the translated function
+        result : Variable
+            The variable returned by the translated function.
 
         Returns
         -------
-        collect_var : Variable
-            The variable which will be provided to PyBuild
+        Variable
+            The variable which will be provided to PyBuild.
 
-        cast_func_stmts : functionCall
-            call to cast function responsible for the conversion of one data type into another
+        FunctionCall
+            Call to cast function responsible for the conversion of one data type into another.
         """
+        out_var = getattr(result, 'original_function_result_variable', result.var)
+        name = self.scope.get_expected_name(out_var.name)
+        variable = self.scope.find(name, category='variables')
         if variable.rank != 0:
             self.add_import(cwrapper_ndarray_import)
 
-
         cast_function = FunctionCall(C_to_Python(variable), [ObjectAddress(variable)])
 
         collect_type = PyccelPyObject()
         collect_var = Variable(dtype = collect_type, memory_handling='alias',
             name = self.scope.get_new_name(variable.name+"_tmp"))
         self.scope.insert_variable(collect_var)
         self._to_free_PyObject_list.append(collect_var) #TODO remove in next PR
@@ -880,41 +933,42 @@
         mod_var_name = self.scope.get_new_name('m')
         mod_var = Variable(dtype = PyccelPyObject(),
                       name       = mod_var_name,
                       memory_handling = 'alias')
         scope.insert_variable(mod_var)
 
         # Collect module variables from translated code
-        orig_vars_to_wrap = [v for v in expr.variables if not v.is_private]
         body = []
-        if self._target_language == 'fortran':
+        if isinstance(expr, BindCModule):
+            orig_vars_to_wrap = [v for v in expr.original_module.variables if not v.is_private]
+            wrapper_funcs = {f.original_function: f for f in expr.variable_wrappers}
             # Collect python compatible module variables
             vars_to_wrap = []
             for v in orig_vars_to_wrap:
-                if v.rank > 0:
+                if v in wrapper_funcs:
                     # Get pointer to store array data
                     var = scope.get_temporary_variable(dtype_or_var = v,
                             name = v.name,
                             memory_handling = 'alias',
                             rank = 0, shape = None, order = None)
-                    # Create variables to store sizes of array
-                    sizes = [scope.get_temporary_variable(NativeInteger(),
+                    # Create variables to store the shape of the array
+                    shape = [scope.get_temporary_variable(NativeInteger(),
                             v.name+'_size') for _ in range(v.rank)]
                     # Get the bind_c function which wraps a fortran array and returns c objects
-                    var_wrapper = wrap_module_array_var(v, scope, expr)
+                    var_wrapper = wrapper_funcs[v]
                     # Call bind_c function
-                    call = Assign(PythonTuple(ObjectAddress(var), *sizes), FunctionCall(var_wrapper, ()))
+                    call = Assign(PythonTuple(ObjectAddress(var), *shape), FunctionCall(var_wrapper, ()))
                     body.append(call)
 
                     # Create ndarray to store array data
                     nd_var = self.scope.get_temporary_variable(dtype_or_var = v,
                             name = v.name,
                             memory_handling = 'alias'
                             )
-                    alloc = Allocate(nd_var, shape=sizes, order=nd_var.order, status='unallocated')
+                    alloc = Allocate(nd_var, shape=shape, order=nd_var.order, status='unallocated')
                     body.append(alloc)
                     # Save raw_data into ndarray to obtain useable pointer
                     set_data = AliasAssign(DottedVariable(NativeVoid(), 'raw_data',
                             memory_handling = 'alias', lhs=nd_var), var)
                     body.append(set_data)
                     # Save the ndarray to vars_to_wrap to be handled as if it came from C
                     vars_to_wrap.append(nd_var)
@@ -924,32 +978,32 @@
                     assign = v.get_user_nodes(Assign)[0]
                     # assign.fst should always exist, but is not always set when the
                     # Assign is created in the codegen stage
                     if assign.fst:
                         w.set_fst(assign.fst)
                     vars_to_wrap.append(w)
         else:
+            orig_vars_to_wrap = [v for v in expr.variables if not v.is_private]
             vars_to_wrap = orig_vars_to_wrap
-        var_names = [str(expr.scope.get_python_name(v.name)) for v in orig_vars_to_wrap]
+        var_names = [str(self.get_python_name(expr.scope, v)) for v in orig_vars_to_wrap]
 
         # If there are any variables in the module then add them to the module object
         if vars_to_wrap:
             # Create variable for temporary python objects
             tmp_var_name = self.scope.get_new_name('tmp')
             tmp_var = Variable(dtype = PyccelPyObject(),
                           name       = tmp_var_name,
                           memory_handling = 'alias')
             scope.insert_variable(tmp_var)
             # Add code to add variable to module
             body.extend(l for n,v in zip(var_names,vars_to_wrap) for l in self.insert_constant(mod_var_name, n, v, tmp_var))
 
         if expr.init_func:
             # Call init function code
-            static_function = self.get_static_function(expr.init_func)
-            body.insert(0,FunctionCall(static_function,[],[]))
+            body.insert(0,FunctionCall(expr.init_func,[],[]))
 
         body.append(Return([LiteralInteger(0)]))
         self.exit_scope()
 
         func = FunctionDef(name = exec_func_name,
             arguments = (FunctionDefArgument(mod_var),),
             results = (FunctionDefResult(scope.get_temporary_variable(NativeInteger(),
@@ -990,31 +1044,41 @@
             self.scope.insert_symbol(n.name)
 
         # Collect arguments and results
         wrapper_args    = self.get_wrapper_arguments()
         wrapper_results = [self.get_new_PyObject("result")]
         self.scope.insert_variable(wrapper_results[0])
 
+        if isinstance(funcs[0], BindCFunctionDef):
+            example_args = funcs[0].bind_c_arguments
+            example_arg_vars = {(a.original_function_argument_variable if isinstance(a, BindCFunctionDefArgument) else a.var): a \
+                    for a in example_args}
+            arg_names = [a.var.name for a in funcs[0].original_function.arguments]
+        else:
+            example_args = funcs[0].arguments
+            example_arg_vars = {(a.original_function_argument_variable if isinstance(a, BindCFunctionDefArgument) else a.var): a \
+                    for a in example_args}
+            arg_names = [a.name for a in example_args]
+
         # Collect argument names for PyArgParse
-        arg_names         = [a.name for a in funcs[0].arguments]
         keyword_list_name = self.scope.get_new_name('kwlist')
         keyword_list      = PyArgKeywords(keyword_list_name, arg_names)
         wrapper_body      = [keyword_list]
 
         wrapper_body_translations = []
         body_tmp = []
 
         # To store the mini function responsible for collecting value and calling interfaces functions and return the builded value
         funcs_def = []
         default_value = {} # dict to collect all initialisation needed in the wrapper
         check_var = Variable(dtype = NativeInteger(), name = self.scope.get_new_name("check"))
         scope.insert_variable(check_var, check_var.name)
-        types_dict = OrderedDict((a.var, set()) for a in funcs[0].arguments) #dict to collect each variable possible type and the corresponding flags
+        types_dict = OrderedDict((a, set()) for a in example_arg_vars) #dict to collect each variable possible type and the corresponding flags
         # collect parse arg
-        parse_args = [self.get_PyArgParseType(a.var) for a in funcs[0].arguments]
+        parse_args = [self.get_PyArgParseType(a) for a in example_arg_vars]
 
         # Determine flags which indicate argument type
         argument_type_flags = self._determine_interface_flags(funcs)
 
         # Managing the body of wrapper
         for func in funcs :
             mini_wrapper_func_body = []
@@ -1022,23 +1086,45 @@
             static_func_args  = []
 
             mini_wrapper_func_name = self.scope.get_new_name(func.name + '_mini_wrapper')
             mini_scope = mod_scope.new_child_scope(mini_wrapper_func_name)
             self.set_scope(mini_scope)
 
             # update ndarray local variables properties
-            arg_vars = {a.var: a for a in func.arguments}
-            result_vars = [r.var for r in func.results]
+            if isinstance(func, BindCFunctionDef):
+                arg_vars = {(a.original_function_argument_variable if isinstance(a, BindCFunctionDefArgument) else a.var): a \
+                        for a in func.bind_c_arguments}
+            else:
+                arg_vars = {(a.original_function_argument_variable if isinstance(a, BindCFunctionDefArgument) else a.var): a \
+                        for a in func.arguments}
+            results = func.bind_c_results if isinstance(func, BindCFunctionDef) else func.results
+            result_vars = []
+            for r in results:
+                var = r.var
+                name = var.name
+                self.scope.insert_symbol(name)
+                if var.rank > 0:
+                    v = var.clone(self.scope.get_expected_name(name), memory_handling = 'alias')
+                else:
+                    v = var.clone(self.scope.get_expected_name(name))
+                result_vars.append(v)
+                self.scope.insert_variable(v)
+                if isinstance(r, BindCFunctionDefResult) and r.shape:
+                    original_var = r.original_function_result_variable
+                    original_name = original_var.name
+                    self.scope.insert_symbol(original_name)
+                    # Declare as pointer as the array should not free its data when it goes out of scope
+                    self.scope.insert_variable(original_var.clone(self.scope.get_expected_name(original_name), memory_handling = 'alias'))
+
             local_arg_vars = {(v.clone(v.name, memory_handling='alias')
                               if isinstance(v, Variable) and v.rank > 0 or v.is_optional \
                               else v) : a for v,a in arg_vars.items()}
+
             for a in local_arg_vars:
                 mini_scope.insert_variable(a)
-            for r in result_vars:
-                mini_scope.insert_variable(r)
 
             # Loop for all args in every functions and create the corresponding condition and body
             for idx, (p_arg, (f_var, f_arg)) in enumerate(zip(parse_args, local_arg_vars.items())):
                 collect_var  = self.get_PyArgParseType(f_var)
                 body, tmp_variable = self._body_management(f_var, p_arg, f_arg.value)
 
                 # get check type function
@@ -1058,32 +1144,39 @@
                 flag_value = argument_type_flags[func][idx]
                 if flag_value >= len(types_dict[f_var]):
                     types_dict[f_var].add((f_var, check, flag_value)) # collect variable type for each arguments
 
                 mini_wrapper_func_body += body
 
             # create the corresponding function call
-            mini_wrapper_func_body.extend(self._get_static_func_call_code(func, static_func_args, result_vars))
+            mini_wrapper_func_body.extend(self._get_static_func_call_code(func, static_func_args, results))
 
 
             # Loop for all res in every functions and create the corresponding body and cast
-            for r in result_vars :
+            for r in results :
                 collect_var, cast_func = self.get_PyBuildValue(r)
                 if cast_func is not None:
                     mini_wrapper_func_body.append(AliasAssign(collect_var, cast_func))
 
                 res_args.append(ObjectAddress(collect_var) if collect_var.is_alias else collect_var)
 
             # Building PybuildValue and freeing the allocated variable after.
             mini_wrapper_func_body.append(AliasAssign(wrapper_results[0],PyBuildValueNode(res_args)))
             mini_wrapper_func_body += [FunctionCall(Py_DECREF, [i]) for i in self._to_free_PyObject_list]
 
             # Call free function for C type
             mini_wrapper_func_body += [If(IfSection(PyccelIsNot(i, Nil()), [Deallocate(i)])) if self.is_c_pointer(i) \
                                         else Deallocate(i) for i in local_arg_vars if i.rank > 0]
+            if self._target_language == 'fortran':
+                dealloc_results = [self.scope.find(self.scope.get_expected_name(r.original_function_result_variable.name), category='variables')
+                                    for r in results]
+            else:
+                dealloc_results = result_vars
+            mini_wrapper_func_body += [If(IfSection(PyccelIsNot(i, Nil()), [Deallocate(i)])) if self.is_c_pointer(i) \
+                                else Deallocate(i) for i in dealloc_results if i.rank > 0]
             mini_wrapper_func_body.append(Return(wrapper_results))
             self._to_free_PyObject_list.clear()
 
             self.set_scope(scope)
 
             # Building Mini wrapper function
             mini_wrapper_func_def = FunctionDef(name = mini_wrapper_func_name,
@@ -1107,15 +1200,15 @@
         body_tmp.append(IfSection(LiteralTrue(),
             [set_python_error_message('PyExc_TypeError', '"This combination of arguments is not valid"'),
             Return([Nil()])]))
         wrapper_body_translations = [If(*body_tmp)]
 
         # Parsing Arguments
         parse_node = PyArg_ParseTupleNode(*wrapper_args[1:],
-                                          funcs[0].arguments,
+                                          example_args,
                                           parse_args, keyword_list)
 
         wrapper_body += list(default_value.values())
         wrapper_body.append(If(IfSection(PyccelNot(parse_node), [Return([Nil()])])))
 
         #finishing the wrapper body
         wrapper_body.append(Assign(check_var, FunctionCall(check_func_def, parse_args)))
@@ -1173,19 +1266,20 @@
         Returns
         -------
         dict
             A dictionary whose keys are the functions and whose values are a list of integers
             which should be used to increment the byte flag if the argument at the same index
             has the type expected by the function.
         """
+        orig_funcs = [func.original_function if isinstance(func, BindCFunctionDef) else func for func in funcs]
         argument_type_flags = {func:[] for func in funcs}
-        nargs = len(funcs[0].arguments)
+        nargs = len(orig_funcs[0].arguments)
         step = 1
         for i in range(nargs):
-            interface_args = [func.arguments[i].var for func in funcs]
+            interface_args = [getattr(func.arguments[i], 'original_function_argument_variable', func.arguments[i].var) for func in orig_funcs]
             interface_types = [(a.dtype, a.precision) for a in interface_args]
             possible_types = list(dict.fromkeys(interface_types)) # Remove duplicates but preserve order
             for func, t in zip(funcs, interface_types):
                 argument_type_flags[func].append(possible_types.index(t)*step)
             step *= len(possible_types)
         return argument_type_flags
 
@@ -1304,43 +1398,60 @@
                 self._print(expr.name),
                 self._print(expr.variable))
 
     def _print_FunctionDef(self, expr):
         self.set_scope(self.scope.new_child_scope(expr.name))
 
         local_arg_vars = {}
-        for a in expr.arguments:
-            v = a.var
+        args = expr.bind_c_arguments if isinstance(expr, BindCFunctionDef) else expr.arguments
+        for a in args:
+            v = (a.original_function_argument_variable if isinstance(a, BindCFunctionDefArgument) else a.var)
             if isinstance(v, Variable):
                 new_name = self.scope.get_new_name(v.name)
                 if isinstance(v, Variable) and (v.rank > 0 or v.is_optional):
                     new_v = v.clone(new_name, memory_handling='alias')
                 else:
                     new_v = v.clone(new_name)
                 local_arg_vars[new_v] = a
                 self.scope.insert_variable(new_v)
             else:
                 self.scope.functions[v.name] = v
                 local_arg_vars[v] = a
 
-        result_vars = [v.var.clone(self.scope.get_new_name(v.var.name)) for v in expr.results]
-        for v in result_vars:
+        results = expr.bind_c_results if isinstance(expr, BindCFunctionDef) else expr.results
+        result_vars = []
+        for r in results:
+            var = r.var
+            name = var.name
+            self.scope.insert_symbol(name)
+            if var.rank > 0:
+                v = var.clone(self.scope.get_expected_name(name), memory_handling = 'alias')
+            else:
+                v = var.clone(self.scope.get_expected_name(name))
+            result_vars.append(v)
             self.scope.insert_variable(v)
+            if isinstance(r, BindCFunctionDefResult) and r.shape:
+                original_var = r.original_function_result_variable
+                original_name = original_var.name
+                self.scope.insert_symbol(original_name)
+                # Declare as pointer as the array should not free its data when it goes out of scope
+                new_var = original_var.clone(self.scope.get_expected_name(original_name), memory_handling='alias')
+                self.scope.insert_variable(new_var)
         # update ndarray and optional local variables properties
 
         # Find a name for the wrapper function
         wrapper_name = self._get_wrapper_name(expr)
 
         # Collect arguments and results
         wrapper_args    = self.get_wrapper_arguments()
         wrapper_results = [self.get_new_PyObject("result")]
         self.scope.insert_variable(wrapper_results[0])
 
         # Collect argument names for PyArgParse
-        arg_names         = [a.var.name for a in local_arg_vars.values()]
+        arg_names         = [a.var.name for a in (expr.original_function.arguments if isinstance(expr, BindCFunctionDef) else expr.arguments)]
         keyword_list_name = self.scope.get_new_name('kwlist')
         keyword_list      = PyArgKeywords(keyword_list_name, arg_names)
 
         if expr.is_private:
             self.exit_scope()
             return self.untranslatable_function(wrapper_name,
                         wrapper_args, wrapper_results,
@@ -1378,19 +1489,19 @@
         parse_node = PyArg_ParseTupleNode(*wrapper_args[1:],
                                           list(local_arg_vars.values()),
                                           parse_args, keyword_list)
 
         wrapper_body.append(If(IfSection(PyccelNot(parse_node), [Return([Nil()])])))
         wrapper_body.extend(wrapper_body_translations)
 
-        wrapper_body.extend(self._get_static_func_call_code(expr, static_func_args, result_vars))
+        wrapper_body.extend(self._get_static_func_call_code(expr, static_func_args, results))
 
         # Loop over results to carry out necessary casts and collect Py_BuildValue type string
         res_args = []
-        for a in result_vars :
+        for a in results :
             collect_var, cast_func = self.get_PyBuildValue(a)
             if cast_func is not None:
                 wrapper_body.append(AliasAssign(collect_var, cast_func))
 
             res_args.append(ObjectAddress(collect_var) if collect_var.is_alias else collect_var)
 
         # Call PyBuildNode
@@ -1398,14 +1509,21 @@
 
         # Call free function for python type
         wrapper_body += [FunctionCall(Py_DECREF, [i]) for i in self._to_free_PyObject_list]
 
         # Call free function for C type
         wrapper_body += [If(IfSection(PyccelIsNot(i, Nil()), [Deallocate(i)])) if self.is_c_pointer(i) \
                             else Deallocate(i) for i in local_arg_vars if i.rank > 0]
+        if self._target_language == 'fortran':
+            dealloc_results = [self.scope.find(self.scope.get_expected_name(r.original_function_result_variable.name), category='variables')
+                                for r in results]
+        else:
+            dealloc_results = result_vars
+        wrapper_body += [If(IfSection(PyccelIsNot(i, Nil()), [Deallocate(i)])) if self.is_c_pointer(i) \
+                            else Deallocate(i) for i in dealloc_results if i.rank > 0]
         self._to_free_PyObject_list.clear()
 
         #Return
         wrapper_body.append(Return(wrapper_results))
 
         # Create FunctionDef and write using classic method
         wrapper_func = FunctionDef(name = wrapper_name,
@@ -1415,73 +1533,63 @@
             scope = self.scope)
 
         self.exit_scope()
 
         return CCodePrinter._print_FunctionDef(self, wrapper_func)
 
     def _print_Module(self, expr):
-        scope = Scope()
+        scope = Scope(original_symbols = expr.scope.python_names.copy())
         self.set_scope(scope)
         # The initialisation and deallocation shouldn't be exposed to python
         funcs_to_wrap = [f for f in expr.funcs if f not in (expr.init_func, expr.free_func)]
 
         # Insert declared objects into scope
-        if self._target_language == 'fortran':
-            for f in expr.funcs:
-                scope.insert_symbol('bind_c_'+f.name.lower())
-            for v in expr.variables:
-                if not v.is_private:
-                    if v.rank > 0:
-                        scope.insert_symbol('bind_c_'+v.name.lower())
-                    else:
-                        scope.insert_symbol(v.name.lower())
-        else:
-            for f in expr.funcs:
-                scope.insert_symbol(f.name.lower())
-            for v in expr.variables:
-                if not v.is_private:
-                    scope.insert_symbol(v.name.lower())
+        variables = expr.original_module.variables if isinstance(expr, BindCModule) else expr.variables
+        for f in expr.funcs:
+            scope.insert_symbol(f.name.lower())
+        for v in variables:
+            if not v.is_private:
+                scope.insert_symbol(v.name.lower())
 
+        funcs = []
         if self._target_language == 'fortran':
             vars_to_wrap_decs = [Declare(v.dtype, v.clone(v.name.lower()), module_variable=True) \
-                                    for v in expr.variables if not v.is_private and v.rank == 0]
+                                    for v in variables if not v.is_private and v.rank == 0]
+
+            for f in expr.original_module.funcs:
+                if f.is_private:
+                    funcs.append(f)
         else:
             vars_to_wrap_decs = [Declare(v.dtype, v, module_variable=True) \
                                     for v in expr.variables if not v.is_private]
 
-        self._module_name  = expr.name
+        self._module_name  = self.get_python_name(scope, expr)
         sep = self._print(SeparatorComment(40))
 
+        function_signatures = ''.join(f'{self.static_function_signature(f)};\n' for f in expr.funcs)
         if self._target_language == 'fortran':
-            static_funcs = [self.get_static_function(f) for f in expr.funcs]
-        else:
-            static_funcs = expr.funcs
-        function_signatures = ''.join('{};\n'.format(self.static_function_signature(f)) for f in static_funcs)
-        if self._target_language == 'fortran':
-            var_wrappers = [wrap_module_array_var(v, self.scope, expr) \
-                    for v in expr.variables if not v.is_private and v.rank > 0]
-            function_signatures += ''.join('{};\n'.format(self.function_signature(v)) for v in var_wrappers)
+            function_signatures += ''.join(f'{self.static_function_signature(f)};\n' for f in expr.variable_wrappers)
 
         interface_funcs = [f.name for i in expr.interfaces for f in i.functions]
-        funcs = [*expr.interfaces, *(f for f in funcs_to_wrap if f.name not in interface_funcs)]
+        funcs += [*expr.interfaces, *(f for f in funcs_to_wrap if f.name not in interface_funcs)]
 
         self._in_header = True
         decs = ''.join('extern '+self._print(d) for d in vars_to_wrap_decs)
         self._in_header = False
 
         function_defs = '\n'.join(self._print(f) for f in funcs)
         cast_functions = '\n'.join(CCodePrinter._print_FunctionDef(self, f)
                                        for f in self._cast_functions_dict.values())
         method_def_func = ''.join(('{{\n'
                                      '"{name}",\n'
                                      '(PyCFunction){wrapper_name},\n'
                                      'METH_VARARGS | METH_KEYWORDS,\n'
                                      '{doc_string}\n'
                                      '}},\n').format(
-                                            name = expr.scope.get_python_name(f.name),
+                                            name = self.get_python_name(expr.scope, f),
                                             wrapper_name = self._function_wrapper_names[f.name],
                                             doc_string = self._print(LiteralString('\n'.join(f.doc_string.comments))) \
                                                         if f.doc_string else '""')
                                      for f in funcs if f is not expr.init_func)
 
         slots_name = self.scope.get_new_name('{}_slots'.format(expr.name))
         exec_func_name = self.scope.get_new_name('exec_func')
@@ -1506,24 +1614,24 @@
                 '/* module documentation, may be NULL */\n'
                 'NULL,\n' #TODO: Add documentation
                 '/* size of per-interpreter state of the module, or -1 if the module keeps state in global variables. */\n'
                 '0,\n'
                 '{method_def_name},\n'
                 '{slots_name}\n'
                 '}};\n'.format(module_def_name = module_def_name,
-                    mod_name = expr.name,
+                    mod_name = self._module_name,
                     method_def_name = method_def_name,
                     slots_name = slots_name))
 
         exec_func = self.get_module_exec_function(expr, exec_func_name)
 
         init_func = ('PyMODINIT_FUNC PyInit_{mod_name}(void)\n{{\n'
                 'import_array();\n'
                 'return PyModuleDef_Init(&{module_def_name});\n'
-                '}}\n'.format(mod_name=expr.name,
+                '}}\n'.format(mod_name=self._module_name,
                     module_def_name = module_def_name))
 
         # Print imports last to be sure that all additional_imports have been collected
         imports  = module_imports.copy()
         imports += self._additional_imports.values()
         imports  = ''.join(self._print(i) for i in imports)
```

### Comparing `pyccel-1.7.4/pyccel/codegen/printing/fcode.py` & `pyccel-1.8.0/pyccel/codegen/printing/fcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import re
 from itertools import chain
 from collections import OrderedDict
 
 import functools
 
 from pyccel.ast.basic import PyccelAstNode
-from pyccel.ast.bind_c import BindCPointer
+from pyccel.ast.bind_c import BindCPointer, BindCFunctionDef, BindCFunctionDefArgument, BindCModule
 from pyccel.ast.core import get_iterable_ranges
 from pyccel.ast.core import FunctionDef, InlineFunctionDef
 from pyccel.ast.core import SeparatorComment, Comment
 from pyccel.ast.core import ConstructorCall
 from pyccel.ast.core import FunctionCallArgument
 from pyccel.ast.core import ErrorExit, FunctionAddress
 from pyccel.ast.core import Return, Module
@@ -454,19 +454,23 @@
         else:
             private = ''
         # ...
 
         # ...
         sep = self._print(SeparatorComment(40))
         interfaces = ''
-        if expr.interfaces:
+        if expr.interfaces and not isinstance(expr, BindCModule):
             interfaces = '\n'.join(self._print(i) for i in expr.interfaces)
 
+        func_strings = []
         if expr.funcs:
-            body += '\n'.join(''.join([sep, self._print(i), sep]) for i in expr.funcs)
+            func_strings = [''.join([sep, self._print(i), sep]) for i in expr.funcs]
+        if isinstance(expr, BindCModule):
+            func_strings += [''.join([sep, self._print(i), sep]) for i in expr.variable_wrappers]
+        body += '\n'.join(func_strings)
         # ...
 
         # ...
         for i in expr.classes:
             # update decs with declarations from ClassDef
             c_decs, c_funcs = self._print(i)
             decs = '{0}\n{1}'.format(decs, c_decs)
@@ -1345,52 +1349,50 @@
 
         if isinstance(expr.variable, InhomogeneousTupleVariable):
             return ''.join(self._print_Declare(Declare(v.dtype,v,intent=expr.intent, static=expr.static)) for v in expr.variable)
 
         # ... TODO improve
         # Group the variables by intent
         var = expr.variable
+        expr_dtype = expr.dtype
         rank            = var.rank
         shape           = var.alloc_shape
-        is_target       = var.is_target
         is_const        = var.is_const
         is_optional     = var.is_optional
         is_private      = var.is_private
-        is_alias        = var.is_alias
+        is_alias        = var.is_alias and not isinstance(expr_dtype, BindCPointer)
         on_heap         = var.on_heap
         on_stack        = var.on_stack
         is_static       = expr.static
         is_external     = expr.external
+        is_target       = var.is_target and not var.is_alias
         intent          = expr.intent
         intent_in = intent and intent != 'out'
 
         if isinstance(shape, (tuple,PythonTuple)) and len(shape) ==1:
             shape = shape[0]
         # ...
 
         # ... print datatype
         if isinstance(expr.dtype, CustomDataType):
-            dtype = expr.dtype
+            name   = expr_dtype.__class__.__name__
+            prefix = expr_dtype.prefix
+            alias  = expr_dtype.alias
 
-            name   = dtype.__class__.__name__
-            prefix = dtype.prefix
-            alias  = dtype.alias
-
-            if dtype.is_polymorphic or expr.passed_from_dotted:
+            if expr_dtype.is_polymorphic or expr.passed_from_dotted:
                 sig = 'class'
             else:
                 sig = 'type'
 
             if alias is None:
                 name = name.replace(prefix, '')
             else:
                 name = alias
-            dtype = '{0}({1})'.format(sig, name)
+            dtype = f'{sig}({name})'
         else:
-            expr_dtype = expr.dtype
             dtype = self._print(expr_dtype)
 
         # ...
             if isinstance(expr_dtype, NativeString):
 
                 if intent_in:
                     dtype = dtype[:9] +'(len =*)'
@@ -1795,86 +1797,14 @@
             return body_code
 
         return ('{name} : Block\n'
                 '{prelude}\n'
                  '{body}\n'
                 'end Block {name}\n').format(name=expr.name, prelude=prelude, body=body_code)
 
-    def _print_BindCFunctionDef(self, expr):
-        name = self._print(expr.name)
-        results = [r.var for r in expr.results]
-
-        self.set_scope(expr.scope)
-        self.scope.functions[expr.name] = expr
-
-        body = self._print(expr.body)
-
-        decs = OrderedDict()
-        for arg in expr.arguments:
-            if arg.inout:
-                intent='inout'
-            else:
-                intent='in'
-
-            arg_var = arg.var
-
-            if isinstance(arg_var, FunctionAddress):
-                # Functions with function addresses as arguments cannot be
-                # exposed to python so there is no need to print their signature
-                return ''
-
-            dec = Declare(arg_var.dtype, arg_var, intent=intent , static=True)
-            decs[arg_var] = dec
-
-        arguments = [a.var for a in expr.arguments]
-
-        for result in results:
-            dec = Declare(result.dtype, result, intent='out', static=True)
-            decs[result] = dec
-
-        decs.update(self._get_external_declarations())
-
-        for i in expr.local_vars:
-            dec = Declare(i.dtype, i)
-            decs[i] = dec
-        vars_to_print = self.scope.variables.values()
-        for v in vars_to_print:
-            if (v not in expr.local_vars) and (v not in expr.results) and (v not in arguments):
-                decs[v] = Declare(v.dtype,v)
-
-        func_type = 'subroutine'
-        func_end  = ''
-        if len(results) == 1 and results[0].rank == 0:
-            func_type = 'function'
-            result = results.pop()
-            func_end = 'result({0})'.format(result.name)
-            dec = Declare(result.dtype, result, static=True)
-            decs[result] = dec
-
-        # ...
-
-        interfaces = '\n'.join(self._print(i) for i in expr.interfaces)
-        arg_code  = ', '.join(self._print(i) for i in chain( arguments, results ))
-        imports   = ''.join(self._print(i) for i in expr.imports)
-        prelude   = ''.join(self._print(i) for i in decs.values())
-        body_code = body
-        doc_string = self._print(expr.doc_string) if expr.doc_string else ''
-
-        self.exit_scope()
-
-        parts = [doc_string,
-                '{0} {1}({2}) bind(c) {3}\n'.format(func_type, name, arg_code, func_end),
-                 imports,
-                'implicit none\n',
-                 prelude,
-                 interfaces,
-                 body_code,
-                 'end {} {}\n'.format(func_type, name)]
-        return '\n'.join(p for p in parts if p)
-
     def _print_FunctionAddress(self, expr):
         return expr.name
 
     def function_signature(self, expr, name):
         """
         Get the different parts of the signature of the function `expr`.
 
@@ -1926,21 +1856,30 @@
             args_decs[result] = Declare(result.dtype, result)
             out_args = []
         # ...
 
         for i, arg in enumerate(arguments):
             arg_var = arg.var
             if isinstance(arg_var, Variable):
-                if i == 0 and expr.cls_name:
-                    dec = Declare(arg_var.dtype, arg_var, intent='inout', passed_from_dotted = True)
-                elif arg.inout:
-                    dec = Declare(arg_var.dtype, arg_var, intent='inout')
+                if isinstance(arg, BindCFunctionDefArgument) and arg.original_function_argument_variable.rank!=0:
+                    for b_arg,inout in zip(arg.get_all_function_def_arguments(), arg.inout):
+                        v = b_arg.var
+                        if inout:
+                            dec = Declare(v.dtype, v, intent='inout')
+                        else:
+                            dec = Declare(v.dtype, v, intent='in')
+                        args_decs[v] = dec
                 else:
-                    dec = Declare(arg_var.dtype, arg_var, intent='in')
-                args_decs[arg_var] = dec
+                    if i == 0 and expr.cls_name:
+                        dec = Declare(arg_var.dtype, arg_var, intent='inout', passed_from_dotted = True)
+                    elif arg.inout:
+                        dec = Declare(arg_var.dtype, arg_var, intent='inout')
+                    else:
+                        dec = Declare(arg_var.dtype, arg_var, intent='in')
+                    args_decs[arg_var] = dec
 
         # treat case of pure function
         sig = '{0}{1} {2}'.format(rec, func_type, name)
         if is_pure:
             sig = 'pure {}'.format(sig)
 
         # treat case of elemental function
@@ -1978,14 +1917,15 @@
         else:
             for i in _default_methods:
                 # because we may have a class Point with init: Point___init__
                 if i in name:
                     name = name.replace(i, _default_methods[i])
 
         sig_parts = self.function_signature(expr, name)
+        bind_c = ' bind(c)' if isinstance(expr, BindCFunctionDef) else ''
         prelude = sig_parts.pop('arg_decs')
         decs = OrderedDict()
         functions = [f for f in expr.functions if not f.is_inline]
         func_interfaces = '\n'.join(self._print(i) for i in expr.interfaces)
         body_code = self._print(expr.body)
         doc_string = self._print(expr.doc_string) if expr.doc_string else ''
 
@@ -2005,15 +1945,15 @@
         if len(functions)>0:
             functions_code = '\n'.join(self._print(i) for  i in functions)
             body_code = body_code +'\ncontains\n' + functions_code
 
         imports = ''.join(self._print(i) for i in expr.imports)
 
         parts = [doc_string,
-                "{}({}) {}\n".format(sig_parts['sig'], sig_parts['arg_code'], sig_parts['func_end']),
+                f"{sig_parts['sig']}({sig_parts['arg_code']}){bind_c} {sig_parts['func_end']}\n",
                 imports,
                 'implicit none\n',
                 prelude,
                 func_interfaces,
                 body_code,
                 'end {} {}\n'.format(sig_parts['func_type'], name)]
 
@@ -2122,14 +2062,15 @@
         return 'exit\n'
 
     def _print_Continue(self, expr):
         return 'cycle\n'
 
     def _print_AugAssign(self, expr):
         new_expr = expr.to_basic_assign()
+        expr.invalidate_node()
         return self._print(new_expr)
 
     def _print_PythonRange(self, expr):
         start = self._print(expr.start)
         step  = self._print(expr.step)
 
         test_step = expr.step
@@ -2458,41 +2399,71 @@
         prolog = "if ( .not. ({0})) then".format(self._print(expr.test))
         body = 'stop 1'
         epilog = 'end if'
         return ('{prolog}\n'
                 '{body}\n'
                 '{epilog}\n').format(prolog=prolog, body=body, epilog=epilog)
 
+    def _handle_not_none(self, lhs, lhs_var):
+        """
+        Print code for `x is not None` statement.
+
+        Print the code which checks if x is not None. This means different
+        things depending on the type of `x`. If `x` is optional it checks
+        if it is present, if `x` is a C pointer it checks if it points at
+        anything.
+
+        Parameters
+        ----------
+        lhs : str
+            The code representing `x`.
+        lhs_var : Variable
+            The Variable `x`.
+
+        Returns
+        -------
+        str
+            The code which checks if `x is not None`.
+        """
+        if isinstance(lhs_var.dtype, BindCPointer):
+            self._constantImports.setdefault('ISO_C_Binding', set()).add('c_associated')
+            return f'c_associated({lhs})'
+        else:
+            return f'present({lhs})'
 
     def _print_PyccelIs(self, expr):
-        lhs = self._print(expr.lhs)
-        rhs = self._print(expr.rhs)
+        lhs_var = expr.lhs
+        rhs_var = expr.rhs
+        lhs = self._print(lhs_var)
+        rhs = self._print(rhs_var)
         a = expr.args[0]
         b = expr.args[1]
 
-        if isinstance(expr.rhs, Nil):
-            return '.not. present({})'.format(lhs)
+        if isinstance(rhs_var, Nil):
+            return '.not. '+ self._handle_not_none(lhs, lhs_var)
 
         if (a.dtype is NativeBool() and b.dtype is NativeBool()):
-            return '{} .eqv. {}'.format(lhs, rhs)
+            return f'{lhs} .eqv. {rhs}'
 
         errors.report(PYCCEL_RESTRICTION_IS_ISNOT,
                       symbol=expr, severity='fatal')
 
     def _print_PyccelIsNot(self, expr):
-        lhs = self._print(expr.lhs)
-        rhs = self._print(expr.rhs)
+        lhs_var = expr.lhs
+        rhs_var = expr.rhs
+        lhs = self._print(lhs_var)
+        rhs = self._print(rhs_var)
         a = expr.args[0]
         b = expr.args[1]
 
-        if isinstance(expr.rhs, Nil):
-            return 'present({})'.format(lhs)
+        if isinstance(rhs_var, Nil):
+            return self._handle_not_none(lhs, lhs_var)
 
         if a.dtype is NativeBool() and b.dtype is NativeBool():
-            return '{} .neqv. {}'.format(lhs, rhs)
+            return f'{lhs} .neqv. {rhs}'
 
         errors.report(PYCCEL_RESTRICTION_IS_ISNOT,
                       symbol=expr, severity='fatal')
 
     def _print_If(self, expr):
         # ...
 
@@ -3095,14 +3066,24 @@
         lhs = self._print(expr.result)
         rhs = self._print(expr.arg)
         self._constantImports.setdefault('ISO_C_Binding', set()).add('c_loc')
         return f'{lhs} = c_loc({rhs})\n'
 
 #=======================================================================================
 
+    def _print_C_F_Pointer(self, expr):
+        self._constantImports.setdefault('ISO_C_Binding', set()).add('C_F_Pointer')
+        shape = ','.join(self._print(s) for s in expr.shape)
+        if shape:
+            return f'call C_F_Pointer({self._print(expr.c_pointer)}, {self._print(expr.f_array)}, [{shape}])\n'
+        else:
+            return f'call C_F_Pointer({self._print(expr.c_pointer)}, {self._print(expr.f_array)})\n'
+
+#=======================================================================================
+
     def _print_PythonConjugate(self, expr):
         return 'conjg( {} )'.format( self._print(expr.internal_var) )
 
 #=======================================================================================
 
     def _wrap_fortran(self, lines):
         """Wrap long Fortran lines
```

### Comparing `pyccel-1.7.4/pyccel/codegen/printing/luacode.py` & `pyccel-1.8.0/pyccel/codegen/printing/luacode.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/codegen/printing/pycode.py` & `pyccel-1.8.0/pyccel/codegen/printing/pycode.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/codegen/python_wrapper.py` & `pyccel-1.8.0/pyccel/codegen/python_wrapper.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 
 import os
 
-from pyccel.ast.bind_c                      import as_static_module
 from pyccel.ast.numpy_wrapper               import get_numpy_max_acceptable_version_file
 from pyccel.codegen.printing.fcode          import fcode
 from pyccel.codegen.printing.cwrappercode   import CWrapperCodePrinter
+from pyccel.codegen.wrapper.fortran_to_c_wrapper   import FortranToCWrapper
 from pyccel.codegen.utilities      import recompile_object
 from pyccel.codegen.utilities      import copy_internal_library
 from pyccel.codegen.utilities      import internal_libs
 from pyccel.naming                 import name_clash_checkers
 from pyccel.parser.scope           import Scope
 from pyccel.utilities.stage        import PyccelStage
 from .compiling.basic     import CompileObj
@@ -32,14 +32,66 @@
                           language,
                           wrapper_flags,
                           pyccel_dirpath,
                           src_compiler,
                           wrapper_compiler,
                           sharedlib_modname=None,
                           verbose = False):
+    """
+    Create a shared library which can be called from Pyccel.
+
+    From a CodePrinter object describing code which has been printed
+    in a target language, create a shared library which can be
+    called from Pyccel. In order to do this the code must be wrapped.
+    First, if the code is not written in C, it must be wrapped to
+    make it callable from C. This intermediary code is printed
+    and compiled. From the C-compatible code a second (first for C)
+    wrapper is created which exposes the C code to Python. This
+    is done via the CWrapper. Finally this new code is compiled
+    to generate the required shared language.
+
+    Parameters
+    ----------
+    codegen : pyccel.codegen.printing.codeprinter.CodePrinter
+        The printer which was used to print the translated code.
+
+    main_obj : pyccel.codegen.compiling.basic.CompileObj
+        The compile object which describes the translated code.
+
+    language : str
+        The language which Pyccel translated to.
+
+    wrapper_flags : iterable
+        Any additional flags which should be used to compile the wrapper.
+
+    pyccel_dirpath : str
+        The path to the directory where the files are created and compiled.
+
+    src_compiler : pyccel.codegen.compiling.compilers.Compiler
+        The compiler which should be used to compile the library.
+
+    wrapper_compiler : pyccel.codegen.compiling.compilers.Compiler
+        The compiler which should be used to compile the wrapper.
+        Often this is the same as src_compiler but it may be different
+        when the language is not C to ensure that src_compiler can link
+        the appropriate language-specific libraries.
+
+    sharedlib_modname : str, default: None
+        The name of the shared library. The default is the name of the
+        module printed by the printer.
+
+    verbose : bool, default: False
+        Indicates if the compiling should be done with verbosity to show the
+        compiler commands.
+
+    Returns
+    -------
+    str
+        The absolute path to the shared library which was created.
+    """
 
     pyccel_stage.set_stage('cwrapper')
 
     # Get module name
     module_name = codegen.name
 
     # Change working directory to '__pyccel__'
@@ -56,29 +108,33 @@
             pyccel_dirpath,
             flags        = wrapper_flags,
             dependencies = (main_obj,),
             accelerators = ('python',))
 
     if language == 'fortran':
         # Construct static interface for passing array shapes and write it to file bind_c_MOD.f90
-        bind_c_mod = as_static_module(codegen.routines, codegen.ast)
+        wrapper = FortranToCWrapper()
+        bind_c_mod = wrapper.wrap(codegen.ast)
         bind_c_code = fcode(bind_c_mod, bind_c_mod.name)
         bind_c_filename = '{}.f90'.format(bind_c_mod.name)
 
         with open(bind_c_filename, 'w') as f:
             f.writelines(bind_c_code)
 
         bind_c_obj=CompileObj(file_name = bind_c_filename,
                 folder = pyccel_dirpath,
                 flags  = main_obj.flags,
                 dependencies = (main_obj,))
         wrapper_compile_obj.add_dependencies(bind_c_obj)
         src_compiler.compile_module(compile_obj=bind_c_obj,
                 output_folder=pyccel_dirpath,
                 verbose=verbose)
+        c_ast = bind_c_mod
+    else:
+        c_ast = codegen.ast
 
     #---------------------------------------
     #     Compile cwrapper from stdlib
     #---------------------------------------
     cwrapper_lib_dest_path = copy_internal_library('cwrapper', pyccel_dirpath,
                                 extra_files = {'numpy_version.h' :
                                                 get_numpy_max_acceptable_version_file()})
@@ -96,28 +152,28 @@
     #---------------------------------------
     #      Print code specific cwrapper
     #---------------------------------------
     module_old_name = codegen.ast.name
     codegen.ast.set_name(sharedlib_modname)
     wrapper_codegen = CWrapperCodePrinter(codegen.parser.filename, language)
     Scope.name_clash_checker = name_clash_checkers['c']
-    wrapper_code = wrapper_codegen.doprint(codegen.ast)
+    wrapper_code = wrapper_codegen.doprint(c_ast)
     if errors.has_errors():
         return
 
     codegen.ast.set_name(module_old_name)
 
     with open(wrapper_filename, 'w') as f:
         f.writelines(wrapper_code)
 
     #--------------------------------------------------------
     #  Compile cwrapper_ndarrays from stdlib (if necessary)
     #--------------------------------------------------------
-    if "ndarrays" in wrapper_codegen.get_additional_imports():
-        for lib_name in ("ndarrays", "cwrapper_ndarrays"):
+    for lib_name in ("ndarrays", "cwrapper_ndarrays"):
+        if lib_name in wrapper_codegen.get_additional_imports():
             stdlib_folder, stdlib = internal_libs[lib_name]
 
             lib_dest_path = copy_internal_library(stdlib_folder, pyccel_dirpath)
 
             # Pylint determines wrong type
             stdlib.reset_folder(lib_dest_path) # pylint: disable=E1101
             # get the include folder path and library files
```

### Comparing `pyccel-1.7.4/pyccel/codegen/utilities.py` & `pyccel-1.8.0/pyccel/codegen/utilities.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/commands/console.py` & `pyccel-1.8.0/pyccel/commands/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,35 @@
 
 #==============================================================================
 # TODO - remove output_dir froms args
 #      - remove files from args
 #      but quickstart and build are still calling it for the moment
 def pyccel(files=None, mpi=None, openmp=None, openacc=None, output_dir=None, compiler=None):
     """
-    pyccel console command.
+    Pyccel console command.
+
+    The Pyccel console command allows translating Python files using Pyccel in a command-line environment. It provides
+    options to specify the files to be translated, enable support for MPI, OpenMP, and OpenACC, specify the output
+    directory for the translated files, and choose the compiler to be used for translation. By default, all parameters
+    are set to None, and the command will use the default behavior defined by Pyccel.
+
+    Parameters
+    ----------
+    files : str or list of str, optional
+        File(s) to be translated. It can be a single file or a list of files (currently pyccel support single), by default None.
+    mpi : bool, optional
+        Enable MPI support, by default None.
+    openmp : bool, optional
+        Enable OpenMP support, by default None.
+    openacc : bool, optional
+        Enable OpenACC support, by default None.
+    output_dir : str, optional
+        Directory to store the translated file(s), by default None.
+    compiler : str, optional
+        Compiler to be used for translation, by default None.
     """
     parser = MyParser(description='pyccel command line')
 
     parser.add_argument('files', metavar='N', type=str, nargs='*',
                         help='a Pyccel file')
 
     #... Version
@@ -111,14 +131,16 @@
     group = parser.add_argument_group('Other options')
     group.add_argument('--verbose', action='store_true', \
                         help='enables verbose mode.')
     group.add_argument('--developer-mode', action='store_true', \
                         help='shows internal messages')
     group.add_argument('--export-compile-info', type=str, default = None, \
                         help='file to which the compiler json file is exported')
+    group.add_argument('--conda-warnings', choices=('off', 'basic', 'verbose'), help='Specify the level of Conda warnings to display (choices: off, basic, verbose), Default is basic.')
+
     # ...
 
     # TODO move to another cmd line
     parser.add_argument('--analysis', action='store_true', \
                         help='enables code analysis mode.')
     # ...
 
@@ -144,14 +166,17 @@
 
     if not openmp:
         openmp = args.openmp
 
     if not openacc:
         openacc = args.openacc
 
+    if not args.conda_warnings:
+        args.conda_warnings = 'basic'
+
     if args.convert_only or args.syntax_only or args.semantic_only:
         compiler = None
     # ...
 
     # ...
 
     if len(files) > 1:
@@ -248,15 +273,16 @@
                        includes      = args.includes,
                        libdirs       = args.libdirs,
                        modules       = (),
                        libs          = args.libs,
                        debug         = args.debug,
                        accelerators  = accelerators,
                        folder        = args.output,
-                       compiler_export_file = compiler_export_file)
+                       compiler_export_file = compiler_export_file,
+                       conda_warnings = args.conda_warnings)
     except PyccelError:
         sys.exit(1)
     finally:
         os.chdir(base_dirpath)
 
 #==============================================================================
 # NOTE: left here for later reference
```

### Comparing `pyccel-1.7.4/pyccel/commands/pyccel_clean.py` & `pyccel-1.8.0/pyccel/commands/pyccel_clean.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/commands/pyccel_init.py` & `pyccel-1.8.0/pyccel/commands/pyccel_init.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/compilers/default_compilers.py` & `pyccel-1.8.0/pyccel/compilers/default_compilers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from numpy import get_include as get_numpy_include
 from pyccel import __version__ as pyccel_version
 
 gfort_info = {'exec' : 'gfortran',
               'mpi_exec' : 'mpif90',
               'language': 'fortran',
               'module_output_flag': '-J',
-              'debug_flags': ("-fcheck=bounds",),
+              'debug_flags': ("-fcheck=bounds","-g","-O0"),
               'release_flags': ("-O3","-funroll-loops",),
               'general_flags' : ('-fPIC',),
               'standard_flags' : ('-std=f2003',),
               'mpi': {
                   },
               'openmp': {
                   'flags' : ('-fopenmp',),
@@ -37,15 +37,15 @@
     gfort_info['mpi']['libdirs']  = (os.environ["MSMPI_LIB64"].rstrip('\\'),)
 
 #------------------------------------------------------------
 ifort_info = {'exec' : 'ifort',
               'mpi_exec' : 'mpiifort',
               'language': 'fortran',
               'module_output_flag': '-module',
-              'debug_flags': ("-check=bounds",),
+              'debug_flags': ("-check=bounds","-g","-O0"),
               'release_flags': ("-O3","-funroll-loops",),
               'general_flags' : ('-fPIC',),
               'standard_flags' : ('-std=f2003',),
               'openmp': {
                   'flags' : ('-fopenmp','-nostandard-realloc-lhs'),
                   'libs'  : ('iomp5',),
                   },
@@ -56,15 +56,15 @@
               }
 
 #------------------------------------------------------------
 pgfortran_info = {'exec' : 'pgfortran',
               'mpi_exec' : 'pgfortran',
               'language': 'fortran',
               'module_output_flag': '-module',
-              'debug_flags': ("-Mbounds",),
+              'debug_flags': ("-Mbounds","-g","-O0"),
               'release_flags': ("-O3","-Munroll",),
               'general_flags' : ('-fPIC',),
               'standard_flags' : ('-Mstandard',),
               'openmp': {
                   'flags' : ('-mp',),
                   },
               'openacc': {
@@ -74,15 +74,15 @@
               }
 
 #------------------------------------------------------------
 nvfort_info = {'exec' : 'nvfort',
               'mpi_exec' : 'nvfort',
               'language': 'fortran',
               'module_output_flag': '-module',
-              'debug_flags': ("-Mbounds",),
+              'debug_flags': ("-Mbounds","-g","-O0"),
               'release_flags': ("-O3","-Munroll",),
               'general_flags' : ('-fPIC',),
               'standard_flags' : ('-Mstandard',),
               'openmp': {
                   'flags' : ('-mp',),
                   },
               'openacc': {
@@ -91,15 +91,15 @@
               'family': 'nvidia',
               }
 
 #------------------------------------------------------------
 gcc_info = {'exec' : 'gcc',
             'mpi_exec' : 'mpicc',
             'language': 'c',
-            'debug_flags': ("-g",),
+            'debug_flags': ("-g","-O0"),
             'release_flags': ("-O3","-funroll-loops",),
             'general_flags' : ('-fPIC',),
             'standard_flags' : ('-std=c99',),
             'mpi': {
                 },
             'openmp': {
                 'flags' : ('-fopenmp',),
@@ -122,15 +122,15 @@
     gcc_info['mpi']['includes'] = (os.environ["MSMPI_INC"].rstrip('\\'),)
     gcc_info['mpi']['libdirs']  = (os.environ["MSMPI_LIB64"].rstrip('\\'),)
 
 #------------------------------------------------------------
 icc_info = {'exec' : 'icc',
             'mpi_exec' : 'mpiicc',
             'language': 'c',
-            'debug_flags': ("-g",),
+            'debug_flags': ("-g","-O0"),
             'release_flags': ("-O3","-funroll-loops",),
             'general_flags' : ('-fPIC',),
             'standard_flags' : ('-std=c99',),
             'openmp': {
                 'flags' : ('-fopenmp',),
                 },
             'openacc': {
@@ -139,15 +139,15 @@
             'family': 'intel',
             }
 
 #------------------------------------------------------------
 pgcc_info = {'exec' : 'pgcc',
             'mpi_exec' : 'pgcc',
             'language': 'c',
-            'debug_flags': ("-g",),
+            'debug_flags': ("-g","-O0"),
             'release_flags': ("-O3","-Munroll",),
             'general_flags' : ('-fPIC',),
             'standard_flags' : ('-std=c99',),
             'openmp': {
                 'flags' : ('-mp',),
                 },
             'openacc': {
@@ -156,15 +156,15 @@
             'family': 'PGI',
             }
 
 #------------------------------------------------------------
 nvc_info = {'exec' : 'nvc',
             'mpi_exec' : 'nvc',
             'language': 'c',
-            'debug_flags': ("-g",),
+            'debug_flags': ("-g","-O0"),
             'release_flags': ("-O3","-Munroll",),
             'general_flags' : ('-fPIC',),
             'standard_flags' : ('-std=c99',),
             'openmp': {
                 'flags' : ('-mp',),
                 },
             'openacc': {
```

### Comparing `pyccel-1.7.4/pyccel/complexity/arithmetic.py` & `pyccel-1.8.0/pyccel/complexity/arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/complexity/basic.py` & `pyccel-1.8.0/pyccel/complexity/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/complexity/memory.py` & `pyccel-1.8.0/pyccel/complexity/memory.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/decorators.py` & `pyccel-1.8.0/pyccel/decorators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/epyccel.py` & `pyccel-1.8.0/pyccel/epyccel.py`

 * *Files 20% similar despite different names*

```diff
@@ -107,16 +107,72 @@
                 accelerators  = (),
                 verbose       = False,
                 debug         = False,
                 includes      = (),
                 libdirs       = (),
                 modules       = (),
                 libs          = (),
-                folder        = None):
+                folder        = None,
+                conda_warnings= 'basic',
+                comm          = None,
+                root          = None,
+                bcast         = None):
+    """
+    Accelerate Python function or module using Pyccel in "embedded" mode.
+
+    This function accelerates a Python function or module using Pyccel in "embedded" mode.
+    It generates optimized code in the specified language (default is 'fortran')
+    and compiles it for improved performance.
 
+    Parameters
+    ----------
+    function_or_module : function | module
+        Python function or module to be accelerated.
+    language : {'fortran', 'c', 'python'}
+        Language of generated code (default: 'fortran').
+    compiler : str, optional
+        User-defined command for compiling generated source code.
+    fflags : iterable of str, optional
+        Compiler flags.
+    wrapper_flags : iterable of str, optional
+        Flags to be passed to the wrapper code generator.
+    accelerators : iterable of str, optional
+        Parallel multi-threading acceleration strategy
+        (currently supported: 'mpi', 'openmp', 'openacc').
+    verbose : bool
+        Print additional information (default: False).
+    debug : bool, optional
+        Enable debug mode.
+    includes : tuple, optional
+        Additional include directories for the compiler.
+    libdirs : tuple, optional
+        Additional library directories for the compiler.
+    modules : tuple, optional
+        Additional modules to be imported.
+    libs : tuple, optional
+        Additional libraries.
+    folder : str, optional
+        Output folder for the compiled code.
+    conda_warnings : {off, basic, verbose}
+        Specify the level of Conda warnings to display (choices: off, basic, verbose), Default is 'basic'.
+
+    Returns
+    -------
+    object
+        Return accelerated Python module and function.
+
+    Other Parameters
+    ----------------
+    comm : mpi4py.MPI.Comm, optional
+        MPI communicator for calling Pyccel in parallel mode (default: None) (for parallel mode).
+    root : int, optional
+        MPI rank of process in charge of accelerating code (default: 0) (for parallel mode).
+    bcast : {True, False}
+        If False, only root process loads accelerated function/module (default: True) (for parallel mode). 
+    """
     # ... get the module source code
     if isinstance(function_or_module, FunctionType):
         pyfunc = function_or_module
         code = get_source_function(pyfunc)
 
         dirpath = os.getcwd()
 
@@ -173,15 +229,16 @@
                            wrapper_flags = wrapper_flags,
                            includes      = includes,
                            libdirs       = libdirs,
                            modules       = modules,
                            libs          = libs,
                            debug         = debug,
                            accelerators  = accelerators,
-                           output_name   = module_name)
+                           output_name   = module_name,
+                           conda_warnings= conda_warnings)
         finally:
             # Change working directory back to starting point
             os.chdir(base_dirpath)
 
 
         # Import shared library
         sys.path.insert(0, epyccel_dirpath)
@@ -211,57 +268,42 @@
     return package, func
 
 #==============================================================================
 def epyccel( python_function_or_module, **kwargs ):
     """
     Accelerate Python function or module using Pyccel in "embedded" mode.
 
+    This function accelerates a Python function or module using Pyccel in "embedded" mode.
+    It generates optimized code in the specified language (default is 'fortran')
+    and compiles it for improved performance
+
     Parameters
     ----------
     python_function_or_module : function | module
         Python function or module to be accelerated.
-
-    verbose : bool
-        Print additional information (default: False).
-
-    language : {'fortran', 'c', 'python'}
-        Language of generated code (default: 'fortran').
-
-    accelerators : iterable of str, optional
-        Parallel multi-threading acceleration strategy
-        (currently supported: 'mpi', 'openmp', 'openacc').
-
-    Options for parallel mode
-    -------------------------
-    comm : mpi4py.MPI.Comm, optional
-        MPI communicator for calling Pyccel in parallel mode (default: None).
-
-    root : int, optional
-        MPI rank of process in charge of accelerating code (default: 0).
-
-    bcast : {True, False}
-        If False, only root process loads accelerated function/module (default: True).
-
-    Other options
-    -------------
-    compiler : str, optional
-        User-defined command for compiling generated source code.
+    **kwargs :
+        Additional keyword arguments for configuring the compilation and acceleration process.
+        Available options are defined in epyccel_seq.
 
     Returns
     -------
-    res : object
+    object
         Accelerated function or module.
 
+    See Also 
+    -------- 
+    epyccel_seq
+        The version of this function called in a sequential context.
+
     Examples
     --------
     >>> def one(): return 1
     >>> from pyccel.epyccel import epyccel
     >>> one_f = epyccel(one, language='fortran')
     >>> one_c = epyccel(one, language='c')
-
     """
     assert isinstance( python_function_or_module, (FunctionType, ModuleType) )
 
     comm  = kwargs.pop('comm', None)
     root  = kwargs.pop('root', 0)
     bcast = kwargs.pop('bcast', True)
     if kwargs.pop('developer_mode', None):
```

### Comparing `pyccel-1.7.4/pyccel/errors/errors.py` & `pyccel-1.8.0/pyccel/errors/errors.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/errors/messages.py` & `pyccel-1.8.0/pyccel/errors/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 STACK_ARRAY_DEFINITION_IN_LOOP = 'Cannot create stack array in loop, because if does not support memory reallocation. Create array before loop, or use standard heap array.'
 STACK_ARRAY_UNKNOWN_SHAPE = 'Cannot create stack array from a shape which is unknown at function entry'
 STACK_ARRAY_SHAPE_UNPURE_FUNC = 'Cannot create stack array from a shape created with an impure function'
 INCOMPATIBLE_ARGUMENT = 'Argument {} : {}, passed to function {} is incompatible (expected {}). Please cast the argument explicitly or overload the function (see https://github.com/pyccel/pyccel/blob/master/tutorial/headers.md for details)'
 INCOMPATIBLE_ORDERING = "Argument {idx} : {arg}, passed to function {func} is incompatible as it has the wrong ordering (expected '{order}'). Please use an argument with '{order}' ordering, explicitly transpose {arg}, or overload the function (see https://github.com/pyccel/pyccel/blob/master/tutorial/headers.md for details)"
 UNRECOGNISED_FUNCTION_CALL = 'Function call cannot be processed. Please ensure that your code runs correctly in python. If this is the case then you may be using function arguments which are not currently supported by pyccel. Please create an issue at https://github.com/pyccel/pyccel/issues and provide a small example of your problem.'
 
+UNSUPPORTED_FEATURE_OOP_EMPTY_CLASS = "Empty classes are not supported"
 UNSUPPORTED_POINTER_RETURN_VALUE = "returning a pointer is not implemented yet."
 UNSUPPORTED_ARRAY_RANK = 'Arrays of dimensions > 15 are currently not supported'
 
 INCOMPATIBLE_TYPES_IN_STR_INTERPOLATION = 'Incompatible types in string interpolation'
 MUST_HAVE_NONE_RETURN_TYPE = 'The return type of "{}" must be None'
 INVALID_TUPLE_INDEX_TYPE = 'Invalid tuple index type'
 TUPLE_INDEX_OUT_OF_RANGE = 'Tuple index out of range'
```

### Comparing `pyccel-1.7.4/pyccel/naming/__init__.py` & `pyccel-1.8.0/pyccel/naming/__init__.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/naming/cnameclashchecker.py` & `pyccel-1.8.0/pyccel/naming/cnameclashchecker.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 """
 Handles name clash problems in C
 """
-from pyccel.utilities.metaclasses import Singleton
-from pyccel.utilities.strings import create_incremented_string
+from .languagenameclashchecker import LanguageNameClashChecker
 
-class CNameClashChecker(metaclass = Singleton):
-    """ Class containing functions to help avoid problematic names in C
+class CNameClashChecker(LanguageNameClashChecker):
+    """
+    Class containing functions to help avoid problematic names in C.
+
+    A class which provides functionalities to check or propose variable names and
+    verify that they do not cause name clashes. Name clashes may be due to
+    new variables, or due to the use of reserved keywords.
     """
     # Keywords as mentioned on https://en.cppreference.com/w/c/keyword
     keywords = set(['isign', 'fsign', 'csign', 'auto', 'break', 'case', 'char', 'const',
         'continue', 'default', 'do', 'double', 'else', 'enum',
         'extern', 'float', 'for', 'goto', 'if', 'inline', 'int',
         'long', 'register', 'restrict', 'return', 'short', 'signed',
         'sizeof', 'static', 'struct', 'switch', 'typedef', 'union',
@@ -38,24 +42,33 @@
     def has_clash(self, name, symbols):
         """ Indicate whether the proposed name causes any clashes
         """
         return any(name == k for k in self.keywords) or \
                any(name == s for s in symbols)
 
     def get_collisionless_name(self, name, symbols):
-        """ Get the name that will be used in the fortran code
+        """
+        Get a valid name which doesn't collision with symbols or C keywords.
+
+        Find a new name based on the suggested name which will not cause
+        conflicts with C keywords, does not appear in the provided symbols,
+        and is a valid name in C code.
+
+        Parameters
+        ----------
+        name : str
+            The suggested name.
+        symbols : set
+            Symbols which should be considered as collisions.
+
+        Returns
+        -------
+        str
+            A new name which is collision free.
         """
         if len(name)>4 and all(name[i] == '_' for i in (0,1,-1,-2)):
             # Ignore magic methods
             return name
         if name[0] == '_':
             name = 'private'+name
-        prefix = name
-        coll_symbols = self.keywords.copy()
-        coll_symbols.update(s.lower() for s in symbols)
-        if prefix in coll_symbols:
-            counter = 1
-            new_name, counter = create_incremented_string(coll_symbols,
-                    prefix = prefix, counter = counter)
-            name = name+new_name[-5:]
-        return name
+        return self._get_collisionless_name(name, symbols)
```

### Comparing `pyccel-1.7.4/pyccel/naming/fortrannameclashchecker.py` & `pyccel-1.8.0/pyccel/naming/fortrannameclashchecker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 # coding: utf-8
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 """
-Handles name clash problems in Fortran
+Handles name clash problems in Fortran.
 """
 import warnings
 
-from pyccel.utilities.metaclasses import Singleton
-from pyccel.utilities.strings import create_incremented_string
+from .languagenameclashchecker import LanguageNameClashChecker
 
-class FortranNameClashChecker(metaclass = Singleton):
-    """ Class containing functions to help avoid problematic names in C
+class FortranNameClashChecker(LanguageNameClashChecker):
+    """
+    Class containing functions to help avoid problematic names in Fortran.
+
+    A class which provides functionalities to check or propose variable names and
+    verify that they do not cause name clashes. Name clashes may be due to
+    capitalisation (as Fortran is not case-sensitive), or due to the use of reserved
+    keywords.
     """
     # Keywords as mentioned on https://fortranwiki.org/fortran/show/Keywords
     # Intrinsic functions as mentioned on https://pages.mtu.edu/~shene/COURSES/cs201/NOTES/chap02/funct.html
     keywords = set(['assign', 'backspace', 'block', 'blockdata',
             'call', 'close', 'common', 'continue', 'data',
             'dimension', 'do', 'else', 'elseif', 'end', 'endfile',
             'endif', 'endfunction', 'endmodule', 'endprogram',
@@ -36,35 +41,45 @@
             'final', 'flush', 'generic', 'import', 'non_overrideable',
             'nopass', 'pass', 'protected', 'value', 'volatile',
             'wait', 'codimension', 'concurrent', 'contiguous',
             'critical', 'error', 'submodule', 'sync', 'lock',
             'unlock', 'test', 'abs', 'sqrt', 'sin', 'cos', 'tan',
             'asin', 'acos', 'atan', 'exp', 'log', 'int', 'nint',
             'floor', 'fraction', 'real', 'max', 'mod', 'count',
-            'pack', 'numpy_sign'])
+            'pack', 'numpy_sign', 'c_associated', 'c_loc', 'c_f_pointer', 'c_ptr'])
 
     def has_clash(self, name, symbols):
         """ Indicate whether the proposed name causes any clashes
         """
         name = name.lower()
         return any(name == k for k in self.keywords) or \
                any(name == s.lower() for s in symbols)
 
     def get_collisionless_name(self, name, symbols):
-        """ Get the name that will be used in the fortran code
+        """
+        Get a valid name which doesn't collide with symbols or Fortran keywords.
+
+        Find a new name based on the suggested name which will not cause
+        conflicts with Fortran keywords, does not conflict with the provided symbols,
+        and is a valid name in Fortran code.
+
+        Parameters
+        ----------
+        name : str
+            The suggested name.
+        symbols : set
+            Symbols which should be considered as collisions.
+
+        Returns
+        -------
+        str
+            A new name which is collision free.
         """
         if len(name)>4 and all(name[i] == '_' for i in (0,1,-1,-2)):
             # Ignore magic methods
             return name
         if name[0] == '_':
             name = 'private'+name
-        prefix = name.lower()
-        coll_symbols = self.keywords.copy()
-        coll_symbols.update(s.lower() for s in symbols)
-        if prefix in coll_symbols:
-            counter = 1
-            new_name, counter = create_incremented_string(coll_symbols,
-                    prefix = prefix, counter = counter)
-            name = name+new_name[-5:]
+        name = self._get_collisionless_name(name, symbols)
         if len(name) > 96:
             warnings.warn("Name {} is too long for Fortran. This may cause compiler errors".format(name))
         return name
```

### Comparing `pyccel-1.7.4/pyccel/naming/pythonnameclashchecker.py` & `pyccel-1.8.0/pyccel/naming/pythonnameclashchecker.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,34 +2,48 @@
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 """
 Handles name clash problems in Python
 """
-from pyccel.utilities.metaclasses import Singleton
-from pyccel.utilities.strings import create_incremented_string
+from .languagenameclashchecker import LanguageNameClashChecker
 
-class PythonNameClashChecker(metaclass = Singleton):
-    """ Class containing functions to help avoid problematic names in Python
+class PythonNameClashChecker(LanguageNameClashChecker):
+    """
+    Class containing functions to help avoid problematic names in Python.
+
+    A class which provides functionalities to check or propose variable names and
+    verify that they do not cause name clashes. Name clashes may arise when
+    generating names for new variables.
     """
     keywords = set()
 
     def has_clash(self, name, symbols):
         """ Indicate whether the proposed name causes any clashes
         """
         return any(name == k for k in self.keywords) or \
                any(name == s for s in symbols)
 
     def get_collisionless_name(self, name, symbols):
-        """ Get the name that will be used in the fortran code
         """
-        prefix = name
-        coll_symbols = self.keywords.copy()
-        coll_symbols.update(s.lower() for s in symbols)
-        if prefix in coll_symbols:
-            counter = 1
-            new_name, counter = create_incremented_string(coll_symbols,
-                    prefix = prefix, counter = counter)
-            name = name+new_name[-5:]
-        return name
+        Get a valid name which doesn't collision with symbols.
+
+        Find a new name based on the suggested name which does not
+        appear in the provided symbols. It is not necessary to exclude
+        keywords for names which were either originally valid Python
+        names, or internally generated names.
+
+        Parameters
+        ----------
+        name : str
+            The suggested name.
+        symbols : set
+            Symbols which should be considered as collisions.
+
+        Returns
+        -------
+        str
+            A new name which is collision free.
+        """
+        return self._get_collisionless_name(name, symbols)
```

### Comparing `pyccel-1.7.4/pyccel/parser/base.py` & `pyccel-1.8.0/pyccel/parser/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,42 +112,41 @@
                   severity='fatal')
 
 
 
 #==============================================================================
 
 class BasicParser(object):
+    """
+    Class for a basic parser.
 
-    """ Class for a base Parser.
-    This class contains functions and properties which are common to SyntacticParser and SemanticParser
-
-    Parameters
-    ----------
-
-        debug: bool
-            True if in debug mode.
-
-        headers: list, tuple
-            list of headers to append to the scope
+    This class contains functions and properties which are common to SyntacticParser and SemanticParser.
 
+    See Also
+    --------
+    SyntacticParser : A parser for Pyccel based on a context-free grammar.
+    SemanticParser : A parser for Pyccel based on a context-sensitive grammar.
+
+    Examples
+    --------
+    To use the BasicParser class, create an instance and call its parse() method:
+    >>> parser = BasicParser()
+    >>> result = parser.parse("1 + 2")
     """
 
-    def __init__(self,
-                 debug=False,
-                 headers=None):
-
+    def __init__(self):
         self._code = None
-        self._fst  = None
-        self._ast  = None
+        self._fst = None
+        self._ast = None
 
         self._filename = None
         self._metavars = {}
 
         # represent the scope of a function
-        self._scope    = Scope()
+        self._scope = Scope()
         self._current_class    = None
         self._current_function = None
 
         # the following flags give us a status on the parsing stage
         self._syntax_done   = False
         self._semantic_done = False
 
@@ -157,21 +156,14 @@
 
         # flag for blocking errors. if True, an error with this flag will cause
         # Pyccel to stop
         # TODO ERROR must be passed to the Parser __init__ as argument
 
         self._blocking = error_mode.value == 'developer'
 
-        if headers:
-            if not isinstance(headers, dict):
-                raise TypeError('Expecting a dict of headers')
-
-
-            self.scope.headers.update(headers)
-
         self._created_from_pickle = False
 
     def __setstate__(self, state):
         copy_slots = ('_code', '_fst', '_ast', '_metavars', '_scope', '_filename',
                 '_metavars', '_scope', '_current_class', '_current_function',
                 '_syntax_done', '_semantic_done', '_current_fst_node')
```

### Comparing `pyccel-1.7.4/pyccel/parser/extend_tree.py` & `pyccel-1.8.0/pyccel/parser/extend_tree.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/parser/grammar/headers.tx` & `pyccel-1.8.0/pyccel/parser/grammar/headers.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/parser/grammar/openacc.tx` & `pyccel-1.8.0/pyccel/parser/grammar/openacc.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/parser/grammar/openmp.tx` & `pyccel-1.8.0/pyccel/parser/grammar/openmp.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/parser/grammar/pyccel.tx` & `pyccel-1.8.0/pyccel/parser/grammar/pyccel.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/parser/parser.py` & `pyccel-1.8.0/pyccel/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/parser/scope.py` & `pyccel-1.8.0/pyccel/parser/scope.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,35 +18,54 @@
 from pyccel.naming.pythonnameclashchecker import PythonNameClashChecker
 
 from pyccel.utilities.strings import create_incremented_string
 
 errors = Errors()
 
 class Scope(object):
-    """ Class representing all objects defined within a given
-    scope
+    """
+    Class representing all objects defined within a given scope.
+
+    This class provides all necessary functionalities for creating new object
+    names without causing name clashes. It also stores all objects defined
+    within the scope. This allows us to search for variables only in relevant
+    scopes.
 
     Parameters
     ----------
-    decorators : dict
-                 A dictionary of any decorators which operate on
-                 objects in this scope
+    decorators : dict, default: ()
+        A dictionary of any decorators which operate on objects in this scope.
+
+    is_loop : bool, default: False
+        Indicates if the scope represents a loop (in Python variables declared
+        in loops are not scoped to the loop).
+
+    parent_scope : Scope, default: None
+        The enclosing scope.
+
+    used_symbols : set, default: None
+        A set of all the names which we know will appear in the scope and which
+        we therefore want to avoid when creating new names.
+
+    original_symbols : dict, default: None
+        A dictionary which maps names used in the code to the original name used
+        in the Python code.
     """
     allow_loop_scoping = False
     name_clash_checker = PythonNameClashChecker()
     __slots__ = ('_imports','_locals','_parent_scope','_sons_scopes',
             '_is_loop','_loops','_temporary_variables', '_used_symbols',
             '_dummy_counter','_original_symbol')
 
     categories = ('functions','variables','classes',
             'imports','symbolic_functions',
             'macros','templates','headers','decorators',
             'cls_constructs')
 
-    def __init__(self, *, decorators=None, is_loop = False,
+    def __init__(self, *, decorators = (), is_loop = False,
                     parent_scope = None, used_symbols = None,
                     original_symbols = None):
 
         self._imports = {k:{} for k in self.categories}
 
         self._locals  = {k:{} for k in self.categories}
 
@@ -56,16 +75,15 @@
             raise RuntimeError("Used symbols must be a dictionary")
 
         self._used_symbols = used_symbols or {}
         self._original_symbol = original_symbols or {}
 
         self._dummy_counter = 0
 
-        if decorators:
-            self._locals['decorators'].update(decorators)
+        self._locals['decorators'].update(decorators)
 
         # TODO use another name for headers
         #      => reserved keyword, or use __
         self._parent_scope       = parent_scope
         self._sons_scopes        = {}
 
 
@@ -403,66 +421,79 @@
         """ Get all symbols which already exist in this scope
         excluding enclosing scopes
         """
         return self._used_symbols
 
     def get_new_incremented_symbol(self, prefix, counter):
         """
-        Creates a new name by adding a numbered suffix to the provided prefix.
+        Create a new name by adding a numbered suffix to the provided prefix.
+
+        Create a new name which does not clash with any existing names by
+        adding a numbered suffix to the provided prefix.
 
-          Parameters
-          ----------
-          prefix : str
+        Parameters
+        ----------
+        prefix : str
+            The prefix from which the new name will be created.
 
-          Returns
-          -------
-          new_name     : str
+        counter : int
+            The starting point for the incrementation.
+
+        Returns
+        -------
+        pyccel.ast.internals.PyccelSymbol
+            The newly created name.
         """
 
-        new_name, counter = create_incremented_string(self.local_used_symbols.values(), prefix = prefix)
+        new_name, counter = create_incremented_string(self.local_used_symbols.values(),
+                                    prefix = prefix, counter = counter, name_clash_checker = self.name_clash_checker)
 
         new_symbol = PyccelSymbol(new_name, is_temp=True)
 
         self.insert_symbol(new_symbol)
 
         return new_symbol, counter
 
     def get_new_name(self, current_name = None):
         """
+        Get a new name which does not clash with any names in the current context.
+
         Creates a new name. A current_name can be provided indicating the name the
         user would like to use if possible. If this name is not available then it
         will be used as a prefix for the new name.
         If no current_name is provided, then the standard prefix is used, and the
         dummy counter is used and updated to facilitate finding the next value of
-        this common case
+        this common case.
+
+        Parameters
+        ----------
+        current_name : str, default: None
+            The name the user would like to use if possible.
 
-          Parameters
-          ----------
-          current_name : str
-
-          Returns
-          -------
-          new_name     : PyccelSymbol
+        Returns
+        -------
+        PyccelSymbol
+            The new name which will be printed in the code.
         """
         if current_name is not None and not self.name_clash_checker.has_clash(current_name, self.all_used_symbols):
             new_name = PyccelSymbol(current_name)
             self.insert_symbol(new_name)
             return new_name
 
         if current_name is None:
             # Avoid confusing names by also searching in parent scopes
             new_name, self._dummy_counter = create_incremented_string(self.all_used_symbols,
                                                 prefix = current_name,
-                                                counter = self._dummy_counter)
+                                                counter = self._dummy_counter,
+                                                name_clash_checker = self.name_clash_checker)
         else:
             # When a name is suggested, try to stick to it
             new_name,_ = create_incremented_string(self.all_used_symbols, prefix = current_name)
 
         new_name = PyccelSymbol(new_name, is_temp = True)
-
         self.insert_symbol(new_name)
 
         return new_name
 
     def get_temporary_variable(self, dtype_or_var, name = None, **kwargs):
         """
         Get a temporary variable
```

### Comparing `pyccel-1.7.4/pyccel/parser/semantic.py` & `pyccel-1.8.0/pyccel/parser/semantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,16 +266,29 @@
         """
         return self._program_namespace
 
     #================================================================
     #                     Public functions
     #================================================================
 
-    def annotate(self, **settings):
-        """."""
+    def annotate(self):
+        """
+        Add type information to the AST.
+
+        This function is the entry point for this class. It annotates the
+        AST object created by the syntactic stage which was collected
+        in the constructor. The annotation adds all necessary information
+        about the type etc to describe the object sufficiently well for
+        printing. See the developer docs for more details.
+
+        Returns
+        -------
+        pyccel.ast.basic.Basic
+            An annotated object which can be printed.
+        """
 
         if self.semantic_done:
             print ('> semantic analysis already done')
             return self.ast
 
         # TODO - add settings to Errors
         #      - filename
@@ -288,15 +301,15 @@
         # then we treat the current file
 
         ast = self.ast
 
         self._allocs.append([])
         # we add the try/except to allow the parser to find all possible errors
         pyccel_stage.set_stage('semantic')
-        ast = self._visit(ast, **settings)
+        ast = self._visit(ast)
 
         self._ast = ast
 
         self._semantic_done = True
 
         return ast
 
@@ -460,34 +473,52 @@
         if len(expr.body)>0 and not isinstance(expr.body[-1], Return):
             deallocs = [Deallocate(i) for i in self._allocs[-1]]
         else:
             deallocs = []
         self._allocs.pop()
         return deallocs
 
-    def _infer_type(self, expr, **settings):
+    def _infer_type(self, expr):
         """
-        type inference for expressions
+        Infer all relevant type information for the expression.
+
+        Create a dictionary describing all the type information that can be
+        inferred about the expression `expr`. This includes information about:
+        - `datatype`
+        - `precision`
+        - `rank`
+        - `shape`
+        - `order`
+        - `memory_handling`
+        - `cls_base`
+        - `is_target`
+
+        Parameters
+        ----------
+        expr : pyccel.ast.basic.Basic
+                An AST object representing an object in the code whose type
+                must be determined.
+
+        Returns
+        -------
+        dict
+            Dictionary containing all the type information which was inferred.
         """
         # TODO - add settings to Errors
         #      - line and column
         #      - blocking errors
 
         errors = Errors()
 
-        verbose = settings.pop('verbose', False)
-        if verbose:
-            print ('*** type inference for : ', type(expr))
-
         d_var = {}
         # TODO improve => put settings as attribut of Parser
 
         if expr in (PythonInt, PythonFloat, PythonComplex, PythonBool, NumpyBool, NumpyInt, NumpyInt8, NumpyInt16,
                       NumpyInt32, NumpyInt64, NumpyComplex, NumpyComplex64,
-					  NumpyComplex128, NumpyFloat, NumpyFloat64, NumpyFloat32):
+                      NumpyComplex128, NumpyFloat, NumpyFloat64, NumpyFloat32):
 
             d_var['datatype'   ] = '*'
             d_var['rank'       ] = 0
             d_var['precision'  ] = 0
             return d_var
 
         elif isinstance(expr, Variable):
@@ -521,15 +552,15 @@
             if any(getattr(a, 'on_heap', False) for a in expr.args):
                 d_var['memory_handling'] = 'heap'
             else:
                 d_var['memory_handling'] = 'stack'
             return d_var
 
         elif isinstance(expr, Duplicate):
-            d = self._infer_type(expr.val, **settings)
+            d = self._infer_type(expr.val)
 
             # TODO must check that it is consistent with pyccel's rules
             # TODO improve
             d_var['datatype'      ] = d['datatype']
             d_var['rank'          ] = expr.rank
             d_var['shape'         ] = expr.shape
             d_var['order'         ] = expr.order
@@ -749,40 +780,37 @@
                     bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                     severity='fatal')
             if isinstance(val, TupleVariable):
                 return PythonTuple(*(val.get_vars()*length))
             else:
                 return PythonTuple(*(val.args*length))
 
-    def _handle_function_args(self, arguments, **settings):
+    def _handle_function_args(self, arguments):
         """
         Get a list of all function arguments.
 
         Get a list of all the function arguments which are passed
         to a function. This is done by visiting the syntactic
         FunctionCallArguments. If this argument contains a
         starred arguments object then the contents of this object
         are extracted into the final list.
 
         Parameters
         ----------
         arguments : list of FunctionCallArgument
             The arguments which were passed to the function.
 
-        **settings : dict
-            Any settings to be passed to the `_visit` function.
-
         Returns
         -------
         list of FunctionCallArgument
             The arguments passed to the function.
         """
         args  = []
         for arg in arguments:
-            a = self._visit(arg, **settings)
+            a = self._visit(arg)
             if isinstance(a.value, StarredArguments):
                 args.extend([FunctionCallArgument(av) for av in a.value.args_var])
             else:
                 args.append(a)
         return args
 
     def get_type_description(self, var, include_rank = True):
@@ -849,15 +877,15 @@
                         symbol = expr,
                         severity='error')
             if f_arg.rank > 1 and i_arg.order != f_arg.order:
                 errors.report(INCOMPATIBLE_ORDERING.format(idx=idx+1, arg=i_arg, func=expr.func_name, order=f_arg.order),
                         symbol = expr,
                         severity='error')
 
-    def _handle_function(self, expr, func, args, **settings):
+    def _handle_function(self, expr, func, args):
         """
         Create the node representing the function call.
 
         Create a FunctionCall or an instance of a PyccelInternalFunction
         from the function information and arguments.
 
         Parameters
@@ -867,17 +895,14 @@
 
         func : FunctionDef instance, Interface instance or PyccelInternalFunction type
                The function being called.
 
         args : tuple
                The arguments passed to the function.
 
-        **settings : dict
-            The settings passed to _visit functions.
-
         Returns
         -------
         FunctionCall/PyccelInternalFunction
             The semantic representation of the call.
         """
         if isinstance(func, PyccelFunctionDef):
             func = func.cls_name
@@ -892,28 +917,30 @@
 
             return new_expr
         else:
             if self._current_function == func.name:
                 if len(func.results)>0 and not isinstance(func.results[0].var, PyccelAstNode):
                     errors.report(RECURSIVE_RESULTS_REQUIRED, symbol=func, severity="fatal")
 
-            parent_assign = expr.get_direct_user_nodes(lambda x: isinstance(x, Assign))
-            if not parent_assign and len(func.results) == 1 and func.results[0].var.rank > 0:
+            parent_assign = expr.get_direct_user_nodes(lambda x: isinstance(x, Assign) and not isinstance(x, AugAssign))
+
+            func_args = func.arguments if isinstance(func, FunctionDef) else func.functions[0].arguments
+            func_results = func.results if isinstance(func, FunctionDef) else func.functions[0].results
+
+            if not parent_assign and len(func_results) == 1 and func_results[0].var.rank > 0:
                 tmp_var = PyccelSymbol(self.scope.get_new_name())
                 assign = Assign(tmp_var, expr)
                 assign.set_fst(expr.fst)
                 self._additional_exprs[-1].append(self._visit(assign))
                 return self._visit(tmp_var)
 
-            if isinstance(func, FunctionDef) and len(args) > len(func.arguments):
+            if len(args) > len(func_args):
                 errors.report("Too many arguments passed in function call",
                         symbol = expr,
                         severity='fatal')
-
-            func_args = func.arguments if isinstance(func, FunctionDef) else func.functions[0].arguments
             # Sort arguments to match the order in the function definition
             input_args = [a for a in args if a.keyword is None]
             nargs = len(input_args)
             for ka in func_args[nargs:]:
                 key = ka.name
                 relevant_args = [a for a in args[nargs:] if a.keyword == key]
                 n_relevant_args = len(relevant_args)
@@ -1033,48 +1060,52 @@
             rhs.is_target = not rhs.is_alias
 
         if isinstance(rhs, IndexedElement) and rhs.rank > 0 and \
                 (getattr(rhs.base, 'is_ndarray', False) or getattr(rhs.base, 'is_alias', False)):
             d_lhs['memory_handling'] = 'alias'
             rhs.base.is_target = not rhs.base.is_alias
 
-    def _assign_lhs_variable(self, lhs, d_var, rhs, new_expressions, is_augassign,arr_in_multirets=False, **settings):
+    def _assign_lhs_variable(self, lhs, d_var, rhs, new_expressions, is_augassign,arr_in_multirets=False):
         """
-        Create a lhs based on the information in d_var
-        If the lhs already exists then check that it has the expected properties.
+        Create a variable from the left-hand side (lhs) of an assignment.
+        
+        Create a lhs based on the information in d_var, if the lhs already exists
+        then check that it has the expected properties.
 
         Parameters
         ----------
         lhs : PyccelSymbol (or DottedName of PyccelSymbols)
-            The representation of the lhs provided by the SyntacticParser
+            The representation of the lhs provided by the SyntacticParser.
 
         d_var : dict
-            Dictionary of expected lhs properties
+            Dictionary of expected lhs properties.
 
         rhs : Variable / expression
             The representation of the rhs provided by the SemanticParser.
             This is necessary in order to set the rhs 'is_target' property
-            if necessary
+            if necessary.
 
-        new_expression : list
+        new_expressions : list
             A list which allows collection of any additional expressions
-            resulting from this operation (e.g. Allocation)
+            resulting from this operation (e.g. Allocation).
 
         is_augassign : bool
             Indicates whether this is an assign ( = ) or an augassign ( += / -= / etc )
             This is necessary as the restrictions on the dtype are less strict in this
-            case
+            case.
 
         arr_in_multirets : bool
             If True, rhs has an array in its results, otherwise, it should be set to False.
             It helps when we don't need lhs to be a pointer in case of a returned array in
             a tuple of results.
 
-        settings : dictionary
-            Provided to all _visit_ClassName functions
+        Returns
+        -------
+        pyccel.ast.variable.Variable
+            The representation of the lhs provided by the SemanticParser.
         """
 
         if isinstance(lhs, IndexedElement):
             lhs = self._visit(lhs)
         elif isinstance(lhs, PyccelSymbol):
 
             name = lhs
@@ -1226,15 +1257,15 @@
                 lhs    = member.clone(member.name, new_class = DottedVariable, lhs = var)
 
                 # update the attributes of the class and push it to the scope
                 attributes += [member]
                 new_cls = ClassDef(cls_name, attributes, [], superclass=parent)
                 self.scope.parent_scope.insert_class(new_cls)
             else:
-                lhs = self._visit(lhs, **settings)
+                lhs = self._visit(lhs)
         else:
             lhs_type = str(type(lhs))
             raise NotImplementedError(f"_assign_lhs_variable does not handle {lhs_type}")
 
         return lhs
 
     def _ensure_inferred_type_matches_existing(self, dtype, d_var, var, is_augassign, new_expressions, rhs):
@@ -1403,41 +1434,44 @@
                     new_expressions.append(Allocate(var,
                         shape=d_var['shape'], order=d_var['order'],
                         status=status))
 
         if var.precision == -1 and precision != var.precision:
             var.use_exact_precision()
 
-    def _assign_GeneratorComprehension(self, lhs_name, expr, **settings):
+    def _assign_GeneratorComprehension(self, lhs_name, expr):
         """
-        Visit the GeneratorComprehension node creating all necessary expressions
-        for its definition
+        Visit the GeneratorComprehension node.
+
+        Create all necessary expressions for the
+        GeneratorComprehension node definition.
 
         Parameters
         ----------
         lhs_name : str
-                    The name to which the expression is assigned
+                    The name to which the expression is assigned.
         expr : GeneratorComprehension
+                The GeneratorComprehension node.
 
-        Results
+        Returns
         -------
-        new_expr : CodeBlock
-                   CodeBlock containing the semantic version of the GeneratorComprehension node
+        pyccel.ast.functionalexpr.GeneratorComprehension
+                CodeBlock containing the semantic version of the GeneratorComprehension node
         """
         result   = expr.expr
 
         loop = expr.loops
         nlevels = 0
         # Create throw-away variable to help obtain result type
         index   = Variable('int',self.scope.get_new_name('to_delete'), is_temp=True)
         self.scope.insert_variable(index)
         new_expr = []
         while isinstance(loop, For):
             nlevels+=1
-            iterable = Iterable(self._visit(loop.iterable, **settings))
+            iterable = Iterable(self._visit(loop.iterable))
             n_index = max(1, iterable.num_loop_counters_required)
             # Set dummy indices to iterable object in order to be able to
             # obtain a target with a deducible dtype
             iterable.set_loop_counter(*[index]*n_index)
 
             iterator = loop.target
 
@@ -1464,35 +1498,35 @@
                     loop_elem = loop.body.body[0]
             loop = loop_elem
         # Remove the throw-away variable from the scope
         self.scope.remove_variable(index)
 
         # Visit result expression (correctly defined as iterator
         # objects exist in the scope despite not being defined)
-        result = self._visit(result, **settings)
+        result = self._visit(result)
         if isinstance(result, CodeBlock):
             result = result.body[-1]
 
         # Infer the final dtype of the expression
-        d_var = self._infer_type(result, **settings)
+        d_var = self._infer_type(result)
         dtype = d_var.pop('datatype')
         d_var['is_temp'] = expr.lhs.is_temp
 
         lhs  = self.check_for_variable(lhs_name)
         if lhs:
             self._ensure_inferred_type_matches_existing(dtype, d_var, lhs, False, new_expr, None)
         else:
             lhs_name = self.scope.get_expected_name(lhs_name)
             lhs = Variable(dtype, lhs_name, **d_var)
             self.scope.insert_variable(lhs)
 
         # Iterate over the loops
         # This provides the definitions of iterators as well
         # as the central expression
-        loops = [self._visit(expr.loops, **settings)]
+        loops = [self._visit(expr.loops)]
 
         # If necessary add additional expressions corresponding
         # to nested GeneratorComprehensions
         if new_expr:
             loop = loops[0]
             for _ in range(nlevels-1):
                 loop = loop.body.body[0]
@@ -1526,48 +1560,59 @@
         return expr_new
 
     #====================================================
     #                 _visit functions
     #====================================================
 
 
-    def _visit(self, expr, **settings):
-        """Annotates the AST.
+    def _visit(self, expr):
+        """
+        Annotate the AST.
 
         The annotation is done by finding the appropriate function _visit_X
         for the object expr. X is the type of the object expr. If this function
         does not exist then the method resolution order is used to search for
         other compatible _visit_X functions. If none are found then an error is
-        raised
+        raised.
+        
+        Parameters
+        ----------
+        expr : pyccel.ast.basic.Basic
+            Object to visit of type X.
+        
+        Returns
+        -------
+        pyccel.ast.basic.Basic
+            AST object which is the semantic equivalent of expr.
         """
 
         # TODO - add settings to Errors
         #      - line and column
         #      - blocking errors
         current_fst = self._current_fst_node
 
         if hasattr(expr,'fst') and expr.fst is not None:
             self._current_fst_node = expr.fst
 
         classes = type(expr).__mro__
         for cls in classes:
             annotation_method = '_visit_' + cls.__name__
             if hasattr(self, annotation_method):
-                obj = getattr(self, annotation_method)(expr, **settings)
+                obj = getattr(self, annotation_method)(expr)
                 if isinstance(obj, Basic) and self._current_fst_node:
                     obj.set_fst(self._current_fst_node)
                 self._current_fst_node = current_fst
                 return obj
 
         # Unknown object, we raise an error.
         return errors.report(PYCCEL_RESTRICTION_TODO, symbol=type(expr),
             bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
             severity='fatal')
 
-    def _visit_Module(self, expr, **settings):
+    def _visit_Module(self, expr):
         body = self._visit(expr.program).body
         program_body      = []
         init_func_body    = []
         mod_name = self.metavars.get('module_name', None)
         if mod_name is None:
             mod_name = expr.name
         else:
@@ -1735,94 +1780,84 @@
                             container.imports['imports'].values(),
                             scope=self._program_namespace)
 
             mod.program = program
 
         return mod
 
-    def _visit_tuple(self, expr, **settings):
-        return tuple(self._visit(i, **settings) for i in expr)
-
-    def _visit_PythonTuple(self, expr, **settings):
-        ls = [self._visit(i, **settings) for i in expr]
+    def _visit_PythonTuple(self, expr):
+        ls = [self._visit(i) for i in expr]
         return PythonTuple(*ls)
 
-    def _visit_PythonList(self, expr, **settings):
-        ls = [self._visit(i, **settings) for i in expr]
+    def _visit_PythonList(self, expr):
+        ls = [self._visit(i) for i in expr]
         expr = PythonList(*ls)
 
         if not expr.is_homogeneous:
             errors.report(PYCCEL_RESTRICTION_INHOMOG_LIST, symbol=expr,
                 bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                 severity='fatal')
         return expr
 
-    def _visit_FunctionCallArgument(self, expr, **settings):
-        value = self._visit(expr.value, **settings)
+    def _visit_FunctionCallArgument(self, expr):
+        value = self._visit(expr.value)
         a = FunctionCallArgument(value, expr.keyword)
         if isinstance(a.value, PyccelArithmeticOperator) and a.value.rank:
             tmp_var = self.scope.get_new_name()
             assign = self._visit(Assign(tmp_var, expr.value, fst = expr.value.fst))
             self._additional_exprs[-1].append(assign)
             a = FunctionCallArgument(self._visit(tmp_var))
         return a
 
-    def _visit_FunctionDefArgument(self, expr, **settings):
-        var   = self._visit(expr.var, **settings)
-        value = self._visit(expr.value, **settings)
-        return FunctionDefArgument(var, value=value,
-                annotation=expr.annotation,
-                kwonly=expr.is_kwonly)
-
-    def _visit_CodeBlock(self, expr, **settings):
+    def _visit_CodeBlock(self, expr):
         ls = []
         self._additional_exprs.append([])
         for b in expr.body:
 
             # Save parsed code
-            line = self._visit(b, **settings)
+            line = self._visit(b)
             ls.extend(self._additional_exprs[-1])
             self._additional_exprs[-1] = []
             if isinstance(line, CodeBlock):
                 ls.extend(line.body)
             else:
                 ls.append(line)
         self._additional_exprs.pop()
 
         return CodeBlock(ls)
 
-    def _visit_Nil(self, expr, **settings):
+    def _visit_Nil(self, expr):
         expr.clear_user_nodes()
         return expr
 
-    def _visit_EmptyNode(self, expr, **settings):
+    def _visit_EmptyNode(self, expr):
         expr.clear_user_nodes()
         return expr
 
-    def _visit_Break(self, expr, **settings):
+    def _visit_Break(self, expr):
         expr.clear_user_nodes()
         return expr
 
-    def _visit_Continue(self, expr, **settings):
+    def _visit_Continue(self, expr):
         expr.clear_user_nodes()
         return expr
 
-    def _visit_Comment(self, expr, **settings):
+    def _visit_Comment(self, expr):
         expr.clear_user_nodes()
         return expr
 
-    def _visit_CommentBlock(self, expr, **settings):
+    def _visit_CommentBlock(self, expr):
         expr.clear_user_nodes()
         return expr
 
-    def _visit_AnnotatedComment(self, expr, **settings):
+    def _visit_AnnotatedComment(self, expr):
         expr.clear_user_nodes()
         return expr
 
-    def _visit_OmpAnnotatedComment(self, expr, **settings):
+    def _visit_OmpAnnotatedComment(self, expr):
         code = expr._user_nodes
         code = code[-1]
         index = code.body.index(expr)
         combined_loop = expr.combined and ('for' in expr.combined or 'distribute' in expr.combined or 'taskloop' in expr.combined)
 
         if isinstance(expr, (OMP_Sections_Construct, OMP_Single_Construct)) \
            and expr.has_nowait:
@@ -1849,52 +1884,52 @@
                 msg = f"Statement after {type_name} must be a for loop."
                 errors.report(msg, symbol=expr,
                     severity='fatal')
 
         expr.clear_user_nodes()
         return expr
 
-    def _visit_Omp_End_Clause(self, expr, **settings):
+    def _visit_Omp_End_Clause(self, expr):
         end_loop = any(c in expr.txt for c in ['for', 'distribute', 'taskloop', 'simd'])
         if end_loop:
             errors.report("For loops do not require an end clause. This clause is ignored",
                     severity='warning', symbol=expr)
             return EmptyNode()
         else:
             expr.clear_user_nodes()
             return expr
 
-    def _visit_Literal(self, expr, **settings):
+    def _visit_Literal(self, expr):
         expr.clear_user_nodes()
         return expr
-    def _visit_PythonComplex(self, expr, **settings):
+    def _visit_PythonComplex(self, expr):
         expr.clear_user_nodes()
         return expr
-    def _visit_Pass(self, expr, **settings):
+    def _visit_Pass(self, expr):
         expr.clear_user_nodes()
         return expr
 
-    def _visit_Variable(self, expr, **settings):
+    def _visit_Variable(self, expr):
         name = self.scope.get_python_name(expr.name)
         return self.get_variable(name)
 
-    def _visit_str(self, expr, **settings):
+    def _visit_str(self, expr):
         return repr(expr)
 
-    def _visit_Slice(self, expr, **settings):
+    def _visit_Slice(self, expr):
         start = self._visit(expr.start) if expr.start is not None else None
         stop = self._visit(expr.stop) if expr.stop is not None else None
         step = self._visit(expr.step) if expr.step is not None else None
 
         return Slice(start, stop, step)
 
-    def _visit_IndexedElement(self, expr, **settings):
+    def _visit_IndexedElement(self, expr):
         var = self._visit(expr.base)
         # TODO check consistency of indices with shape/rank
-        args = [self._visit(idx, **settings) for idx in expr.indices]
+        args = [self._visit(idx) for idx in expr.indices]
 
         if (len(args) == 1 and isinstance(args[0], (TupleVariable, PythonTuple))):
             args = args[0]
 
         elif any(isinstance(a, (TupleVariable, PythonTuple)) for a in args):
             n_exprs = None
             for a in args:
@@ -1905,15 +1940,15 @@
                         n_exprs = len(a)
             new_expr_args = [[a[i] if hasattr(a, '__getitem__') else a for a in args]
                              for i in range(n_exprs)]
             return NumpyArray(PythonTuple(*[var[a] for a in new_expr_args]))
 
         return self._extract_indexed_from_var(var, args, expr)
 
-    def _visit_PyccelSymbol(self, expr, **settings):
+    def _visit_PyccelSymbol(self, expr):
         name = expr
 
         var = self.check_for_variable(name)
 
         if var is None:
             var = self.scope.find(name, 'functions')
         if var is None:
@@ -1929,15 +1964,15 @@
             else:
                 errors.report(UNDEFINED_VARIABLE, symbol=name,
                     bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                     severity='fatal')
         return var
 
 
-    def _visit_DottedName(self, expr, **settings):
+    def _visit_DottedName(self, expr):
 
         var = self.check_for_variable(_get_name(expr))
         if var:
             return var
 
         lhs = expr.name[0] if len(expr.name) == 2 \
                 else DottedName(*expr.name[:-1])
@@ -1975,20 +2010,20 @@
                 elif isinstance(rhs, ConstructorCall):
                     self.scope.imports['classes'][new_name] = first[rhs_name]
                 elif isinstance(rhs, Variable):
                     self.scope.imports['variables'][new_name] = rhs
 
                 if isinstance(rhs, FunctionCall):
                     # If object is a function
-                    args  = self._handle_function_args(rhs.args, **settings)
+                    args  = self._handle_function_args(rhs.args)
                     func  = first[rhs_name]
                     if new_name != rhs_name:
                         if hasattr(func, 'clone') and not isinstance(func, PyccelFunctionDef):
                             func  = func.clone(new_name)
-                    return self._handle_function(expr, func, args, **settings)
+                    return self._handle_function(expr, func, args)
                 elif isinstance(rhs, Constant):
                     var = first[rhs_name]
                     if new_name != rhs_name:
                         var.name = new_name
                     return var
                 else:
                     # If object is something else (eg. dict)
@@ -2022,19 +2057,19 @@
                             self._current_fst_node.col_offset),
                         severity='fatal')
             macro = self.scope.find(rhs_name, 'macros')
             if macro is not None:
                 master = macro.master
                 args = rhs.args
                 args = [lhs] + list(args)
-                args = [self._visit(i, **settings) for i in args]
+                args = [self._visit(i) for i in args]
                 args = macro.apply(args)
                 return FunctionCall(master, args, self._current_function)
 
-            args = [self._visit(arg, **settings) for arg in
+            args = [self._visit(arg) for arg in
                     rhs.args]
             for i in methods:
                 if str(i.name) == rhs_name:
                     if 'numpy_wrapper' in i.decorators.keys():
                         func = i.decorators['numpy_wrapper']
                         self.insert_import('numpy', AsName(func, rhs_name))
                         return func(visited_lhs, *args)
@@ -2051,15 +2086,15 @@
                         symbol=method.name,
                         bounding_box=(self._current_fst_node.lineno,
                             self._current_fst_node.col_offset),
                         severity='fatal')
             # standard class attribute
             if rhs in attr_name:
                 self._current_class = cls_base
-                second = self._visit(rhs, **settings)
+                second = self._visit(rhs)
                 self._current_class = None
                 return second.clone(second.name, new_class = DottedVariable, lhs = visited_lhs)
 
             # class property?
             else:
                 for i in methods:
                     if i.name == rhs and \
@@ -2085,20 +2120,20 @@
                 return FunctionCall(macro.master, args, self._current_function)
 
         # did something go wrong?
         return errors.report(f'Attribute {rhs_name} not found',
             bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
             severity='fatal')
 
-    def _visit_PyccelOperator(self, expr, **settings):
-        args     = [self._visit(a, **settings) for a in expr.args]
+    def _visit_PyccelOperator(self, expr):
+        args     = [self._visit(a) for a in expr.args]
         return self._create_PyccelOperator(expr, args)
 
-    def _visit_PyccelAdd(self, expr, **settings):
-        args = [self._visit(a, **settings) for a in expr.args]
+    def _visit_PyccelAdd(self, expr):
+        args = [self._visit(a) for a in expr.args]
         if isinstance(args[0], (TupleVariable, PythonTuple, Concatenate, Duplicate)):
             is_homogeneous = all((isinstance(a, (TupleVariable, PythonTuple)) and a.is_homogeneous) \
                                 or isinstance(a, (Concatenate, Duplicate)) for a in args)
             if is_homogeneous:
                 return Concatenate(*args)
             else:
                 def get_vars(a):
@@ -2117,26 +2152,26 @@
                         raise NotImplementedError(f"Unexpected type {a_type} in tuple addition")
                 tuple_args = [ai for a in args for ai in get_vars(a)]
                 expr_new = PythonTuple(*tuple_args)
         else:
             expr_new = self._create_PyccelOperator(expr, args)
         return expr_new
 
-    def _visit_PyccelMul(self, expr, **settings):
-        args = [self._visit(a, **settings) for a in expr.args]
+    def _visit_PyccelMul(self, expr):
+        args = [self._visit(a) for a in expr.args]
         if isinstance(args[0], (TupleVariable, PythonTuple, PythonList)):
             expr_new = self._create_Duplicate(args[0], args[1])
         elif isinstance(args[1], (TupleVariable, PythonTuple, PythonList)):
             expr_new = self._create_Duplicate(args[1], args[0])
         else:
             expr_new = self._create_PyccelOperator(expr, args)
         return expr_new
 
-    def _visit_PyccelPow(self, expr, **settings):
-        base, exponent = [self._visit(a, **settings) for a in expr.args]
+    def _visit_PyccelPow(self, expr):
+        base, exponent = [self._visit(a) for a in expr.args]
 
         exp_val = exponent
         if isinstance(exponent, LiteralInteger):
             exp_val = exponent.python_value
         elif isinstance(exponent, PyccelAssociativeParenthesis):
             exp = exponent.args[0]
             # Handle (1/2)
@@ -2159,17 +2194,17 @@
 
             pyccel_stage.set_stage('semantic')
 
             return self._visit(new_call)
         else:
             return PyccelPow(base, exponent)
 
-    def _visit_MathSqrt(self, expr, **settings):
+    def _visit_MathSqrt(self, expr):
         func = self.scope.find(expr.funcdef, 'functions')
-        arg, = self._handle_function_args(expr.args, **settings) #pylint: disable=unbalanced-tuple-unpacking
+        arg, = self._handle_function_args(expr.args) #pylint: disable=unbalanced-tuple-unpacking
         if isinstance(arg.value, PyccelMul):
             mul1, mul2 = arg.value.args
             mul1_syn, mul2_syn = expr.args[0].value.args
             is_abs = False
             if mul1 is mul2 and mul1.dtype in (NativeInteger(), NativeFloat()):
                 pyccel_stage.set_stage('syntactic')
 
@@ -2214,17 +2249,17 @@
                 self._visit(new_import)
                 new_call = FunctionCall(fabs_name, [base_syn])
 
                 pyccel_stage.set_stage('semantic')
 
                 return self._visit(new_call)
 
-        return self._handle_function(expr, func, (arg,), **settings)
+        return self._handle_function(expr, func, (arg,))
 
-    def _visit_Lambda(self, expr, **settings):
+    def _visit_Lambda(self, expr):
         expr_names = set(str(a) for a in expr.expr.get_attribute_nodes(PyccelSymbol))
         var_names = map(str, expr.variables)
         missing_vars = expr_names.difference(var_names)
         if len(missing_vars) > 0:
             errors.report(UNDEFINED_LAMBDA_VARIABLE, symbol = missing_vars,
                 bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                 severity='fatal')
@@ -2239,30 +2274,30 @@
             else:
 
                 f = f(*func.args)
                 expr_new = expr.expr.subs(func, f)
                 expr = Lambda(tuple(expr.variables), expr_new)
         return expr
 
-    def _visit_FunctionCall(self, expr, **settings):
+    def _visit_FunctionCall(self, expr):
         name     = expr.funcdef
         try:
             name = self.scope.get_expected_name(name)
         except RuntimeError:
             pass
 
         func     = self.scope.find(name, 'functions')
 
         # Check for specialised method
         if isinstance(func, PyccelFunctionDef):
             annotation_method = '_visit_' + func.cls_name.__name__
             if hasattr(self, annotation_method):
-                return getattr(self, annotation_method)(expr, **settings)
+                return getattr(self, annotation_method)(expr)
 
-        args = self._handle_function_args(expr.args, **settings)
+        args = self._handle_function_args(expr.args)
         # Correct keyword names if scope is available
         # The scope is only available if the function body has been parsed
         # (i.e. not for headers or builtin functions)
         if isinstance(func, FunctionDef) and func.scope:
             args = [a if a.keyword is None else \
                     FunctionCallArgument(a.value, func.scope.get_expected_name(a.keyword)) \
                     for a in args]
@@ -2314,81 +2349,81 @@
             else:
                 func = self.scope.find(name, 'functions')
             if func is None:
                 return errors.report(UNDEFINED_FUNCTION, symbol=name,
                         bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                         severity='fatal')
             else:
-                return self._handle_function(expr, func, args, **settings)
+                return self._handle_function(expr, func, args)
 
-    def _visit_Expr(self, expr, **settings):
+    def _visit_Expr(self, expr):
         errors.report(PYCCEL_RESTRICTION_TODO, symbol=expr,
             bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
             severity='fatal')
 
 
-    def _visit_Assign(self, expr, **settings):
+    def _visit_Assign(self, expr):
         # TODO unset position at the end of this part
         new_expressions = []
         fst = expr.fst
         assert(fst)
 
         rhs = expr.rhs
         lhs = expr.lhs
 
         # Steps before visiting
         if isinstance(rhs, GeneratorComprehension):
             rhs.substitute(rhs.lhs, lhs)
-            genexp = self._assign_GeneratorComprehension(_get_name(lhs), rhs, **settings)
+            genexp = self._assign_GeneratorComprehension(_get_name(lhs), rhs)
             if isinstance(expr, AugAssign):
                 new_expressions.append(genexp)
                 rhs = genexp.lhs
             elif genexp.lhs.name == lhs:
                 return genexp
             else:
                 new_expressions.append(genexp)
                 rhs = genexp.lhs
         elif isinstance(rhs, IfTernaryOperator):
-            value_true  = self._visit(rhs.value_true, **settings)
+            value_true  = self._visit(rhs.value_true)
             if value_true.rank > 0 or value_true.dtype is NativeString():
                 # Temporarily deactivate type checks to construct syntactic assigns
                 pyccel_stage.set_stage('syntactic')
                 assign_true  = Assign(lhs, rhs.value_true, fst = fst)
                 assign_false = Assign(lhs, rhs.value_false, fst = fst)
                 pyccel_stage.set_stage('semantic')
 
-                cond  = self._visit(rhs.cond, **settings)
+                cond  = self._visit(rhs.cond)
                 true_section  = IfSection(cond, [self._visit(assign_true)])
                 false_section = IfSection(LiteralTrue(), [self._visit(assign_false)])
                 return If(true_section, false_section)
 
         # Visit object
         if isinstance(rhs, FunctionCall):
             name = rhs.funcdef
             macro = self.scope.find(name, 'macros')
             if macro is None:
-                rhs = self._visit(rhs, **settings)
+                rhs = self._visit(rhs)
             else:
 
                 # TODO check types from FunctionDef
                 master = macro.master
                 results = []
-                args = [self._visit(i, **settings) for i in rhs.args]
+                args = [self._visit(i) for i in rhs.args]
                 args_names = [arg.value.name for arg in args if isinstance(arg.value, Variable)]
                 d_m_args = {arg.value.name:arg.value for arg in macro.master_arguments
                                   if isinstance(arg.value, Variable)}
 
                 if not sympy_iterable(lhs):
                     lhs = [lhs]
                 results_shapes = macro.get_results_shapes(args)
                 for m_result, shape, result in zip(macro.results, results_shapes, lhs):
                     if m_result in d_m_args and not result in args_names:
                         d_result = self._infer_type(d_m_args[m_result])
                         d_result['shape'] = shape
-                        tmp = self._assign_lhs_variable(result, d_result, None, new_expressions, False, **settings)
+                        tmp = self._assign_lhs_variable(result, d_result, None, new_expressions, False)
                         results.append(tmp)
                     elif result in args_names:
                         _name = _get_name(result)
                         tmp = self.get_variable(_name)
                         results.append(tmp)
                     else:
                         # TODO: check for result in master_results
@@ -2407,66 +2442,24 @@
                         return func_call
                 else:
                     # TODO treate interface case
                     errors.report(PYCCEL_RESTRICTION_TODO,
                                   bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                                   severity='fatal')
 
-        elif isinstance(rhs, DottedVariable):
-            var = rhs.rhs
-            name = _get_name(var)
-            macro = self.scope.find(name, 'macros')
-            if macro is None:
-                rhs = self._visit(rhs, **settings)
-            else:
-                master = macro.master
-                if isinstance(macro, MacroVariable):
-                    rhs = master
-                else:
-                    # If macro is function, create left-hand side variable
-                    if isinstance(master, FunctionDef) and master.results:
-                        d_var = self._infer_type(master.results[0].var, **settings)
-                        dtype = d_var.pop('datatype')
-                        lhs = Variable(dtype, lhs.name, **d_var, is_temp=lhs.is_temp)
-                        var = self.check_for_variable(lhs.name)
-                        if var is None:
-                            self.scope.insert_variable(lhs)
-
-                    name = macro.name
-                    if not sympy_iterable(lhs):
-                        lhs = [lhs]
-                    results = []
-                    for a in lhs:
-                        _name = _get_name(a)
-                        var = self.get_variable(_name)
-                        results.append(var)
-
-                    args = rhs.rhs.args
-                    args = [rhs.lhs] + list(args)
-                    args = [self._visit(i, **settings) for i in args]
-
-                    args = macro.apply(args, results=results)
-
-                    # Distinguish between function
-                    if master.results:
-                        return Assign(lhs[0], FunctionCall(master, args, self._current_function))
-                    else:
-                        return FunctionCall(master, args, self._current_function)
-
         else:
-            rhs = self._visit(rhs, **settings)
+            rhs = self._visit(rhs)
 
         if isinstance(rhs, FunctionDef):
 
             # case of lambdify
 
             rhs = rhs.rename(expr.lhs.name)
             for i in rhs.body:
                 i.set_fst(fst)
-            rhs = self._visit_FunctionDef(rhs, **settings)
             return rhs
 
         elif isinstance(rhs, CodeBlock):
             if len(rhs.body)>1 and isinstance(rhs.body[1], FunctionalFor):
                 return rhs
 
             # case of complex stmt
@@ -2474,84 +2467,72 @@
             # into a list of stmts
             stmts = rhs.body
             stmt  = stmts[-1]
             lhs   = expr.lhs
             if isinstance(lhs, PyccelSymbol):
                 name = lhs
                 if self.check_for_variable(name) is None:
-                    d_var = self._infer_type(stmt, **settings)
+                    d_var = self._infer_type(stmt)
                     dtype = d_var.pop('datatype')
                     lhs = Variable(dtype, name , **d_var, is_temp = lhs.is_temp)
                     self.scope.insert_variable(lhs)
 
             if isinstance(expr, Assign):
                 stmt = Assign(lhs, stmt)
             elif isinstance(expr, AugAssign):
                 stmt = AugAssign(lhs, expr.op, stmt)
             stmt.set_fst(fst)
             stmts[-1] = stmt
             return CodeBlock(stmts)
 
         elif isinstance(rhs, FunctionCall):
             func = rhs.funcdef
-            if isinstance(func, FunctionDef):
-                results = func.results
-                if results:
-                    if len(results)==1:
-                        d_var = self._infer_type(results[0].var, **settings)
-                    else:
-                        d_var = self._infer_type(PythonTuple(*[r.var for r in results]), **settings)
-                elif expr.lhs.is_temp:
-                    return rhs
+            results = func.results
+            if results:
+                if len(results)==1:
+                    d_var = self._infer_type(results[0].var)
                 else:
-                    raise NotImplementedError("Cannot assign result of a function without a return")
-
-                # case of elemental function
-                # if the input and args of func do not have the same shape,
-                # then the lhs must be already declared
-                if func.is_elemental:
-                    # we first compare the funcdef args with the func call
-                    # args
-#                   d_var = None
-                    func_args = func.arguments
-                    call_args = rhs.args
-                    f_ranks = [x.var.rank for x in func_args]
-                    c_ranks = [x.value.rank for x in call_args]
-                    same_ranks = [x==y for (x,y) in zip(f_ranks, c_ranks)]
-                    if not all(same_ranks):
-                        assert(len(c_ranks) == 1)
-                        arg = call_args[0].value
-                        d_var['shape'          ] = arg.shape
-                        d_var['rank'           ] = arg.rank
-                        d_var['memory_handling'] = arg.memory_handling
-                        d_var['order'          ] = arg.order
-
-            elif isinstance(func, Interface):
-                d_var = [self._infer_type(i.var, **settings) for i in
-                         func.functions[0].results]
-
-                # TODO imporve this will not work for
-                # the case of different results types
-                d_var[0]['datatype'] = rhs.dtype
-
+                    d_var = self._infer_type(PythonTuple(*[r.var for r in results]))
+            elif expr.lhs.is_temp:
+                return rhs
             else:
-                d_var = self._infer_type(rhs, **settings)
+                raise NotImplementedError("Cannot assign result of a function without a return")
+
+            # case of elemental function
+            # if the input and args of func do not have the same shape,
+            # then the lhs must be already declared
+            if func.is_elemental:
+                # we first compare the funcdef args with the func call
+                # args
+                # d_var = None
+                func_args = func.arguments
+                call_args = rhs.args
+                f_ranks = [x.var.rank for x in func_args]
+                c_ranks = [x.value.rank for x in call_args]
+                same_ranks = [x==y for (x,y) in zip(f_ranks, c_ranks)]
+                if not all(same_ranks):
+                    assert(len(c_ranks) == 1)
+                    arg = call_args[0].value
+                    d_var['shape'          ] = arg.shape
+                    d_var['rank'           ] = arg.rank
+                    d_var['memory_handling'] = arg.memory_handling
+                    d_var['order'          ] = arg.order
 
         elif isinstance(rhs, NumpyTranspose):
-            d_var  = self._infer_type(rhs, **settings)
+            d_var  = self._infer_type(rhs)
             if d_var['memory_handling'] == 'alias' and not isinstance(lhs, IndexedElement):
                 rhs = rhs.internal_var
         elif isinstance(rhs, PyccelInternalFunction) and isinstance(rhs.dtype, NativeVoid):
             if expr.lhs.is_temp:
                 return rhs
             else:
                 raise NotImplementedError("Cannot assign result of a function without a return")
 
         else:
-            d_var  = self._infer_type(rhs, **settings)
+            d_var  = self._infer_type(rhs)
             d_list = d_var if isinstance(d_var, list) else [d_var]
 
             for d in d_list:
                 name = d['datatype'].__class__.__name__
 
                 if name.startswith('Pyccel'):
                     name = name[6:]
@@ -2576,67 +2557,67 @@
                 if len(d_var) == 1:
                     d_var = d_var[0]
                 else:
                     errors.report(WRONG_NUMBER_OUTPUT_ARGS, symbol=expr,
                         bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                         severity='error')
                     return None
-            lhs = self._assign_lhs_variable(lhs, d_var, rhs, new_expressions, isinstance(expr, AugAssign), **settings)
+            lhs = self._assign_lhs_variable(lhs, d_var, rhs, new_expressions, isinstance(expr, AugAssign))
         elif isinstance(lhs, PythonTuple):
             n = len(lhs)
             if isinstance(rhs, (PythonTuple, InhomogeneousTupleVariable, FunctionCall)):
                 if isinstance(rhs, FunctionCall):
                     r_iter = [r.var for r in rhs.funcdef.results]
                 else:
                     r_iter = rhs
                 new_lhs = []
                 for i,(l,r) in enumerate(zip(lhs,r_iter)):
-                    d = self._infer_type(r, **settings)
-                    new_lhs.append( self._assign_lhs_variable(l, d, r, new_expressions, isinstance(expr, AugAssign),arr_in_multirets=r.rank>0 ,**settings) )
+                    d = self._infer_type(r)
+                    new_lhs.append( self._assign_lhs_variable(l, d, r, new_expressions, isinstance(expr, AugAssign),arr_in_multirets=r.rank>0 ) )
                 lhs = PythonTuple(*new_lhs)
 
             elif isinstance(rhs, HomogeneousTupleVariable):
                 new_lhs = []
                 d_var = self._infer_type(rhs[0])
                 new_rhs = []
                 for i,l in enumerate(lhs):
                     new_lhs.append( self._assign_lhs_variable(l, d_var.copy(),
-                        rhs[i], new_expressions, isinstance(expr, AugAssign), **settings) )
+                        rhs[i], new_expressions, isinstance(expr, AugAssign)) )
                     new_rhs.append(rhs[i])
                 rhs = PythonTuple(*new_rhs)
                 d_var = [d_var]
                 lhs = PythonTuple(*new_lhs)
 
             elif isinstance(d_var, list) and len(d_var)== n:
                 new_lhs = []
                 if hasattr(rhs,'__getitem__'):
                     for i,l in enumerate(lhs):
-                        new_lhs.append( self._assign_lhs_variable(l, d_var[i].copy(), rhs[i], new_expressions, isinstance(expr, AugAssign), **settings) )
+                        new_lhs.append( self._assign_lhs_variable(l, d_var[i].copy(), rhs[i], new_expressions, isinstance(expr, AugAssign)) )
                 else:
                     for i,l in enumerate(lhs):
-                        new_lhs.append( self._assign_lhs_variable(l, d_var[i].copy(), rhs, new_expressions, isinstance(expr, AugAssign), **settings) )
+                        new_lhs.append( self._assign_lhs_variable(l, d_var[i].copy(), rhs, new_expressions, isinstance(expr, AugAssign)) )
                 lhs = PythonTuple(*new_lhs)
 
             elif d_var['shape'][0]==n:
                 new_lhs = []
                 new_rhs = []
 
                 for l, r in zip(lhs, rhs):
-                    new_lhs.append( self._assign_lhs_variable(l, self._infer_type(r), r, new_expressions, isinstance(expr, AugAssign), **settings) )
+                    new_lhs.append( self._assign_lhs_variable(l, self._infer_type(r), r, new_expressions, isinstance(expr, AugAssign)) )
                     new_rhs.append(r)
 
                 lhs = PythonTuple(*new_lhs)
                 rhs = new_rhs
             else:
                 errors.report(WRONG_NUMBER_OUTPUT_ARGS, symbol=expr,
                     bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                     severity='error')
                 return None
         else:
-            lhs = self._visit(lhs, **settings)
+            lhs = self._visit(lhs)
 
         if not isinstance(lhs, (list, tuple)):
             lhs = [lhs]
             if isinstance(d_var,dict):
                 d_var = [d_var]
 
         if len(lhs) == 1:
@@ -2673,52 +2654,53 @@
                     new_lhs.append(l)
                     new_rhs.append(r)
             lhs = new_lhs
             rhs = new_rhs
 
         # Examine each assign and determine assign type (Assign, AliasAssign, etc)
         for l, r in zip(lhs,rhs):
-            is_pointer_i = l.is_alias if isinstance(l, Variable) else is_pointer
-
-            new_expr = Assign(l, r)
-
             if isinstance(expr, AugAssign):
                 new_expr = AugAssign(l, expr.op, r)
-            elif is_pointer_i:
-                new_expr = AliasAssign(l, r)
+            else:
+                is_pointer_i = l.is_alias if isinstance(l, Variable) else is_pointer
+                new_expr = Assign(l, r)
 
+                if is_pointer_i:
+                    new_expr = AliasAssign(l, r)
 
-            elif new_expr.is_symbolic_alias:
-                new_expr = SymbolicAssign(l, r)
+                elif new_expr.is_symbolic_alias:
+                    new_expr = SymbolicAssign(l, r)
 
-                # in a symbolic assign, the rhs can be a lambda expression
-                # it is then treated as a def node
+                    # in a symbolic assign, the rhs can be a lambda expression
+                    # it is then treated as a def node
+
+                    F = self.scope.find(l, 'symbolic_functions')
+                    if F is None:
+                        self.insert_symbolic_function(new_expr)
+                    else:
+                        errors.report(PYCCEL_RESTRICTION_TODO,
+                                      bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
+                                      severity='fatal')
 
-                F = self.scope.find(l, 'symbolic_functions')
-                if F is None:
-                    self.insert_symbolic_function(new_expr)
-                else:
-                    errors.report(PYCCEL_RESTRICTION_TODO,
-                                  bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
-                                  severity='fatal')
             new_expressions.append(new_expr)
+
         if (len(new_expressions)==1):
             new_expressions = new_expressions[0]
 
             return new_expressions
         else:
             result = CodeBlock(new_expressions)
             return result
 
-    def _visit_For(self, expr, **settings):
+    def _visit_For(self, expr):
 
         scope = self.create_new_loop_scope()
 
         # treatment of the index/indices
-        iterable = Iterable(self._visit(expr.iterable, **settings))
+        iterable = Iterable(self._visit(expr.iterable))
 
         new_expr = []
 
         start = LiteralInteger(0)
         iterator_d_var = self._infer_type(start)
 
         iterator = expr.target
@@ -2733,58 +2715,62 @@
             else:
                 iterator = self.scope.get_expected_name(iterator)
                 syntactic_index = iterator
             index = self.check_for_variable(syntactic_index)
             if index is None:
                 index = self._assign_lhs_variable(syntactic_index, iterator_d_var,
                                 rhs=start, new_expressions=new_expr,
-                                is_augassign=False, **settings)
+                                is_augassign=False)
             iterable.set_loop_counter(index)
 
         if isinstance(iterator, PyccelSymbol):
             iterator_rhs = iterable.get_target_from_range()
             iterator_d_var = self._infer_type(iterator_rhs)
 
             target = self._assign_lhs_variable(iterator, iterator_d_var,
                             rhs=iterator_rhs, new_expressions=new_expr,
-                            is_augassign=False, **settings)
+                            is_augassign=False)
 
         elif isinstance(iterator, PythonTuple):
             iterator_rhs = iterable.get_target_from_range()
             target = [self._assign_lhs_variable(it, self._infer_type(rhs),
                                 rhs=rhs, new_expressions=new_expr,
-                                is_augassign=False, **settings)
+                                is_augassign=False)
                         for it, rhs in zip(iterator, iterator_rhs)]
         else:
 
             errors.report(INVALID_FOR_ITERABLE, symbol=expr.target,
                    bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                    severity='error')
 
-
-        body = self._visit(expr.body, **settings)
+        body = self._visit(expr.body)
 
         self.exit_loop_scope()
 
         if isinstance(iterable.iterable, Product):
             for_expr = body
             scopes = self.scope.create_product_loop_scope(scope, len(target))
 
-            for t, r, s in zip(target, iterable.get_range(), scopes[::-1]):
-                for_expr = For(t, r, for_expr, scope=s)
+            for t, i, r, s in zip(target[::-1], iterable.loop_counters[::-1], iterable.get_target_from_range()[::-1], scopes[::-1]):
+                # Create Variable iterable
+                loop_iter = Iterable(r.base)
+                loop_iter.set_loop_counter(i)
+
+                # Create a For loop for each level of the Product
+                for_expr = For(t, loop_iter, for_expr, scope=s)
                 for_expr.end_annotation = expr.end_annotation
                 for_expr = [for_expr]
             for_expr = for_expr[0]
         else:
             for_expr = For(target, iterable, body, scope=scope)
             for_expr.end_annotation = expr.end_annotation
         return for_expr
 
 
-    def _visit_FunctionalFor(self, expr, **settings):
+    def _visit_FunctionalFor(self, expr):
         old_index   = expr.index
         new_index   = self.scope.get_new_name()
         expr.substitute(old_index, new_index)
 
         target  = expr.expr
         index   = new_index
         indices = [self.scope.get_expected_name(i) for i in expr.indices]
@@ -2800,33 +2786,33 @@
         while isinstance(body, For):
 
             stop  = None
             start = LiteralInteger(0)
             step  = LiteralInteger(1)
             var   = indices[i]
             i += 1
-            a     = self._visit(body.iterable, **settings)
+            a     = self._visit(body.iterable)
             if isinstance(a, PythonRange):
                 var   = self._create_variable(var, 'int', start, {})
-                dvar  = self._infer_type(var, **settings)
+                dvar  = self._infer_type(var)
                 stop  = a.stop
                 start = a.start
                 step  = a.step
             elif isinstance(a, (PythonZip, PythonEnumerate)):
-                dvar  = self._infer_type(a.element, **settings)
+                dvar  = self._infer_type(a.element)
                 dtype = dvar.pop('datatype')
                 if dvar['rank'] > 0:
                     dvar['rank' ] -= 1
                     dvar['shape'] = (dvar['shape'])[1:]
                 if dvar['rank'] == 0:
                     dvar['memory_handling'] = 'stack'
                 var  = Variable(dtype, var, **dvar)
                 stop = a.element.shape[0]
             elif isinstance(a, Variable):
-                dvar  = self._infer_type(a, **settings)
+                dvar  = self._infer_type(a)
                 dtype = dvar.pop('datatype')
                 if dvar['rank'] == 1:
                     dvar['rank']  = 0
                     dvar['shape'] = None
                 if dvar['rank'] > 1:
                     dvar['rank'] -= 1
                     dvar['shape'] = (dvar['shape'])[1:]
@@ -2837,15 +2823,15 @@
                 stop = a.shape[0]
             else:
                 errors.report(PYCCEL_RESTRICTION_TODO,
                               bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                               severity='fatal')
             existing_var = self.scope.find(var.name, 'variables')
             if existing_var:
-                if self._infer_type(existing_var, **settings) != dvar:
+                if self._infer_type(existing_var) != dvar:
                     errors.report(f"Variable {var} already exists with different type",
                             symbol = expr, severity='error')
             else:
                 self.scope.insert_variable(var)
             step.invalidate_node()
             step  = pyccel_to_sympy(step , idx_subs, tmp_used_names)
             start.invalidate_node()
@@ -2921,16 +2907,16 @@
 
         # TODO find a faster way to calculate dim
         # when step>1 and not isinstance(dim, Sum)
         # maybe use the c++ library of sympy
 
         # we annotate the target to infere the type of the list created
 
-        target = self._visit(target, **settings)
-        d_var = self._infer_type(target, **settings)
+        target = self._visit(target)
+        d_var = self._infer_type(target)
 
         dtype = d_var['datatype']
 
         if dtype is NativeGeneric():
             errors.report(LIST_OF_TUPLES,
                           bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                           severity='fatal')
@@ -2947,64 +2933,64 @@
 
         # ...
         # TODO [YG, 30.10.2020]:
         #  - Check if we should allow the possibility that is_stack_array=True
         # ...
         lhs_symbol = expr.lhs.base
         ne = []
-        lhs = self._assign_lhs_variable(lhs_symbol, d_var, rhs=expr, new_expressions=ne, is_augassign=False, **settings)
+        lhs = self._assign_lhs_variable(lhs_symbol, d_var, rhs=expr, new_expressions=ne, is_augassign=False)
         lhs_alloc = ne[0]
 
         if isinstance(target, PythonTuple) and not target.is_homogeneous:
             errors.report(LIST_OF_TUPLES, symbol=expr,
                 bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                 severity='error')
 
         target.invalidate_node()
 
-        loops = [self._visit(i, **settings) for i in expr.loops]
-        index = self._visit(index, **settings)
+        loops = [self._visit(i) for i in expr.loops]
+        index = self._visit(index)
 
         l = loops[-1]
         for idx in indices:
             assert isinstance(l, For)
             # Sub in indices as defined here for coherent naming
             if idx.is_temp:
                 self.scope.remove_variable(l.target)
                 l.substitute(l.target, idx_subs[idx])
             l = l.body.body[-1]
 
         #self.exit_loop_scope()
 
         return CodeBlock([lhs_alloc, FunctionalFor(loops, lhs=lhs, indices=indices, index=index)])
 
-    def _visit_GeneratorComprehension(self, expr, **settings):
+    def _visit_GeneratorComprehension(self, expr):
         lhs = self.check_for_variable(expr.lhs)
         if lhs is None:
             if expr.lhs.is_temp:
                 lhs = PyccelSymbol(self.scope.get_new_name(), is_temp=True)
             else:
                 lhs = expr.lhs
 
             creation = self._visit(Assign(lhs, expr, fst=expr.fst))
             self._additional_exprs[-1].append(creation)
             return self.get_variable(lhs)
         else:
             return lhs
 
-    def _visit_While(self, expr, **settings):
+    def _visit_While(self, expr):
 
         scope = self.create_new_loop_scope()
-        test = self._visit(expr.test, **settings)
-        body = self._visit(expr.body, **settings)
+        test = self._visit(expr.test)
+        body = self._visit(expr.body)
         self.exit_loop_scope()
 
         return While(test, body, scope=scope)
 
-    def _visit_IfSection(self, expr, **settings):
+    def _visit_IfSection(self, expr):
         condition = expr.condition
 
         name_symbol = PyccelSymbol('__name__')
         main = LiteralString('__main__')
         prog_check = isinstance(condition, PyccelEq) \
                 and all(a in (name_symbol, main) for a in condition.args)
 
@@ -3019,16 +3005,16 @@
             # it will add the necessary Deallocate nodes
             # to the ast
             body.insert2body(*self._garbage_collector(body))
             self.change_to_module_scope()
 
         return IfSection(cond, body)
 
-    def _visit_If(self, expr, **settings):
-        args = [self._visit(i, **settings) for i in expr.blocks]
+    def _visit_If(self, expr):
+        args = [self._visit(i) for i in expr.blocks]
 
         conds = [b.condition for b in args]
         if any(isinstance(c, InProgram) for c in conds):
             if not all(isinstance(c, (InProgram,LiteralTrue)) for c in conds):
                 errors.report("Determination of main module is too complicated to handle",
                         symbol=expr, severity='error')
 
@@ -3047,93 +3033,93 @@
                 same_shapes = False
 
             if not same_shapes:
                 v.set_changeable_shape()
 
         return If(*args)
 
-    def _visit_IfTernaryOperator(self, expr, **settings):
-        value_true  = self._visit(expr.value_true, **settings)
+    def _visit_IfTernaryOperator(self, expr):
+        value_true  = self._visit(expr.value_true)
         if value_true.rank > 0 or value_true.dtype is NativeString():
             lhs = PyccelSymbol(self.scope.get_new_name(), is_temp=True)
             # Temporarily deactivate type checks to construct syntactic assigns
             pyccel_stage.set_stage('syntactic')
             assign_true  = Assign(lhs, expr.value_true, fst = expr.fst)
             assign_false = Assign(lhs, expr.value_false, fst = expr.fst)
             pyccel_stage.set_stage('semantic')
 
-            cond  = self._visit(expr.cond, **settings)
+            cond  = self._visit(expr.cond)
             true_section  = IfSection(cond, [self._visit(assign_true)])
             false_section = IfSection(LiteralTrue(), [self._visit(assign_false)])
             self._additional_exprs[-1].append(If(true_section, false_section))
 
             return self._visit(lhs)
         else:
-            cond        = self._visit(expr.cond, **settings)
-            value_false = self._visit(expr.value_false, **settings)
+            cond        = self._visit(expr.cond)
+            value_false = self._visit(expr.value_false)
             return IfTernaryOperator(cond, value_true, value_false)
 
-    def _visit_VariableHeader(self, expr, **settings):
+    def _visit_VariableHeader(self, expr):
 
         # TODO improve
         #      move it to the ast like create_definition for FunctionHeader?
 
         name  = expr.name
         d_var = expr.dtypes.copy()
         dtype = d_var.pop('datatype')
         d_var.pop('is_func')
 
         var = Variable(dtype, name, **d_var)
         self.scope.insert_variable(var)
         return expr
 
-    def _visit_FunctionHeader(self, expr, **settings):
+    def _visit_FunctionHeader(self, expr):
         # TODO should we return it and keep it in the AST?
         expr.clear_user_nodes()
         self.scope.insert_header(expr)
         return expr
 
-    def _visit_Template(self, expr, **settings):
+    def _visit_Template(self, expr):
         expr.clear_user_nodes()
         self.scope.insert_template(expr)
         return expr
 
-    def _visit_ClassHeader(self, expr, **settings):
+    def _visit_ClassHeader(self, expr):
         # TODO should we return it and keep it in the AST?
         expr.clear_user_nodes()
         self.scope.insert_header(expr)
         return expr
 
-    def _visit_Return(self, expr, **settings):
+    def _visit_Return(self, expr):
 
         results     = expr.expr
         f_name      = self._current_function
         if isinstance(f_name, DottedName):
             f_name = f_name.name[-1]
 
         return_objs = self.scope.find(f_name, 'functions').results
         assigns     = []
         for o,r in zip(return_objs, results):
             v = o.var
             if not (isinstance(r, PyccelSymbol) and r == (v.name if isinstance(v, Variable) else v)):
                 a = self._visit(Assign(v, r, fst=expr.fst))
                 assigns.append(a)
 
-        results = [self._visit(i.var, **settings) for i in return_objs]
+        results = [self._visit(i.var) for i in return_objs]
 
         # add the Deallocate node before the Return node and eliminating the Deallocate nodes
         # the arrays that will be returned.
         code = assigns + [Deallocate(i) for i in self._allocs[-1] if i not in results]
         if code:
             expr  = Return(results, CodeBlock(code))
         else:
             expr  = Return(results)
         return expr
 
-    def _visit_FunctionDef(self, expr, **settings):
+    def _visit_FunctionDef(self, expr):
         name            = self.scope.get_expected_name(expr.name)
         cls_name        = expr.cls_name
         decorators      = expr.decorators
         funcs           = []
         sub_funcs       = []
         func_interfaces = []
         is_pure         = expr.is_pure
@@ -3257,15 +3243,15 @@
                         if a.has_default:
                             # optional argument only if the value is None
                             if isinstance(a.value, Nil):
                                 d_var['is_optional'] = True
                         a_new = FunctionAddress(self.scope.get_expected_name(a.name),
                                         ahv.arguments, ahv.results, [], **d_var)
                     else:
-                        d_var = self._infer_type(ahv, **settings)
+                        d_var = self._infer_type(ahv)
                         d_var['shape'] = ahv.alloc_shape
                         d_var['is_argument'] = True
                         d_var['is_const'] = ahv.is_const
                         dtype = d_var.pop('datatype')
                         if not d_var['cls_base']:
                             d_var['cls_base'] = get_cls_base( dtype, d_var['precision'], d_var['rank'] )
 
@@ -3298,15 +3284,15 @@
                         self.scope.insert_variable(a_new, a.name)
             results = expr.results
             if header_results:
                 new_results = []
 
                 for a, ah in zip(results, header_results):
                     av = a.var
-                    d_var = self._infer_type(ah.var, **settings)
+                    d_var = self._infer_type(ah.var)
                     dtype = d_var.pop('datatype')
                     a_new = Variable(dtype, self.scope.get_expected_name(av),
                             **d_var, is_temp = av.is_temp)
                     self.scope.insert_variable(a_new, av)
                     new_results.append(FunctionDefResult(a_new, annotation = ah.annotation))
 
                 results = new_results
@@ -3446,28 +3432,34 @@
             for f in funcs:
                 self.insert_function(f)
 
             funcs = Interface(interface_name, funcs)
             self.insert_function(funcs)
 #        TODO move this to codegen
 #        if vec_func:
-#           self._visit_FunctionDef(vec_func, **settings)
+#           self._visit_FunctionDef(vec_func)
 #           vec_func = self.scope.functions.pop(vec_name)
 #           if isinstance(funcs, Interface):
 #               funcs = list(funcs.funcs)+[vec_func]
 #           else:
 #               self.scope.sons_scopes['sc_'+ name] = self.scope.sons_scopes[name]
 #               funcs = funcs.rename('sc_'+ name)
 #               funcs = [funcs, vec_func]
 #           funcs = Interface(name, funcs)
 #           self.insert_function(funcs)
         return EmptyNode()
 
-    def _visit_PythonPrint(self, expr, **settings):
-        args = [self._visit(i, **settings) for i in expr.expr]
+    def _visit_PythonPrint(self, expr):
+        args = [self._visit(i) for i in expr.expr]
+        for i, arg in enumerate(args):
+            rhs = arg.value
+            if getattr(rhs, 'rank', 0) and isinstance(rhs, PyccelInternalFunction):
+                tmp_var = self._assign_lhs_variable(self.scope.get_new_name(), self._infer_type(rhs) , rhs, self._additional_exprs[-1] , is_augassign=False)
+                self._additional_exprs[-1].append(Assign(tmp_var, rhs, fst=rhs.fst))
+                args[i] = FunctionCallArgument(tmp_var)
         if len(args) == 0:
             return PythonPrint(args)
 
         def is_symbolic(var):
             return isinstance(var, Variable) \
                 and isinstance(var.dtype, NativeSymbol)
 
@@ -3489,15 +3481,15 @@
                     # TODO improve: how can we print SymbolicAssign as  lhs = rhs
 
                     _args.append(f)
             return SymbolicPrint(_args)
         else:
             return PythonPrint(args)
 
-    def _visit_ClassDef(self, expr, **settings):
+    def _visit_ClassDef(self, expr):
 
         # TODO - improve the use and def of interfaces
         #      - wouldn't be better if it is done inside ClassDef?
 
         name = expr.name
         name = name.replace("'", '')
         scope = self.create_new_class_scope(name, used_symbols=expr.scope.local_used_symbols,
@@ -3511,29 +3503,29 @@
         self.scope.insert_class(cls)
         const = None
 
         for (i, method) in enumerate(methods):
             m_name = method.name.replace("'", '')
 
             if m_name == '__init__':
-                self._visit_FunctionDef(method, **settings)
+                self._visit_FunctionDef(method)
                 methods.pop(i)
                 const = self.scope.functions.pop(m_name)
                 break
 
 
 
         if not const:
             errors.report(UNDEFINED_INIT_METHOD, symbol=name,
                    bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                    severity='error')
 
         ms = []
         for i in methods:
-            self._visit_FunctionDef(i, **settings)
+            self._visit_FunctionDef(i)
             m_name = i.name.replace("'", '')
             m = self.scope.functions.pop(m_name)
             ms.append(m)
 
         methods = [const] + ms
         header = self.get_headers(name)
 
@@ -3553,20 +3545,20 @@
 
         cls = ClassDef(name, attributes, methods,
               interfaces=interfaces, superclass=parent, scope=scope)
         self.scope.insert_class(cls)
 
         return EmptyNode()
 
-    def _visit_Del(self, expr, **settings):
+    def _visit_Del(self, expr):
 
-        ls = [self._visit(i, **settings) for i in expr.variables]
+        ls = [self._visit(i) for i in expr.variables]
         return Del(ls)
 
-    def _visit_PyccelIs(self, expr, **settings):
+    def _visit_PyccelIs(self, expr):
         # Handles PyccelIs and PyccelIsNot
         IsClass = type(expr)
 
         # TODO ERROR wrong position ??
 
         var1 = self._visit(expr.lhs)
         var2 = self._visit(expr.rhs)
@@ -3610,15 +3602,15 @@
             return IsClass(var1, var2)
 
         errors.report(PYCCEL_RESTRICTION_IS_ISNOT,
             bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
             severity='error')
         return IsClass(var1, var2)
 
-    def _visit_Import(self, expr, **settings):
+    def _visit_Import(self, expr):
 
         # TODO - must have a dict where to store things that have been
         #        imported
         #      - should not use scope
 
         container = self.scope.imports
 
@@ -3756,32 +3748,32 @@
                 expr = Import(source, targets, mod=mod)
                 container['imports'][source_target] = expr
 
         return result
 
 
 
-    def _visit_With(self, expr, **settings):
+    def _visit_With(self, expr):
         scope = self.create_new_loop_scope()
 
-        domaine = self._visit(expr.test, **settings)
+        domaine = self._visit(expr.test)
         parent  = domaine.cls_base
         if not parent.is_with_construct:
             errors.report(UNDEFINED_WITH_ACCESS,
                    bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                    severity='fatal')
 
-        body = self._visit(expr.body, **settings)
+        body = self._visit(expr.body)
 
         self.exit_loop_scope()
         return With(domaine, body, scope).block
 
 
 
-    def _visit_MacroFunction(self, expr, **settings):
+    def _visit_MacroFunction(self, expr):
         # we change here the master name to its FunctionDef
 
         f_name = expr.master
         header = self.get_headers(f_name)
         if not header:
             func = self.scope.find(f_name, 'functions')
             if func is None:
@@ -3811,19 +3803,19 @@
         master = FunctionCall(func, master_args)
         macro   = MacroFunction(name, args, master, master_args,
                                 results=expr.results, results_shapes=expr.results_shapes)
         self.scope.insert_macro(macro)
 
         return macro
 
-    def _visit_MacroShape(self, expr, **settings):
+    def _visit_MacroShape(self, expr):
         expr.clear_user_nodes()
         return expr
 
-    def _visit_MacroVariable(self, expr, **settings):
+    def _visit_MacroVariable(self, expr):
 
         master = expr.master
         if isinstance(master, DottedName):
             errors.report(PYCCEL_RESTRICTION_TODO,
                           bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                           severity='fatal')
         header = self.get_headers(master)
@@ -3834,51 +3826,51 @@
 
                 # TODO -> Said: must handle interface
 
         expr = MacroVariable(expr.name, var)
         self.scope.insert_macro(expr)
         return expr
 
-    def _visit_StarredArguments(self, expr, **settings):
+    def _visit_StarredArguments(self, expr):
         var = self._visit(expr.args_var)
         assert(var.rank==1)
         size = var.shape[0]
         return StarredArguments([var[i] for i in range(size)])
 
-    def _visit_NumpyMatmul(self, expr, **settings):
+    def _visit_NumpyMatmul(self, expr):
         if isinstance(expr, FunctionCall):
             a = self._visit(expr.args[0].value)
             b = self._visit(expr.args[1].value)
         else:
             self.insert_import('numpy', AsName(NumpyMatmul, 'matmul'))
             a = self._visit(expr.a)
             b = self._visit(expr.b)
         return NumpyMatmul(a, b)
 
-    def _visit_Assert(self, expr, **settings):
-        test = self._visit(expr.test, **settings)
+    def _visit_Assert(self, expr):
+        test = self._visit(expr.test)
         return Assert(test)
 
-    def _visit_NumpyWhere(self, func_call, **settings):
-        func_call_args = self._handle_function_args(func_call.args, **settings)
+    def _visit_NumpyWhere(self, func_call):
+        func_call_args = self._handle_function_args(func_call.args)
         # expr is a FunctionCall
         args = [a.value for a in func_call_args if not a.has_keyword]
         kwargs = {a.keyword: a.value for a in func_call.args if a.has_keyword}
         nargs = len(args)+len(kwargs)
         if nargs == 1:
             return self._visit_NumpyNonZero(func_call)
         return NumpyWhere(*args, **kwargs)
 
-    def _visit_NumpyNonZero(self, func_call, **settings):
-        func_call_args = self._handle_function_args(func_call.args, **settings)
+    def _visit_NumpyNonZero(self, func_call):
+        func_call_args = self._handle_function_args(func_call.args)
         # expr is a FunctionCall
         arg = func_call_args[0].value
         if not isinstance(arg, Variable):
             new_symbol = PyccelSymbol(self.scope.get_new_name())
             creation = self._visit(Assign(new_symbol, arg, fst=func_call.fst))
             self._additional_exprs[-1].append(creation)
             arg = self._visit(new_symbol)
         return NumpyWhere(arg)
 
-    def _visit_FunctionDefResult(self, expr, **settings):
+    def _visit_FunctionDefResult(self, expr):
         var = self._visit(expr.var)
         return FunctionDefResult(var, annotation = expr.annotation)
```

### Comparing `pyccel-1.7.4/pyccel/parser/syntactic.py` & `pyccel-1.8.0/pyccel/parser/syntactic.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,19 +141,29 @@
 
         self.load()
 
         tree                = extend_tree(code)
         self._fst           = tree
         self._in_lhs_assign = False
 
-        self.parse(verbose=True)
+        self.parse()
         self.dump()
 
-    def parse(self, verbose=False):
-        """converts python ast to sympy ast."""
+    def parse(self):
+        """
+        Convert Python's AST to Pyccel's AST object.
+
+        Convert Python's AST to Pyccel's AST object and raise errors
+        for any unsupported objects.
+
+        Returns
+        -------
+        pyccel.ast.basic.Basic
+            The Pyccel AST object.
+        """
 
         if self.syntax_done:
             return self.ast
 
         # TODO - add settings to Errors
         #      - filename
         errors.set_parser_stage('syntax')
@@ -827,15 +837,20 @@
 
         return func
 
     def _visit_ClassDef(self, stmt):
 
         name = stmt.name
         scope = self.create_new_class_scope(name)
-        methods = [self._visit(i) for i in stmt.body if isinstance(i, ast.FunctionDef)]
+        methods = []
+        for i in stmt.body:
+            if isinstance(i, ast.FunctionDef):
+                methods.append(self._visit(i))
+            elif isinstance(i, ast.Pass):
+                return errors.report(UNSUPPORTED_FEATURE_OOP_EMPTY_CLASS, symbol = stmt, severity='error')
         for i in methods:
             i.cls_name = name
         attributes = [a.var for a in methods[0].arguments]
         parent = [self._visit(i) for i in stmt.bases]
         self.exit_class_scope()
         expr = ClassDef(name=name, attributes=attributes,
                         methods=methods, superclass=parent, scope=scope)
```

### Comparing `pyccel-1.7.4/pyccel/parser/syntax/basic.py` & `pyccel-1.8.0/pyccel/parser/syntax/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/parser/syntax/headers.py` & `pyccel-1.8.0/pyccel/parser/syntax/headers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/parser/syntax/openacc.py` & `pyccel-1.8.0/pyccel/parser/syntax/openacc.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/parser/syntax/openmp.py` & `pyccel-1.8.0/pyccel/parser/syntax/openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/parser/utilities.py` & `pyccel-1.8.0/pyccel/parser/utilities.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/cwrapper/cwrapper.c` & `pyccel-1.8.0/pyccel/stdlib/cwrapper/cwrapper.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/cwrapper/cwrapper.h` & `pyccel-1.8.0/pyccel/stdlib/cwrapper/cwrapper.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c` & `pyccel-1.8.0/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c`

 * *Files 6% similar despite different names*

```diff
@@ -459,21 +459,65 @@
 /*
  * Function: nd_data
  * --------------------
  * Return data pointed by array
  *
  * 	Parameters	:
  *		a 	  : python array object
- *      index : dimension index
  * 	Returns		:
  *		return NULL if object is NULL or the data of the array
  * reference of the used c/numpy api function
  * -------------------------------------------
  * https://numpy.org/doc/1.17/reference/c-api.array.html#c.PyArray_DIM
  */
 void    *nd_data(t_ndarray *a)
 {
 	if (a == NULL)
 		return NULL;
 
 	return a->raw_data;
 }
+
+/*
+ * Function: nd_step_C
+ * --------------------
+ * Return the step in the nth dimension for a C-ordered array (decreasing strides)
+ *
+ * 	Parameters	:
+ *		a 	  : python array object
+ * 		index	  : dimension index
+ * 	Returns		:
+ *		return 1 if object is NULL or the step along the indexed dimension
+ */
+int     nd_nstep_C(t_ndarray *a, int n)
+{
+	if (a == NULL || a->length == 0)
+		return 1;
+
+	int step = a->strides[n];
+	for (int i = n+1; i<a->nd; ++i) {
+		step /= a->shape[i];
+	}
+	return step > 0 ? step : 1;
+}
+/*
+ * Function: nd_step_F
+ * --------------------
+ * Return the step in the nth dimension for a F-ordered array (increasing strides)
+ *
+ * 	Parameters	:
+ *		a 	  : python array object
+ * 		index	  : dimension index
+ * 	Returns		:
+ *		return 1 if object is NULL or the step along the indexed dimension
+ */
+int     nd_nstep_F(t_ndarray *a, int n)
+{
+	if (a == NULL || a->length == 0)
+		return 1;
+
+	int step = a->strides[n];
+	for (int i = 0; i<n; ++i) {
+		step /= a->shape[i];
+	}
+	return step > 0 ? step : 1;
+}
```

### Comparing `pyccel-1.7.4/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h` & `pyccel-1.8.0/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h`

 * *Files 6% similar despite different names*

```diff
@@ -45,9 +45,11 @@
 
 /* arrays checkers and helpers */
 bool	pyarray_check(PyObject *o, int dtype, int rank, int flag);
 bool	is_numpy_array(PyObject *o, int dtype, int rank, int flag);
 
 void    *nd_data(t_ndarray *a);
 int     nd_ndim(t_ndarray *a, int n);
+int     nd_nstep_C(t_ndarray *a, int n);
+int     nd_nstep_F(t_ndarray *a, int n);
 
 #endif
```

### Comparing `pyccel-1.7.4/pyccel/stdlib/external/dfftpack.py` & `pyccel-1.8.0/pyccel/stdlib/external/dfftpack.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/external/fitpack.py` & `pyccel-1.8.0/pyccel/stdlib/external/fitpack.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/external/lapack.py` & `pyccel-1.8.0/pyccel/stdlib/external/lapack.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/external/mpi4py.py` & `pyccel-1.8.0/pyccel/stdlib/external/mpi4py.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/blas.pyccel` & `pyccel-1.8.0/pyccel/stdlib/internal/blas.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 9585 8900 0000 0000 008c 2034 3262  ............ 42b
 00000010: 6161 3166 6235 3832 3336 3335 3866 3565  aa1fb58236358f5e
 00000020: 6636 6435 6530 3434 3362 3533 3894 8c05  f6d5e0443b538...
-00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
+00000030: 312e 382e 3094 8c17 7079 6363 656c 2e70  1.8.0...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 911e 0000 2320 7079 6363 656c 2068 6561  ....# pyccel hea
 00000080: 6465 7220 666f 7220 424c 4153 2e0a 0a23  der for BLAS...#
 00000090: 2420 6865 6164 6572 206d 6574 6176 6172  $ header metavar
 000000a0: 206d 6f64 756c 655f 7665 7273 696f 6e3d   module_version=
```

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/blas.pyh` & `pyccel-1.8.0/pyccel/stdlib/internal/blas.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/dfftpack.pyccel` & `pyccel-1.8.0/pyccel/stdlib/internal/dfftpack.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 9529 1700 0000 0000 008c 2031 3362  ...)........ 13b
 00000010: 6133 3830 6537 3438 3037 6630 3830 3266  a380e74807f0802f
 00000020: 6366 3030 3564 6138 3432 6366 3894 8c05  cf005da842cf8...
-00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
+00000030: 312e 382e 3094 8c17 7079 6363 656c 2e70  1.8.0...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 7804 0000 2320 7079 6363 656c 2068 6561  x...# pyccel hea
 00000080: 6465 7220 666f 7220 4446 5454 5041 434b  der for DFTTPACK
 00000090: 2e0a 0a23 2420 6865 6164 6572 206d 6574  ...#$ header met
 000000a0: 6176 6172 2069 676e 6f72 655f 6174 5f69  avar ignore_at_i
```

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/dfftpack.pyh` & `pyccel-1.8.0/pyccel/stdlib/internal/dfftpack.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/fftw.pyh` & `pyccel-1.8.0/pyccel/stdlib/internal/fftw.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/fitpack.pyccel` & `pyccel-1.8.0/pyccel/stdlib/internal/fitpack.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 9528 0b00 0000 0000 008c 2062 6362  ...(........ bcb
 00000010: 3932 6461 3730 6233 3364 3836 3939 3234  92da70b33d869924
 00000020: 6537 3333 3034 3531 3564 3365 3494 8c05  e73304515d3e4...
-00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
+00000030: 312e 382e 3094 8c17 7079 6363 656c 2e70  1.8.0...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 5701 0000 2320 7079 6363 656c 2068 6561  W...# pyccel hea
 00000080: 6465 7220 666f 7220 4649 5450 4143 4b2e  der for FITPACK.
 00000090: 0a0a 0a23 2420 6865 6164 6572 206d 6574  ...#$ header met
 000000a0: 6176 6172 2069 676e 6f72 655f 6174 5f69  avar ignore_at_i
```

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/hdf5.pyh` & `pyccel-1.8.0/pyccel/stdlib/internal/hdf5.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/lapack.pyccel` & `pyccel-1.8.0/pyccel/stdlib/internal/lapack.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 9599 0001 0000 0000 008c 2066 3964  ............ f9d
 00000010: 6365 6637 3662 6261 6633 6165 6261 6366  cef76bbaf3aebacf
 00000020: 3532 3330 3865 3364 3637 3736 3194 8c05  52308e3d67761...
-00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
+00000030: 312e 382e 3094 8c17 7079 6363 656c 2e70  1.8.0...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 25e3 0000 2320 7079 6363 656c 2068 6561  %...# pyccel hea
 00000080: 6465 7220 666f 7220 4c41 5041 434b 2e0a  der for LAPACK..
 00000090: 0a23 2420 6865 6164 6572 206d 6574 6176  .#$ header metav
 000000a0: 6172 206d 6f64 756c 655f 7665 7273 696f  ar module_versio
```

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/lapack.pyh` & `pyccel-1.8.0/pyccel/stdlib/internal/lapack.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/mpi.pyccel` & `pyccel-1.8.0/pyccel/stdlib/internal/mpi.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 9597 6200 0000 0000 008c 2061 3734  ....b....... a74
 00000010: 6338 3636 3630 3230 6665 3735 6335 3935  c8666020fe75c595
 00000020: 3335 3238 6638 3532 3065 3939 3894 8c05  3528f8520e998...
-00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
+00000030: 312e 382e 3094 8c17 7079 6363 656c 2e70  1.8.0...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 1717 0000 2320 7079 6363 656c 2068 6561  ....# pyccel hea
 00000080: 6465 7220 666f 7220 4d50 492e 0a23 0a0a  der for MPI..#..
 00000090: 2320 4f6e 2074 7261 7669 732c 2027 7573  # On travis, 'us
 000000a0: 6520 6d70 692c 206f 6e6c 793a 206d 7069  e mpi, only: mpi
```

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/mpi.pyh` & `pyccel-1.8.0/pyccel/stdlib/internal/mpi.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/mpiext.py` & `pyccel-1.8.0/pyccel/stdlib/internal/mpiext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/openacc.pyccel` & `pyccel-1.8.0/pyccel/stdlib/internal/openacc.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 95fe 2a00 0000 0000 008c 2039 3265  ....*....... 92e
 00000010: 3531 6230 3535 3231 6330 3337 3164 3037  51b05521c0371d07
 00000020: 3034 6535 3738 3737 3135 3361 6294 8c05  04e57877153ab...
-00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
+00000030: 312e 382e 3094 8c17 7079 6363 656c 2e70  1.8.0...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 730a 0000 2320 7079 6363 656c 2068 6561  s...# pyccel hea
 00000080: 6465 7220 666f 7220 4f70 656e 4143 432e  der for OpenACC.
 00000090: 0a23 204f 7065 6e41 4343 2064 6972 6563  .# OpenACC direc
 000000a0: 7469 7665 7320 616e 6420 436f 6e73 7472  tives and Constr
```

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/openacc.pyh` & `pyccel-1.8.0/pyccel/stdlib/internal/openacc.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/openmp.py` & `pyccel-1.8.0/pyccel/stdlib/internal/openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/openmp.pyccel` & `pyccel-1.8.0/pyccel/stdlib/internal/openmp.pyccel`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 8004 953a 2700 0000 0000 008c 2062 6331  ...:'....... bc1
 00000010: 3734 3231 3738 6137 6338 3035 6261 3062  742178a7c805ba0b
 00000020: 3630 3738 3263 6466 3138 3933 3194 8c05  60782cdf18931...
-00000030: 312e 372e 3494 8c17 7079 6363 656c 2e70  1.7.4...pyccel.p
+00000030: 312e 382e 3094 8c17 7079 6363 656c 2e70  1.8.0...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 550a 0000 2320 7079 6363 656c 2068 6561  U...# pyccel hea
 00000080: 6465 7220 666f 7220 4f70 656e 4d50 2e0a  der for OpenMP..
 00000090: 2320 4f70 656e 4d50 2064 6972 6563 7469  # OpenMP directi
 000000a0: 7665 7320 616e 6420 436f 6e73 7472 7563  ves and Construc
```

### Comparing `pyccel-1.7.4/pyccel/stdlib/internal/openmp.pyh` & `pyccel-1.8.0/pyccel/stdlib/internal/openmp.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/math/pyc_math_c.c` & `pyccel-1.8.0/pyccel/stdlib/math/pyc_math_c.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/math/pyc_math_c.h` & `pyccel-1.8.0/pyccel/stdlib/math/pyc_math_c.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/math/pyc_math_f90.f90` & `pyccel-1.8.0/pyccel/stdlib/math/pyc_math_f90.f90`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/ndarrays/ndarrays.c` & `pyccel-1.8.0/pyccel/stdlib/ndarrays/ndarrays.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/ndarrays/ndarrays.h` & `pyccel-1.8.0/pyccel/stdlib/ndarrays/ndarrays.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/numpy/numpy_c.c` & `pyccel-1.8.0/pyccel/stdlib/numpy/numpy_c.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/numpy/numpy_c.h` & `pyccel-1.8.0/pyccel/stdlib/numpy/numpy_c.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/numpy/numpy_f90.f90` & `pyccel-1.8.0/pyccel/stdlib/numpy/numpy_f90.f90`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/stdlib/parallel/mpi.py` & `pyccel-1.8.0/pyccel/stdlib/parallel/mpi.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/symbolic/lambdify.py` & `pyccel-1.8.0/pyccel/symbolic/lambdify.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/utilities/metaclasses.py` & `pyccel-1.8.0/pyccel/utilities/metaclasses.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,20 +8,25 @@
 
 __all__ = (
     'Singleton',
     'ArgumentSingleton',
 )
 
 class Singleton(type):
-    """ Indicates that there is only one instance of the class
+    """
+    Metaclass indicating that there is only one instance of the class.
+
+    A metaclass which ensures that only one instance of the class is ever
+    created. Trying to create a second instance will result in accessing
+    the first.
     """
     _instances = {}
-    def __call__(cls, *args, **kwargs):
+    def __call__(cls):
         if cls not in cls._instances:
-            cls._instances[cls] = super().__call__(*args, **kwargs)
+            cls._instances[cls] = super().__call__()
         return cls._instances[cls]
 
 class ArgumentSingleton(type):
     """ Indicates that there is only one instance of the class
     for any given set of arguments
     """
     _instances = {}
```

### Comparing `pyccel-1.7.4/pyccel/utilities/stage.py` & `pyccel-1.8.0/pyccel/utilities/stage.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/pyccel/utilities/strings.py` & `pyccel-1.8.0/pyccel/utilities/strings.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,46 +2,56 @@
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 """ Module containing helper functions for managing strings
 """
 
-def create_incremented_string(forbidden_exprs, prefix = 'Dummy', counter = 1):
-    """This function takes a prefix and a counter and uses them to construct
+def create_incremented_string(forbidden_exprs, prefix = 'Dummy', counter = 1, name_clash_checker = None):
+    """
+    Create a new unique string by incrementing a prefix.
+
+    This function takes a prefix and a counter and uses them to construct
     a new name of the form:
             prefix_counter
     Where counter is formatted to fill 4 characters
     The new name is checked against a list of forbidden expressions. If the
     constructed name is forbidden then the counter is incremented until a valid
-    name is found
-
-      Parameters
-      ----------
-      forbidden_exprs : Set
-                        A set of all the values which are not valid solutions to this problem
-      prefix          : str
-                        The prefix used to begin the string
-      counter         : int
-                        The expected value of the next name
-
-      Returns
-      ----------
-      name            : str
-                        The incremented string name
-      counter         : int
-                        The expected value of the next name
+    name is found.
 
+    Parameters
+    ----------
+    forbidden_exprs : set
+        A set of all the values which are not valid solutions to this problem.
+    prefix : str
+        The prefix used to begin the string.
+    counter : int
+        The expected value of the next name.
+    name_clash_checker : pyccel.naming.languagenameclashchecker.LanguageNameClashChecker
+        A class instance providing access to a `has_clash` function which determines
+        if names clash in a given language.
+
+    Returns
+    -------
+    name : str
+        The incremented string name.
+    counter : int
+        The expected value of the next name.
     """
     nDigits = 4
 
     if prefix is None:
         prefix = 'Dummy'
 
     name_format = "{prefix}_{counter:0="+str(nDigits)+"d}"
     name = name_format.format(prefix=prefix, counter = counter)
     counter += 1
-    while name in forbidden_exprs:
-        name = name_format.format(prefix=prefix, counter = counter)
-        counter += 1
+    if name_clash_checker:
+        while name_clash_checker.has_clash(name, forbidden_exprs):
+            name = name_format.format(prefix=prefix, counter = counter)
+            counter += 1
+    else:
+        while name in forbidden_exprs:
+            name = name_format.format(prefix=prefix, counter = counter)
+            counter += 1
 
     return name, counter
```

### Comparing `pyccel-1.7.4/pyccel.egg-info/PKG-INFO` & `pyccel-1.8.0/pyccel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyccel
-Version: 1.7.4
+Version: 1.8.0
 Summary: UNKNOWN
 Home-page: https://github.com/pyccel/pyccel
 Author: Pyccel development team
 License: LICENSE
 Keywords: math
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pyccel-1.7.4/pyccel.egg-info/SOURCES.txt` & `pyccel-1.8.0/pyccel.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,17 @@
 pyccel/codegen/printing/__init__.py
 pyccel/codegen/printing/ccode.py
 pyccel/codegen/printing/codeprinter.py
 pyccel/codegen/printing/cwrappercode.py
 pyccel/codegen/printing/fcode.py
 pyccel/codegen/printing/luacode.py
 pyccel/codegen/printing/pycode.py
+pyccel/codegen/wrapper/__init__.py
+pyccel/codegen/wrapper/fortran_to_c_wrapper.py
+pyccel/codegen/wrapper/wrapper.py
 pyccel/commands/__init__.py
 pyccel/commands/console.py
 pyccel/commands/pyccel_clean.py
 pyccel/commands/pyccel_init.py
 pyccel/compilers/__init__.py
 pyccel/compilers/default_compilers.py
 pyccel/complexity/__init__.py
@@ -70,14 +73,15 @@
 pyccel/complexity/memory.py
 pyccel/errors/__init__.py
 pyccel/errors/errors.py
 pyccel/errors/messages.py
 pyccel/naming/__init__.py
 pyccel/naming/cnameclashchecker.py
 pyccel/naming/fortrannameclashchecker.py
+pyccel/naming/languagenameclashchecker.py
 pyccel/naming/pythonnameclashchecker.py
 pyccel/parser/__init__.py
 pyccel/parser/base.py
 pyccel/parser/extend_tree.py
 pyccel/parser/parser.py
 pyccel/parser/scope.py
 pyccel/parser/semantic.py
@@ -87,15 +91,14 @@
 pyccel/parser/grammar/himi.tx
 pyccel/parser/grammar/openacc.tx
 pyccel/parser/grammar/openmp.tx
 pyccel/parser/grammar/pyccel.tx
 pyccel/parser/syntax/__init__.py
 pyccel/parser/syntax/basic.py
 pyccel/parser/syntax/headers.py
-pyccel/parser/syntax/himi.py
 pyccel/parser/syntax/openacc.py
 pyccel/parser/syntax/openmp.py
 pyccel/stdlib/__init__.py
 pyccel/stdlib/cwrapper/cwrapper.c
 pyccel/stdlib/cwrapper/cwrapper.h
 pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c
 pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h
@@ -348,14 +351,15 @@
 tests/errors/semantic/non_blocking/is.py
 tests/errors/semantic/non_blocking/var_is_none.py
 tests/errors/syntax_blockers/ex1.py
 tests/errors/syntax_blockers/imports.py
 tests/errors/syntax_errors/TEMPLATE_WRONG_KEY.py
 tests/errors/syntax_errors/TEMPLATE_WRONG_NUMBER_ARGS.py
 tests/errors/syntax_errors/dict_str_keys.py
+tests/errors/syntax_errors/empty_class.py
 tests/errors/syntax_errors/functions_in_template.py
 tests/errors/syntax_errors/functions_in_uniontype.py
 tests/errors/syntax_errors/import_star.py
 tests/errors/syntax_errors/list_comprehension_no_assign.py
 tests/errors/syntax_errors/nargs.py
 tests/errors/syntax_errors/not_implemented.py
 tests/errors/syntax_errors/raise.py
@@ -443,15 +447,14 @@
 tests/macro/scripts/blas/bugs/dnrm2.py
 tests/macro/scripts/lapack/runtest_dgbtrf.py
 tests/ndarrays/conftest.py
 tests/ndarrays/leaks_check.py
 tests/ndarrays/test_ndarrays.c
 tests/parser/test_comments.py
 tests/parser/test_headers.py
-tests/parser/test_himi.py
 tests/parser/test_openacc.py
 tests/parser/test_openmp.py
 tests/parser/scripts/comments.py
 tests/preprocess/test_preprocess.py
 tests/preprocess/scripts/omp.py
 tests/pyccel/run_import_function.py
 tests/pyccel/test_pyccel.py
```

### Comparing `pyccel-1.7.4/samples/mxm_openmp.py` & `pyccel-1.8.0/samples/mxm_openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/setup.cfg` & `pyccel-1.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/setup.py` & `pyccel-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/ast/test_basic.py` & `pyccel-1.8.0/tests/ast/test_basic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,177 +1,194 @@
 # pylint: disable=missing-function-docstring, missing-module-docstring
 import os
 
 from pyccel.parser.parser   import Parser
 from pyccel.errors.errors   import Errors
 
 from pyccel.ast.basic       import Basic
-from pyccel.ast.core        import Assign, Return, FunctionDef
+from pyccel.ast.core        import Assign, Return, FunctionDef, AugAssign, FunctionDefArgument
 from pyccel.ast.literals    import LiteralInteger
-from pyccel.ast.operators   import PyccelOperator, PyccelAdd, PyccelMinus
+from pyccel.ast.operators   import PyccelOperator, PyccelAdd, PyccelMinus, PyccelMul
 from pyccel.ast.variable    import Variable
 
 base_dir = os.path.dirname(os.path.realpath(__file__))
 path_dir = os.path.join(base_dir, 'scripts')
 
 def get_functions(filename):
     pyccel = Parser(filename)
     errors = Errors()
 
     ast = pyccel.parse()
 
     # Assert syntactic success
-    assert(not errors.has_errors())
+    assert not errors.has_errors()
 
     settings = {}
     ast = pyccel.annotate(**settings)
 
     # Assert semantic success
-    assert(not errors.has_errors())
+    assert not errors.has_errors()
 
     return list(ast.scope.functions.values())
 
 def test_get_attribute_nodes():
     filename = os.path.join(path_dir, "math.py")
 
     fst = get_functions(filename)[0]
     atts = fst.get_attribute_nodes(Variable)
 
-    assert(all(isinstance(a, Variable) for a in atts))
+    assert all(isinstance(a, Variable) for a in atts)
 
     expected = [Variable('int', 'a'),
                 Variable('int', 'b'),
                 Variable('int', 'c'),
                 Variable('int', 'd'),
                 Variable('int', 'e'),
                 Variable('int', 'g')]
 
     for e in expected:
-        assert(e in atts)
+        assert e in atts
 
 def test_get_attribute_nodes_exclude():
     filename = os.path.join(path_dir, "math.py")
 
     fst = get_functions(filename)[0]
     atts = fst.get_attribute_nodes(PyccelOperator, excluded_nodes=(PyccelAdd,))
 
-    assert(all(isinstance(a, PyccelOperator) for a in atts))
-    assert(all(not isinstance(a, PyccelAdd) for a in atts))
-    assert(len(atts)==1)
+    assert all(isinstance(a, PyccelOperator) for a in atts)
+    assert all(not isinstance(a, PyccelAdd) for a in atts)
+    assert len(atts)==1
     minus = atts[0]
-    assert(isinstance(minus, PyccelMinus)==1)
+    assert isinstance(minus, PyccelMinus)==1
 
     a = Variable('int', 'a')
     b = Variable('int', 'b')
-    assert(minus.args[0] == a)
-    assert(minus.args[1] == b)
+    assert minus.args[0] == a
+    assert minus.args[1] == b
 
 def test_get_user_nodes():
     filename = os.path.join(path_dir, "math.py")
 
     interesting_var = Variable('int', 'a')
 
     fst = get_functions(filename)[0]
     atts = set(fst.get_attribute_nodes(Variable))
     atts = [v for v in atts  if v == interesting_var]
 
     a_var = atts[0]
 
     sums = set(a_var.get_user_nodes((PyccelAdd, PyccelMinus)))
 
-    assert(all(isinstance(s, (PyccelAdd, PyccelMinus)) for s in sums))
+    assert all(isinstance(s, (PyccelAdd, PyccelMinus)) for s in sums)
 
-    assert(len(sums) == 3)
+    assert len(sums) == 3
 
 def test_get_user_nodes_excluded():
     filename = os.path.join(path_dir, "math.py")
 
     interesting_var = Variable('int', 'a')
 
     fst = get_functions(filename)[0]
     atts = set(fst.get_attribute_nodes(Variable))
     atts = [v for v in atts  if v == interesting_var]
 
     a_var = atts[0]
 
     plus_assign = a_var.get_user_nodes(Assign, excluded_nodes = PyccelMinus)
-    assert(len(plus_assign)==2)
+    assert len(plus_assign)==2
+
+def test_get_all_user_nodes():
+    filename = os.path.join(path_dir, "math.py")
+
+    interesting_var = Variable('int', 'b')
+
+    fst = get_functions(filename)[0]
+    atts = set(fst.get_attribute_nodes(Variable))
+    atts = [v for v in atts  if v == interesting_var]
+
+    a_var = atts[0]
+
+    users = set(a_var.get_all_user_nodes())
+
+    assert all(isinstance(s, (PyccelMul, PyccelMinus, AugAssign, FunctionDefArgument)) for s in users)
+
+    assert len(users) == 4
 
 def test_get_direct_user_nodes():
     filename = os.path.join(path_dir, "math.py")
 
     interesting_var = Variable('int', 'a')
 
     fst = get_functions(filename)[0]
     atts = set(fst.get_attribute_nodes(Variable))
     atts = [v for v in atts  if v == interesting_var]
 
     a_var = atts[0]
 
     sums = set(a_var.get_direct_user_nodes(lambda x : isinstance(x,(PyccelAdd, PyccelMinus))))
 
-    assert(all(isinstance(s, (PyccelAdd, PyccelMinus)) for s in sums))
+    assert all(isinstance(s, (PyccelAdd, PyccelMinus)) for s in sums)
 
-    assert(len(sums) == 2)
+    assert len(sums) == 2
 
 def test_substitute():
     filename = os.path.join(path_dir, "math.py")
 
     interesting_var = Variable('int', 'a')
     new_var = Variable('int', 'Z')
 
     fst = get_functions(filename)[0]
     atts = set(fst.get_attribute_nodes(Variable))
     atts = [v for v in atts  if v == interesting_var]
 
     a_var = atts[0]
     old_parents = a_var.get_user_nodes(Basic)
-    assert(len(a_var.get_user_nodes(Basic))>0)
+    assert len(a_var.get_user_nodes(Basic))>0
 
     fst.substitute(a_var, new_var)
 
-    assert(len(a_var.get_user_nodes(Basic))==0)
+    assert len(a_var.get_user_nodes(Basic))==0
 
     atts = set(fst.get_attribute_nodes(Variable))
-    assert(new_var in atts)
-    assert(set(new_var.get_user_nodes(Basic)) == set(old_parents))
+    assert new_var in atts
+    assert set(new_var.get_user_nodes(Basic)) == set(old_parents)
 
 def test_substitute_exclude():
     filename = os.path.join(path_dir, "math.py")
 
     interesting_var = Variable('int', 'a')
     new_var = Variable('int', 'Z')
 
     fst = get_functions(filename)[0]
     atts = set(fst.get_attribute_nodes(Variable))
     atts = [v for v in atts  if v == interesting_var]
 
     a_var = atts[0]
     old_parents = set(a_var.get_user_nodes(Basic))
-    assert(len(a_var.get_user_nodes(Basic))>0)
+    assert len(a_var.get_user_nodes(Basic))>0
 
     fst.substitute(a_var, new_var, excluded_nodes=(PyccelMinus))
 
-    assert(len(a_var.get_user_nodes(Basic))==1)
+    assert len(a_var.get_user_nodes(Basic))==1
 
     atts = set(fst.get_attribute_nodes(Variable))
-    assert(new_var in atts)
+    assert new_var in atts
 
     new_parents = set(new_var.get_user_nodes(Basic))
-    assert(len(new_parents.difference(old_parents))==0)
-    assert(len(old_parents.difference(new_parents))==1)
+    assert len(new_parents.difference(old_parents))==0
+    assert len(old_parents.difference(new_parents))==1
 
 def test_recursive():
     filename = os.path.join(path_dir, "cyclic_dependence.py")
 
     fst = get_functions(filename)[0]
 
     atts = fst.get_attribute_nodes(PyccelMinus)
-    assert(len(set(atts))==2)
+    assert len(set(atts))==2
 
     var = atts[0].args[0]
 
     atts = var.get_user_nodes(FunctionDef)
-    assert(len(set(atts))==2) # The actual FunctionDef + the signature version
+    assert len(set(atts))==2 # The actual FunctionDef + the signature version
 
     fst.substitute(LiteralInteger(2), LiteralInteger(3))
```

### Comparing `pyccel-1.7.4/tests/codegen/ccode/scripts/arrays.py` & `pyccel-1.8.0/tests/codegen/ccode/scripts/arrays.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_create.py` & `pyccel-1.8.0/tests/codegen/ccode/scripts/arrays_create.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_indexing.py` & `pyccel-1.8.0/tests/codegen/ccode/scripts/arrays_indexing.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_pointers.py` & `pyccel-1.8.0/tests/codegen/ccode/scripts/arrays_pointers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/ccode/scripts/arrays_slicing.py` & `pyccel-1.8.0/tests/codegen/ccode/scripts/arrays_slicing.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/ccode/scripts/functions.py` & `pyccel-1.8.0/tests/codegen/ccode/scripts/functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/ccode/scripts/ifs.py` & `pyccel-1.8.0/tests/codegen/ccode/scripts/ifs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/ccode/scripts/loops.py` & `pyccel-1.8.0/tests/codegen/ccode/scripts/loops.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/ccode/test_ccode_codegen.py` & `pyccel-1.8.0/tests/codegen/ccode/test_ccode_codegen.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/CommentBlock.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/CommentBlock.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/Functional_Stmts.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/Functional_Stmts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/classes.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/classes.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/classes_2.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/classes_2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/classes_3.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/classes_3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/classes_4.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/classes_4.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/context.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/context.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/decorators.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/decorators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/decorators_types.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/decorators_types.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/functions_inout.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/functions_inout.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/ifs.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/ifs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/loops.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/loops.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/macros.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/macros.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/matrix_assembly.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/matrix_assembly.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/matrix_mul.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/matrix_mul.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/numpyext.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/numpyext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/precision.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/precision.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/scripts/recursive_functions.py` & `pyccel-1.8.0/tests/codegen/fcode/scripts/recursive_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/fcode/test_fcode_codegen.py` & `pyccel-1.8.0/tests/codegen/fcode/test_fcode_codegen.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/pycode/scripts/loops.py` & `pyccel-1.8.0/tests/codegen/pycode/scripts/loops.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/codegen/pycode/test_pycode_codegen.py` & `pyccel-1.8.0/tests/codegen/pycode/test_pycode_codegen.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/complexity/test_complexity.py` & `pyccel-1.8.0/tests/complexity/test_complexity.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/conftest.py` & `pyccel-1.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/Module_5.py` & `pyccel-1.8.0/tests/epyccel/modules/Module_5.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/Module_6.py` & `pyccel-1.8.0/tests/epyccel/modules/Module_6.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/Module_7.py` & `pyccel-1.8.0/tests/epyccel/modules/Module_7.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/array_consts.py` & `pyccel-1.8.0/tests/epyccel/modules/array_consts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/arrays.py` & `pyccel-1.8.0/tests/epyccel/modules/arrays.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/augassign.py` & `pyccel-1.8.0/tests/epyccel/modules/augassign.py`

 * *Files 9% similar despite different names*

```diff
@@ -149,7 +149,18 @@
     return b[0][0]
 
 @types('complex[:,:]')
 def augassign_div_2d_complex(a):
     b = a
     b /= (4.0 + 2.0j)
     return b[0][0]
+
+def augassign_func(x : float, y : float):
+    def fun1(x: 'float') -> 'float':
+        return x + 1
+    x %= fun1(y)
+    return x
+
+def augassign_array_func(x : 'float[:]', y : 'float[:]'):
+    def fun1(x: 'float[:]') -> 'float[:]':
+        return x + 1
+    x %= fun1(y)
```

### Comparing `pyccel-1.7.4/tests/epyccel/modules/base.py` & `pyccel-1.8.0/tests/epyccel/modules/base.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/bitwise.py` & `pyccel-1.8.0/tests/epyccel/modules/bitwise.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/call_user_defined_funcs.py` & `pyccel-1.8.0/tests/epyccel/modules/call_user_defined_funcs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/complex_func.py` & `pyccel-1.8.0/tests/epyccel/modules/complex_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/external_functions.py` & `pyccel-1.8.0/tests/epyccel/modules/external_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/functionals.py` & `pyccel-1.8.0/tests/epyccel/modules/functionals.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/generic_functions.py` & `pyccel-1.8.0/tests/epyccel/modules/generic_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/generic_functions_2.py` & `pyccel-1.8.0/tests/epyccel/modules/generic_functions_2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/highorder_functions.py` & `pyccel-1.8.0/tests/epyccel/modules/highorder_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/loops.py` & `pyccel-1.8.0/tests/epyccel/modules/loops.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,14 +92,27 @@
     x = [i for i in range(m)]
     y = [j for j in range(n)]
 
     for i,j in product( x, y ):
         z[i,j] = i-j
 
 # ...
+def product_loop( z : 'float[:]', m : int, n : int ):
+
+    from itertools import product
+
+    x = [i*3+2 for i in range(m)]
+    y = [j*7+6 for j in range(n)]
+
+    k = 0
+    for i,j in product( x, y ):
+        z[k] = i-j
+        k += 1
+
+# ...
 @types( 'int[:]' )
 def map_on_1d_array( z ):
 
     @types( int )
     def f( x ):
         return x+5
```

### Comparing `pyccel-1.7.4/tests/epyccel/modules/mpi_collective.py` & `pyccel-1.8.0/tests/epyccel/modules/mpi_collective.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/mpi_point_to_point.py` & `pyccel-1.8.0/tests/epyccel/modules/mpi_point_to_point.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/multi_rank.py` & `pyccel-1.8.0/tests/epyccel/modules/multi_rank.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/numpy_sign.py` & `pyccel-1.8.0/tests/epyccel/modules/numpy_sign.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/openmp.py` & `pyccel-1.8.0/tests/epyccel/modules/openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/pointers.py` & `pyccel-1.8.0/tests/epyccel/modules/pointers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/python_annotations.py` & `pyccel-1.8.0/tests/epyccel/modules/python_annotations.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/strings.py` & `pyccel-1.8.0/tests/epyccel/modules/strings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/tuples.py` & `pyccel-1.8.0/tests/epyccel/modules/tuples.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/modules/types.py` & `pyccel-1.8.0/tests/epyccel/modules/types.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py` & `pyccel-1.8.0/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/recognised_functions/test_math_funcs.py` & `pyccel-1.8.0/tests/epyccel/recognised_functions/test_math_funcs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/recognised_functions/test_numpy_funcs.py` & `pyccel-1.8.0/tests/epyccel/recognised_functions/test_numpy_funcs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/recognised_functions/test_numpy_types.py` & `pyccel-1.8.0/tests/epyccel/recognised_functions/test_numpy_types.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_array_as_func_args.py` & `pyccel-1.8.0/tests/epyccel/test_array_as_func_args.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_arrays.py` & `pyccel-1.8.0/tests/epyccel/test_arrays.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,42 +81,84 @@
     a = randint(low = -1e9, high = 1e9, dtype = np.int32)
 
     f1(x1, a)
     f2(x2, a)
 
     assert np.array_equal( x1, x2 )
 
+def test_array_int32_1d_scalar_add_stride(language):
+
+    f1 = arrays.array_int32_1d_scalar_add
+    f2 = epyccel( f1 , language = language)
+
+    x1 = np.array( [1,2,3,4,5,6,7,8], dtype=np.int32 )
+    x2 = np.copy(x1)
+    a = randint(low = -1e9, high = 1e9, dtype = np.int32)
+
+    f1(x1[::3], a)
+    f2(x2[::3], a)
+
+    assert np.array_equal( x1, x2 )
+
 def test_array_int32_1d_scalar_sub(language):
 
     f1 = arrays.array_int32_1d_scalar_sub
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [1,2,3], dtype=np.int32 )
     x2 = np.copy(x1)
     a = randint(low = -1e9, high = 1e9, dtype = np.int32)
 
     f1(x1, a)
     f2(x2, a)
 
     assert np.array_equal( x1, x2 )
 
+def test_array_int32_1d_scalar_sub_stride(language):
+
+    f1 = arrays.array_int32_1d_scalar_sub
+    f2 = epyccel( f1 , language = language)
+
+    x1 = np.array( [1,2,3,4,5,6,7,8,9], dtype=np.int32 )
+    x2 = np.copy(x1)
+    a = randint(low = -1e9, high = 1e9, dtype = np.int32)
+
+    f1(x1[::2], a)
+    f2(x2[::2], a)
+
+    assert np.array_equal( x1, x2 )
+
 def test_array_int32_1d_scalar_mul(language):
 
     f1 = arrays.array_int32_1d_scalar_mul
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [1,2,3], dtype=np.int32 )
     x2 = np.copy(x1)
     a = randint(low = -1e9, high = 1e9, dtype = np.int32)
 
     f1(x1, a)
     f2(x2, a)
 
     assert np.array_equal( x1, x2 )
 
+def test_array_int32_1d_scalar_mul_stride(language):
+
+    f1 = arrays.array_int32_1d_scalar_mul
+    f2 = epyccel( f1 , language = language)
+
+    x1 = np.array( [1,2,3,4,5,6,7,8,9], dtype=np.int32 )
+    x2 = np.copy(x1)
+    a = randint(low = -1e9, high = 1e9, dtype = np.int32)
+
+    f1(x1[3:7:2], a)
+    f2(x2[3:7:2], a)
+
+    assert np.array_equal( x1, x2 )
+
 def test_array_int32_1d_scalar_div(language):
 
     f1 = arrays.array_int32_1d_scalar_div
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [1,2,3], dtype=np.int32 )
     x2 = np.copy(x1)
@@ -137,14 +179,28 @@
     a = randint(low = 1, high = 1e9, dtype = np.int32)
 
     f1(x1, a)
     f2(x2, a)
 
     assert np.array_equal( x1, x2 )
 
+def test_array_int32_1d_scalar_idiv_stride(language):
+
+    f1 = arrays.array_int32_1d_scalar_idiv
+    f2 = epyccel( f1 , language = language)
+
+    x1 = np.array( [1,2,3,4,5,6,7,8,9], dtype=np.int32 )
+    x2 = np.copy(x1)
+    a = randint(low = 1, high = 1e9, dtype = np.int32)
+
+    f1(x1[:3:2], a)
+    f2(x2[:3:2], a)
+
+    assert np.array_equal( x1, x2 )
+
 def test_array_int32_1d_add(language):
 
     f1 = arrays.array_int32_1d_add
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [1,2,3], dtype=np.int32 )
     x2 = np.copy(x1)
@@ -260,56 +316,132 @@
     a = randint(low = -1e9, high = 1e9, dtype = np.int32)
 
     f1(x1, a)
     f2(x2, a)
 
     assert np.array_equal( x1, x2 )
 
+def test_array_int32_2d_C_scalar_add_stride(language):
+
+    f1 = arrays.array_int32_2d_C_scalar_add
+    f2 = epyccel( f1 , language = language)
+
+    x1 = np.array( [[1,2,3], [4,5,6]], dtype=np.int32 )
+    x2 = np.copy(x1)
+    a = randint(low = -1e9, high = 1e9, dtype = np.int32)
+
+    f1(x1[::2,:], a)
+    f2(x2[::2,:], a)
+
+    assert np.array_equal( x1, x2 )
+
 def test_array_int32_2d_C_scalar_sub(language):
 
     f1 = arrays.array_int32_2d_C_scalar_sub
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [[1,2,3], [4,5,6]], dtype=np.int32 )
     x2 = np.copy(x1)
     a = randint(low = -1e9, high = 1e9, dtype = np.int32)
 
     f1(x1, a)
     f2(x2, a)
 
     assert np.array_equal( x1, x2 )
 
+@pytest.mark.parametrize( 'language', [
+        pytest.param("c", marks = [
+            pytest.mark.xfail(reason="Ordering is unknown on non-contiguous array"),
+            pytest.mark.c]),
+        pytest.param("fortran", marks = [
+            pytest.mark.xfail(reason="Ordering is unknown on non-contiguous array"),
+            pytest.mark.fortran]),
+        pytest.param("python", marks = pytest.mark.python)
+    ]
+)
+def test_array_int32_2d_C_scalar_sub_stride(language):
+
+    f1 = arrays.array_int32_2d_C_scalar_sub
+    f2 = epyccel( f1 , language = language)
+
+    x1 = np.array( [[1,2,3,7], [4,5,6,8]], dtype=np.int32 )
+    x2 = np.copy(x1)
+    a = randint(low = -1e9, high = 1e9, dtype = np.int32)
+
+    f1(x1[:,::2], a)
+    f2(x2[:,::2], a)
+
+    assert np.array_equal( x1, x2 )
+
 def test_array_int32_2d_C_scalar_mul(language):
 
     f1 = arrays.array_int32_2d_C_scalar_mul
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [[1,2,3], [4,5,6]], dtype=np.int32 )
     x2 = np.copy(x1)
     a = randint(low = -1e9, high = 1e9, dtype = np.int32)
 
     f1(x1, a)
     f2(x2, a)
 
     assert np.array_equal( x1, x2 )
 
+def test_array_int32_2d_C_scalar_mul_stride(language):
+
+    f1 = arrays.array_int32_2d_C_scalar_mul
+    f2 = epyccel( f1 , language = language)
+
+    x1 = np.array( [[1,2,3], [4,5,6]], dtype=np.int32 )
+    x2 = np.copy(x1)
+    a = randint(low = -1e9, high = 1e9, dtype = np.int32)
+
+    f1(x1[1:,:], a)
+    f2(x2[1:,:], a)
+
+    assert np.array_equal( x1, x2 )
+
 def test_array_int32_2d_C_scalar_idiv(language):
 
     f1 = arrays.array_int32_2d_C_scalar_idiv
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [[1,2,3], [4,5,6]], dtype=np.int32 )
     x2 = np.copy(x1)
     a = randint(low = 1, high = 1e9, dtype = np.int32)
 
     f1(x1, a)
     f2(x2, a)
 
     assert np.array_equal( x1, x2 )
 
+@pytest.mark.parametrize( 'language', [
+        pytest.param("c", marks = [
+            pytest.mark.xfail(reason="Ordering is unknown on non-contiguous array"),
+            pytest.mark.c]),
+        pytest.param("fortran", marks = [
+            pytest.mark.xfail(reason="Ordering is unknown on non-contiguous array"),
+            pytest.mark.fortran]),
+        pytest.param("python", marks = pytest.mark.python)
+    ]
+)
+def test_array_int32_2d_C_scalar_idiv_stride(language):
+
+    f1 = arrays.array_int32_2d_C_scalar_idiv
+    f2 = epyccel( f1 , language = language)
+
+    x1 = np.array( [[1,2,3], [4,5,6]], dtype=np.int32 )
+    x2 = np.copy(x1)
+    a = randint(low = 1, high = 1e9, dtype = np.int32)
+
+    f1(x1[:,1:], a)
+    f2(x2[:,1:], a)
+
+    assert np.array_equal( x1, x2 )
+
 def test_array_int32_2d_C_add(language):
 
     f1 = arrays.array_int32_2d_C_add
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [[1,2,3], [4,5,6]], dtype=np.int32 )
     x2 = np.copy(x1)
@@ -376,28 +508,76 @@
     a = randint(low = -1e9, high = 1e9, dtype = np.int32)
 
     f1(x1, a)
     f2(x2, a)
 
     assert np.array_equal( x1, x2 )
 
+@pytest.mark.parametrize( 'language', [
+        pytest.param("c", marks = [
+            pytest.mark.xfail(reason="Ordering is unknown on non-contiguous array"),
+            pytest.mark.c]),
+        pytest.param("fortran", marks = [
+            pytest.mark.xfail(reason="Ordering is unknown on non-contiguous array"),
+            pytest.mark.fortran]),
+        pytest.param("python", marks = pytest.mark.python)
+    ]
+)
+def test_array_int32_2d_F_scalar_add_stride(language):
+
+    f1 = arrays.array_int32_2d_F_scalar_add
+    f2 = epyccel( f1 , language = language)
+
+    x1 = np.array( [[1,2,3], [4,5,6], [7,8,9]], dtype=np.int32, order='F' )
+    x2 = np.copy(x1)
+    a = randint(low = -1e9, high = 1e9, dtype = np.int32)
+
+    f1(x1[1::2,::2], a)
+    f2(x2[1::2,::2], a)
+
+    assert np.array_equal( x1, x2 )
+
 def test_array_int32_2d_F_scalar_sub(language):
 
     f1 = arrays.array_int32_2d_F_scalar_sub
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [[1,2,3], [4,5,6]], dtype=np.int32, order='F' )
     x2 = np.copy(x1)
     a = randint(low = -1e9, high = 1e9, dtype = np.int32)
 
     f1(x1, a)
     f2(x2, a)
 
     assert np.array_equal( x1, x2 )
 
+@pytest.mark.parametrize( 'language', [
+        pytest.param("c", marks = [
+            pytest.mark.xfail(reason="Ordering is unknown on non-contiguous array"),
+            pytest.mark.c]),
+        pytest.param("fortran", marks = [
+            pytest.mark.xfail(reason="Ordering is unknown on non-contiguous array"),
+            pytest.mark.fortran]),
+        pytest.param("python", marks = pytest.mark.python)
+    ]
+)
+def test_array_int32_2d_F_scalar_sub_stride(language):
+
+    f1 = arrays.array_int32_2d_F_scalar_sub
+    f2 = epyccel( f1 , language = language)
+
+    x1 = np.array( [[1,2,3], [4,5,6], [7,8,9]], dtype=np.int32, order='F' )
+    x2 = np.copy(x1)
+    a = randint(low = -1e9, high = 1e9, dtype = np.int32)
+
+    f1(x1[::2,1::2], a)
+    f2(x2[::2,1::2], a)
+
+    assert np.array_equal( x1, x2 )
+
 def test_array_int32_2d_F_scalar_mul(language):
 
     f1 = arrays.array_int32_2d_F_scalar_mul
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [[1,2,3], [4,5,6]], dtype=np.int32, order='F' )
     x2 = np.copy(x1)
```

### Comparing `pyccel-1.7.4/tests/epyccel/test_arrays_multiple_assignments.py` & `pyccel-1.8.0/tests/epyccel/test_arrays_multiple_assignments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # pylint: disable=missing-function-docstring, missing-module-docstring
+import os
+import sys
 import pytest
 
 from pyccel.epyccel import epyccel
 from pyccel.decorators import stack_array, types
 from pyccel.errors.errors import Errors, PyccelSemanticError
 from pyccel.errors.messages import (ARRAY_REALLOCATION,
                                     ARRAY_DEFINITION_IN_LOOP,
@@ -297,14 +299,33 @@
     # Check that we don't get a Pyccel warning
     assert not errors.has_warnings()
 
     assert f(True,True) == f2(True,True)
     assert f(True,False) == f2(True,False)
     assert f(False,True) == f2(False,True)
 
+@pytest.mark.skipif(sys.platform == 'win32', reason="Compilation problem. NumPy causing unreadable Windows output see issue #1405")
+def test_conda_flag_disable(language):
+    def one():
+        return True
+    with pytest.warns(None) as record1:
+        epyccel(one, language='c', conda_warnings = 'off')
+    assert len(record1) == 0 # Equals 0 on every platform
+
+@pytest.mark.skipif(sys.platform == 'win32', reason="Compilation problem. NumPy causing unreadable Windows output see issue #1405")
+def test_conda_flag_verbose(language):
+    def one():
+        return True
+    with pytest.warns(None) as record1:
+        epyccel(one, language='c', conda_warnings = 'verbose')
+    if len(record1)>0:
+        warn_message = record1[0].message
+        p = str(warn_message).split(":")[2].strip()
+        assert p in os.environ['PATH']
+
 #==============================================================================
 
 if __name__ == '__main__':
 
     for l in ['fortran']:
 
         test_no_reallocation(l)
```

### Comparing `pyccel-1.7.4/tests/epyccel/test_base.py` & `pyccel-1.8.0/tests/epyccel/test_base.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_bitwise.py` & `pyccel-1.8.0/tests/epyccel/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_builtins.py` & `pyccel-1.8.0/tests/epyccel/test_builtins.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_class_expressions.py` & `pyccel-1.8.0/tests/epyccel/test_class_expressions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_compare_expressions.py` & `pyccel-1.8.0/tests/epyccel/test_compare_expressions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_default_precision_template.py` & `pyccel-1.8.0/tests/epyccel/test_default_precision_template.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_docstrings.py` & `pyccel-1.8.0/tests/epyccel/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_IfTernaryOperator.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_IfTernaryOperator.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_complex_func.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_complex_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_decorators.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_decorators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_default_args.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_default_args.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_division.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_division.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_functions.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_generators.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_generators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_mod.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_mod.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_modules.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_modules.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_multi_rank.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_multi_rank.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_openmp.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_optional_args.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_optional_args.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_pow.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_pow.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_python_annotations.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_python_annotations.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_return_arrays.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_return_arrays.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_sign.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_sign.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_transpose.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_transpose.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_epyccel_types.py` & `pyccel-1.8.0/tests/epyccel/test_epyccel_types.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_external_functions.py` & `pyccel-1.8.0/tests/epyccel/test_external_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_functionals.py` & `pyccel-1.8.0/tests/epyccel/test_functionals.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_generic_functions.py` & `pyccel-1.8.0/tests/epyccel/test_generic_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_higherorder_functions.py` & `pyccel-1.8.0/tests/epyccel/test_higherorder_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_imports.py` & `pyccel-1.8.0/tests/epyccel/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_kind.py` & `pyccel-1.8.0/tests/epyccel/test_kind.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_loops.py` & `pyccel-1.8.0/tests/epyccel/test_loops.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,26 @@
     x = np.zeros( (11,4), dtype=int, order='F' )
     y = np.ones ( (11,4), dtype=int, order='F' )
 
     f1( x )
     f2( y )
     assert np.array_equal( x, y )
 
+def test_product_loop(language):
+
+    f1 = loops.product_loop
+    f2 = epyccel(f1, language=language)
+
+    x = np.zeros( (44), dtype=float )
+    y = np.zeros( (44), dtype=float )
+
+    f1( x, 4, 11 )
+    f2( y, 4, 11 )
+    assert np.array_equal( x, y )
+
 @pytest.mark.parametrize( 'language', (
         pytest.param("fortran", marks = pytest.mark.fortran),
         pytest.param("c", marks = [
             pytest.mark.xfail(reason="Function in function not implemented in C"),
             pytest.mark.c]
         ),
         pytest.param("python", marks = pytest.mark.python)
```

### Comparing `pyccel-1.7.4/tests/epyccel/test_mpi_collective.py` & `pyccel-1.8.0/tests/epyccel/test_mpi_collective.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_mpi_point_to_point.py` & `pyccel-1.8.0/tests/epyccel/test_mpi_point_to_point.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_multiple_results.py` & `pyccel-1.8.0/tests/epyccel/test_multiple_results.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_parallel_epyccel.py` & `pyccel-1.8.0/tests/epyccel/test_parallel_epyccel.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_pointers.py` & `pyccel-1.8.0/tests/epyccel/test_pointers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_return.py` & `pyccel-1.8.0/tests/epyccel/test_return.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_strings.py` & `pyccel-1.8.0/tests/epyccel/test_strings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/test_tuples.py` & `pyccel-1.8.0/tests/epyccel/test_tuples.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/epyccel/utilities.py` & `pyccel-1.8.0/tests/epyccel/utilities.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/errors/known_bugs/ex4.py` & `pyccel-1.8.0/tests/errors/known_bugs/ex4.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/errors/known_bugs/generic_methods.py` & `pyccel-1.8.0/tests/errors/known_bugs/generic_methods.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/errors/known_bugs/header_interface.py` & `pyccel-1.8.0/tests/errors/known_bugs/header_interface.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/errors/known_bugs/inheritance.py` & `pyccel-1.8.0/tests/errors/known_bugs/inheritance.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/errors/test_errors.py` & `pyccel-1.8.0/tests/errors/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/lapack/ex1.py` & `pyccel-1.8.0/tests/external/scripts/lapack/ex1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/mpi4py/bcast.py` & `pyccel-1.8.0/tests/external/scripts/mpi4py/bcast.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/mpi4py/bugs/ex6.py` & `pyccel-1.8.0/tests/external/scripts/mpi4py/bugs/ex6.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/mpi4py/bugs/ex8.py` & `pyccel-1.8.0/tests/external/scripts/mpi4py/bugs/ex8.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/mpi4py/gather.py` & `pyccel-1.8.0/tests/external/scripts/mpi4py/gather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/mpi4py/np_Bcast.py` & `pyccel-1.8.0/tests/external/scripts/mpi4py/np_Bcast.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/mpi4py/np_Gather.py` & `pyccel-1.8.0/tests/external/scripts/mpi4py/np_Gather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/mpi4py/np_Sendrecv.py` & `pyccel-1.8.0/tests/external/scripts/mpi4py/np_Sendrecv.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/mpi4py/np_point_to_point.py` & `pyccel-1.8.0/tests/external/scripts/mpi4py/np_point_to_point.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/mpi4py/np_point_to_point_3.py` & `pyccel-1.8.0/tests/external/scripts/mpi4py/np_point_to_point_3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/scripts/mpi4py/point_to_point_3.py` & `pyccel-1.8.0/tests/external/scripts/mpi4py/point_to_point_3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/external/test_external.py` & `pyccel-1.8.0/tests/external/test_external.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/blas/ex1.py` & `pyccel-1.8.0/tests/internal/scripts/blas/ex1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/blas/ex2.py` & `pyccel-1.8.0/tests/internal/scripts/blas/ex2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/blas/ex3.py` & `pyccel-1.8.0/tests/internal/scripts/blas/ex3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/blas/ex4.py` & `pyccel-1.8.0/tests/internal/scripts/blas/ex4.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/blas/ex5.py` & `pyccel-1.8.0/tests/internal/scripts/blas/ex5.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/lapack/ex1.py` & `pyccel-1.8.0/tests/internal/scripts/lapack/ex1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/allgather.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/allgather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/allreduce.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/allreduce.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/alltoall.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/alltoall.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/bcast.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/bcast.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/column.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/column.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/gather.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/gather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/line.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/line.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/nonblocking.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/nonblocking.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/point_to_point_1.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/point_to_point_1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/point_to_point_2.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/point_to_point_2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/reduce.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/reduce.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/scatter.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/scatter.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/sendrecv.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/sendrecv.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/sendrecv_replace.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/sendrecv_replace.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/split.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/split.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/mpi/who_am_i.py` & `pyccel-1.8.0/tests/internal/scripts/mpi/who_am_i.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/openacc/sum.py` & `pyccel-1.8.0/tests/internal/scripts/openacc/sum.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/openacc/sum_kernels.py` & `pyccel-1.8.0/tests/internal/scripts/openacc/sum_kernels.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/scripts/openmp/ex1.py` & `pyccel-1.8.0/tests/internal/scripts/openmp/ex1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/internal/test_internal.py` & `pyccel-1.8.0/tests/internal/test_internal.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/bcast.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/bcast.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/bug/ex6.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/bug/ex6.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/bug/ex8.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/bug/ex8.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/gather.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/gather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/mpi4py.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/mpi4py.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/np_Allreduce.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/np_Allreduce.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/np_Bcast.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/np_Bcast.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/np_Gather.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/np_Gather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/np_Reduce.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/np_Reduce.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/np_Sendrecv.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/np_Sendrecv.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/np_point_to_point.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point_2.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/np_point_to_point_2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/np_point_to_point_3.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/np_point_to_point_3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/point_to_point_2.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/point_to_point_2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/MPI/point_to_point_3.py` & `pyccel-1.8.0/tests/macro/scripts/MPI/point_to_point_3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/blas/runtest_daxpy.py` & `pyccel-1.8.0/tests/macro/scripts/blas/runtest_daxpy.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/blas/runtest_dgemm.py` & `pyccel-1.8.0/tests/macro/scripts/blas/runtest_dgemm.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/blas/runtest_dgemv.py` & `pyccel-1.8.0/tests/macro/scripts/blas/runtest_dgemv.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/blas/runtest_dger.py` & `pyccel-1.8.0/tests/macro/scripts/blas/runtest_dger.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/blas/runtest_dswap.py` & `pyccel-1.8.0/tests/macro/scripts/blas/runtest_dswap.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/scripts/lapack/runtest_dgbtrf.py` & `pyccel-1.8.0/tests/macro/scripts/lapack/runtest_dgbtrf.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/macro/test_macro.py` & `pyccel-1.8.0/tests/macro/test_macro.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/ndarrays/conftest.py` & `pyccel-1.8.0/tests/ndarrays/conftest.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/ndarrays/leaks_check.py` & `pyccel-1.8.0/tests/ndarrays/leaks_check.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/ndarrays/test_ndarrays.c` & `pyccel-1.8.0/tests/ndarrays/test_ndarrays.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/parser/scripts/comments.py` & `pyccel-1.8.0/tests/parser/scripts/comments.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/parser/test_comments.py` & `pyccel-1.8.0/tests/parser/test_comments.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/parser/test_headers.py` & `pyccel-1.8.0/tests/parser/test_headers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/preprocess/scripts/omp.py` & `pyccel-1.8.0/tests/preprocess/scripts/omp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/preprocess/test_preprocess.py` & `pyccel-1.8.0/tests/preprocess/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/array_binary_operation.py` & `pyccel-1.8.0/tests/pyccel/scripts/array_binary_operation.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/arrays_view.py` & `pyccel-1.8.0/tests/pyccel/scripts/arrays_view.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/bool_comp.py` & `pyccel-1.8.0/tests/pyccel/scripts/bool_comp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/c_arrays.py` & `pyccel-1.8.0/tests/pyccel/scripts/c_arrays.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/classes/classes.py` & `pyccel-1.8.0/tests/pyccel/scripts/classes/classes.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/classes/classes_1.py` & `pyccel-1.8.0/tests/pyccel/scripts/classes/classes_1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/decorators_inline.py` & `pyccel-1.8.0/tests/pyccel/scripts/decorators_inline.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/default_args_mod.py` & `pyccel-1.8.0/tests/pyccel/scripts/default_args_mod.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/expressions.py` & `pyccel-1.8.0/tests/pyccel/scripts/expressions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/functions.py` & `pyccel-1.8.0/tests/pyccel/scripts/functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/generic_functions.py` & `pyccel-1.8.0/tests/pyccel/scripts/generic_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py` & `pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py` & `pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py` & `pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks/quicksort.py` & `pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks/quicksort.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py` & `pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py` & `pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py` & `pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py` & `pyccel-1.8.0/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import.py` & `pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as.py` & `pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import_as.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py` & `pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/from_mod_import_func.py` & `pyccel-1.8.0/tests/pyccel/scripts/import_syntax/from_mod_import_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod.py` & `pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as.py` & `pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod_as.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_as_func.py` & `pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod_as_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/import_syntax/import_mod_func.py` & `pyccel-1.8.0/tests/pyccel/scripts/import_syntax/import_mod_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/lapack_subroutine.py` & `pyccel-1.8.0/tests/pyccel/scripts/lapack_subroutine.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/numpy/numpy_kernels.py` & `pyccel-1.8.0/tests/pyccel/scripts/numpy/numpy_kernels.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/numpy/numpy_sign.py` & `pyccel-1.8.0/tests/pyccel/scripts/numpy/numpy_sign.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/print_integers.py` & `pyccel-1.8.0/tests/pyccel/scripts/print_integers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/print_sp_and_end.py` & `pyccel-1.8.0/tests/pyccel/scripts/print_sp_and_end.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/print_strings.py` & `pyccel-1.8.0/tests/pyccel/scripts/print_strings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/return_numpy_arrays.py` & `pyccel-1.8.0/tests/pyccel/scripts/return_numpy_arrays.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,7 +25,8 @@
 d = f(False, True)
 e = f(1+2j, 3+4j)
 h,g = multi_returns()
 k = single_return() + 1
 
 if __name__ == '__main__':
     print(a, b, c, d, e, h, g, k)
+    print(np.array([1,2,3,4]), np.array([1, 3]), np.array([1., 3.]), np.array([False, True]), np.array([1+2j, 3+4j]))
```

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/runtest_default_args.py` & `pyccel-1.8.0/tests/pyccel/scripts/runtest_default_args.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/runtest_degree_in.py` & `pyccel-1.8.0/tests/pyccel/scripts/runtest_degree_in.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/runtest_generic_functions.py` & `pyccel-1.8.0/tests/pyccel/scripts/runtest_generic_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/scripts/runtest_multiple_results.py` & `pyccel-1.8.0/tests/pyccel/scripts/runtest_multiple_results.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/pyccel/test_pyccel.py` & `pyccel-1.8.0/tests/pyccel/test_pyccel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # pylint: disable=missing-function-docstring, missing-module-docstring
 import subprocess
 import json
 import os
 import shutil
 import sys
 import re
+import random
 import pytest
 import numpy as np
+from pyccel.codegen.pipeline import execute_pyccel
+from pyccel.ast.utilities import python_builtin_libs
 
 #==============================================================================
 # UTILITIES
 #==============================================================================
 
 #------------------------------------------------------------------------------
 
@@ -991,7 +994,14 @@
         dict_1 = json.load(f)
     pyccel_test("scripts/runtest_funcs.py", language = 'fortran',
         pyccel_commands='--compiler test.json --export-compile-info test2.json')
     with open(get_abs_path('scripts/test2.json'),'r') as f:
         dict_2 = json.load(f)
 
     assert dict_1 == dict_2
+
+#------------------------------------------------------------------------------
+def test_reserved_file_name():
+    with pytest.raises(ValueError) as exc_info:
+        libname = str(random.choice(tuple(python_builtin_libs))) + ".py" # nosec B311
+        execute_pyccel(fname=libname)
+    assert str(exc_info.value) == f"File called {libname} has the same name as a Python built-in package and can't be imported from Python. See #1402"
```

### Comparing `pyccel-1.7.4/tests/run_tests.bat` & `pyccel-1.8.0/tests/run_tests.bat`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/run_tests_py3.sh` & `pyccel-1.8.0/tests/run_tests_py3.sh`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/semantic/scripts/expressions.py` & `pyccel-1.8.0/tests/semantic/scripts/expressions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/semantic/scripts/functions.py` & `pyccel-1.8.0/tests/semantic/scripts/functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/semantic/test_semantic.py` & `pyccel-1.8.0/tests/semantic/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/symbolic/scripts/decorator.py` & `pyccel-1.8.0/tests/symbolic/scripts/decorator.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/symbolic/scripts/neural_net.py` & `pyccel-1.8.0/tests/symbolic/scripts/neural_net.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/symbolic/test_symbolic.py` & `pyccel-1.8.0/tests/symbolic/test_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/syntax/scripts/Functional_Stmts.py` & `pyccel-1.8.0/tests/syntax/scripts/Functional_Stmts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/syntax/scripts/class_member_index.py` & `pyccel-1.8.0/tests/syntax/scripts/class_member_index.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/syntax/scripts/expressions.py` & `pyccel-1.8.0/tests/syntax/scripts/expressions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/syntax/test_syntax.py` & `pyccel-1.8.0/tests/syntax/test_syntax.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tests/warnings/test_warnings.py` & `pyccel-1.8.0/tests/warnings/test_warnings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tutorial/builtin-functions.md` & `pyccel-1.8.0/tutorial/builtin-functions.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tutorial/const_keyword.md` & `pyccel-1.8.0/tutorial/const_keyword.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tutorial/decorators.md` & `pyccel-1.8.0/tutorial/decorators.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tutorial/function-pointers-as-arguments.md` & `pyccel-1.8.0/tutorial/function-pointers-as-arguments.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tutorial/header-files.md` & `pyccel-1.8.0/tutorial/header-files.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tutorial/ndarrays.md` & `pyccel-1.8.0/tutorial/ndarrays.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tutorial/numpy-functions.md` & `pyccel-1.8.0/tutorial/numpy-functions.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tutorial/openmp.md` & `pyccel-1.8.0/tutorial/openmp.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tutorial/quickstart.md` & `pyccel-1.8.0/tutorial/quickstart.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.7.4/tutorial/templates.md` & `pyccel-1.8.0/tutorial/templates.md`

 * *Files identical despite different names*

