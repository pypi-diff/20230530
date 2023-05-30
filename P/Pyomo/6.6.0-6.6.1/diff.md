# Comparing `tmp/Pyomo-6.6.0.tar.gz` & `tmp/Pyomo-6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pyomo-6.6.0.tar", last modified: Wed May 24 22:09:31 2023, max compression
+gzip compressed data, was "Pyomo-6.6.1.tar", last modified: Tue May 30 19:53:45 2023, max compression
```

## Comparing `Pyomo-6.6.0.tar` & `Pyomo-6.6.1.tar`

### file list

```diff
@@ -1,1414 +1,1415 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.733651 Pyomo-6.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-24 22:09:20.000000 Pyomo-6.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 22:09:20.000000 Pyomo-6.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-24 22:09:31.733651 Pyomo-6.6.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.605650 Pyomo-6.6.0/Pyomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-24 22:09:31.000000 Pyomo-6.6.0/Pyomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    49659 2023-05-24 22:09:31.000000 Pyomo-6.6.0/Pyomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:09:31.000000 Pyomo-6.6.0/Pyomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-24 22:09:31.000000 Pyomo-6.6.0/Pyomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-24 22:09:31.000000 Pyomo-6.6.0/Pyomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 22:09:31.000000 Pyomo-6.6.0/Pyomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-24 22:09:20.000000 Pyomo-6.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.605650 Pyomo-6.6.0/pyomo/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.609650 Pyomo-6.6.0/pyomo/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12462 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/autoslots.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/backports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/cmake_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.613650 Pyomo-6.6.0/pyomo/common/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/collections/bunch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/collections/component_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/collections/component_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/collections/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)    93438 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    27155 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    26360 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/gc_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/getGSL.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/gsl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/multithread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/numeric_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/pyomo_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)    16094 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tempfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.617650 Pyomo-6.6.0/pyomo/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/config_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/dep_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/dep_mod_except.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/import_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/relo_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/relo_mod_new.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/relocated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_bunch.py
--rw-r--r--   0 runner    (1001) docker     (123)   105969 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    23916 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_fileutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16629 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_multithread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_tee.py
--rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_tempfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24109 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/tests/test_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)    36980 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/common/unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.617650 Pyomo-6.6.0/pyomo/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.617650 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.617650 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/src/FindASL.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/src/functions.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.617650 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/tests/test_ampl_function_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.617650 Pyomo-6.6.0/pyomo/contrib/appsi/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63191 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.617650 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/cmodel_bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/common.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    68508 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/expression.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    32798 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/expression.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/fbbt_model.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/fbbt_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    32293 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/interval.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/interval.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/lp_writer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/lp_writer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/model_base.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/model_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/nl_writer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/nl_writer.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/tests/test_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/examples/getting_started.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/examples/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/examples/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/examples/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/fbbt.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/cbc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/cplex.py
--rw-r--r--   0 runner    (1001) docker     (123)    60137 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/gurobi.py
--rw-r--r--   0 runner    (1001) docker     (123)    28563 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/highs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19154 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/ipopt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23165 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/tests/test_gurobi_persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/tests/test_ipopt_persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    49399 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/solvers/tests/test_persistent_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/tests/test_fbbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/tests/test_interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/utils/collect_vars_and_named_exprs.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/utils/get_objective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/utils/tests/test_collect_vars_and_named_exprs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/writers/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/writers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/writers/lp_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/writers/nl_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.621650 Pyomo-6.6.0/pyomo/contrib/appsi/writers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/writers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/appsi/writers/tests/test_nl_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/benders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/benders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/benders/benders_cuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/benders/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/benders/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/benders/examples/farmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/benders/examples/grothey_ex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/benders/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/benders/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/benders/tests/test_benders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/community_detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/community_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/community_detection/community_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    41063 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/community_detection/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/community_detection/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/community_detection/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/community_detection/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/community_detection/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63498 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/community_detection/tests/test_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/cp/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/interval_var.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/cp/repn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/repn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46867 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/repn/docplex_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/cp/scheduling_expr/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/scheduling_expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/scheduling_expr/precedence_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/scheduling_expr/step_function_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/cp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50133 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/tests/test_docplex_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/tests/test_docplex_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/tests/test_interval_var.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20260 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/tests/test_logical_to_disjunctive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/tests/test_precedence_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    19693 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/tests/test_step_function_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/cp/transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/transform/logical_to_disjunctive_program.py
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/cp/transform/logical_to_disjunctive_walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/doe/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45357 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/doe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.625650 Pyomo-6.6.0/pyomo/contrib/doe/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/examples/reactor_compute_FIM.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/examples/reactor_grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/examples/reactor_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/examples/reactor_optimize_doe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    29563 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/doe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/tests/test_fim_doe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/doe/tests/test_reactor_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/example/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/example/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/example/foo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/example/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/example/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/example/plugins/ex_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/example/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/example/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/example/tests/test_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/fbbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fbbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63827 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fbbt/fbbt.py
--rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fbbt/interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/fbbt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fbbt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43081 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fbbt/tests/test_fbbt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fbbt/tests/test_interval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/fme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fme/fourier_motzkin_elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fme/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/fme/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fme/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38423 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/fme/tests/test_fourier_motzkin_elimination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/gdp_bounds/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdp_bounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdp_bounds/compute_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdp_bounds/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdp_bounds/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/gdp_bounds/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdp_bounds/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdp_bounds/tests/test_gdp_bounds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.629650 Pyomo-6.6.0/pyomo/contrib/gdpopt/
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/GDPopt.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/algorithm_base_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    25992 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/branch_and_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/config_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/create_oa_subproblems.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/cut_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/discrete_problem_initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/enumerate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/gloa.py
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/loa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/nlp_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/oa_algorithm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/ric.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/solve_discrete_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/solve_subproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.633650 Pyomo-6.6.0/pyomo/contrib/gdpopt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/tests/common_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/tests/test_LBB.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/tests/test_enumerate.py
--rw-r--r--   0 runner    (1001) docker     (123)    72674 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/tests/test_gdpopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    21219 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gdpopt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.633650 Pyomo-6.6.0/pyomo/contrib/gjh/
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gjh/GJH.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gjh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gjh/getGJH.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/gjh/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.633650 Pyomo-6.6.0/pyomo/contrib/iis/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/iis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/iis/iis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.633650 Pyomo-6.6.0/pyomo/contrib/iis/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/iis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/iis/tests/test_iis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.633650 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.633650 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/common/dulmage_mendelsohn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.633650 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/common/tests/test_dulmage_mendelsohn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/connected.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/dulmage_mendelsohn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/incidence.py
--rw-r--r--   0 runner    (1001) docker     (123)    36014 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/scc_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.633650 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/models_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_connected.py
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_dulmage_mendelsohn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_incidence.py
--rw-r--r--   0 runner    (1001) docker     (123)    70937 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_scc_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15890 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_triangularize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/triangularize.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/incidence_analysis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.633650 Pyomo-6.6.0/pyomo/contrib/interior_point/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.633650 Pyomo-6.6.0/pyomo/contrib/interior_point/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/examples/ex1.py
--rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    27675 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/interior_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/inverse_reduced_hessian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.637650 Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/base_linear_solver_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/ma27_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/mumps_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/scipy_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.637650 Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/tests/test_linear_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/tests/test_realloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.637650 Pyomo-6.6.0/pyomo/contrib/interior_point/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/tests/test_interior_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/tests/test_inverse_reduced_hessian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/tests/test_realloc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/interior_point/tests/test_reg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.637650 Pyomo-6.6.0/pyomo/contrib/mcpp/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mcpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mcpp/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mcpp/getMCPP.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mcpp/mcppInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mcpp/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mcpp/pyomo_mcpp.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mcpp/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12697 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mcpp/test_mcpp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.637650 Pyomo-6.6.0/pyomo/contrib/mindtpy/
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/MindtPy.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   133056 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/algorithm_base_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    26495 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/config_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    16924 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/cut_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/extended_cutting_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/feasibility_pump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/global_outer_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19632 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/mip_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)    20638 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/nlp_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/outer_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    44785 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/single_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tabu_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.641650 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/MINLP2_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/MINLP3_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/MINLP4_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/MINLP5_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/MINLP_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/constraint_qualification_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/eight_process_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/feasibility_pump1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/feasibility_pump2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/from_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/nonconvex1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/nonconvex2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/nonconvex3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/nonconvex4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/online_doc_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    18410 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_ECP.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_feas_pump.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_global_lp_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_lp_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_solution_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    50885 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mindtpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.641650 Pyomo-6.6.0/pyomo/contrib/mpc/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.641650 Pyomo-6.6.0/pyomo/contrib/mpc/data/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/dynamic_data_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/find_nearest_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/get_cuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/interval_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/scalar_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/series_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.641650 Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_find_nearest_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_get_cuid.py
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_interval_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_scalar_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_series_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.641650 Pyomo-6.6.0/pyomo/contrib/mpc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.641650 Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/run_mpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/run_openloop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.641650 Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/tests/test_openloop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.641650 Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/copy_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/model_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.641650 Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23841 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/tests/test_var_linker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/var_linker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.645650 Pyomo-6.6.0/pyomo/contrib/mpc/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/modeling/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/modeling/cost_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/modeling/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.645650 Pyomo-6.6.0/pyomo/contrib/mpc/modeling/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/modeling/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/modeling/tests/test_cost_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/modeling/tests/test_input_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/mpc/modeling/tests/test_terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.645650 Pyomo-6.6.0/pyomo/contrib/multistart/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/multistart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/multistart/high_conf_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/multistart/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/multistart/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/multistart/reinit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/multistart/test_multi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.645650 Pyomo-6.6.0/pyomo/contrib/parmest/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.645650 Pyomo-6.6.0/pyomo/contrib/parmest/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.645650 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reaction_kinetics/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reaction_kinetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reaction_kinetics/simple_reaction_parmest_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.645650 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/bootstrap_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/datarec_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/leaveNout_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/likelihood_ratio_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/multisensor_data_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/parameter_estimation_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/reactor_design.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/timeseries_data_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.645650 Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/bootstrap_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/likelihood_ratio_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/parameter_estimation_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler_with_constraint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.645650 Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/parallel_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/parameter_estimation_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/scenario_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/semibatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/ipopt_solver_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    51756 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/parmest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/scenariocreator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.649650 Pyomo-6.6.0/pyomo/contrib/parmest/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)    35606 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_parmest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_scenariocreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.649650 Pyomo-6.6.0/pyomo/contrib/parmest/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/utils/create_ef.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/utils/ipopt_solver_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/utils/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/utils/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/parmest/utils/scenario_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.649650 Pyomo-6.6.0/pyomo/contrib/piecewise/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/piecewise_linear_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/piecewise_linear_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.649650 Pyomo-6.6.0/pyomo/contrib/piecewise/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/tests/common_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/tests/test_inner_repn_gdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/tests/test_outer_repn_gdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/tests/test_piecewise_linear_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/tests/test_reduced_inner_repn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.649650 Pyomo-6.6.0/pyomo/contrib/piecewise/transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/transform/convex_combination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/transform/disaggregated_convex_combination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/transform/inner_representation_gdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/transform/multiple_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/transform/outer_representation_gdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/transform/piecewise_to_gdp_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/transform/piecewise_to_mip_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/piecewise/transform/reduced_inner_representation_gdp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.649650 Pyomo-6.6.0/pyomo/contrib/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.649650 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/bounds_to_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/constraint_tightener.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/deactivate_trivial_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/detect_fixed_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/equality_propagate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/induced_linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/init_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/int_to_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/remove_zero_terms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/strip_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/var_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/zero_sum_propagator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.653650 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_bounds_to_vars_xfrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_constraint_tightener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_deactivate_trivial_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_detect_fixed_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_equality_propagate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_induced_linearity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_init_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_int_to_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_strip_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_var_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_zero_sum_propagate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_zero_term_removal.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/preprocessing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.653650 Pyomo-6.6.0/pyomo/contrib/pynumero/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.653650 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.653650 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/cyipopt_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    24973 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/implicit_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/pyomo_ext_cyipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    17076 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/scipy_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/square_solver_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.653650 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/test_implicit_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/test_pyomo_ext_cyipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)    22682 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/test_scipy_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/asl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.653650 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.653650 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/callback/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/callback/cyipopt_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/callback/cyipopt_callback_halt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/callback/cyipopt_functor_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/callback/reactor_design.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.653650 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.653650 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/param_est/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/param_est/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/param_est/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/param_est/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/param_est/perform_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.657650 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/react_example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/react_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_ratio_residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/feasibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/mumps_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/nlp_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/nlp_interface_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/parallel_matvec.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/parallel_vector_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/sqp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.657650 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/tests/test_cyipopt_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/examples/tests/test_mpi_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.657650 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33715 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/ampl_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13388 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/cyipopt_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/external_grey_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/external_pyomo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/nlp_projections.py
--rw-r--r--   0 runner    (1001) docker     (123)    33215 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/pyomo_grey_box_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    59681 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/pyomo_nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.657650 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/compare_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/external_grey_box_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_cyipopt_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    23094 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_dynamic_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_external_asl_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    86169 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_external_grey_box_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    43340 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    43266 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    33269 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23319 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_nlp_projections.py
--rw-r--r--   0 runner    (1001) docker     (123)   102434 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_pyomo_grey_box_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/intrinsic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.657650 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/ma27.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/ma27_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/ma57.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/ma57_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/mumps_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/scipy_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.661650 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/tests/test_linear_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/tests/test_ma27.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/tests/test_ma57.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/tests/test_mumps_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.661650 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/base_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    46496 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/block_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    59918 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/block_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/mpi_block_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    55787 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/mpi_block_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.661650 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32251 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_block_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    36356 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_block_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_intrinsics.py
--rw-r--r--   0 runner    (1001) docker     (123)    53461 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    62153 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_sparse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.661650 Pyomo-6.6.0/pyomo/contrib/pynumero/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/src/AmplInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/src/AmplInterface.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/src/AssertUtils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/src/ma27Interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/src/ma57Interface.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.661650 Pyomo-6.6.0/pyomo/contrib/pynumero/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/src/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/src/tests/simple_nlp.nl
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/src/tests/simple_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.661650 Pyomo-6.6.0/pyomo/contrib/pynumero/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pynumero/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.661650 Pyomo-6.6.0/pyomo/contrib/pyros/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pyros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29849 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pyros/master_problem_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    35206 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pyros/pyros.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pyros/pyros_algorithm_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    43608 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pyros/separation_problem_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    24240 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pyros/solve_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.661650 Pyomo-6.6.0/pyomo/contrib/pyros/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pyros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   206920 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pyros/tests/test_grcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    96394 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pyros/uncertainty_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)    57837 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/pyros/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.665650 Pyomo-6.6.0/pyomo/contrib/satsolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/satsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/satsolver/satsolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/satsolver/test_satsolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.665650 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.665650 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9721 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/HIV_Transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/feedbackController.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/parameter_kaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/rangeInequality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/rooney_biegler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/k_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    27828 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/sens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.665650 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/tests/test_k_aug_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    34637 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/tests/test_sens.py
--rw-r--r--   0 runner    (1001) docker     (123)    34792 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/tests/test_sens_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.665650 Pyomo-6.6.0/pyomo/contrib/simplemodel/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/simplemodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.665650 Pyomo-6.6.0/pyomo/contrib/trustregion/
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/TRF.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.665650 Pyomo-6.6.0/pyomo/contrib/trustregion/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2294 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/examples/example1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/examples/example2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.665650 Pyomo-6.6.0/pyomo/contrib/trustregion/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/tests/test_TRF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/trustregion/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.665650 Pyomo-6.6.0/pyomo/contrib/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/main.ui
--rw-r--r--   0 runner    (1001) docker     (123)    22117 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/model_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/model_browser.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/model_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/model_select.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/pyomo_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/residual_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/residual_table.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.669650 Pyomo-6.6.0/pyomo/contrib/viewer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/tests/test_data_model_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/tests/test_data_model_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/contrib/viewer/ui_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.669650 Pyomo-6.6.0/pyomo/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.673650 Pyomo-6.6.0/pyomo/core/base/
--rw-r--r--   0 runner    (1001) docker     (123)    34605 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/PyomoModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    92221 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/blockutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/boolean_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/check.py
--rw-r--r--   0 runner    (1001) docker     (123)    40011 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/component_namer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/component_order.py
--rw-r--r--   0 runner    (1001) docker     (123)    25954 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/componentuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    38405 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/disable_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/global_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    47362 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/indexed_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    41755 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/indexed_component_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/instance2dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/logical_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/matrix_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/numvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)    20043 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    35750 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/param.py
--rw-r--r--   0 runner    (1001) docker     (123)    58687 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/piecewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    35299 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/range.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/rangeset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32911 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)   154605 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/set.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/set_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/sets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/sos.py
--rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/symbol_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/template_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    58224 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/units_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    35769 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/base/var.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.673650 Pyomo-6.6.0/pyomo/core/beta/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/beta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/beta/dict_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/beta/list_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.673650 Pyomo-6.6.0/pyomo/core/expr/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/boolean_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.673650 Pyomo-6.6.0/pyomo/core/expr/calculus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/calculus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/calculus/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/calculus/diff_with_pyomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/calculus/diff_with_sympy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/cnf_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/expr_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/expr_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/logical_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    91757 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/numeric_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    32280 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/numvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/relational_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/symbol_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/sympy_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/taylor_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    38066 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/template_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    58576 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/expr/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.677651 Pyomo-6.6.0/pyomo/core/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/component_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/component_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    29756 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/conic.py
--rw-r--r--   0 runner    (1001) docker     (123)    29434 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/container_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/dict_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/heterogeneous_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/homogeneous_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/list_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/matrix_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.677651 Pyomo-6.6.0/pyomo/core/kernel/piecewise_library/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/piecewise_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45131 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/piecewise_library/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/piecewise_library/transforms_nd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/piecewise_library/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/register_numpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/set_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/sos.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/tuple_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/kernel/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.677651 Pyomo-6.6.0/pyomo/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.677651 Pyomo-6.6.0/pyomo/core/plugins/transform/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/add_slack_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/discrete_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/eliminate_fixed_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/equality_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/expand_connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/logical_to_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/nonnegative_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/radix_linearization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/relax_integrality.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/standard_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/plugins/transform/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/pyomoobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/staleflag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.677651 Pyomo-6.6.0/pyomo/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.677651 Pyomo-6.6.0/pyomo/core/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/data/test_odbc_ini.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.677651 Pyomo-6.6.0/pyomo/core/tests/diet/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/diet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/diet/test_diet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.681650 Pyomo-6.6.0/pyomo/core/tests/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/examples/pmedian.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/examples/pmedian1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/examples/pmedian2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/examples/pmedian4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/examples/test_amplbook2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/examples/test_kernel_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/examples/test_pyomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/examples/test_tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.681650 Pyomo-6.6.0/pyomo/core/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/transform/test_add_slacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/transform/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    29458 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/transform/test_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.689651 Pyomo-6.6.0/pyomo/core/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.689651 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    88988 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_component_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_component_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    30208 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_conic.py
--rw-r--r--   0 runner    (1001) docker     (123)    68680 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    36873 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_dict_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    24614 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_list_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    44828 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_matrix_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    39687 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_piecewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_sos.py
--rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)    31639 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_tuple_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    37512 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_action.py
--rw-r--r--   0 runner    (1001) docker     (123)   116672 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_block_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_componentuid.py
--rw-r--r--   0 runner    (1001) docker     (123)    56939 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_con.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_concrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    30492 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_derivs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_dict_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_disable_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_expr_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_external.py
--rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)    29172 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_indexed_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)    26513 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_kernel_register_numpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_labelers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_list_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_logical_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_logical_expr_expanded.py
--rw-r--r--   0 runner    (1001) docker     (123)    33829 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_logical_to_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_matrix_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    36104 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_mutable.py
--rw-r--r--   0 runner    (1001) docker     (123)   196231 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_numeric_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    41263 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_numeric_expr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   276875 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_numeric_expr_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)   250800 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_numeric_expr_zerofilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_numpy_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_numvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    75413 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_param.py
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_piecewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    34645 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_range.py
--rw-r--r--   0 runner    (1001) docker     (123)    46148 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15319 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_relational_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)   223573 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_set.py
--rw-r--r--   0 runner    (1001) docker     (123)   129623 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_smap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_sos.py
--rw-r--r--   0 runner    (1001) docker     (123)    65846 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_suffix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_symbol_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_taylor_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    26144 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_template_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    46205 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    59145 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_var.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_var_set_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    60219 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/test_xfrm_discrete_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/uninstantiated_model_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/tests/unit/uninstantiated_model_quadratic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.689651 Pyomo-6.6.0/pyomo/dae/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/contset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/diffvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    24249 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/integral.py
--rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.689651 Pyomo-6.6.0/pyomo/dae/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27279 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/plugins/colloc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/plugins/finitedifference.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/set_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.693651 Pyomo-6.6.0/pyomo/dae/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25303 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/test_colloc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/test_contset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/test_diffvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/test_finite_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    78715 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/test_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/test_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/test_integral.py
--rw-r--r--   0 runner    (1001) docker     (123)    35439 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/test_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/tests/test_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    71365 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dae/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.693651 Pyomo-6.6.0/pyomo/dataportal/
--rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/DataPortal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/TableData.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15965 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/parse_datacmds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.693651 Pyomo-6.6.0/pyomo/dataportal/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/plugins/csv_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/plugins/datacommands.py
--rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/plugins/db_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/plugins/json_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/plugins/sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/plugins/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/plugins/xml_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    33388 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/process_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.693651 Pyomo-6.6.0/pyomo/dataportal/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/tests/test_dat_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    80115 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/dataportal/tests/test_dataportal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.693651 Pyomo-6.6.0/pyomo/duality/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/duality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/duality/collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/duality/lagrangian_dual.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/duality/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.693651 Pyomo-6.6.0/pyomo/duality/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/duality/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/duality/tests/test_linear_dual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.693651 Pyomo-6.6.0/pyomo/environ/
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/environ/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.693651 Pyomo-6.6.0/pyomo/environ/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/environ/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/environ/tests/standalone_minimal_pyomo_driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/environ/tests/test_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/environ/tests/test_package_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.693651 Pyomo-6.6.0/pyomo/gdp/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/basic_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/disjunct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.697651 Pyomo-6.6.0/pyomo/gdp/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/between_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/bigm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/bigm_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/bilinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/bound_pretransformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/chull.py
--rw-r--r--   0 runner    (1001) docker     (123)    52037 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/cuttingplane.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/fix_disjuncts.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/gdp_to_mip_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/gdp_var_mover.py
--rw-r--r--   0 runner    (1001) docker     (123)    43911 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/hull.py
--rw-r--r--   0 runner    (1001) docker     (123)    31121 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/multiple_bigm.py
--rw-r--r--   0 runner    (1001) docker     (123)    38530 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/plugins/partition_disjuncts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.697651 Pyomo-6.6.0/pyomo/gdp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69861 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/common_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    34783 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_basic_step.py
--rw-r--r--   0 runner    (1001) docker     (123)   114035 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_bigm.py
--rw-r--r--   0 runner    (1001) docker     (123)    30686 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_bound_pretransformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    49436 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_cuttingplane.py
--rw-r--r--   0 runner    (1001) docker     (123)    25476 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_disjunct.py
--rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_fix_disjuncts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_gdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_gdp_reclassification_error.py
--rw-r--r--   0 runner    (1001) docker     (123)   107329 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_hull.py
--rw-r--r--   0 runner    (1001) docker     (123)    34192 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_mbigm.py
--rw-r--r--   0 runner    (1001) docker     (123)    88882 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_partition_disjuncts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_reclassify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/transformed_disjunct.py
--rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/gdp/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.697651 Pyomo-6.6.0/pyomo/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/kernel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.697651 Pyomo-6.6.0/pyomo/mpec/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/complementarity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.697651 Pyomo-6.6.0/pyomo/mpec/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/plugins/mpec1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/plugins/mpec2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/plugins/mpec3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/plugins/mpec4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/plugins/pathampl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/plugins/solver1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/plugins/solver2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.701650 Pyomo-6.6.0/pyomo/mpec/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/tests/test_complementarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/tests/test_minlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/tests/test_nlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/mpec/tests/test_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.701650 Pyomo-6.6.0/pyomo/neos/
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/neos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/neos/kestrel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.701650 Pyomo-6.6.0/pyomo/neos/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/neos/plugins/NEOS.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/neos/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/neos/plugins/kestrel_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.701650 Pyomo-6.6.0/pyomo/neos/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/neos/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/neos/tests/model_min_lp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/neos/tests/test_neos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.701650 Pyomo-6.6.0/pyomo/network/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/arc.py
--rw-r--r--   0 runner    (1001) docker     (123)    39258 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)    34795 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/foqus_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.701650 Pyomo-6.6.0/pyomo/network/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/plugins/expand_arcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29294 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.701650 Pyomo-6.6.0/pyomo/network/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86491 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/tests/test_arc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29150 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/tests/test_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)    17236 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/tests/test_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/network/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.701650 Pyomo-6.6.0/pyomo/opt/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.701650 Pyomo-6.6.0/pyomo/opt/base/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/base/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/base/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/base/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/base/opt_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/base/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/base/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    28146 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/base/solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.701650 Pyomo-6.6.0/pyomo/opt/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/parallel/async_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/parallel/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/parallel/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.705651 Pyomo-6.6.0/pyomo/opt/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/plugins/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/plugins/res.py
--rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/plugins/sol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.705651 Pyomo-6.6.0/pyomo/opt/problem/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/problem/ampl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.705651 Pyomo-6.6.0/pyomo/opt/results/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/results/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/results/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/results/results_.py
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/results/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/results/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.705651 Pyomo-6.6.0/pyomo/opt/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/solver/ilmcmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/solver/shellcmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.705651 Pyomo-6.6.0/pyomo/opt/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/testing/pyunit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.705651 Pyomo-6.6.0/pyomo/opt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.709651 Pyomo-6.6.0/pyomo/opt/tests/base/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/tests/base/test_ampl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/tests/base/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/tests/base/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/tests/base/test_sol.py
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/tests/base/test_soln.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/tests/base/test_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.709651 Pyomo-6.6.0/pyomo/opt/tests/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/tests/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/opt/tests/solver/test_shellcmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.709651 Pyomo-6.6.0/pyomo/pysp/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/pysp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.713651 Pyomo-6.6.0/pyomo/repn/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.713651 Pyomo-6.6.0/pyomo/repn/beta/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/beta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24946 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/beta/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    30869 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.713651 Pyomo-6.6.0/pyomo/repn/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.713651 Pyomo-6.6.0/pyomo/repn/plugins/ampl/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/plugins/ampl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79887 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/plugins/ampl/ampl_.py
--rw-r--r--   0 runner    (1001) docker     (123)    31663 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/plugins/baron_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/plugins/cpxlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    39974 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/plugins/gams_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/plugins/lp_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32022 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/plugins/mps.py
--rw-r--r--   0 runner    (1001) docker     (123)    99140 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/plugins/nl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13519 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/quadratic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/standard_aux.py
--rw-r--r--   0 runner    (1001) docker     (123)    59218 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/standard_repn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.717651 Pyomo-6.6.0/pyomo/repn/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.717651 Pyomo-6.6.0/pyomo/repn/tests/ampl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/nl_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small10_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small11_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small12_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small13_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small14_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small15_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small1_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small2_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small3_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small4_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small5_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small6_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small7_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small8_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/small9_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/test_ampl_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/test_ampl_nl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/test_ampl_repn.py
--rw-r--r--   0 runner    (1001) docker     (123)    34709 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/test_nlv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/ampl/test_suffixes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.717651 Pyomo-6.6.0/pyomo/repn/tests/baron/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/baron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/baron/small14a_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/baron/test_baron.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/baron/test_baron_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.717651 Pyomo-6.6.0/pyomo/repn/tests/cpxlp/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/cpxlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/cpxlp/test_cpxlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/diffutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.721651 Pyomo-6.6.0/pyomo/repn/tests/gams/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/gams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/gams/small14a_testCase.py
--rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/gams/test_gams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/gams/test_gams_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/lp_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.721651 Pyomo-6.6.0/pyomo/repn/tests/mps/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/mps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/mps/test_mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/nl_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    49439 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/test_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/test_quadratic.py
--rw-r--r--   0 runner    (1001) docker     (123)   163933 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/test_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)    24202 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/repn/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.721651 Pyomo-6.6.0/pyomo/scripting/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/driver_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.721651 Pyomo-6.6.0/pyomo/scripting/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/plugins/build_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/plugins/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/plugins/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/plugins/extras.py
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/plugins/solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/pyomo_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/pyomo_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/pyomo_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/solve_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.721651 Pyomo-6.6.0/pyomo/scripting/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/tests/test_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)    42600 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/scripting/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.721651 Pyomo-6.6.0/pyomo/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/mockmip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.721651 Pyomo-6.6.0/pyomo/solvers/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.721651 Pyomo-6.6.0/pyomo/solvers/plugins/converter/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/converter/ampl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/converter/glpsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/converter/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/converter/pico.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.725651 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/ASL.py
--rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/BARON.py
--rw-r--r--   0 runner    (1001) docker     (123)    50993 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/CBCplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/CONOPT.py
--rw-r--r--   0 runner    (1001) docker     (123)    46100 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/CPLEX.py
--rw-r--r--   0 runner    (1001) docker     (123)    56740 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/GAMS.py
--rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/GLPK.py
--rw-r--r--   0 runner    (1001) docker     (123)    22792 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/GUROBI.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/GUROBI_RUN.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/IPOPT.py
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/SCIPAMPL.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/XPRESS.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41128 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/cplex_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/cplex_persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/direct_or_persistent_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/direct_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    41308 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/gurobi_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)    24856 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/gurobi_persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    54400 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/mosek_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/mosek_persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23614 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/persistent_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/pywrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    44160 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/xpress_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/plugins/solvers/xpress_persistent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.725651 Pyomo-6.6.0/pyomo/solvers/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.725651 Pyomo-6.6.0/pyomo/solvers/tests/checks/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_BARON.py
--rw-r--r--   0 runner    (1001) docker     (123)    19032 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_CBCplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21968 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_CPLEXDirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_CPLEXPersistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_GAMS.py
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_MOSEKDirect.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_MOSEKPersistent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_cbc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_cplex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_gurobi.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_gurobi_persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_no_solution_behavior.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/checks/test_xpress_persistent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.729651 Pyomo-6.6.0/pyomo/solvers/tests/mip/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/test_asl.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/test_ipopt.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/test_mip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/test_scip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/test_scip_log_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/test_scip_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/mip/test_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.729651 Pyomo-6.6.0/pyomo/solvers/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_compiled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_constant_objective1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_constant_objective2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_duals_maximize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_duals_minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_inactive_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_infeasible1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_infeasible2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_piecewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_trivial_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_unbounded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_unique_duals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/LP_unused_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/MILP_discrete_var_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/MILP_infeasible1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/MILP_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/MILP_unbounded.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/MILP_unused_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/MIQCP_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/MIQP_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/QCP_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/QP_constant_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/QP_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/SOS1_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/SOS2_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.729651 Pyomo-6.6.0/pyomo/solvers/tests/piecewise_linear/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/piecewise_linear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/piecewise_linear/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/tests/testcases.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/solvers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.729651 Pyomo-6.6.0/pyomo/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/blockutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/calc_var_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/check_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/components.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/infeasible.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/model_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/report_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/slices.py
--rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/subsystems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.733651 Pyomo-6.6.0/pyomo/util/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/tests/test_blockutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/tests/test_calc_var_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/tests/test_check_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/tests/test_infeasible.py
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/tests/test_model_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/tests/test_report_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    28108 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/tests/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)    28274 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/tests/test_subsystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/util/vars_from_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.733651 Pyomo-6.6.0/pyomo/version/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/version/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:09:31.733651 Pyomo-6.6.0/pyomo/version/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/version/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/version/tests/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-24 22:09:20.000000 Pyomo-6.6.0/pyomo/version/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-24 22:09:31.733651 Pyomo-6.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11828 2023-05-24 22:09:20.000000 Pyomo-6.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.371044 Pyomo-6.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-30 19:53:34.000000 Pyomo-6.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 19:53:34.000000 Pyomo-6.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-30 19:53:45.371044 Pyomo-6.6.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.215042 Pyomo-6.6.1/Pyomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-05-30 19:53:44.000000 Pyomo-6.6.1/Pyomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    49708 2023-05-30 19:53:45.000000 Pyomo-6.6.1/Pyomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:53:44.000000 Pyomo-6.6.1/Pyomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 19:53:44.000000 Pyomo-6.6.1/Pyomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-30 19:53:44.000000 Pyomo-6.6.1/Pyomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 19:53:44.000000 Pyomo-6.6.1/Pyomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-30 19:53:34.000000 Pyomo-6.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.215042 Pyomo-6.6.1/pyomo/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.219042 Pyomo-6.6.1/pyomo/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12462 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/autoslots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/backports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/cmake_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.219042 Pyomo-6.6.1/pyomo/common/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/collections/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/collections/component_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/collections/component_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/collections/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93516 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27155 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21295 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14411 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26360 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/gc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/getGSL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/gsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/numeric_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/pyomo_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16094 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tempfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.223042 Pyomo-6.6.1/pyomo/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/config_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/dep_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/dep_mod_except.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/import_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/relo_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/relo_mod_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/relocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_bunch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108896 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15597 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23914 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16629 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_multithread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24109 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/tests/test_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36980 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19118 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/common/unittest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.223042 Pyomo-6.6.1/pyomo/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.223042 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.223042 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/src/FindASL.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/src/functions.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.223042 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/tests/test_ampl_function_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.223042 Pyomo-6.6.1/pyomo/contrib/appsi/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63191 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.223042 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.227042 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/cmodel_bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    68508 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/expression.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32798 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/expression.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/fbbt_model.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/fbbt_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32293 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/interval.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5245 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/interval.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13751 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/lp_writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/lp_writer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/model_base.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/model_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17203 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/nl_writer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/nl_writer.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.227042 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.227042 Pyomo-6.6.1/pyomo/contrib/appsi/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/examples/getting_started.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.227042 Pyomo-6.6.1/pyomo/contrib/appsi/examples/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/examples/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/examples/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11009 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/fbbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.227042 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17164 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/cbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16611 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/cplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60137 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/gurobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28563 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/highs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19154 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/ipopt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.227042 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23165 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/tests/test_gurobi_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/tests/test_ipopt_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49399 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/solvers/tests/test_persistent_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.227042 Pyomo-6.6.1/pyomo/contrib/appsi/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/tests/test_fbbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/tests/test_interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.227042 Pyomo-6.6.1/pyomo/contrib/appsi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/utils/collect_vars_and_named_exprs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/utils/get_objective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/appsi/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/utils/tests/test_collect_vars_and_named_exprs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/appsi/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/writers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/writers/lp_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/writers/nl_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/appsi/writers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/writers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/appsi/writers/tests/test_nl_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/benders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/benders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/benders/benders_cuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/benders/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/benders/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/benders/examples/farmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/benders/examples/grothey_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/benders/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/benders/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/benders/tests/test_benders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/community_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/community_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/community_detection/community_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41063 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/community_detection/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/community_detection/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/community_detection/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/community_detection/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/community_detection/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63498 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/community_detection/tests/test_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/cp/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/interval_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/cp/repn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/repn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46867 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/repn/docplex_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/cp/scheduling_expr/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/scheduling_expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/scheduling_expr/precedence_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/scheduling_expr/step_function_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/cp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50133 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/tests/test_docplex_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/tests/test_docplex_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/tests/test_interval_var.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23110 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/tests/test_logical_to_disjunctive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/tests/test_precedence_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19693 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/tests/test_step_function_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.231042 Pyomo-6.6.1/pyomo/contrib/cp/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/transform/logical_to_disjunctive_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/cp/transform/logical_to_disjunctive_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/doe/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45358 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/doe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/doe/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/examples/reactor_compute_FIM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/examples/reactor_grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/examples/reactor_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/examples/reactor_optimize_doe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29563 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/doe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/tests/test_fim_doe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/doe/tests/test_reactor_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/example/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/example/foo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/example/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/example/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/example/plugins/ex_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/example/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/example/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/example/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/fbbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fbbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63827 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fbbt/fbbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fbbt/interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/fbbt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fbbt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43511 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fbbt/tests/test_fbbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fbbt/tests/test_interval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/fme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32588 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fme/fourier_motzkin_elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fme/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/fme/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fme/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38423 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/fme/tests/test_fourier_motzkin_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/gdp_bounds/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdp_bounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdp_bounds/compute_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdp_bounds/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdp_bounds/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.235042 Pyomo-6.6.1/pyomo/contrib/gdp_bounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdp_bounds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdp_bounds/tests/test_gdp_bounds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.239042 Pyomo-6.6.1/pyomo/contrib/gdpopt/
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/GDPopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/algorithm_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25992 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/branch_and_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/config_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/create_oa_subproblems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/cut_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/discrete_problem_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/gloa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/loa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/nlp_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/oa_algorithm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/ric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/solve_discrete_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/solve_subproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.239042 Pyomo-6.6.1/pyomo/contrib/gdpopt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/tests/common_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/tests/test_LBB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/tests/test_enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72674 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/tests/test_gdpopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21219 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gdpopt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.239042 Pyomo-6.6.1/pyomo/contrib/gjh/
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gjh/GJH.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gjh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gjh/getGJH.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/gjh/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.239042 Pyomo-6.6.1/pyomo/contrib/iis/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/iis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/iis/iis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.239042 Pyomo-6.6.1/pyomo/contrib/iis/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/iis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/iis/tests/test_iis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.243043 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.243043 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/common/dulmage_mendelsohn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.243043 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/common/tests/test_dulmage_mendelsohn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/dulmage_mendelsohn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/incidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36014 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/scc_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.243043 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/models_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_connected.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_dulmage_mendelsohn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_incidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70937 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18355 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_scc_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15890 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_triangularize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/triangularize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/incidence_analysis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.243043 Pyomo-6.6.1/pyomo/contrib/interior_point/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.243043 Pyomo-6.6.1/pyomo/contrib/interior_point/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/examples/ex1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18769 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27675 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/interior_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/inverse_reduced_hessian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.243043 Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/base_linear_solver_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/ma27_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/mumps_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/scipy_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.243043 Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/tests/test_linear_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/tests/test_realloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.243043 Pyomo-6.6.1/pyomo/contrib/interior_point/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/tests/test_interior_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/tests/test_inverse_reduced_hessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/tests/test_realloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/interior_point/tests/test_reg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.243043 Pyomo-6.6.1/pyomo/contrib/mcpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mcpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mcpp/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mcpp/getMCPP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mcpp/mcppInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mcpp/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mcpp/pyomo_mcpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mcpp/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12697 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mcpp/test_mcpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.247043 Pyomo-6.6.1/pyomo/contrib/mindtpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/MindtPy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133902 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/algorithm_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26506 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/config_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16924 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/cut_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/extended_cutting_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/feasibility_pump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/global_outer_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19645 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/mip_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20919 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/nlp_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/outer_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45090 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/single_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tabu_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/MINLP2_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/MINLP3_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/MINLP4_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/MINLP5_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/MINLP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/constraint_qualification_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/eight_process_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/feasibility_pump1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/feasibility_pump2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/from_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/nonconvex1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/nonconvex2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/nonconvex3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/nonconvex4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/online_doc_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19324 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_ECP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_feas_pump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_global_lp_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_lp_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_solution_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51099 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mindtpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mpc/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/dynamic_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/find_nearest_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/get_cuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/interval_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/scalar_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/series_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_find_nearest_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_get_cuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_interval_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_scalar_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_series_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mpc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/run_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/run_openloop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/tests/test_openloop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/copy_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15717 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/model_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23841 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/tests/test_var_linker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/var_linker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mpc/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/modeling/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/modeling/cost_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/modeling/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.251043 Pyomo-6.6.1/pyomo/contrib/mpc/modeling/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/modeling/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21740 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/modeling/tests/test_cost_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/modeling/tests/test_input_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/mpc/modeling/tests/test_terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.255043 Pyomo-6.6.1/pyomo/contrib/multistart/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/multistart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/multistart/high_conf_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/multistart/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/multistart/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/multistart/reinit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/multistart/test_multi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.255043 Pyomo-6.6.1/pyomo/contrib/parmest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.255043 Pyomo-6.6.1/pyomo/contrib/parmest/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.255043 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reaction_kinetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reaction_kinetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reaction_kinetics/simple_reaction_parmest_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.255043 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/bootstrap_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/datarec_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/leaveNout_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/likelihood_ratio_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/multisensor_data_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/parameter_estimation_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/reactor_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/timeseries_data_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.255043 Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/bootstrap_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/likelihood_ratio_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/parameter_estimation_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler_with_constraint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.255043 Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/parallel_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/parameter_estimation_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/scenario_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/semibatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21310 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/ipopt_solver_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51757 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/parmest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/scenariocreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.255043 Pyomo-6.6.1/pyomo/contrib/parmest/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35606 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_parmest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_scenariocreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.259043 Pyomo-6.6.1/pyomo/contrib/parmest/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13160 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/utils/create_ef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/utils/ipopt_solver_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/utils/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/utils/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/parmest/utils/scenario_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.259043 Pyomo-6.6.1/pyomo/contrib/piecewise/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/piecewise_linear_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/piecewise_linear_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.259043 Pyomo-6.6.1/pyomo/contrib/piecewise/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/tests/common_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/tests/test_inner_repn_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/tests/test_outer_repn_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19998 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/tests/test_piecewise_linear_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/tests/test_reduced_inner_repn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.259043 Pyomo-6.6.1/pyomo/contrib/piecewise/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/transform/convex_combination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/transform/disaggregated_convex_combination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/transform/inner_representation_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/transform/multiple_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/transform/outer_representation_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/transform/piecewise_to_gdp_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/transform/piecewise_to_mip_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/piecewise/transform/reduced_inner_representation_gdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.259043 Pyomo-6.6.1/pyomo/contrib/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.259043 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/bounds_to_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/constraint_tightener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/deactivate_trivial_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/detect_fixed_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9848 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/equality_propagate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16533 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/induced_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/init_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/int_to_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/remove_zero_terms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/strip_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/var_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/zero_sum_propagator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.263043 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_bounds_to_vars_xfrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_constraint_tightener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_deactivate_trivial_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_detect_fixed_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_equality_propagate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_induced_linearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_init_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_int_to_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_strip_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_var_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_zero_sum_propagate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_zero_term_removal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/preprocessing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.263043 Pyomo-6.6.1/pyomo/contrib/pynumero/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.263043 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.263043 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/cyipopt_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24973 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/implicit_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/pyomo_ext_cyipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17076 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/scipy_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/square_solver_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.263043 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9184 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/test_implicit_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14262 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/test_pyomo_ext_cyipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22682 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/test_scipy_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/asl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.263043 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.267043 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/callback/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/callback/cyipopt_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/callback/cyipopt_callback_halt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/callback/cyipopt_functor_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/callback/reactor_design.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.267043 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.267043 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/param_est/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/param_est/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/param_est/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/param_est/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/param_est/perform_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.267043 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/react_example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/react_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_ratio_residuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_residuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/feasibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/mumps_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/nlp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/nlp_interface_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/parallel_matvec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/parallel_vector_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/sqp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.267043 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/tests/test_cyipopt_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/examples/tests/test_mpi_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.267043 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33715 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/ampl_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13388 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/cyipopt_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17555 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/external_grey_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/external_pyomo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16595 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/nlp_projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33215 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/pyomo_grey_box_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59681 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/pyomo_nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.271043 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/compare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21183 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/external_grey_box_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_cyipopt_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23094 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_dynamic_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_external_asl_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86169 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_external_grey_box_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43340 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43266 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33269 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23319 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_nlp_projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102434 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_pyomo_grey_box_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/intrinsic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.271043 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/ma27.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/ma27_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/ma57.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/ma57_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/mumps_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/scipy_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.271043 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/tests/test_linear_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/tests/test_ma27.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/tests/test_ma57.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/tests/test_mumps_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.271043 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/base_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46496 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/block_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59918 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/block_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/mpi_block_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55787 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/mpi_block_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.271043 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32251 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_block_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36356 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_block_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_intrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53461 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62153 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_sparse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.275043 Pyomo-6.6.1/pyomo/contrib/pynumero/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18075 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/src/AmplInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/src/AmplInterface.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/src/AssertUtils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/src/ma27Interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/src/ma57Interface.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.275043 Pyomo-6.6.1/pyomo/contrib/pynumero/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/src/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/src/tests/simple_nlp.nl
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/src/tests/simple_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.275043 Pyomo-6.6.1/pyomo/contrib/pynumero/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pynumero/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.275043 Pyomo-6.6.1/pyomo/contrib/pyros/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pyros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29849 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pyros/master_problem_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35206 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pyros/pyros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pyros/pyros_algorithm_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43608 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pyros/separation_problem_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24240 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pyros/solve_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.275043 Pyomo-6.6.1/pyomo/contrib/pyros/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pyros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   206920 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pyros/tests/test_grcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96394 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pyros/uncertainty_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57837 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/pyros/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.275043 Pyomo-6.6.1/pyomo/contrib/satsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/satsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/satsolver/satsolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/satsolver/test_satsolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.279043 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.279043 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9721 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/HIV_Transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/feedbackController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/parameter_kaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/rangeInequality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/rooney_biegler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/k_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27828 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/sens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.279043 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/tests/test_k_aug_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34637 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/tests/test_sens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34792 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/tests/test_sens_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.279043 Pyomo-6.6.1/pyomo/contrib/simplemodel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/simplemodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.283043 Pyomo-6.6.1/pyomo/contrib/trustregion/
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/TRF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.283043 Pyomo-6.6.1/pyomo/contrib/trustregion/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2294 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/examples/example1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/examples/example2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.283043 Pyomo-6.6.1/pyomo/contrib/trustregion/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/tests/test_TRF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20844 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/trustregion/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.287043 Pyomo-6.6.1/pyomo/contrib/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/main.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    22117 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/model_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/model_browser.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/model_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/model_select.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/pyomo_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/residual_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/residual_table.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.287043 Pyomo-6.6.1/pyomo/contrib/viewer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/tests/test_data_model_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/tests/test_data_model_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/contrib/viewer/ui_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.287043 Pyomo-6.6.1/pyomo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.299043 Pyomo-6.6.1/pyomo/core/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    34605 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/PyomoModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92221 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/blockutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/boolean_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40011 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/component_namer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/component_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25954 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/componentuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38405 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/disable_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/global_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47362 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/indexed_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41827 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/indexed_component_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/instance2dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/logical_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/matrix_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/numvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20043 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35750 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58687 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/piecewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35299 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32911 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154605 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/set_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/sos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/symbol_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/template_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58224 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/units_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35769 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/base/var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.299043 Pyomo-6.6.1/pyomo/core/beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/beta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/beta/dict_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/beta/list_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.303043 Pyomo-6.6.1/pyomo/core/expr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15308 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/boolean_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.303043 Pyomo-6.6.1/pyomo/core/expr/calculus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/calculus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/calculus/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/calculus/diff_with_pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/calculus/diff_with_sympy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/cnf_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/expr_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/expr_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/logical_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91757 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/numeric_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32280 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/numvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/relational_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/symbol_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/sympy_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/taylor_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38066 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/template_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58576 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/expr/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.303043 Pyomo-6.6.1/pyomo/core/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/component_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/component_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29756 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/conic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29434 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/container_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/dict_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/heterogeneous_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/homogeneous_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/list_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15732 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/matrix_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.303043 Pyomo-6.6.1/pyomo/core/kernel/piecewise_library/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/piecewise_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45131 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/piecewise_library/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/piecewise_library/transforms_nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/piecewise_library/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/register_numpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/set_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/sos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/tuple_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/kernel/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.303043 Pyomo-6.6.1/pyomo/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.307043 Pyomo-6.6.1/pyomo/core/plugins/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/add_slack_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/discrete_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/eliminate_fixed_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/equality_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/expand_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16656 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/logical_to_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/nonnegative_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/radix_linearization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/relax_integrality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/standard_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/plugins/transform/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/pyomoobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/staleflag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.307043 Pyomo-6.6.1/pyomo/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.307043 Pyomo-6.6.1/pyomo/core/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/data/test_odbc_ini.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.307043 Pyomo-6.6.1/pyomo/core/tests/diet/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/diet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/diet/test_diet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.307043 Pyomo-6.6.1/pyomo/core/tests/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/examples/pmedian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/examples/pmedian1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/examples/pmedian2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/examples/pmedian4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/examples/test_amplbook2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/examples/test_kernel_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12765 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/examples/test_pyomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/examples/test_tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.307043 Pyomo-6.6.1/pyomo/core/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24260 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/transform/test_add_slacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/transform/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29458 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/transform/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.315044 Pyomo-6.6.1/pyomo/core/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.319044 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88988 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_component_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_component_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30208 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_conic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68680 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36873 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_dict_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24614 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_list_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44828 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_matrix_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39687 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_piecewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_sos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31639 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_tuple_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37512 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116672 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_block_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_componentuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56939 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_con.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_concrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30492 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_derivs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14215 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_dict_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_disable_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_expr_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35904 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29152 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_indexed_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26513 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_kernel_register_numpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_labelers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_list_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_logical_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_logical_expr_expanded.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33829 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_logical_to_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_matrix_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36104 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_mutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)   196231 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_numeric_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41263 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_numeric_expr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   276875 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_numeric_expr_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   250800 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_numeric_expr_zerofilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_numpy_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16093 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_numvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75413 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_piecewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34645 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46148 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15319 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_relational_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   223573 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129623 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_smap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_sos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65846 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_symbol_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_taylor_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26144 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_template_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46205 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59145 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_var_set_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60219 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/test_xfrm_discrete_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/uninstantiated_model_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/tests/unit/uninstantiated_model_quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.319044 Pyomo-6.6.1/pyomo/dae/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11294 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/contset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/diffvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24249 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18691 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.319044 Pyomo-6.6.1/pyomo/dae/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27279 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/plugins/colloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/plugins/finitedifference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.319044 Pyomo-6.6.1/pyomo/dae/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25303 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/test_colloc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/test_contset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/test_diffvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/test_finite_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78715 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/test_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/test_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/test_integral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35439 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/test_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49558 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/tests/test_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71365 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dae/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.323044 Pyomo-6.6.1/pyomo/dataportal/
+-rw-r--r--   0 runner    (1001) docker     (123)    14942 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/DataPortal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/TableData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15965 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/parse_datacmds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.323044 Pyomo-6.6.1/pyomo/dataportal/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/plugins/csv_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/plugins/datacommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/plugins/db_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/plugins/json_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/plugins/sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/plugins/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/plugins/xml_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33388 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/process_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.323044 Pyomo-6.6.1/pyomo/dataportal/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/tests/test_dat_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80115 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/dataportal/tests/test_dataportal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.323044 Pyomo-6.6.1/pyomo/duality/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/duality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9830 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/duality/collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/duality/lagrangian_dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/duality/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.323044 Pyomo-6.6.1/pyomo/duality/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/duality/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/duality/tests/test_linear_dual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.323044 Pyomo-6.6.1/pyomo/environ/
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/environ/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.323044 Pyomo-6.6.1/pyomo/environ/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/environ/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/environ/tests/standalone_minimal_pyomo_driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/environ/tests/test_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/environ/tests/test_package_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.323044 Pyomo-6.6.1/pyomo/gdp/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/basic_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/disjunct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.327044 Pyomo-6.6.1/pyomo/gdp/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/between_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/bigm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/bigm_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/bilinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/bound_pretransformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/chull.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52037 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/cuttingplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/fix_disjuncts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/gdp_to_mip_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/gdp_var_mover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43911 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/hull.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31121 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/multiple_bigm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38530 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/plugins/partition_disjuncts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.327044 Pyomo-6.6.1/pyomo/gdp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69861 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/common_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34783 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_basic_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114035 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_bigm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30686 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_bound_pretransformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49436 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_cuttingplane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25476 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_disjunct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6774 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_fix_disjuncts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_gdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_gdp_reclassification_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107329 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_hull.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34192 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_mbigm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88882 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_partition_disjuncts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_reclassify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/transformed_disjunct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/gdp/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.327044 Pyomo-6.6.1/pyomo/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/kernel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.327044 Pyomo-6.6.1/pyomo/mpec/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/complementarity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/mpec/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/plugins/mpec1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/plugins/mpec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/plugins/mpec3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/plugins/mpec4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/plugins/pathampl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/plugins/solver1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/plugins/solver2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/mpec/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/tests/test_complementarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/tests/test_minlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/tests/test_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/mpec/tests/test_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/neos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/neos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15676 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/neos/kestrel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/neos/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/neos/plugins/NEOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/neos/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/neos/plugins/kestrel_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/neos/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/neos/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/neos/tests/model_min_lp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/neos/tests/test_neos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39258 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34795 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/foqus_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/network/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/plugins/expand_arcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29294 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/network/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86491 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/tests/test_arc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29150 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/tests/test_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17236 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/tests/test_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/network/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/opt/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/base/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/base/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/base/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/base/opt_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/base/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/base/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28146 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/base/solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.331044 Pyomo-6.6.1/pyomo/opt/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/parallel/async_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/parallel/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7718 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/parallel/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/opt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/plugins/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/plugins/res.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12025 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/plugins/sol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/opt/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/problem/ampl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/opt/results/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/results/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/results/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/results/results_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/results/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/results/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/opt/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/solver/ilmcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/solver/shellcmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/opt/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/testing/pyunit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/opt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/opt/tests/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/tests/base/test_ampl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/tests/base/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/tests/base/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/tests/base/test_sol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/tests/base/test_soln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/tests/base/test_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/opt/tests/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/tests/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/opt/tests/solver/test_shellcmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/pysp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/pysp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/repn/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/repn/beta/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/beta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24946 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/beta/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30916 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.335044 Pyomo-6.6.1/pyomo/repn/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.339044 Pyomo-6.6.1/pyomo/repn/plugins/ampl/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/plugins/ampl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79887 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/plugins/ampl/ampl_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31663 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/plugins/baron_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/plugins/cpxlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39974 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/plugins/gams_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22297 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/plugins/lp_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32022 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/plugins/mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99145 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/plugins/nl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13519 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/standard_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59218 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/standard_repn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.339044 Pyomo-6.6.1/pyomo/repn/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.347044 Pyomo-6.6.1/pyomo/repn/tests/ampl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/nl_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small10_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small11_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small12_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small13_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small14_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small15_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small1_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small2_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small3_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small4_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small5_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small6_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small7_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small8_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/small9_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/test_ampl_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/test_ampl_nl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/test_ampl_repn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36728 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/test_nlv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/ampl/test_suffixes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.347044 Pyomo-6.6.1/pyomo/repn/tests/baron/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/baron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/baron/small14a_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/baron/test_baron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/baron/test_baron_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.347044 Pyomo-6.6.1/pyomo/repn/tests/cpxlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/cpxlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/cpxlp/test_cpxlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/diffutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.351044 Pyomo-6.6.1/pyomo/repn/tests/gams/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/gams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/gams/small14a_testCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/gams/test_gams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/gams/test_gams_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/lp_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.351044 Pyomo-6.6.1/pyomo/repn/tests/mps/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/mps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/mps/test_mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/nl_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49872 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/test_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/test_quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163933 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/test_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24202 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16155 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/repn/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.351044 Pyomo-6.6.1/pyomo/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/driver_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.355044 Pyomo-6.6.1/pyomo/scripting/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/plugins/build_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/plugins/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/plugins/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/plugins/extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/plugins/solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/pyomo_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/pyomo_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/pyomo_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15111 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/solve_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.355044 Pyomo-6.6.1/pyomo/scripting/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/tests/test_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42600 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/scripting/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.355044 Pyomo-6.6.1/pyomo/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/mockmip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.355044 Pyomo-6.6.1/pyomo/solvers/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.355044 Pyomo-6.6.1/pyomo/solvers/plugins/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/converter/ampl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/converter/glpsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/converter/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/converter/pico.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.363044 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/ASL.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24289 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/BARON.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50993 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/CBCplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/CONOPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46100 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/CPLEX.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56740 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/GAMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21966 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/GLPK.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22792 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/GUROBI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/GUROBI_RUN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/IPOPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/SCIPAMPL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/XPRESS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41128 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/cplex_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/cplex_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/direct_or_persistent_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/direct_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/gurobi_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24856 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/gurobi_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54400 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/mosek_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/mosek_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23614 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/persistent_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/pywrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44160 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/xpress_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/plugins/solvers/xpress_persistent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.363044 Pyomo-6.6.1/pyomo/solvers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.363044 Pyomo-6.6.1/pyomo/solvers/tests/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_BARON.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19032 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_CBCplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21968 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_CPLEXDirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_CPLEXPersistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19126 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_GAMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_MOSEKDirect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_MOSEKPersistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_cbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_cplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_gurobi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16409 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_gurobi_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_gurobi_persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_no_solution_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11840 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/checks/test_xpress_persistent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.363044 Pyomo-6.6.1/pyomo/solvers/tests/mip/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/test_asl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/test_ipopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/test_mip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/test_scip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/test_scip_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10703 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/test_scip_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/mip/test_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.367045 Pyomo-6.6.1/pyomo/solvers/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_compiled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_constant_objective1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_constant_objective2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_duals_maximize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_duals_minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_inactive_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_infeasible1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_infeasible2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_piecewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_trivial_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_unbounded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_unique_duals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/LP_unused_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/MILP_discrete_var_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/MILP_infeasible1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/MILP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/MILP_unbounded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/MILP_unused_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/MIQCP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/MIQP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/QCP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/QP_constant_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/QP_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/SOS1_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/SOS2_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.367045 Pyomo-6.6.1/pyomo/solvers/tests/piecewise_linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/piecewise_linear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/piecewise_linear/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19851 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/tests/testcases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/solvers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.371044 Pyomo-6.6.1/pyomo/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/blockutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/calc_var_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/check_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/infeasible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/model_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/report_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10600 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/subsystems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.371044 Pyomo-6.6.1/pyomo/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/tests/test_blockutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/tests/test_calc_var_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/tests/test_check_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/tests/test_infeasible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/tests/test_model_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/tests/test_report_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28108 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28274 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/tests/test_subsystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/util/vars_from_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.371044 Pyomo-6.6.1/pyomo/version/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/version/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:53:45.371044 Pyomo-6.6.1/pyomo/version/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/version/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/version/tests/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-30 19:53:34.000000 Pyomo-6.6.1/pyomo/version/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-30 19:53:45.371044 Pyomo-6.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-30 19:53:34.000000 Pyomo-6.6.1/setup.py
```

### Comparing `Pyomo-6.6.0/LICENSE.md` & `Pyomo-6.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/PKG-INFO` & `Pyomo-6.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyomo
-Version: 6.6.0
+Version: 6.6.1
 Summary: Pyomo: Python Optimization Modeling Objects
 Home-page: http://pyomo.org
 Maintainer: Pyomo Developer Team
 Maintainer-email: pyomo-developers@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://pyomo.readthedocs.io/
 Project-URL: Source, https://github.com/Pyomo/pyomo
```

### Comparing `Pyomo-6.6.0/Pyomo.egg-info/PKG-INFO` & `Pyomo-6.6.1/Pyomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyomo
-Version: 6.6.0
+Version: 6.6.1
 Summary: Pyomo: Python Optimization Modeling Objects
 Home-page: http://pyomo.org
 Maintainer: Pyomo Developer Team
 Maintainer-email: pyomo-developers@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://pyomo.readthedocs.io/
 Project-URL: Source, https://github.com/Pyomo/pyomo
```

### Comparing `Pyomo-6.6.0/Pyomo.egg-info/SOURCES.txt` & `Pyomo-6.6.1/Pyomo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1136,14 +1136,15 @@
 pyomo/solvers/tests/checks/test_CPLEXPersistent.py
 pyomo/solvers/tests/checks/test_GAMS.py
 pyomo/solvers/tests/checks/test_MOSEKDirect.py
 pyomo/solvers/tests/checks/test_MOSEKPersistent.py
 pyomo/solvers/tests/checks/test_cbc.py
 pyomo/solvers/tests/checks/test_cplex.py
 pyomo/solvers/tests/checks/test_gurobi.py
+pyomo/solvers/tests/checks/test_gurobi_direct.py
 pyomo/solvers/tests/checks/test_gurobi_persistent.py
 pyomo/solvers/tests/checks/test_no_solution_behavior.py
 pyomo/solvers/tests/checks/test_pickle.py
 pyomo/solvers/tests/checks/test_writers.py
 pyomo/solvers/tests/checks/test_xpress_persistent.py
 pyomo/solvers/tests/mip/__init__.py
 pyomo/solvers/tests/mip/model.py
```

### Comparing `Pyomo-6.6.0/README.md` & `Pyomo-6.6.1/README.md`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/__init__.py` & `Pyomo-6.6.1/pyomo/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/__init__.py` & `Pyomo-6.6.1/pyomo/common/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/_command.py` & `Pyomo-6.6.1/pyomo/common/_command.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/_common.py` & `Pyomo-6.6.1/pyomo/common/_common.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/autoslots.py` & `Pyomo-6.6.1/pyomo/common/autoslots.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/backports.py` & `Pyomo-6.6.1/pyomo/common/backports.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/cmake_builder.py` & `Pyomo-6.6.1/pyomo/common/cmake_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,18 @@
     else:
         raise
 
 
 def build_cmake_project(
     targets, package_name=None, description=None, user_args=[], parallel=None
 ):
-    import distutils.core
+    # Note: setuptools must be imported before distutils to avoid
+    # warnings / errors with recent setuptools distributions
     from setuptools import Extension
+    import distutils.core
     from distutils.command.build_ext import build_ext
 
     class _CMakeBuild(build_ext, object):
         def run(self):
             for cmake_ext in self.extensions:
                 self._cmake_build_target(cmake_ext)
```

### Comparing `Pyomo-6.6.0/pyomo/common/collections/__init__.py` & `Pyomo-6.6.1/pyomo/common/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/collections/bunch.py` & `Pyomo-6.6.1/pyomo/common/collections/bunch.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/collections/component_map.py` & `Pyomo-6.6.1/pyomo/common/collections/component_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/collections/component_set.py` & `Pyomo-6.6.1/pyomo/common/collections/component_set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/collections/orderedset.py` & `Pyomo-6.6.1/pyomo/common/collections/orderedset.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/config.py` & `Pyomo-6.6.1/pyomo/common/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1289,25 +1289,27 @@
         _item_body_formatter = lambda doc: pattern
 
     def _item_body_cb(self, indent, obj):
         _doc = obj._doc or obj._description or ""
         if not _doc:
             return ''
         wraplines = '\n ' not in _doc
-        _doc = _item_body_formatter(_doc).strip()
+        _doc = _item_body_formatter(_doc).rstrip()
         if not _doc:
             return ''
         _indent = indent + ' ' * self.indent_spacing
         if wraplines:
             doc_lines = textwrap.wrap(
                 _doc, self.width, initial_indent=_indent, subsequent_indent=_indent
             )
             self.out.write(('\n'.join(doc_lines)).rstrip() + '\n')
+        elif _doc.lstrip() == _doc:
+            self.out.write(_indent + _doc + '\n')
         else:
-            self.out.write(_doc.rstrip() + '\n')
+            self.out.write(_doc + '\n')
 
     return types.MethodType(_item_body_cb, formatter)
 
 
 class ConfigFormatter(object):
     def _initialize(self, indent_spacing, width, visibility):
         self.out = io.StringIO()
```

### Comparing `Pyomo-6.6.0/pyomo/common/dependencies.py` & `Pyomo-6.6.1/pyomo/common/dependencies.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/deprecation.py` & `Pyomo-6.6.1/pyomo/common/deprecation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/download.py` & `Pyomo-6.6.1/pyomo/common/download.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/env.py` & `Pyomo-6.6.1/pyomo/common/env.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/envvar.py` & `Pyomo-6.6.1/pyomo/common/envvar.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/errors.py` & `Pyomo-6.6.1/pyomo/common/errors.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/extensions.py` & `Pyomo-6.6.1/pyomo/common/extensions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/factory.py` & `Pyomo-6.6.1/pyomo/common/factory.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/fileutils.py` & `Pyomo-6.6.1/pyomo/common/fileutils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/formatting.py` & `Pyomo-6.6.1/pyomo/common/formatting.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/gc_manager.py` & `Pyomo-6.6.1/pyomo/common/gc_manager.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/getGSL.py` & `Pyomo-6.6.1/pyomo/common/getGSL.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/gsl.py` & `Pyomo-6.6.1/pyomo/common/gsl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/log.py` & `Pyomo-6.6.1/pyomo/common/log.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/modeling.py` & `Pyomo-6.6.1/pyomo/common/modeling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/multithread.py` & `Pyomo-6.6.1/pyomo/common/multithread.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/numeric_types.py` & `Pyomo-6.6.1/pyomo/common/numeric_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/plugin.py` & `Pyomo-6.6.1/pyomo/common/plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/plugin_base.py` & `Pyomo-6.6.1/pyomo/common/plugin_base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/plugins.py` & `Pyomo-6.6.1/pyomo/common/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/pyomo_typing.py` & `Pyomo-6.6.1/pyomo/common/pyomo_typing.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/shutdown.py` & `Pyomo-6.6.1/pyomo/common/shutdown.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/sorting.py` & `Pyomo-6.6.1/pyomo/common/sorting.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tee.py` & `Pyomo-6.6.1/pyomo/common/tee.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tempfiles.py` & `Pyomo-6.6.1/pyomo/common/tempfiles.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/__init__.py` & `Pyomo-6.6.1/pyomo/common/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/config_plugin.py` & `Pyomo-6.6.1/pyomo/common/tests/config_plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/dep_mod.py` & `Pyomo-6.6.1/pyomo/common/tests/dep_mod.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/dep_mod_except.py` & `Pyomo-6.6.1/pyomo/common/tests/dep_mod_except.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/deps.py` & `Pyomo-6.6.1/pyomo/common/tests/deps.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/relo_mod.py` & `Pyomo-6.6.1/pyomo/common/tests/relo_mod.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/relo_mod_new.py` & `Pyomo-6.6.1/pyomo/common/tests/relo_mod_new.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/relocated.py` & `Pyomo-6.6.1/pyomo/common/tests/relocated.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_bunch.py` & `Pyomo-6.6.1/pyomo/common/tests/test_bunch.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_config.py` & `Pyomo-6.6.1/pyomo/common/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,77 @@
 
 
 class GlobalClass(object):
     "test class for test_known_types"
     pass
 
 
+def ExampleConfig():
+    CONFIG = ConfigDict()
+    CONFIG.declare(
+        'option_1',
+        ConfigValue(default=5, domain=int, doc='The first configuration option'),
+    )
+    SOLVER = CONFIG.declare('solver_options', ConfigDict())
+    SOLVER.declare(
+        'solver_option_1',
+        ConfigValue(
+            default=1,
+            domain=float,
+            doc='The first solver configuration option',
+            visibility=DEVELOPER_OPTION,
+        ),
+    )
+    SOLVER.declare(
+        'solver_option_2',
+        ConfigValue(
+            default=1,
+            domain=float,
+            doc="""The second solver configuration option
+
+        With a very long line containing
+        wrappable text in a long, silly paragraph
+        with little actual information.
+        #) but a bulleted list
+        #) with two bullets
+        """,
+        ),
+    )
+    SOLVER.declare(
+        'solver_option_3',
+        ConfigValue(
+            default=1,
+            domain=float,
+            doc="""
+            The third solver configuration option
+
+            This has a leading newline and a very long line containing
+            wrappable text in a long, silly paragraph with
+            little actual information.
+
+         .. and_a_list::
+            #) but a bulleted list
+            #) with two bullets """,
+        ),
+    )
+    CONFIG.declare(
+        'option_2',
+        ConfigValue(
+            default=5,
+            domain=int,
+            doc="""The second solver configuration option
+        with a very long line containing
+        wrappable text in a long, silly paragraph
+        with little actual information.
+        """,
+        ),
+    )
+    return CONFIG
+
+
 class TestConfigDomains(unittest.TestCase):
     def test_Bool(self):
         c = ConfigDict()
         c.declare('a', ConfigValue(True, Bool))
         self.assertEqual(c.a, True)
         c.a = False
         self.assertEqual(c.a, False)
@@ -1728,15 +1791,15 @@
     endItem{epanet file}
   endBlock{network}
   startItem{scenario}
     item{Single scenario block}
   endItem{scenario}
   startBlock{scenario}
     startItem{scenario file}
-item{This is the (long) documentation for the 'scenario file'
+      item{This is the (long) documentation for the 'scenario file'
 parameter.  It contains multiple lines, and some internal
 formatting; like a bulleted list:
   - item 1
   - item 2
 }
     endItem{scenario file}
     startItem{merlion}
@@ -1749,15 +1812,15 @@
     endItem{detection}
   endBlock{scenario}
   startItem{scenarios}
     item{List of scenario blocks}
   endItem{scenarios}
   startBlock{scenarios}
     startItem{scenario file}
-item{This is the (long) documentation for the 'scenario file'
+      item{This is the (long) documentation for the 'scenario file'
 parameter.  It contains multiple lines, and some internal
 formatting; like a bulleted list:
   - item 1
   - item 2
 }
     endItem{scenario file}
     startItem{merlion}
@@ -1953,14 +2016,71 @@
         with self.assertRaisesRegex(
             ValueError, "Unrecognized documentation formatter, 'unknown'"
         ):
             cfg.generate_documentation(format="unknown")
 
         self.assertEqual(cfg.generate_documentation(format=ConfigFormatter()), '')
 
+    def test_generate_documentation_StringFormatter(self):
+        # This test verifies behavior with simple StringFormatters (in
+        # particular, the handling of newlines and indentation reported
+        # in #IDAES/idaes-pse#1191)
+        CONFIG = ExampleConfig()
+        doc = CONFIG.generate_documentation(
+            format=String_ConfigFormatter(
+                block_start="",  # %s\n",
+                block_end="",
+                item_start="%s\n",
+                item_body="%s",
+                item_end="\n",
+            ),
+            indent_spacing=4,
+            width=66,
+        )
+
+        # print(doc)
+        ref = """    option_1
+        The first configuration option
+
+    solver_options
+
+        solver_option_1
+            The first solver configuration option
+
+        solver_option_2
+            The second solver configuration option
+
+        With a very long line containing
+        wrappable text in a long, silly paragraph
+        with little actual information.
+        #) but a bulleted list
+        #) with two bullets
+
+        solver_option_3
+            The third solver configuration option
+
+            This has a leading newline and a very long line containing
+            wrappable text in a long, silly paragraph with
+            little actual information.
+
+         .. and_a_list::
+            #) but a bulleted list
+            #) with two bullets
+
+    option_2
+        The second solver configuration option with a very long
+        line containing wrappable text in a long, silly paragraph
+        with little actual information.
+
+"""
+        self.assertEqual(
+            [_.rstrip() for _ in ref.splitlines()],
+            [_.rstrip() for _ in doc.splitlines()],
+        )
+
     def test_block_get(self):
         self.assertTrue('scenario' in self.config)
         self.assertNotEqual(self.config.get('scenario', 'bogus').value(), 'bogus')
         self.assertFalse('fubar' in self.config)
         self.assertEqual(self.config.get('fubar', 'bogus').value(), 'bogus')
 
         cfg = ConfigDict()
@@ -2789,58 +2909,15 @@
             cfg2.declare_from({})
 
     def test_docstring_decorator(self):
         self.maxDiff = None
 
         @document_kwargs_from_configdict('CONFIG')
         class ExampleClass(object):
-            CONFIG = ConfigDict()
-            CONFIG.declare(
-                'option_1',
-                ConfigValue(
-                    default=5, domain=int, doc='The first configuration option'
-                ),
-            )
-            SOLVER = CONFIG.declare('solver_options', ConfigDict())
-            SOLVER.declare(
-                'solver_option_1',
-                ConfigValue(
-                    default=1,
-                    domain=float,
-                    doc='The first solver configuration option',
-                    visibility=DEVELOPER_OPTION,
-                ),
-            )
-            SOLVER.declare(
-                'solver_option_2',
-                ConfigValue(
-                    default=1,
-                    domain=float,
-                    doc="""The second solver configuration option
-
-                With a very long line containing
-                wrappable text in a long, silly paragraph
-                with little actual information.
-                #) but a bulleted list
-                #) with two bullets
-                """,
-                ),
-            )
-            CONFIG.declare(
-                'option_2',
-                ConfigValue(
-                    default=5,
-                    domain=int,
-                    doc="""The second solver configuration option
-                with a very long line containing
-                wrappable text in a long, silly paragraph
-                with little actual information.
-                """,
-                ),
-            )
+            CONFIG = ExampleConfig()
 
             @document_kwargs_from_configdict(CONFIG)
             def __init__(self):
                 "A simple docstring"
 
             @document_kwargs_from_configdict(
                 CONFIG, doc="A simple docstring\n", visibility=USER_OPTION
@@ -2865,14 +2942,25 @@
         The second solver configuration option
 
         With a very long line containing wrappable text in a long, silly
         paragraph with little actual information.
         #) but a bulleted list
         #) with two bullets
 
+    solver_option_3: float, default=1
+        The third solver configuration option
+
+           This has a leading newline and a very long line containing
+           wrappable text in a long, silly paragraph with little actual
+           information.
+
+        .. and_a_list::
+           #) but a bulleted list
+           #) with two bullets
+
 option_2: int, default=5
     The second solver configuration option with a very long line
     containing wrappable text in a long, silly paragraph with little
     actual information."""
         self.assertEqual(ExampleClass.__doc__, ref.lstrip())
         self.assertEqual(ExampleClass.__init__.__doc__, "A simple docstring\n" + ref)
 
@@ -2888,14 +2976,25 @@
         The second solver configuration option
 
         With a very long line containing wrappable text in a long, silly
         paragraph with little actual information.
         #) but a bulleted list
         #) with two bullets
 
+    solver_option_3: float, default=1
+        The third solver configuration option
+
+           This has a leading newline and a very long line containing
+           wrappable text in a long, silly paragraph with little actual
+           information.
+
+        .. and_a_list::
+           #) but a bulleted list
+           #) with two bullets
+
 option_2: int, default=5
     The second solver configuration option with a very long line
     containing wrappable text in a long, silly paragraph with little
     actual information."""
         self.assertEqual(ExampleClass.fcn.__doc__, "A simple docstring\n" + ref)
 
         ref = """
@@ -2909,14 +3008,23 @@
     solver_option_2: float, default=1
         The second solver configuration option
 
         With a very long line containing wrappable text in a long, silly paragraph with little actual information.
         #) but a bulleted list
         #) with two bullets
 
+    solver_option_3: float, default=1
+        The third solver configuration option
+
+           This has a leading newline and a very long line containing wrappable text in a long, silly paragraph with little actual information.
+
+        .. and_a_list::
+           #) but a bulleted list
+           #) with two bullets
+
 option_2: int, default=5
     The second solver configuration option with a very long line containing wrappable text in a long, silly paragraph with little actual information."""
         with LoggingIntercept() as LOG:
             self.assertEqual(add_docstring_list("", ExampleClass.CONFIG), ref)
         self.assertIn('add_docstring_list is deprecated', LOG.getvalue())
```

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_dependencies.py` & `Pyomo-6.6.1/pyomo/common/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_deprecated.py` & `Pyomo-6.6.1/pyomo/common/tests/test_deprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,23 +55,23 @@
         self.assertIn(
             '(deprecated in 1.2, will be removed in (or after) 3.4)',
             DEP_OUT.getvalue().replace('\n', ' '),
         )
 
     def test_no_version_exception(self):
         with self.assertRaisesRegex(
-            DeveloperError, "@deprecated\(\): missing 'version' argument"
+            DeveloperError, r"@deprecated\(\): missing 'version' argument"
         ):
 
             @deprecated()
             def foo():
                 pass
 
         with self.assertRaisesRegex(
-            DeveloperError, "@deprecated\(\): missing 'version' argument"
+            DeveloperError, r"@deprecated\(\): missing 'version' argument"
         ):
 
             @deprecated()
             class foo(object):
                 pass
 
         # But no exception if the class can infer a version from the
@@ -258,15 +258,15 @@
         class foo(object):
             def __init__(self):
                 logger.warning('yeah')
 
         self.assertIs(type(foo), type)
         self.assertRegex(
             foo.__doc__,
-            r'.. deprecated:: test\n' r'   This class \(.*\.foo\) has been deprecated',
+            r'.. deprecated:: test\n   This class \(.*\.foo\) has been deprecated',
         )
 
         # Test the default argument
         DEP_OUT = StringIO()
         FCN_OUT = StringIO()
         with LoggingIntercept(DEP_OUT, 'pyomo'):
             with LoggingIntercept(FCN_OUT, 'local'):
```

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_download.py` & `Pyomo-6.6.1/pyomo/common/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_env.py` & `Pyomo-6.6.1/pyomo/common/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_errors.py` & `Pyomo-6.6.1/pyomo/common/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_fileutils.py` & `Pyomo-6.6.1/pyomo/common/tests/test_fileutils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_formatting.py` & `Pyomo-6.6.1/pyomo/common/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_gc.py` & `Pyomo-6.6.1/pyomo/common/tests/test_gc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_log.py` & `Pyomo-6.6.1/pyomo/common/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_modeling.py` & `Pyomo-6.6.1/pyomo/common/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_multithread.py` & `Pyomo-6.6.1/pyomo/common/tests/test_multithread.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_orderedset.py` & `Pyomo-6.6.1/pyomo/common/tests/test_orderedset.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_plugin.py` & `Pyomo-6.6.1/pyomo/common/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_sorting.py` & `Pyomo-6.6.1/pyomo/common/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_tee.py` & `Pyomo-6.6.1/pyomo/common/tests/test_tee.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_tempfile.py` & `Pyomo-6.6.1/pyomo/common/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_timing.py` & `Pyomo-6.6.1/pyomo/common/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_typing.py` & `Pyomo-6.6.1/pyomo/common/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/tests/test_unittest.py` & `Pyomo-6.6.1/pyomo/common/tests/test_unittest.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/timing.py` & `Pyomo-6.6.1/pyomo/common/timing.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/common/unittest.py` & `Pyomo-6.6.1/pyomo/common/unittest.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,15 +464,15 @@
             _save_re = self.expected_regex
             self.expected_regex = None
             if not super().__exit__(exc_type, exc_value, tb):
                 return False
         finally:
             self.expected_regex = _save_re
 
-        exc_value = re.sub('(?s)\s+', ' ', str(exc_value))
+        exc_value = re.sub(r'(?s)\s+', ' ', str(exc_value))
         if not _save_re.search(exc_value):
             self._raiseFailure(
                 '"{}" does not match "{}"'.format(_save_re.pattern, exc_value)
             )
         return True
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/build.py` & `Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/build.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/src/CMakeLists.txt` & `Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/src/FindASL.cmake` & `Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/src/FindASL.cmake`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/src/functions.c` & `Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/src/functions.c`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/ampl_function_demo/tests/test_ampl_function_demo.py` & `Pyomo-6.6.1/pyomo/contrib/ampl_function_demo/tests/test_ampl_function_demo.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/base.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/build.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/build.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/cmodel_bindings.cpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/cmodel_bindings.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/expression.cpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/expression.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/expression.hpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/expression.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/fbbt_model.cpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/fbbt_model.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/fbbt_model.hpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/fbbt_model.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/interval.cpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/interval.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/interval.hpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/interval.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/lp_writer.cpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/lp_writer.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/lp_writer.hpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/lp_writer.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/model_base.cpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/model_base.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/model_base.hpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/model_base.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/nl_writer.cpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/nl_writer.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/src/nl_writer.hpp` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/src/nl_writer.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/cmodel/tests/test_import.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/cmodel/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/examples/getting_started.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/examples/getting_started.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/examples/tests/test_examples.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/examples/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/fbbt.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/fbbt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/solvers/cbc.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/solvers/cbc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/solvers/cplex.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/solvers/cplex.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/solvers/gurobi.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/solvers/gurobi.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/solvers/highs.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/solvers/highs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/solvers/ipopt.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/solvers/ipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/solvers/tests/test_gurobi_persistent.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/solvers/tests/test_gurobi_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/solvers/tests/test_ipopt_persistent.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/solvers/tests/test_ipopt_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/solvers/tests/test_persistent_solvers.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/solvers/tests/test_persistent_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/tests/test_base.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/tests/test_fbbt.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/tests/test_fbbt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/tests/test_interval.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/tests/test_interval.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/utils/collect_vars_and_named_exprs.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/utils/collect_vars_and_named_exprs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/utils/tests/test_collect_vars_and_named_exprs.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/utils/tests/test_collect_vars_and_named_exprs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/writers/lp_writer.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/writers/lp_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/writers/nl_writer.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/writers/nl_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/appsi/writers/tests/test_nl_writer.py` & `Pyomo-6.6.1/pyomo/contrib/appsi/writers/tests/test_nl_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/benders/benders_cuts.py` & `Pyomo-6.6.1/pyomo/contrib/benders/benders_cuts.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/benders/examples/farmer.py` & `Pyomo-6.6.1/pyomo/contrib/benders/examples/farmer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/benders/examples/grothey_ex.py` & `Pyomo-6.6.1/pyomo/contrib/benders/examples/grothey_ex.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/benders/tests/test_benders.py` & `Pyomo-6.6.1/pyomo/contrib/benders/tests/test_benders.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/community_detection/community_graph.py` & `Pyomo-6.6.1/pyomo/contrib/community_detection/community_graph.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/community_detection/detection.py` & `Pyomo-6.6.1/pyomo/contrib/community_detection/detection.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/community_detection/event_log.py` & `Pyomo-6.6.1/pyomo/contrib/community_detection/event_log.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/community_detection/tests/test_detection.py` & `Pyomo-6.6.1/pyomo/contrib/community_detection/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/interval_var.py` & `Pyomo-6.6.1/pyomo/contrib/cp/interval_var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/cp/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/repn/docplex_writer.py` & `Pyomo-6.6.1/pyomo/contrib/cp/repn/docplex_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/scheduling_expr/precedence_expressions.py` & `Pyomo-6.6.1/pyomo/contrib/cp/scheduling_expr/precedence_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/scheduling_expr/step_function_expressions.py` & `Pyomo-6.6.1/pyomo/contrib/cp/scheduling_expr/step_function_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/tests/test_docplex_walker.py` & `Pyomo-6.6.1/pyomo/contrib/cp/tests/test_docplex_walker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/tests/test_docplex_writer.py` & `Pyomo-6.6.1/pyomo/contrib/cp/tests/test_docplex_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/tests/test_interval_var.py` & `Pyomo-6.6.1/pyomo/contrib/cp/tests/test_interval_var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/tests/test_logical_to_disjunctive.py` & `Pyomo-6.6.1/pyomo/contrib/cp/tests/test_logical_to_disjunctive.py`

 * *Files 4% similar despite different names*

```diff
@@ -279,14 +279,94 @@
             self, m.disjuncts[1].constraint.expr, m.z[1] + m.z[2] + m.z[3] <= 1
         )
 
         assertExpressionsEqual(
             self, m.cons[1].expr, m.disjuncts[0].binary_indicator_var >= 1
         )
 
+    def test_boolean_fixed_true(self):
+        m = self.make_model()
+        e = m.a.implies(m.b)
+        m.a.fix(True)
+
+        visitor = LogicalToDisjunctiveVisitor()
+        m.cons = visitor.constraints
+        m.z = visitor.z_vars
+        m.disjuncts = visitor.disjuncts
+        m.disjunctions = visitor.disjunctions
+
+        visitor.walk_expression(e)
+        # we'll get !a v b
+        self.assertEqual(len(m.z), 3)
+        self.assertEqual(len(m.cons), 4)
+
+        self.assertIs(m.a.get_associated_binary(), m.z[1])
+        self.assertTrue(m.z[1].fixed)
+        self.assertEqual(value(m.z[1]), 1)
+        self.assertIs(m.b.get_associated_binary(), m.z[2])
+
+        assertExpressionsEqual(
+            self, m.cons[1].expr, (1 - m.z[3]) + (1 - m.z[1]) + m.z[2] >= 1
+        )
+        assertExpressionsEqual(self, m.cons[2].expr, 1 - (1 - m.z[1]) + m.z[3] >= 1)
+        assertExpressionsEqual(self, m.cons[3].expr, m.z[3] + (1 - m.z[2]) >= 1)
+        assertExpressionsEqual(self, m.cons[4].expr, m.z[3] >= 1)
+
+    def test_boolean_fixed_false(self):
+        m = self.make_model()
+        e = m.a & m.b
+        m.a.fix(False)
+
+        visitor = LogicalToDisjunctiveVisitor()
+        m.cons = visitor.constraints
+        m.z = visitor.z_vars
+        m.disjuncts = visitor.disjuncts
+        m.disjunctions = visitor.disjunctions
+
+        visitor.walk_expression(e)
+        # we'll get !a v b
+        self.assertEqual(len(m.z), 3)
+        self.assertEqual(len(m.cons), 3)
+
+        self.assertIs(m.a.get_associated_binary(), m.z[1])
+        self.assertTrue(m.z[1].fixed)
+        self.assertEqual(value(m.z[1]), 0)
+        self.assertIs(m.b.get_associated_binary(), m.z[2])
+
+        assertExpressionsEqual(self, m.cons[1].expr, m.z[1] >= m.z[3])
+        assertExpressionsEqual(self, m.cons[2].expr, m.z[2] >= m.z[3])
+        assertExpressionsEqual(self, m.cons[3].expr, m.z[3] >= 1)
+
+    def test_boolean_fixed_none(self):
+        m = self.make_model()
+        e = m.a & m.b
+        # I don't get what this means, but you can do it, so... I guess we need
+        # to handle it.
+        m.a.fix(None)
+
+        visitor = LogicalToDisjunctiveVisitor()
+        m.cons = visitor.constraints
+        m.z = visitor.z_vars
+        m.disjuncts = visitor.disjuncts
+        m.disjunctions = visitor.disjunctions
+
+        visitor.walk_expression(e)
+        # we'll get !a v b
+        self.assertEqual(len(m.z), 3)
+        self.assertEqual(len(m.cons), 3)
+
+        self.assertIs(m.a.get_associated_binary(), m.z[1])
+        self.assertTrue(m.z[1].fixed)
+        self.assertIsNone(m.z[1].value)
+        self.assertIs(m.b.get_associated_binary(), m.z[2])
+
+        assertExpressionsEqual(self, m.cons[1].expr, m.z[1] >= m.z[3])
+        assertExpressionsEqual(self, m.cons[2].expr, m.z[2] >= m.z[3])
+        assertExpressionsEqual(self, m.cons[3].expr, m.z[3] >= 1)
+
     def test_no_need_to_walk(self):
         m = self.make_model()
         e = m.a
 
         visitor = LogicalToDisjunctiveVisitor()
         m.cons = visitor.constraints
         m.z = visitor.z_vars
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/tests/test_precedence_constraints.py` & `Pyomo-6.6.1/pyomo/contrib/cp/tests/test_precedence_constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/tests/test_step_function_expressions.py` & `Pyomo-6.6.1/pyomo/contrib/cp/tests/test_step_function_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/transform/logical_to_disjunctive_program.py` & `Pyomo-6.6.1/pyomo/contrib/cp/transform/logical_to_disjunctive_program.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/cp/transform/logical_to_disjunctive_walker.py` & `Pyomo-6.6.1/pyomo/contrib/cp/transform/logical_to_disjunctive_walker.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,19 @@
         binary = node.get_associated_binary()
         if binary is not None:
             visitor.boolean_to_binary_map[node] = binary
         else:
             z = visitor.z_vars.add()
             visitor.boolean_to_binary_map[node] = z
             node.associate_binary_var(z)
+    if node.fixed:
+        visitor.boolean_to_binary_map[node].fixed = True
+        visitor.boolean_to_binary_map[node].set_value(
+            int(node.value) if node.value is not None else None, skip_validation=True
+        )
     return False, visitor.boolean_to_binary_map[node]
 
 
 def _dispatch_var(visitor, node):
     return False, node
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/doe/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/doe.py` & `Pyomo-6.6.1/pyomo/contrib/doe/doe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1031,15 +1031,15 @@
         def trace_calc(m):
             """
             Calculate FIM elements. Can scale each element with 1000 for performance
             """
             return m.trace == sum(m.fim[j, j] for j in m.regression_parameters)
 
         def det_general(m):
-            """Calculate determinant. Can be applied to FIM of any size.
+            r"""Calculate determinant. Can be applied to FIM of any size.
             det(A) = sum_{\sigma \in \S_n} (sgn(\sigma) * \Prod_{i=1}^n a_{i,\sigma_i})
             Use permutation() to get permutations, sgn() to get signature
             """
             r_list = list(range(len(m.regression_parameters)))
             # get all permutations
             object_p = permutations(r_list)
             list_p = list(object_p)
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/examples/reactor_compute_FIM.py` & `Pyomo-6.6.1/pyomo/contrib/doe/examples/reactor_compute_FIM.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/examples/reactor_grid_search.py` & `Pyomo-6.6.1/pyomo/contrib/doe/examples/reactor_grid_search.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/examples/reactor_kinetics.py` & `Pyomo-6.6.1/pyomo/contrib/doe/examples/reactor_kinetics.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/examples/reactor_optimize_doe.py` & `Pyomo-6.6.1/pyomo/contrib/doe/examples/reactor_optimize_doe.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/measurements.py` & `Pyomo-6.6.1/pyomo/contrib/doe/measurements.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/result.py` & `Pyomo-6.6.1/pyomo/contrib/doe/result.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/scenario.py` & `Pyomo-6.6.1/pyomo/contrib/doe/scenario.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/tests/test_example.py` & `Pyomo-6.6.1/pyomo/contrib/doe/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/tests/test_fim_doe.py` & `Pyomo-6.6.1/pyomo/contrib/doe/tests/test_fim_doe.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/doe/tests/test_reactor_example.py` & `Pyomo-6.6.1/pyomo/contrib/doe/tests/test_reactor_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/example/tests/test_example.py` & `Pyomo-6.6.1/pyomo/contrib/example/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/fbbt/fbbt.py` & `Pyomo-6.6.1/pyomo/contrib/fbbt/fbbt.py`

 * *Files 0% similar despite different names*

```diff
@@ -440,15 +440,15 @@
         If the bounds computed on the body of a constraint violate the bounds of the constraint by more than
         feasibility_tol, then the constraint is considered infeasible and an exception is raised. This tolerance
         is also used when performing certain interval arithmetic operations to ensure that none of the feasible
         region is removed due to floating point arithmetic and to prevent math domain errors (a larger value
         is more conservative).
     """
     if node.expr.__class__ in native_types:
-        expr_lb = expr_up = node.expr
+        expr_lb = expr_ub = node.expr
     else:
         expr_lb, expr_ub = bnds_dict[node.expr]
     bnds_dict[node] = (expr_lb, expr_ub)
 
 
 _prop_bnds_leaf_to_root_map = dict()
 _prop_bnds_leaf_to_root_map[
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/fbbt/interval.py` & `Pyomo-6.6.1/pyomo/contrib/fbbt/interval.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/fbbt/tests/test_fbbt.py` & `Pyomo-6.6.1/pyomo/contrib/fbbt/tests/test_fbbt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1313,11 +1313,25 @@
 
         self.tightener(m)
         self.assertAlmostEqual(m.x.lb, 0)
         self.assertAlmostEqual(m.x.ub, 1)
         self.assertAlmostEqual(m.y.lb, 0)
         self.assertAlmostEqual(m.y.ub, 3)
 
+    def test_named_expr(self):
+        m = pyo.ConcreteModel()
+        m.x = pyo.Var(bounds=(0, None))
+        m.y = pyo.Var(bounds=(1, 6))
+        m.e_const = pyo.Expression(expr=3)
+        m.e_var = pyo.Expression(expr=m.y + m.e_const)
+
+        m.c = pyo.Constraint(expr=m.x**2 == m.e_var)
+
+        self.tightener(m)
+        self.tightener(m)
+        self.assertAlmostEqual(m.x.lb, 2)
+        self.assertAlmostEqual(m.x.ub, 3)
+
 
 class TestFBBT(FbbtTestBase, unittest.TestCase):
     def setUp(self) -> None:
         self.tightener = fbbt
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/fbbt/tests/test_interval.py` & `Pyomo-6.6.1/pyomo/contrib/fbbt/tests/test_interval.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/fme/fourier_motzkin_elimination.py` & `Pyomo-6.6.1/pyomo/contrib/fme/fourier_motzkin_elimination.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/fme/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/fme/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/fme/tests/test_fourier_motzkin_elimination.py` & `Pyomo-6.6.1/pyomo/contrib/fme/tests/test_fourier_motzkin_elimination.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdp_bounds/compute_bounds.py` & `Pyomo-6.6.1/pyomo/contrib/gdp_bounds/compute_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdp_bounds/info.py` & `Pyomo-6.6.1/pyomo/contrib/gdp_bounds/info.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdp_bounds/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/gdp_bounds/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdp_bounds/tests/test_gdp_bounds.py` & `Pyomo-6.6.1/pyomo/contrib/gdp_bounds/tests/test_gdp_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/GDPopt.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/GDPopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/algorithm_base_class.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/algorithm_base_class.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/branch_and_bound.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/branch_and_bound.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/config_options.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/config_options.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/create_oa_subproblems.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/create_oa_subproblems.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/cut_generation.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/cut_generation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/discrete_problem_initialize.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/discrete_problem_initialize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/enumerate.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/enumerate.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/gloa.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/gloa.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/loa.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/loa.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/nlp_initialization.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/nlp_initialization.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/oa_algorithm_utils.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/oa_algorithm_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/ric.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/ric.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/solve_discrete_problem.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/solve_discrete_problem.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/solve_subproblem.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/solve_subproblem.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/tests/common_tests.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/tests/common_tests.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/tests/test_LBB.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/tests/test_LBB.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/tests/test_enumerate.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/tests/test_enumerate.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/tests/test_gdpopt.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/tests/test_gdpopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gdpopt/util.py` & `Pyomo-6.6.1/pyomo/contrib/gdpopt/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gjh/GJH.py` & `Pyomo-6.6.1/pyomo/contrib/gjh/GJH.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gjh/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/gjh/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gjh/getGJH.py` & `Pyomo-6.6.1/pyomo/contrib/gjh/getGJH.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/gjh/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/gjh/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/iis/iis.py` & `Pyomo-6.6.1/pyomo/contrib/iis/iis.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/iis/tests/test_iis.py` & `Pyomo-6.6.1/pyomo/contrib/iis/tests/test_iis.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/common/dulmage_mendelsohn.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/common/dulmage_mendelsohn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/common/tests/test_dulmage_mendelsohn.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/common/tests/test_dulmage_mendelsohn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/config.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/connected.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/connected.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/dulmage_mendelsohn.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/dulmage_mendelsohn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/incidence.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/incidence.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/interface.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/matching.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/matching.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/scc_solver.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/scc_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/models_for_testing.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/models_for_testing.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_connected.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_connected.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_dulmage_mendelsohn.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_dulmage_mendelsohn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_incidence.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_incidence.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_interface.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_matching.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_scc_solver.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_scc_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/tests/test_triangularize.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/tests/test_triangularize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/triangularize.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/triangularize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/incidence_analysis/util.py` & `Pyomo-6.6.1/pyomo/contrib/incidence_analysis/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/examples/ex1.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/examples/ex1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/interface.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/interior_point.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/interior_point.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/inverse_reduced_hessian.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/inverse_reduced_hessian.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/base_linear_solver_interface.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/base_linear_solver_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/ma27_interface.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/ma27_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/mumps_interface.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/mumps_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/scipy_interface.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/scipy_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/tests/test_linear_solvers.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/tests/test_linear_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/linalg/tests/test_realloc.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/linalg/tests/test_realloc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/tests/test_interior_point.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/tests/test_interior_point.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/tests/test_inverse_reduced_hessian.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/tests/test_inverse_reduced_hessian.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/tests/test_realloc.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/tests/test_realloc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/interior_point/tests/test_reg.py` & `Pyomo-6.6.1/pyomo/contrib/interior_point/tests/test_reg.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mcpp/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/mcpp/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mcpp/build.py` & `Pyomo-6.6.1/pyomo/contrib/mcpp/build.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mcpp/getMCPP.py` & `Pyomo-6.6.1/pyomo/contrib/mcpp/getMCPP.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mcpp/mcppInterface.cpp` & `Pyomo-6.6.1/pyomo/contrib/mcpp/mcppInterface.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mcpp/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/mcpp/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mcpp/pyomo_mcpp.py` & `Pyomo-6.6.1/pyomo/contrib/mcpp/pyomo_mcpp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mcpp/setup.py` & `Pyomo-6.6.1/pyomo/contrib/mcpp/setup.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mcpp/test_mcpp.py` & `Pyomo-6.6.1/pyomo/contrib/mcpp/test_mcpp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/MindtPy.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/MindtPy.py`

 * *Files 11% similar despite different names*

```diff
@@ -74,19 +74,14 @@
     - Outer approximation (OA)
     - Global outer approximation (GOA)
     - Regularized outer approximation (ROA)
     - LP/NLP based branch-and-bound (LP/NLP)
     - Global LP/NLP based branch-and-bound (GLP/NLP)
     - Regularized LP/NLP based branch-and-bound (RLP/NLP)
     - Feasibility pump (FP)
-
-    This solver implementation has been developed by David Bernal <https://github.com/bernalde>
-    and Zedong Peng <https://github.com/ZedongPeng> as part of research efforts at the Grossmann
-    Research Group (http://egon.cheme.cmu.edu/) at the Department of Chemical Engineering at
-    Carnegie Mellon University.
     """
 
     CONFIG = _get_MindtPy_config()
 
     def available(self, exception_flag=True):
         """Check if solver is available."""
         return True
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/algorithm_base_class.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/algorithm_base_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -802,15 +802,15 @@
             self.dual_bound = float('-inf')
         else:
             self.primal_bound = float('-inf')
             self.dual_bound = float('inf')
         self.primal_bound_progress = [self.primal_bound]
         self.dual_bound_progress = [self.dual_bound]
 
-        if config.nlp_solver == 'ipopt':
+        if config.nlp_solver in {'ipopt', 'cyipopt'}:
             if not hasattr(self.working_model, 'ipopt_zL_out'):
                 self.working_model.ipopt_zL_out = Suffix(direction=Suffix.IMPORT)
             if not hasattr(self.working_model, 'ipopt_zU_out'):
                 self.working_model.ipopt_zU_out = Suffix(direction=Suffix.IMPORT)
 
         if config.quadratic_strategy == 0:
             self.mip_objective_polynomial_degree = {0, 1}
@@ -896,19 +896,30 @@
                     self.dual_bound,
                     self.rel_gap,
                     get_main_elapsed_time(self.timing),
                 )
             )
             # Add OA cut
             if add_oa_cuts:
-                dual_values = (
-                    list(m.dual[c] for c in MindtPy.constraint_list)
-                    if config.calculate_dual_at_solution
-                    else None
-                )
+                if (
+                    self.config.nlp_solver == 'cyipopt'
+                    and self.objective_sense == minimize
+                ):
+                    # TODO: recover the opposite dual when cyipopt issue #2831 is solved.
+                    dual_values = (
+                        list(-1 * m.dual[c] for c in MindtPy.constraint_list)
+                        if config.calculate_dual_at_solution
+                        else None
+                    )
+                else:
+                    dual_values = (
+                        list(m.dual[c] for c in MindtPy.constraint_list)
+                        if config.calculate_dual_at_solution
+                        else None
+                    )
                 copy_var_list_values(
                     m.MindtPy_utils.variable_list,
                     self.mip.MindtPy_utils.variable_list,
                     config,
                 )
                 if config.init_strategy == 'FP':
                     copy_var_list_values(
@@ -1190,14 +1201,20 @@
             self.working_model.MindtPy_utils.variable_list,
             config,
         )
         if config.calculate_dual_at_solution:
             for c in fixed_nlp.tmp_duals:
                 if fixed_nlp.dual.get(c, None) is None:
                     fixed_nlp.dual[c] = fixed_nlp.tmp_duals[c]
+                elif (
+                    self.config.nlp_solver == 'cyipopt'
+                    and self.objective_sense == minimize
+                ):
+                    # TODO: recover the opposite dual when cyipopt issue #2831 is solved.
+                    fixed_nlp.dual[c] = -fixed_nlp.dual[c]
             dual_values = list(
                 fixed_nlp.dual[c] for c in fixed_nlp.MindtPy_utils.constraint_list
             )
         else:
             dual_values = None
         main_objective = fixed_nlp.MindtPy_utils.objective_list[-1]
         self.update_primal_bound(value(main_objective.expr))
@@ -1794,15 +1811,15 @@
 
         Returns
         -------
         mainopt : SolverFactory
             The customized MIP solver.
         """
         # Deactivate extraneous IMPORT/EXPORT suffixes
-        if config.nlp_solver == 'ipopt':
+        if config.nlp_solver in {'ipopt', 'cyipopt'}:
             getattr(self.mip, 'ipopt_zL_out', _DoNothing()).deactivate()
             getattr(self.mip, 'ipopt_zU_out', _DoNothing()).deactivate()
         if regularization_problem:
             mainopt = SolverFactory(config.mip_regularization_solver)
         else:
             if config.mip_solver == 'gurobi_persistent' and config.single_tree:
                 mainopt = GurobiPersistent4MindtPy()
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/config_options.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/config_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,15 +504,15 @@
     CONFIG : ConfigBlock
         The specific configurations for MindtPy.
     """
     CONFIG.declare(
         'nlp_solver',
         ConfigValue(
             default='ipopt',
-            domain=In(['ipopt', 'appsi_ipopt', 'gams', 'baron']),
+            domain=In(['ipopt', 'appsi_ipopt', 'gams', 'baron', 'cyipopt']),
             description='NLP subsolver name',
             doc='Which NLP subsolver is going to be used for solving the nonlinear'
             'subproblems.',
         ),
     )
     CONFIG.declare(
         'nlp_solver_args',
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/cut_generation.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/cut_generation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/extended_cutting_plane.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/extended_cutting_plane.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,35 +20,24 @@
 from pyomo.contrib.mindtpy.cut_generation import add_ecp_cuts
 from pyomo.opt import TerminationCondition as tc
 
 
 @SolverFactory.register(
     'mindtpy.ecp', doc='MindtPy: Mixed-Integer Nonlinear Decomposition Toolbox in Pyomo'
 )
-class MindtPy_OA_Solver(_MindtPyAlgorithm):
+class MindtPy_ECP_Solver(_MindtPyAlgorithm):
     """
     Decomposition solver for Mixed-Integer Nonlinear Programming (MINLP) problems.
 
     The MindtPy (Mixed-Integer Nonlinear Decomposition Toolbox in Pyomo) solver
     applies a variety of decomposition-based approaches to solve Mixed-Integer
     Nonlinear Programming (MINLP) problems.
-    These approaches include:
+    This class includes:
 
-    - Outer approximation (OA)
-    - Global outer approximation (GOA)
-    - Regularized outer approximation (ROA)
-    - LP/NLP based branch-and-bound (LP/NLP)
-    - Global LP/NLP based branch-and-bound (GLP/NLP)
-    - Regularized LP/NLP based branch-and-bound (RLP/NLP)
-    - Feasibility pump (FP)
-
-    This solver implementation has been developed by David Bernal <https://github.com/bernalde>
-    and Zedong Peng <https://github.com/ZedongPeng> as part of research efforts at the Grossmann
-    Research Group (http://egon.cheme.cmu.edu/) at the Department of Chemical Engineering at
-    Carnegie Mellon University.
+    - Extended Cutting Plane (ECP)
     """
 
     CONFIG = _get_MindtPy_ECP_config()
 
     def MindtPy_iteration_loop(self, config):
         """Main loop for MindtPy Algorithms.
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/feasibility_pump.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/feasibility_pump.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,28 +33,17 @@
 class MindtPy_FP_Solver(_MindtPyAlgorithm):
     """
     Decomposition solver for Mixed-Integer Nonlinear Programming (MINLP) problems.
 
     The MindtPy (Mixed-Integer Nonlinear Decomposition Toolbox in Pyomo) solver
     applies a variety of decomposition-based approaches to solve Mixed-Integer
     Nonlinear Programming (MINLP) problems.
-    These approaches include:
+    This class includes:
 
-    - Outer approximation (OA)
-    - Global outer approximation (GOA)
-    - Regularized outer approximation (ROA)
-    - LP/NLP based branch-and-bound (LP/NLP)
-    - Global LP/NLP based branch-and-bound (GLP/NLP)
-    - Regularized LP/NLP based branch-and-bound (RLP/NLP)
     - Feasibility pump (FP)
-
-    This solver implementation has been developed by David Bernal <https://github.com/bernalde>
-    and Zedong Peng <https://github.com/ZedongPeng> as part of research efforts at the Grossmann
-    Research Group (http://egon.cheme.cmu.edu/) at the Department of Chemical Engineering at
-    Carnegie Mellon University.
     """
 
     CONFIG = _get_MindtPy_FP_config()
 
     def check_config(self):
         # feasibility pump alone will lead to iteration_limit = 0, important!
         self.config.iteration_limit = 0
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/global_outer_approximation.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/global_outer_approximation.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,35 +41,25 @@
 from operator import itemgetter
 from pyomo.contrib.mindtpy.cut_generation import add_affine_cuts
 
 
 @SolverFactory.register(
     'mindtpy.goa', doc='MindtPy: Mixed-Integer Nonlinear Decomposition Toolbox in Pyomo'
 )
-class MindtPy_OA_Solver(_MindtPyAlgorithm):
+class MindtPy_GOA_Solver(_MindtPyAlgorithm):
     """
     Decomposition solver for Mixed-Integer Nonlinear Programming (MINLP) problems.
 
     The MindtPy (Mixed-Integer Nonlinear Decomposition Toolbox in Pyomo) solver
     applies a variety of decomposition-based approaches to solve Mixed-Integer
     Nonlinear Programming (MINLP) problems.
-    These approaches include:
+    This class includes:
 
-    - Outer approximation (OA)
     - Global outer approximation (GOA)
-    - Regularized outer approximation (ROA)
-    - LP/NLP based branch-and-bound (LP/NLP)
     - Global LP/NLP based branch-and-bound (GLP/NLP)
-    - Regularized LP/NLP based branch-and-bound (RLP/NLP)
-    - Feasibility pump (FP)
-
-    This solver implementation has been developed by David Bernal <https://github.com/bernalde>
-    and Zedong Peng <https://github.com/ZedongPeng> as part of research efforts at the Grossmann
-    Research Group (http://egon.cheme.cmu.edu/) at the Department of Chemical Engineering at
-    Carnegie Mellon University.
     """
 
     CONFIG = _get_MindtPy_GOA_config()
 
     def check_config(self):
         config = self.config
         config.add_slack = False
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/mip_solve.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/mip_solve.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
     Returns
     -------
     mainopt : SolverFactory
         The customized MIP solver.
     """
     # Deactivate extraneous IMPORT/EXPORT suffixes
-    if config.nlp_solver == 'ipopt':
+    if config.nlp_solver in {'ipopt', 'cyipopt'}:
         getattr(solve_data.mip, 'ipopt_zL_out', _DoNothing()).deactivate()
         getattr(solve_data.mip, 'ipopt_zU_out', _DoNothing()).deactivate()
     if regularization_problem:
         mainopt = SolverFactory(config.mip_regularization_solver)
     else:
         if config.mip_solver == 'gurobi_persistent' and config.single_tree:
             mainopt = GurobiPersistent4MindtPy()
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/nlp_solve.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/nlp_solve.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,20 @@
         solve_data.working_model.MindtPy_utils.variable_list,
         config,
     )
     if config.calculate_dual_at_solution:
         for c in fixed_nlp.tmp_duals:
             if fixed_nlp.dual.get(c, None) is None:
                 fixed_nlp.dual[c] = fixed_nlp.tmp_duals[c]
+            elif (
+                config.nlp_solver == 'cyipopt'
+                and solve_data.objective_sense == minimize
+            ):
+                # TODO: recover the opposite dual when cyipopt issue #2831 is solved.
+                fixed_nlp.dual[c] = -fixed_nlp.dual[c]
         dual_values = list(
             fixed_nlp.dual[c] for c in fixed_nlp.MindtPy_utils.constraint_list
         )
     else:
         dual_values = None
     main_objective = fixed_nlp.MindtPy_utils.objective_list[-1]
     update_primal_bound(solve_data, value(main_objective.expr))
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/outer_approximation.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/outer_approximation.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,28 +25,20 @@
 class MindtPy_OA_Solver(_MindtPyAlgorithm):
     """
     Decomposition solver for Mixed-Integer Nonlinear Programming (MINLP) problems.
 
     The MindtPy (Mixed-Integer Nonlinear Decomposition Toolbox in Pyomo) solver
     applies a variety of decomposition-based approaches to solve Mixed-Integer
     Nonlinear Programming (MINLP) problems.
-    These approaches include:
+    This class includes:
 
     - Outer approximation (OA)
-    - Global outer approximation (GOA)
     - Regularized outer approximation (ROA)
     - LP/NLP based branch-and-bound (LP/NLP)
-    - Global LP/NLP based branch-and-bound (GLP/NLP)
     - Regularized LP/NLP based branch-and-bound (RLP/NLP)
-    - Feasibility pump (FP)
-
-    This solver implementation has been developed by David Bernal <https://github.com/bernalde>
-    and Zedong Peng <https://github.com/ZedongPeng> as part of research efforts at the Grossmann
-    Research Group (http://egon.cheme.cmu.edu/) at the Department of Chemical Engineering at
-    Carnegie Mellon University.
     """
 
     CONFIG = _get_MindtPy_OA_config()
 
     def check_config(self):
         config = self.config
         if config.add_regularization is not None:
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/single_tree.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/single_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,14 +494,20 @@
         opt : SolverFactory
             The cplex_persistent solver.
         """
         if config.calculate_dual_at_solution:
             for c in fixed_nlp.tmp_duals:
                 if fixed_nlp.dual.get(c, None) is None:
                     fixed_nlp.dual[c] = fixed_nlp.tmp_duals[c]
+                elif (
+                    config.nlp_solver == 'cyipopt'
+                    and solve_data.objective_sense == minimize
+                ):
+                    # TODO: recover the opposite dual when cyipopt issue #2831 is solved.
+                    fixed_nlp.dual[c] = -fixed_nlp.dual[c]
             dual_values = list(
                 fixed_nlp.dual[c] for c in fixed_nlp.MindtPy_utils.constraint_list
             )
         else:
             dual_values = None
         main_objective = fixed_nlp.MindtPy_utils.objective_list[-1]
         update_primal_bound(solve_data, value(main_objective.expr))
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tabu_list.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tabu_list.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/MINLP2_simple.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/MINLP2_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/MINLP3_simple.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/MINLP3_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/MINLP4_simple.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/MINLP4_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/MINLP5_simple.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/MINLP5_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/MINLP_simple.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/MINLP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/constraint_qualification_example.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/constraint_qualification_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/eight_process_problem.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/eight_process_problem.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/feasibility_pump1.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/feasibility_pump1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/feasibility_pump2.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/feasibility_pump2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/from_proposal.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/from_proposal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/nonconvex1.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/nonconvex1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/nonconvex2.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/nonconvex2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/nonconvex3.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/nonconvex3.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/nonconvex4.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/nonconvex4.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/online_doc_example.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/online_doc_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,38 @@
                     results.solver.termination_condition,
                     [TerminationCondition.optimal, TerminationCondition.feasible],
                 )
                 self.assertAlmostEqual(
                     value(model.objective.expr), model.optimal_value, places=1
                 )
 
+    @unittest.skipUnless(
+        SolverFactory('cyipopt').available(exception_flag=False),
+        "APPSI_IPOPT not available.",
+    )
+    def test_OA_cyipopt(self):
+        """Test the outer approximation decomposition algorithm."""
+        with SolverFactory('mindtpy') as opt:
+            for model in nonconvex_model_list:
+                results = opt.solve(
+                    model,
+                    strategy='OA',
+                    mip_solver=required_solvers[1],
+                    nlp_solver='cyipopt',
+                    heuristic_nonconvex=True,
+                )
+
+                self.assertIn(
+                    results.solver.termination_condition,
+                    [TerminationCondition.optimal, TerminationCondition.feasible],
+                )
+                self.assertAlmostEqual(
+                    value(model.objective.expr), model.optimal_value, places=1
+                )
+
     def test_OA_integer_to_binary(self):
         """Test the outer approximation decomposition algorithm."""
         with SolverFactory('mindtpy') as opt:
             for model in model_list:
                 results = opt.solve(
                     model,
                     strategy='OA',
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_ECP.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_ECP.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_feas_pump.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_feas_pump.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_global.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_global.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_global_lp_nlp.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_global_lp_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_lp_nlp.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_lp_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_regularization.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_regularization.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/tests/test_mindtpy_solution_pool.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/tests/test_mindtpy_solution_pool.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mindtpy/util.py` & `Pyomo-6.6.1/pyomo/contrib/mindtpy/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,26 +137,28 @@
                 if var.is_integer():
                     var.setub(config.integer_var_bound)
                 else:
                     var.setub(config.continuous_var_bound)
 
 
 def generate_norm2sq_objective_function(model, setpoint_model, discrete_only=False):
-    """This function generates objective (FP-NLP subproblem) for minimum euclidean distance to setpoint_model.
+    r"""This function generates objective (FP-NLP subproblem) for minimum
+    euclidean distance to setpoint_model.
 
     L2 distance of (x,y) = \sqrt{\sum_i (x_i - y_i)^2}.
 
     Parameters
     ----------
     model : Pyomo model
         The model that needs new objective function.
     setpoint_model : Pyomo model
         The model that provides the base point for us to calculate the distance.
     discrete_only : bool, optional
-        Whether to only optimize on distance between the discrete variables, by default False.
+        Whether to only optimize on distance between the discrete
+        variables, by default False.
 
     Returns
     -------
     Objective
         The norm2 square objective function.
     """
     # skip objective_value variable and slack_var variables
@@ -191,31 +193,34 @@
                 ]
             )
         )
     )
 
 
 def generate_norm1_objective_function(model, setpoint_model, discrete_only=False):
-    """This function generates objective (PF-OA main problem) for minimum Norm1 distance to setpoint_model.
+    r"""This function generates objective (PF-OA main problem) for minimum
+    Norm1 distance to setpoint_model.
 
     Norm1 distance of (x,y) = \sum_i |x_i - y_i|.
 
     Parameters
     ----------
     model : Pyomo model
         The model that needs new objective function.
     setpoint_model : Pyomo model
         The model that provides the base point for us to calculate the distance.
     discrete_only : bool, optional
-        Whether to only optimize on distance between the discrete variables, by default False.
+        Whether to only optimize on distance between the discrete
+        variables, by default False.
 
     Returns
     -------
     Objective
         The norm1 objective function.
+
     """
     # skip objective_value variable and slack_var variables
     var_filter = (
         (lambda v: v.is_integer())
         if discrete_only
         else (
             lambda v: 'MindtPy_utils.objective_value' not in v.name
@@ -429,30 +434,35 @@
                         for (model_var, setpoint_var) in zip(model_vars, setpoint_vars)
                     ]
                 )
             )
 
 
 def generate_norm1_norm_constraint(model, setpoint_model, config, discrete_only=True):
-    """This function generates constraint (PF-OA main problem) for minimum Norm1 distance to setpoint_model.
+    r"""This function generates constraint (PF-OA main problem) for minimum
+    Norm1 distance to setpoint_model.
+
+    Norm constraint is used to guarantees the monotonicity of the norm
+    objective value sequence of all iterations.
 
-    Norm constraint is used to guarantees the monotonicity of the norm objective value sequence of all iterations
     Norm1 distance of (x,y) = \sum_i |x_i - y_i|.
     Ref: Paper 'A storm of feasibility pumps for nonconvex MINLP' Eq. (16).
 
     Parameters
     ----------
     model : Pyomo model
         The model that needs the norm constraint.
     setpoint_model : Pyomo model
         The model that provides the base point for us to calculate the distance.
     config : ConfigBlock
         The specific configurations for MindtPy.
     discrete_only : bool, optional
-        Whether to only optimize on distance between the discrete variables, by default True.
+        Whether to only optimize on distance between the discrete
+        variables, by default True.
+
     """
     var_filter = (lambda v: v.is_integer()) if discrete_only else (lambda v: True)
     model_vars = list(filter(var_filter, model.MindtPy_utils.variable_list))
     setpoint_vars = list(filter(var_filter, setpoint_model.MindtPy_utils.variable_list))
     assert len(model_vars) == len(
         setpoint_vars
     ), 'Trying to generate Norm1 norm constraint for models with different number of variables'
@@ -561,14 +571,17 @@
         opt.options['mipgap'] = config.mip_solver_mipgap
     elif solver_name == 'baron':
         opt.options['MaxTime'] = remaining
         opt.options['AbsConFeasTol'] = config.zero_tolerance
     elif solver_name in {'ipopt', 'appsi_ipopt'}:
         opt.options['max_cpu_time'] = remaining
         opt.options['constr_viol_tol'] = config.zero_tolerance
+    elif solver_name == 'cyipopt':
+        opt.config.options['max_cpu_time'] = float(remaining)
+        opt.config.options['constr_viol_tol'] = config.zero_tolerance
     elif solver_name == 'gams':
         if solver_type == 'mip':
             opt.options['add_options'] = [
                 'option optcr=%s;' % config.mip_solver_mipgap,
                 'option reslim=%s;' % remaining,
             ]
         elif solver_type == 'nlp':
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/convert.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/dynamic_data_base.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/dynamic_data_base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/find_nearest_index.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/find_nearest_index.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/get_cuid.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/get_cuid.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/interval_data.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/interval_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/scalar_data.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/scalar_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/series_data.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/series_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_convert.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_find_nearest_index.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_find_nearest_index.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_get_cuid.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_get_cuid.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_interval_data.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_interval_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_scalar_data.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_scalar_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/data/tests/test_series_data.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/data/tests/test_series_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/model.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/run_mpc.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/run_mpc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/run_openloop.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/run_openloop.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/tests/test_mpc.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/examples/cstr/tests/test_openloop.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/examples/cstr/tests/test_openloop.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/copy_values.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/copy_values.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/load_data.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/load_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/model_interface.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/model_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/tests/test_interface.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/tests/test_var_linker.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/tests/test_var_linker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/interfaces/var_linker.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/interfaces/var_linker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/modeling/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/modeling/constraints.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/modeling/constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/modeling/cost_expressions.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/modeling/cost_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/modeling/terminal.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/modeling/terminal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/modeling/tests/test_cost_expressions.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/modeling/tests/test_cost_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/modeling/tests/test_input_constraints.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/modeling/tests/test_input_constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/mpc/modeling/tests/test_terminal.py` & `Pyomo-6.6.1/pyomo/contrib/mpc/modeling/tests/test_terminal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/multistart/high_conf_stop.py` & `Pyomo-6.6.1/pyomo/contrib/multistart/high_conf_stop.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/multistart/multi.py` & `Pyomo-6.6.1/pyomo/contrib/multistart/multi.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/multistart/reinit.py` & `Pyomo-6.6.1/pyomo/contrib/multistart/reinit.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/multistart/test_multi.py` & `Pyomo-6.6.1/pyomo/contrib/multistart/test_multi.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reaction_kinetics/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reaction_kinetics/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reaction_kinetics/simple_reaction_parmest_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reaction_kinetics/simple_reaction_parmest_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/bootstrap_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/bootstrap_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/datarec_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/datarec_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/leaveNout_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/leaveNout_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/likelihood_ratio_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/likelihood_ratio_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/multisensor_data_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/multisensor_data_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/parameter_estimation_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/parameter_estimation_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/reactor_design.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/reactor_design.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/reactor_design/timeseries_data_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/reactor_design/timeseries_data_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/bootstrap_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/bootstrap_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/likelihood_ratio_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/likelihood_ratio_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/parameter_estimation_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/parameter_estimation_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler_with_constraint.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/rooney_biegler/rooney_biegler_with_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/parallel_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/parallel_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/parameter_estimation_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/parameter_estimation_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/scenario_example.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/scenario_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/examples/semibatch/semibatch.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/examples/semibatch/semibatch.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/graphics.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/graphics.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/ipopt_solver_wrapper.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/ipopt_solver_wrapper.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/parmest.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/parmest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1230,15 +1230,15 @@
         dfcols = list(theta_names) + ['obj']
         obj_at_theta = pd.DataFrame(data=global_all_obj, columns=dfcols)
         return obj_at_theta
 
     def likelihood_ratio_test(
         self, obj_at_theta, obj_value, alphas, return_thresholds=False
     ):
-        """
+        r"""
         Likelihood ratio test to identify theta values within a confidence
         region using the :math:`\chi^2` distribution
 
         Parameters
         ----------
         obj_at_theta: pd.DataFrame, columns = theta_names + 'obj'
             Objective values for each theta value (returned by
```

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/scenariocreator.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/scenariocreator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/tests/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_examples.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_graphics.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_graphics.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_parmest.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_parmest.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_scenariocreator.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_scenariocreator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_solver.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/tests/test_utils.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/utils/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/utils/create_ef.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/utils/create_ef.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/utils/ipopt_solver_wrapper.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/utils/ipopt_solver_wrapper.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/utils/model_utils.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/utils/mpi_utils.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/utils/mpi_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/parmest/utils/scenario_tree.py` & `Pyomo-6.6.1/pyomo/contrib/parmest/utils/scenario_tree.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/piecewise_linear_expression.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/piecewise_linear_expression.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/piecewise_linear_function.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/piecewise_linear_function.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/tests/common_tests.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/tests/common_tests.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/tests/models.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/tests/models.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/tests/test_inner_repn_gdp.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/tests/test_inner_repn_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/tests/test_outer_repn_gdp.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/tests/test_outer_repn_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/tests/test_piecewise_linear_function.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/tests/test_piecewise_linear_function.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/tests/test_reduced_inner_repn.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/tests/test_reduced_inner_repn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/transform/convex_combination.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/transform/convex_combination.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/transform/disaggregated_convex_combination.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/transform/disaggregated_convex_combination.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/transform/inner_representation_gdp.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/transform/inner_representation_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/transform/multiple_choice.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/transform/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/transform/outer_representation_gdp.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/transform/outer_representation_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/transform/piecewise_to_gdp_transformation.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/transform/piecewise_to_gdp_transformation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/transform/piecewise_to_mip_visitor.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/transform/piecewise_to_mip_visitor.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/piecewise/transform/reduced_inner_representation_gdp.py` & `Pyomo-6.6.1/pyomo/contrib/piecewise/transform/reduced_inner_representation_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/bounds_to_vars.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/bounds_to_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/constraint_tightener.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/constraint_tightener.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/deactivate_trivial_constraints.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/deactivate_trivial_constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/detect_fixed_vars.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/detect_fixed_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/equality_propagate.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/equality_propagate.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/induced_linearity.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/induced_linearity.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/init_vars.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/init_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/int_to_binary.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/int_to_binary.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/remove_zero_terms.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/remove_zero_terms.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/strip_bounds.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/strip_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/var_aggregator.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/var_aggregator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/plugins/zero_sum_propagator.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/plugins/zero_sum_propagator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_bounds_to_vars_xfrm.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_bounds_to_vars_xfrm.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_constraint_tightener.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_constraint_tightener.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_deactivate_trivial_constraints.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_deactivate_trivial_constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_detect_fixed_vars.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_detect_fixed_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_equality_propagate.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_equality_propagate.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_induced_linearity.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_induced_linearity.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_init_vars.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_init_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_int_to_binary.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_int_to_binary.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_strip_bounds.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_strip_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_var_aggregator.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_var_aggregator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_zero_sum_propagate.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_zero_sum_propagate.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/tests/test_zero_term_removal.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/tests/test_zero_term_removal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/preprocessing/util.py` & `Pyomo-6.6.1/pyomo/contrib/preprocessing/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/cyipopt_solver.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/cyipopt_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/implicit_functions.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/implicit_functions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/pyomo_ext_cyipopt.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/pyomo_ext_cyipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/scipy_solvers.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/scipy_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/square_solver_base.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/square_solver_base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_interfaces.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_interfaces.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_solver.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/test_cyipopt_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/test_implicit_functions.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/test_implicit_functions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/test_pyomo_ext_cyipopt.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/test_pyomo_ext_cyipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/algorithms/solvers/tests/test_scipy_solvers.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/algorithms/solvers/tests/test_scipy_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/asl.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/asl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/build.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/build.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/dependencies.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/dependencies.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/callback/cyipopt_callback.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/callback/cyipopt_callback.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/callback/cyipopt_callback_halt.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/callback/cyipopt_callback_halt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/callback/cyipopt_functor_callback.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/callback/cyipopt_functor_callback.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/callback/reactor_design.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/callback/reactor_design.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/param_est/generate_data.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/param_est/generate_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/param_est/models.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/param_est/models.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/param_est/perform_estimation.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/param_est/perform_estimation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_outputs.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_outputs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_ratio_residuals.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/react_example/maximize_cb_ratio_residuals.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_outputs.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_outputs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_residuals.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/external_grey_box/react_example/reactor_model_residuals.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/feasibility.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/feasibility.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/mumps_example.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/mumps_example.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/nlp_interface.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/nlp_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/nlp_interface_2.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/nlp_interface_2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/parallel_matvec.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/parallel_matvec.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/parallel_vector_ops.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/parallel_vector_ops.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/sensitivity.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/sensitivity.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/sqp.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/sqp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/tests/test_cyipopt_examples.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/tests/test_cyipopt_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/tests/test_examples.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/examples/tests/test_mpi_examples.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/examples/tests/test_mpi_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/ampl_nlp.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/ampl_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/cyipopt_interface.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/cyipopt_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/external_grey_box.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/external_grey_box.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/external_pyomo_model.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/external_pyomo_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/nlp.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/nlp_projections.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/nlp_projections.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/pyomo_grey_box_nlp.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/pyomo_grey_box_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/pyomo_nlp.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/pyomo_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/compare_utils.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/compare_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/external_grey_box_models.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/external_grey_box_models.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_cyipopt_interface.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_cyipopt_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_dynamic_model.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_dynamic_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_external_asl_function.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_external_asl_function.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_external_grey_box_model.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_external_grey_box_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_block.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_model.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_external_pyomo_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_nlp.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_nlp_projections.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_nlp_projections.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_pyomo_grey_box_nlp.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_pyomo_grey_box_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/tests/test_utils.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/interfaces/utils.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/intrinsic.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/intrinsic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/base.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/ma27.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/ma27.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/ma27_interface.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/ma27_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/ma57.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/ma57.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/ma57_interface.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/ma57_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/mumps_interface.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/mumps_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/scipy_interface.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/scipy_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/tests/test_linear_solvers.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/tests/test_linear_solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/tests/test_ma27.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/tests/test_ma27.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/tests/test_ma57.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/tests/test_ma57.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/tests/test_mumps_interface.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/tests/test_mumps_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/linalg/utils.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/linalg/utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/base_block.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/base_block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/block_matrix.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/block_matrix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/block_vector.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/block_vector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/mpi_block_matrix.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/mpi_block_matrix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/mpi_block_vector.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/mpi_block_vector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_block_matrix.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_block_matrix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_block_vector.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_block_vector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_intrinsics.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_matrix.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_matrix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_vector.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_mpi_block_vector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/tests/test_sparse_utils.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/tests/test_sparse_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/sparse/utils.py` & `Pyomo-6.6.1/pyomo/contrib/pynumero/sparse/utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/src/AmplInterface.cpp` & `Pyomo-6.6.1/pyomo/contrib/pynumero/src/AmplInterface.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/src/AmplInterface.hpp` & `Pyomo-6.6.1/pyomo/contrib/pynumero/src/AmplInterface.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/src/AssertUtils.hpp` & `Pyomo-6.6.1/pyomo/contrib/pynumero/src/AssertUtils.hpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/src/CMakeLists.txt` & `Pyomo-6.6.1/pyomo/contrib/pynumero/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/src/ma27Interface.cpp` & `Pyomo-6.6.1/pyomo/contrib/pynumero/src/ma27Interface.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/src/ma57Interface.cpp` & `Pyomo-6.6.1/pyomo/contrib/pynumero/src/ma57Interface.cpp`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pynumero/src/tests/simple_nlp.nl` & `Pyomo-6.6.1/pyomo/contrib/pynumero/src/tests/simple_nlp.nl`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pyros/master_problem_methods.py` & `Pyomo-6.6.1/pyomo/contrib/pyros/master_problem_methods.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pyros/pyros.py` & `Pyomo-6.6.1/pyomo/contrib/pyros/pyros.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pyros/pyros_algorithm_methods.py` & `Pyomo-6.6.1/pyomo/contrib/pyros/pyros_algorithm_methods.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pyros/separation_problem_methods.py` & `Pyomo-6.6.1/pyomo/contrib/pyros/separation_problem_methods.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pyros/solve_data.py` & `Pyomo-6.6.1/pyomo/contrib/pyros/solve_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pyros/tests/test_grcs.py` & `Pyomo-6.6.1/pyomo/contrib/pyros/tests/test_grcs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pyros/uncertainty_sets.py` & `Pyomo-6.6.1/pyomo/contrib/pyros/uncertainty_sets.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/pyros/util.py` & `Pyomo-6.6.1/pyomo/contrib/pyros/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/satsolver/satsolver.py` & `Pyomo-6.6.1/pyomo/contrib/satsolver/satsolver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/satsolver/test_satsolver.py` & `Pyomo-6.6.1/pyomo/contrib/satsolver/test_satsolver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/HIV_Transmission.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/HIV_Transmission.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/feedbackController.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/feedbackController.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/parameter.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/parameter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/parameter_kaug.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/parameter_kaug.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/rangeInequality.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/rangeInequality.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/examples/rooney_biegler.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/examples/rooney_biegler.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/k_aug.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/k_aug.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/sens.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/sens.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/tests/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/tests/test_k_aug_interface.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/tests/test_k_aug_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/tests/test_sens.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/tests/test_sens.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/sensitivity_toolbox/tests/test_sens_unit.py` & `Pyomo-6.6.1/pyomo/contrib/sensitivity_toolbox/tests/test_sens_unit.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/simplemodel/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/simplemodel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/TRF.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/TRF.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/examples/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/examples/example1.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/examples/example1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/examples/example2.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/examples/example2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/filter.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/filter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/interface.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/plugins.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/tests/__init__.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/tests/test_TRF.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/tests/test_TRF.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/tests/test_examples.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/tests/test_filter.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/tests/test_interface.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/tests/test_util.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/trustregion/util.py` & `Pyomo-6.6.1/pyomo/contrib/trustregion/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/main.ui` & `Pyomo-6.6.1/pyomo/contrib/viewer/main.ui`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/model_browser.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/model_browser.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/model_browser.ui` & `Pyomo-6.6.1/pyomo/contrib/viewer/model_browser.ui`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/model_select.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/model_select.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/model_select.ui` & `Pyomo-6.6.1/pyomo/contrib/viewer/model_select.ui`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/pyomo_viewer.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/pyomo_viewer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/qt.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/qt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/report.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/report.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/residual_table.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/residual_table.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/residual_table.ui` & `Pyomo-6.6.1/pyomo/contrib/viewer/residual_table.ui`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/tests/test_data_model_item.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/tests/test_data_model_item.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/tests/test_data_model_tree.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/tests/test_data_model_tree.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/tests/test_qt.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/tests/test_report.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/ui.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/ui.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/contrib/viewer/ui_data.py` & `Pyomo-6.6.1/pyomo/contrib/viewer/ui_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/__init__.py` & `Pyomo-6.6.1/pyomo/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/PyomoModel.py` & `Pyomo-6.6.1/pyomo/core/base/PyomoModel.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/__init__.py` & `Pyomo-6.6.1/pyomo/core/base/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/action.py` & `Pyomo-6.6.1/pyomo/core/base/action.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/block.py` & `Pyomo-6.6.1/pyomo/core/base/block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/blockutil.py` & `Pyomo-6.6.1/pyomo/core/base/blockutil.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/boolean_var.py` & `Pyomo-6.6.1/pyomo/core/base/boolean_var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/check.py` & `Pyomo-6.6.1/pyomo/core/base/check.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/component.py` & `Pyomo-6.6.1/pyomo/core/base/component.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/component_namer.py` & `Pyomo-6.6.1/pyomo/core/base/component_namer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/component_order.py` & `Pyomo-6.6.1/pyomo/core/base/component_order.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/componentuid.py` & `Pyomo-6.6.1/pyomo/core/base/componentuid.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/config.py` & `Pyomo-6.6.1/pyomo/core/base/config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/connector.py` & `Pyomo-6.6.1/pyomo/core/base/connector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/constraint.py` & `Pyomo-6.6.1/pyomo/core/base/constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/disable_methods.py` & `Pyomo-6.6.1/pyomo/core/base/disable_methods.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/enums.py` & `Pyomo-6.6.1/pyomo/core/base/enums.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/expression.py` & `Pyomo-6.6.1/pyomo/core/base/expression.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/external.py` & `Pyomo-6.6.1/pyomo/core/base/external.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/global_set.py` & `Pyomo-6.6.1/pyomo/core/base/global_set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/indexed_component.py` & `Pyomo-6.6.1/pyomo/core/base/indexed_component.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/indexed_component_slice.py` & `Pyomo-6.6.1/pyomo/core/base/indexed_component_slice.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,23 +334,23 @@
         ans._call_stack = ans._call_stack[: ans._len]
         return ans
 
     def index_wildcard_keys(self, sort):
         _iter = _IndexedComponent_slice_iter(self, iter_over_index=True, sort=sort)
         return (_iter.get_last_index_wildcards() for _ in _iter)
 
-    def wildcard_keys(self, sort):
+    def wildcard_keys(self, sort=SortComponents.UNSORTED):
         _iter = _IndexedComponent_slice_iter(self, sort=sort)
         return (_iter.get_last_index_wildcards() for _ in _iter)
 
-    def wildcard_values(self, sort):
+    def wildcard_values(self, sort=SortComponents.UNSORTED):
         """Return an iterator over this slice"""
         return _IndexedComponent_slice_iter(self, sort=sort)
 
-    def wildcard_items(self, sort):
+    def wildcard_items(self, sort=SortComponents.UNSORTED):
         _iter = _IndexedComponent_slice_iter(self, sort=sort)
         return ((_iter.get_last_index_wildcards(), _) for _ in _iter)
 
     def expanded_keys(self):
         _iter = self.__iter__()
         return (_iter.get_last_index() for _ in _iter)
```

### Comparing `Pyomo-6.6.0/pyomo/core/base/initializer.py` & `Pyomo-6.6.1/pyomo/core/base/initializer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/instance2dat.py` & `Pyomo-6.6.1/pyomo/core/base/instance2dat.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/label.py` & `Pyomo-6.6.1/pyomo/core/base/label.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/logical_constraint.py` & `Pyomo-6.6.1/pyomo/core/base/logical_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/matrix_constraint.py` & `Pyomo-6.6.1/pyomo/core/base/matrix_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/misc.py` & `Pyomo-6.6.1/pyomo/core/base/misc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/numvalue.py` & `Pyomo-6.6.1/pyomo/core/base/numvalue.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/objective.py` & `Pyomo-6.6.1/pyomo/core/base/objective.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/param.py` & `Pyomo-6.6.1/pyomo/core/base/param.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/piecewise.py` & `Pyomo-6.6.1/pyomo/core/base/piecewise.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/plugin.py` & `Pyomo-6.6.1/pyomo/core/base/plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/range.py` & `Pyomo-6.6.1/pyomo/core/base/range.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/rangeset.py` & `Pyomo-6.6.1/pyomo/core/base/rangeset.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/reference.py` & `Pyomo-6.6.1/pyomo/core/base/reference.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/set.py` & `Pyomo-6.6.1/pyomo/core/base/set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/set_types.py` & `Pyomo-6.6.1/pyomo/core/base/set_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/sets.py` & `Pyomo-6.6.1/pyomo/core/base/sets.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/sos.py` & `Pyomo-6.6.1/pyomo/core/base/sos.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                 is not used.
 
     Example:
 
       model = AbstractModel()
       model.A = Set()
       model.B = Set(A)
-      model.X = Set(B)
+      model.X = Var(B)
 
       model.C1 = SOSConstraint(model.A, var=model.X, set=model.B, sos=1)
 
     This constraint actually creates one SOS-1 constraint for each
     element of model.A (e.g., if |A| == N, there are N constraints).
     In each constraint, model.X is indexed by the elements of
     model.B[a], where 'a' is the current index of model.A.
```

### Comparing `Pyomo-6.6.0/pyomo/core/base/suffix.py` & `Pyomo-6.6.1/pyomo/core/base/suffix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/symbol_map.py` & `Pyomo-6.6.1/pyomo/core/base/symbol_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/symbolic.py` & `Pyomo-6.6.1/pyomo/core/base/symbolic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/template_expr.py` & `Pyomo-6.6.1/pyomo/core/base/template_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/transformation.py` & `Pyomo-6.6.1/pyomo/core/base/transformation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/units_container.py` & `Pyomo-6.6.1/pyomo/core/base/units_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/util.py` & `Pyomo-6.6.1/pyomo/core/base/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/base/var.py` & `Pyomo-6.6.1/pyomo/core/base/var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/beta/__init__.py` & `Pyomo-6.6.1/pyomo/core/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/beta/dict_objects.py` & `Pyomo-6.6.1/pyomo/core/beta/dict_objects.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/beta/list_objects.py` & `Pyomo-6.6.1/pyomo/core/beta/list_objects.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/__init__.py` & `Pyomo-6.6.1/pyomo/core/expr/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/base.py` & `Pyomo-6.6.1/pyomo/core/expr/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/boolean_value.py` & `Pyomo-6.6.1/pyomo/core/expr/boolean_value.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/calculus/derivatives.py` & `Pyomo-6.6.1/pyomo/core/expr/calculus/derivatives.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/calculus/diff_with_pyomo.py` & `Pyomo-6.6.1/pyomo/core/expr/calculus/diff_with_pyomo.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/calculus/diff_with_sympy.py` & `Pyomo-6.6.1/pyomo/core/expr/calculus/diff_with_sympy.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/cnf_walker.py` & `Pyomo-6.6.1/pyomo/core/expr/cnf_walker.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/compare.py` & `Pyomo-6.6.1/pyomo/core/expr/compare.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/current.py` & `Pyomo-6.6.1/pyomo/core/expr/current.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/expr_common.py` & `Pyomo-6.6.1/pyomo/core/expr/expr_common.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/expr_errors.py` & `Pyomo-6.6.1/pyomo/core/expr/expr_errors.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/logical_expr.py` & `Pyomo-6.6.1/pyomo/core/expr/logical_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/numeric_expr.py` & `Pyomo-6.6.1/pyomo/core/expr/numeric_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/numvalue.py` & `Pyomo-6.6.1/pyomo/core/expr/numvalue.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/relational_expr.py` & `Pyomo-6.6.1/pyomo/core/expr/relational_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/symbol_map.py` & `Pyomo-6.6.1/pyomo/core/expr/symbol_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/sympy_tools.py` & `Pyomo-6.6.1/pyomo/core/expr/sympy_tools.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/taylor_series.py` & `Pyomo-6.6.1/pyomo/core/expr/taylor_series.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/template_expr.py` & `Pyomo-6.6.1/pyomo/core/expr/template_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/expr/visitor.py` & `Pyomo-6.6.1/pyomo/core/expr/visitor.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/__init__.py` & `Pyomo-6.6.1/pyomo/core/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/base.py` & `Pyomo-6.6.1/pyomo/core/kernel/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/block.py` & `Pyomo-6.6.1/pyomo/core/kernel/block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/component_map.py` & `Pyomo-6.6.1/pyomo/core/kernel/component_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/component_set.py` & `Pyomo-6.6.1/pyomo/core/kernel/component_set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/conic.py` & `Pyomo-6.6.1/pyomo/core/kernel/conic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/constraint.py` & `Pyomo-6.6.1/pyomo/core/kernel/constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/container_utils.py` & `Pyomo-6.6.1/pyomo/core/kernel/container_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/dict_container.py` & `Pyomo-6.6.1/pyomo/core/kernel/dict_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/expression.py` & `Pyomo-6.6.1/pyomo/core/kernel/expression.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/heterogeneous_container.py` & `Pyomo-6.6.1/pyomo/core/kernel/heterogeneous_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/homogeneous_container.py` & `Pyomo-6.6.1/pyomo/core/kernel/homogeneous_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/list_container.py` & `Pyomo-6.6.1/pyomo/core/kernel/list_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/matrix_constraint.py` & `Pyomo-6.6.1/pyomo/core/kernel/matrix_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/objective.py` & `Pyomo-6.6.1/pyomo/core/kernel/objective.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/parameter.py` & `Pyomo-6.6.1/pyomo/core/kernel/parameter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/piecewise_library/__init__.py` & `Pyomo-6.6.1/pyomo/core/kernel/piecewise_library/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/piecewise_library/transforms.py` & `Pyomo-6.6.1/pyomo/core/kernel/piecewise_library/transforms.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/piecewise_library/transforms_nd.py` & `Pyomo-6.6.1/pyomo/core/kernel/piecewise_library/transforms_nd.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/piecewise_library/util.py` & `Pyomo-6.6.1/pyomo/core/kernel/piecewise_library/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/register_numpy_types.py` & `Pyomo-6.6.1/pyomo/core/kernel/register_numpy_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/set_types.py` & `Pyomo-6.6.1/pyomo/core/kernel/set_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/sos.py` & `Pyomo-6.6.1/pyomo/core/kernel/sos.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/suffix.py` & `Pyomo-6.6.1/pyomo/core/kernel/suffix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/tuple_container.py` & `Pyomo-6.6.1/pyomo/core/kernel/tuple_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/kernel/variable.py` & `Pyomo-6.6.1/pyomo/core/kernel/variable.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/core/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/__init__.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/add_slack_vars.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/add_slack_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/discrete_vars.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/discrete_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/eliminate_fixed_vars.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/eliminate_fixed_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/equality_transform.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/equality_transform.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/expand_connectors.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/expand_connectors.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/hierarchy.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/hierarchy.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/logical_to_linear.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/logical_to_linear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/model.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/nonnegative_transform.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/nonnegative_transform.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/radix_linearization.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/radix_linearization.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/relax_integrality.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/relax_integrality.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/scaling.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/scaling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/standard_form.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/standard_form.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/plugins/transform/util.py` & `Pyomo-6.6.1/pyomo/core/plugins/transform/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/pyomoobject.py` & `Pyomo-6.6.1/pyomo/core/pyomoobject.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/staleflag.py` & `Pyomo-6.6.1/pyomo/core/staleflag.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/__init__.py` & `Pyomo-6.6.1/pyomo/core/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/data/__init__.py` & `Pyomo-6.6.1/pyomo/core/tests/data/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/data/test_odbc_ini.py` & `Pyomo-6.6.1/pyomo/core/tests/data/test_odbc_ini.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/diet/__init__.py` & `Pyomo-6.6.1/pyomo/core/tests/diet/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/diet/test_diet.py` & `Pyomo-6.6.1/pyomo/core/tests/diet/test_diet.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/examples/__init__.py` & `Pyomo-6.6.1/pyomo/core/tests/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/examples/pmedian.py` & `Pyomo-6.6.1/pyomo/core/tests/examples/pmedian.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/examples/pmedian1.py` & `Pyomo-6.6.1/pyomo/core/tests/examples/pmedian1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/examples/pmedian2.py` & `Pyomo-6.6.1/pyomo/core/tests/examples/pmedian2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/examples/pmedian4.py` & `Pyomo-6.6.1/pyomo/core/tests/examples/pmedian4.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/examples/test_amplbook2.py` & `Pyomo-6.6.1/pyomo/core/tests/examples/test_amplbook2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/examples/test_kernel_examples.py` & `Pyomo-6.6.1/pyomo/core/tests/examples/test_kernel_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/examples/test_pyomo.py` & `Pyomo-6.6.1/pyomo/core/tests/examples/test_pyomo.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/examples/test_tutorials.py` & `Pyomo-6.6.1/pyomo/core/tests/examples/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/transform/__init__.py` & `Pyomo-6.6.1/pyomo/core/tests/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/transform/test_add_slacks.py` & `Pyomo-6.6.1/pyomo/core/tests/transform/test_add_slacks.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/transform/test_scaling.py` & `Pyomo-6.6.1/pyomo/core/tests/transform/test_scaling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/transform/test_transform.py` & `Pyomo-6.6.1/pyomo/core/tests/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/__init__.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/__init__.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_block.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_component_map.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_component_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_component_set.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_component_set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_conic.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_conic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_constraint.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_dict_container.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_dict_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_expression.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_expression.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_kernel.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_kernel.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_list_container.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_list_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_matrix_constraint.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_matrix_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_objective.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_objective.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_parameter.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_parameter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_piecewise.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_piecewise.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_sos.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_sos.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_suffix.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_suffix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_tuple_container.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_tuple_container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/kernel/test_variable.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/kernel/test_variable.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_action.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_action.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_block.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_block_model.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_block_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_bounds.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_check.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_check.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_compare.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_compare.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_component.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_component.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_componentuid.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_componentuid.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_con.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_con.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_concrete.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_concrete.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_connector.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_connector.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_deprecation.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_derivs.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_derivs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_dict_objects.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_dict_objects.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_disable_methods.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_disable_methods.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_enums.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_enums.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_expr_misc.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_expr_misc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_expression.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_expression.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_external.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_external.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_indexed.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_indexed.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_indexed_slice.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_indexed_slice.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,30 +488,30 @@
         _slicer.call_errors_generate_exceptions = True
         self.assertRaises(TypeError, _slicer.next)
 
     def test_iterators(self):
         m = self.m
 
         _slice = self.m.x[...]
-        self.assertEqual(list(_slice.wildcard_keys(False)), [7, 8, 9])
+        self.assertEqual(list(_slice.wildcard_keys()), [7, 8, 9])
         self.assertEqual(
-            list(_slice.wildcard_items(False)), [(7, m.x[7]), (8, m.x[8]), (9, m.x[9])]
+            list(_slice.wildcard_items()), [(7, m.x[7]), (8, m.x[8]), (9, m.x[9])]
         )
         self.assertEqual(list(_slice.expanded_keys()), [7, 8, 9])
         self.assertEqual(
             list(_slice.expanded_items()), [(7, m.x[7]), (8, m.x[8]), (9, m.x[9])]
         )
 
         _slice = self.m.b[...]
         self.assertEqual(
-            list(_slice.wildcard_keys(False)),
+            list(_slice.wildcard_keys()),
             [(1, 4), (1, 5), (1, 6), (2, 4), (2, 5), (2, 6), (3, 4), (3, 5), (3, 6)],
         )
         self.assertEqual(
-            list(_slice.wildcard_items(False)),
+            list(_slice.wildcard_items()),
             [
                 ((1, 4), m.b[1, 4]),
                 ((1, 5), m.b[1, 5]),
                 ((1, 6), m.b[1, 6]),
                 ((2, 4), m.b[2, 4]),
                 ((2, 5), m.b[2, 5]),
                 ((2, 6), m.b[2, 6]),
```

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_initializer.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_initializer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_kernel_register_numpy_types.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_kernel_register_numpy_types.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_labelers.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_labelers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_list_objects.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_list_objects.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_logical_constraint.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_logical_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_logical_expr_expanded.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_logical_expr_expanded.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_logical_to_linear.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_logical_to_linear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_matrix_constraint.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_matrix_constraint.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_misc.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_misc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_model.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_mutable.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_mutable.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_numeric_expr.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_numeric_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_numeric_expr_api.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_numeric_expr_api.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_numeric_expr_dispatcher.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_numeric_expr_dispatcher.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_numeric_expr_zerofilter.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_numeric_expr_zerofilter.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_numpy_expr.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_numpy_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_numvalue.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_numvalue.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_obj.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_obj.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_param.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_param.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_pickle.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_pickle.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_piecewise.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_piecewise.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_preprocess.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_range.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_range.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_reference.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_reference.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_relational_expr.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_relational_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_set.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_set.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_sets.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_sets.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_smap.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_smap.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_sos.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_sos.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_suffix.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_suffix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_symbol_map.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_symbol_map.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_symbolic.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_symbolic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_taylor_series.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_taylor_series.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_template_expr.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_template_expr.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_units.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_units.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_var.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_var.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_var_set_bounds.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_var_set_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_visitor.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_visitor.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/test_xfrm_discrete_vars.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/test_xfrm_discrete_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/uninstantiated_model_linear.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/uninstantiated_model_linear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/tests/unit/uninstantiated_model_quadratic.py` & `Pyomo-6.6.1/pyomo/core/tests/unit/uninstantiated_model_quadratic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/core/util.py` & `Pyomo-6.6.1/pyomo/core/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/__init__.py` & `Pyomo-6.6.1/pyomo/dae/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/contset.py` & `Pyomo-6.6.1/pyomo/dae/contset.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/diffvar.py` & `Pyomo-6.6.1/pyomo/dae/diffvar.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/flatten.py` & `Pyomo-6.6.1/pyomo/dae/flatten.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/initialization.py` & `Pyomo-6.6.1/pyomo/dae/initialization.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/integral.py` & `Pyomo-6.6.1/pyomo/dae/integral.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/misc.py` & `Pyomo-6.6.1/pyomo/dae/misc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/dae/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/plugins/colloc.py` & `Pyomo-6.6.1/pyomo/dae/plugins/colloc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/plugins/finitedifference.py` & `Pyomo-6.6.1/pyomo/dae/plugins/finitedifference.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/set_utils.py` & `Pyomo-6.6.1/pyomo/dae/set_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/simulator.py` & `Pyomo-6.6.1/pyomo/dae/simulator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/__init__.py` & `Pyomo-6.6.1/pyomo/dae/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/test_colloc.py` & `Pyomo-6.6.1/pyomo/dae/tests/test_colloc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/test_contset.py` & `Pyomo-6.6.1/pyomo/dae/tests/test_contset.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/test_diffvar.py` & `Pyomo-6.6.1/pyomo/dae/tests/test_diffvar.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/test_finite_diff.py` & `Pyomo-6.6.1/pyomo/dae/tests/test_finite_diff.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/test_flatten.py` & `Pyomo-6.6.1/pyomo/dae/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/test_initialization.py` & `Pyomo-6.6.1/pyomo/dae/tests/test_initialization.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/test_integral.py` & `Pyomo-6.6.1/pyomo/dae/tests/test_integral.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/test_misc.py` & `Pyomo-6.6.1/pyomo/dae/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/test_set_utils.py` & `Pyomo-6.6.1/pyomo/dae/tests/test_set_utils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/tests/test_simulator.py` & `Pyomo-6.6.1/pyomo/dae/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dae/utilities.py` & `Pyomo-6.6.1/pyomo/dae/utilities.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/DataPortal.py` & `Pyomo-6.6.1/pyomo/dataportal/DataPortal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/TableData.py` & `Pyomo-6.6.1/pyomo/dataportal/TableData.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/__init__.py` & `Pyomo-6.6.1/pyomo/dataportal/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/factory.py` & `Pyomo-6.6.1/pyomo/dataportal/factory.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/parse_datacmds.py` & `Pyomo-6.6.1/pyomo/dataportal/parse_datacmds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/dataportal/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/plugins/csv_table.py` & `Pyomo-6.6.1/pyomo/dataportal/plugins/csv_table.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/plugins/datacommands.py` & `Pyomo-6.6.1/pyomo/dataportal/plugins/datacommands.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/plugins/db_table.py` & `Pyomo-6.6.1/pyomo/dataportal/plugins/db_table.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/plugins/json_dict.py` & `Pyomo-6.6.1/pyomo/dataportal/plugins/json_dict.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/plugins/sheet.py` & `Pyomo-6.6.1/pyomo/dataportal/plugins/sheet.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/plugins/text.py` & `Pyomo-6.6.1/pyomo/dataportal/plugins/text.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/plugins/xml_table.py` & `Pyomo-6.6.1/pyomo/dataportal/plugins/xml_table.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/process_data.py` & `Pyomo-6.6.1/pyomo/dataportal/process_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/tests/__init__.py` & `Pyomo-6.6.1/pyomo/dataportal/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/tests/test_dat_parser.py` & `Pyomo-6.6.1/pyomo/dataportal/tests/test_dat_parser.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/dataportal/tests/test_dataportal.py` & `Pyomo-6.6.1/pyomo/dataportal/tests/test_dataportal.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/duality/__init__.py` & `Pyomo-6.6.1/pyomo/duality/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/duality/collect.py` & `Pyomo-6.6.1/pyomo/duality/collect.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/duality/lagrangian_dual.py` & `Pyomo-6.6.1/pyomo/duality/lagrangian_dual.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/duality/plugins.py` & `Pyomo-6.6.1/pyomo/duality/plugins.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/duality/tests/__init__.py` & `Pyomo-6.6.1/pyomo/duality/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/duality/tests/test_linear_dual.py` & `Pyomo-6.6.1/pyomo/duality/tests/test_linear_dual.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/environ/__init__.py` & `Pyomo-6.6.1/pyomo/environ/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/environ/tests/__init__.py` & `Pyomo-6.6.1/pyomo/environ/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/environ/tests/standalone_minimal_pyomo_driver.py` & `Pyomo-6.6.1/pyomo/environ/tests/standalone_minimal_pyomo_driver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/environ/tests/test_environ.py` & `Pyomo-6.6.1/pyomo/environ/tests/test_environ.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/environ/tests/test_package_layout.py` & `Pyomo-6.6.1/pyomo/environ/tests/test_package_layout.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/__init__.py` & `Pyomo-6.6.1/pyomo/gdp/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/basic_step.py` & `Pyomo-6.6.1/pyomo/gdp/basic_step.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/disjunct.py` & `Pyomo-6.6.1/pyomo/gdp/disjunct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/between_steps.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/between_steps.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/bigm.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/bigm.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/bigm_mixin.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/bigm_mixin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/bilinear.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/bilinear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/bound_pretransformation.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/bound_pretransformation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/chull.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/chull.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/cuttingplane.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/cuttingplane.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/fix_disjuncts.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/fix_disjuncts.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/gdp_to_mip_transformation.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/gdp_to_mip_transformation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/gdp_var_mover.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/gdp_var_mover.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/hull.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/hull.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/multiple_bigm.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/multiple_bigm.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/plugins/partition_disjuncts.py` & `Pyomo-6.6.1/pyomo/gdp/plugins/partition_disjuncts.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/__init__.py` & `Pyomo-6.6.1/pyomo/gdp/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/common_tests.py` & `Pyomo-6.6.1/pyomo/gdp/tests/common_tests.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/models.py` & `Pyomo-6.6.1/pyomo/gdp/tests/models.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_basic_step.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_basic_step.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_bigm.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_bigm.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_bound_pretransformation.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_bound_pretransformation.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_cuttingplane.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_cuttingplane.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_disjunct.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_disjunct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_fix_disjuncts.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_fix_disjuncts.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_gdp.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_gdp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_gdp_reclassification_error.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_gdp_reclassification_error.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_hull.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_hull.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_mbigm.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_mbigm.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_partition_disjuncts.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_partition_disjuncts.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_reclassify.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_reclassify.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/tests/test_util.py` & `Pyomo-6.6.1/pyomo/gdp/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/transformed_disjunct.py` & `Pyomo-6.6.1/pyomo/gdp/transformed_disjunct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/gdp/util.py` & `Pyomo-6.6.1/pyomo/gdp/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/kernel/__init__.py` & `Pyomo-6.6.1/pyomo/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/kernel/util.py` & `Pyomo-6.6.1/pyomo/kernel/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/__init__.py` & `Pyomo-6.6.1/pyomo/mpec/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/complementarity.py` & `Pyomo-6.6.1/pyomo/mpec/complementarity.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/mpec/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/plugins/mpec1.py` & `Pyomo-6.6.1/pyomo/mpec/plugins/mpec1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/plugins/mpec2.py` & `Pyomo-6.6.1/pyomo/mpec/plugins/mpec2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/plugins/mpec3.py` & `Pyomo-6.6.1/pyomo/mpec/plugins/mpec3.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/plugins/mpec4.py` & `Pyomo-6.6.1/pyomo/mpec/plugins/mpec4.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/plugins/pathampl.py` & `Pyomo-6.6.1/pyomo/mpec/plugins/pathampl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/plugins/solver1.py` & `Pyomo-6.6.1/pyomo/mpec/plugins/solver1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/plugins/solver2.py` & `Pyomo-6.6.1/pyomo/mpec/plugins/solver2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/tests/__init__.py` & `Pyomo-6.6.1/pyomo/mpec/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/tests/test_complementarity.py` & `Pyomo-6.6.1/pyomo/mpec/tests/test_complementarity.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/tests/test_minlp.py` & `Pyomo-6.6.1/pyomo/mpec/tests/test_minlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/tests/test_nlp.py` & `Pyomo-6.6.1/pyomo/mpec/tests/test_nlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/mpec/tests/test_path.py` & `Pyomo-6.6.1/pyomo/mpec/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/neos/__init__.py` & `Pyomo-6.6.1/pyomo/neos/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/neos/kestrel.py` & `Pyomo-6.6.1/pyomo/neos/kestrel.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/neos/plugins/NEOS.py` & `Pyomo-6.6.1/pyomo/neos/plugins/NEOS.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/neos/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/neos/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/neos/plugins/kestrel_plugin.py` & `Pyomo-6.6.1/pyomo/neos/plugins/kestrel_plugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/neos/tests/__init__.py` & `Pyomo-6.6.1/pyomo/neos/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/neos/tests/model_min_lp.py` & `Pyomo-6.6.1/pyomo/neos/tests/model_min_lp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/neos/tests/test_neos.py` & `Pyomo-6.6.1/pyomo/neos/tests/test_neos.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/__init__.py` & `Pyomo-6.6.1/pyomo/network/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/arc.py` & `Pyomo-6.6.1/pyomo/network/arc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/decomposition.py` & `Pyomo-6.6.1/pyomo/network/decomposition.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/foqus_graph.py` & `Pyomo-6.6.1/pyomo/network/foqus_graph.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/network/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/plugins/expand_arcs.py` & `Pyomo-6.6.1/pyomo/network/plugins/expand_arcs.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/port.py` & `Pyomo-6.6.1/pyomo/network/port.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/tests/__init__.py` & `Pyomo-6.6.1/pyomo/network/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/tests/test_arc.py` & `Pyomo-6.6.1/pyomo/network/tests/test_arc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/tests/test_decomposition.py` & `Pyomo-6.6.1/pyomo/network/tests/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/tests/test_port.py` & `Pyomo-6.6.1/pyomo/network/tests/test_port.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/network/util.py` & `Pyomo-6.6.1/pyomo/network/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/__init__.py` & `Pyomo-6.6.1/pyomo/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/base/__init__.py` & `Pyomo-6.6.1/pyomo/opt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/base/convert.py` & `Pyomo-6.6.1/pyomo/opt/base/convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/base/error.py` & `Pyomo-6.6.1/pyomo/opt/base/error.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/base/formats.py` & `Pyomo-6.6.1/pyomo/opt/base/formats.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/base/opt_config.py` & `Pyomo-6.6.1/pyomo/opt/base/opt_config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/base/problem.py` & `Pyomo-6.6.1/pyomo/opt/base/problem.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/base/results.py` & `Pyomo-6.6.1/pyomo/opt/base/results.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/base/solvers.py` & `Pyomo-6.6.1/pyomo/opt/base/solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/parallel/__init__.py` & `Pyomo-6.6.1/pyomo/opt/parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/parallel/async_solver.py` & `Pyomo-6.6.1/pyomo/opt/parallel/async_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/parallel/local.py` & `Pyomo-6.6.1/pyomo/opt/parallel/local.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/parallel/manager.py` & `Pyomo-6.6.1/pyomo/opt/parallel/manager.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/opt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/plugins/driver.py` & `Pyomo-6.6.1/pyomo/opt/plugins/driver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/plugins/res.py` & `Pyomo-6.6.1/pyomo/opt/plugins/res.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/plugins/sol.py` & `Pyomo-6.6.1/pyomo/opt/plugins/sol.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/problem/__init__.py` & `Pyomo-6.6.1/pyomo/opt/problem/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/problem/ampl.py` & `Pyomo-6.6.1/pyomo/opt/problem/ampl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/results/__init__.py` & `Pyomo-6.6.1/pyomo/opt/results/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/results/container.py` & `Pyomo-6.6.1/pyomo/opt/results/container.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/results/problem.py` & `Pyomo-6.6.1/pyomo/opt/results/problem.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/results/results_.py` & `Pyomo-6.6.1/pyomo/opt/results/results_.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/results/solution.py` & `Pyomo-6.6.1/pyomo/opt/results/solution.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/results/solver.py` & `Pyomo-6.6.1/pyomo/opt/results/solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/solver/__init__.py` & `Pyomo-6.6.1/pyomo/opt/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/solver/ilmcmd.py` & `Pyomo-6.6.1/pyomo/opt/solver/ilmcmd.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/solver/shellcmd.py` & `Pyomo-6.6.1/pyomo/opt/solver/shellcmd.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/testing/__init__.py` & `Pyomo-6.6.1/pyomo/opt/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/testing/pyunit.py` & `Pyomo-6.6.1/pyomo/opt/testing/pyunit.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/tests/__init__.py` & `Pyomo-6.6.1/pyomo/opt/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/tests/base/__init__.py` & `Pyomo-6.6.1/pyomo/opt/tests/base/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/tests/base/test_ampl.py` & `Pyomo-6.6.1/pyomo/opt/tests/base/test_ampl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/tests/base/test_convert.py` & `Pyomo-6.6.1/pyomo/opt/tests/base/test_convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/tests/base/test_factory.py` & `Pyomo-6.6.1/pyomo/opt/tests/base/test_factory.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/tests/base/test_sol.py` & `Pyomo-6.6.1/pyomo/opt/tests/base/test_sol.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/tests/base/test_soln.py` & `Pyomo-6.6.1/pyomo/opt/tests/base/test_soln.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/tests/base/test_solver.py` & `Pyomo-6.6.1/pyomo/opt/tests/base/test_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/tests/solver/__init__.py` & `Pyomo-6.6.1/pyomo/opt/tests/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/opt/tests/solver/test_shellcmd.py` & `Pyomo-6.6.1/pyomo/opt/tests/solver/test_shellcmd.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/pysp/__init__.py` & `Pyomo-6.6.1/pyomo/pysp/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/__init__.py` & `Pyomo-6.6.1/pyomo/repn/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/beta/__init__.py` & `Pyomo-6.6.1/pyomo/repn/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/beta/matrix.py` & `Pyomo-6.6.1/pyomo/repn/beta/matrix.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/linear.py` & `Pyomo-6.6.1/pyomo/repn/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,14 +340,16 @@
         _type, _arg = arg1
         ans = _type, _arg.duplicate()
         for i in range(1, exp):
             ans = visitor.exit_node_dispatcher[(ProductExpression, ans[0], _type)](
                 visitor, None, ans, (_type, _arg.duplicate())
             )
         return ans
+    elif exp == 0:
+        return _CONSTANT, 1
     else:
         return _handle_pow_nonlinear(visitor, node, arg1, arg2)
 
 
 def _handle_pow_nonlinear(visitor, node, arg1, arg2):
     ans = visitor.Result()
     ans.nonlinear = to_expression(visitor, arg1) ** to_expression(visitor, arg2)
```

### Comparing `Pyomo-6.6.0/pyomo/repn/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/repn/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/plugins/ampl/__init__.py` & `Pyomo-6.6.1/pyomo/repn/plugins/ampl/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/plugins/ampl/ampl_.py` & `Pyomo-6.6.1/pyomo/repn/plugins/ampl/ampl_.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/plugins/baron_writer.py` & `Pyomo-6.6.1/pyomo/repn/plugins/baron_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/plugins/cpxlp.py` & `Pyomo-6.6.1/pyomo/repn/plugins/cpxlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/plugins/gams_writer.py` & `Pyomo-6.6.1/pyomo/repn/plugins/gams_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/plugins/lp_writer.py` & `Pyomo-6.6.1/pyomo/repn/plugins/lp_writer.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/plugins/mps.py` & `Pyomo-6.6.1/pyomo/repn/plugins/mps.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/plugins/nl_writer.py` & `Pyomo-6.6.1/pyomo/repn/plugins/nl_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,15 +680,15 @@
 
         n_lcons = 0  # We do not yet support logical constraints
 
         # We need to check the SOS constraints before finalizing the
         # variable order because the SOS constraint *could* reference a
         # variable not yet seen in the model.
         for block in component_map[SOSConstraint]:
-            for sos in block.component_objects(
+            for sos in block.component_data_objects(
                 SOSConstraint, active=True, descend_into=False, sort=sorter
             ):
                 for v in sos.variables:
                     if id(v) not in var_map:
                         _id = id(v)
                         var_map[_id] = v
                         con_vars_linear.add(_id)
```

### Comparing `Pyomo-6.6.0/pyomo/repn/quadratic.py` & `Pyomo-6.6.1/pyomo/repn/quadratic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/standard_aux.py` & `Pyomo-6.6.1/pyomo/repn/standard_aux.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/standard_repn.py` & `Pyomo-6.6.1/pyomo/repn/standard_repn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/__init__.py` & `Pyomo-6.6.1/pyomo/repn/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/helper.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/helper.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/nl_diff.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/nl_diff.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small10_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small10_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small11_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small11_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small12_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small12_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small13_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small13_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small14_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small14_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small15_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small15_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small1_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small1_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small2_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small2_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small3_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small3_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small4_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small4_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small5_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small5_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small6_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small6_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small7_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small7_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small8_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small8_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/small9_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/small9_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/test_ampl_comparison.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/test_ampl_comparison.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/test_ampl_nl.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/test_ampl_nl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/test_ampl_repn.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/test_ampl_repn.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/test_nlv2.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/test_nlv2.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     Var,
     log,
     ExternalFunction,
     Suffix,
     Constraint,
     Expression,
 )
+import pyomo.environ as pyo
 
 _invalid_1j = r'InvalidNumber\((\([-+0-9.e]+\+)?1j\)?\)'
 
 
 class INFO(object):
     def __init__(self, symbolic=False):
         if symbolic:
@@ -955,7 +956,77 @@
 J0 2
 0 5
 1 10
 """,
                 OUT.getvalue(),
             )
         )
+
+    def test_indexed_sos_constraints(self):
+        # This tests the example from issue #2827
+        m = pyo.ConcreteModel()
+        m.A = pyo.Set(initialize=[1])
+        m.B = pyo.Set(initialize=[1, 2, 3])
+        m.C = pyo.Set(initialize=[1])
+
+        m.param_cx = pyo.Param(m.A, initialize={1: 1})
+        m.param_cy = pyo.Param(m.B, initialize={1: 2, 2: 3, 3: 1})
+
+        m.x = pyo.Var(m.A, domain=pyo.NonNegativeReals, bounds=(0, 40))
+        m.y = pyo.Var(m.B, domain=pyo.NonNegativeIntegers)
+
+        @m.Objective()
+        def OBJ(m):
+            return sum(m.param_cx[a] * m.x[a] for a in m.A) + sum(
+                m.param_cy[b] * m.y[b] for b in m.B
+            )
+
+        m.y[3].bounds = (2, 3)
+
+        m.mysos = pyo.SOSConstraint(
+            m.C, var=m.y, sos=1, index={1: [2, 3]}, weights={2: 25.0, 3: 18.0}
+        )
+
+        OUT = io.StringIO()
+        with LoggingIntercept() as LOG:
+            nl_writer.NLWriter().write(m, OUT, symbolic_solver_labels=True)
+        self.assertEqual(LOG.getvalue(), "")
+        self.assertEqual(
+            *nl_diff(
+                """g3 1 1 0        # problem unknown
+ 4 0 1 0 0      # vars, constraints, objectives, ranges, eqns
+ 0 0 0 0 0 0    # nonlinear constrs, objs; ccons: lin, nonlin, nd, nzlb
+ 0 0    # network constraints: nonlinear, linear
+ 0 0 0  # nonlinear vars in constraints, objectives, both
+ 0 0 0 1        # linear network variables; functions; arith, flags
+ 0 3 0 0 0      # discrete variables: binary, integer, nonlinear (b,c,o)
+ 0 4    # nonzeros in Jacobian, obj. gradient
+ 3 4    # max name lengths: constraints, variables
+ 0 0 0 0 0      # common exprs: b,c,o,c1,o1
+S0 2 sosno
+2 1
+3 1
+S0 2 ref
+2 25.0
+3 18.0
+O0 0    #OBJ
+n0
+x0      # initial guess
+r       #0 ranges (rhs's)
+b       #4 bounds (on variables)
+0 0 40  #x[1]
+2 0     #y[1]
+2 0     #y[2]
+0 2 3   #y[3]
+k3      #intermediate Jacobian column lengths
+0
+0
+0
+G0 4    #OBJ
+0 1
+1 2
+2 3
+3 1
+""",
+                OUT.getvalue(),
+            )
+        )
```

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/ampl/test_suffixes.py` & `Pyomo-6.6.1/pyomo/repn/tests/ampl/test_suffixes.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/baron/__init__.py` & `Pyomo-6.6.1/pyomo/repn/tests/baron/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/baron/small14a_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/baron/small14a_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/baron/test_baron.py` & `Pyomo-6.6.1/pyomo/repn/tests/baron/test_baron.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/baron/test_baron_comparison.py` & `Pyomo-6.6.1/pyomo/repn/tests/baron/test_baron_comparison.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/cpxlp/__init__.py` & `Pyomo-6.6.1/pyomo/repn/tests/cpxlp/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/cpxlp/test_cpxlp.py` & `Pyomo-6.6.1/pyomo/repn/tests/cpxlp/test_cpxlp.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/diffutils.py` & `Pyomo-6.6.1/pyomo/repn/tests/diffutils.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/gams/__init__.py` & `Pyomo-6.6.1/pyomo/repn/tests/gams/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/gams/small14a_testCase.py` & `Pyomo-6.6.1/pyomo/repn/tests/gams/small14a_testCase.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/gams/test_gams.py` & `Pyomo-6.6.1/pyomo/repn/tests/gams/test_gams.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/gams/test_gams_comparison.py` & `Pyomo-6.6.1/pyomo/repn/tests/gams/test_gams_comparison.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/lp_diff.py` & `Pyomo-6.6.1/pyomo/repn/tests/lp_diff.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/mps/__init__.py` & `Pyomo-6.6.1/pyomo/repn/tests/mps/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/mps/test_mps.py` & `Pyomo-6.6.1/pyomo/repn/tests/mps/test_mps.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/nl_diff.py` & `Pyomo-6.6.1/pyomo/repn/tests/nl_diff.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/test_linear.py` & `Pyomo-6.6.1/pyomo/repn/tests/test_linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -848,14 +848,26 @@
         self.assertEqual(cfg.var_map, {id(m.x): m.x})
         self.assertEqual(cfg.var_order, {id(m.x): 0})
         self.assertEqual(repn.multiplier, 1)
         self.assertEqual(repn.constant, 0)
         self.assertEqual(repn.linear, {id(m.x): 1})
         self.assertEqual(repn.nonlinear, None)
 
+        m.p = 0
+
+        cfg = VisitorConfig()
+        repn = LinearRepnVisitor(*cfg).walk_expression(e)
+        self.assertEqual(cfg.subexpr, {})
+        self.assertEqual(cfg.var_map, {id(m.x): m.x})
+        self.assertEqual(cfg.var_order, {id(m.x): 0})
+        self.assertEqual(repn.multiplier, 1)
+        self.assertEqual(repn.constant, 1)
+        self.assertEqual(repn.linear, {})
+        self.assertEqual(repn.nonlinear, None)
+
         m.p = 2
 
         cfg = VisitorConfig()
         repn = LinearRepnVisitor(*cfg).walk_expression(e)
         self.assertEqual(cfg.subexpr, {})
         self.assertEqual(cfg.var_map, {id(m.x): m.x})
         self.assertEqual(cfg.var_order, {id(m.x): 0})
```

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/test_quadratic.py` & `Pyomo-6.6.1/pyomo/repn/tests/test_quadratic.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/test_standard.py` & `Pyomo-6.6.1/pyomo/repn/tests/test_standard.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/tests/test_util.py` & `Pyomo-6.6.1/pyomo/repn/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/repn/util.py` & `Pyomo-6.6.1/pyomo/repn/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/__init__.py` & `Pyomo-6.6.1/pyomo/scripting/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/commands.py` & `Pyomo-6.6.1/pyomo/scripting/commands.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/convert.py` & `Pyomo-6.6.1/pyomo/scripting/convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/driver_help.py` & `Pyomo-6.6.1/pyomo/scripting/driver_help.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/interface.py` & `Pyomo-6.6.1/pyomo/scripting/interface.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/scripting/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/plugins/build_ext.py` & `Pyomo-6.6.1/pyomo/scripting/plugins/build_ext.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/plugins/convert.py` & `Pyomo-6.6.1/pyomo/scripting/plugins/convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/plugins/download.py` & `Pyomo-6.6.1/pyomo/scripting/plugins/download.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/plugins/extras.py` & `Pyomo-6.6.1/pyomo/scripting/plugins/extras.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/plugins/solve.py` & `Pyomo-6.6.1/pyomo/scripting/plugins/solve.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/pyomo_command.py` & `Pyomo-6.6.1/pyomo/scripting/pyomo_command.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/pyomo_main.py` & `Pyomo-6.6.1/pyomo/scripting/pyomo_main.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/pyomo_parser.py` & `Pyomo-6.6.1/pyomo/scripting/pyomo_parser.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/solve_config.py` & `Pyomo-6.6.1/pyomo/scripting/solve_config.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/tests/__init__.py` & `Pyomo-6.6.1/pyomo/scripting/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/tests/test_cmds.py` & `Pyomo-6.6.1/pyomo/scripting/tests/test_cmds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/scripting/util.py` & `Pyomo-6.6.1/pyomo/scripting/util.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/__init__.py` & `Pyomo-6.6.1/pyomo/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/mockmip.py` & `Pyomo-6.6.1/pyomo/solvers/mockmip.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/__init__.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/converter/__init__.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/converter/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/converter/ampl.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/converter/ampl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/converter/glpsol.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/converter/glpsol.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/converter/model.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/converter/model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/converter/pico.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/converter/pico.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/ASL.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/ASL.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/BARON.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/BARON.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/CBCplugin.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/CBCplugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/CONOPT.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/CONOPT.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/CPLEX.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/CPLEX.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/GAMS.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/GAMS.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/GLPK.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/GLPK.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/GUROBI.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/GUROBI.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/GUROBI_RUN.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/GUROBI_RUN.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/IPOPT.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/IPOPT.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/SCIPAMPL.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/SCIPAMPL.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/XPRESS.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/XPRESS.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/__init__.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/cplex_direct.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/cplex_direct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/cplex_persistent.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/cplex_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/direct_or_persistent_solver.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/direct_or_persistent_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/direct_solver.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/direct_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/gurobi_direct.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/gurobi_direct.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,23 +70,88 @@
     # without a license, which means we can't explicitly test for that
     # exception!
     catch_exceptions=(Exception,),
     callback=_parse_gurobi_version,
 )
 
 
+def _set_options(model_or_env, options):
+    # Set a parameters from the dictionary 'options' on the given gurobipy
+    # model or environment.
+    for key, option in options.items():
+        # When options come from the pyomo command, all
+        # values are string types, so we try to cast
+        # them to a numeric value in the event that
+        # setting the parameter fails.
+        try:
+            model_or_env.setParam(key, option)
+        except TypeError:
+            # we place the exception handling for
+            # checking the cast of option to a float in
+            # another function so that we can simply
+            # call raise here instead of except
+            # TypeError as e / raise e, because the
+            # latter does not preserve the Gurobi stack
+            # trace
+            if not _is_numeric(option):
+                raise
+            model_or_env.setParam(key, float(option))
+
+
 @SolverFactory.register('gurobi_direct', doc='Direct python interface to Gurobi')
 class GurobiDirect(DirectSolver):
-    _verified_license = None
-    _import_messages = ''
+    """A direct interface to Gurobi using gurobipy.
+
+    :param manage_env: Set to True if this solver instance should create and
+        manage its own Gurobi environment (defaults to False)
+    :type manage_env: bool
+    :param options: Dictionary of Gurobi parameters to set
+    :type options: dict
+
+    If ``manage_env`` is set to True, the ``GurobiDirect`` object creates a local
+    Gurobi environment and manage all associated Gurobi resources. Importantly,
+    this enables Gurobi licenses to be freed and connections terminated when the
+    solver context is exited::
+
+        with SolverFactory('gurobi', solver_io='python', manage_env=True) as opt:
+            opt.solve(model)
+
+        # All Gurobi models and environments are freed
+
+    If ``manage_env`` is set to False (the default), the ``GurobiDirect`` object
+    uses the global default Gurobi environment::
+
+        with SolverFactory('gurobi', solver_io='python') as opt:
+            opt.solve(model)
+
+        # Only models created by `opt` are freed, the global default
+        # environment remains active
+
+    ``manage_env=True`` is required when setting license or connection parameters
+    programmatically. The ``options`` argument is used to pass parameters to the
+    Gurobi environment. For example, to connect to a Gurobi Cluster Manager::
+
+        options = {
+            "CSManager": "<url>",
+            "CSAPIAccessID": "<access-id>",
+            "CSAPISecret": "<api-key>",
+        }
+        with SolverFactory(
+            'gurobi', solver_io='python', manage_env=True, options=options
+        ) as opt:
+            opt.solve(model)  # Model solved on compute server
+        # Compute server connection terminated
+    """
+
     _name = None
     _version = 0
     _version_major = 0
+    _default_env_started = False
 
-    def __init__(self, **kwds):
+    def __init__(self, manage_env=False, **kwds):
         if 'type' not in kwds:
             kwds['type'] = 'gurobi_direct'
         super(GurobiDirect, self).__init__(**kwds)
         self._pyomo_var_to_solver_var_map = ComponentMap()
         self._solver_var_to_pyomo_var_map = ComponentMap()
         self._pyomo_con_to_solver_con_map = dict()
         self._solver_con_to_pyomo_con_map = ComponentMap()
@@ -117,90 +182,87 @@
             self._capabilities.quadratic_constraint = False
 
         # remove the instance-level definition of the gurobi version:
         # because the version comes from an imported module, only one
         # version of gurobi is supported (and stored as a class attribute)
         del self._version
 
+        self._manage_env = manage_env
+        self._env = None
+        self._env_options = None
+        self._solver_model = None
+
     def available(self, exception_flag=True):
+        """Returns True if the solver is available.
+
+        :param exception_flag: If True, raise an exception instead of returning
+            False if the solver is unavailable (defaults to False)
+        :type exception_flag: bool
+
+        In general, ``available()`` does not need to be called by the user, as
+        the check is run automatically when solving a model. However it is useful
+        for a simple retry loop when using a shared Gurobi license::
+
+            with SolverFactory('gurobi', solver_io='python') as opt:
+                while not available(exception_flag=False):
+                    time.sleep(1)
+                opt.solve(model)
+
+        """
+        # First check gurobipy is imported
         if not gurobipy_available:
             if exception_flag:
                 gurobipy.log_import_warning(logger=__name__)
                 raise ApplicationError(
                     "No Python bindings available for %s solver plugin" % (type(self),)
                 )
             return False
-        if self._verified_license is None:
-            with capture_output(capture_fd=True) as OUT:
-                try:
-                    # verify that we can get a Gurobi license
-                    # Gurobipy writes out license file information when creating
-                    # the environment
-                    m = gurobipy.Model()
-                    m.dispose()
-                    GurobiDirect._verified_license = True
-                except Exception as e:
-                    GurobiDirect._import_messages += (
-                        "\nCould not create Model - gurobi message=%s\n" % (e,)
-                    )
-                    GurobiDirect._verified_license = False
-            if OUT.getvalue():
-                GurobiDirect._import_messages += "\n" + OUT.getvalue()
-        if exception_flag and not self._verified_license:
-            logger.warning(GurobiDirect._import_messages)
+
+        # Ensure environment is started to check for a valid license
+        with capture_output(capture_fd=True) as OUT:
+            try:
+                self._init_env()
+                return True
+            except gurobipy.GurobiError as e:
+                msg = "Could not create Model - gurobi message=%s\n" % (e,)
+        if OUT.getvalue():
+            msg += "\n" + OUT.getvalue()
+        # Didn't return, so environment start failed
+        if exception_flag:
+            logger.warning(msg)
             raise ApplicationError(
-                "Could not create a gurobipy Model for %s solver plugin" % (type(self),)
+                "Could not create Model for %s solver plugin - gurobi message=%s"
+                % (type(self), msg)
             )
-        return self._verified_license
+        else:
+            return False
 
     def _apply_solver(self):
         StaleFlagManager.mark_all_as_stale()
 
         if self._tee:
             self._solver_model.setParam('OutputFlag', 1)
         else:
             self._solver_model.setParam('OutputFlag', 0)
 
         if self._keepfiles:
             # Only save log file when the user wants to keep it.
             self._solver_model.setParam('LogFile', self._log_file)
             print("Solver log file: " + self._log_file)
 
-        # Options accepted by gurobi (case insensitive):
-        # ['Cutoff', 'IterationLimit', 'NodeLimit', 'SolutionLimit', 'TimeLimit',
-        #  'FeasibilityTol', 'IntFeasTol', 'MarkowitzTol', 'MIPGap', 'MIPGapAbs',
-        #  'OptimalityTol', 'PSDTol', 'Method', 'PerturbValue', 'ObjScale', 'ScaleFlag',
-        #  'SimplexPricing', 'Quad', 'NormAdjust', 'BarIterLimit', 'BarConvTol',
-        #  'BarCorrectors', 'BarOrder', 'Crossover', 'CrossoverBasis', 'BranchDir',
-        #  'Heuristics', 'MinRelNodes', 'MIPFocus', 'NodefileStart', 'NodefileDir',
-        #  'NodeMethod', 'PumpPasses', 'RINS', 'SolutionNumber', 'SubMIPNodes', 'Symmetry',
-        #  'VarBranch', 'Cuts', 'CutPasses', 'CliqueCuts', 'CoverCuts', 'CutAggPasses',
-        #  'FlowCoverCuts', 'FlowPathCuts', 'GomoryPasses', 'GUBCoverCuts', 'ImpliedCuts',
-        #  'MIPSepCuts', 'MIRCuts', 'NetworkCuts', 'SubMIPCuts', 'ZeroHalfCuts', 'ModKCuts',
-        #  'Aggregate', 'AggFill', 'PreDual', 'DisplayInterval', 'IISMethod', 'InfUnbdInfo',
-        #  'LogFile', 'PreCrush', 'PreDepRow', 'PreMIQPMethod', 'PrePasses', 'Presolve',
-        #  'ResultFile', 'ImproveStartTime', 'ImproveStartGap', 'Threads', 'Dummy', 'OutputFlag']
-        for key, option in self.options.items():
-            # When options come from the pyomo command, all
-            # values are string types, so we try to cast
-            # them to a numeric value in the event that
-            # setting the parameter fails.
-            try:
-                self._solver_model.setParam(key, option)
-            except TypeError:
-                # we place the exception handling for
-                # checking the cast of option to a float in
-                # another function so that we can simply
-                # call raise here instead of except
-                # TypeError as e / raise e, because the
-                # latter does not preserve the Gurobi stack
-                # trace
-                if not _is_numeric(option):
-                    raise
-                self._solver_model.setParam(key, float(option))
+        # Only pass along changed parameters to the model
+        if self._env_options:
+            new_options = {
+                key: option
+                for key, option in self.options.items()
+                if key not in self._env_options or self._env_options[key] != option
+            }
+        else:
+            new_options = self.options
+        _set_options(self._solver_model, new_options)
 
         if self._version_major >= 5:
             for suffix in self._suffixes:
                 if re.match(suffix, "dual"):
                     self._solver_model.setParam(gurobipy.GRB.Param.QCPDual, 1)
 
         self._solver_model.optimize(self._callback)
@@ -290,26 +352,118 @@
 
         self._pyomo_var_to_solver_var_map[var] = gurobipy_var
         self._solver_var_to_pyomo_var_map[gurobipy_var] = var
         self._referenced_variables[var] = 0
 
         self._needs_updated = True
 
+    def close_global(self):
+        """Frees all Gurobi models used by this solver, and frees the global
+        default Gurobi environment.
+
+        The default environment is used by all ``GurobiDirect`` solvers started
+        with ``manage_env=False`` (the default). To guarantee that all Gurobi
+        resources are freed, all instantiated ``GurobiDirect`` solvers must also
+        be correctly closed.
+
+        The following example will free all Gurobi resources assuming the user did
+        not create any other models (e.g. via another ``GurobiDirect`` object with
+        ``manage_env=False``)::
+
+            opt = SolverFactory('gurobi', solver_io='python')
+            try:
+                opt.solve(model)
+            finally:
+                opt.close_global()
+            # All Gurobi models created by `opt` are freed and the default
+            # Gurobi environment is closed
+        """
+        self.close()
+        with capture_output(capture_fd=True):
+            gurobipy.disposeDefaultEnv()
+        GurobiDirect._default_env_started = False
+
+    def _init_env(self):
+        if self._manage_env:
+            # Ensure an environment is active for this instance
+            if self._env is None:
+                assert self._solver_model is None
+                env = gurobipy.Env(empty=True)
+                _set_options(env, self.options)
+                env.start()
+                # Successful start (no errors): store the environment
+                self._env = env
+                self._env_options = dict(self.options)
+        else:
+            # Ensure the (global) default env is started
+            if not GurobiDirect._default_env_started:
+                m = gurobipy.Model()
+                m.close()
+                GurobiDirect._default_env_started = True
+
+    def _create_model(self, model):
+        self._init_env()
+        if self._solver_model is not None:
+            self._solver_model.close()
+        if model.name is not None:
+            self._solver_model = gurobipy.Model(model.name, env=self._env)
+        else:
+            self._solver_model = gurobipy.Model(env=self._env)
+
+    def close(self):
+        """Frees local Gurobi resources used by this solver instance.
+
+        All Gurobi models created by the solver are freed. If the solver was
+        created with ``manage_env=True``, this method also closes the Gurobi
+        environment used by this solver instance. Calling ``.close()`` achieves
+        the same result as exiting the solver context (although using context
+        managers is preferred where possible)::
+
+            opt = SolverFactory('gurobi', solver_io='python', manage_env=True)
+            try:
+                opt.solve(model)
+            finally:
+                opt.close()
+            # Gurobi models and environments created by `opt` are freed
+
+        As with the context manager, if ``manage_env=False`` (the default) was
+        used, only the Gurobi models created by this solver are freed. The
+        default global Gurobi environment will still be active::
+
+            opt = SolverFactory('gurobi', solver_io='python')
+            try:
+                opt.solve(model)
+            finally:
+                opt.close()
+            # Gurobi models created by `opt` are freed; however the
+            # default/global Gurobi environment is still active
+        """
+
+        if self._solver_model is not None:
+            self._solver_model.close()
+            self._solver_model = None
+        if self._manage_env:
+            if self._env is not None:
+                self._env.close()
+                self._env = None
+                self._env_options = None
+
+    def __exit__(self, t, v, traceback):
+        super().__exit__(t, v, traceback)
+        self.close()
+
     def _set_instance(self, model, kwds={}):
         self._range_constraints = set()
         DirectOrPersistentSolver._set_instance(self, model, kwds)
         self._pyomo_con_to_solver_con_map = dict()
         self._solver_con_to_pyomo_con_map = ComponentMap()
         self._pyomo_var_to_solver_var_map = ComponentMap()
         self._solver_var_to_pyomo_var_map = ComponentMap()
         try:
-            if model.name is not None:
-                self._solver_model = gurobipy.Model(model.name)
-            else:
-                self._solver_model = gurobipy.Model()
+            self._create_model(model)
         except Exception:
             e = sys.exc_info()[1]
             msg = (
                 "Unable to create Gurobi model. "
                 "Have you installed the Python "
                 "bindings for Gurobi?\n\n\t" + "Error message: {0}".format(e)
             )
```

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/gurobi_persistent.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/gurobi_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/mosek_direct.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/mosek_direct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/mosek_persistent.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/mosek_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/persistent_solver.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/persistent_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/pywrapper.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/pywrapper.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/xpress_direct.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/xpress_direct.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/plugins/solvers/xpress_persistent.py` & `Pyomo-6.6.1/pyomo/solvers/plugins/solvers/xpress_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/__init__.py` & `Pyomo-6.6.1/pyomo/solvers/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/__init__.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_BARON.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_BARON.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_CBCplugin.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_CBCplugin.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_CPLEXDirect.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_CPLEXDirect.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_CPLEXPersistent.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_CPLEXPersistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_GAMS.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_GAMS.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_MOSEKDirect.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_MOSEKDirect.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_MOSEKPersistent.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_MOSEKPersistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_cbc.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_cbc.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_cplex.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_cplex.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_gurobi.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_gurobi.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_gurobi_persistent.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_gurobi_persistent.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 import pyomo.common.unittest as unittest
 import pyomo.environ as pyo
 from pyomo.core.expr.taylor_series import taylor_series_expansion
 
 try:
     import gurobipy
 
-    m = gurobipy.Model()
+    with gurobipy.Env():
+        pass
+
     gurobipy_available = True
 except:
     gurobipy_available = False
 
 
 class TestGurobiPersistent(unittest.TestCase):
     @unittest.skipIf(not gurobipy_available, "gurobipy is not available")
```

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_no_solution_behavior.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_no_solution_behavior.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_pickle.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_pickle.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_writers.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_writers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/checks/test_xpress_persistent.py` & `Pyomo-6.6.1/pyomo/solvers/tests/checks/test_xpress_persistent.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/__init__.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/model.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/model.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/test_asl.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/test_asl.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/test_convert.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/test_convert.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/test_factory.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/test_factory.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/test_ipopt.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/test_ipopt.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/test_mip.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/test_mip.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/test_scip.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/test_scip.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/test_scip_log_data.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/test_scip_log_data.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/test_scip_version.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/test_scip_version.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/mip/test_solver.py` & `Pyomo-6.6.1/pyomo/solvers/tests/mip/test_solver.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_block.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_block.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_compiled.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_compiled.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_constant_objective1.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_constant_objective1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_constant_objective2.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_constant_objective2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_duals_maximize.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_duals_maximize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_duals_minimize.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_duals_minimize.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_inactive_index.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_inactive_index.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_infeasible1.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_infeasible1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_infeasible2.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_infeasible2.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_piecewise.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_piecewise.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_simple.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_trivial_constraints.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_trivial_constraints.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_unbounded.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_unbounded.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_unique_duals.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_unique_duals.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/LP_unused_vars.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/LP_unused_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/MILP_discrete_var_bounds.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/MILP_discrete_var_bounds.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/MILP_infeasible1.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/MILP_infeasible1.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/MILP_simple.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/MILP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/MILP_unbounded.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/MILP_unbounded.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/MILP_unused_vars.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/MILP_unused_vars.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/MIQCP_simple.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/MIQCP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/MIQP_simple.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/MIQP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/QCP_simple.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/QCP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/QP_constant_objective.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/QP_constant_objective.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/QP_simple.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/QP_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/SOS1_simple.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/SOS1_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/SOS2_simple.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/SOS2_simple.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/__init__.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/models/base.py` & `Pyomo-6.6.1/pyomo/solvers/tests/models/base.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/piecewise_linear/__init__.py` & `Pyomo-6.6.1/pyomo/solvers/tests/piecewise_linear/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/piecewise_linear/test_examples.py` & `Pyomo-6.6.1/pyomo/solvers/tests/piecewise_linear/test_examples.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear.py` & `Pyomo-6.6.1/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear_kernel.py` & `Pyomo-6.6.1/pyomo/solvers/tests/piecewise_linear/test_piecewise_linear_kernel.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/solvers.py` & `Pyomo-6.6.1/pyomo/solvers/tests/solvers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/tests/testcases.py` & `Pyomo-6.6.1/pyomo/solvers/tests/testcases.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/solvers/wrappers.py` & `Pyomo-6.6.1/pyomo/solvers/wrappers.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/blockutil.py` & `Pyomo-6.6.1/pyomo/util/blockutil.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/calc_var_value.py` & `Pyomo-6.6.1/pyomo/util/calc_var_value.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/check_units.py` & `Pyomo-6.6.1/pyomo/util/check_units.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/components.py` & `Pyomo-6.6.1/pyomo/util/components.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/diagnostics.py` & `Pyomo-6.6.1/pyomo/util/diagnostics.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/infeasible.py` & `Pyomo-6.6.1/pyomo/util/infeasible.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/model_size.py` & `Pyomo-6.6.1/pyomo/util/model_size.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/report_scaling.py` & `Pyomo-6.6.1/pyomo/util/report_scaling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/slices.py` & `Pyomo-6.6.1/pyomo/util/slices.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/subsystems.py` & `Pyomo-6.6.1/pyomo/util/subsystems.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/tests/test_blockutil.py` & `Pyomo-6.6.1/pyomo/util/tests/test_blockutil.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/tests/test_calc_var_value.py` & `Pyomo-6.6.1/pyomo/util/tests/test_calc_var_value.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/tests/test_check_units.py` & `Pyomo-6.6.1/pyomo/util/tests/test_check_units.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/tests/test_components.py` & `Pyomo-6.6.1/pyomo/util/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/tests/test_infeasible.py` & `Pyomo-6.6.1/pyomo/util/tests/test_infeasible.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/tests/test_model_size.py` & `Pyomo-6.6.1/pyomo/util/tests/test_model_size.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/tests/test_report_scaling.py` & `Pyomo-6.6.1/pyomo/util/tests/test_report_scaling.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/tests/test_slices.py` & `Pyomo-6.6.1/pyomo/util/tests/test_slices.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/tests/test_subsystems.py` & `Pyomo-6.6.1/pyomo/util/tests/test_subsystems.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/util/vars_from_expressions.py` & `Pyomo-6.6.1/pyomo/util/vars_from_expressions.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/version/__init__.py` & `Pyomo-6.6.1/pyomo/version/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/version/info.py` & `Pyomo-6.6.1/pyomo/version/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #
 # The VOTD zipbuilder will automatically change releaselevel to "VOTD
 # {hash}" and set the serial number to YYMMDDhhmm.  The serial number
 # should generally be left at 0, unless a downstream package is tracking
 # main and needs a hard reference to "suitably new" development.
 major = 6
 minor = 6
-micro = 0
+micro = 1
 # releaselevel = 'invalid'
 releaselevel = 'final'
 serial = 0
 
 if releaselevel == 'final':
     pass
 elif '/tags/' in _init_url:  # pragma:nocover
```

### Comparing `Pyomo-6.6.0/pyomo/version/tests/__init__.py` & `Pyomo-6.6.1/pyomo/version/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/version/tests/check.py` & `Pyomo-6.6.1/pyomo/version/tests/check.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/pyomo/version/tests/test_version.py` & `Pyomo-6.6.1/pyomo/version/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/setup.cfg` & `Pyomo-6.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `Pyomo-6.6.0/setup.py` & `Pyomo-6.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,17 +260,16 @@
             # 'PeekNamedPipe' is available from pywin32
             'pywin32; platform_system=="Windows"',
             #
             # The following optional dependencies are difficult to
             # install on PyPy (binary wheels are not available), so we
             # will only "require" them on other (CPython) platforms:
             #
-            # DAE can use casadi; as of 1 Nov 22, casadi has not been
-            # released for Python 3.11
-            'casadi; implementation_name!="pypy" and python_version<"3.11"',
+            # DAE can use casadi
+            'casadi; implementation_name!="pypy"',
             'numdifftools; implementation_name!="pypy"',  # pynumero
             'pandas; implementation_name!="pypy"',
             'seaborn; implementation_name!="pypy"',  # parmest.graphics
         ],
     },
     packages=find_packages(exclude=("scripts",)),
     package_data={
```

