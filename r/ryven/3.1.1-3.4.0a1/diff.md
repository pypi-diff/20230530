# Comparing `tmp/ryven-3.1.1.tar.gz` & `tmp/ryven-3.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryven-3.1.1.tar", last modified: Fri Jan  7 13:18:17 2022, max compression
+gzip compressed data, was "ryven-3.4.0a1.tar", last modified: Mon May 29 23:21:23 2023, max compression
```

## Comparing `ryven-3.1.1.tar` & `ryven-3.4.0a1.tar`

### file list

```diff
@@ -1,232 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.414027 ryven-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1018 2022-01-07 13:18:04.000000 ryven-3.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-01-07 13:18:04.000000 ryven-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-01-07 13:18:04.000000 ryven-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8748 2022-01-07 13:18:17.414027 ryven-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8235 2022-01-07 13:18:04.000000 ryven-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.374027 ryven-3.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.382027 ryven-3.1.1/docs/img/
--rw-r--r--   0 runner    (1001) docker     (121)    46855 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    50881 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/stylus.png
--rw-r--r--   0 runner    (1001) docker     (121)    89262 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/stylus_dark.png
--rw-r--r--   0 runner    (1001) docker     (121)    85860 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/stylus_light.png
--rw-r--r--   0 runner    (1001) docker     (121)    95421 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_1_blender.png
--rw-r--r--   0 runner    (1001) docker     (121)    81063 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_1_ghost.png
--rw-r--r--   0 runner    (1001) docker     (121)  1698942 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_1_merged.png
--rw-r--r--   0 runner    (1001) docker     (121)    98584 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_1_samuel1d.png
--rw-r--r--   0 runner    (1001) docker     (121)    95033 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_1_samuel1l.png
--rw-r--r--   0 runner    (1001) docker     (121)   135784 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_1_samuel2d.png
--rw-r--r--   0 runner    (1001) docker     (121)    93157 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_1_simple.png
--rw-r--r--   0 runner    (1001) docker     (121)   257602 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_1_toy.png
--rw-r--r--   0 runner    (1001) docker     (121)   134657 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_1_tron.png
--rw-r--r--   0 runner    (1001) docker     (121)   109586 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_1_ueli.png
--rw-r--r--   0 runner    (1001) docker     (121)   574949 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/img/themes_with_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.382027 ryven-3.1.1/docs/node tutorials/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/node tutorials/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     4985 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/node tutorials/basic operators.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.374027 ryven-3.1.1/docs/node tutorials/doc_examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.386027 ryven-3.1.1/docs/node tutorials/doc_examples/custom_widgets/
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/node tutorials/doc_examples/custom_widgets/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/node tutorials/doc_examples/custom_widgets/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.386027 ryven-3.1.1/docs/node tutorials/doc_examples/mypackage/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/node tutorials/doc_examples/mypackage/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.386027 ryven-3.1.1/docs/node tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (121)    21267 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/node tutorials/img/plus.png
--rw-r--r--   0 runner    (1001) docker     (121)    28080 2022-01-07 13:18:04.000000 ryven-3.1.1/docs/node tutorials/img/plus2.png
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-01-07 13:18:04.000000 ryven-3.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.386027 ryven-3.1.1/ryven/
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/NENV.py
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/NWENV.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.374027 ryven-3.1.1/ryven/example_nodes/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.386027 ryven-3.1.1/ryven/example_nodes/OpenCV/
--rw-r--r--   0 runner    (1001) docker     (121)    37536 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/OpenCV/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6101 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/OpenCV/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.386027 ryven-3.1.1/ryven/example_nodes/auto_generated/
--rw-r--r--   0 runner    (1001) docker     (121)     4729 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/auto_generated/autogen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.386027 ryven-3.1.1/ryven/example_nodes/linalg/
--rw-r--r--   0 runner    (1001) docker     (121)     5266 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/linalg/matrix_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     9340 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/linalg/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4029 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/linalg/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.386027 ryven-3.1.1/ryven/example_nodes/std/
--rw-r--r--   0 runner    (1001) docker     (121)     6297 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/std/basic_operators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4760 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/std/control_structures.py
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/std/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)    21888 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/std/special_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5820 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/example_nodes/std/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.386027 ryven-3.1.1/ryven/examples_projects/
--rw-r--r--   0 runner    (1001) docker     (121)    29976 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/examples_projects/basics.json
--rw-r--r--   0 runner    (1001) docker     (121)    26900 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/examples_projects/matrices.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.390027 ryven-3.1.1/ryven/gui/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.390027 ryven-3.1.1/ryven/gui/code_editor/
--rw-r--r--   0 runner    (1001) docker     (121)     3994 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/code_editor/CodeEditorWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     9250 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/code_editor/CodePreviewWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     2213 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/code_editor/EditSrcCodeInfoDialog.py
--rw-r--r--   0 runner    (1001) docker     (121)     4659 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/code_editor/SourceCodeUpdater.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/code_editor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.390027 ryven-3.1.1/ryven/gui/code_editor/pygments/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/code_editor/pygments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/code_editor/pygments/dracula.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/code_editor/pygments/light.py
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10700 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/main_console.py
--rw-r--r--   0 runner    (1001) docker     (121)    14735 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     3118 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/script_UI.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.390027 ryven-3.1.1/ryven/gui/startup_dialog/
--rw-r--r--   0 runner    (1001) docker     (121)     5835 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/startup_dialog/SelectPackages_Dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)     6193 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/startup_dialog/StartupDialog.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/startup_dialog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.390027 ryven-3.1.1/ryven/gui/styling/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/styling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3363 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/styling/design_config.json
--rw-r--r--   0 runner    (1001) docker     (121)     2354 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/styling/window_theme.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.390027 ryven-3.1.1/ryven/gui/uic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/uic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6236 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/uic/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/uic/script.ui
--rw-r--r--   0 runner    (1001) docker     (121)    10936 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/uic/ui_main_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     5335 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/uic/ui_script.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/gui/uic/w_ui_script.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.390027 ryven-3.1.1/ryven/main/
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/main/Ryven.py
--rw-r--r--   0 runner    (1001) docker     (121)     2978 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/main/RyvenConsole.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.390027 ryven-3.1.1/ryven/main/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/main/nodes/NodeBase.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/main/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.390027 ryven-3.1.1/ryven/main/nodes/built_in/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/main/nodes/built_in/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7205 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/main/nodes/built_in/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/main/nodes/built_in/widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/main/nodes_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     4297 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.378027 ryven-3.1.1/ryven/resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.390027 ryven-3.1.1/ryven/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.394027 ryven-3.1.1/ryven/resources/fonts/asap/
--rw-r--r--   0 runner    (1001) docker     (121)   102416 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/asap/Asap-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   111664 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/asap/Asap-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   109800 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/asap/Asap-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   102444 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/asap/Asap-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   111808 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/asap/Asap-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   101032 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/asap/Asap-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   102688 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/asap/Asap-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   112712 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/asap/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/asap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.398027 ryven-3.1.1/ryven/resources/fonts/poppins/
--rw-r--r--   0 runner    (1001) docker     (121)     4372 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (121)   138520 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   155420 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   140724 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   159688 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   139684 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   158172 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   147416 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   170376 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   166604 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   145936 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   168408 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   142980 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   164976 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   144776 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   141612 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   161360 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   148440 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   171772 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/poppins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.406027 ryven-3.1.1/ryven/resources/fonts/source_code_pro/
--rw-r--r--   0 runner    (1001) docker     (121)     4528 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (121)   191284 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   155056 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   191568 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   155288 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   193360 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   156884 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   161376 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   193160 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   156984 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   191984 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   156156 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   192740 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   191792 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   155568 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/fonts/source_code_pro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.406027 ryven-3.1.1/ryven/resources/pics/
--rw-r--r--   0 runner    (1001) docker     (121)   391573 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/pics/Ryven_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)   786058 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/pics/Ryven_icon_blurred.png
--rw-r--r--   0 runner    (1001) docker     (121)    46855 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/pics/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.406027 ryven-3.1.1/ryven/resources/stylesheets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.410027 ryven-3.1.1/ryven/resources/stylesheets/icons/
--rw-r--r--   0 runner    (1001) docker     (121)     3682 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/branch-closed.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/branch-end.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4043 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/branch-more.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/branch-open.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4121 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3565 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/close.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3312 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/downarrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3332 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/downarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3750 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/float.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/leftarrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/leftarrow2.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.414027 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/
--rw-r--r--   0 runner    (1001) docker     (121)     7477 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/base.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8852 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/branch-closed.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8307 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/branch-end.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8525 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/branch-more.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9148 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/branch-open.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8691 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8910 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8619 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8056 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/close.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7801 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/downarrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/downarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8239 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/float.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7797 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/leftarrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3344 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/leftarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8522 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8215 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7800 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/rightarrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3347 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/rightarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (121)    10503 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8109 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/slider.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9268 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9323 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8050 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/tab_close.svg
--rw-r--r--   0 runner    (1001) docker     (121)    11390 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (121)    11636 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7797 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/uparrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/uparrow2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8027 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/orig/vline.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/radiobutton_checked.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3717 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3311 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/rightarrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3343 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/rightarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6014 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3620 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/slider.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3354 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/splitter-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/splitter-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3561 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/tab_close.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6903 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7149 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/uparrow.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/uparrow2.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3536 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/icons/vline.svg
--rw-r--r--   0 runner    (1001) docker     (121)    22441 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/resources/stylesheets/style_template.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.414027 ryven-3.1.1/ryven/unused/
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/unused/EditVal_Dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/unused/NodeDetailsWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     2878 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/unused/NodesTreeListWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)   574832 2022-01-07 13:18:04.000000 ryven-3.1.1/ryven/unused/test.stl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 13:18:17.386027 ryven-3.1.1/ryven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8748 2022-01-07 13:18:17.000000 ryven-3.1.1/ryven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8408 2022-01-07 13:18:17.000000 ryven-3.1.1/ryven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-07 13:18:17.000000 ryven-3.1.1/ryven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-01-07 13:18:17.000000 ryven-3.1.1/ryven.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-01-07 13:18:17.000000 ryven-3.1.1/ryven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-07 13:18:17.000000 ryven-3.1.1/ryven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-01-07 13:18:17.414027 ryven-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-01-07 13:18:04.000000 ryven-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.488635 ryven-3.4.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-29 23:21:11.000000 ryven-3.4.0a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 23:21:11.000000 ryven-3.4.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-29 23:21:11.000000 ryven-3.4.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-29 23:21:23.488635 ryven-3.4.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-05-29 23:21:11.000000 ryven-3.4.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.424635 ryven-3.4.0a1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50881 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/stylus.png
+-rw-r--r--   0 runner    (1001) docker     (123)    89262 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/stylus_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85860 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/stylus_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95421 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_blender.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81063 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_ghost.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1698942 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_merged.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98584 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_samuel1d.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95033 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_samuel1l.png
+-rw-r--r--   0 runner    (1001) docker     (123)   135784 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_samuel2d.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93157 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_simple.png
+-rw-r--r--   0 runner    (1001) docker     (123)   257602 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_toy.png
+-rw-r--r--   0 runner    (1001) docker     (123)   134657 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_tron.png
+-rw-r--r--   0 runner    (1001) docker     (123)   109586 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_ueli.png
+-rw-r--r--   0 runner    (1001) docker     (123)   574949 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_with_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/docs/node tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/basic operators.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.424635 ryven-3.4.0a1/docs/node tutorials/doc_examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/docs/node tutorials/doc_examples/custom_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/doc_examples/custom_widgets/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/doc_examples/custom_widgets/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/docs/node tutorials/doc_examples/mypackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/doc_examples/mypackage/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/docs/node tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    21267 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/img/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28080 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/img/plus2.png
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-29 23:21:11.000000 ryven-3.4.0a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/ryven/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.428635 ryven-3.4.0a1/ryven/example_nodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.444635 ryven-3.4.0a1/ryven/example_nodes/OpenCV/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/OpenCV/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    37537 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/OpenCV/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/OpenCV/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.444635 ryven-3.4.0a1/ryven/example_nodes/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/linalg/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/linalg/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/linalg/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.444635 ryven-3.4.0a1/ryven/example_nodes/std/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/basic_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17061 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/special_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.444635 ryven-3.4.0a1/ryven/examples_projects/
+-rw-r--r--   0 runner    (1001) docker     (123)    63369 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/examples_projects/basics.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/examples_projects/basics_OLD.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40944 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/examples_projects/matrices.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/examples_projects/matrices_OLD.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.448635 ryven-3.4.0a1/ryven/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.448635 ryven-3.4.0a1/ryven/gui/code_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/CodeEditorWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/CodePreviewWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/EditSrcCodeInfoDialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/SourceCodeUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/codes_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.448635 ryven-3.4.0a1/ryven/gui/code_editor/pygments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/pygments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/pygments/dracula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/pygments/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/flow_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/main_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.448635 ryven-3.4.0a1/ryven/gui/startup_dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)    27615 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/startup_dialog/StartupDialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/startup_dialog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/std_input_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.448635 ryven-3.4.0a1/ryven/gui/styling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/styling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/styling/design_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/styling/window_theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.452635 ryven-3.4.0a1/ryven/gui/uic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/uic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/uic/flow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/uic/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/uic/ui_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/uic/ui_main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.452635 ryven-3.4.0a1/ryven/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/Ryven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/RyvenConsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.452635 ryven-3.4.0a1/ryven/main/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.452635 ryven-3.4.0a1/ryven/main/packages/built_in/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/built_in/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/built_in/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/built_in/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/gui_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/node_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/nodes_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/node_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.432635 ryven-3.4.0a1/ryven/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.452635 ryven-3.4.0a1/ryven/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.456635 ryven-3.4.0a1/ryven/resources/fonts/asap/
+-rw-r--r--   0 runner    (1001) docker     (123)   102416 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111664 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   109800 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   102444 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111808 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   101032 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   102688 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112712 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.464635 ryven-3.4.0a1/ryven/resources/fonts/poppins/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   138520 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155420 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   140724 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159688 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   139684 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158172 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   147416 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   170376 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   166604 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   145936 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   168408 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   142980 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   164976 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   144776 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   148440 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171772 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.472635 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   191284 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155056 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   191568 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155288 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193360 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156884 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161376 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193160 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156984 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   191984 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156156 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   192740 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   191792 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155568 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.472635 ryven-3.4.0a1/ryven/resources/pics/
+-rw-r--r--   0 runner    (1001) docker     (123)    61897 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/pics/Ryven_icon.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   391573 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/pics/Ryven_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   786058 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/pics/Ryven_icon_blurred.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/pics/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.472635 ryven-3.4.0a1/ryven/resources/stylesheets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.480635 ryven-3.4.0a1/ryven/resources/stylesheets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-end.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-more.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-open.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/downarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/downarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/float.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/leftarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/leftarrow2.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.488635 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/base.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-end.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-more.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-open.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/downarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/downarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/float.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/leftarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/leftarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/rightarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/rightarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/slider.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/tab_close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/uparrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/uparrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/vline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/radiobutton_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/rightarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/rightarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/slider.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/splitter-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/splitter-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/tab_close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/uparrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/uparrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/vline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/style_template.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.488635 ryven-3.4.0a1/ryven/unused/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/unused/EditVal_Dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/unused/NodeDetailsWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/unused/NodesTreeListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)   574832 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/unused/test.stl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.444635 ryven-3.4.0a1/ryven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-29 23:21:23.488635 ryven-3.4.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 23:21:11.000000 ryven-3.4.0a1/setup.py
```

### Comparing `ryven-3.1.1/CONTRIBUTING.md` & `ryven-3.4.0a1/CONTRIBUTING.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 # Contributions In General :rocket:
 
 There are many ways you can contribute to the Ryven project. Particularly effective options include improvement of
 
 - docstrings
 - online documentation
 - example content: nodes and projects
-- tutorials
-
-Also check out the other repositories.
+- modularity improvements
 
 # Creating Good Issues :mega:
 
-- you might want to check the [information on the website](https://ryven.org/guide)
-- be precise and include a minimal procedure to reproduce the problem
-- notice there's a *discussions* section which can be used for all kinds of questions or suggestions
+- you might want to check
+  - the [information on the website](https://ryven.org/)
+  - the [wiki](https://github.com/leon-thomm/Ryven/wiki)
+  - the [ryvencore documentation](https://leon-thomm.github.io/ryvencore/)
+- be precise and **include a minimal procedure to reproduce the problem**
+- notice there's also a [discussions section](https://github.com/leon-thomm/ryven/discussions), but you can also use the issue tracker for questions
 
 Thanks for hanging around and have a nice day!
```

### Comparing `ryven-3.1.1/LICENSE` & `ryven-3.4.0a1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Leon Thomm
+Copyright (c) 2022 Leon Thomm
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ryven-3.1.1/docs/img/logo.png` & `ryven-3.4.0a1/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/stylus.png` & `ryven-3.4.0a1/docs/img/stylus.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/stylus_dark.png` & `ryven-3.4.0a1/docs/img/stylus_dark.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/stylus_light.png` & `ryven-3.4.0a1/docs/img/stylus_light.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_1_blender.png` & `ryven-3.4.0a1/docs/img/themes_1_blender.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_1_ghost.png` & `ryven-3.4.0a1/docs/img/themes_1_ghost.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_1_merged.png` & `ryven-3.4.0a1/docs/img/themes_1_merged.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_1_samuel1d.png` & `ryven-3.4.0a1/docs/img/themes_1_samuel1d.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_1_samuel1l.png` & `ryven-3.4.0a1/docs/img/themes_1_samuel1l.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_1_samuel2d.png` & `ryven-3.4.0a1/docs/img/themes_1_samuel2d.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_1_simple.png` & `ryven-3.4.0a1/docs/img/themes_1_simple.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_1_toy.png` & `ryven-3.4.0a1/docs/img/themes_1_toy.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_1_tron.png` & `ryven-3.4.0a1/docs/img/themes_1_tron.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_1_ueli.png` & `ryven-3.4.0a1/docs/img/themes_1_ueli.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/img/themes_with_logo.png` & `ryven-3.4.0a1/docs/img/themes_with_logo.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/node tutorials/basic operators.md` & `ryven-3.4.0a1/docs/node tutorials/basic operators.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 This tutorial shows how to create nodes for some basic operations/relations, in particular **arithmetic operations**, **logic operations**, and **value comparisons**. The full nodes package is part of the `std` package, see `ryven/example_nodes/std/basic_operators.py`.
 
 As always, we should first define a parent node class for this scope. It can be completely empty, but it's good practice to always include it as this prevents node identification issues which might occur in complex hierarchies in case you add it later.
 
 ```python
-from ryven.NENV import *
+from ryven.node_env import *
 
-class NodeBase(Node):
 
+class NodeBase(Node):
     version = 'v0.1'
-    
+
     # most of our operators are binary, so let's already put this here (we can override that in subclasses for the exceptions)
     init_inputs = [
         NodeInputBP(dtype=dtypes.Data(size='s')),
         NodeInputBP(dtype=dtypes.Data(size='s')),
     ]
     # operators in python can be defined on objects of different classes, so let's just use Data dtype inputs for now. recall that Data inputs will evaluate input expressions (as opposed to just interpreting it as string for example)
-    
+
     init_outputs = [
         NodeOutputBP(),
     ]
-    
+
     style = 'small'
 ```
 
 Let's leave it like this just for now, we can later extend this class. A simple node definition for addition can now look just like this
 
 ```python
 class PlusNode(NodeBase):
```

### Comparing `ryven-3.1.1/docs/node tutorials/doc_examples/custom_widgets/nodes.py` & `ryven-3.4.0a1/docs/node tutorials/doc_examples/custom_widgets/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ryven.NENV import *
-widgets = import_widgets(__file__)  # this loads all exported widgets from widgets.py into the object
+from ryven.node_env import *
+widgets = import_guis(__file__)  # this loads all exported widgets from gui.py into the object
 
 
 class MyNode(Node):
     title = 'my node'
 
     # this one gets automatically created once for each object
     main_widget_class = widgets.MyMainWidget
```

### Comparing `ryven-3.1.1/docs/node tutorials/doc_examples/custom_widgets/widgets.py` & `ryven-3.4.0a1/docs/node tutorials/doc_examples/custom_widgets/widgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ryven.NWENV import *
+from ryven.gui_env import *
 
 from qtpy.QtWidgets import QWidget, QVBoxLayout, QLabel, QPushButton, QLineEdit
 
 
 class MyMainWidget(MWB, QWidget):
     def __init__(self, params):
         MWB.__init__(self, params)
```

### Comparing `ryven-3.1.1/docs/node tutorials/doc_examples/mypackage/nodes.py` & `ryven-3.4.0a1/docs/node tutorials/doc_examples/mypackage/nodes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ryven.NENV import *
+from ryven.node_env import *
 
 
 class NodeBase(Node):
 
     def __init__(self, params):
         super().__init__(params)
```

### Comparing `ryven-3.1.1/docs/node tutorials/img/plus.png` & `ryven-3.4.0a1/docs/node tutorials/img/plus.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/docs/node tutorials/img/plus2.png` & `ryven-3.4.0a1/docs/node tutorials/img/plus2.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/NENV.py` & `ryven-3.4.0a1/ryven/main/packages/node_env.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,130 +1,116 @@
-"""This module automatically imports all requirements for custom nodes.
-It should lie in the same location as Ryven.py so it can get imported directly from the custom sources
-without path modifications which caused issues in the past."""
+"""
+This module automatically imports all requirements for custom nodes.
+"""
 
-import inspect
-import sys
 import os
+from typing import Type
 
+from ryven.main.packages.nodes_package import load_from_file, NodesPackage
 
-# types
-Node = None
-NodeInputBP = None
-NodeOutputBP = None
-dtypes = None
+from ryvencore import Node, NodeInputType, NodeOutputType, Data, serialize, deserialize
 
 
 def init_node_env():
-    global Node
-    global NodeInputBP
-    global NodeOutputBP
-    global dtypes
 
+    # Note 1:
+    #   Because the wrapper classes were removed from ryvencore-qt recently, we don't need to import from
+    #   difference ryvencore sources here anymore depending on the mode, ryvencore stuff comes from ryvencore
+    #   directly now.
+
+    # Note 2:
+    #   I removed the NodeWrp class, which just added the actions dict to the Node base class, because it
+    #   should be moved to ryvencore soon.
+
+    # Note 3:
+    #   I removed dtypes imports, they are currently not supported and are expected to become a new add-on
+    #   some time in the future.
 
-    if os.environ['RYVEN_MODE'] == 'gui':
-
-        from ryvencore_qt import \
-            NodeInputBP as NodeInputBP_, \
-            NodeOutputBP as NodeOutputBP_, \
-            dtypes as dtypes_
-        from ryven.main.nodes.NodeBase import NodeBase as Node_
-
-        Node = Node_
-        NodeInputBP = NodeInputBP_
-        NodeOutputBP = NodeOutputBP_
-        dtypes = dtypes_
-
-    else:
-
-        # import sources directly from backend if not running in gui mode
-        from ryvencore import \
-            Node as _Node, \
-            NodeInputBP as NodeInputBP_, \
-            NodeOutputBP as NodeOutputBP_, \
-            dtypes as dtypes_
-
-        class NodeWrp(_Node):
-            """
-            Wraps the nodes s.t. their usages of ryvencore-qt or Ryven features don't brake them.
-            TODO: move actions to ryvencore
-            """
-
-            def __init__(self, params):
-                self.actions = dict()
-                super().__init__(params)
-
-        Node = NodeWrp
-        NodeInputBP = NodeInputBP_
-        NodeOutputBP = NodeOutputBP_
-        dtypes = dtypes_
-
+    # Note 4:
+    #   I removed the import of NodeBase, because it's messy to override the Node class in the first place.
 
-from ryven.main.utils import load_from_file
+    if os.environ['RYVEN_MODE'] == 'gui':
+        import ryvencore_qt
 
 
-def import_widgets(origin_file: str, rel_file_path='widgets.py'):
+def import_guis(origin_file: str, gui_file_name='gui.py'):
     """
-    Import all exported widgets from 'widgets.py' with respect to the origin_file location.
-    Returns an object with all exported widgets as attributes for direct access.
+    Import all exported GUI classes from gui_file_name with respect to the origin_file location.
+    Returns an object with all exported gui classes as attributes for direct access.
     """
 
     caller_location = os.path.dirname(origin_file)
 
     # alternative solution without __file__ argument; does not work with debugging, so it's not the best idea
     #   caller_location = os.path.dirname(stack()[1].filename)  # getting caller file path from stack frame
 
-    abs_path = os.path.join(caller_location, rel_file_path)
+    abs_path = os.path.join(caller_location, gui_file_name)
 
     if os.environ['RYVEN_MODE'] == 'gui':
 
-        # import the widgets module
+        # import the gui module
         load_from_file(abs_path)
 
-        # in GUI mode, import the widgets container from NWENV containing all the exported widget classes
-        from ryven import NWENV
-        widgets_container = NWENV.WidgetsRegistry.exported_widgets[-1]
+        # in GUI mode, import the gui classes container from gui_env containing all the exported gui classes
+        from ryven import gui_env
+        gui_classes_container = gui_env.GuiClassesRegistry.exported_guis[-1]
 
     else:
         # in non-gui mode, return an object that just returns None for all accessed attributes
-        # so widgets.MyWidget in the nodes file just returns None then
-        class PlaceholderWidgetsContainer:
+        # so guis.MyGUI in the nodes file just returns None then
+        class PlaceholderGuisContainer:
             def __getattr__(self, item):
                 return None
-        widgets_container = PlaceholderWidgetsContainer()
-
-    return widgets_container
+        gui_classes_container = PlaceholderGuisContainer()
 
-# ------------------------------------------------------
+    return gui_classes_container
 
 
-class NodesRegistry:
+class NodesEnvRegistry:
     """
-    Stores the nodes exported via export_nodes on import of a nodes package.
-    After running the imported nodes.py module (which causes export_nodes() to run),
-    Ryven can find the exported nodes in exported_nodes.
+    Statically stores custom `ryvencore.Node` and `ryvencore.Data` subclasses
+    exported via export_nodes on import of a nodes package.
+    After running the imported nodes.py module (which needs to call
+    `export_nodes()` to run), Ryven can then retrieve the exported types from
+    this class.
     """
-    exported_nodes: [[Node]] = []
-    exported_node_sources: [[str]] = []
 
+    # stores, for each nodes package separately, a list of exported node types
+    exported_nodes: [[Type[Node]]] = []
+
+    # stores, for each nodes package separately, a list of exported data types
+    exported_data_types: [[Type[Data]]] = []
+
+    # stores the package that is currently being imported; set by the nodes package
+    # loader ryven.main.packages.nodes_package.import_nodes_package;
+    # needed for extending the identifiers of node types to include the package name
+    current_package: NodesPackage = None
 
-def export_nodes(*args):
+
+def export_nodes(node_types: [Type[Node]], data_types: [Type[Data]] = None):
     """
     Exports/exposes the specified nodes to Ryven for use in flows.
     """
 
-    if not isinstance(args, tuple):
-        if issubclass(args, Node):
-            nodes = tuple(args)
-        else:
-            return
-    else:
-        nodes = list(args)
-
-    NodesRegistry.exported_nodes.append(nodes)
+    if data_types is None:
+        data_types = []
 
-    # get sources
-    node_sources = [inspect.getsource(n) for n in nodes]
-    NodesRegistry.exported_node_sources.append(node_sources)
+    # extend identifiers of node types to include the package name
+    for node_type in node_types:
+        # store the package name as identifier prefix, which will be added
+        # by ryvencore when registering the node type
+        node_type.identifier_prefix = NodesEnvRegistry.current_package.name
+
+        # also add the identifier without the prefix as fallback for older versions
+        node_type.legacy_identifiers = [
+            *node_type.legacy_identifiers,
+            node_type.identifier if node_type.identifier else node_type.__name__
+        ]
 
+    NodesEnvRegistry.exported_nodes.append(node_types)
+    NodesEnvRegistry.exported_data_types.append(data_types)
 
-# ------------------------------------------------------
+    if os.environ['RYVEN_MODE'] == 'gui':
+        # store node sources for code inspection
+        from ryven.gui.code_editor.codes_storage import register_node_type
+        for node_type in node_types:
+            register_node_type(node_type)
```

### Comparing `ryven-3.1.1/ryven/example_nodes/OpenCV/nodes.py` & `ryven-3.4.0a1/ryven/example_nodes/OpenCV/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from ryven.NENV import *
+from ryven.node_env import *
 
-widgets = import_widgets(__file__)
+widgets = import_guis(__file__)
 
 import cv2
 import numpy as np
 
 
 class CVImage:
     """
```

### Comparing `ryven-3.1.1/ryven/example_nodes/OpenCV/widgets.py` & `ryven-3.4.0a1/ryven/example_nodes/OpenCV/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ryven.NWENV import *
+from ryven.gui_env import *
 from qtpy.QtWidgets import QLabel, QPushButton, QFileDialog, QVBoxLayout, QWidget, QTextEdit
 from qtpy.QtGui import QImage, QPixmap, QFont
 from qtpy.QtCore import Signal, QSize, QTimer
 
 import cv2
 import os
```

### Comparing `ryven-3.1.1/ryven/example_nodes/linalg/matrix_widget.py` & `ryven-3.4.0a1/ryven/example_nodes/linalg/gui.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,60 @@
-from ryven.NWENV import *
+from ryven.gui_env import *
 
 from qtpy.QtWidgets import QTextEdit
-# from qtpy.QtCore import ...
-from qtpy.QtGui import QFontMetrics, QFont
+from qtpy.QtGui import QFontMetrics
 
 import numpy as np
 
 
-class MatrixWidget(QTextEdit, MWB):
+class MatrixWidget(NodeMainWidget, QTextEdit):
+
     def __init__(self, params, base_width=50, base_height=50):
-        MWB.__init__(self, params)
+        NodeMainWidget.__init__(self, params)
         QTextEdit.__init__(self)
 
-
-
-        c = self.parent_node_instance.color.name()
-        self.setStyleSheet('''
-QTextEdit{
-    color: '''+c+''';
+        c = self.node.gui.color
+        self.setStyleSheet(f'''
+QTextEdit{{
+    color: {c};
     background: transparent;
-    border: 1px solid '''+c+''';
+    border: none;
     border-radius: 4px;
-}
-        ''')
-        self.setFont(QFont('source code pro', 10))
+    padding: 0px;
+    font-family: Source Code Pro;
+    font-size: 10pt;
+}}
+        ''')  
+        # border: 1px solid '''+c+''';
+        
+        # self.setFont(font)
         self.base_width = base_width
         self.base_height = base_height
         self.setFixedSize(self.base_width, self.base_height)
         self.setReadOnly(True)
         self.hidden_size = None
 
-    #     self.textChanged.connect(M(self.text_changed))
-    #
-    #
-    # def text_changed(self, new_text):
-    #     fm = QFontMetrics(self.font())
-    #     text_width = fm.width(new_text)
-    #     new_width = text_width+15
-    #     self.setFixedWidth(new_width if new_width > self.base_width else self.base_width)
-    #
-    #     self.parent_node_instance.update_shape()
-    #     self.parent_node_instance.rebuild_ui()  # see rebuild_ui() for explanation
+    @property
+    def gui(self):
+        return self.node.gui
 
     def update_matrix(self, m):
         if m is None:
             self.setText('')
             return
 
         longest_exp_length = -1
         lines = []
 
         try:
             matrix = np.around(m, 4)
         except Exception:
             matrix = m
-            # non computable matrix (expression matrix)
 
-            # if matrix.ndim == 1:
-            #     longest_exp_length = self.get_row_lxl(matrix)
-            #     lines.append(self.format_row_to_str(matrix, longest_exp_length))
-            # elif matrix.ndim == 2:
-            #     for row in matrix:
-            #         nlxl = self.get_row_lxl(row)
-            #         if nlxl > longest_exp_length:
-            #             longest_exp_length = nlxl
-            #     for row in matrix:
-            #         lines.append(self.format_row_to_str(row, longest_exp_length))
-            #
-            # self.setText('\n'.join(lines))
-            # return
-            pass
-
-        if matrix.ndim == 0:    # can happen with scalars
+        if matrix.ndim == 0:    # scalars
             lines = [str(m)]
 
         elif matrix.ndim == 1:
             longest_exp_length = self.get_row_lxl(matrix)
             row = matrix
             lines.append(self.format_row_to_str(row, longest_exp_length))
 
@@ -111,49 +90,109 @@
 
     def resize_to_content(self, lines):
         if len(lines) == 0:
             lines.append('')
 
         # resize properly
         fm = QFontMetrics(self.font())
-        text_width = fm.width(lines[0]+'__')
+        text_width = fm.width(lines[0]+('_'*2))
         text_width = text_width+20  # some buffer
-        text_height = fm.height()*(len(lines))+12  # also some vertical buffer
+        text_height = fm.height()*(len(lines))+15  # vertical buffer for padding etc.
         self.setFixedWidth(text_width if text_width > self.base_width else self.base_width)
         self.setFixedHeight(text_height if text_height > self.base_height else self.base_height)
-        self.parent_node_instance.update_shape()
-
-        # if self.hidden_size is None:
-        #     # resize properly
-        #     fm = QFontMetrics(self.font())
-        #     text_width = fm.width(lines[0]+'__')
-        #     text_width = text_width+20  # some buffer
-        #     text_height = fm.height()*(len(lines))+12  # also some vertical buffer
-        #     self.setFixedWidth(text_width if text_width > self.base_width else self.base_width)
-        #     self.setFixedHeight(text_height if text_height > self.base_height else self.base_height)
-        #     self.parent_node_instance.update_shape()
+        self.gui.update_shape()
 
     def hide(self):
         self.hidden_size = self.size()
         self.setFixedSize(0, 0)
-        self.parent_node_instance.update_shape()
+        self.gui.update_shape()
 
     def show(self):
         self.setFixedSize(self.hidden_size)
-        self.parent_node_instance.update_shape()
+        self.gui.update_shape()
         self.hidden_size = None
 
 
     def get_state(self):
-        data = {'text': self.toPlainText(),
-                'shown': self.hidden_size is None
-                }
+        data = {
+            'text': self.toPlainText(),
+            'shown': self.hidden_size is None
+        }
         return data
 
     def set_state(self, data):
         self.setText(data['text'])
         self.resize_to_content(data['text'].splitlines())
         if not data['shown']:
             self.hide()
 
-    def remove_event(self):
-        pass
+
+class EditMatrixWidget(MatrixWidget):
+    def __init__(self, params):
+        super().__init__(params, 100, 80)
+
+        self.setReadOnly(False)
+        self.textChanged.connect(self.text_changed)
+
+    def text_changed(self):
+        self.node.parse_matrix(self.toPlainText())
+        self.resize_to_content(lines=self.toPlainText().splitlines())
+
+    def focusOutEvent(self, e):
+        self.update_matrix(self.node.expression_matrix)
+        QTextEdit.focusOutEvent(self, e)
+
+
+class MatrixNodeBaseGui(NodeGUI):
+    main_widget_class = MatrixWidget
+    main_widget_pos = 'below ports'
+    color = '#3344ff'
+
+    def __init__(self, params):
+        super().__init__(params)
+
+        self.main_widget_hidden = False
+
+    def initialized(self):
+        if 'show preview' not in self.actions:  # this happens when loading a project
+            self.actions['hide preview'] = {'method': self.ac_hide_mw}
+
+    def show_matrix(self, mat):
+        self.main_widget().update_matrix(mat)
+
+    def ac_hide_mw(self):
+        self.main_widget().hide()
+        del self.actions['hide preview']
+        self.actions['show preview'] = {'method': self.ac_show_mw}
+        self.main_widget_hidden = True
+        self.update_shape()
+
+    def ac_show_mw(self):
+        self.main_widget().show()
+        del self.actions['show preview']
+        self.actions['hide preview'] = {'method': self.ac_hide_mw}
+        self.main_widget_hidden = False
+        self.update_shape()
+
+    def get_state(self):
+        return {
+            **super().get_state(),
+            'main_widget_hidden': self.main_widget_hidden
+        }
+
+    def set_state(self, data):
+        super().set_state(data)
+        if data['main_widget_hidden']:
+            self.ac_hide_mw()
+        # shown by default
+
+
+class EditMatrixNodeGui(MatrixNodeBaseGui):
+    main_widget_class = EditMatrixWidget
+    main_widget_pos = 'below ports'
+    color = '#3344ff'
+
+
+export_guis([
+    MatrixNodeBaseGui,
+    EditMatrixNodeGui,
+])
```

### Comparing `ryven-3.1.1/ryven/example_nodes/linalg/nodes.py` & `ryven-3.4.0a1/ryven/example_nodes/linalg/nodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,360 +1,450 @@
-from ryven.NENV import *
-widgets = import_widgets(__file__)
-
-import numpy as np
+from typing import Optional, List
 
+import ryvencore.addons.Variables
 
-class MatrixNodeBase(Node):
-    main_widget_class = widgets.MatrixWidget
-    main_widget_pos = 'below ports'
-    init_inputs = [
-        NodeInputBP()
-    ]
-    init_outputs = [
-        NodeOutputBP()
-    ]
-    color = '#3344ff'
+from ryven.node_env import *
+guis = import_guis(__file__)
 
-    def __init__(self, params):
-        super().__init__(params)
-        self.mat = None
-
-    def show_matrix(self):
-        if self.session.gui and self.main_widget():
-            self.main_widget().update_matrix(self.mat)
-    
-    def update_event(self, inp=-1):
-        self.mat = self.get_mat()
-        self.show_matrix()
-        self.set_output_val(0, self.mat)
+import numpy as np
+from itertools import chain
 
 
-class ShowMatrix(MatrixNodeBase):
-    """Displays a matrix"""
+class MatrixData(Data):
+    # currently, there should not be any implicit
+    # data sharing between nodes, because their
+    # operations are copying the data anyway
 
-    title = 'Show Matrix'
+    # notice that numpy arrays are pickle serializable
 
-    def get_mat(self):
-        return self.input(0)
+    pass
 
-# ------------------------------------------------------------------------------
 
+class MatrixNodeBase(Node):
+    """
+    Base class for nodes handling matrices.
+    It implements basic forward propagation of a mutated matrix,
+    defined by some operation in the get_mat() method, and a GUI
+    for displaying the matrix.
+    """
 
-class Matrix_Node(Node):
-    """Evaluates a matrix"""
-    title = 'Matrix'
-    init_inputs = []
+    version = 'v0.2'
+    init_inputs = [
+        NodeInputType()
+    ]
     init_outputs = [
-        NodeOutputBP()
+        NodeOutputType()
     ]
-    main_widget_class = widgets.MatrixNode_MainWidget
-    main_widget_pos = 'below ports'
-    color = '#3344ff'
+    GUI = guis.MatrixNodeBaseGui
 
     def __init__(self, params):
-        super(Matrix_Node, self).__init__(params)
-
-        self.actions['hide preview'] = {'method': self.action_hide_mw}
-        self.main_widget_hidden = False
-        self.expression_matrix = None
-        self.evaluated_matrix = None
-        self.used_variable_names = []
+        super().__init__(params)
+        self.mat = None
 
-    def place_event(self):
-        self.update()
+    def get_mat(self):
+        """
+        Returns the processed matrix.
+        Pre: self.inputs_ready() is True.
+        """
+        raise NotImplementedError
+
+    def inputs_ready(self):
+        """Returns True if no input is None."""
+        return all(self.input(i) is not None for i in range(len(self.inputs)))
 
     def update_event(self, inp=-1):
-        self.set_output_val(0, self.evaluated_matrix)
-        
-    def parse_matrix(self, s):
-        lines = s.splitlines()
-        # the list(filter(...)) creates an array of strings for every line
-        try:
-            self.expression_matrix = np.array([[exp for exp in list(filter(lambda s: s != '', l.split(' ')))] for l in lines])
-            self.eval_expression_matrix()
-            self.update()
-        except ValueError:
-            # something like 2+ (which could become 2+1j) can't get parsed yet
+        if not self.inputs_ready():
             return
 
-    def eval_expression_matrix(self):
-        if not self.register_vars(self.expression_matrix):
-            return  # return if parsing failed
-
-        self.evaluated_matrix = self.eval_matrix(self.expression_matrix)
-
-        if self.evaluated_matrix is None:
-            return  # matrix could not be evaluated
-        # custom_array = [list(map(number_type, list(filter(lambda s: s != '', l.split(' '))))) for l in lines]
-
-        try:
-            self.evaluated_matrix = np.array(self.evaluated_matrix)
-        except Exception:
-            return
-
-    def eval_matrix(self, lines):
-        v = self.get_var_val
-        evaled_exp_array = []
-        for l in lines:
-            evaled_exp_array.append([])
-            for exp in l:
-                evaled_exp_array[-1].append(eval(exp))
-        float_exp_array = [[float(exp) if type(exp) == int else exp for exp in l] for l in evaled_exp_array]
-        return np.array(float_exp_array)
-
-    def register_vars(self, lines):
-        try:
-            # clear used variables
-            for name in self.used_variable_names:
-                self.unregister_var_receiver(name, self.var_val_updated)
-            self.used_variable_names.clear()
-
-            v = self.register_variable
-            for l in lines:
-                for exp in l:
-                    eval(exp)
-            return True
-        except Exception:
-            return False
+        self.mat = self.get_mat()
 
-    def register_variable(self, name):
-        # connect to variable changes
-        self.register_var_receiver(name, self.var_val_updated)
-        self.used_variable_names.append(name)
+        if self.have_gui():
+            self.gui.show_matrix(self.mat)
 
-    def var_val_updated(self, name, val):
-        self.evaluated_matrix = self.eval_matrix(self.expression_matrix)
-        self.update()
+        self.set_output_val(0, MatrixData(self.mat))
 
-    def action_hide_mw(self):
-        self.main_widget().hide()
-        del self.actions['hide preview']
-        self.actions['show preview'] = {'method': self.action_show_mw}
-        self.main_widget_hidden = True
-        self.update_shape()
-
-    def action_show_mw(self):
-        self.main_widget().show()
-        del self.actions['show preview']
-        self.actions['hide preview'] = {'method': self.action_hide_mw}
-        self.main_widget_hidden = False
-        self.update_shape()
+    def have_gui(self):
+        return hasattr(self, 'gui')
 
-    def get_state(self):
-        expression_matrix_list = self.expression_matrix
-        if expression_matrix_list is not None:  # ndarrays are not json serializaple
-            expression_matrix_list = expression_matrix_list.tolist()
 
-        data = {'main widget hidden': self.main_widget_hidden,
-                'expression matrix': expression_matrix_list}
-        return data
+class ShowMatrix(MatrixNodeBase):
+    """Simply displays a matrix"""
+    title = 'Show Matrix'
 
-    def set_state(self, data, version):
-        if self.session.gui:
-            self.main_widget_hidden = data['main widget hidden']
-            if self.main_widget_hidden:
-                self.action_hide_mw()
-            # shown by default
-        
-        self.expression_matrix = np.array(data['expression matrix'])
-        self.eval_expression_matrix()
+    def get_mat(self):
+        return self.input(0).payload
 
 
 class Conjugate(MatrixNodeBase):
     """Conjugates a matrix"""
     title = 'Conjugate'
 
     def get_mat(self):
-        return np.conjugate(self.input(0))
+        return np.conjugate(self.input(0).payload)
 
 
 class Transpose(MatrixNodeBase):
     """Transposes a matrix"""
     title = 'Transpose'
 
     def get_mat(self):
-        return np.transpose(self.input(0))
+        return np.transpose(self.input(0).payload)
 
 
 class DetOfMatrix(MatrixNodeBase):
     """Computes the determinant of a matrix."""
     title = 'Determinant'
 
     def get_mat(self):
-        return np.linalg.det(self.input(0))
+        return np.linalg.det(self.input(0).payload)
 
 
 class DotProduct(MatrixNodeBase):
     """Computes the dot product of a matrix."""
     title = 'Dot Product'
     init_inputs = [
-        NodeInputBP(),
-        NodeInputBP(),
+        NodeInputType(),
+        NodeInputType(),
     ]
     
     def get_mat(self):
-        return np.dot(self.input(0), self.input(1))
+        return np.dot(
+            self.input(0).payload,
+            self.input(1).payload
+        )
 
 
 class HermMatrix(MatrixNodeBase):
     """Computes the hermetian matrix."""
     title = 'Herm'
 
     def get_mat(self):
-        return np.transpose(np.conjugate(self.input(0)))
+        return np.transpose(np.conjugate(self.input(0).payload))
 
 
 class IDMatrix(MatrixNodeBase):
     """Creates an identity matrix."""
     title = 'ID Matrix'
 
     def get_mat(self):
-        return np.identity(self.input(0))
+        return np.identity(self.input(0).payload)
 
 
 class ImagMatrix(MatrixNodeBase):
     """Extracts the imaginary parts of the matrix."""
     title = 'Imag'
 
     def get_mat(self):
-        return np.imag(self.input(0))
+        return np.imag(self.input(0).payload)
 
 
 class RealMatrix(MatrixNodeBase):
     """Extracts the real parts of the matrix."""
     title = 'Real'
 
     def get_mat(self):
-        return np.real(self.input(0))
+        return np.real(self.input(0).payload)
 
 
 class InnerProduct(MatrixNodeBase):
     """Computes the inner product of the input matrices."""
     title = 'Inner'
     init_inputs = [
-        NodeInputBP(),
-        NodeInputBP(),
+        NodeInputType(),
+        NodeInputType(),
     ]
     
     def get_mat(self):
-        return np.inner(self.input(0), self.input(1))
+        return np.inner(
+            self.input(0).payload,
+            self.input(1).payload
+        )
 
 
 class OuterProduct(MatrixNodeBase):
     """Creates the outer product of two matrices."""
     title = 'Outer'
     init_inputs = [
-        NodeInputBP(),
-        NodeInputBP(),
+        NodeInputType(),
+        NodeInputType(),
     ]
 
     def get_mat(self):
-        return np.outer(self.input(0), self.input(1))
+        return np.outer(
+            self.input(0).payload,
+            self.input(1).payload
+        )
 
 
 class InverseMatrix(MatrixNodeBase):
     """Computes the inverse matrix"""
     title = 'Inverse'
 
     def get_mat(self):
-        return np.linalg.inv(self.input(0))
+        return np.linalg.inv(
+            self.input(0).payload
+        )
 
 
 class KronMatrix(MatrixNodeBase):
     """"""
     title = 'Kron'
 
     def get_mat(self):
-        return np.kron(self.input(0), self.input(1))
+        return np.kron(
+            self.input(0).payload,
+            self.input(1).payload
+        )
 
 
 class MaskLower(MatrixNodeBase):
     """"""
     title = 'Mask Lower'
 
     def get_mat(self):
-        return np.tril(self.input(0))
+        return np.tril(
+            self.input(0).payload
+        )
 
 
 class MaskUpper(MatrixNodeBase):
     """"""
     title = 'Mask Upper'
 
     def get_mat(self):
-        return np.triu(self.input(0))
+        return np.triu(
+            self.input(0).payload
+        )
 
 
 class MatMul(MatrixNodeBase):
     """Performs a matrix multiplication."""
     title = 'Mult'
     init_inputs = [
-        NodeInputBP(),
-        NodeInputBP(),
+        NodeInputType(),
+        NodeInputType(),
     ]
 
     def get_mat(self):
-        return np.matmul(self.input(0), self.input(1))
+        return np.matmul(
+            self.input(0).payload,
+            self.input(1).payload
+        )
 
 
 class MatPower(MatrixNodeBase):
     """Powers a matrix."""
     title = 'Power'
     init_inputs = [
-        NodeInputBP(),
-        NodeInputBP(),
+        NodeInputType(),
+        NodeInputType(),
     ]
 
     def get_mat(self):
-        return np.linalg.matrix_power(self.input(0), self.input(1))
+        return np.linalg.matrix_power(
+            self.input(0).payload,
+            self.input(1).payload
+        )
 
 
 class NullMatrix(MatrixNodeBase):
     """Creates a matrix of zeros."""
     title = 'Null'
 
     def get_mat(self):
-        return np.zeros(shape=(self.input(0), self.input(1)))
+        return np.zeros(shape=(self.input(0).payload, self.input(1).payload))
 
 
 class OnesMatrix(MatrixNodeBase):
     """Creates a matrix of ones."""
     title = 'Ones'
 
     def get_mat(self):
-        return np.ones(shape=(self.input(0), self.input(1)))
+        return np.ones(shape=(self.input(0).payload, self.input(1).payload))
 
 
 class RandomMatrix(MatrixNodeBase):
     """Creates a matrix with random values between 0 and 1."""
     title = 'Rand'
     init_inputs = [
-        NodeInputBP(),
-        NodeInputBP(),
+        NodeInputType(),
+        NodeInputType(),
     ]
 
     def get_mat(self):
-        m = np.random.rand(self.input(0), self.input(1))
-        return m
+        return np.random.rand(
+            self.input(0).payload,
+            self.input(1).payload
+        )
 
 
 class SolveLEq(MatrixNodeBase):
     """Solves a linear equation system."""
     title = 'Solve'
     init_inputs = [
-        NodeInputBP(),
-        NodeInputBP(),
+        NodeInputType(),
+        NodeInputType(),
     ]
 
     def get_mat(self):
-        return np.linalg.solve(self.input(0), self.input(1))
+        return np.linalg.solve(
+            self.input(0).payload,
+            self.input(1).payload
+        )
+
+
+class EditMatrixNode(Node):
+    """
+    A special node for hand-designing matrices with specific
+    numerical values. It also supports Ryven variables and
+    automatically adapts the matrix when they change.
+    """
+    title = 'Matrix'
+    identifier = 'EditMatrix_Node'
+    legacy_identifiers = ['Matrix_Node', 'linalg.Matrix_Node']
+    init_inputs = []
+    init_outputs = [
+        NodeOutputType()
+    ]
+    GUI = guis.EditMatrixNodeGui
+
+    def __init__(self, params):
+        super().__init__(params)
+
+        self.expression_matrix: Optional[np.ndarray] = None
+        self.evaluated_matrix: Optional[MatrixData] = None
+
+        self.used_variable_names = []
+
+    def update_event(self, inp=-1):
+        if self.expression_matrix is not None:
+            self.set_output_val(0, self.evaluated_matrix)
+
+    def parse_matrix(self, s):  # called from gui
+        lines = s.splitlines()
+
+        try:
+            # this throws a ValueError if the matrix is not rectangular
+            exp_mat = np.array([
+                list(filter(lambda s: s != '', l.split(' ')))  # array of expression strings
+                for l in lines
+            ])
+
+            # check if all expressions are valid
+            for exp in self.flatten_2d(exp_mat):
+                if not self.exp_is_var(exp):
+                    eval(exp)
+                elif not self.var_exists(exp):
+                    raise NameError
+        except (ValueError, NameError):
+            # something like 2+ (which could become 2+1j) can't get parsed yet
+            return
+
+        self.expression_matrix = exp_mat
+        self.register_vars_and_eval_matrix()
+        self.update()
+
+    def register_vars_and_eval_matrix(self):
+        if not self.register_vars(self.expression_matrix):
+            return  # abort if vars registration failed
+        self.evaluated_matrix = self.eval_matrix(self.expression_matrix)
+
+    def register_vars(self, lines: np.ndarray) -> bool:
+        """Updates subscriptions for the variables used in the matrix."""
+
+        for _ in range(len(self.used_variable_names)):
+            self.unsub_var(self.used_variable_names[0])
+
+        var_names = set()
+        for exp in filter(self.exp_is_var, self.flatten_2d(lines)):
+            if self.var_exists(exp):
+                var_names.add(exp)
+            else:
+                return False
+
+        for var_name in var_names:
+            self.sub_var(var_name)
+
+        return True
+
+    def eval_matrix(self, lines) -> MatrixData:
+        """
+        Evaluates a matrix from string expressions of numerals and variables.
+        """
+
+        # replace old v('name') syntax with new 'name' syntax
+        lines = [
+            [exp.replace('v(', '').replace(')', '') if 'v(' in exp else exp
+             for exp in l]
+            for l in lines
+        ]
+
+        # evaluate expressions
+        evaled_exp_array = [
+            [
+                eval(exp)
+                if not self.exp_is_var(exp) else
+                self.var_val(exp)
+                for exp in l
+            ]
+            for l in lines
+        ]
+
+        # convert ints to floats; leave complex numbers
+        int_to_float = lambda v: float(v) if isinstance(v, int) else v
+        float_exp_array = [
+            list(map(int_to_float, l))
+            for l in evaled_exp_array
+        ]
+
+        # build matrix and wrap in MatrixData
+        return MatrixData(np.array(float_exp_array))
+
+    def var_exists(self, name):
+        return self.get_addon('Variables').var_exists(self.flow, name)
+
+    def sub_var(self, name) -> bool:
+        if not self.var_exists(name):
+            return False
+
+        self.get_addon('Variables').subscribe(self, name, self.var_val_updated)
+        self.used_variable_names.append(name)
+        return True
+
+    def unsub_var(self, name):
+        self.get_addon('Variables').unsubscribe(self, name, self.var_val_updated)
+        self.used_variable_names.remove(name)
+
+    def var_val_updated(self, var: ryvencore.addons.Variables.Variable):
+        self.evaluated_matrix = self.eval_matrix(self.expression_matrix)
+        self.update()
+
+    def var(self, name) -> ryvencore.addons.Variables.Variable:
+        return self.get_addon('Variables').var(self.flow, name)
+
+    def var_val(self, name):
+        return self.var(name).get()
+
+    def exp_is_var(self, s: str):
+        return s.isidentifier()
+
+    def flatten_2d(self, mat: np.ndarray) -> np.ndarray:
+        return np.array(list(chain(*mat)))
+
+    def get_state(self):
+        data = {'expression matrix': serialize(self.expression_matrix)}
+        return data
+
+    def set_state(self, data, version):
+        self.expression_matrix = deserialize(data['expression matrix'])
+        self.register_vars_and_eval_matrix()
 
 
-export_nodes(
-    Matrix_Node,
+export_nodes([
+    EditMatrixNode,
     ShowMatrix,
     Conjugate,
     Transpose,
     DetOfMatrix,
     DotProduct,
     HermMatrix,
     IDMatrix,
@@ -368,8 +458,10 @@
     MaskUpper,
     MatMul,
     MatPower,
     NullMatrix,
     OnesMatrix,
     RandomMatrix,
     SolveLEq,
+],
+    data_types=[MatrixData]
 )
```

### Comparing `ryven-3.1.1/ryven/example_nodes/std/control_structures.py` & `ryven-3.4.0a1/ryven/example_nodes/std/control_structures.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,72 @@
-from ryven.NENV import *
+from ryven.node_env import *
 
+guis = import_guis(__file__)
 
-class CSNodeBase(Node):
-    version = 'v0.1'
-    style = 'normal'
-    color = '#b33a27'
 
+class CSNodeBase(Node):
+    version = 'v0.2'
+    GUI = guis.CSNodeBaseGui
 
 class If_Node(CSNodeBase):
     title = 'branch'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(type_='exec'),
-        NodeInputBP(dtype=dtypes.Boolean(), label='cond'),
+        NodeInputType(type_='exec'),
+        NodeInputType(label='cond'),
     ]
     init_outputs = [
-        NodeOutputBP('true', type_='exec', ),
-        NodeOutputBP('false', type_='exec'),
+        NodeOutputType('true', type_='exec', ),
+        NodeOutputType('false', type_='exec'),
     ]
 
     def update_event(self, inp=-1):
         if inp == 0:
-            if self.input(1):
+            if self.input(1).payload:
                 self.exec_output(0)
             else:
                 self.exec_output(1)
 
 
 class ForLoop_Node(CSNodeBase):
     """n dimensional for loop!"""
 
     title = 'for'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(type_='exec'),
-        NodeInputBP(dtype=dtypes.Integer(), label='from'),
-        NodeInputBP(dtype=dtypes.Integer(), label='to'),
+        NodeInputType(type_='exec'),
+        NodeInputType(label='from'),
+        NodeInputType(label='to'),
     ]
     init_outputs = [
-        NodeOutputBP('loop', type_='exec'),
-        NodeOutputBP('i', type_='data'),
-        NodeOutputBP('finished', type_='exec'),
+        NodeOutputType('loop', type_='exec'),
+        NodeOutputType('i', type_='data'),
+        NodeOutputType('finished', type_='exec'),
     ]
+    GUI = guis.ForLoopGui
 
     def __init__(self, params):
         super().__init__(params)
 
-        self.actions['add dimension'] = {'method': self.add_dimension}
-
         self.dims = 1
 
     def add_dimension(self):
         new_dim = self.dims + 1
-        self.create_input_dt(dtype=dtypes.Integer(), label=f'{new_dim} from')
-        self.create_input_dt(dtype=dtypes.Integer(), label=f'{new_dim} to')
+        self.create_input(label=f'{new_dim} from')
+        self.create_input(label=f'{new_dim} to')
         self.create_output(f'loop {new_dim}', 'exec', insert=-1)
         self.create_output(f'i {new_dim}', 'data', insert=-1)
         self.dims += 1
 
-        self.actions[f'remove dimension {new_dim}'] = {
-            'method': self.remove_dimension,
-            'data': new_dim
-        }
-
     def remove_dimension(self, dim):
         inp_index = self.input_from_dim(dim)
         self.delete_input(inp_index)
         self.delete_input(inp_index)
         out_index = self.output_from_dim(dim)
         self.delete_output(out_index)
         self.delete_output(out_index)
         self.dims -= 1
-        # del self.actions[f'remove dimension {dim}']
-        self.rebuild_remove_actions()
-
-    def rebuild_remove_actions(self):
-
-        remove_keys = []
-        for k, v in self.actions.items():
-            if k.startswith('remove dimension'):
-                remove_keys.append(k)
-
-        for k in remove_keys:
-            del self.actions[k]
-
-        for i in range(1, self.dims):
-            self.actions[f'remove dimension {i+1}'] = {'method': self.remove_dimension, 'data': i+1}
 
     def input_from_dim(self, dim):
         return 1 + 2*(dim-1)
 
     def output_from_dim(self, dim):
         return 2*(dim-1)
 
@@ -101,79 +78,77 @@
     def iterate(self, dim):
 
         inp_index = self.input_from_dim(dim)
 
         exec_out_index = self.output_from_dim(dim)
         data_out_index = exec_out_index+1
 
-        for i in range(self.input(inp_index),
-                       self.input(inp_index+1)):
+        for i in range(self.input(inp_index).payload,
+                       self.input(inp_index+1).payload):
 
-            self.set_output_val(data_out_index, i)
+            self.set_output_val(data_out_index, Data(i))
             self.exec_output(exec_out_index)
 
             if dim < self.dims:
                 self.iterate(dim+1)
 
 
 class ForEachLoop_Node(CSNodeBase):
     title = 'for each'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(type_='exec'),
-        NodeInputBP(dtype=dtypes.Integer(), label='elements'),
+        NodeInputType(type_='exec'),
+        NodeInputType(label='elements'),
     ]
     init_outputs = [
-        NodeOutputBP('loop', type_='exec'),
-        NodeOutputBP('e', type_='data'),
-        NodeOutputBP('finished', type_='exec'),
+        NodeOutputType('loop', type_='exec'),
+        NodeOutputType('e', type_='data'),
+        NodeOutputType('finished', type_='exec'),
     ]
+    GUI = guis.ForEachLoopGui
 
     def update_event(self, inp=-1):
-        for e in self.input(0):
+        for e in self.input(0).payload:
             self.set_output_val(1, e)
             self.exec_output(0)
 
         self.exec_output(2)
 
 
 class WhileLoop_Node(CSNodeBase):
     title = 'while'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(type_='exec'),
-        NodeInputBP(dtype=dtypes.Boolean(), label='cond'),
+        NodeInputType(type_='exec'),
+        NodeInputType(label='cond'),
     ]
     init_outputs = [
-        NodeOutputBP('loop', type_='exec'),
-        NodeOutputBP('finished', type_='exec'),
+        NodeOutputType('loop', type_='exec'),
+        NodeOutputType('finished', type_='exec'),
     ]
 
     def update_event(self, inp=-1):
-        while self.input(0):
+        while self.input(0).payload:
             self.exec_output(0)
 
         self.exec_output(1)
 
 
 class DoWhileLoop_Node(CSNodeBase):
     title = 'do while'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(type_='exec'),
-        NodeInputBP(dtype=dtypes.Boolean(), label='cond'),
+        NodeInputType(type_='exec'),
+        NodeInputType(label='cond'),
     ]
     init_outputs = [
-        NodeOutputBP('loop', type_='exec'),
-        NodeOutputBP('finished', type_='exec'),
+        NodeOutputType('loop', type_='exec'),
+        NodeOutputType('finished', type_='exec'),
     ]
 
     def update_event(self, inp=-1):
         self.exec_output(0)
-        while self.input(0):
+        while self.input(0).payload:
             self.exec_output(0)
         self.exec_output(1)
 
 
 nodes = [
     If_Node,
     ForLoop_Node,
```

### Comparing `ryven-3.1.1/ryven/example_nodes/std/special_nodes.py` & `ryven-3.4.0a1/ryven/example_nodes/std/special_nodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,459 +1,341 @@
 import code
 from contextlib import redirect_stdout, redirect_stderr
+from packaging.version import Version
 
-from ryven.NENV import *
-widgets = import_widgets(__file__)
+from ryvencore.addons.Logging import LoggingAddon
+from ryven.node_env import *
+
+guis = import_guis(__file__)
 
 
 class NodeBase(Node):
-    version = 'v0.1'
-    color = '#FFCA00'
+    version = 'v0.2'
+    GUI = guis.SpecialNodeGuiBase
+
+    def have_gui(self):
+        return hasattr(self, 'gui')
 
 
 class DualNodeBase(NodeBase):
     """For nodes that can be active and passive"""
 
-    version = 'v0.1'
+    GUI = guis.DualNodeBaseGui
 
     def __init__(self, params, active=True):
         super().__init__(params)
 
         self.active = active
-        if active:
-            self.actions['make passive'] = {'method': self.make_passive}
-        else:
-            self.actions['make active'] = {'method': self.make_active}
 
     def make_passive(self):
-        del self.actions['make passive']
-
         self.delete_input(0)
         self.delete_output(0)
         self.active = False
 
-        self.actions['make active'] = {'method': self.make_active}
-
     def make_active(self):
-        del self.actions['make active']
-
         self.create_input(type_='exec', insert=0)
         self.create_output(type_='exec', insert=0)
         self.active = True
 
-        self.actions['make passive'] = {'method': self.make_passive}
-
     def get_state(self) -> dict:
         return {
             'active': self.active
         }
 
     def set_state(self, data: dict, version):
         self.active = data['active']
 
 
-# -------------------------------------------
-
-
-class Checkpoint_Node(NodeBase):
+class Checkpoint_Node(DualNodeBase):
     """Provides a simple checkpoint to reroute your connections"""
 
     title = 'checkpoint'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(type_='data'),
+        NodeInputType(type_='data'),
     ]
     init_outputs = [
-        NodeOutputBP(type_='data'),
+        NodeOutputType(type_='data'),
     ]
-    style = 'small'
+    GUI = guis.CheckpointNodeGui
 
     def __init__(self, params):
         super().__init__(params)
 
-        self.display_title = ''
-
         self.active = False
 
-        # initial actions
-        self.actions['add output'] = {
-            'method': self.add_output
-        }
-        self.actions['remove output'] = {
-            '0': {'method': self.remove_output, 'data': 0}
-        }
-        self.actions['make active'] = {
-            'method': self.make_active
-        }
-
-    """State transitions"""
+    """
+    state transitions
+    """
 
     def clear_ports(self):
         # remove all outputs
         for i in range(len(self.outputs)):
             self.delete_output(0)
 
         # remove all inputs
         for i in range(len(self.inputs)):
             self.delete_input(0)
 
     def make_active(self):
-        self.active = True
-
-        # rebuild inputs and outputs
+        num_outputs = len(self.outputs)
         self.clear_ports()
-        self.create_input(type_='exec')
-        self.create_output(type_='exec')
+        super().make_active()
+        for i in range(1, num_outputs):
+            self.add_output()
 
-        # update actions
-        del self.actions['make active']
-        self.actions['make passive'] = {
-            'method': self.make_passive
-        }
-        self.actions['remove output'] = {
-            '0': {'method': self.remove_output, 'data': 0}
-        }
 
     def make_passive(self):
-        self.active = False
-
-        # rebuild inputs and outputs
+        num_outputs = len(self.outputs)
+        super().make_passive()
         self.clear_ports()
-        self.create_input(type_='data')
-        self.create_output(type_='data')
-
-        # update actions
-        del self.actions['make passive']
-        self.actions['make active'] = {
-            'method': self.make_active
-        }
-        self.actions['remove output'] = {
-            '0': {'method': self.remove_output, 'data': 0}
-        }
-
-    """Actions"""
+        for i in range(num_outputs):
+            self.add_output()
 
     def add_output(self):
-        index = len(self.outputs)
-
-        if self.active:
-            self.create_output(type_='exec')
-        else:
-            self.create_output(type_='data')
-
-        self.actions['remove output'][str(index)] = {
-            'method': self.remove_output,
-            'data': index,
-        }
+        self.create_output(type_='exec' if self.active else 'data')
 
     def remove_output(self, index):
         self.delete_output(index)
 
-        del self.actions['remove output'][str(len(self.outputs))]
-
-    """Behavior"""
+    """
+    update
+    """
 
     def update_event(self, inp=-1):
         if self.active and inp == 0:
             for i in range(len(self.outputs)):
                 self.exec_output(i)
 
         elif not self.active:
             data = self.input(0)
             for i in range(len(self.outputs)):
                 self.set_output_val(i, data)
 
-    """State Reload"""
-
-    def get_state(self) -> dict:
-        return {
-            'active': self.active,
-            'num outputs': len(self.outputs),
-        }
-
-    def set_state(self, data: dict, version):
-        self.actions['remove output'] = {
-            {'method': self.remove_output, 'data': i}
-            for i in range(data['num outputs'])
-        }
-
-        if data['active']:
-            self.make_active()
-
 
 class Button_Node(NodeBase):
     title = 'Button'
-    version = 'v0.1'
-    main_widget_class = widgets.ButtonNode_MainWidget
-    main_widget_pos = 'between ports'
-    init_inputs = [
-
-    ]
+    init_inputs = []
     init_outputs = [
-        NodeOutputBP(type_='exec')
+        NodeOutputType(type_='exec')
     ]
-    color = '#99dd55'
+    GUI = guis.ButtonNodeGui
 
     def update_event(self, inp=-1):
         self.exec_output(0)
 
 
 class Print_Node(DualNodeBase):
     title = 'Print'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(type_='exec'),
-        NodeInputBP(dtype=dtypes.Data(size='m')),
+        NodeInputType(type_='exec'),
+        NodeInputType(),
     ]
     init_outputs = [
-        NodeOutputBP(type_='exec'),
+        NodeOutputType(type_='exec'),
     ]
-    color = '#5d95de'
 
     def __init__(self, params):
         super().__init__(params, active=True)
 
     def update_event(self, inp=-1):
-        if self.active and inp == 0:
-            print(self.input(1))
-        elif not self.active:
-            print(self.input(0))
+        if inp == 0:
+            print(self.input(1 if self.active else 0).payload)
 
 
 import logging
 
 
 class Log_Node(DualNodeBase):
     title = 'Log'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(type_='exec'),
-        NodeInputBP('msg', type_='data'),
+        NodeInputType(type_='exec'),
+        NodeInputType('msg', type_='data'),
     ]
     init_outputs = [
-        NodeOutputBP(type_='exec'),
+        NodeOutputType(type_='exec'),
     ]
-    main_widget_class = widgets.LogNode_MainWidget
-    main_widget_pos = 'below ports'
-    color = '#5d95de'
+    GUI = guis.LogNodeGui
+
+    logs = {}   # {int: Logger}
+    in_use = set()  # make sure we don't reuse numbers on copy & paste
 
     def __init__(self, params):
         super().__init__(params, active=True)
 
-        self.logger = self.new_logger('Log Node')
+        self.number: int = None
+        self.logger: logging.Logger = None
 
-        self.targets = {
-            **self.script.logs_manager.default_loggers,
-            'own': self.logger,
-        }
-        self.target = 'global'
+    def place_event(self):
+        if self.number is None:
+            # didn't load; initialize
+            self.number = len(self.logs)
+            self.logs[self.number] = \
+                self.logs_ext().new_logger(self, 'Log Node')
+            self.in_use.add(self.number)
+
+    def logs_ext(self) -> LoggingAddon:
+        return self.get_addon('Logging')
 
     def update_event(self, inp=-1):
-        if self.active and inp == 0:
-            i = 1
-        elif not self.active:
-            i = 0
-        else:
-            return
-
-        msg = self.input(i)
-
-        self.targets[self.target].log(logging.INFO, msg=msg)
+        if inp == 0:
+            msg = self.input(1 if self.active and inp == 0 else 0).payload
+            self.logs[self.number].log(logging.INFO, msg=msg)
+            # TODO: support more than INFO, with a dropdown menu in main widget
 
     def get_state(self) -> dict:
         return {
             **super().get_state(),
-            'target': self.target,
+            'number': self.number,
         }
 
     def set_state(self, data: dict, version):
+        if Version(version) < Version('0.2'):
+            # ignore old version
+            return
         super().set_state(data, version)
-        self.target = data['target']
-        if self.session.gui and self.main_widget():
-            self.main_widget().set_target(self.target)
+        n = data['number']
+        if n not in self.in_use:
+            self.number = n
+        else:
+            # number already in use; generate a new one
+            # happens on copy & paste
+            self.number = len(self.logs)
+
+        # the logging addon will have re-created the logger
+        # for us already
+        self.logs[self.number] = \
+            self.logs_ext().new_logger(self, 'Log Node')
 
 
 class Clock_Node(NodeBase):
     title = 'clock'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(dtype=dtypes.Float(default=0.1), label='delay'),
-        NodeInputBP(dtype=dtypes.Integer(default=-1, bounds=(-1, 1000)), label='iterations'),
+        NodeInputType('delay'),
+        NodeInputType('iterations'),
     ]
     init_outputs = [
-        NodeOutputBP(type_='exec')
+        NodeOutputType(type_='exec')
     ]
-    color = '#5d95de'
-    main_widget_class = widgets.ClockNode_MainWidget
-    main_widget_pos = 'below ports'
+    GUI = guis.ClockNodeGui
+
+    # When running with GUI, this node uses QTime which doesn't
+    # block the GUI. When running without GUI, it uses time.sleep()
 
     def __init__(self, params):
         super().__init__(params)
 
-        self.actions['start'] = {'method': self.start}
-        self.actions['stop'] = {'method': self.stop}
+        self.running_with_qt = False
 
-        if self.session.gui:
+    def place_event(self):
+        self.running_with_qt = self.GUI is not None
 
+        if self.running_with_qt:
             from qtpy.QtCore import QTimer
-            self.timer = QTimer(self)
+            self.timer = QTimer()
             self.timer.timeout.connect(self.timeouted)
             self.iteration = 0
 
-
     def timeouted(self):
         self.exec_output(0)
         self.iteration += 1
-        if -1 < self.input(1) <= self.iteration:
+        if -1 < self.input(1).payload <= self.iteration:
             self.stop()
 
     def start(self):
-        if self.session.gui:
-            self.timer.setInterval(self.input(0)*1000)
+        if self.running_with_qt:
+            self.timer.setInterval(self.input(0).payload)
             self.timer.start()
         else:
             import time
-            for i in range(self.input(1)):
+            for i in range(self.input(1).payload):
                 self.exec_output(0)
-                time.sleep(self.input(0))
+                time.sleep(self.input(0).payload/1000)
 
     def stop(self):
+        assert self.running_with_qt
+        self.timer.stop()
         self.iteration = 0
-        if self.session.gui:
-            self.timer.stop()
 
     def toggle(self):
         # triggered from main widget
-        if self.session.gui:
+        if self.running_with_qt:
             if self.timer.isActive():
                 self.stop()
             else:
                 self.start()
+        # toggling is impossible when using time.sleep()
 
     def update_event(self, inp=-1):
-        if self.session.gui:
-            self.timer.setInterval(self.input(0)*1000)
+        if self.running_with_qt:
+            self.timer.setInterval(self.input(0).payload)
 
     def remove_event(self):
-        self.stop()
+        if self.running_with_qt:
+            self.stop()
 
 
 class Slider_Node(NodeBase):
     title = 'slider'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(dtype=dtypes.Integer(default=1), label='scl'),
-        NodeInputBP(dtype=dtypes.Boolean(default=False), label='round'),
+        NodeInputType('scl'),
+        NodeInputType('round'),
     ]
     init_outputs = [
-        NodeOutputBP(),
+        NodeOutputType(),
     ]
-    main_widget_class = widgets.SliderNode_MainWidget
-    main_widget_pos = 'below ports'
+    GUI = guis.SliderNodeGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.val = 0
 
     def place_event(self):
         self.update()
 
-    def view_place_event(self):
-        # when running in gui mode, the value might come from the input widget
-        self.update()
-
     def update_event(self, inp=-1):
-
-        v = self.input(0) * self.val
-        if self.input(1):
+        v = self.input(0).payload * self.val
+        if self.input(1).payload:
             v = round(v)
-
-        self.set_output_val(0, v)
+        self.set_output_val(0, Data(v))
 
     def get_state(self) -> dict:
-        return {
-            'val': self.val,
-        }
+        return {'val': self.val}
 
     def set_state(self, data: dict, version):
         self.val = data['val']
 
 
 class _DynamicPorts_Node(NodeBase):
-    version = 'v0.1'
     init_inputs = []
     init_outputs = []
+    GUI = guis.DynamicPortsGui
 
-    def __init__(self, params):
-        super().__init__(params)
-
-        self.actions['add input'] = {'method': self.add_inp}
-        self.actions['add output'] = {'method': self.add_out}
-
-        self.num_inputs = 0
-        self.num_outputs = 0
-
-    def add_inp(self):
+    def add_input(self):
         self.create_input()
 
-        index = self.num_inputs
-        self.actions[f'remove input {index}'] = {
-            'method': self.remove_inp,
-            'data': index
-        }
-
-        self.num_inputs += 1
-
-    def remove_inp(self, index):
+    def remove_input(self, index):
         self.delete_input(index)
-        self.num_inputs -= 1
-        del self.actions[f'remove input {self.num_inputs}']
 
-    def add_out(self):
+    def add_output(self):
         self.create_output()
 
-        index = self.num_outputs
-        self.actions[f'remove output {index}'] = {
-            'method': self.remove_out,
-            'data': index
-        }
-
-        self.num_outputs += 1
-
-    def remove_out(self, index):
+    def remove_output(self, index):
         self.delete_output(index)
-        self.num_outputs -= 1
-        del self.actions[f'remove output {self.num_outputs}']
-
-    def get_state(self) -> dict:
-        return {
-            'num inputs': self.num_inputs,
-            'num outputs': self.num_outputs,
-        }
-
-    def set_state(self, data: dict):
-        self.num_inputs = data['num inputs']
-        self.num_outputs = data['num outputs']
 
 
 class Exec_Node(_DynamicPorts_Node):
     title = 'exec'
-    version = 'v0.1'
-    main_widget_class = widgets.CodeNode_MainWidget
-    main_widget_pos = 'between ports'
+    GUI = guis.ExecNodeGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.code = None
 
-    def place_event(self):
-        pass
-
     def update_event(self, inp=-1):
         exec(self.code)
 
     def get_state(self) -> dict:
         return {
             **super().get_state(),
             'code': self.code,
@@ -462,102 +344,101 @@
     def set_state(self, data: dict, version):
         super().set_state(data, version)
         self.code = data['code']
 
 
 class Eval_Node(NodeBase):
     title = 'eval'
-    version = 'v0.1'
     init_inputs = [
-        # NodeInputBP(),
+        # NodeInputType(),
     ]
     init_outputs = [
-        NodeOutputBP(),
+        NodeOutputType(),
     ]
-    main_widget_class = widgets.EvalNode_MainWidget
-    main_widget_pos = 'between ports'
+    GUI = guis.EvalNodeGui
 
     def __init__(self, params):
         super().__init__(params)
 
-        self.actions['add input'] = {'method': self.add_param_input}
-
         self.number_param_inputs = 0
         self.expression_code = None
 
     def place_event(self):
         if self.number_param_inputs == 0:
             self.add_param_input()
 
     def add_param_input(self):
         self.create_input()
 
-        index = self.number_param_inputs
-        self.actions[f'remove input {index}'] = {
-            'method': self.remove_param_input,
-            'data': index
-        }
-
         self.number_param_inputs += 1
 
     def remove_param_input(self, index):
         self.delete_input(index)
         self.number_param_inputs -= 1
-        del self.actions[f'remove input {self.number_param_inputs}']
 
     def update_event(self, inp=-1):
-        inp = [self.input(i) for i in range(self.number_param_inputs)]
-        self.set_output_val(0, eval(self.expression_code))
+        inp = [
+            self.input(i).payload if self.input(i) is not None else None
+            for i in range(self.number_param_inputs)
+        ]
+        self.set_output_val(0, Data(eval(self.expression_code)))
 
     def get_state(self) -> dict:
         return {
             'num param inputs': self.number_param_inputs,
             'expression code': self.expression_code,
         }
 
     def set_state(self, data: dict, version):
         self.number_param_inputs = data['num param inputs']
         self.expression_code = data['expression code']
 
 
 class Interpreter_Node(NodeBase):
-    """Provides a python interpreter via a basic console with access to the
-    node's properties."""
+    """
+    Provides a python interpreter via a basic console with access to the
+    node's properties.
+    """
     title = 'interpreter'
-    version = 'v0.1'
     init_inputs = []
     init_outputs = []
-    main_widget_class = widgets.InterpreterConsole
+    GUI = guis.InterpreterConsoleGui
 
-    # DEFAULT COMMANDS
+    """
+    commands
+    """
 
     def clear(self):
         self.hist.clear()
         self._hist_updated()
 
     def reset(self):
         self.interp = code.InteractiveInterpreter(locals=locals())
 
     COMMANDS = {
         'clear': clear,
         'reset': reset,
     }
 
+    """
+    behaviour
+    """
+
     def __init__(self, params):
         super().__init__(params)
 
         self.interp = None
         self.hist: [str] = []
         self.buffer: [str] = []
 
         self.reset()
 
     def _hist_updated(self):
-        if self.session.gui:
-            self.main_widget().interp_updated()
+        if self.have_gui():
+            self.gui.main_widget().interp_updated()
 
     def process_input(self, cmds: str):
         m = self.COMMANDS.get(cmds)
         if m is not None:
             m()
         else:
             for l in cmds.splitlines():
@@ -578,109 +459,90 @@
 
     def write(self, line: str):
         self.hist.append(line)
         self._hist_updated()
 
 
 class Storage_Node(NodeBase):
-    """Sequentially stores all the data provided at the input in an array.
-    A COPY of the storage array is provided at the output"""
+    """
+    Sequentially stores all the data provided at the input in an array.
+    A shallow copy of the storage array is provided at the output
+    """
 
     title = 'store'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(),
+        NodeInputType(),
     ]
     init_outputs = [
-        NodeOutputBP(),
+        NodeOutputType(),
     ]
-    color = '#aadd55'
+    GUI = guis.StorageNodeGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.storage = []
 
-        self.actions['clear'] = {'method': self.clear}
-
     def clear(self):
         self.storage.clear()
-        self.set_output_val(0, [])
+        self.set_output_val(0, Data([]))
 
     def update_event(self, inp=-1):
-        self.storage.append(self.input(0))
-        self.set_output_val(0, self.storage.copy())
+        self.storage.append(self.input(0).payload)
+        self.set_output_val(0, Data(self.storage.copy()))
 
     def get_state(self) -> dict:
         return {
             'data': self.storage,
         }
 
     def set_state(self, data: dict, version):
         self.storage = data['data']
 
 
 import uuid
 
 
 class LinkIN_Node(NodeBase):
-    """You can use link OUT nodes to link them up to this node.
+    """
     Whenever a link IN node receives data (or an execution signal),
-    if there is a linked OUT node, it will receive the data
-    and propagate it further."""
+    if there is a linked LinkOUT node, it will receive the data
+    and propagate it further.
+    Notice that this breaks the data flow, which can have substantial
+    performance implications and is generally not recommended.
+    """
 
     title = 'link IN'
-    version = 'v0.1'
     init_inputs = [
-        NodeInputBP(),
+        NodeInputType(),
     ]
     init_outputs = []  # no outputs
+    GUI = guis.LinkIN_NodeGui
 
     # instances registration
     INSTANCES = {}  # {UUID: node}
 
     def __init__(self, params):
         super().__init__(params)
-        self.display_title = 'link'
 
         # register
         self.ID: uuid.UUID = uuid.uuid4()
         self.INSTANCES[str(self.ID)] = self
 
-        self.actions['add input'] = {
-            'method': self.add_inp
-        }
-        self.actions['remove inp'] = {}
-        self.actions['copy ID'] = {
-            'method': self.copy_ID
-        }
-
         self.linked_node: LinkOUT_Node = None
 
-    def copy_ID(self):
-        from qtpy.QtWidgets import QApplication
-        QApplication.clipboard().setText(str(self.ID))
-
-    def add_inp(self):
-        index = len(self.inputs)
-
+    def add_input(self):
         self.create_input()
-
-        self.actions['remove inp'][str(index)] = {
-            'method': self.rem_inp,
-            'data': index,
-        }
         if self.linked_node is not None:
-            self.linked_node.add_out()
+            self.linked_node.add_output()
 
-    def rem_inp(self, index):
+    def remove_input(self, index):
         self.delete_input(index)
-        del self.actions['remove inp'][str(len(self.inputs))]
         if self.linked_node is not None:
-            self.linked_node.rem_out(index)
+            self.linked_node.remove_output(index)
 
     def update_event(self, inp=-1):
         if self.linked_node is not None:
             self.linked_node.set_output_val(inp, self.input(inp))
 
     def get_state(self) -> dict:
         return {
@@ -709,17 +571,17 @@
             self.linked_node = None
 
 
 class LinkOUT_Node(NodeBase):
     """The complement to the link IN node"""
 
     title = 'link OUT'
-    version = 'v0.1'
     init_inputs = []  # no inputs
     init_outputs = []  # will be synchronized with linked IN node
+    GUI = guis.LinkOUT_NodeGui
 
     INSTANCES = []
     PENDING_LINK_BUILDS = {}
     # because a link OUT node might get initialized BEFORE it's corresponding
     # link IN, it then stores itself together with the ID of the link IN it's
     # waiting for in PENDING_LINK_BUILDS
 
@@ -727,51 +589,18 @@
     def new_link_in_loaded(cls, n: LinkIN_Node):
         for out_node, in_ID in cls.PENDING_LINK_BUILDS.items():
             if in_ID == str(n.ID):
                 out_node.link_to(n)
 
     def __init__(self, params):
         super().__init__(params)
-        self.display_title = 'link'
 
         self.INSTANCES.append(self)
         self.linked_node: LinkIN_Node = None
 
-        self.actions['link to ID'] = {
-            'method': self.choose_link_ID
-        }
-
-    def choose_link_ID(self):
-        """opens a small input dialog for providing a copied link IN ID"""
-
-        from qtpy.QtWidgets import QDialog, QMessageBox, QVBoxLayout, QLineEdit
-
-        class IDInpDialog(QDialog):
-            def __init__(self):
-                super().__init__()
-                self.id_str = None
-                self.setLayout(QVBoxLayout())
-                self.line_edit = QLineEdit()
-                self.layout().addWidget(self.line_edit)
-                self.line_edit.returnPressed.connect(self.return_pressed)
-
-            def return_pressed(self):
-                self.id_str = self.line_edit.text()
-                self.accept()
-
-        d = IDInpDialog()
-        d.exec_()
-
-        if d.id_str is not None:
-            n = LinkIN_Node.INSTANCES.get(d.id_str)
-            if n is None:
-                QMessageBox.warning(title='link failed', text='couldn\'t find a valid link in node')
-            else:
-                self.link_to(n)
-
     def link_to(self, n: LinkIN_Node):
         self.linked_node = n
         n.linked_node = self
 
         o = len(self.outputs)
         i = len(self.linked_node.inputs)
 
@@ -781,19 +610,19 @@
 
         # add outputs if there are too few
         for j in range(o, i):
             self.create_output()
 
         self.update()
 
-    def add_out(self):
+    def add_output(self):
         # triggered by linked_node
         self.create_output()
 
-    def rem_out(self, index):
+    def remove_output(self, index):
         # triggered by linked_node
         self.delete_output(index)
 
     def update_event(self, inp=-1):
         if self.linked_node is None:
             return
 
@@ -823,17 +652,14 @@
     def remove_event(self):
         # break existent link
         if self.linked_node:
             self.linked_node.linked_node = None
             self.linked_node = None
 
 
-# -------------------------------------------
-
-
 nodes = [
     Checkpoint_Node,
     Button_Node,
     Print_Node,
     Log_Node,
     Clock_Node,
     Slider_Node,
```

### Comparing `ryven-3.1.1/ryven/examples_projects/basics.json` & `ryven-3.4.0a1/ryven/examples_projects/basics_OLD.json`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/examples_projects/matrices.json` & `ryven-3.4.0a1/ryven/examples_projects/matrices_OLD.json`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/gui/code_editor/CodeEditorWidget.py` & `ryven-3.4.0a1/ryven/gui/code_editor/CodeEditorWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,19 @@
         self.lexer = get_lexer_by_name('python')
 
         if theme.name == 'dark':
             self.formatter = get_formatter_by_name('html', noclasses=True, style=DraculaStyle)
         else:
             self.formatter = get_formatter_by_name('html', noclasses=True, style=LightStyle)
 
+        if self.editing:
+            self.enable_editing()
+        else:
+            self.disable_editing()
+
     def enable_editing(self):
         self.editing = True
         self.setReadOnly(False)
         self.update_appearance()
 
     def disable_editing(self):
         self.editing = False
```

### Comparing `ryven-3.1.1/ryven/gui/code_editor/CodePreviewWidget.py` & `ryven-3.4.0a1/ryven/gui/code_editor/CodePreviewWidget.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,269 +1,247 @@
+from dataclasses import dataclass
+from typing import Type, Optional
+
 from qtpy.QtCore import Qt
 from qtpy.QtWidgets import QWidget, QHBoxLayout, QVBoxLayout, QRadioButton, QLabel, QCheckBox, QGridLayout, \
     QPushButton
+from ryvencore import Node
 
 from ryven.gui.code_editor.EditSrcCodeInfoDialog import EditSrcCodeInfoDialog
 from ryven.gui.code_editor.CodeEditorWidget import CodeEditorWidget
 from ryven.gui.code_editor.SourceCodeUpdater import SrcCodeUpdater
+from ryven.gui.code_editor.codes_storage import class_codes, mod_codes, modif_codes, NodeTypeCodes, \
+    Inspectable, NodeInspectable, MainWidgetInspectable, CustomInputWidgetInspectable
 
 
 class LinkedRadioButton(QRadioButton):
-    """Represents a button linked to one particular"""
+    """Represents a button linked to one particular inspectable object."""
 
-    def __init__(self, name, node, obj):
+    def __init__(self, name, obj: Inspectable):
         super().__init__(name)
-
-        self.node = node
-        self.obj = obj
+        self.representing: Inspectable = obj
 
 
 class CodePreviewWidget(QWidget):
-    def __init__(self, main_window, flow):
-        super(CodePreviewWidget, self).__init__()
+    def __init__(self, main_window, flow_view):
+        super().__init__()
 
-        self.codes = {
-            # structure:
-            #
-            #   <node>: {
-            #       <object>: {                 (the node instance or some widget instance)
-            #           'title': str,           (for faster widget building)
-            #           'original': str,        (original code comes from Node.__class_codes__)
-            #           'edited': str(None),    (initially None)
-            #       }
-            #   }
-        }
-        self.node = None            # currently displayed node
-        self.current_obj = None     # reference to the currently shown/edited object
-        self.radio_buttons = []     # the radio buttons to select a source
-
-        flow.nodes_selection_changed.connect(self.set_selected_nodes)
+        self.edits_enabled = main_window.config.src_code_edits_enabled
+        self.current_insp: Optional[Inspectable] = None
 
+        # widgets
+        self.radio_buttons = []
         self.text_edit = CodeEditorWidget(main_window.theme)
-        self.setup_ui()
 
-        self.set_node(None)
+        self.setup_ui()
+        self._set_node(None)
+        flow_view.nodes_selection_changed.connect(self.set_selected_nodes)
 
     def setup_ui(self):
 
         secondary_layout = QHBoxLayout()
 
         # class radio buttons widget
         self.class_selection_layout = QHBoxLayout()  # QGridLayout()
 
         secondary_layout.addLayout(self.class_selection_layout)
         self.class_selection_layout.setAlignment(Qt.AlignLeft)
         # secondary_layout.setAlignment(self.class_selection_layout, Qt.AlignLeft)
 
         # edit source code buttons
-        self.edit_code_button = QPushButton('edit')
-        self.edit_code_button.setProperty('class', 'small_button')
-        self.edit_code_button.setMaximumWidth(100)
-        self.edit_code_button.clicked.connect(self.edit_code_button_clicked)
-        self.override_code_button = QPushButton('override')
-        self.override_code_button.setProperty('class', 'small_button')
-        self.override_code_button.setMaximumWidth(100)
-        self.override_code_button.setEnabled(False)
-        self.override_code_button.clicked.connect(self.override_code_button_clicked)
-        self.reset_code_button = QPushButton('reset')
-        self.reset_code_button.setProperty('class', 'small_button')
-        self.reset_code_button.setMaximumWidth(206)
-        self.reset_code_button.setEnabled(False)
-        self.reset_code_button.clicked.connect(self.reset_code_button_clicked)
-
-        edit_buttons_layout = QHBoxLayout()
-        # edit_buttons_layout.addWidget(self.highlight_code_button)
-        edit_buttons_layout.addWidget(self.edit_code_button)
-        edit_buttons_layout.addWidget(self.override_code_button)
-        edit_buttons_layout.addWidget(self.reset_code_button)
-        # edit_buttons_layout.addWidget(self.highlight_code_button)
+        if self.edits_enabled:
+            self.edit_code_button = QPushButton('edit')
+            self.edit_code_button.setProperty('class', 'small_button')
+            self.edit_code_button.setMaximumWidth(100)
+            self.edit_code_button.clicked.connect(self._edit_code_button_clicked)
+            self.override_code_button = QPushButton('override')
+            self.override_code_button.setProperty('class', 'small_button')
+            self.override_code_button.setMaximumWidth(100)
+            self.override_code_button.setEnabled(False)
+            self.override_code_button.clicked.connect(self._override_code_button_clicked)
+            self.reset_code_button = QPushButton('reset')
+            self.reset_code_button.setProperty('class', 'small_button')
+            self.reset_code_button.setMaximumWidth(206)
+            self.reset_code_button.setEnabled(False)
+            self.reset_code_button.clicked.connect(self._reset_code_button_clicked)
 
-        secondary_layout.addLayout(edit_buttons_layout)
-        edit_buttons_layout.setAlignment(Qt.AlignRight)
+            edit_buttons_layout = QHBoxLayout()
+            # edit_buttons_layout.addWidget(self.highlight_code_button)
+            edit_buttons_layout.addWidget(self.edit_code_button)
+            edit_buttons_layout.addWidget(self.override_code_button)
+            edit_buttons_layout.addWidget(self.reset_code_button)
+            # edit_buttons_layout.addWidget(self.highlight_code_button)
+
+            secondary_layout.addLayout(edit_buttons_layout)
+            edit_buttons_layout.setAlignment(Qt.AlignRight)
 
         main_layout = QVBoxLayout()
         main_layout.addLayout(secondary_layout)
         main_layout.addWidget(self.text_edit)
         self.setLayout(main_layout)
 
     def set_selected_nodes(self, nodes):
         if len(nodes) == 0:
-            self.set_node(None)
+            self._set_node(None)
         else:
-            self.set_node(nodes[-1])
-
-    def set_node(self, node):
+            self._set_node(nodes[-1])
 
+    def _set_node(self, node: Optional[Node]):
         self.node = node
 
-        if node is None or node.__class_codes__ is None:  # no node selected / only imported nodes have __class_codes__
+        if node is None:
             # clear view
+            if self.edits_enabled:
+                self.edit_code_button.setEnabled(False)
+                self.override_code_button.setEnabled(False)
+                self.reset_code_button.setEnabled(False)
             self.text_edit.set_code('')
-            self.edit_code_button.setEnabled(False)
-            self.override_code_button.setEnabled(False)
-            self.reset_code_button.setEnabled(False)
-            self.clear_class_layout()
+            self._clear_class_layout()
             return
 
+        self._rebuild_class_selection(node)
 
-        if node not in self.codes:  # node not yet registered
+        code = class_codes[node.__class__].node_cls
 
-            # save class sources for all objects (node, main_widget, custom input widgets)
+        if self.edits_enabled and node in modif_codes:
+            code = modif_codes[node]
 
-            # saving it in this structure enables easy view updates and src code overrides
+        self._update_code(NodeInspectable(node, code))
 
-            node_objects = {
-                node: {
-                    'title': 'node',
-                    'original cls': node.__class_codes__['node cls'],
-                    'original mod': node.__class_codes__['node mod'],
-                    'modified cls': None,
-                },
-            }
-
-            if node.main_widget():
-                node_objects[node.main_widget()] = {
-                    'title': 'main widget',
-                    'original cls': node.__class_codes__['main widget cls'],
-                    'original mod': node.__class_codes__['main widget mod'],
-                    'modified cls': None
-                }
-
-            for i in range(len(node.inputs)):
-                iw = node.item.inputs[i].widget
-                if iw:
-                    # find code
-                    code = ''
-                    for name, cls in node.input_widget_classes.items():
-                        if cls == iw.__class__:
-                            code = node.__class_codes__['custom input widgets'][name]['cls']
-                            break
-
-                    else:  # no break -> no custom widget (builtin widget) -> ignore
-                        continue
-
-                    node_objects[iw] = {
-                        'title': f'inp {i}',
-                        'original cls': code,
-                        'modified cls': None,
-                    }
-
-            self.codes[node] = node_objects
-
-        self.rebuild_class_selection(node)
-        self.update_edit_statuses()
-
-        self.edit_code_button.setEnabled(True)
-
-        self.update_code(node, node)
-
-    def update_code(self, node, obj):
-        """
-        Updates the 'modified' field in the nodes dict
-        """
 
-        self.disable_editing()
-        self.text_edit.disable_highlighting()
-
-        self.current_obj = obj
+    def _update_code(self, insp: Inspectable):
+        if self.edits_enabled:
+            self._disable_editing()
+            self._update_radio_buttons_edit_status()
+            self.edit_code_button.setEnabled(True)
+            self.reset_code_button.setEnabled(insp.obj in modif_codes)
 
-        orig = self.codes[node][obj]['original cls']
-        modf = self.codes[node][obj]['modified cls']
-
-        if modf:
-            code = modf
-            self.reset_code_button.setEnabled(True)
-        else:
-            code = orig
-            self.reset_code_button.setEnabled(False)
-
-        self.text_edit.set_code(code)
+        self.text_edit.disable_highlighting()
 
-    def rebuild_class_selection(self, node):
+        self.current_insp = insp
+        self.text_edit.set_code(insp.code)
 
-        self.clear_class_layout()
 
+    def _rebuild_class_selection(self, node: Node):
+        self._clear_class_layout()
         self.radio_buttons.clear()
 
-        for obj, d in self.codes[node].items():
-            rb = LinkedRadioButton(d['title'], node, obj)
-            rb.toggled.connect(self.class_RB_toggled)
-            self.class_selection_layout.addWidget(rb)
-            self.radio_buttons.append(rb)
+        codes: NodeTypeCodes = class_codes[node.__class__]
 
-        self.radio_buttons[0].setChecked(True)
+        def register_rb(rb: QRadioButton):
+           rb.toggled.connect(self._class_rb_toggled)
+           self.class_selection_layout.addWidget(rb)
+           self.radio_buttons.append(rb)
+
+        # node radio button
+        code = codes.node_cls
+        code = modif_codes.get(node, code)
+        register_rb(LinkedRadioButton('node', NodeInspectable(node, code)))
+
+        # main widget radio button
+        if codes.main_widget_cls is not None:
+            mw = node.gui.main_widget()
+            code = codes.main_widget_cls
+            code = modif_codes.get(mw, code)
+            register_rb(LinkedRadioButton(
+                'main widget',
+                MainWidgetInspectable(node, node.gui.main_widget(), code)
+            ))
+
+        # custom input widgets
+        for i in range(len(node.inputs)):
+            inp = node.inputs[i]
+            if inp in node.gui.input_widgets:
+                name = node.gui.input_widgets[inp]['name']
+                widget = node.gui.item.inputs[i].widget
+                code = codes.custom_input_widget_clss[name]
+                code = modif_codes.get(widget, code)
+                register_rb(LinkedRadioButton(
+                    f'input {i}', CustomInputWidgetInspectable(node, widget, code)
+                ))
 
-    def clear_class_layout(self):
+        self.radio_buttons[0].setChecked(True)
 
+    def _clear_class_layout(self):
         # clear layout
         for i in range(self.class_selection_layout.count()):
             item = self.class_selection_layout.itemAt(0)
             widget = item.widget()
             widget.hide()
             self.class_selection_layout.removeItem(item)
 
-    def update_edit_statuses(self):
-        """
-        Draws radio buttons referring to modified objects bold
-        """
+    def _update_radio_buttons_edit_status(self):
+        """Draws radio buttons referring to modified objects bold."""
 
-        for b in self.radio_buttons:
-            if self.codes[b.node][b.obj]['modified cls']:
+        for br in self.radio_buttons:
+            if modif_codes.get(br.representing.obj) is not None:
                 # o.setStyleSheet('color: #3B9CD9;')
-                f = b.font()
+                f = br.font()
                 f.setBold(True)
-                b.setFont(f)
+                br.setFont(f)
             else:
                 # o.setStyleSheet('color: white;')
-                f = b.font()
+                f = br.font()
                 f.setBold(False)
-                b.setFont(f)
+                br.setFont(f)
 
-    def class_RB_toggled(self, checked):
+    def _class_rb_toggled(self, checked):
         if checked:
-            self.update_code(self.sender().node, self.sender().obj)
+            rb: LinkedRadioButton = self.sender()
+            self._update_code(rb.representing)
 
-    def edit_code_button_clicked(self):
+    def _edit_code_button_clicked(self):
         if not EditSrcCodeInfoDialog.dont_show_again:
             info_dialog = EditSrcCodeInfoDialog(self)
             accepted = info_dialog.exec_()
             if not accepted:
                 return
-        self.enable_editing()
+        self._enable_editing()
 
-    def enable_editing(self):
+    def _enable_editing(self):
         self.text_edit.enable_editing()
         self.override_code_button.setEnabled(True)
 
-    def disable_editing(self):
+    def _disable_editing(self):
         self.text_edit.disable_editing()
         self.override_code_button.setEnabled(False)
 
-    def override_code_button_clicked(self):
-
+    def _override_code_button_clicked(self):
         new_code = self.text_edit.get_code()
-
-        SrcCodeUpdater.override_code(
-            obj=self.current_obj,
+        err = SrcCodeUpdater.override_code(
+            obj=self.current_insp.obj,
             new_class_src=new_code,
         )
+        if err is None:
+            self.current_insp.code = new_code
+            modif_codes[self.current_insp.obj] = new_code
+            self._disable_editing()
+            self.reset_code_button.setEnabled(True)
+            self._update_radio_buttons_edit_status()
+        else:
+            # TODO: show error message
+            ...
 
-        self.codes[self.node][self.current_obj]['modified cls'] = new_code
-
-        self.disable_editing()
-
-        self.reset_code_button.setEnabled(True)
-        self.update_edit_statuses()
-
-    def reset_code_button_clicked(self):
-
-        code = self.codes[self.node][self.current_obj]['original cls']
+    def _reset_code_button_clicked(self):
 
-        SrcCodeUpdater.override_code(
-            obj=self.current_obj,
-            new_class_src=code
+        insp = self.current_insp
+        o = insp.obj
+        orig_code = ''
+        if isinstance(insp, NodeInspectable):
+            orig_code = class_codes[o.__class__].node_cls
+        elif isinstance(insp, MainWidgetInspectable):
+            orig_code = class_codes[o.__class__].main_widget_cls
+        elif isinstance(insp, CustomInputWidgetInspectable):
+            orig_code = class_codes[o.__class__].custom_input_widget_clss[o.__class__]
+
+        err = SrcCodeUpdater.override_code(
+            obj=self.current_insp.obj,
+            new_class_src=orig_code
         )
 
-        self.codes[self.node][self.current_obj]['modified cls'] = None
-
-        self.update_code(self.node, self.current_obj)
-        self.update_edit_statuses()
+        if err is None:
+            self.current_insp.code = orig_code
+            del modif_codes[self.current_insp.obj]
+            self._update_code(self.current_insp)
+        else:
+            # TODO: show error message
+            ...
```

### Comparing `ryven-3.1.1/ryven/gui/code_editor/EditSrcCodeInfoDialog.py` & `ryven-3.4.0a1/ryven/gui/code_editor/EditSrcCodeInfoDialog.py`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/gui/code_editor/SourceCodeUpdater.py` & `ryven-3.4.0a1/ryven/gui/code_editor/SourceCodeUpdater.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,67 @@
 import types
-import traceback
+from typing import Union
 
 
 def get_method_funcs(cls_def_str: str, obj):
     """
-    Returns a dict with functions under their names parsed from the methods in the class definition string using ast.
+    Parses the class definition string and returns a dict with python functions under their names,
+    parsed from the methods in the class definition string using the ast module.
     """
 
-    # requires Python >= 3.9
+    import sys
+    if sys.version_info < (3, 9):
+        raise Exception('src code modifications are only supported on Python >=3.9')
+
+    # requires Python >= 3.9 for ast.unparse()
     import ast
 
-    # extracting the functions
-    ast_funcs: [ast.FunctionDef] = [f for f in ast.parse(cls_def_str).body[0].body if type(f) == ast.FunctionDef]
+    # extract functions
+    ast_funcs: [ast.FunctionDef] = [
+        f
+        for f in ast.parse(cls_def_str).body[0].body
+        if type(f) == ast.FunctionDef
+    ]
 
     funcs = {}
     for astf in ast_funcs:
         d = __builtins__.copy()  # important: provide builtins when parsing the function
-
-        try:
-            exec(ast.unparse(astf), d)  # parse
-        except AttributeError as e:     # ast.unparse() was introduced in Python 3.9
-            print(traceback.format_exc())
-            print('\n\nNOTICE: src code override only works on Python version 3.9+, '
-                  'so you may have to update to 3.9 to use it')
-            return None
-
+        exec(ast.unparse(astf), d)
         f = d[astf.name]
-
         # # add locals scope of the object to the function
         # f.__dict__ = obj.
 
-        # add new function to the list, identified by its name
-        funcs = {
-            **funcs,
-            astf.name: f  # d[astf.name]
-        }
+        funcs[astf.name] = f
 
     return funcs
 
 
 class SrcCodeUpdater:
     """
-    Provides functionality to override method implementations of an object
+    Provides functionality to override method implementations of an inspectable object.
     """
 
     @staticmethod
-    def override_code(obj: object, new_class_src):
-
-        funcs = get_method_funcs(new_class_src, obj)
-
-        if funcs is None:
-            return
-
-        for name, f in funcs.items():  # override all methods
-            setattr(obj, name, types.MethodType(f, obj))
-            # types.MethodType() creates a bound method, bound to obj, from the function f
-
-    # -----------------------------------------------------------------------
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+    def override_code(obj: object, new_class_src) -> Union[None, Exception]:
+        try:
+            funcs = get_method_funcs(new_class_src, obj)
+            for name, f in funcs.items():  # override all methods
+                setattr(obj, name, types.MethodType(f, obj))
+                # types.MethodType() creates a method bound to obj, from the function f
+        except Exception as e:
+            return e
 
 
+    #
+    # below is the old implementation, for documentation purposes only; see discussion below
+    #
 
 
     @staticmethod
     def override_code_OLD(obj: object, orig_class_src, orig_mod_src, new_class_src):
-        """
-        ONLY FOR DOCUMENTATION: THIS IS THE OLD IMPLEMENTATION, SEE DISCUSSION BELOW
-        """
 
         import inspect
 
         # OLD INSPECT BASED VERSION:
         # original_module = inspect.getmodule(obj.__class__)
         # original_module_source_code = inspect.getsource(original_module)
         # original_class_source_code = inspect.getsource(obj.__class__)
```

### Comparing `ryven-3.1.1/ryven/gui/code_editor/pygments/dracula.py` & `ryven-3.4.0a1/ryven/gui/code_editor/pygments/dracula.py`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/gui/dialogs.py` & `ryven-3.4.0a1/ryven/gui/dialogs.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,30 +18,30 @@
         self.accept()
 
     def get_text(self):
         self.exec_()
         return self.text
 
 
-class ChooseScriptDialog(QDialog):
-    def __init__(self, window_title, scripts, parent=None):
+class ChooseFlowDialog(QDialog):
+    def __init__(self, window_title, flows, parent=None):
         super().__init__(parent)
 
-        self.script = None
-        self.button_scripts = {}
+        self.flow = None
+        self.button_flows = {}
 
         self.setLayout(QVBoxLayout())
-        for s in scripts:
+        for s in flows:
             b = QPushButton(s.title)
             b.pressed.connect(self.button_pressed)
-            self.button_scripts[b] = s
+            self.button_flows[b] = s
             self.layout().addWidget(b)
 
         self.setWindowTitle(window_title)
 
     def button_pressed(self):
-        self.script = self.button_scripts[self.sender()]
+        self.flow = self.button_flows[self.sender()]
         self.accept()
 
-    def get_script(self):
+    def get_flow(self):
         self.exec_()
-        return self.script
+        return self.flow
```

### Comparing `ryven-3.1.1/ryven/gui/main_console.py` & `ryven-3.4.0a1/ryven/gui/main_console.py`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/gui/script_UI.py` & `ryven-3.4.0a1/ryven/gui/flow_ui.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,71 @@
-"""A UI for scripts. Will be displayed in the tab widget in MainWindow."""
+"""A UI for flows. Will be displayed in the tab widget in MainWindow."""
 
 from qtpy.QtWidgets import QWidget, QHBoxLayout, QComboBox
 
-import ryvencore_qt.src.conv_gui as GUI
+import ryvencore_qt.src.widgets as GUI
 from ryvencore.RC import FlowAlg
 
 from ryven.gui.code_editor.CodePreviewWidget import CodePreviewWidget
-from ryven.gui.uic.ui_script import Ui_script_widget
+from ryven.gui.uic.ui_flow import Ui_flow_widget
 
 
-class ScriptUI(QWidget):
+class FlowUI(QWidget):
 
     flow_alg_mode_display_titles = {
         FlowAlg.DATA: 'data-flow',
         FlowAlg.DATA_OPT: 'data-flow opt',
         FlowAlg.EXEC: 'exec-flow',
     }
 
-    def __init__(self, main_window, script, flow_view):
+    def __init__(self, main_window, flow, flow_view):
         super().__init__(main_window)
 
-        self.script = script
+        self.flow = flow
         self.flow_view = flow_view
         
         # UI
-        self.ui = Ui_script_widget()
+        self.ui = Ui_flow_widget()
         self.ui.setupUi(self)
 
-        self.script.flow.algorithm_mode_changed.connect(self.flow_alg_mode_changed)
-        # self.script.flow_view.viewport_update_mode_changed.connect(self.flow_vp_update_mode_changed)
+        self.flow.algorithm_mode_changed.sub(self.flow_alg_mode_changed)
 
         self.flow_alg_mode_dropdown = QComboBox()
         for mode, title in self.flow_alg_mode_display_titles.items():
             self.flow_alg_mode_dropdown.addItem(title)
         self.ui.settings_groupBox.layout().addWidget(self.flow_alg_mode_dropdown)
         self.flow_alg_mode_dropdown.currentTextChanged.connect(self.flow_algorithm_mode_toggled)
 
         # catch up on flow modes
-        self.flow_alg_mode_changed(self.script.flow.algorithm_mode())
-        # self.flow_vp_update_mode_changed(self.script.flow_view.viewport_update_mode())
+        self.flow_alg_mode_changed(self.flow.algorithm_mode())
 
         # variables list widget
-        self.vars_list_widget = GUI.VarsList(self.script.vars_manager)
+        self.vars_list_widget = GUI.VarsList(self.flow.session.addons.get('Variables'), self.flow) # TODO: how are vars now managed?
         self.ui.variables_group_box.layout().addWidget(self.vars_list_widget)
         self.ui.settings_vars_splitter.setSizes([40, 700])
 
         # flow
         self.ui.splitter.insertWidget(0, self.flow_view)
 
         # code preview
         self.code_preview_widget = CodePreviewWidget(main_window, self.flow_view)
         self.ui.source_code_groupBox.layout().addWidget(self.code_preview_widget)
 
         # logs
         self.ui.logs_scrollArea.setWidget(self.create_loggers_widget())
         self.ui.splitter.setSizes([700, 0])
-        self.script.logs_manager.new_logger_created.connect(self.add_logger_widget)
+
+        # TODO: need to connect to logging event but seems it isn't implemented yet
+        #self.flow.session.addons.get('Logging').logs_manager.new_logger_created.connect(self.add_logger_widget)
 
         # catch up on logs which might have been loaded from a project already
-        for logger in self.script.logs_manager.loggers:
+        logging = self.flow.session.addons.get('Logging')
+        for logger in logging.loggers:
             self.add_logger_widget(logger)
+        logging.log_created.sub(self.add_logger_widget)
 
 
     def create_loggers_widget(self):
         w = QWidget()
         w.setLayout(QHBoxLayout())
         # w.setStyleSheet('')
         return w
@@ -77,13 +79,13 @@
         self.flow_alg_mode_dropdown.setCurrentText(
             self.flow_alg_mode_display_titles[FlowAlg.from_str(mode)]
         )
 
     
     def flow_algorithm_mode_toggled(self):
 
-        self.script.flow.set_algorithm_mode(
+        self.flow.set_algorithm_mode(
             FlowAlg.str(
                 list(self.flow_alg_mode_display_titles.keys())
                 [self.flow_alg_mode_dropdown.currentIndex()]
             )
         )
```

### Comparing `ryven-3.1.1/ryven/gui/startup_dialog/StartupDialog.py` & `ryven-3.4.0a1/ryven/main/packages/nodes_package.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,152 +1,197 @@
-from qtpy.QtWidgets import QDialog, QVBoxLayout, QHBoxLayout, QPushButton, QTextEdit, QFileDialog, QRadioButton
-from qtpy.QtGui import QIcon
+"""
+This module, together with the node_env and gui_env defines Ryven's nodes
+package system. It can be used outside of Ryven as well.
+"""
 
-from ryven.main.nodes_package import NodesPackage
-from ryven.main.utils import abs_path_from_package_dir, abs_path_from_ryven_dir
-from ryven.gui.styling.window_theme import apply_stylesheet
-from ryven.gui.startup_dialog.SelectPackages_Dialog import SelectPackages_Dialog
-
-
-class StartupDialog(QDialog):
-    """
-    The welcome dialog. The user can choose between creating a new project and loading a saved project.
-    When a project is loaded, it scans for validity of all the required packages for the project, and in case
-    some paths are invalid, the SelectPackages_Dialog is opened to get the paths to those missing package files.
-    """
-
-    def __init__(self, init_window_theme_name='dark', parent=None):
-        super().__init__(parent)
-
-        layout = QVBoxLayout()
-
-        # info text edit
-        info_text_edit = QTextEdit()
-        info_text_edit.setHtml('''
-            <center>
-                <h2 style="font-family: Segoe UI; font-size: xx-large; font-weight: 400; color: #a9d5ef;">
-                    Welcome to Ryven
-                </h2>
-            </center>
-            <div style="font-family: Corbel; font-size: x-large;">
-            
-                <p>
-                    <img style="float:right;" height=120 src="../resources/pics/Ryven_icon_blurred.png">Hey,
-                    it's Leon, the creator of Ryven. Keep in mind that this
-                    is not a professional piece of software. Don\'t forget to save!
-                    There are always some bugs and issues but as long as you keep behaving
-                    as intended, you shouldn\'t get into too much trouble. Have fun!
-                </p>
-            </div>
-        ''')
-        info_text_edit.setReadOnly(True)
-        layout.addWidget(info_text_edit)
-
-        # buttons
-        plain_project_push_button = QPushButton('create new project')
-        plain_project_push_button.setFocus()
-        plain_project_push_button.clicked.connect(self.plain_project_button_clicked)
-        load_project_push_button = QPushButton('load project')
-        load_project_push_button.clicked.connect(self.load_project_button_clicked)
-        load_example_project_push_button = QPushButton('load example')
-        load_example_project_push_button.clicked.connect(self.load_example_project_button_clicked)
-
-        buttons_layout = QHBoxLayout()
-        buttons_layout.addWidget(plain_project_push_button)
-        buttons_layout.addWidget(load_project_push_button)
-        buttons_layout.addWidget(load_example_project_push_button)
-
-        layout.addLayout(buttons_layout)
-
-        self.window_theme = apply_stylesheet(init_window_theme_name)
-
-        choose_theme_layout = QHBoxLayout()
-        self.dark_theme_rb = QRadioButton('dark')
-        self.dark_theme_rb.toggled.connect(self.theme_toggled)
-        self.dark_theme_rb.setChecked(init_window_theme_name == 'dark')
-        self.light_theme_rb = QRadioButton('light')
-        self.light_theme_rb.toggled.connect(self.theme_toggled)
-        self.light_theme_rb.setChecked(init_window_theme_name == 'light')
-        choose_theme_layout.addWidget(self.dark_theme_rb)
-        choose_theme_layout.addWidget(self.light_theme_rb)
-        layout.addLayout(choose_theme_layout)
-
-        self.setLayout(layout)
-
-        self.setWindowTitle('Ryven')
-        self.setWindowIcon(QIcon(abs_path_from_package_dir('resources/pics/Ryven_icon.png')))
-        self.setFixedSize(500, 280)
-
-        self.editor_startup_configuration = {}
-
-
-    def theme_toggled(self):
-        if self.dark_theme_rb.isChecked():
-            self.window_theme = apply_stylesheet('dark')
+import importlib.util
+import os
+import pathlib
+from os.path import basename, dirname, splitext, normpath, join
+from typing import Tuple, List, Type, Union, Set, Optional
+
+from ryvencore import Node, Data
+
+from ryven.main.utils import read_project, ryven_dir_path, abs_path_from_package_dir
+
+
+class NodesPackage:
+    """
+    A small container to store meta data about imported node packages.
+    """
+
+    def __init__(self, directory: str):
+
+        self.name = basename(normpath(directory))
+        self.directory = directory
+
+        self.file_path = normpath(join(directory, 'nodes.py'))
+
+    def __str__(self):
+        return f'{self.__class__.__name__}({self.name})'
+
+    def __repr__(self):
+        return f'{self.__class__.__name__}({self.name}, {self.directory})'
+
+    def __eq__(self, other):
+        if isinstance(other, NodesPackage):
+            return self.name == other.name
         else:
-            self.window_theme = apply_stylesheet('light')
+            return self.name == str(other)
 
+    def __hash__(self):
+        return hash(self.name)
 
-    def plain_project_button_clicked(self):
-        self.editor_startup_configuration['action'] = 'create project'
-        self.accept()
+    def config_data(self):
+        return {
+            'name': self.name,
+            'dir': self.directory,
+        }
 
 
-    def load_project_button_clicked(self):
-        self.open_project(base_dir=abs_path_from_ryven_dir('saves'))
+def load_from_file(file: str = None, components_list: [str] = None) -> tuple:
+    """
+    Imports specified components from a python module with given file path.
+    """
+    if components_list is None:
+        components_list = []
 
+    name = basename(file).split('.')[0]
+    spec = importlib.util.spec_from_file_location(name, file)
 
-    def load_example_project_button_clicked(self):
-        self.open_project(base_dir=abs_path_from_package_dir('examples_projects'))
+    importlib.util.module_from_spec(spec)
 
+    mod = spec.loader.load_module(name)
+    # using load_module(name) instead of exec_module(mod) here,
+    # because exec_module() somehow then registers it as "built-in"
+    # which is wrong and prevents inspect from parsing the source
 
-    def open_project(self, base_dir: str):
-        """1. Opens a file dialog for selecting a project tile; returns on FileNotFoundError,
-        2. Opens the project and scans all required node packages,
-        3. If node packages are missing (i.e. they cannot be found under the path specified
-        in the project file anymore) it opens the SelectPackages_Dialog
+    comps = tuple([getattr(mod, c) for c in components_list])
 
-        :param base_dir: path to directory where file dialog opens
-        """
+    return comps
 
-        self.editor_startup_configuration['action'] = 'open project'
-        import json
 
-        file_name = \
-            QFileDialog.getOpenFileName(
-                self, 'select project file',
-                base_dir, 'JSON (*.json)'
-            )[0]
+def import_nodes_package(package: NodesPackage = None, directory: str = None) -> \
+        Tuple[List[Type[Node]], List[Type[Data]]]:
+    """Loads node and data classes from a Ryven nodes package and returns both in separate lists.
 
-        try:
-            f = open(file_name)
-            project_str = f.read()
-            f.close()
-        except FileNotFoundError:
-            # TODO: do something useful here
-            return
+    Can be used without a running Ryven instance, but you need to specify in which mode nodes should be loaded
+    by setting the environment variable RYVEN_MODE to either 'gui' (gui imports enabled) or 'no-gui'.
 
-        # strict=False has to be to allow 'control characters' like '\n' for newline when loading the json
-        project_dict = json.loads(project_str, strict=False)
+    :param package: The NodesPackage object.
+    :param directory: The path to the directory where the nodes.py file is located, used if package is None.
+    :return: A tuple containing node types (classes) first, and the data types exported by the package second.
+    """
 
-        # scan for all required packages
-        valid_node_packages = []
-        missing_node_package_names = []
-        for p in project_dict['required packages']:
-            try:
-                f = open(p['dir']+'/nodes.py')
-                f.close()
-                valid_node_packages.append(NodesPackage(p['dir']))
-            except FileNotFoundError:
-                missing_node_package_names.append(p['name'])
+    if package is None:
+        package = NodesPackage(directory)
 
-        node_packages = valid_node_packages.copy()
+    if 'RYVEN_MODE' not in os.environ:
+        raise Exception(
+            "Please specify the environment variable RYVEN_MODE ('gui' or 'no-gui') before loading any packages. "
+            "For example set os.environ['RYVEN_MODE'] = 'no-gui' for gui-less deployment."
+        )
+
+    from ryven import node_env
+    node_env.NodesEnvRegistry.current_package = package
+    load_from_file(package.file_path)
+
+    node_types = node_env.NodesEnvRegistry.exported_nodes[-1]
+    data_types = node_env.NodesEnvRegistry.exported_data_types[-1]
+
+    return node_types, data_types
+
+
+def process_nodes_packages(
+    project_or_nodes: Union[
+        Union[str, pathlib.Path],                       # path to Ryven project
+        List[Union[str, pathlib.Path, NodesPackage]]    # list of node packages
+    ],
+    requested_packages: List[NodesPackage] = None
+) -> Tuple[Set[NodesPackage], List[pathlib.Path], Optional[dict]]:
+    """Takes a project or list of node packages and additionally requested node
+    packages and checks whether the node packages are valid.
+
+    It also removes duplicates based on the name (and not the contents!).
+
+    :param project_or_nodes:
+        Either a path to a Ryven project or a list of node packages.
+        If a Ryven project is given, the required nodes packages specified
+        in the project file are looked for.
+        If a list is given, `NodesPackage` instances are  copied into the
+        resulting list; paths are considered to direct to 'nodes.py'.
+        If 'nodes.py' is found in the path,
+        a `NodesPackage` instance is created and added to the resulting list.
+        If 'nodes.py' cannot be found in the path, the package is searched in
+        Ryven's example nodes dir, e.g. if "std" is given and not found
+        locally, the "std" package included in Ryven is loaded.
+    :param requested_packages:
+        A list of additional node package, which were requested. These take
+        precedence over `nodes`.
+        The default is `[]`.
+
+    :return:
+        A tuple of three elements:
+            - Set of available nodes required by the project or from list of nodes.
+            - Set of nodes required by the project or from list of nodes, which could not be found.
+            - Dictionary with the contents of the project or `None`.
+    """
+    # from ryven.main.packages.nodes_package import NodesPackage
 
-        if len(missing_node_package_names) > 0:
-            select_packages_dialog = SelectPackages_Dialog(self, required_packages=missing_node_package_names)
-            select_packages_dialog.exec_()
-            node_packages += select_packages_dialog.packages
+    if requested_packages is None:
+        requested_packages = []
 
-        self.editor_startup_configuration['required packages'] = node_packages
-        self.editor_startup_configuration['content'] = project_dict
+    # Find nodes in the project file
+    try:
+        project_dict = read_project(project_or_nodes)
+        node_pkg_paths = [p['dir'] for p in project_dict['required packages']]
+    except TypeError:
+        project_dict = None
+        node_pkg_paths = project_or_nodes
+    except KeyError:
+        # No required packages found
+        project_dict = None
+        node_pkg_paths = []
+
+    pkgs = set()
+    pkgs_not_found = set()
+    for pkg in node_pkg_paths:
+        if isinstance(pkg, NodesPackage):
+            pkgs.add(pkg)
+        else:
+            # For backward compatibility we have to deal with Windows and Posix
+            # paths in the project's file
+            pkg_windows_path = pathlib.PureWindowsPath(pkg)
+            pkg_posix_path = pathlib.PurePosixPath(pkg)
+            if len(pkg_windows_path.parts) > len(pkg_posix_path.parts):
+                pkg_path = pathlib.Path(pkg_windows_path)
+            else:
+                pkg_path = pathlib.Path(pkg_posix_path)
+            if pkg_path.joinpath('nodes.py').exists():
+                pkgs.add(NodesPackage(str(pkg_path)))
+                continue
+
+            # Try to find the nodes package in Ryven's custom nodes dir
+            pkg_custom_path = pathlib.Path(ryven_dir_path(), 'nodes', pkg)
+            if pkg_custom_path.joinpath('nodes.py').exists():
+                pkgs.add(NodesPackage(str(pkg_custom_path)))
+                continue
+
+            # Try to find in Ryven's example nodes
+            pkg_example_path = pathlib.Path(abs_path_from_package_dir('example_nodes'), pkg)
+            if pkg_example_path.joinpath('nodes.py').exists():
+                pkgs.add(NodesPackage(str(pkg_example_path)))
+                continue
+
+            # Package could not be found
+            pkgs_not_found.add(pkg_path)
+
+    # Check, if nodes which could not be found are already available in
+    # `requested_nodes`.
+    # This check is done by comparing the path name to the nodes' names
+    args_pkgs_names = [pkg.name for pkg in requested_packages]
+    pkgs_not_found = [
+        pkg_path
+        for pkg_path in pkgs_not_found
+        if pkg_path.name not in args_pkgs_names]
 
-        self.accept()
+    return pkgs, pkgs_not_found, project_dict
```

### Comparing `ryven-3.1.1/ryven/gui/styling/design_config.json` & `ryven-3.4.0a1/ryven/gui/styling/design_config.json`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/gui/styling/window_theme.py` & `ryven-3.4.0a1/ryven/gui/styling/window_theme.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from qtpy.QtWidgets import QApplication
 from ryven.main.utils import abs_path_from_package_dir
 
 
 def hex_to_rgb(hex: str):
-    return tuple(int(hex[i:i + 2], 16) for i in (1, 3, 5))
+    if hex is None:
+        return None
+    else:
+        return tuple(int(hex[i:i + 2], 16) for i in (1, 3, 5))
 
 
 class WindowTheme:
 
     name = ''
     colors = {}
     rules = {}
@@ -59,38 +62,57 @@
         'secondaryTextColor': '#6E6E6E',
         'danger': '#dc3545',
         'warning': '#ffc107',
         'success': '#17a2b8',
     }
 
 
+class WindowTheme_Plain(WindowTheme):
+    name = 'plain'
+    colors = {
+        'primaryColor': None,
+        'primaryLightColor': None,
+        'secondaryColor': None,
+        'secondaryLightColor': None,
+        'secondaryDarkColor': None,
+        'primaryTextColor': None,
+        'secondaryTextColor': None,
+        'danger': None,
+        'warning': None,
+        'success': None,
+    }
+
+
 def apply_stylesheet(style: str):
 
     # set to None if not used
     icons_dir = abs_path_from_package_dir('resources/stylesheets/icons')
-
-    # path to the template stylesheet file
-    template_file = abs_path_from_package_dir('resources/stylesheets/style_template.css')
-
-    # ------------------------------
-
     if icons_dir is not None:
         from qtpy.QtCore import QDir
         d = QDir()
         d.setSearchPaths('icon', [icons_dir])
 
-    if style == 'dark':
-        window_theme = WindowTheme_Dark()
+    if style in (None, 'plain'):
+        window_theme = WindowTheme_Plain()
+        stylesheet = None
     else:
-        window_theme = WindowTheme_Light()
-
-    f = open(template_file)
-
-    from jinja2 import Template
-    jinja_template = Template(f.read())
+        if style == 'dark':
+            window_theme = WindowTheme_Dark()
+        elif style == 'light':
+            window_theme = WindowTheme_Light()
+        else:
+            raise ValueError(
+                f'Unknown window theme. '
+                f'Got: {style}')
+
+        from jinja2 import Template
+        # path to the template stylesheet file
+        template_file = abs_path_from_package_dir('resources/stylesheets/style_template.css')
+        with open(template_file) as f:
+            jinja_template = Template(f.read())
 
-    f.close()
+        stylesheet = jinja_template.render(window_theme.rules)
 
     app = QApplication.instance()
-    app.setStyleSheet(jinja_template.render(window_theme.rules))
+    app.setStyleSheet(stylesheet)
 
     return window_theme
```

### Comparing `ryven-3.1.1/ryven/gui/uic/main_window.ui` & `ryven-3.4.0a1/ryven/gui/uic/main_window.ui`

 * *Files 3% similar despite different names*

#### Comparing `ryven-3.1.1/ryven/gui/uic/main_window.ui` & `ryven-3.4.0a1/ryven/gui/uic/main_window.ui`

```diff
@@ -30,28 +30,28 @@
               <property name="orientation">
                 <enum>Qt::Horizontal</enum>
               </property>
               <widget class="QSplitter" name="splitter">
                 <property name="orientation">
                   <enum>Qt::Vertical</enum>
                 </property>
-                <widget class="QGroupBox" name="scripts_groupBox">
+                <widget class="QGroupBox" name="flows_groupBox">
                   <property name="title">
-                    <string>Scripts</string>
+                    <string>Flows</string>
                   </property>
                   <layout class="QVBoxLayout" name="verticalLayout_2"/>
                 </widget>
                 <widget class="QGroupBox" name="nodes_groupBox">
                   <property name="title">
                     <string>Nodes</string>
                   </property>
                   <layout class="QVBoxLayout" name="verticalLayout"/>
                 </widget>
               </widget>
-              <widget class="QTabWidget" name="scripts_tab_widget">
+              <widget class="QTabWidget" name="flows_tab_widget">
                 <property name="sizePolicy">
                   <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                     <horstretch>0</horstretch>
                     <verstretch>0</verstretch>
                   </sizepolicy>
                 </property>
                 <property name="currentIndex">
@@ -71,28 +71,28 @@
     </widget>
     <widget class="QMenuBar" name="menuBar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>1368</width>
-          <height>21</height>
+          <height>30</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
           <string>File</string>
         </property>
         <widget class="QMenu" name="menuScripts">
           <property name="title">
             <string>Scripts</string>
           </property>
-          <addaction name="actionNew_Script"/>
-          <addaction name="actionRename_Script"/>
-          <addaction name="actionDelete_Script"/>
+          <addaction name="actionNew_Flow"/>
+          <addaction name="actionRename_Flow"/>
+          <addaction name="actionDelete_Flow"/>
         </widget>
         <addaction name="actionImport_Nodes"/>
         <addaction name="actionImport_Example_Nodes"/>
         <addaction name="actionSave_Project"/>
         <addaction name="menuScripts"/>
       </widget>
       <widget class="QMenu" name="menuView">
@@ -178,25 +178,25 @@
       </property>
       <property name="toolTip">
         <string>Saves a picture of the whole current scene. 
 The more you zoomed in, the sharper the picture.
 This will take a few seconds.</string>
       </property>
     </action>
-    <action name="actionNew_Script">
+    <action name="actionNew_Flow">
       <property name="text">
         <string>New</string>
       </property>
     </action>
-    <action name="actionRename_Script">
+    <action name="actionRename_Flow">
       <property name="text">
         <string>Rename</string>
       </property>
     </action>
-    <action name="actionDelete_Script">
+    <action name="actionDelete_Flow">
       <property name="text">
         <string>Delete</string>
       </property>
     </action>
     <action name="actionImport_Example_Nodes">
       <property name="text">
         <string>Import Example Nodes</string>
```

### Comparing `ryven-3.1.1/ryven/gui/uic/script.ui` & `ryven-3.4.0a1/ryven/gui/uic/flow.ui`

 * *Files 7% similar despite different names*

#### Comparing `ryven-3.1.1/ryven/gui/uic/script.ui` & `ryven-3.4.0a1/ryven/gui/uic/flow.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>script_widget</class>
-  <widget class="QWidget" name="script_widget">
+  <class>flow_widget</class>
+  <widget class="QWidget" name="flow_widget">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>1223</width>
         <height>876</height>
       </rect>
@@ -38,16 +38,16 @@
                         <bool>true</bool>
                       </property>
                       <widget class="QWidget" name="scrollAreaWidgetContents">
                         <property name="geometry">
                           <rect>
                             <x>0</x>
                             <y>0</y>
-                            <width>297</width>
-                            <height>812</height>
+                            <width>544</width>
+                            <height>818</height>
                           </rect>
                         </property>
                         <layout class="QHBoxLayout" name="horizontalLayout_3"/>
                       </widget>
                     </widget>
                   </item>
                 </layout>
@@ -103,12 +103,8 @@
           </widget>
         </widget>
       </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
-  <buttongroups>
-    <buttongroup name="algorithm_buttonGroup"/>
-    <buttongroup name="viewport_update_mode_buttonGroup"/>
-  </buttongroups>
 </ui>
```

### Comparing `ryven-3.1.1/ryven/gui/uic/ui_main_window.py` & `ryven-3.4.0a1/ryven/gui/uic/ui_main_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,20 +35,20 @@
         self.actionEnableInfoMessages.setObjectName(u"actionEnableInfoMessages")
         self.actionDisableInfoMessages = QAction(MainWindow)
         self.actionDisableInfoMessages.setObjectName(u"actionDisableInfoMessages")
         self.actionSave_Pic_Viewport = QAction(MainWindow)
         self.actionSave_Pic_Viewport.setObjectName(u"actionSave_Pic_Viewport")
         self.actionSave_Pic_Whole_Scene_scaled = QAction(MainWindow)
         self.actionSave_Pic_Whole_Scene_scaled.setObjectName(u"actionSave_Pic_Whole_Scene_scaled")
-        self.actionNew_Script = QAction(MainWindow)
-        self.actionNew_Script.setObjectName(u"actionNew_Script")
-        self.actionRename_Script = QAction(MainWindow)
-        self.actionRename_Script.setObjectName(u"actionRename_Script")
-        self.actionDelete_Script = QAction(MainWindow)
-        self.actionDelete_Script.setObjectName(u"actionDelete_Script")
+        self.actionNew_Flow = QAction(MainWindow)
+        self.actionNew_Flow.setObjectName(u"actionNew_Flow")
+        self.actionRename_Flow = QAction(MainWindow)
+        self.actionRename_Flow.setObjectName(u"actionRename_Flow")
+        self.actionDelete_Flow = QAction(MainWindow)
+        self.actionDelete_Flow.setObjectName(u"actionDelete_Flow")
         self.actionImport_Example_Nodes = QAction(MainWindow)
         self.actionImport_Example_Nodes.setObjectName(u"actionImport_Example_Nodes")
         self.centralWidget = QWidget(MainWindow)
         self.centralWidget.setObjectName(u"centralWidget")
         self.gridLayout = QGridLayout(self.centralWidget)
         self.gridLayout.setSpacing(6)
         self.gridLayout.setContentsMargins(11, 11, 11, 11)
@@ -58,51 +58,51 @@
         self.main_vertical_splitter.setOrientation(Qt.Vertical)
         self.main_horizontal_splitter = QSplitter(self.main_vertical_splitter)
         self.main_horizontal_splitter.setObjectName(u"main_horizontal_splitter")
         self.main_horizontal_splitter.setOrientation(Qt.Horizontal)
         self.splitter = QSplitter(self.main_horizontal_splitter)
         self.splitter.setObjectName(u"splitter")
         self.splitter.setOrientation(Qt.Vertical)
-        self.scripts_groupBox = QGroupBox(self.splitter)
-        self.scripts_groupBox.setObjectName(u"scripts_groupBox")
-        self.verticalLayout_2 = QVBoxLayout(self.scripts_groupBox)
+        self.flows_groupBox = QGroupBox(self.splitter)
+        self.flows_groupBox.setObjectName(u"flows_groupBox")
+        self.verticalLayout_2 = QVBoxLayout(self.flows_groupBox)
         self.verticalLayout_2.setSpacing(6)
         self.verticalLayout_2.setContentsMargins(11, 11, 11, 11)
         self.verticalLayout_2.setObjectName(u"verticalLayout_2")
-        self.splitter.addWidget(self.scripts_groupBox)
+        self.splitter.addWidget(self.flows_groupBox)
         self.nodes_groupBox = QGroupBox(self.splitter)
         self.nodes_groupBox.setObjectName(u"nodes_groupBox")
         self.verticalLayout = QVBoxLayout(self.nodes_groupBox)
         self.verticalLayout.setSpacing(6)
         self.verticalLayout.setContentsMargins(11, 11, 11, 11)
         self.verticalLayout.setObjectName(u"verticalLayout")
         self.splitter.addWidget(self.nodes_groupBox)
         self.main_horizontal_splitter.addWidget(self.splitter)
-        self.scripts_tab_widget = QTabWidget(self.main_horizontal_splitter)
-        self.scripts_tab_widget.setObjectName(u"scripts_tab_widget")
+        self.flows_tab_widget = QTabWidget(self.main_horizontal_splitter)
+        self.flows_tab_widget.setObjectName(u"flows_tab_widget")
         sizePolicy1 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
         sizePolicy1.setHorizontalStretch(0)
         sizePolicy1.setVerticalStretch(0)
-        sizePolicy1.setHeightForWidth(self.scripts_tab_widget.sizePolicy().hasHeightForWidth())
-        self.scripts_tab_widget.setSizePolicy(sizePolicy1)
+        sizePolicy1.setHeightForWidth(self.flows_tab_widget.sizePolicy().hasHeightForWidth())
+        self.flows_tab_widget.setSizePolicy(sizePolicy1)
         self.tab = QWidget()
         self.tab.setObjectName(u"tab")
-        self.scripts_tab_widget.addTab(self.tab, "")
-        self.main_horizontal_splitter.addWidget(self.scripts_tab_widget)
+        self.flows_tab_widget.addTab(self.tab, "")
+        self.main_horizontal_splitter.addWidget(self.flows_tab_widget)
         self.main_vertical_splitter.addWidget(self.main_horizontal_splitter)
         self.console_placeholder_widget = QWidget(self.main_vertical_splitter)
         self.console_placeholder_widget.setObjectName(u"console_placeholder_widget")
         self.main_vertical_splitter.addWidget(self.console_placeholder_widget)
 
         self.gridLayout.addWidget(self.main_vertical_splitter, 0, 0, 1, 1)
 
         MainWindow.setCentralWidget(self.centralWidget)
         self.menuBar = QMenuBar(MainWindow)
         self.menuBar.setObjectName(u"menuBar")
-        self.menuBar.setGeometry(QRect(0, 0, 1368, 21))
+        self.menuBar.setGeometry(QRect(0, 0, 1368, 30))
         self.menuFile = QMenu(self.menuBar)
         self.menuFile.setObjectName(u"menuFile")
         self.menuScripts = QMenu(self.menuFile)
         self.menuScripts.setObjectName(u"menuScripts")
         self.menuView = QMenu(self.menuBar)
         self.menuView.setObjectName(u"menuView")
         self.menuFlow_Design_Style = QMenu(self.menuView)
@@ -121,29 +121,29 @@
         self.menuBar.addAction(self.menuFile.menuAction())
         self.menuBar.addAction(self.menuView.menuAction())
         self.menuBar.addAction(self.menuDebugging.menuAction())
         self.menuFile.addAction(self.actionImport_Nodes)
         self.menuFile.addAction(self.actionImport_Example_Nodes)
         self.menuFile.addAction(self.actionSave_Project)
         self.menuFile.addAction(self.menuScripts.menuAction())
-        self.menuScripts.addAction(self.actionNew_Script)
-        self.menuScripts.addAction(self.actionRename_Script)
-        self.menuScripts.addAction(self.actionDelete_Script)
+        self.menuScripts.addAction(self.actionNew_Flow)
+        self.menuScripts.addAction(self.actionRename_Flow)
+        self.menuScripts.addAction(self.actionDelete_Flow)
         self.menuView.addSeparator()
         self.menuView.addAction(self.menuFlow_Design_Style.menuAction())
         self.menuView.addAction(self.menuSave_Picture.menuAction())
         self.menuSave_Picture.addAction(self.actionSave_Pic_Viewport)
         self.menuSave_Picture.addAction(self.actionSave_Pic_Whole_Scene_scaled)
         self.menuDebugging.addAction(self.menuInfo_Messages.menuAction())
         self.menuInfo_Messages.addAction(self.actionEnableInfoMessages)
         self.menuInfo_Messages.addAction(self.actionDisableInfoMessages)
 
         self.retranslateUi(MainWindow)
 
-        self.scripts_tab_widget.setCurrentIndex(0)
+        self.flows_tab_widget.setCurrentIndex(0)
 
 
         QMetaObject.connectSlotsByName(MainWindow)
     # setupUi
 
     def retranslateUi(self, MainWindow):
         MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"MainWindow", None))
@@ -160,21 +160,21 @@
 #endif // QT_CONFIG(tooltip)
         self.actionSave_Pic_Whole_Scene_scaled.setText(QCoreApplication.translate("MainWindow", u"Save Pic - Whole Scene (scaled)", None))
 #if QT_CONFIG(tooltip)
         self.actionSave_Pic_Whole_Scene_scaled.setToolTip(QCoreApplication.translate("MainWindow", u"Saves a picture of the whole current scene. \n"
 "The more you zoomed in, the sharper the picture.\n"
 "This will take a few seconds.", None))
 #endif // QT_CONFIG(tooltip)
-        self.actionNew_Script.setText(QCoreApplication.translate("MainWindow", u"New", None))
-        self.actionRename_Script.setText(QCoreApplication.translate("MainWindow", u"Rename", None))
-        self.actionDelete_Script.setText(QCoreApplication.translate("MainWindow", u"Delete", None))
+        self.actionNew_Flow.setText(QCoreApplication.translate("MainWindow", u"New", None))
+        self.actionRename_Flow.setText(QCoreApplication.translate("MainWindow", u"Rename", None))
+        self.actionDelete_Flow.setText(QCoreApplication.translate("MainWindow", u"Delete", None))
         self.actionImport_Example_Nodes.setText(QCoreApplication.translate("MainWindow", u"Import Example Nodes", None))
-        self.scripts_groupBox.setTitle(QCoreApplication.translate("MainWindow", u"Scripts", None))
+        self.flows_groupBox.setTitle(QCoreApplication.translate("MainWindow", u"Flows", None))
         self.nodes_groupBox.setTitle(QCoreApplication.translate("MainWindow", u"Nodes", None))
-        self.scripts_tab_widget.setTabText(self.scripts_tab_widget.indexOf(self.tab), QCoreApplication.translate("MainWindow", u"Main", None))
+        self.flows_tab_widget.setTabText(self.flows_tab_widget.indexOf(self.tab), QCoreApplication.translate("MainWindow", u"Main", None))
         self.menuFile.setTitle(QCoreApplication.translate("MainWindow", u"File", None))
         self.menuScripts.setTitle(QCoreApplication.translate("MainWindow", u"Scripts", None))
         self.menuView.setTitle(QCoreApplication.translate("MainWindow", u"View", None))
         self.menuFlow_Design_Style.setTitle(QCoreApplication.translate("MainWindow", u"Flow Theme", None))
         self.menuSave_Picture.setTitle(QCoreApplication.translate("MainWindow", u"Save Picture", None))
         self.menuDebugging.setTitle(QCoreApplication.translate("MainWindow", u"Options", None))
         self.menuInfo_Messages.setTitle(QCoreApplication.translate("MainWindow", u"Info Messages", None))
```

### Comparing `ryven-3.1.1/ryven/gui/uic/ui_script.py` & `ryven-3.4.0a1/ryven/gui/uic/ui_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 
 ################################################################################
-## Form generated from reading UI file 'script.ui'
+## Form generated from reading UI file 'flow.ui'
 ##
 ## Created by: Qt User Interface Compiler version 5.15.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
-from PySide2.QtCore import *
-from PySide2.QtGui import *
-from PySide2.QtWidgets import *
+from qtpy.QtCore import *
+from qtpy.QtGui import *
+from qtpy.QtWidgets import *
 
 
-class Ui_script_widget(object):
-    def setupUi(self, script_widget):
-        if not script_widget.objectName():
-            script_widget.setObjectName(u"script_widget")
-        script_widget.resize(1223, 876)
-        self.gridLayout_4 = QGridLayout(script_widget)
+class Ui_flow_widget(object):
+    def setupUi(self, flow_widget):
+        if not flow_widget.objectName():
+            flow_widget.setObjectName(u"flow_widget")
+        flow_widget.resize(1223, 876)
+        self.gridLayout_4 = QGridLayout(flow_widget)
         self.gridLayout_4.setObjectName(u"gridLayout_4")
-        self.splitter_3 = QSplitter(script_widget)
+        self.splitter_3 = QSplitter(flow_widget)
         self.splitter_3.setObjectName(u"splitter_3")
         self.splitter_3.setOrientation(Qt.Horizontal)
         self.splitter = QSplitter(self.splitter_3)
         self.splitter.setObjectName(u"splitter")
         self.splitter.setOrientation(Qt.Vertical)
         self.splitter_2 = QSplitter(self.splitter)
         self.splitter_2.setObjectName(u"splitter_2")
@@ -34,15 +34,15 @@
         self.gridLayout_2 = QGridLayout(self.log_groupBox)
         self.gridLayout_2.setObjectName(u"gridLayout_2")
         self.logs_scrollArea = QScrollArea(self.log_groupBox)
         self.logs_scrollArea.setObjectName(u"logs_scrollArea")
         self.logs_scrollArea.setWidgetResizable(True)
         self.scrollAreaWidgetContents = QWidget()
         self.scrollAreaWidgetContents.setObjectName(u"scrollAreaWidgetContents")
-        self.scrollAreaWidgetContents.setGeometry(QRect(0, 0, 297, 812))
+        self.scrollAreaWidgetContents.setGeometry(QRect(0, 0, 544, 818))
         self.horizontalLayout_3 = QHBoxLayout(self.scrollAreaWidgetContents)
         self.horizontalLayout_3.setObjectName(u"horizontalLayout_3")
         self.logs_scrollArea.setWidget(self.scrollAreaWidgetContents)
 
         self.gridLayout_2.addWidget(self.logs_scrollArea, 0, 0, 1, 1)
 
         self.splitter_2.addWidget(self.log_groupBox)
@@ -85,20 +85,20 @@
         self.gridLayout_5.addWidget(self.settings_vars_splitter, 0, 0, 1, 1)
 
         self.splitter_3.addWidget(self.contents_widget)
 
         self.gridLayout_4.addWidget(self.splitter_3, 0, 0, 1, 1)
 
 
-        self.retranslateUi(script_widget)
+        self.retranslateUi(flow_widget)
 
-        QMetaObject.connectSlotsByName(script_widget)
+        QMetaObject.connectSlotsByName(flow_widget)
     # setupUi
 
-    def retranslateUi(self, script_widget):
-        script_widget.setWindowTitle(QCoreApplication.translate("script_widget", u"Form", None))
-        self.log_groupBox.setTitle(QCoreApplication.translate("script_widget", u"Log", None))
-        self.source_code_groupBox.setTitle(QCoreApplication.translate("script_widget", u"Source Code", None))
-        self.settings_groupBox.setTitle(QCoreApplication.translate("script_widget", u"Settings", None))
-        self.variables_group_box.setTitle(QCoreApplication.translate("script_widget", u"Variables", None))
+    def retranslateUi(self, flow_widget):
+        flow_widget.setWindowTitle(QCoreApplication.translate("flow_widget", u"Form", None))
+        self.log_groupBox.setTitle(QCoreApplication.translate("flow_widget", u"Log", None))
+        self.source_code_groupBox.setTitle(QCoreApplication.translate("flow_widget", u"Source Code", None))
+        self.settings_groupBox.setTitle(QCoreApplication.translate("flow_widget", u"Settings", None))
+        self.variables_group_box.setTitle(QCoreApplication.translate("flow_widget", u"Variables", None))
     # retranslateUi
```

### Comparing `ryven-3.1.1/ryven/main/nodes/built_in/nodes.py` & `ryven-3.4.0a1/ryven/main/packages/built_in/nodes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,282 +1,269 @@
-from ryven.NENV import *
-widgets = import_widgets(__file__)
+from ryven.node_env import *
+guis = import_guis(__file__)
+import ryvencore as rc
 
 
 class NodeBase(Node):
-    pass
+    def have_gui(self):
+        return hasattr(self, 'gui')
+
+    def vars_addon(self):
+        return self.get_addon('Variables')
+
+    def get_var_val(self, var_name):
+        return self.vars_addon().var(self.flow, var_name).get()
+
+    def set_var_val(self, var_name, val):
+        return self.vars_addon().var(self.flow, var_name).set(val)
+
 
 
 class GetVar_Node(NodeBase):
     """Gets the value of a script variable"""
 
-    version = 'v0.1'
+    version = 'v0.2'
 
     title = 'get var'
     init_inputs = [
-        NodeInputBP(dtype=dtypes.String(size='m')),
+        NodeInputType(),
     ]
     init_outputs = [
-        NodeOutputBP(label='val')
+        NodeOutputType(label='val')
     ]
-    color = '#c69a15'
+    GUI = guis.GetVarGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.var_name = ''
         self.temp_var_val = None
 
     def place_event(self):
         self.update()
-
-    def view_place_event(self):
-        self.var_name = self.input(0)
+        if self.input(0) is not None:
+            self.var_name = self.input(0).payload
 
     def update_event(self, input_called=-1):
-        if self.input(0) != self.var_name:
+        if self.input(0).payload != self.var_name:
 
             if self.var_name != '':  # disconnect old var val update connection
-                self.unregister_var_receiver(self.var_name, self.var_val_changed)
+                self.vars_addon().unsubscribe(self, self.var_name, self.var_val_changed)
 
-            self.var_name = self.input(0)
+            self.var_name = self.input(0).payload
 
             # create new var update connection
-            self.register_var_receiver(self.var_name, self.var_val_changed)
+            self.vars_addon().subscribe(self, self.var_name, self.var_val_changed)
 
-        self.set_output_val(0, self.get_var_val(self.var_name))
+        self.set_output_val(0, Data(self.get_var_val(self.var_name)))
 
-    def var_val_changed(self, name, val):
-        self.set_output_val(0, val)
+    def var_val_changed(self, _):
+        self.set_output_val(0, Data(self.get_var_val(self.var_name)))
 
 
 class Result_Node(NodeBase):
     """Simply shows a value converted to str"""
 
-    version = 'v0.1'
+    version = 'v0.2'
 
     title = 'result'
     init_inputs = [
-        NodeInputBP(type_='data'),
+        NodeInputType(type_='data'),
     ]
-    main_widget_class = widgets.Result_Node_MainWidget
-    main_widget_pos = 'between ports'
-    color = '#c69a15'
+    GUI = guis.ResultGui
 
     def __init__(self, params):
         super().__init__(params)
         self.val = None
 
-    def place_event(self):
+    def rebuilt(self):
         self.update()
 
-    def view_place_event(self):
-        self.main_widget().show_val(self.val)
-
     def update_event(self, input_called=-1):
-        self.val = self.input(0)
-        if self.session.gui:
-            self.main_widget().show_val(self.val)
+        self.val = self.input(0).payload
+        if self.have_gui():
+            self.gui.main_widget().show_val(self.val)
 
 
 class Val_Node(NodeBase):
     """Evaluates a string from the input field"""
 
-    version = 'v0.1'
+    version = 'v0.2'
 
     title = 'val'
     init_inputs = [
-        NodeInputBP(dtype=dtypes.Data(size='s')),
+        # NodeInputType(default=Data()),
     ]
     init_outputs = [
-        NodeInputBP(type_='data'),
+        NodeInputType(type_='data'),
     ]
-    style = 'small'
-    color = '#c69a15'
+    GUI = guis.ValGui
 
     def __init__(self, params):
         super().__init__(params)
 
         self.display_title = ''
-        self.actions['edit val via dialog'] = {'method': self.action_edit_via_dialog}
-        self.val = None
+        self.val = Data()
 
 
     def place_event(self):
         self.update()
 
     def update_event(self, input_called=-1):
-        self.val = self.input(0)
         self.set_output_val(0, self.val)
 
-    def action_edit_via_dialog(self):
-        return
-
-        # from ..EditVal_Dialog import EditVal_Dialog
-        #
-        # val_dialog = EditVal_Dialog(parent=None, init_val=self.val)
-        # accepted = val_dialog.exec_()
-        # if accepted:
-        #     self.main_widget().setText(str(val_dialog.get_val()))
-        #     self.update()
-
     def get_current_var_name(self):
-        return self.input(0)
+        return self.input(0).payload if self.input(0) is not None else None
 
     def get_state(self):
         return {
             'val': self.val  # self.main_widget().get_val()
         }
 
     def set_state(self, data, version):
         self.val = data['val']
 
-        if version is None:
-
-            self.display_title = ''
-
-            self.create_input_dt(dtype=dtypes.Data(size='s'))
-
-            # the old version didn't use a dtype
-            self.inputs[0].dtype.val = self.val
-            self.inputs[0].update(self.val)
-
-
 
 class SetVar_Node(NodeBase):
     """Sets the value of a script variable"""
 
     version = 'v0.1'
 
     title = 'set var'
     init_inputs = [
-        NodeInputBP(type_='exec'),
-        NodeInputBP(dtype=dtypes.String(), label='var'),
-        NodeInputBP(dtype=dtypes.Data(size='s'), label='val'),
+        NodeInputType(type_='exec'),
+        NodeInputType(label='var'),
+        NodeInputType(label='val'),
     ]
     init_outputs = [
-        NodeOutputBP(type_='exec'),
-        NodeOutputBP(type_='data', label='val'),
+        NodeOutputType(type_='exec'),
+        NodeOutputType(type_='data', label='val'),
     ]
-    style = 'normal'
-    color = '#c69a15'
+
+    GUI = guis.SetVarGui
 
     def __init__(self, params):
         super().__init__(params)
 
-        self.actions['make passive'] = {'method': self.action_make_passive}
         self.active = True
 
         self.var_name = ''
         self.num_vars = 1
 
+    def place_event(self):
+        if self.have_gui():
+            self.gui.actions['make passive'] = {'method': self.action_make_passive}
+
     def update_event(self, input_called=-1):
 
         if self.active and input_called == 0:
 
-            if self.set_var_val(self.input(1), self.input(2)):
+            if self.set_var_val(self.input(1).payload, self.input(2).payload):
                 self.set_output_val(1, self.input(2))
             self.exec_output(0)
 
         elif not self.active:
 
-            self.var_name = self.input(0)
-            if self.set_var_val(self.input(0), self.input(1)):
-                self.set_output_val(0, self.get_var_val(self.var_name))
+            self.var_name = self.input(0).payload
+            if self.set_var_val(self.input(0).payload, self.input(1).payload):
+                self.set_output_val(0, Data(self.get_var_val(self.var_name)))
 
     def action_make_passive(self):
         self.active = False
         self.delete_input(0)
         self.delete_output(0)
-        del self.actions['make passive']
-        self.actions['make active'] = {'method': self.action_make_active}
+        del self.gui.actions['make passive']
+        self.gui.actions['make active'] = {'method': self.action_make_active}
 
     def action_make_active(self):
         self.active = True
         self.create_input(type_='exec', pos=0)
         self.create_output(type_='exec', pos=0)
-        del self.actions['make active']
-        self.actions['make passive'] = {'method': self.action_make_passive}
+        del self.gui.actions['make active']
+        self.gui.actions['make passive'] = {'method': self.action_make_passive}
 
     def get_state(self):
         return {'active': self.active}
 
     def set_state(self, data, version):
         self.active = data['active']
 
+        # because otherwise he widgets won't work
+        if not self.active:
+            self.action_make_passive()
+
 
 class SetVarsPassive_Node(NodeBase):
     """Sets the values of multiple script variables"""
 
     version = 'v0.1'
 
     title = 'set vars passive'
     init_inputs = []
     init_outputs = []
-    style = 'normal'
-    color = '#c69a15'
+    GUI = guis.SetVarsGui
 
     def __init__(self, params):
         super().__init__(params)
 
-        self.actions['add var input'] = {'method': self.add_var_input}
-
         self.num_vars = 0
 
-    def place_event(self):
-        if self.num_vars == 0:
-            self.add_var_input()
-
     def add_var_input(self):
-        self.create_input_dt(label='var', dtype=dtypes.String(size='l'))
-        self.create_input_dt(label='val', dtype=dtypes.Data(size='l'))
+        # self.create_input_dt(label='var', dtype=dtypes.String(size='l'))
+        # self.create_input_dt(label='val', dtype=dtypes.Data(size='l'))
+        self.create_input(label='var')
+        self.create_input(label='val')
+
         self.num_vars += 1
 
-        self.actions[f'remove var {self.num_vars}'] = {
-            'method': self.remove_var_input,
-            'data': self.num_vars
-        }
+        if self.have_gui():
+            self.gui.rebuild_remove_actions()
 
     def remove_var_input(self, number):
         self.delete_input((number-1)*2)
         self.delete_input((number-1)*2)
         self.num_vars -= 1
-        self.rebuild_remove_actions()
+        # self.rebuild_remove_actions()
 
-    def rebuild_remove_actions(self):
+        if self.have_gui():
+            self.gui.rebuild_remove_actions()
 
-        remove_keys = []
-        for k, v in self.actions.items():
-            if k.startswith('remove var'):
-                remove_keys.append(k)
-
-        for k in remove_keys:
-            del self.actions[k]
-
-        for i in range(self.num_vars):
-            self.actions[f'remove var {i+1}'] = {
-                'method': self.remove_var_input,
-                'data': i+1
-            }
+    # def rebuild_remove_actions(self):
+    #     if not self.have_gui():
+    #         return
+    #
+    #     remove_keys = []
+    #     for k, v in self.gui.actions.items():
+    #         if k.startswith('remove var'):
+    #             remove_keys.append(k)
+    #
+    #     for k in remove_keys:
+    #         del self.gui.actions[k]
+    #
+    #     for i in range(self.num_vars):
+    #         self.gui.actions[f'remove var {i+1}'] = {
+    #             'method': self.remove_var_input,
+    #             'data': i+1
+    #         }
 
     def update_event(self, input_called=-1):
 
-        var_names = [self.input(i) for i in range(0, len(self.inputs), 2)]
-        values = [self.input(i) for i in range(1, len(self.inputs), 2)]
+        var_names = [self.input(i).payload for i in range(0, len(self.inputs), 2)]
+        values = [self.input(i).payload for i in range(1, len(self.inputs), 2)]
 
         for i in range(len(var_names)):
             self.set_var_val(var_names[i], values[i])
 
     def get_state(self):
         return {'num vars': self.num_vars}
 
     def set_state(self, data, version):
         self.num_vars = data['num vars']
 
 
-export_nodes(
+export_nodes([
     SetVar_Node,
     GetVar_Node,
     Val_Node,
     Result_Node,
-    SetVarsPassive_Node,
-)
+    SetVarsPassive_Node
+])
```

### Comparing `ryven-3.1.1/ryven/resources/fonts/asap/Asap-Bold.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/asap/Asap-BoldItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/asap/Asap-Italic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/asap/Asap-Medium.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/asap/Asap-MediumItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/asap/Asap-Regular.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/asap/Asap-SemiBold.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/asap/OFL.txt` & `ryven-3.4.0a1/ryven/resources/fonts/asap/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/OFL.txt` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Black.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Bold.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Italic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Light.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Medium.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Regular.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-Thin.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/OFL.txt` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf` & `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/pics/Ryven_icon.png` & `ryven-3.4.0a1/ryven/resources/pics/Ryven_icon.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/pics/Ryven_icon_blurred.png` & `ryven-3.4.0a1/ryven/resources/pics/Ryven_icon_blurred.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/pics/logo.png` & `ryven-3.4.0a1/ryven/resources/pics/logo.png`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/branch-closed.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-closed.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/branch-end.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-end.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/branch-more.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-more.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/branch-open.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-open.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/checkbox_checked.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/checkbox_unchecked.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/close.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/downarrow.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/downarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/downarrow2.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/downarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/float.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/float.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/leftarrow.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/leftarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/leftarrow2.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/leftarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/base.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/base.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/branch-closed.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-closed.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/branch-end.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-end.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/branch-more.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-more.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/branch-open.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-open.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/close.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/downarrow.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/downarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/downarrow2.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/downarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/float.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/float.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/leftarrow.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/leftarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/leftarrow2.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/leftarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/rightarrow.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/rightarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/rightarrow2.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/rightarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/sizegrip.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/sizegrip.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/slider.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/slider.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/tab_close.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/tab_close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/uparrow.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/uparrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/uparrow2.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/uparrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/orig/vline.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/vline.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/radiobutton_checked.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/radiobutton_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/rightarrow.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/rightarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/rightarrow2.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/rightarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/sizegrip.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/sizegrip.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/slider.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/slider.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/splitter-horizontal.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/splitter-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/splitter-vertical.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/splitter-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/tab_close.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/tab_close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/uparrow.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/uparrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/uparrow2.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/uparrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/icons/vline.svg` & `ryven-3.4.0a1/ryven/resources/stylesheets/icons/vline.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/resources/stylesheets/style_template.css` & `ryven-3.4.0a1/ryven/resources/stylesheets/style_template.css`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/unused/EditVal_Dialog.py` & `ryven-3.4.0a1/ryven/unused/EditVal_Dialog.py`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/unused/NodeDetailsWidget.py` & `ryven-3.4.0a1/ryven/unused/NodeDetailsWidget.py`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/unused/NodesTreeListWidget.py` & `ryven-3.4.0a1/ryven/unused/NodesTreeListWidget.py`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven/unused/test.stl` & `ryven-3.4.0a1/ryven/unused/test.stl`

 * *Files identical despite different names*

### Comparing `ryven-3.1.1/ryven.egg-info/SOURCES.txt` & `ryven-3.4.0a1/ryven.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,71 +23,77 @@
 docs/node tutorials/README.md
 docs/node tutorials/basic operators.md
 docs/node tutorials/doc_examples/custom_widgets/nodes.py
 docs/node tutorials/doc_examples/custom_widgets/widgets.py
 docs/node tutorials/doc_examples/mypackage/nodes.py
 docs/node tutorials/img/plus.png
 docs/node tutorials/img/plus2.png
-ryven/NENV.py
-ryven/NWENV.py
 ryven/__init__.py
+ryven/gui_env.py
+ryven/node_env.py
 ryven.egg-info/PKG-INFO
 ryven.egg-info/SOURCES.txt
 ryven.egg-info/dependency_links.txt
 ryven.egg-info/entry_points.txt
 ryven.egg-info/requires.txt
 ryven.egg-info/top_level.txt
+ryven/example_nodes/OpenCV/README.md
 ryven/example_nodes/OpenCV/nodes.py
 ryven/example_nodes/OpenCV/widgets.py
-ryven/example_nodes/auto_generated/autogen.py
-ryven/example_nodes/linalg/matrix_widget.py
+ryven/example_nodes/linalg/README.md
+ryven/example_nodes/linalg/gui.py
 ryven/example_nodes/linalg/nodes.py
-ryven/example_nodes/linalg/widgets.py
+ryven/example_nodes/std/README.md
 ryven/example_nodes/std/basic_operators.py
 ryven/example_nodes/std/control_structures.py
+ryven/example_nodes/std/gui.py
 ryven/example_nodes/std/nodes.py
 ryven/example_nodes/std/special_nodes.py
-ryven/example_nodes/std/widgets.py
 ryven/examples_projects/basics.json
+ryven/examples_projects/basics_OLD.json
 ryven/examples_projects/matrices.json
+ryven/examples_projects/matrices_OLD.json
 ryven/gui/__init__.py
 ryven/gui/dialogs.py
+ryven/gui/flow_ui.py
 ryven/gui/main_console.py
 ryven/gui/main_window.py
-ryven/gui/script_UI.py
+ryven/gui/std_input_widgets.py
 ryven/gui/code_editor/CodeEditorWidget.py
 ryven/gui/code_editor/CodePreviewWidget.py
 ryven/gui/code_editor/EditSrcCodeInfoDialog.py
 ryven/gui/code_editor/SourceCodeUpdater.py
 ryven/gui/code_editor/__init__.py
+ryven/gui/code_editor/codes_storage.py
 ryven/gui/code_editor/pygments/__init__.py
 ryven/gui/code_editor/pygments/dracula.py
 ryven/gui/code_editor/pygments/light.py
-ryven/gui/startup_dialog/SelectPackages_Dialog.py
 ryven/gui/startup_dialog/StartupDialog.py
 ryven/gui/startup_dialog/__init__.py
 ryven/gui/styling/__init__.py
 ryven/gui/styling/design_config.json
 ryven/gui/styling/window_theme.py
 ryven/gui/uic/__init__.py
+ryven/gui/uic/flow.ui
 ryven/gui/uic/main_window.ui
-ryven/gui/uic/script.ui
+ryven/gui/uic/ui_flow.py
 ryven/gui/uic/ui_main_window.py
-ryven/gui/uic/ui_script.py
-ryven/gui/uic/w_ui_script.py
 ryven/main/Ryven.py
 ryven/main/RyvenConsole.py
 ryven/main/__init__.py
-ryven/main/nodes_package.py
+ryven/main/args_parser.py
+ryven/main/config.py
 ryven/main/utils.py
-ryven/main/nodes/NodeBase.py
-ryven/main/nodes/__init__.py
-ryven/main/nodes/built_in/__init__.py
-ryven/main/nodes/built_in/nodes.py
-ryven/main/nodes/built_in/widgets.py
+ryven/main/packages/__init__.py
+ryven/main/packages/gui_env.py
+ryven/main/packages/node_env.py
+ryven/main/packages/nodes_package.py
+ryven/main/packages/built_in/__init__.py
+ryven/main/packages/built_in/gui.py
+ryven/main/packages/built_in/nodes.py
 ryven/resources/fonts/__init__.py
 ryven/resources/fonts/asap/Asap-Bold.ttf
 ryven/resources/fonts/asap/Asap-BoldItalic.ttf
 ryven/resources/fonts/asap/Asap-Italic.ttf
 ryven/resources/fonts/asap/Asap-Medium.ttf
 ryven/resources/fonts/asap/Asap-MediumItalic.ttf
 ryven/resources/fonts/asap/Asap-Regular.ttf
@@ -127,14 +133,15 @@
 ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
 ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
 ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
 ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
 ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
 ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
 ryven/resources/fonts/source_code_pro/__init__.py
+ryven/resources/pics/Ryven_icon.jpg
 ryven/resources/pics/Ryven_icon.png
 ryven/resources/pics/Ryven_icon_blurred.png
 ryven/resources/pics/logo.png
 ryven/resources/stylesheets/style_template.css
 ryven/resources/stylesheets/icons/branch-closed.svg
 ryven/resources/stylesheets/icons/branch-end.svg
 ryven/resources/stylesheets/icons/branch-more.svg
```

### Comparing `ryven-3.1.1/setup.cfg` & `ryven-3.4.0a1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [metadata]
 name = ryven
-version = v3.1.1
+version = 3.4.0a1
 author = Leon Thomm
 author_email = l.thomm@mailbox.org
 description = Flow-based visual scripting for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
-license_file = LICENSE
+license_files = 
+	LICENSE
 url = https://github.com/leon-thomm/Ryven
 project_urls = 
 	Website = https://ryven.org
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.6, !=3.10
 install_requires = 
-	ryvencore-qt ==0.3.1.*
-	ryvencore ==0.3.1.*
+	ryvencore-qt ==0.4.*
+	ryvencore ==0.4.*
 	Jinja2
 	Pygments
 	textdistance
+	packaging
 
 [options.entry_points]
 console_scripts = 
 	ryven = ryven:run_ryven
-	ryven_console = ryven:run_ryven_console
+	ryven-console = ryven:run_ryven_console
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

