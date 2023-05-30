# Comparing `tmp/ryven-3.4.0a1.tar.gz` & `tmp/ryven-3.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryven-3.4.0a1.tar", last modified: Mon May 29 23:21:23 2023, max compression
+gzip compressed data, was "ryven-3.4.0a2.tar", last modified: Tue May 30 08:12:06 2023, max compression
```

## Comparing `ryven-3.4.0a1.tar` & `ryven-3.4.0a2.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.488635 ryven-3.4.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-29 23:21:11.000000 ryven-3.4.0a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 23:21:11.000000 ryven-3.4.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-29 23:21:11.000000 ryven-3.4.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-29 23:21:23.488635 ryven-3.4.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-05-29 23:21:11.000000 ryven-3.4.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.424635 ryven-3.4.0a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    50881 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/stylus.png
--rw-r--r--   0 runner    (1001) docker     (123)    89262 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/stylus_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    85860 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/stylus_light.png
--rw-r--r--   0 runner    (1001) docker     (123)    95421 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_blender.png
--rw-r--r--   0 runner    (1001) docker     (123)    81063 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_ghost.png
--rw-r--r--   0 runner    (1001) docker     (123)  1698942 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_merged.png
--rw-r--r--   0 runner    (1001) docker     (123)    98584 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_samuel1d.png
--rw-r--r--   0 runner    (1001) docker     (123)    95033 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_samuel1l.png
--rw-r--r--   0 runner    (1001) docker     (123)   135784 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_samuel2d.png
--rw-r--r--   0 runner    (1001) docker     (123)    93157 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_simple.png
--rw-r--r--   0 runner    (1001) docker     (123)   257602 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_toy.png
--rw-r--r--   0 runner    (1001) docker     (123)   134657 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_tron.png
--rw-r--r--   0 runner    (1001) docker     (123)   109586 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_1_ueli.png
--rw-r--r--   0 runner    (1001) docker     (123)   574949 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/img/themes_with_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/docs/node tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/basic operators.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.424635 ryven-3.4.0a1/docs/node tutorials/doc_examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/docs/node tutorials/doc_examples/custom_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/doc_examples/custom_widgets/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/doc_examples/custom_widgets/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/docs/node tutorials/doc_examples/mypackage/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/doc_examples/mypackage/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/docs/node tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (123)    21267 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/img/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)    28080 2023-05-29 23:21:11.000000 ryven-3.4.0a1/docs/node tutorials/img/plus2.png
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-29 23:21:11.000000 ryven-3.4.0a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.440635 ryven-3.4.0a1/ryven/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.428635 ryven-3.4.0a1/ryven/example_nodes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.444635 ryven-3.4.0a1/ryven/example_nodes/OpenCV/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/OpenCV/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    37537 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/OpenCV/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/OpenCV/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.444635 ryven-3.4.0a1/ryven/example_nodes/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/linalg/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/linalg/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/linalg/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.444635 ryven-3.4.0a1/ryven/example_nodes/std/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/basic_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/control_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17061 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/example_nodes/std/special_nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.444635 ryven-3.4.0a1/ryven/examples_projects/
--rw-r--r--   0 runner    (1001) docker     (123)    63369 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/examples_projects/basics.json
--rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/examples_projects/basics_OLD.json
--rw-r--r--   0 runner    (1001) docker     (123)    40944 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/examples_projects/matrices.json
--rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/examples_projects/matrices_OLD.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.448635 ryven-3.4.0a1/ryven/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.448635 ryven-3.4.0a1/ryven/gui/code_editor/
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/CodeEditorWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/CodePreviewWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/EditSrcCodeInfoDialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/SourceCodeUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/codes_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.448635 ryven-3.4.0a1/ryven/gui/code_editor/pygments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/pygments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/pygments/dracula.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/code_editor/pygments/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/flow_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/main_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/main_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.448635 ryven-3.4.0a1/ryven/gui/startup_dialog/
--rw-r--r--   0 runner    (1001) docker     (123)    27615 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/startup_dialog/StartupDialog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/startup_dialog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/std_input_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.448635 ryven-3.4.0a1/ryven/gui/styling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/styling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/styling/design_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/styling/window_theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.452635 ryven-3.4.0a1/ryven/gui/uic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/uic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/uic/flow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/uic/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/uic/ui_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui/uic/ui_main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/gui_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.452635 ryven-3.4.0a1/ryven/main/
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/Ryven.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/RyvenConsole.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.452635 ryven-3.4.0a1/ryven/main/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.452635 ryven-3.4.0a1/ryven/main/packages/built_in/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/built_in/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/built_in/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/built_in/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/gui_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/node_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/packages/nodes_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/main/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/node_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.432635 ryven-3.4.0a1/ryven/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.452635 ryven-3.4.0a1/ryven/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.456635 ryven-3.4.0a1/ryven/resources/fonts/asap/
--rw-r--r--   0 runner    (1001) docker     (123)   102416 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   111664 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   109800 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   102444 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   111808 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   101032 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   102688 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   112712 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/asap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.464635 ryven-3.4.0a1/ryven/resources/fonts/poppins/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)   138520 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155420 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   140724 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   159688 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   139684 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158172 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   147416 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   170376 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   166604 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   145936 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   168408 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   142980 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   164976 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   144776 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   148440 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171772 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/poppins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.472635 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)   191284 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155056 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   191568 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155288 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   193360 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156884 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161376 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   193160 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156984 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   191984 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156156 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   192740 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   191792 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155568 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.472635 ryven-3.4.0a1/ryven/resources/pics/
--rw-r--r--   0 runner    (1001) docker     (123)    61897 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/pics/Ryven_icon.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   391573 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/pics/Ryven_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   786058 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/pics/Ryven_icon_blurred.png
--rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/pics/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.472635 ryven-3.4.0a1/ryven/resources/stylesheets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.480635 ryven-3.4.0a1/ryven/resources/stylesheets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-closed.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-end.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-more.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-open.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/downarrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/downarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/float.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/leftarrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/leftarrow2.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.488635 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/base.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-closed.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-end.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-more.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-open.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/downarrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/downarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/float.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/leftarrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/leftarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/rightarrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/rightarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/slider.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/tab_close.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/uparrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/uparrow2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/vline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/radiobutton_checked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/rightarrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/rightarrow2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/sizegrip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/slider.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/splitter-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/splitter-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/tab_close.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/uparrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/uparrow2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/icons/vline.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/resources/stylesheets/style_template.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.488635 ryven-3.4.0a1/ryven/unused/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/unused/EditVal_Dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/unused/NodeDetailsWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/unused/NodesTreeListWidget.py
--rw-r--r--   0 runner    (1001) docker     (123)   574832 2023-05-29 23:21:11.000000 ryven-3.4.0a1/ryven/unused/test.stl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:21:23.444635 ryven-3.4.0a1/ryven.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 23:21:23.000000 ryven-3.4.0a1/ryven.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-29 23:21:23.488635 ryven-3.4.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-29 23:21:11.000000 ryven-3.4.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.549633 ryven-3.4.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-30 08:11:54.000000 ryven-3.4.0a2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 08:11:54.000000 ryven-3.4.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-30 08:11:54.000000 ryven-3.4.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-30 08:12:06.549633 ryven-3.4.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-05-30 08:11:54.000000 ryven-3.4.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.477632 ryven-3.4.0a2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.489632 ryven-3.4.0a2/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50881 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/stylus.png
+-rw-r--r--   0 runner    (1001) docker     (123)    89262 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/stylus_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85860 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/stylus_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95421 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_1_blender.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81063 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_1_ghost.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1698942 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_1_merged.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98584 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_1_samuel1d.png
+-rw-r--r--   0 runner    (1001) docker     (123)    95033 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_1_samuel1l.png
+-rw-r--r--   0 runner    (1001) docker     (123)   135784 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_1_samuel2d.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93157 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_1_simple.png
+-rw-r--r--   0 runner    (1001) docker     (123)   257602 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_1_toy.png
+-rw-r--r--   0 runner    (1001) docker     (123)   134657 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_1_tron.png
+-rw-r--r--   0 runner    (1001) docker     (123)   109586 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_1_ueli.png
+-rw-r--r--   0 runner    (1001) docker     (123)   574949 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/img/themes_with_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.493632 ryven-3.4.0a2/docs/node tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/node tutorials/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/node tutorials/basic operators.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.477632 ryven-3.4.0a2/docs/node tutorials/doc_examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.493632 ryven-3.4.0a2/docs/node tutorials/doc_examples/custom_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/node tutorials/doc_examples/custom_widgets/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/node tutorials/doc_examples/custom_widgets/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.493632 ryven-3.4.0a2/docs/node tutorials/doc_examples/mypackage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/node tutorials/doc_examples/mypackage/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.493632 ryven-3.4.0a2/docs/node tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    21267 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/node tutorials/img/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28080 2023-05-30 08:11:54.000000 ryven-3.4.0a2/docs/node tutorials/img/plus2.png
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-30 08:11:54.000000 ryven-3.4.0a2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.493632 ryven-3.4.0a2/ryven/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.481632 ryven-3.4.0a2/ryven/example_nodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.497632 ryven-3.4.0a2/ryven/example_nodes/OpenCV/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/OpenCV/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    37537 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/OpenCV/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/OpenCV/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.497632 ryven-3.4.0a2/ryven/example_nodes/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/linalg/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/linalg/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/linalg/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.497632 ryven-3.4.0a2/ryven/example_nodes/std/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/std/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/std/basic_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/std/control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/std/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/std/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17061 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/example_nodes/std/special_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.497632 ryven-3.4.0a2/ryven/examples_projects/
+-rw-r--r--   0 runner    (1001) docker     (123)    63369 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/examples_projects/basics.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29976 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/examples_projects/basics_OLD.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40944 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/examples_projects/matrices.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26900 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/examples_projects/matrices_OLD.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.501632 ryven-3.4.0a2/ryven/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.501632 ryven-3.4.0a2/ryven/gui/code_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/code_editor/CodeEditorWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/code_editor/CodePreviewWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/code_editor/EditSrcCodeInfoDialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/code_editor/SourceCodeUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/code_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/code_editor/codes_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.501632 ryven-3.4.0a2/ryven/gui/code_editor/pygments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/code_editor/pygments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/code_editor/pygments/dracula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/code_editor/pygments/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/flow_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/main_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16332 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/main_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.501632 ryven-3.4.0a2/ryven/gui/startup_dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)    27615 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/startup_dialog/StartupDialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/startup_dialog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/std_input_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.501632 ryven-3.4.0a2/ryven/gui/styling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/styling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/styling/design_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/styling/window_theme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.505632 ryven-3.4.0a2/ryven/gui/uic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/uic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/uic/flow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/uic/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/uic/ui_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10872 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui/uic/ui_main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/gui_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.505632 ryven-3.4.0a2/ryven/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/Ryven.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/RyvenConsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.505632 ryven-3.4.0a2/ryven/main/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.505632 ryven-3.4.0a2/ryven/main/packages/built_in/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/packages/built_in/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/packages/built_in/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/packages/built_in/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/packages/gui_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/packages/node_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/packages/nodes_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/main/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/node_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.481632 ryven-3.4.0a2/ryven/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.505632 ryven-3.4.0a2/ryven/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.509632 ryven-3.4.0a2/ryven/resources/fonts/asap/
+-rw-r--r--   0 runner    (1001) docker     (123)   102416 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111664 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   109800 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   102444 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111808 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   101032 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   102688 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112712 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/asap/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/asap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.517632 ryven-3.4.0a2/ryven/resources/fonts/poppins/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   138520 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155420 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   140724 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159688 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   139684 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158172 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   147416 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   170376 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   166604 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   145936 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   168408 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   142980 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   164976 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   144776 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   148440 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171772 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/poppins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.525632 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   191284 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155056 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   191568 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155288 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193360 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156884 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161376 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193160 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156984 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   191984 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156156 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   192740 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   191792 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155568 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.529632 ryven-3.4.0a2/ryven/resources/pics/
+-rw-r--r--   0 runner    (1001) docker     (123)    61897 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/pics/Ryven_icon.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   391573 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/pics/Ryven_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   786058 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/pics/Ryven_icon_blurred.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46855 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/pics/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.529632 ryven-3.4.0a2/ryven/resources/stylesheets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.537632 ryven-3.4.0a2/ryven/resources/stylesheets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/branch-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/branch-end.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/branch-more.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/branch-open.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/downarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/downarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/float.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/leftarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/leftarrow2.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.549633 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/base.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/branch-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/branch-end.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/branch-more.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/branch-open.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/downarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/downarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/float.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/leftarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/leftarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/rightarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/rightarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/slider.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/tab_close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/uparrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/uparrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/vline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/radiobutton_checked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/rightarrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/rightarrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/sizegrip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/slider.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/splitter-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/splitter-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/tab_close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/uparrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/uparrow2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/icons/vline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/resources/stylesheets/style_template.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.549633 ryven-3.4.0a2/ryven/unused/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/unused/EditVal_Dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/unused/NodeDetailsWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/unused/NodesTreeListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)   574832 2023-05-30 08:11:54.000000 ryven-3.4.0a2/ryven/unused/test.stl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:12:06.493632 ryven-3.4.0a2/ryven.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-05-30 08:12:06.000000 ryven-3.4.0a2/ryven.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-05-30 08:12:06.000000 ryven-3.4.0a2/ryven.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:12:06.000000 ryven-3.4.0a2/ryven.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-30 08:12:06.000000 ryven-3.4.0a2/ryven.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 08:12:06.000000 ryven-3.4.0a2/ryven.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 08:12:06.000000 ryven-3.4.0a2/ryven.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-30 08:12:06.549633 ryven-3.4.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-30 08:11:54.000000 ryven-3.4.0a2/setup.py
```

### Comparing `ryven-3.4.0a1/CONTRIBUTING.md` & `ryven-3.4.0a2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/LICENSE` & `ryven-3.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/PKG-INFO` & `ryven-3.4.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryven
-Version: 3.4.0a1
+Version: 3.4.0a2
 Summary: Flow-based visual scripting for Python
 Home-page: https://github.com/leon-thomm/Ryven
 Author: Leon Thomm
 Author-email: l.thomm@mailbox.org
 Project-URL: Website, https://ryven.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ryven-3.4.0a1/README.md` & `ryven-3.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/logo.png` & `ryven-3.4.0a2/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/stylus.png` & `ryven-3.4.0a2/docs/img/stylus.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/stylus_dark.png` & `ryven-3.4.0a2/docs/img/stylus_dark.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/stylus_light.png` & `ryven-3.4.0a2/docs/img/stylus_light.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_1_blender.png` & `ryven-3.4.0a2/docs/img/themes_1_blender.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_1_ghost.png` & `ryven-3.4.0a2/docs/img/themes_1_ghost.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_1_merged.png` & `ryven-3.4.0a2/docs/img/themes_1_merged.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_1_samuel1d.png` & `ryven-3.4.0a2/docs/img/themes_1_samuel1d.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_1_samuel1l.png` & `ryven-3.4.0a2/docs/img/themes_1_samuel1l.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_1_samuel2d.png` & `ryven-3.4.0a2/docs/img/themes_1_samuel2d.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_1_simple.png` & `ryven-3.4.0a2/docs/img/themes_1_simple.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_1_toy.png` & `ryven-3.4.0a2/docs/img/themes_1_toy.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_1_tron.png` & `ryven-3.4.0a2/docs/img/themes_1_tron.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_1_ueli.png` & `ryven-3.4.0a2/docs/img/themes_1_ueli.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/img/themes_with_logo.png` & `ryven-3.4.0a2/docs/img/themes_with_logo.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/node tutorials/basic operators.md` & `ryven-3.4.0a2/docs/node tutorials/basic operators.md`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/node tutorials/doc_examples/custom_widgets/nodes.py` & `ryven-3.4.0a2/docs/node tutorials/doc_examples/custom_widgets/nodes.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/node tutorials/doc_examples/custom_widgets/widgets.py` & `ryven-3.4.0a2/docs/node tutorials/doc_examples/custom_widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/node tutorials/doc_examples/mypackage/nodes.py` & `ryven-3.4.0a2/docs/node tutorials/doc_examples/mypackage/nodes.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/node tutorials/img/plus.png` & `ryven-3.4.0a2/docs/node tutorials/img/plus.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/docs/node tutorials/img/plus2.png` & `ryven-3.4.0a2/docs/node tutorials/img/plus2.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/example_nodes/OpenCV/nodes.py` & `ryven-3.4.0a2/ryven/example_nodes/OpenCV/nodes.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/example_nodes/OpenCV/widgets.py` & `ryven-3.4.0a2/ryven/example_nodes/OpenCV/widgets.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/example_nodes/linalg/gui.py` & `ryven-3.4.0a2/ryven/example_nodes/linalg/gui.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/example_nodes/linalg/nodes.py` & `ryven-3.4.0a2/ryven/example_nodes/linalg/nodes.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/example_nodes/std/basic_operators.py` & `ryven-3.4.0a2/ryven/example_nodes/std/basic_operators.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/example_nodes/std/control_structures.py` & `ryven-3.4.0a2/ryven/example_nodes/std/control_structures.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/example_nodes/std/gui.py` & `ryven-3.4.0a2/ryven/example_nodes/std/gui.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/example_nodes/std/special_nodes.py` & `ryven-3.4.0a2/ryven/example_nodes/std/special_nodes.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/examples_projects/basics.json` & `ryven-3.4.0a2/ryven/examples_projects/basics.json`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/examples_projects/basics_OLD.json` & `ryven-3.4.0a2/ryven/examples_projects/basics_OLD.json`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/examples_projects/matrices.json` & `ryven-3.4.0a2/ryven/examples_projects/matrices.json`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/examples_projects/matrices_OLD.json` & `ryven-3.4.0a2/ryven/examples_projects/matrices_OLD.json`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/code_editor/CodeEditorWidget.py` & `ryven-3.4.0a2/ryven/gui/code_editor/CodeEditorWidget.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/code_editor/CodePreviewWidget.py` & `ryven-3.4.0a2/ryven/gui/code_editor/CodePreviewWidget.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/code_editor/EditSrcCodeInfoDialog.py` & `ryven-3.4.0a2/ryven/gui/code_editor/EditSrcCodeInfoDialog.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/code_editor/SourceCodeUpdater.py` & `ryven-3.4.0a2/ryven/gui/code_editor/SourceCodeUpdater.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/code_editor/codes_storage.py` & `ryven-3.4.0a2/ryven/gui/code_editor/codes_storage.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/code_editor/pygments/dracula.py` & `ryven-3.4.0a2/ryven/gui/code_editor/pygments/dracula.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/dialogs.py` & `ryven-3.4.0a2/ryven/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/flow_ui.py` & `ryven-3.4.0a2/ryven/gui/flow_ui.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/main_console.py` & `ryven-3.4.0a2/ryven/gui/main_console.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/main_window.py` & `ryven-3.4.0a2/ryven/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/startup_dialog/StartupDialog.py` & `ryven-3.4.0a2/ryven/gui/startup_dialog/StartupDialog.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/std_input_widgets.py` & `ryven-3.4.0a2/ryven/gui/std_input_widgets.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/styling/design_config.json` & `ryven-3.4.0a2/ryven/gui/styling/design_config.json`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/styling/window_theme.py` & `ryven-3.4.0a2/ryven/gui/styling/window_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from qtpy.QtWidgets import QApplication
 from ryven.main.utils import abs_path_from_package_dir
 
 
 def hex_to_rgb(hex: str):
     if hex is None:
         return None
     else:
@@ -79,14 +78,15 @@
         'danger': None,
         'warning': None,
         'success': None,
     }
 
 
 def apply_stylesheet(style: str):
+    from qtpy.QtWidgets import QApplication
 
     # set to None if not used
     icons_dir = abs_path_from_package_dir('resources/stylesheets/icons')
     if icons_dir is not None:
         from qtpy.QtCore import QDir
         d = QDir()
         d.setSearchPaths('icon', [icons_dir])
```

### Comparing `ryven-3.4.0a1/ryven/gui/uic/flow.ui` & `ryven-3.4.0a2/ryven/gui/uic/flow.ui`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/uic/main_window.ui` & `ryven-3.4.0a2/ryven/gui/uic/main_window.ui`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/uic/ui_flow.py` & `ryven-3.4.0a2/ryven/gui/uic/ui_flow.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/gui/uic/ui_main_window.py` & `ryven-3.4.0a2/ryven/gui/uic/ui_main_window.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/main/Ryven.py` & `ryven-3.4.0a2/ryven/main/Ryven.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import os
 import sys
 
 import ryven.main.packages.nodes_package
 from ryven.main import utils
 from ryven.main.config import Config
-from ryven.node_env import init_node_env
-from ryven.gui_env import init_node_guis_env
 from ryven.main.args_parser import process_args
 
 
 def run(*args_,
         qt_app=None, gui_parent=None, use_sysargs=True,
         **kwargs):
     """Start the Ryven window.
@@ -62,14 +60,17 @@
         the wrong number of positional arguments are specified.
 
     Returns
     -------
     None|Main Window
     """
 
+    from ryven.node_env import init_node_env
+    from ryven.gui_env import init_node_guis_env    # Qt dependency
+
     # Process command line and method's arguments
     conf: Config = process_args(use_sysargs, *args_, **kwargs)
 
     #
     # Qt application setup
     #
```

### Comparing `ryven-3.4.0a1/ryven/main/RyvenConsole.py` & `ryven-3.4.0a2/ryven/main/RyvenConsole.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/main/args_parser.py` & `ryven-3.4.0a2/ryven/main/args_parser.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/main/config.py` & `ryven-3.4.0a2/ryven/main/config.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/main/packages/built_in/gui.py` & `ryven-3.4.0a2/ryven/main/packages/built_in/gui.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/main/packages/built_in/nodes.py` & `ryven-3.4.0a2/ryven/main/packages/built_in/nodes.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/main/packages/gui_env.py` & `ryven-3.4.0a2/ryven/main/packages/gui_env.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/main/packages/node_env.py` & `ryven-3.4.0a2/ryven/main/packages/node_env.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/main/packages/nodes_package.py` & `ryven-3.4.0a2/ryven/main/packages/nodes_package.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/main/utils.py` & `ryven-3.4.0a2/ryven/main/utils.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Bold.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-BoldItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Italic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Medium.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-MediumItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-Regular.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-SemiBold.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/asap/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/asap/OFL.txt` & `ryven-3.4.0a2/ryven/resources/fonts/asap/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/OFL.txt` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Black.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Bold.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Italic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Light.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Medium.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Regular.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-Thin.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/poppins/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/OFL.txt` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Black.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Light.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf` & `ryven-3.4.0a2/ryven/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/pics/Ryven_icon.jpg` & `ryven-3.4.0a2/ryven/resources/pics/Ryven_icon.jpg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/pics/Ryven_icon.png` & `ryven-3.4.0a2/ryven/resources/pics/Ryven_icon.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/pics/Ryven_icon_blurred.png` & `ryven-3.4.0a2/ryven/resources/pics/Ryven_icon_blurred.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/pics/logo.png` & `ryven-3.4.0a2/ryven/resources/pics/logo.png`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-closed.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/branch-closed.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-end.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/branch-end.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-more.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/branch-more.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/branch-open.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/branch-open.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_checked.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/checkbox_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/checkbox_indeterminate.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/checkbox_unchecked.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/checkbox_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/close.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/downarrow.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/downarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/downarrow2.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/downarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/float.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/float.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/leftarrow.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/leftarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/leftarrow2.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/leftarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/base.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/base.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-closed.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/branch-closed.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-end.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/branch-end.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-more.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/branch-more.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/branch-open.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/branch-open.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/checkbox_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/checkbox_indeterminate.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/checkbox_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/close.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/downarrow.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/downarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/downarrow2.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/downarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/float.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/float.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/leftarrow.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/leftarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/leftarrow2.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/leftarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/radiobutton_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/radiobutton_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/rightarrow.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/rightarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/rightarrow2.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/rightarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/sizegrip.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/sizegrip.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/slider.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/slider.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/splitter-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/splitter-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/tab_close.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/tab_close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/toolbar-handle-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/toolbar-handle-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/uparrow.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/uparrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/uparrow2.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/uparrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/orig/vline.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/orig/vline.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/radiobutton_checked.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/radiobutton_checked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/radiobutton_unchecked.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/rightarrow.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/rightarrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/rightarrow2.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/rightarrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/sizegrip.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/sizegrip.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/slider.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/slider.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/splitter-horizontal.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/splitter-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/splitter-vertical.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/splitter-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/tab_close.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/tab_close.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/toolbar-handle-horizontal.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/toolbar-handle-vertical.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/uparrow.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/uparrow.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/uparrow2.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/uparrow2.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/icons/vline.svg` & `ryven-3.4.0a2/ryven/resources/stylesheets/icons/vline.svg`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/resources/stylesheets/style_template.css` & `ryven-3.4.0a2/ryven/resources/stylesheets/style_template.css`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/unused/EditVal_Dialog.py` & `ryven-3.4.0a2/ryven/unused/EditVal_Dialog.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/unused/NodeDetailsWidget.py` & `ryven-3.4.0a2/ryven/unused/NodeDetailsWidget.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/unused/NodesTreeListWidget.py` & `ryven-3.4.0a2/ryven/unused/NodesTreeListWidget.py`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven/unused/test.stl` & `ryven-3.4.0a2/ryven/unused/test.stl`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/ryven.egg-info/PKG-INFO` & `ryven-3.4.0a2/ryven.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryven
-Version: 3.4.0a1
+Version: 3.4.0a2
 Summary: Flow-based visual scripting for Python
 Home-page: https://github.com/leon-thomm/Ryven
 Author: Leon Thomm
 Author-email: l.thomm@mailbox.org
 Project-URL: Website, https://ryven.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ryven-3.4.0a1/ryven.egg-info/SOURCES.txt` & `ryven-3.4.0a2/ryven.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryven-3.4.0a1/setup.cfg` & `ryven-3.4.0a2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ryven
-version = 3.4.0a1
+version = 3.4.0a2
 author = Leon Thomm
 author_email = l.thomm@mailbox.org
 description = Flow-based visual scripting for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = 
 	LICENSE
```

### Comparing `ryven-3.4.0a1/setup.py` & `ryven-3.4.0a2/setup.py`

 * *Files identical despite different names*

