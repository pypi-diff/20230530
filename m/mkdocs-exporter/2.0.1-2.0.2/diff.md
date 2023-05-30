# Comparing `tmp/mkdocs_exporter-2.0.1.tar.gz` & `tmp/mkdocs_exporter-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-2.0.1.tar", max compression
+gzip compressed data, was "mkdocs_exporter-2.0.2.tar", max compression
```

## Comparing `mkdocs_exporter-2.0.1.tar` & `mkdocs_exporter-2.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-2.0.1/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-27 16:58:40.207217 mkdocs_exporter-2.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-2.0.1/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1973 2023-05-27 18:11:03.211214 mkdocs_exporter-2.0.1/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-2.0.1/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      543 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/page.py
--rw-r--r--   0        0        0     1805 2023-05-27 18:11:03.211214 mkdocs_exporter-2.0.1/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      796 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0     1075 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      526 2023-05-27 12:57:36.091210 mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0     1040 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4612 2023-05-27 18:11:03.211214 mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2215 2023-05-27 18:11:03.211214 mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     4115 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-2.0.1/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-2.0.1/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/resources/css/__init__.py
--rw-r--r--   0        0        0       93 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/resources/css/readthedocs.css
--rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-2.0.1/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   504034 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0      599 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/theme.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/themes/__init__.py
--rw-r--r--   0        0        0      650 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/themes/factory.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/themes/material/__init__.py
--rw-r--r--   0        0        0      681 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/themes/material/icons.py
--rw-r--r--   0        0        0     1317 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/themes/material/theme.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/themes/readthedocs/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-27 16:58:36.537218 mkdocs_exporter-2.0.1/mkdocs_exporter/themes/readthedocs/theme.py
--rw-r--r--   0        0        0     1593 2023-05-27 18:11:27.041207 mkdocs_exporter-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     4661 1970-01-01 00:00:00.000000 mkdocs_exporter-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-09 09:23:22.592488 mkdocs_exporter-2.0.2/LICENSE
+-rw-r--r--   0        0        0     4007 2023-05-30 06:07:05.064243 mkdocs_exporter-2.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.0.2/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0     1973 2023-05-30 06:07:05.064243 mkdocs_exporter-2.0.2/mkdocs_exporter/browser.py
+-rw-r--r--   0        0        0       96 2023-05-09 09:23:22.592488 mkdocs_exporter-2.0.2/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      543 2023-05-30 06:07:05.064243 mkdocs_exporter-2.0.2/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0     1864 2023-05-30 06:13:17.034229 mkdocs_exporter-2.0.2/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      867 2023-05-30 06:10:52.764231 mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0     1121 2023-05-30 06:11:08.624231 mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0      526 2023-05-22 10:55:25.061256 mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0     1040 2023-05-30 06:07:05.064243 mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4636 2023-05-30 06:09:40.294234 mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2215 2023-05-30 06:07:05.064243 mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     4115 2023-05-30 06:30:33.584215 mkdocs_exporter-2.0.2/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-09 09:23:22.592488 mkdocs_exporter-2.0.2/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.0.2/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:07:05.064243 mkdocs_exporter-2.0.2/mkdocs_exporter/resources/css/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-30 06:07:05.064243 mkdocs_exporter-2.0.2/mkdocs_exporter/resources/css/readthedocs.css
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.0.2/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   504034 2023-05-30 06:07:05.074243 mkdocs_exporter-2.0.2/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0      599 2023-05-30 06:07:05.074243 mkdocs_exporter-2.0.2/mkdocs_exporter/theme.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-2.0.2/mkdocs_exporter/themes/__init__.py
+-rw-r--r--   0        0        0      650 2023-05-30 06:07:05.074243 mkdocs_exporter-2.0.2/mkdocs_exporter/themes/factory.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-2.0.2/mkdocs_exporter/themes/material/__init__.py
+-rw-r--r--   0        0        0      681 2023-05-30 06:07:05.074243 mkdocs_exporter-2.0.2/mkdocs_exporter/themes/material/icons.py
+-rw-r--r--   0        0        0     1317 2023-05-30 06:07:05.074243 mkdocs_exporter-2.0.2/mkdocs_exporter/themes/material/theme.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-2.0.2/mkdocs_exporter/themes/readthedocs/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-30 06:07:05.074243 mkdocs_exporter-2.0.2/mkdocs_exporter/themes/readthedocs/theme.py
+-rw-r--r--   0        0        0     1593 2023-05-30 06:31:39.744224 mkdocs_exporter-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5367 1970-01-01 00:00:00.000000 mkdocs_exporter-2.0.2/PKG-INFO
```

### Comparing `mkdocs_exporter-2.0.1/LICENSE` & `mkdocs_exporter-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/README.md` & `mkdocs_exporter-2.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,210 +1,251 @@
 00000000: 2320 4d6b 446f 6373 2045 7870 6f72 7465  # MkDocs Exporte
-00000010: 720a 0a41 2068 6967 686c 792d 636f 6e66  r..A highly-conf
-00000020: 6967 7572 6162 6c65 2070 6c75 6769 6e20  igurable plugin 
-00000030: 666f 7220 5b2a 4d6b 446f 6373 2a5d 2868  for [*MkDocs*](h
-00000040: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000050: 6d2f 6d6b 646f 6373 2f6d 6b64 6f63 7329  m/mkdocs/mkdocs)
-00000060: 2074 6861 7420 6578 706f 7274 7320 796f   that exports yo
-00000070: 7572 2070 6167 6573 2074 6f20 5044 4620  ur pages to PDF 
-00000080: 6669 6c65 732e 0a0a 2d20 5b44 6f63 756d  files...- [Docum
-00000090: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-000000a0: 2f2f 6164 7269 656e 6272 6967 6e6f 6e2e  //adrienbrignon.
-000000b0: 6769 7468 7562 2e69 6f2f 6d6b 646f 6373  github.io/mkdocs
-000000c0: 2d65 7870 6f72 7465 7229 0a2d 205b 5079  -exporter).- [Py
-000000d0: 5049 5d28 6874 7470 733a 2f2f 7079 7069  PI](https://pypi
-000000e0: 2e6f 7267 2f70 726f 6a65 6374 2f6d 6b64  .org/project/mkd
-000000f0: 6f63 732d 6578 706f 7274 6572 290a 0a23  ocs-exporter)..#
-00000100: 2320 4665 6174 7572 6573 0a0a 2d20 f09f  # Features..- ..
-00000110: 9a80 202a 2a46 6173 742a 2a20 2d20 5044  .. **Fast** - PD
-00000120: 4620 646f 6375 6d65 6e74 7320 6172 6520  F documents are 
-00000130: 6765 6e65 7261 7465 6420 636f 6e63 7572  generated concur
-00000140: 7265 6e74 6c79 210a 2d20 f09f 8ea8 202a  rently!.- .... *
-00000150: 2a43 7573 746f 6d69 7a61 626c 652a 2a20  *Customizable** 
-00000160: 2d20 6675 6c6c 2063 6f6e 7472 6f6c 206f  - full control o
-00000170: 7665 7220 7468 6520 7265 7375 6c74 696e  ver the resultin
-00000180: 6720 646f 6375 6d65 6e74 730a 2020 2d20  g documents.  - 
-00000190: 436f 7665 7220 7061 6765 7320 2873 7570  Cover pages (sup
-000001a0: 706f 7274 7320 5b60 6d61 6372 6f73 605d  ports [`macros`]
-000001b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000001c0: 636f 6d2f 6672 616c 6175 2f6d 6b64 6f63  com/fralau/mkdoc
-000001d0: 735f 6d61 6372 6f73 5f70 6c75 6769 6e29  s_macros_plugin)
-000001e0: 2070 6c75 6769 6e29 0a20 202d 2044 6566   plugin).  - Def
-000001f0: 696e 6520 6375 7374 6f6d 2073 6372 6970  ine custom scrip
-00000200: 7473 2061 6e64 2073 7479 6c65 7368 6565  ts and styleshee
-00000210: 7473 2074 6f20 6375 7374 6f6d 697a 6520  ts to customize 
-00000220: 796f 7572 2050 4446 2064 6f63 756d 656e  your PDF documen
-00000230: 7473 0a20 202d 2044 6566 696e 6520 2262  ts.  - Define "b
-00000240: 7574 746f 6e73 2220 6174 2074 6865 2074  uttons" at the t
-00000250: 6f70 206f 6620 796f 7572 2064 6f63 756d  op of your docum
-00000260: 656e 7461 7469 6f6e 2070 6167 6573 2028  entation pages (
-00000270: 5b65 7861 6d70 6c65 5d28 6874 7470 733a  [example](https:
-00000280: 2f2f 6164 7269 656e 6272 6967 6e6f 6e2e  //adrienbrignon.
-00000290: 6769 7468 7562 2e69 6f2f 6d6b 646f 6373  github.io/mkdocs
-000002a0: 2d65 7870 6f72 7465 722f 7365 7475 702f  -exporter/setup/
-000002b0: 7365 7474 696e 672d 7570 2d62 7574 746f  setting-up-butto
-000002c0: 6e73 2f29 290a 2020 2d20 436f 6d70 6174  ns/)).  - Compat
-000002d0: 6962 6c65 2077 6974 6820 5b60 6d61 7465  ible with [`mate
-000002e0: 7269 616c 605d 2868 7474 7073 3a2f 2f67  rial`](https://g
-000002f0: 6974 6875 622e 636f 6d2f 7371 7569 6466  ithub.com/squidf
-00000300: 756e 6b2f 6d6b 646f 6373 2d6d 6174 6572  unk/mkdocs-mater
-00000310: 6961 6c29 2061 6e64 205b 6072 6561 6474  ial) and [`readt
-00000320: 6865 646f 6373 605d 2868 7474 7073 3a2f  hedocs`](https:/
-00000330: 2f77 7777 2e6d 6b64 6f63 732e 6f72 672f  /www.mkdocs.org/
-00000340: 7573 6572 2d67 7569 6465 2f63 686f 6f73  user-guide/choos
-00000350: 696e 672d 796f 7572 2d74 6865 6d65 2f23  ing-your-theme/#
-00000360: 7265 6164 7468 6564 6f63 7329 2074 6865  readthedocs) the
-00000370: 6d65 730a 2d20 e2ad 9020 2a2a 506f 7765  mes.- ... **Powe
-00000380: 7266 756c 2a2a 202d 2069 7420 7573 6573  rful** - it uses
-00000390: 2061 2068 6561 646c 6573 7320 6272 6f77   a headless brow
-000003a0: 7365 7220 616e 6420 736f 6d65 2061 7765  ser and some awe
-000003b0: 736f 6d65 206c 6962 7261 7269 6573 2075  some libraries u
-000003c0: 6e64 6572 2074 6865 2068 6f6f 6420 746f  nder the hood to
-000003d0: 2067 656e 6572 6174 6520 5044 4620 6669   generate PDF fi
-000003e0: 6c65 730a 2020 2d20 5b2a 506c 6179 7772  les.  - [*Playwr
-000003f0: 6967 6874 2a5d 2868 7474 7073 3a2f 2f67  ight*](https://g
-00000400: 6974 6875 622e 636f 6d2f 6d69 6372 6f73  ithub.com/micros
-00000410: 6f66 742f 706c 6179 7772 6967 6874 2d70  oft/playwright-p
-00000420: 7974 686f 6e29 2074 6f20 6175 746f 6d61  ython) to automa
-00000430: 7465 2062 726f 7773 6572 730a 2020 2d20  te browsers.  - 
-00000440: 5b2a 5061 6765 642e 6a73 2a5d 2868 7474  [*Paged.js*](htt
-00000450: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000460: 7061 6765 646a 732f 7061 6765 646a 7329  pagedjs/pagedjs)
-00000470: 2070 6f6c 7966 696c 6c73 2061 7265 2069   polyfills are i
-00000480: 6e63 6c75 6465 6420 285b 5061 6765 6420  ncluded ([Paged 
-00000490: 4d65 6469 615d 2868 7474 7073 3a2f 2f77  Media](https://w
-000004a0: 7777 2e77 332e 6f72 672f 5452 2f63 7373  ww.w3.org/TR/css
-000004b0: 2d70 6167 652d 332f 2920 616e 6420 5b47  -page-3/) and [G
-000004c0: 656e 6572 6174 6564 2043 6f6e 7465 6e74  enerated Content
-000004d0: 5d28 6874 7470 733a 2f2f 7777 772e 7733  ](https://www.w3
-000004e0: 2e6f 7267 2f54 522f 6373 732d 6763 706d  .org/TR/css-gcpm
-000004f0: 2d33 2f29 2043 5353 206d 6f64 756c 6573  -3/) CSS modules
-00000500: 290a 2020 2d20 5b2a 5361 7373 2a5d 2868  ).  - [*Sass*](h
-00000510: 7474 7073 3a2f 2f73 6173 732d 6c61 6e67  ttps://sass-lang
-00000520: 2e63 6f6d 2f29 2073 7570 706f 7274 2028  .com/) support (
-00000530: 7669 6120 5b60 6c69 6273 6173 7360 5d28  via [`libsass`](
-00000540: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000550: 6f6d 2f73 6173 732f 6c69 6273 6173 732d  om/sass/libsass-
-00000560: 7079 7468 6f6e 2929 2066 6f72 2079 6f75  python)) for you
-00000570: 7220 7374 796c 6573 6865 6574 730a 0a23  r stylesheets..#
-00000580: 2320 5072 6572 6571 7569 7369 7465 730a  # Prerequisites.
-00000590: 0a2d 2050 7974 686f 6e20 603e 3d20 332e  .- Python `>= 3.
-000005a0: 3760 0a2d 204d 6b44 6f63 7320 603e 3d20  7`.- MkDocs `>= 
-000005b0: 312e 3460 0a0a 2323 2049 6e73 7461 6c6c  1.4`..## Install
-000005c0: 6174 696f 6e0a 0a54 6865 2070 6c75 6769  ation..The plugi
-000005d0: 6e20 6973 2068 6f73 7465 6420 6f6e 205b  n is hosted on [
-000005e0: 2a50 7950 492a 5d28 6874 7470 733a 2f2f  *PyPI*](https://
-000005f0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000600: 2f6d 6b64 6f63 732d 6578 706f 7274 6572  /mkdocs-exporter
-00000610: 2f29 2061 6e64 2063 616e 2062 6520 696e  /) and can be in
-00000620: 7374 616c 6c65 6420 7669 6120 6070 6970  stalled via `pip
-00000630: 6020 286f 7220 796f 7572 2066 6176 6f75  ` (or your favou
-00000640: 7269 7465 2070 6163 6b61 6765 206d 616e  rite package man
-00000650: 6167 6572 293a 0a0a 6060 6062 6173 680a  ager):..```bash.
-00000660: 7069 7020 696e 7374 616c 6c20 6d6b 646f  pip install mkdo
-00000670: 6373 2d65 7870 6f72 7465 720a 6060 600a  cs-exporter.```.
-00000680: 0a23 2320 5573 6167 650a 0a54 6872 6565  .## Usage..Three
-00000690: 2070 6c75 6769 6e73 2061 7265 2063 7572   plugins are cur
-000006a0: 7265 6e74 6c79 2061 7661 696c 6162 6c65  rently available
-000006b0: 3a0a 0a2d 2060 6d6b 646f 6373 2f65 7870  :..- `mkdocs/exp
-000006c0: 6f72 7465 7260 2028 2a72 6571 7569 7265  orter` (*require
-000006d0: 642a 293a 2062 6173 6520 706c 7567 696e  d*): base plugin
-000006e0: 2077 6869 6368 206d 7573 7420 7072 6563   which must prec
-000006f0: 6564 6520 7468 6520 6f74 6865 7273 0a2d  ede the others.-
-00000700: 2060 6d6b 646f 6373 2f65 7870 6f72 7465   `mkdocs/exporte
-00000710: 722f 7064 6660 2028 2a6f 7074 696f 6e61  r/pdf` (*optiona
-00000720: 6c2a 293a 2070 6c75 6769 6e20 7468 6174  l*): plugin that
-00000730: 2065 7870 6f72 7473 2079 6f75 7220 7061   exports your pa
-00000740: 6765 7320 6173 2069 6e64 6976 6964 7561  ges as individua
-00000750: 6c20 5044 4620 646f 6375 6d65 6e74 730a  l PDF documents.
-00000760: 2d20 606d 6b64 6f63 732f 6578 706f 7274  - `mkdocs/export
-00000770: 6572 2f65 7874 7261 7360 2028 2a6f 7074  er/extras` (*opt
-00000780: 696f 6e61 6c2a 293a 2070 726f 7669 6465  ional*): provide
-00000790: 7320 6578 7472 6120 6675 6e63 7469 6f6e  s extra function
-000007a0: 616c 6974 6965 7320 2862 7574 746f 6e73  alities (buttons
-000007b0: 2c20 4854 4d4c 2075 7469 6c69 7469 6573  , HTML utilities
-000007c0: 2e2e 2e29 0a0a 2323 2320 4578 616d 706c  ...)..### Exampl
-000007d0: 650a 0a54 6865 2066 6f6c 6c6f 7769 6e67  e..The following
-000007e0: 2063 6f6e 6669 6775 7261 7469 6f6e 2065   configuration e
-000007f0: 7863 6572 7074 2066 726f 6d20 606d 6b64  xcerpt from `mkd
-00000800: 6f63 732e 796d 6c60 2073 686f 756c 6420  ocs.yml` should 
-00000810: 636f 7665 7220 7468 6520 6261 7369 6320  cover the basic 
-00000820: 6675 6e63 7469 6f6e 616c 6974 6965 7320  functionalities 
-00000830: 6f66 2074 6869 7320 706c 7567 696e 3a0a  of this plugin:.
-00000840: 0a60 6060 7961 6d6c 0a70 6c75 6769 6e73  .```yaml.plugins
-00000850: 3a0a 2020 2d20 6d6b 646f 6373 2f65 7870  :.  - mkdocs/exp
-00000860: 6f72 7465 720a 2020 2d20 6d6b 646f 6373  orter.  - mkdocs
-00000870: 2f65 7870 6f72 7465 722f 7064 663a 0a20  /exporter/pdf:. 
-00000880: 2020 2020 2063 6f6e 6375 7272 656e 6379       concurrency
-00000890: 3a20 380a 2020 2020 2020 636f 7665 7273  : 8.      covers
-000008a0: 3a0a 2020 2020 2020 2020 6672 6f6e 743a  :.        front:
-000008b0: 2072 6573 6f75 7263 6573 2f74 656d 706c   resources/templ
-000008c0: 6174 6573 2f63 6f76 6572 732f 6672 6f6e  ates/covers/fron
-000008d0: 742e 6874 6d6c 2e6a 320a 2020 2020 2020  t.html.j2.      
-000008e0: 2020 6261 636b 3a20 7265 736f 7572 6365    back: resource
-000008f0: 732f 7465 6d70 6c61 7465 732f 636f 7665  s/templates/cove
-00000900: 7273 2f62 6163 6b2e 6874 6d6c 2e6a 320a  rs/back.html.j2.
-00000910: 2020 2020 2020 7374 796c 6573 6865 6574        stylesheet
-00000920: 733a 0a20 2020 2020 2020 202d 2072 6573  s:.        - res
-00000930: 6f75 7263 6573 2f73 7479 6c65 7368 6565  ources/styleshee
-00000940: 7473 2f70 6466 2e73 6373 730a 2020 2d20  ts/pdf.scss.  - 
-00000950: 6d6b 646f 6373 2f65 7870 6f72 7465 722f  mkdocs/exporter/
-00000960: 6578 7472 6173 3a0a 2020 2020 2020 6275  extras:.      bu
-00000970: 7474 6f6e 733a 0a20 2020 2020 2020 202d  ttons:.        -
-00000980: 2074 6974 6c65 3a20 446f 776e 6c6f 6164   title: Download
-00000990: 2061 7320 5044 460a 2020 2020 2020 2020   as PDF.        
-000009a0: 2020 656e 6162 6c65 643a 2021 2170 7974    enabled: !!pyt
-000009b0: 686f 6e2f 6e61 6d65 3a6d 6b64 6f63 735f  hon/name:mkdocs_
-000009c0: 6578 706f 7274 6572 2e70 6c75 6769 6e73  exporter.plugins
-000009d0: 2e70 6466 2e62 7574 746f 6e2e 656e 6162  .pdf.button.enab
-000009e0: 6c65 640a 2020 2020 2020 2020 2020 6963  led.          ic
-000009f0: 6f6e 3a20 2121 7079 7468 6f6e 2f6e 616d  on: !!python/nam
-00000a00: 653a 6d6b 646f 6373 5f65 7870 6f72 7465  e:mkdocs_exporte
-00000a10: 722e 706c 7567 696e 732e 7064 662e 6275  r.plugins.pdf.bu
-00000a20: 7474 6f6e 2e69 636f 6e0a 2020 2020 2020  tton.icon.      
-00000a30: 2020 2020 6174 7472 6962 7574 6573 3a0a      attributes:.
-00000a40: 2020 2020 2020 2020 2020 2020 6872 6566              href
-00000a50: 3a20 2121 7079 7468 6f6e 2f6e 616d 653a  : !!python/name:
-00000a60: 6d6b 646f 6373 5f65 7870 6f72 7465 722e  mkdocs_exporter.
-00000a70: 706c 7567 696e 732e 7064 662e 6275 7474  plugins.pdf.butt
-00000a80: 6f6e 2e68 7265 660a 2020 2020 2020 2020  on.href.        
-00000a90: 2020 2020 646f 776e 6c6f 6164 3a20 2121      download: !!
-00000aa0: 7079 7468 6f6e 2f6e 616d 653a 6d6b 646f  python/name:mkdo
-00000ab0: 6373 5f65 7870 6f72 7465 722e 706c 7567  cs_exporter.plug
-00000ac0: 696e 732e 7064 662e 6275 7474 6f6e 2e64  ins.pdf.button.d
-00000ad0: 6f77 6e6c 6f61 640a 6060 600a 0a43 6865  ownload.```..Che
-00000ae0: 636b 206f 7574 2061 205b 7361 6d70 6c65  ck out a [sample
-00000af0: 2050 4446 2067 656e 6572 6174 6564 2062   PDF generated b
-00000b00: 7920 7468 6973 2070 6c75 6769 6e5d 2865  y this plugin](e
-00000b10: 7861 6d70 6c65 732f 6578 616d 706c 652e  xamples/example.
-00000b20: 7064 6629 2066 726f 6d20 7468 6520 6465  pdf) from the de
-00000b30: 6661 756c 7420 7061 6765 206f 6620 7468  fault page of th
-00000b40: 6520 5b4d 6174 6572 6961 6c20 666f 7220  e [Material for 
-00000b50: 4d6b 446f 6373 5d28 6874 7470 733a 2f2f  MkDocs](https://
-00000b60: 7371 7569 6466 756e 6b2e 6769 7468 7562  squidfunk.github
-00000b70: 2e69 6f2f 6d6b 646f 6373 2d6d 6174 6572  .io/mkdocs-mater
-00000b80: 6961 6c29 2074 6865 6d65 2e20 200a 4974  ial) theme.  .It
-00000b90: 2068 6173 2062 6565 6e20 6275 696c 7420   has been built 
-00000ba0: 7769 7468 2073 6f6d 6520 6375 7374 6f6d  with some custom
-00000bb0: 2043 5353 2061 6e64 2066 6561 7475 7265   CSS and feature
-00000bc0: 7320 636f 7665 7220 7061 6765 732e 0a0a  s cover pages...
-00000bd0: 2323 2052 6f61 646d 6170 0a0a 2d20 456e  ## Roadmap..- En
-00000be0: 7375 7265 2066 756c 6c20 636f 6d70 6174  sure full compat
-00000bf0: 6962 696c 6974 7920 7769 7468 206f 7468  ibility with oth
-00000c00: 6572 2074 6865 6d65 7320 7468 616e 2060  er themes than `
-00000c10: 6d6b 646f 6373 2d6d 6174 6572 6961 6c60  mkdocs-material`
-00000c20: 0a2d 2043 6f6d 6269 6e65 2061 6c6c 2070  .- Combine all p
-00000c30: 6167 6573 2061 7320 6f6e 6520 5044 460a  ages as one PDF.
-00000c40: 0a46 6565 6c20 6672 6565 2074 6f20 7265  .Feel free to re
-00000c50: 7175 6573 7420 6164 6469 7469 6f6e 616c  quest additional
-00000c60: 2066 6561 7475 7265 7320 6279 2073 7562   features by sub
-00000c70: 6d69 7474 696e 6720 616e 2069 7373 7565  mitting an issue
-00000c80: 206f 7220 6279 2063 6f6e 7472 6962 7574   or by contribut
-00000c90: 696e 6720 7468 726f 7567 6820 6120 7075  ing through a pu
-00000ca0: 6c6c 2072 6571 7565 7374 2e0a 0a23 2320  ll request...## 
-00000cb0: 4c69 6365 6e73 650a 0a54 6869 7320 7072  License..This pr
-00000cc0: 6f6a 6563 7420 6973 206c 6963 656e 7365  oject is license
-00000cd0: 6420 756e 6465 7220 7468 6520 604d 4954  d under the `MIT
-00000ce0: 204c 6963 656e 7365 2028 4d49 5429 602c   License (MIT)`,
-00000cf0: 2077 6869 6368 2079 6f75 2063 616e 2072   which you can r
-00000d00: 6561 6420 5b68 6572 655d 284c 4943 454e  ead [here](LICEN
-00000d10: 5345 292e 0a                             SE)..
+00000010: 720a 0a3c 6469 763e 0a20 203c 6120 6872  r..<div>.  <a hr
+00000020: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+00000030: 2e6f 7267 2f70 726f 6a65 6374 2f6d 6b64  .org/project/mkd
+00000040: 6f63 732d 6578 706f 7274 6572 223e 0a20  ocs-exporter">. 
+00000050: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00000060: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000070: 2e69 6f2f 7079 7069 2f76 2f6d 6b64 6f63  .io/pypi/v/mkdoc
+00000080: 732d 6578 706f 7274 6572 3f63 6f6c 6f72  s-exporter?color
+00000090: 3d62 6c75 6522 3e0a 2020 3c2f 613e 0a20  =blue">.  </a>. 
+000000a0: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000000b0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+000000c0: 6374 2f6d 6b64 6f63 732d 6578 706f 7274  ct/mkdocs-export
+000000d0: 6572 223e 0a20 2020 203c 696d 6720 7372  er">.    <img sr
+000000e0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000000f0: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
+00000100: 7976 6572 7369 6f6e 732f 6d6b 646f 6373  yversions/mkdocs
+00000110: 2d65 7870 6f72 7465 723f 636f 6c6f 723d  -exporter?color=
+00000120: 626c 7565 223e 0a20 203c 2f61 3e0a 2020  blue">.  </a>.  
+00000130: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000140: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000150: 742f 6d6b 646f 6373 2d65 7870 6f72 7465  t/mkdocs-exporte
+00000160: 7222 3e0a 2020 2020 3c69 6d67 2073 7263  r">.    <img src
+00000170: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000180: 6965 6c64 732e 696f 2f70 7970 692f 646d  ields.io/pypi/dm
+00000190: 2f6d 6b64 6f63 732d 6578 706f 7274 6572  /mkdocs-exporter
+000001a0: 3f63 6f6c 6f72 3d63 6163 7475 7322 3e0a  ?color=cactus">.
+000001b0: 2020 3c2f 613e 0a20 203c 6120 6872 6566    </a>.  <a href
+000001c0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
+000001d0: 2e63 6f6d 2f61 6472 6965 6e62 7269 676e  .com/adrienbrign
+000001e0: 6f6e 2f6d 6b64 6f63 732d 6578 706f 7274  on/mkdocs-export
+000001f0: 6572 2f62 6c6f 622f 6d61 7374 6572 2f4c  er/blob/master/L
+00000200: 4943 454e 5345 223e 0a20 2020 203c 696d  ICENSE">.    <im
+00000210: 6720 616c 6967 6e3d 2272 6967 6874 2220  g align="right" 
+00000220: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000230: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000240: 7562 2f6c 6963 656e 7365 2f61 6472 6965  ub/license/adrie
+00000250: 6e62 7269 676e 6f6e 2f6d 6b64 6f63 732d  nbrignon/mkdocs-
+00000260: 6578 706f 7274 6572 3f63 6f6c 6f72 3d77  exporter?color=w
+00000270: 6869 7465 223e 0a20 203c 2f61 3e0a 3c2f  hite">.  </a>.</
+00000280: 6469 763e 0a3c 6272 202f 3e0a 0a41 2068  div>.<br />..A h
+00000290: 6967 686c 792d 636f 6e66 6967 7572 6162  ighly-configurab
+000002a0: 6c65 2070 6c75 6769 6e20 666f 7220 5b2a  le plugin for [*
+000002b0: 4d6b 446f 6373 2a5d 2868 7474 7073 3a2f  MkDocs*](https:/
+000002c0: 2f67 6974 6875 622e 636f 6d2f 6d6b 646f  /github.com/mkdo
+000002d0: 6373 2f6d 6b64 6f63 7329 2074 6861 7420  cs/mkdocs) that 
+000002e0: 6578 706f 7274 7320 796f 7572 2070 6167  exports your pag
+000002f0: 6573 2074 6f20 5044 4620 6669 6c65 732e  es to PDF files.
+00000300: 0a0a 2d20 5b44 6f63 756d 656e 7461 7469  ..- [Documentati
+00000310: 6f6e 5d28 6874 7470 733a 2f2f 6164 7269  on](https://adri
+00000320: 656e 6272 6967 6e6f 6e2e 6769 7468 7562  enbrignon.github
+00000330: 2e69 6f2f 6d6b 646f 6373 2d65 7870 6f72  .io/mkdocs-expor
+00000340: 7465 7229 0a2d 205b 5079 5049 5d28 6874  ter).- [PyPI](ht
+00000350: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000360: 726f 6a65 6374 2f6d 6b64 6f63 732d 6578  roject/mkdocs-ex
+00000370: 706f 7274 6572 290a 2d20 5b45 7861 6d70  porter).- [Examp
+00000380: 6c65 735d 282e 2f65 7861 6d70 6c65 7329  les](./examples)
+00000390: 0a0a 2323 2046 6561 7475 7265 730a 0a2d  ..## Features..-
+000003a0: 20f0 9f9a 8020 2a2a 4661 7374 2a2a 202d   .... **Fast** -
+000003b0: 2050 4446 2064 6f63 756d 656e 7473 2061   PDF documents a
+000003c0: 7265 2067 656e 6572 6174 6564 2063 6f6e  re generated con
+000003d0: 6375 7272 656e 746c 7921 0a2d 20f0 9f8e  currently!.- ...
+000003e0: a820 2a2a 4375 7374 6f6d 697a 6162 6c65  . **Customizable
+000003f0: 2a2a 202d 2066 756c 6c20 636f 6e74 726f  ** - full contro
+00000400: 6c20 6f76 6572 2074 6865 2072 6573 756c  l over the resul
+00000410: 7469 6e67 2064 6f63 756d 656e 7473 0a20  ting documents. 
+00000420: 202d 2043 6f76 6572 2070 6167 6573 2028   - Cover pages (
+00000430: 7375 7070 6f72 7473 205b 606d 6163 726f  supports [`macro
+00000440: 7360 5d28 6874 7470 733a 2f2f 6769 7468  s`](https://gith
+00000450: 7562 2e63 6f6d 2f66 7261 6c61 752f 6d6b  ub.com/fralau/mk
+00000460: 646f 6373 5f6d 6163 726f 735f 706c 7567  docs_macros_plug
+00000470: 696e 2920 706c 7567 696e 290a 2020 2d20  in) plugin).  - 
+00000480: 4465 6669 6e65 2063 7573 746f 6d20 7363  Define custom sc
+00000490: 7269 7074 7320 616e 6420 7374 796c 6573  ripts and styles
+000004a0: 6865 6574 7320 746f 2063 7573 746f 6d69  heets to customi
+000004b0: 7a65 2079 6f75 7220 5044 4620 646f 6375  ze your PDF docu
+000004c0: 6d65 6e74 730a 2020 2d20 4465 6669 6e65  ments.  - Define
+000004d0: 2022 6275 7474 6f6e 7322 2061 7420 7468   "buttons" at th
+000004e0: 6520 746f 7020 6f66 2079 6f75 7220 646f  e top of your do
+000004f0: 6375 6d65 6e74 6174 696f 6e20 7061 6765  cumentation page
+00000500: 7320 285b 6578 616d 706c 655d 2868 7474  s ([example](htt
+00000510: 7073 3a2f 2f61 6472 6965 6e62 7269 676e  ps://adrienbrign
+00000520: 6f6e 2e67 6974 6875 622e 696f 2f6d 6b64  on.github.io/mkd
+00000530: 6f63 732d 6578 706f 7274 6572 2f73 6574  ocs-exporter/set
+00000540: 7570 2f73 6574 7469 6e67 2d75 702d 6275  up/setting-up-bu
+00000550: 7474 6f6e 732f 2929 0a20 202d 2043 6f6d  ttons/)).  - Com
+00000560: 7061 7469 626c 6520 7769 7468 205b 606d  patible with [`m
+00000570: 6174 6572 6961 6c60 5d28 6874 7470 733a  aterial`](https:
+00000580: 2f2f 6769 7468 7562 2e63 6f6d 2f73 7175  //github.com/squ
+00000590: 6964 6675 6e6b 2f6d 6b64 6f63 732d 6d61  idfunk/mkdocs-ma
+000005a0: 7465 7269 616c 2920 616e 6420 5b60 7265  terial) and [`re
+000005b0: 6164 7468 6564 6f63 7360 5d28 6874 7470  adthedocs`](http
+000005c0: 733a 2f2f 7777 772e 6d6b 646f 6373 2e6f  s://www.mkdocs.o
+000005d0: 7267 2f75 7365 722d 6775 6964 652f 6368  rg/user-guide/ch
+000005e0: 6f6f 7369 6e67 2d79 6f75 722d 7468 656d  oosing-your-them
+000005f0: 652f 2372 6561 6474 6865 646f 6373 2920  e/#readthedocs) 
+00000600: 7468 656d 6573 0a20 2020 202d 2043 6865  themes.    - Che
+00000610: 636b 206f 7574 2073 6f6d 6520 7361 6d70  ck out some samp
+00000620: 6c65 2050 4446 2064 6f63 756d 656e 7473  le PDF documents
+00000630: 205b 6865 7265 5d28 2e2f 6578 616d 706c   [here](./exampl
+00000640: 6573 2f74 6865 6d65 7329 0a2d 20e2 ad90  es/themes).- ...
+00000650: 202a 2a50 6f77 6572 6675 6c2a 2a20 2d20   **Powerful** - 
+00000660: 6974 2075 7365 7320 6120 6865 6164 6c65  it uses a headle
+00000670: 7373 2062 726f 7773 6572 2061 6e64 2073  ss browser and s
+00000680: 6f6d 6520 6177 6573 6f6d 6520 6c69 6272  ome awesome libr
+00000690: 6172 6965 7320 756e 6465 7220 7468 6520  aries under the 
+000006a0: 686f 6f64 2074 6f20 6765 6e65 7261 7465  hood to generate
+000006b0: 2050 4446 2066 696c 6573 0a20 202d 205b   PDF files.  - [
+000006c0: 2a50 6c61 7977 7269 6768 742a 5d28 6874  *Playwright*](ht
+000006d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000006e0: 2f6d 6963 726f 736f 6674 2f70 6c61 7977  /microsoft/playw
+000006f0: 7269 6768 742d 7079 7468 6f6e 2920 746f  right-python) to
+00000700: 2061 7574 6f6d 6174 6520 6272 6f77 7365   automate browse
+00000710: 7273 0a20 202d 205b 2a50 6167 6564 2e6a  rs.  - [*Paged.j
+00000720: 732a 5d28 6874 7470 733a 2f2f 6769 7468  s*](https://gith
+00000730: 7562 2e63 6f6d 2f70 6167 6564 6a73 2f70  ub.com/pagedjs/p
+00000740: 6167 6564 6a73 2920 706f 6c79 6669 6c6c  agedjs) polyfill
+00000750: 7320 6172 6520 696e 636c 7564 6564 2028  s are included (
+00000760: 5b50 6167 6564 204d 6564 6961 5d28 6874  [Paged Media](ht
+00000770: 7470 733a 2f2f 7777 772e 7733 2e6f 7267  tps://www.w3.org
+00000780: 2f54 522f 6373 732d 7061 6765 2d33 2f29  /TR/css-page-3/)
+00000790: 2061 6e64 205b 4765 6e65 7261 7465 6420   and [Generated 
+000007a0: 436f 6e74 656e 745d 2868 7474 7073 3a2f  Content](https:/
+000007b0: 2f77 7777 2e77 332e 6f72 672f 5452 2f63  /www.w3.org/TR/c
+000007c0: 7373 2d67 6370 6d2d 332f 2920 4353 5320  ss-gcpm-3/) CSS 
+000007d0: 6d6f 6475 6c65 7329 0a20 202d 205b 2a53  modules).  - [*S
+000007e0: 6173 732a 5d28 6874 7470 733a 2f2f 7361  ass*](https://sa
+000007f0: 7373 2d6c 616e 672e 636f 6d2f 2920 7375  ss-lang.com/) su
+00000800: 7070 6f72 7420 2876 6961 205b 606c 6962  pport (via [`lib
+00000810: 7361 7373 605d 2868 7474 7073 3a2f 2f67  sass`](https://g
+00000820: 6974 6875 622e 636f 6d2f 7361 7373 2f6c  ithub.com/sass/l
+00000830: 6962 7361 7373 2d70 7974 686f 6e29 2920  ibsass-python)) 
+00000840: 666f 7220 796f 7572 2073 7479 6c65 7368  for your stylesh
+00000850: 6565 7473 0a0a 2323 2050 7265 7265 7175  eets..## Prerequ
+00000860: 6973 6974 6573 0a0a 2d20 5079 7468 6f6e  isites..- Python
+00000870: 2060 3e3d 2033 2e37 600a 2d20 4d6b 446f   `>= 3.7`.- MkDo
+00000880: 6373 2060 3e3d 2031 2e34 600a 0a23 2320  cs `>= 1.4`..## 
+00000890: 496e 7374 616c 6c61 7469 6f6e 0a0a 5468  Installation..Th
+000008a0: 6520 706c 7567 696e 2069 7320 686f 7374  e plugin is host
+000008b0: 6564 206f 6e20 5b2a 5079 5049 2a5d 2868  ed on [*PyPI*](h
+000008c0: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
+000008d0: 7072 6f6a 6563 742f 6d6b 646f 6373 2d65  project/mkdocs-e
+000008e0: 7870 6f72 7465 722f 2920 616e 6420 6361  xporter/) and ca
+000008f0: 6e20 6265 2069 6e73 7461 6c6c 6564 2076  n be installed v
+00000900: 6961 2060 7069 7060 2028 6f72 2079 6f75  ia `pip` (or you
+00000910: 7220 6661 766f 7572 6974 6520 7061 636b  r favourite pack
+00000920: 6167 6520 6d61 6e61 6765 7229 3a0a 0a60  age manager):..`
+00000930: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
+00000940: 6c6c 206d 6b64 6f63 732d 6578 706f 7274  ll mkdocs-export
+00000950: 6572 0a60 6060 0a0a 2323 2055 7361 6765  er.```..## Usage
+00000960: 0a0a 5468 7265 6520 706c 7567 696e 7320  ..Three plugins 
+00000970: 6172 6520 6375 7272 656e 746c 7920 6176  are currently av
+00000980: 6169 6c61 626c 653a 0a0a 2d20 606d 6b64  ailable:..- `mkd
+00000990: 6f63 732f 6578 706f 7274 6572 6020 282a  ocs/exporter` (*
+000009a0: 7265 7175 6972 6564 2a29 3a20 6261 7365  required*): base
+000009b0: 2070 6c75 6769 6e20 7768 6963 6820 6d75   plugin which mu
+000009c0: 7374 2070 7265 6365 6465 2074 6865 206f  st precede the o
+000009d0: 7468 6572 730a 2d20 606d 6b64 6f63 732f  thers.- `mkdocs/
+000009e0: 6578 706f 7274 6572 2f70 6466 6020 282a  exporter/pdf` (*
+000009f0: 6f70 7469 6f6e 616c 2a29 3a20 706c 7567  optional*): plug
+00000a00: 696e 2074 6861 7420 6578 706f 7274 7320  in that exports 
+00000a10: 796f 7572 2070 6167 6573 2061 7320 696e  your pages as in
+00000a20: 6469 7669 6475 616c 2050 4446 2064 6f63  dividual PDF doc
+00000a30: 756d 656e 7473 0a2d 2060 6d6b 646f 6373  uments.- `mkdocs
+00000a40: 2f65 7870 6f72 7465 722f 6578 7472 6173  /exporter/extras
+00000a50: 6020 282a 6f70 7469 6f6e 616c 2a29 3a20  ` (*optional*): 
+00000a60: 7072 6f76 6964 6573 2065 7874 7261 2066  provides extra f
+00000a70: 756e 6374 696f 6e61 6c69 7469 6573 2028  unctionalities (
+00000a80: 6275 7474 6f6e 732c 2048 544d 4c20 7574  buttons, HTML ut
+00000a90: 696c 6974 6965 732e 2e2e 290a 0a23 2323  ilities...)..###
+00000aa0: 2045 7861 6d70 6c65 0a0a 5468 6520 666f   Example..The fo
+00000ab0: 6c6c 6f77 696e 6720 636f 6e66 6967 7572  llowing configur
+00000ac0: 6174 696f 6e20 6578 6365 7270 7420 6672  ation excerpt fr
+00000ad0: 6f6d 2060 6d6b 646f 6373 2e79 6d6c 6020  om `mkdocs.yml` 
+00000ae0: 7368 6f75 6c64 2063 6f76 6572 2074 6865  should cover the
+00000af0: 2062 6173 6963 2066 756e 6374 696f 6e61   basic functiona
+00000b00: 6c69 7469 6573 206f 6620 7468 6973 2070  lities of this p
+00000b10: 6c75 6769 6e3a 0a0a 6060 6079 616d 6c0a  lugin:..```yaml.
+00000b20: 706c 7567 696e 733a 0a20 202d 206d 6b64  plugins:.  - mkd
+00000b30: 6f63 732f 6578 706f 7274 6572 0a20 202d  ocs/exporter.  -
+00000b40: 206d 6b64 6f63 732f 6578 706f 7274 6572   mkdocs/exporter
+00000b50: 2f70 6466 3a0a 2020 2020 2020 636f 6e63  /pdf:.      conc
+00000b60: 7572 7265 6e63 793a 2038 0a20 2020 2020  urrency: 8.     
+00000b70: 2063 6f76 6572 733a 0a20 2020 2020 2020   covers:.       
+00000b80: 2066 726f 6e74 3a20 7265 736f 7572 6365   front: resource
+00000b90: 732f 7465 6d70 6c61 7465 732f 636f 7665  s/templates/cove
+00000ba0: 7273 2f66 726f 6e74 2e68 746d 6c2e 6a32  rs/front.html.j2
+00000bb0: 0a20 2020 2020 2020 2062 6163 6b3a 2072  .        back: r
+00000bc0: 6573 6f75 7263 6573 2f74 656d 706c 6174  esources/templat
+00000bd0: 6573 2f63 6f76 6572 732f 6261 636b 2e68  es/covers/back.h
+00000be0: 746d 6c2e 6a32 0a20 2020 2020 2073 7479  tml.j2.      sty
+00000bf0: 6c65 7368 6565 7473 3a0a 2020 2020 2020  lesheets:.      
+00000c00: 2020 2d20 7265 736f 7572 6365 732f 7374    - resources/st
+00000c10: 796c 6573 6865 6574 732f 7064 662e 7363  ylesheets/pdf.sc
+00000c20: 7373 0a20 202d 206d 6b64 6f63 732f 6578  ss.  - mkdocs/ex
+00000c30: 706f 7274 6572 2f65 7874 7261 733a 0a20  porter/extras:. 
+00000c40: 2020 2020 2062 7574 746f 6e73 3a0a 2020       buttons:.  
+00000c50: 2020 2020 2020 2d20 7469 746c 653a 2044        - title: D
+00000c60: 6f77 6e6c 6f61 6420 6173 2050 4446 0a20  ownload as PDF. 
+00000c70: 2020 2020 2020 2020 2065 6e61 626c 6564           enabled
+00000c80: 3a20 2121 7079 7468 6f6e 2f6e 616d 653a  : !!python/name:
+00000c90: 6d6b 646f 6373 5f65 7870 6f72 7465 722e  mkdocs_exporter.
+00000ca0: 706c 7567 696e 732e 7064 662e 6275 7474  plugins.pdf.butt
+00000cb0: 6f6e 2e65 6e61 626c 6564 0a20 2020 2020  on.enabled.     
+00000cc0: 2020 2020 2069 636f 6e3a 2021 2170 7974       icon: !!pyt
+00000cd0: 686f 6e2f 6e61 6d65 3a6d 6b64 6f63 735f  hon/name:mkdocs_
+00000ce0: 6578 706f 7274 6572 2e70 6c75 6769 6e73  exporter.plugins
+00000cf0: 2e70 6466 2e62 7574 746f 6e2e 6963 6f6e  .pdf.button.icon
+00000d00: 0a20 2020 2020 2020 2020 2061 7474 7269  .          attri
+00000d10: 6275 7465 733a 0a20 2020 2020 2020 2020  butes:.         
+00000d20: 2020 2068 7265 663a 2021 2170 7974 686f     href: !!pytho
+00000d30: 6e2f 6e61 6d65 3a6d 6b64 6f63 735f 6578  n/name:mkdocs_ex
+00000d40: 706f 7274 6572 2e70 6c75 6769 6e73 2e70  porter.plugins.p
+00000d50: 6466 2e62 7574 746f 6e2e 6872 6566 0a20  df.button.href. 
+00000d60: 2020 2020 2020 2020 2020 2064 6f77 6e6c             downl
+00000d70: 6f61 643a 2021 2170 7974 686f 6e2f 6e61  oad: !!python/na
+00000d80: 6d65 3a6d 6b64 6f63 735f 6578 706f 7274  me:mkdocs_export
+00000d90: 6572 2e70 6c75 6769 6e73 2e70 6466 2e62  er.plugins.pdf.b
+00000da0: 7574 746f 6e2e 646f 776e 6c6f 6164 0a60  utton.download.`
+00000db0: 6060 0a0a 4368 6563 6b20 6f75 7420 6120  ``..Check out a 
+00000dc0: 5b73 616d 706c 6520 5044 4620 6765 6e65  [sample PDF gene
+00000dd0: 7261 7465 6420 6279 2074 6869 7320 706c  rated by this pl
+00000de0: 7567 696e 5d28 6578 616d 706c 6573 2f65  ugin](examples/e
+00000df0: 7861 6d70 6c65 2e70 6466 2920 6672 6f6d  xample.pdf) from
+00000e00: 2074 6865 2064 6566 6175 6c74 2070 6167   the default pag
+00000e10: 6520 6f66 2074 6865 205b 4d61 7465 7269  e of the [Materi
+00000e20: 616c 2066 6f72 204d 6b44 6f63 735d 2868  al for MkDocs](h
+00000e30: 7474 7073 3a2f 2f73 7175 6964 6675 6e6b  ttps://squidfunk
+00000e40: 2e67 6974 6875 622e 696f 2f6d 6b64 6f63  .github.io/mkdoc
+00000e50: 732d 6d61 7465 7269 616c 2920 7468 656d  s-material) them
+00000e60: 652e 2020 0a49 7420 6861 7320 6265 656e  e.  .It has been
+00000e70: 2062 7569 6c74 2077 6974 6820 736f 6d65   built with some
+00000e80: 2063 7573 746f 6d20 4353 5320 616e 6420   custom CSS and 
+00000e90: 6665 6174 7572 6573 2063 6f76 6572 2070  features cover p
+00000ea0: 6167 6573 2e0a 0a23 2320 526f 6164 6d61  ages...## Roadma
+00000eb0: 700a 0a2d 2043 6f6d 6269 6e65 2061 6c6c  p..- Combine all
+00000ec0: 2070 6167 6573 2061 7320 6f6e 6520 5044   pages as one PD
+00000ed0: 460a 0a46 6565 6c20 6672 6565 2074 6f20  F..Feel free to 
+00000ee0: 7265 7175 6573 7420 6164 6469 7469 6f6e  request addition
+00000ef0: 616c 2066 6561 7475 7265 7320 6279 2073  al features by s
+00000f00: 7562 6d69 7474 696e 6720 616e 2069 7373  ubmitting an iss
+00000f10: 7565 206f 7220 6279 2063 6f6e 7472 6962  ue or by contrib
+00000f20: 7574 696e 6720 7468 726f 7567 6820 6120  uting through a 
+00000f30: 7075 6c6c 2072 6571 7565 7374 2e0a 0a23  pull request...#
+00000f40: 2320 4c69 6365 6e73 650a 0a54 6869 7320  # License..This 
+00000f50: 7072 6f6a 6563 7420 6973 206c 6963 656e  project is licen
+00000f60: 7365 6420 756e 6465 7220 7468 6520 604d  sed under the `M
+00000f70: 4954 204c 6963 656e 7365 2028 4d49 5429  IT License (MIT)
+00000f80: 602c 2077 6869 6368 2079 6f75 2063 616e  `, which you can
+00000f90: 2072 6561 6420 5b68 6572 655d 284c 4943   read [here](LIC
+00000fa0: 454e 5345 292e 0a                        ENSE)..
```

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/browser.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/browser.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/page.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/page.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/plugin.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 class Plugin(BasePlugin):
   """The plugin."""
 
 
   def __init__(self) -> None:
     """The constructor."""
 
-    self.files: list[File] = []
+    self.stylesheets: list[File] = []
 
 
   def on_config(self, config: dict) -> None:
     """Invoked when the configuration has been loaded."""
 
     self.theme = ThemeFactory.create(config['theme'])
 
 
   def on_pre_build(self, **kwargs) -> None:
     """Invoked before the build process starts."""
 
-    self.files = []
+    self.stylesheets.clear()
 
 
   def on_pre_page(self, page: Page, **kwargs) -> None:
     """Invoked after a page has been built."""
 
     page.html = None
     page.formats = {}
@@ -39,32 +39,32 @@
   @event_priority(-100)
   def on_post_page(self, html: str, page: Page, **kwargs) -> str:
     """Invoked after a page has been built (and after all other plugins)."""
 
     preprocessor = Preprocessor(theme=page.theme)
 
     preprocessor.preprocess(html)
-    preprocessor.remove('*[data-decompose=true]')
+    preprocessor.remove('*[data-decompose="true"]')
     preprocessor.teleport()
 
     return preprocessor.done()
 
 
   def on_files(self, files: Files, **kwargs) -> Files:
     """Invoked when files are ready to be manipulated."""
 
-    self.files.extend(files.css_files())
+    self.stylesheets.extend(files.css_files())
 
     return files
 
 
   @event_priority(100)
   def on_post_build(self, **kwargs) -> None:
     """Invoked when the build process is done."""
 
-    for file in self.files:
-      css = None
+    for stylesheet in self.stylesheets:
+      content = None
 
-      with open(file.abs_dest_path, 'r', encoding='utf-8') as reader:
-        css = self.theme.stylesheet(reader.read())
-      with open(file.abs_dest_path, 'w+', encoding='utf-8') as writer:
-        writer.write(css)
+      with open(stylesheet.abs_dest_path, 'r', encoding='utf-8') as reader:
+        content = self.theme.stylesheet(reader.read())
+      with open(stylesheet.abs_dest_path, 'w+', encoding='utf-8') as writer:
+        writer.write(content)
```

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/extras/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,12 +18,15 @@
   attributes = c.Type((dict, Callable), default={})
   """Some extra attributes to add to the button."""
 
 
 class Config(BaseConfig):
   """The plugin's configuration."""
 
+  enabled = c.Type(bool, default=True)
+  """Is the plugin enabled?"""
+
   downloads = c.ListOfItems(c.Choice(('pdf', 'html')), default=['pdf'])
   """The download buttons to show."""
 
   buttons = c.ListOfItems(c.SubConfig(ButtonConfig))
   """The buttons to add."""
```

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,17 @@
   """The plugin."""
 
 
   @event_priority(-85)
   def on_post_page(self, html: str, page: Page, **kwargs) -> Optional[str]:
     """Invoked after a page has been built."""
 
+    if not self.config.enabled:
+      return
+
     def resolve(object):
       if callable(object):
         return resolve(object(page))
       if isinstance(object, list):
         return [resolve(v) for v in object]
       if isinstance(object, (dict, UserDict)):
         return {k: resolve(v) for k, v in object.items()}
```

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/pdf/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,43 +80,45 @@
     for script in self.config.scripts:
       self.renderer.add_script(script)
 
 
   def on_pre_page(self, page: Page, config: dict, **kwargs):
     """Invoked before building the page."""
 
-    if not hasattr(page, 'html'):
-      raise Exception('Missing `mkdocs/exporter` plugin or your plugins are not ordered properly!')
     if not self._enabled():
       return
+    if not hasattr(page, 'html'):
+      raise Exception('Missing `mkdocs/exporter` plugin or your plugins are not ordered properly!')
 
     directory = os.path.dirname(page.file.abs_dest_path)
     filename = os.path.splitext(os.path.basename(page.file.abs_dest_path))[0] + '.pdf'
     fullpath = os.path.join(directory, filename)
 
     page.formats['pdf'] = os.path.relpath(fullpath, config['site_dir'])
 
 
   @event_priority(-75)
   def on_post_page(self, html: str, page: Page, config: dict) -> Optional[str]:
     """Invoked after a page has been built."""
 
-    page.html = html
-
     if not self._enabled(page) and 'pdf' in page.formats:
       del page.formats['pdf']
     if 'pdf' not in page.formats:
       return html
 
+    page.html = html
+
     async def render(page: Page) -> None:
       logger.info('Rendering PDF for %s...', page.file.src_path)
 
       pdf = await self.renderer.render(page)
       fullpath = os.path.join(config['site_dir'], page.formats['pdf'])
 
+      page.html = None
+
       with open(fullpath, 'wb+') as file:
         file.write(pdf)
 
       logger.info('File written to %s!', fullpath)
 
     self.tasks.append(render(page))
```

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/preprocessor.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-2.0.2/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/theme.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/themes/factory.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/themes/factory.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/themes/material/icons.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/themes/material/icons.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/themes/material/theme.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/themes/material/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/mkdocs_exporter/themes/readthedocs/theme.py` & `mkdocs_exporter-2.0.2/mkdocs_exporter/themes/readthedocs/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.0.1/pyproject.toml` & `mkdocs_exporter-2.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "2.0.1"
+version = "2.0.2"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `mkdocs_exporter-2.0.1/PKG-INFO` & `mkdocs_exporter-2.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6d6b 646f  : 2.1.Name: mkdo
 00000020: 6373 2d65 7870 6f72 7465 720a 5665 7273  cs-exporter.Vers
-00000030: 696f 6e3a 2032 2e30 2e31 0a53 756d 6d61  ion: 2.0.1.Summa
+00000030: 696f 6e3a 2032 2e30 2e32 0a53 756d 6d61  ion: 2.0.2.Summa
 00000040: 7279 3a20 4120 6869 6768 6c79 2d63 6f6e  ry: A highly-con
 00000050: 6669 6775 7261 626c 6520 706c 7567 696e  figurable plugin
 00000060: 2066 6f72 204d 6b44 6f63 7320 7468 6174   for MkDocs that
 00000070: 2065 7870 6f72 7473 2079 6f75 7220 7061   exports your pa
 00000080: 6765 7320 746f 2050 4446 2066 696c 6573  ges to PDF files
 00000090: 2e0a 486f 6d65 2d70 6167 653a 2068 7474  ..Home-page: htt
 000000a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
@@ -39,254 +39,298 @@
 00000260: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
 00000270: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 00000280: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
 00000290: 2033 2e31 300a 436c 6173 7369 6669 6572   3.10.Classifier
 000002a0: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
 000002b0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
 000002c0: 203a 3a20 332e 3131 0a43 6c61 7373 6966   :: 3.11.Classif
-000002d0: 6965 723a 2054 6f70 6963 203a 3a20 446f  ier: Topic :: Do
-000002e0: 6375 6d65 6e74 6174 696f 6e0a 436c 6173  cumentation.Clas
-000002f0: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
-00000300: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
-00000310: 706d 656e 7420 3a3a 2044 6f63 756d 656e  pment :: Documen
-00000320: 7461 7469 6f6e 0a43 6c61 7373 6966 6965  tation.Classifie
-00000330: 723a 2054 6f70 6963 203a 3a20 5465 7874  r: Topic :: Text
-00000340: 2050 726f 6365 7373 696e 6720 3a3a 204d   Processing :: M
-00000350: 6172 6b75 7020 3a3a 2048 544d 4c0a 5265  arkup :: HTML.Re
-00000360: 7175 6972 6573 2d44 6973 743a 2062 6561  quires-Dist: bea
-00000370: 7574 6966 756c 736f 7570 3420 283e 3d34  utifulsoup4 (>=4
-00000380: 2e31 322e 3229 0a52 6571 7569 7265 732d  .12.2).Requires-
-00000390: 4469 7374 3a20 696d 706f 7274 6c69 622d  Dist: importlib-
-000003a0: 6d65 7461 6461 7461 2028 3c35 2e30 290a  metadata (<5.0).
-000003b0: 5265 7175 6972 6573 2d44 6973 743a 2069  Requires-Dist: i
-000003c0: 6d70 6f72 746c 6962 2d72 6573 6f75 7263  mportlib-resourc
-000003d0: 6573 2028 3e3d 352e 3029 0a52 6571 7569  es (>=5.0).Requi
-000003e0: 7265 732d 4469 7374 3a20 6c69 6273 6173  res-Dist: libsas
-000003f0: 7320 283e 3d30 2e32 322e 3029 0a52 6571  s (>=0.22.0).Req
-00000400: 7569 7265 732d 4469 7374 3a20 6c78 6d6c  uires-Dist: lxml
-00000410: 2028 3e3d 342e 3929 0a52 6571 7569 7265   (>=4.9).Require
-00000420: 732d 4469 7374 3a20 6d6b 646f 6373 2028  s-Dist: mkdocs (
-00000430: 3e3d 312e 3429 0a52 6571 7569 7265 732d  >=1.4).Requires-
-00000440: 4469 7374 3a20 706c 6179 7772 6967 6874  Dist: playwright
-00000450: 2028 3e3d 312e 3333 290a 5072 6f6a 6563   (>=1.33).Projec
-00000460: 742d 5552 4c3a 2042 7567 2054 7261 636b  t-URL: Bug Track
-00000470: 6572 2c20 6874 7470 733a 2f2f 6769 7468  er, https://gith
-00000480: 7562 2e63 6f6d 2f61 6472 6965 6e62 7269  ub.com/adrienbri
-00000490: 676e 6f6e 2f6d 6b64 6f63 732d 6578 706f  gnon/mkdocs-expo
-000004a0: 7274 6572 2f69 7373 7565 730a 5072 6f6a  rter/issues.Proj
-000004b0: 6563 742d 5552 4c3a 2052 6570 6f73 6974  ect-URL: Reposit
-000004c0: 6f72 792c 2068 7474 7073 3a2f 2f67 6974  ory, https://git
-000004d0: 6875 622e 636f 6d2f 6164 7269 656e 6272  hub.com/adrienbr
-000004e0: 6967 6e6f 6e2f 6d6b 646f 6373 2d65 7870  ignon/mkdocs-exp
-000004f0: 6f72 7465 720a 4465 7363 7269 7074 696f  orter.Descriptio
-00000500: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000510: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
-00000520: 204d 6b44 6f63 7320 4578 706f 7274 6572   MkDocs Exporter
-00000530: 0a0a 4120 6869 6768 6c79 2d63 6f6e 6669  ..A highly-confi
-00000540: 6775 7261 626c 6520 706c 7567 696e 2066  gurable plugin f
-00000550: 6f72 205b 2a4d 6b44 6f63 732a 5d28 6874  or [*MkDocs*](ht
-00000560: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000570: 2f6d 6b64 6f63 732f 6d6b 646f 6373 2920  /mkdocs/mkdocs) 
-00000580: 7468 6174 2065 7870 6f72 7473 2079 6f75  that exports you
-00000590: 7220 7061 6765 7320 746f 2050 4446 2066  r pages to PDF f
-000005a0: 696c 6573 2e0a 0a2d 205b 446f 6375 6d65  iles...- [Docume
-000005b0: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
-000005c0: 2f61 6472 6965 6e62 7269 676e 6f6e 2e67  /adrienbrignon.g
-000005d0: 6974 6875 622e 696f 2f6d 6b64 6f63 732d  ithub.io/mkdocs-
-000005e0: 6578 706f 7274 6572 290a 2d20 5b50 7950  exporter).- [PyP
-000005f0: 495d 2868 7474 7073 3a2f 2f70 7970 692e  I](https://pypi.
-00000600: 6f72 672f 7072 6f6a 6563 742f 6d6b 646f  org/project/mkdo
-00000610: 6373 2d65 7870 6f72 7465 7229 0a0a 2323  cs-exporter)..##
-00000620: 2046 6561 7475 7265 730a 0a2d 20f0 9f9a   Features..- ...
-00000630: 8020 2a2a 4661 7374 2a2a 202d 2050 4446  . **Fast** - PDF
-00000640: 2064 6f63 756d 656e 7473 2061 7265 2067   documents are g
-00000650: 656e 6572 6174 6564 2063 6f6e 6375 7272  enerated concurr
-00000660: 656e 746c 7921 0a2d 20f0 9f8e a820 2a2a  ently!.- .... **
-00000670: 4375 7374 6f6d 697a 6162 6c65 2a2a 202d  Customizable** -
-00000680: 2066 756c 6c20 636f 6e74 726f 6c20 6f76   full control ov
-00000690: 6572 2074 6865 2072 6573 756c 7469 6e67  er the resulting
-000006a0: 2064 6f63 756d 656e 7473 0a20 202d 2043   documents.  - C
-000006b0: 6f76 6572 2070 6167 6573 2028 7375 7070  over pages (supp
-000006c0: 6f72 7473 205b 606d 6163 726f 7360 5d28  orts [`macros`](
-000006d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000006e0: 6f6d 2f66 7261 6c61 752f 6d6b 646f 6373  om/fralau/mkdocs
-000006f0: 5f6d 6163 726f 735f 706c 7567 696e 2920  _macros_plugin) 
-00000700: 706c 7567 696e 290a 2020 2d20 4465 6669  plugin).  - Defi
-00000710: 6e65 2063 7573 746f 6d20 7363 7269 7074  ne custom script
-00000720: 7320 616e 6420 7374 796c 6573 6865 6574  s and stylesheet
-00000730: 7320 746f 2063 7573 746f 6d69 7a65 2079  s to customize y
-00000740: 6f75 7220 5044 4620 646f 6375 6d65 6e74  our PDF document
-00000750: 730a 2020 2d20 4465 6669 6e65 2022 6275  s.  - Define "bu
-00000760: 7474 6f6e 7322 2061 7420 7468 6520 746f  ttons" at the to
-00000770: 7020 6f66 2079 6f75 7220 646f 6375 6d65  p of your docume
-00000780: 6e74 6174 696f 6e20 7061 6765 7320 285b  ntation pages ([
-00000790: 6578 616d 706c 655d 2868 7474 7073 3a2f  example](https:/
-000007a0: 2f61 6472 6965 6e62 7269 676e 6f6e 2e67  /adrienbrignon.g
-000007b0: 6974 6875 622e 696f 2f6d 6b64 6f63 732d  ithub.io/mkdocs-
-000007c0: 6578 706f 7274 6572 2f73 6574 7570 2f73  exporter/setup/s
-000007d0: 6574 7469 6e67 2d75 702d 6275 7474 6f6e  etting-up-button
-000007e0: 732f 2929 0a20 202d 2043 6f6d 7061 7469  s/)).  - Compati
-000007f0: 626c 6520 7769 7468 205b 606d 6174 6572  ble with [`mater
-00000800: 6961 6c60 5d28 6874 7470 733a 2f2f 6769  ial`](https://gi
-00000810: 7468 7562 2e63 6f6d 2f73 7175 6964 6675  thub.com/squidfu
-00000820: 6e6b 2f6d 6b64 6f63 732d 6d61 7465 7269  nk/mkdocs-materi
-00000830: 616c 2920 616e 6420 5b60 7265 6164 7468  al) and [`readth
-00000840: 6564 6f63 7360 5d28 6874 7470 733a 2f2f  edocs`](https://
-00000850: 7777 772e 6d6b 646f 6373 2e6f 7267 2f75  www.mkdocs.org/u
-00000860: 7365 722d 6775 6964 652f 6368 6f6f 7369  ser-guide/choosi
-00000870: 6e67 2d79 6f75 722d 7468 656d 652f 2372  ng-your-theme/#r
-00000880: 6561 6474 6865 646f 6373 2920 7468 656d  eadthedocs) them
-00000890: 6573 0a2d 20e2 ad90 202a 2a50 6f77 6572  es.- ... **Power
-000008a0: 6675 6c2a 2a20 2d20 6974 2075 7365 7320  ful** - it uses 
-000008b0: 6120 6865 6164 6c65 7373 2062 726f 7773  a headless brows
-000008c0: 6572 2061 6e64 2073 6f6d 6520 6177 6573  er and some awes
-000008d0: 6f6d 6520 6c69 6272 6172 6965 7320 756e  ome libraries un
-000008e0: 6465 7220 7468 6520 686f 6f64 2074 6f20  der the hood to 
-000008f0: 6765 6e65 7261 7465 2050 4446 2066 696c  generate PDF fil
-00000900: 6573 0a20 202d 205b 2a50 6c61 7977 7269  es.  - [*Playwri
-00000910: 6768 742a 5d28 6874 7470 733a 2f2f 6769  ght*](https://gi
-00000920: 7468 7562 2e63 6f6d 2f6d 6963 726f 736f  thub.com/microso
-00000930: 6674 2f70 6c61 7977 7269 6768 742d 7079  ft/playwright-py
-00000940: 7468 6f6e 2920 746f 2061 7574 6f6d 6174  thon) to automat
-00000950: 6520 6272 6f77 7365 7273 0a20 202d 205b  e browsers.  - [
-00000960: 2a50 6167 6564 2e6a 732a 5d28 6874 7470  *Paged.js*](http
-00000970: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-00000980: 6167 6564 6a73 2f70 6167 6564 6a73 2920  agedjs/pagedjs) 
-00000990: 706f 6c79 6669 6c6c 7320 6172 6520 696e  polyfills are in
-000009a0: 636c 7564 6564 2028 5b50 6167 6564 204d  cluded ([Paged M
-000009b0: 6564 6961 5d28 6874 7470 733a 2f2f 7777  edia](https://ww
-000009c0: 772e 7733 2e6f 7267 2f54 522f 6373 732d  w.w3.org/TR/css-
-000009d0: 7061 6765 2d33 2f29 2061 6e64 205b 4765  page-3/) and [Ge
-000009e0: 6e65 7261 7465 6420 436f 6e74 656e 745d  nerated Content]
-000009f0: 2868 7474 7073 3a2f 2f77 7777 2e77 332e  (https://www.w3.
-00000a00: 6f72 672f 5452 2f63 7373 2d67 6370 6d2d  org/TR/css-gcpm-
-00000a10: 332f 2920 4353 5320 6d6f 6475 6c65 7329  3/) CSS modules)
-00000a20: 0a20 202d 205b 2a53 6173 732a 5d28 6874  .  - [*Sass*](ht
-00000a30: 7470 733a 2f2f 7361 7373 2d6c 616e 672e  tps://sass-lang.
-00000a40: 636f 6d2f 2920 7375 7070 6f72 7420 2876  com/) support (v
-00000a50: 6961 205b 606c 6962 7361 7373 605d 2868  ia [`libsass`](h
-00000a60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000a70: 6d2f 7361 7373 2f6c 6962 7361 7373 2d70  m/sass/libsass-p
-00000a80: 7974 686f 6e29 2920 666f 7220 796f 7572  ython)) for your
-00000a90: 2073 7479 6c65 7368 6565 7473 0a0a 2323   stylesheets..##
-00000aa0: 2050 7265 7265 7175 6973 6974 6573 0a0a   Prerequisites..
-00000ab0: 2d20 5079 7468 6f6e 2060 3e3d 2033 2e37  - Python `>= 3.7
-00000ac0: 600a 2d20 4d6b 446f 6373 2060 3e3d 2031  `.- MkDocs `>= 1
-00000ad0: 2e34 600a 0a23 2320 496e 7374 616c 6c61  .4`..## Installa
-00000ae0: 7469 6f6e 0a0a 5468 6520 706c 7567 696e  tion..The plugin
-00000af0: 2069 7320 686f 7374 6564 206f 6e20 5b2a   is hosted on [*
-00000b00: 5079 5049 2a5d 2868 7474 7073 3a2f 2f70  PyPI*](https://p
-00000b10: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000b20: 6d6b 646f 6373 2d65 7870 6f72 7465 722f  mkdocs-exporter/
-00000b30: 2920 616e 6420 6361 6e20 6265 2069 6e73  ) and can be ins
-00000b40: 7461 6c6c 6564 2076 6961 2060 7069 7060  talled via `pip`
-00000b50: 2028 6f72 2079 6f75 7220 6661 766f 7572   (or your favour
-00000b60: 6974 6520 7061 636b 6167 6520 6d61 6e61  ite package mana
-00000b70: 6765 7229 3a0a 0a60 6060 6261 7368 0a70  ger):..```bash.p
-00000b80: 6970 2069 6e73 7461 6c6c 206d 6b64 6f63  ip install mkdoc
-00000b90: 732d 6578 706f 7274 6572 0a60 6060 0a0a  s-exporter.```..
-00000ba0: 2323 2055 7361 6765 0a0a 5468 7265 6520  ## Usage..Three 
-00000bb0: 706c 7567 696e 7320 6172 6520 6375 7272  plugins are curr
-00000bc0: 656e 746c 7920 6176 6169 6c61 626c 653a  ently available:
-00000bd0: 0a0a 2d20 606d 6b64 6f63 732f 6578 706f  ..- `mkdocs/expo
-00000be0: 7274 6572 6020 282a 7265 7175 6972 6564  rter` (*required
-00000bf0: 2a29 3a20 6261 7365 2070 6c75 6769 6e20  *): base plugin 
-00000c00: 7768 6963 6820 6d75 7374 2070 7265 6365  which must prece
-00000c10: 6465 2074 6865 206f 7468 6572 730a 2d20  de the others.- 
-00000c20: 606d 6b64 6f63 732f 6578 706f 7274 6572  `mkdocs/exporter
-00000c30: 2f70 6466 6020 282a 6f70 7469 6f6e 616c  /pdf` (*optional
-00000c40: 2a29 3a20 706c 7567 696e 2074 6861 7420  *): plugin that 
-00000c50: 6578 706f 7274 7320 796f 7572 2070 6167  exports your pag
-00000c60: 6573 2061 7320 696e 6469 7669 6475 616c  es as individual
-00000c70: 2050 4446 2064 6f63 756d 656e 7473 0a2d   PDF documents.-
-00000c80: 2060 6d6b 646f 6373 2f65 7870 6f72 7465   `mkdocs/exporte
-00000c90: 722f 6578 7472 6173 6020 282a 6f70 7469  r/extras` (*opti
-00000ca0: 6f6e 616c 2a29 3a20 7072 6f76 6964 6573  onal*): provides
-00000cb0: 2065 7874 7261 2066 756e 6374 696f 6e61   extra functiona
-00000cc0: 6c69 7469 6573 2028 6275 7474 6f6e 732c  lities (buttons,
-00000cd0: 2048 544d 4c20 7574 696c 6974 6965 732e   HTML utilities.
-00000ce0: 2e2e 290a 0a23 2323 2045 7861 6d70 6c65  ..)..### Example
-00000cf0: 0a0a 5468 6520 666f 6c6c 6f77 696e 6720  ..The following 
-00000d00: 636f 6e66 6967 7572 6174 696f 6e20 6578  configuration ex
-00000d10: 6365 7270 7420 6672 6f6d 2060 6d6b 646f  cerpt from `mkdo
-00000d20: 6373 2e79 6d6c 6020 7368 6f75 6c64 2063  cs.yml` should c
-00000d30: 6f76 6572 2074 6865 2062 6173 6963 2066  over the basic f
-00000d40: 756e 6374 696f 6e61 6c69 7469 6573 206f  unctionalities o
-00000d50: 6620 7468 6973 2070 6c75 6769 6e3a 0a0a  f this plugin:..
-00000d60: 6060 6079 616d 6c0a 706c 7567 696e 733a  ```yaml.plugins:
-00000d70: 0a20 202d 206d 6b64 6f63 732f 6578 706f  .  - mkdocs/expo
-00000d80: 7274 6572 0a20 202d 206d 6b64 6f63 732f  rter.  - mkdocs/
-00000d90: 6578 706f 7274 6572 2f70 6466 3a0a 2020  exporter/pdf:.  
-00000da0: 2020 2020 636f 6e63 7572 7265 6e63 793a      concurrency:
-00000db0: 2038 0a20 2020 2020 2063 6f76 6572 733a   8.      covers:
-00000dc0: 0a20 2020 2020 2020 2066 726f 6e74 3a20  .        front: 
-00000dd0: 7265 736f 7572 6365 732f 7465 6d70 6c61  resources/templa
-00000de0: 7465 732f 636f 7665 7273 2f66 726f 6e74  tes/covers/front
-00000df0: 2e68 746d 6c2e 6a32 0a20 2020 2020 2020  .html.j2.       
-00000e00: 2062 6163 6b3a 2072 6573 6f75 7263 6573   back: resources
-00000e10: 2f74 656d 706c 6174 6573 2f63 6f76 6572  /templates/cover
-00000e20: 732f 6261 636b 2e68 746d 6c2e 6a32 0a20  s/back.html.j2. 
-00000e30: 2020 2020 2073 7479 6c65 7368 6565 7473       stylesheets
-00000e40: 3a0a 2020 2020 2020 2020 2d20 7265 736f  :.        - reso
-00000e50: 7572 6365 732f 7374 796c 6573 6865 6574  urces/stylesheet
-00000e60: 732f 7064 662e 7363 7373 0a20 202d 206d  s/pdf.scss.  - m
-00000e70: 6b64 6f63 732f 6578 706f 7274 6572 2f65  kdocs/exporter/e
-00000e80: 7874 7261 733a 0a20 2020 2020 2062 7574  xtras:.      but
-00000e90: 746f 6e73 3a0a 2020 2020 2020 2020 2d20  tons:.        - 
-00000ea0: 7469 746c 653a 2044 6f77 6e6c 6f61 6420  title: Download 
-00000eb0: 6173 2050 4446 0a20 2020 2020 2020 2020  as PDF.         
-00000ec0: 2065 6e61 626c 6564 3a20 2121 7079 7468   enabled: !!pyth
-00000ed0: 6f6e 2f6e 616d 653a 6d6b 646f 6373 5f65  on/name:mkdocs_e
-00000ee0: 7870 6f72 7465 722e 706c 7567 696e 732e  xporter.plugins.
-00000ef0: 7064 662e 6275 7474 6f6e 2e65 6e61 626c  pdf.button.enabl
-00000f00: 6564 0a20 2020 2020 2020 2020 2069 636f  ed.          ico
-00000f10: 6e3a 2021 2170 7974 686f 6e2f 6e61 6d65  n: !!python/name
-00000f20: 3a6d 6b64 6f63 735f 6578 706f 7274 6572  :mkdocs_exporter
-00000f30: 2e70 6c75 6769 6e73 2e70 6466 2e62 7574  .plugins.pdf.but
-00000f40: 746f 6e2e 6963 6f6e 0a20 2020 2020 2020  ton.icon.       
-00000f50: 2020 2061 7474 7269 6275 7465 733a 0a20     attributes:. 
-00000f60: 2020 2020 2020 2020 2020 2068 7265 663a             href:
-00000f70: 2021 2170 7974 686f 6e2f 6e61 6d65 3a6d   !!python/name:m
-00000f80: 6b64 6f63 735f 6578 706f 7274 6572 2e70  kdocs_exporter.p
-00000f90: 6c75 6769 6e73 2e70 6466 2e62 7574 746f  lugins.pdf.butto
-00000fa0: 6e2e 6872 6566 0a20 2020 2020 2020 2020  n.href.         
-00000fb0: 2020 2064 6f77 6e6c 6f61 643a 2021 2170     download: !!p
-00000fc0: 7974 686f 6e2f 6e61 6d65 3a6d 6b64 6f63  ython/name:mkdoc
-00000fd0: 735f 6578 706f 7274 6572 2e70 6c75 6769  s_exporter.plugi
-00000fe0: 6e73 2e70 6466 2e62 7574 746f 6e2e 646f  ns.pdf.button.do
-00000ff0: 776e 6c6f 6164 0a60 6060 0a0a 4368 6563  wnload.```..Chec
-00001000: 6b20 6f75 7420 6120 5b73 616d 706c 6520  k out a [sample 
-00001010: 5044 4620 6765 6e65 7261 7465 6420 6279  PDF generated by
-00001020: 2074 6869 7320 706c 7567 696e 5d28 6578   this plugin](ex
-00001030: 616d 706c 6573 2f65 7861 6d70 6c65 2e70  amples/example.p
-00001040: 6466 2920 6672 6f6d 2074 6865 2064 6566  df) from the def
-00001050: 6175 6c74 2070 6167 6520 6f66 2074 6865  ault page of the
-00001060: 205b 4d61 7465 7269 616c 2066 6f72 204d   [Material for M
-00001070: 6b44 6f63 735d 2868 7474 7073 3a2f 2f73  kDocs](https://s
-00001080: 7175 6964 6675 6e6b 2e67 6974 6875 622e  quidfunk.github.
-00001090: 696f 2f6d 6b64 6f63 732d 6d61 7465 7269  io/mkdocs-materi
-000010a0: 616c 2920 7468 656d 652e 2020 0a49 7420  al) theme.  .It 
-000010b0: 6861 7320 6265 656e 2062 7569 6c74 2077  has been built w
-000010c0: 6974 6820 736f 6d65 2063 7573 746f 6d20  ith some custom 
-000010d0: 4353 5320 616e 6420 6665 6174 7572 6573  CSS and features
-000010e0: 2063 6f76 6572 2070 6167 6573 2e0a 0a23   cover pages...#
-000010f0: 2320 526f 6164 6d61 700a 0a2d 2045 6e73  # Roadmap..- Ens
-00001100: 7572 6520 6675 6c6c 2063 6f6d 7061 7469  ure full compati
-00001110: 6269 6c69 7479 2077 6974 6820 6f74 6865  bility with othe
-00001120: 7220 7468 656d 6573 2074 6861 6e20 606d  r themes than `m
-00001130: 6b64 6f63 732d 6d61 7465 7269 616c 600a  kdocs-material`.
-00001140: 2d20 436f 6d62 696e 6520 616c 6c20 7061  - Combine all pa
-00001150: 6765 7320 6173 206f 6e65 2050 4446 0a0a  ges as one PDF..
-00001160: 4665 656c 2066 7265 6520 746f 2072 6571  Feel free to req
-00001170: 7565 7374 2061 6464 6974 696f 6e61 6c20  uest additional 
-00001180: 6665 6174 7572 6573 2062 7920 7375 626d  features by subm
-00001190: 6974 7469 6e67 2061 6e20 6973 7375 6520  itting an issue 
-000011a0: 6f72 2062 7920 636f 6e74 7269 6275 7469  or by contributi
-000011b0: 6e67 2074 6872 6f75 6768 2061 2070 756c  ng through a pul
-000011c0: 6c20 7265 7175 6573 742e 0a0a 2323 204c  l request...## L
-000011d0: 6963 656e 7365 0a0a 5468 6973 2070 726f  icense..This pro
-000011e0: 6a65 6374 2069 7320 6c69 6365 6e73 6564  ject is licensed
-000011f0: 2075 6e64 6572 2074 6865 2060 4d49 5420   under the `MIT 
-00001200: 4c69 6365 6e73 6520 284d 4954 2960 2c20  License (MIT)`, 
-00001210: 7768 6963 6820 796f 7520 6361 6e20 7265  which you can re
-00001220: 6164 205b 6865 7265 5d28 4c49 4345 4e53  ad [here](LICENS
-00001230: 4529 2e0a 0a                             E)...
+000002d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000002e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002f0: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
+00000300: 6965 723a 2054 6f70 6963 203a 3a20 446f  ier: Topic :: Do
+00000310: 6375 6d65 6e74 6174 696f 6e0a 436c 6173  cumentation.Clas
+00000320: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000330: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
+00000340: 706d 656e 7420 3a3a 2044 6f63 756d 656e  pment :: Documen
+00000350: 7461 7469 6f6e 0a43 6c61 7373 6966 6965  tation.Classifie
+00000360: 723a 2054 6f70 6963 203a 3a20 5465 7874  r: Topic :: Text
+00000370: 2050 726f 6365 7373 696e 6720 3a3a 204d   Processing :: M
+00000380: 6172 6b75 7020 3a3a 2048 544d 4c0a 5265  arkup :: HTML.Re
+00000390: 7175 6972 6573 2d44 6973 743a 2062 6561  quires-Dist: bea
+000003a0: 7574 6966 756c 736f 7570 3420 283e 3d34  utifulsoup4 (>=4
+000003b0: 2e31 322e 3229 0a52 6571 7569 7265 732d  .12.2).Requires-
+000003c0: 4469 7374 3a20 696d 706f 7274 6c69 622d  Dist: importlib-
+000003d0: 6d65 7461 6461 7461 2028 3c35 2e30 290a  metadata (<5.0).
+000003e0: 5265 7175 6972 6573 2d44 6973 743a 2069  Requires-Dist: i
+000003f0: 6d70 6f72 746c 6962 2d72 6573 6f75 7263  mportlib-resourc
+00000400: 6573 2028 3e3d 352e 3029 0a52 6571 7569  es (>=5.0).Requi
+00000410: 7265 732d 4469 7374 3a20 6c69 6273 6173  res-Dist: libsas
+00000420: 7320 283e 3d30 2e32 322e 3029 0a52 6571  s (>=0.22.0).Req
+00000430: 7569 7265 732d 4469 7374 3a20 6c78 6d6c  uires-Dist: lxml
+00000440: 2028 3e3d 342e 3929 0a52 6571 7569 7265   (>=4.9).Require
+00000450: 732d 4469 7374 3a20 6d6b 646f 6373 2028  s-Dist: mkdocs (
+00000460: 3e3d 312e 3429 0a52 6571 7569 7265 732d  >=1.4).Requires-
+00000470: 4469 7374 3a20 706c 6179 7772 6967 6874  Dist: playwright
+00000480: 2028 3e3d 312e 3333 290a 5072 6f6a 6563   (>=1.33).Projec
+00000490: 742d 5552 4c3a 2042 7567 2054 7261 636b  t-URL: Bug Track
+000004a0: 6572 2c20 6874 7470 733a 2f2f 6769 7468  er, https://gith
+000004b0: 7562 2e63 6f6d 2f61 6472 6965 6e62 7269  ub.com/adrienbri
+000004c0: 676e 6f6e 2f6d 6b64 6f63 732d 6578 706f  gnon/mkdocs-expo
+000004d0: 7274 6572 2f69 7373 7565 730a 5072 6f6a  rter/issues.Proj
+000004e0: 6563 742d 5552 4c3a 2052 6570 6f73 6974  ect-URL: Reposit
+000004f0: 6f72 792c 2068 7474 7073 3a2f 2f67 6974  ory, https://git
+00000500: 6875 622e 636f 6d2f 6164 7269 656e 6272  hub.com/adrienbr
+00000510: 6967 6e6f 6e2f 6d6b 646f 6373 2d65 7870  ignon/mkdocs-exp
+00000520: 6f72 7465 720a 4465 7363 7269 7074 696f  orter.Descriptio
+00000530: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00000540: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
+00000550: 204d 6b44 6f63 7320 4578 706f 7274 6572   MkDocs Exporter
+00000560: 0a0a 3c64 6976 3e0a 2020 3c61 2068 7265  ..<div>.  <a hre
+00000570: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+00000580: 6f72 672f 7072 6f6a 6563 742f 6d6b 646f  org/project/mkdo
+00000590: 6373 2d65 7870 6f72 7465 7222 3e0a 2020  cs-exporter">.  
+000005a0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000005b0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000005c0: 696f 2f70 7970 692f 762f 6d6b 646f 6373  io/pypi/v/mkdocs
+000005d0: 2d65 7870 6f72 7465 723f 636f 6c6f 723d  -exporter?color=
+000005e0: 626c 7565 223e 0a20 203c 2f61 3e0a 2020  blue">.  </a>.  
+000005f0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000600: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000610: 742f 6d6b 646f 6373 2d65 7870 6f72 7465  t/mkdocs-exporte
+00000620: 7222 3e0a 2020 2020 3c69 6d67 2073 7263  r">.    <img src
+00000630: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000640: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
+00000650: 7665 7273 696f 6e73 2f6d 6b64 6f63 732d  versions/mkdocs-
+00000660: 6578 706f 7274 6572 3f63 6f6c 6f72 3d62  exporter?color=b
+00000670: 6c75 6522 3e0a 2020 3c2f 613e 0a20 203c  lue">.  </a>.  <
+00000680: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000690: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000006a0: 2f6d 6b64 6f63 732d 6578 706f 7274 6572  /mkdocs-exporter
+000006b0: 223e 0a20 2020 203c 696d 6720 7372 633d  ">.    <img src=
+000006c0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+000006d0: 656c 6473 2e69 6f2f 7079 7069 2f64 6d2f  elds.io/pypi/dm/
+000006e0: 6d6b 646f 6373 2d65 7870 6f72 7465 723f  mkdocs-exporter?
+000006f0: 636f 6c6f 723d 6361 6374 7573 223e 0a20  color=cactus">. 
+00000700: 203c 2f61 3e0a 2020 3c61 2068 7265 663d   </a>.  <a href=
+00000710: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000720: 636f 6d2f 6164 7269 656e 6272 6967 6e6f  com/adrienbrigno
+00000730: 6e2f 6d6b 646f 6373 2d65 7870 6f72 7465  n/mkdocs-exporte
+00000740: 722f 626c 6f62 2f6d 6173 7465 722f 4c49  r/blob/master/LI
+00000750: 4345 4e53 4522 3e0a 2020 2020 3c69 6d67  CENSE">.    <img
+00000760: 2061 6c69 676e 3d22 7269 6768 7422 2073   align="right" s
+00000770: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000780: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+00000790: 622f 6c69 6365 6e73 652f 6164 7269 656e  b/license/adrien
+000007a0: 6272 6967 6e6f 6e2f 6d6b 646f 6373 2d65  brignon/mkdocs-e
+000007b0: 7870 6f72 7465 723f 636f 6c6f 723d 7768  xporter?color=wh
+000007c0: 6974 6522 3e0a 2020 3c2f 613e 0a3c 2f64  ite">.  </a>.</d
+000007d0: 6976 3e0a 3c62 7220 2f3e 0a0a 4120 6869  iv>.<br />..A hi
+000007e0: 6768 6c79 2d63 6f6e 6669 6775 7261 626c  ghly-configurabl
+000007f0: 6520 706c 7567 696e 2066 6f72 205b 2a4d  e plugin for [*M
+00000800: 6b44 6f63 732a 5d28 6874 7470 733a 2f2f  kDocs*](https://
+00000810: 6769 7468 7562 2e63 6f6d 2f6d 6b64 6f63  github.com/mkdoc
+00000820: 732f 6d6b 646f 6373 2920 7468 6174 2065  s/mkdocs) that e
+00000830: 7870 6f72 7473 2079 6f75 7220 7061 6765  xports your page
+00000840: 7320 746f 2050 4446 2066 696c 6573 2e0a  s to PDF files..
+00000850: 0a2d 205b 446f 6375 6d65 6e74 6174 696f  .- [Documentatio
+00000860: 6e5d 2868 7474 7073 3a2f 2f61 6472 6965  n](https://adrie
+00000870: 6e62 7269 676e 6f6e 2e67 6974 6875 622e  nbrignon.github.
+00000880: 696f 2f6d 6b64 6f63 732d 6578 706f 7274  io/mkdocs-export
+00000890: 6572 290a 2d20 5b50 7950 495d 2868 7474  er).- [PyPI](htt
+000008a0: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
+000008b0: 6f6a 6563 742f 6d6b 646f 6373 2d65 7870  oject/mkdocs-exp
+000008c0: 6f72 7465 7229 0a2d 205b 4578 616d 706c  orter).- [Exampl
+000008d0: 6573 5d28 2e2f 6578 616d 706c 6573 290a  es](./examples).
+000008e0: 0a23 2320 4665 6174 7572 6573 0a0a 2d20  .## Features..- 
+000008f0: f09f 9a80 202a 2a46 6173 742a 2a20 2d20  .... **Fast** - 
+00000900: 5044 4620 646f 6375 6d65 6e74 7320 6172  PDF documents ar
+00000910: 6520 6765 6e65 7261 7465 6420 636f 6e63  e generated conc
+00000920: 7572 7265 6e74 6c79 210a 2d20 f09f 8ea8  urrently!.- ....
+00000930: 202a 2a43 7573 746f 6d69 7a61 626c 652a   **Customizable*
+00000940: 2a20 2d20 6675 6c6c 2063 6f6e 7472 6f6c  * - full control
+00000950: 206f 7665 7220 7468 6520 7265 7375 6c74   over the result
+00000960: 696e 6720 646f 6375 6d65 6e74 730a 2020  ing documents.  
+00000970: 2d20 436f 7665 7220 7061 6765 7320 2873  - Cover pages (s
+00000980: 7570 706f 7274 7320 5b60 6d61 6372 6f73  upports [`macros
+00000990: 605d 2868 7474 7073 3a2f 2f67 6974 6875  `](https://githu
+000009a0: 622e 636f 6d2f 6672 616c 6175 2f6d 6b64  b.com/fralau/mkd
+000009b0: 6f63 735f 6d61 6372 6f73 5f70 6c75 6769  ocs_macros_plugi
+000009c0: 6e29 2070 6c75 6769 6e29 0a20 202d 2044  n) plugin).  - D
+000009d0: 6566 696e 6520 6375 7374 6f6d 2073 6372  efine custom scr
+000009e0: 6970 7473 2061 6e64 2073 7479 6c65 7368  ipts and stylesh
+000009f0: 6565 7473 2074 6f20 6375 7374 6f6d 697a  eets to customiz
+00000a00: 6520 796f 7572 2050 4446 2064 6f63 756d  e your PDF docum
+00000a10: 656e 7473 0a20 202d 2044 6566 696e 6520  ents.  - Define 
+00000a20: 2262 7574 746f 6e73 2220 6174 2074 6865  "buttons" at the
+00000a30: 2074 6f70 206f 6620 796f 7572 2064 6f63   top of your doc
+00000a40: 756d 656e 7461 7469 6f6e 2070 6167 6573  umentation pages
+00000a50: 2028 5b65 7861 6d70 6c65 5d28 6874 7470   ([example](http
+00000a60: 733a 2f2f 6164 7269 656e 6272 6967 6e6f  s://adrienbrigno
+00000a70: 6e2e 6769 7468 7562 2e69 6f2f 6d6b 646f  n.github.io/mkdo
+00000a80: 6373 2d65 7870 6f72 7465 722f 7365 7475  cs-exporter/setu
+00000a90: 702f 7365 7474 696e 672d 7570 2d62 7574  p/setting-up-but
+00000aa0: 746f 6e73 2f29 290a 2020 2d20 436f 6d70  tons/)).  - Comp
+00000ab0: 6174 6962 6c65 2077 6974 6820 5b60 6d61  atible with [`ma
+00000ac0: 7465 7269 616c 605d 2868 7474 7073 3a2f  terial`](https:/
+00000ad0: 2f67 6974 6875 622e 636f 6d2f 7371 7569  /github.com/squi
+00000ae0: 6466 756e 6b2f 6d6b 646f 6373 2d6d 6174  dfunk/mkdocs-mat
+00000af0: 6572 6961 6c29 2061 6e64 205b 6072 6561  erial) and [`rea
+00000b00: 6474 6865 646f 6373 605d 2868 7474 7073  dthedocs`](https
+00000b10: 3a2f 2f77 7777 2e6d 6b64 6f63 732e 6f72  ://www.mkdocs.or
+00000b20: 672f 7573 6572 2d67 7569 6465 2f63 686f  g/user-guide/cho
+00000b30: 6f73 696e 672d 796f 7572 2d74 6865 6d65  osing-your-theme
+00000b40: 2f23 7265 6164 7468 6564 6f63 7329 2074  /#readthedocs) t
+00000b50: 6865 6d65 730a 2020 2020 2d20 4368 6563  hemes.    - Chec
+00000b60: 6b20 6f75 7420 736f 6d65 2073 616d 706c  k out some sampl
+00000b70: 6520 5044 4620 646f 6375 6d65 6e74 7320  e PDF documents 
+00000b80: 5b68 6572 655d 282e 2f65 7861 6d70 6c65  [here](./example
+00000b90: 732f 7468 656d 6573 290a 2d20 e2ad 9020  s/themes).- ... 
+00000ba0: 2a2a 506f 7765 7266 756c 2a2a 202d 2069  **Powerful** - i
+00000bb0: 7420 7573 6573 2061 2068 6561 646c 6573  t uses a headles
+00000bc0: 7320 6272 6f77 7365 7220 616e 6420 736f  s browser and so
+00000bd0: 6d65 2061 7765 736f 6d65 206c 6962 7261  me awesome libra
+00000be0: 7269 6573 2075 6e64 6572 2074 6865 2068  ries under the h
+00000bf0: 6f6f 6420 746f 2067 656e 6572 6174 6520  ood to generate 
+00000c00: 5044 4620 6669 6c65 730a 2020 2d20 5b2a  PDF files.  - [*
+00000c10: 506c 6179 7772 6967 6874 2a5d 2868 7474  Playwright*](htt
+00000c20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000c30: 6d69 6372 6f73 6f66 742f 706c 6179 7772  microsoft/playwr
+00000c40: 6967 6874 2d70 7974 686f 6e29 2074 6f20  ight-python) to 
+00000c50: 6175 746f 6d61 7465 2062 726f 7773 6572  automate browser
+00000c60: 730a 2020 2d20 5b2a 5061 6765 642e 6a73  s.  - [*Paged.js
+00000c70: 2a5d 2868 7474 7073 3a2f 2f67 6974 6875  *](https://githu
+00000c80: 622e 636f 6d2f 7061 6765 646a 732f 7061  b.com/pagedjs/pa
+00000c90: 6765 646a 7329 2070 6f6c 7966 696c 6c73  gedjs) polyfills
+00000ca0: 2061 7265 2069 6e63 6c75 6465 6420 285b   are included ([
+00000cb0: 5061 6765 6420 4d65 6469 615d 2868 7474  Paged Media](htt
+00000cc0: 7073 3a2f 2f77 7777 2e77 332e 6f72 672f  ps://www.w3.org/
+00000cd0: 5452 2f63 7373 2d70 6167 652d 332f 2920  TR/css-page-3/) 
+00000ce0: 616e 6420 5b47 656e 6572 6174 6564 2043  and [Generated C
+00000cf0: 6f6e 7465 6e74 5d28 6874 7470 733a 2f2f  ontent](https://
+00000d00: 7777 772e 7733 2e6f 7267 2f54 522f 6373  www.w3.org/TR/cs
+00000d10: 732d 6763 706d 2d33 2f29 2043 5353 206d  s-gcpm-3/) CSS m
+00000d20: 6f64 756c 6573 290a 2020 2d20 5b2a 5361  odules).  - [*Sa
+00000d30: 7373 2a5d 2868 7474 7073 3a2f 2f73 6173  ss*](https://sas
+00000d40: 732d 6c61 6e67 2e63 6f6d 2f29 2073 7570  s-lang.com/) sup
+00000d50: 706f 7274 2028 7669 6120 5b60 6c69 6273  port (via [`libs
+00000d60: 6173 7360 5d28 6874 7470 733a 2f2f 6769  ass`](https://gi
+00000d70: 7468 7562 2e63 6f6d 2f73 6173 732f 6c69  thub.com/sass/li
+00000d80: 6273 6173 732d 7079 7468 6f6e 2929 2066  bsass-python)) f
+00000d90: 6f72 2079 6f75 7220 7374 796c 6573 6865  or your styleshe
+00000da0: 6574 730a 0a23 2320 5072 6572 6571 7569  ets..## Prerequi
+00000db0: 7369 7465 730a 0a2d 2050 7974 686f 6e20  sites..- Python 
+00000dc0: 603e 3d20 332e 3760 0a2d 204d 6b44 6f63  `>= 3.7`.- MkDoc
+00000dd0: 7320 603e 3d20 312e 3460 0a0a 2323 2049  s `>= 1.4`..## I
+00000de0: 6e73 7461 6c6c 6174 696f 6e0a 0a54 6865  nstallation..The
+00000df0: 2070 6c75 6769 6e20 6973 2068 6f73 7465   plugin is hoste
+00000e00: 6420 6f6e 205b 2a50 7950 492a 5d28 6874  d on [*PyPI*](ht
+00000e10: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000e20: 726f 6a65 6374 2f6d 6b64 6f63 732d 6578  roject/mkdocs-ex
+00000e30: 706f 7274 6572 2f29 2061 6e64 2063 616e  porter/) and can
+00000e40: 2062 6520 696e 7374 616c 6c65 6420 7669   be installed vi
+00000e50: 6120 6070 6970 6020 286f 7220 796f 7572  a `pip` (or your
+00000e60: 2066 6176 6f75 7269 7465 2070 6163 6b61   favourite packa
+00000e70: 6765 206d 616e 6167 6572 293a 0a0a 6060  ge manager):..``
+00000e80: 6062 6173 680a 7069 7020 696e 7374 616c  `bash.pip instal
+00000e90: 6c20 6d6b 646f 6373 2d65 7870 6f72 7465  l mkdocs-exporte
+00000ea0: 720a 6060 600a 0a23 2320 5573 6167 650a  r.```..## Usage.
+00000eb0: 0a54 6872 6565 2070 6c75 6769 6e73 2061  .Three plugins a
+00000ec0: 7265 2063 7572 7265 6e74 6c79 2061 7661  re currently ava
+00000ed0: 696c 6162 6c65 3a0a 0a2d 2060 6d6b 646f  ilable:..- `mkdo
+00000ee0: 6373 2f65 7870 6f72 7465 7260 2028 2a72  cs/exporter` (*r
+00000ef0: 6571 7569 7265 642a 293a 2062 6173 6520  equired*): base 
+00000f00: 706c 7567 696e 2077 6869 6368 206d 7573  plugin which mus
+00000f10: 7420 7072 6563 6564 6520 7468 6520 6f74  t precede the ot
+00000f20: 6865 7273 0a2d 2060 6d6b 646f 6373 2f65  hers.- `mkdocs/e
+00000f30: 7870 6f72 7465 722f 7064 6660 2028 2a6f  xporter/pdf` (*o
+00000f40: 7074 696f 6e61 6c2a 293a 2070 6c75 6769  ptional*): plugi
+00000f50: 6e20 7468 6174 2065 7870 6f72 7473 2079  n that exports y
+00000f60: 6f75 7220 7061 6765 7320 6173 2069 6e64  our pages as ind
+00000f70: 6976 6964 7561 6c20 5044 4620 646f 6375  ividual PDF docu
+00000f80: 6d65 6e74 730a 2d20 606d 6b64 6f63 732f  ments.- `mkdocs/
+00000f90: 6578 706f 7274 6572 2f65 7874 7261 7360  exporter/extras`
+00000fa0: 2028 2a6f 7074 696f 6e61 6c2a 293a 2070   (*optional*): p
+00000fb0: 726f 7669 6465 7320 6578 7472 6120 6675  rovides extra fu
+00000fc0: 6e63 7469 6f6e 616c 6974 6965 7320 2862  nctionalities (b
+00000fd0: 7574 746f 6e73 2c20 4854 4d4c 2075 7469  uttons, HTML uti
+00000fe0: 6c69 7469 6573 2e2e 2e29 0a0a 2323 2320  lities...)..### 
+00000ff0: 4578 616d 706c 650a 0a54 6865 2066 6f6c  Example..The fol
+00001000: 6c6f 7769 6e67 2063 6f6e 6669 6775 7261  lowing configura
+00001010: 7469 6f6e 2065 7863 6572 7074 2066 726f  tion excerpt fro
+00001020: 6d20 606d 6b64 6f63 732e 796d 6c60 2073  m `mkdocs.yml` s
+00001030: 686f 756c 6420 636f 7665 7220 7468 6520  hould cover the 
+00001040: 6261 7369 6320 6675 6e63 7469 6f6e 616c  basic functional
+00001050: 6974 6965 7320 6f66 2074 6869 7320 706c  ities of this pl
+00001060: 7567 696e 3a0a 0a60 6060 7961 6d6c 0a70  ugin:..```yaml.p
+00001070: 6c75 6769 6e73 3a0a 2020 2d20 6d6b 646f  lugins:.  - mkdo
+00001080: 6373 2f65 7870 6f72 7465 720a 2020 2d20  cs/exporter.  - 
+00001090: 6d6b 646f 6373 2f65 7870 6f72 7465 722f  mkdocs/exporter/
+000010a0: 7064 663a 0a20 2020 2020 2063 6f6e 6375  pdf:.      concu
+000010b0: 7272 656e 6379 3a20 380a 2020 2020 2020  rrency: 8.      
+000010c0: 636f 7665 7273 3a0a 2020 2020 2020 2020  covers:.        
+000010d0: 6672 6f6e 743a 2072 6573 6f75 7263 6573  front: resources
+000010e0: 2f74 656d 706c 6174 6573 2f63 6f76 6572  /templates/cover
+000010f0: 732f 6672 6f6e 742e 6874 6d6c 2e6a 320a  s/front.html.j2.
+00001100: 2020 2020 2020 2020 6261 636b 3a20 7265          back: re
+00001110: 736f 7572 6365 732f 7465 6d70 6c61 7465  sources/template
+00001120: 732f 636f 7665 7273 2f62 6163 6b2e 6874  s/covers/back.ht
+00001130: 6d6c 2e6a 320a 2020 2020 2020 7374 796c  ml.j2.      styl
+00001140: 6573 6865 6574 733a 0a20 2020 2020 2020  esheets:.       
+00001150: 202d 2072 6573 6f75 7263 6573 2f73 7479   - resources/sty
+00001160: 6c65 7368 6565 7473 2f70 6466 2e73 6373  lesheets/pdf.scs
+00001170: 730a 2020 2d20 6d6b 646f 6373 2f65 7870  s.  - mkdocs/exp
+00001180: 6f72 7465 722f 6578 7472 6173 3a0a 2020  orter/extras:.  
+00001190: 2020 2020 6275 7474 6f6e 733a 0a20 2020      buttons:.   
+000011a0: 2020 2020 202d 2074 6974 6c65 3a20 446f       - title: Do
+000011b0: 776e 6c6f 6164 2061 7320 5044 460a 2020  wnload as PDF.  
+000011c0: 2020 2020 2020 2020 656e 6162 6c65 643a          enabled:
+000011d0: 2021 2170 7974 686f 6e2f 6e61 6d65 3a6d   !!python/name:m
+000011e0: 6b64 6f63 735f 6578 706f 7274 6572 2e70  kdocs_exporter.p
+000011f0: 6c75 6769 6e73 2e70 6466 2e62 7574 746f  lugins.pdf.butto
+00001200: 6e2e 656e 6162 6c65 640a 2020 2020 2020  n.enabled.      
+00001210: 2020 2020 6963 6f6e 3a20 2121 7079 7468      icon: !!pyth
+00001220: 6f6e 2f6e 616d 653a 6d6b 646f 6373 5f65  on/name:mkdocs_e
+00001230: 7870 6f72 7465 722e 706c 7567 696e 732e  xporter.plugins.
+00001240: 7064 662e 6275 7474 6f6e 2e69 636f 6e0a  pdf.button.icon.
+00001250: 2020 2020 2020 2020 2020 6174 7472 6962            attrib
+00001260: 7574 6573 3a0a 2020 2020 2020 2020 2020  utes:.          
+00001270: 2020 6872 6566 3a20 2121 7079 7468 6f6e    href: !!python
+00001280: 2f6e 616d 653a 6d6b 646f 6373 5f65 7870  /name:mkdocs_exp
+00001290: 6f72 7465 722e 706c 7567 696e 732e 7064  orter.plugins.pd
+000012a0: 662e 6275 7474 6f6e 2e68 7265 660a 2020  f.button.href.  
+000012b0: 2020 2020 2020 2020 2020 646f 776e 6c6f            downlo
+000012c0: 6164 3a20 2121 7079 7468 6f6e 2f6e 616d  ad: !!python/nam
+000012d0: 653a 6d6b 646f 6373 5f65 7870 6f72 7465  e:mkdocs_exporte
+000012e0: 722e 706c 7567 696e 732e 7064 662e 6275  r.plugins.pdf.bu
+000012f0: 7474 6f6e 2e64 6f77 6e6c 6f61 640a 6060  tton.download.``
+00001300: 600a 0a43 6865 636b 206f 7574 2061 205b  `..Check out a [
+00001310: 7361 6d70 6c65 2050 4446 2067 656e 6572  sample PDF gener
+00001320: 6174 6564 2062 7920 7468 6973 2070 6c75  ated by this plu
+00001330: 6769 6e5d 2865 7861 6d70 6c65 732f 6578  gin](examples/ex
+00001340: 616d 706c 652e 7064 6629 2066 726f 6d20  ample.pdf) from 
+00001350: 7468 6520 6465 6661 756c 7420 7061 6765  the default page
+00001360: 206f 6620 7468 6520 5b4d 6174 6572 6961   of the [Materia
+00001370: 6c20 666f 7220 4d6b 446f 6373 5d28 6874  l for MkDocs](ht
+00001380: 7470 733a 2f2f 7371 7569 6466 756e 6b2e  tps://squidfunk.
+00001390: 6769 7468 7562 2e69 6f2f 6d6b 646f 6373  github.io/mkdocs
+000013a0: 2d6d 6174 6572 6961 6c29 2074 6865 6d65  -material) theme
+000013b0: 2e20 200a 4974 2068 6173 2062 6565 6e20  .  .It has been 
+000013c0: 6275 696c 7420 7769 7468 2073 6f6d 6520  built with some 
+000013d0: 6375 7374 6f6d 2043 5353 2061 6e64 2066  custom CSS and f
+000013e0: 6561 7475 7265 7320 636f 7665 7220 7061  eatures cover pa
+000013f0: 6765 732e 0a0a 2323 2052 6f61 646d 6170  ges...## Roadmap
+00001400: 0a0a 2d20 436f 6d62 696e 6520 616c 6c20  ..- Combine all 
+00001410: 7061 6765 7320 6173 206f 6e65 2050 4446  pages as one PDF
+00001420: 0a0a 4665 656c 2066 7265 6520 746f 2072  ..Feel free to r
+00001430: 6571 7565 7374 2061 6464 6974 696f 6e61  equest additiona
+00001440: 6c20 6665 6174 7572 6573 2062 7920 7375  l features by su
+00001450: 626d 6974 7469 6e67 2061 6e20 6973 7375  bmitting an issu
+00001460: 6520 6f72 2062 7920 636f 6e74 7269 6275  e or by contribu
+00001470: 7469 6e67 2074 6872 6f75 6768 2061 2070  ting through a p
+00001480: 756c 6c20 7265 7175 6573 742e 0a0a 2323  ull request...##
+00001490: 204c 6963 656e 7365 0a0a 5468 6973 2070   License..This p
+000014a0: 726f 6a65 6374 2069 7320 6c69 6365 6e73  roject is licens
+000014b0: 6564 2075 6e64 6572 2074 6865 2060 4d49  ed under the `MI
+000014c0: 5420 4c69 6365 6e73 6520 284d 4954 2960  T License (MIT)`
+000014d0: 2c20 7768 6963 6820 796f 7520 6361 6e20  , which you can 
+000014e0: 7265 6164 205b 6865 7265 5d28 4c49 4345  read [here](LICE
+000014f0: 4e53 4529 2e0a 0a                        NSE)...
```

