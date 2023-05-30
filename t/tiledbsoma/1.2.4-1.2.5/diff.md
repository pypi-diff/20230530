# Comparing `tmp/tiledbsoma-1.2.4.tar.gz` & `tmp/tiledbsoma-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledbsoma-1.2.4.tar", last modified: Mon May 22 22:52:31 2023, max compression
+gzip compressed data, was "tiledbsoma-1.2.5.tar", last modified: Tue May 30 20:56:37 2023, max compression
```

## Comparing `tiledbsoma-1.2.4.tar` & `tiledbsoma-1.2.5.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-22 22:52:28.000000 tiledbsoma-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-05-22 22:52:28.000000 tiledbsoma-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 22:52:30.000000 tiledbsoma-1.2.4/RELEASE-VERSION
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-05-22 22:52:28.000000 tiledbsoma-1.2.4/dist_links/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     8992 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Superbuild.cmake
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/inputs/
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/patches/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/reader.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/reader.uml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/
--rw-r--r--   0 runner    (1001) docker     (122)    10987 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     4146 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/cli/cli.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/span/
--rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/span/span.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     7142 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
--rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
--rw-r--r--   0 runner    (1001) docker     (122)     6694 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/
--rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/logger_public.h
--rw-r--r--   0 runner    (1001) docker     (122)     7106 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    10181 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/managed_query.h
--rw-r--r--   0 runner    (1001) docker     (122)    14643 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15637 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_array.h
--rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (122)     9491 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_group.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/array_buffers.h
--rw-r--r--   0 runner    (1001) docker     (122)     7272 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/carrow.h
--rw-r--r--   0 runner    (1001) docker     (122)     7844 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/column_buffer.h
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/common.h
--rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/logger.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/logger.h
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/stats.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/stats.h
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/util.cc
--rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/util.h
--rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/version.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/version.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/
--rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_soma_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_soma_array.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_soma_group.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.596076 tiledbsoma-1.2.4/dist_links/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)     2537 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/scripts/bld
--rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/scripts/run-clang-format.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/scripts/show-versions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/dist_links/scripts/update-tiledb-version.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    10989 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.592076 tiledbsoma-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_arrow_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    27087 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     7131 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_common_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    33740 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_dense_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_general_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_read_iters.py
--rw-r--r--   0 runner    (1001) docker     (122)    11918 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_sparse_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_tdb_handles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7628 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_tiledb_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_tiledb_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/eta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/experiment_query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/src/tiledbsoma/io/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/io/conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    55729 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/io/ingest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/src/tiledbsoma/options/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/options/_soma_tiledb_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/options/_tiledb_create_options.py
--rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/pytiledbsoma.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/src/tiledbsoma/query_condition.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 22:52:31.600076 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-22 22:52:31.000000 tiledbsoma-1.2.4/src/tiledbsoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-05-22 22:52:29.000000 tiledbsoma-1.2.4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-30 20:56:36.000000 tiledbsoma-1.2.5/RELEASE-VERSION
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/dist_links/
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     8992 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5006 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5158 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Superbuild.cmake
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/inputs/
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/reader.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/reader.uml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/
+-rw-r--r--   0 runner    (1001) docker     (122)    10987 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     4146 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/cli/cli.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/span/
+-rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/span/span.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     7142 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     6694 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/
+-rw-r--r--   0 runner    (1001) docker     (122)     2886 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/logger_public.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7106 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10181 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/managed_query.h
+-rw-r--r--   0 runner    (1001) docker     (122)    14643 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15637 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_array.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5451 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     9491 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_group.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.787899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3727 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/array_buffers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7272 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/arrow_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/carrow.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7844 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7742 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/column_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)     6904 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/logger.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/logger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/stats.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/stats.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/util.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/util.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/version.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1650 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/version.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.791899 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     2212 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6489 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_soma_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     5644 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    10530 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_soma_array.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_soma_group.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.791899 tiledbsoma-1.2.5/dist_links/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2537 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/scripts/bld
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/scripts/run-clang-format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/scripts/show-versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/dist_links/scripts/update-tiledb-version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    10989 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.783899 tiledbsoma-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.791899 tiledbsoma-1.2.5/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     5370 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_arrow_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27175 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7213 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_common_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33854 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6920 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_dense_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2592 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6792 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1742 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_general_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3188 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2492 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_read_iters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11918 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_sparse_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_tdb_handles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7628 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_tiledb_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_tiledb_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/eta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/experiment_query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/src/tiledbsoma/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/io/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    55615 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/io/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/src/tiledbsoma/options/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4896 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/options/_soma_tiledb_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11206 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/options/_tiledb_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26382 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/pytiledbsoma.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7776 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/src/tiledbsoma/query_condition.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 20:56:37.795899 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4292 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-30 20:56:37.000000 tiledbsoma-1.2.5/src/tiledbsoma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-05-30 20:56:35.000000 tiledbsoma-1.2.5/version.py
```

### Comparing `tiledbsoma-1.2.4/PKG-INFO` & `tiledbsoma-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.2.4/README.md` & `tiledbsoma-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/CMakeLists.txt` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/README.md` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/Superbuild.cmake` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/Superbuild.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/cmake/patches/spdlog.patch` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/cmake/patches/spdlog.patch`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/reader.svg` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/reader.svg`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/doc/reader.uml` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/doc/reader.uml`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/CMakeLists.txt` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/cli/cli.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/cli/cli.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/.clang-format` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/.clang-format`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/span/span.hpp` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/span/span.hpp`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/producer_consumer_queue.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/status.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/include/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/thread_pool/status.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/external/src/thread_pool/thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/logger_public.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/logger_public.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/managed_query.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/managed_query.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/managed_query.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_array.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_array.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_array.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_array.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_group.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/soma/soma_group.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/soma/soma_group.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/tiledbsoma/tiledbsoma`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/array_buffers.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/array_buffers.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/arrow_adapter.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/arrow_adapter.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/carrow.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/carrow.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/column_buffer.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/column_buffer.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/column_buffer.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/common.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/common.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/logger.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/logger.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/logger.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/logger.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/stats.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/stats.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/stats.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/stats.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/util.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/util.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/util.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/util.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/version.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/version.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/src/utils/version.h` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/src/utils/version.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/CMakeLists.txt` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_query_condition.py` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_simple.py` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/test_soma_array.py` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/test_soma_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_column_buffer.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_managed_query.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_soma_array.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_soma_array.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_soma_group.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_soma_group.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/libtiledbsoma/test/unit_thread_pool.cc` & `tiledbsoma-1.2.5/dist_links/libtiledbsoma/test/unit_thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/scripts/bld` & `tiledbsoma-1.2.5/dist_links/scripts/bld`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/scripts/run-clang-format.sh` & `tiledbsoma-1.2.5/dist_links/scripts/run-clang-format.sh`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/scripts/show-versions.py` & `tiledbsoma-1.2.5/dist_links/scripts/show-versions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/dist_links/scripts/update-tiledb-version.py` & `tiledbsoma-1.2.5/dist_links/scripts/update-tiledb-version.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/setup.py` & `tiledbsoma-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         "numba==0.56.4; python_version<'3.11'",
         "numba==0.57.0rc1; python_version=='3.11'",
         "numpy>=1.18,<1.24",
         "pandas",
         "pyarrow>=9.0.0",
         "scanpy>=1.9.2",
         "scipy",
-        "somacore==1.0.2",
+        "somacore==1.0.3",
         "tiledb~=0.21.3",
         "typing-extensions",  # Note "-" even though `import typing_extensions`
     ],
     extras_require={
         "dev": [
             "black",
             "ruff",
```

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/__init__.py` & `tiledbsoma-1.2.5/src/tiledbsoma/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     get_implementation_version,
     get_SOMA_version,
     get_storage_engine,
     show_package_versions,
 )
 from ._measurement import Measurement
 from ._sparse_nd_array import SparseNDArray
-from .options import SOMATileDBContext
+from .options import SOMATileDBContext, TileDBCreateOptions
 from .pytiledbsoma import (
     tiledbsoma_stats_disable,
     tiledbsoma_stats_dump,
     tiledbsoma_stats_enable,
     tiledbsoma_stats_reset,
 )
 
@@ -136,18 +136,19 @@
     "ExperimentAxisQuery",
     "get_implementation_version",
     "get_implementation",
     "get_SOMA_version",
     "get_storage_engine",
     "Measurement",
     "open",
+    "ResultOrder",
     "show_package_versions",
+    "SOMA_JOINID",
     "SOMAError",
-    "ResultOrder",
     "SOMATileDBContext",
-    "SOMA_JOINID",
     "SparseNDArray",
+    "TileDBCreateOptions",
     "tiledbsoma_stats_disable",
     "tiledbsoma_stats_dump",
     "tiledbsoma_stats_enable",
     "tiledbsoma_stats_reset",
 ]
```

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_arrow_types.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_arrow_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_collection.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 from ._sparse_nd_array import SparseNDArray
 from ._tiledb_object import AnyTileDBObject, TileDBObject
 from ._types import OpenTimestamp
 from ._util import (
     is_relative_uri,
     make_relative_path,
     uri_joinpath,
-    validate_platform_config,
 )
 from .options import SOMATileDBContext
 from .options._soma_tiledb_context import _validate_soma_tiledb_context
 
 # A collection can hold any sub-type of TileDBObject
 CollectionElementType = TypeVar("CollectionElementType", bound=AnyTileDBObject)
 _TDBO = TypeVar("_TDBO", bound=AnyTileDBObject)
@@ -92,16 +91,19 @@
         This creates a new SOMA collection of the current type in storage and
         returns it opened for writing.
 
         Args:
             uri:
                 The location to create this SOMA collection at.
             platform_config:
-                Platform-specific options used to create this collection, provided in the form
-                ``{"tiledb": {"create": {"sparse_nd_array_dim_zstd_level": 7}}}``.
+                Platform-specific options used to create this collection.
+                This may be provided as settings in a dictionary, with options
+                located in the ``{'tiledb': {'create': ...}}`` key,
+                or as a :class:`~tiledbsoma.TileDBCreateOptions` object.
+                (Currently unused for collections.)
             context:
                 If provided, the :class:`SOMATileDBContext` to use when creating and
                 opening this collection.
             tiledb_timestamp:
                 If specified, overrides the default timestamp
                 used to open this object. If unset, uses the timestamp provided by
                 the context.
@@ -110,15 +112,14 @@
             TileDBError:
                 If unable to create the underlying object.
 
         Lifecycle:
             Experimental.
         """
         context = _validate_soma_tiledb_context(context)
-        validate_platform_config(platform_config)
         tiledb.group_create(uri=uri, ctx=context.tiledb_ctx)
         handle = cls._wrapper_type.open(uri, "w", context, tiledb_timestamp)
         cls._set_create_metadata(handle)
         return cls(
             handle,
             _dont_call_this_use_create_or_open_instead="tiledbsoma-internal-code",
         )
```

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_common_nd_array.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_common_nd_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,16 +55,18 @@
                 None)``, as the sequence length determines the number of dimensions
                 N in the N-dimensional array.
 
                 For :class:`SparseNDArray` only, if a slot is None, then the maximum
                 possible int64 will be used.  This makes a :class:`SparseNDArray`
                 growable.
             platform_config:
-                Platform-specific options used to create this array, provided in the form
-                ``{"tiledb": {"create": {"sparse_nd_array_dim_zstd_level": 7}}}``.
+                Platform-specific options used to create this array.
+                This may be provided as settings in a dictionary, with options
+                located in the ``{'tiledb': {'create': ...}}`` key,
+                or as a :class:`~tiledbsoma.TileDBCreateOptions` object.
             tiledb_timestamp:
                 If specified, overrides the default timestamp
                 used to open this object. If unset, uses the timestamp provided by
                 the context.
 
         Returns:
             The created NDArray.
@@ -84,15 +86,14 @@
         # reason that the latter, while temptingly simple, is actually untrue is that tiledb core
         # requires that the capacity, when rounded up to an exact multiple of the extent, needs to
         # be representable as a signed 64-bit integer.  So in particular when a unit test (or anyone
         # else) sets extent to a not-power-of-two number like 999 or 1000 then the create fails if
         # the upper limit is exactly 2**63-1.
 
         context = _validate_soma_tiledb_context(context)
-        _util.validate_platform_config(platform_config)
         schema = cls._build_tiledb_schema(
             type,
             shape,
             TileDBCreateOptions.from_platform_config(platform_config),
             context,
             is_sparse=cls.is_sparse,
         )
@@ -147,48 +148,48 @@
                 dim_name, dim_shape, create_options
             )
             dim = tiledb.Dim(
                 name=dim_name,
                 domain=(0, dim_capacity - 1),
                 tile=dim_extent,
                 dtype=np.int64,
-                filters=create_options.dim_filters(
+                filters=create_options.dim_filters_tiledb(
                     dim_name,
                     [
                         dict(
                             _type="ZstdFilter",
-                            level=create_options.sparse_nd_array_dim_zstd_level(),
+                            level=create_options.sparse_nd_array_dim_zstd_level,
                         )
                     ],
                 ),
             )
             dims.append(dim)
         dom = tiledb.Domain(dims, ctx=context.tiledb_ctx)
 
         attrs = [
             tiledb.Attr(
                 name="soma_data",
                 dtype=_arrow_types.tiledb_type_from_arrow_type(type),
-                filters=create_options.attr_filters("soma_data", ["ZstdFilter"]),
+                filters=create_options.attr_filters_tiledb("soma_data", ["ZstdFilter"]),
                 ctx=context.tiledb_ctx,
             )
         ]
 
         cell_order, tile_order = create_options.cell_tile_orders()
 
         # TODO: accept more TileDB array-schema options from create_options
         # https://github.com/single-cell-data/TileDB-SOMA/issues/876
         return tiledb.ArraySchema(
             domain=dom,
             attrs=attrs,
             sparse=is_sparse,
-            allows_duplicates=create_options.allows_duplicates(),
-            offsets_filters=create_options.offsets_filters(),
-            validity_filters=create_options.validity_filters(),
-            capacity=create_options.capacity(),
+            allows_duplicates=create_options.allows_duplicates,
+            offsets_filters=create_options.offsets_filters_tiledb(),
+            validity_filters=create_options.validity_filters_tiledb(),
+            capacity=create_options.capacity,
             tile_order=tile_order,
             cell_order=cell_order,
             ctx=context.tiledb_ctx,
         )
 
     @classmethod
     def _dim_capacity_and_extent(
```

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_dataframe.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2021-2023 TileDB, Inc.
 #
 # Licensed under the MIT License.
 
 """
 Implementation of a SOMA DataFrame
 """
-from typing import Any, Mapping, Optional, Sequence, Tuple, Type, Union, cast
+from typing import Any, Optional, Sequence, Tuple, Type, Union, cast
 
 import numpy as np
 import pyarrow as pa
 import somacore
 import tiledb
 from somacore import options
 from typing_extensions import Self
@@ -156,16 +156,18 @@
                 stored in that column.  If provided, this sequence must have the same
                 length as ``index_column_names``, and the index-column domain will be as
                 specified.  If omitted entirely, or if ``None`` in a given dimension,
                 the corresponding index-column domain will use the minimum and maximum
                 possible values for the column's datatype.  This makes a
                 :class:`DataFrame` growable.
             platform_config:
-                Platform-specific options used to create this array, provided in the form
-                ``{"tiledb": {"create": {"dataframe_dim_zstd_level": 7}}}``.
+                Platform-specific options used to create this array.
+                This may be provided as settings in a dictionary, with options
+                located in the ``{'tiledb': {'create': ...}}`` key,
+                or as a :class:`~tiledbsoma.TileDBCreateOptions` object.
             tiledb_timestamp:
                 If specified, overrides the default timestamp
                 used to open this object. If unset, uses the timestamp provided by
                 the context.
 
         Returns:
             The DataFrame.
@@ -197,15 +199,14 @@
             0            0    a
             1            1    b
 
         Lifecycle:
             Experimental.
         """
         context = _validate_soma_tiledb_context(context)
-        _util.validate_platform_config(platform_config)
         schema = _canonicalize_schema(schema, index_column_names)
         tdb_schema = _build_tiledb_schema(
             schema,
             index_column_names,
             domain,
             TileDBCreateOptions.from_platform_config(platform_config),
             context,
@@ -348,15 +349,15 @@
         # TODO: platform_config
         # TODO: batch_size
 
         sr.submit()
         return TableReadIter(sr)
 
     def write(
-        self, values: pa.Table, platform_config: Optional[Mapping[str, Any]] = None
+        self, values: pa.Table, platform_config: Optional[options.PlatformConfig] = None
     ) -> Self:
         """Writes an `Arrow table <https://arrow.apache.org/docs/python/generated/pyarrow.Table.html>`_
         to the persistent object. As duplicate index values are not allowed, index values already
         present in the object are overwritten
         and new index values are added.
 
         Args:
@@ -695,20 +696,20 @@
         )
 
         dim = tiledb.Dim(
             name=index_column_name,
             domain=slot_domain,
             tile=extent,
             dtype=dtype,
-            filters=tiledb_create_options.dim_filters(
+            filters=tiledb_create_options.dim_filters_tiledb(
                 index_column_name,
                 [
                     dict(
                         _type="ZstdFilter",
-                        level=tiledb_create_options.dataframe_dim_zstd_level(),
+                        level=tiledb_create_options.dataframe_dim_zstd_level,
                     )
                 ],
             ),
         )
         dims.append(dim)
 
     dom = tiledb.Domain(dims, ctx=context.tiledb_ctx)
@@ -720,29 +721,31 @@
             continue
         attr = tiledb.Attr(
             name=attr_name,
             dtype=_arrow_types.tiledb_type_from_arrow_type(
                 schema.field(attr_name).type
             ),
             nullable=metadata.get(attr_name.encode("utf-8")) == b"nullable",
-            filters=tiledb_create_options.attr_filters(attr_name, ["ZstdFilter"]),
+            filters=tiledb_create_options.attr_filters_tiledb(
+                attr_name, ["ZstdFilter"]
+            ),
             ctx=context.tiledb_ctx,
         )
         attrs.append(attr)
 
     cell_order, tile_order = tiledb_create_options.cell_tile_orders()
 
     return tiledb.ArraySchema(
         domain=dom,
         attrs=attrs,
         sparse=True,
-        allows_duplicates=tiledb_create_options.allows_duplicates(),
-        offsets_filters=tiledb_create_options.offsets_filters(),
-        validity_filters=tiledb_create_options.validity_filters(),
-        capacity=tiledb_create_options.capacity(),
+        allows_duplicates=tiledb_create_options.allows_duplicates,
+        offsets_filters=tiledb_create_options.offsets_filters_tiledb(),
+        validity_filters=tiledb_create_options.validity_filters_tiledb(),
+        capacity=tiledb_create_options.capacity,
         cell_order=cell_order,
         # As of TileDB core 2.8.2, we cannot consolidate string-indexed sparse arrays with
         # col-major tile order: so we write ``X`` with row-major tile order.
         tile_order=tile_order,
         ctx=context.tiledb_ctx,
     )
```

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_dense_nd_array.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_dense_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_exception.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_exception.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 
 import tiledb
 
 
 class SOMAError(Exception):
     """Base error type for SOMA-specific exceptions.
 
-    Lifecycle: Experimental.
+    Lifecycle: maturing
     """
 
     pass
 
 
 class DoesNotExistError(SOMAError):
     """Raised when attempting to open a non-existent or inaccessible SOMA object.
 
-    Lifecycle: Experimental.
+    Lifecycle: maturing
     """
 
     pass
 
 
 def is_does_not_exist_error(e: tiledb.TileDBError) -> bool:
     """Given a TileDBError, return true if it indicates the object does not exist
 
-    Lifecycle:
-        Experimental.
+    Lifecycle: maturing
 
     Example:
         try:
             with tiledb.open(uri):
                 ...
         except tiledb.TileDBError as e:
             if is_does_not_exist_error(e):
@@ -56,14 +55,14 @@
     return False
 
 
 def is_duplicate_group_key_error(e: tiledb.TileDBError) -> bool:
     """Given a TileDBError, return try if it indicates a duplicate member
     add request in a tiledb.Group.
 
-    Lifecycle: Experimental.
+    Lifecycle: maturing
     """
     stre = str(e)
     if "member already exists in group" in stre:
         return True
 
     return False
```

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_experiment.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_experiment.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_factory.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_factory.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_funcs.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_funcs.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_general_utilities.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_general_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,51 +14,51 @@
 
 from .pytiledbsoma import version as libtiledbsoma_version
 
 
 def get_SOMA_version() -> str:
     """Returns semver-compatible version of the supported SOMA API.
 
-    Lifecycle: Experimental.
+    Lifecycle: maturing
     """
     return "0.2.0-dev"
 
 
 def get_implementation() -> str:
     """Returns the implementation name, e.g., "python-tiledb".
 
-    Lifecycle: Experimental.
+    Lifecycle: maturing
     """
     return "python-tiledb"
 
 
 def get_implementation_version() -> str:
     """Returns the package implementation version as a semver.
 
-    Lifecycle: Experimental.
+    Lifecycle: maturing
     """
     try:
         return get_distribution("tiledbsoma").version
     except DistributionNotFound:
         return "unknown"
 
 
 def get_storage_engine() -> str:
     """Returns underlying storage engine name, e.g., "tiledb".
 
-    Lifecycle: Experimental.
+    Lifecycle: maturing
     """
     return "tiledb"
 
 
 def show_package_versions() -> None:
     """Nominal use is for bug reports, so issue filers and issue fixers can be on
     the same page.
 
-    Lifecycle: Experimental.
+    Lifecycle: maturing
     """
     print("tiledbsoma.__version__       ", get_implementation_version())
     print("TileDB-Py tiledb.version()   ", tiledb.version())
     print(
         "TileDB core version          ",
         ".".join(str(ijk) for ijk in list(tiledb.libtiledb.version())),
     )
```

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_measurement.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_measurement.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_query_condition.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_read_iters.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_read_iters.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_sparse_nd_array.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_sparse_nd_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_tdb_handles.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_tdb_handles.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_tiledb_array.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_tiledb_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_tiledb_object.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_tiledb_object.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_types.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/_util.py` & `tiledbsoma-1.2.5/src/tiledbsoma/_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from itertools import zip_longest
 from typing import Any, Optional, Tuple, Type, TypeVar
 
 import somacore
 from somacore import options
 
 from ._types import OpenTimestamp, Slice, is_slice_of
-from .options._tiledb_create_options import TileDBCreateOptions
 
 
 def get_start_stamp() -> float:
     """Returns information about start time of an event.
 
     Nominally float seconds since the epoch, but articulated here
     as being compatible with the format_elapsed function.
@@ -257,16 +256,7 @@
 
     This may raise an exception, since millis may be outside the representable
     range for a Python datetime.
     """
     secs, millis = divmod(millis, 1000)
     dt = datetime.datetime.fromtimestamp(secs, tz=datetime.timezone.utc)
     return dt.replace(microsecond=millis * 1000)
-
-
-def validate_platform_config(platform_config: Any) -> None:
-    """Offers a run-time type check on this ingestion/creation argument, which is easy to miskey."""
-    if platform_config is not None:
-        if isinstance(platform_config, TileDBCreateOptions):
-            raise TypeError(
-                """platform_config argument is of type TileDBCreateOptions -- please wrap it in `{"tiledb": {"create": argument}}`."""
-            )
```

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/eta.py` & `tiledbsoma-1.2.5/src/tiledbsoma/eta.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/experiment_query.py` & `tiledbsoma-1.2.5/src/tiledbsoma/experiment_query.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/io/conversions.py` & `tiledbsoma-1.2.5/src/tiledbsoma/io/conversions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/io/ingest.py` & `tiledbsoma-1.2.5/src/tiledbsoma/io/ingest.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,16 +212,14 @@
         )
 
     if not isinstance(anndata, ad.AnnData):
         raise TypeError(
             "Second argument is not an AnnData object -- did you want from_h5ad?"
         )
 
-    _util.validate_platform_config(platform_config)
-
     context = _validate_soma_tiledb_context(context)
 
     # Without _at least_ an index, there is nothing to indicate the dimension indices.
     if anndata.obs.index.empty or anndata.var.index.empty:
         raise NotImplementedError("Empty AnnData.obs or AnnData.var unsupported.")
 
     s = _util.get_start_stamp()
@@ -675,16 +673,14 @@
 ) -> _NDArr:
     """
     Create and populate the ``soma_matrix`` from the contents of ``matrix``.
 
     Lifecycle:
         Experimental.
     """
-    _util.validate_platform_config(platform_config)
-
     # SparseDataset has no ndim but it has a shape
     if len(matrix.shape) != 2:
         raise ValueError(f"expected matrix.shape == 2; got {matrix.shape}")
 
     s = _util.get_start_stamp()
     logging.log_io(None, f"START  WRITING {uri}")
 
@@ -855,26 +851,26 @@
         if _chunk_is_contained_in(matrix_bounds, storage_ned):
             logging.log_io(
                 f"Skipped {soma_ndarray.uri}", f"SKIPPED WRITING {soma_ndarray.uri}"
             )
             return
 
     # Write all at once?
-    if not tiledb_create_options.write_X_chunked():
+    if not tiledb_create_options.write_X_chunked:
         if not isinstance(matrix, np.ndarray):
             matrix = matrix.toarray()
         soma_ndarray.write((slice(None),), pa.Tensor.from_numpy(matrix))
         return
 
     # OR, write in chunks
     eta_tracker = eta.Tracker()
     nrow, ncol = matrix.shape
     i = 0
     # Number of rows to chunk by. Dense writes, so this is a constant.
-    chunk_size = int(math.ceil(tiledb_create_options.goal_chunk_nnz() / ncol))
+    chunk_size = int(math.ceil(tiledb_create_options.goal_chunk_nnz / ncol))
     while i < nrow:
         t1 = time.time()
         i2 = i + chunk_size
 
         # Print doubly-inclusive lo..hi like 0..17 and 18..31.
         chunk_percent = min(100, 100 * (i2 - 1) / nrow)
         logging.log_io(
@@ -1034,15 +1030,15 @@
         if _chunk_is_contained_in(matrix_bounds, storage_ned):
             logging.log_io(
                 f"Skipped {soma_ndarray.uri}", f"SKIPPED WRITING {soma_ndarray.uri}"
             )
             return
 
     # Write all at once?
-    if not tiledb_create_options.write_X_chunked():
+    if not tiledb_create_options.write_X_chunked:
         soma_ndarray.write(_coo_to_table(sp.coo_matrix(matrix)))
         return
 
     # Or, write in chunks, striding across the most efficient slice axis
 
     stride_axis = 0
     if sp.isspmatrix_csc(matrix):
@@ -1051,15 +1047,15 @@
     if isinstance(matrix, SparseDataset) and matrix.format_str == "csc":
         # E.g. if we used anndata.X without the [:]
         stride_axis = 1
 
     dim_max_size = matrix.shape[stride_axis]
 
     eta_tracker = eta.Tracker()
-    goal_chunk_nnz = tiledb_create_options.goal_chunk_nnz()
+    goal_chunk_nnz = tiledb_create_options.goal_chunk_nnz
 
     coords = [slice(None), slice(None)]
     i = 0
     while i < dim_max_size:
         t1 = time.time()
 
         # Chunk size on the stride axis
```

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/logging.py` & `tiledbsoma-1.2.5/src/tiledbsoma/logging.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/options/_soma_tiledb_context.py` & `tiledbsoma-1.2.5/src/tiledbsoma/options/_soma_tiledb_context.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/pytiledbsoma.cc` & `tiledbsoma-1.2.5/src/tiledbsoma/pytiledbsoma.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma/query_condition.cc` & `tiledbsoma-1.2.5/src/tiledbsoma/query_condition.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma.egg-info/PKG-INFO` & `tiledbsoma-1.2.5/src/tiledbsoma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.4
+Version: 1.2.5
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
```

### Comparing `tiledbsoma-1.2.4/src/tiledbsoma.egg-info/SOURCES.txt` & `tiledbsoma-1.2.5/src/tiledbsoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.4/version.py` & `tiledbsoma-1.2.5/version.py`

 * *Files identical despite different names*

