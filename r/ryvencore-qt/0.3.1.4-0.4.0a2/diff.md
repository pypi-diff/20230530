# Comparing `tmp/ryvencore-qt-0.3.1.4.tar.gz` & `tmp/ryvencore-qt-0.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryvencore-qt-0.3.1.4.tar", last modified: Mon Oct  3 01:29:24 2022, max compression
+gzip compressed data, was "ryvencore-qt-0.4.0a2.tar", last modified: Mon May 29 23:18:07 2023, max compression
```

## Comparing `ryvencore-qt-0.3.1.4.tar` & `ryvencore-qt-0.4.0a2.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.120111 ryvencore-qt-0.3.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)    26526 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5120 2022-10-03 01:29:24.120111 ryvencore-qt-0.3.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4561 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.100111 ryvencore-qt-0.3.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (121)    16888 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.100111 ryvencore-qt-0.3.1.4/docs/img/
--rw-r--r--   0 runner    (1001) docker     (121)    39205 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/img/function_node.png
--rw-r--r--   0 runner    (1001) docker     (121)    80217 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/img/logic_editor_screenshot1.png
--rw-r--r--   0 runner    (1001) docker     (121)    93408 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/img/logic_editor_screenshot2.png
--rw-r--r--   0 runner    (1001) docker     (121)   110773 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/img/logic_editor_screenshot3.png
--rw-r--r--   0 runner    (1001) docker     (121)    71305 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    26535 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/img/macro.png
--rw-r--r--   0 runner    (1001) docker     (121)    50000 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/img/macro2.png
--rw-r--r--   0 runner    (1001) docker     (121)  1179406 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/img/ryvencore-drawio_.png
--rw-r--r--   0 runner    (1001) docker     (121)    94645 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/img/ryvencore_screenshot1.png
--rw-r--r--   0 runner    (1001) docker     (121)    85860 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/img/stylus_light.png
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.104111 ryvencore-qt-0.3.1.4/docs/unused/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/unused/_sidebar.md
--rw-r--r--   0 runner    (1001) docker     (121)    24147 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/unused/api.md
--rw-r--r--   0 runner    (1001) docker     (121)    16088 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/unused/features.md
--rw-r--r--   0 runner    (1001) docker     (121)    16369 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/unused/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (121)     3391 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/unused/gui.md
--rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/docs/unused/threading.md
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.104111 ryvencore-qt-0.3.1.4/ryvencore_qt/
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.104111 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.104111 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.104111 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/
--rw-r--r--   0 runner    (1001) docker     (121)   102416 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   111664 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   109800 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   102444 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   111808 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   101032 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   102688 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   112712 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.108111 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/
--rw-r--r--   0 runner    (1001) docker     (121)     4372 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (121)   138520 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   155420 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   140724 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   159688 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   139684 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   158172 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   147416 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   170376 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   166604 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   145936 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   168408 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   142980 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   164976 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   144776 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   141612 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   161360 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   148440 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   171772 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.112111 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/
--rw-r--r--   0 runner    (1001) docker     (121)     4528 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (121)   191284 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   155056 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   191568 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   155288 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   193360 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   156884 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   161376 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   193160 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   156984 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   191984 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   156156 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   192740 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   191792 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   155568 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2711 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/node_collapse_icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2708 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/node_expand_icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.116111 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25091 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/code_block_picture.png
--rw-r--r--   0 runner    (1001) docker     (121)    23985 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/code_block_picture2.png
--rw-r--r--   0 runner    (1001) docker     (121)    17618 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/code_block_picture3.png
--rw-r--r--   0 runner    (1001) docker     (121)    20454 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/function_picture.png
--rw-r--r--   0 runner    (1001) docker     (121)     5798 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/function_picture_.png
--rw-r--r--   0 runner    (1001) docker     (121)    71305 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)    19733 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/macro_icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)    86801 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/macro_node_icon.png
--rw-r--r--   0 runner    (1001) docker     (121)    20715 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/macro_script_picture.png
--rw-r--r--   0 runner    (1001) docker     (121)  2383140 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/opencv_example.png
--rw-r--r--   0 runner    (1001) docker     (121)    12682 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/script_picture.png
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/script_picture.svg
--rw-r--r--   0 runner    (1001) docker     (121)    16509 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/script_picture_old.png
--rw-r--r--   0 runner    (1001) docker     (121)    18389 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/variable_picture.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.116111 ryvencore-qt-0.3.1.4/ryvencore_qt/src/
--rw-r--r--   0 runner    (1001) docker     (121)     4705 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/Design.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/GUIBase.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/GlobalAttributes.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/RCQT.py
--rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/SessionThreadInterface.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.120111 ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/EditVal_Dialog.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/ListWidget_NameLineEdit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/LogWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     3356 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/ScriptsListWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     3625 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/ScriptsList_ScriptWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     3490 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/VariablesListWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     4406 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/VarsList_VarWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.120111 ryvencore-qt-0.3.1.4/ryvencore_qt/src/core_wrapper/
--rw-r--r--   0 runner    (1001) docker     (121)     9193 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/core_wrapper/Node.py
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/core_wrapper/Session.py
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/core_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.120111 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/
--rw-r--r--   0 runner    (1001) docker     (121)    11546 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowCommands.py
--rw-r--r--   0 runner    (1001) docker     (121)    57377 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowTheme.py
--rw-r--r--   0 runner    (1001) docker     (121)    46818 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowView.py
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowViewProxyWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     4451 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowViewStylusModesWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowViewZoomWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.120111 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/connections/
--rw-r--r--   0 runner    (1001) docker     (121)     6707 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/connections/ConnectionItem.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/connections/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.120111 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/drawings/
--rw-r--r--   0 runner    (1001) docker     (121)     8297 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/drawings/DrawingObject.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/drawings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.120111 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/node_list_widget/
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/node_list_widget/NodeListWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     3419 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/node_list_widget/NodeWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/node_list_widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/node_list_widget/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.120111 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/
--rw-r--r--   0 runner    (1001) docker     (121)    17209 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItem.py
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItemAction.py
--rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItemAnimator.py
--rw-r--r--   0 runner    (1001) docker     (121)    10520 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItemWidget.py
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItem_CollapseButton.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItem_Icon.py
--rw-r--r--   0 runner    (1001) docker     (121)     2382 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItem_TitleLabel.py
--rw-r--r--   0 runner    (1001) docker     (121)    12402 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/PortItem.py
--rw-r--r--   0 runner    (1001) docker     (121)     8682 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/PortItemInputWidgets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/WidgetBaseClasses.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6725 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/ryvencore_qt/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-03 01:29:24.104111 ryvencore-qt-0.3.1.4/ryvencore_qt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5120 2022-10-03 01:29:24.000000 ryvencore-qt-0.3.1.4/ryvencore_qt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6347 2022-10-03 01:29:24.000000 ryvencore-qt-0.3.1.4/ryvencore_qt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-03 01:29:24.000000 ryvencore-qt-0.3.1.4/ryvencore_qt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-03 01:29:24.000000 ryvencore-qt-0.3.1.4/ryvencore_qt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-03 01:29:24.000000 ryvencore-qt-0.3.1.4/ryvencore_qt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-03 01:29:24.120111 ryvencore-qt-0.3.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-03 01:29:15.000000 ryvencore-qt-0.3.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.347023 ryvencore-qt-0.4.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-29 23:18:07.347023 ryvencore-qt-0.4.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.283018 ryvencore-qt-0.4.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.287018 ryvencore-qt-0.4.0a2/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    39205 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/img/function_node.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80217 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/img/logic_editor_screenshot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93408 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/img/logic_editor_screenshot2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   110773 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/img/logic_editor_screenshot3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71305 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26535 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/img/macro.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50000 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/img/macro2.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1179406 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/img/ryvencore-drawio_.png
+-rw-r--r--   0 runner    (1001) docker     (123)    94645 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/img/ryvencore_screenshot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85860 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/img/stylus_light.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.291018 ryvencore-qt-0.4.0a2/docs/unused/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/unused/_sidebar.md
+-rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/unused/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/unused/features.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16369 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/unused/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/unused/gui.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/docs/unused/threading.md
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.291018 ryvencore-qt-0.4.0a2/ryvencore_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.291018 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.295019 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.299019 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/
+-rw-r--r--   0 runner    (1001) docker     (123)   102416 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111664 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   109800 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   102444 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111808 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   101032 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   102688 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112712 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.311020 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   138520 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155420 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   140724 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159688 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   139684 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158172 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   147416 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   170376 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   166604 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   145936 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   168408 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   142980 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   164976 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   144776 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   148440 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171772 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.319020 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   191284 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155056 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   191568 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155288 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193360 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156884 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161376 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193160 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156984 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   191984 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156156 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   192740 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   191792 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155568 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/node_collapse_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/node_expand_icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.327021 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25091 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/code_block_picture.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23985 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/code_block_picture2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17618 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/code_block_picture3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/function_picture.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/function_picture_.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71305 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/macro_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    86801 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/macro_node_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/macro_script_picture.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2383140 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/opencv_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/script_picture.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/script_picture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/script_picture_old.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18389 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/variable_picture.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41046 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/warning.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/resources/warning.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.331021 ryvencore-qt-0.4.0a2/ryvencore_qt/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/Design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/GUIBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/GlobalAttributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/RCQT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/SessionGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.335022 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58050 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowTheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46345 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowView.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowViewProxyWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowViewStylusModesWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowViewZoomWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.335022 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/connections/
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/connections/ConnectionItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/connections/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.335022 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/drawings/
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/drawings/DrawingObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/drawings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.335022 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/node_list_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/node_list_widget/NodeListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/node_list_widget/NodeWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/node_list_widget/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/node_list_widget/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.343022 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeErrorIndicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItemAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItemAnimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItemWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItem_CollapseButton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItem_Icon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItem_TitleLabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/PortItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/PortItemInputWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/WidgetBaseClasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.343022 ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/EditVal_Dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/FlowsListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/FlowsList_FlowWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/ListWidget_NameLineEdit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/LogWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/VariablesListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/VarsList_VarWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:18:07.291018 ryvencore-qt-0.4.0a2/ryvencore_qt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-29 23:18:07.000000 ryvencore-qt-0.4.0a2/ryvencore_qt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-29 23:18:07.000000 ryvencore-qt-0.4.0a2/ryvencore_qt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:18:07.000000 ryvencore-qt-0.4.0a2/ryvencore_qt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-29 23:18:07.000000 ryvencore-qt-0.4.0a2/ryvencore_qt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 23:18:07.000000 ryvencore-qt-0.4.0a2/ryvencore_qt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 23:18:07.347023 ryvencore-qt-0.4.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-29 23:17:56.000000 ryvencore-qt-0.4.0a2/setup.py
```

### Comparing `ryvencore-qt-0.3.1.4/LICENSE` & `ryvencore-qt-0.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/PKG-INFO` & `ryvencore-qt-0.4.0a2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryvencore-qt
-Version: 0.3.1.4
+Version: 0.4.0a2
 Summary: Qt frontend for ryvencore; Library for building Visual Node Editors
 Home-page: https://github.com/leon-thomm/ryvencore-qt
 Author: Leon Thomm
 Author-email: l.thomm@mailbox.org
 Project-URL: Website, https://ryven.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
@@ -14,32 +14,39 @@
 License-File: LICENSE
 
 
 <p align="center">
   <img src="./ryvencore_qt/resources/pics/logo.png" alt="drawing" width="70%"/>
 </p>
 
-`rvencore-qt` is a wrapper around [ryvencore](https://github.com/leon-thomm/ryvencore) and provides a Qt frontend for it. It comes from the [Ryven](https://github.com/leon-thomm/Ryven) project and will be the foundation for future Ryven versions. So, ryvencore-qt can be used to build cross-platform standalone visual node editors based on Python. Projects made with ryvencore-qt can be natively deployed directly on the backend, ryvencore. The development of ryvencore-qt is currently closely tied to Ryven.
+`ryvencore-qt` provides Qt-based GUI classes for [ryvencore](https://github.com/leon-thomm/ryvencore), to provide a visual flow-based programming interface. The [Ryven](https://github.com/leon-thomm/Ryven) editor is built on top of `ryvencore-qt`, and their development is currently tightly coupled.
 
 ### Installation
 
+You need to have Python and pip installed. Then, either install from PyPI using pip:
+
 ```
 pip install ryvencore-qt
 ```
 
 or build from sources
+
 ```
 git clone https://github.com/leon-thomm/ryvencore-qt
 cd ryvencore-qt
 pip install .
 ```
 
 ### Dependencies
 
-ryvencore-qt runs on PySide2 (Python bindings for Qt) using [QtPy](https://github.com/spyder-ide/qtpy) as a wrapper to (eventually, once supported) enable seamless switching between PySide2 and PySide6. Notice that `ryvencore-qt` does not work with PyQt, due to crucial inheritance restrictions in PyQt.
+ryvencore-qt uses Python bindings for Qt using [QtPy](https://github.com/spyder-ide/qtpy). I usually run it with PySide2, running on PySide6 should also work with minor changes. PyQt is not supported, due to crucial inheritance restrictions in PyQt.
+
+### Documentation
+
+An extensive documentation doesn't currently exist.
 
 ### quick start
 
 The below code demonstrates how to set up an editor with custom defined nodes. You can also find the code in the *examples* folder.
 
 `main.py`
 ``` python
@@ -130,33 +137,12 @@
 
 export_nodes = [
     PrintNode,
     RandNode,
 ]
 ```
 
-For a more detailed overview, including a precise definition of flows, see the [Features Page](https://leon-thomm.github.io/ryvencore-qt/features/) and [ryvencore](https://github.com/leon-thomm/ryvencore).
-
 ### Development
 
-The code is not 100% PEP 8 conform, and some parts which are under development might seem messy. I'm doing my best :) feel free to improve. The individual subpackages have their own READMEs giving a quick overview which should be quite helpful to gain understanding about implementations.
+The individual subpackages have their own READMEs giving a quick overview which should be quite helpful to gain understanding about implementations.
 
 Cheers.
-
-<!--
-### Contributions and Development
-
-This project will eventually need a community in order to survive. Particularly effective ways to contribute outside of direct development of the software are creating
-
-- tutorials
-- nodes
-- small editors
-- documentation
-- tests
-- etc
-
-If you have any questions, suggestions, or want to show something you've built with this project notice the *discussions* area which is the perfect place for that.
-
-To give a quick overview over the most important class relations, see the below class diagram. The DrawIO diagram file is in the repository.
-
-![](./docs/img/ryvencore-drawio_.png)
--->
```

### Comparing `ryvencore-qt-0.3.1.4/README.md` & `ryvencore-qt-0.4.0a2/ryvencore_qt.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,52 @@
+Metadata-Version: 2.1
+Name: ryvencore-qt
+Version: 0.4.0a2
+Summary: Qt frontend for ryvencore; Library for building Visual Node Editors
+Home-page: https://github.com/leon-thomm/ryvencore-qt
+Author: Leon Thomm
+Author-email: l.thomm@mailbox.org
+Project-URL: Website, https://ryven.org
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 <p align="center">
   <img src="./ryvencore_qt/resources/pics/logo.png" alt="drawing" width="70%"/>
 </p>
 
-`rvencore-qt` is a wrapper around [ryvencore](https://github.com/leon-thomm/ryvencore) and provides a Qt frontend for it. It comes from the [Ryven](https://github.com/leon-thomm/Ryven) project and will be the foundation for future Ryven versions. So, ryvencore-qt can be used to build cross-platform standalone visual node editors based on Python. Projects made with ryvencore-qt can be natively deployed directly on the backend, ryvencore. The development of ryvencore-qt is currently closely tied to Ryven.
+`ryvencore-qt` provides Qt-based GUI classes for [ryvencore](https://github.com/leon-thomm/ryvencore), to provide a visual flow-based programming interface. The [Ryven](https://github.com/leon-thomm/Ryven) editor is built on top of `ryvencore-qt`, and their development is currently tightly coupled.
 
 ### Installation
 
+You need to have Python and pip installed. Then, either install from PyPI using pip:
+
 ```
 pip install ryvencore-qt
 ```
 
 or build from sources
+
 ```
 git clone https://github.com/leon-thomm/ryvencore-qt
 cd ryvencore-qt
 pip install .
 ```
 
 ### Dependencies
 
-ryvencore-qt runs on PySide2 (Python bindings for Qt) using [QtPy](https://github.com/spyder-ide/qtpy) as a wrapper to (eventually, once supported) enable seamless switching between PySide2 and PySide6. Notice that `ryvencore-qt` does not work with PyQt, due to crucial inheritance restrictions in PyQt.
+ryvencore-qt uses Python bindings for Qt using [QtPy](https://github.com/spyder-ide/qtpy). I usually run it with PySide2, running on PySide6 should also work with minor changes. PyQt is not supported, due to crucial inheritance restrictions in PyQt.
+
+### Documentation
+
+An extensive documentation doesn't currently exist.
 
 ### quick start
 
 The below code demonstrates how to set up an editor with custom defined nodes. You can also find the code in the *examples* folder.
 
 `main.py`
 ``` python
@@ -115,33 +137,12 @@
 
 export_nodes = [
     PrintNode,
     RandNode,
 ]
 ```
 
-For a more detailed overview, including a precise definition of flows, see the [Features Page](https://leon-thomm.github.io/ryvencore-qt/features/) and [ryvencore](https://github.com/leon-thomm/ryvencore).
-
 ### Development
 
-The code is not 100% PEP 8 conform, and some parts which are under development might seem messy. I'm doing my best :) feel free to improve. The individual subpackages have their own READMEs giving a quick overview which should be quite helpful to gain understanding about implementations.
+The individual subpackages have their own READMEs giving a quick overview which should be quite helpful to gain understanding about implementations.
 
 Cheers.
-
-<!--
-### Contributions and Development
-
-This project will eventually need a community in order to survive. Particularly effective ways to contribute outside of direct development of the software are creating
-
-- tutorials
-- nodes
-- small editors
-- documentation
-- tests
-- etc
-
-If you have any questions, suggestions, or want to show something you've built with this project notice the *discussions* area which is the perfect place for that.
-
-To give a quick overview over the most important class relations, see the below class diagram. The DrawIO diagram file is in the repository.
-
-![](./docs/img/ryvencore-drawio_.png)
--->
```

### Comparing `ryvencore-qt-0.3.1.4/docs/README.md` & `ryvencore-qt-0.4.0a2/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 ## Logging
 
 Every *script* has a *logs manager*. The `Node`'s API already includes methods for requesting custom loggers.
 
 <!--
 ## Convenience Classes
 
-ryvecore already comes with a few convenience classes for widgets. Those convenience classes only use ryvencore's public API, so if you have experience with Qt, you can totally implemenent them yourself. But in most cases they make it much easier to get started. See [convenience GUI section](../conv_gui).
+ryvecore already comes with a few convenience classes for widgets. Those convenience classes only use ryvencore's public API, so if you have experience with Qt, you can totally implemenent them yourself. But in most cases they make it much easier to get started. See [convenience GUI section](../widgets).
 -->
 
 # `ryvencore-qt`
 
 ### Custom GUI
 
 You can add custom Qt widgets to your nodes. For instructions on how to register custom widgets in your nodes see Ryven docs.
```

### Comparing `ryvencore-qt-0.3.1.4/docs/img/function_node.png` & `ryvencore-qt-0.4.0a2/docs/img/function_node.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/img/logic_editor_screenshot1.png` & `ryvencore-qt-0.4.0a2/docs/img/logic_editor_screenshot1.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/img/logic_editor_screenshot2.png` & `ryvencore-qt-0.4.0a2/docs/img/logic_editor_screenshot2.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/img/logic_editor_screenshot3.png` & `ryvencore-qt-0.4.0a2/docs/img/logic_editor_screenshot3.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/img/logo.png` & `ryvencore-qt-0.4.0a2/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/img/macro.png` & `ryvencore-qt-0.4.0a2/docs/img/macro.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/img/macro2.png` & `ryvencore-qt-0.4.0a2/docs/img/macro2.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/img/ryvencore-drawio_.png` & `ryvencore-qt-0.4.0a2/docs/img/ryvencore-drawio_.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/img/ryvencore_screenshot1.png` & `ryvencore-qt-0.4.0a2/docs/img/ryvencore_screenshot1.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/img/stylus_light.png` & `ryvencore-qt-0.4.0a2/docs/img/stylus_light.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/index.html` & `ryvencore-qt-0.4.0a2/docs/index.html`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/unused/api.md` & `ryvencore-qt-0.4.0a2/docs/unused/api.md`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/unused/features.md` & `ryvencore-qt-0.4.0a2/docs/unused/features.md`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 ## Logging
 
 Every *script* has a *logs manager*. The `Node`'s API already includes methods for requesting custom loggers.
 
 <!--
 ## Convenience Classes
 
-ryvecore already comes with a few convenience classes for widgets. Those convenience classes only use ryvencore's public API, so if you have experience with Qt, you can totally implemenent them yourself. But in most cases they make it much easier to get started. See [convenience GUI section](../conv_gui).
+ryvecore already comes with a few convenience classes for widgets. Those convenience classes only use ryvencore's public API, so if you have experience with Qt, you can totally implemenent them yourself. But in most cases they make it much easier to get started. See [convenience GUI section](../widgets).
 -->
 
 ### Custom GUI
 
 You can add custom Qt widgets to your nodes. For instructions on how to register custom widgets in your nodes see Ryven docs.
 
 ## Styling
```

### Comparing `ryvencore-qt-0.3.1.4/docs/unused/getting_started.md` & `ryvencore-qt-0.4.0a2/docs/unused/getting_started.md`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/docs/unused/gui.md` & `ryvencore-qt-0.4.0a2/docs/unused/gui.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 A main widget must additionally subclass ryvencore's `MWB` (MainWidgetBase) class. Example:
 
 ```python
 import ryvencore_qt as rc
 from PySide2.QtWidgets import QPushButton
 
 
-class MyMainWidget(rc.MWB, QPushButton):
+class MyMainWidget(rc.NodeMainWidget, QPushButton):
     def __init__(self, params):
-        rc.MWB.__init__(self, params)
+        rc.NodeMainWidget.__init__(self, params)
         QPushButton.__init__(self)
-        
+
         # then do your stuff like
         self.setEnabled(False)
         self.clicked.connect(self.node.update)
 ```
 
 After `rc.MWB.__init__(self, params)`, you have access to the node object via `self.node`. A custom main widget class must be referenced in the node's class definition
```

### Comparing `ryvencore-qt-0.3.1.4/docs/unused/threading.md` & `ryvencore-qt-0.4.0a2/docs/unused/threading.md`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-Bold.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-BoldItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-Italic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-Medium.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-MediumItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-Regular.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-SemiBold.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/Asap-SemiBoldItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/Asap-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/asap/OFL.txt` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/asap/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/OFL.txt` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Black.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-BlackItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Bold.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-BoldItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBold.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLight.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Italic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Light.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-LightItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Medium.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-MediumItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Regular.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBold.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-Thin.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/poppins/Poppins-ThinItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/poppins/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/OFL.txt` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/OFL.txt`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Black.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Black.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Light.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Light.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Medium.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/fonts/source_code_pro/SourceCodePro-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/node_collapse_icon.svg` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/node_collapse_icon.svg`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 000007d0: 3232 3931 382c 2d31 2e33 3232 3931 2031  22918,-1.32291 1
 000007e0: 2e33 3232 3931 352c 312e 3332 3239 3122  .322915,1.32291"
 000007f0: 0a20 2020 2020 2020 6964 3d22 7061 7468  .       id="path
 00000800: 3833 3522 0a20 2020 2020 2020 736f 6469  835".       sodi
 00000810: 706f 6469 3a6e 6f64 6574 7970 6573 3d22  podi:nodetypes="
 00000820: 6363 6322 202f 3e0a 2020 2020 3c70 6174  ccc" />.    <pat
 00000830: 680a 2020 2020 2020 2073 7479 6c65 3d22  h.       style="
-00000840: 6669 6c6c 3a23 4139 4435 4546 3b66 696c  fill:#A9D5EF;fil
+00000840: 6669 6c6c 3a23 7878 7878 7878 3b66 696c  fill:#xxxxxx;fil
 00000850: 6c2d 6f70 6163 6974 793a 313b 7374 726f  l-opacity:1;stro
 00000860: 6b65 3a23 3030 3030 3030 3b73 7472 6f6b  ke:#000000;strok
 00000870: 652d 7769 6474 683a 302e 3236 353b 7374  e-width:0.265;st
 00000880: 726f 6b65 2d6c 696e 6563 6170 3a62 7574  roke-linecap:but
 00000890: 743b 7374 726f 6b65 2d6c 696e 656a 6f69  t;stroke-linejoi
 000008a0: 6e3a 726f 756e 643b 7374 726f 6b65 2d6d  n:round;stroke-m
 000008b0: 6974 6572 6c69 6d69 743a 343b 7374 726f  iterlimit:4;stro
@@ -147,15 +147,15 @@
 00000920: 3338 3132 3520 322e 3338 3132 352c 322e  38125 2.38125,2.
 00000930: 3338 3132 3520 302e 3236 3435 3833 2c2d  38125 0.264583,-
 00000940: 302e 3236 3435 3820 2d32 2e36 3435 3833  0.26458 -2.64583
 00000950: 332c 2d32 2e36 3435 3833 207a 220a 2020  3,-2.64583 z".  
 00000960: 2020 2020 2069 643d 2270 6174 6838 3339       id="path839
 00000970: 2220 2f3e 0a20 2020 203c 7061 7468 0a20  " />.    <path. 
 00000980: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
-00000990: 6c3a 2341 3944 3545 463b 6669 6c6c 2d6f  l:#A9D5EF;fill-o
+00000990: 6c3a 2378 7878 7878 783b 6669 6c6c 2d6f  l:#xxxxxx;fill-o
 000009a0: 7061 6369 7479 3a31 3b73 7472 6f6b 653a  pacity:1;stroke:
 000009b0: 2330 3030 3030 303b 7374 726f 6b65 2d77  #000000;stroke-w
 000009c0: 6964 7468 3a30 3b73 7472 6f6b 652d 6c69  idth:0;stroke-li
 000009d0: 6e65 6361 703a 6275 7474 3b73 7472 6f6b  necap:butt;strok
 000009e0: 652d 6c69 6e65 6a6f 696e 3a6d 6974 6572  e-linejoin:miter
 000009f0: 3b73 7472 6f6b 652d 6d69 7465 726c 696d  ;stroke-miterlim
 00000a00: 6974 3a34 3b73 7472 6f6b 652d 6461 7368  it:4;stroke-dash
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/node_expand_icon.svg` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/node_expand_icon.svg`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/code_block_picture.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/code_block_picture.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/code_block_picture2.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/code_block_picture2.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/code_block_picture3.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/code_block_picture3.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/function_picture.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/function_picture.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/function_picture_.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/function_picture_.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/logo.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/logo.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/macro_icon.svg` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/macro_icon.svg`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/macro_node_icon.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/macro_node_icon.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/macro_script_picture.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/macro_script_picture.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/opencv_example.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/opencv_example.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/script_picture.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/script_picture.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/script_picture.svg` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/script_picture.svg`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/script_picture_old.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/script_picture_old.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/resources/pics/variable_picture.png` & `ryvencore-qt-0.4.0a2/ryvencore_qt/resources/pics/variable_picture.png`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/Design.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/Design.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import json
 
 from qtpy.QtCore import QObject, Signal
 from qtpy.QtGui import QFontDatabase
 
-from .flows.FlowTheme import FlowTheme_Toy, FlowTheme_DarkTron, FlowTheme_Ghost, FlowTheme_Blender, \
-    FlowTheme_Simple, FlowTheme_Ueli, FlowTheme_PureDark, FlowTheme, FlowTheme_PureLight, \
-    FlowTheme_Colorful, FlowTheme_ColorfulLight, FlowTheme_Industrial, FlowTheme_Fusion
+from .flows.FlowTheme import FlowTheme, flow_themes
 from .GlobalAttributes import Location
 
 
 class Design(QObject):
     """Design serves as a container for the stylesheet and flow themes, and sends signals to notify GUI elements
     on change of the flow theme. A configuration for the flow themes can be loaded from a json file."""
 
@@ -17,24 +15,23 @@
 
     flow_theme_changed = Signal(str)
     performance_mode_changed = Signal(str)
 
     def __init__(self):
         super().__init__()
 
-        self.flow_themes = []
+        self.flow_themes = flow_themes
         self.flow_theme: FlowTheme = None
         self.default_flow_size = None
         self.performance_mode: str = None
         self.node_item_shadows_enabled: bool = None
         self.animations_enabled: bool = None
         self.node_selection_stylesheet: str = None
 
         # load standard default values
-        self.register_flow_themes()
         self._default_flow_theme = self.flow_themes[-1]
         self.set_performance_mode('pretty')
         self.set_animations_enabled(True)
         self.default_flow_size = [1000, 700]
         self.set_flow_theme(self._default_flow_theme)
 
     @staticmethod
@@ -46,30 +43,14 @@
         db.addApplicationFont(
             Location.PACKAGE_PATH + '/resources/fonts/source_code_pro/SourceCodePro-Regular.ttf'
         )
         db.addApplicationFont(
             Location.PACKAGE_PATH + '/resources/fonts/asap/Asap-Regular.ttf'
         )
 
-    def register_flow_themes(self):
-        self.flow_themes = [
-            FlowTheme_Toy(),
-            FlowTheme_DarkTron(),
-            FlowTheme_Ghost(),
-            FlowTheme_Blender(),
-            FlowTheme_Simple(),
-            FlowTheme_Ueli(),
-            FlowTheme_PureDark(),
-            FlowTheme_Colorful(),
-            FlowTheme_PureLight(),
-            FlowTheme_ColorfulLight(),
-            FlowTheme_Industrial(),
-            FlowTheme_Fusion(),
-        ]
-
     def load_from_config(self, filepath: str):
         """Loads design configs from a config json file"""
 
         f = open(filepath, 'r')
         data = f.read()
         f.close()
 
@@ -95,15 +76,15 @@
             self.default_flow_size = IMPORT_DATA['default flow size']
 
     def available_flow_themes(self) -> dict:
         return {theme.name: theme for theme in self.flow_themes}
 
     def flow_theme_by_name(self, name: str) -> FlowTheme:
         for theme in self.flow_themes:
-            if theme.name == name:
+            if theme.name.casefold() == name.casefold():
                 return theme
         return None
 
     def set_flow_theme(self, theme: FlowTheme = None, name: str = ''):
         """You can either specify the theme by name, or directly provide a FlowTheme object"""
         if theme:
             self.flow_theme = theme
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/GUIBase.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/GUIBase.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,17 +22,15 @@
 
             if isinstance(obj, dict):
                 GID = obj.get('GID')
                 if GID is not None:
                     # find representative
                     comp = GUIBase.FRONTEND_COMPONENT_ASSIGNMENTS.get(GID)
                     if comp:
-                        obj = session.threading_bridge__backend.run(
-                            comp.complete_data, (obj,)
-                        )  # run complete_data() (in frontend thread)
+                        obj = comp.complete_data(obj)
 
                 # look for child objects
                 for key, value in obj.items():
                     obj[key] = analyze(value)
 
             elif isinstance(obj, list):
                 for i in range(len(obj)):
@@ -43,13 +41,13 @@
             return obj
 
         return analyze
 
     def __init__(self, representing_component: Base = None):
         """parameter `representing` indicates representation of a specific backend component"""
         if representing_component is not None:
-            GUIBase.FRONTEND_COMPONENT_ASSIGNMENTS[representing_component.GLOBAL_ID] = self
+            GUIBase.FRONTEND_COMPONENT_ASSIGNMENTS[representing_component.global_id] = self
 
     # OVERRIDE
     def complete_data(self, data: dict) -> dict:
         """completes the data dict of the represented backend component by adding all frontend data"""
         return data
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/EditVal_Dialog.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/EditVal_Dialog.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/LogWidget.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/LogWidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from qtpy.QtGui import QFont
 from qtpy.QtWidgets import QWidget, QHBoxLayout, QVBoxLayout, QLabel, QPushButton, QPlainTextEdit
 
 # from ..core_wrapper.WRAPPERS import Logger
-from ryvencore import Logger
+from ryvencore.addons.Logging import Logger
 import logging
 
 
 class LogWidget(QWidget):
     """Convenience class for a QWidget representing a log."""
 
     def __init__(self, logger: Logger):
         super().__init__()
 
         self.logger = logger
         self.logger.addHandler(logging.StreamHandler(self))
-        self.logger.sig_disabled.connect(self.disable)
-        self.logger.sig_enabled.connect(self.enable)
+        self.logger.sig_disabled.sub(self.disable)
+        self.logger.sig_enabled.sub(self.enable)
 
         self.main_layout = QVBoxLayout()
         self.header_layout = QHBoxLayout()
 
         title_label = QLabel(self.logger.name)
         title_label.setFont(QFont('Poppins', 12))
         self.header_layout.addWidget(title_label)
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/ScriptsListWidget.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/FlowsListWidget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from qtpy.QtCore import Qt
 from qtpy.QtWidgets import QWidget, QMessageBox, QVBoxLayout, QLineEdit, QHBoxLayout, QPushButton, QScrollArea
 
-from .ScriptsList_ScriptWidget import ScriptsList_ScriptWidget
+from .FlowsList_FlowWidget import FlowsList_FlowWidget
 
 
-class ScriptsListWidget(QWidget):
-    """Convenience class for a QWidget to easily manage the scripts of a session."""
+class FlowsListWidget(QWidget):
+    """Convenience class for a QWidget to easily manage the flows of a session."""
 
-    def __init__(self, session):
+    def __init__(self, session_gui):
         super().__init__()
 
-        self.session = session
+        self.session_gui = session_gui
         self.list_widgets = []
         self.ignore_name_line_edit_signal = False  # because disabling causes firing twice otherwise
 
         self.setup_UI()
 
-        self.session.flow_view_created.connect(self.add_new_script)
-        self.session.script_deleted.connect(self.recreate_list)
+        self.session_gui.flow_view_created.connect(self.add_new_flow)
+        self.session_gui.flow_deleted.connect(self.recreate_list)
 
 
     def setup_UI(self):
         main_layout = QVBoxLayout(self)
         main_layout.setAlignment(Qt.AlignTop)
         self.setLayout(main_layout)
 
@@ -42,53 +42,53 @@
         self.list_layout.setAlignment(Qt.AlignTop)
         self.scroll_area_widget.setLayout(self.list_layout)
 
         self.layout().addWidget(self.list_scroll_area)
 
         # line edit
 
-        self.new_script_title_lineedit = QLineEdit()
-        self.new_script_title_lineedit.setPlaceholderText('new script\'s title')
-        self.new_script_title_lineedit.returnPressed.connect(self.create_script)
+        self.new_flow_title_lineedit = QLineEdit()
+        self.new_flow_title_lineedit.setPlaceholderText('new flow\'s title')
+        self.new_flow_title_lineedit.returnPressed.connect(self.create_flow)
 
-        main_layout.addWidget(self.new_script_title_lineedit)
+        main_layout.addWidget(self.new_flow_title_lineedit)
 
 
         self.recreate_list()
 
 
     def recreate_list(self):
-        # remove script widgets
+        # remove flow widgets
         for i in reversed(range(self.list_layout.count())):
             self.list_layout.itemAt(i).widget().setParent(None)
 
         self.list_widgets.clear()
 
-        for s in self.session.scripts:
-            new_widget = ScriptsList_ScriptWidget(self, self.session, s)
+        for s in self.session_gui.core_session.flows:
+            new_widget = FlowsList_FlowWidget(self, self.session_gui, s)
             self.list_widgets.append(new_widget)
 
         for w in self.list_widgets:
             self.list_layout.addWidget(w)
 
-    def create_script(self):
-        title = self.new_script_title_lineedit.text()
+    def create_flow(self):
+        title = self.new_flow_title_lineedit.text()
 
-        if self.session.script_title_valid(title):
-            self.session.create_script(title=title)
+        if self.session_gui.core_session.flow_title_valid(title):
+            self.session_gui.core_session.create_flow(title=title)
 
-    def add_new_script(self, script, flow_view):
+    def add_new_flow(self, flow, flow_view):
         self.recreate_list()
 
-    def del_script(self, script, script_widget):
-        msg_box = QMessageBox(QMessageBox.Warning, 'sure about deleting script?',
-                              'You are about to delete a script. This cannot be undone, all content will be lost. '
+    def del_flow(self, flow, flow_widget):
+        msg_box = QMessageBox(QMessageBox.Warning, 'sure about deleting flow?',
+                              'You are about to delete a flow. This cannot be undone, all content will be lost. '
                               'Do you want to continue?', QMessageBox.Cancel | QMessageBox.Yes, self)
         msg_box.setDefaultButton(QMessageBox.Cancel)
         ret = msg_box.exec_()
         if ret != QMessageBox.Yes:
             return
 
-        self.list_widgets.remove(script_widget)
-        script_widget.setParent(None)
-        self.session.delete_script(script)
+        self.list_widgets.remove(flow_widget)
+        flow_widget.setParent(None)
+        self.session_gui.core_session.delete_flow(flow)
         # self.recreate_list()
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/ScriptsList_ScriptWidget.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/FlowsList_FlowWidget.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,47 +2,48 @@
 from qtpy.QtGui import QIcon, QImage
 from qtpy.QtCore import Qt, QEvent, QBuffer, QByteArray
 
 from ..GlobalAttributes import Location
 from .ListWidget_NameLineEdit import ListWidget_NameLineEdit
 
 
-class ScriptsList_ScriptWidget(QWidget):
-    """A QWidget representing a single Script for the ScriptsListWidget."""
+class FlowsList_FlowWidget(QWidget):
+    """A QWidget representing a single Flow for the FlowsListWidget."""
 
-    def __init__(self, scripts_list_widget, session, script):
+    def __init__(self, flows_list_widget, session_gui, flow):
         super().__init__()
 
-        self.session = session
-        self.script = script
-        self.flow_view = self.session.flow_views[script]
-        self.scripts_list_widget = scripts_list_widget
-        self.previous_script_title = ''
+        self.session_gui = session_gui
+        self.flow = flow
+        self.flow_view = self.session_gui.flow_views[flow]
+        self.flows_list_widget = flows_list_widget
+        self.previous_flow_title = ''
         self._thumbnail_source = ''
         self.ignore_title_line_edit_signal = False
 
 
         # UI
 
         main_layout = QHBoxLayout()
         main_layout.setContentsMargins(0, 0, 0, 0)
 
         #   create icon
 
-        script_icon = QIcon(Location.PACKAGE_PATH + '/resources/pics/script_picture.png')
+        # TODO: change this icon
+        flow_icon = QIcon(Location.PACKAGE_PATH + '/resources/pics/script_picture.png')
 
         icon_label = QLabel()
         icon_label.setFixedSize(20, 20)
         icon_label.setStyleSheet('border:none;')
-        icon_label.setPixmap(script_icon.pixmap(20, 20))
+        icon_label.setPixmap(flow_icon.pixmap(20, 20))
         main_layout.addWidget(icon_label)
 
         #   title line edit
 
-        self.title_line_edit = ListWidget_NameLineEdit(script.title, self)
+        self.title_line_edit = ListWidget_NameLineEdit(flow.title, self)
         self.title_line_edit.setPlaceholderText('title')
         self.title_line_edit.setEnabled(False)
         self.title_line_edit.editingFinished.connect(self.title_line_edit_editing_finished)
 
         main_layout.addWidget(self.title_line_edit)
 
         self.setLayout(main_layout)
@@ -85,33 +86,33 @@
         for a in actions:
             menu.addAction(a)
 
         menu.exec_(event.globalPos())
 
 
     def action_delete_triggered(self):
-        self.scripts_list_widget.del_script(self.script, self)
+        self.flows_list_widget.del_flow(self.flow, self)
 
 
     def title_line_edit_double_clicked(self):
         self.title_line_edit.setEnabled(True)
         self.title_line_edit.setFocus()
         self.title_line_edit.selectAll()
 
-        self.previous_script_title = self.title_line_edit.text()
+        self.previous_flow_title = self.title_line_edit.text()
 
 
     def title_line_edit_editing_finished(self):
         if self.ignore_title_line_edit_signal:
             return
 
         title = self.title_line_edit.text()
 
         self.ignore_title_line_edit_signal = True
 
-        if self.session.script_title_valid(title):
-            self.session.rename_script(script=self.script, title=title)
+        if self.session_gui.core_session.flow_title_valid(title):
+            self.session_gui.core_session.rename_flow(flow=self.flow, title=title)
         else:
-            self.title_line_edit.setText(self.previous_script_title)
+            self.title_line_edit.setText(self.previous_flow_title)
 
         self.title_line_edit.setEnabled(False)
         self.ignore_title_line_edit_signal = False
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/conv_gui/VarsList_VarWidget.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/widgets/VarsList_VarWidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 
 import json
 
 from ..GlobalAttributes import Location
 from .ListWidget_NameLineEdit import ListWidget_NameLineEdit
 from ..utils import shorten
 from .EditVal_Dialog import EditVal_Dialog
+from ryvencore.addons.Variables import VarsAddon
 
 
 class VarsList_VarWidget(QWidget):
     """A QWidget representing a single script variable for the VariablesListWidget."""
 
-    def __init__(self, vars_list_widget, vars_manager, var):
+    def __init__(self, vars_list_widget, vars_addon: VarsAddon, flow, var):
         super().__init__()
 
-        self.vars_manager = vars_manager
+        self.vars_addon = vars_addon
+        self.flow = flow
         self.var = var
         self.vars_list_widget = vars_list_widget
         self.previous_var_name = ''  # for editing
 
         self.ignore_name_line_edit_signal = False
 
 
@@ -37,15 +39,15 @@
         icon_label.setFixedSize(15, 15)
         icon_label.setStyleSheet('border:none;')
         icon_label.setPixmap(variable_icon.pixmap(15, 15))
         main_layout.addWidget(icon_label)
 
         #   name line edit
 
-        self.name_line_edit = ListWidget_NameLineEdit(var.name, self)
+        self.name_line_edit = ListWidget_NameLineEdit(self.var.name, self)
         self.name_line_edit.setPlaceholderText('name')
         self.name_line_edit.setEnabled(False)
         self.name_line_edit.editingFinished.connect(self.name_line_edit_editing_finished)
 
         main_layout.addWidget(self.name_line_edit)
 
         self.setLayout(main_layout)
@@ -71,18 +73,18 @@
             return
 
 
     def event(self, event):
         if event.type() == QEvent.ToolTip:
             val_str = ''
             try:
-                val_str = str(self.var.val)
+                val_str = str(self.var.get())
             except Exception as e:
                 val_str = "couldn't stringify value"
-            self.setToolTip('val type: '+str(type(self.var.val))+'\nval: '+shorten(val_str, 3000, line_break=True))
+            self.setToolTip('val type: '+str(type(self.var.get()))+'\nval: '+shorten(val_str, 3000, line_break=True))
 
         return QWidget.event(self, event)
 
 
     def contextMenuEvent(self, event):
         menu: QMenu = QMenu(self)
 
@@ -96,48 +98,49 @@
         for a in actions:
             menu.addAction(a)
 
         menu.exec_(event.globalPos())
 
 
     def action_delete_triggered(self):
-        self.vars_list_widget.del_variable(self.var, self)
+        self.vars_list_widget.del_var(self.var)
 
 
     def action_edit_val_triggered(self):
-        edit_var_val_dialog = EditVal_Dialog(self, self.var.val)
+        edit_var_val_dialog = EditVal_Dialog(self, self.var.get())
         accepted = edit_var_val_dialog.exec_()
         if accepted:
-            self.vars_manager.set_var(self.var.name, edit_var_val_dialog.get_val())
+            self.var.set(edit_var_val_dialog.get_val())
+            # self.vars_addon.create_var(self.flow, self.var.name, edit_var_val_dialog.get_val())
 
 
     def name_line_edit_double_clicked(self):
         self.name_line_edit.setEnabled(True)
         self.name_line_edit.setFocus()
         self.name_line_edit.selectAll()
 
         self.previous_var_name = self.name_line_edit.text()
 
 
     def get_drag_data(self):
         data = {'type': 'variable',
                 'name': self.var.name,
-                'value': self.var.val}  # value is probably unnecessary
+                'value': self.var.get()}  # value is probably unnecessary
         data_text = json.dumps(data)
         return data_text
 
 
     def name_line_edit_editing_finished(self):
         if self.ignore_name_line_edit_signal:
             return
 
         name = self.name_line_edit.text()
 
         self.ignore_name_line_edit_signal = True
 
-        if self.vars_manager.var_name_valid(name):
+        if self.vars_addon.var_name_valid(self.flow, name):
             self.var.name = name
         else:
             self.name_line_edit.setText(self.previous_var_name)
 
         self.name_line_edit.setEnabled(False)
         self.ignore_name_line_edit_signal = False
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/core_wrapper/Node.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeGUI.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,278 +1,252 @@
-from qtpy.QtCore import QObject, Signal
+from queue import Queue
+from typing import List, Dict, Tuple, Optional, Union
 
-from ryvencore import Node as RC_Node
-from ..GlobalAttributes import Location
-from ryvencore.dtypes import DType
+from qtpy.QtCore import QObject, Signal
 
 
-class Node(RC_Node, QObject):
-    """Base class nodes in ryvencore-qt"""
+class NodeGUI(QObject):
+    """
+    Interface class between nodes and their GUI representation.
+    """
 
+    # customizable gui attributes
     description_html: str = None
     main_widget_class: list = None
     main_widget_pos: str = 'below ports'
     input_widget_classes: dict = {}
+    init_input_widgets: dict = {}
     style: str = 'normal'
     color: str = '#c69a15'
+    display_title: str = None
     icon: str = None
 
-    # SIGNALS
-    updated = Signal()
-    input_added = Signal(object, object)
-    output_added = Signal(object, object)
-    input_removed = Signal(object)
-    output_removed = Signal(object)
+    # qt signals
+    updating = Signal()
+    update_error = Signal(object)
+    input_added = Signal(int, object)
+    output_added = Signal(int, object)
+    input_removed = Signal(int, object)
+    output_removed = Signal(int, object)
     update_shape_triggered = Signal()
     hide_unconnected_ports_triggered = Signal()
     show_unconnected_ports_triggered = Signal()
 
     def __init__(self, params):
         QObject.__init__(self)
-        RC_Node.__init__(self, params)
 
-        self.default_actions = self.init_default_actions()
-        self.actions = {}
-        self.display_title = self.title
+        node, session_gui = params
+        self.node = node
+        self.item = None   # set by the node item directly after this __init__ call
+        self.session_gui = session_gui
+        setattr(node, 'gui', self)
+
+        self.actions = self._init_default_actions()
+
+        if self.display_title is None:
+            self.display_title = self.node.title
+
+        self.input_widgets = {}     # {input: widget name}
+        for i, widget_data in self.init_input_widgets.items():
+            self.input_widgets[self.node.inputs[i]] = widget_data
+        # using attach_input_widgets() one can buffer input widget
+        # names for inputs that are about to get created
+        self._next_input_widgets = Queue()
+
+        self.error_during_update = False
+
+        # turn ryvencore signals into Qt signals
+        self.node.updating.sub(self._on_updating)
+        self.node.update_error.sub(self._on_update_error)
+        self.node.input_added.sub(self._on_new_input_added)
+        self.node.output_added.sub(self._on_new_output_added)
+        self.node.input_removed.sub(self._on_input_removed)
+        self.node.output_removed.sub(self._on_output_removed)
+
+    def initialized(self):
+        """
+        *VIRTUAL*
+
+        Called after the node GUI has been fully initialized.
+        The Node has been created already (including all ports) and loaded.
+        No connections have been made to ports of the node yet.
+        """
+        pass
 
-        self.item = None  # set by the flow view
+    """
+    slots
+    """
 
-    """actions"""
+    # TODO: displaying update errors is currently prevented by the
+    #   lack of an appropriate updated event in ryvencore.
+    #   Update: there is an updating event now.
+
+    # def on_updated(self, inp):
+    #     if self.error_during_update:
+    #         # an error should prevent an update event, so if we
+    #         # are here, the update was successful
+    #         self.self.error_during_update = False
+    #         self.item.remove_error_message()
+    #     self.updated.emit()
+    #
+    def _on_update_error(self, e):
+    #     self.item.display_error(e)
+    #     self.error_during_update = True
+        self.update_error.emit(e)
+
+    def _on_updating(self, inp: int):
+        # update input widget
+        if inp != -1 and self.item.inputs[inp].widget is not None:
+            o = self.node.flow.connected_output(self.node.inputs[inp])
+            if o is not None:
+                self.item.inputs[inp].widget.val_update_event(o.val)
+
+        self.updating.emit()
+
+    def _on_new_input_added(self, _, index, inp):
+        if not self._next_input_widgets.empty():
+            self.input_widgets[inp] = self._next_input_widgets.get()
+        self.input_added.emit(index, inp)
+
+    def _on_new_output_added(self, _, index, out):
+        self.output_added.emit(index, out)
+
+    def _on_input_removed(self, _, index, inp):
+        self.input_removed.emit(index, inp)
+
+    def _on_output_removed(self, _, index, out):
+        self.output_removed.emit(index, out)
+
+    """
+    actions
+    
+    TODO: move actions to ryvencore?
+    """
 
-    def init_default_actions(self) -> dict:
-        actions = {
+    def _init_default_actions(self):
+        """
+        Returns the default actions every node should have
+        """
+        return {
             'update shape': {'method': self.update_shape},
             'hide unconnected ports': {'method': self.hide_unconnected_ports},
-            'change title': {'method': self.change_title}
+            'change title': {'method': self.change_title},
         }
-        return actions
-
 
-    def set_special_actions_data(self, actions_data):
-        actions = {}
-        for key in actions_data:
-            if type(actions_data[key]) != dict:
+    def _deserialize_actions(self, actions_data):
+        """
+        Recursively reconstructs the actions dict from the serialized version
+        """
+
+        def _transform(actions_data: dict):
+            """
+            Mutates the actions_data argument by replacing the method names
+            with the actual methods. Doesn't modify the original dict.
+            """
+            new_actions = {}
+            for key, value in actions_data.items():
                 if key == 'method':
                     try:
-                        actions['method'] = getattr(self, actions_data[key])
-                    except AttributeError:  # outdated method referenced
-                        pass
-                elif key == 'data':
-                    actions['data'] = actions_data[key]
-            else:
-                actions[key] = self.set_special_actions_data(actions_data[key])
-        return actions
-
-
-    def get_special_actions_data(self, actions):
-        cleaned_actions = actions.copy()
-        for key in cleaned_actions:
-            v = cleaned_actions[key]
-            # if type(v) == M:  # callable(v):
-            #     cleaned_actions[key] = v.method_name
-            if callable(v):
-                cleaned_actions[key] = v.__name__
-            elif type(v) == dict:
-                cleaned_actions[key] = self.get_special_actions_data(v)
-            else:
-                cleaned_actions[key] = v
-        return cleaned_actions
-
-
-    def get_extended_default_actions(self):
-        actions_dict = self.default_actions.copy()
-        for index in range(len(self.inputs)):
-            inp = self.inputs[index]
-            if inp.type_ == 'exec':
-                actions_dict['exec input '+str(index)] = {'method': self.action_exec_input,
-                                                          'data': {'input index': index}}
-        return actions_dict
-
+                        value = getattr(self, value)
+                    except AttributeError:
+                        print(f'Warning: action method "{value}" not found in node "{self.node.title}", skipping.')
+                elif isinstance(value, dict):
+                    value = _transform(value)
+                new_actions[key] = value
+            return new_actions
+
+        return _transform(actions_data)
+
+    def _serialize_actions(self, actions):
+        """
+        Recursively transforms the actions dict into a JSON-compatible dict
+        by replacing methods with their name. Doesn't modify the original dict.
+        """
+
+        def _transform(actions: dict):
+            new_actions = {}
+            for key, value in actions.items():
+                if key == 'method':
+                    new_actions[key] = value.__name__
+                elif isinstance(value, dict):
+                    new_actions[key] = _transform(value)
+                else:
+                    new_actions[key] = value
+            return new_actions
 
-    def action_exec_input(self, data):
-        self.update(data['input index'])
+        return _transform(actions)
 
     """
-    specifications of ryvencore.Node's default behavior:
+    serialization
     """
 
-    # @override
-    def update(self, inp=-1):
-        RC_Node.update(self, inp)
-        self.updated.emit()
-
-    # @override
-    def create_input(self, label: str = '', type_: str = 'data', add_data={}, insert: int = None):
-        RC_Node.create_input(self, label=label, type_=type_, add_data=add_data, insert=insert)
-
-        if insert is not None:
-
-            if insert < 0:
-                index = insert-1
-            else:
-                index = insert
-
-            self.input_added.emit(self.inputs[index], insert)
-
-        else:
-            self.input_added.emit(self.inputs[-1], None)
-
-    # @override
-    def create_input_dt(self, dtype: DType, label: str = '', add_data={}, insert: int = None):
-        RC_Node.create_input_dt(self, dtype=dtype, label=label, add_data=add_data, insert=insert)
-
-        if insert is not None:
-
-            if insert < 0:
-                index = insert-1
-            else:
-                index = insert
-
-            self.input_added.emit(self.inputs[index], insert)
-        else:
-            self.input_added.emit(self.inputs[-1], None)
-
-    # @override
-    def rename_input(self, index: int, label: str):
-        RC_Node.rename_input(self, index=index, label=label)
-        self.update_shape()
-
-    # @override
-    def delete_input(self, index):
-        inp = self.inputs[index]
-        RC_Node.delete_input(self, index=index)
-        self.input_removed.emit(inp)
-
-    # @override
-    def create_output(self, label: str = '', type_: str = 'data', insert: int = None):
-        RC_Node.create_output(self, label=label, type_=type_, insert=insert)
-
-        if insert is not None:
-
-            if insert < 0:
-                index = insert-1
-            else:
-                index = insert
-
-            self.output_added.emit(self.outputs[index], insert)
-        else:
-            self.output_added.emit(self.outputs[-1], None)
-
-    # @override
-    def rename_output(self, index: int, label: str):
-        RC_Node.rename_output(self, index=index, label=label)
-        self.update_shape()
-
-    # @override
-    def delete_output(self, index):
-        out = self.outputs[index]
-        RC_Node.delete_output(self, index=index)
-        self.output_removed.emit(out)
-
-    # @override
-    def additional_data(self) -> dict:
+    def data(self):
         return {
-            'special actions': self.get_special_actions_data(self.actions),
+            'actions': self._serialize_actions(self.actions),
             'display title': self.display_title,
         }
 
-    # @override
-    def load_additional_data(self, data: dict):
-        self.actions = self.set_special_actions_data(data['special actions'])
-        self.display_title = data['display title']
-
-    # @override
-    def input(self, index: int):
-        if len(self.inputs[index].connections) == 0 and self.item:
-            iw = self.input_widget(index)
-            return iw.get_val() if iw else None
-        else:
-            return RC_Node.input(self, index)
-
-    # @override
-    def prepare_removal(self):  # gets also subclassed by user
-        if self.main_widget():
-            self.main_widget().remove_event()
-        RC_Node.prepare_removal(self)
+    def load(self, data):
+        if 'actions' in data:   # otherwise keep default
+            self.actions = self._deserialize_actions(data['actions'])
+        if 'display title' in data:
+            self.display_title = data['display title']
 
+        if 'special actions' in data:   # backward compatibility
+            self.actions = self._deserialize_actions(data['special actions'])
 
     """
-    additional stuff for GUI access:
-    [everything below is pure ryvencore-qt API]
+    GUI access methods
     """
 
-
     def set_display_title(self, t: str):
         self.display_title = t
         self.update_shape()
 
-
     def flow_view(self):
-        """Returns the registered FlowView of the parent script, but None if the view isn't existent
-        which can happen if you call this early"""
-
-        return self.session.flow_views[self.flow.script] if self.flow.script in self.session.flow_views else None
-
+        return self.item.flow_view
 
     def main_widget(self):
         """Returns the main_widget object, or None if the item doesn't exist (yet)"""
-        if self.item:
-            return self.item.main_widget
-        else:
-            return None
 
+        return self.item.main_widget
 
-    def has_main_widget(self):
-        return self.main_widget() is not None
+    def attach_input_widgets(self, widget_names: List[str]):
+        """Attaches the input widget to the next created input."""
 
+        for w in widget_names:
+            self._next_input_widgets.queue(w)
 
     def input_widget(self, index: int):
         """Returns a reference to the widget of the corresponding input"""
 
-        return self.port_item(self.inputs[index]).widget
-
-
-    def session_stylesheet(self) -> str:
-        """Returns the registered stylesheet of the session"""
-
-        return self.session.design.global_stylesheet
-
-
-    def port_item(self, port_obj):
-        """Returns the port item object associated with a given port object"""
-
-        if port_obj in self.inputs:
-            return self.item.inputs[self.inputs.index(port_obj)]
-        elif port_obj in self.outputs:
-            return self.item.outputs[self.outputs.index(port_obj)]
-        return None
+        return self.item.inputs[index].widget
 
+    def session_stylesheet(self):
+        return self.session_gui.design.global_stylesheet
 
     def update_shape(self):
         """Causes recompilation of the whole shape of the GUI item."""
 
         self.update_shape_triggered.emit()
 
-
     def hide_unconnected_ports(self):
-        """Causes the GUI item to hide all unconnected ports"""
+        """Hides all ports that are not connected to anything."""
 
-        del self.default_actions['hide unconnected ports']
-        self.default_actions['show unconnected ports'] = {'method': self.show_unconnected_ports}
+        del self.actions['hide unconnected ports']
+        self.actions['show unconnected ports'] = {'method': self.show_unconnected_ports}
         self.hide_unconnected_ports_triggered.emit()
 
-
     def show_unconnected_ports(self):
-        """Causes the GUI item to show all unconnected ports that have been hidden previously"""
+        """Shows all ports that are not connected to anything."""
 
-        del self.default_actions['show unconnected ports']
-        self.default_actions['hide unconnected ports'] = {'method': self.hide_unconnected_ports}
+        del self.actions['show unconnected ports']
+        self.actions['hide unconnected ports'] = {'method': self.hide_unconnected_ports}
         self.show_unconnected_ports_triggered.emit()
 
-
     def change_title(self):
         from qtpy.QtWidgets import QDialog, QVBoxLayout, QLineEdit
 
         class ChangeTitleDialog(QDialog):
             def __init__(self, title):
                 super().__init__()
                 self.new_title = None
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowCommands.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowCommands.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """
 This file contains the implementations of undoable actions for FlowView.
-
-Why not in Flow?
--> Because there are actions that only regard the GUI and are therefore unnoticed by the Flow but still undoable, like
-adding a DrawingObject.
-
-The main characteristic of these implementations is that the communication to the Flow is down through the threading
-interface, because these actions and the Flow might live in different threads.
 """
 
 
 from qtpy.QtCore import QObject, QPointF
 from qtpy.QtWidgets import QUndoCommand
 
 from .drawings.DrawingObject import DrawingObject
 from .nodes.NodeItem import NodeItem
+from typing import Tuple
+from ryvencore.NodePort import NodePort, NodeInput, NodeOutput
 
 
 class FlowUndoCommand(QObject, QUndoCommand):
     """
     The main difference to normal QUndoCommands is the activate feature. This allows the flow widget to add the
     undo command to the undo stack before redo() is called. This is important since some of these commands can cause
     other commands to be added while they are performing redo(), so to prevent those commands to be added to the
@@ -52,28 +47,14 @@
         pass
 
     def undo_(self):
         """subclassed"""
         pass
 
 
-    def call(self, target_method, args: tuple, then=None):
-        """Calls the backend thread to execute some method and runs 'then' with the response if provided"""
-
-        # disable threading for now
-        ret = target_method(*args)
-        if then is not None:
-            then(ret)
-
-        # ret = self.flow_view.thread_interface.run(target_method, args)
-        #
-        # if then is not None:
-        #     then(ret)
-
-
 class MoveComponents_Command(FlowUndoCommand):
     def __init__(self, flow_view, items_list, p_from, p_to):
         super(MoveComponents_Command, self).__init__(flow_view)
 
         self.items_list = items_list
         self.p_from = p_from
         self.p_to = p_to
@@ -103,31 +84,22 @@
     def __init__(self, flow_view, node_class, pos):
         super().__init__(flow_view)
 
         self.node_class = node_class
         self.node = None
         self.item_pos = pos
 
-        self.flow_view.node_placed.connect(self.node_placed_in_flow_view)
-
     def undo_(self):
-        self.call(self.flow.remove_node, (self.node,))
+        self.flow.remove_node(self.node)
 
     def redo_(self):
         if self.node:
-            self.call(self.flow.add_node, (self.node,))
+            self.flow.add_node(self.node)
         else:
-            self.flow_view.node_placed.connect(self.node_placed_in_flow_view)
-            self.call(self.flow.create_node, (self.node_class,))
-
-        # --> node_placed_in_flow_view()
-
-    def node_placed_in_flow_view(self, node):
-        self.flow_view.node_placed.disconnect(self.node_placed_in_flow_view)
-        self.node = node
+            self.node = self.flow.create_node(self.node_class)
 
 
 class PlaceDrawing_Command(FlowUndoCommand):
     def __init__(self, flow_view, posF, drawing):
         super().__init__(flow_view)
 
         self.drawing = drawing
@@ -164,35 +136,34 @@
                 self.node_items.append(i)
                 self.nodes.append(i.node)
             elif isinstance(i, DrawingObject):
                 self.drawings.append(i)
 
         for n in self.nodes:
             for i in n.inputs:
-                for c in i.connections:
-                    cp = c.out
+                cp = n.flow.connected_output(i)
+                if cp is not None:
                     cn = cp.node
                     if cn not in self.nodes:
-                        self.broken_connections.append(c)
+                        self.broken_connections.append((cp, i))
                     else:
-                        self.internal_connections.add(c)
+                        self.internal_connections.add((cp, i))
             for o in n.outputs:
-                for c in o.connections:
-                    cp = c.inp
+                for cp in n.flow.connected_inputs(o):
                     cn = cp.node
                     if cn not in self.nodes:
-                        self.broken_connections.append(c)
+                        self.broken_connections.append((o, cp))
                     else:
-                        self.internal_connections.add(c)
+                        self.internal_connections.add((o, cp))
 
     def undo_(self):
 
         # add nodes
         for n in self.nodes:
-            self.call(self.flow.add_node, (n,))
+            self.flow.add_node(n)
 
         # add drawings
         for d in self.drawings:
             self.flow_view.add_drawing(d)
 
         # add connections
         self.restore_broken_connections()
@@ -202,78 +173,73 @@
 
         # remove connections
         self.remove_broken_connections()
         self.remove_internal_connections()
 
         # remove nodes
         for n in self.nodes:
-            self.call(self.flow.remove_node, (n,))
+            self.flow.remove_node(n)
 
         # remove drawings
         for d in self.drawings:
             self.flow_view.remove_drawing(d)
 
     def restore_internal_connections(self):
         for c in self.internal_connections:
-            self.call(self.flow.add_connection, (c,))
+            self.flow.add_connection(c)
 
     def remove_internal_connections(self):
         for c in self.internal_connections:
-            self.call(self.flow.remove_connection, (c,))
+            self.flow.remove_connection(c)
 
     def restore_broken_connections(self):
         for c in self.broken_connections:
-            self.call(self.flow.add_connection, (c,))
+            self.flow.add_connection(c)
 
     def remove_broken_connections(self):
         for c in self.broken_connections:
-            self.call(self.flow.remove_connection, (c,))
+            self.flow.remove_connection(c)
 
 
 class ConnectPorts_Command(FlowUndoCommand):
 
     def __init__(self, flow_view, out, inp):
         super().__init__(flow_view)
 
         # CAN ALSO LEAD TO DISCONNECT INSTEAD OF CONNECT!!
 
         self.out = out
         self.inp = inp
         self.connection = None
         self.connecting = True
 
-        for c in self.out.connections:
-            if c.inp == self.inp:
-                self.connection = c
+        for i in flow_view.flow.connected_inputs(out):
+            if i == self.inp:
+                self.connection = (out, i)
                 self.connecting = False
 
 
     def undo_(self):
         if self.connecting:
             # remove connection
-            self.call(self.flow.remove_connection, (self.connection,))
+            self.flow.remove_connection(self.connection)
         else:
             # recreate former connection
-            self.call(self.flow.add_connection, (self.connection,))
+            self.flow.add_connection(self.connection)
 
     def redo_(self):
         if self.connecting:
             if self.connection:
-                self.call(self.flow.add_connection, (self.connection,))
+                self.flow.add_connection(self.connection)
             else:
                 # connection hasn't been created yet
-                self.flow.connection_added.connect(self.connection_created)
-                self.call(self.flow.connect_nodes, (self.out, self.inp))
+                self.connection = self.flow.connect_nodes(self.out, self.inp)
         else:
             # remove existing connection
-            self.call(self.flow.remove_connection, (self.connection,))
-
-    def connection_created(self, c):
-        self.flow.connection_added.disconnect(self.connection_created)
-        self.connection = c
+            self.flow.remove_connection(self.connection)
 
 
 
 
 class Paste_Command(FlowUndoCommand):
 
     def __init__(self, flow_view, data, offset_for_middle_pos):
@@ -296,35 +262,41 @@
 
     def redo_(self):
         if self.pasted_components is None:
             self.pasted_components = {}
 
             # create components
             self.create_drawings()
-            self.call(self.flow.create_nodes_from_data, (self.data['nodes'],),
-                      then=self.nodes_created)
-            # --> nodes_created()
+
+            self.pasted_components['nodes'], self.pasted_components['connections'] = \
+                self.flow.load_components(
+                    nodes_data=self.data['nodes'],
+                    conns_data=self.data['connections'],
+                    output_data=self.data['output data'],
+                )
+
+            self.select_new_components_in_view()
         else:
             self.add_existing_components()
 
     def undo_(self):
         # remove components and their items from flow
-        for n in self.pasted_components['nodes']:
-            self.call(self.flow.remove_node, (n,))
         for c in self.pasted_components['connections']:
-            self.call(self.flow.remove_connection, (c,))
+            self.flow.remove_connection(c)
+        for n in self.pasted_components['nodes']:
+            self.flow.remove_node(n)
         for d in self.pasted_components['drawings']:
             self.flow_view.remove_drawing(d)
 
     def add_existing_components(self):
         # add existing components and items to flow
         for n in self.pasted_components['nodes']:
-            self.call(self.flow.add_node, (n,))
+            self.flow.add_node(n)
         for c in self.pasted_components['connections']:
-            self.call(self.flow.add_connection, (c,))
+            self.flow.add_connection(c)
         for d in self.pasted_components['drawings']:
             self.flow_view.add_drawing(d)
 
         self.select_new_components_in_view()
 
     def select_new_components_in_view(self):
         self.flow_view.clear_selection()
@@ -332,28 +304,14 @@
             d: DrawingObject
             d.setSelected(True)
         for n in self.pasted_components['nodes']:
             n: NodeItem
             ni: NodeItem = self.flow_view.node_items[n]
             ni.setSelected(True)
 
-
-
-
-    def nodes_created(self, nodes):
-        self.pasted_components['nodes'] = nodes
-        self.call(self.flow.connect_nodes_from_data, (nodes, self.data['connections']),
-                  then=self.connections_created)
-        # --> connections_created()
-
-    def connections_created(self, connections):
-        self.pasted_components['connections'] = connections
-
-        self.select_new_components_in_view()
-
     def create_drawings(self):
         drawings = []
         for d in self.data['drawings']:
             new_drawing = self.flow_view.create_drawing(d)
             self.flow_view.add_drawing(new_drawing, posF=QPointF(d['pos x'], d['pos y']))
             drawings.append(new_drawing)
         self.pasted_components['drawings'] = drawings
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowTheme.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowTheme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 from qtpy.QtCore import Qt, QPointF, QPoint, QRectF, QMargins, QMarginsF
 from qtpy.QtGui import QColor, QPainter, QBrush, QRadialGradient, QLinearGradient, QPen, QPainterPath, QFont, QPolygon
 from qtpy.QtWidgets import QStyle, QStyleOption
 
 from ..utils import pythagoras
 
 
+#
+#   notice: available themes are hardcoded in Ryven for CLI; make sure to update those
+#   in case of changes affecting it
+#
+
+
 class FlowTheme:
-    # STATIC ATTRIBUTES
+
     name = ''
     type_ = 'dark'
 
     node_selection_stylesheet__base = '''
 QScrollArea {
     border: 0px solid grey;
     border-radius: 0px;
@@ -69,43 +75,43 @@
 
             elif k == 'flow background color':
                 self.flow_background_brush.setColor(self.hex_to_col(v))
 
     def build_node_selection_stylesheet(self):
         return self.node_selection_stylesheet__base + '\n' + self.node_selection_stylesheet
 
-    def paint_NI_title_label(self, node, selected: bool, hovering: bool, painter: QPainter, option: QStyleOption,
+    def paint_NI_title_label(self, node_gui, selected: bool, hovering: bool, painter: QPainter, option: QStyleOption,
                              node_style: str, node_title: str, node_color: QColor, node_item_bounding_rect):
         pass
 
-    def paint_PI_label(self, node, painter: QPainter, option: QStyleOption, type_: str, connected: bool, label_str: str,
+    def paint_PI_label(self, node_gui, painter: QPainter, option: QStyleOption, type_: str, connected: bool, label_str: str,
                        node_color: QColor, bounding_rect: QRectF):
         pass
 
-    def paint_PI(self, node, painter: QPainter, option: QStyleOption, node_color: QColor, type_: str, connected: bool,
+    def paint_PI(self, node_gui, painter: QPainter, option: QStyleOption, node_color: QColor, type_: str, connected: bool,
                  rect: QRectF):  # padding, w, h):
         pass
 
-    def paint_NI(self, node,
+    def paint_NI(self, node_gui,
                  selected: bool, hovered: bool, node_style: str,
                  painter: QPainter, option: QStyleOption,
                  color: QColor, w, h, bounding_rect, title_rect):
 
         painter.setRenderHint(QPainter.Antialiasing)
 
         if node_style == 'normal':
-            self.draw_NI_normal(node, selected, hovered, painter, color, w, h, bounding_rect, title_rect)
+            self.draw_NI_normal(node_gui, selected, hovered, painter, color, w, h, bounding_rect, title_rect)
         elif node_style == 'small':
-            self.draw_NI_small(node, selected, hovered, painter, color, w, h, bounding_rect)
+            self.draw_NI_small(node_gui, selected, hovered, painter, color, w, h, bounding_rect)
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter: QPainter, c: QColor, w, h, bounding_rect, title_rect):
         pass
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter: QPainter, c: QColor, w, h, bounding_rect, background_color=None):
         pass
 
     def paint_NI_selection_border(self, ni, painter: QPainter, color: QColor, w, h, bounding_rect):
         pen = QPen(self.flow_highlight_pen_color)
         pen.setWidth(3)
         painter.setPen(pen)
@@ -225,15 +231,15 @@
 
     data_conn_color = QColor(188, 187, 242)
     data_conn_width = 5
     data_conn_pen_style = Qt.DashLine
 
     flow_background_brush = QBrush(QColor('#333333'))
 
-    def paint_NI_title_label(self, node, selected, hovering, painter, option, node_style, node_title, node_color,
+    def paint_NI_title_label(self, node_gui, selected, hovering, painter, option, node_style, node_title, node_color,
                              node_item_bounding_rect):
 
         if node_style == 'normal':
             self.paint_NI_title_label_default(
                 painter=painter,
                 node_style=node_style,
                 title=node_title,
@@ -249,31 +255,31 @@
                 title=node_title,
                 color=QColor(30, 43, 48) if not hovering else node_color.lighter(),
                 pen_w=1.5,
                 font=QFont('K2D', 20, QFont.Bold, True),
                 node_item_bounding_rect=node_item_bounding_rect
             )
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         c = QColor('#FFFFFF')
         self.paint_PI_label_default(painter, label_str, c, QFont("Source Code Pro", 10, QFont.Bold), bounding_rect)
 
-    def paint_PI(self, node, painter, option, node_color, type_, connected, rect):
+    def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
         color = QColor('#2E688C') if type_ == 'data' else QColor('#3880ad')
         if option.state & QStyle.State_MouseOver:
             color = color.lighter()
 
         brush = QBrush(QColor(color))
         painter.setBrush(brush)
         painter.setPen(Qt.NoPen)
 
         painter.drawEllipse(rect)
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter: QPainter, c: QColor, w, h, bounding_rect, title_rect):
 
         # main rect
         header_color = QColor(c.red() / 10 + 100, c.green() / 10 + 100, c.blue() / 10 + 100)
         if selected:
             header_color = header_color.lighter()
         body_gradient = QRadialGradient(bounding_rect.topLeft(), pythagoras(h, w))
@@ -288,15 +294,15 @@
                                           FlowTheme_Toy.get_header_rect(w, h, title_rect).bottomLeft())
         header_gradient.setColorAt(0, QColor(c.red(), c.green(), c.blue(), 255))
         header_gradient.setColorAt(1, QColor(c.red(), c.green(), c.blue(), 0))
         painter.setBrush(header_gradient)
         painter.setPen(Qt.NoPen)
         painter.drawRoundedRect(FlowTheme_Toy.get_header_rect(w, h, title_rect), 12, 12)
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter: QPainter, c: QColor, w, h, bounding_rect, background_color=None):
 
         path = QPainterPath()
         path.moveTo(-w / 2, 0)
 
         path.cubicTo(-w / 2, -h / 2,
                      -w / 2, -h / 2,
@@ -336,15 +342,15 @@
 
     data_conn_color = QColor(0, 120, 180)
     data_conn_width = 4
     data_conn_pen_style = Qt.DashLine
 
     flow_background_brush = QBrush(QColor('#333333'))
 
-    def paint_NI_title_label(self, node, selected, hovering, painter, option, node_style, node_title, node_color,
+    def paint_NI_title_label(self, node_gui, selected, hovering, painter, option, node_style, node_title, node_color,
                              node_item_bounding_rect):
         if node_style == 'normal':
             self.paint_NI_title_label_default(
                 painter=painter,
                 node_style=node_style,
                 title=node_title,
                 color=node_color if not (hovering or selected) else node_color.lighter().lighter(),
@@ -359,23 +365,23 @@
                 title=node_title,
                 color=node_color,
                 pen_w=2,
                 font=QFont('K2D', 20, QFont.Bold, True),
                 node_item_bounding_rect=node_item_bounding_rect
             )
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         if type_ == 'exec':
             c = QColor('#FFFFFF')
         else:
             c = node_color
 
         self.paint_PI_label_default(painter, label_str, c, QFont("Source Code Pro", 10, QFont.Bold), bounding_rect)
 
-    def paint_PI(self, node, painter, option, node_color, type_, connected, rect):
+    def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
         color = QColor('#FFFFFF') if type_ == 'exec' else node_color
         pen = QPen(color)
         pen.setWidth(2)
         painter.setPen(pen)
         if connected or \
                 option.state & QStyle.State_MouseOver:  # also fill when mouse hovers
@@ -399,15 +405,15 @@
     #         self.draw_NI_normal(node, painter, color, w, h, bounding_rect, title_rect)
     #     elif node_style == 'small':
     #         if option.state & QStyle.State_MouseOver:  # use special dark background color when mouse hovers
     #             self.draw_NI_small(node, painter, color, w, h, bounding_rect, color.darker())
     #         else:
     #             self.draw_NI_small(node, painter, color, w, h, bounding_rect, QColor('#212429'))
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter, c: QColor, w: int, h: int, bounding_rect, title_rect):
 
         background_color = QColor('#212224')
         painter.setBrush(background_color)
         pen = QPen(c if not selected else c.lighter())
         pen.setWidth(2)
         painter.setPen(pen)
@@ -455,15 +461,15 @@
         path.lineTo(-w / 2, header_bottom - c_s)
         path.lineTo(-w / 2 + c_s, header_bottom)
         path.lineTo(+w / 2 - c_s, header_bottom)
         path.lineTo(+w / 2, header_bottom - c_s)
         path.closeSubpath()
         return path
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter: QPainter, c: QColor, w, h, bounding_rect, background_color=None):
 
         if hovered:
             background_color = c.darker()
         else:
             background_color = QColor('#212429')
 
@@ -525,15 +531,15 @@
                 self.node_color = self.hex_to_col(v)
             elif k == 'small nodes color':
                 self.node_small_color = self.hex_to_col(v)
             elif k == 'flow background color':
                 self.flow_background_color = self.hex_to_col(v)
                 self.flow_background_brush = QBrush(self.flow_background_color)
 
-    def paint_NI_title_label(self, node, selected, hovering, painter, option, node_style, node_title, node_color,
+    def paint_NI_title_label(self, node_gui, selected, hovering, painter, option, node_style, node_title, node_color,
                              node_item_bounding_rect):
 
         if node_style == 'normal':
             self.paint_NI_title_label_default(
                 painter=painter,
                 node_style=node_style,
                 title=node_title,
@@ -549,23 +555,23 @@
                 title=node_title,
                 color=node_color,
                 pen_w=2,
                 font=QFont('K2D', 20, QFont.Bold, True),
                 node_item_bounding_rect=node_item_bounding_rect
             )
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         if type_ == 'exec':
             c = QColor('#FFFFFF')
         else:
             c = node_color
 
         self.paint_PI_label_default(painter, label_str, c, QFont("Source Code Pro", 10, QFont.Bold), bounding_rect)
 
-    def paint_PI(self, node, painter, option, node_color, type_, connected, rect):
+    def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
         color = QColor('#FFFFFF') if type_ == 'exec' else node_color
 
         if type_ == 'exec':
             if connected or \
                     option.state & QStyle.State_MouseOver:  # also fill when mouse hovers
                 brush = QBrush(QColor(255, 255, 255, 100))
@@ -598,15 +604,15 @@
     #         self.draw_NI_normal(node, painter, color, w, h, bounding_rect, title_rect)
     #     elif node_style == 'small':
     #         if option.state & QStyle.State_MouseOver:  # use special dark background color when mouse hovers
     #             self.draw_NI_small(node, painter, color, w, h, bounding_rect, background_color=color.darker())
     #         else:
     #             self.draw_NI_small(node, painter, color, w, h, bounding_rect)
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter, c, w, h, bounding_rect, title_rect):
 
         background_color = self.node_color
 
         # body_gradient = QRadialGradient(QPointF(bounding_rect.topLeft().x() + w,
         #                                         bounding_rect.topLeft().y() - h),
         #                                 pythagoras(2 * h, 2 * w))
@@ -634,15 +640,15 @@
         path.lineTo(-w / 2, +h / 2 - c_s)
         path.lineTo(-w / 2 + c_s, +h / 2)
         path.lineTo(+w / 2 - c_s, +h / 2)
         path.lineTo(+w / 2, +h / 2 - c_s)
         path.closeSubpath()
         return path
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter, c, w, h, bounding_rect, background_color=None):
 
         background_color = self.node_small_color
         c_s = 10  # corner size
 
         path = self.get_extended_body_path(c_s, w, h)  # equals the small in this case
 
@@ -688,15 +694,15 @@
         for k, v in imported.items():
             if k == 'nodes color':
                 self.node_color = self.hex_to_col(v)
             elif k == 'flow background color':
                 self.flow_background_color = self.hex_to_col(v)
                 self.flow_background_brush = QBrush(self.flow_background_color)
 
-    def paint_NI_title_label(self, node, selected, hovering, painter, option, node_style, node_title, node_color,
+    def paint_NI_title_label(self, node_gui, selected, hovering, painter, option, node_style, node_title, node_color,
                              node_item_bounding_rect):
         if node_style == 'normal':
             self.paint_NI_title_label_default(
                 painter=painter,
                 node_style=node_style,
                 title=node_title,
                 color=QColor('#FFFFFF'),
@@ -711,23 +717,23 @@
                 title=node_title,
                 color=node_color,
                 pen_w=2,
                 font=QFont('Segoe UI', 15, QFont.Bold, True),
                 node_item_bounding_rect=node_item_bounding_rect
             )
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         if type_ == 'exec':
             c = QColor('#FFFFFF')
         else:
             c = node_color
 
         self.paint_PI_label_default(painter, label_str, c, QFont("Source Code Pro", 10, QFont.Bold), bounding_rect)
 
-    def paint_PI(self, node, painter, option, node_color, type_, connected, rect):
+    def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
         color = QColor('#FFFFFF') if type_ == 'exec' else node_color
 
         painter.setBrush(QBrush(color))
 
         # if type_ == 'exec':
         #     if connected or \
@@ -748,15 +754,15 @@
         #         painter.setBrush(Qt.NoBrush)
 
         pen = QPen(color)
         pen.setWidth(1)
         painter.setPen(pen)
         painter.drawEllipse(rect.marginsRemoved(QMarginsF(2, 2, 2, 2)))
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter, c, w, h, bounding_rect, title_rect):
 
         background_color = self.node_color
         header_color = QColor(c.red(), c.green(), c.blue(), 180)
         if selected:
             header_color = header_color.lighter()
 
@@ -772,15 +778,15 @@
         painter.setPen(
             Qt.NoPen
             if not selected else
             QPen(QColor(200, 200, 200))
         )
         painter.drawRoundedRect(bounding_rect, self.corner_radius_normal, self.corner_radius_normal)
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter, c, w, h, bounding_rect, background_color=None):
 
         background_color = QColor('#212429')
         painter.setBrush(self.interpolate_color(c, background_color, 0.97))
         painter.setPen(
             QPen(c)
             if not selected else
@@ -825,15 +831,15 @@
                 self.node_background_color = self.hex_to_col(v)
             elif k == 'small nodes background color':
                 self.node_small_background_color = self.hex_to_col(v)
             elif k == 'flow background color':
                 self.flow_background_color = self.hex_to_col(v)
                 self.flow_background_brush = QBrush(self.flow_background_color)
 
-    def paint_NI_title_label(self, node, selected, hovering, painter, option, node_style, node_title, node_color,
+    def paint_NI_title_label(self, node_gui, selected, hovering, painter, option, node_style, node_title, node_color,
                              node_item_bounding_rect):
         if node_style == 'normal':
             self.paint_NI_title_label_default(
                 painter=painter,
                 node_style=node_style,
                 title=node_title,
                 color=QColor('#312b29'),
@@ -848,27 +854,27 @@
                 title=node_title,
                 color=node_color,
                 pen_w=2,
                 font=QFont('Poppins', 15, QFont.Thin),
                 node_item_bounding_rect=node_item_bounding_rect
             )
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         c = None
         if not connected:
             c = QColor('#53585c')
         else:
             if type_ == 'exec':
                 c = QColor('#cccccc')
             else:
                 c = node_color
 
         self.paint_PI_label_default(painter, label_str, c, QFont("Courier New", 10, QFont.Bold), bounding_rect)
 
-    def paint_PI(self, node, painter, option, node_color, type_, connected, rect):
+    def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
         color = None
         if not connected:
             color = QColor('#53585c')
         else:
             if type_ == 'exec':
                 color = QColor('#dddddd')
@@ -896,15 +902,15 @@
         brush = QBrush(QColor(color))
         painter.setBrush(brush)
         painter.setPen(Qt.NoPen)
 
         painter.drawEllipse(rect.marginsRemoved(QMarginsF(2, 2, 2, 2)))
         # painter.drawEllipse(QRectF(padding+w/8, padding+h/8, 3*w/4, 3*h/4))
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter, c, w, h, bounding_rect, title_rect):
 
         background_color = self.node_background_color
 
         if selected:
             header_color = c.lighter()
         else:
@@ -917,15 +923,15 @@
         gradient.setColorAt(rel_header_height + 0.0001, background_color)
         gradient.setColorAt(1, background_color)
 
         painter.setBrush(gradient)
         painter.setPen(Qt.NoPen)  # QPen(c.darker()))
         painter.drawRoundedRect(bounding_rect, 9, 9)
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter, c, w, h, bounding_rect, background_color=None):
 
         background_color = self.node_small_background_color
         c_s = 10
         painter.setBrush(self.interpolate_color(c, background_color, 0.97))
         painter.setPen(Qt.NoPen)
         painter.drawRoundedRect(bounding_rect, c_s, c_s)
@@ -967,15 +973,15 @@
                 self.nodes_background_color = c
             elif k == 'small nodes background color':
                 self.small_nodes_background_color = self.hex_to_col(v)
             elif k == 'flow background color':
                 self.flow_background_color = self.hex_to_col(v)
                 self.flow_background_brush = QBrush(self.flow_background_color)
 
-    def paint_NI_title_label(self, node, selected, hovering, painter, option, node_style, node_title, node_color,
+    def paint_NI_title_label(self, node_gui, selected, hovering, painter, option, node_style, node_title, node_color,
                              node_item_bounding_rect):
         if node_style == 'normal':
             painter.setPen(QPen(QColor(node_color.name())))
             painter.setFont(QFont('Poppins', 13))
             painter.drawText(node_item_bounding_rect, Qt.AlignLeft | Qt.AlignVCenter, node_title)
         else:
             self.paint_NI_title_label_default(
@@ -984,28 +990,28 @@
                 title=node_title,
                 color=node_color,
                 pen_w=2,
                 font=QFont('Poppins', 15, QFont.Thin),
                 node_item_bounding_rect=node_item_bounding_rect
             )
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
 
         c = None
         if not connected:
             c = QColor('#53585c')
         else:
             if type_ == 'exec':
                 c = QColor('#cccccc')
             else:
                 c = node_color
 
         self.paint_PI_label_default(painter, label_str, c, QFont("Courier New", 10, QFont.Bold), bounding_rect)
 
-    def paint_PI(self, node, painter, option, node_color, type_, connected, rect):
+    def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
         color = None
         if not connected:
             color = QColor('#53585c')
         else:
             if type_ == 'exec':
                 color = QColor('#dddddd')
@@ -1033,15 +1039,15 @@
         brush = QBrush(QColor(color))
         painter.setBrush(brush)
         painter.setPen(Qt.NoPen)
 
         painter.drawEllipse(rect.marginsRemoved(QMarginsF(2, 2, 2, 2)))
         # painter.drawEllipse(QRectF(padding+w/8, padding+h/8, 3*w/4, 3*h/4))
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter, c, w, h, bounding_rect: QRectF, title_rect):
 
         if selected:
             background_color = self.interpolate_color(self.nodes_background_color, c.darker(), 0.18)
         else:
             background_color = self.nodes_background_color
 
@@ -1058,15 +1064,15 @@
         painter.setBrush(QBrush(background_color))
         painter.setPen(Qt.NoPen)  # QPen(c.darker()))
         painter.drawRoundedRect(QRectF(
             QPointF(bounding_rect.left(), bounding_rect.top() + header_height),
             bounding_rect.bottomRight()
         ), 6, 6)
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter, c, w, h, bounding_rect, background_color=None):
         background_color = self.small_nodes_background_color
         c_s = 10  # corner size
         painter.setBrush(self.interpolate_color(c, background_color, 0.97))
         painter.setPen(Qt.NoPen)
         painter.drawRoundedRect(bounding_rect, c_s, c_s)
 
@@ -1112,41 +1118,41 @@
             elif k == 'small node background color':
                 self.node_small_bg_col = self.hex_to_col(v)
             elif k == 'node title color':
                 self.node_title_color = self.hex_to_col(v)
             elif k == 'port pin pen color':
                 self.port_pin_pen_color = self.hex_to_col(v)
 
-    def paint_NI_title_label(self, node, selected, hovering, painter, option, node_style, node_title, node_color,
+    def paint_NI_title_label(self, node_gui, selected, hovering, painter, option, node_style, node_title, node_color,
                              node_item_bounding_rect):
 
         painter.setPen(QPen(self.node_title_color))
 
         if node_style == 'normal':
             painter.setFont(QFont('Segoe UI', 11))
             align = Qt.AlignLeft | Qt.AlignVCenter
         else:
             painter.setFont(QFont('Segoe UI', 15))
             align = Qt.AlignCenter
 
         painter.drawText(node_item_bounding_rect, align, node_title)
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         c = None
         if not connected:
             c = QColor('#53585c')
         else:
             if type_ == 'exec':
                 c = QColor('#cccccc')
             else:
                 c = node_color
 
         self.paint_PI_label_default(painter, label_str, c, QFont("Segoe UI", 10), bounding_rect)
 
-    def paint_PI(self, node, painter, option, node_color, type_, connected, rect):
+    def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
         if connected:
             painter.setBrush(QColor('#508AD8'))
             painter.setPen(Qt.NoPen)
         else:
             painter.setBrush(Qt.NoBrush)
             p = QPen(self.port_pin_pen_color)
@@ -1155,15 +1161,15 @@
 
         # rect = QRectF(padding + w / 8, padding + h / 8, 3 * w / 4, 3 * h / 4)
         if type_ == 'exec':
             painter.setBrush(QBrush(QColor('white')))
         # painter.drawEllipse(rect)
         painter.drawEllipse(rect.marginsRemoved(QMarginsF(2, 2, 2, 2)))
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter, c, w, h, bounding_rect: QRectF, title_rect):
 
         if selected:
             background_color = self.interpolate_color(self.node_normal_bg_col, c.darker(), 0.18)
         else:
             background_color = self.node_normal_bg_col
 
@@ -1180,15 +1186,15 @@
         p.setWidthF(2.3)
         painter.setPen(p)
         painter.drawLine(
             QPointF(bounding_rect.left(), bounding_rect.top() + header_height),
             QPointF(bounding_rect.right(), bounding_rect.top() + header_height)
         )
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter, c, w, h, bounding_rect, background_color=None):
 
         painter.setBrush(QBrush(self.node_small_bg_col))
         painter.setPen(Qt.NoPen)
         painter.drawRoundedRect(bounding_rect, 4, 4)
 
 
@@ -1253,55 +1259,55 @@
 
         for k, v in imported.items():
             if k == 'node title color':
                 self.node_title_color = self.hex_to_col(v)
             elif k == 'port pin pen color':
                 self.port_pin_pen_color = self.hex_to_col(v)
 
-    def paint_NI_title_label(self, node, selected, hovering, painter, option, node_style, node_title, node_color,
+    def paint_NI_title_label(self, node_gui, selected, hovering, painter, option, node_style, node_title, node_color,
                              node_item_bounding_rect):
 
         painter.setPen(QPen(self.node_title_color))
 
         if node_style == 'normal':
             painter.setFont(QFont('Segoe UI', 11))
             align = Qt.AlignLeft | Qt.AlignVCenter
         else:
             painter.setFont(QFont('Segoe UI', 15))
             align = Qt.AlignCenter
 
         painter.drawText(node_item_bounding_rect, align, node_title)
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         c = None
         if not connected:
             c = QColor('#dddddd')
         else:
             if type_ == 'exec':
                 c = QColor('#cccccc')
             else:
                 c = node_color
 
         self.paint_PI_label_default(painter, label_str, c, QFont("Segoe UI", 10), bounding_rect)
 
-    def paint_PI(self, node, painter, option, node_color, type_, connected, rect):
+    def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
         if connected:
             painter.setBrush(QColor('#508AD8'))
             painter.setPen(Qt.NoPen)
         else:
             painter.setBrush(Qt.NoBrush)
             p = QPen(self.port_pin_pen_color)
             p.setWidthF(1.1)
             painter.setPen(p)
 
         painter.drawEllipse(rect.marginsRemoved(QMarginsF(2, 2, 2, 2)))
         # painter.drawEllipse(QRectF(padding + w / 8, padding + h / 8, 3 * w / 4, 3 * h / 4))
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter, c, w, h, bounding_rect: QRectF, title_rect):
 
         background_color = c
         background_color.setAlpha(150)
 
         if selected:
             header_color = QColor(c.red(), c.green(), c.blue(), 130)
@@ -1315,15 +1321,15 @@
         gradient.setColorAt(rel_header_height + 0.0001, background_color)
         gradient.setColorAt(1, background_color)
 
         painter.setBrush(gradient)
         painter.setPen(Qt.NoPen)
         painter.drawRoundedRect(bounding_rect, 7, 7)
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter, c, w, h, bounding_rect, background_color=None):
 
         painter.setBrush(QBrush(QColor(c.red(), c.green(), c.blue(), 150)))
         painter.setPen(Qt.NoPen)
         painter.drawRoundedRect(bounding_rect, 8, 8)
 
 
@@ -1341,27 +1347,27 @@
     flow_background_grid = ('points', QColor('#dddddd'), 2, 20, 20)
 
     node_title_color = QColor('#1f1f1f')
     port_pin_pen_color = QColor('#1f1f1f')
 
     node_item_shadow_color = QColor('#cccccc')
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         c = None
         if not connected:
             c = QColor('#1f1f1f')
         else:
             if type_ == 'exec':
                 c = QColor('#cccccc')
             else:
                 c = node_color
 
         self.paint_PI_label_default(painter, label_str, c, QFont("Segoe UI", 10), bounding_rect)
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool, painter, c, w, h, bounding_rect: QRectF, title_rect):
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool, painter, c, w, h, bounding_rect: QRectF, title_rect):
 
         background_color = c.lighter()
         background_color.setAlpha(150)
 
         header_color = QColor(c.red(), c.green(), c.blue(), 130).darker()
 
         rel_header_height = self.get_header_rect(w, h, title_rect).height() / h
@@ -1371,15 +1377,15 @@
         gradient.setColorAt(rel_header_height + 0.0001, background_color)
         gradient.setColorAt(1, background_color)
 
         painter.setBrush(gradient)
         painter.setPen(Qt.NoPen)
         painter.drawRoundedRect(bounding_rect, 7, 7)
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter, c, w, h, bounding_rect, background_color=None):
 
         painter.setBrush(QBrush(QColor(c.red(), c.green(), c.blue(), 150)))
         painter.setPen(Qt.NoPen)
         painter.drawRoundedRect(bounding_rect, 8, 8)
 
 
@@ -1398,15 +1404,15 @@
 
     flow_background_brush = QBrush(QColor(19, 19, 19))
     flow_background_grid = ('points', QColor(80, 80, 80), 2, 30, 30)
 
     node_color = QColor(10, 10, 10, 250)
     node_item_shadow_color = QColor(0, 0, 0)
 
-    def paint_NI_title_label(self, node, selected, hovering, painter, option, node_style, node_title, node_color,
+    def paint_NI_title_label(self, node_gui, selected, hovering, painter, option, node_style, node_title, node_color,
                              node_item_bounding_rect):
         if node_style == 'normal':
             self.paint_NI_title_label_default(
                 painter=painter,
                 node_style=node_style,
                 title=node_title,
                 color=QColor(200, 200, 200),
@@ -1421,19 +1427,19 @@
                 title=node_title,
                 color=node_color,
                 pen_w=2,
                 font=QFont('Segoe UI', 15, QFont.Bold),
                 node_item_bounding_rect=node_item_bounding_rect
             )
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         c = QColor('#FFFFFF')
         self.paint_PI_label_default(painter, label_str, c, QFont("Segoe UI", 8, QFont.Normal), bounding_rect)
 
-    def paint_PI(self, node, painter, option, node_color, type_, connected, rect):
+    def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
         color = QColor('#FFFFFF') if type_ == 'exec' else node_color
 
         # add = 2
         # padd = padding + add
         outer_ellipse_rect = rect.marginsRemoved(QMarginsF(2, 2, 2, 2))  # QRectF(padd, padd, w - 2*padd, h - 2*padd)
         # add = 4
@@ -1470,15 +1476,15 @@
                 painter.setBrush(brush)
                 painter.drawEllipse(inner_ellipse_rect)
 
             # draw outer ellipse
             painter.setBrush(Qt.NoBrush)
             painter.drawEllipse(outer_ellipse_rect)
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter, c, w, h, bounding_rect, title_rect):
 
         background_color = QColor(14, 14, 14)
         header_color = QColor(105, 105, 105, 150)
 
         rel_header_height = self.get_header_rect(w, h, title_rect).height() / h
         gradient = QLinearGradient(bounding_rect.topLeft(), bounding_rect.bottomLeft())
@@ -1487,15 +1493,15 @@
         gradient.setColorAt(rel_header_height + 0.0001, background_color)
         gradient.setColorAt(1, background_color)
 
         painter.setBrush(gradient)
         painter.setPen(Qt.NoPen)  # QPen(c.darker())
         painter.drawRoundedRect(bounding_rect, 2, 2)
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter, c, w, h, bounding_rect, background_color=None):
 
         background_color = QColor(217, 217, 217, 50)
         c_s = 2
         painter.setBrush(self.interpolate_color(c, background_color, 0.97))
         pen = QPen(QColor(130, 130, 130))
         painter.setPen(pen)
@@ -1527,38 +1533,38 @@
     node_small_bg_col = QColor('#cccdcf')
     node_title_color = QColor('#1f1f1f')
     port_pin_pen_color = QColor('#1f1f1f')
 
     node_item_shadow_color = QColor('#cccccc')
 
 
-    def paint_NI_title_label(self, node, selected, hovering, painter, option, node_style, node_title, node_color,
+    def paint_NI_title_label(self, node_gui, selected, hovering, painter, option, node_style, node_title, node_color,
                              node_item_bounding_rect):
 
         painter.setPen(QPen(self.node_title_color))
 
         if node_style == 'normal':
             painter.setFont(QFont('Segoe UI', 10))
             align = Qt.AlignLeft | Qt.AlignVCenter
         else:
             painter.setFont(QFont('Segoe UI', 12))
             align = Qt.AlignCenter
 
         painter.drawText(node_item_bounding_rect, align, node_title)
 
 
-    def paint_PI_label(self, node, painter, option, type_, connected, label_str, node_color, bounding_rect):
+    def paint_PI_label(self, node_gui, painter, option, type_, connected, label_str, node_color, bounding_rect):
         pen = QPen(QColor('#000000'))
         pen.setWidthF(1.2)
         painter.setPen(pen)
 
         self.paint_PI_label_default(painter, label_str, QColor(0, 0, 0), QFont("Segoe UI", 8), bounding_rect)
 
 
-    def paint_PI(self, node, painter, option, node_color, type_, connected, rect):
+    def paint_PI(self, node_gui, painter, option, node_color, type_, connected, rect):
 
         painter.setBrush(QColor('#000000'))
         painter.setPen(Qt.NoPen)
 
         if type_ == 'data':
             painter.drawEllipse(rect.marginsRemoved(QMarginsF(3, 3, 3, 3)))
         else:
@@ -1567,15 +1573,15 @@
             path.lineTo(QPointF(draw_rect.right(), draw_rect.center().y()))
             path.lineTo(draw_rect.bottomLeft())
             path.closeSubpath()
 
             painter.drawPath(path)
 
 
-    def draw_NI_normal(self, node, selected: bool, hovered: bool,
+    def draw_NI_normal(self, node_gui, selected: bool, hovered: bool,
                        painter, c, w, h, bounding_rect: QRectF, title_rect):
 
         pen = QPen(c)
         col_top = self.node_normal_bg_col.lighter(105)
         col_bottom = self.node_normal_bg_col
 
         if not selected:
@@ -1593,13 +1599,29 @@
         gradient.setColorAt(1, col_bottom)
 
         painter.setBrush(QBrush(gradient))
         painter.setPen(pen)
         painter.drawRoundedRect(bounding_rect, 3, 3)
 
 
-    def draw_NI_small(self, node, selected: bool, hovered: bool,
+    def draw_NI_small(self, node_gui, selected: bool, hovered: bool,
                       painter, c, w, h, bounding_rect, background_color=None):
 
         painter.setBrush(QBrush(self.node_small_bg_col))
         painter.setPen(Qt.NoPen)
         painter.drawRoundedRect(bounding_rect, 4, 4)
+
+
+flow_themes = [
+    FlowTheme_Toy(),
+    FlowTheme_DarkTron(),
+    FlowTheme_Ghost(),
+    FlowTheme_Blender(),
+    FlowTheme_Simple(),
+    FlowTheme_Ueli(),
+    FlowTheme_PureDark(),
+    FlowTheme_Colorful(),
+    FlowTheme_PureLight(),
+    FlowTheme_ColorfulLight(),
+    FlowTheme_Industrial(),
+    FlowTheme_Fusion(),
+]
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowView.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowView.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import json
 
+from typing import Tuple
+
 from qtpy.QtCore import Qt, QPointF, QPoint, QRectF, QSizeF, Signal, QTimer, QTimeLine, QEvent
 from qtpy.QtGui import QPainter, QPen, QColor, QKeySequence, QTabletEvent, QImage, QGuiApplication, QFont, QTouchEvent
 from qtpy.QtWidgets import QGraphicsView, QGraphicsScene, QShortcut, QMenu, QGraphicsItem, QUndoStack
 
 from ryvencore.Flow import Flow
 from ryvencore.Node import Node
-from ryvencore.NodePort import NodePort
-from ryvencore.Connection import Connection, DataConnection
+from ryvencore.NodePort import NodePort, NodeInput, NodeOutput
+#from ryvencore.Connection import Connection, DataConnection
 from ryvencore.InfoMsgs import InfoMsgs
 from ryvencore.RC import PortObjPos
 from ryvencore.utils import node_from_identifier
 
 from ..GUIBase import GUIBase
 from ..utils import *
 from .FlowCommands import MoveComponents_Command, PlaceNode_Command, \
     PlaceDrawing_Command, RemoveComponents_Command, ConnectPorts_Command, Paste_Command, FlowUndoCommand
 from .FlowViewProxyWidget import FlowViewProxyWidget
 from .FlowViewStylusModesWidget import FlowViewStylusModesWidget
 from .node_list_widget.NodeListWidget import NodeListWidget
+from .nodes.NodeGUI import NodeGUI
 from .nodes.NodeItem import NodeItem
 from .nodes.PortItem import PortItemPin, PortItem
 from .connections.ConnectionItem import default_cubic_connection_path, ConnectionItem, DataConnectionItem, \
     ExecConnectionItem
 from .drawings.DrawingObject import DrawingObject
 
 
@@ -31,55 +34,53 @@
 
     nodes_selection_changed = Signal(list)
     node_placed = Signal(Node)
 
     create_node_request = Signal(object, dict)
     remove_node_request = Signal(Node)
 
-    check_connection_validity_request = Signal(NodePort, NodePort, bool)
+    check_connection_validity_request = Signal((NodeOutput, NodeInput), bool)
     connect_request = Signal(NodePort, NodePort)
 
-    get_nodes_data_request = Signal(list)
-    get_connections_data_request = Signal(list)
+    #get_nodes_data_request = Signal(list)
+    #get_connections_data_request = Signal(list)
     get_flow_data_request = Signal()
 
     viewport_update_mode_changed = Signal(str)
 
-    def __init__(self, session, script, flow, load_data=None, flow_size: list = None, parent=None):
+    def __init__(self, session_gui, flow, parent=None):
         GUIBase.__init__(self, representing_component=flow)
         QGraphicsView.__init__(self, parent=parent)
 
-        # UNDO/REDO
+        # UNDO STACK
         self._undo_stack = QUndoStack(self)
         self._undo_action = self._undo_stack.createUndoAction(self, 'undo')
         self._undo_action.setShortcuts(QKeySequence.Undo)
         self._redo_action = self._undo_stack.createRedoAction(self, 'redo')
         self._redo_action.setShortcuts(QKeySequence.Redo)
 
         # SHORTCUTS
         self._init_shortcuts()
 
         # GENERAL ATTRIBUTES
-        self.session = session
-        # self.CLASSES = self.session.CLASSES
-        self.script = script
+        self.session_gui = session_gui
+
         self.flow: Flow = flow
         self.node_items: dict = {}  # {Node: NodeItem}
         self.node_items__cache: dict = {}
         self.connection_items: dict = {}  # {Connection: ConnectionItem}
         self.connection_items__cache: dict = {}
 
         # PRIVATE FIELDS
         self._tmp_data = None
         self._selected_pin: PortItemPin = None
         self._dragging_connection = False
         self._temp_connection_ports = None
         self._waiting_for_connection_request: bool = False
         self.mouse_event_taken = False  # for stylus - see tablet event
-        self._showing_framerate = False
         self._last_mouse_move_pos: QPointF = None
         self._node_place_pos = QPointF()
         self._left_mouse_pressed_in_flow = False
         self._right_mouse_pressed_in_flow = False
         self._mouse_press_pos: QPointF = None
         self._auto_connection_pin = None  # stores the gate that we may try to auto connect to a newly placed NI
         self._panning = False
@@ -92,37 +93,31 @@
             'scene pos': None,
             'delta': 0,
         }
 
         # CONNECTIONS TO FLOW
         self.create_node_request.connect(self.flow.create_node)
         self.remove_node_request.connect(self.flow.remove_node)
-        self.node_placed.connect(self.flow.node_view_placed)
         self.check_connection_validity_request.connect(self.flow.check_connection_validity)
-        self.get_nodes_data_request.connect(self.flow.gen_nodes_data)
-        self.get_connections_data_request.connect(self.flow.gen_conns_data)
+        # TODO: need to check if the 2 lines below are used
+        #self.get_nodes_data_request.connect(self.flow.gen_nodes_data)
+        #self.get_connections_data_request.connect(self.flow.gen_conns_data)
         self.get_flow_data_request.connect(self.flow.data)
 
         # CONNECTIONS FROM FLOW
-        self.flow.node_added.connect(self.add_node)
-        self.flow.node_removed.connect(self.remove_node)
-        self.flow.connection_added.connect(self.add_connection)
-        self.flow.connection_removed.connect(self.remove_connection)
-        self.flow.connection_request_valid.connect(self.connection_request_valid)
-
-        # SESSION THREAD
-        self.thread_interface = self.session.threading_bridge__frontend
+        self.flow.node_added.sub(self.add_node)
+        self.flow.node_removed.sub(self.remove_node)
+        self.flow.connection_added.sub(self.add_connection)
+        self.flow.connection_removed.sub(self.remove_connection)
+        self.flow.connection_request_valid.sub(self.connection_request_valid)
 
         # CREATE UI
         scene = QGraphicsScene(self)
         scene.setItemIndexMethod(QGraphicsScene.NoIndex)
-        if flow_size is None:
-            scene.setSceneRect(0, 0, 10 * self.width(), 10 * self.height())
-        else:
-            scene.setSceneRect(0, 0, flow_size[0], flow_size[1])
+        scene.setSceneRect(0, 0, 10000, 7000)
 
         self.setScene(scene)
         self.setCacheMode(QGraphicsView.CacheBackground)
         self.setViewportUpdateMode(QGraphicsView.BoundingRectViewportUpdate)
         self.setRenderHint(QPainter.Antialiasing)
         self.setTransformationAnchor(QGraphicsView.AnchorUnderMouse)
         self.setDragMode(QGraphicsView.RubberBandDrag)
@@ -131,15 +126,15 @@
 
         self.centerOn(QPointF(self.viewport().width() / 2, self.viewport().height() / 2))
 
         self.scene_rect_width = self.mapFromScene(self.sceneRect()).boundingRect().width()
         self.scene_rect_height = self.mapFromScene(self.sceneRect()).boundingRect().height()
 
         # NODE LIST WIDGET
-        self._node_list_widget = NodeListWidget(self.session)
+        self._node_list_widget = NodeListWidget(self.session_gui)
         self._node_list_widget.setMinimumWidth(260)
         self._node_list_widget.setFixedHeight(300)
         self._node_list_widget.escaped.connect(self.hide_node_list_widget)
         self._node_list_widget.node_chosen.connect(self.create_node__cmd)
 
         self._node_list_widget_proxy = FlowViewProxyWidget(self)
         self._node_list_widget_proxy.setZValue(1000)
@@ -175,55 +170,34 @@
         # recognizer = PanGestureRecognizer()
         # pan_gesture_id = QGestureRecognizer.registerRecognizer(recognizer) <--- CRASH HERE
         # self.grabGesture(pan_gesture_id)
         self.viewport().setAttribute(Qt.WA_AcceptTouchEvents)
         self.last_pinch_points_dist = 0
 
         # DESIGN
-        self.session.design.flow_theme_changed.connect(self._theme_changed)
-        self.session.design.performance_mode_changed.connect(self._perf_mode_changed)
-
-        # FRAMERATE TRACKING
-        self.num_frames = 0
-        self.framerate = 0
-        self.framerate_timer = QTimer(self)
-        self.framerate_timer.timeout.connect(self._on_framerate_timer_timeout)
-
-        # self.show_framerate(m_sec_interval=100)  # for testing
+        self.session_gui.design.flow_theme_changed.connect(self._theme_changed)
+        self.session_gui.design.performance_mode_changed.connect(self._perf_mode_changed)
 
         # DATA
-        if load_data is not None:
-            if 'flow view' in load_data:
-                view_data = load_data['flow view']
-            else:
-                view_data = load_data  # backwards compatibility
-
+        data = self.flow.load_data
+        if data is not None:
+            view_data = data['flow view']
             if 'drawings' in view_data:  # not all (old) project files have drawings arr
                 self.place_drawings_from_data(view_data['drawings'])
-
             if 'view size' in view_data:
                 self.setSceneRect(0, 0, view_data['view size'][0], view_data['view size'][1])
 
             self._undo_stack.clear()
 
         # CATCH UP ON FLOW
         for node in self.flow.nodes:
             self.add_node(node)
-        for c in self.flow.connections:
+        for c in [(o, i) for o, conns in self.flow.graph_adj.items() for i in conns]:
             self.add_connection(c)
 
-    def show_framerate(self, show: bool = True, m_sec_interval: int = 1000):
-        self._showing_framerate = show
-        self.framerate_timer.setInterval(m_sec_interval)
-        self.framerate_timer.start()
-
-    def _on_framerate_timer_timeout(self):
-        self.framerate = self.num_frames
-        self.num_frames = 0
-
     def _init_shortcuts(self):
         place_new_node_shortcut = QShortcut(QKeySequence('Shift+P'), self)
         place_new_node_shortcut.activated.connect(self._place_new_node_by_shortcut)
         move_selected_components_left_shortcut = QShortcut(QKeySequence('Shift+Left'), self)
         move_selected_components_left_shortcut.activated.connect(self._move_selected_comps_left)
         move_selected_components_up_shortcut = QShortcut(QKeySequence('Shift+Up'), self)
         move_selected_components_up_shortcut.activated.connect(self._move_selected_comps_up)
@@ -242,15 +216,15 @@
 
         undo_shortcut = QShortcut(QKeySequence.Undo, self)
         undo_shortcut.activated.connect(self._undo_activated)
         redo_shortcut = QShortcut(QKeySequence.Redo, self)
         redo_shortcut.activated.connect(self._redo_activated)
 
     def _theme_changed(self, t):
-        self._node_list_widget.setStyleSheet(self.session.design.node_selection_stylesheet)
+        self._node_list_widget.setStyleSheet(self.session_gui.design.node_selection_stylesheet)
         for n, ni in self.node_items.items():
             ni.widget.rebuild_ui()
 
         # TODO: repaint background. how?
         self.viewport().update()
         self.scene().update(self.sceneRect())
 
@@ -568,29 +542,29 @@
         try:
             text = str(event.mimeData().data('application/json'), 'utf-8')
             data: dict = json.loads(text)
 
             if data['type'] == 'node':
                 self._node_place_pos = self.mapToScene(event.pos())
                 self.create_node__cmd(
-                    node_from_identifier(data['node identifier'], self.session.nodes)
+                    node_from_identifier(data['node identifier'], self.session_gui.core_session.nodes)
                 )
         except Exception:
             pass
 
     # PAINTING
     def drawBackground(self, painter, rect):
 
-        painter.setBrush(self.session.design.flow_theme.flow_background_brush)
+        painter.setBrush(self.session_gui.design.flow_theme.flow_background_brush)
         painter.drawRect(rect.intersected(self.sceneRect()))
         painter.setPen(Qt.NoPen)
         painter.drawRect(self.sceneRect())
 
-        if self.session.design.performance_mode == 'pretty':
-            theme = self.session.design.flow_theme
+        if self.session_gui.design.performance_mode == 'pretty':
+            theme = self.session_gui.design.flow_theme
             if theme.flow_background_grid and self._current_scale >= 0.7:
                 if theme.flow_background_grid[0] == 'points':
                     color = theme.flow_background_grid[1]
                     pen_width = theme.flow_background_grid[2]
                     diff_x = theme.flow_background_grid[3]
                     diff_y = theme.flow_background_grid[4]
 
@@ -603,24 +577,14 @@
                             painter.drawPoint(x, y)
 
         self.set_stylus_proxy_pos()  # has to be called here instead of in drawForeground to prevent lagging
         # self.set_zoom_proxy_pos()
 
     def drawForeground(self, painter, rect):
 
-        if self._showing_framerate:
-            self.num_frames += 1
-            pen = QPen(QColor('#A9D5EF'))
-            pen.setWidthF(2)
-            painter.setPen(pen)
-
-            pos = self.mapToScene(10, 23)
-            painter.setFont(QFont('Poppins', round(11 * self._total_scale_div)))
-            painter.drawText(pos, "{:.2f}".format(self.framerate))
-
         # DRAW CURRENTLY DRAGGED CONNECTION
         if self._dragging_connection:
             pen = QPen(QColor('#101520'))
             pen.setWidth(3)
             pen.setStyle(Qt.DotLine)
             painter.setPen(pen)
 
@@ -738,15 +702,15 @@
             dialog_pos.setY(dialog_pos.y() - (
                     dialog_pos.y() + self._node_list_widget.height() / self._total_scale_div - self.viewport().height()))
         dialog_pos = self.mapToScene(dialog_pos)
 
         # open nodes dialog
         # the dialog emits 'node_chosen' which is connected to self.place_node__cmd
         self._node_list_widget.update_list(
-            nodes if nodes is not None else self.session.nodes
+            nodes if nodes is not None else self.session_gui.core_session.nodes
         )
         self._node_list_widget_proxy.setPos(dialog_pos)
         self._node_list_widget_proxy.show()
         self._node_list_widget.refocus()
 
     def hide_node_list_widget(self):
         self._node_list_widget_proxy.hide()
@@ -838,26 +802,29 @@
 
         if node in self.node_items__cache.keys():  # load from cache
             # print('using a cached item')
             item = self.node_items__cache[node]
             self._add_node_item(item)
 
         else:  # create new item
-            item_data = node.init_data
-            item = NodeItem(node, params=(self, self.session.design, item_data))
-            node.item = item
+            item = NodeItem(
+                node=node,
+                node_gui=
+                    (node.GUI if hasattr(node, 'GUI') else NodeGUI)     # use custom GUI class if available
+                    ((node, self.session_gui)),                         # calls __init__ of NodeGUI class with tuple arg
+                flow_view=self,
+                design=self.session_gui.design,
+            )
             item.initialize()
+
             self.node_placed.emit(node)
 
-            pos = None
-            if item_data is not None:
-                if 'pos x' in item_data:
-                    pos = QPointF(item_data['pos x'], item_data['pos y'])
-                elif 'position x' in item_data:  # backwards compatibility
-                    pos = QPointF(item_data['position x'], item_data['position y'])
+            item_data = node.load_data
+            if item_data is not None and 'pos x' in item_data:
+                pos = QPointF(item_data['pos x'], item_data['pos y'])
             else:
                 pos = self._node_place_pos
 
             self._add_node_item(item, pos)
 
         # auto connect
         if self._auto_connection_pin:
@@ -883,17 +850,27 @@
     def _remove_node_item(self, item: NodeItem):
         # store item in case the remove action gets undone later
         self.node_items__cache[item.node] = item
         self.scene().removeItem(item)
 
     # CONNECTIONS
     def connect_node_ports__cmd(self, p1: NodePort, p2: NodePort):
-        self._temp_connection_ports = (p1, p2)
-        self._waiting_for_connection_request = True
-        self.check_connection_validity_request.emit(p1, p2, True)
+        # Need to check order of ports since Flow.check_connection_validity needs (NodeOutput, NodeInput)
+        if isinstance(p1, NodeOutput) and isinstance(p2, NodeInput):
+            self._temp_connection_ports = (p1, p2)
+            self._waiting_for_connection_request = True
+            self.check_connection_validity_request.emit((p1, p2), True)
+
+        elif isinstance(p1, NodeInput) and isinstance(p2, NodeOutput):
+            self._temp_connection_ports = (p2, p1)
+            self._waiting_for_connection_request = True
+            self.check_connection_validity_request.emit((p2, p1), True)
+
+        else:
+            self.connection_request_valid(False)
 
     def connection_request_valid(self, valid: bool):
         """
         Triggered after the abstract flow evaluated validity of pending connect request.
         This can also lead to a disconnect!
         """
 
@@ -903,56 +880,52 @@
             return
 
         if valid:
             out, inp = self._temp_connection_ports
             if out.io_pos == PortObjPos.INPUT:
                 out, inp = inp, out
 
-            # remove forbidden connections
-            if inp.type_ == 'data':
-                for c in inp.connections:
-
-                    if c.out == out:
-                        # if the exact connection exists, we want to remove it by command
-                        continue
-
-                    self._push_undo(
-                        ConnectPorts_Command(self, out=c.out, inp=inp)
-                    )
-
-            self._push_undo(
-                ConnectPorts_Command(self, out=out, inp=inp)
-            )
+            if self.flow.connected_output(inp) == out:
+                # if the exact connection exists, we want to remove it by command
+                self._push_undo(
+                    ConnectPorts_Command(self, out=self.flow.connected_output(inp), inp=inp)
+                )
+            else:
+                self._push_undo(
+                    ConnectPorts_Command(self, out=out, inp=inp)
+                )
 
-    def add_connection(self, c: Connection):
+    def add_connection(self, c: Tuple[NodeOutput, NodeInput]):
+        out, inp = c
 
+        #TODO: need to verify that connection_items_cache still works fine with new connection object
         item: ConnectionItem = None
         if c in self.connection_items__cache.keys():
             item = self.connection_items__cache[c]
 
         else:
-            if isinstance(c, DataConnection):
+            if inp.type_ == 'data':
                 # item = self.CLASSES['data conn item'](c, self.session.design)
-                item = DataConnectionItem(c, self.session.design)
+                item = DataConnectionItem(c, self.session_gui.design)
             else:
                 # item = self.CLASSES['exec conn item'](c, self.session.design)
-                item = ExecConnectionItem(c, self.session.design)
+                item = ExecConnectionItem(c, self.session_gui.design)
 
         self._add_connection_item(item)
 
         item.out_item.port_connected()
         item.inp_item.port_connected()
 
     def _add_connection_item(self, item: ConnectionItem):
         self.connection_items[item.connection] = item
         self.scene().addItem(item)
         item.setZValue(10)
         # self.viewport().repaint()
 
-    def remove_connection(self, c: Connection):
+    def remove_connection(self, c: Tuple[NodeOutput, NodeInput]):
         item = self.connection_items[c]
         self._remove_connection_item(item)
 
         item.out_item.port_disconnected()
         item.inp_item.port_disconnected()
 
         del self.connection_items[c]
@@ -971,15 +944,15 @@
         elif p.io_pos == PortObjPos.INPUT:
             for out in n.outputs:
                 if p.type_ == out.type_:
                     # connect exactly once
                     self.connect_node_ports__cmd(p, out)
                     return
 
-    def update_conn_item(self, c: Connection):
+    def update_conn_item(self, c: Tuple[NodeOutput, NodeInput]):
         if c in self.connection_items:
             self.connection_items[c].changed = True
             self.connection_items[c].update()
 
     # DRAWINGS
     def create_drawing(self, data=None) -> DrawingObject:
         """Creates and returns a new DrawingObject."""
@@ -1141,14 +1114,15 @@
             c.setSelected(True)
 
     # ACTIONS
     def _copy(self):  # ctrl+c
         data = {
             'nodes': self._get_nodes_data(self.selected_nodes()),
             'connections': self._get_connections_data(self.selected_nodes()),
+            'output data': self._get_output_data(self.selected_nodes()),
             'drawings': self._get_drawings_data(self.selected_drawings())
         }
         QGuiApplication.clipboard().setText(json.dumps(data))
 
     def _cut(self):  # ctrl+x
         data = {
             'nodes': self._get_nodes_data(self.selected_nodes()),
@@ -1205,34 +1179,24 @@
             'view size': [self.sceneRect().size().width(), self.sceneRect().size().height()]
         }
 
         return data
 
     def _get_nodes_data(self, nodes):
         """generates the data for the specified list of nodes"""
-
-        data = self.thread_interface.run(
-            self.flow.gen_nodes_data, (nodes,)
-        )
-
-        complete_data = self.thread_interface.run(
-            self.flow.complete_data, (data,)
-        )
-
-        return complete_data
+        f_complete_data = self.session_gui.core_session.complete_data
+        return f_complete_data(self.flow._gen_nodes_data(nodes))
 
     def _get_connections_data(self, nodes):
         """generates the connections data for connections between a specified list of nodes"""
+        f_complete_data = self.session_gui.core_session.complete_data
+        return f_complete_data(self.flow._gen_conns_data(nodes))
 
-        data = self.thread_interface.run(
-            self.flow.gen_conns_data, (nodes,)
-        )
-        complete_data = self.thread_interface.run(
-            self.flow.complete_data, (data,)
-        )
-
-        return complete_data
+    def _get_output_data(self, nodes):
+        """generates the serialized data of output ports of the specified nodes"""
+        f_complete_data = self.session_gui.core_session.complete_data
+        return f_complete_data(self.flow._gen_output_data(nodes))
 
     def _get_drawings_data(self, drawings):
         """generates the data for a list of drawings"""
 
         return [d.data() for d in drawings]
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowViewProxyWidget.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowViewProxyWidget.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowViewStylusModesWidget.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowViewStylusModesWidget.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/FlowViewZoomWidget.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/FlowViewZoomWidget.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/connections/ConnectionItem.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/connections/ConnectionItem.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,26 @@
 
 class ConnectionItem(GUIBase, QGraphicsPathItem):
     """The GUI representative for a connection. The classes ExecConnectionItem and DataConnectionItem will be ready
     for reimplementation later, so users can add GUI for the enhancements of DataConnection and ExecConnection,
     like input fields for weights."""
 
     def __init__(self, connection, session_design):
-        GUIBase.__init__(self, representing_component=connection)
+        #GUIBase.__init__(self, representing_component=connection) # ConnectionItem doesn't have a representing component
         QGraphicsPathItem.__init__(self)
 
         self.setAcceptHoverEvents(True)
 
         self.connection = connection
+        out, inp = self.connection
 
-        out = self.connection.out
-        inp = self.connection.inp
-        out_node = out.node
-        inp_node = inp.node
-        self.out_item = out_node.port_item(out)
-        self.inp_item = inp_node.port_item(inp)
+        out_port_index = out.node.outputs.index(out)
+        inp_port_index = inp.node.inputs.index(inp)
+        self.out_item = out.node.gui.item.outputs[out_port_index]
+        self.inp_item = inp.node.gui.item.inputs[inp_port_index]
 
         self.session_design = session_design
         self.session_design.flow_theme_changed.connect(self.recompute)
         self.session_design.performance_mode_changed.connect(self.recompute)
 
         # for rendering flow pictures
         self.setCacheMode(QGraphicsItem.DeviceCoordinateCache)
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/drawings/DrawingObject.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/drawings/DrawingObject.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/node_list_widget/NodeListWidget.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/node_list_widget/NodeListWidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from qtpy.QtWidgets import QWidget, QVBoxLayout, QLineEdit, QScrollArea
 from qtpy.QtCore import Qt, Signal
 
+from ryvencore import Node
 from .utils import search, sort_nodes, inc, dec
 from ..node_list_widget.NodeWidget import NodeWidget
 
 from statistics import median
 
 
 class NodeListWidget(QWidget):
-    """notice, that 'nodes' refers to node CLASSES here"""
 
     # SIGNALS
     escaped = Signal()
     node_chosen = Signal(object)
 
     def __init__(self, session):
         super().__init__()
 
         self.session = session
-        self.nodes = []
+        self.nodes: list[type[Node]] = []
 
         self.current_nodes = []             # currently selectable nodes
         self.active_node_widget_index = -1  # index of focused node widget
         self.active_node_widget = None      # focused node widget
         self.node_widgets = {}              # Node-NodeWidget assignments
         self._node_widget_index_counter = 0
 
-        self.setup_UI()
+        self._setup_UI()
 
 
-    def setup_UI(self):
+    def _setup_UI(self):
 
         self.main_layout = QVBoxLayout(self)
         self.main_layout.setAlignment(Qt.AlignTop)
         self.setLayout(self.main_layout)
 
         # adding all stuff to the layout
         self.search_line_edit = QLineEdit(self)
         self.search_line_edit.setPlaceholderText('search for node...')
-        self.search_line_edit.textChanged.connect(self.update_view)
+        self.search_line_edit.textChanged.connect(self._update_view)
         self.layout().addWidget(self.search_line_edit)
 
 
         self.list_scroll_area = QScrollArea(self)
         self.list_scroll_area.setVerticalScrollBarPolicy(Qt.ScrollBarAsNeeded)
         self.list_scroll_area.setHorizontalScrollBarPolicy(Qt.ScrollBarAsNeeded)
         self.list_scroll_area.setWidgetResizable(True)
@@ -55,15 +55,15 @@
         self.list_layout = QVBoxLayout()
         self.list_layout.setContentsMargins(0, 0, 0, 0)
         self.list_layout.setAlignment(Qt.AlignTop)
         self.list_scroll_area_widget.setLayout(self.list_layout)
 
         self.layout().addWidget(self.list_scroll_area)
 
-        self.update_view('')
+        self._update_view('')
 
         self.setStyleSheet(self.session.design.node_selection_stylesheet)
 
         self.search_line_edit.setFocus()
 
 
     def mousePressEvent(self, event):
@@ -77,25 +77,25 @@
 
         num_items = len(self.current_nodes)
 
         if event.key() == Qt.Key_Escape:
             self.escaped.emit()
 
         elif event.key() == Qt.Key_Down:
-            self.set_active_node_widget_index(
+            self._set_active_node_widget_index(
                 inc(self.active_node_widget_index, length=num_items)
             )
         elif event.key() == Qt.Key_Up:
-            self.set_active_node_widget_index(
+            self._set_active_node_widget_index(
                 dec(self.active_node_widget_index, num_items)
             )
 
         elif event.key() == Qt.Key_Return or event.key() == Qt.Key_Enter:
             if len(self.current_nodes) > 0:
-                self.place_node(self.active_node_widget_index)
+                self._place_node(self.active_node_widget_index)
         else:
             event.setAccepted(False)
 
 
     def wheelEvent(self, event):
         # need to accept the event, so the scene doesn't process it further
         QWidget.wheelEvent(self, event)
@@ -107,18 +107,18 @@
         self.search_line_edit.setFocus()
         self.search_line_edit.selectAll()
 
 
     def update_list(self, nodes):
         """update the list of available nodes"""
         self.nodes = sort_nodes(nodes)
-        self.update_view('')
+        self._update_view('')
 
 
-    def update_view(self, search_text=''):
+    def _update_view(self, search_text=''):
         if len(self.nodes) == 0:
             return
 
         search_text = search_text.lower()
 
         # remove all node widgets
 
@@ -143,51 +143,51 @@
         for n, dist in sorted_distances.items():
             if search_text != '' and dist > cutoff:
                 continue
 
             self.current_nodes.append(n)
 
             if self.node_widgets.get(n) is None:
-                self.node_widgets[n] = self.create_node_widget(n)
+                self.node_widgets[n] = self._create_node_widget(n)
 
             self.list_layout.addWidget(self.node_widgets[n])
 
         # focus on first result
         if len(self.current_nodes) > 0:
-            self.set_active_node_widget_index(0)
+            self._set_active_node_widget_index(0)
 
 
-    def create_node_widget(self, node):
+    def _create_node_widget(self, node):
         node_widget = NodeWidget(self, node)
-        node_widget.custom_focused_from_inside.connect(self.node_widget_focused_from_inside)
+        node_widget.custom_focused_from_inside.connect(self._node_widget_focused_from_inside)
         node_widget.setObjectName('node_widget_' + str(self._node_widget_index_counter))
         self._node_widget_index_counter += 1
-        node_widget.chosen.connect(self.node_widget_chosen)
+        node_widget.chosen.connect(self._node_widget_chosen)
 
         return node_widget
 
-    def node_widget_focused_from_inside(self):
+    def _node_widget_focused_from_inside(self):
         index = self.list_layout.indexOf(self.sender())
-        self.set_active_node_widget_index(index)
+        self._set_active_node_widget_index(index)
 
-    def set_active_node_widget_index(self, index):
+    def _set_active_node_widget_index(self, index):
         self.active_node_widget_index = index
         node_widget = self.list_layout.itemAt(index).widget()
 
         if self.active_node_widget:
             self.active_node_widget.set_custom_focus(False)
 
         node_widget.set_custom_focus(True)
         self.active_node_widget = node_widget
         self.list_scroll_area.ensureWidgetVisible(self.active_node_widget)
 
 
-    def node_widget_chosen(self):
+    def _node_widget_chosen(self):
         index = int(self.sender().objectName()[self.sender().objectName().rindex('_')+1:])
-        self.place_node(index)
+        self._place_node(index)
 
 
-    def place_node(self, index):
+    def _place_node(self, index):
         node_index = index
         node = self.current_nodes[node_index]
         self.node_chosen.emit(node)
         self.escaped.emit()
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/node_list_widget/NodeWidget.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/node_list_widget/NodeWidget.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,33 +24,33 @@
 
         self_ = self
         class NameLabel(QLineEdit):
             def __init__(self, text):
                 super().__init__(text)
 
                 self.setReadOnly(True)
-                self.setFont(QFont('Poppins', 10))
+                self.setFont(QFont('Source Code Pro', 8))
             def mouseMoveEvent(self, ev):
                 self_.custom_focused_from_inside.emit()
                 ev.ignore()
             def mousePressEvent(self, ev):
                 ev.ignore()
             def mouseReleaseEvent(self, ev):
                 ev.ignore()
 
         name_label = NameLabel(node.title)
 
         type_layout = QHBoxLayout()
 
-        type_label = QLabel(node.type_)
-        type_label.setFont(QFont('Segoe UI', 8, italic=True))
+        #type_label = QLabel(node.type_)
+        #type_label.setFont(QFont('Segoe UI', 8, italic=True))
         # type_label.setStyleSheet('color: white;')
 
         main_layout.addWidget(name_label, 0, 0)
-        main_layout.addWidget(type_label, 0, 1)
+        #main_layout.addWidget(type_label, 0, 1)
 
         self.setLayout(main_layout)
         self.setContentsMargins(0, 0, 0, 0)
         self.setMaximumWidth(250)
 
         self.setToolTip(node.__doc__)
         self.update_stylesheet()
@@ -80,32 +80,34 @@
             self.chosen.emit()
 
     def set_custom_focus(self, new_focus):
         self.custom_focused = new_focus
         self.update_stylesheet()
 
     def update_stylesheet(self):
-        bcol = QColor(self.node.color)
+        color = self.node.GUI.color if hasattr(self.node, 'GUI') else '#888888'
+
+        r, g, b = QColor(color).red(), QColor(color).green(), QColor(color).blue()
+
         new_style_sheet = f'''
 NodeWidget {{
-    border: 0px solid rgba({(
-        f'{QColor(self.node.color).red()},{QColor(self.node.color).green()},{QColor(self.node.color).blue()},150'
-    )});
+    border: 1px solid rgba(255,255,255,150);
     border-radius: 2px;
     {(
-        f'background-color: rgba({bcol.red()},{bcol.green()},{bcol.blue()},40);'
+        f'background-color: rgba(255,255,255,80);'
     ) if self.custom_focused else ''}
-}}   
+}}
 QLabel {{
     background: transparent;
 }}
 QLineEdit {{
-    color: {self.node.color};
+    color: white;
     background: transparent;
     border: none;
+    padding: 2px;
 }}
         '''
 
         self.setStyleSheet(new_style_sheet)
 
     def paintEvent(self, event):  # just to enable stylesheets
         o = QStyleOption()
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/node_list_widget/utils.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/node_list_widget/utils.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItem.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,87 +1,99 @@
+import traceback
+from typing import Optional, Tuple
+
 from qtpy.QtWidgets import QGraphicsItem, QGraphicsObject, QMenu, QGraphicsDropShadowEffect
 from qtpy.QtCore import Qt, QRectF, QObject, QPointF
 from qtpy.QtGui import QColor
 
+from .NodeErrorIndicator import NodeErrorIndicator
+from .NodeGUI import NodeGUI
 from ...GUIBase import GUIBase
 from ryvencore.NodePort import NodeInput, NodeOutput
 from .NodeItemAction import NodeItemAction
 from .NodeItemAnimator import NodeItemAnimator
 from .NodeItemWidget import NodeItemWidget
 from .PortItem import InputPortItem, OutputPortItem
 from ...utils import serialize, deserialize
 from ...utils import MovementEnum
 
 
 class NodeItem(GUIBase, QGraphicsObject):  # QGraphicsItem, QObject):
     """The GUI representative for nodes. Unlike the Node class, this class is not subclassed individually and works
     the same for every node."""
 
-    def __init__(self, node, params):
+    def __init__(self, node, node_gui, flow_view, design):
         # QGraphicsItem.__init__(self)
         # QObject.__init__(self)
         GUIBase.__init__(self, representing_component=node)
         QGraphicsObject.__init__(self)
 
         self.node = node
-        flow_view, design, load_data = params
+        self.node_gui = node_gui
+        self.node_gui.item = self
         self.flow_view = flow_view
         self.session_design = design
         self.movement_state = None
         self.movement_pos_from = None
         self.painted_once = False
         self.inputs = []
         self.outputs = []
-        self.color = QColor(self.node.color)  # manipulated by self.animator
+        self.color = QColor(self.node_gui.color)  # manipulated by self.animator
 
         self.collapsed = False
         self.hovered = False
         self.hiding_unconnected_ports = False
+        self.displaying_error = False
 
         self.personal_logs = []
 
         # 'initializing' will be set to False below. It's needed for the ports setup, to prevent shape updating stuff
         self.initializing = True
 
         # self.temp_state_data = None
-        self.init_data = load_data
+        self.init_data = self.node.load_data
 
         # CONNECT TO NODE
-        self.node.updated.connect(self.node_updated)
-        self.node.update_shape_triggered.connect(self.update_shape)
-        self.node.hide_unconnected_ports_triggered.connect(self.hide_unconnected_ports_triggered)
-        self.node.show_unconnected_ports_triggered.connect(self.show_unconnected_ports_triggered)
-        self.node.input_added.connect(self.add_new_input)
-        self.node.output_added.connect(self.add_new_output)
-        self.node.input_removed.connect(self.remove_input)
-        self.node.output_removed.connect(self.remove_output)
+        self.node_gui.updating.connect(self.node_updating)
+        self.node_gui.update_shape_triggered.connect(self.update_shape)
+        self.node_gui.hide_unconnected_ports_triggered.connect(self.hide_unconnected_ports_triggered)
+        self.node_gui.show_unconnected_ports_triggered.connect(self.show_unconnected_ports_triggered)
+        self.node_gui.input_added.connect(self.on_node_input_added)
+        self.node_gui.output_added.connect(self.on_node_output_added)
+        self.node_gui.input_removed.connect(self.on_node_input_removed)
+        self.node_gui.output_removed.connect(self.on_node_output_removed)
 
         # FLAGS
         self.setFlags(
             QGraphicsItem.ItemIsSelectable |
             QGraphicsItem.ItemIsMovable |
             QGraphicsItem.ItemSendsScenePositionChanges
         )
+
         self.setAcceptHoverEvents(True)
         self.setCacheMode(QGraphicsItem.DeviceCoordinateCache)
 
         # UI
         self.shadow_effect = None
         self.main_widget = None
-        if self.node.main_widget_class is not None:
-            self.main_widget = self.node.main_widget_class((self.node, self))
-        self.widget = NodeItemWidget(self.node, self)  # QGraphicsWidget(self)
+        if self.node_gui.main_widget_class is not None:
+            self.main_widget = self.node_gui.main_widget_class((self.node, self, self.node_gui))
+        self.widget = NodeItemWidget(self.node_gui, self)  # QGraphicsWidget(self)
         self.animator = NodeItemAnimator(self)  # needs self.title_label
+        self.error_indicator = NodeErrorIndicator(self)
+        self.error_indicator.hide()
 
         # TOOLTIP
-        if self.node.description_html:
-            self.setToolTip(self.node.description_html)
-        elif self.node.__doc__:
-            self.setToolTip('<html><head/><body><p>' + self.node.__doc__ + '</p></body></html>')
-        self.setCursor(Qt.SizeAllCursor)
+        self.tooltip_descr_html_content = \
+            self.node_gui.description_html \
+            if self.node_gui.description_html is not None \
+            else \
+            f'<p>{self.node.__doc__}</p>'
+
+        self.setToolTip(f'<html><head/><body>{self.tooltip_descr_html_content}</body></html>')
 
         # DESIGN THEME
         self.session_design.flow_theme_changed.connect(self.update_design)
         self.session_design.performance_mode_changed.connect(self.update_design)
 
     def initialize(self):
         """All ports and the main widget get finally created here."""
@@ -91,66 +103,109 @@
             if self.main_widget:
                 try:
                     self.main_widget.set_state(deserialize(self.init_data['main widget data']))
                 except Exception as e:
                     print('Exception while setting data in', self.node.title, 'Node\'s main widget:', e,
                           ' (was this intended?)')
 
-        # catch up on ports
-        for i in self.node.inputs:
-            self.add_new_input(i)
+        # catch up on init ports
+        for inp in self.node.inputs:
+            self.add_new_input(inp)
 
-        for o in self.node.outputs:
-            self.add_new_output(o)
+        for out in self.node.outputs:
+            self.add_new_output(out)
 
         if self.init_data is not None:
             if self.init_data.get('unconnected ports hidden'):
                 self.hide_unconnected_ports_triggered()
             if self.init_data.get('collapsed'):
                 self.collapse()
 
+        if self.init_data is not None:
+            self.node_gui.load(self.init_data)
+
+        self.node_gui.initialized()
+
         self.initializing = False
 
         # No self.update_shape() here because for some reason, the bounding rect hasn't been initialized yet, so
         # self.update_shape() gets called when the item is being drawn the first time (see paint event in NI painter)
         # https://forum.qt.io/topic/117179/force-qgraphicsitem-to-update-immediately-wait-for-update-event
 
         self.update_design()  # load current design, update QGraphicsItem
 
         self.update()  # ... not sure if I need that
 
     # --------------------------------------------------------------------------------------
-    # UI STUFF ----------------------------------------
+    # UI STUFF -------------------------#---------------
 
-    def node_updated(self):
+    def node_updating(self):
         if self.session_design.animations_enabled:
             if not self.animator.running():
                 self.animator.start()
             elif self.animator.fading_out():
                 self.animator.set_animation_max()
 
         self.update()
 
+    def display_error(self, e):
+        self.error_indicator.set_error(e)
+        self.error_indicator.show()
+        self.displaying_error = True
+
+    def remove_error_message(self):
+        self.error_indicator.hide()
+        self.setToolTip(f'<html><head/><body>{self.tooltip_descr_html_content}</body></html>')
+
+    def set_tooltip(self, error_msg=None):
+
+        if error_msg is not None:
+            err = f'<p style="background: red; color: white">{error_msg}</p>'
+        else:
+            err = ''
+
+        if self.node.description_html:
+            html = self.node.description_html + f'<html><head/><body>{err}</body></html>'
+        elif self.node.__doc__:
+            html = f'<html><head/><body><p>{self.node.__doc__}</p>{err}</body></html>'
+
+        self.setToolTip(html)
+        self.setCursor(Qt.SizeAllCursor)
+
+    def on_node_input_added(self, index, inp: NodeInput):
+        insert = index if index == len(self.node.inputs) - 1 else None
+        self.add_new_input(inp, insert)
+
     def add_new_input(self, inp: NodeInput, insert: int = None):
 
+        if inp in self.node_gui.input_widgets:
+            widget_name = self.node_gui.input_widgets[inp]['name']
+            widget_class = self.node_gui.input_widget_classes[widget_name]
+            widget_pos = self.node_gui.input_widgets[inp]['pos']
+            widget = (widget_class, widget_pos)
+        else:
+            widget = None
+
         # create item
-        # inp.item = InputPortItem(inp.node, self, inp)
-        item = InputPortItem(inp.node, self, inp)
+        item = InputPortItem(self.node_gui, self, inp, input_widget=widget)
 
         if insert is not None:
             self.inputs.insert(insert, item)
             self.widget.insert_input_into_layout(insert, item)
         else:
             self.inputs.append(item)
             self.widget.add_input_to_layout(item)
 
         if not self.initializing:
             self.update_shape()
             self.update()
 
+    def on_node_input_removed(self, index, inp: NodeInput):
+        self.remove_input(inp)
+
     def remove_input(self, inp: NodeInput):
         item = None
         for inp_item in self.inputs:
             if inp_item.port == inp:
                 item = inp_item
                 break
 
@@ -167,31 +222,38 @@
         self.inputs.remove(item)
         self.widget.remove_input_from_layout(item)
 
         if not self.initializing:
             self.update_shape()
             self.update()
 
+    def on_node_output_added(self, index, out: NodeOutput):
+        insert = index if index == len(self.node.outputs) - 1 else None
+        self.add_new_output(out, insert)
+
     def add_new_output(self, out: NodeOutput, insert: int = None):
 
         # create item
         # out.item = OutputPortItem(out.node, self, out)
-        item = OutputPortItem(out.node, self, out)
+        item = OutputPortItem(self.node_gui, self, out)
 
         if insert is not None:
             self.outputs.insert(insert, item)
             self.widget.insert_output_into_layout(insert, item)
         else:
             self.outputs.append(item)
             self.widget.add_output_to_layout(item)
 
         if not self.initializing:
             self.update_shape()
             self.update()
 
+    def on_node_output_removed(self, index, out: NodeOutput):
+        self.remove_output(out)
+
     def remove_output(self, out: NodeOutput):
         item = None
         for out_item in self.outputs:
             if out_item.port == out:
                 item = out_item
                 break
 
@@ -292,20 +354,21 @@
             # leads to a QT crash without error, which is really strange. Calling update_design multiple times
             # principally isn't a problem, but, for some reason, here it leads to a crash in QT. It's not necessary
             # anymore, so I removed it.
             # self.update_design()
 
             self.update_shape()
             self.update_conn_pos()
+            self.error_indicator.setPos(self.boundingRect().bottomRight())
 
         self.session_design.flow_theme.paint_NI(
-            node=self.node,
+            node_gui=self.node_gui,
             selected=self.isSelected(),
             hovered=self.hovered,
-            node_style=self.node.style,
+            node_style=self.node_gui.style,
             painter=painter,
             option=option,
             color=self.color,
             w=self.boundingRect().width(),
             h=self.boundingRect().height(),
             bounding_rect=self.boundingRect(),
             title_rect=self.widget.header_widget.boundingRect()
@@ -338,23 +401,15 @@
         self.painted_once = True
 
     # MOUSE INTERACTION
 
     def get_context_menu(self):
         menu = QMenu(self.flow_view)
 
-        for a in self.get_actions(self.node.get_extended_default_actions(), menu):  # menu needed for 'parent'
-            if type(a) == NodeItemAction:
-                menu.addAction(a)
-            elif type(a) == QMenu:
-                menu.addMenu(a)
-
-        menu.addSeparator()
-
-        actions = self.get_actions(self.node.actions, menu)
+        actions = self.get_actions(self.node_gui.actions, menu)
         for a in actions:  # menu needed for 'parent'
             if type(a) == NodeItemAction:
                 menu.addAction(a)
             elif type(a) == QMenu:
                 menu.addMenu(a)
 
         return menu
@@ -365,43 +420,43 @@
 
         if change == QGraphicsItem.ItemPositionChange:
             if self.session_design.performance_mode == 'pretty':
                 self.flow_view.viewport().update()
             if self.movement_state == MovementEnum.mouse_clicked:
                 self.movement_state = MovementEnum.position_changed
 
-        self.update_conn_pos()
+            self.update_conn_pos()
 
         return QGraphicsItem.itemChange(self, change, value)
 
     def update_conn_pos(self):
         """Updates the scene positions of connections"""
 
         for o in self.node.outputs:
-            for c in o.connections:
+            for i in self.node.flow.connected_inputs(o):
                 # c.item.recompute()
 
-                if c not in self.flow_view.connection_items:
+                if (o, i) not in self.flow_view.connection_items:
                     # it can happen that the connection item hasn't been
                     # created yet
                     continue
 
-                item = self.flow_view.connection_items[c]
+                item = self.flow_view.connection_items[(o,i)]
                 item.recompute()
         for i in self.node.inputs:
-            for c in i.connections:
-                # c.item.recompute()
+            o = self.node.flow.connected_output(i)
+            # c.item.recompute()
 
-                if c not in self.flow_view.connection_items:
-                    # it can happen that the connection item hasn't been
-                    # created yet
-                    continue
+            if (o, i) not in self.flow_view.connection_items:
+                # it can happen that the connection item hasn't been
+                # created yet
+                continue
 
-                item = self.flow_view.connection_items[c]
-                item.recompute()
+            item = self.flow_view.connection_items[(o,i)]
+            item.recompute()
 
     def hoverEnterEvent(self, event):
         self.hovered = True
         self.widget.title_label.set_NI_hover_state(hovering=True)
         QGraphicsItem.hoverEnterEvent(self, event)
 
     def hoverLeaveEvent(self, event):
@@ -439,18 +494,15 @@
             try:
                 method = v_dict['method']
                 data = None
                 try:
                     data = v_dict['data']
                 except KeyError:
                     pass
-                action = NodeItemAction(node=self.node, text=k, method=method, menu=menu, data=data)
-                action.triggered_with_data.connect(self.flow_view.thread_interface.trigger_node_action)
-                action.triggered_without_data.connect(self.flow_view.thread_interface.trigger_node_action)
-
+                action = NodeItemAction(node_gui=self.node_gui, text=k, method=method, menu=menu, data=data)
                 actions.append(action)
             except KeyError:
                 action_menu = QMenu(k, menu)
                 sub_actions = self.get_actions(v_dict, action_menu)
                 for a in sub_actions:
                     action_menu.addAction(a)
                 actions.append(action_menu)
@@ -466,8 +518,10 @@
         data['pos y'] = self.pos().y()
         if self.main_widget:
             data['main widget data'] = serialize(self.main_widget.get_state())
 
         data['unconnected ports hidden'] = self.hiding_unconnected_ports
         data['collapsed'] = self.collapsed
 
+        data = {**data, **self.node_gui.data()}
+
         return data
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItemAction.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItemAction.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,29 +10,24 @@
     So, if a special action does not have 'data', the connected method does not need to have a data parameter.
     Both signals get connected to the target method but only if data isn't None, the signal with the data parameter
     is used."""
 
     triggered_with_data = Signal(object, object)
     triggered_without_data = Signal(object)
 
-    def __init__(self, node, text, method, menu, data=None):
+    def __init__(self, node_gui, text, method, menu, data=None):
         super(NodeItemAction, self).__init__(text=text, parent=menu)
 
-        self.node = node
+        self.node_gui = node_gui
         self.data = data
         self.method = method
-        self.triggered.connect(self.triggered_)  # yeah, I think that's ugly but I didn't find a nicer way; it works
+        self.triggered.connect(self.triggered_)
 
     def triggered_(self):
         if self.data is not None:
-            self.triggered_with_data.emit(self.grab_method(), self.data)
+            self.grab_method()(self.data)
         else:
-            self.triggered_without_data.emit(self.grab_method())
+            self.grab_method()()
 
     def grab_method(self):
-        """
-        Replacement for the retain mechanism. Because some editors (like Ryven) might add source code editing features,
-        before calling a method here
-        :return:
-        """
-        updated_method = getattr(self.node, self.method.__name__)
-        return updated_method
+        # the method object could have changed since the action was created
+        return getattr(self.node_gui, self.method.__name__)
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItemAnimator.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItemAnimator.py`

 * *Files identical despite different names*

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItemWidget.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItemWidget.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 from .NodeItem_TitleLabel import TitleLabel
 from .PortItem import InputPortItem, OutputPortItem
 
 
 class NodeItemWidget(QGraphicsWidget):
     """The QGraphicsWidget managing all GUI components of a NodeItem in widgets and layouts."""
 
-    def __init__(self, node, node_item):
+    def __init__(self, node_gui, node_item):
         super().__init__(parent=node_item)
 
-        self.node = node
+        self.node_gui = node_gui
         self.node_item = node_item
         self.flow_view = self.node_item.flow_view
+        self.flow = self.flow_view.flow
 
         self.body_padding = 6
         self.header_padding = (0, 0, 0, 0)  # theme dependent and hence updated in setup_layout()!
 
-        self.icon = NodeItem_Icon(node, node_item) if node.icon else None
-        self.collapse_button = NodeItem_CollapseButton(node, node_item) if node.style == 'normal' else None
-        self.title_label = TitleLabel(node, node_item)
+        self.icon = NodeItem_Icon(node_gui, node_item) if node_gui.icon else None
+        self.collapse_button = NodeItem_CollapseButton(node_gui, node_item) if node_gui.style == 'normal' else None
+        self.title_label = TitleLabel(node_gui, node_item)
         self.main_widget_proxy: FlowViewProxyWidget = None
         if self.node_item.main_widget:
             self.main_widget_proxy = FlowViewProxyWidget(self.flow_view)
             self.main_widget_proxy.setWidget(self.node_item.main_widget)
         self.header_layout: QGraphicsWidget = None
         self.header_widget: QGraphicsWidget = None
         self.body_layout: QGraphicsLinearLayout = None
@@ -42,15 +43,15 @@
         self.header_padding = self.node_item.session_design.flow_theme.header_padding
 
         #   main layout
         layout = QGraphicsLinearLayout(Qt.Vertical)
         layout.setContentsMargins(0, 0, 0, 0)
         layout.setSpacing(0)
 
-        if self.node.style == 'normal':
+        if self.node_gui.style == 'normal':
             self.header_widget = QGraphicsWidget()
             # self.header_widget.setContentsMargins(0, 0, 0, 0)
             self.header_widget.setSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
             self.header_layout = QGraphicsLinearLayout(Qt.Horizontal)
             self.header_layout.setSpacing(5)
             self.header_layout.setContentsMargins(
                 *self.header_padding
@@ -156,62 +157,62 @@
             self.adjustSize()
 
         self.body_layout.invalidate()
         self.layout().invalidate()
         self.layout().activate()
         # very essential; repositions everything in case content has changed (inputs/outputs/widget)
 
-        if self.node.style == 'small':
+        if self.node_gui.style == 'small':
 
             # making it recompute its true minimumWidth here
             self.adjustSize()
 
             if self.layout().minimumWidth() < self.title_label.width + 15:
                 self.layout().setMinimumWidth(self.title_label.width + 15)
                 self.layout().activate()
 
         w = self.boundingRect().width()
         h = self.boundingRect().height()
         rect = QRectF(QPointF(-w / 2, -h / 2),
                       QPointF(w / 2, h / 2))
         self.setPos(rect.left(), rect.top())
 
-        if not self.node.style == 'normal':
+        if not self.node_gui.style == 'normal':
             if self.icon:
                 self.icon.setPos(
                     QPointF(-self.icon.boundingRect().width() / 2,
                             -self.icon.boundingRect().height() / 2)
                 )
                 self.title_label.hide()
             else:
                 self.title_label.setPos(
                     QPointF(-self.title_label.boundingRect().width() / 2,
                             -self.title_label.boundingRect().height() / 2)
                 )
 
 
     def add_main_widget_to_layout(self):
-        if self.node.main_widget_pos == 'between ports':
+        if self.node_gui.main_widget_pos == 'between ports':
             self.body_layout.insertItem(1, self.main_widget_proxy)
             self.body_layout.insertStretch(2)
 
-        elif self.node.main_widget_pos == 'below ports':
+        elif self.node_gui.main_widget_pos == 'below ports':
             self.layout().addItem(self.main_widget_proxy)
             self.layout().setAlignment(self.main_widget_proxy, Qt.AlignHCenter)
 
     def add_input_to_layout(self, inp: InputPortItem):
         if self.inputs_layout.count() > 0:
             self.inputs_layout.addStretch()
         self.inputs_layout.addItem(inp)
         self.inputs_layout.setAlignment(inp, Qt.AlignLeft)
 
     def insert_input_into_layout(self, index: int, inp: InputPortItem):
         self.inputs_layout.insertItem(index * 2 + 1, inp)  # *2 bcs of the stretches
         self.inputs_layout.setAlignment(inp, Qt.AlignLeft)
-        if len(self.node.inputs) > 1:
+        if len(self.node_gui.node.inputs) > 1:
             self.inputs_layout.insertStretch(index * 2 + 1)  # *2+1 because of the stretches, too
 
     def remove_input_from_layout(self, inp: InputPortItem):
         self.inputs_layout.removeItem(inp)
 
         # just a temporary workaround for the issues discussed here:
         # https://forum.qt.io/topic/116268/qgraphicslayout-not-properly-resizing-to-change-of-content
@@ -222,15 +223,15 @@
             self.outputs_layout.addStretch()
         self.outputs_layout.addItem(out)
         self.outputs_layout.setAlignment(out, Qt.AlignRight)
 
     def insert_output_into_layout(self, index: int, out: OutputPortItem):
         self.outputs_layout.insertItem(index * 2 + 1, out)  # *2 because of the stretches
         self.outputs_layout.setAlignment(out, Qt.AlignRight)
-        if len(self.node.outputs) > 1:
+        if len(self.node_gui.node.outputs) > 1:
             self.outputs_layout.insertStretch(index * 2 + 1)  # *2+1 because of the stretches, too
 
     def remove_output_from_layout(self, out: OutputPortItem):
         self.outputs_layout.removeItem(out)
 
         # just a temporary workaround for the issues discussed here:
         # https://forum.qt.io/topic/116268/qgraphicslayout-not-properly-resizing-to-change-of-content
@@ -243,19 +244,19 @@
 
     def expand(self):
         self.body_widget.show()
         if self.main_widget_proxy:
             self.main_widget_proxy.show()
 
     def hide_unconnected_ports(self):
-        for inp in self.node_item.inputs:
-            if len(inp.port.connections) == 0:
+        for inp in self.node_item.node.inputs:
+            if self.flow.connected_output(inp) is None:
                 inp.hide()
-        for out in self.node_item.outputs:
-            if len(out.port.connections) == 0:
+        for out in self.node_item.node.outputs:
+            if len(self.flow.connected_inputs(out)):
                 out.hide()
 
     def show_unconnected_ports(self):
         for inp in self.node_item.inputs:
             inp.show()
         for out in self.node_item.outputs:
             out.show()
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItem_CollapseButton.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItem_Icon.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,50 @@
-from qtpy.QtCore import QSize, QRectF, QPointF, QSizeF, Qt
-from qtpy.QtWidgets import QGraphicsWidget, QGraphicsLayoutItem
+from qtpy.QtCore import QSize, QRectF, QPointF, QSizeF
+from qtpy.QtGui import QPixmap, QImage, QPainter, QIcon, QPicture
+from qtpy.QtWidgets import QGraphicsPixmapItem, QGraphicsWidget, QGraphicsLayoutItem
 
-from ...GlobalAttributes import Location
 from ...utils import change_svg_color
 
 
-class NodeItem_CollapseButton(QGraphicsWidget):
-    def __init__(self, node, node_item):
+class NodeItem_Icon(QGraphicsWidget):
+    def __init__(self, node_gui, node_item):
         super().__init__(parent=node_item)
 
-        self.node = node
-        self.node_item = node_item
-
-        self.size = QSizeF(14, 7)
+        if node_gui.style == 'normal':
+            self.size = QSize(20, 20)
+        else:
+            self.size = QSize(50, 50)
 
         self.setGraphicsItem(self)
-        self.setCursor(Qt.PointingHandCursor)
-
 
-        self.collapse_pixmap = change_svg_color(Location.PACKAGE_PATH+'/resources/node_collapse_icon.svg',
-                                                self.node.color)
-        self.expand_pixmap = change_svg_color(Location.PACKAGE_PATH+'/resources/node_expand_icon.svg',
-                                              self.node.color)
+        image = QImage(node_gui.icon)
+        self.pixmap = QPixmap.fromImage(image)
+        # self.pixmap = change_svg_color(node.icon, node.color)
 
 
     def boundingRect(self):
         return QRectF(QPointF(0, 0), self.size)
 
     def setGeometry(self, rect):
         self.prepareGeometryChange()
         QGraphicsLayoutItem.setGeometry(self, rect)
         self.setPos(rect.topLeft())
 
     def sizeHint(self, which, constraint=...):
         return QSizeF(self.size.width(), self.size.height())
 
-    def mousePressEvent(self, event):
-        event.accept()  # make sure the event doesn't get passed on
-        self.node_item.flow_view.mouse_event_taken = True
-
-        if self.node_item.collapsed:
-            self.node_item.expand()
-        else:
-            self.node_item.collapse()
-
-    # def hoverEnterEvent(self, event):
 
     def paint(self, painter, option, widget=None):
 
-        # doesn't work: ...
+        # TODO: anti aliasing for node icons
+
+        # this doesn't work: ...
         # painter.setRenderHint(QPainter.Antialiasing, True)
         # painter.setRenderHint(QPainter.HighQualityAntialiasing, True)
         # painter.setRenderHint(QPainter.SmoothPixmapTransform, True)
 
-        if not self.node_item.hovered:
-            return
-
-        if self.node_item.collapsed:
-            pixmap = self.expand_pixmap
-        else:
-            pixmap = self.collapse_pixmap
 
         painter.drawPixmap(
             0, 0,
             self.size.width(), self.size.height(),
-            pixmap
+            self.pixmap
         )
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItem_Icon.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItem_CollapseButton.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,73 @@
-from qtpy.QtCore import QSize, QRectF, QPointF, QSizeF
-from qtpy.QtGui import QPixmap, QImage, QPainter, QIcon, QPicture
-from qtpy.QtWidgets import QGraphicsPixmapItem, QGraphicsWidget, QGraphicsLayoutItem
+from qtpy.QtCore import QSize, QRectF, QPointF, QSizeF, Qt
+from qtpy.QtWidgets import QGraphicsWidget, QGraphicsLayoutItem
+from qtpy.QtGui import QColor
 
-from ...utils import change_svg_color
+from ...GlobalAttributes import Location
+from ...utils import change_svg_color, get_resource
 
 
-class NodeItem_Icon(QGraphicsWidget):
-    def __init__(self, node, node_item):
+class NodeItem_CollapseButton(QGraphicsWidget):
+    def __init__(self, node_gui, node_item):
         super().__init__(parent=node_item)
 
-        if node.style == 'normal':
-            self.size = QSize(20, 20)
-        else:
-            self.size = QSize(50, 50)
+        self.node_gui = node_gui
+        self.node_item = node_item
+
+        self.size = QSizeF(14, 7)
 
         self.setGraphicsItem(self)
+        self.setCursor(Qt.PointingHandCursor)
+
 
-        image = QImage(node.icon)
-        self.pixmap = QPixmap.fromImage(image)
-        # self.pixmap = change_svg_color(node.icon, node.color)
+        self.collapse_pixmap = change_svg_color(
+            get_resource('node_collapse_icon.svg'),
+            self.node_gui.color
+        )
+        self.expand_pixmap = change_svg_color(
+            get_resource('node_expand_icon.svg'),
+            self.node_gui.color
+        )
 
 
     def boundingRect(self):
         return QRectF(QPointF(0, 0), self.size)
 
     def setGeometry(self, rect):
         self.prepareGeometryChange()
         QGraphicsLayoutItem.setGeometry(self, rect)
         self.setPos(rect.topLeft())
 
     def sizeHint(self, which, constraint=...):
         return QSizeF(self.size.width(), self.size.height())
 
+    def mousePressEvent(self, event):
+        event.accept()  # make sure the event doesn't get passed on
+        self.node_item.flow_view.mouse_event_taken = True
 
-    def paint(self, painter, option, widget=None):
+        if self.node_item.collapsed:
+            self.node_item.expand()
+        else:
+            self.node_item.collapse()
+
+    # def hoverEnterEvent(self, event):
 
-        # TODO: anti aliasing for node icons
+    def paint(self, painter, option, widget=None):
 
-        # this doesn't work: ...
+        # doesn't work: ...
         # painter.setRenderHint(QPainter.Antialiasing, True)
         # painter.setRenderHint(QPainter.HighQualityAntialiasing, True)
         # painter.setRenderHint(QPainter.SmoothPixmapTransform, True)
 
+        if not self.node_item.hovered:
+            return
+
+        if self.node_item.collapsed:
+            pixmap = self.expand_pixmap
+        else:
+            pixmap = self.collapse_pixmap
 
         painter.drawPixmap(
             0, 0,
             self.size.width(), self.size.height(),
-            self.pixmap
+            pixmap
         )
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/NodeItem_TitleLabel.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/NodeItem_TitleLabel.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,37 +3,37 @@
 from qtpy.QtWidgets import QGraphicsWidget, QGraphicsLayoutItem, QGraphicsItem
 
 from ...utils import get_longest_line
 
 
 class TitleLabel(QGraphicsWidget):
 
-    def __init__(self, node, node_item):
+    def __init__(self, node_gui, node_item):
         super(TitleLabel, self).__init__(parent=node_item)
 
         self.setGraphicsItem(self)
 
-        self.node = node
+        self.node_gui = node_gui
         self.node_item = node_item
 
-        font = QFont('Poppins', 15) if self.node.style == 'normal' else \
+        font = QFont('Poppins', 15) if self.node_gui.style == 'normal' else \
             QFont('K2D', 20, QFont.Bold, True)  # should be quite similar to every specific font chosen by the painter
         self.fm = QFontMetricsF(font)
         self.title_str, self.width, self.height = None, None, None
         self.update_shape()
 
         self.color = QColor(30, 43, 48)
         self.pen_width = 1.5
         self.hovering = False  # whether the mouse is hovering over the parent NI (!)
 
         # # Design.flow_theme_changed.connect(self.theme_changed)
         # self.update_design()
 
     def update_shape(self):
-        self.title_str = self.node.display_title
+        self.title_str = self.node_gui.display_title
 
         # approximately!
         self.width = self.fm.width(get_longest_line(self.title_str)+'___')
         self.height = self.fm.height() * 0.7 * (self.title_str.count('\n') + 1)
 
     def boundingRect(self):
         return QRectF(QPointF(0, 0), self.geometry().size())
@@ -44,21 +44,21 @@
         self.setPos(rect.topLeft())
 
     def sizeHint(self, which, constraint=...):
         return QSizeF(self.width, self.height)
 
     def paint(self, painter, option, widget=None):
         self.node_item.session_design.flow_theme.paint_NI_title_label(
-            self.node, self.node_item.isSelected(), self.hovering, painter, option,
+            self.node_gui, self.node_item.isSelected(), self.hovering, painter, option,
             self.design_style(), self.title_str,
             self.node_item.color, self.boundingRect()
         )
 
     def design_style(self):
-        return self.node.style
+        return self.node_gui.style
 
     def set_NI_hover_state(self, hovering: bool):
         self.hovering = hovering
         # self.update_design()
         self.update()
 
     # ANIMATION STUFF
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/PortItem.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/PortItem.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,78 @@
-from qtpy.QtWidgets import QGraphicsGridLayout, QGraphicsWidget, \
-    QGraphicsLayoutItem
+from typing import Tuple
+
+from qtpy.QtWidgets import QGraphicsGridLayout, QGraphicsWidget, QGraphicsLayoutItem
 from qtpy.QtCore import Qt, QRectF, QPointF, QSizeF
 from qtpy.QtGui import QFontMetricsF, QFont
 
 from ...GUIBase import GUIBase
-from .PortItemInputWidgets import \
-    Data_IW_S, Data_IW_M, Data_IW_L, Float_IW, Integer_IW, Choice_IW, Boolean_IW, String_IW_S, String_IW_M, String_IW_L
-from ryvencore import dtypes, serialize
+from .PortItemInputWidgets import Data_IW_S, Data_IW_M, Data_IW_L, Float_IW, Integer_IW, \
+    Choice_IW, Boolean_IW, String_IW_S, String_IW_M, String_IW_L
+from ryvencore import serialize, Data
+from ryvencore.NodePort import NodeOutput, NodeInput, NodePort
 from ryvencore.utils import deserialize
 from ...utils import get_longest_line, shorten
 
 from ..FlowViewProxyWidget import FlowViewProxyWidget
 
+#
+# Utils
+#
+
+def is_connected(port):
+    if isinstance(port, NodeOutput):
+        is_connected = len(port.node.flow.connected_inputs(port)) > 0
+    else:
+        is_connected = port.node.flow.connected_output(port) is not None
+    return is_connected
+
+def val(port):
+    if isinstance(port, NodeOutput):
+        return port.val.payload if isinstance(port.val, Data) else None
+    else:
+        conn_out = port.node.flow.connected_output(port)
+        if conn_out:
+            return conn_out.val.payload if conn_out.val is not None else None
+        else:
+            return None
+
+def connections(port):
+    if isinstance(port, NodeOutput):
+        return [(port, i) for i in port.node.flow.connected_inputs(port)]
+    else:
+        conn_out = port.node.flow.connected_output(port)
+        if conn_out:
+            return [(port.node.flow.connected_output(port), port)]
+        else:
+            return []
+
+#
+# Classes
+#
 
 class PortItem(GUIBase, QGraphicsWidget):
     """The GUI representative for ports of nodes, also handling mouse events for connections."""
 
-    def __init__(self, node, node_item, port, flow_view):
+    def __init__(self, node_gui, node_item, port, flow_view):
         GUIBase.__init__(self, representing_component=port)
         QGraphicsWidget.__init__(self)
 
         self.setGraphicsItem(self)
 
-        self.node = node
+        self.node_gui = node_gui
         self.node_item = node_item
-        self.port = port
+        self.port: NodePort = port
         self.flow_view = flow_view
 
         # self.port.has_been_connected.connect(self.port_connected)
         # self.port.has_been_disconnected.connect(self.port_disconnected)
 
-        self.pin = PortItemPin(self.port, self, self.node, self.node_item)
+        self.pin = PortItemPin(self.port, self, self.node_gui, self.node_item)
 
-        self.label = PortItemLabel(self.port, self, self.node, self.node_item)
+        self.label = PortItemLabel(self.port, self, self.node_gui, self.node_item)
 
         self._layout = QGraphicsGridLayout()
         self._layout.setSpacing(0)
         self._layout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(self._layout)
 
     # --------------------------------------------
@@ -56,154 +92,106 @@
         pass
 
     def port_disconnected(self):
         pass
 
 
 class InputPortItem(PortItem):
-    def __init__(self, node, node_item, port):
-        super().__init__(node, node_item, port, node.flow)
-
-        self.proxy = None  # widget proxy
-        self.widget = self.create_widget()
+    def __init__(self, node_gui, node_item, port, input_widget: Tuple[type, str] = None):
+        super().__init__(node_gui, node_item, port, node_gui.flow_view())
 
-        if self.widget:
-            self.proxy = FlowViewProxyWidget(self.flow_view, parent=self.node_item)
-            self.proxy.setWidget(self.widget)
+        self.proxy = None   # widget proxy
+        self.widget = None  # widget
+        if input_widget is not None:
+            self.create_widget(input_widget[0], input_widget[1])
 
         self.update_widget_value = self.widget is not None  # modified by FlowView when performance mode changes
 
         # catch up to missed connections
-        if len(self.port.connections) > 0:
+        if self.port.node.flow.connected_output(self.port) is not None:
             self.port_connected()
 
-        if self.port.add_data:
-
-            if self.port.dtype:
-                c_d = self.port.add_data['widget data']
+        if self.port.type_ == 'data' and self.port.load_data is not None and self.port.load_data['has widget']:
+            c_d = self.port.load_data['widget data']
+            if c_d is not None:
                 self.widget.set_state(deserialize(c_d))
-
-            elif 'widget data' in self.port.add_data:
-                try:
-                    c_d = self.port.add_data['widget data']
-                    if type(c_d) == dict:  # backwards compatibility
-                        self.widget.set_state(c_d)
-                    else:
-                        self.widget.set_state(deserialize(c_d))
-                except Exception as e:
-                    print('Exception while setting data in', self.node.title,
-                          '\'s input widget:', e, ' (was this intended?)')
+            else:
+                # this is a little feature that lets us prevent loading of input widgets
+                # which is occasionally useful, e.g. when changing an input widget class:
+                # to prevent loading of the input widget, 'widget data' must be None
+                pass
 
         self.setup_ui()
 
     def setup_ui(self):
         l = self._layout
 
         # l.setSpacing(0)
         l.addItem(self.pin, 0, 0)
         l.setAlignment(self.pin, Qt.AlignVCenter | Qt.AlignLeft)
         l.addItem(self.label, 0, 1)
         l.setAlignment(self.label, Qt.AlignVCenter | Qt.AlignLeft)
         if self.widget:
-            if self.port.add_data and self.port.add_data.get('widget pos') == 'below':
+            if self.widget.position == 'below':
                 l.addItem(self.proxy, 1, 0, 1, 2)
+            elif self.widget.position == 'besides':
+                l.addItem(self.proxy, 0, 2)
             else:
-                l.addItem(self.proxy, 0, 2)  # besides
+                print('Unknown input widget position:', self.widget.position)
 
             l.setAlignment(self.proxy, Qt.AlignCenter)
 
-    def create_widget(self):
-
-        params = (self.port, self, self.node, self.node_item)
-
-        if self.port.dtype:
-
-            dtype = self.port.dtype
-
-            if isinstance(dtype, dtypes.Data):
-                if dtype.size == 's':
-                    return Data_IW_S(params)
-                elif dtype.size == 'm':
-                    return Data_IW_M(params)
-                elif dtype.size == 'l':
-                    return Data_IW_L(params)
+    def create_widget(self, widget_class, widget_pos):
 
-            elif isinstance(dtype, dtypes.String):
-                if dtype.size == 's':
-                    return String_IW_S(params)
-                elif dtype.size == 'm':
-                    return String_IW_M(params)
-                elif dtype.size == 'l':
-                    return String_IW_L(params)
+        if widget_class is None:
+            return
 
-            elif isinstance(dtype, dtypes.Integer):
-                return Integer_IW(params)
+        if self.port.type_ != 'data':
+            # TODO: how about input widgets for exec inputs?
+            return
 
-            elif isinstance(dtype, dtypes.Float):
-                return Float_IW(params)
+        params = (self.port, self, self.node_gui.node, self.node_gui, widget_pos)
 
-            elif isinstance(dtype, dtypes.Boolean):
-                return Boolean_IW(params)
-
-            elif isinstance(dtype, dtypes.Choice):
-                return Choice_IW(params)
-
-        elif self.port.type_ == 'data' and self.port.add_data and 'widget name' in self.port.add_data:
-
-            # custom input widget
-            return self.get_input_widget_class(self.port.add_data['widget name'])(params)
-
-        else:
-            return None
-
-
-    def get_input_widget_class(self, widget_name):
-        """Returns the CLASS of a defined custom input widget"""
-        return self.node.input_widget_classes[widget_name]
+        # custom input widget
+        self.widget = widget_class(params)
+        self.proxy = FlowViewProxyWidget(self.flow_view, parent=self.node_item)
+        self.proxy.setWidget(self.widget)
 
     def port_connected(self):
         """Disables the widget"""
         if self.widget:
             self.widget.setEnabled(False)
 
-        if self.port.type_ == 'data':
-            self.port.connections[0].activated.connect(self._port_val_updated)
-
-        self._port_val_updated(self.port.val)
+        # https://github.com/leon-thomm/Ryven/pull/137#issuecomment-1433783052
+        # if self.port.type_ == 'data':
+        #     self.port.connections[0].activated.connect(self._port_val_updated)
+        #
+        # self._port_val_updated(self.port.val)
 
     def port_disconnected(self):
         """Enables the widget again"""
         if self.widget:
             self.widget.setEnabled(True)
 
-    def _port_val_updated(self, val):
-        """Called from output port"""
-
-        if self.update_widget_value:  # this might be quite slow
-            self.widget.val_update_event(val)
-
     def complete_data(self, data: dict) -> dict:
         if self.port.type_ == 'data':
             if self.widget:
                 data['has widget'] = True
-                if not self.port.dtype:
-                    # this stuff is statically stored in port.add_data
-                    data['widget name'] = self.port.add_data['widget name']
-                    data['widget pos'] = self.port.add_data['widget pos']
-
+                data['widget name'] = self.node_gui.input_widgets[self.port]['name']
+                data['widget pos'] = self.node_gui.input_widgets[self.port]['pos']
                 data['widget data'] = serialize(self.widget.get_state())
             else:
                 data['has widget'] = False
 
         return data
 
 
 class OutputPortItem(PortItem):
-    def __init__(self, node, node_item, port):
-        super().__init__(node, node_item, port, node.flow)
+    def __init__(self, node_gui, node_item, port):
+        super().__init__(node_gui, node_item, port, node_gui.flow_view())
         # super(OutputPortItem, self).__init__(parent_node_instance, PortObjPos.OUTPUT, type_, label_str)
 
         self.setup_ui()
 
     def setup_ui(self):
         l = self._layout
 
@@ -215,20 +203,20 @@
         l.setAlignment(self.pin, Qt.AlignVCenter | Qt.AlignRight)
 
 
 # CONTENTS -------------------------------------------------------------------------------------------------------------
 
 
 class PortItemPin(QGraphicsWidget):
-    def __init__(self, port, port_item, node, node_item):
+    def __init__(self, port, port_item, node_gui, node_item):
         super(PortItemPin, self).__init__(node_item)
 
         self.port = port
         self.port_item = port_item
-        self.node = node
+        self.node_gui = node_gui
         self.node_item = node_item
         self.flow_view = self.node_item.flow_view
 
         self.setGraphicsItem(self)
         self.setAcceptHoverEvents(True)
         self.hovered = False
         self.setCursor(Qt.CrossCursor)
@@ -252,20 +240,20 @@
         self.setPos(rect.topLeft())
 
     def sizeHint(self, which, constraint=...):
         return QSizeF(self.width, self.height)
 
     def paint(self, painter, option, widget=None):
         self.node_item.session_design.flow_theme.paint_PI(
-            node=self.node,
+            node_gui=self.node_gui,
             painter=painter,
             option=option,
-            node_color=self.node_item.color,
+            node_color=self.node_gui.color,
             type_=self.port.type_,
-            connected=len(self.port.connections) > 0,
+            connected=is_connected(self.port),
             rect=QRectF(self.padding, self.padding, self.width-2*self.padding, self.height-2*self.padding)
         )
 
     def mousePressEvent(self, event):
         if event.button() == Qt.LeftButton:  # DRAG NEW CONNECTION
             self.flow_view.mouse_event_taken = True
             self.flow_view._selected_pin = self
@@ -286,30 +274,30 @@
             # if the items are grouped (which means they move together), don't recompute
             if i.out.group() is None or i.out.group() != i.inp.group():  # not entirely sure if this is working
                 i.recompute()
 
 
     def hoverEnterEvent(self, event):
         if self.port.type_ == 'data':  # and self.parent_port_instance.io_pos == PortPos.OUTPUT:
-            self.setToolTip(shorten(str(self.port.val), 1000, line_break=True))
+            self.setToolTip(shorten(str(val(self.port)), 1000, line_break=True))
 
         # highlight connections
         items = self.flow_view.connection_items
-        for c in self.port.connections:
+        for c in connections(self.port):
             items[c].set_highlighted(True)
 
         self.hovered = True
 
         QGraphicsWidget.hoverEnterEvent(self, event)
 
     def hoverLeaveEvent(self, event):
 
         # un-highlight connections
         items = self.flow_view.connection_items
-        for c in self.port.connections:
+        for c in connections(self.port):
             items[c].set_highlighted(False)
 
         self.hovered = False
 
         QGraphicsWidget.hoverLeaveEvent(self, event)
 
     def get_scene_center_pos(self):
@@ -320,21 +308,21 @@
             if isinstance(self.port_item, InputPortItem):
                 return self.node_item.get_left_body_header_vertex_scene_pos()
             else:
                 return self.node_item.get_right_body_header_vertex_scene_pos()
 
 
 class PortItemLabel(QGraphicsWidget):
-    def __init__(self, port, port_item, node, node_item):
+    def __init__(self, port, port_item, node_gui, node_item):
         super(PortItemLabel, self).__init__(node_item)
         self.setGraphicsItem(self)
 
         self.port = port
         self.port_item = port_item
-        self.node = node
+        self.node_gui = node_gui
         self.node_item = node_item
 
         self.font = QFont("Source Code Pro", 10, QFont.Bold)
         font_metrics = QFontMetricsF(self.font)  # approximately! the designs can use different fonts
         self.width = font_metrics.width(get_longest_line(self.port.label_str))
         self.height = font_metrics.height() * (self.port.label_str.count('\n') + 1)
         self.port_local_pos = None
@@ -348,15 +336,15 @@
         self.setPos(rect.topLeft())
 
     def sizeHint(self, which, constraint=...):
         return QSizeF(self.width, self.height)
 
     def paint(self, painter, option, widget=None):
         self.node_item.session_design.flow_theme.paint_PI_label(
-            self.node,
+            self.node_gui,
             painter, option,
             self.port.type_,
-            len(self.port.connections) > 0,
+            is_connected(self.port),
             self.port.label_str,
-            self.node_item.color,
+            self.node_gui.color,
             self.boundingRect()
         )
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/flows/nodes/PortItemInputWidgets.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/flows/nodes/PortItemInputWidgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from qtpy.QtGui import QFontMetrics, QFont
 from qtpy.QtWidgets import QSpinBox, QLineEdit, QCheckBox, QComboBox
 
-from .WidgetBaseClasses import IWB
+from .WidgetBaseClasses import NodeInputWidget
 
 
-class DType_IW_Base(IWB):
+class DType_IW_Base(NodeInputWidget):
 
     def __init__(self, params):
         super().__init__(params)
 
         self.dtype = self.input.dtype
         self.block = False
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt/src/utils.py` & `ryvencore-qt-0.4.0a2/ryvencore_qt/src/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import bisect
 import enum
 import json
-import os
+import pathlib
 from math import sqrt
-from waiting import wait
 from typing import List, Dict
 
+from qtpy.QtCore import QPointF, QByteArray
+
 from ryvencore.utils import serialize, deserialize
-from qtpy.QtCore import QPointF
+from .GlobalAttributes import *
 
 
 class Container:
     """used for threading; accessed from multiple threads"""
 
     def __init__(self):
         self.payload = None
@@ -21,18 +22,14 @@
         self.payload = val
         self.has_been_set = True
 
     def is_set(self):
         return self.has_been_set
 
 
-def wait_until(func):
-    return wait(func, sleep_seconds=0.001)
-
-
 def pythagoras(a, b):
     return sqrt(a ** 2 + b ** 2)
 
 
 def get_longest_line(s: str):
     lines = s.split('\n')
     lines = [line.replace('\n', '') for line in lines]
@@ -74,91 +71,48 @@
 class MovementEnum(enum.Enum):
     # this should maybe get removed later
     mouse_clicked = 1
     position_changed = 2
     mouse_released = 3
 
 
+def get_resource(filepath: str):
+    return pathlib.Path(Location.PACKAGE_PATH, 'resources', filepath)
+
+
 def change_svg_color(filepath: str, color_hex: str):
-    # doesnt seem to work properly yet :(
+    """Loads an SVG, changes all '#xxxxxx' occurrences to color_hex, renders it into and a pixmap and returns it"""
+
+    # https://stackoverflow.com/questions/15123544/change-the-color-of-an-svg-in-qt
 
     from qtpy.QtSvg import QSvgRenderer
     from qtpy.QtGui import QPixmap, QPainter
     from qtpy.QtCore import Qt
 
     with open(filepath) as f:
         data = f.read()
-    data = data.replace('fill:#000000', 'fill:'+color_hex)
-    with open(filepath, 'w') as f:
-        f.write(data)
+    data = data.replace('fill:#xxxxxx', 'fill:'+color_hex)
+
+    svg_renderer = QSvgRenderer(QByteArray(bytes(data, 'ascii')))
 
-    svg_renderer = QSvgRenderer(filepath)
     pix = QPixmap(svg_renderer.defaultSize())
     pix.fill(Qt.transparent)
     pix_painter = QPainter(pix)
     svg_renderer.render(pix_painter)
 
     return pix
 
 
 
-    # """
-    # Changes the color of an SVG image and returns a QPixmap
-    #
-    # https://stackoverflow.com/questions/15123544/change-the-color-of-an-svg-in-qt
-    # """
-    #
-    # from qtpy.QtGui import Qt, QPainter
-    # from qtpy.QtXml import QDomDocument, QDomElement
-    # from qtpy.QtSvg import QSvgRenderer
-    # from qtpy.QtGui import QPixmap
-    #
-    #
-    # def change_svg_color__set_attr_recur(elem: QDomElement, strtagname: str, strattr: str, strattrval: str):
-    #
-    #     # if it has the tag name then overwrite desired attribute
-    #     if elem.tagName() == strtagname:
-    #         elem.setAttribute(strattr, strattrval)
-    #
-    #     # loop all children
-    #     for i in range(elem.childNodes().count()):
-    #         if not elem.childNodes().at(i).isElement():
-    #             continue
-    #
-    #         change_svg_color__set_attr_recur(elem.childNodes().at(i).toElement(), strtagname, strattr, strattrval)
-    #
-    #
-    # # open svg resource load contents to qbytearray
-    # f = open(filepath)
-    # data = f.read()
-    # f.close()
-    # # load svg contents to xml document and edit contents
-    # doc = QDomDocument()
-    # doc.setContent(data)
-    # # recursively change color
-    # change_svg_color__set_attr_recur(doc.documentElement(), 'path', 'fill', color_hex)
-    # # create svg renderer with edited contents
-    # svg_renderer = QSvgRenderer(doc.toByteArray())
-    # # create pixmap target (could be a QImage)
-    # pix = QPixmap(svg_renderer.defaultSize())
-    # pix.fill(Qt.transparent)
-    # # create painter to act over pixmap
-    # pix_painter = QPainter(pix)
-    # # use renderer to render over painter which paints on pixmap
-    # svg_renderer.render(pix_painter)
-    #
-    # return pix
-
-
 def translate_project(project: Dict) -> Dict:
     """
     Transforms a v3.0 project file into something that can be loaded in v3.1,
     i.e. turns macros into scripts and removes macro nodes from the flows.
     """
-
+    # TODO: this needs to be changed to match ryvencore 0.4 structure
     new_project = project.copy()
 
     # turn macros into scripts
 
     fixed_scripts = []
 
     for script in (project['macro scripts']+project['scripts']):
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt.egg-info/PKG-INFO` & `ryvencore-qt-0.4.0a2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-Metadata-Version: 2.1
-Name: ryvencore-qt
-Version: 0.3.1.4
-Summary: Qt frontend for ryvencore; Library for building Visual Node Editors
-Home-page: https://github.com/leon-thomm/ryvencore-qt
-Author: Leon Thomm
-Author-email: l.thomm@mailbox.org
-Project-URL: Website, https://ryven.org
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 <p align="center">
   <img src="./ryvencore_qt/resources/pics/logo.png" alt="drawing" width="70%"/>
 </p>
 
-`rvencore-qt` is a wrapper around [ryvencore](https://github.com/leon-thomm/ryvencore) and provides a Qt frontend for it. It comes from the [Ryven](https://github.com/leon-thomm/Ryven) project and will be the foundation for future Ryven versions. So, ryvencore-qt can be used to build cross-platform standalone visual node editors based on Python. Projects made with ryvencore-qt can be natively deployed directly on the backend, ryvencore. The development of ryvencore-qt is currently closely tied to Ryven.
+`ryvencore-qt` provides Qt-based GUI classes for [ryvencore](https://github.com/leon-thomm/ryvencore), to provide a visual flow-based programming interface. The [Ryven](https://github.com/leon-thomm/Ryven) editor is built on top of `ryvencore-qt`, and their development is currently tightly coupled.
 
 ### Installation
 
+You need to have Python and pip installed. Then, either install from PyPI using pip:
+
 ```
 pip install ryvencore-qt
 ```
 
 or build from sources
+
 ```
 git clone https://github.com/leon-thomm/ryvencore-qt
 cd ryvencore-qt
 pip install .
 ```
 
 ### Dependencies
 
-ryvencore-qt runs on PySide2 (Python bindings for Qt) using [QtPy](https://github.com/spyder-ide/qtpy) as a wrapper to (eventually, once supported) enable seamless switching between PySide2 and PySide6. Notice that `ryvencore-qt` does not work with PyQt, due to crucial inheritance restrictions in PyQt.
+ryvencore-qt uses Python bindings for Qt using [QtPy](https://github.com/spyder-ide/qtpy). I usually run it with PySide2, running on PySide6 should also work with minor changes. PyQt is not supported, due to crucial inheritance restrictions in PyQt.
+
+### Documentation
+
+An extensive documentation doesn't currently exist.
 
 ### quick start
 
 The below code demonstrates how to set up an editor with custom defined nodes. You can also find the code in the *examples* folder.
 
 `main.py`
 ``` python
@@ -130,33 +122,12 @@
 
 export_nodes = [
     PrintNode,
     RandNode,
 ]
 ```
 
-For a more detailed overview, including a precise definition of flows, see the [Features Page](https://leon-thomm.github.io/ryvencore-qt/features/) and [ryvencore](https://github.com/leon-thomm/ryvencore).
-
 ### Development
 
-The code is not 100% PEP 8 conform, and some parts which are under development might seem messy. I'm doing my best :) feel free to improve. The individual subpackages have their own READMEs giving a quick overview which should be quite helpful to gain understanding about implementations.
-
-Cheers.
-
-<!--
-### Contributions and Development
-
-This project will eventually need a community in order to survive. Particularly effective ways to contribute outside of direct development of the software are creating
-
-- tutorials
-- nodes
-- small editors
-- documentation
-- tests
-- etc
-
-If you have any questions, suggestions, or want to show something you've built with this project notice the *discussions* area which is the perfect place for that.
-
-To give a quick overview over the most important class relations, see the below class diagram. The DrawIO diagram file is in the repository.
+The individual subpackages have their own READMEs giving a quick overview which should be quite helpful to gain understanding about implementations.
 
-![](./docs/img/ryvencore-drawio_.png)
--->
+Cheers.
```

### Comparing `ryvencore-qt-0.3.1.4/ryvencore_qt.egg-info/SOURCES.txt` & `ryvencore-qt-0.4.0a2/ryvencore_qt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ryvencore_qt.egg-info/SOURCES.txt
 ryvencore_qt.egg-info/dependency_links.txt
 ryvencore_qt.egg-info/requires.txt
 ryvencore_qt.egg-info/top_level.txt
 ryvencore_qt/resources/__init__.py
 ryvencore_qt/resources/node_collapse_icon.svg
 ryvencore_qt/resources/node_expand_icon.svg
+ryvencore_qt/resources/warning.svg
 ryvencore_qt/resources/fonts/__init__.py
 ryvencore_qt/resources/fonts/asap/Asap-Bold.ttf
 ryvencore_qt/resources/fonts/asap/Asap-BoldItalic.ttf
 ryvencore_qt/resources/fonts/asap/Asap-Italic.ttf
 ryvencore_qt/resources/fonts/asap/Asap-Medium.ttf
 ryvencore_qt/resources/fonts/asap/Asap-MediumItalic.ttf
 ryvencore_qt/resources/fonts/asap/Asap-Regular.ttf
@@ -90,32 +91,22 @@
 ryvencore_qt/resources/pics/macro_node_icon.png
 ryvencore_qt/resources/pics/macro_script_picture.png
 ryvencore_qt/resources/pics/opencv_example.png
 ryvencore_qt/resources/pics/script_picture.png
 ryvencore_qt/resources/pics/script_picture.svg
 ryvencore_qt/resources/pics/script_picture_old.png
 ryvencore_qt/resources/pics/variable_picture.png
+ryvencore_qt/resources/pics/warning.png
 ryvencore_qt/src/Design.py
 ryvencore_qt/src/GUIBase.py
 ryvencore_qt/src/GlobalAttributes.py
 ryvencore_qt/src/RCQT.py
-ryvencore_qt/src/SessionThreadInterface.py
+ryvencore_qt/src/SessionGUI.py
 ryvencore_qt/src/__init__.py
 ryvencore_qt/src/utils.py
-ryvencore_qt/src/conv_gui/EditVal_Dialog.py
-ryvencore_qt/src/conv_gui/ListWidget_NameLineEdit.py
-ryvencore_qt/src/conv_gui/LogWidget.py
-ryvencore_qt/src/conv_gui/ScriptsListWidget.py
-ryvencore_qt/src/conv_gui/ScriptsList_ScriptWidget.py
-ryvencore_qt/src/conv_gui/VariablesListWidget.py
-ryvencore_qt/src/conv_gui/VarsList_VarWidget.py
-ryvencore_qt/src/conv_gui/__init__.py
-ryvencore_qt/src/core_wrapper/Node.py
-ryvencore_qt/src/core_wrapper/Session.py
-ryvencore_qt/src/core_wrapper/__init__.py
 ryvencore_qt/src/flows/FlowCommands.py
 ryvencore_qt/src/flows/FlowTheme.py
 ryvencore_qt/src/flows/FlowView.py
 ryvencore_qt/src/flows/FlowViewProxyWidget.py
 ryvencore_qt/src/flows/FlowViewStylusModesWidget.py
 ryvencore_qt/src/flows/FlowViewZoomWidget.py
 ryvencore_qt/src/flows/__init__.py
@@ -123,18 +114,28 @@
 ryvencore_qt/src/flows/connections/__init__.py
 ryvencore_qt/src/flows/drawings/DrawingObject.py
 ryvencore_qt/src/flows/drawings/__init__.py
 ryvencore_qt/src/flows/node_list_widget/NodeListWidget.py
 ryvencore_qt/src/flows/node_list_widget/NodeWidget.py
 ryvencore_qt/src/flows/node_list_widget/__init__.py
 ryvencore_qt/src/flows/node_list_widget/utils.py
+ryvencore_qt/src/flows/nodes/NodeErrorIndicator.py
+ryvencore_qt/src/flows/nodes/NodeGUI.py
 ryvencore_qt/src/flows/nodes/NodeItem.py
 ryvencore_qt/src/flows/nodes/NodeItemAction.py
 ryvencore_qt/src/flows/nodes/NodeItemAnimator.py
 ryvencore_qt/src/flows/nodes/NodeItemWidget.py
 ryvencore_qt/src/flows/nodes/NodeItem_CollapseButton.py
 ryvencore_qt/src/flows/nodes/NodeItem_Icon.py
 ryvencore_qt/src/flows/nodes/NodeItem_TitleLabel.py
 ryvencore_qt/src/flows/nodes/PortItem.py
 ryvencore_qt/src/flows/nodes/PortItemInputWidgets.py
 ryvencore_qt/src/flows/nodes/WidgetBaseClasses.py
-ryvencore_qt/src/flows/nodes/__init__.py
+ryvencore_qt/src/flows/nodes/__init__.py
+ryvencore_qt/src/widgets/EditVal_Dialog.py
+ryvencore_qt/src/widgets/FlowsListWidget.py
+ryvencore_qt/src/widgets/FlowsList_FlowWidget.py
+ryvencore_qt/src/widgets/ListWidget_NameLineEdit.py
+ryvencore_qt/src/widgets/LogWidget.py
+ryvencore_qt/src/widgets/VariablesListWidget.py
+ryvencore_qt/src/widgets/VarsList_VarWidget.py
+ryvencore_qt/src/widgets/__init__.py
```

### Comparing `ryvencore-qt-0.3.1.4/setup.cfg` & `ryvencore-qt-0.4.0a2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ryvencore-qt
-version = v0.3.1.4
+version = v0.4.0a2
 author = Leon Thomm
 author_email = l.thomm@mailbox.org
 description = Qt frontend for ryvencore; Library for building Visual Node Editors
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 url = https://github.com/leon-thomm/ryvencore-qt
@@ -16,16 +16,17 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 install_requires = 
-	ryvencore ==0.3.1.*
+	ryvencore ==0.4.*
 	PySide2
 	QtPy
 	waiting
+	textdistance
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

