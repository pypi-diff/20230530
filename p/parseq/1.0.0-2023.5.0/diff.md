# Comparing `tmp/parseq-1.0.0.zip` & `tmp/parseq-2023.5.0.zip`

## zipinfo {}

```diff
@@ -1,161 +1,179 @@
-Zip file size: 2080031 bytes, number of entries: 159
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq.egg-info/
--rw-rw-rw-  2.0 fat     1099 b- defN 20-Nov-24 00:11 parseq-1.0.0/LICENSE
--rw-rw-rw-  2.0 fat     4892 b- defN 23-Apr-04 11:46 parseq-1.0.0/PKG-INFO
--rw-rw-rw-  2.0 fat       42 b- defN 23-Apr-04 11:46 parseq-1.0.0/setup.cfg
--rw-rw-rw-  2.0 fat     3552 b- defN 23-Apr-04 11:44 parseq-1.0.0/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/core/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/gui/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/help/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/third_party/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/utils/
--rw-rw-rw-  2.0 fat      386 b- defN 18-Nov-18 11:39 parseq-1.0.0/parseq/CODERULES.txt
--rw-rw-rw-  2.0 fat     4060 b- defN 23-Mar-10 17:22 parseq-1.0.0/parseq/description.py
--rw-rw-rw-  2.0 fat      133 b- defN 23-Apr-04 11:26 parseq-1.0.0/parseq/version.py
--rw-rw-rw-  2.0 fat      753 b- defN 23-Apr-04 11:34 parseq-1.0.0/parseq/__init__.py
--rw-rw-rw-  2.0 fat     7916 b- defN 23-Mar-30 17:09 parseq-1.0.0/parseq/core/commons.py
--rw-rw-rw-  2.0 fat     2273 b- defN 23-Mar-04 22:10 parseq-1.0.0/parseq/core/config.py
--rw-rw-rw-  2.0 fat     1251 b- defN 23-Feb-18 18:40 parseq-1.0.0/parseq/core/logger.py
--rw-rw-rw-  2.0 fat    10207 b- defN 23-Feb-18 16:09 parseq-1.0.0/parseq/core/nodes.py
--rw-rw-rw-  2.0 fat     9375 b- defN 23-Mar-31 09:38 parseq-1.0.0/parseq/core/plotExport.py
--rw-rw-rw-  2.0 fat    14578 b- defN 23-Mar-30 17:18 parseq-1.0.0/parseq/core/save_restore.py
--rw-rw-rw-  2.0 fat     1283 b- defN 22-Sep-29 10:38 parseq-1.0.0/parseq/core/singletons.py
--rw-rw-rw-  2.0 fat    64902 b- defN 23-Mar-24 21:58 parseq-1.0.0/parseq/core/spectra.py
--rw-rw-rw-  2.0 fat    28758 b- defN 23-Mar-21 23:40 parseq-1.0.0/parseq/core/transforms.py
--rw-rw-rw-  2.0 fat     6768 b- defN 23-Mar-22 14:39 parseq-1.0.0/parseq/core/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/gui/_images/
--rw-rw-rw-  2.0 fat    13767 b- defN 23-Mar-10 12:26 parseq-1.0.0/parseq/gui/aboutDialog.py
--rw-rw-rw-  2.0 fat     9545 b- defN 22-Dec-16 16:01 parseq-1.0.0/parseq/gui/calibrateEnergy.py
--rw-rw-rw-  2.0 fat    17918 b- defN 23-Mar-28 10:46 parseq-1.0.0/parseq/gui/columnFormat.py
--rw-rw-rw-  2.0 fat     5605 b- defN 23-Mar-22 18:09 parseq-1.0.0/parseq/gui/combineSpectra.py
--rw-rw-rw-  2.0 fat    19562 b- defN 23-Mar-22 11:21 parseq-1.0.0/parseq/gui/dataRebin.py
--rw-rw-rw-  2.0 fat    50421 b- defN 23-Mar-28 11:15 parseq-1.0.0/parseq/gui/dataTreeModelView.py
--rw-rw-rw-  2.0 fat     9237 b- defN 23-Mar-21 10:07 parseq-1.0.0/parseq/gui/fileDialogs.py
--rw-rw-rw-  2.0 fat    64255 b- defN 23-Apr-04 11:33 parseq-1.0.0/parseq/gui/fileTreeModelView.py
--rw-rw-rw-  2.0 fat    14406 b- defN 23-Feb-26 10:40 parseq-1.0.0/parseq/gui/gcommons.py
--rw-rw-rw-  2.0 fat    33439 b- defN 23-Apr-01 23:55 parseq-1.0.0/parseq/gui/mainWindow.py
--rw-rw-rw-  2.0 fat    48129 b- defN 23-Apr-02 00:27 parseq-1.0.0/parseq/gui/nodeWidget.py
--rw-rw-rw-  2.0 fat     3663 b- defN 23-Jan-03 15:01 parseq-1.0.0/parseq/gui/plot.py
--rw-rw-rw-  2.0 fat    25381 b- defN 23-Mar-15 15:16 parseq-1.0.0/parseq/gui/plotOptions.py
--rw-rw-rw-  2.0 fat     9346 b- defN 23-Mar-01 12:11 parseq-1.0.0/parseq/gui/propsOfData.py
--rw-rw-rw-  2.0 fat    36335 b- defN 23-Mar-28 11:01 parseq-1.0.0/parseq/gui/propWidget.py
--rw-rw-rw-  2.0 fat    46665 b- defN 23-Mar-21 10:53 parseq-1.0.0/parseq/gui/roi.py
--rw-rw-rw-  2.0 fat     1636 b- defN 23-Feb-10 23:36 parseq-1.0.0/parseq/gui/transformer.py
--rw-rw-rw-  2.0 fat     4937 b- defN 22-Oct-14 12:12 parseq-1.0.0/parseq/gui/undoredo.py
--rw-rw-rw-  2.0 fat     9649 b- defN 23-Apr-01 16:25 parseq-1.0.0/parseq/gui/webWidget.py
--rw-rw-rw-  2.0 fat     6799 b- defN 23-Mar-26 11:57 parseq-1.0.0/parseq/gui/__init__.py
--rw-rw-rw-  2.0 fat     5831 b- defN 21-Apr-21 15:48 parseq-1.0.0/parseq/gui/_images/icon-help.png
--rw-rw-rw-  2.0 fat     5473 b- defN 21-Apr-21 15:48 parseq-1.0.0/parseq/gui/_images/icon-info.png
--rw-rw-rw-  2.0 fat     1340 b- defN 21-May-13 14:48 parseq-1.0.0/parseq/gui/_images/icon-item-1dim-32.png
--rw-rw-rw-  2.0 fat     2414 b- defN 22-Jun-02 12:07 parseq-1.0.0/parseq/gui/_images/icon-item-1dim-64.png
--rw-rw-rw-  2.0 fat     1244 b- defN 22-Jul-20 22:55 parseq-1.0.0/parseq/gui/_images/icon-item-1dim-busy-32.png
--rw-rw-rw-  2.0 fat     2221 b- defN 22-Jul-20 22:55 parseq-1.0.0/parseq/gui/_images/icon-item-1dim-busy-64.png
--rw-rw-rw-  2.0 fat      461 b- defN 21-May-13 14:39 parseq-1.0.0/parseq/gui/_images/icon-item-2dim-32.png
--rw-rw-rw-  2.0 fat      582 b- defN 22-Jun-02 12:09 parseq-1.0.0/parseq/gui/_images/icon-item-2dim-64.png
--rw-rw-rw-  2.0 fat      452 b- defN 22-Jul-20 22:56 parseq-1.0.0/parseq/gui/_images/icon-item-2dim-busy-32.png
--rw-rw-rw-  2.0 fat      557 b- defN 22-Jul-20 22:56 parseq-1.0.0/parseq/gui/_images/icon-item-2dim-busy-64.png
--rw-rw-rw-  2.0 fat     1441 b- defN 21-May-13 14:39 parseq-1.0.0/parseq/gui/_images/icon-item-3dim-32.png
--rw-rw-rw-  2.0 fat     2834 b- defN 22-Jun-02 12:10 parseq-1.0.0/parseq/gui/_images/icon-item-3dim-64.png
--rw-rw-rw-  2.0 fat     1347 b- defN 22-Jul-20 22:57 parseq-1.0.0/parseq/gui/_images/icon-item-3dim-busy-32.png
--rw-rw-rw-  2.0 fat     2673 b- defN 22-Jul-20 22:57 parseq-1.0.0/parseq/gui/_images/icon-item-3dim-busy-64.png
--rw-rw-rw-  2.0 fat     2164 b- defN 22-Jul-21 12:50 parseq-1.0.0/parseq/gui/_images/icon-item-ndim-32.png
--rw-rw-rw-  2.0 fat     4780 b- defN 22-Jul-21 12:50 parseq-1.0.0/parseq/gui/_images/icon-item-ndim-64.png
--rw-rw-rw-  2.0 fat     2005 b- defN 22-Jul-21 12:50 parseq-1.0.0/parseq/gui/_images/icon-item-ndim-busy-32.png
--rw-rw-rw-  2.0 fat     4515 b- defN 22-Jul-21 12:51 parseq-1.0.0/parseq/gui/_images/icon-item-ndim-busy-64.png
--rw-rw-rw-  2.0 fat     5529 b- defN 21-Apr-22 22:43 parseq-1.0.0/parseq/gui/_images/icon-load-proj.png
--rw-rw-rw-  2.0 fat     3575 b- defN 21-Apr-21 15:56 parseq-1.0.0/parseq/gui/_images/icon-redo.png
--rw-rw-rw-  2.0 fat     5462 b- defN 21-Apr-22 22:44 parseq-1.0.0/parseq/gui/_images/icon-save-proj.png
--rw-rw-rw-  2.0 fat     4662 b- defN 21-Apr-22 22:44 parseq-1.0.0/parseq/gui/_images/icon-save-text.png
--rw-rw-rw-  2.0 fat     3625 b- defN 21-Apr-21 15:56 parseq-1.0.0/parseq/gui/_images/icon-undo.png
--rw-rw-rw-  2.0 fat    67646 b- defN 17-Aug-08 13:54 parseq-1.0.0/parseq/gui/_images/parseq.ico
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/help/exts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/help/_images/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/help/_static/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/help/_templates/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/help/_themes/
--rw-rw-rw-  2.0 fat     7052 b- defN 23-Mar-10 09:23 parseq-1.0.0/parseq/help/conf.py
--rw-rw-rw-  2.0 fat     3547 b- defN 22-Sep-30 12:10 parseq-1.0.0/parseq/help/conf_doc.py
--rw-rw-rw-  2.0 fat      173 b- defN 22-Sep-28 19:08 parseq-1.0.0/parseq/help/data.rst
--rw-rw-rw-  2.0 fat       43 b- defN 22-Sep-30 15:27 parseq-1.0.0/parseq/help/howto.rst
--rw-rw-rw-  2.0 fat      392 b- defN 22-Sep-28 19:30 parseq-1.0.0/parseq/help/index.rst
--rw-rw-rw-  2.0 fat     1134 b- defN 22-Sep-28 17:01 parseq-1.0.0/parseq/help/license.rst
--rwx---     2.0 fat     5356 b- defN 16-Aug-10 15:09 parseq-1.0.0/parseq/help/make.bat
--rw-rw-rw-  2.0 fat      141 b- defN 22-Sep-28 19:02 parseq-1.0.0/parseq/help/nodes.rst
--rw-rw-rw-  2.0 fat       45 b- defN 22-Sep-28 19:30 parseq-1.0.0/parseq/help/notesgui.rst
--rw-rw-rw-  2.0 fat      804 b- defN 23-Mar-09 10:03 parseq-1.0.0/parseq/help/top.rst
--rw-rw-rw-  2.0 fat      143 b- defN 22-Sep-28 19:21 parseq-1.0.0/parseq/help/transforms.rst
--rw-rw-rw-  2.0 fat      189 b- defN 23-Jan-23 18:49 parseq-1.0.0/parseq/help/widgets.rst
--rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-1.0.0/parseq/help/__init__.py
--rw-rw-rw-  2.0 fat     8824 b- defN 22-Sep-30 10:44 parseq-1.0.0/parseq/help/exts/animation.py
--rw-rw-rw-  2.0 fat   873847 b- defN 21-Jun-21 17:49 parseq-1.0.0/parseq/help/_images/mickey-rtfm.gif
--rw-rw-rw-  2.0 fat   176184 b- defN 23-Mar-10 17:16 parseq-1.0.0/parseq/help/_images/node1.png
--rw-rw-rw-  2.0 fat    98843 b- defN 23-Mar-10 17:17 parseq-1.0.0/parseq/help/_images/node2.png
--rw-rw-rw-  2.0 fat   187993 b- defN 23-Mar-10 17:17 parseq-1.0.0/parseq/help/_images/node3.png
--rw-rw-rw-  2.0 fat   115965 b- defN 23-Mar-10 17:18 parseq-1.0.0/parseq/help/_images/node4.png
--rw-rw-rw-  2.0 fat    67646 b- defN 17-Aug-08 13:54 parseq-1.0.0/parseq/help/_images/parseq.ico
--rw-rw-rw-  2.0 fat   216689 b- defN 22-Sep-28 15:24 parseq-1.0.0/parseq/help/_images/parseq_big.png
--rw-rw-rw-  2.0 fat    19518 b- defN 19-Mar-15 00:18 parseq-1.0.0/parseq/help/_images/XAS_icon.ico
--rw-rw-rw-  2.0 fat    19518 b- defN 21-Jul-23 18:16 parseq-1.0.0/parseq/help/_images/XES_dispersive_icon.ico
--rw-rw-rw-  2.0 fat    19518 b- defN 21-Jun-18 22:43 parseq-1.0.0/parseq/help/_images/XES_scan_icon.ico
--rw-rw-rw-  2.0 fat     1171 b- defN 16-Aug-16 17:36 parseq-1.0.0/parseq/help/_static/animation.js
--rw-rw-rw-  2.0 fat     1148 b- defN 21-Sep-22 15:17 parseq-1.0.0/parseq/help/_static/thumbnail.css
--rw-rw-rw-  2.0 fat      504 b- defN 22-Sep-28 22:11 parseq-1.0.0/parseq/help/_templates/layout.html
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/help/_themes/mytheme/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/help/_themes/parseq/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/help/_themes/mytheme/static/
--rw-rw-rw-  2.0 fat      384 b- defN 18-Jun-28 10:33 parseq-1.0.0/parseq/help/_themes/mytheme/layout.html
--rw-rw-rw-  2.0 fat       74 b- defN 23-Mar-03 12:15 parseq-1.0.0/parseq/help/_themes/mytheme/theme.conf
--rw-rw-rw-  2.0 fat     4514 b- defN 23-Apr-02 12:36 parseq-1.0.0/parseq/help/_themes/mytheme/static/mycss.css_t
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/help/_themes/parseq/static/
--rw-rw-rw-  2.0 fat      868 b- defN 21-Jun-20 14:53 parseq-1.0.0/parseq/help/_themes/parseq/layout.html
--rw-rw-rw-  2.0 fat      525 b- defN 18-Aug-13 16:19 parseq-1.0.0/parseq/help/_themes/parseq/page.html
--rw-rw-rw-  2.0 fat      721 b- defN 18-Aug-13 16:19 parseq-1.0.0/parseq/help/_themes/parseq/theme.conf
--rw-rw-rw-  2.0 fat     7732 b- defN 23-Apr-02 12:36 parseq-1.0.0/parseq/help/_themes/parseq/static/default.css_t
--rw-rw-rw-  2.0 fat      488 b- defN 18-Aug-13 16:19 parseq-1.0.0/parseq/help/_themes/parseq/static/math_config_win32.js
--rw-rw-rw-  2.0 fat     2243 b- defN 22-Jan-28 15:42 parseq-1.0.0/parseq/help/_themes/parseq/static/utils.js
--rw-rw-rw-  2.0 fat    69161 b- defN 22-Nov-02 17:20 parseq-1.0.0/parseq/tests/circles-rect.png
--rw-rw-rw-  2.0 fat    33688 b- defN 22-Aug-01 18:50 parseq-1.0.0/parseq/tests/circles.png
--rw-rw-rw-  2.0 fat    21073 b- defN 21-Aug-09 10:56 parseq-1.0.0/parseq/tests/modeltest.py
--rw-rw-rw-  2.0 fat      503 b- defN 22-Aug-27 11:17 parseq-1.0.0/parseq/tests/test_aboutWidget.py
--rw-rw-rw-  2.0 fat      841 b- defN 22-Aug-27 11:15 parseq-1.0.0/parseq/tests/test_calibrateEnergyWidget.py
--rw-rw-rw-  2.0 fat     1570 b- defN 22-Jul-13 15:11 parseq-1.0.0/parseq/tests/test_columnStrings.py
--rw-rw-rw-  2.0 fat      592 b- defN 22-Aug-27 11:16 parseq-1.0.0/parseq/tests/test_combineSpectraWidget.py
--rw-rw-rw-  2.0 fat     1027 b- defN 23-Feb-12 19:15 parseq-1.0.0/parseq/tests/test_commons.py
--rw-rw-rw-  2.0 fat     1859 b- defN 22-Aug-02 14:07 parseq-1.0.0/parseq/tests/test_curve_shear.py
--rw-rw-rw-  2.0 fat     2339 b- defN 23-Jan-24 14:23 parseq-1.0.0/parseq/tests/test_dataRebinWidget.py
--rw-rw-rw-  2.0 fat     2641 b- defN 22-Aug-27 11:16 parseq-1.0.0/parseq/tests/test_dataTreeModelView.py
--rw-rw-rw-  2.0 fat      646 b- defN 22-Aug-27 11:15 parseq-1.0.0/parseq/tests/test_fileDialog.py
--rw-rw-rw-  2.0 fat     1612 b- defN 22-Jul-15 10:53 parseq-1.0.0/parseq/tests/test_fileTreeModelView.py
--rw-rw-rw-  2.0 fat      760 b- defN 22-Apr-15 08:28 parseq-1.0.0/parseq/tests/test_flowLayout.py
--rw-rw-rw-  2.0 fat     2302 b- defN 22-Jul-13 15:37 parseq-1.0.0/parseq/tests/test_hdf5.py
--rw-rw-rw-  2.0 fat     1300 b- defN 22-Aug-27 11:17 parseq-1.0.0/parseq/tests/test_mainWindow.py
--rw-rw-rw-  2.0 fat     1160 b- defN 22-Sep-24 11:41 parseq-1.0.0/parseq/tests/test_node.py
--rw-rw-rw-  2.0 fat      817 b- defN 22-Aug-27 11:15 parseq-1.0.0/parseq/tests/test_nodeWidget.py
--rw-rw-rw-  2.0 fat     2649 b- defN 22-Nov-18 11:49 parseq-1.0.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py
--rw-rw-rw-  2.0 fat     2762 b- defN 22-Aug-20 22:24 parseq-1.0.0/parseq/tests/test_plotInteractiveImageSingleROI.py
--rw-rw-rw-  2.0 fat     1060 b- defN 22-Aug-27 11:15 parseq-1.0.0/parseq/tests/test_plotOptions.py
--rw-rw-rw-  2.0 fat     1485 b- defN 22-Jul-23 17:28 parseq-1.0.0/parseq/tests/test_QSortFilterProxyModel.py
--rw-rw-rw-  2.0 fat     1248 b- defN 21-Aug-09 10:56 parseq-1.0.0/parseq/tests/test_ROI.py
--rw-rw-rw-  2.0 fat     1028 b- defN 21-Aug-09 10:56 parseq-1.0.0/parseq/tests/test_slice.py
--rw-rw-rw-  2.0 fat      572 b- defN 23-Feb-24 09:56 parseq-1.0.0/parseq/tests/test_stateButtons.py
--rw-rw-rw-  2.0 fat      218 b- defN 22-Aug-27 11:17 parseq-1.0.0/parseq/tests/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-04 11:46 parseq-1.0.0/parseq/third_party/data/
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-03 20:36 parseq-1.0.0/parseq/third_party/XAFSmass.py
--rw-rw-rw-  2.0 fat      732 b- defN 22-Aug-28 12:11 parseq-1.0.0/parseq/third_party/xrt.py
--rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-1.0.0/parseq/third_party/__init__.py
--rw-rw-rw-  2.0 fat     7812 b- defN 17-Aug-04 10:49 parseq-1.0.0/parseq/third_party/data/Energies.txt
--rw-rw-rw-  2.0 fat      345 b- defN 22-Mar-31 11:43 parseq-1.0.0/parseq/utils/format.py
--rw-rw-rw-  2.0 fat     2009 b- defN 23-Mar-06 14:40 parseq-1.0.0/parseq/utils/ft.py
--rw-rw-rw-  2.0 fat     1660 b- defN 23-Mar-20 16:04 parseq-1.0.0/parseq/utils/h5reduce.py
--rw-rw-rw-  2.0 fat     3873 b- defN 23-Feb-28 17:40 parseq-1.0.0/parseq/utils/math.py
--rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-1.0.0/parseq/utils/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-04 11:46 parseq-1.0.0/parseq.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-04 11:40 parseq-1.0.0/parseq.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat     4892 b- defN 23-Apr-04 11:46 parseq-1.0.0/parseq.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      140 b- defN 23-Apr-04 11:46 parseq-1.0.0/parseq.egg-info/requires.txt
--rw-rw-rw-  2.0 fat     4451 b- defN 23-Apr-04 11:46 parseq-1.0.0/parseq.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-04 11:46 parseq-1.0.0/parseq.egg-info/top_level.txt
-159 files, 2751605 bytes uncompressed, 2054755 bytes compressed:  25.3%
+Zip file size: 2245699 bytes, number of entries: 177
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/
+-rw-rw-rw-  2.0 fat     1099 b- defN 20-Nov-24 00:11 parseq-2023.5.0/LICENSE
+-rw-rw-rw-  2.0 fat     5037 b- defN 23-May-30 17:00 parseq-2023.5.0/PKG-INFO
+-rw-rw-rw-  2.0 fat       42 b- defN 23-May-30 17:00 parseq-2023.5.0/setup.cfg
+-rw-rw-rw-  2.0 fat     3613 b- defN 23-May-30 16:48 parseq-2023.5.0/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/core/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/fits/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/gui/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/tests/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/third_party/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/utils/
+-rw-rw-rw-  2.0 fat      386 b- defN 18-Nov-18 11:39 parseq-2023.5.0/parseq/CODERULES.txt
+-rw-rw-rw-  2.0 fat     4202 b- defN 23-May-29 10:53 parseq-2023.5.0/parseq/description.py
+-rw-rw-rw-  2.0 fat      137 b- defN 23-May-30 16:51 parseq-2023.5.0/parseq/version.py
+-rw-rw-rw-  2.0 fat      753 b- defN 23-Apr-04 11:34 parseq-2023.5.0/parseq/__init__.py
+-rw-rw-rw-  2.0 fat     7916 b- defN 23-Mar-30 17:09 parseq-2023.5.0/parseq/core/commons.py
+-rw-rw-rw-  2.0 fat     2546 b- defN 23-May-08 15:31 parseq-2023.5.0/parseq/core/config.py
+-rw-rw-rw-  2.0 fat     1251 b- defN 23-Feb-18 18:40 parseq-2023.5.0/parseq/core/logger.py
+-rw-rw-rw-  2.0 fat    10207 b- defN 23-Feb-18 16:09 parseq-2023.5.0/parseq/core/nodes.py
+-rw-rw-rw-  2.0 fat     9439 b- defN 23-May-10 23:46 parseq-2023.5.0/parseq/core/plotExport.py
+-rw-rw-rw-  2.0 fat    15090 b- defN 23-May-10 16:47 parseq-2023.5.0/parseq/core/save_restore.py
+-rw-rw-rw-  2.0 fat     1295 b- defN 23-May-08 16:03 parseq-2023.5.0/parseq/core/singletons.py
+-rw-rw-rw-  2.0 fat    67284 b- defN 23-May-29 21:45 parseq-2023.5.0/parseq/core/spectra.py
+-rw-rw-rw-  2.0 fat    28882 b- defN 23-May-30 16:09 parseq-2023.5.0/parseq/core/transforms.py
+-rw-rw-rw-  2.0 fat     7290 b- defN 23-May-30 10:44 parseq-2023.5.0/parseq/core/__init__.py
+-rw-rw-rw-  2.0 fat    23452 b- defN 23-May-30 16:02 parseq-2023.5.0/parseq/fits/basefit.py
+-rw-rw-rw-  2.0 fat     6018 b- defN 23-May-30 14:50 parseq-2023.5.0/parseq/fits/functionfit.py
+-rw-rw-rw-  2.0 fat    11104 b- defN 23-May-29 17:27 parseq-2023.5.0/parseq/fits/lcf.py
+-rw-rw-rw-  2.0 fat       57 b- defN 23-May-30 16:39 parseq-2023.5.0/parseq/fits/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/gui/fits/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/gui/_images/
+-rw-rw-rw-  2.0 fat    14810 b- defN 23-May-28 23:01 parseq-2023.5.0/parseq/gui/aboutDialog.py
+-rw-rw-rw-  2.0 fat     9545 b- defN 22-Dec-16 16:01 parseq-2023.5.0/parseq/gui/calibrateEnergy.py
+-rw-rw-rw-  2.0 fat    17918 b- defN 23-Mar-28 10:46 parseq-2023.5.0/parseq/gui/columnFormat.py
+-rw-rw-rw-  2.0 fat     5605 b- defN 23-Mar-22 18:09 parseq-2023.5.0/parseq/gui/combineSpectra.py
+-rw-rw-rw-  2.0 fat    18954 b- defN 23-Apr-13 12:04 parseq-2023.5.0/parseq/gui/dataRebin.py
+-rw-rw-rw-  2.0 fat    50740 b- defN 23-May-23 19:59 parseq-2023.5.0/parseq/gui/dataTreeModelView.py
+-rw-rw-rw-  2.0 fat     9343 b- defN 23-May-29 23:05 parseq-2023.5.0/parseq/gui/fileDialogs.py
+-rw-rw-rw-  2.0 fat    64592 b- defN 23-May-08 23:37 parseq-2023.5.0/parseq/gui/fileTreeModelView.py
+-rw-rw-rw-  2.0 fat    17817 b- defN 23-Apr-27 09:30 parseq-2023.5.0/parseq/gui/gcommons.py
+-rw-rw-rw-  2.0 fat    33432 b- defN 23-May-17 13:32 parseq-2023.5.0/parseq/gui/mainWindow.py
+-rw-rw-rw-  2.0 fat    53525 b- defN 23-May-30 11:39 parseq-2023.5.0/parseq/gui/nodeWidget.py
+-rw-rw-rw-  2.0 fat     3663 b- defN 23-Jan-03 15:01 parseq-2023.5.0/parseq/gui/plot.py
+-rw-rw-rw-  2.0 fat    25381 b- defN 23-Mar-15 15:16 parseq-2023.5.0/parseq/gui/plotOptions.py
+-rw-rw-rw-  2.0 fat     9346 b- defN 23-Mar-01 12:11 parseq-2023.5.0/parseq/gui/propsOfData.py
+-rw-rw-rw-  2.0 fat    36606 b- defN 23-May-08 20:39 parseq-2023.5.0/parseq/gui/propWidget.py
+-rw-rw-rw-  2.0 fat    46720 b- defN 23-May-26 21:19 parseq-2023.5.0/parseq/gui/roi.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-May-08 15:59 parseq-2023.5.0/parseq/gui/tasker.py
+-rw-rw-rw-  2.0 fat     4937 b- defN 22-Oct-14 12:12 parseq-2023.5.0/parseq/gui/undoredo.py
+-rw-rw-rw-  2.0 fat     9804 b- defN 23-May-28 22:26 parseq-2023.5.0/parseq/gui/webWidget.py
+-rw-rw-rw-  2.0 fat     7206 b- defN 23-May-30 11:59 parseq-2023.5.0/parseq/gui/__init__.py
+-rw-rw-rw-  2.0 fat     4463 b- defN 23-May-30 16:08 parseq-2023.5.0/parseq/gui/fits/gbasefit.py
+-rw-rw-rw-  2.0 fat    15986 b- defN 23-May-30 14:50 parseq-2023.5.0/parseq/gui/fits/gfunctionfit.py
+-rw-rw-rw-  2.0 fat    19210 b- defN 23-May-29 17:26 parseq-2023.5.0/parseq/gui/fits/glcf.py
+-rw-rw-rw-  2.0 fat       25 b- defN 23-May-30 16:42 parseq-2023.5.0/parseq/gui/fits/__init__.py
+-rw-rw-rw-  2.0 fat     2255 b- defN 23-May-29 00:07 parseq-2023.5.0/parseq/gui/_images/icon-fit-32.png
+-rw-rw-rw-  2.0 fat     4846 b- defN 23-May-29 00:06 parseq-2023.5.0/parseq/gui/_images/icon-fit-64.png
+-rw-rw-rw-  2.0 fat     5831 b- defN 21-Apr-21 15:48 parseq-2023.5.0/parseq/gui/_images/icon-help.png
+-rw-rw-rw-  2.0 fat     5473 b- defN 21-Apr-21 15:48 parseq-2023.5.0/parseq/gui/_images/icon-info.png
+-rw-rw-rw-  2.0 fat     1340 b- defN 21-May-13 14:48 parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-32.png
+-rw-rw-rw-  2.0 fat     2414 b- defN 22-Jun-02 12:07 parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-64.png
+-rw-rw-rw-  2.0 fat     1244 b- defN 22-Jul-20 22:55 parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-32.png
+-rw-rw-rw-  2.0 fat     2221 b- defN 22-Jul-20 22:55 parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-64.png
+-rw-rw-rw-  2.0 fat      461 b- defN 21-May-13 14:39 parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-32.png
+-rw-rw-rw-  2.0 fat      582 b- defN 22-Jun-02 12:09 parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-64.png
+-rw-rw-rw-  2.0 fat      452 b- defN 22-Jul-20 22:56 parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-busy-32.png
+-rw-rw-rw-  2.0 fat      557 b- defN 22-Jul-20 22:56 parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-busy-64.png
+-rw-rw-rw-  2.0 fat     1441 b- defN 21-May-13 14:39 parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-32.png
+-rw-rw-rw-  2.0 fat     2834 b- defN 22-Jun-02 12:10 parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-64.png
+-rw-rw-rw-  2.0 fat     1347 b- defN 22-Jul-20 22:57 parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-32.png
+-rw-rw-rw-  2.0 fat     2673 b- defN 22-Jul-20 22:57 parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-64.png
+-rw-rw-rw-  2.0 fat     2164 b- defN 22-Jul-21 12:50 parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-32.png
+-rw-rw-rw-  2.0 fat     4780 b- defN 22-Jul-21 12:50 parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-64.png
+-rw-rw-rw-  2.0 fat     2005 b- defN 22-Jul-21 12:50 parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-32.png
+-rw-rw-rw-  2.0 fat     4515 b- defN 22-Jul-21 12:51 parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-64.png
+-rw-rw-rw-  2.0 fat     5529 b- defN 21-Apr-22 22:43 parseq-2023.5.0/parseq/gui/_images/icon-load-proj.png
+-rw-rw-rw-  2.0 fat     3575 b- defN 21-Apr-21 15:56 parseq-2023.5.0/parseq/gui/_images/icon-redo.png
+-rw-rw-rw-  2.0 fat     5462 b- defN 21-Apr-22 22:44 parseq-2023.5.0/parseq/gui/_images/icon-save-proj.png
+-rw-rw-rw-  2.0 fat     4662 b- defN 21-Apr-22 22:44 parseq-2023.5.0/parseq/gui/_images/icon-save-text.png
+-rw-rw-rw-  2.0 fat     3625 b- defN 21-Apr-21 15:56 parseq-2023.5.0/parseq/gui/_images/icon-undo.png
+-rw-rw-rw-  2.0 fat    67646 b- defN 17-Aug-08 13:54 parseq-2023.5.0/parseq/gui/_images/parseq.ico
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/exts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_images/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_static/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_templates/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_themes/
+-rw-rw-rw-  2.0 fat     7052 b- defN 23-Mar-10 09:23 parseq-2023.5.0/parseq/help/conf.py
+-rw-rw-rw-  2.0 fat     3547 b- defN 22-Sep-30 12:10 parseq-2023.5.0/parseq/help/conf_doc.py
+-rw-rw-rw-  2.0 fat      173 b- defN 22-Sep-28 19:08 parseq-2023.5.0/parseq/help/data.rst
+-rw-rw-rw-  2.0 fat      222 b- defN 23-May-30 16:09 parseq-2023.5.0/parseq/help/fits.rst
+-rw-rw-rw-  2.0 fat       43 b- defN 22-Sep-30 15:27 parseq-2023.5.0/parseq/help/howto.rst
+-rw-rw-rw-  2.0 fat      405 b- defN 23-May-30 11:34 parseq-2023.5.0/parseq/help/index.rst
+-rw-rw-rw-  2.0 fat     1134 b- defN 22-Sep-28 17:01 parseq-2023.5.0/parseq/help/license.rst
+-rwx---     2.0 fat     5356 b- defN 16-Aug-10 15:09 parseq-2023.5.0/parseq/help/make.bat
+-rw-rw-rw-  2.0 fat      141 b- defN 22-Sep-28 19:02 parseq-2023.5.0/parseq/help/nodes.rst
+-rw-rw-rw-  2.0 fat       45 b- defN 22-Sep-28 19:30 parseq-2023.5.0/parseq/help/notesgui.rst
+-rw-rw-rw-  2.0 fat      804 b- defN 23-Mar-09 10:03 parseq-2023.5.0/parseq/help/top.rst
+-rw-rw-rw-  2.0 fat      143 b- defN 22-Sep-28 19:21 parseq-2023.5.0/parseq/help/transforms.rst
+-rw-rw-rw-  2.0 fat      189 b- defN 23-Jan-23 18:49 parseq-2023.5.0/parseq/help/widgets.rst
+-rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-2023.5.0/parseq/help/__init__.py
+-rw-rw-rw-  2.0 fat     8824 b- defN 22-Sep-30 10:44 parseq-2023.5.0/parseq/help/exts/animation.py
+-rw-rw-rw-  2.0 fat   873847 b- defN 21-Jun-21 17:49 parseq-2023.5.0/parseq/help/_images/mickey-rtfm.gif
+-rw-rw-rw-  2.0 fat   176184 b- defN 23-Mar-10 17:16 parseq-2023.5.0/parseq/help/_images/node1.png
+-rw-rw-rw-  2.0 fat    98843 b- defN 23-Mar-10 17:17 parseq-2023.5.0/parseq/help/_images/node2.png
+-rw-rw-rw-  2.0 fat   187993 b- defN 23-Mar-10 17:17 parseq-2023.5.0/parseq/help/_images/node3.png
+-rw-rw-rw-  2.0 fat   115965 b- defN 23-Mar-10 17:18 parseq-2023.5.0/parseq/help/_images/node4.png
+-rw-rw-rw-  2.0 fat    67646 b- defN 17-Aug-08 13:54 parseq-2023.5.0/parseq/help/_images/parseq.ico
+-rw-rw-rw-  2.0 fat   216689 b- defN 22-Sep-28 15:24 parseq-2023.5.0/parseq/help/_images/parseq_big.png
+-rw-rw-rw-  2.0 fat    19518 b- defN 19-Mar-15 00:18 parseq-2023.5.0/parseq/help/_images/XAS_icon.ico
+-rw-rw-rw-  2.0 fat    19518 b- defN 21-Jul-23 18:16 parseq-2023.5.0/parseq/help/_images/XES_dispersive_icon.ico
+-rw-rw-rw-  2.0 fat    19518 b- defN 21-Jun-18 22:43 parseq-2023.5.0/parseq/help/_images/XES_scan_icon.ico
+-rw-rw-rw-  2.0 fat     1171 b- defN 16-Aug-16 17:36 parseq-2023.5.0/parseq/help/_static/animation.js
+-rw-rw-rw-  2.0 fat     1148 b- defN 21-Sep-22 15:17 parseq-2023.5.0/parseq/help/_static/thumbnail.css
+-rw-rw-rw-  2.0 fat      504 b- defN 22-Sep-28 22:11 parseq-2023.5.0/parseq/help/_templates/layout.html
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_themes/mytheme/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_themes/parseq/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_themes/mytheme/static/
+-rw-rw-rw-  2.0 fat      384 b- defN 18-Jun-28 10:33 parseq-2023.5.0/parseq/help/_themes/mytheme/layout.html
+-rw-rw-rw-  2.0 fat       74 b- defN 23-Mar-03 12:15 parseq-2023.5.0/parseq/help/_themes/mytheme/theme.conf
+-rw-rw-rw-  2.0 fat     4514 b- defN 23-Apr-02 12:36 parseq-2023.5.0/parseq/help/_themes/mytheme/static/mycss.css_t
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/help/_themes/parseq/static/
+-rw-rw-rw-  2.0 fat      868 b- defN 21-Jun-20 14:53 parseq-2023.5.0/parseq/help/_themes/parseq/layout.html
+-rw-rw-rw-  2.0 fat      525 b- defN 18-Aug-13 16:19 parseq-2023.5.0/parseq/help/_themes/parseq/page.html
+-rw-rw-rw-  2.0 fat      721 b- defN 18-Aug-13 16:19 parseq-2023.5.0/parseq/help/_themes/parseq/theme.conf
+-rw-rw-rw-  2.0 fat     8115 b- defN 23-May-28 23:33 parseq-2023.5.0/parseq/help/_themes/parseq/static/default.css_t
+-rw-rw-rw-  2.0 fat      488 b- defN 18-Aug-13 16:19 parseq-2023.5.0/parseq/help/_themes/parseq/static/math_config_win32.js
+-rw-rw-rw-  2.0 fat     2243 b- defN 22-Jan-28 15:42 parseq-2023.5.0/parseq/help/_themes/parseq/static/utils.js
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/tests/data/
+-rw-rw-rw-  2.0 fat    69161 b- defN 22-Nov-02 17:20 parseq-2023.5.0/parseq/tests/circles-rect.png
+-rw-rw-rw-  2.0 fat    33688 b- defN 22-Aug-01 18:50 parseq-2023.5.0/parseq/tests/circles.png
+-rw-rw-rw-  2.0 fat    21073 b- defN 21-Aug-09 10:56 parseq-2023.5.0/parseq/tests/modeltest.py
+-rw-rw-rw-  2.0 fat      503 b- defN 22-Aug-27 11:17 parseq-2023.5.0/parseq/tests/test_aboutWidget.py
+-rw-rw-rw-  2.0 fat      841 b- defN 22-Aug-27 11:15 parseq-2023.5.0/parseq/tests/test_calibrateEnergyWidget.py
+-rw-rw-rw-  2.0 fat     1570 b- defN 22-Jul-13 15:11 parseq-2023.5.0/parseq/tests/test_columnStrings.py
+-rw-rw-rw-  2.0 fat      592 b- defN 22-Aug-27 11:16 parseq-2023.5.0/parseq/tests/test_combineSpectraWidget.py
+-rw-rw-rw-  2.0 fat     1027 b- defN 23-Feb-12 19:15 parseq-2023.5.0/parseq/tests/test_commons.py
+-rw-rw-rw-  2.0 fat     1859 b- defN 22-Aug-02 14:07 parseq-2023.5.0/parseq/tests/test_curve_shear.py
+-rw-rw-rw-  2.0 fat     2339 b- defN 23-Jan-24 14:23 parseq-2023.5.0/parseq/tests/test_dataRebinWidget.py
+-rw-rw-rw-  2.0 fat     2641 b- defN 22-Aug-27 11:16 parseq-2023.5.0/parseq/tests/test_dataTreeModelView.py
+-rw-rw-rw-  2.0 fat      646 b- defN 22-Aug-27 11:15 parseq-2023.5.0/parseq/tests/test_fileDialog.py
+-rw-rw-rw-  2.0 fat     1612 b- defN 22-Jul-15 10:53 parseq-2023.5.0/parseq/tests/test_fileTreeModelView.py
+-rw-rw-rw-  2.0 fat     9805 b- defN 23-May-30 14:47 parseq-2023.5.0/parseq/tests/test_fit.py
+-rw-rw-rw-  2.0 fat      760 b- defN 22-Apr-15 08:28 parseq-2023.5.0/parseq/tests/test_flowLayout.py
+-rw-rw-rw-  2.0 fat     2302 b- defN 22-Jul-13 15:37 parseq-2023.5.0/parseq/tests/test_hdf5.py
+-rw-rw-rw-  2.0 fat     1300 b- defN 22-Aug-27 11:17 parseq-2023.5.0/parseq/tests/test_mainWindow.py
+-rw-rw-rw-  2.0 fat     1160 b- defN 22-Sep-24 11:41 parseq-2023.5.0/parseq/tests/test_node.py
+-rw-rw-rw-  2.0 fat      817 b- defN 22-Aug-27 11:15 parseq-2023.5.0/parseq/tests/test_nodeWidget.py
+-rw-rw-rw-  2.0 fat     2649 b- defN 22-Nov-18 11:49 parseq-2023.5.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py
+-rw-rw-rw-  2.0 fat     2762 b- defN 22-Aug-20 22:24 parseq-2023.5.0/parseq/tests/test_plotInteractiveImageSingleROI.py
+-rw-rw-rw-  2.0 fat     1060 b- defN 22-Aug-27 11:15 parseq-2023.5.0/parseq/tests/test_plotOptions.py
+-rw-rw-rw-  2.0 fat     1485 b- defN 22-Jul-23 17:28 parseq-2023.5.0/parseq/tests/test_QSortFilterProxyModel.py
+-rw-rw-rw-  2.0 fat     1248 b- defN 21-Aug-09 10:56 parseq-2023.5.0/parseq/tests/test_ROI.py
+-rw-rw-rw-  2.0 fat     1028 b- defN 21-Aug-09 10:56 parseq-2023.5.0/parseq/tests/test_slice.py
+-rw-rw-rw-  2.0 fat      572 b- defN 23-Feb-24 09:56 parseq-2023.5.0/parseq/tests/test_stateButtons.py
+-rw-rw-rw-  2.0 fat      218 b- defN 22-Aug-27 11:17 parseq-2023.5.0/parseq/tests/__init__.py
+-rw-rw-rw-  2.0 fat   209750 b- defN 19-Nov-27 14:45 parseq-2023.5.0/parseq/tests/data/cu-ref-mix.res
+-rw-rw-rw-  2.0 fat    77692 b- defN 19-Nov-27 14:47 parseq-2023.5.0/parseq/tests/data/pb-ref-mix.res
+-rw-rw-rw-  2.0 fat   167161 b- defN 19-Nov-27 14:46 parseq-2023.5.0/parseq/tests/data/zn-ref-mix.res
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-30 17:00 parseq-2023.5.0/parseq/third_party/data/
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-03 20:36 parseq-2023.5.0/parseq/third_party/XAFSmass.py
+-rw-rw-rw-  2.0 fat      732 b- defN 22-Aug-28 12:11 parseq-2023.5.0/parseq/third_party/xrt.py
+-rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-2023.5.0/parseq/third_party/__init__.py
+-rw-rw-rw-  2.0 fat     7812 b- defN 17-Aug-04 10:49 parseq-2023.5.0/parseq/third_party/data/Energies.txt
+-rw-rw-rw-  2.0 fat      345 b- defN 22-Mar-31 11:43 parseq-2023.5.0/parseq/utils/format.py
+-rw-rw-rw-  2.0 fat     2009 b- defN 23-Mar-29 00:12 parseq-2023.5.0/parseq/utils/ft.py
+-rw-rw-rw-  2.0 fat     1660 b- defN 23-Mar-20 16:04 parseq-2023.5.0/parseq/utils/h5reduce.py
+-rw-rw-rw-  2.0 fat     3873 b- defN 23-Apr-26 18:43 parseq-2023.5.0/parseq/utils/math.py
+-rw-rw-rw-  2.0 fat        6 b- defN 17-Jul-08 15:01 parseq-2023.5.0/parseq/utils/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat     5037 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      140 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat     5003 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-30 17:00 parseq-2023.5.0/parseq.egg-info/top_level.txt
+177 files, 3319887 bytes uncompressed, 2216633 bytes compressed:  33.2%
```

## zipnote {}

```diff
@@ -1,478 +1,532 @@
-Filename: parseq-1.0.0/
+Filename: parseq-2023.5.0/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/
+Filename: parseq-2023.5.0/parseq/
 Comment: 
 
-Filename: parseq-1.0.0/parseq.egg-info/
+Filename: parseq-2023.5.0/parseq.egg-info/
 Comment: 
 
-Filename: parseq-1.0.0/LICENSE
+Filename: parseq-2023.5.0/LICENSE
 Comment: 
 
-Filename: parseq-1.0.0/PKG-INFO
+Filename: parseq-2023.5.0/PKG-INFO
 Comment: 
 
-Filename: parseq-1.0.0/setup.cfg
+Filename: parseq-2023.5.0/setup.cfg
 Comment: 
 
-Filename: parseq-1.0.0/setup.py
+Filename: parseq-2023.5.0/setup.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/
+Filename: parseq-2023.5.0/parseq/core/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/
+Filename: parseq-2023.5.0/parseq/fits/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/
+Filename: parseq-2023.5.0/parseq/gui/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/
+Filename: parseq-2023.5.0/parseq/help/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/third_party/
+Filename: parseq-2023.5.0/parseq/tests/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/utils/
+Filename: parseq-2023.5.0/parseq/third_party/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/CODERULES.txt
+Filename: parseq-2023.5.0/parseq/utils/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/description.py
+Filename: parseq-2023.5.0/parseq/CODERULES.txt
 Comment: 
 
-Filename: parseq-1.0.0/parseq/version.py
+Filename: parseq-2023.5.0/parseq/description.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/__init__.py
+Filename: parseq-2023.5.0/parseq/version.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/commons.py
+Filename: parseq-2023.5.0/parseq/__init__.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/config.py
+Filename: parseq-2023.5.0/parseq/core/commons.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/logger.py
+Filename: parseq-2023.5.0/parseq/core/config.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/nodes.py
+Filename: parseq-2023.5.0/parseq/core/logger.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/plotExport.py
+Filename: parseq-2023.5.0/parseq/core/nodes.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/save_restore.py
+Filename: parseq-2023.5.0/parseq/core/plotExport.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/singletons.py
+Filename: parseq-2023.5.0/parseq/core/save_restore.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/spectra.py
+Filename: parseq-2023.5.0/parseq/core/singletons.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/transforms.py
+Filename: parseq-2023.5.0/parseq/core/spectra.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/core/__init__.py
+Filename: parseq-2023.5.0/parseq/core/transforms.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/
+Filename: parseq-2023.5.0/parseq/core/__init__.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/aboutDialog.py
+Filename: parseq-2023.5.0/parseq/fits/basefit.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/calibrateEnergy.py
+Filename: parseq-2023.5.0/parseq/fits/functionfit.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/columnFormat.py
+Filename: parseq-2023.5.0/parseq/fits/lcf.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/combineSpectra.py
+Filename: parseq-2023.5.0/parseq/fits/__init__.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/dataRebin.py
+Filename: parseq-2023.5.0/parseq/gui/fits/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/dataTreeModelView.py
+Filename: parseq-2023.5.0/parseq/gui/_images/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/fileDialogs.py
+Filename: parseq-2023.5.0/parseq/gui/aboutDialog.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/fileTreeModelView.py
+Filename: parseq-2023.5.0/parseq/gui/calibrateEnergy.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/gcommons.py
+Filename: parseq-2023.5.0/parseq/gui/columnFormat.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/mainWindow.py
+Filename: parseq-2023.5.0/parseq/gui/combineSpectra.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/nodeWidget.py
+Filename: parseq-2023.5.0/parseq/gui/dataRebin.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/plot.py
+Filename: parseq-2023.5.0/parseq/gui/dataTreeModelView.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/plotOptions.py
+Filename: parseq-2023.5.0/parseq/gui/fileDialogs.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/propsOfData.py
+Filename: parseq-2023.5.0/parseq/gui/fileTreeModelView.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/propWidget.py
+Filename: parseq-2023.5.0/parseq/gui/gcommons.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/roi.py
+Filename: parseq-2023.5.0/parseq/gui/mainWindow.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/transformer.py
+Filename: parseq-2023.5.0/parseq/gui/nodeWidget.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/undoredo.py
+Filename: parseq-2023.5.0/parseq/gui/plot.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/webWidget.py
+Filename: parseq-2023.5.0/parseq/gui/plotOptions.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/__init__.py
+Filename: parseq-2023.5.0/parseq/gui/propsOfData.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-help.png
+Filename: parseq-2023.5.0/parseq/gui/propWidget.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-info.png
+Filename: parseq-2023.5.0/parseq/gui/roi.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-1dim-32.png
+Filename: parseq-2023.5.0/parseq/gui/tasker.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-1dim-64.png
+Filename: parseq-2023.5.0/parseq/gui/undoredo.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-1dim-busy-32.png
+Filename: parseq-2023.5.0/parseq/gui/webWidget.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-1dim-busy-64.png
+Filename: parseq-2023.5.0/parseq/gui/__init__.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-2dim-32.png
+Filename: parseq-2023.5.0/parseq/gui/fits/gbasefit.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-2dim-64.png
+Filename: parseq-2023.5.0/parseq/gui/fits/gfunctionfit.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-2dim-busy-32.png
+Filename: parseq-2023.5.0/parseq/gui/fits/glcf.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-2dim-busy-64.png
+Filename: parseq-2023.5.0/parseq/gui/fits/__init__.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-3dim-32.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-fit-32.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-3dim-64.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-fit-64.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-3dim-busy-32.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-help.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-3dim-busy-64.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-info.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-ndim-32.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-32.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-ndim-64.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-64.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-ndim-busy-32.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-32.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-item-ndim-busy-64.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-64.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-load-proj.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-32.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-redo.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-64.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-save-proj.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-busy-32.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-save-text.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-busy-64.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/icon-undo.png
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-32.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/gui/_images/parseq.ico
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-64.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/exts/
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-32.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-64.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_static/
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-32.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_templates/
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-64.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-32.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/conf.py
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-64.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/conf_doc.py
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-load-proj.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/data.rst
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-redo.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/howto.rst
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-save-proj.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/index.rst
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-save-text.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/license.rst
+Filename: parseq-2023.5.0/parseq/gui/_images/icon-undo.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/make.bat
+Filename: parseq-2023.5.0/parseq/gui/_images/parseq.ico
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/nodes.rst
+Filename: parseq-2023.5.0/parseq/help/exts/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/notesgui.rst
+Filename: parseq-2023.5.0/parseq/help/_images/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/top.rst
+Filename: parseq-2023.5.0/parseq/help/_static/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/transforms.rst
+Filename: parseq-2023.5.0/parseq/help/_templates/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/widgets.rst
+Filename: parseq-2023.5.0/parseq/help/_themes/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/__init__.py
+Filename: parseq-2023.5.0/parseq/help/conf.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/exts/animation.py
+Filename: parseq-2023.5.0/parseq/help/conf_doc.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/mickey-rtfm.gif
+Filename: parseq-2023.5.0/parseq/help/data.rst
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/node1.png
+Filename: parseq-2023.5.0/parseq/help/fits.rst
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/node2.png
+Filename: parseq-2023.5.0/parseq/help/howto.rst
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/node3.png
+Filename: parseq-2023.5.0/parseq/help/index.rst
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/node4.png
+Filename: parseq-2023.5.0/parseq/help/license.rst
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/parseq.ico
+Filename: parseq-2023.5.0/parseq/help/make.bat
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/parseq_big.png
+Filename: parseq-2023.5.0/parseq/help/nodes.rst
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/XAS_icon.ico
+Filename: parseq-2023.5.0/parseq/help/notesgui.rst
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/XES_dispersive_icon.ico
+Filename: parseq-2023.5.0/parseq/help/top.rst
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_images/XES_scan_icon.ico
+Filename: parseq-2023.5.0/parseq/help/transforms.rst
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_static/animation.js
+Filename: parseq-2023.5.0/parseq/help/widgets.rst
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_static/thumbnail.css
+Filename: parseq-2023.5.0/parseq/help/__init__.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_templates/layout.html
+Filename: parseq-2023.5.0/parseq/help/exts/animation.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/mytheme/
+Filename: parseq-2023.5.0/parseq/help/_images/mickey-rtfm.gif
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/parseq/
+Filename: parseq-2023.5.0/parseq/help/_images/node1.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/mytheme/static/
+Filename: parseq-2023.5.0/parseq/help/_images/node2.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/mytheme/layout.html
+Filename: parseq-2023.5.0/parseq/help/_images/node3.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/mytheme/theme.conf
+Filename: parseq-2023.5.0/parseq/help/_images/node4.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/mytheme/static/mycss.css_t
+Filename: parseq-2023.5.0/parseq/help/_images/parseq.ico
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/parseq/static/
+Filename: parseq-2023.5.0/parseq/help/_images/parseq_big.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/parseq/layout.html
+Filename: parseq-2023.5.0/parseq/help/_images/XAS_icon.ico
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/parseq/page.html
+Filename: parseq-2023.5.0/parseq/help/_images/XES_dispersive_icon.ico
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/parseq/theme.conf
+Filename: parseq-2023.5.0/parseq/help/_images/XES_scan_icon.ico
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/parseq/static/default.css_t
+Filename: parseq-2023.5.0/parseq/help/_static/animation.js
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/parseq/static/math_config_win32.js
+Filename: parseq-2023.5.0/parseq/help/_static/thumbnail.css
 Comment: 
 
-Filename: parseq-1.0.0/parseq/help/_themes/parseq/static/utils.js
+Filename: parseq-2023.5.0/parseq/help/_templates/layout.html
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/circles-rect.png
+Filename: parseq-2023.5.0/parseq/help/_themes/mytheme/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/circles.png
+Filename: parseq-2023.5.0/parseq/help/_themes/parseq/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/modeltest.py
+Filename: parseq-2023.5.0/parseq/help/_themes/mytheme/static/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_aboutWidget.py
+Filename: parseq-2023.5.0/parseq/help/_themes/mytheme/layout.html
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_calibrateEnergyWidget.py
+Filename: parseq-2023.5.0/parseq/help/_themes/mytheme/theme.conf
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_columnStrings.py
+Filename: parseq-2023.5.0/parseq/help/_themes/mytheme/static/mycss.css_t
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_combineSpectraWidget.py
+Filename: parseq-2023.5.0/parseq/help/_themes/parseq/static/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_commons.py
+Filename: parseq-2023.5.0/parseq/help/_themes/parseq/layout.html
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_curve_shear.py
+Filename: parseq-2023.5.0/parseq/help/_themes/parseq/page.html
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_dataRebinWidget.py
+Filename: parseq-2023.5.0/parseq/help/_themes/parseq/theme.conf
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_dataTreeModelView.py
+Filename: parseq-2023.5.0/parseq/help/_themes/parseq/static/default.css_t
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_fileDialog.py
+Filename: parseq-2023.5.0/parseq/help/_themes/parseq/static/math_config_win32.js
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_fileTreeModelView.py
+Filename: parseq-2023.5.0/parseq/help/_themes/parseq/static/utils.js
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_flowLayout.py
+Filename: parseq-2023.5.0/parseq/tests/data/
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_hdf5.py
+Filename: parseq-2023.5.0/parseq/tests/circles-rect.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_mainWindow.py
+Filename: parseq-2023.5.0/parseq/tests/circles.png
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_node.py
+Filename: parseq-2023.5.0/parseq/tests/modeltest.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_nodeWidget.py
+Filename: parseq-2023.5.0/parseq/tests/test_aboutWidget.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py
+Filename: parseq-2023.5.0/parseq/tests/test_calibrateEnergyWidget.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_plotInteractiveImageSingleROI.py
+Filename: parseq-2023.5.0/parseq/tests/test_columnStrings.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_plotOptions.py
+Filename: parseq-2023.5.0/parseq/tests/test_combineSpectraWidget.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_QSortFilterProxyModel.py
+Filename: parseq-2023.5.0/parseq/tests/test_commons.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_ROI.py
+Filename: parseq-2023.5.0/parseq/tests/test_curve_shear.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_slice.py
+Filename: parseq-2023.5.0/parseq/tests/test_dataRebinWidget.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/test_stateButtons.py
+Filename: parseq-2023.5.0/parseq/tests/test_dataTreeModelView.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/tests/__init__.py
+Filename: parseq-2023.5.0/parseq/tests/test_fileDialog.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/third_party/data/
+Filename: parseq-2023.5.0/parseq/tests/test_fileTreeModelView.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/third_party/XAFSmass.py
+Filename: parseq-2023.5.0/parseq/tests/test_fit.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/third_party/xrt.py
+Filename: parseq-2023.5.0/parseq/tests/test_flowLayout.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/third_party/__init__.py
+Filename: parseq-2023.5.0/parseq/tests/test_hdf5.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/third_party/data/Energies.txt
+Filename: parseq-2023.5.0/parseq/tests/test_mainWindow.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/utils/format.py
+Filename: parseq-2023.5.0/parseq/tests/test_node.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/utils/ft.py
+Filename: parseq-2023.5.0/parseq/tests/test_nodeWidget.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/utils/h5reduce.py
+Filename: parseq-2023.5.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/utils/math.py
+Filename: parseq-2023.5.0/parseq/tests/test_plotInteractiveImageSingleROI.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq/utils/__init__.py
+Filename: parseq-2023.5.0/parseq/tests/test_plotOptions.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq.egg-info/dependency_links.txt
+Filename: parseq-2023.5.0/parseq/tests/test_QSortFilterProxyModel.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq.egg-info/not-zip-safe
+Filename: parseq-2023.5.0/parseq/tests/test_ROI.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq.egg-info/PKG-INFO
+Filename: parseq-2023.5.0/parseq/tests/test_slice.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq.egg-info/requires.txt
+Filename: parseq-2023.5.0/parseq/tests/test_stateButtons.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq.egg-info/SOURCES.txt
+Filename: parseq-2023.5.0/parseq/tests/__init__.py
 Comment: 
 
-Filename: parseq-1.0.0/parseq.egg-info/top_level.txt
+Filename: parseq-2023.5.0/parseq/tests/data/cu-ref-mix.res
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/tests/data/pb-ref-mix.res
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/tests/data/zn-ref-mix.res
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/third_party/data/
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/third_party/XAFSmass.py
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/third_party/xrt.py
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/third_party/__init__.py
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/third_party/data/Energies.txt
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/utils/format.py
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/utils/ft.py
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/utils/h5reduce.py
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/utils/math.py
+Comment: 
+
+Filename: parseq-2023.5.0/parseq/utils/__init__.py
+Comment: 
+
+Filename: parseq-2023.5.0/parseq.egg-info/dependency_links.txt
+Comment: 
+
+Filename: parseq-2023.5.0/parseq.egg-info/not-zip-safe
+Comment: 
+
+Filename: parseq-2023.5.0/parseq.egg-info/PKG-INFO
+Comment: 
+
+Filename: parseq-2023.5.0/parseq.egg-info/requires.txt
+Comment: 
+
+Filename: parseq-2023.5.0/parseq.egg-info/SOURCES.txt
+Comment: 
+
+Filename: parseq-2023.5.0/parseq.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `parseq-1.0.0/LICENSE` & `parseq-2023.5.0/LICENSE`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/PKG-INFO` & `parseq-2023.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parseq
-Version: 1.0.0
+Version: 2023.5.0
 Summary: ParSeq is a python software library for Parallel execution of Sequential data analysis.
 Home-page: http://parseq.readthedocs.io
 Author: Konstantin Klementiev
 Author-email: konstantin.klementiev@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/kklmn/ParSeq
 Keywords: data-analysis pipeline framework gui synchrotron spectroscopy
@@ -53,16 +53,19 @@
    pipeline.
 
 -  Creation of cross-data combinations (e.g. averaging, RMS or PCA) and their
    propagation downstream the pipeline together with the parental data. The
    possibility of termination of the parental data at any selected downstream
    node.
 
--  Parallel execution of data analysis with multiprocessing or multithreading
-   (can be opted by the pipeline application).
+-  Parallel execution of data transformations with multiprocessing or
+   multithreading (can be opted by the pipeline application).
+
+-  Optional curve fitting solvers, also executed in parallel for multiple data
+   items.
 
 -  Informative error handling that provides alerts and stack traceback -- the
    type and location of the occurred error.
 
 -  Export of the workflow into a project file. Export of data into various data
    formats with accompanied Python scripts that visualize the exported data for
    the user to tune their publication plots.
@@ -75,17 +78,17 @@
    from the analysis widget doc strings. The help pages are built by Sphinx at
    the startup time.
 
 -  The pipeline can be operated via scripts or GUI.
 
 -  Optional automatic loading of new data during a measurement time.
 
-The mechanisms for creating nodes and transformations, connecting them together
-and creating Qt widgets for the transformations are exemplified by separately
-installed analysis packages:
+The mechanisms for creating nodes, transformations and curve fitting solvers,
+connecting them together and creating Qt widgets for the transformations and
+and curve fits are exemplified by separately installed analysis packages:
 
 - `ParSeq-XES-scan <https://github.com/kklmn/ParSeq-XES-scan>`_
 - `ParSeq-XES-dispersive <https://github.com/kklmn/ParSeq-XES-dispersive>`_
 - `ParSeq-XAS <https://github.com/kklmn/ParSeq-XAS>`_
 
 Dependencies
 ------------
```

## Comparing `parseq-1.0.0/setup.py` & `parseq-2023.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,26 +55,27 @@
     platforms='OS Independent',
     license='MIT License',
     keywords='data-analysis pipeline framework gui synchrotron spectroscopy',
     # python_requires=,
     zip_safe=False,  # True: build zipped egg, False: unzipped
     packages=['parseq',
               'parseq.core',
-              'parseq.gui',
+              'parseq.fits',
+              'parseq.gui', 'parseq.gui.fits',
               'parseq.help',
               'parseq.tests', 'parseq.third_party', 'parseq.utils'],
     # package_dir={'parseq': '.'},
     package_data={
         'parseq': ['CODERULES.txt'],
         'parseq.gui': ['_images/*.*'],
         'parseq.help': [
             '*.rst', '*.bat',
             '_images/*.*', '_static/*.*', '_templates/*.*',
             '_themes/*/*.*', '_themes/*/*/*.*', 'exts/*.*'],
-        'parseq.tests': ['*.png'],
+        'parseq.tests': ['*.png', 'data/*.*'],
         'parseq.third_party': ['data/*.*'],
         },
     install_requires=['numpy>=1.8.0', 'scipy>=0.17.0', 'matplotlib>=2.0.0',
                       'sphinx>=1.6.2', 'sphinxcontrib-jquery', 'autopep8',
                       'h5py', 'silx>=1.1.0', 'hdf5plugin', 'psutil',
                       'docutils', 'distro'],
     classifiers=['Development Status :: 5 - Production/Stable',
```

## Comparing `parseq-1.0.0/parseq/description.py` & `parseq-2023.5.0/parseq/description.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,19 @@
    pipeline.
 
 -  Creation of cross-data combinations (e.g. averaging, RMS or PCA) and their
    propagation downstream the pipeline together with the parental data. The
    possibility of termination of the parental data at any selected downstream
    node.
 
--  Parallel execution of data analysis with multiprocessing or multithreading
-   (can be opted by the pipeline application).
+-  Parallel execution of data transformations with multiprocessing or
+   multithreading (can be opted by the pipeline application).
+
+-  Optional curve fitting solvers, also executed in parallel for multiple data
+   items.
 
 -  Informative error handling that provides alerts and stack traceback -- the
    type and location of the occurred error.
 
 -  Export of the workflow into a project file. Export of data into various data
    formats with accompanied Python scripts that visualize the exported data for
    the user to tune their publication plots.
@@ -58,17 +61,17 @@
    from the analysis widget doc strings. The help pages are built by Sphinx at
    the startup time.
 
 -  The pipeline can be operated via scripts or GUI.
 
 -  Optional automatic loading of new data during a measurement time.
 
-The mechanisms for creating nodes and transformations, connecting them together
-and creating Qt widgets for the transformations are exemplified by separately
-installed analysis packages:
+The mechanisms for creating nodes, transformations and curve fitting solvers,
+connecting them together and creating Qt widgets for the transformations and
+and curve fits are exemplified by separately installed analysis packages:
 
 - `ParSeq-XES-scan <https://github.com/kklmn/ParSeq-XES-scan>`_
 - `ParSeq-XES-dispersive <https://github.com/kklmn/ParSeq-XES-dispersive>`_
 - `ParSeq-XAS <https://github.com/kklmn/ParSeq-XAS>`_
 
 Dependencies
 ------------
```

## Comparing `parseq-1.0.0/parseq/__init__.py` & `parseq-2023.5.0/parseq/__init__.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/core/commons.py` & `parseq-2023.5.0/parseq/core/commons.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/core/config.py` & `parseq-2023.5.0/parseq/core/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 __author__ = "Konstantin Klementiev"
-__date__ = "2 Apr 2021"
+__date__ = "5 May 2021"
 # !!! SEE CODERULES.TXT !!!
 
 import os
 
 try:
     from configparser import ConfigParser
 except ImportError:
@@ -24,14 +24,18 @@
 configGUI = ConfigParser()
 configGUI.read(iniFileGUI, encoding=encoding)
 
 iniFileTransforms = (os.path.join(iniDir, 'transforms.ini'))
 configTransforms = ConfigParser()
 configTransforms.read(iniFileTransforms, encoding=encoding)
 
+iniFileFits = (os.path.join(iniDir, 'fits.ini'))
+configFits = ConfigParser()
+configFits.read(iniFileFits, encoding=encoding)
+
 iniFileFormats = (os.path.join(iniDir, 'formats.ini'))
 configFormats = ConfigParser()
 configFormats.read(iniFileFormats, encoding=encoding)
 configFormats.optionxform = str  # makes it case sensitive
 
 
 def get(conf, section, entry, default=None):
@@ -61,10 +65,13 @@
             configLoad.write(cf)
     if (what == 'all') or ('gui' in whatl):
         with open(iniFileGUI, 'w+', encoding=encoding) as cf:
             configGUI.write(cf)
     if (what == 'all') or ('transform' in whatl):
         with open(iniFileTransforms, 'w+', encoding=encoding) as cf:
             configTransforms.write(cf)
+    if (what == 'all') or ('fit' in whatl):
+        with open(iniFileFits, 'w+', encoding=encoding) as cf:
+            configFits.write(cf)
     if (what == 'all') or ('format' in whatl):
         with open(iniFileFormats, 'w+', encoding=encoding) as cf:
             configFormats.write(cf)
```

## Comparing `parseq-1.0.0/parseq/core/logger.py` & `parseq-2023.5.0/parseq/core/logger.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/core/nodes.py` & `parseq-2023.5.0/parseq/core/nodes.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/core/plotExport.py` & `parseq-2023.5.0/parseq/core/plotExport.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,16 @@
         arrays = readFile(saveType, fname)
         x = arrays[:, 0]
         ys = [arrays[:, iy+1] for iy in range(arrays.shape[1]-1)]
         curves.append([x, ys, headers])
     elif saveType.endswith(('json', 'pickle', 'h5')):
         data, h5file = readFile(saveType, fname)
         # slicing is needed to create an ndarray from HDF5 object
+        if props[2][0] not in data:
+            return curves
         x = data[props[2][0]][:]
         ys = [data[prop][:] for prop in headers]
         curves.append([x, ys, headers])
         if len(props) > 4:  # auxArrays
             auxs = props[4]
             for aux in auxs:
                 xa = data[aux[0]][:]
```

## Comparing `parseq-1.0.0/parseq/core/save_restore.py` & `parseq-2023.5.0/parseq/core/save_restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 __author__ = "Konstantin Klementiev"
-__date__ = "3 Mar 2023"
+__date__ = "6 Apr 2023"
 # !!! SEE CODERULES.TXT !!!
 
 import os
 import numpy as np
 import pickle
 import json
 import autopep8
@@ -86,19 +86,21 @@
                str(root.colorAutoUpdate))
 
     dirname = os.path.dirname(fname)
     for item in csi.dataRootItem.get_items(alsoGroupHeads=True):
         item.save_to_project(configProject, dirname)
     if save_perspective:
         save_perspective(configProject)
+    os.chdir(os.path.dirname(fname))
     with open(fname, 'w+', encoding=encoding) as cf:
         configProject.write(cf)
 
 
 def save_data(fname, saveNodes, saveTypes, qMessageBox=None):
+    os.chdir(os.path.dirname(fname))
     if fname.endswith('.pspj'):
         fname = fname.replace('.pspj', '')
 
     plots = []
     if ('txt' in saveTypes) or ('txt.gz' in saveTypes):
         for iNode, ((nodeName, node), saveNode) in enumerate(
                 zip(csi.nodes.items(), saveNodes)):
@@ -108,14 +110,15 @@
                 header = [node.plotXArray] + [y for y in node.plotYArrays]
             else:
                 continue
 
             curves = {}
             for it in csi.selectedItems:
                 dataToSave = [getattr(it, arr) for arr in header]
+                dataToSave = [d for d in dataToSave if d is not None]
                 nname = nodeName.translate(chars2removeMap)
                 dname = it.alias.translate(chars2removeMap)
                 sname = u'{0}-{1}-{2}'.format(iNode+1, nname, dname)
                 if 'txt' in saveTypes:
                     np.savetxt(sname+'.txt', np.column_stack(dataToSave),
                                fmt='%.12g', header=' '.join(header))
                 if 'txt.gz' in saveTypes:
@@ -166,20 +169,22 @@
                 header = node.plot2DArray
             elif node.plotDimension == 3:
                 header = node.plot3DArray
 
             curves = {}
             for it, sname in zip(csi.selectedItems, snames):
                 for aN in node.arrays:
-                    dataToSave[it][aN] = getattr(it, aN).tolist()
+                    d = getattr(it, aN)
+                    dataToSave[it][aN] = d.tolist() if d is not None else None
                 for aN in [j for i in node.auxArrays for j in i]:
                     try:
-                        dataToSave[it][aN] = getattr(it, aN).tolist()
+                        d = getattr(it, aN)
                     except AttributeError:
                         continue
+                    dataToSave[it][aN] = d.tolist() if d is not None else None
                 curves[sname] = [it.alias, it.color, header,
                                  it.plotProps[node.name]]
                 if node.auxArrays:
                     headerAux = []
                     for aG in node.auxArrays:
                         for yN in aG:
                             if not hasattr(it, yN):
@@ -222,15 +227,18 @@
                 header = node.plot2DArray
             elif node.plotDimension == 3:
                 header = node.plot3DArray
 
             curves = {}
             for it, sname in zip(csi.selectedItems, snames):
                 for aN in node.arrays:
-                    dataToSave[it][aN] = getattr(it, aN)
+                    try:
+                        dataToSave[it][aN] = getattr(it, aN)
+                    except AttributeError:
+                        continue
                 for aN in [j for i in node.auxArrays for j in i]:
                     try:
                         dataToSave[it][aN] = getattr(it, aN)
                     except AttributeError:
                         continue
                 curves[sname] = [it.alias, it.color, header,
                                  it.plotProps[node.name]]
@@ -255,14 +263,16 @@
                     dname = it.alias.translate(chars2removeMap)
                     if dname in f:
                         continue
                     grp = dataGrp.create_group(dname)
                     for aN in dataToSave[it]:
                         if aN in grp:
                             continue
+                        if dataToSave[it][aN] is None:  # when optional
+                            continue
                         com = None if np.isscalar(dataToSave[it][aN]) else\
                             'gzip'
                         grp.create_dataset(aN, data=dataToSave[it][aN],
                                            compression=com)
                     grp.create_dataset('transformParams',
                                        data=str(it.transformParams))
                 for plot in h5plots:
@@ -339,9 +349,10 @@
         output.extend(["    from silx.gui import qt",
                        "    app = qt.QApplication([])"])
     output.extend(["    plotSavedData(plots, '{0}')".format(lib), ""])
     if lib == 'silx':
         output.extend(["    app.exec_()"])
 
     fnameOut = '{0}_{1}.py'.format(fname, lib)
+    os.chdir(os.path.dirname(fname))
     with open(fnameOut, 'w', encoding=encoding) as f:
         f.write('\n'.join(output))
```

## Comparing `parseq-1.0.0/parseq/core/singletons.py` & `parseq-2023.5.0/parseq/core/singletons.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 appAuthor = None
 appLicense = None
 appVersion = None
 # end defined by the app
 
 nodes = OrderedDict()
 transforms = OrderedDict()
+fits = OrderedDict()
 # transformWidgets = OrderedDict()
 mainWindow = None
 currentNode = None
 
 withGUI = 'not set yet'
 # updated later by MainWindowParSeq as qt.qApp.desktop().logicalDpiX() / 120.:
 screenFactor = 1
@@ -42,9 +43,9 @@
 modelLeadingColumns = ['data name', '']  # the last one is for view state (eye)
 
 selectionModel = None
 selectedItems, selectedTopItems = [], []  # common for all data trees
 recentlyLoadedItems = []
 allLoadedItems = []
 
-# transformer will be created in MainWindow ParSeq init
-transformer = None
+# tasker will be created in MainWindow ParSeq init
+tasker = None
```

## Comparing `parseq-1.0.0/parseq/core/spectra.py` & `parseq-2023.5.0/parseq/core/spectra.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 documentation explains how. Otherwise, most typically it is used within the
 ParSeq GUI, where the tree model feeds the `model-view-controller
 <https://doc.qt.io/qt-6/model-view-programming.html>`_ software architecture of
 Qt, where the user does not have to know about the underlying objects and
 methods. See :ref:`Notes on usage of GUI <notesgui>`.
 """
 __author__ = "Konstantin Klementiev"
-__date__ = "3 Mar 2023"
+__date__ = "6 Apr 2023"
 # !!! SEE CODERULES.TXT !!!
 
 # import sys
 import os.path as osp
 import re
 import time
 import copy
@@ -540,45 +540,52 @@
         self.aliasExtra = None  # for extra name qualifier
         self.meta = {'text': '', 'modified': '', 'size': 0}
         self.combinesTo = []  # list of instances of Spectrum if not empty
 
         self.transformParams = {}  # each transform will add to this dict
         # init self.transformParams:
         for tr in csi.transforms.values():
-            self.transformParams.update(tr.defaultParams)
+            self.transformParams.update(copy.deepcopy(tr.defaultParams))
+
+        self.fitParams = {}  # each fit will add to this dict
+        # init self.fitParams:
+        for fit in csi.fits.values():
+            self.fitParams.update(copy.deepcopy(fit.defaultParams))
 
         if insertAt is None:
             parentItem.childItems.append(self)
         else:
             parentItem.childItems.insert(insertAt, self)
 
         if ((isinstance(self.madeOf, str) and self.dataFormat) or
                 isinstance(self.madeOf, (list, tuple, dict))):
             copyTransformParams = kwargs.pop(
                 'copyTransformParams',
                 csi.dataRootItem.kwargs['copyTransformParams'])
             transformParams = kwargs.pop(
                 'transformParams',
                 csi.dataRootItem.kwargs.get('transformParams', {}))
+            fitParams = kwargs.pop('fitParams', {})
             shouldLoadNow = kwargs.pop(
                 'shouldLoadNow',
                 csi.dataRootItem.kwargs.get('shouldLoadNow', True))
             runDownstream = kwargs.pop(
                 'runDownstream',
                 csi.dataRootItem.kwargs.get('runDownstream', False))
             if csi.withGUI:
                 self.init_plot_props()
                 plotProps = kwargs.pop('plotProps', {})
                 if plotProps:
-                    self.plotProps.update(plotProps)
+                    self.plotProps.update(copy.deepcopy(plotProps))
 
             self.read_data(shouldLoadNow=shouldLoadNow,
                            runDownstream=runDownstream,
                            copyTransformParams=copyTransformParams,
-                           transformParams=transformParams)
+                           transformParams=transformParams,
+                           fitParams=fitParams)
 
         elif isinstance(self.madeOf, str) and not self.dataFormat:
             # i.e. is a group
             self.dataType = cco.DATA_GROUP
             if csi.withGUI:
                 from ..gui import gcommons as gco
                 cp = (kwargs.pop('colorPolicy', 'loop1')).lower()
@@ -628,19 +635,21 @@
                                 pv = v[ind]
                             else:
                                 pv = v
                             plotParams[k] = pv
                         self.plotProps[node.name][yName] = plotParams
 
     def get_state(self, nodeName):
+        if self.error is not None:
+            return cco.DATA_STATE_BAD
         return self.state[nodeName]
 
     def read_data(self, shouldLoadNow=True, runDownstream=False,
-                  copyTransformParams=True, transformParams={}):
-        toNode = csi.nodes[self.originNodeName]
+                  copyTransformParams=True, transformParams={}, fitParams={}):
+        fromNode = csi.nodes[self.originNodeName]
         if isinstance(self.madeOf, dict):
             self.dataType = cco.DATA_BRANCH
             if self.alias == 'auto':
                 tmpalias = '{0}_{1}'.format(
                     self.parentItem.alias, self.parentItem.child_count())
             if shouldLoadNow:
                 self.branch_data()
@@ -669,15 +678,15 @@
                 self.dataType = cco.DATA_DATASET
             else:
                 self.dataType = cco.DATA_COLUMN_FILE
             self.set_auto_color_tag()
             if shouldLoadNow:
                 self.read_file()
 
-            if self.state[toNode.name] == cco.DATA_STATE_GOOD:
+            if self.state[fromNode.name] == cco.DATA_STATE_GOOD:
                 if not self.check_shape():
                     print('Incompatible data shapes!')
                     self.state[self.originNodeName] = cco.DATA_STATE_BAD
                     self.colorTag = 3
 
             basename = osp.basename(self.madeOf)
             if self.alias == 'auto':
@@ -705,32 +714,39 @@
             self.alias = tmpalias
 
 #        csi.undo.append([self, insertAt, lenData])
 
         if copyTransformParams:
             if len(csi.selectedItems) > 0:
                 self.transformParams.update(
-                    csi.selectedItems[0].transformParams)
+                    copy.deepcopy(csi.selectedItems[0].transformParams))
+                self.fitParams.update(
+                    copy.deepcopy(csi.selectedItems[0].fitParams))
             else:
                 for tr in csi.transforms.values():
-                    self.transformParams.update(tr.iniParams)
+                    self.transformParams.update(
+                        copy.deepcopy(tr.iniParams))
+                for fit in csi.fits.values():
+                    self.fitParams.update(
+                        copy.deepcopy(fit.iniParams))
 
-        self.transformParams.update(transformParams)
+        self.transformParams.update(copy.deepcopy(transformParams))
+        self.fitParams.update(copy.deepcopy(fitParams))
 
-        # replot if toNode is not reached by any transform, otherwise it will
+        # replot if fromNode is not reached by any transform, otherwise it will
         # be replotted by that transform:
-        for tr in toNode.transformsOut:
+        for tr in fromNode.transformsOut:
             if tr.fromNode is tr.toNode:
                 break
         else:
-            csi.nodesToReplot = [toNode]
+            csi.nodesToReplot = [fromNode]
 
-        if runDownstream and toNode.transformsOut and \
-                self.state[toNode.name] == cco.DATA_STATE_GOOD:
-            for tr in toNode.transformsOut:
+        if runDownstream and fromNode.transformsOut and \
+                self.state[fromNode.name] == cco.DATA_STATE_GOOD:
+            for tr in fromNode.transformsOut:
                 tr.run(dataItems=[self])  # no need for multiprocessing here
                 if csi.model is not None:
                     csi.model.invalidateData()
 
     def set_auto_color_tag(self):
         if self.colorTag != 0:
             return
@@ -740,24 +756,24 @@
 
         if self.dataType == cco.DATA_DATASET:
             self.colorTag = 1
         elif self.dataType == cco.DATA_COLUMN_FILE:
             self.colorTag = 2
 
     def check_shape(self):
-        toNode = csi.nodes[self.originNodeName]
-        for iarr, arrName in enumerate(toNode.checkShapes):
+        fromNode = csi.nodes[self.originNodeName]
+        for iarr, arrName in enumerate(fromNode.checkShapes):
             pos = arrName.find('[')
             if pos > 0:
                 stem = arrName[:pos]
                 sl = arrName[pos+1:-1]
             else:
                 stem = arrName
                 sl = '0'
-            checkName = toNode.get_prop(stem, 'raw')
+            checkName = fromNode.get_prop(stem, 'raw')
             arr = getattr(self, checkName)
             shape = arr.shape[eval(sl)] if arr is not None else []
             if iarr == 0:
                 shape0 = shape
                 continue
             if shape != shape0:
                 return False
@@ -783,14 +799,30 @@
         """This method searches for one or more sequences in the elements of
         `dataSource` list. If found, these sequences should be of an equal
         length and the same number of spectra will be added to the data model
         in a separate group. If a shorter sequence is found, only its first
         element will be used for the expansion of this sequence to the length
         of the longest sequence(s)."""
 
+        def getTransformParams(configData):
+            res = {}
+            for tr in csi.transforms.values():
+                for key, val in tr.defaultParams.items():
+                    res[key] = config.get(configData, name, key, default=val)
+            return res
+
+        def getFitParams(configData):
+            res = {}
+            for fit in csi.fits.values():
+                for key, val in fit.defaultParams.items():
+                    if key == fit.ioAttrs['result']:
+                        continue
+                    res[key] = config.get(configData, name, key, default=val)
+            return res
+
         nameFull = None
         if 'configData' in kwargs:  # ini file
             configData = kwargs['configData']
             if name in configData:
                 madeOf = config.get(configData, name, 'madeOf')
                 if (isinstance(madeOf, str) and
                         'dataFormat' in configData[name]):
@@ -803,32 +835,24 @@
                         tmp['dataFormat'] = tmp['dataFormat_relative']
                     if 'colorIndividual' in configData[name]:
                         tmp['colorIndividual'] = config.get(
                             configData, name, 'colorIndividual')
                     if 'plotProps' in configData[name]:
                         tmp['plotProps'] = config.get(
                             configData, name, 'plotProps')
-                    trParams = {}
-                    for tr in csi.transforms.values():
-                        for key, val in tr.defaultParams.items():
-                            trParams[key] = config.get(configData, name, key,
-                                                       default=val)
-                    tmp['transformParams'] = trParams
+                    tmp['transformParams'] = getTransformParams(configData)
+                    tmp['fitParams'] = getFitParams(configData)
                     name = tmp.pop('madeOf_relative')
                     nameFull = tmp.pop('madeOf')
                 elif isinstance(madeOf, (dict, list, tuple)):
                     tmp = {entry: config.get(configData, name, entry)
                            for entry in self.configFieldsCombined}
                     tmp['alias'] = name
-                    trParams = {}
-                    for tr in csi.transforms.values():
-                        for key, val in tr.defaultParams.items():
-                            trParams[key] = config.get(configData, name, key,
-                                                       default=val)
-                    tmp['transformParams'] = trParams
+                    tmp['transformParams'] = getTransformParams(configData)
+                    tmp['fitParams'] = getFitParams(configData)
                     if isinstance(madeOf, dict):
                         tmp['dataFormat'] = {}
                         name = tmp.pop('madeOf')
                     elif isinstance(madeOf, (list, tuple)):
                         name = tmp.pop('madeOf')
                         tmp['shouldLoadNow'] = False
                         # for spName in madeOf:
@@ -923,18 +947,18 @@
         if csi.withGUI:
             group.init_colors(group.childItems)
 
         return group
 
     def read_file(self):
         madeOf = self.madeOf
-        toNode = csi.nodes[self.originNodeName]
+        fromNode = csi.nodes[self.originNodeName]
         df = dict(self.dataFormat)
         df.update(csi.extraDataFormat)
-        formatSection = 'Format_' + toNode.name
+        formatSection = 'Format_' + fromNode.name
         config.configLoad[formatSection] = dict(df)
 
         arr = []
         if self.dataType == cco.DATA_COLUMN_FILE:
             header = cco.get_header(madeOf, df)
         elif self.dataType == cco.DATA_DATASET:
             header = []
@@ -963,37 +987,37 @@
             raise TypeError('wrong datafile type')
 
         try:
             df['skip_header'] = df.pop('skiprows', 0)
             dataSource = df.pop('dataSource', None)
             sliceStrs = df.pop('slices', ['' for ds in dataSource])
             conversionFactors = df.pop('conversionFactors',
-                                       [None for arr in toNode.arrays])
+                                       [None for arr in fromNode.arrays])
             df.pop('metadata', None)
             if dataSource is None:
                 raise ValueError('bad dataSource settings')
             if self.dataType == cco.DATA_COLUMN_FILE:
                 with warnings.catch_warnings():
                     warnings.simplefilter("ignore")
                     arrs = np.genfromtxt(madeOf, unpack=True, **df)
                 if len(arrs) == 0:
                     raise ValueError('bad data file')
 
-            roles = toNode.get_arrays_prop('role')
+            roles = fromNode.get_arrays_prop('role')
 
             # Create optional arrays and assign None.
             # This loop is needed when dataSource list is shorter than arrays.
-            for aName, role in zip(toNode.arrays, roles):
-                setName = toNode.get_prop(aName, 'raw')
+            for aName, role in zip(fromNode.arrays, roles):
+                setName = fromNode.get_prop(aName, 'raw')
                 if role == 'optional':
                     setattr(self, setName, None)
 
             for aName, txt, sliceStr, role in zip(
-                    toNode.arrays, dataSource, sliceStrs, roles):
-                setName = toNode.get_prop(aName, 'raw')
+                    fromNode.arrays, dataSource, sliceStrs, roles):
+                setName = fromNode.get_prop(aName, 'raw')
                 if (role == 'optional') and (txt == ''):
                     setattr(self, setName, None)
                     continue
                 try:
                     if self.dataType == cco.DATA_COLUMN_FILE:
                         if isinstance(txt, int):
                             arr = arrs[txt]
@@ -1010,18 +1034,18 @@
                             else:
                                 sliceTuple = tuple(
                                     cco.parse_slice_str(slc)
                                     for slc in sliceStr.split(','))
                                 arr = arr[sliceTuple]
                     setattr(self, setName, arr)
                 except Exception as e:
-                    print(e)
                     setattr(self, setName, None)
+                    raise ValueError(e)
 
-            self.state[toNode.name] = cco.DATA_STATE_GOOD
+            self.state[fromNode.name] = cco.DATA_STATE_GOOD
         except (ValueError, OSError, IndexError) as e:
             print('Error in read_file(): {0}'.format(e))
             self.state = dict((n, cco.DATA_STATE_NOTFOUND) for n in csi.nodes)
             return
 
         self.convert_units(conversionFactors)
         # define metadata
@@ -1044,15 +1068,15 @@
         start = 5 if self.madeOf.startswith('silx:') else 0
         end = self.madeOf.find('::') if '::' in self.madeOf else None
         path = self.madeOf[start:end]
         abspath = osp.abspath(path).replace('\\', '/')
         toSave = self.madeOf[:start] + abspath
         if end is not None:
             toSave += self.madeOf[end:]
-        config.put(config.configLoad, 'Data', toNode.name, toSave)
+        config.put(config.configLoad, 'Data', fromNode.name, toSave)
         config.write_configs('transform')
 
     def interpret_array_formula(self, colStr, treeObj=None):
         if "np." in colStr:
             try:
                 arr = eval(colStr)
                 return arr
@@ -1064,15 +1088,16 @@
         except Exception:
             pass
 
         keys = re.findall(r'\[(.*?)\]', colStr)
         if len(keys) == 0:
             if "Col" in colStr:
                 regex = re.compile('Col([0-9]*)')
-                subkeys = regex.findall(colStr)
+                # remove possible duplicates by list(dict.fromkeys())
+                subkeys = list(dict.fromkeys(regex.findall(colStr)))
                 keys = ['Col'+ch for ch in subkeys]
                 for ch in subkeys:
                     colStr = colStr.replace('Col'+ch, 'd["Col{0}"]'.format(ch))
             else:
                 keys = [colStr]
                 colStr = 'd[r"{0}"]'.format(colStr)
         else:
@@ -1098,19 +1123,19 @@
                 d[kn] = d[k]
                 locals()[k] = k
         return eval(colStr)
 
     def convert_units(self, conversionFactors):
         if not conversionFactors:
             return
-        toNode = csi.nodes[self.originNodeName]
-        for aName, cFactor in zip(toNode.arrays, conversionFactors):
+        fromNode = csi.nodes[self.originNodeName]
+        for aName, cFactor in zip(fromNode.arrays, conversionFactors):
             if not cFactor:
                 continue
-            setName = toNode.get_prop(aName, 'raw')
+            setName = fromNode.get_prop(aName, 'raw')
             arr = getattr(self, setName)
             try:
                 if isinstance(cFactor, str):
                     if cFactor.startswith('transpose'):
                         axes = eval(cFactor[9:])
                         setattr(self, setName, arr.transpose(*axes))
                     elif cFactor.startswith('f'):
@@ -1148,21 +1173,21 @@
 
 #        self.meta['modified'] = osp.getmtime(madeOf)
         self.meta['modified'] = time.strftime("%a, %d %b %Y %H:%M:%S")
         self.meta['size'] = -1
 
         try:
             assert isinstance(madeOf, (list, tuple))
-            toNode = csi.nodes[self.originNodeName]
+            fromNode = csi.nodes[self.originNodeName]
 
             # if no 'raw' present, returns arrayName itself:
-            dNames = toNode.get_arrays_prop('raw')
-            xNames = toNode.get_arrays_prop('raw', role='x') +\
-                toNode.get_arrays_prop('raw', role='0D')
-            dims = toNode.get_arrays_prop('ndim')
+            dNames = fromNode.get_arrays_prop('raw')
+            xNames = fromNode.get_arrays_prop('raw', role='x') +\
+                fromNode.get_arrays_prop('raw', role='0D')
+            dims = fromNode.get_arrays_prop('ndim')
 
             # check equal shape of data to combine:
             shapes = [None]*4
             for dName, dim in zip(dNames, dims):
                 if 1 <= dim <= 3:
                     for data in madeOf:
                         if getattr(data, dName) is None:  # optional
@@ -1177,18 +1202,17 @@
                 if self not in data.combinesTo:
                     data.combinesTo.append(self)
 
             ns = len(madeOf)
             # x and 0D as average over all contributing spectra:
             for arrayName in xNames:
                 sumx = 0
-                setName = toNode.get_prop(arrayName, 'raw')
                 for data in madeOf:
-                    sumx += np.array(getattr(data, setName))
-                setattr(self, setName, sumx/ns)
+                    sumx += np.array(getattr(data, arrayName))
+                setattr(self, arrayName, sumx/ns)
 
             dimArray = None
             for arrayName, dim in zip(dNames, dims):
                 if arrayName in xNames:
                     continue
                 if what in (cco.COMBINE_AVE, cco.COMBINE_SUM, cco.COMBINE_RMS):
                     arrays = [getattr(data, arrayName) for data in madeOf]
@@ -1206,30 +1230,30 @@
                         s2 = sum((a-s/ns)**2 for a in arrays if a is not None)
                         v = (s2 / ns)**0.5
                 elif what == cco.COMBINE_PCA:
                     raise NotImplementedError  # TODO
                 else:
                     raise ValueError("unknown data combination")
                 setattr(self, arrayName, v)
-                if dim == toNode.plotDimension:
+                if dim == fromNode.plotDimension:
                     dimArray = v
 
             self.meta['length'] = len(dimArray) if dimArray is not None else 0
-            self.state[toNode.name] = cco.DATA_STATE_GOOD
+            self.state[fromNode.name] = cco.DATA_STATE_GOOD
         except AssertionError:
-            self.state[toNode.name] = cco.DATA_STATE_MATHERROR
+            self.state[fromNode.name] = cco.DATA_STATE_MATHERROR
             msg = '\nThe conbined arrays have different lengths'
             self.meta['text'] += msg
             if csi.DEBUG_LEVEL > 50:
                 print('calc_combined', self.alias, msg)
 
     @logger(minLevel=50, attrs=[(0, 'alias')])
     def branch_data(self):
         """Case of *madeOf* as dict, when branching out."""
-        toNode = csi.nodes[self.originNodeName]
+        fromNode = csi.nodes[self.originNodeName]
         try:
             for key, value in self.madeOf.items():
                 if isinstance(value, np.ndarray):
                     setattr(self, key, value)
                 elif isinstance(value, str):
                     base = self.get_top().find_data_item(value)
                     try:
@@ -1237,46 +1261,56 @@
                     except Exception:
                         pass
                     self.meta = base.meta
                     if base.branch is None:
                         base.branch = self.parentItem
                 else:
                     raise ValueError('unknown data type')
-            self.state[toNode.name] = cco.DATA_STATE_GOOD
+            self.state[fromNode.name] = cco.DATA_STATE_GOOD
 
         except Exception as e:
             print('Exception in "branch_data()" for "{0}":'.format(
                 self.alias), e)
-            self.state[toNode.name] = cco.DATA_STATE_BAD
+            self.state[fromNode.name] = cco.DATA_STATE_BAD
 
     @logger(minLevel=50, attrs=[(0, 'alias')])
     def create_data(self):
         """Case of *madeOf* as callable"""
-        toNode = csi.nodes[self.originNodeName]
+        fromNode = csi.nodes[self.originNodeName]
         try:
             res = self.madeOf(self, **self.dataFormat)
             if res is not None:
-                for arrayName, arr in zip(toNode.arrays, res):
-                    setName = toNode.get_prop(arrayName, 'raw')
+                for arrayName, arr in zip(fromNode.arrays, res):
+                    setName = fromNode.get_prop(arrayName, 'raw')
                     setattr(self, setName, arr)
-            self.state[toNode.name] = cco.DATA_STATE_GOOD
+            self.state[fromNode.name] = cco.DATA_STATE_GOOD
         except Exception as e:
             print('Exception in "create_data":', e)
-            self.state[toNode.name] = cco.DATA_STATE_BAD
+            self.state[fromNode.name] = cco.DATA_STATE_BAD
 
     def save_transform_params(self):
         dtparams = self.transformParams
         for tr in csi.transforms.values():
             for key in tr.defaultParams:
                 if isinstance(dtparams[key], np.ndarray):
                     toSave = dtparams[key].tolist()
                 else:
                     toSave = dtparams[key]
                 config.put(config.configTransforms, tr.name, key, str(toSave))
 
+    def save_fit_params(self):
+        dtparams = self.fitParams
+        for fit in csi.fits.values():
+            for key in fit.defaultParams:
+                if isinstance(dtparams[key], np.ndarray):
+                    toSave = dtparams[key].tolist()
+                else:
+                    toSave = dtparams[key]
+                config.put(config.configFits, fit.name, key, str(toSave))
+
     def save_to_project(self, configProject, dirname):
         from ..gui import gcommons as gco  # only needed with gui
         item = self
         if ((isinstance(item.madeOf, str) and item.dataFormat) or
                 isinstance(item.madeOf, (list, tuple, dict))):
             if isinstance(item.madeOf, str):
                 start = 5 if item.madeOf.startswith('silx:') else 0
@@ -1297,15 +1331,15 @@
                 dataFormatCopy = copy.deepcopy(item.dataFormat)
                 dataSource = list(dataFormatCopy.get('dataSource', []))
                 if 'conversionFactors' in dataFormatCopy:
                     if dataFormatCopy['conversionFactors'] == \
                             [None for ds in dataSource]:  # all None's
                         dataFormatCopy.pop('conversionFactors', None)
                 for ids, ds in enumerate(dataSource):
-                    if 'silx:' in ds:
+                    if isinstance(ds, str) and 'silx:' in ds:
                         start = 5
                         end = ds.find('::') if '::' in ds else None
                         path = ds[start:end]
                         abspath = osp.abspath(path).replace('\\', '/')
                         dsabs = ds[:start] + abspath + ds[end:]
                         ind = dataFormatCopy['dataSource'].index(ds)
                         dataFormatCopy['dataSource'][ind] = dsabs
@@ -1323,28 +1357,28 @@
                 config.put(configProject, item.alias, 'dataFormat', dataFormat)
             elif isinstance(item.madeOf, dict):
                 config.put(configProject, item.alias, 'madeOf',
                            str(item.madeOf))
 
             dataSource = list(item.dataFormat.get('dataSource', []))
             for ds in dataSource:
-                if 'silx:' in ds:
+                if isinstance(ds, str) and 'silx:' in ds:
                     needRelative = True
                     break
             else:
                 needRelative = False
             if needRelative:
                 dataFormatRel = copy.deepcopy(item.dataFormat)
                 dataSourceRel = dataFormatRel['dataSource']
                 if 'conversionFactors' in dataFormatRel:
                     if dataFormatRel['conversionFactors'] == \
                             [None for ds in dataSourceRel]:  # all None's
                         dataFormatRel.pop('conversionFactors', None)
                 for ids, ds in enumerate(dataSourceRel):
-                    if 'silx:' in ds:
+                    if isinstance(ds, str) and 'silx:' in ds:
                         start = 5
                         end = ds.find('::') if '::' in ds else None
                         path = ds[start:end]
                         relpath = osp.relpath(path, dirname).replace('\\', '/')
                         madeOfRel = ds[:start] + relpath + ds[end:]
                         dataSourceRel[ids] = madeOfRel
                 dataFormat = json.dumps(dataFormatRel)
@@ -1379,14 +1413,30 @@
             for key in dtparams:
                 if isinstance(dtparams[key], np.ndarray):
                     toSave = dtparams[key].tolist()
                 else:
                     toSave = dtparams[key]
                 config.put(configProject, item.alias, key, str(toSave))
 
+            noFitsSoFar = True
+            dtparams = item.fitParams
+            for fit in csi.fits.values():
+                if dtparams[fit.ioAttrs['result']] == fit.defaultResult:
+                    continue
+                if noFitsSoFar:
+                    configProject.set(
+                        item.alias, ';fit params:')  # ';'=comment out
+                    noFitsSoFar = False
+                for key in fit.defaultParams:
+                    if isinstance(dtparams[key], np.ndarray):
+                        toSave = dtparams[key].tolist()
+                    else:
+                        toSave = dtparams[key]
+                    config.put(configProject, item.alias, key, str(toSave))
+
         elif isinstance(item.madeOf, str) and not item.dataFormat:
             # i.e. is a group
             config.put(
                 configProject, item.alias, 'colorPolicy',
                 gco.COLOR_POLICY_NAMES[item.colorPolicy])
             if item.colorPolicy == gco.COLOR_POLICY_GRADIENT:
                 config.put(
@@ -1431,14 +1481,15 @@
                                           self.branch.child_count()+1),
                 originNodeName=nodeStart, transformNames=transformNames,
                 runDownstream=False)
             dictToTransfer = {key: self.alias for key in toTransfer}
             newItem = self.branch.insert_item(
                 dictToTransfer, self.branch.child_count(), **kw)
             newItem.transformParams = self.transformParams
+            newItem.fitParams = self.fitParams
             newItem.meta = self.meta
             newItem.colorTag = 4
         self.init_colors(self.branch.childItems)
         for newItem in self.branch.childItems:
             newItem.state[nodeStart] = cco.DATA_STATE_GOOD
             for key in toTransfer:
                 setattr(newItem, key, getattr(self, key))
```

## Comparing `parseq-1.0.0/parseq/core/transforms.py` & `parseq-2023.5.0/parseq/core/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 u"""
 Data transformations
 --------------------
 
 Data transformations provide values for all the arrays defined in one
-transformation node given arrays defined in another transformation node. Each
-transformation defines a dictionary of transformation parameters; the values of
-these parameters are individual per data item. Each transformation in a
-pipeline requires subclassing from :class:`Transform`.
+transformation node (`fromNode`) given arrays defined in another transformation
+node (`toNode`). Each transformation defines a dictionary of transformation
+parameters; the values of these parameters are individual per data item. Each
+transformation in a pipeline requires subclassing from :class:`Transform`.
 """
 __author__ = "Konstantin Klementiev"
 __date__ = "17 Feb 2023"
 # !!! SEE CODERULES.TXT !!!
 
 import sys
 # import os
@@ -424,14 +424,16 @@
         progress will be visualized as an expanding colored background
         rectangle in the data tree. Quick transformations do not need progress
         reporting.
 
         Should an error happen during the transformation, the error state will
         be notified in the ParSeq status bar and the traceback will be shown in
         the data item's tooltip in the data tree view.
+
+        Returns True when successful.
         """
         raise NotImplementedError  # must be overridden
 
     def run_post(self, dataItems, runDownstream=True):
         # do data.calc_combined() if a member of data.combinesTo has
         # its originNode as toNode:
         toBeUpdated = []
@@ -689,30 +691,32 @@
             itemsByOrigin[it.originNodeName] = [it]
         else:
             itemsByOrigin[it.originNodeName].append(it)
 
     for originNodeName, its in itemsByOrigin.items():
         for tr in csi.nodes[originNodeName].transformsOut:
             # first bottomItems, then topItems...:
-            if (csi.transformer is not None) and len(itemsByOrigin) == 1:
+            if (csi.tasker is not None) and len(itemsByOrigin) == 1:
                 # with a threaded transform
-                csi.transformer.prepare(tr, dataItems=its, starter=tr.widget)
-                csi.transformer.thread().start()
+                csi.tasker.prepare(
+                    tr, runDownstream=True, dataItems=its, starter=tr.widget)
+                csi.tasker.thread().start()
             else:
                 # if len(itemsByOrigin) > 1, the transforms cannot be
                 # parallelized, so do it in the same thread:
                 tr.run(dataItems=its)
                 if hasattr(tr, 'widget'):  # when with GUI
                     tr.widget.replotAllDownstream(tr.name)
             if tr.fromNode is tr.toNode:
                 break
 
             # # no need for dependentItems, it is invoked in run_post:
             # # ...then dependentItems:
             # if len(csi.transforms.values()) > 0:
-            #     if csi.transformer is not None:  # with a threaded transform
-            #         csi.transformer.prepare(
-            #             tr, dataItems=dependentItems, starter=tr.widget)
-            #         csi.transformer.thread().start()
+            #     if csi.tasker is not None:  # with a threaded transform
+            #         csi.tasker.prepare(
+            #             tr, runDownstream=True, dataItems=dependentItems,
+            #             starter=tr.widget)
+            #         csi.tasker.thread().start()
             #     else:  # in the same thread
             #         tr.run(dataItems=dependentItems)
             #         tr.widget.replotAllDownstream(tr.name)
```

## Comparing `parseq-1.0.0/parseq/core/__init__.py` & `parseq-2023.5.0/parseq/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,32 @@
 values are supposed to be changed in user supplied GUI widgets. This change can
 be done simultaneously for one or several active data objects. Alternatively,
 any parameter can be copied to one or several later selected data.
 
 Each transformation can optionally define the number of threads or processes
 that will start in parallel and run the transformation of several data items.
 The multiprocessing python API requires the main transformation method as a
-*static* method (not an instance method). Additionally, for the sake of
-multiprocessing, all input and output arrays have to be added to ``inArrays``
-and ``outArrays`` lists (attributes of the transformation class).
+*static* or *class* method (not an instance method). Additionally, for the sake
+of data transfer in multiprocessing, all input and output arrays have to be
+added to ``inArrays`` and ``outArrays`` lists (attributes of the transformation
+class).
 
 In the user-supplied GUI widgets, one for each data node, all interactive GUI
 elements should get registered using a few dedicated methods. The registration
 will enable automatic GUI update from the active data and will run
 transformations given the updated parameters, so no
 `signal slots <https://doc.qt.io/qt-6/signalsandslots.html>`_
 are typically required. The registration will also enable copying
 transformation parameters to other data by means of popup menus on each GUI
 element.
 
+One or more curve fitting routines can optionally be defined per data node.
+Similarly to transformations, fitting solvers can run in parallel for several
+data items. Fitting parameters can be constrained or tied to other parameters.
+
 The data model is a single object throughout the pipeline. Data can be
 rearranged by the user: ordered, renamed, grouped and removed. The data model
 tree is present in *each* data node, not as a single tree instance, with the
 idea also to serve as a plot legend that should always be close to the plot.
 User selection in the data model is common for all transformation nodes. For 1D
 data, the line color is the same in all data nodes. 1D data plotting can
 optionally be done for dynamically (via mouse selection) or statically (via
@@ -108,19 +113,26 @@
 Because each transformation already has a set of default parameter values,
 these GUI widgets can gradually grow during the development time, without
 compromising the data pipeline functionality.
 
 Provide docstrings in reStructuredText markup, they will be built by Sphinx and
 displayed near the corresponding widgets.
 
+Make fitting worker classes
+---------------------------
+
+Similarly to a transformation class, a fitting class defines a dictionary
+`defaultParams`, defines multiprocessing/multithreading and a static or a class
+method :meth:`.Fit.run_main`.
+
 Make data pipeline
 ------------------
 
-This is a small module that instantiates the above nodes, transformations and
-widgets and connects them together.
+This is a small module that instantiates the above nodes, transformations, fits
+and widgets and connects them together.
 
 Create test data tree
 ---------------------
 
 Put a few data files in a local folder (i.e. `data`) and create a module that
 defines a function that loads the data into a :ref:`data tree <data>`, defines
 suitable transformation parameters and launches the first transformation (the
```

## Comparing `parseq-1.0.0/parseq/gui/aboutDialog.py` & `parseq-2023.5.0/parseq/gui/aboutDialog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 __author__ = "Konstantin Klementiev"
-__date__ = "26 Feb 2023"
+__date__ = "28 May 2023"
 # !!! SEE CODERULES.TXT !!!
 
 import os
 import os.path as osp
+import numpy as np
 import re
 import sphinx
 from silx.gui import qt
 from silx import version as versilx
 import platform as pythonplatform
 import webbrowser
 
@@ -71,16 +72,16 @@
         layout.addWidget(self.webView)
         self.setLayout(layout)
         self.resize(0, 0)
 
     def makeWebView(self):
         self.webView = gww.QWebView(self)
         self.webView.page().setLinkDelegationPolicy(2)
-        self.webView.setMinimumWidth(550)
-        self.webView.setMinimumHeight(550+30*len(csi.nodes))
+        self.webView.setMinimumWidth(560)
+        self.webView.setMinimumHeight(450+30*len(csi.nodes))
         self.webView.history().clear()
         self.webView.page().history().clear()
         self.lastBrowserLink = ''
         self.webView.page().linkClicked.connect(
             self.linkClicked, type=qt.Qt.UniqueConnection)
 
         self.sphinxThread = qt.QThread(self)
@@ -124,14 +125,15 @@
                           " distro string")
         if isOpenCL:
             vercl = cl.VERSION
             if isinstance(vercl, (list, tuple)):
                 vercl = '.'.join(map(str, vercl))
         else:
             vercl = isOpenStatus
+        strNumpy = r'numpy {0}'.format(np.__version__)
         strOpenCL = r'pyopencl {0}'.format(vercl)
         strSphinx = 'Sphinx {0}'.format(sphinx.__version__)
         strSilx = r'silx {0}'.format(versilx)
         strParSeq = '{0}'.format(PARSEQPATH).replace('\\', '/')
         if type(self.parseq_pypi_version) is tuple:
             pypiver, curver = self.parseq_pypi_version
             pstr = "`PyPI <https://pypi.python.org/pypi/parseq>`_"
@@ -167,42 +169,54 @@
 :Version:
     {3}
 :Your system:
     {4}, Python {5}\n
     Qt {6}, {7} {8}\n
     {9}\n
     {10}\n
-    {11}""".format(
+    {11}\n
+    {12}""".format(
             parseq.__synopsis__, parseq.__doc__, strParSeq, parseqversion,
             locos, pythonplatform.python_version(),
             Qt_version, qt.BINDING, PyQt_version,
-            strOpenCL, strSphinx, strSilx)
+            strNumpy, strOpenCL, strSphinx, strSilx)
 #        txt = txt.replace('imagezoom::', 'image::')
         return txt
 
     def makeGraphPipeline(self):
         ranks = {}
         for i in range(len(csi.nodes)):
             nodes = []
             transforms = []
             icons = []
+            fits = {}
+            fitIcon = 'icon-fit-32'
             for name, node in csi.nodes.items():
                 if len(node.upstreamNodes) == i:
                     nodes.append(name)
                     if node.plotDimension is None:
                         iName = None
                     elif node.plotDimension < 4:
-                        iName = 'icon-item-{0}dim-32'.format(node.plotDimension)
+                        iName = 'icon-item-{0}dim-32'.format(
+                            node.plotDimension)
                     else:
                         iName = 'icon-item-ndim-32'
                     icons.append(iName)
                     for tr in node.transformsOut:
                         transforms.append(
                             [tr.name, tr.fromNode.name, tr.toNode.name])
-            ranks[i] = dict(nodes=nodes, icons=icons, transforms=transforms)
+                    for fit in csi.fits.values():
+                        if fit.node is node:
+                            if name in fits:
+                                fits[name].append(fit.name)
+                            else:
+                                fits[name] = [fit.name]
+
+            ranks[i] = dict(nodes=nodes, icons=icons, transforms=transforms,
+                            fits=fits)
 
         # ranks = {  # a fake test pipeline
         #     0: {'nodes': ['aaaaa', 'bbbbbbbbb'],
         #         'transforms': [['tr ac jhvcqwvedvsd', 'aaaaa', 'cccc'],
         #                        ['tr bc jhvpyvv', 'bbbbbbbbb', 'cccc'],
         #                        ['tr bb j', 'bbbbbbbbb', 'bbbbbbbbb']],
         #         'icons': ['icon-item-ndim', 'icon-item-ndim']},
@@ -222,15 +236,16 @@
 
         flowChart = """\n
     <div class="pipeline">
     <svg><defs>"""
         for i in range(len(gco.colorCycle1)):
             flowChart += """\n
     <filter id="flt{0}" filterUnits="userSpaceOnUse" id="shadow" x="-2" y="1">
-      <feGaussianBlur in="SourceAlpha" stdDeviation="1.5" result="blur"></feGaussianBlur>
+      <feGaussianBlur in="SourceAlpha" stdDeviation="1.5" result="blur">
+      </feGaussianBlur>
       <feOffset in="blur" dx="1.5" dy="0" result="shadow"></feOffset>
       <feFlood flood-color="{1}99" result="color" />
       <feComposite in="color" in2="shadow" operator="in" />
       <feComposite in="SourceGraphic"/>
     </filter>
     <marker id="arrow{0}" markerWidth="12" markerHeight="8"
     refX="7" refY="4" orient="auto" markerUnits="userSpaceOnUse">
@@ -239,36 +254,46 @@
         flowChart += """\n
     </defs></svg>"""
 
         iline = 0
         for irank, (rank, rankDict) in enumerate(ranks.items()):
             names = rankDict['nodes']
             icons = rankDict['icons']
+            fits = rankDict['fits']
             if not names:
                 continue
             flowChart += """\n      <div class="pipeline-rank">"""
             for name, iName in zip(names, icons):
                 name_ = "_".join(name.split())
                 iconTxt = '' if iName is None else \
                     '<img src="_images/{0}.png" height="20" />'.format(iName)
                 flowChart += u"""\n
-        <div id="pn_{0}" class="pipeline-node">{1} {2}</div>""".format(
+                    <div id="pn_{0}" class="pipeline-node">{1} {2}""".format(
                     name_, iconTxt, name)
+                if name in fits:
+                    ficonTxt = '<img src="_images/{0}.png" height="20" />'\
+                        .format(fitIcon)
+                    for fitName in fits[name]:
+                        flowChart += u"""&nbsp <span id=
+                            "fn_{0}" class="pipeline-fit">{1} {2}</span>"""\
+                                .format(name_, ficonTxt, fitName)
+                flowChart += "</div>"
             flowChart += """\n      </div>"""  # class="pipeline-rank"
 
             transforms = rankDict['transforms']
             if not transforms:
                 continue
             flowChart += """\n      <div class="pipeline-transforms">"""
             if len(transforms) % 2 == 1:
                 flowChart += u"""\n        <div class="pipeline-tr" ></div>"""
             for transform in transforms:
                 iline_ = iline % len(gco.colorCycle1)
                 color = gco.colorCycle1[iline_]
-                colorStr = 'style="color: {0}; text-shadow: 1px 1.5px 3px {0}99;"'\
+                colorStr = \
+                    'style="color: {0}; text-shadow: 1px 1.5px 3px {0}99;"'\
                     .format(color)
                 flowChart += u"""\n        <div class="pipeline-tr" {1}>
                 {0}</div>""".format(transform[0], colorStr)
                 name1_ = "_".join(transform[1].split())
                 name2_ = "_".join(transform[2].split())
                 colorStr = """style="stroke: {0}; """\
                     """marker-end: url(#arrow{1}); filter: url(#flt{1})" """\
```

## Comparing `parseq-1.0.0/parseq/gui/calibrateEnergy.py` & `parseq-2023.5.0/parseq/gui/calibrateEnergy.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/columnFormat.py` & `parseq-2023.5.0/parseq/gui/columnFormat.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/combineSpectra.py` & `parseq-2023.5.0/parseq/gui/combineSpectra.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/dataRebin.py` & `parseq-2023.5.0/parseq/gui/dataRebin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,21 @@
 # -*- coding: utf-8 -*-
 __author__ = "Konstantin Klementiev"
 __date__ = "28 Oct 2022"
 # !!! SEE CODERULES.TXT !!!
 
 from silx.gui import qt
+from .gcommons import getFormatStr, getDecimals
 
 ROWHEIGHT = 24
 HEADERHEIGHT = 28
 DOTSIZE = 2, 4
 DOTDELTA = 1
 
 
-def getFormatStr(step):
-    if 0.1 <= step < 1:
-        return '{0:.1f}'
-    elif 0.01 <= step < 0.1:
-        return '{0:.2f}'
-    elif 0.001 <= step < 0.01:
-        return '{0:.3f}'
-    elif 0.0001 <= step < 0.001:
-        return '{0:.4f}'
-    elif 0.00001 <= step < 0.0001:
-        return '{0:.5f}'
-    else:
-        return '{0:.0f}'
-
-
-def getDecimals(step):
-    if 0.1 <= step < 1:
-        return 1
-    elif 0.01 <= step < 0.1:
-        return 2
-    elif 0.001 <= step < 0.01:
-        return 3
-    elif 0.0001 <= step < 0.001:
-        return 4
-    elif 0.00001 <= step < 0.0001:
-        return 5
-    else:
-        return 0
-
-
 def formatted(region):  # region: label, value, min, max, step
     if len(region) < 5:
         return ''
     val = region[1]
     if isinstance(val, (float, int)):
         step = region[4]
         fmt = getFormatStr(step)
```

## Comparing `parseq-1.0.0/parseq/gui/dataTreeModelView.py` & `parseq-2023.5.0/parseq/gui/dataTreeModelView.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,19 +236,27 @@
         self.selectItems(items)
         return items
 
     def selectItems(self, items=None):
         mode = qt.QItemSelectionModel.Select | qt.QItemSelectionModel.Rows
         if items is None:
             items = self.rootItem.get_items()
-        for item in items:
+        elif not isinstance(items, (list, tuple)):
+            items = [items]
+        for i, item in enumerate(items):
             row = item.row()
             index = self.createIndex(row, 0, item)
-            csi.selectionModel.select(index, mode)
-            csi.selectionModel.setCurrentIndex(index, mode)
+            if i == 0:
+                selection = qt.QItemSelection(index, index)
+            else:
+                selection.select(index, index)
+        csi.selectionModel.select(selection, mode)
+        csi.selectionModel.setCurrentIndex(index, mode)
+        csi.selectedItems[:] = []
+        csi.selectedItems.extend(items)
 
     def _removeFromGlobalLists(self, item):
         for ll in (csi.selectedItems, csi.selectedTopItems,
                    csi.recentlyLoadedItems, csi.allLoadedItems):
             if item in ll:
                 ll.remove(item)
```

## Comparing `parseq-1.0.0/parseq/gui/fileDialogs.py` & `parseq-2023.5.0/parseq/gui/fileDialogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.saveData.setLayout(layoutC)
         self.layout().addWidget(
             self.saveData, self.layout().rowCount(), 0, 1, 2)
         self.layout().setRowStretch(self.layout().rowCount(), 0)
 
         self.finished.connect(self.onFinish)
 
-        self.setMinimumHeight(500)
+        self.setMinimumSize(1000, 700)
 
     def onFinish(self, result):
         if not result:
             return
         resFile = self.selectedFiles()
         saveData = self.saveData.isChecked()
         if not saveData:
@@ -214,26 +214,30 @@
 
         configProject = config.ConfigParser()
         try:
             configProject.read(path, encoding=config.encoding)
             self.previewPanel.groups = int(configProject.get('Root', 'groups'))
             self.previewPanel.items = int(configProject.get('Root', 'items'))
             active = config.get(configProject, 'Docks', 'active', '')
-            self.previewPanel.pmIndex = list(csi.nodes.keys()).index(active)
         except Exception:
             pass
 
+        self.previewPanel.pmIndex = 0
         self.previewPanel.pms = []
         self.previewPanel.pmNames = []
+        curInd = 0
         for i, (name, node) in enumerate(csi.nodes.items()):
             pngName = fname + '-{0}-{1}.png'.format(i+1, name)
             pmName = u'{0} \u2013 {1}'.format(i+1, name)
             if os.path.exists(pngName):
                 self.previewPanel.pms.append(qt.QPixmap(pngName))
                 self.previewPanel.pmNames.append(pmName)
+                if name == active:
+                    self.previewPanel.pmIndex = curInd
+                curInd += 1
         self.previewPanel.updatePreview()
 
     def onFinish(self, result):
         if not result:
             return
         resFile = self.selectedFiles()
         self.ready.emit([resFile])
```

## Comparing `parseq-1.0.0/parseq/gui/fileTreeModelView.py` & `parseq-2023.5.0/parseq/gui/fileTreeModelView.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,15 +438,16 @@
         dataStr = [s.strip() for s in dataStr.split(',')]
         out = []
         for colStr in dataStr:
             keys = re.findall(r'\[(.*?)\]', colStr)
             if len(keys) == 0:
                 if "Col" in colStr:
                     regex = re.compile('Col([0-9]*)')
-                    subkeys = regex.findall(colStr)
+                    # remove possible duplicates by list(dict.fromkeys())
+                    subkeys = list(dict.fromkeys(regex.findall(colStr)))
                     keys = ['Col'+ch for ch in subkeys]
                     colStrD = str(colStr)
                     for ch in subkeys:
                         colStrD = colStrD.replace(
                             'Col'+ch, 'd["Col{0}"]'.format(ch))
                 else:
                     keys = [colStr]
@@ -512,31 +513,35 @@
         lres = []
         try:
             cdf = df.copy()
             cco.get_header(fname, cdf)
             cdf['skip_header'] = cdf.pop('skiprows', 0)
             dataS = cdf.pop('dataSource', [])
             roles = self.transformNode.get_arrays_prop('role')
+            nds = self.transformNode.get_arrays_prop('ndim')
             cdf.pop('conversionFactors', [])
             cdf.pop('metadata', [])
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 arrs = np.genfromtxt(fname, unpack=True, max_rows=2, **cdf)
             if len(arrs) == 0:
                 return
 
-            for data, role in zip(dataS, roles):
+            for data, nd, role in zip(dataS, nds, roles):
                 if role == 'optional':
                     lres.append('')
                     continue
                 if len(data) == 0:
                     return
                 colEval = self.interpretArrayFormula(data, arrs, 'col')
                 if colEval is None:
                     return
+                if nd:
+                    if len(colEval[0][3]) < nd:
+                        return
                 lres.append(colEval)
         except Exception:  # as e:
             # print('tryLoadColDataset:', e)
             return
         return lres, df
 
     def tryLoadHDF5Dataset(self, indexH5):
@@ -554,18 +559,18 @@
         if not df:
             return
 
         lres = []
         try:
             datas = df.get('dataSource', [])  # from dataEdits
             roles = self.transformNode.get_arrays_prop('role')
+            nds = self.transformNode.get_arrays_prop('ndim')
             slcs = df.get('slices', ['' for ds in datas])  # from sliceEdits
             for idata, (data, slc, nd, role) in enumerate(zip(
-                datas, slcs, self.transformNode.get_arrays_prop('ndim'),
-                    roles)):
+                    datas, slcs, nds, roles)):
                 if role == 'optional':
                     lres.append('')
                     continue
                 if len(data) == 0:
                     return
                 colEval = self.interpretArrayFormula(data, nodeH5, 'h5')
                 if colEval is None:
@@ -779,14 +784,16 @@
                     continue
                 if re.search(filt.replace('*', '+'), fileName):
                     return qt.QModelIndex()
         return indexFS
 
     def reloadHdf5(self, index):
         h5pyObject = self.data(index, role=H5PY_OBJECT_ROLE)
+        if h5pyObject is None:
+            return
         if isinstance(h5pyObject, type('')):
             filename = h5pyObject
         else:
             filename = h5pyObject.file.filename
         indexFS = self.indexFileName(filename)
         indexH5 = self.mapFStoH5(indexFS)
 
@@ -1321,15 +1328,15 @@
                     urls.append(model.getHDF5FullPath(ind))
         return urls
 
     def getActiveDir(self, path=None):  # used in autoLoad
         if path is None:
             sIndexes = self.selectionModel().selectedRows()
             if len(sIndexes) == 0:
-                return
+                return '', []
             model, ind = self.getSourceModel(sIndexes[0])
         else:
             model = self.getSourceModel()
             if path.startswith('silx:'):
                 if path.endswith('::/'):
                     ind = model.indexFileName(path[5:-3])
                 else:
```

## Comparing `parseq-1.0.0/parseq/gui/gcommons.py` & `parseq-2023.5.0/parseq/gui/gcommons.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,14 +27,58 @@
 BUSY_COLOR_BGND = qt.QColor('#ffe9a1')
 BUSY_COLOR_FGND = qt.QColor('#aaaa00')
 BAD_COLOR = qt.QColor('#f47070')
 UNDEFINED_COLOR = qt.QColor('#cccccc')
 NOTFOUND_COLOR = qt.QColor('#ff88ff')
 MATHERROR_COLOR = qt.QColor('#ffa500')
 
+LIMITS_ROLE = qt.Qt.UserRole + 1
+
+
+def getFormatStr(step):
+    if 0.1 <= step < 1:
+        return '{0:.1f}'
+    elif 0.01 <= step < 0.1:
+        return '{0:.2f}'
+    elif 0.001 <= step < 0.01:
+        return '{0:.3f}'
+    elif 0.0001 <= step < 0.001:
+        return '{0:.4f}'
+    elif 0.00001 <= step < 0.0001:
+        return '{0:.5f}'
+    elif 0.000001 <= step < 0.00001:
+        return '{0:.6f}'
+    elif 0.0000001 <= step < 0.000001:
+        return '{0:.7f}'
+    elif 0.00000001 <= step < 0.0000001:
+        return '{0:.8f}'
+    else:
+        return '{0}'
+
+
+def getDecimals(step):
+    if 0.1 <= step < 1:
+        return 1
+    elif 0.01 <= step < 0.1:
+        return 2
+    elif 0.001 <= step < 0.01:
+        return 3
+    elif 0.0001 <= step < 0.001:
+        return 4
+    elif 0.00001 <= step < 0.0001:
+        return 5
+    elif 0.000001 <= step < 0.00001:
+        return 6
+    elif 0.0000001 <= step < 0.000001:
+        return 7
+    elif 0.00000001 <= step < 0.0000001:
+        return 8
+    else:
+        return 0
+
 
 def makeGradientCollection(color1, color2, ncolor=8):
     c1 = np.array(qt.QColor(color1).getHsvF())
     c2 = np.array(qt.QColor(color2).getHsvF())
     c1[c1 < 0] = 0  # for gray, getHsvF returns hue=-1 that is not accepted by fromHsv  # noqa
     c2[c2 < 0] = 0
     t = np.linspace(0, 1, ncolor)[:, np.newaxis]
@@ -45,14 +89,41 @@
     return res
 
 
 def getColorName(color):
     return qt.QColor(color).name()
 
 
+class CheckBoxDelegate(qt.QItemDelegate):
+    """
+    The standard checkbox (of items with Qt.ItemIsUserCheckable) without text
+    draws an empty focus rectangle on the right of the checkbox. This delegate
+    draws only a centered check box.
+    """
+
+    def __init__(self, parent=None):
+        self.defSize = qt.QSize(
+            qt.QApplication.style().pixelMetric(qt.QStyle.PM_IndicatorWidth),
+            qt.QApplication.style().pixelMetric(qt.QStyle.PM_IndicatorHeight))
+        super().__init__(parent)
+
+    def paint(self, painter, option, index):
+        left = option.rect.center().x() - self.defSize.width()//2
+        top = option.rect.center().y() - self.defSize.height()//2
+        rect = qt.QRect(left, top, self.defSize.width(), self.defSize.height())
+        self.drawCheck(painter, option, rect, index.data(qt.Qt.CheckStateRole))
+
+    def editorEvent(self, event, model, option, index):
+        if event.type() == qt.QEvent.MouseButtonRelease:
+            value = index.data(qt.Qt.CheckStateRole)
+            model.setData(index, not value, qt.Qt.CheckStateRole)
+            return True
+        return super().editorEvent(event, model, option, index)
+
+
 class MultiLineEditDelegate(qt.QStyledItemDelegate):
     def createEditor(self, parent, option, index):
         edit = qt.QTextEdit(parent)
         edit.setVerticalScrollBarPolicy(qt.Qt.ScrollBarAlwaysOff)
         return edit
 
     def setEditorData(self, editor, index):
@@ -77,14 +148,47 @@
         return False
 
     # def updateEditorGeometry(self, editor, option, index):
     #     editor.setGeometry(option.rect.x(), option.rect.y(),
     #                        option.rect.width(), option.rect.height()-10)
 
 
+class DoubleSpinBoxDelegate(qt.QStyledItemDelegate):
+    """
+    This delegate ctreates a QDoubleSpinBox and sets its limits and step as got
+    from the model's data with a role LIMITS_ROLE.
+    """
+
+    def __init__(self, parent, alignment):
+        super().__init__(parent)
+        self.alignment = alignment
+
+    def createEditor(self, parent, option, index):
+        dsb = qt.QDoubleSpinBox(parent)
+        dsb.setAccelerated(True)
+        limits = index.data(role=LIMITS_ROLE)
+        if limits:
+            dsb.setMinimum(float(limits[0]))
+            dsb.setMaximum(float(limits[1]))
+            step = limits[2]
+            dsb.setSingleStep(step)
+            decimals = getDecimals(step)
+            dsb.setDecimals(decimals)
+        dsb.setAlignment(self.alignment)
+        dsb.valueChanged.connect(self.valueChanged)
+        return dsb
+
+    def valueChanged(self):
+        self.commitData.emit(self.sender())
+
+    def updateEditorGeometry(self, editor, option, index):
+        editor.setGeometry(option.rect.x(), option.rect.y(),
+                           option.rect.width(), option.rect.height()-1)
+
+
 class RichTextPushButton(qt.QPushButton):
     def __init__(self, text, parent):
         super().__init__(parent)
         self.__lbl = qt.QLabel(self)
         self.lbl = self.__lbl
         self.__lbl.setText(text)
         self.__lyt = qt.QHBoxLayout()
```

## Comparing `parseq-1.0.0/parseq/gui/mainWindow.py` & `parseq-2023.5.0/parseq/gui/mainWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from ..core import config
 from ..core import singletons as csi
 from ..core import commons as cco
 # from ..core import spectra as csp
 from ..core import save_restore as csr
 from ..gui import undoredo as gur
 from .nodeWidget import NodeWidget
-from .transformer import Transformer
+from .tasker import Tasker
 from .fileDialogs import SaveProjectDlg, LoadProjectDlg
 from .aboutDialog import AboutDialog
 from . import gcommons as gco
 from . import webWidget as gww
 
 # fontSize = 12 if sys.platform == "darwin" else 8.5
 mainWindowWidth, mainWindowHeight = 1600, 768
@@ -144,21 +144,20 @@
         self.runIcon = qt.QIcon(osp.join(self.iconDir, 'parseq.ico'))
         # self.emptyIcon = qt.QIcon(qt.QPixmap.fromImage(qt.QImage.fromData(
         #     b'<svg version="1.1" viewBox="0 0  32"'
         #     b' xmlns="http://www.w3.org/2000/svg"></svg>')))
         # self.emptyIcon = qt.QIcon()
 
         transformThread = qt.QThread(self)
-        csi.transformer = Transformer()
-        csi.transformer.moveToThread(transformThread)
+        csi.tasker = Tasker()
+        csi.tasker.moveToThread(transformThread)
         transformThread.started.connect(
             partial(self.displayStatusMessage, u'calculating…'))
-        transformThread.started.connect(csi.transformer.run)
-        csi.transformer.ready.connect(
-            partial(self.displayStatusMessage, u'ready'))
+        transformThread.started.connect(csi.tasker.run)
+        csi.tasker.ready.connect(partial(self.displayStatusMessage, u'ready'))
         csi.mainWindow = self
         self.setWindowTitle(u"ParSeq  \u2014  " + csi.pipelineName)
         self.helpFile = gww.HELPFILE
 
         self.initTabs()
 
         # self.settings = qt.QSettings('parseq.ini', qt.QSettings.IniFormat)
@@ -645,24 +644,25 @@
         config.put(config.configLoad, 'Project', csi.pipelineName, fname)
 
     def closeEvent(self, event):
         self.timerCPU.stop()
         self.save_perspective()
         if len(csi.selectedItems) > 0:
             csi.selectedItems[0].save_transform_params()
+            csi.selectedItems[0].save_fit_params()
         nodes = csi.nodes.values()
         for node in nodes:
             if hasattr(node.widget.transformWidget, 'properties'):
                 node.widget.transformWidget.save_properties()
         config.write_configs()
         time.sleep(0.1)
         for dock, _, _ in self.docks.values():
             dock.deleteLater()
-        csi.transformer.thread().quit()
-        csi.transformer.deleteLater()
+        csi.tasker.thread().quit()
+        csi.tasker.deleteLater()
         super().closeEvent(event)
 
     def updateItemView(self, state, items):
         if state == 1:
             try:
                 for item in items:
                     ind = csi.model.indexFromItem(item)
```

## Comparing `parseq-1.0.0/parseq/gui/nodeWidget.py` & `parseq-2023.5.0/parseq/gui/nodeWidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     def __init__(self, text, parent, isVertical=False,
                  margin=SPLITTER_BUTTON_MARGIN):
         super().__init__(text, parent)
         self.rawText = str(text)
         self.isVertical = isVertical
         fontSize = "10" if sys.platform == "darwin" else "8.5" \
             if sys.platform == "linux" else "8"
-        grad = "x1: 0, y1: 0, x2: 0, y2: 1"
+        grad = "x1: 0, y1: 1, x2: 0, y2: 0"
         bottomMargin = '-1' if isVertical else '-3'
         self.setStyleSheet("""
             QPushButton {
                 font-size: """ + fontSize + """pt; color: #151575;
                 text-align: bottom; border-radius: 6px;
                 margin: 0px 0px """ + bottomMargin + """px 0px;
                 background-color: qlineargradient(
@@ -119,14 +119,15 @@
         node.widget = self
         self.transformWidget = None
         self.tree = None
         self.help = None
         self.pendingPropDialog = None
         self.wasNeverPlotted = True
         self.onTransform = False
+        self.fitLines = []
 
         self.makeSplitters()
 
         self.fillSplitterFiles()
         self.fillSplitterData()
         self.fillSplitterPlot()
         self.makeTransformWidget(self.splitterTransform)
@@ -161,26 +162,29 @@
     def makeSplitters(self):
         layout = qt.QHBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         self.splitter = qt.QSplitter(self)
         self.splitter.setOrientation(qt.Qt.Horizontal)
         layout.addWidget(self.splitter)
         self.setLayout(layout)
-        grad = "x1: 0, y1: 0, x2: 0, y2: 1"
+        # grad = "x1: 0, y1: 0, x2: 0, y2: 1"
+        # self.splitter.setStyleSheet(
+        #     "QSplitterHandle:hover {} "
+        #     "QSplitter::handle:horizontal:hover{background-color: "
+        #     "qlineargradient(" + grad + ", stop: 0 #6087cefa, "
+        #     "stop: 1 #7097eeff);}")
+        # self.splitter.setStyleSheet(
+        #     "QSplitterHandle:hover {} "
+        #     "QSplitter::handle:horizontal:hover{background-color: #6087cefa;"
+        #     "margin: 5px;}"
+        #     "QSplitter::handle:vertical:hover{background-color: #6087cefa;"
+        #     "margin: 5px;}")
         self.splitter.setStyleSheet(
             "QSplitterHandle:hover {} "
-            "QSplitter::handle:horizontal:hover{background-color: "
-            "qlineargradient(" + grad + ", stop: 0 #6087cefa, "
-            "stop: 1 #7097eeff);}")
-
-        self.splitter.setStyleSheet(
-            "QSplitterHandle:hover {} "
-            "QSplitter::handle:horizontal:hover{background-color: #6087cefa;"
-            "margin: 5px;}"
-            "QSplitter::handle:vertical:hover{background-color: #6087cefa;"
+            "QSplitter::handle:hover{background-color: #6087cefa;"
             "margin: 5px;}")
 
         self.splitterFiles = qt.QSplitter(self.splitter)
         self.splitterFiles.setOrientation(qt.Qt.Vertical)
         self.splitterData = qt.QSplitter(self.splitter)
         self.splitterData.setOrientation(qt.Qt.Vertical)
         self.splitterPlot = qt.QSplitter(self.splitter)
@@ -305,66 +309,25 @@
         self.combiner = CombineSpectraWidget(self.splitterData, self.node)
 
         self.splitterData.setStretchFactor(0, 1)  # don't remove
         self.splitterData.setStretchFactor(1, 0)
         self.splitterData.setSizes([1, 0])
 
     def fillSplitterPlot(self):
-        node = self.node
-        # self.backend = dict(backend='opengl')
-        self.backend = dict(backend='matplotlib')
-
-        if node.plotDimension == 3:
-            self.plot = Plot3D(self.splitterPlot, position=Plot3D.posInfo,
-                               **self.backend)
-            self.plot.setCustomPosInfo()
-            self.plot.setTitleCallback(self.titleCallback3D)
-        elif node.plotDimension == 2:
-            self.plot = Plot2D(self.splitterPlot, **self.backend)
-        elif node.plotDimension == 1:
-            xLbl = node.get_arrays_prop('qLabel', role='x')[0]
-            yLbl = node.get_arrays_prop('qLabel', role='y')[0]
-            hasCustomCursorLabels = False
-            if self.node.widgetClass is not None:
-                if (hasattr(self.node.widgetClass, 'cursorPositionCallback')
-                        and hasattr(self.node.widgetClass, 'cursorLabels')):
-                    hasCustomCursorLabels = True
-            if hasCustomCursorLabels:
-                position = [
-                    (label, partial(
-                        self.node.widgetClass.cursorPositionCallback, label))
-                    for label in self.node.widgetClass.cursorLabels]
-            else:
-                position = [(xLbl, lambda x, y: x), (yLbl, lambda x, y: y)]
-            self.plot = Plot1D(self.splitterPlot, position=position,
-                               **self.backend)
-            self.plot.getXAxis().setLabel(xLbl)
-            self.plot.getYAxis().setLabel(yLbl)
-        else:
-            raise ValueError("wrong plot dimension")
-        self.plotSetup()
-        self.plot.setMinimumWidth(20)
-        self.savedPlotProps = {}
-
-        self.metadata = qt.QTextEdit(self.splitterPlot)
-        self.metadata.setStyleSheet("QTextEdit {border: none;}")
-        self.metadata.setReadOnly(True)
-#        self.metadata.setContentsMargins(0, 0, 0, 0)
-        self.metadata.setMinimumHeight(80)
-        self.metadata.setAlignment(qt.Qt.AlignLeft | qt.Qt.AlignTop)
-        self.metadata.setText("text metadata here")
-        self.metadata.setHorizontalScrollBarPolicy(qt.Qt.ScrollBarAlwaysOff)
-        self.metadata.setVerticalScrollBarPolicy(qt.Qt.ScrollBarAlwaysOn)
-        self.metadata.setSizePolicy(
-            qt.QSizePolicy.Expanding, qt.QSizePolicy.Expanding)
+        self.makePlotWidget()
+        self.makeFitWidgets()
+        self.makeMetadataWidget()
 
         self.splitterPlot.setCollapsible(0, False)
         self.splitterPlot.setStretchFactor(0, 1)  # don't remove
-        self.splitterPlot.setStretchFactor(1, 0)
-        self.splitterPlot.setSizes([1, 1])
+        for i in range(1, self.splitterPlot.count()):
+            self.splitterPlot.setStretchFactor(i, 0)
+        sizes = [0] * self.splitterPlot.count()
+        sizes[0] = 1
+        self.splitterPlot.setSizes(sizes)
 
     def fillSplitterTransform(self):
         self.help = QWebView(self.splitterTransform)
         # self.help.setHtml('no documentation available')
         self.help.setMinimumSize(qt.QSize(100, 5))
         self.help.page().setLinkDelegationPolicy(2)
         self.help.history().clear()
@@ -400,29 +363,39 @@
         "Orientation should be given for the closed state."
         self.splitterButtons = {}
         self.makeSplitterButton('files && containers', self.splitter, 1, 0)
         self.makeSplitterButton('data', self.splitter, 2, 1)
         self.makeSplitterButton('transform', self.splitter, 3, 3)
         self.makeSplitterButton('data format', self.splitterFiles, 1, 1)
         self.makeSplitterButton('combine', self.splitterData, 1, 1)
-        self.makeSplitterButton('metadata', self.splitterPlot, 1, 1)
+
+        ind = 1
+        for fit in csi.fits.values():
+            if fit.node is self.node and fit.widgetClass is not None:
+                but = self.makeSplitterButton(
+                    fit.name, self.splitterPlot, ind, ind)
+                but.setToolTip(fit.tooltip)
+                ind += 1
+        self.makeSplitterButton('metadata', self.splitterPlot, ind, ind)
+
         self.makeSplitterButton('help', self.splitterTransform, 1, 1)
         self.makeSplitterHelpButton(self.splitterTransform, 1)
 
     def makeSplitterButton(self, name, splitter, indHandle, indSizes):
         handle = splitter.handle(indHandle)
         if handle is None:
             return
         isVerical = splitter.orientation() == qt.Qt.Horizontal
         trNames = ''
-        if self.node.widgetClass is not None:
-            if hasattr(self.node.widgetClass, 'name'):
-                trNames = self.node.widgetClass.name
-        if not trNames:
-            trNames = ', '.join([tr.name for tr in self.node.transformsIn])
+        if name == 'transform':
+            if self.node.widgetClass is not None:
+                if hasattr(self.node.widgetClass, 'name'):
+                    trNames = self.node.widgetClass.name
+            if not trNames:
+                trNames = ', '.join([tr.name for tr in self.node.transformsIn])
         if trNames:
             nameBut = name + ': ' + trNames
         else:
             nameBut = name
         button = QSplitterButton(nameBut, handle, isVerical)
         button.setText(button.rawText)
         if isVerical:
@@ -439,14 +412,15 @@
             sLayout = qt.QHBoxLayout()
         sLayout.setContentsMargins(0, 0, 0, 0)
         sLayout.addStretch(1)
         sLayout.addWidget(button, 0)
         sLayout.addStretch(1)
         handle.setLayout(sLayout)
         self.splitterButtons[name] = button
+        return button
 
     def makeSplitterHelpButton(self, splitter, indHandle):
         handle = splitter.handle(indHandle)
         if handle is None:
             return
         button = QSplitterButton("open in browser", handle, margin=10)
         button.clicked.connect(self.handleSplitterHelpButton)
@@ -458,14 +432,16 @@
         splitter = button.parent().splitter()
         sizes = splitter.sizes()
         if sizes[indSizes]:
             sizes[indSizes] = 0
         else:
             sizes[indSizes] = 1
         splitter.setSizes(sizes)
+        if splitter is self.splitterPlot:
+            self.updateFits(shouldClear=True)
 
     def handleSplitterHelpButton(self):
         webbrowser.open_new_tab(self.helpFile)
         # webbrowser.open_new_tab("https://github.com/")
 
     def setIncludeFilter(self):
         txt = self.editIncludeFilter.text()
@@ -544,14 +520,51 @@
             except Exception:
                 return ""
         try:
             return title.format(ind)
         except Exception:
             return ""
 
+    def makePlotWidget(self):
+        node = self.node
+        # self.backend = dict(backend='opengl')
+        self.backend = dict(backend='matplotlib')
+
+        if node.plotDimension == 3:
+            self.plot = Plot3D(self.splitterPlot, position=Plot3D.posInfo,
+                               **self.backend)
+            self.plot.setCustomPosInfo()
+            self.plot.setTitleCallback(self.titleCallback3D)
+        elif node.plotDimension == 2:
+            self.plot = Plot2D(self.splitterPlot, **self.backend)
+        elif node.plotDimension == 1:
+            xLbl = node.get_arrays_prop('qLabel', role='x')[0]
+            yLbl = node.get_arrays_prop('qLabel', role='y')[0]
+            hasCustomCursorLabels = False
+            if self.node.widgetClass is not None:
+                if (hasattr(self.node.widgetClass, 'cursorPositionCallback')
+                        and hasattr(self.node.widgetClass, 'cursorLabels')):
+                    hasCustomCursorLabels = True
+            if hasCustomCursorLabels:
+                position = [
+                    (label, partial(
+                        self.node.widgetClass.cursorPositionCallback, label))
+                    for label in self.node.widgetClass.cursorLabels]
+            else:
+                position = [(xLbl, lambda x, y: x), (yLbl, lambda x, y: y)]
+            self.plot = Plot1D(self.splitterPlot, position=position,
+                               **self.backend)
+            self.plot.getXAxis().setLabel(xLbl)
+            self.plot.getYAxis().setLabel(yLbl)
+        else:
+            raise ValueError("wrong plot dimension")
+        self.plotSetup()
+        self.plot.setMinimumWidth(20)
+        self.savedPlotProps = {}
+
     def plotSetup(self):
         node = self.node
         if node.plotDimension == 1:
             try:
                 unit = node.get_arrays_prop('plotUnit', role='x')[0]
                 strUnit = u" ({0})".format(unit) if unit else ""
             except AttributeError:
@@ -566,14 +579,40 @@
             self.plot.getYAxis().setLabel(axisLabels[1])
         elif node.plotDimension == 3:
             self.plot.setColormap(COLORMAP)
             labels = node.get_prop(node.plot3DArray, 'plotLabel')
             axisLabels = self._makeAxisLabels(labels)
             self.plot.setLabels(axisLabels)
 
+    def makeFitWidgets(self):
+        self.fitWidgets = []
+        for ifit, fit in enumerate(csi.fits.values()):
+            if fit.node is self.node and fit.widgetClass is not None:
+                fitWidget = fit.widgetClass(self.splitterPlot, fit, self.plot)
+                fitWidget.fitReady.connect(
+                    partial(self.replotFit, fit, ifit))
+                self.fitWidgets.append(fitWidget)
+                curveLabel = fit.dataAttrs['fit']
+                if curveLabel not in self.fitLines:
+                    self.fitLines.append(curveLabel)
+                    self.fitLines.append(curveLabel+'.residue')
+
+    def makeMetadataWidget(self):
+        self.metadata = qt.QTextEdit(self.splitterPlot)
+        self.metadata.setStyleSheet("QTextEdit {border: none;}")
+        self.metadata.setReadOnly(True)
+        # self.metadata.setContentsMargins(0, 0, 0, 0)
+        self.metadata.setMinimumHeight(84)
+        self.metadata.setAlignment(qt.Qt.AlignLeft | qt.Qt.AlignTop)
+        self.metadata.setText("text metadata here")
+        self.metadata.setHorizontalScrollBarPolicy(qt.Qt.ScrollBarAlwaysOff)
+        self.metadata.setVerticalScrollBarPolicy(qt.Qt.ScrollBarAlwaysOn)
+        self.metadata.setSizePolicy(
+            qt.QSizePolicy.Expanding, qt.QSizePolicy.Expanding)
+
     def getAxisLabels(self):
         plot = self.plot
         if self.node.plotDimension == 1:
             res = [plot.getGraphXLabel(), plot.getGraphYLabel(axis='left'),
                    plot.getGraphYLabel(axis='right')]
             return res
         elif self.node.plotDimension == 2:
@@ -679,17 +718,17 @@
             self.plot.clearImages()
             # self.plot.clearMarkers()
             nPlottedItems = 0
             leftAxisColumns, rightAxisColumns = [], []
             leftAxisUnits, rightAxisUnits = [], []
             for item in csi.allLoadedItems:
                 if not self.shouldPlotItem(item):
-                    for yN in node.plotYArrays:
-                        curveLabel = item.alias + '.' + yN
-                        self.plot.remove(curveLabel, kind='curve')
+                    for yN in node.plotYArrays + self.fitLines:
+                        legend = '{0}.{1}'.format(item.alias, yN)
+                        self.plot.remove(legend, kind='curve')
                     continue
                 try:
                     x = getattr(item, node.plotXArray)
                 except AttributeError:
                     continue
                 if (csi.nodes[item.originNodeName] is node and
                         'conversionFactors' in item.dataFormat):
@@ -774,15 +813,15 @@
                 rightAxisColumns, rightAxisUnits)
             self.plot.setGraphYLabel(label=self.plotRightYLabel, axis='right')
         if node.plotDimension == 2:
             self.plot.clearCurves()
             # if needClear:
             if True:
                 self.plot.clearImages()
-                self.plot.clearMarkers()
+                # self.plot.clearMarkers()  # clears roi lines, don't add
             if len(csi.selectedItems) > 0:
                 item = csi.selectedItems[0]  # it could be the last one but
                 # then when going with arrows up and down in the data tree and
                 # passing a group that becomes selected, the displayed item
                 # jumps between the first and the last
             elif len(csi.allLoadedItems) > 0:
                 item = csi.allLoadedItems[-1]
@@ -802,19 +841,19 @@
 
             xOrigin, xScale = self.getCalibration(item, 'x')
             yOrigin, yScale = self.getCalibration(item, 'y')
             self.plot.addImage(image, colormap=colors.Colormap(COLORMAP),
                                origin=(xOrigin, yOrigin),
                                scale=(xScale, yScale), z=-100)
         if node.plotDimension == 3:
-            self.plot._plot.clearCurves()  # clears roi lines
+            self.plot._plot.clearCurves()
             # if needClear:
             if True:
                 self.plot._plot.clearImages()
-                self.plot._plot.clearMarkers()
+                # self.plot._plot.clearMarkers()  # clears roi lines, don't add
             item = None
             if len(csi.selectedItems) > 0:
                 item = csi.selectedItems[0]
             elif len(csi.allLoadedItems) > 0:
                 item = csi.allLoadedItems[-1]
             else:
                 return
@@ -844,17 +883,79 @@
             #     print(e)
             pass
 
         # if self.wasNeverPlotted and node.plotDimension == 1:
         #     self.plot.resetZoom()
         self.wasNeverPlotted = False
 
+    @logger(minLevel=50, attrs=[(0, 'node')])
+    def replotFit(self, fitWorker, ifit):
+        def plotOne(item, x, y, curveLabel, plotProps):
+            symbolsize = plotProps.pop('symbolsize', 2)
+            curve = self.plot.getCurve(curveLabel)
+            z = 1 if item in csi.selectedItems else 0
+            try:
+                if curve is None:
+                    self.plot.addCurve(
+                        x, y, legend=curveLabel, color=item.color, z=z,
+                        **plotProps)
+                else:
+                    curve.setData(x, y)
+                    curve.setZValue(z)
+            except Exception as e:
+                print('plotting in {0} failed for ({1}, len={2}) vs '
+                      '({3}, len={4}): {5}'
+                      .format(node.name, fitAttrName, len(y), xAttrName,
+                              len(x), e))
+                tb = traceback.format_exc()
+                print(tb)
+                return
+            symbol = plotProps.get('symbol', None)
+            if symbol is not None:
+                curve = self.plot.getCurve(curveLabel)
+                if curve is not None:
+                    if self.backend['backend'] == 'opengl':
+                        # don't know why it is small with opengl
+                        symbolsize *= 2
+                    curve.setSymbolSize(symbolsize)
+
+        node = self.node
+        xAttrName, yAttrName, fitAttrName = [
+            fitWorker.dataAttrs[a] for a in ('x', 'y', 'fit')]
+        fitSizes = self.splitterPlot.sizes()[1:-1]
+        assert len(fitSizes) == len(self.fitWidgets)
+
+        if node.plotDimension == 1:
+            plotProps = fitWorker.plotParams['fit']
+            residueProps = fitWorker.plotParams['residue']
+            for item in csi.allLoadedItems:
+                curveLabel = item.alias + '.' + fitAttrName
+                residueLabel = curveLabel + '.residue'
+                if not self.shouldPlotItem(item) or fitSizes[ifit] == 0:
+                    self.plot.remove(curveLabel, kind='curve')
+                    self.plot.remove(residueLabel, kind='curve')
+                    continue
+                try:
+                    x = getattr(item, xAttrName)
+                    y = getattr(item, yAttrName)
+                    fity = getattr(item, fitAttrName)
+                except AttributeError:
+                    continue
+                plotOne(item, x, fity, curveLabel, dict(plotProps))
+                if fity.any():  # any non-zero
+                    plotOne(item, x, y-fity, residueLabel, dict(residueProps))
+        else:
+            raise NotImplementedError('fit plot not implemented for dim={0}'
+                                      .format(node.plotDimension))
+
     def saveGraph(self, fname, i, name):
         if fname.endswith('.pspj'):
             fname = fname.replace('.pspj', '')
+        if len(self.plot.getItems()) == 0:
+            return
         fname += '-{0}-{1}.png'.format(i+1, name)
         if self.node.plotDimension in [1, 2]:
             self.plot.saveGraph(fname)
         elif self.node.plotDimension in [3]:
             self.plot._plot.saveGraph(fname)
 
     def _makeYLabel(self, yNames, yUnits):
@@ -913,14 +1014,15 @@
         if fname:
             self.files.gotoWhenReady(fname)
             self.columnFormat.setUIFromData()
 
         self.updateMeta()
         self.combiner.setUIFromData()
         self.updateTransforms()
+        self.updateFits()
 
     def shouldUpdateFileModel(self):
         for it in csi.selectedItems:
             if it.dataType in (cco.DATA_COLUMN_FILE, cco.DATA_DATASET) and\
                     csi.nodes[it.originNodeName] is self.node:
                 return it.madeOf
 
@@ -957,19 +1059,22 @@
 
         fileNamesFull = self.files.getFullFileNames(fileNamesFull)
         if fileNamesFull is None:  # when isDir
             return
         fileNames = [osp.normcase(nf) for nf in fileNamesFull]
         allLoadedItemNames = []
         for d in csi.allLoadedItems:
-            lfn = d.madeOf[5:] if d.madeOf.startswith('silx:') else d.madeOf
-            lfns = osp.normcase(osp.abspath(lfn))
-            if d.madeOf.startswith('silx:'):
-                lfns = 'silx:' + lfns
-            allLoadedItemNames.append(lfns)
+            if isinstance(d.madeOf, str):
+                ln = d.madeOf[5:] if d.madeOf.startswith('silx:') else d.madeOf
+                nln = osp.normcase(osp.abspath(ln))
+                if d.madeOf.startswith('silx:'):
+                    nln = 'silx:' + nln
+                allLoadedItemNames.append(nln)
+            else:
+                allLoadedItemNames.append(str(d))
         allLoadedItemsCount = Counter(allLoadedItemNames)
         duplicates, duplicatesN = [], []
         fileNamesFullN = []
         for fname, fnameFull in zip(fileNames, fileNamesFull):
             n = allLoadedItemsCount[osp.normcase(fnameFull)]
             if n > 0:
                 duplicates.append(fnameFull)
@@ -1038,14 +1143,29 @@
             self.transformWidget.setEnabled(False)
         else:
             self.transformWidget.setEnabled(True)
             # in tests, transformWidget is a QWidget instance:
             if hasattr(self.transformWidget, 'setUIFromData'):
                 self.transformWidget.setUIFromData()
 
+    def updateFits(self, shouldClear=False):
+        if len(csi.selectedItems) < 1:
+            return
+        fitSizes = self.splitterPlot.sizes()[1:-1]
+        assert len(fitSizes) == len(self.fitWidgets)
+        for fitWidget, fitSize in zip(self.fitWidgets, fitSizes):
+            if fitSize > 0 or shouldClear:
+                fitWidget.setSpectrum(csi.selectedItems[0])
+            if shouldClear:
+                roi = fitWidget.rangeWidget.roi
+                if roi is not None:
+                    roi.blockSignals(True)
+                    roi.setVisible(fitSize > 0)
+                    roi.blockSignals(False)
+
     def linkClicked(self, url):
         strURL = str(url.toString())
         if strURL.startswith('http') or strURL.startswith('ftp'):
             if self.lastBrowserLink == strURL:
                 return
             webbrowser.open(strURL)
             self.lastBrowserLink = strURL
@@ -1108,15 +1228,16 @@
     def doAutoLoad(self):
         if self.autoDirName.startswith('silx:'):
             model = self.files.getSourceModel()
             if self.autoDirName.endswith('::/'):
                 ind = model.indexFileName(self.autoDirName[5:-3])
             else:
                 ind = model.indexFromH5Path(self.autoDirName)
-            self.files.synchronizeHDF5Index(ind)
+            model.reloadHdf5(ind)
+            # self.files.synchronizeHDF5Index(ind)
 
         # this first solution doesn't work in NFS in Linux:
         # newFileList = self.files.getActiveDir(self.autoDirName)
 
         dirname = str(self.autoDirName)
         if not dirname.endswith('/'):
             dirname += '/'
```

## Comparing `parseq-1.0.0/parseq/gui/plot.py` & `parseq-2023.5.0/parseq/gui/plot.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/plotOptions.py` & `parseq-2023.5.0/parseq/gui/plotOptions.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/propsOfData.py` & `parseq-2023.5.0/parseq/gui/propsOfData.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/propWidget.py` & `parseq-2023.5.0/parseq/gui/propWidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,16 @@
         self.spinTimer = qt.QTimer(self)
         self.spinTimer.setSingleShot(True)
         self.spinTimer.timeout.connect(self.spinDelayed)
         self.spinBoxProps = None
 
         self.read_ini_properties()
 
-        if csi.transformer is not None:
-            csi.transformer.ready.connect(self._onTransformThreadReady)
+        if csi.tasker is not None:
+            csi.tasker.ready.connect(self._onTransformThreadReady)
 
     def read_ini_properties(self):
         sec = self.__class__.__name__
         if config.configTransforms.has_section(sec):
             for key in self.properties:
                 try:
                     testStr = config.configTransforms.get(sec, key)
@@ -178,15 +178,19 @@
                 except Exception:
                     pass
         if hdf5Path:
             menu.addSeparator()
             self._addAction(menu, "go to hdf5 location",
                             partial(self.gotoHDF5, hdf5Path))
 
+        for w in widgetsOver:  # editingFinished is emitted before menu.exec_
+            w.blockSignals(True)
         menu.exec_(event.globalPos())
+        for w in widgetsOver:
+            w.blockSignals(False)
 
     def fillMenuApply(self, widgetsOver, menu):
         if len(csi.selectedItems) == 0:
             return
         actionStr = 'apply {0}{1}'
         data = csi.selectedItems[0]
 
@@ -658,15 +662,15 @@
                 raise ValueError('unknown key "{0}" of type {1}'.format(
                     key, type(key)))
             params = {param: value}
 
         tr = None
         data = dataItems[0]
         # in the case when several transforms come to one node, we need to
-        # check which one to rune, there can be only one!
+        # check which one to run, there can be only one!
         for tName in tNames:
             if isinstance(tName, str):
                 tr = csi.transforms[tName]
                 if (tr.fromNode.is_between_nodes(
                     data.originNodeName, data.terminalNodeName) and
                     tr.toNode.is_between_nodes(
                         data.originNodeName, data.terminalNodeName)):
@@ -675,21 +679,24 @@
                 for tN in tName:
                     tr = csi.transforms[tN]
                     if (tr.fromNode.is_between_nodes(
                         data.originNodeName, data.terminalNodeName) and
                         tr.toNode.is_between_nodes(
                             data.originNodeName, data.terminalNodeName)):
                         break
+        else:
+            tr = csi.nodes[data.originNodeName].transformsOut[0]
         if tr is None:
             return
 
-        if csi.transformer is not None:
-            csi.transformer.prepare(
-                tr, params=params, dataItems=dataItems, starter=self)
-            csi.transformer.thread().start()
+        if csi.tasker is not None:
+            csi.tasker.prepare(
+                tr, params=params, runDownstream=True, dataItems=dataItems,
+                starter=self)
+            csi.tasker.thread().start()
         else:
             tr.run(params=params, dataItems=dataItems)
 
     # @logger(minLevel=50, attrs=[(0, 'node')])
     def _onTransformThreadReady(
             self, starter, tName='', tStr='', props={}, duration=0, err=None):
         if starter is not self:
```

## Comparing `parseq-1.0.0/parseq/gui/roi.py` & `parseq-2023.5.0/parseq/gui/roi.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                 return section
         elif role == qt.Qt.TextAlignmentRole:
             return qt.Qt.AlignHCenter
 
     def flags(self, index):
         if not index.isValid():
             return qt.Qt.NoItemFlags
-        res = qt.Qt.ItemIsEnabled | qt.Qt.ItemIsSelectable
+        res = qt.Qt.ItemIsEnabled  # | qt.Qt.ItemIsSelectable
         column = index.column()
         if column == 1:  # use
             res |= qt.Qt.ItemIsUserCheckable
         elif column in (0, 2):  # label, geometry
             res |= qt.Qt.ItemIsEditable
         return res
 
@@ -137,16 +137,15 @@
                 return self.getReadableRoiDescription(roi)
             elif column == 3:  # counts
                 while len(self.roiCounts) < row+1:
                     self.roiCounts.append(0)
                 return '{0:.0f}'.format(self.roiCounts[row])
         elif role == qt.Qt.CheckStateRole:
             if column == 1:  # use
-                return int(
-                    qt.Qt.Checked if roi.isVisible() else qt.Qt.Unchecked)
+                return qt.Qt.Checked if roi.isVisible() else qt.Qt.Unchecked
         elif role == qt.Qt.ToolTipRole:
             return "{0}\ncan be removed via the plot's popup menu".format(
                 roi.__class__.__name__)
         elif role == qt.Qt.TextAlignmentRole:
             if column == 1:
                 return qt.Qt.AlignCenter
 
@@ -377,14 +376,15 @@
             horHeaders.setSectionResizeMode(2, qt.QHeaderView.Stretch)
             horHeaders.setSectionsClickable(True)
             verHeaders.setSectionResizeMode(qt.QHeaderView.ResizeToContents)
         horHeaders.setStretchLastSection(False)
         horHeaders.setMinimumSectionSize(20)
         # verHeaders.setMinimumSectionSize(70)
 
+        self.setItemDelegateForColumn(1, gco.CheckBoxDelegate(self))
         self.setItemDelegateForColumn(2, gco.MultiLineEditDelegate(self))
 
         for i in range(len(HEADERS)):
             self.setColumnWidth(i, int(columnWidths[i]*csi.screenFactor))
         self.setMinimumWidth(int(sum(columnWidths)*csi.screenFactor) + 2)
         self.setMinimumHeight(int(horHeaders.height()*4*csi.screenFactor))
 
@@ -778,14 +778,16 @@
         model = self.table.roiModel
         row = rois.index(curRoi)
         ind1 = model.index(row, 2)
         ind2 = model.index(row, 3)
         model.dataChanged.emit(ind1, ind2)
 
     def setRois(self, roiDicts):
+        if not roiDicts:
+            return
         if not isinstance(roiDicts, (tuple, list)):
             roiDicts = roiDicts,
         roiDicts = [dict(roid) for roid in roiDicts]  # deep copy
         rois = self.roiManager.getRois()
         if len(rois) != len(roiDicts):
             needReset = True
         else:
@@ -820,16 +822,16 @@
                 elif kind == 'CrossROI':
                     roi = CrossROI()
                 elif kind == 'PointROI':
                     roi = PointROI()
                 elif kind == 'HorizontalRangeROI':
                     roi = HorizontalRangeROI()
                 else:
-                    continue
-                    # raise ValueError('unsupported ROI "{0}"'.format(kind))
+                    # continue
+                    raise ValueError('unsupported ROI "{0}"'.format(kind))
                 if name:
                     roi.setName(name)
                 roi.setVisible(True)
                 model.setRoi(roi, roid)
                 self.roiManager.addRoi(roi)
             self.roiManager.setCurrentRoi(roi)
         else:
@@ -932,15 +934,15 @@
         spinbox values.
         """
         return vmin, vmax  # just pass through
 
 
 class RangeWidget(RangeWidgetBase):
     def __init__(self, parent, plot, caption, tooltip, rangeName, color,
-                 formatStr, defaultRange):
+                 formatStr, defaultRange=[0, 1]):
         """
         *defaultRange*: callable or 2-sequence
         """
         super().__init__(parent)
         self.plot = plot
         self.is3dStack = hasattr(plot, '_plot')
         self.formatStr = formatStr
@@ -960,18 +962,14 @@
         panel = qt.QGroupBox(self)
         panel.setFlat(True)
         panel.setTitle(caption)
         layoutP = qt.QHBoxLayout()
         layoutP.setContentsMargins(10, 0, 0, 0)
         self.rbAuto = qt.QRadioButton('auto', panel)
         self.rbAuto.clicked.connect(self.setAutoRange)
-        if not callable(self.defaultRange):
-            fs = "[" + self.formatStr + "]{1}{2}"
-            self.rbAuto.setToolTip(fs.format(
-                self.defaultRange, ' as ' if tooltip else '', tooltip))
         layoutP.addWidget(self.rbAuto)
         self.rbCustom = qt.QRadioButton('custom', panel)
         self.rbCustom.setStyleSheet("QRadioButton{color: " + color + ";}")
         self.rbCustom.clicked.connect(self.setCustomRange)
         layoutP.addWidget(self.rbCustom)
         self.editCustom = qt.QLineEdit()
         self.editCustom.setStyleSheet("QLineEdit{color: " + color + ";}")
@@ -1009,14 +1007,17 @@
             self.roi.setVisible(not isDefault)
 
     def setAutoRange(self):
         if callable(self.defaultRange):
             defRange = self.defaultRange()
         else:
             defRange = self.defaultRange
+            fs = "[" + self.formatStr + "]{1}{2}"
+            self.rbAuto.setToolTip(fs.format(
+                defRange, ' as ' if self.tooltip else '', self.tooltip))
         if self.roi is not None:
             self.setRange(defRange)
         self.rangeChanged.emit(defRange)
         self.editSetText(defRange)
         self.rbAuto.setChecked(True)
         self.rbCustom.setChecked(False)
```

## Comparing `parseq-1.0.0/parseq/gui/undoredo.py` & `parseq-2023.5.0/parseq/gui/undoredo.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/webWidget.py` & `parseq-2023.5.0/parseq/gui/webWidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,14 +232,19 @@
 
         shutil.copytree(osp.join(CONFDIR, '_images'),
                         osp.join(DOCDIR, '_images'), dirs_exist_ok=True)
         for ico in ['1', '2', '3', 'n']:
             fname = 'icon-item-{0}dim-32.png'.format(ico)
             shutil.copy2(osp.join(GUIDIR, '_images', fname),
                          osp.join(DOCDIR, '_images', fname))
+
+        fname = 'icon-fit-32.png'
+        shutil.copy2(osp.join(GUIDIR, '_images', fname),
+                     osp.join(DOCDIR, '_images', fname))
+
         shutil.copytree(osp.join(CONFDIR, '_themes'),
                         osp.join(DOCDIR, '_themes'))
         shutil.copy2(osp.join(CONFDIR, 'conf_doc.py'),
                      osp.join(DOCDIR, 'conf.py'))
 
         srcdir = osp.join(DOCDIR, '_sources')
         if not osp.exists(srcdir):
```

## Comparing `parseq-1.0.0/parseq/gui/__init__.py` & `parseq-2023.5.0/parseq/gui/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 =====================
 
 Load project
 ------------
 
 To start testing a GUI, load a test project, typically located in `saved`
 directory. The "Load project" dialog has a preview panel that displays all node
-plots in the project, just browse over them. The default plot displays the
-transformation node that was active when the project was saved.
+plots in the project, just browse over them. The initial visible plot displays
+the transformation node that was active when the project was saved.
 
 Docked node widgets
 -------------------
 
 With the idea of flexible usage of screen area, the node widgets were made
 detachable and dockable into the main ParSeq window. To do this, drag a node
 widget by its caption bar. To dock it back, hover it over the main window or
@@ -105,21 +105,35 @@
 item in the data tree widget. Auxiliary curves can be added in user-defined
 transformation widgets by specifying a method `extraPlot()`. The curves should
 have their `legend` property defined in the following format: the data item
 alias followed by a dot followed by a sub-name. If this convention is followed,
 the curves become clickable, which will select the corresponding data item in
 the data tree. Selected data items are plotted on top of unselected items.
 
+Fit widgets
+-----------
+
+If one or more fit widgets were specified for a given node, they appear in
+separate QSplitter under the node's plot. In the initial view, the splitters
+are collapsed.
+
 Help panel
 ----------
 
 The help panel under transformation widgets is hidden by default and can be
 made visible by clicking on the small button "help" at the very bottom of the
 main window. Alternatively, it can be opened in the system browser.
 
+About dialog
+------------
+
+The about dialog displays the connectivity between the pipeline nodes in a
+dynamically created svg graph. If a fit is defined in a node, it is also
+displayed here.
+
 Undo and redo lists
 -------------------
 
 When a transformation parameter has been changed or a data item has been
 deleted, this action is inserted into the undo list. Clicking on the big undo
 button will revert the last action and put it into the redo list (not for the
 undelete operation). Any undo action can also be executed separately, not
```

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-help.png` & `parseq-2023.5.0/parseq/gui/_images/icon-help.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-info.png` & `parseq-2023.5.0/parseq/gui/_images/icon-info.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-1dim-32.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-32.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-1dim-64.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-64.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-1dim-busy-32.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-32.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-1dim-busy-64.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-1dim-busy-64.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-2dim-64.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-64.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-2dim-busy-64.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-2dim-busy-64.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-3dim-32.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-32.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-3dim-64.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-64.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-3dim-busy-32.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-32.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-3dim-busy-64.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-3dim-busy-64.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-ndim-32.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-32.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-ndim-64.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-64.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-ndim-busy-32.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-32.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-item-ndim-busy-64.png` & `parseq-2023.5.0/parseq/gui/_images/icon-item-ndim-busy-64.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-load-proj.png` & `parseq-2023.5.0/parseq/gui/_images/icon-load-proj.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-redo.png` & `parseq-2023.5.0/parseq/gui/_images/icon-redo.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-save-proj.png` & `parseq-2023.5.0/parseq/gui/_images/icon-save-proj.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-save-text.png` & `parseq-2023.5.0/parseq/gui/_images/icon-save-text.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/icon-undo.png` & `parseq-2023.5.0/parseq/gui/_images/icon-undo.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/gui/_images/parseq.ico` & `parseq-2023.5.0/parseq/gui/_images/parseq.ico`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/conf.py` & `parseq-2023.5.0/parseq/help/conf.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/conf_doc.py` & `parseq-2023.5.0/parseq/help/conf_doc.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/license.rst` & `parseq-2023.5.0/parseq/help/license.rst`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/make.bat` & `parseq-2023.5.0/parseq/help/make.bat`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/top.rst` & `parseq-2023.5.0/parseq/help/top.rst`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/exts/animation.py` & `parseq-2023.5.0/parseq/help/exts/animation.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_images/mickey-rtfm.gif` & `parseq-2023.5.0/parseq/help/_images/mickey-rtfm.gif`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_images/node1.png` & `parseq-2023.5.0/parseq/help/_images/node1.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_images/node2.png` & `parseq-2023.5.0/parseq/help/_images/node2.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_images/node3.png` & `parseq-2023.5.0/parseq/help/_images/node3.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_images/node4.png` & `parseq-2023.5.0/parseq/help/_images/node4.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_images/parseq.ico` & `parseq-2023.5.0/parseq/help/_images/parseq.ico`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_images/parseq_big.png` & `parseq-2023.5.0/parseq/help/_images/parseq_big.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_images/XAS_icon.ico` & `parseq-2023.5.0/parseq/help/_images/XAS_icon.ico`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_images/XES_dispersive_icon.ico` & `parseq-2023.5.0/parseq/help/_images/XES_dispersive_icon.ico`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_images/XES_scan_icon.ico` & `parseq-2023.5.0/parseq/help/_images/XES_scan_icon.ico`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_static/animation.js` & `parseq-2023.5.0/parseq/help/_static/animation.js`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_static/thumbnail.css` & `parseq-2023.5.0/parseq/help/_static/thumbnail.css`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_themes/mytheme/static/mycss.css_t` & `parseq-2023.5.0/parseq/help/_themes/mytheme/static/mycss.css_t`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_themes/parseq/layout.html` & `parseq-2023.5.0/parseq/help/_themes/parseq/layout.html`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_themes/parseq/page.html` & `parseq-2023.5.0/parseq/help/_themes/parseq/page.html`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_themes/parseq/theme.conf` & `parseq-2023.5.0/parseq/help/_themes/parseq/theme.conf`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/help/_themes/parseq/static/default.css_t` & `parseq-2023.5.0/parseq/help/_themes/parseq/static/default.css_t`

 * *Files 2% similar despite different names*

```diff
@@ -367,24 +367,41 @@
     display: grid;
     grid-auto-columns: 1fr;
     grid-auto-flow: column;
     padding: 2px;
 }
 
 .pipeline-node {
-    padding: 5px;
+    padding: 7px;
     margin: 0px;
     margin-left: 10px;
     width: auto;
-    //height: 22px;
+    height: 24px;
     border-radius: 11px;
-    background: #dde;
-    box-shadow: 1px 2px 3px #aac, inset 0px 0px 7px rgba(0,0,0,1);
+    background: #eef;
+    box-shadow: 1px 2px 3px #aac, inset 0px 0px 7px rgba(0,0,50,1);
+    text-align: center;
+
+    /* center a div insie another div*/
+    display: flex;
+    justify-content: center;
+    align-items: center;
+}
+
+.pipeline-fit {
+    padding: 7px;
+    margin: 0 auto;
+    width: auto;
+    height: 16px;
+    border-radius: 7px;
+    background: #ded;
+    box-shadow: 1px 2px 3px #caa, inset 0px 0px 3px rgba(0,0,0,1);
     vertical-align: middle;
     text-align: center;
+    position: relative;
 }
 
 .pipeline-tr {
     padding: 5px;
     margin: 0px;
     margin-left: 10px;
     width: auto;
```

## Comparing `parseq-1.0.0/parseq/help/_themes/parseq/static/utils.js` & `parseq-2023.5.0/parseq/help/_themes/parseq/static/utils.js`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/circles-rect.png` & `parseq-2023.5.0/parseq/tests/circles-rect.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/circles.png` & `parseq-2023.5.0/parseq/tests/circles.png`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/modeltest.py` & `parseq-2023.5.0/parseq/tests/modeltest.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_calibrateEnergyWidget.py` & `parseq-2023.5.0/parseq/tests/test_calibrateEnergyWidget.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_columnStrings.py` & `parseq-2023.5.0/parseq/tests/test_columnStrings.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_combineSpectraWidget.py` & `parseq-2023.5.0/parseq/tests/test_combineSpectraWidget.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_commons.py` & `parseq-2023.5.0/parseq/tests/test_commons.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_curve_shear.py` & `parseq-2023.5.0/parseq/tests/test_curve_shear.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_dataRebinWidget.py` & `parseq-2023.5.0/parseq/tests/test_dataRebinWidget.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_dataTreeModelView.py` & `parseq-2023.5.0/parseq/tests/test_dataTreeModelView.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_fileDialog.py` & `parseq-2023.5.0/parseq/tests/test_fileDialog.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_fileTreeModelView.py` & `parseq-2023.5.0/parseq/tests/test_fileTreeModelView.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_flowLayout.py` & `parseq-2023.5.0/parseq/tests/test_flowLayout.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_hdf5.py` & `parseq-2023.5.0/parseq/tests/test_hdf5.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_mainWindow.py` & `parseq-2023.5.0/parseq/tests/test_mainWindow.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_node.py` & `parseq-2023.5.0/parseq/tests/test_node.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_nodeWidget.py` & `parseq-2023.5.0/parseq/tests/test_nodeWidget.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py` & `parseq-2023.5.0/parseq/tests/test_plotInteractiveImageROIwithKeys.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_plotInteractiveImageSingleROI.py` & `parseq-2023.5.0/parseq/tests/test_plotInteractiveImageSingleROI.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_plotOptions.py` & `parseq-2023.5.0/parseq/tests/test_plotOptions.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_QSortFilterProxyModel.py` & `parseq-2023.5.0/parseq/tests/test_QSortFilterProxyModel.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_ROI.py` & `parseq-2023.5.0/parseq/tests/test_ROI.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_slice.py` & `parseq-2023.5.0/parseq/tests/test_slice.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/tests/test_stateButtons.py` & `parseq-2023.5.0/parseq/tests/test_stateButtons.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/third_party/XAFSmass.py` & `parseq-2023.5.0/parseq/third_party/XAFSmass.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/third_party/xrt.py` & `parseq-2023.5.0/parseq/third_party/xrt.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/third_party/data/Energies.txt` & `parseq-2023.5.0/parseq/third_party/data/Energies.txt`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/utils/ft.py` & `parseq-2023.5.0/parseq/utils/ft.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/utils/h5reduce.py` & `parseq-2023.5.0/parseq/utils/h5reduce.py`

 * *Files identical despite different names*

## Comparing `parseq-1.0.0/parseq/utils/math.py` & `parseq-2023.5.0/parseq/utils/math.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         dist2 = (xs-x)**2 + (ys-y)**2
         return (dist2 >= r1**2) & (dist2 <= r2**2)
     elif geom['kind'] == 'BandROI':
         x1, y1 = geom['begin']
         x2, y2 = geom['end']
         k, b = line((x1, x2), (y1, y2))
         w = geom['width']
-        return (ys >= k*(xs-w/2) + b) & (ys <= k*(xs+w/2) + b)
+        return (ys >= k*xs + b - w/2) & (ys <= k*xs + b + w/2)
     elif geom['kind'] == 'HorizontalRangeROI':
         vmin, vmax = geom['vmin'], geom['vmax']
         return (xs >= vmin) & (xs <= vmax) & (ys > 0)
     else:
         raise ValueError('unsupported ROI type')
```

## Comparing `parseq-1.0.0/parseq.egg-info/PKG-INFO` & `parseq-2023.5.0/parseq.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parseq
-Version: 1.0.0
+Version: 2023.5.0
 Summary: ParSeq is a python software library for Parallel execution of Sequential data analysis.
 Home-page: http://parseq.readthedocs.io
 Author: Konstantin Klementiev
 Author-email: konstantin.klementiev@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/kklmn/ParSeq
 Keywords: data-analysis pipeline framework gui synchrotron spectroscopy
@@ -53,16 +53,19 @@
    pipeline.
 
 -  Creation of cross-data combinations (e.g. averaging, RMS or PCA) and their
    propagation downstream the pipeline together with the parental data. The
    possibility of termination of the parental data at any selected downstream
    node.
 
--  Parallel execution of data analysis with multiprocessing or multithreading
-   (can be opted by the pipeline application).
+-  Parallel execution of data transformations with multiprocessing or
+   multithreading (can be opted by the pipeline application).
+
+-  Optional curve fitting solvers, also executed in parallel for multiple data
+   items.
 
 -  Informative error handling that provides alerts and stack traceback -- the
    type and location of the occurred error.
 
 -  Export of the workflow into a project file. Export of data into various data
    formats with accompanied Python scripts that visualize the exported data for
    the user to tune their publication plots.
@@ -75,17 +78,17 @@
    from the analysis widget doc strings. The help pages are built by Sphinx at
    the startup time.
 
 -  The pipeline can be operated via scripts or GUI.
 
 -  Optional automatic loading of new data during a measurement time.
 
-The mechanisms for creating nodes and transformations, connecting them together
-and creating Qt widgets for the transformations are exemplified by separately
-installed analysis packages:
+The mechanisms for creating nodes, transformations and curve fitting solvers,
+connecting them together and creating Qt widgets for the transformations and
+and curve fits are exemplified by separately installed analysis packages:
 
 - `ParSeq-XES-scan <https://github.com/kklmn/ParSeq-XES-scan>`_
 - `ParSeq-XES-dispersive <https://github.com/kklmn/ParSeq-XES-dispersive>`_
 - `ParSeq-XAS <https://github.com/kklmn/ParSeq-XAS>`_
 
 Dependencies
 ------------
```

## Comparing `parseq-1.0.0/parseq.egg-info/SOURCES.txt` & `parseq-2023.5.0/parseq.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 parseq/core/logger.py
 parseq/core/nodes.py
 parseq/core/plotExport.py
 parseq/core/save_restore.py
 parseq/core/singletons.py
 parseq/core/spectra.py
 parseq/core/transforms.py
+parseq/fits/__init__.py
+parseq/fits/basefit.py
+parseq/fits/functionfit.py
+parseq/fits/lcf.py
 parseq/gui/__init__.py
 parseq/gui/aboutDialog.py
 parseq/gui/calibrateEnergy.py
 parseq/gui/columnFormat.py
 parseq/gui/combineSpectra.py
 parseq/gui/dataRebin.py
 parseq/gui/dataTreeModelView.py
@@ -34,17 +38,19 @@
 parseq/gui/mainWindow.py
 parseq/gui/nodeWidget.py
 parseq/gui/plot.py
 parseq/gui/plotOptions.py
 parseq/gui/propWidget.py
 parseq/gui/propsOfData.py
 parseq/gui/roi.py
-parseq/gui/transformer.py
+parseq/gui/tasker.py
 parseq/gui/undoredo.py
 parseq/gui/webWidget.py
+parseq/gui/_images/icon-fit-32.png
+parseq/gui/_images/icon-fit-64.png
 parseq/gui/_images/icon-help.png
 parseq/gui/_images/icon-info.png
 parseq/gui/_images/icon-item-1dim-32.png
 parseq/gui/_images/icon-item-1dim-64.png
 parseq/gui/_images/icon-item-1dim-busy-32.png
 parseq/gui/_images/icon-item-1dim-busy-64.png
 parseq/gui/_images/icon-item-2dim-32.png
@@ -61,18 +67,23 @@
 parseq/gui/_images/icon-item-ndim-busy-64.png
 parseq/gui/_images/icon-load-proj.png
 parseq/gui/_images/icon-redo.png
 parseq/gui/_images/icon-save-proj.png
 parseq/gui/_images/icon-save-text.png
 parseq/gui/_images/icon-undo.png
 parseq/gui/_images/parseq.ico
+parseq/gui/fits/__init__.py
+parseq/gui/fits/gbasefit.py
+parseq/gui/fits/gfunctionfit.py
+parseq/gui/fits/glcf.py
 parseq/help/__init__.py
 parseq/help/conf.py
 parseq/help/conf_doc.py
 parseq/help/data.rst
+parseq/help/fits.rst
 parseq/help/howto.rst
 parseq/help/index.rst
 parseq/help/license.rst
 parseq/help/make.bat
 parseq/help/nodes.rst
 parseq/help/notesgui.rst
 parseq/help/top.rst
@@ -97,19 +108,24 @@
 parseq/help/_themes/parseq/layout.html
 parseq/help/_themes/parseq/page.html
 parseq/help/_themes/parseq/theme.conf
 parseq/help/_themes/parseq/static/default.css_t
 parseq/help/_themes/parseq/static/math_config_win32.js
 parseq/help/_themes/parseq/static/utils.js
 parseq/help/exts/animation.py
+parseq/tests/Cu-mix-res.png
+parseq/tests/Pb-mix-res.png
+parseq/tests/Zn-mix-res.png
 parseq/tests/_PySide2.py
 parseq/tests/__init__.py
+parseq/tests/_fit.py
 parseq/tests/_ft.py
 parseq/tests/_htmlwidgets.py
 parseq/tests/_test_LSQUnivariateSpline.py
+parseq/tests/_test_fit_local.py
 parseq/tests/_test_polyfit.py
 parseq/tests/_test_setup.py
 parseq/tests/circles-rect.png
 parseq/tests/circles.png
 parseq/tests/modeltest.py
 parseq/tests/test_QSortFilterProxyModel.py
 parseq/tests/test_ROI.py
@@ -119,24 +135,28 @@
 parseq/tests/test_combineSpectraWidget.py
 parseq/tests/test_commons.py
 parseq/tests/test_curve_shear.py
 parseq/tests/test_dataRebinWidget.py
 parseq/tests/test_dataTreeModelView.py
 parseq/tests/test_fileDialog.py
 parseq/tests/test_fileTreeModelView.py
+parseq/tests/test_fit.py
 parseq/tests/test_flowLayout.py
 parseq/tests/test_hdf5.py
 parseq/tests/test_mainWindow.py
 parseq/tests/test_node.py
 parseq/tests/test_nodeWidget.py
 parseq/tests/test_plotInteractiveImageROIwithKeys.py
 parseq/tests/test_plotInteractiveImageSingleROI.py
 parseq/tests/test_plotOptions.py
 parseq/tests/test_slice.py
 parseq/tests/test_stateButtons.py
+parseq/tests/data/cu-ref-mix.res
+parseq/tests/data/pb-ref-mix.res
+parseq/tests/data/zn-ref-mix.res
 parseq/third_party/XAFSmass.py
 parseq/third_party/__init__.py
 parseq/third_party/xrt.py
 parseq/third_party/data/Energies.txt
 parseq/utils/__init__.py
 parseq/utils/format.py
 parseq/utils/ft.py
```

