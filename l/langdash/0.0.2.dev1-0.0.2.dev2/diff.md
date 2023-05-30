# Comparing `tmp/langdash-0.0.2.dev1.tar.gz` & `tmp/langdash-0.0.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-0.0.2.dev1.tar", last modified: Tue May 30 04:33:01 2023, max compression
+gzip compressed data, was "langdash-0.0.2.dev2.tar", last modified: Tue May 30 15:34:23 2023, max compression
```

## Comparing `langdash-0.0.2.dev1.tar` & `langdash-0.0.2.dev2.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.963760 langdash-0.0.2.dev1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.2.dev1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-30 04:33:01.963760 langdash-0.0.2.dev1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2670 2023-05-30 04:30:36.000000 langdash-0.0.2.dev1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.887762 langdash-0.0.2.dev1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       31 2023-05-25 22:58:46.000000 langdash-0.0.2.dev1/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1440 2023-05-28 22:26:32.000000 langdash-0.0.2.dev1/langdash/_langdash.py
--rw-rw-r--   0 user      (1000) user      (1000)    13289 2023-05-30 03:59:32.000000 langdash-0.0.2.dev1/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.887762 langdash-0.0.2.dev1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.2.dev1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.2.dev1/langdash/classify/token_qa.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.879763 langdash-0.0.2.dev1/langdash/extern/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.895762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/
--rw-rw-r--   0 user      (1000) user      (1000)    16349 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeCache.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.895762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.899762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/
--rw-r--r--   0 user      (1000) user      (1000)     2441 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake
--rw-r--r--   0 user      (1000) user      (1000)     5439 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake
--rwxrwxr-x   0 user      (1000) user      (1000)    15968 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin
--rwxrwxr-x   0 user      (1000) user      (1000)    15992 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin
--rw-r--r--   0 user      (1000) user      (1000)      402 2023-05-25 00:05:29.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeSystem.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.899762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/
--rw-rw-r--   0 user      (1000) user      (1000)    24853 2023-05-25 00:05:29.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c
--rwxrwxr-x   0 user      (1000) user      (1000)    16088 2023-05-25 00:05:29.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.899762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/
--rw-rw-r--   0 user      (1000) user      (1000)    24597 2023-05-25 00:05:29.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp
--rwxrwxr-x   0 user      (1000) user      (1000)    16096 2023-05-25 00:05:29.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    50084 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log
--rw-rw-r--   0 user      (1000) user      (1000)     7911 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     9844 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2
--rw-rw-r--   0 user      (1000) user      (1000)     3155 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt
--rw-rw-r--   0 user      (1000) user      (1000)       85 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/cmake.check_cache
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/progress.marks
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.903762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      692 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     4674 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      276 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      679 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)   101576 2023-05-25 00:05:37.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o
--rw-rw-r--   0 user      (1000) user      (1000)    11910 2023-05-25 00:05:37.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d
--rw-rw-r--   0 user      (1000) user      (1000)     6908 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)      376 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CTestTestfile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1338 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/FILE_FORMAT.md
--rw-rw-r--   0 user      (1000) user      (1000)     1067 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     8978 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     6412 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.903762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)   165600 2023-05-25 00:05:38.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/bin/test_ggml_basics
--rwxrwxr-x   0 user      (1000) user      (1000)    16728 2023-05-25 00:05:38.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv
--rw-rw-r--   0 user      (1000) user      (1000)     2013 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     3799 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/compile_commands.json
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.903762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.903762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/progress.marks
--rw-rw-r--   0 user      (1000) user      (1000)     2552 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1072 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     7013 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     3707 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.903762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/cmake/
--rw-rw-r--   0 user      (1000) user      (1000)     2037 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      717 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1496 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.907761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/
--rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     8583 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp
--rw-rw-r--   0 user      (1000) user      (1000)      410 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.h
--rw-rw-r--   0 user      (1000) user      (1000)    15664 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     3311 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.907761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/
--rw-rw-r--   0 user      (1000) user      (1000)      319 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6201 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    28339 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp
--rw-rw-r--   0 user      (1000) user      (1000)   241358 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.911761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/
--rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6370 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     6313 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     4873 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     6436 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py
--rwxrwxr-x   0 user      (1000) user      (1000)     1752 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh
--rwxrwxr-x   0 user      (1000) user      (1000)     1117 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh
--rw-rw-r--   0 user      (1000) user      (1000)    29187 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5467 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.911761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/
--rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)    11108 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     5509 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py
--rwxrwxr-x   0 user      (1000) user      (1000)     1728 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      571 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh
--rw-rw-r--   0 user      (1000) user      (1000)    25782 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.915761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     3689 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     1491 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     7679 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.883762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.915761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/
--rw-rw-r--   0 user      (1000) user      (1000)  1591571 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict
--rw-rw-r--   0 user      (1000) user      (1000)  7840016 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.931761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/
--rw-rw-r--   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     4755 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    27316 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.935761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/
--rw-rw-r--   0 user      (1000) user      (1000)      501 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)      718 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     9506 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    36271 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     7693 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp
--rw-rw-r--   0 user      (1000) user      (1000)   184690 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp
--rw-rw-r--   0 user      (1000) user      (1000)    23750 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.883762 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/include/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.935761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/include/ggml/
--rw-rw-r--   0 user      (1000) user      (1000)    31202 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.935761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/scripts/
--rwxrwxr-x   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/scripts/sync-llama.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      921 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.939761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.939761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.939761 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      597 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5420 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      269 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean_target.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)     1057 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)   201672 2023-05-25 00:05:35.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o
--rw-rw-r--   0 user      (1000) user      (1000)    10631 2023-05-25 00:05:35.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d
--rw-rw-r--   0 user      (1000) user      (1000)       80 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/progress.marks
--rw-rw-r--   0 user      (1000) user      (1000)     8040 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     8522 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     1573 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    24594 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu
--rw-rw-r--   0 user      (1000) user      (1000)      638 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h
--rw-rw-r--   0 user      (1000) user      (1000)    13447 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c
--rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h
--rw-rw-r--   0 user      (1000) user      (1000)   428283 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml.c
--rw-rw-r--   0 user      (1000) user      (1000)   205118 2023-05-25 00:05:35.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/libggml.a
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.943760 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/
--rw-rw-r--   0 user      (1000) user      (1000)     9198 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6569 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c
--rw-rw-r--   0 user      (1000) user      (1000)    11463 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c
--rw-rw-r--   0 user      (1000) user      (1000)    10265 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c
--rw-rw-r--   0 user      (1000) user      (1000)     9003 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c
--rw-rw-r--   0 user      (1000) user      (1000)    91837 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c
--rw-rw-r--   0 user      (1000) user      (1000)     5141 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c
--rw-rw-r--   0 user      (1000) user      (1000)     3157 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c
--rw-rw-r--   0 user      (1000) user      (1000)    21179 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c
--rw-rw-r--   0 user      (1000) user      (1000)     7310 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c
--rw-rw-r--   0 user      (1000) user      (1000)     1182 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test0.c
--rw-rw-r--   0 user      (1000) user      (1000)    15073 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test1.c
--rw-rw-r--   0 user      (1000) user      (1000)     5703 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test2.c
--rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-25 00:05:22.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test3.c
--rwxrwxr-x   0 user      (1000) user      (1000)   243024 2023-05-25 00:05:38.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/librwkv.so
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.951760 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/
--rw-rw-r--   0 user      (1000) user      (1000)  2467981 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.951760 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/
--rw-rw-r--   0 user      (1000) user      (1000)     4174 2023-05-25 00:05:38.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     6921 2023-05-25 00:05:39.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     8813 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py
--rw-rw-r--   0 user      (1000) user      (1000)     3320 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py
--rw-rw-r--   0 user      (1000) user      (1000)     2380 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/generate_completions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3886 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py
--rw-rw-r--   0 user      (1000) user      (1000)     5833 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.955760 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/
--rw-rw-r--   0 user      (1000) user      (1000)      947 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      139 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1095 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      764 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1433 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      979 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1106 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/quantize.py
--rw-rw-r--   0 user      (1000) user      (1000)       23 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)     4359 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py
--rw-rw-r--   0 user      (1000) user      (1000)     7528 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py
--rw-rw-r--   0 user      (1000) user      (1000)     1255 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/sampling.py
--rw-rw-r--   0 user      (1000) user      (1000)    39641 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     4691 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.955760 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.959760 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/progress.marks
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.963760 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      871 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5923 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      359 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      119 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      123 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)      100 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      224 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)     5152 2023-05-25 00:05:38.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o
--rw-rw-r--   0 user      (1000) user      (1000)     3717 2023-05-25 00:05:38.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.963760 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      345 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      121 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       98 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)     9816 2023-05-25 00:05:38.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o
--rw-rw-r--   0 user      (1000) user      (1000)     4064 2023-05-25 00:05:38.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d
--rw-rw-r--   0 user      (1000) user      (1000)      577 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1309 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    10760 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     1292 2023-05-25 00:05:30.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1024 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/expected_logits.bin
--rw-rw-r--   0 user      (1000) user      (1000)     1724 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c
--rw-rw-r--   0 user      (1000) user      (1000)     5039 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c
--rw-rw-r--   0 user      (1000) user      (1000)  1338429 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin
--rw-rw-r--   0 user      (1000) user      (1000)  2649149 2023-05-25 00:04:50.000000 langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-25 22:58:46.000000 langdash-0.0.2.dev1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)      558 2023-05-29 18:12:41.000000 langdash-0.0.2.dev1/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     5371 2023-05-29 17:35:06.000000 langdash-0.0.2.dev1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.891762 langdash-0.0.2.dev1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.2.dev1/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      624 2023-05-25 22:58:44.000000 langdash-0.0.2.dev1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     6283 2023-05-30 02:47:10.000000 langdash-0.0.2.dev1/langdash/models/rwkvcpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 18:14:56.000000 langdash-0.0.2.dev1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     5766 2023-05-29 17:50:27.000000 langdash-0.0.2.dev1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      259 2023-05-25 22:58:46.000000 langdash-0.0.2.dev1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2156 2023-05-27 04:12:41.000000 langdash-0.0.2.dev1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.891762 langdash-0.0.2.dev1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.2.dev1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.2.dev1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.2.dev1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.2.dev1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 04:33:01.891762 langdash-0.0.2.dev1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-30 04:33:01.000000 langdash-0.0.2.dev1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    12207 2023-05-30 04:33:01.000000 langdash-0.0.2.dev1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-30 04:33:01.000000 langdash-0.0.2.dev1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-30 04:33:01.000000 langdash-0.0.2.dev1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-30 04:33:01.000000 langdash-0.0.2.dev1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-30 04:33:01.963760 langdash-0.0.2.dev1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1262 2023-05-30 04:32:55.000000 langdash-0.0.2.dev1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.284158 langdash-0.0.2.dev2/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.2.dev2/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-30 15:34:23.284158 langdash-0.0.2.dev2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2670 2023-05-30 08:29:06.000000 langdash-0.0.2.dev2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.176167 langdash-0.0.2.dev2/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       31 2023-05-25 22:58:46.000000 langdash-0.0.2.dev2/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3129 2023-05-30 08:35:04.000000 langdash-0.0.2.dev2/langdash/_langdash.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14626 2023-05-30 08:35:25.000000 langdash-0.0.2.dev2/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.176167 langdash-0.0.2.dev2/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.2.dev2/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.2.dev2/langdash/classify/token_qa.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.168168 langdash-0.0.2.dev2/langdash/extern/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.184167 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/
+-rw-rw-r--   0 user      (1000) user      (1000)    16349 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeCache.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.184167 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.188166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/
+-rw-r--r--   0 user      (1000) user      (1000)     2441 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake
+-rw-r--r--   0 user      (1000) user      (1000)     5439 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake
+-rwxrwxr-x   0 user      (1000) user      (1000)    15968 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin
+-rwxrwxr-x   0 user      (1000) user      (1000)    15992 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin
+-rw-r--r--   0 user      (1000) user      (1000)      402 2023-05-25 00:05:29.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeSystem.cmake
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.188166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/
+-rw-rw-r--   0 user      (1000) user      (1000)    24853 2023-05-25 00:05:29.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c
+-rwxrwxr-x   0 user      (1000) user      (1000)    16088 2023-05-25 00:05:29.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.188166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/
+-rw-rw-r--   0 user      (1000) user      (1000)    24597 2023-05-25 00:05:29.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp
+-rwxrwxr-x   0 user      (1000) user      (1000)    16096 2023-05-25 00:05:29.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)    50084 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log
+-rw-rw-r--   0 user      (1000) user      (1000)     7911 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     9844 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2
+-rw-rw-r--   0 user      (1000) user      (1000)     3155 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       85 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/cmake.check_cache
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/progress.marks
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.192166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      692 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     4674 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      276 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      679 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)   101576 2023-05-25 00:05:37.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o
+-rw-rw-r--   0 user      (1000) user      (1000)    11910 2023-05-25 00:05:37.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d
+-rw-rw-r--   0 user      (1000) user      (1000)     6908 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      376 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CTestTestfile.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     1338 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/FILE_FORMAT.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1067 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     8978 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     6412 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.196166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)   165600 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/bin/test_ggml_basics
+-rwxrwxr-x   0 user      (1000) user      (1000)    16728 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv
+-rw-rw-r--   0 user      (1000) user      (1000)     2013 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/cmake_install.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     3799 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/compile_commands.json
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.196166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.196166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/progress.marks
+-rw-rw-r--   0 user      (1000) user      (1000)     2552 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1072 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     7013 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     3707 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.196166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake/
+-rw-rw-r--   0 user      (1000) user      (1000)     2037 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      717 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     1496 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.200165 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/
+-rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     8583 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)      410 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.h
+-rw-rw-r--   0 user      (1000) user      (1000)    15664 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     3311 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.200165 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/
+-rw-rw-r--   0 user      (1000) user      (1000)      319 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     6201 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28339 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)   241358 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.204165 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/
+-rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     6370 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     6313 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4873 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6436 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     1752 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)     1117 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh
+-rw-rw-r--   0 user      (1000) user      (1000)    29187 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5467 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.204165 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/
+-rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)    11108 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     5509 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     1728 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)      571 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh
+-rw-rw-r--   0 user      (1000) user      (1000)    25782 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.208165 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     3689 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1491 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7679 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.172168 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.212164 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/
+-rw-rw-r--   0 user      (1000) user      (1000)  1591571 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict
+-rw-rw-r--   0 user      (1000) user      (1000)  7840016 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.232163 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/
+-rw-rw-r--   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     4755 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27316 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.236162 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/
+-rw-rw-r--   0 user      (1000) user      (1000)      501 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      718 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     9506 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)    36271 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     7693 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)   184690 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)    23750 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.172168 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/include/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.236162 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/
+-rw-rw-r--   0 user      (1000) user      (1000)    31202 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.236162 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/scripts/
+-rwxrwxr-x   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-llama.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)      921 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.240162 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.240162 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.244161 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      597 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     5420 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      269 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean_target.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)     1057 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)   201672 2023-05-25 00:05:35.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o
+-rw-rw-r--   0 user      (1000) user      (1000)    10631 2023-05-25 00:05:35.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d
+-rw-rw-r--   0 user      (1000) user      (1000)       80 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/progress.marks
+-rw-rw-r--   0 user      (1000) user      (1000)     8040 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     8522 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     1573 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)    24594 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu
+-rw-rw-r--   0 user      (1000) user      (1000)      638 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h
+-rw-rw-r--   0 user      (1000) user      (1000)    13447 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c
+-rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h
+-rw-rw-r--   0 user      (1000) user      (1000)   428283 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml.c
+-rw-rw-r--   0 user      (1000) user      (1000)   205118 2023-05-25 00:05:35.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/libggml.a
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.252161 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)     9198 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     6569 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    11463 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10265 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c
+-rw-rw-r--   0 user      (1000) user      (1000)     9003 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c
+-rw-rw-r--   0 user      (1000) user      (1000)    91837 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5141 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3157 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    21179 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7310 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1182 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    15073 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test1.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5703 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test2.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test3.c
+-rwxrwxr-x   0 user      (1000) user      (1000)   243024 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/librwkv.so
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.260160 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/
+-rw-rw-r--   0 user      (1000) user      (1000)  2467981 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.264160 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/
+-rw-rw-r--   0 user      (1000) user      (1000)     4174 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     6921 2023-05-25 00:05:39.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     8813 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3320 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2380 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/generate_completions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3886 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5833 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.264160 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/
+-rw-rw-r--   0 user      (1000) user      (1000)      947 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json
+-rw-rw-r--   0 user      (1000) user      (1000)      139 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-QA.json
+-rw-rw-r--   0 user      (1000) user      (1000)     1095 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json
+-rw-rw-r--   0 user      (1000) user      (1000)      764 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json
+-rw-rw-r--   0 user      (1000) user      (1000)     1433 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json
+-rw-rw-r--   0 user      (1000) user      (1000)      979 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json
+-rw-rw-r--   0 user      (1000) user      (1000)     1106 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/quantize.py
+-rw-rw-r--   0 user      (1000) user      (1000)       23 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     4359 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7528 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1255 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/sampling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    39641 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     4691 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.272159 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.280158 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/progress.marks
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.280158 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      871 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     5923 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      359 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      119 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      123 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)      100 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)      224 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)     5152 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o
+-rw-rw-r--   0 user      (1000) user      (1000)     3717 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.284158 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      345 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      121 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)     9816 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o
+-rw-rw-r--   0 user      (1000) user      (1000)     4064 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d
+-rw-rw-r--   0 user      (1000) user      (1000)      577 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1309 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)    10760 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     1292 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/cmake_install.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     1024 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/expected_logits.bin
+-rw-rw-r--   0 user      (1000) user      (1000)     1724 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5039 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c
+-rw-rw-r--   0 user      (1000) user      (1000)  1338429 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin
+-rw-rw-r--   0 user      (1000) user      (1000)  2649149 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-30 08:12:32.000000 langdash-0.0.2.dev2/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1212 2023-05-30 08:27:52.000000 langdash-0.0.2.dev2/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6466 2023-05-30 08:56:47.000000 langdash-0.0.2.dev2/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.176167 langdash-0.0.2.dev2/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.2.dev2/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      624 2023-05-25 22:58:44.000000 langdash-0.0.2.dev2/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6967 2023-05-30 08:14:45.000000 langdash-0.0.2.dev2/langdash/models/rwkvcpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 18:14:56.000000 langdash-0.0.2.dev2/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6066 2023-05-30 08:16:06.000000 langdash-0.0.2.dev2/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      259 2023-05-25 22:58:46.000000 langdash-0.0.2.dev2/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2156 2023-05-27 04:12:41.000000 langdash-0.0.2.dev2/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.176167 langdash-0.0.2.dev2/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.2.dev2/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.2.dev2/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.2.dev2/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.2.dev2/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.180167 langdash-0.0.2.dev2/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-30 15:34:23.000000 langdash-0.0.2.dev2/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    12207 2023-05-30 15:34:23.000000 langdash-0.0.2.dev2/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-30 15:34:23.000000 langdash-0.0.2.dev2/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-30 15:34:23.000000 langdash-0.0.2.dev2/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-30 15:34:23.000000 langdash-0.0.2.dev2/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-30 15:34:23.284158 langdash-0.0.2.dev2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1262 2023-05-30 15:33:03.000000 langdash-0.0.2.dev2/setup.py
```

### Comparing `langdash-0.0.2.dev1/LICENSE.txt` & `langdash-0.0.2.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/PKG-INFO` & `langdash-0.0.2.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.2.dev1
+Version: 0.0.2.dev2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `langdash-0.0.2.dev1/README.md` & `langdash-0.0.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/chains.py` & `langdash-0.0.2.dev2/langdash/chains.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,24 +37,36 @@
     self._ld = ld
     self._args = args
     self._returns = returns
     assert len(nodes) > 0, "at least one node must be given to chain"
     self._nodes = self._preprocess_nodes(nodes)
   
   def cached(self, model: str, **model_kwargs) -> "LDChainCached":
+    """
+    Cache the chain for a specific model
+    
+    Args:
+      model: The model name
+      
+    Returns:
+      The cached chain
+    """
     return LDChainCached(
       model=model,
       model_kwargs=model_kwargs,
       _ld=self._ld,
       _args=self._args,
       _returns=self._returns,
       _nodes=self._nodes,
     )
   
   def argtype(self, name: str) -> Optional[Type]:
+    """
+    Return the type of the argument.
+    """
     try:
       return self._args[name]
     except KeyError:
       return None
   
   def _preprocess_nodes(self, nodes: List[Union["LDNode", str]]) -> List["LDNode"]:
     pp_nodes: List[Optional[LDNode]] = []
@@ -123,14 +135,21 @@
   def _stream(self, session: "LLMGenerationSession", args: LDNodeArgs):
     for node in self._node_pass(session, args):
       if isinstance(node, LDReturns):
         yield RespReturns(key=node._returns)
       yield from node(session, args)
   
   def stream(self, ctx: Union[str, "LLMGenerationSession"], **kwargs):
+    """
+    Stream data generated from the LLM within the specified session.
+    
+    Args:
+        session: The LLM generation session.
+        args: The arguments to pass to generation.
+    """
     return self._stream(session=self._load_session(ctx), **kwargs)
   
   def _call(
     self,
     session: "LLMGenerationSession",
     args: LDNodeArgs = {},
     return_session: bool = False,
@@ -147,14 +166,30 @@
     if return_session:
       if set_global_args:
         session.global_args = args
       return result, session
     return result
   
   def call(self, ctx: Union[str, "LLMGenerationSession"], **kwargs):
+    """
+    Returns data generated from the LLM within the specified session.
+    
+    Args:
+      ctx:
+        The LLM generation session, or the model name.
+      args:
+        The arguments to pass to generation.
+      return_session:
+        Whether or not to return the generation session after generation.
+      set_global_args:
+        Whether or not to set current arguments as global arguments.
+    
+    Returns:
+      The result, or a tuple with (result, session).
+    """
     return self._call(session=self._load_session(ctx), **kwargs)
 
 @dataclass
 class LDChainCacheState:
   state: "LLMState"
   skip_nodes: int
 
@@ -289,34 +324,51 @@
     return super()._stream(session=self._load_session(args=kwargs.get("args")), **kwargs)
   
   def call(self, **kwargs):
     return super()._call(session=self._load_session(args=kwargs.get("args")), **kwargs)
 
 @dataclass
 class LDResult:
+  """
+  Class for storing the results of inference.
+  """
   returns: Dict[str, Any]
   prompt_tokens: int
   completion_tokens: int
   
   def __init__(self):
     self.returns = {}
     self.prompt_tokens = 0
     self.completion_tokens = 0
     
-  def update_results(self, key: str, cast, generator: LDNodeGenerator):
+  def update_results(self, key: str, cast_function, generator: LDNodeGenerator):
+    """
+    Update the results with the given key.
+    
+    Args:
+      key: The key of the language model.
+      cast_function: The function to cast the results.
+      generator: Node generator that runs to get the results.
+    """
     text = ""
     for resp in generator:
       if isinstance(resp, RespInfer):
         text = resp.running_infer
         self.completion_tokens += 1
       else:
         raise NotImplementedError(resp.__class__.__name__)
-    self.returns[key] = cast(text)
+    self.returns[key] = cast_function(text)
   
   def update_stats(self, generator: LDNodeGenerator):
+    """
+    Update the stats of the result, given a node generator.
+    
+    Args:
+      generator: Node generator that runs to get the results.
+    """
     for resp in generator:
       if isinstance(resp, RespInject):
         self.prompt_tokens += resp.tokens_counter
       else:
         continue
 
 class LDNode:
```

### Comparing `langdash-0.0.2.dev1/langdash/classify/token_qa.py` & `langdash-0.0.2.dev2/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeCache.txt` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/CMakeLists.txt` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/FILE_FORMAT.md` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/FILE_FORMAT.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/LICENSE` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/Makefile` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/README.md` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/bin/test_ggml_basics` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/bin/test_ggml_basics`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/cmake_install.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/compile_commands.json` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/compile_commands.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/LICENSE` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/LICENSE`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/Makefile` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/README.md` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.h` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/Makefile` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/src/libggml.a` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/libggml.a`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test0.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test1.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test1.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test2.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test2.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/ggml/tests/test3.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test3.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/librwkv.so` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/librwkv.so`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/generate_completions.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/generate_completions.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/quantize.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/quantize.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv/sampling.py` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv.cpp` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/rwkv.h` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CMakeLists.txt` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/Makefile` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/cmake_install.cmake` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/expected_logits.bin` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/expected_logits.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin` & `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/llm_session.py` & `langdash-0.0.2.dev2/langdash/llm_session.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,18 +7,24 @@
 from langdash.infer import InferArgs
 from langdash.llm import LLM
 
 if TYPE_CHECKING:
   from langdash._langdash import Langdash
 
 class LLMSession:
+  """
+  A session for LLM.
+  """
   def clone(self) -> "LLMSession":
     raise NotImplementedError("clone")
 
 class LLMState:
+  """
+  A state class for a language model.
+  """
   pass
 
 T_LLM = TypeVar('T_LLM', bound=LLM)
 T_LLMState = TypeVar("T_LLMState", bound=LLMState)
 
 class LLMGenerationSession(LLMSession, Generic[T_LLM, T_LLMState]):
   def __init__(self,
@@ -35,20 +41,33 @@
       [] if track_called_chains else None
     )
     self.token_healing = token_healing
     self.global_args = global_args
     self.tokens_counter = 0
     
   def set_state(self, state: Optional[T_LLMState]):
+    """
+    Set the state of the language model.
+
+    Args:
+      state:
+        The state of the language model, or None to clear the state.
+    """
     raise NotImplementedError("set_state")
   
   def clone_state(self) -> T_LLMState:
+    """
+    Clone the current state of the language model.
+    """
     raise NotImplementedError("clone_state")
   
   def clone(self) -> "LLMGenerationSession":
+    """
+    Clone the current session.
+    """
     session = self.__class__(
       llm=self.llm,
       ld=self._ld,
       default_infer_args=self.default_infer_args,
       track_called_chains=False,
       global_args=copy.copy(self.global_args)
     )
@@ -63,27 +82,50 @@
                            tokens_used: int):
     if self.called_chains is None:
       pass
     else:
       self.called_chains.append(CalledChain(node=node, args=args, tokens_used=tokens_used))
   
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
+    """
+    Tokenize the given text into a list of tokens.
+
+    Args:
+      text: The text to tokenize.
+      add_special_tokens: Whether to add special tokens to the output.
+
+    Returns:
+      The list of tokens.
+    """
     raise NotImplementedError("tokenize")
   
   def next_token_probs(self) -> Sequence[float]:
+    """
+    Returns the probabilities for next token.
+    """
     raise NotImplementedError("next_token_probs")
   
   def _infer(self,
             end: Optional[Union[str, int]],
             args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
     raise NotImplementedError("_infer")
 
   def infer(self,
             end: Optional[Union[str, int]],
             args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
+    """
+    Infer the next token from the input sequence.
+
+    Args:
+      end: The end of the input sequence.
+      args: Additional arguments to pass to the inference function.
+        
+    Returns:
+      Inference response
+    """
     if not args:
       args = self.default_infer_args
     yield from self._infer(end, args)
     
   def inject(self, text: str, add_special_tokens: bool = False) -> int:
     raise NotImplementedError("inject")
 
@@ -142,21 +184,31 @@
         num_toks += 1
       for tokid in input_ids:
         self._logits = self._eval(tokid)
       num_toks += len(input_ids)
 
     return num_toks
 
-T_Emb = TypeVar('T_Emb')
+T_Embedding = TypeVar('T_Embedding')
 
-class LLMEmbeddingSession(LLMSession, Generic[T_LLM, T_Emb]):
+class LLMEmbeddingSession(LLMSession, Generic[T_LLM, T_Embedding]):
   def __init__(self,
                llm: T_LLM,
                ld: "Langdash"):
     self._ld = ld
     self.llm = llm
     
   def embedding_size(self) -> int:
+    """
+    Returns the embedding size of the model.
+    """
     raise NotImplementedError("embedding_size")
     
-  def infer(self, text: str) -> T_Emb:
+  def infer(self, text: str) -> T_Embedding:
+    """
+    Infer the embedding of a text.
+    Args:
+      text: The text to be embedded.
+    Returns:
+      The embedding of the text.
+    """
     raise NotImplementedError("infer")
```

### Comparing `langdash-0.0.2.dev1/langdash/models/mock.py` & `langdash-0.0.2.dev2/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/models/rwkvcpp.py` & `langdash-0.0.2.dev2/langdash/models/transformers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,193 +1,182 @@
-from typing import Generator, List, Optional, Tuple, Union
+from typing import Generator, List, Optional, Tuple, Union, Any
 from math import inf
 from dataclasses import dataclass
 import copy
 
 from langdash.response import RespInfer
 from langdash.llm import LLM
 from langdash.llm_session import LLMGenerationSessionForRawText, LLMState
 from langdash.infer import InferArgs
 import langdash.sampling as sampling
 
-import os
-import sys
+import transformers
 import torch
-import pathlib
-
-def _load_rwkv_import():
-  import langdash
-  import subprocess
-  import shutil
-  
-  rwkv_cpp_folder = os.path.join(os.path.dirname(langdash.__file__), "extern/rwkv.cpp")
-  if not os.path.isdir(rwkv_cpp_folder):
-    print("rwkv.cpp isn't installed, clone and install? (requires git, cmake)")
-    do_install = input("Type 'y' (without quotes) to install: ") == 'y'
-    if not do_install:
-      raise ImportError("rwkv.cpp is not installed")
-    
-    os.makedirs(rwkv_cpp_folder, exist_ok=True)
-    git = shutil.which("git")
-    if git == None:
-      raise ImportError("git is needed for compiling rwkv.cpp")
-    subprocess.check_call(
-      [git, "clone", "--recursive", "https://github.com/saharNooby/rwkv.cpp", rwkv_cpp_folder],
-      cwd=rwkv_cpp_folder
-    )
-    
-  if 'win32' in sys.platform or 'cygwin' in sys.platform:
-    file_name = 'rwkv.dll'
-  elif 'darwin' in sys.platform:
-    file_name = 'librwkv.dylib'
-  else:
-    file_name = 'librwkv.so'
-  if not os.path.isfile(os.path.join(rwkv_cpp_folder, file_name)):
-    cmake = shutil.which("cmake")
-    if cmake == None:
-      raise ImportError("cmake is needed for compiling rwkv.cpp")
-    subprocess.check_call(
-      [cmake, "."],
-      cwd=rwkv_cpp_folder
-    )
-    subprocess.check_call(
-      [cmake, "--build", ".", "--config", "Release"],
-      cwd=rwkv_cpp_folder
-    )
-  sys.path.append(os.path.join(rwkv_cpp_folder, "rwkv"))
-
-_load_rwkv_import()
-
-import tokenizers # type: ignore
-import rwkv_cpp_model # type: ignore
-import rwkv_cpp_shared_library # type: ignore
 
 @dataclass
-class RWKVCppState(LLMState):
+class TransformersState(LLMState):
   _logits: Optional[torch.Tensor] = None
-  _state: Optional[torch.Tensor] = None
+  _past_key_values: Any = None
   _next_token: Optional[Tuple[int, str]] = None
 
-class RWKVCppSession(LLMGenerationSessionForRawText["RWKVCppModel", RWKVCppState, torch.Tensor]):
-  _rwkv: rwkv_cpp_model.RWKVModel
-  _tokenizer: tokenizers.Tokenizer
+class TransformersSession(LLMGenerationSessionForRawText["TransformersModel", TransformersState, torch.Tensor]):
+  _next_token: Optional[Tuple[int, str]]
   
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
     
-    def load_model(llm: RWKVCppModel):
-      model = rwkv_cpp_model.RWKVModel(
-        rwkv_cpp_shared_library.load_rwkv_shared_library(),
-        llm._model_path
-      )
-      tokenizer = tokenizers.Tokenizer.from_file(llm._tokenizer_path)
+    def load_model(llm: TransformersModel):
+      model = transformers.AutoModelForCausalLM.from_pretrained(llm._model_name)
+      tokenizer = transformers.AutoTokenizer.from_pretrained(llm._tokenizer_name)
       return model, tokenizer
       
-    self._rwkv, self._tokenizer = self._ld.get_model_internal(self.llm, load_model)
+    self._model, self._tokenizer = self._ld.get_model_internal(self.llm, load_model)
     
-    self._logits, self._state = None, None
+    if isinstance(
+      self._tokenizer,
+      Union[
+        transformers.GPT2Tokenizer,
+        transformers.GPT2TokenizerFast
+      ]
+    ):
+      self._space_token = "\u0120"
+      self._buffered_token_head = set(
+        v for k, v in self._tokenizer.get_vocab().items() if "\u0122" in k
+      )
+    else:
+      self._space_token = " "
+      self._buffered_token_head = set()
+
+    self._logits = None
+    self._past_key_values = None
     self._next_token = None
   
-  def _eval(self, tokid: int) -> torch.Tensor:
-    self._logits, self._state = self._rwkv.eval(tokid, self._state)
-    return self._logits
+  def _heal_token(self, tok_a: int, tok_b: int) -> str:
+    return self._tokenizer.decode([tok_a, tok_b])
   
-  def _token_to_str(self, tokid: int) -> str:
-    return self._tokenizer.id_to_token(tokid)
-  
-  def set_state(self, state: Optional[RWKVCppState]):
+  def set_state(self, state: Optional[TransformersState]):
     if state is None:
-      self._logits, self._state = None, None
+      self._logits = None
+      self._past_key_values = None
       self._next_token = None
     else:
       self._logits = copy.deepcopy(state._logits)
-      self._state = copy.deepcopy(state._state)
+      self._past_key_values = copy.deepcopy(state._past_key_values)
       self._next_token = state._next_token
     
-  def clone_state(self) -> RWKVCppState:
-    return RWKVCppState(
+  def clone_state(self) -> TransformersState:
+    return TransformersState(
       _logits = copy.deepcopy(self._logits),
-      _state = copy.deepcopy(self._state),
+      _past_key_values = copy.deepcopy(self._past_key_values),
       _next_token = self._next_token,
     )
-
+  
+  def _eval(self, tokid: int):
+    outputs = self._model.forward(
+      torch.IntTensor([tokid]),
+      past_key_values=self._past_key_values,
+      use_cache=True
+    )
+    self._past_key_values = outputs.past_key_values
+    return outputs.logits[-1]
+  
+  def _token_to_str(self, tokid: int) -> str:
+    return self._tokenizer.convert_ids_to_tokens(tokid)
+  
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
-    return self._tokenizer.encode(text, add_special_tokens=add_special_tokens).ids
+    return list(self._tokenizer.encode(text, add_special_tokens=add_special_tokens))
   
   def next_token_probs(self) -> torch.Tensor:
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
-      logits, _ = self._rwkv.eval(self._next_token[0], self._state)
+      logits = self._model.forward(
+        torch.IntTensor([self._next_token[0]]),
+        past_key_values=self._past_key_values,
+        use_cache=True
+      )._logits[-1]
     return torch.nn.functional.softmax(logits, dim=-1)
-
+  
   def _infer(self,
             end: Optional[Union[str, int]],
             args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
     generated = ""
     ctx: List[int] = []
     buffered_tokens: List[int] = []
     stops_at_eot = (
       (isinstance(end, str) and len(end) == 0) or
-      (isinstance(end, int) and end == 0)
+      (isinstance(end, int) and end == self._tokenizer.eos_token_id)
     )
     
     for i in range(args.max_new_tokens):
-      strip_left = 0
+      postprocess_fn = None
       
       if i == 0 and self._next_token is not None:
         _, tokstr = self._next_token
-        for key, value in self._tokenizer.get_vocab().items():
-          if not key.startswith(tokstr):
-            self._logits[value] = -inf
-        strip_left = len(tokstr)
+        if tokstr == " ":
+          for key, value in self._tokenizer.get_vocab().items():
+            #https://github.com/openai/gpt-2/issues/80
+            #starts with 0x120
+            if key.startswith(self._space_token):
+              self._logits[value] = -inf
+          postprocess_fn = lambda x: " " + x
+        else:
+          for key, value in self._tokenizer.get_vocab().items():
+            if not key.startswith(tokstr):
+              self._logits[value] = -inf
+          _tokstr_len = len(tokstr)
+          postprocess_fn = lambda x: x[_tokstr_len:]
+        # self._next_token = None
       
       if not stops_at_eot: # no early endoftext
         self._logits[0] = -inf
-        
+      
       tokid = sampling.sample(self._logits, args, ctx)
       ctx.append(tokid)
       
-      if tokid == end: # implies end is int
-        break
-      
-      tokstr = self._tokenizer.decode([tokid])
-      
-      if stops_at_eot and tokid == 0:
+      if stops_at_eot and tokid == self._tokenizer.eos_token_id:
         break
-      elif "\ufffd" in tokstr:
+      elif tokid in self._buffered_token_head:
         buffered_tokens.append(tokid)
-        self._next_token = (tokid, "")
       else:
         if buffered_tokens:
-          tokstr = self._tokenizer.decode(buffered_tokens)
-          tokstr += self._tokenizer.decode([tokid])
-          buffered_tokens.clear()
+          tokstr = self._tokenizer.decode(buffered_tokens + [tokid])
+          buffered_tokens = []
         else:
-          if strip_left:
-            tokstr = tokstr[strip_left:]
-      
+          tokstr = self._tokenizer.decode([tokid])
+        
+        if postprocess_fn is not None:
+          tokstr = postprocess_fn(tokstr)
+        
         self._next_token = (tokid, tokstr)
         
         generated += tokstr
         if isinstance(end, str) and end and generated.endswith(end):
           generated = generated[:-len(end)]
           break
-        
+      
         yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
-        
-      self._logits, self._state = self._rwkv.eval(tokid, self._state)
+      
+      self._logits = self._eval(tokid)
     
     yield RespInfer(tokid=0, tokstr="", running_infer=generated)
 
-class RWKVCppModel(LLM[RWKVCppSession]):
-  Session = RWKVCppSession
+class TransformersModel(LLM[TransformersSession]):
+  Session = TransformersSession
   
-  def __init__(self, model_path: str, tokenizer_path: Optional[str] = None):
-    self._model_path = model_path
-    if tokenizer_path is None:
-      self._tokenizer_path = str(pathlib.Path(os.path.abspath(model_path)).parent / '20B_tokenizer.json')
-    else:
-      self._tokenizer_path = tokenizer_path
-      
+  def __init__(self, model_name: str, tokenizer_name: Optional[str] = None):
+    """
+    Creates a template for a language model powered by the transformers library.
+    
+    Args:
+      model_name (str):
+        The name of the model.
+      tokenizer_name (str):
+        The name of the tokenizer.
+        If None, the model_name will be used to detect the tokenizer.
+    """
+    if tokenizer_name is None:
+      tokenizer_name = model_name
+    self._model_name = model_name
+    self._tokenizer_name = tokenizer_name
```

### Comparing `langdash-0.0.2.dev1/langdash/models/sentence_transformers.py` & `langdash-0.0.2.dev2/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/sampling.py` & `langdash-0.0.2.dev2/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/search/embedding_search.py` & `langdash-0.0.2.dev2/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash/search/multichoice_search.py` & `langdash-0.0.2.dev2/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/langdash.egg-info/PKG-INFO` & `langdash-0.0.2.dev2/langdash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.2.dev1
+Version: 0.0.2.dev2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `langdash-0.0.2.dev1/langdash.egg-info/SOURCES.txt` & `langdash-0.0.2.dev2/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev1/setup.py` & `langdash-0.0.2.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='langdash',
-    version='0.0.2.dev1',
+    version='0.0.2.dev2',
     description='A simple library for interfacing with language models.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Nana Mochizuki',
     author_email='nana@mysymphony.jp.net',
     url='https://git.mysymphony.jp.net/nana/langdash',
     classifiers=[
```

