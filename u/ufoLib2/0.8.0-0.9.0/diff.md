# Comparing `tmp/ufoLib2-0.8.0.zip` & `tmp/ufoLib2-0.9.0.zip`

## zipinfo {}

```diff
@@ -1,99 +1,100 @@
-Zip file size: 82448 bytes, number of entries: 97
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/src/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/.github/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/tests/
--rw-r--r--  2.0 unx      466 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/requirements.txt
--rw-r--r--  2.0 unx      227 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/.editorconfig
--rw-r--r--  2.0 unx     1445 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/.gitignore
--rw-r--r--  2.0 unx      561 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/mypy.ini
--rw-r--r--  2.0 unx       94 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/setup.py
--rw-r--r--  2.0 unx     1013 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/setup.cfg
--rw-r--r--  2.0 unx      165 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/.pyup.yml
--rw-r--r--  2.0 unx      398 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/.readthedocs.yml
--rw-r--r--  2.0 unx     1231 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/requirements-dev.txt
--rw-r--r--  2.0 unx    11357 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/LICENSE
--rw-r--r--  2.0 unx       51 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/requirements-dev.in
--rw-r--r--  2.0 unx      289 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/.gitattributes
--rw-r--r--  2.0 unx      272 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/pyproject.toml
--rw-r--r--  2.0 unx      782 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/.coveragerc
--rw-r--r--  2.0 unx     1313 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/PKG-INFO
--rw-r--r--  2.0 unx      553 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/README.md
--rw-r--r--  2.0 unx       77 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/.codecov.yml
--rw-r--r--  2.0 unx     1089 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tox.ini
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/pointPens/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/
--rw-r--r--  2.0 unx        0 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/py.typed
--rw-r--r--  2.0 unx      634 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/typing.py
--rw-r--r--  2.0 unx      235 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/__init__.py
--rw-r--r--  2.0 unx       80 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/constants.py
--rw-r--r--  2.0 unx      116 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/_version.py
--rw-r--r--  2.0 unx       66 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/errors.py
--rw-r--r--  2.0 unx     1865 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/pointPens/glyphPointPen.py
--rw-r--r--  2.0 unx        0 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/pointPens/__init__.py
--rw-r--r--  2.0 unx     1437 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/guideline.py
--rw-r--r--  2.0 unx     1844 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/imageSet.py
--rw-r--r--  2.0 unx      385 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/features.py
--rw-r--r--  2.0 unx     2014 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/image.py
--rw-r--r--  2.0 unx    11060 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/layerSet.py
--rw-r--r--  2.0 unx    21341 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/font.py
--rw-r--r--  2.0 unx    18759 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/glyph.py
--rw-r--r--  2.0 unx      789 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/anchor.py
--rw-r--r--  2.0 unx     1177 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/point.py
--rw-r--r--  2.0 unx     1494 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/dataSet.py
--rw-r--r--  2.0 unx      634 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/__init__.py
--rw-r--r--  2.0 unx    10213 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/info.py
--rw-r--r--  2.0 unx    11348 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/layer.py
--rw-r--r--  2.0 unx     5654 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/contour.py
--rw-r--r--  2.0 unx     2837 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/component.py
--rw-r--r--  2.0 unx     7832 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2/objects/misc.py
--rw-r--r--  2.0 unx     2413 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        8 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2.egg-info/top_level.txt
--rw-r--r--  2.0 unx       94 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2.egg-info/requires.txt
--rw-r--r--  2.0 unx     1313 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/src/ufoLib2.egg-info/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/.github/workflows/
--rw-r--r--  2.0 unx     1355 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/.github/workflows/test.yml
--rw-r--r--  2.0 unx      923 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/.github/workflows/publish.yml
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/docs/source/
--rw-r--r--  2.0 unx       91 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/docs/requirements.txt
--rw-r--r--  2.0 unx      752 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/docs/source/index.rst
--rw-r--r--  2.0 unx     2427 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/docs/source/explanations.rst
--rw-r--r--  2.0 unx     2031 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/docs/source/reference.rst
--rw-r--r--  2.0 unx     2110 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/docs/source/conf.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/tests/objects/
--rw-r--r--  2.0 unx      350 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/conftest.py
--rw-r--r--  2.0 unx     4669 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/test_ufoLib2.py
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/
--rw-r--r--  2.0 unx     4673 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/LICENSE_UbuTestData.txt
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs.public.background/
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs/
--rw-r--r--  2.0 unx      401 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/layercontents.plist
--rw-r--r--  2.0 unx     7444 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/fontinfo.plist
--rw-r--r--  2.0 unx      300 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/lib.plist
--rw-r--r--  2.0 unx      318 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/metainfo.plist
-drwxr-xr-x  2.0 unx        0 b- stor 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/
--rw-r--r--  2.0 unx      594 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.daltonmaag.vttLib.plist
--rw-r--r--  2.0 unx     1440 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__3.ttx
--rw-r--r--  2.0 unx      204 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__5.ttx
--rw-r--r--  2.0 unx      189 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__2.ttx
--rw-r--r--  2.0 unx      189 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__0.ttx
--rw-r--r--  2.0 unx    44327 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__1.ttx
--rw-r--r--  2.0 unx      863 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs.public.background/A_.glif
--rw-r--r--  2.0 unx      283 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs.public.background/contents.plist
--rw-r--r--  2.0 unx     1588 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs.public.background/a.glif
--rw-r--r--  2.0 unx     1026 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs/A_.glif
--rw-r--r--  2.0 unx      283 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs/contents.plist
--rw-r--r--  2.0 unx     1903 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs/a.glif
--rw-r--r--  2.0 unx     2982 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/objects/test_layer.py
--rw-r--r--  2.0 unx    10253 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/objects/test_glyph.py
--rw-r--r--  2.0 unx     1131 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/objects/test_component.py
--rw-r--r--  2.0 unx     1993 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/objects/test_font.py
--rw-r--r--  2.0 unx     1001 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/objects/test_datastore.py
--rw-r--r--  2.0 unx      593 b- defN 20-Jun-03 10:18 ufoLib2-0.8.0/tests/objects/test_contour.py
-97 files, 225712 bytes uncompressed, 66940 bytes compressed:  70.3%
+Zip file size: 84771 bytes, number of entries: 98
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/.github/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/src/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/tests/
+-rw-r--r--  2.0 unx      782 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/.coveragerc
+-rw-r--r--  2.0 unx       51 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/requirements-dev.in
+-rw-r--r--  2.0 unx      220 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/pyproject.toml
+-rw-r--r--  2.0 unx       77 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/.codecov.yml
+-rw-r--r--  2.0 unx     1077 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tox.ini
+-rw-r--r--  2.0 unx      165 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/.pyup.yml
+-rw-r--r--  2.0 unx      289 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/.gitattributes
+-rw-r--r--  2.0 unx      553 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/README.md
+-rw-r--r--  2.0 unx    11357 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/LICENSE
+-rw-r--r--  2.0 unx     1230 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/requirements-dev.txt
+-rw-r--r--  2.0 unx      398 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/.readthedocs.yml
+-rw-r--r--  2.0 unx     1013 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/setup.cfg
+-rw-r--r--  2.0 unx      227 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/.editorconfig
+-rw-r--r--  2.0 unx      561 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/mypy.ini
+-rw-r--r--  2.0 unx       93 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/setup.py
+-rw-r--r--  2.0 unx     1445 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/.gitignore
+-rw-r--r--  2.0 unx     1313 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/PKG-INFO
+-rw-r--r--  2.0 unx      466 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/requirements.txt
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/.github/workflows/
+-rw-r--r--  2.0 unx      923 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/.github/workflows/publish.yml
+-rw-r--r--  2.0 unx     1399 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/.github/workflows/test.yml
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/
+-rw-r--r--  2.0 unx       94 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     2446 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        8 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1313 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2.egg-info/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/pointPens/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/
+-rw-r--r--  2.0 unx        0 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/py.typed
+-rw-r--r--  2.0 unx       66 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/errors.py
+-rw-r--r--  2.0 unx      235 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/__init__.py
+-rw-r--r--  2.0 unx      839 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/typing.py
+-rw-r--r--  2.0 unx      317 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/constants.py
+-rw-r--r--  2.0 unx      116 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/_version.py
+-rw-r--r--  2.0 unx        0 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/pointPens/__init__.py
+-rw-r--r--  2.0 unx     1865 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/pointPens/glyphPointPen.py
+-rw-r--r--  2.0 unx     2837 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/component.py
+-rw-r--r--  2.0 unx     1494 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/dataSet.py
+-rw-r--r--  2.0 unx     1177 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/point.py
+-rw-r--r--  2.0 unx    11060 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/layerSet.py
+-rw-r--r--  2.0 unx    10210 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/info.py
+-rw-r--r--  2.0 unx    19746 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/glyph.py
+-rw-r--r--  2.0 unx      634 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/__init__.py
+-rw-r--r--  2.0 unx      385 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/features.py
+-rw-r--r--  2.0 unx     5654 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/contour.py
+-rw-r--r--  2.0 unx     2016 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/image.py
+-rw-r--r--  2.0 unx    22418 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/font.py
+-rw-r--r--  2.0 unx     1844 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/imageSet.py
+-rw-r--r--  2.0 unx    12252 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/layer.py
+-rw-r--r--  2.0 unx     1437 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/guideline.py
+-rw-r--r--  2.0 unx     9114 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/misc.py
+-rw-r--r--  2.0 unx      789 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/src/ufoLib2/objects/anchor.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/docs/source/
+-rw-r--r--  2.0 unx       91 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/docs/requirements.txt
+-rw-r--r--  2.0 unx     2136 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/docs/source/conf.py
+-rw-r--r--  2.0 unx     2031 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/docs/source/reference.rst
+-rw-r--r--  2.0 unx     2427 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/docs/source/explanations.rst
+-rw-r--r--  2.0 unx      752 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/docs/source/index.rst
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/tests/objects/
+-rw-r--r--  2.0 unx     4669 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/test_ufoLib2.py
+-rw-r--r--  2.0 unx      350 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/conftest.py
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/
+-rw-r--r--  2.0 unx     4673 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/LICENSE_UbuTestData.txt
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs.public.background/
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs/
+-rw-r--r--  2.0 unx      401 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/layercontents.plist
+-rw-r--r--  2.0 unx     7444 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/fontinfo.plist
+-rw-r--r--  2.0 unx      318 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/metainfo.plist
+-rw-r--r--  2.0 unx      300 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/lib.plist
+drwxr-xr-x  2.0 unx        0 b- stor 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/
+-rw-r--r--  2.0 unx      594 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.daltonmaag.vttLib.plist
+-rw-r--r--  2.0 unx      189 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__2.ttx
+-rw-r--r--  2.0 unx      204 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__5.ttx
+-rw-r--r--  2.0 unx     1440 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__3.ttx
+-rw-r--r--  2.0 unx    44327 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__1.ttx
+-rw-r--r--  2.0 unx      189 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__0.ttx
+-rw-r--r--  2.0 unx     1588 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs.public.background/a.glif
+-rw-r--r--  2.0 unx      863 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs.public.background/A_.glif
+-rw-r--r--  2.0 unx      283 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs.public.background/contents.plist
+-rw-r--r--  2.0 unx     1903 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs/a.glif
+-rw-r--r--  2.0 unx     1026 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs/A_.glif
+-rw-r--r--  2.0 unx      283 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs/contents.plist
+-rw-r--r--  2.0 unx     2982 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/objects/test_layer.py
+-rw-r--r--  2.0 unx      593 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/objects/test_contour.py
+-rw-r--r--  2.0 unx    10253 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/objects/test_glyph.py
+-rw-r--r--  2.0 unx     1001 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/objects/test_datastore.py
+-rw-r--r--  2.0 unx     1993 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/objects/test_font.py
+-rw-r--r--  2.0 unx     3412 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/objects/test_object_lib.py
+-rw-r--r--  2.0 unx     1131 b- defN 20-Nov-27 14:45 ufoLib2-0.9.0/tests/objects/test_component.py
+98 files, 233852 bytes uncompressed, 69095 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -1,292 +1,295 @@
-Filename: ufoLib2-0.8.0/
+Filename: ufoLib2-0.9.0/
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/
+Filename: ufoLib2-0.9.0/.github/
 Comment: 
 
-Filename: ufoLib2-0.8.0/.github/
+Filename: ufoLib2-0.9.0/src/
 Comment: 
 
-Filename: ufoLib2-0.8.0/docs/
+Filename: ufoLib2-0.9.0/docs/
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/
+Filename: ufoLib2-0.9.0/tests/
 Comment: 
 
-Filename: ufoLib2-0.8.0/requirements.txt
+Filename: ufoLib2-0.9.0/.coveragerc
 Comment: 
 
-Filename: ufoLib2-0.8.0/.editorconfig
+Filename: ufoLib2-0.9.0/requirements-dev.in
 Comment: 
 
-Filename: ufoLib2-0.8.0/.gitignore
+Filename: ufoLib2-0.9.0/pyproject.toml
 Comment: 
 
-Filename: ufoLib2-0.8.0/mypy.ini
+Filename: ufoLib2-0.9.0/.codecov.yml
 Comment: 
 
-Filename: ufoLib2-0.8.0/setup.py
+Filename: ufoLib2-0.9.0/tox.ini
 Comment: 
 
-Filename: ufoLib2-0.8.0/setup.cfg
+Filename: ufoLib2-0.9.0/.pyup.yml
 Comment: 
 
-Filename: ufoLib2-0.8.0/.pyup.yml
+Filename: ufoLib2-0.9.0/.gitattributes
 Comment: 
 
-Filename: ufoLib2-0.8.0/.readthedocs.yml
+Filename: ufoLib2-0.9.0/README.md
 Comment: 
 
-Filename: ufoLib2-0.8.0/requirements-dev.txt
+Filename: ufoLib2-0.9.0/LICENSE
 Comment: 
 
-Filename: ufoLib2-0.8.0/LICENSE
+Filename: ufoLib2-0.9.0/requirements-dev.txt
 Comment: 
 
-Filename: ufoLib2-0.8.0/requirements-dev.in
+Filename: ufoLib2-0.9.0/.readthedocs.yml
 Comment: 
 
-Filename: ufoLib2-0.8.0/.gitattributes
+Filename: ufoLib2-0.9.0/setup.cfg
 Comment: 
 
-Filename: ufoLib2-0.8.0/pyproject.toml
+Filename: ufoLib2-0.9.0/.editorconfig
 Comment: 
 
-Filename: ufoLib2-0.8.0/.coveragerc
+Filename: ufoLib2-0.9.0/mypy.ini
 Comment: 
 
-Filename: ufoLib2-0.8.0/PKG-INFO
+Filename: ufoLib2-0.9.0/setup.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/README.md
+Filename: ufoLib2-0.9.0/.gitignore
 Comment: 
 
-Filename: ufoLib2-0.8.0/.codecov.yml
+Filename: ufoLib2-0.9.0/PKG-INFO
 Comment: 
 
-Filename: ufoLib2-0.8.0/tox.ini
+Filename: ufoLib2-0.9.0/requirements.txt
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/
+Filename: ufoLib2-0.9.0/.github/workflows/
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2.egg-info/
+Filename: ufoLib2-0.9.0/.github/workflows/publish.yml
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/pointPens/
+Filename: ufoLib2-0.9.0/.github/workflows/test.yml
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/
+Filename: ufoLib2-0.9.0/src/ufoLib2.egg-info/
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/py.typed
+Filename: ufoLib2-0.9.0/src/ufoLib2/
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/typing.py
+Filename: ufoLib2-0.9.0/src/ufoLib2.egg-info/requires.txt
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/__init__.py
+Filename: ufoLib2-0.9.0/src/ufoLib2.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/constants.py
+Filename: ufoLib2-0.9.0/src/ufoLib2.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/_version.py
+Filename: ufoLib2-0.9.0/src/ufoLib2.egg-info/top_level.txt
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/errors.py
+Filename: ufoLib2-0.9.0/src/ufoLib2.egg-info/PKG-INFO
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/pointPens/glyphPointPen.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/pointPens/
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/pointPens/__init__.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/guideline.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/py.typed
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/imageSet.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/errors.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/features.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/__init__.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/image.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/typing.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/layerSet.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/constants.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/font.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/_version.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/glyph.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/pointPens/__init__.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/anchor.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/pointPens/glyphPointPen.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/point.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/component.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/dataSet.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/dataSet.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/__init__.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/point.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/info.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/layerSet.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/layer.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/info.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/contour.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/glyph.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/component.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/__init__.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2/objects/misc.py
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/features.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2.egg-info/SOURCES.txt
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/contour.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2.egg-info/dependency_links.txt
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/image.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2.egg-info/top_level.txt
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/font.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2.egg-info/requires.txt
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/imageSet.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/src/ufoLib2.egg-info/PKG-INFO
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/layer.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/.github/workflows/
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/guideline.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/.github/workflows/test.yml
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/misc.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/.github/workflows/publish.yml
+Filename: ufoLib2-0.9.0/src/ufoLib2/objects/anchor.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/docs/source/
+Filename: ufoLib2-0.9.0/docs/source/
 Comment: 
 
-Filename: ufoLib2-0.8.0/docs/requirements.txt
+Filename: ufoLib2-0.9.0/docs/requirements.txt
 Comment: 
 
-Filename: ufoLib2-0.8.0/docs/source/index.rst
+Filename: ufoLib2-0.9.0/docs/source/conf.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/docs/source/explanations.rst
+Filename: ufoLib2-0.9.0/docs/source/reference.rst
 Comment: 
 
-Filename: ufoLib2-0.8.0/docs/source/reference.rst
+Filename: ufoLib2-0.9.0/docs/source/explanations.rst
 Comment: 
 
-Filename: ufoLib2-0.8.0/docs/source/conf.py
+Filename: ufoLib2-0.9.0/docs/source/index.rst
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/
+Filename: ufoLib2-0.9.0/tests/data/
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/objects/
+Filename: ufoLib2-0.9.0/tests/objects/
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/conftest.py
+Filename: ufoLib2-0.9.0/tests/test_ufoLib2.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/test_ufoLib2.py
+Filename: ufoLib2-0.9.0/tests/conftest.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/LICENSE_UbuTestData.txt
+Filename: ufoLib2-0.9.0/tests/data/LICENSE_UbuTestData.txt
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs.public.background/
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs.public.background/
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs/
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs/
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/layercontents.plist
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/layercontents.plist
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/fontinfo.plist
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/fontinfo.plist
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/lib.plist
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/metainfo.plist
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/metainfo.plist
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/lib.plist
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.daltonmaag.vttLib.plist
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.daltonmaag.vttLib.plist
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__3.ttx
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__2.ttx
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__5.ttx
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__5.ttx
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__2.ttx
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__3.ttx
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__0.ttx
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__1.ttx
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__1.ttx
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__0.ttx
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs.public.background/A_.glif
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs.public.background/a.glif
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs.public.background/contents.plist
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs.public.background/A_.glif
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs.public.background/a.glif
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs.public.background/contents.plist
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs/A_.glif
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs/a.glif
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs/contents.plist
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs/A_.glif
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs/a.glif
+Filename: ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs/contents.plist
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/objects/test_layer.py
+Filename: ufoLib2-0.9.0/tests/objects/test_layer.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/objects/test_glyph.py
+Filename: ufoLib2-0.9.0/tests/objects/test_contour.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/objects/test_component.py
+Filename: ufoLib2-0.9.0/tests/objects/test_glyph.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/objects/test_font.py
+Filename: ufoLib2-0.9.0/tests/objects/test_datastore.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/objects/test_datastore.py
+Filename: ufoLib2-0.9.0/tests/objects/test_font.py
 Comment: 
 
-Filename: ufoLib2-0.8.0/tests/objects/test_contour.py
+Filename: ufoLib2-0.9.0/tests/objects/test_object_lib.py
+Comment: 
+
+Filename: ufoLib2-0.9.0/tests/objects/test_component.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ufoLib2-0.8.0/.gitignore` & `ufoLib2-0.9.0/.gitignore`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/mypy.ini` & `ufoLib2-0.9.0/mypy.ini`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/setup.cfg` & `ufoLib2-0.9.0/setup.cfg`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/requirements-dev.txt` & `ufoLib2-0.9.0/requirements-dev.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #
 # This file is autogenerated by pip-compile
 # To update, run:
 #
 #    pip-compile requirements-dev.in
 #
 appdirs==1.4.4            # via black
-attrs==19.3.0             # via black, pytest
-black==19.10b0            # via -r requirements-dev.in
+attrs==20.3.0             # via black, pytest
+black==20.8b1            # via -r requirements-dev.in
 click==7.1.2              # via black
-coverage==5.1           # via -r requirements-dev.in
+coverage==5.3           # via -r requirements-dev.in
 entrypoints==0.3          # via flake8
-flake8==3.8.2             # via -r requirements-dev.in
-isort[pyproject]==4.3.21  # via -r requirements-dev.in
+flake8==3.8.4             # via -r requirements-dev.in
+isort[pyproject]==5.6.4  # via -r requirements-dev.in
 mccabe==0.6.1             # via flake8
-more-itertools==8.3.0     # via pytest
+more-itertools==8.6.0     # via pytest
 mypy-extensions==0.4.3    # via mypy
-mypy==0.770               # via -r requirements-dev.in
+mypy==0.790               # via -r requirements-dev.in
 packaging==20.4           # via pytest
-pathspec==0.8.0           # via black
+pathspec==0.8.1           # via black
 pluggy==0.13.1            # via pytest
-py==1.8.1                 # via pytest
+py==1.9.0                 # via pytest
 pycodestyle==2.6.0        # via flake8
 pyflakes==2.2.0           # via flake8
 pyparsing==2.4.7          # via packaging
-pytest==5.4.2             # via -r requirements-dev.in
-regex==2020.5.14          # via black
+pytest==6.1.2             # via -r requirements-dev.in
+regex==2020.11.13          # via black
 six==1.15.0               # via packaging
-toml==0.10.1              # via black, isort
+toml==0.10.2              # via black, isort
 typed-ast==1.4.1          # via black, mypy
-typing-extensions==3.7.4.2  # via mypy
-wcwidth==0.1.9            # via pytest
+typing-extensions==3.7.4.3  # via mypy
+wcwidth==0.2.5            # via pytest
```

## Comparing `ufoLib2-0.8.0/LICENSE` & `ufoLib2-0.9.0/LICENSE`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/.coveragerc` & `ufoLib2-0.9.0/.coveragerc`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/PKG-INFO` & `ufoLib2-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufoLib2
-Version: 0.8.0
+Version: 0.9.0
 Summary: ufoLib2 is a UFO font processing library.
 Home-page: https://github.com/fonttools/ufoLib2
 Author: Adrien Tétar
 Author-email: adri-from-59@hotmail.fr
 License: Apache 2.0
 Description: # ufoLib2
```

## Comparing `ufoLib2-0.8.0/README.md` & `ufoLib2-0.9.0/README.md`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tox.ini` & `ufoLib2-0.9.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [testenv:lint]
 skip_install = true
 deps =
     -r requirements.txt
     -r requirements-dev.txt
 commands =
     black --check --diff .
-    isort --check-only --diff --recursive src tests
+    isort --check-only --diff src tests
     mypy src tests .
     flake8
 
 [testenv:docs]
 deps =
     -r docs/requirements.txt
 skip_install = true
```

## Comparing `ufoLib2-0.8.0/src/ufoLib2/typing.py` & `ufoLib2-0.9.0/src/ufoLib2/typing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import sys
-from typing import TypeVar, Union
+from typing import Optional, TypeVar, Union
 
 from fontTools.pens.basePen import AbstractPen
 
 if sys.version_info >= (3, 8):
     from typing import Protocol
 else:
     from typing_extensions import Protocol
@@ -21,7 +21,14 @@
     """Stand-in for an object that can draw itself with a given pen.
 
     See :mod:`fontTools.pens.basePen` for an introduction to pens.
     """
 
     def draw(self, pen: AbstractPen) -> None:
         ...
+
+
+class HasIdentifier(Protocol):
+    """Any object that has a unique identifier in some context that can be
+    used as a key in a public.objectLibs dictionary."""
+
+    identifier: Optional[str]
```

## Comparing `ufoLib2-0.8.0/src/ufoLib2/pointPens/glyphPointPen.py` & `ufoLib2-0.9.0/src/ufoLib2/pointPens/glyphPointPen.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/guideline.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/guideline.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/imageSet.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/imageSet.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/image.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         "xyScale",
         "yxScale",
         "yScale",
         "xOffset",
         "yOffset",
     )
     _valid_keys_: Tuple[str, str, str, str, str, str, str, str] = (
-        "fileName",
-    ) + _transformation_keys_ + ("color",)
+        ("fileName",) + _transformation_keys_ + ("color",)
+    )
 
     def __getitem__(self, key: str) -> Any:
         try:
             i = self._transformation_keys_.index(key)
         except ValueError:
             try:
                 return getattr(self, key)
```

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/layerSet.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/layerSet.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/font.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/font.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,21 @@
 from ufoLib2.objects.features import Features
 from ufoLib2.objects.glyph import Glyph
 from ufoLib2.objects.guideline import Guideline
 from ufoLib2.objects.imageSet import ImageSet
 from ufoLib2.objects.info import Info
 from ufoLib2.objects.layer import Layer
 from ufoLib2.objects.layerSet import LayerSet
-from ufoLib2.objects.misc import BoundingBox, _deepcopy_unlazify_attrs
-from ufoLib2.typing import PathLike, T
+from ufoLib2.objects.misc import (
+    BoundingBox,
+    _deepcopy_unlazify_attrs,
+    _object_lib,
+    _prune_object_libs,
+)
+from ufoLib2.typing import HasIdentifier, PathLike, T
 
 
 def _convert_Info(value: Union[Info, Mapping[str, Any]]) -> Info:
     return value if isinstance(value, Info) else Info(**value)
 
 
 def _convert_DataSet(value: Union[DataSet, Mapping[str, Any]]) -> DataSet:
@@ -120,35 +125,33 @@
     )
     """LayerSet: A mapping of layer names to Layer objects."""
 
     info: Info = attr.ib(factory=Info, converter=_convert_Info, kw_only=True)
     """Info: The font Info object."""
 
     features: Features = attr.ib(
-        factory=Features, converter=_convert_Features, kw_only=True,
+        factory=Features, converter=_convert_Features, kw_only=True
     )
     """Features: The font Features object."""
 
     groups: Dict[str, List[str]] = attr.ib(factory=dict, kw_only=True)
     """Dict[str, List[str]]: A mapping of group names to a list of glyph names."""
 
     kerning: Dict[Tuple[str, str], float] = attr.ib(factory=dict, kw_only=True)
     """Dict[Tuple[str, str], float]: A mapping of a tuple of first and second kerning
     pair to a kerning value."""
 
     lib: Dict[str, Any] = attr.ib(factory=dict, kw_only=True)
     """Dict[str, Any]: A mapping of keys to arbitrary values."""
 
-    data: DataSet = attr.ib(
-        factory=DataSet, converter=_convert_DataSet, kw_only=True,
-    )
+    data: DataSet = attr.ib(factory=DataSet, converter=_convert_DataSet, kw_only=True)
     """DataSet: A mapping of data file paths to arbitrary data."""
 
     images: ImageSet = attr.ib(
-        factory=ImageSet, converter=_convert_ImageSet, kw_only=True,
+        factory=ImageSet, converter=_convert_ImageSet, kw_only=True
     )
     """ImageSet: A mapping of image file paths to arbitrary image data."""
 
     _lazy: Optional[bool] = attr.ib(default=None, kw_only=True)
     _validate: bool = attr.ib(default=True, kw_only=True)
 
     _reader: Optional[UFOReader] = attr.ib(default=None, kw_only=True, init=False)
@@ -170,15 +173,15 @@
             self.lib = reader.readLib()
             self._fileStructure = reader.fileStructure
             if self._lazy:
                 # keep the reader around so we can close it when done
                 self._reader = reader
 
     @classmethod
-    def open(cls, path: PathLike, lazy: bool = True, validate: bool = True,) -> "Font":
+    def open(cls, path: PathLike, lazy: bool = True, validate: bool = True) -> "Font":
         """Instantiates a new Font object from a path to a UFO.
 
         Args:
             path: The path to the UFO to load.
             lazy: If True, load glyphs, data files and images as they are accessed. If
                 False, load everything up front.
             validate: If True, enable UFO data model validation during loading. If
@@ -364,14 +367,35 @@
 
     @guidelines.setter
     def guidelines(self, value: Iterable[Union[Guideline, Mapping[str, Any]]]) -> None:
         self.info.guidelines = []
         for guideline in value:
             self.appendGuideline(guideline)
 
+    def object_lib(self, object: HasIdentifier) -> Dict[str, Any]:
+        """Return the lib for an object with an identifier, as stored in a font's lib.
+
+        If the object does not yet have an identifier, a new one is assigned to it. If
+        the font lib does not yet contain the object's lib, a new one is inserted and
+        returned.
+
+        .. doctest::
+
+            >>> from ufoLib2.objects import Font, Guideline
+            >>> font = Font()
+            >>> font.guidelines = [Guideline(x=100)]
+            >>> guideline_lib = font.object_lib(font.guidelines[0])
+            >>> guideline_lib["com.test.foo"] = 1234
+            >>> guideline_id = font.guidelines[0].identifier
+            >>> assert guideline_id is not None
+            >>> assert font.lib["public.objectLibs"][guideline_id] is guideline_lib
+        """
+
+        return _object_lib(self.lib, object)
+
     @property
     def path(self) -> Optional[PathLike]:
         """Return the path of the UFO, if it was set, or None."""
         return self._path
 
     @property
     def bounds(self) -> Optional[BoundingBox]:
@@ -472,14 +496,18 @@
         if self.layers.defaultLayer.name != DEFAULT_LAYER_NAME:
             assert DEFAULT_LAYER_NAME not in self.layers.layerOrder
         # save font attrs
         writer.writeFeatures(self.features.text)
         writer.writeGroups(self.groups)
         writer.writeInfo(self.info)
         writer.writeKerning(self.kerning)
+        _prune_object_libs(
+            self.lib,
+            {g.identifier for g in self.guidelines if g.identifier is not None},
+        )
         writer.writeLib(self.lib)
         # save the layers
         self.layers.write(writer, saveAs=saveAs)
         # save bin parts
         self.data.write(writer, saveAs=saveAs)
         self.images.write(writer, saveAs=saveAs)
```

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/glyph.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/glyph.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 )
 
 from ufoLib2.objects.anchor import Anchor
 from ufoLib2.objects.component import Component
 from ufoLib2.objects.contour import Contour
 from ufoLib2.objects.guideline import Guideline
 from ufoLib2.objects.image import Image
-from ufoLib2.objects.misc import BoundingBox, getBounds, getControlBounds
+from ufoLib2.objects.misc import BoundingBox, _object_lib, getBounds, getControlBounds
 from ufoLib2.pointPens.glyphPointPen import GlyphPointPen
+from ufoLib2.typing import HasIdentifier
 
 if TYPE_CHECKING:
     from ufoLib2.objects.layer import Layer  # noqa: F401
 
 
 @attr.s(auto_attribs=True, slots=True, repr=False)
 class Glyph:
@@ -212,14 +213,36 @@
                     image["yScale"],
                     image["xOffset"],
                     image["yOffset"],
                 ),
                 color=image.get("color"),
             )
 
+    def object_lib(self, object: HasIdentifier) -> Dict[str, Any]:
+        """Return the lib for an object with an identifier, as stored in a glyph's lib.
+
+        If the object does not yet have an identifier, a new one is assigned to it. If
+        the font lib does not yet contain the object's lib, a new one is inserted and
+        returned.
+
+        .. doctest::
+
+            >>> from ufoLib2.objects import Font, Guideline
+            >>> font = Font()
+            >>> glyph = font.newGlyph("a")
+            >>> glyph.guidelines = [Guideline(x=100)]
+            >>> guideline_lib = glyph.object_lib(glyph.guidelines[0])
+            >>> guideline_lib["com.test.foo"] = 1234
+            >>> guideline_id = glyph.guidelines[0].identifier
+            >>> assert guideline_id is not None
+            >>> assert glyph.lib["public.objectLibs"][guideline_id] is guideline_lib
+        """
+
+        return _object_lib(self.lib, object)
+
     def clear(self) -> None:
         """Clears out anchors, components, contours, guidelines and image
         references."""
         del self._anchors[:]
         del self.components[:]
         del self.contours[:]
         del self._guidelines[:]
@@ -275,15 +298,15 @@
                 )
             guideline = Guideline(**guideline)
         self._guidelines.append(guideline)
 
     def appendContour(self, contour: Contour) -> None:
         """Appends a :class:`.Contour` object to glyph's list of contours."""
         if not isinstance(contour, Contour):
-            raise TypeError(f"Expected Contour, found {type(contour).__name__}",)
+            raise TypeError(f"Expected Contour, found {type(contour).__name__}")
         self.contours.append(contour)
 
     def copy(self, name: Optional[str] = None) -> "Glyph":
         """Returns a new Glyph (deep) copy, optionally override the new glyph
         name."""
         other = deepcopy(self)
         if name is not None:
```

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/anchor.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/anchor.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/point.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/point.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/dataSet.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/dataSet.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/__init__.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/__init__.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/info.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     ULTRA_EXPANDED = 9
 
 
 Tc = TypeVar("Tc", Guideline, GaspRangeRecord, NameRecord)
 
 
 def _convert_optional_list(
-    lst: Optional[Sequence[Any]], klass: Type[Tc],
+    lst: Optional[Sequence[Any]], klass: Type[Tc]
 ) -> Optional[List[Tc]]:
     if lst is None:
         return None
     result = []
     for d in lst:
         if isinstance(d, klass):
             result.append(d)
@@ -141,28 +141,28 @@
         return self._guidelines
 
     @guidelines.setter
     def guidelines(self, value: Optional[List[Guideline]]) -> None:
         self._guidelines = _convert_guidelines(value)
 
     _openTypeGaspRangeRecords: Optional[List[GaspRangeRecord]] = attr.ib(
-        default=None, converter=_convert_gasp_range_records,
+        default=None, converter=_convert_gasp_range_records
     )
 
     @property
     def openTypeGaspRangeRecords(self) -> Optional[List[GaspRangeRecord]]:
         return self._openTypeGaspRangeRecords
 
     @openTypeGaspRangeRecords.setter
     def openTypeGaspRangeRecords(self, value: Optional[List[GaspRangeRecord]]) -> None:
         self._openTypeGaspRangeRecords = _convert_gasp_range_records(value)
 
     openTypeHeadCreated: Optional[str] = None
     openTypeHeadLowestRecPPEM: Optional[int] = attr.ib(
-        default=None, validator=_optional_positive,
+        default=None, validator=_optional_positive
     )
     openTypeHeadFlags: Optional[List[int]] = None
 
     openTypeHheaAscender: Optional[int] = None
     openTypeHheaDescender: Optional[int] = None
     openTypeHheaLineGap: Optional[int] = None
     openTypeHheaCaretSlopeRise: Optional[int] = None
```

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/layer.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/layer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Any, Dict, Iterator, KeysView, Optional, Sequence, Type, Union
+from typing import Any, Dict, Iterator, KeysView, Optional, Sequence, Set, Type, Union
 
 import attr
 from fontTools.ufoLib.glifLib import GlyphSet
 
 from ufoLib2.constants import DEFAULT_LAYER_NAME
 from ufoLib2.objects.glyph import Glyph
 from ufoLib2.objects.misc import (
     _NOT_LOADED,
     BoundingBox,
     Placeholder,
     _deepcopy_unlazify_attrs,
+    _prune_object_libs,
     unionBounds,
 )
 from ufoLib2.typing import T
 
 
 def _convert_glyphs(
     value: Union[Dict[str, Union[Glyph, Placeholder]], Sequence[Glyph]]
@@ -321,15 +322,38 @@
                 glyphSet.deleteGlyph(name)
         for name, glyph in glyphs.items():
             if isinstance(glyph, Placeholder):
                 if saveAs:
                     glyph = self.loadGlyph(name)
                 else:
                     continue
+            _prune_object_libs(glyph.lib, _fetch_glyph_identifiers(glyph))
             glyphSet.writeGlyph(
                 name, glyphObject=glyph, drawPointsFunc=glyph.drawPoints
             )
         glyphSet.writeContents()
         glyphSet.writeLayerInfo(self)
         if saveAs:
             # all glyphs are loaded by now, no need to keep ref to glyphSet
             self._glyphSet = None
+
+
+def _fetch_glyph_identifiers(glyph: Glyph) -> Set[str]:
+    """Returns all identifiers in use in a glyph."""
+
+    identifiers = set()
+    for anchor in glyph.anchors:
+        if anchor.identifier is not None:
+            identifiers.add(anchor.identifier)
+    for guideline in glyph.guidelines:
+        if guideline.identifier is not None:
+            identifiers.add(guideline.identifier)
+    for contour in glyph.contours:
+        if contour.identifier is not None:
+            identifiers.add(contour.identifier)
+        for point in contour:
+            if point.identifier is not None:
+                identifiers.add(point.identifier)
+    for component in glyph.components:
+        if component.identifier is not None:
+            identifiers.add(component.identifier)
+    return identifiers
```

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/contour.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/contour.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/component.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/component.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/src/ufoLib2/objects/misc.py` & `ufoLib2-0.9.0/src/ufoLib2/objects/misc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import collections.abc
+import uuid
 from abc import abstractmethod
 from collections.abc import Mapping, MutableMapping
 from copy import deepcopy
 from typing import (
     Any,
     Dict,
     Iterator,
@@ -17,15 +19,16 @@
 
 import attr
 from fontTools.misc.arrayTools import unionRect
 from fontTools.misc.transform import Transform
 from fontTools.pens.boundsPen import BoundsPen, ControlBoundsPen
 from fontTools.ufoLib import UFOReader, UFOWriter
 
-from ufoLib2.typing import Drawable
+from ufoLib2.constants import OBJECT_LIBS_KEY
+from ufoLib2.typing import Drawable, HasIdentifier
 
 
 class BoundingBox(NamedTuple):
     """Represents a bounding box as a tuple of (xMin, yMin, xMax, yMax)."""
 
     xMin: float
     yMin: float
@@ -73,14 +76,49 @@
             )
             for a in attr.fields(self.__class__)
             if a.init and a.metadata.get("copyable", True)
         },
     )
 
 
+def _object_lib(parent_lib: Dict[str, Any], object: HasIdentifier) -> Dict[str, Any]:
+    if object.identifier is None:
+        # Use UUID4 because it allows us to set a new identifier without
+        # checking if it's already used anywhere else and be right most
+        # of the time.
+        object.identifier = str(uuid.uuid4())
+
+    if "public.objectLibs" not in parent_lib:
+        object_libs = parent_lib["public.objectLibs"] = {}
+    else:
+        object_libs = parent_lib["public.objectLibs"]
+        assert isinstance(object_libs, collections.abc.MutableMapping)
+
+    if object.identifier in object_libs:
+        return object_libs[object.identifier]
+    lib = object_libs[object.identifier] = {}
+    return lib
+
+
+def _prune_object_libs(parent_lib: Dict[str, Any], identifiers: Set[str]) -> None:
+    """Prune non-existing objects and empty libs from a lib's
+    public.objectLibs.
+
+    Empty object libs are pruned, but object identifiers stay.
+    """
+
+    if OBJECT_LIBS_KEY not in parent_lib:
+        return
+
+    object_libs = parent_lib[OBJECT_LIBS_KEY]
+    parent_lib[OBJECT_LIBS_KEY] = {
+        k: v for k, v in object_libs.items() if k in identifiers and v
+    }
+
+
 class Placeholder:
     """Represents a sentinel value to signal a "lazy" object hasn't been loaded yet."""
 
 
 _NOT_LOADED = Placeholder()
```

## Comparing `ufoLib2-0.8.0/src/ufoLib2.egg-info/SOURCES.txt` & `ufoLib2-0.9.0/src/ufoLib2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,8 +71,9 @@
 tests/data/UbuTestData.ufo/glyphs.public.background/a.glif
 tests/data/UbuTestData.ufo/glyphs.public.background/contents.plist
 tests/objects/test_component.py
 tests/objects/test_contour.py
 tests/objects/test_datastore.py
 tests/objects/test_font.py
 tests/objects/test_glyph.py
-tests/objects/test_layer.py
+tests/objects/test_layer.py
+tests/objects/test_object_lib.py
```

## Comparing `ufoLib2-0.8.0/src/ufoLib2.egg-info/PKG-INFO` & `ufoLib2-0.9.0/src/ufoLib2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ufoLib2
-Version: 0.8.0
+Version: 0.9.0
 Summary: ufoLib2 is a UFO font processing library.
 Home-page: https://github.com/fonttools/ufoLib2
 Author: Adrien Tétar
 Author-email: adri-from-59@hotmail.fr
 License: Apache 2.0
 Description: # ufoLib2
```

## Comparing `ufoLib2-0.8.0/.github/workflows/test.yml` & `ufoLib2-0.9.0/.github/workflows/test.yml`

 * *Files 18% similar despite different names*

```diff
@@ -11,51 +11,53 @@
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python
       uses: actions/setup-python@v1
       with:
-        python-version: '3.8'
+        python-version: '3.x'
     - name: Lint
       run: |
         pip install tox
         tox -e lint
 
   docs:  # To see if they build.
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python
       uses: actions/setup-python@v1
       with:
-        python-version: '3.8'
+        python-version: '3.x'
     - name: Lint
       run: |
         pip install tox
         tox -e docs
 
   build:
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8]
+        python-version: [3.6, 3.9]
         platform: [ubuntu-latest, windows-latest]
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
-    - name: Test with tox
+    - name: Install packages
+      run: pip install tox coverage
+    - name: Run Tox
+      run: tox -e py-cov
+    - name: Produce coverage files
       run: |
-        pip install tox -r requirements-dev.txt
-        tox -e py-cov
         coverage combine
         coverage xml
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v1
       with:
         file: coverage.xml
         flags: unittests
```

## Comparing `ufoLib2-0.8.0/.github/workflows/publish.yml` & `ufoLib2-0.9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/docs/source/index.rst` & `ufoLib2-0.9.0/docs/source/index.rst`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/docs/source/explanations.rst` & `ufoLib2-0.9.0/docs/source/explanations.rst`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/docs/source/reference.rst` & `ufoLib2-0.9.0/docs/source/reference.rst`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/docs/source/conf.py` & `ufoLib2-0.9.0/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 master_doc = "index"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinx_rtd_theme",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
```

## Comparing `ufoLib2-0.8.0/tests/test_ufoLib2.py` & `ufoLib2-0.9.0/tests/test_ufoLib2.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/data/LICENSE_UbuTestData.txt` & `ufoLib2-0.9.0/tests/data/LICENSE_UbuTestData.txt`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/data/UbuTestData.ufo/fontinfo.plist` & `ufoLib2-0.9.0/tests/data/UbuTestData.ufo/fontinfo.plist`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.daltonmaag.vttLib.plist` & `ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.daltonmaag.vttLib.plist`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__3.ttx` & `ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__3.ttx`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__1.ttx` & `ufoLib2-0.9.0/tests/data/UbuTestData.ufo/data/com.github.fonttools.ttx/T_S_I__1.ttx`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs.public.background/A_.glif` & `ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs.public.background/A_.glif`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs.public.background/a.glif` & `ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs.public.background/a.glif`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs/A_.glif` & `ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs/A_.glif`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/data/UbuTestData.ufo/glyphs/a.glif` & `ufoLib2-0.9.0/tests/data/UbuTestData.ufo/glyphs/a.glif`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/objects/test_layer.py` & `ufoLib2-0.9.0/tests/objects/test_layer.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/objects/test_glyph.py` & `ufoLib2-0.9.0/tests/objects/test_glyph.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/objects/test_component.py` & `ufoLib2-0.9.0/tests/objects/test_component.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/objects/test_font.py` & `ufoLib2-0.9.0/tests/objects/test_font.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/objects/test_datastore.py` & `ufoLib2-0.9.0/tests/objects/test_datastore.py`

 * *Files identical despite different names*

## Comparing `ufoLib2-0.8.0/tests/objects/test_contour.py` & `ufoLib2-0.9.0/tests/objects/test_contour.py`

 * *Files identical despite different names*

