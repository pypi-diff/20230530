# Comparing `tmp/pyopal-0.2.0.tar.gz` & `tmp/pyopal-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopal-0.2.0.tar", last modified: Mon Oct 17 16:10:24 2022, max compression
+gzip compressed data, was "pyopal-0.3.0.tar", last modified: Tue May 30 12:36:00 2023, max compression
```

## Comparing `pyopal-0.2.0.tar` & `pyopal-0.3.0.tar`

### file list

```diff
@@ -1,101 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.627115 pyopal-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-10-17 16:10:01.000000 pyopal-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-10-17 16:10:01.000000 pyopal-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-10-17 16:10:01.000000 pyopal-0.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      684 2022-10-17 16:10:01.000000 pyopal-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10099 2022-10-17 16:10:24.627115 pyopal-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8413 2022-10-17 16:10:01.000000 pyopal-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/include/
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-10-17 16:10:01.000000 pyopal-0.2.0/include/_unicode.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/include/cpu_features/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:01.000000 pyopal-0.2.0/include/cpu_features/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-10-17 16:10:01.000000 pyopal-0.2.0/include/cpu_features/aarch64.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-10-17 16:10:01.000000 pyopal-0.2.0/include/cpu_features/arm.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-10-17 16:10:01.000000 pyopal-0.2.0/include/cpu_features/x86.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/include/opal/
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-10-17 16:10:01.000000 pyopal-0.2.0/include/opal/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-10-17 16:10:01.000000 pyopal-0.2.0/include/opal/score_matrix.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/pyopal/
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3791 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_opal.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    37018 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_opal.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_opal_avx2.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_opal_avx2.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_opal_neon.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_opal_neon.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_opal_sse2.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_opal_sse2.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_opal_sse4.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_opal_sse4.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/pyopal/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3397 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (121)     3242 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3121 2022-10-17 16:10:01.000000 pyopal-0.2.0/pyopal/tests/test_search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/pyopal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10099 2022-10-17 16:10:24.000000 pyopal-0.2.0/pyopal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-10-17 16:10:24.000000 pyopal-0.2.0/pyopal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 16:10:24.000000 pyopal-0.2.0/pyopal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 16:10:24.000000 pyopal-0.2.0/pyopal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-17 16:10:24.000000 pyopal-0.2.0/pyopal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-10-17 16:10:24.000000 pyopal-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2900 2022-10-17 16:10:24.627115 pyopal-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    27557 2022-10-17 16:10:01.000000 pyopal-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.615115 pyopal-0.2.0/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/vendor/cpu_features/
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    12876 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8068 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/vendor/cpu_features/ci/
--rw-r--r--   0 runner    (1001) docker     (121)     2896 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/ci/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/vendor/cpu_features/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/cmake/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/vendor/cpu_features/include/
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/cpu_features_cache_info.h
--rw-r--r--   0 runner    (1001) docker     (121)     7081 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/cpu_features_macros.h
--rw-r--r--   0 runner    (1001) docker     (121)     5451 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/cpuinfo_aarch64.h
--rw-r--r--   0 runner    (1001) docker     (121)     3723 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/cpuinfo_arm.h
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/cpuinfo_mips.h
--rw-r--r--   0 runner    (1001) docker     (121)     4493 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/cpuinfo_ppc.h
--rw-r--r--   0 runner    (1001) docker     (121)     6650 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/cpuinfo_x86.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/vendor/cpu_features/include/internal/
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/internal/bit_utils.h
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/internal/cpuid_x86.h
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/internal/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (121)     7085 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/internal/hwcaps.h
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/internal/stack_line_reader.h
--rw-r--r--   0 runner    (1001) docker     (121)     4127 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/include/internal/string_view.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.619115 pyopal-0.2.0/vendor/cpu_features/ndk_compat/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/ndk_compat/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.623115 pyopal-0.2.0/vendor/cpu_features/src/
--rw-r--r--   0 runner    (1001) docker     (121)      736 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/copy.inl
--rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/define_introspection.inl
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/define_introspection_and_hwcaps.inl
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/equals.inl
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/filesystem.c
--rw-r--r--   0 runner    (1001) docker     (121)     5177 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/hwcaps.c
--rw-r--r--   0 runner    (1001) docker     (121)     7686 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/impl_aarch64_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (121)     9080 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/impl_arm_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/impl_mips_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (121)     7876 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/impl_ppc_linux.c
--rw-r--r--   0 runner    (1001) docker     (121)    76257 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/impl_x86__base_implementation.inl
--rw-r--r--   0 runner    (1001) docker     (121)     2660 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/impl_x86_freebsd.c
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/impl_x86_linux_or_android.c
--rw-r--r--   0 runner    (1001) docker     (121)     2173 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/impl_x86_macos.c
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/impl_x86_windows.c
--rw-r--r--   0 runner    (1001) docker     (121)     4136 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/stack_line_reader.c
--rw-r--r--   0 runner    (1001) docker     (121)     6603 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/string_view.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.623115 pyopal-0.2.0/vendor/cpu_features/src/utils/
--rw-r--r--   0 runner    (1001) docker     (121)    13848 2022-10-17 16:10:06.000000 pyopal-0.2.0/vendor/cpu_features/src/utils/list_cpu_features.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.623115 pyopal-0.2.0/vendor/opal/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-10-17 16:10:07.000000 pyopal-0.2.0/vendor/opal/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4336 2022-10-17 16:10:07.000000 pyopal-0.2.0/vendor/opal/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 16:10:24.623115 pyopal-0.2.0/vendor/opal/src/
--rw-r--r--   0 runner    (1001) docker     (121)     3943 2022-10-17 16:10:07.000000 pyopal-0.2.0/vendor/opal/src/ScoreMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-10-17 16:10:07.000000 pyopal-0.2.0/vendor/opal/src/ScoreMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    85988 2022-10-17 16:10:07.000000 pyopal-0.2.0/vendor/opal/src/opal.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     8325 2022-10-17 16:10:07.000000 pyopal-0.2.0/vendor/opal/src/opal.h
--rw-r--r--   0 runner    (1001) docker     (121)    13260 2022-10-17 16:10:07.000000 pyopal-0.2.0/vendor/opal/src/opal_aligner.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    15339 2022-10-17 16:10:07.000000 pyopal-0.2.0/vendor/opal/src/test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-30 12:35:44.000000 pyopal-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-30 12:35:44.000000 pyopal-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-30 12:35:44.000000 pyopal-0.3.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 12:35:44.000000 pyopal-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-30 12:36:00.510659 pyopal-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-30 12:35:44.000000 pyopal-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.506659 pyopal-0.3.0/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/_unicode.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/include/cpu_features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/cpu_features/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/cpu_features/aarch64.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/cpu_features/arm.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/cpu_features/x86.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/include/opal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/opal/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-30 12:35:44.000000 pyopal-0.3.0/include/opal/score_matrix.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/pyopal/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39490 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_avx2.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_avx2.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_neon.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_neon.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_sse2.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_sse2.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_sse4.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_opal_sse4.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/pyopal/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-30 12:35:44.000000 pyopal-0.3.0/pyopal/tests/test_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/pyopal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyopal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 12:36:00.000000 pyopal-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-30 12:36:00.510659 pyopal-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    18986 2023-05-30 12:35:44.000000 pyopal-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.506659 pyopal-0.3.0/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/vendor/opal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:36:00.510659 pyopal-0.3.0/vendor/opal/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/ScoreMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/ScoreMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    86020 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/opal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/opal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/opal_aligner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15339 2023-05-30 12:35:45.000000 pyopal-0.3.0/vendor/opal/src/test.cpp
```

### Comparing `pyopal-0.2.0/CONTRIBUTING.md` & `pyopal-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/COPYING` & `pyopal-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/PKG-INFO` & `pyopal-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 Metadata-Version: 2.1
 Name: pyopal
-Version: 0.2.0
+Version: 0.3.0
 Summary: Cython bindings and Python interface to Opal, a SIMD-accelerated pairwise aligner.
 Home-page: https://github.com/althonos/pyopal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Documentation, https://pyopal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyopal/issues
 Project-URL: Changelog, https://github.com/althonos/pyopal/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://codecov.io/gh/althonos/pyopal/
 Project-URL: Builds, https://github.com/althonos/pyopal/actions
 Project-URL: PyPI, https://pypi.org/project/pyopal
 Keywords: bioinformatics,pairwise,sequence,alignment,opal
 Platform: any
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # 🐍🌈🪨 PyOpal [![Stars](https://img.shields.io/github/stars/althonos/pyopal.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/pyopal/stargazers)
 
 *[Cython](https://cython.org/) bindings and Python interface to [Opal](https://github.com/Martinsos/opal), a SIMD-accelerated database search aligner.*
 
-[![Actions](https://img.shields.io/github/workflow/status/althonos/pyopal/Test/main?logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pyopal/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/althonos/pyopal/test.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pyopal/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/pyopal?style=flat-square&maxAge=3600&logo=codecov)](https://codecov.io/gh/althonos/pyopal/)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/mit/)
 [![PyPI](https://img.shields.io/pypi/v/pyopal.svg?style=flat-square&maxAge=3600&logo=PyPI)](https://pypi.org/project/pyopal)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/pyopal?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/pyopal)
 [![AUR](https://img.shields.io/aur/version/python-pyopal?logo=archlinux&style=flat-square&maxAge=3600)](https://aur.archlinux.org/packages/python-pyopal)
 [![Wheel](https://img.shields.io/pypi/wheel/pyopal.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/pyopal/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pyopal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pyopal/#files)
```

### Comparing `pyopal-0.2.0/README.md` & `pyopal-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # 🐍🌈🪨 PyOpal [![Stars](https://img.shields.io/github/stars/althonos/pyopal.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/pyopal/stargazers)
 
 *[Cython](https://cython.org/) bindings and Python interface to [Opal](https://github.com/Martinsos/opal), a SIMD-accelerated database search aligner.*
 
-[![Actions](https://img.shields.io/github/workflow/status/althonos/pyopal/Test/main?logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pyopal/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/althonos/pyopal/test.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pyopal/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/pyopal?style=flat-square&maxAge=3600&logo=codecov)](https://codecov.io/gh/althonos/pyopal/)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/mit/)
 [![PyPI](https://img.shields.io/pypi/v/pyopal.svg?style=flat-square&maxAge=3600&logo=PyPI)](https://pypi.org/project/pyopal)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/pyopal?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/pyopal)
 [![AUR](https://img.shields.io/aur/version/python-pyopal?logo=archlinux&style=flat-square&maxAge=3600)](https://aur.archlinux.org/packages/python-pyopal)
 [![Wheel](https://img.shields.io/pypi/wheel/pyopal.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/pyopal/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pyopal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pyopal/#files)
```

### Comparing `pyopal-0.2.0/include/_unicode.pxd` & `pyopal-0.3.0/include/_unicode.pxd`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/include/cpu_features/aarch64.pxd` & `pyopal-0.3.0/include/cpu_features/aarch64.pxd`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/include/cpu_features/arm.pxd` & `pyopal-0.3.0/include/cpu_features/arm.pxd`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/include/opal/__init__.pxd` & `pyopal-0.3.0/include/opal/__init__.pxd`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/pyopal/__init__.py` & `pyopal-0.3.0/pyopal/__init__.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/pyopal/_opal.pyi` & `pyopal-0.3.0/pyopal/_opal.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,16 @@
         self, sequences: typing.Iterable[typing.Union[str, bytes, bytearray]]
     ) -> None: ...
     def append(self, sequence: typing.Union[str, bytes, bytearray]) -> None: ...
     def reverse(self) -> None: ...
     def insert(
         self, index: int, sequence: typing.Union[str, bytes, bytearray]
     ) -> None: ...
+    def mask(self, bitmask: typing.Sequence[bool]) -> Database: ...
+    def extract(self, indices: typing.Sequence[int]) -> Database: ...
     @typing.overload
     def search(
         self,
         sequence: typing.Union[str, bytes, bytearray],
         *,
         gap_open: int = 3,
         gap_extend: int = 1,
```

### Comparing `pyopal-0.2.0/pyopal/_opal.pyx` & `pyopal-0.3.0/pyopal/_opal.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
       PLoS One. 2015;10(12):e0145857. Published 2015 Dec 31.
       :doi:`10.1371/journal.pone.0145857`.
 
 """
 
 # --- C imports ----------------------------------------------------------------
 
-from libc.string cimport memset
+from libc.string cimport memset, memcpy
 from libc.limits cimport UCHAR_MAX
 from libcpp.string cimport string
 from libcpp.vector cimport vector
 
 from cpython cimport Py_INCREF
 from cpython.buffer cimport PyBUF_FORMAT
 from cpython.list cimport PyList_New, PyList_SET_ITEM
@@ -97,42 +97,30 @@
     'D': opal.OPAL_ALIGN_DEL,
     'I': opal.OPAL_ALIGN_INS,
     'X': opal.OPAL_ALIGN_MISMATCH,
 }
 
 # --- Runtime CPU detection ----------------------------------------------------
 
-_TARGET_CPU           = TARGET_CPU
-_SSE2_RUNTIME_SUPPORT = False
-_SSE2_BUILD_SUPPORT   = False
-_SSE4_RUNTIME_SUPPORT = False
-_SSE4_BUILD_SUPPORT   = False
-_AVX2_RUNTIME_SUPPORT = False
-_AVX2_BUILD_SUPPORT   = False
-_NEON_RUNTIME_SUPPORT = False
-_NEON_BUILD_SUPPORT   = False
-
-IF TARGET_CPU == "x86" and TARGET_SYSTEM in ("freebsd", "linux_or_android", "macos", "windows"):
-    from cpu_features.x86 cimport GetX86Info, X86Info
-    cdef X86Info cpu_info = GetX86Info()
-    _SSE2_BUILD_SUPPORT   = SSE2_BUILD_SUPPORT
-    _SSE2_RUNTIME_SUPPORT = SSE2_BUILD_SUPPORT and cpu_info.features.sse2 != 0
-    _SSE4_BUILD_SUPPORT   = SSE4_BUILD_SUPPORT
-    _SSE4_RUNTIME_SUPPORT = SSE4_BUILD_SUPPORT and cpu_info.features.sse4_1 != 0
-    _AVX2_BUILD_SUPPORT   = AVX2_BUILD_SUPPORT
-    _AVX2_RUNTIME_SUPPORT = AVX2_BUILD_SUPPORT and cpu_info.features.avx2 != 0
-ELIF TARGET_CPU == "arm":
-    from cpu_features.arm cimport GetArmInfo, ArmInfo
-    cdef ArmInfo arm_info = GetArmInfo()
-    _NEON_BUILD_SUPPORT   = NEON_BUILD_SUPPORT
-    _NEON_RUNTIME_SUPPORT = NEON_BUILD_SUPPORT and arm_info.features.neon != 0
-ELIF TARGET_CPU == "aarch64":
-    _NEON_BUILD_SUPPORT   = NEON_BUILD_SUPPORT
-    _NEON_RUNTIME_SUPPORT = NEON_BUILD_SUPPORT # always runtime support on Aarch64
+import archspec.cpu
 
+_HOST_CPU             = archspec.cpu.host()
+_SSE2_BUILD_SUPPORT   = SSE2_BUILD_SUPPORT
+_SSE4_BUILD_SUPPORT   = SSE4_BUILD_SUPPORT
+_AVX2_BUILD_SUPPORT   = AVX2_BUILD_SUPPORT
+_NEON_BUILD_SUPPORT   = NEON_BUILD_SUPPORT
+_SSE2_RUNTIME_SUPPORT = SSE2_BUILD_SUPPORT and "sse2" in _HOST_CPU.features
+_SSE4_RUNTIME_SUPPORT = SSE4_BUILD_SUPPORT and "sse4_1" in _HOST_CPU.features
+_AVX2_RUNTIME_SUPPORT = AVX2_BUILD_SUPPORT and "avx2" in _HOST_CPU.features
+_NEON_RUNTIME_SUPPORT = NEON_BUILD_SUPPORT and "neon" in _HOST_CPU.features
+
+# NOTE(@althonos): NEON is always supported on Aarch64 so we should only check
+#                  that the extension was built with NEON support.
+if _HOST_CPU.family.name == "aarch64":
+    _NEON_RUNTIME_SUPPORT = NEON_BUILD_SUPPORT
 
 # --- Type definitions ---------------------------------------------------------
 
 ctypedef unsigned char     digit_t
 ctypedef digit_t*          seq_t
 ctypedef OpalSearchResult* OpalSearchResult_ptr
 
@@ -649,31 +637,31 @@
         return (<float> matches) / (<float> (matches + mismatches))
 
     cpdef float coverage(self, str reference="query"):
         """coverage(self, reference="query")\n--
 
         Compute the coverage of the alignment.
 
-        Argument:
+        Arguments:
             reference (`str`): The reference sequence to take to compute
                 the coverage: either ``query`` or ``target``.
 
         Returns:
-            `float`: The coverage of the alignment against the 
+            `float`: The coverage of the alignment against the
             reference, as a fraction (between *0* and *1*).
 
         Example:
-            If we align the test sequences from the Opal dataset with 
+            If we align the test sequences from the Opal dataset with
             Needleman-Wunsch, we get the following alignment::
 
                 T: AACCGCTG (0 - 7)
                 Q: -ACCTC-G (0 - 5)
 
             The query coverage will be 100%, but the target coverage will
-            only be 87.5%, since the first letter of the target is not 
+            only be 87.5%, since the first letter of the target is not
             covered by the alignment::
 
                 >>> db = Database(["AACCGCTG"])
                 >>> hit = db.search("ACCTCG", mode="full", algorithm="nw")[0]
                 >>> hit.coverage("query")
                 1.0
                 >>> hit.coverage("target")
@@ -729,30 +717,48 @@
 
     """
 
     cdef readonly SharedMutex   lock
     cdef readonly ScoreMatrix   score_matrix
     cdef          vector[seq_t] _sequences
     cdef          vector[int]   _lengths
+    cdef          searchfn_t    _search
 
     # --- Magic methods --------------------------------------------------------
 
     def __cinit__(self):
         self.lock       = SharedMutex()
         self._sequences = vector[seq_t]()
         self._lengths   = vector[int]()
+        self._search    = NULL
 
     def __init__(self, object sequences=(), ScoreMatrix score_matrix=None):
         # reset the collection is `__init__` is called more than once
         self.clear()
         # record the score matrix
         self.score_matrix = score_matrix or ScoreMatrix.aa()
         # add the sequences to the database
         self.extend(sequences)
 
+        # Select the best available SIMD backend
+        IF SSE2_BUILD_SUPPORT:
+            if _SSE2_RUNTIME_SUPPORT:
+                self._search = opalSearchDatabaseSSE2
+        IF SSE4_BUILD_SUPPORT:
+            if _SSE4_RUNTIME_SUPPORT:
+                self._search = opalSearchDatabaseSSE4
+        IF AVX2_BUILD_SUPPORT:
+            if _AVX2_RUNTIME_SUPPORT:
+                self._search = opalSearchDatabaseAVX2
+        IF NEON_BUILD_SUPPORT:
+            if _NEON_RUNTIME_SUPPORT:
+                self._search = opalSearchDatabaseNEON
+        if self._search is NULL:
+            raise RuntimeError("No supported SIMD backend available")
+
     def __dealloc__(self):
         cdef size_t i
         for i in range(self._sequences.size()):
             PyMem_Free(self._sequences[i])
 
     def __reduce__(self):
         return (type(self), ((), self.score_matrix), None, iter(self))
@@ -948,14 +954,106 @@
                 index_ = size
 
             encode(sequence, self.score_matrix._ahash, &encoded, &length)
             self._sequences.insert(self._sequences.begin() + index_, encoded)
             self._lengths.insert(self._lengths.begin() + index_, length)
 
 
+    # --- Subset ---------------------------------------------------------------
+
+    cpdef Database mask(self, object bitmask):
+        """mask(self, bitmask)\n--
+
+        Extract a subset of the database where the bitmask is `True`.
+
+        Arguments:
+            bitmask (`collections.abc.Sequence` of `bool`): A sequence of 
+                `bool` objects with the same length as the database.
+
+        Raises:
+            `IndexError`: When the bitmask has a different dimension.
+
+        Example:
+            >>> db = pyopal.Database(['AAAA', 'CCCC', 'KKKK', 'FFFF'])
+            >>> list(db.mask([True, False, False, True]))
+            ['AAAA', 'FFFF']
+
+        .. versionadded:: 0.3.0
+
+        """
+        cdef ssize_t  i
+        cdef int      length
+        cdef seq_t    seq
+        cdef Database subdb
+
+        if len(bitmask) != len(self):
+            raise IndexError(bitmask)
+
+        subdb = Database.__new__(Database)
+        subdb.score_matrix = self.score_matrix
+        subdb._search = self._search
+
+        for i, b in enumerate(bitmask):
+            if b:
+                length = self._lengths[i]
+                seq = <seq_t> PyMem_Malloc(length * sizeof(digit_t))
+                if seq is NULL:
+                    raise MemoryError("Failed to allocate sequence data")
+                with nogil:
+                    memcpy(seq, self._sequences[i], length * sizeof(digit_t))
+                    subdb._sequences.push_back(seq)
+                    subdb._lengths.push_back(length)
+
+        return subdb
+
+    cpdef Database extract(self, object indices):
+        """extract(self, indices)\n--
+
+        Extract a subset of the database using the given indices.
+
+        Arguments:
+            indices (`collections.abc.Sequence` of `int`): A sequence of 
+                `int` objects to use to index the database.
+
+        Raises:
+            `IndexError`: When ``indices`` contains an invalid index.
+
+        Example:
+            >>> db = pyopal.Database(['AAAA', 'CCCC', 'KKKK', 'FFFF'])
+            >>> list(db.extract([2, 0]))
+            ['KKKK', 'AAAA']
+
+        .. versionadded:: 0.3.0
+
+        """
+        cdef ssize_t  index
+        cdef int      length
+        cdef seq_t    seq
+        cdef Database subdb
+
+        subdb = Database.__new__(Database)
+        subdb.score_matrix = self.score_matrix
+        subdb._search = self._search
+        subdb._sequences.reserve(len(indices))
+        subdb._lengths.reserve(len(indices))
+
+        for index in indices:
+            if index < 0 or index >= len(self):
+                raise IndexError(index)
+            length = self._lengths[index]
+            seq = <seq_t> PyMem_Malloc(length * sizeof(digit_t))
+            if seq is NULL:
+                raise MemoryError("Failed to allocate sequence data")
+            with nogil:
+                memcpy(seq, self._sequences[index], length * sizeof(digit_t))
+                subdb._sequences.push_back(seq)
+                subdb._lengths.push_back(length)
+
+        return subdb
+
     # --- Opal search ----------------------------------------------------------
 
     def search(
         self,
         object sequence,
         *,
         int gap_open = 3,
@@ -1009,40 +1107,40 @@
         Raises:
             `ValueError`: When ``sequence`` contains invalid characters
                 with respect to the alphabet of the database scoring
                 matrix.
 
         """
         assert self.score_matrix is not None
+        assert self._search is not NULL
 
         cdef int                          _mode
         cdef int                          _overflow
         cdef int                          _algo
         cdef size_t                       i
         cdef int                          retcode
         cdef int                          length
         cdef ScoreResult                  result
         cdef FullResult                   full_result
         cdef type                         result_type
         cdef list                         results
         cdef vector[OpalSearchResult_ptr] results_raw
         cdef size_t                       size
         cdef seq_t                        query       = NULL
-        cdef searchfn_t                   searchfn    = NULL
 
         # validate parameters
         if mode in _OPAL_SEARCH_MODES:
             _mode = _OPAL_SEARCH_MODES[mode]
             result_type = _OPAL_SEARCH_RESULTS[mode]
         else:
             raise ValueError(f"Invalid search mode: {mode!r}")
         if overflow in _OPAL_OVERFLOW_MODES:
             _overflow = _OPAL_OVERFLOW_MODES[overflow]
         else:
-            raise ValueError(f"Invalid overflow mode: {mode!r}")
+            raise ValueError(f"Invalid overflow mode: {overflow!r}")
         if algorithm in _OPAL_ALGORITHMS:
             _algo = _OPAL_ALGORITHMS[algorithm]
         else:
             raise ValueError(f"Invalid algorithm: {algorithm!r}")
 
         # Prepare query
         encode(sequence, self.score_matrix._ahash, &query, &length)
@@ -1057,33 +1155,17 @@
             for i in range(size):
                 result = result_type.__new__(result_type)
                 result._target_index = i
                 Py_INCREF(result)
                 PyList_SET_ITEM(results, i, result)
                 results_raw.push_back(&result._result)
 
-            # Select best available SIMD backend
-            IF AVX2_BUILD_SUPPORT:
-                if _AVX2_RUNTIME_SUPPORT and searchfn is NULL:
-                    searchfn = opalSearchDatabaseAVX2
-            IF SSE4_BUILD_SUPPORT:
-                if _SSE4_RUNTIME_SUPPORT and searchfn is NULL:
-                    searchfn = opalSearchDatabaseSSE4
-            IF SSE2_BUILD_SUPPORT:
-                if _SSE2_RUNTIME_SUPPORT and searchfn is NULL:
-                    searchfn = opalSearchDatabaseSSE2
-            IF NEON_BUILD_SUPPORT:
-                if _NEON_RUNTIME_SUPPORT and searchfn is NULL:
-                    searchfn = opalSearchDatabaseNEON
-            if searchfn is NULL:
-                raise RuntimeError("No supported SIMD backend available")
-
             # Run search pipeline in nogil mode
             with nogil:
-                retcode = searchfn(
+                retcode = self._search(
                     query,
                     length,
                     self._sequences.data(),
                     self._sequences.size(),
                     self._lengths.data(),
                     gap_open,
                     gap_extend,
```

### Comparing `pyopal-0.2.0/pyopal/_opal_avx2.pyx` & `pyopal-0.3.0/pyopal/_opal_avx2.pyx`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/pyopal/_opal_neon.pyx` & `pyopal-0.3.0/pyopal/_opal_neon.pyx`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/pyopal/_opal_sse2.pyx` & `pyopal-0.3.0/pyopal/_opal_sse2.pyx`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/pyopal/_opal_sse4.pyx` & `pyopal-0.3.0/pyopal/_opal_sse4.pyx`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/pyopal/tests/test_database.py` & `pyopal-0.3.0/pyopal/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/pyopal/tests/test_doctest.py` & `pyopal-0.3.0/pyopal/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/pyopal/tests/test_search.py` & `pyopal-0.3.0/pyopal/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/pyopal.egg-info/PKG-INFO` & `pyopal-0.3.0/pyopal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 Metadata-Version: 2.1
 Name: pyopal
-Version: 0.2.0
+Version: 0.3.0
 Summary: Cython bindings and Python interface to Opal, a SIMD-accelerated pairwise aligner.
 Home-page: https://github.com/althonos/pyopal
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: MIT
 Project-URL: Documentation, https://pyopal.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/althonos/pyopal/issues
 Project-URL: Changelog, https://github.com/althonos/pyopal/blob/main/CHANGELOG.md
 Project-URL: Coverage, https://codecov.io/gh/althonos/pyopal/
 Project-URL: Builds, https://github.com/althonos/pyopal/actions
 Project-URL: PyPI, https://pypi.org/project/pyopal
 Keywords: bioinformatics,pairwise,sequence,alignment,opal
 Platform: any
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Typing :: Typed
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # 🐍🌈🪨 PyOpal [![Stars](https://img.shields.io/github/stars/althonos/pyopal.svg?style=social&maxAge=3600&label=Star)](https://github.com/althonos/pyopal/stargazers)
 
 *[Cython](https://cython.org/) bindings and Python interface to [Opal](https://github.com/Martinsos/opal), a SIMD-accelerated database search aligner.*
 
-[![Actions](https://img.shields.io/github/workflow/status/althonos/pyopal/Test/main?logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pyopal/actions)
+[![Actions](https://img.shields.io/github/actions/workflow/status/althonos/pyopal/test.yml?branch=main&logo=github&style=flat-square&maxAge=300)](https://github.com/althonos/pyopal/actions)
 [![Coverage](https://img.shields.io/codecov/c/gh/althonos/pyopal?style=flat-square&maxAge=3600&logo=codecov)](https://codecov.io/gh/althonos/pyopal/)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square&maxAge=2678400)](https://choosealicense.com/licenses/mit/)
 [![PyPI](https://img.shields.io/pypi/v/pyopal.svg?style=flat-square&maxAge=3600&logo=PyPI)](https://pypi.org/project/pyopal)
 [![Bioconda](https://img.shields.io/conda/vn/bioconda/pyopal?style=flat-square&maxAge=3600&logo=anaconda)](https://anaconda.org/bioconda/pyopal)
 [![AUR](https://img.shields.io/aur/version/python-pyopal?logo=archlinux&style=flat-square&maxAge=3600)](https://aur.archlinux.org/packages/python-pyopal)
 [![Wheel](https://img.shields.io/pypi/wheel/pyopal.svg?style=flat-square&maxAge=3600)](https://pypi.org/project/pyopal/#files)
 [![Python Versions](https://img.shields.io/pypi/pyversions/pyopal.svg?style=flat-square&maxAge=600&logo=python)](https://pypi.org/project/pyopal/#files)
```

### Comparing `pyopal-0.2.0/setup.cfg` & `pyopal-0.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,27 @@
 description = Cython bindings and Python interface to Opal, a SIMD-accelerated pairwise aligner.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 platform = any
 keywords = bioinformatics, pairwise, sequence, alignment, opal
 classifier = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: C
 	Programming Language :: Cython
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Medical Science Apps.
 	Typing :: Typed
 project_urls = 
 	Documentation = https://pyopal.readthedocs.io/en/stable/
@@ -40,14 +41,16 @@
 zip_safe = false
 packages = pyopal, pyopal.tests
 include_package_data = false
 python_requires = >=3.5
 setup_requires = 
 	setuptools >=46.4
 	cython ~=0.29.16
+install_requires = 
+	archspec ~=0.2
 tests_require = 
 	importlib-resources ; python_version < '3.7'
 
 [options.package_data]
 pyopal = py.typed, *.pyi
 pyopal.tests = requirements.txt
 pyopal.tests.data = *
```

### Comparing `pyopal-0.2.0/setup.py` & `pyopal-0.3.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 import re
 import setuptools
 import setuptools.extension
 import subprocess
 import sys
 from distutils.command.clean import clean as _clean
 from distutils.errors import CompileError
-from setuptools.command.build_clib import build_clib as _build_clib
 from setuptools.command.build_ext import build_ext as _build_ext
 from setuptools.command.sdist import sdist as _sdist
 from setuptools.extension import Library
 
 try:
     from Cython.Build import cythonize
 except ImportError as err:
@@ -427,225 +426,14 @@
         # cythonize the extensions (retaining platform-specific sources)
         self.extensions = cythonize(extensions, **cython_args)
 
         # build the extensions as normal
         _build_ext.build_extensions(self)
 
 
-class build_clib(_build_clib):
-    """A custom `build_clib` that makes all C++ class attributes public."""
-
-    # --- Compatibility with `setuptools.Command`
-
-    user_options = _build_clib.user_options + [
-        ("parallel", "j", "number of parallel build jobs"),
-    ]
-
-    def initialize_options(self):
-        _build_clib.initialize_options(self)
-        self.parallel = None
-
-    def finalize_options(self):
-        _build_clib.finalize_options(self)
-        if self.parallel is not None:
-            self.parallel = int(self.parallel)
-
-    # --- Autotools-like helpers ---
-
-    def _patch_file(self, input, output):
-        basename = os.path.basename(input)
-        patchname = os.path.realpath(
-            os.path.join(__file__, os.pardir, "patches", "{}.patch".format(basename))
-        )
-        if os.path.exists(patchname):
-            _eprint(
-                "patching", os.path.relpath(input), "with", os.path.relpath(patchname)
-            )
-            with open(patchname, "r") as patchfile:
-                patch = patchfile.read()
-            with open(input, "r") as src:
-                srcdata = src.read()
-            with open(output, "w") as dst:
-                dst.write(_apply_patch(srcdata, patch))
-        else:
-            self.copy_file(input, output)
-
-    def _check_function(self, funcname, header, args="()"):
-        _eprint("checking whether function", repr(funcname), "is available", end="... ")
-
-        self.mkpath(self.build_temp)
-        base = "have_{}".format(funcname)
-        testfile = os.path.join(self.build_temp, "{}.c".format(base))
-        binfile = self.compiler.executable_filename(base, output_dir=self.build_temp)
-        objects = []
-
-        with open(testfile, "w") as f:
-            f.write(
-                """
-                #include <{}>
-                int main() {{
-                    {}{};
-                    return 0;
-                }}
-            """.format(
-                    header, funcname, args
-                )
-            )
-        try:
-            objects = self.compiler.compile([testfile], debug=self.debug)
-            self.compiler.link_executable(objects, base, output_dir=self.build_temp)
-        except:
-            _eprint("no")
-            return False
-        else:
-            _eprint("yes")
-            return True
-        finally:
-            os.remove(testfile)
-            for obj in filter(os.path.isfile, objects):
-                os.remove(obj)
-            if os.path.isfile(binfile):
-                os.remove(binfile)
-
-    # --- Compatibility with base `build_clib` command ---
-
-    def check_library_list(self, libraries):
-        pass
-
-    def get_library_names(self):
-        return [lib.name for lib in self.libraries]
-
-    def get_source_files(self):
-        return [source for lib in self.libraries for source in lib.sources]
-
-    def get_library(self, name):
-        return next(lib for lib in self.libraries if lib.name == name)
-
-    # --- Build code ---
-
-    def build_libraries(self, libraries):
-        # check for functions required for libcpu_features on OSX
-        if TARGET_SYSTEM == "macos":
-            _patch_osx_compiler(self.compiler)
-            if self._check_function(
-                "sysctlbyname", "sys/sysctl.h", args="(NULL, NULL, 0, NULL, 0)"
-            ):
-                self.compiler.define_macro("HAVE_SYSCTLBYNAME", 1)
-
-        # build each library only if the sources are outdated
-        self.mkpath(self.build_clib)
-        for library in libraries:
-            libname = self.compiler.library_filename(
-                library.name, output_dir=self.build_clib
-            )
-            self.make_file(library.sources, libname, self.build_library, (library,))
-
-    def build_library(self, library):
-        # show the compiler being used
-        _eprint(
-            "building", library.name, "with", self.compiler.compiler_type, "compiler"
-        )
-
-        # detect hardware detection capabilities of CPU features
-        hwcaps = False
-        if self._check_function("getauxval", "sys/auxv.h", "(0)"):
-            library.define_macros.append(("HAVE_STRONG_GETAUXVAL", 1))
-            hwcaps = True
-        if self._check_function("dlclose", "dlfcn.h", "(0)"):
-            library.define_macros.append(("HAVE_DLFCN_H", 1))
-            hwcaps = True
-        if library.name == "cpu_features" and hwcaps and TARGET_SYSTEM in ("linux_or_android", "freebsd", "macos"):
-            library.sources.extend(
-                os.path.join("vendor", "cpu_features", "src", basename)
-                for basename in [
-                    "hwcaps.c",
-                    "copy.inl",
-                    "define_introspection.inl",
-                    "define_introspection_and_hwcaps.inl",
-                    "equals.inl",
-                    "impl_x86__base_implementation.inl",
-                ]
-            )
-
-        # add debug flags if we are building in debug mode
-        if self.debug:
-            if self.compiler.compiler_type in {"unix", "cygwin", "mingw32"}:
-                library.extra_compile_args.append("-g")
-            elif self.compiler.compiler_type == "msvc":
-                library.extra_compile_args.append("/Z7")
-
-        # add C++11 flags
-        if library.language == "c++":
-            if self.compiler.compiler_type in {"unix", "cygwin", "mingw32"}:
-                library.extra_compile_args.append("-std=c++11")
-                library.extra_link_args.append("-Wno-alloc-size-larger-than")
-            elif self.compiler.compiler_type == "msvc":
-                library.extra_compile_args.append("/std:c11")
-
-        # add Windows flags
-        if self.compiler.compiler_type == "msvc":
-            library.define_macros.append(("WIN32", 1))
-
-        # expose all private members and copy headers to build directory
-        for header in library.depends:
-            output = os.path.join(
-                self.build_clib, os.path.relpath(header, INCLUDE_FOLDER)
-            )
-            self.mkpath(os.path.dirname(output))
-            self.make_file([header], output, self._patch_file, (header, output))
-
-        # copy sources to build directory
-        sources = [
-            os.path.join(self.build_temp, os.path.basename(source))
-            for source in library.sources
-        ]
-        for source, source_copy in zip(library.sources, sources):
-            self.make_file(
-                [source], source_copy, self._patch_file, (source, source_copy)
-            )
-
-        # store compile args
-        compile_args = (
-            None,
-            library.define_macros,
-            library.include_dirs + [self.build_clib],
-            self.debug,
-            library.extra_compile_args,
-            None,
-            library.depends,
-        )
-        # manually prepare sources and get the names of object files
-        objects = [
-            re.sub(r"(.cpp|.c)$", self.compiler.obj_extension, s) for s in sources
-        ]
-        # only compile outdated files
-        with multiprocessing.pool.ThreadPool(self.parallel) as pool:
-            pool.starmap(
-                functools.partial(self._compile_file, compile_args=compile_args),
-                zip(sources, objects),
-            )
-
-        # link into a static library
-        libfile = self.compiler.library_filename(
-            library.name,
-            output_dir=self.build_clib,
-        )
-        self.make_file(
-            objects,
-            libfile,
-            self.compiler.create_static_lib,
-            (objects, library.name, self.build_clib, None, self.debug),
-        )
-
-    def _compile_file(self, source, object, compile_args):
-        self.make_file(
-            [source], object, self.compiler.compile, ([source], *compile_args)
-        )
-
-
 class clean(_clean):
     """A `clean` that removes intermediate files created by Cython."""
 
     def run(self):
 
         source_dir = os.path.join(os.path.dirname(__file__), "pymuscle5")
 
@@ -660,35 +448,14 @@
 
         _clean.run(self)
 
 
 # --- Setup ---------------------------------------------------------------------
 
 setuptools.setup(
-    libraries=[
-        Library(
-            "cpu_features",
-            language="c",
-            sources=[
-                os.path.join("vendor", "cpu_features", "src", base)
-                for base in [
-                    "impl_{}_{}.c".format(TARGET_CPU, TARGET_SYSTEM),
-                    "filesystem.c",
-                    "stack_line_reader.c",
-                    "string_view.c",
-
-                ]
-            ],
-            include_dirs=[
-                os.path.join("vendor", "cpu_features", "include"),
-                os.path.join("vendor", "cpu_features", "src"),
-            ],
-            define_macros=[("STACK_LINE_READER_BUFFER_SIZE", 1024)],
-        )
-    ],
     ext_modules=[
         Extension(
             "pyopal._opal_neon",
             language="c++",
             requires="NEON",
             define_macros=[
                 ("__ARM_NEON", 1),
@@ -759,21 +526,19 @@
             language="c++",
             sources=[
                 os.path.join("vendor", "opal", "src", "ScoreMatrix.cpp"),
                 os.path.join("pyopal", "_opal.pyx"),
             ],
             extra_compile_args=[],
             include_dirs=[
-                os.path.join("vendor", "cpu_features", "include"),
                 os.path.join("vendor", "opal", "src"),
                 "pyopal",
                 "include",
             ],
         ),
     ],
     cmdclass={
         "sdist": sdist,
         "build_ext": build_ext,
-        "build_clib": build_clib,
         "clean": clean,
     },
 )
```

### Comparing `pyopal-0.2.0/vendor/opal/LICENSE` & `pyopal-0.3.0/vendor/opal/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/vendor/opal/README.md` & `pyopal-0.3.0/vendor/opal/README.md`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/vendor/opal/src/ScoreMatrix.cpp` & `pyopal-0.3.0/vendor/opal/src/ScoreMatrix.cpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/vendor/opal/src/ScoreMatrix.hpp` & `pyopal-0.3.0/vendor/opal/src/ScoreMatrix.hpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/vendor/opal/src/opal.cpp` & `pyopal-0.3.0/vendor/opal/src/opal.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1596,17 +1596,17 @@
     Cell::Field field = Cell::Field::H;  // Current field type.
     while (rIdx >= 0 && cIdx >= 0) {
         Cell cell = matrix[cIdx][rIdx];  // Current cell.
 
         // Determine to which cell and which field we should go next, move, and add operation to alignment.
         switch (field) {
         case Cell::Field::H:
-            if (cell.H == cell.E) {
+            if ((cell.H == cell.E) && (cIdx > 0)) {
                 field = Cell::Field::E;
-            } else if (cell.H == cell.F) {
+            } else if ((cell.H == cell.F) && (rIdx > 0)) {
                 field = Cell::Field::F;
             } else {
                 alignment[alignmentLength++] = (query[rIdx] == target[cIdx] ? OPAL_ALIGN_MATCH
                                                 : OPAL_ALIGN_MISMATCH);
                 cIdx--; rIdx--;
             }
             break;
```

### Comparing `pyopal-0.2.0/vendor/opal/src/opal.h` & `pyopal-0.3.0/vendor/opal/src/opal.h`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/vendor/opal/src/opal_aligner.cpp` & `pyopal-0.3.0/vendor/opal/src/opal_aligner.cpp`

 * *Files identical despite different names*

### Comparing `pyopal-0.2.0/vendor/opal/src/test.cpp` & `pyopal-0.3.0/vendor/opal/src/test.cpp`

 * *Files identical despite different names*

