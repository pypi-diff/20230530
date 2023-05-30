# Comparing `tmp/conan-2.0.5.tar.gz` & `tmp/conan-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/conan-2.0.5.tar", last modified: Thu May 18 13:49:06 2023, max compression
+gzip compressed data, was "dist/conan-2.0.6.tar", last modified: Fri May 26 11:31:04 2023, max compression
```

## Comparing `conan-2.0.5.tar` & `conan-2.0.6.tar`

### file list

```diff
@@ -1,349 +1,349 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.151381 conan-2.0.5/
--rw-r--r--   0 root         (0) root         (0)     1084 2023-05-18 13:48:59.000000 conan-2.0.5/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-18 13:48:59.000000 conan-2.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8324 2023-05-18 13:49:06.152381 conan-2.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6041 2023-05-18 13:48:59.000000 conan-2.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.107377 conan-2.0.5/conan/
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-18 13:48:59.000000 conan-2.0.5/conan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.108377 conan-2.0.5/conan/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2360 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/conan_api.py
--rw-r--r--   0 root         (0) root         (0)     5892 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/model.py
--rw-r--r--   0 root         (0) root         (0)     8089 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.111378 conan-2.0.5/conan/api/subapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4308 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/cache.py
--rw-r--r--   0 root         (0) root         (0)     1101 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/config.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/download.py
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/export.py
--rw-r--r--   0 root         (0) root         (0)    11124 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/graph.py
--rw-r--r--   0 root         (0) root         (0)     3131 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/install.py
--rw-r--r--   0 root         (0) root         (0)     7652 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/list.py
--rw-r--r--   0 root         (0) root         (0)     5110 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/local.py
--rw-r--r--   0 root         (0) root         (0)     4386 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/lockfile.py
--rw-r--r--   0 root         (0) root         (0)     4864 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/new.py
--rw-r--r--   0 root         (0) root         (0)     4426 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/profiles.py
--rw-r--r--   0 root         (0) root         (0)     4478 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/remotes.py
--rw-r--r--   0 root         (0) root         (0)     2212 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/remove.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/search.py
--rw-r--r--   0 root         (0) root         (0)     3907 2023-05-18 13:48:59.000000 conan-2.0.5/conan/api/subapi/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.111378 conan-2.0.5/conan/cli/
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7582 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/args.py
--rw-r--r--   0 root         (0) root         (0)    10967 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     6522 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.115378 conan-2.0.5/conan/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3311 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/build.py
--rw-r--r--   0 root         (0) root         (0)     4419 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/cache.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)     8474 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/create.py
--rw-r--r--   0 root         (0) root         (0)     3065 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/download.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/editable.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/export.py
--rw-r--r--   0 root         (0) root         (0)     5634 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/export_pkg.py
--rw-r--r--   0 root         (0) root         (0)     8632 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/graph.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/inspect.py
--rw-r--r--   0 root         (0) root         (0)     4827 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)     5192 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/list.py
--rw-r--r--   0 root         (0) root         (0)     5485 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/lock.py
--rw-r--r--   0 root         (0) root         (0)     4239 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/new.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/profile.py
--rw-r--r--   0 root         (0) root         (0)    11410 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/remote.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/remove.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/search.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/source.py
--rw-r--r--   0 root         (0) root         (0)     3717 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/test.py
--rw-r--r--   0 root         (0) root         (0)     3830 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/commands/upload.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/exit_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.115378 conan-2.0.5/conan/cli/formatters/
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.116378 conan-2.0.5/conan/cli/formatters/graph/
--rw-r--r--   0 root         (0) root         (0)      110 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5019 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/graph/graph_info_text.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/graph/info_graph_dot.py
--rw-r--r--   0 root         (0) root         (0)     5583 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/graph/info_graph_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.116378 conan-2.0.5/conan/cli/formatters/list/
--rw-r--r--   0 root         (0) root         (0)       37 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4612 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/list/binary_html_table.py
--rw-r--r--   0 root         (0) root         (0)      939 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/list/list.py
--rw-r--r--   0 root         (0) root         (0)    12834 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/formatters/list/search_table_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.117378 conan-2.0.5/conan/cli/printers/
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/printers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5649 2023-05-18 13:48:59.000000 conan-2.0.5/conan/cli/printers/graph.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-05-18 13:48:59.000000 conan-2.0.5/conan/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.117378 conan-2.0.5/conan/internal/
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.117378 conan-2.0.5/conan/internal/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.119378 conan-2.0.5/conan/internal/api/new/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/alias_new.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/autoools_exe.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/autotools_lib.py
--rw-r--r--   0 root         (0) root         (0)     2843 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/basic.py
--rw-r--r--   0 root         (0) root         (0)     2066 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/bazel_exe.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/bazel_lib.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/cmake_exe.py
--rw-r--r--   0 root         (0) root         (0)     7076 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/cmake_lib.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/meson_exe.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/meson_lib.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/msbuild_exe.py
--rw-r--r--   0 root         (0) root         (0)    12247 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/api/new/msbuild_lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.120378 conan-2.0.5/conan/internal/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10247 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/conan_reference_layout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.120378 conan-2.0.5/conan/internal/cache/db/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3842 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/db/cache_database.py
--rw-r--r--   0 root         (0) root         (0)     7953 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/db/packages_table.py
--rw-r--r--   0 root         (0) root         (0)     5264 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/db/recipes_table.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/cache/db/table.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/conan_app.py
--rw-r--r--   0 root         (0) root         (0)     3490 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/deploy.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-05-18 13:48:59.000000 conan-2.0.5/conan/internal/integrity_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.121379 conan-2.0.5/conan/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.121379 conan-2.0.5/conan/tools/android/
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/android/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1138 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/android/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.122379 conan-2.0.5/conan/tools/apple/
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/apple/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11201 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/apple/apple.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/apple/xcodebuild.py
--rw-r--r--   0 root         (0) root         (0)    16380 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/apple/xcodedeps.py
--rw-r--r--   0 root         (0) root         (0)     5683 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/apple/xcodetoolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.123379 conan-2.0.5/conan/tools/build/
--rw-r--r--   0 root         (0) root         (0)     4143 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11104 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/cppstd.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/cpu.py
--rw-r--r--   0 root         (0) root         (0)     2043 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/cross_building.py
--rw-r--r--   0 root         (0) root         (0)    15410 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/flags.py
--rw-r--r--   0 root         (0) root         (0)      563 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/build/stdcpp_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.124379 conan-2.0.5/conan/tools/cmake/
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9956 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.124379 conan-2.0.5/conan/tools/cmake/cmakedeps/
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8152 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/cmakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.125379 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/
--rw-r--r--   0 root         (0) root         (0)     4273 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4451 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/config.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/config_version.py
--rw-r--r--   0 root         (0) root         (0)     5704 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/macros.py
--rw-r--r--   0 root         (0) root         (0)    14925 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/target_configuration.py
--rw-r--r--   0 root         (0) root         (0)    19484 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/target_data.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/cmakedeps/templates/targets.py
--rw-r--r--   0 root         (0) root         (0)     5365 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/file_api.py
--rw-r--r--   0 root         (0) root         (0)     4045 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/layout.py
--rw-r--r--   0 root         (0) root         (0)    14423 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/presets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.126379 conan-2.0.5/conan/tools/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/toolchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35919 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/toolchain/blocks.py
--rw-r--r--   0 root         (0) root         (0)    11205 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/toolchain/toolchain.py
--rw-r--r--   0 root         (0) root         (0)      171 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/cmake/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.126379 conan-2.0.5/conan/tools/env/
--rw-r--r--   0 root         (0) root         (0)      168 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25389 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/env/environment.py
--rw-r--r--   0 root         (0) root         (0)     3233 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/env/virtualbuildenv.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/env/virtualrunenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.127379 conan-2.0.5/conan/tools/files/
--rw-r--r--   0 root         (0) root         (0)      572 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1468 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/conandata.py
--rw-r--r--   0 root         (0) root         (0)     6009 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/copy_pattern.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/cpp_package.py
--rw-r--r--   0 root         (0) root         (0)    24621 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/files.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/packager.py
--rw-r--r--   0 root         (0) root         (0)     5824 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/patches.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.128379 conan-2.0.5/conan/tools/files/symlinks/
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/symlinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/files/symlinks/symlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.129379 conan-2.0.5/conan/tools/gnu/
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6234 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/autotools.py
--rw-r--r--   0 root         (0) root         (0)     2954 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/autotoolsdeps.py
--rw-r--r--   0 root         (0) root         (0)    13228 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/autotoolstoolchain.py
--rw-r--r--   0 root         (0) root         (0)     3557 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/get_gnu_triplet.py
--rw-r--r--   0 root         (0) root         (0)     3596 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/gnudeps_flags.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/pkgconfig.py
--rw-r--r--   0 root         (0) root         (0)    17816 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/gnu/pkgconfigdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.130379 conan-2.0.5/conan/tools/google/
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/google/bazel.py
--rw-r--r--   0 root         (0) root         (0)    10956 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/google/bazeldeps.py
--rw-r--r--   0 root         (0) root         (0)      585 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/google/layout.py
--rw-r--r--   0 root         (0) root         (0)      857 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/google/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.130379 conan-2.0.5/conan/tools/intel/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/intel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/intel/intel_cc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.130379 conan-2.0.5/conan/tools/layout/
--rw-r--r--   0 root         (0) root         (0)      605 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/layout/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.131379 conan-2.0.5/conan/tools/meson/
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/meson/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4073 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/meson/helpers.py
--rw-r--r--   0 root         (0) root         (0)     3880 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/meson/meson.py
--rw-r--r--   0 root         (0) root         (0)    22075 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/meson/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.132379 conan-2.0.5/conan/tools/microsoft/
--rw-r--r--   0 root         (0) root         (0)      558 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/layout.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/msbuild.py
--rw-r--r--   0 root         (0) root         (0)    19194 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/msbuilddeps.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/nmakedeps.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/nmaketoolchain.py
--rw-r--r--   0 root         (0) root         (0)      596 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/subsystems.py
--rw-r--r--   0 root         (0) root         (0)    10844 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/toolchain.py
--rw-r--r--   0 root         (0) root         (0)    13070 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/microsoft/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.133380 conan-2.0.5/conan/tools/premake/
--rw-r--r--   0 root         (0) root         (0)      103 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/premake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/premake/premake.py
--rw-r--r--   0 root         (0) root         (0)    10592 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/premake/premakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.133380 conan-2.0.5/conan/tools/qbs/
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/qbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/qbs/qbs.py
--rw-r--r--   0 root         (0) root         (0)     9874 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/qbs/qbsprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.133380 conan-2.0.5/conan/tools/scm/
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/scm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8619 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/scm/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.134380 conan-2.0.5/conan/tools/system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16286 2023-05-18 13:48:59.000000 conan-2.0.5/conan/tools/system/package_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.108377 conan-2.0.5/conan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8324 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9035 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      470 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 13:49:06.000000 conan-2.0.5/conan.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.135380 conan-2.0.5/conans/
--rw-r--r--   0 root         (0) root         (0)      201 2023-05-18 13:48:59.000000 conan-2.0.5/conans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.137380 conan-2.0.5/conans/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.138380 conan-2.0.5/conans/client/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10687 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cache/editable.py
--rw-r--r--   0 root         (0) root         (0)     6569 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cache/remote_registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.138380 conan-2.0.5/conans/client/cmd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cmd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7671 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cmd/export.py
--rw-r--r--   0 root         (0) root         (0)    12827 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cmd/uploader.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/cmd/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.139380 conan-2.0.5/conans/client/conanfile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conanfile/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conanfile/build.py
--rw-r--r--   0 root         (0) root         (0)     2208 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conanfile/configure.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conanfile/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.140380 conan-2.0.5/conans/client/conf/
--rw-r--r--   0 root         (0) root         (0)     6347 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9195 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conf/config_installer.py
--rw-r--r--   0 root         (0) root         (0)    14006 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conf/detect.py
--rw-r--r--   0 root         (0) root         (0)     5473 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conf/detect_vs.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/conf/required_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.140380 conan-2.0.5/conans/client/downloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/downloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9459 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/downloaders/caching_file_downloader.py
--rw-r--r--   0 root         (0) root         (0)     3856 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/downloaders/download_cache.py
--rw-r--r--   0 root         (0) root         (0)     6126 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/downloaders/file_downloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.141380 conan-2.0.5/conans/client/generators/
--rw-r--r--   0 root         (0) root         (0)     9520 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/generators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.143380 conan-2.0.5/conans/client/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/build_mode.py
--rw-r--r--   0 root         (0) root         (0)     4571 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/compatibility.py
--rw-r--r--   0 root         (0) root         (0)     3832 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/compute_pid.py
--rw-r--r--   0 root         (0) root         (0)    14526 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)    16759 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/graph_binaries.py
--rw-r--r--   0 root         (0) root         (0)    17797 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/graph_builder.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/graph_error.py
--rw-r--r--   0 root         (0) root         (0)    12486 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/install_graph.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/profile_node_definer.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/provides.py
--rw-r--r--   0 root         (0) root         (0)     6536 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/proxy.py
--rw-r--r--   0 root         (0) root         (0)     5806 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/python_requires.py
--rw-r--r--   0 root         (0) root         (0)     4692 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/graph/range_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2595 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/hook_manager.py
--rw-r--r--   0 root         (0) root         (0)    21320 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/installer.py
--rw-r--r--   0 root         (0) root         (0)    15815 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/loader.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/loader_txt.py
--rw-r--r--   0 root         (0) root         (0)     1860 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/migrations.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/pkg_sign.py
--rw-r--r--   0 root         (0) root         (0)    16848 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/profile_loader.py
--rw-r--r--   0 root         (0) root         (0)    11423 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/remote_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.144380 conan-2.0.5/conans/client/rest/
--rw-r--r--   0 root         (0) root         (0)      838 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5987 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/auth_manager.py
--rw-r--r--   0 root         (0) root         (0)     6132 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/client_routes.py
--rw-r--r--   0 root         (0) root         (0)     6894 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/conan_requester.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/file_uploader.py
--rw-r--r--   0 root         (0) root         (0)     5388 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/rest_client.py
--rw-r--r--   0 root         (0) root         (0)    10011 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/rest_client_common.py
--rw-r--r--   0 root         (0) root         (0)    13590 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/rest/rest_client_v2.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.144380 conan-2.0.5/conans/client/store/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/store/localdb.py
--rw-r--r--   0 root         (0) root         (0)     8798 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/subsystems.py
--rw-r--r--   0 root         (0) root         (0)     5457 2023-05-18 13:48:59.000000 conan-2.0.5/conans/client/userio.py
--rwxr-xr-x   0 root         (0) root         (0)      118 2023-05-18 13:48:59.000000 conan-2.0.5/conans/conan.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-05-18 13:48:59.000000 conan-2.0.5/conans/conan_server.py
--rw-r--r--   0 root         (0) root         (0)     7817 2023-05-18 13:48:59.000000 conan-2.0.5/conans/errors.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-05-18 13:48:59.000000 conan-2.0.5/conans/migrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.147381 conan-2.0.5/conans/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19581 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/build_info.py
--rw-r--r--   0 root         (0) root         (0)    12460 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/conan_file.py
--rw-r--r--   0 root         (0) root         (0)     2775 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/conanfile_interface.py
--rw-r--r--   0 root         (0) root         (0)    29433 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/conf.py
--rw-r--r--   0 root         (0) root         (0)     5901 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/dependencies.py
--rw-r--r--   0 root         (0) root         (0)    10886 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/graph_lock.py
--rw-r--r--   0 root         (0) root         (0)    13067 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/info.py
--rw-r--r--   0 root         (0) root         (0)     5193 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/layout.py
--rw-r--r--   0 root         (0) root         (0)     4883 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/manifest.py
--rw-r--r--   0 root         (0) root         (0)    17174 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/options.py
--rw-r--r--   0 root         (0) root         (0)     3861 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/package_ref.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/pkg_type.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/profile.py
--rw-r--r--   0 root         (0) root         (0)     7585 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/recipe_ref.py
--rw-r--r--   0 root         (0) root         (0)    24590 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/requires.py
--rw-r--r--   0 root         (0) root         (0)     2171 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/rest_routes.py
--rw-r--r--   0 root         (0) root         (0)    13368 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/settings.py
--rw-r--r--   0 root         (0) root         (0)     6038 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/version.py
--rw-r--r--   0 root         (0) root         (0)     4350 2023-05-18 13:48:59.000000 conan-2.0.5/conans/model/version_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.147381 conan-2.0.5/conans/paths/
--rw-r--r--   0 root         (0) root         (0)     2184 2023-05-18 13:48:59.000000 conan-2.0.5/conans/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-05-18 13:48:59.000000 conan-2.0.5/conans/pylint_plugin.py
--rw-r--r--   0 root         (0) root         (0)      252 2023-05-18 13:48:59.000000 conan-2.0.5/conans/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-05-18 13:48:59.000000 conan-2.0.5/conans/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-18 13:48:59.000000 conan-2.0.5/conans/requirements_server.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.148381 conan-2.0.5/conans/search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3814 2023-05-18 13:48:59.000000 conan-2.0.5/conans/search/query_parse.py
--rw-r--r--   0 root         (0) root         (0)     4384 2023-05-18 13:48:59.000000 conan-2.0.5/conans/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.148381 conan-2.0.5/conans/test/
--rw-r--r--   0 root         (0) root         (0)      203 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13174 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.150381 conan-2.0.5/conans/test/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4868 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/mocks.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/profiles.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/scm.py
--rw-r--r--   0 root         (0) root         (0)     3858 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/server_launcher.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/test_files.py
--rw-r--r--   0 root         (0) root         (0)    35320 2023-05-18 13:48:59.000000 conan-2.0.5/conans/test/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 13:49:06.151381 conan-2.0.5/conans/util/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/config_parser.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/dates.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/encrypt.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/env.py
--rw-r--r--   0 root         (0) root         (0)    11263 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/files.py
--rw-r--r--   0 root         (0) root         (0)     3657 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/locks.py
--rw-r--r--   0 root         (0) root         (0)     3688 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/runners.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/sha.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-18 13:48:59.000000 conan-2.0.5/conans/util/windows.py
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-18 13:49:06.152381 conan-2.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5058 2023-05-18 13:48:59.000000 conan-2.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.210594 conan-2.0.6/
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-05-26 11:30:56.000000 conan-2.0.6/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-26 11:30:56.000000 conan-2.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8324 2023-05-26 11:31:04.210594 conan-2.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6041 2023-05-26 11:30:56.000000 conan-2.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.172591 conan-2.0.6/conan/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-05-26 11:30:56.000000 conan-2.0.6/conan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.174591 conan-2.0.6/conan/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/conan_api.py
+-rw-r--r--   0 root         (0) root         (0)     5892 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/model.py
+-rw-r--r--   0 root         (0) root         (0)     8089 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.175591 conan-2.0.6/conan/api/subapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4308 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/config.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/download.py
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/export.py
+-rw-r--r--   0 root         (0) root         (0)    11124 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3131 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/install.py
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/list.py
+-rw-r--r--   0 root         (0) root         (0)     5110 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/local.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/lockfile.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/new.py
+-rw-r--r--   0 root         (0) root         (0)     4426 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     4478 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/remotes.py
+-rw-r--r--   0 root         (0) root         (0)     2212 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/search.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-05-26 11:30:56.000000 conan-2.0.6/conan/api/subapi/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.176591 conan-2.0.6/conan/cli/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7582 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/args.py
+-rw-r--r--   0 root         (0) root         (0)    11009 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     6522 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.179591 conan-2.0.6/conan/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3311 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/build.py
+-rw-r--r--   0 root         (0) root         (0)     4419 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/cache.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)     8409 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/create.py
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/download.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/editable.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/export.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/export_pkg.py
+-rw-r--r--   0 root         (0) root         (0)     8632 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/inspect.py
+-rw-r--r--   0 root         (0) root         (0)     4787 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/list.py
+-rw-r--r--   0 root         (0) root         (0)     5485 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/lock.py
+-rw-r--r--   0 root         (0) root         (0)     4239 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/new.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/profile.py
+-rw-r--r--   0 root         (0) root         (0)    11410 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/remote.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/search.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/source.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/commands/upload.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/exit_codes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.180591 conan-2.0.6/conan/cli/formatters/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/formatters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.181591 conan-2.0.6/conan/cli/formatters/graph/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/formatters/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/formatters/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/formatters/graph/graph_info_text.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/formatters/graph/info_graph_dot.py
+-rw-r--r--   0 root         (0) root         (0)     5583 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/formatters/graph/info_graph_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.181591 conan-2.0.6/conan/cli/formatters/list/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/formatters/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/formatters/list/binary_html_table.py
+-rw-r--r--   0 root         (0) root         (0)      939 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/formatters/list/list.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/formatters/list/search_table_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.182592 conan-2.0.6/conan/cli/printers/
+-rw-r--r--   0 root         (0) root         (0)      331 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/printers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-05-26 11:30:56.000000 conan-2.0.6/conan/cli/printers/graph.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-05-26 11:30:56.000000 conan-2.0.6/conan/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.182592 conan-2.0.6/conan/internal/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.182592 conan-2.0.6/conan/internal/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.184592 conan-2.0.6/conan/internal/api/new/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/alias_new.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/autoools_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/autotools_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/bazel_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/bazel_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/cmake_exe.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/cmake_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/meson_exe.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/meson_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/msbuild_exe.py
+-rw-r--r--   0 root         (0) root         (0)    12247 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/api/new/msbuild_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.185592 conan-2.0.6/conan/internal/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10247 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/cache/conan_reference_layout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.185592 conan-2.0.6/conan/internal/cache/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/cache/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3842 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/cache/db/cache_database.py
+-rw-r--r--   0 root         (0) root         (0)     7953 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/cache/db/packages_table.py
+-rw-r--r--   0 root         (0) root         (0)     5264 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/cache/db/recipes_table.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/cache/db/table.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/conan_app.py
+-rw-r--r--   0 root         (0) root         (0)     3490 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-05-26 11:30:56.000000 conan-2.0.6/conan/internal/integrity_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.186592 conan-2.0.6/conan/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.186592 conan-2.0.6/conan/tools/android/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/android/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/android/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.186592 conan-2.0.6/conan/tools/apple/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/apple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11201 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/apple/apple.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/apple/xcodebuild.py
+-rw-r--r--   0 root         (0) root         (0)    16380 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/apple/xcodedeps.py
+-rw-r--r--   0 root         (0) root         (0)     5683 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/apple/xcodetoolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.187592 conan-2.0.6/conan/tools/build/
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11104 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/build/cppstd.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/build/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/build/cross_building.py
+-rw-r--r--   0 root         (0) root         (0)    15410 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/build/flags.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/build/stdcpp_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.188592 conan-2.0.6/conan/tools/cmake/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9963 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/cmake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.188592 conan-2.0.6/conan/tools/cmake/cmakedeps/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/cmakedeps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8152 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/cmakedeps/cmakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.189592 conan-2.0.6/conan/tools/cmake/cmakedeps/templates/
+-rw-r--r--   0 root         (0) root         (0)     4273 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/cmakedeps/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/cmakedeps/templates/config.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/cmakedeps/templates/config_version.py
+-rw-r--r--   0 root         (0) root         (0)     5704 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/cmakedeps/templates/macros.py
+-rw-r--r--   0 root         (0) root         (0)    14925 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/cmakedeps/templates/target_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    19484 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/cmakedeps/templates/target_data.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/cmakedeps/templates/targets.py
+-rw-r--r--   0 root         (0) root         (0)     5365 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/file_api.py
+-rw-r--r--   0 root         (0) root         (0)     4045 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/layout.py
+-rw-r--r--   0 root         (0) root         (0)    14423 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/presets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.189592 conan-2.0.6/conan/tools/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/toolchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35919 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/toolchain/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    11205 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/toolchain/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)      171 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/cmake/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.190592 conan-2.0.6/conan/tools/env/
+-rw-r--r--   0 root         (0) root         (0)      168 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25389 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/env/environment.py
+-rw-r--r--   0 root         (0) root         (0)     3233 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/env/virtualbuildenv.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/env/virtualrunenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.191592 conan-2.0.6/conan/tools/files/
+-rw-r--r--   0 root         (0) root         (0)      572 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/files/conandata.py
+-rw-r--r--   0 root         (0) root         (0)     6009 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/files/copy_pattern.py
+-rw-r--r--   0 root         (0) root         (0)     2933 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/files/cpp_package.py
+-rw-r--r--   0 root         (0) root         (0)    24621 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/files/files.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/files/packager.py
+-rw-r--r--   0 root         (0) root         (0)     5824 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/files/patches.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.191592 conan-2.0.6/conan/tools/files/symlinks/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/files/symlinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/files/symlinks/symlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.192592 conan-2.0.6/conan/tools/gnu/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/gnu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6234 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/gnu/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/gnu/autotoolsdeps.py
+-rw-r--r--   0 root         (0) root         (0)    13228 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/gnu/autotoolstoolchain.py
+-rw-r--r--   0 root         (0) root         (0)     3557 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/gnu/get_gnu_triplet.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/gnu/gnudeps_flags.py
+-rw-r--r--   0 root         (0) root         (0)     4029 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/gnu/pkgconfig.py
+-rw-r--r--   0 root         (0) root         (0)    17816 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/gnu/pkgconfigdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.193592 conan-2.0.6/conan/tools/google/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/google/bazel.py
+-rw-r--r--   0 root         (0) root         (0)    10956 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/google/bazeldeps.py
+-rw-r--r--   0 root         (0) root         (0)      585 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/google/layout.py
+-rw-r--r--   0 root         (0) root         (0)      857 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/google/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.193592 conan-2.0.6/conan/tools/intel/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/intel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/intel/intel_cc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.193592 conan-2.0.6/conan/tools/layout/
+-rw-r--r--   0 root         (0) root         (0)      605 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/layout/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.194593 conan-2.0.6/conan/tools/meson/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/meson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4073 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/meson/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     3880 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/meson/meson.py
+-rw-r--r--   0 root         (0) root         (0)    22075 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/meson/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.195592 conan-2.0.6/conan/tools/microsoft/
+-rw-r--r--   0 root         (0) root         (0)      558 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/microsoft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/microsoft/layout.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/microsoft/msbuild.py
+-rw-r--r--   0 root         (0) root         (0)    19194 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/microsoft/msbuilddeps.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/microsoft/nmakedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/microsoft/nmaketoolchain.py
+-rw-r--r--   0 root         (0) root         (0)      596 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/microsoft/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)    10844 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/microsoft/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)    13070 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/microsoft/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.195592 conan-2.0.6/conan/tools/premake/
+-rw-r--r--   0 root         (0) root         (0)      103 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/premake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/premake/premake.py
+-rw-r--r--   0 root         (0) root         (0)    10534 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/premake/premakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.196593 conan-2.0.6/conan/tools/qbs/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/qbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/qbs/qbs.py
+-rw-r--r--   0 root         (0) root         (0)     9874 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/qbs/qbsprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.196593 conan-2.0.6/conan/tools/scm/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/scm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8619 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/scm/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.196593 conan-2.0.6/conan/tools/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16286 2023-05-26 11:30:56.000000 conan-2.0.6/conan/tools/system/package_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.173591 conan-2.0.6/conan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8324 2023-05-26 11:31:03.000000 conan-2.0.6/conan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9035 2023-05-26 11:31:04.000000 conan-2.0.6/conan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 11:31:03.000000 conan-2.0.6/conan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-26 11:31:03.000000 conan-2.0.6/conan.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      470 2023-05-26 11:31:03.000000 conan-2.0.6/conan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-26 11:31:03.000000 conan-2.0.6/conan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.197593 conan-2.0.6/conans/
+-rw-r--r--   0 root         (0) root         (0)      201 2023-05-26 11:30:56.000000 conan-2.0.6/conans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.199593 conan-2.0.6/conans/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.199593 conan-2.0.6/conans/client/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10687 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/cache/editable.py
+-rw-r--r--   0 root         (0) root         (0)     6569 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/cache/remote_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.199593 conan-2.0.6/conans/client/cmd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/cmd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7671 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/cmd/export.py
+-rw-r--r--   0 root         (0) root         (0)    12827 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/cmd/uploader.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/cmd/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.200593 conan-2.0.6/conans/client/conanfile/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/conanfile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/conanfile/build.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/conanfile/configure.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/conanfile/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.201593 conan-2.0.6/conans/client/conf/
+-rw-r--r--   0 root         (0) root         (0)     6347 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9195 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/conf/config_installer.py
+-rw-r--r--   0 root         (0) root         (0)    14006 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/conf/detect.py
+-rw-r--r--   0 root         (0) root         (0)     5473 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/conf/detect_vs.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/conf/required_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.201593 conan-2.0.6/conans/client/downloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/downloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9514 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/downloaders/caching_file_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     3856 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/downloaders/download_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6263 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/downloaders/file_downloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.201593 conan-2.0.6/conans/client/generators/
+-rw-r--r--   0 root         (0) root         (0)     9520 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/generators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.203593 conan-2.0.6/conans/client/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4818 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/build_mode.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/compute_pid.py
+-rw-r--r--   0 root         (0) root         (0)    14873 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)    16759 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/graph_binaries.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/graph_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/graph_error.py
+-rw-r--r--   0 root         (0) root         (0)    12486 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/install_graph.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/profile_node_definer.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/provides.py
+-rw-r--r--   0 root         (0) root         (0)     6536 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     5806 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/python_requires.py
+-rw-r--r--   0 root         (0) root         (0)     4692 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/graph/range_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/hook_manager.py
+-rw-r--r--   0 root         (0) root         (0)    21297 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/installer.py
+-rw-r--r--   0 root         (0) root         (0)    15815 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/loader.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/loader_txt.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/migrations.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/pkg_sign.py
+-rw-r--r--   0 root         (0) root         (0)    16848 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/profile_loader.py
+-rw-r--r--   0 root         (0) root         (0)    11706 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/remote_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.204594 conan-2.0.6/conans/client/rest/
+-rw-r--r--   0 root         (0) root         (0)      838 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5987 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/rest/auth_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/rest/client_routes.py
+-rw-r--r--   0 root         (0) root         (0)     6894 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/rest/conan_requester.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/rest/file_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     5388 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/rest/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)    10011 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/rest/rest_client_common.py
+-rw-r--r--   0 root         (0) root         (0)    13652 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/rest/rest_client_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.204594 conan-2.0.6/conans/client/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/store/localdb.py
+-rw-r--r--   0 root         (0) root         (0)     8798 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)     5457 2023-05-26 11:30:56.000000 conan-2.0.6/conans/client/userio.py
+-rwxr-xr-x   0 root         (0) root         (0)      118 2023-05-26 11:30:56.000000 conan-2.0.6/conans/conan.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-05-26 11:30:56.000000 conan-2.0.6/conans/conan_server.py
+-rw-r--r--   0 root         (0) root         (0)     7817 2023-05-26 11:30:56.000000 conan-2.0.6/conans/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-05-26 11:30:56.000000 conan-2.0.6/conans/migrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.207594 conan-2.0.6/conans/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19600 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/build_info.py
+-rw-r--r--   0 root         (0) root         (0)    12420 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/conan_file.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/conanfile_interface.py
+-rw-r--r--   0 root         (0) root         (0)    29524 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/conf.py
+-rw-r--r--   0 root         (0) root         (0)     5901 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    10886 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/graph_lock.py
+-rw-r--r--   0 root         (0) root         (0)    13067 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/info.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/layout.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/options.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/package_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/pkg_type.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/profile.py
+-rw-r--r--   0 root         (0) root         (0)     7585 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/recipe_ref.py
+-rw-r--r--   0 root         (0) root         (0)    24646 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/requires.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/rest_routes.py
+-rw-r--r--   0 root         (0) root         (0)    13368 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/settings.py
+-rw-r--r--   0 root         (0) root         (0)     6038 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/version.py
+-rw-r--r--   0 root         (0) root         (0)     4350 2023-05-26 11:30:56.000000 conan-2.0.6/conans/model/version_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.207594 conan-2.0.6/conans/paths/
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-05-26 11:30:56.000000 conan-2.0.6/conans/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-05-26 11:30:56.000000 conan-2.0.6/conans/pylint_plugin.py
+-rw-r--r--   0 root         (0) root         (0)      252 2023-05-26 11:30:56.000000 conan-2.0.6/conans/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-26 11:30:56.000000 conan-2.0.6/conans/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-26 11:30:56.000000 conan-2.0.6/conans/requirements_server.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.207594 conan-2.0.6/conans/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2023-05-26 11:30:56.000000 conan-2.0.6/conans/search/query_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4384 2023-05-26 11:30:56.000000 conan-2.0.6/conans/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.207594 conan-2.0.6/conans/test/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-05-26 11:30:56.000000 conan-2.0.6/conans/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13174 2023-05-26 11:30:56.000000 conan-2.0.6/conans/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.208594 conan-2.0.6/conans/test/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/test/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2023-05-26 11:30:56.000000 conan-2.0.6/conans/test/utils/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-05-26 11:30:56.000000 conan-2.0.6/conans/test/utils/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-05-26 11:30:56.000000 conan-2.0.6/conans/test/utils/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-05-26 11:30:56.000000 conan-2.0.6/conans/test/utils/scm.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-05-26 11:30:56.000000 conan-2.0.6/conans/test/utils/server_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-05-26 11:30:56.000000 conan-2.0.6/conans/test/utils/test_files.py
+-rw-r--r--   0 root         (0) root         (0)    35320 2023-05-26 11:30:56.000000 conan-2.0.6/conans/test/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 11:31:04.210594 conan-2.0.6/conans/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/config_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1516 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/dates.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/env.py
+-rw-r--r--   0 root         (0) root         (0)    11263 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/files.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/locks.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/runners.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/sha.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-26 11:30:56.000000 conan-2.0.6/conans/util/windows.py
+-rw-r--r--   0 root         (0) root         (0)      101 2023-05-26 11:31:04.210594 conan-2.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5058 2023-05-26 11:30:56.000000 conan-2.0.6/setup.py
```

### Comparing `conan-2.0.5/LICENSE.md` & `conan-2.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/PKG-INFO` & `conan-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.0.5
+Version: 2.0.6
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.0.5/README.md` & `conan-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/conan_api.py` & `conan-2.0.6/conan/api/conan_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/model.py` & `conan-2.0.6/conan/api/model.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/output.py` & `conan-2.0.6/conan/api/output.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/cache.py` & `conan-2.0.6/conan/api/subapi/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/config.py` & `conan-2.0.6/conan/api/subapi/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/download.py` & `conan-2.0.6/conan/api/subapi/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/export.py` & `conan-2.0.6/conan/api/subapi/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/graph.py` & `conan-2.0.6/conan/api/subapi/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/install.py` & `conan-2.0.6/conan/api/subapi/install.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/list.py` & `conan-2.0.6/conan/api/subapi/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/local.py` & `conan-2.0.6/conan/api/subapi/local.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/lockfile.py` & `conan-2.0.6/conan/api/subapi/lockfile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/new.py` & `conan-2.0.6/conan/api/subapi/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/profiles.py` & `conan-2.0.6/conan/api/subapi/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/remotes.py` & `conan-2.0.6/conan/api/subapi/remotes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/remove.py` & `conan-2.0.6/conan/api/subapi/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/search.py` & `conan-2.0.6/conan/api/subapi/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/api/subapi/upload.py` & `conan-2.0.6/conan/api/subapi/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/args.py` & `conan-2.0.6/conan/cli/args.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/cli.py` & `conan-2.0.6/conan/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                     self._add_command(module_name, module_name.replace("cmd_", ""))
                 except Exception as e:
                     ConanOutput().error("Error loading custom command "
                                         "'{}.py': {}".format(module_name, e))
         # layers
         for folder in os.listdir(custom_commands_path):
             layer_folder = os.path.join(custom_commands_path, folder)
+            sys.path.append(layer_folder)
             if not os.path.isdir(layer_folder):
                 continue
             for module in pkgutil.iter_modules([layer_folder]):
                 module_name = module[1]
                 if module_name.startswith("cmd_"):
                     module_path = f"{folder}.{module_name}"
                     try:
```

### Comparing `conan-2.0.5/conan/cli/command.py` & `conan-2.0.6/conan/cli/command.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/build.py` & `conan-2.0.6/conan/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/cache.py` & `conan-2.0.6/conan/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/config.py` & `conan-2.0.6/conan/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/create.py` & `conan-2.0.6/conan/cli/commands/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,22 @@
-import json
 import os
 import shutil
 
-from conan.api.output import ConanOutput, cli_out_write
+from conan.api.output import ConanOutput
+from conan.cli.args import add_lockfile_args, add_common_install_arguments
 from conan.cli.command import conan_command, OnceArgument
 from conan.cli.commands.export import common_args_export
-from conan.cli.args import add_lockfile_args, add_common_install_arguments
+from conan.cli.formatters.graph import format_graph_json
 from conan.cli.printers import print_profiles
 from conan.cli.printers.graph import print_graph_packages, print_graph_basic
 from conan.errors import ConanException
 from conans.util.files import mkdir
 
 
-def json_create(deps_graph):
-    if deps_graph is None:
-        return
-    cli_out_write(json.dumps({"graph": deps_graph.serialize()}, indent=4))
-
-
-@conan_command(group="Creator", formatters={"json": json_create})
+@conan_command(group="Creator", formatters={"json": format_graph_json})
 def create(conan_api, parser, *args):
     """
     Create a package.
     """
     common_args_export(parser)
     add_lockfile_args(parser)
     add_common_install_arguments(parser)
@@ -98,15 +92,16 @@
         deps_graph = run_test(conan_api, test_conanfile_path, ref, profile_host, profile_build,
                               remotes, lockfile, update=False, build_modes=args.build,
                               tested_python_requires=tested_python_requires)
         lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
                                                       clean=args.lockfile_clean)
 
     conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
-    return deps_graph
+    return {"graph": deps_graph,
+            "conan_api": conan_api}
 
 
 def _check_tested_reference_matches(deps_graph, tested_ref, out):
     """ Check the test_profile_override_conflict test. If we are testing a build require
     but we specify the build require with a different version in the profile, it has priority,
     it is correct but weird and likely a mistake"""
     # https://github.com/conan-io/conan/issues/10453
```

### Comparing `conan-2.0.5/conan/cli/commands/download.py` & `conan-2.0.6/conan/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/editable.py` & `conan-2.0.6/conan/cli/commands/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/export.py` & `conan-2.0.6/conan/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/export_pkg.py` & `conan-2.0.6/conan/cli/commands/export_pkg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-import json
 import os
 
-from conan.api.output import cli_out_write, ConanOutput
-from conan.cli.command import conan_command, OnceArgument
-from conan.cli.args import add_lockfile_args, add_profiles_args, add_reference_args
+from conan.api.output import ConanOutput
 from conan.cli import make_abs_path
+from conan.cli.args import add_lockfile_args, add_profiles_args, add_reference_args
+from conan.cli.command import conan_command, OnceArgument
 from conan.cli.commands.create import _get_test_conanfile_path
+from conan.cli.formatters.graph import format_graph_json
 from conan.cli.printers.graph import print_graph_basic
 
 
-def json_export_pkg(info):
-    deps_graph = info
-    cli_out_write(json.dumps({"graph": deps_graph.serialize()}, indent=4))
-
-
-@conan_command(group="Creator", formatters={"json": json_export_pkg})
+@conan_command(group="Creator", formatters={"json": format_graph_json})
 def export_pkg(conan_api, parser, *args):
     """
     Create a package directly from pre-compiled binaries.
     """
     parser.add_argument("path", help="Path to a folder containing a recipe (conanfile.py)")
     parser.add_argument("-of", "--output-folder",
                         help='The root output folder for generated and build files')
@@ -96,8 +91,9 @@
     if test_conanfile_path:
         from conan.cli.commands.test import run_test
         deps_graph = run_test(conan_api, test_conanfile_path, ref, profile_host, profile_build,
                               remotes=None, lockfile=lockfile, update=False, build_modes=None)
         # TODO: Do something with lockfile, same as create()
 
     conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
-    return deps_graph
+    return {"graph": deps_graph,
+            "conan_api": conan_api}
```

### Comparing `conan-2.0.5/conan/cli/commands/graph.py` & `conan-2.0.6/conan/cli/commands/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/inspect.py` & `conan-2.0.6/conan/cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/install.py` & `conan-2.0.6/conan/cli/commands/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-import json
 import os
 
-from conan.api.output import ConanOutput, cli_out_write
+from conan.api.output import ConanOutput
+from conan.cli import make_abs_path
 from conan.cli.args import common_graph_args, validate_common_graph_args
 from conan.cli.command import conan_command
-from conan.cli import make_abs_path
+from conan.cli.formatters.graph import format_graph_json
 from conan.cli.printers import print_profiles
 from conan.cli.printers.graph import print_graph_packages, print_graph_basic
 
 
-def json_install(info):
-    deps_graph = info
-    cli_out_write(json.dumps({"graph": deps_graph.serialize()}, indent=4))
-
-
-@conan_command(group="Consumer", formatters={"json": json_install})
+@conan_command(group="Consumer", formatters={"json": format_graph_json})
 def install(conan_api, parser, *args):
     """
     Install the requirements specified in a recipe (conanfile.py or conanfile.txt).
 
     It can also be used to install a concrete package specifying a
     reference. If any requirement is not found in the local cache, it will
     retrieve the recipe from a remote, looking for it sequentially in the
@@ -91,8 +86,10 @@
                                        deploy=args.deployer
                                        )
 
     out.success("Install finished successfully")
     lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
                                                   clean=args.lockfile_clean)
     conan_api.lockfile.save_lockfile(lockfile, args.lockfile_out, cwd)
-    return deps_graph
+    return {"graph": deps_graph,
+            "conan_api": conan_api}
+
```

### Comparing `conan-2.0.5/conan/cli/commands/list.py` & `conan-2.0.6/conan/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/lock.py` & `conan-2.0.6/conan/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/new.py` & `conan-2.0.6/conan/cli/commands/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/profile.py` & `conan-2.0.6/conan/cli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/remote.py` & `conan-2.0.6/conan/cli/commands/remote.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/remove.py` & `conan-2.0.6/conan/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/search.py` & `conan-2.0.6/conan/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/source.py` & `conan-2.0.6/conan/cli/commands/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/test.py` & `conan-2.0.6/conan/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/commands/upload.py` & `conan-2.0.6/conan/cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/formatters/graph/graph.py` & `conan-2.0.6/conan/cli/formatters/graph/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from conan.cli.formatters.graph.info_graph_html import graph_info_html
 from conans.client.graph.graph import BINARY_CACHE, \
     BINARY_DOWNLOAD, BINARY_BUILD, BINARY_MISSING, BINARY_UPDATE
 from conans.client.installer import build_id
 from conans.util.files import load
 
 
+# FIXME: Check all this code when format_graph_[html/dot] use serialized graph
+
 class _PrinterGraphItem(object):
     def __init__(self, _id, node, is_build_time_node):
         self.id = _id
         self._ref = node.ref
         self._conanfile = node.conanfile
         self._is_build_time_node = is_build_time_node
         self.package_id = node.package_id
@@ -35,27 +37,21 @@
             return self.label
 
     @property
     def is_build_requires(self):
         return self._is_build_time_node
 
     def data(self):
-
-        def ensure_iterable(value):
-            if isinstance(value, (list, tuple)):
-                return value
-            return value,
-
         return {
             'build_id': build_id(self._conanfile),
             'url': self._conanfile.url,
             'homepage': self._conanfile.homepage,
             'license': self._conanfile.license,
             'author': self._conanfile.author,
-            'topics': ensure_iterable(self._conanfile.topics) if self._conanfile.topics else None
+            'topics': self._conanfile.topics
         }
 
 
 class _Grapher(object):
     def __init__(self, deps_graph):
         self._deps_graph = deps_graph
         self.nodes, self.edges = self._build_graph()
@@ -127,15 +123,15 @@
     cli_out_write(_render_graph(graph, template, template_folder))
     if graph.error:
         raise graph.error
 
 
 def format_graph_json(result):
     graph = result["graph"]
-    field_filter = result["field_filter"]
-    package_filter = result["package_filter"]
+    field_filter = result.get("field_filter")
+    package_filter = result.get("package_filter")
     serial = graph.serialize()
-    serial = filter_graph(serial, package_filter, field_filter)
-    json_result = json.dumps(serial, indent=4)
+    serial = filter_graph(serial, package_filter=package_filter, field_filter=field_filter)
+    json_result = json.dumps({"graph": serial}, indent=4)
     cli_out_write(json_result)
     if graph.error:
         raise graph.error
```

### Comparing `conan-2.0.5/conan/cli/formatters/graph/graph_info_text.py` & `conan-2.0.6/conan/cli/formatters/graph/graph_info_text.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import fnmatch
 from collections import OrderedDict
 
 from conan.api.output import ConanOutput
 
 
-def filter_graph(graph, package_filter, field_filter=None):
+def filter_graph(graph, package_filter=None, field_filter=None):
     if package_filter is not None:
-        graph["nodes"] = [n for n in graph["nodes"]
-                          if any(fnmatch.fnmatch(n["ref"] or "", p) for p in package_filter)]
+        graph["nodes"] = {id_: n for id_, n in graph["nodes"].items()
+                          if any(fnmatch.fnmatch(n["ref"] or "", p) for p in package_filter)}
     if field_filter is not None:
         if "ref" not in field_filter:
             field_filter.append("ref")
-        result = []
-        for n in graph["nodes"]:
+        result = {}
+        for id_, n in graph["nodes"].items():
             new_node = OrderedDict((k, v) for k, v in n.items() if k in field_filter)
-            result.append(new_node)
+            result[id_] = new_node
         graph["nodes"] = result
     return graph
 
 
 def format_graph_info(result):
     """ More complete graph output, including information for every node in the graph
     Used for 'graph info' command
@@ -27,15 +27,15 @@
     field_filter = result["field_filter"]
     package_filter = result["package_filter"]
 
     out = ConanOutput()
     out.title("Basic graph information")
     serial = graph.serialize()
     serial = filter_graph(serial, package_filter, field_filter)
-    for n in serial["nodes"]:
+    for n in serial["nodes"].values():
         out.writeln(f"{n['ref']}:")  # FIXME: This can be empty for consumers and it is ugly ":"
         _serial_pretty_printer(n, indent="  ")
     if graph.error:
         raise graph.error
 
 
 def _serial_pretty_printer(data, indent=""):
```

### Comparing `conan-2.0.5/conan/cli/formatters/graph/info_graph_html.py` & `conan-2.0.6/conan/cli/formatters/graph/info_graph_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/formatters/list/binary_html_table.py` & `conan-2.0.6/conan/cli/formatters/list/binary_html_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/formatters/list/list.py` & `conan-2.0.6/conan/cli/formatters/list/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/formatters/list/search_table_html.py` & `conan-2.0.6/conan/cli/formatters/list/search_table_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/cli/printers/graph.py` & `conan-2.0.6/conan/cli/printers/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,8 +119,8 @@
 
     _format_requires("Requirements", requires)
     _format_requires("Test requirements", test_requires)
     _format_requires("Build requirements", build_requires)
 
     if skipped_requires and not output.level_allowed(LEVEL_VERBOSE):
         output.info("Skipped binaries", Color.BRIGHT_YELLOW)
-        output.info(f"{tab}{skipped_requires}", Color.BRIGHT_CYAN)
+        output.info(f"{tab}{', '.join(skipped_requires)}", Color.BRIGHT_CYAN)
```

### Comparing `conan-2.0.5/conan/internal/api/new/autoools_exe.py` & `conan-2.0.6/conan/internal/api/new/autoools_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/api/new/autotools_lib.py` & `conan-2.0.6/conan/internal/api/new/autotools_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/api/new/basic.py` & `conan-2.0.6/conan/internal/api/new/basic.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/api/new/bazel_exe.py` & `conan-2.0.6/conan/internal/api/new/bazel_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/api/new/bazel_lib.py` & `conan-2.0.6/conan/internal/api/new/bazel_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/api/new/cmake_exe.py` & `conan-2.0.6/conan/internal/api/new/cmake_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/api/new/cmake_lib.py` & `conan-2.0.6/conan/internal/api/new/cmake_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/api/new/meson_exe.py` & `conan-2.0.6/conan/internal/api/new/meson_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/api/new/meson_lib.py` & `conan-2.0.6/conan/internal/api/new/meson_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/api/new/msbuild_exe.py` & `conan-2.0.6/conan/internal/api/new/msbuild_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/api/new/msbuild_lib.py` & `conan-2.0.6/conan/internal/api/new/msbuild_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/cache/cache.py` & `conan-2.0.6/conan/internal/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/cache/conan_reference_layout.py` & `conan-2.0.6/conan/internal/cache/conan_reference_layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/cache/db/cache_database.py` & `conan-2.0.6/conan/internal/cache/db/cache_database.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/cache/db/packages_table.py` & `conan-2.0.6/conan/internal/cache/db/packages_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/cache/db/recipes_table.py` & `conan-2.0.6/conan/internal/cache/db/recipes_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/cache/db/table.py` & `conan-2.0.6/conan/internal/cache/db/table.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/conan_app.py` & `conan-2.0.6/conan/internal/conan_app.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/deploy.py` & `conan-2.0.6/conan/internal/deploy.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/internal/integrity_check.py` & `conan-2.0.6/conan/internal/integrity_check.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/android/utils.py` & `conan-2.0.6/conan/tools/android/utils.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/apple/__init__.py` & `conan-2.0.6/conan/tools/apple/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/apple/apple.py` & `conan-2.0.6/conan/tools/apple/apple.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/apple/xcodebuild.py` & `conan-2.0.6/conan/tools/apple/xcodebuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/apple/xcodedeps.py` & `conan-2.0.6/conan/tools/apple/xcodedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/apple/xcodetoolchain.py` & `conan-2.0.6/conan/tools/apple/xcodetoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/build/__init__.py` & `conan-2.0.6/conan/tools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/build/cppstd.py` & `conan-2.0.6/conan/tools/build/cppstd.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/build/cpu.py` & `conan-2.0.6/conan/tools/build/cpu.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/build/cross_building.py` & `conan-2.0.6/conan/tools/build/cross_building.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/build/flags.py` & `conan-2.0.6/conan/tools/build/flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/build/stdcpp_library.py` & `conan-2.0.6/conan/tools/build/stdcpp_library.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/cmake.py` & `conan-2.0.6/conan/tools/cmake/cmake.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         # Conan generated presets will have exactly 1 configurePresets, no more
         configure_preset = cmake_presets["configurePresets"][0]
 
         self._generator = configure_preset["generator"]
         self._toolchain_file = configure_preset.get("toolchainFile")
         self._cache_variables = configure_preset["cacheVariables"]
 
-        self._cmake_program = "cmake"  # Path to CMake should be handled by environment
+        self._cmake_program = conanfile.conf.get("tools.cmake:cmake_program", default="cmake")
 
     def configure(self, variables=None, build_script_folder=None, cli_args=None):
         """
 
         Reads the ``CMakePresets.json`` file generated by the
         :param cli_args: Extra CLI arguments to pass to cmake invocation
         :ref:`CMakeToolchain<conan-cmake-toolchain>` to get:
```

### Comparing `conan-2.0.5/conan/tools/cmake/cmakedeps/cmakedeps.py` & `conan-2.0.6/conan/tools/cmake/cmakedeps/cmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/__init__.py` & `conan-2.0.6/conan/tools/cmake/cmakedeps/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/config.py` & `conan-2.0.6/conan/tools/cmake/cmakedeps/templates/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/config_version.py` & `conan-2.0.6/conan/tools/cmake/cmakedeps/templates/config_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/macros.py` & `conan-2.0.6/conan/tools/cmake/cmakedeps/templates/macros.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/target_configuration.py` & `conan-2.0.6/conan/tools/cmake/cmakedeps/templates/target_configuration.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/target_data.py` & `conan-2.0.6/conan/tools/cmake/cmakedeps/templates/target_data.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/cmakedeps/templates/targets.py` & `conan-2.0.6/conan/tools/cmake/cmakedeps/templates/targets.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/file_api.py` & `conan-2.0.6/conan/tools/cmake/file_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/layout.py` & `conan-2.0.6/conan/tools/cmake/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/presets.py` & `conan-2.0.6/conan/tools/cmake/presets.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/toolchain/blocks.py` & `conan-2.0.6/conan/tools/cmake/toolchain/blocks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/cmake/toolchain/toolchain.py` & `conan-2.0.6/conan/tools/cmake/toolchain/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/env/environment.py` & `conan-2.0.6/conan/tools/env/environment.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/env/virtualbuildenv.py` & `conan-2.0.6/conan/tools/env/virtualbuildenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/env/virtualrunenv.py` & `conan-2.0.6/conan/tools/env/virtualrunenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/files/__init__.py` & `conan-2.0.6/conan/tools/files/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/files/conandata.py` & `conan-2.0.6/conan/tools/files/conandata.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/files/copy_pattern.py` & `conan-2.0.6/conan/tools/files/copy_pattern.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/files/cpp_package.py` & `conan-2.0.6/conan/tools/files/cpp_package.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/files/files.py` & `conan-2.0.6/conan/tools/files/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/files/packager.py` & `conan-2.0.6/conan/tools/files/packager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/files/patches.py` & `conan-2.0.6/conan/tools/files/patches.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/files/symlinks/symlinks.py` & `conan-2.0.6/conan/tools/files/symlinks/symlinks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/gnu/autotools.py` & `conan-2.0.6/conan/tools/gnu/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/gnu/autotoolsdeps.py` & `conan-2.0.6/conan/tools/gnu/autotoolsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/gnu/autotoolstoolchain.py` & `conan-2.0.6/conan/tools/gnu/autotoolstoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/gnu/get_gnu_triplet.py` & `conan-2.0.6/conan/tools/gnu/get_gnu_triplet.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/gnu/gnudeps_flags.py` & `conan-2.0.6/conan/tools/gnu/gnudeps_flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/gnu/pkgconfig.py` & `conan-2.0.6/conan/tools/gnu/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/gnu/pkgconfigdeps.py` & `conan-2.0.6/conan/tools/gnu/pkgconfigdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/google/bazel.py` & `conan-2.0.6/conan/tools/google/bazel.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/google/bazeldeps.py` & `conan-2.0.6/conan/tools/google/bazeldeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/google/layout.py` & `conan-2.0.6/conan/tools/google/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/google/toolchain.py` & `conan-2.0.6/conan/tools/google/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/intel/intel_cc.py` & `conan-2.0.6/conan/tools/intel/intel_cc.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/layout/__init__.py` & `conan-2.0.6/conan/tools/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/meson/helpers.py` & `conan-2.0.6/conan/tools/meson/helpers.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/meson/meson.py` & `conan-2.0.6/conan/tools/meson/meson.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/meson/toolchain.py` & `conan-2.0.6/conan/tools/meson/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/microsoft/__init__.py` & `conan-2.0.6/conan/tools/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/microsoft/layout.py` & `conan-2.0.6/conan/tools/microsoft/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/microsoft/msbuild.py` & `conan-2.0.6/conan/tools/microsoft/msbuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/microsoft/msbuilddeps.py` & `conan-2.0.6/conan/tools/microsoft/msbuilddeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/microsoft/nmakedeps.py` & `conan-2.0.6/conan/tools/microsoft/nmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/microsoft/nmaketoolchain.py` & `conan-2.0.6/conan/tools/microsoft/nmaketoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/microsoft/subsystems.py` & `conan-2.0.6/conan/tools/microsoft/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/microsoft/toolchain.py` & `conan-2.0.6/conan/tools/microsoft/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/microsoft/visual.py` & `conan-2.0.6/conan/tools/microsoft/visual.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/premake/premake.py` & `conan-2.0.6/conan/tools/premake/premake.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/premake/premakedeps.py` & `conan-2.0.6/conan/tools/premake/premakedeps.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,19 +79,19 @@
     conan_setup_link(conf, pkg)
 end
 """
 
 
 # Helper class that expands cpp_info meta information in lua readable string sequences
 class _PremakeTemplate(object):
-    def __init__(self, dep_cpp_info, pkg_folder):
+    def __init__(self, dep_cpp_info):
         def _format_paths(paths):
             if not paths:
                 return ""
-            return ",\n".join(f'"{pkg_folder}/{p}"'.replace("\\", "/") for p in paths)
+            return ",\n".join(f'"{p}"'.replace("\\", "/") for p in paths)
 
         def _format_flags(flags):
             if not flags:
                 return ""
             return ", ".join('"%s"' % p.replace('"', '\\"') for p in flags)
 
         self.includedirs = _format_paths(dep_cpp_info.includedirs)
@@ -102,15 +102,15 @@
         self.defines = _format_flags(dep_cpp_info.defines)
         self.cxxflags = _format_flags(dep_cpp_info.cxxflags)
         self.cflags = _format_flags(dep_cpp_info.cflags)
         self.sharedlinkflags = _format_flags(dep_cpp_info.sharedlinkflags)
         self.exelinkflags = _format_flags(dep_cpp_info.exelinkflags)
         self.frameworks = ", ".join('"%s.framework"' % p.replace('"', '\\"') for p in
                                     dep_cpp_info.frameworks) if dep_cpp_info.frameworks else ""
-        self.sysroot = f"{pkg_folder}/{dep_cpp_info.sysroot}".replace("\\", "/") \
+        self.sysroot = f"{dep_cpp_info.sysroot}".replace("\\", "/") \
             if dep_cpp_info.sysroot else ""
 
 
 class PremakeDeps(object):
     """
     PremakeDeps class generator
     conandeps.premake5.lua: unconditional import of all *direct* dependencies only
@@ -207,15 +207,15 @@
             # Convert and aggregate dependency's
             dep_aggregate = dep.cpp_info.aggregated_components()
 
             # Generate config dependent package variable and setup premake file
             var_filename = PREMAKE_VAR_FILE.format(pkgname=dep_name, config=conf_suffix)
             self._output_lua_file(var_filename, [
                 PREMAKE_TEMPLATE_VAR.format(pkgname=dep_name,
-                    config=conf_name, deps=_PremakeTemplate(dep_aggregate, dep.package_folder))
+                    config=conf_name, deps=_PremakeTemplate(dep_aggregate))
             ])
 
             # Create list of all available profiles by searching on disk
             file_pattern = PREMAKE_VAR_FILE.format(pkgname=dep_name, config="_*")
             file_regex = PREMAKE_VAR_FILE.format(pkgname=re.escape(dep_name), config="_(([^_]*)_(.*))")
             available_files = glob.glob(file_pattern)
             # Add filename of current generations var file if not already present
```

### Comparing `conan-2.0.5/conan/tools/qbs/qbs.py` & `conan-2.0.6/conan/tools/qbs/qbs.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/qbs/qbsprofile.py` & `conan-2.0.6/conan/tools/qbs/qbsprofile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/scm/git.py` & `conan-2.0.6/conan/tools/scm/git.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan/tools/system/package_manager.py` & `conan-2.0.6/conan/tools/system/package_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conan.egg-info/PKG-INFO` & `conan-2.0.6/conan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.0.5
+Version: 2.0.6
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
```

### Comparing `conan-2.0.5/conan.egg-info/SOURCES.txt` & `conan-2.0.6/conan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/cache/cache.py` & `conan-2.0.6/conans/client/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/cache/editable.py` & `conan-2.0.6/conans/client/cache/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/cache/remote_registry.py` & `conan-2.0.6/conans/client/cache/remote_registry.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/cmd/export.py` & `conan-2.0.6/conans/client/cmd/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/cmd/uploader.py` & `conan-2.0.6/conans/client/cmd/uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/cmd/user.py` & `conan-2.0.6/conans/client/cmd/user.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/conanfile/build.py` & `conan-2.0.6/conans/client/conanfile/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/conanfile/configure.py` & `conan-2.0.6/conans/client/conanfile/configure.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/conanfile/package.py` & `conan-2.0.6/conans/client/conanfile/package.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/conf/__init__.py` & `conan-2.0.6/conans/client/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/conf/config_installer.py` & `conan-2.0.6/conans/client/conf/config_installer.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/conf/detect.py` & `conan-2.0.6/conans/client/conf/detect.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/conf/detect_vs.py` & `conan-2.0.6/conans/client/conf/detect_vs.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/conf/required_version.py` & `conan-2.0.6/conans/client/conf/required_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/downloaders/caching_file_downloader.py` & `conan-2.0.6/conans/client/downloaders/caching_file_downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class SourcesCachingDownloader:
     """ Class for downloading recipe download() urls
     if the config is active, it can use caching/backup-sources
     """
     def __init__(self, conanfile):
         helpers = getattr(conanfile, "_conan_helpers")
         self._global_conf = helpers.global_conf
-        self._file_downloader = FileDownloader(helpers.requester)
+        self._file_downloader = FileDownloader(helpers.requester, scope=conanfile.display_name)
         self._cache = helpers.cache
         self._output = conanfile.output
         self._conanfile = conanfile
 
     def download(self, urls, file_path,
                  retry, retry_wait, verify_ssl, auth, headers, md5, sha1, sha256):
         download_cache_folder = self._global_conf.get("core.sources:download_cache")
@@ -148,19 +148,19 @@
                 else:
                     raise
 
 
 class ConanInternalCacheDownloader:
     """ This is used for the download of Conan packages from server, not for sources/backup sources
     """
-    def __init__(self, requester, config):
+    def __init__(self, requester, config, scope=None):
         self._download_cache = config.get("core.download:download_cache")
         if self._download_cache and not os.path.isabs(self._download_cache):
             raise ConanException("core.download:download_cache must be an absolute path")
-        self._file_downloader = FileDownloader(requester)
+        self._file_downloader = FileDownloader(requester, scope=scope)
 
     def download(self, url, file_path, auth, verify_ssl, retry, retry_wait):
         if not self._download_cache:
             self._file_downloader.download(url, file_path, retry=retry, retry_wait=retry_wait,
                                            verify_ssl=verify_ssl, auth=auth, overwrite=False)
             return
```

### Comparing `conan-2.0.5/conans/client/downloaders/download_cache.py` & `conan-2.0.6/conans/client/downloaders/download_cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/downloaders/file_downloader.py` & `conan-2.0.6/conans/client/downloaders/file_downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from conans.errors import ConanException, NotFoundException, AuthenticationException, \
     ForbiddenException, ConanConnectionError, RequestErrorException
 from conans.util.sha import check_with_algorithm_sum
 
 
 class FileDownloader:
 
-    def __init__(self, requester):
-        self._output = ConanOutput()
+    def __init__(self, requester, scope=None):
+        self._output = ConanOutput(scope=scope)
         self._requester = requester
 
     def download(self, url, file_path, retry=2, retry_wait=0, verify_ssl=True, auth=None,
                  overwrite=False, headers=None, md5=None, sha1=None, sha256=None):
         """ in order to make the download concurrent, the folder for file_path MUST exist
         """
         assert file_path, "Conan 2.0 always downloads files to disk, not to memory"
@@ -98,17 +98,19 @@
                 return int(match.group(3))
             else:
                 total_size = response.headers.get('Content-Length') or len(response.content)
                 return int(total_size)
 
         try:
             total_length = get_total_length()
-            if total_length > 100000:
+            if total_length > 1000000:  # 10 Mb
+                from conan.tools.files.files import _human_size
+                hs = _human_size(total_length)
                 action = "Downloading" if range_start == 0 else "Continuing download of"
-                description = f"${action} {os.path.basename(file_path)} from {url}"
+                description = f"{action} {hs} {os.path.basename(file_path)}"
                 self._output.info(description)
 
             chunk_size = 1024 * 100
             total_downloaded_size = range_start
             mode = "ab" if range_start else "wb"
             with open(file_path, mode) as file_handler:
                 for chunk in response.iter_content(chunk_size):
```

### Comparing `conan-2.0.5/conans/client/generators/__init__.py` & `conan-2.0.6/conans/client/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/build_mode.py` & `conan-2.0.6/conans/client/graph/build_mode.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/compatibility.py` & `conan-2.0.6/conans/client/graph/compatibility.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/compute_pid.py` & `conan-2.0.6/conans/client/graph/compute_pid.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/graph.py` & `conan-2.0.6/conans/client/graph/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -218,17 +218,19 @@
         result["build_id"] = build_id(self.conanfile)
         result["binary"] = self.binary
         # TODO: This doesn't match the model, check it
         result["invalid_build"] = self.cant_build
         result["info_invalid"] = getattr(getattr(self.conanfile, "info", None), "invalid", None)
         # Adding the conanfile information: settings, options, etc
         result.update(self.conanfile.serialize())
+        result.pop("requires", None)  # superseded by "dependencies" (graph.transitive_deps)
+        result["dependencies"] = {d.node.id: d.require.serialize()
+                                  for d in self.transitive_deps.values() if d.node is not None}
         result["context"] = self.context
         result["test"] = self.test
-        result["requires"] = {n.id: n.ref.repr_notime() for n in self.neighbors()}
         return result
 
     def overrides(self):
 
         def transitive_subgraph():
             result = set()
             opened = {self}
@@ -375,12 +377,14 @@
 
     def report_graph_error(self):
         if self.error:
             raise self.error
 
     def serialize(self):
         for i, n in enumerate(self.nodes):
-            n.id = i
+            n.id = str(i)
         result = OrderedDict()
-        result["nodes"] = [n.serialize() for n in self.nodes]
+        result["nodes"] = {n.id: n.serialize() for n in self.nodes}
         result["root"] = {self.root.id: repr(self.root.ref)}  # TODO: ref of consumer/virtual
+        result["overrides"] = self.overrides().serialize()
+        result["resolved_ranges"] = {repr(r): s.repr_notime() for r, s in self.resolved_ranges.items()}
         return result
```

### Comparing `conan-2.0.5/conans/client/graph/graph_binaries.py` & `conan-2.0.6/conans/client/graph/graph_binaries.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/graph_builder.py` & `conan-2.0.6/conans/client/graph/graph_builder.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/graph_error.py` & `conan-2.0.6/conans/client/graph/graph_error.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/install_graph.py` & `conan-2.0.6/conans/client/graph/install_graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/profile_node_definer.py` & `conan-2.0.6/conans/client/graph/profile_node_definer.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/provides.py` & `conan-2.0.6/conans/client/graph/provides.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/proxy.py` & `conan-2.0.6/conans/client/graph/proxy.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/python_requires.py` & `conan-2.0.6/conans/client/graph/python_requires.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/graph/range_resolver.py` & `conan-2.0.6/conans/client/graph/range_resolver.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/hook_manager.py` & `conan-2.0.6/conans/client/hook_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/installer.py` & `conan-2.0.6/conans/client/installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,16 +328,14 @@
         pkg_folder = package_layout.package()
         assert os.path.isdir(pkg_folder), "Pkg '%s' folder must exist: %s" % (str(pref), pkg_folder)
         for n in package.nodes:
             n.prev = pref.revision  # Make sure the prev is assigned
             conanfile = n.conanfile
             # Call the info method
             conanfile.folders.set_base_package(pkg_folder)
-            conanfile.folders.set_base_source(None)
-            conanfile.folders.set_base_build(None)
             self._call_package_info(conanfile, pkg_folder, is_editable=False)
 
     def _handle_node_editable(self, install_node):
         # It will only run generation
         node = install_node.nodes[0]
         conanfile = node.conanfile
         ref = node.ref
@@ -398,15 +396,16 @@
     def _call_package_info(self, conanfile, package_folder, is_editable):
 
         with chdir(package_folder):
             with conanfile_exception_formatter(conanfile, "package_info"):
                 self._hook_manager.execute("pre_package_info", conanfile=conanfile)
 
                 if hasattr(conanfile, "package_info"):
-                    with conanfile_remove_attr(conanfile, ['info'], "package_info"):
+                    with conanfile_remove_attr(conanfile, ['info', "source_folder", "build_folder"],
+                                               "package_info"):
                         MockInfoProperty.package = str(conanfile)
                         conanfile.package_info()
 
                 # TODO: Check this package_folder usage for editable when not defined
                 conanfile.cpp.package.set_relative_base_folder(package_folder)
 
                 if is_editable:
```

### Comparing `conan-2.0.5/conans/client/loader.py` & `conan-2.0.6/conans/client/loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/loader_txt.py` & `conan-2.0.6/conans/client/loader_txt.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/migrations.py` & `conan-2.0.6/conans/client/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/pkg_sign.py` & `conan-2.0.6/conans/client/pkg_sign.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/profile_loader.py` & `conan-2.0.6/conans/client/profile_loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/remote_manager.py` & `conan-2.0.6/conans/client/remote_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import shutil
 from typing import List
 
 from requests.exceptions import ConnectionError
 
 from conan.api.output import ConanOutput
 from conan.internal.cache.conan_reference_layout import METADATA
+from conan.tools.files.files import _human_size
 from conans.client.cache.remote_registry import Remote
 from conans.client.pkg_sign import PkgSignaturesPlugin
 from conans.errors import ConanConnectionError, ConanException, NotFoundException, \
     PackageNotFoundException
 from conans.model.info import load_binary_info
 from conans.model.package_ref import PkgReference
 from conans.model.recipe_ref import RecipeReference
@@ -71,15 +72,15 @@
             ConanOutput(scope=str(ref)).error(f"Error downloading from remote '{remote.name}'")
             self._cache.remove_recipe_layout(layout)
             raise
         export_folder = layout.export()
         tgz_file = zipped_files.pop(EXPORT_TGZ_NAME, None)
 
         if tgz_file:
-            uncompress_file(tgz_file, export_folder)
+            uncompress_file(tgz_file, export_folder, scope=str(ref))
         mkdir(export_folder)
         for file_name, file_path in zipped_files.items():  # copy CONANFILE
             shutil.move(file_path, os.path.join(export_folder, file_name))
 
         # Make sure that the source dir is deleted
         rmdir(layout.source())
 
@@ -90,15 +91,15 @@
         export_sources_folder = layout.export_sources()
         zipped_files = self._call_remote(remote, "get_recipe_sources", ref, download_folder)
         if not zipped_files:
             mkdir(export_sources_folder)  # create the folder even if no source files
             return
 
         tgz_file = zipped_files[EXPORT_SOURCES_TGZ_NAME]
-        uncompress_file(tgz_file, export_sources_folder)
+        uncompress_file(tgz_file, export_sources_folder, scope=str(ref))
 
     def get_package(self, conanfile, pref, remote):
         conanfile.output.info("Retrieving package %s from remote '%s' " % (pref.package_id,
                                                                            remote.name))
 
         assert pref.revision is not None
 
@@ -119,15 +120,15 @@
             for f in ("conaninfo.txt", "conanmanifest.txt", "conan_package.tgz"):
                 if f not in zipped_files:
                     raise ConanException(f"Corrupted {pref} in '{remote.name}' remote: no {f}")
             self._signer.verify(pref, download_pkg_folder)
 
             tgz_file = zipped_files.pop(PACKAGE_TGZ_NAME, None)
             package_folder = layout.package()
-            uncompress_file(tgz_file, package_folder)
+            uncompress_file(tgz_file, package_folder, scope=str(pref.ref))
             mkdir(package_folder)  # Just in case it doesn't exist, because uncompress did nothing
             for file_name, file_path in zipped_files.items():  # copy CONANINFO and CONANMANIFEST
                 shutil.move(file_path, os.path.join(package_folder, file_name))
 
             scoped_output.success('Package installed %s' % pref.package_id)
             scoped_output.info("Downloaded package revision %s" % pref.revision)
         except NotFoundException:
@@ -212,17 +213,21 @@
         except ConanException as exc:
             exc.remote = remote
             raise
         except Exception as exc:
             raise ConanException(exc, remote=remote)
 
 
-def uncompress_file(src_path, dest_folder):
+def uncompress_file(src_path, dest_folder, scope=None):
     try:
-        ConanOutput().info("Decompressing %s" % os.path.basename(src_path))
+        filesize = os.path.getsize(src_path)
+        big_file = filesize > 1000000  # 10 Mb
+        if big_file:
+            hs = _human_size(filesize)
+            ConanOutput(scope=scope).info(f"Decompressing {hs} {os.path.basename(src_path)}")
         with open(src_path, mode='rb') as file_handler:
             tar_extract(file_handler, dest_folder)
     except Exception as e:
         error_msg = "Error while extracting downloaded file '%s' to %s\n%s\n"\
                     % (src_path, dest_folder, str(e))
         # try to remove the files
         try:
```

### Comparing `conan-2.0.5/conans/client/rest/__init__.py` & `conan-2.0.6/conans/client/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/rest/auth_manager.py` & `conan-2.0.6/conans/client/rest/auth_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/rest/client_routes.py` & `conan-2.0.6/conans/client/rest/client_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/rest/conan_requester.py` & `conan-2.0.6/conans/client/rest/conan_requester.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/rest/file_uploader.py` & `conan-2.0.6/conans/client/rest/file_uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/rest/rest_client.py` & `conan-2.0.6/conans/client/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/rest/rest_client_common.py` & `conan-2.0.6/conans/client/rest/rest_client_common.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/rest/rest_client_v2.py` & `conan-2.0.6/conans/client/rest/rest_client_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,28 +57,28 @@
         files = data["files"]
         if EXPORT_SOURCES_TGZ_NAME not in files:
             return None
         files = [EXPORT_SOURCES_TGZ_NAME, ]
 
         # If we didn't indicated reference, server got the latest, use absolute now, it's safer
         urls = {fn: self.router.recipe_file(ref, fn) for fn in files}
-        self._download_and_save_files(urls, dest_folder, files)
+        self._download_and_save_files(urls, dest_folder, files, scope=str(ref))
         ret = {fn: os.path.join(dest_folder, fn) for fn in files}
         return ret
 
     def get_package(self, pref, dest_folder):
         url = self.router.package_snapshot(pref)
         data = self._get_file_list_json(url)
         files = data["files"]
         # Download only known files, but not metadata (except sign)
         accepted_files = ["conaninfo.txt", "conan_package.tgz", "conanmanifest.txt", "metadata/sign"]
         files = [f for f in files if any(f.startswith(m) for m in accepted_files)]
         # If we didn't indicated reference, server got the latest, use absolute now, it's safer
         urls = {fn: self.router.package_file(pref, fn) for fn in files}
-        self._download_and_save_files(urls, dest_folder, files)
+        self._download_and_save_files(urls, dest_folder, files, scope=str(pref.ref))
         ret = {fn: os.path.join(dest_folder, fn) for fn in files}
         return ret
 
     @staticmethod
     def _is_dir(path, files):
         if path == ".":
             return True
@@ -133,20 +133,20 @@
                 output.error("\nError uploading file: %s, '%s'" % (filename, exc))
                 failed.append(filename)
 
         if failed:
             raise ConanException("Execute upload again to retry upload the failed files: %s"
                                  % ", ".join(failed))
 
-    def _download_and_save_files(self, urls, dest_folder, files, parallel=False):
+    def _download_and_save_files(self, urls, dest_folder, files, parallel=False, scope=None):
         # Take advantage of filenames ordering, so that conan_package.tgz and conan_export.tgz
         # can be < conanfile, conaninfo, and sent always the last, so smaller files go first
         retry = self._config.get("core.download:retry", check_type=int, default=2)
         retry_wait = self._config.get("core.download:retry_wait", check_type=int, default=0)
-        downloader = ConanInternalCacheDownloader(self.requester, self._config)
+        downloader = ConanInternalCacheDownloader(self.requester, self._config, scope=scope)
         threads = []
 
         for filename in sorted(files, reverse=True):
             resource_url = urls[filename]
             abs_path = os.path.join(dest_folder, filename)
             os.makedirs(os.path.dirname(abs_path), exist_ok=True)  # filename in subfolder must exist
             if parallel:
```

### Comparing `conan-2.0.5/conans/client/source.py` & `conan-2.0.6/conans/client/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/store/localdb.py` & `conan-2.0.6/conans/client/store/localdb.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/subsystems.py` & `conan-2.0.6/conans/client/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/client/userio.py` & `conan-2.0.6/conans/client/userio.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/conan_server.py` & `conan-2.0.6/conans/conan_server.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/errors.py` & `conan-2.0.6/conans/errors.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/migrations.py` & `conan-2.0.6/conans/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/build_info.py` & `conan-2.0.6/conans/model/build_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
         missing_internal = list(internal.difference(self.components))
         if missing_internal:
             raise ConanException(f"{conanfile}: Internal components not found: {missing_internal}")
         if not external:
             return
         # Only direct host (not test) dependencies can define required components
         direct_dependencies = [d.ref.name for d in conanfile.requires.values()
-                               if not d.build and not d.is_test and d.visible]
+                               if not d.build and not d.is_test and d.visible and not d.override]
 
         for e in external:
             if e not in direct_dependencies:
                 raise ConanException(
                     f"{conanfile}: required component package '{e}::' not in dependencies")
         # TODO: discuss if there are cases that something is required but not transitive
         for e in direct_dependencies:
```

### Comparing `conan-2.0.5/conans/model/conan_file.py` & `conan-2.0.6/conans/model/conan_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,22 +121,20 @@
 
     def serialize(self):
         result = {}
 
         for a in ("name", "user", "channel", "url", "license",
                   "author", "description", "homepage", "build_policy", "upload_policy",
                   "revision_mode", "provides", "deprecated", "win_bash", "win_bash_run",
-                  "default_options", "options_description",):
+                  "default_options", "options_description"):
             v = getattr(self, a, None)
-            if v is not None:
-                result[a] = v
-        if self.version is not None:
-            result["version"] = str(self.version)
-        if self.topics is not None:
-            result["topics"] = list(self.topics)
+            result[a] = v
+
+        result["version"] = str(self.version) if self.version is not None else None
+        result["topics"] = list(self.topics) if self.topics is not None else None
         result["package_type"] = str(self.package_type)
 
         settings = self.settings
         if settings is not None:
             result["settings"] = settings.serialize() if isinstance(settings, Settings) else list(settings)
 
         result["options"] = self.options.serialize()
```

### Comparing `conan-2.0.5/conans/model/conanfile_interface.py` & `conan-2.0.6/conans/model/conanfile_interface.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/conf.py` & `conan-2.0.6/conans/model/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     "tools.cmake.cmaketoolchain:toolchain_file": "Use other existing file rather than conan_toolchain.cmake one",
     "tools.cmake.cmaketoolchain:user_toolchain": "Inject existing user toolchains at the beginning of conan_toolchain.cmake",
     "tools.cmake.cmaketoolchain:system_name": "Define CMAKE_SYSTEM_NAME in CMakeToolchain",
     "tools.cmake.cmaketoolchain:system_version": "Define CMAKE_SYSTEM_VERSION in CMakeToolchain",
     "tools.cmake.cmaketoolchain:system_processor": "Define CMAKE_SYSTEM_PROCESSOR in CMakeToolchain",
     "tools.cmake.cmaketoolchain:toolset_arch": "Toolset architecture to be used as part of CMAKE_GENERATOR_TOOLSET in CMakeToolchain",
     "tools.cmake.cmake_layout:build_folder_vars": "Settings and Options that will produce a different build folder and different CMake presets names",
+    "tools.cmake:cmake_program": "Path to CMake executable",
     "tools.files.download:retry": "Number of retries in case of failure when downloading",
     "tools.files.download:retry_wait": "Seconds to wait between download attempts",
     "tools.gnu:make_program": "Indicate path to make program",
     "tools.gnu:define_libcxx11_abi": "Force definition of GLIBCXX_USE_CXX11_ABI=1 for libstdc++11",
     "tools.gnu:pkg_config": "Path to pkg-config executable used by PkgConfig build helper",
     "tools.gnu:host_triplet": "Custom host triplet to pass to Autotools scripts",
     "tools.google.bazel:configs": "Define Bazel config file",
@@ -80,15 +81,15 @@
     "tools.microsoft.msbuildtoolchain:compile_options": "Dictionary with MSBuild compiler options",
     "tools.microsoft.bash:subsystem": "The subsystem to be used when conanfile.win_bash==True. Possible values: msys2, msys, cygwin, wsl, sfu",
     "tools.microsoft.bash:path": "The path to the shell to run when conanfile.win_bash==True",
     "tools.microsoft.bash:active": "If Conan is already running inside bash terminal in Windows",
     "tools.intel:installation_path": "Defines the Intel oneAPI installation root path",
     "tools.intel:setvars_args": "Custom arguments to be passed onto the setvars.sh|bat script from Intel oneAPI",
     "tools.system.package_manager:tool": "Default package manager tool: 'apt-get', 'yum', 'dnf', 'brew', 'pacman', 'choco', 'zypper', 'pkg' or 'pkgutil'",
-    "tools.system.package_manager:mode": "Mode for package_manager tools: 'check' or 'install'",
+    "tools.system.package_manager:mode": "Mode for package_manager tools: 'check', 'report', 'report-installed' or 'install'",
     "tools.system.package_manager:sudo": "Use 'sudo' when invoking the package manager tools in Linux (False by default)",
     "tools.system.package_manager:sudo_askpass": "Use the '-A' argument if using sudo in Linux to invoke the system package manager (False by default)",
     "tools.apple:sdk_path": "Path to the SDK to be used",
     "tools.apple:enable_bitcode": "(boolean) Enable/Disable Bitcode Apple Clang flags",
     "tools.apple:enable_arc": "(boolean) Enable/Disable ARC Apple Clang flags",
     "tools.apple:enable_visibility": "(boolean) Enable/Disable Visibility Apple Clang flags",
     "tools.env.virtualenv:powershell": "If it is set to True it will generate powershell launchers if os=Windows",
```

### Comparing `conan-2.0.5/conans/model/dependencies.py` & `conan-2.0.6/conans/model/dependencies.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/graph_lock.py` & `conan-2.0.6/conans/model/graph_lock.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/info.py` & `conan-2.0.6/conans/model/info.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/layout.py` & `conan-2.0.6/conans/model/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/manifest.py` & `conan-2.0.6/conans/model/manifest.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/options.py` & `conan-2.0.6/conans/model/options.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/package_ref.py` & `conan-2.0.6/conans/model/package_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/pkg_type.py` & `conan-2.0.6/conans/model/pkg_type.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/profile.py` & `conan-2.0.6/conans/model/profile.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/recipe_ref.py` & `conan-2.0.6/conans/model/recipe_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/requires.py` & `conan-2.0.6/conans/model/requires.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,21 +351,23 @@
     def deduce_package_id_mode(self, pkg_type, dep_node, non_embed_mode, embed_mode, build_mode,
                                unknown_mode):
         # If defined by the ``require(package_id_mode=xxx)`` trait, that is higher priority
         # The "conf" values are defaults, no hard overrides
         if self.package_id_mode:
             return
 
+        if self.test:
+            return  # test_requires never affect the binary_id
         dep_conanfile = dep_node.conanfile
         dep_pkg_type = dep_conanfile.package_type
         if self.build:
             build_mode = getattr(dep_conanfile, "build_mode", build_mode)
             if build_mode and self.direct:
                 self.package_id_mode = build_mode
-            return  # At the moment no defaults
+            return
 
         if pkg_type is PackageType.HEADER:
             self.package_id_mode = "unrelated_mode"
             return
 
         # If the dependency defines the mode, that has priority over default
         embed_mode = getattr(dep_conanfile, "package_id_embed_mode", embed_mode)
```

### Comparing `conan-2.0.5/conans/model/rest_routes.py` & `conan-2.0.6/conans/model/rest_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/settings.py` & `conan-2.0.6/conans/model/settings.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/version.py` & `conan-2.0.6/conans/model/version.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/model/version_range.py` & `conan-2.0.6/conans/model/version_range.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/paths/__init__.py` & `conan-2.0.6/conans/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/pylint_plugin.py` & `conan-2.0.6/conans/pylint_plugin.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/search/query_parse.py` & `conan-2.0.6/conans/search/query_parse.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/search/search.py` & `conan-2.0.6/conans/search/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/test/conftest.py` & `conan-2.0.6/conans/test/conftest.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/test/utils/artifactory.py` & `conan-2.0.6/conans/test/utils/artifactory.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/test/utils/mocks.py` & `conan-2.0.6/conans/test/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/test/utils/profiles.py` & `conan-2.0.6/conans/test/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/test/utils/scm.py` & `conan-2.0.6/conans/test/utils/scm.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/test/utils/server_launcher.py` & `conan-2.0.6/conans/test/utils/server_launcher.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/test/utils/test_files.py` & `conan-2.0.6/conans/test/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/test/utils/tools.py` & `conan-2.0.6/conans/test/utils/tools.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/util/config_parser.py` & `conan-2.0.6/conans/util/config_parser.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/util/dates.py` & `conan-2.0.6/conans/util/dates.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/util/encrypt.py` & `conan-2.0.6/conans/util/encrypt.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/util/env.py` & `conan-2.0.6/conans/util/env.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/util/files.py` & `conan-2.0.6/conans/util/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/util/locks.py` & `conan-2.0.6/conans/util/locks.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/util/runners.py` & `conan-2.0.6/conans/util/runners.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/util/sha.py` & `conan-2.0.6/conans/util/sha.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/conans/util/windows.py` & `conan-2.0.6/conans/util/windows.py`

 * *Files identical despite different names*

### Comparing `conan-2.0.5/setup.py` & `conan-2.0.6/setup.py`

 * *Files identical despite different names*

