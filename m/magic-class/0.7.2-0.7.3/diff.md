# Comparing `tmp/magic_class-0.7.2.tar.gz` & `tmp/magic_class-0.7.3.tar.gz`

## Comparing `magic_class-0.7.2.tar` & `magic_class-0.7.3.tar`

### file list

```diff
@@ -1,137 +1,137 @@
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/__init__.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_app.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_register_types.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/command_palette.py
--rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/core.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/core.pyi
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/help.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/plot_api.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/signature.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/undo.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/__init__.py
--rw-r--r--   0        0        0    47075 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/_base.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/_dock_widget.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/_function_gui.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/_gui_modes.py
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/_icon.py
--rw-r--r--   0        0        0    23956 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/_macro.py
--rw-r--r--   0        0        0    12944 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/_macro_utils.py
--rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/_message_box.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/_napari_type.py
--rw-r--r--   0        0        0    26462 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/class_gui.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/keybinding.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/menu_gui.py
--rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/mgui_ext.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/runner.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/toolbar.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/_gui/utils.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/__init__.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/_doc.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/_shared_utils.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/dask/__init__.py
--rw-r--r--   0        0        0     8005 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/dask/progress.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/dask/resource.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/napari/__init__.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/napari/_magicgui.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/napari/types.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/napari/utils.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/napari/viewer.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/napari/widgets.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pandas/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pandas/_viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pandas/tests/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pandas/tests/test_viewer.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/polars/__init__.py
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/polars/_viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/polars/tests/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/polars/tests/test_viewer.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pyqtgraph/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pyqtgraph/_const.py
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pyqtgraph/components.py
--rw-r--r--   0        0        0    24189 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pyqtgraph/graph_items.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pyqtgraph/mouse_event.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pyqtgraph/plot_api.py
--rw-r--r--   0        0        0    32686 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pyqtgraph/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pyqtgraph/tests/__init__.py
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/pyqtgraph/tests/test_qtgraph.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/qtconsole/__init__.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/qtconsole/_qt.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/qtconsole/widgets.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/__init__.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/_base.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/camera.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/layer2d.py
--rw-r--r--   0        0        0    20691 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/layer3d.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/layerlist.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/plot_api.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/widgets2d.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/widgets3d.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/tests/__init__.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vispy/tests/test_vispy2d.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vtk/__init__.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vtk/components.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vtk/const.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vtk/volume.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/ext/vtk/widgets.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/fields/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/fields/_define.py
--rw-r--r--   0        0        0    29154 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/fields/_fields.py
--rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/fields/_group.py
--rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/fields/_property.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/functools/__init__.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/functools/_dispatch.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/functools/_partial.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/functools/_wraps.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/logging/__init__.py
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/logging/core.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/stylesheets/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/testing/__init__.py
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/testing/_function_gui_test.py
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/testing/_gui_test.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/types/__init__.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/types/_bound.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/types/_choices.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/types/_const.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/types/_expr.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/types/_optional.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/types/_path.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/types/_union.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/utils/__init__.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/utils/_click.py
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/utils/_functions.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/utils/_recent.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/utils/qt.py
--rw-r--r--   0        0        0    32376 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/utils/qthreading.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/utils/qtsignal.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/__init__.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/_html.py
--rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/_mpl_canvas.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/_union.py
--rw-r--r--   0        0        0    25634 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/codeedit.py
--rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/color.py
--rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/colormap.py
--rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/containers.py
--rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/eval.py
--rw-r--r--   0        0        0    20883 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/logger.py
--rw-r--r--   0        0        0    16683 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/misc.py
--rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/plot.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/separator.py
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/toggle_switch.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/utils.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/pywidgets/__init__.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/pywidgets/dict.py
--rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/pywidgets/list.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/pywidgets/object.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/pywidgets/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/tests/__init__.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/widgets/tests/test_eval.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/wrappers/__init__.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/wrappers/_abstractapi.py
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/wrappers/_confirm.py
--rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/wrappers/_misc.py
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 magic_class-0.7.2/magicclass/wrappers/_preview.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 magic_class-0.7.2/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 magic_class-0.7.2/LICENSE
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 magic_class-0.7.2/README.md
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 magic_class-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 magic_class-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/__init__.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_app.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_register_types.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/command_palette.py
+-rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/core.py
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/help.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/plot_api.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/signature.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/undo.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/__init__.py
+-rw-r--r--   0        0        0    47075 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_base.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_dock_widget.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_function_gui.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_gui_modes.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_icon.py
+-rw-r--r--   0        0        0    23956 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_macro.py
+-rw-r--r--   0        0        0    12944 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_macro_utils.py
+-rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_message_box.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/_napari_type.py
+-rw-r--r--   0        0        0    26462 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/class_gui.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/keybinding.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/menu_gui.py
+-rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/mgui_ext.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/runner.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/toolbar.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/_gui/utils.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/_doc.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/_shared_utils.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/dask/__init__.py
+-rw-r--r--   0        0        0     8005 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/dask/progress.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/dask/resource.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/__init__.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/_magicgui.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/types.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/utils.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/viewer.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/napari/widgets.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pandas/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pandas/_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pandas/tests/__init__.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pandas/tests/test_viewer.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/polars/__init__.py
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/polars/_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/polars/tests/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/polars/tests/test_viewer.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/_const.py
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/components.py
+-rw-r--r--   0        0        0    24189 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/graph_items.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/mouse_event.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/plot_api.py
+-rw-r--r--   0        0        0    32686 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/tests/__init__.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/pyqtgraph/tests/test_qtgraph.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/qtconsole/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/qtconsole/_qt.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/qtconsole/widgets.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/__init__.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/_base.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/camera.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/layer2d.py
+-rw-r--r--   0        0        0    20691 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/layer3d.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/layerlist.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/plot_api.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/widgets2d.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/widgets3d.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/tests/__init__.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vispy/tests/test_vispy2d.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vtk/__init__.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vtk/components.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vtk/const.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vtk/volume.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/ext/vtk/widgets.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/fields/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/fields/_define.py
+-rw-r--r--   0        0        0    29154 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/fields/_fields.py
+-rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/fields/_group.py
+-rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/fields/_property.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/functools/__init__.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/functools/_dispatch.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/functools/_partial.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/functools/_wraps.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/logging/__init__.py
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/logging/core.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/stylesheets/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/__init__.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_bound.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_choices.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_const.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_expr.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_optional.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_path.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/types/_union.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/__init__.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/_click.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/_functions.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/_recent.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/qt.py
+-rw-r--r--   0        0        0    32376 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/qthreading.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/utils/qtsignal.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/__init__.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/_html.py
+-rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/_mpl_canvas.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/_union.py
+-rw-r--r--   0        0        0    25634 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/codeedit.py
+-rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/color.py
+-rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/colormap.py
+-rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/containers.py
+-rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/eval.py
+-rw-r--r--   0        0        0    20883 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/logger.py
+-rw-r--r--   0        0        0    16683 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/misc.py
+-rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/plot.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/separator.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/toggle_switch.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/utils.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/pywidgets/__init__.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/pywidgets/dict.py
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/pywidgets/list.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/pywidgets/object.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/pywidgets/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/tests/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/widgets/tests/test_eval.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/wrappers/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/wrappers/_abstractapi.py
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/wrappers/_confirm.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/wrappers/_misc.py
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/wrappers/_preview.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/core.pyi
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/testing/__init__.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/testing/_function_gui_test.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 magic_class-0.7.3/magicclass/testing/_gui_test.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 magic_class-0.7.3/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 magic_class-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 magic_class-0.7.3/README.md
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 magic_class-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 magic_class-0.7.3/PKG-INFO
```

### Comparing `magic_class-0.7.2/magicclass/__init__.py` & `magic_class-0.7.3/magicclass/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 from .core import (
     magicclass,
     magicmenu,
     magiccontext,
     magictoolbar,
     Parameters,
```

### Comparing `magic_class-0.7.2/magicclass/_app.py` & `magic_class-0.7.3/magicclass/_app.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_register_types.py` & `magic_class-0.7.3/magicclass/_register_types.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/command_palette.py` & `magic_class-0.7.3/magicclass/command_palette.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/core.py` & `magic_class-0.7.3/magicclass/core.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/core.pyi` & `magic_class-0.7.3/magicclass/core.pyi`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/help.py` & `magic_class-0.7.3/magicclass/help.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/plot_api.py` & `magic_class-0.7.3/magicclass/plot_api.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/signature.py` & `magic_class-0.7.3/magicclass/signature.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/undo.py` & `magic_class-0.7.3/magicclass/undo.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/_base.py` & `magic_class-0.7.3/magicclass/_gui/_base.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/_dock_widget.py` & `magic_class-0.7.3/magicclass/_gui/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/_function_gui.py` & `magic_class-0.7.3/magicclass/_gui/_function_gui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/_gui_modes.py` & `magic_class-0.7.3/magicclass/_gui/_gui_modes.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/_icon.py` & `magic_class-0.7.3/magicclass/_gui/_icon.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/_macro.py` & `magic_class-0.7.3/magicclass/_gui/_macro.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/_macro_utils.py` & `magic_class-0.7.3/magicclass/_gui/_macro_utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/_message_box.py` & `magic_class-0.7.3/magicclass/_gui/_message_box.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/_napari_type.py` & `magic_class-0.7.3/magicclass/_gui/_napari_type.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/class_gui.py` & `magic_class-0.7.3/magicclass/_gui/class_gui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/keybinding.py` & `magic_class-0.7.3/magicclass/_gui/keybinding.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/menu_gui.py` & `magic_class-0.7.3/magicclass/_gui/menu_gui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/mgui_ext.py` & `magic_class-0.7.3/magicclass/_gui/mgui_ext.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/runner.py` & `magic_class-0.7.3/magicclass/_gui/runner.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/toolbar.py` & `magic_class-0.7.3/magicclass/_gui/toolbar.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/_gui/utils.py` & `magic_class-0.7.3/magicclass/_gui/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/_doc.py` & `magic_class-0.7.3/magicclass/ext/_doc.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/dask/progress.py` & `magic_class-0.7.3/magicclass/ext/dask/progress.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/dask/resource.py` & `magic_class-0.7.3/magicclass/ext/dask/resource.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/napari/_magicgui.py` & `magic_class-0.7.3/magicclass/ext/napari/_magicgui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/napari/types.py` & `magic_class-0.7.3/magicclass/ext/napari/types.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/napari/utils.py` & `magic_class-0.7.3/magicclass/ext/napari/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/napari/viewer.py` & `magic_class-0.7.3/magicclass/ext/napari/viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/napari/widgets.py` & `magic_class-0.7.3/magicclass/ext/napari/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/pandas/_viewer.py` & `magic_class-0.7.3/magicclass/ext/pandas/_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/pandas/tests/test_viewer.py` & `magic_class-0.7.3/magicclass/ext/pandas/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/polars/_viewer.py` & `magic_class-0.7.3/magicclass/ext/polars/_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/polars/tests/test_viewer.py` & `magic_class-0.7.3/magicclass/ext/polars/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/pyqtgraph/__init__.py` & `magic_class-0.7.3/magicclass/ext/pyqtgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/pyqtgraph/components.py` & `magic_class-0.7.3/magicclass/ext/pyqtgraph/components.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/pyqtgraph/graph_items.py` & `magic_class-0.7.3/magicclass/ext/pyqtgraph/graph_items.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/pyqtgraph/mouse_event.py` & `magic_class-0.7.3/magicclass/ext/pyqtgraph/mouse_event.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/pyqtgraph/plot_api.py` & `magic_class-0.7.3/magicclass/ext/pyqtgraph/plot_api.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/pyqtgraph/widgets.py` & `magic_class-0.7.3/magicclass/ext/pyqtgraph/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/pyqtgraph/tests/test_qtgraph.py` & `magic_class-0.7.3/magicclass/ext/pyqtgraph/tests/test_qtgraph.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/qtconsole/__init__.py` & `magic_class-0.7.3/magicclass/ext/qtconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/qtconsole/_qt.py` & `magic_class-0.7.3/magicclass/ext/qtconsole/_qt.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/qtconsole/widgets.py` & `magic_class-0.7.3/magicclass/ext/qtconsole/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vispy/_base.py` & `magic_class-0.7.3/magicclass/ext/vispy/_base.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vispy/camera.py` & `magic_class-0.7.3/magicclass/ext/vispy/camera.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vispy/layer2d.py` & `magic_class-0.7.3/magicclass/ext/vispy/layer2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vispy/layer3d.py` & `magic_class-0.7.3/magicclass/ext/vispy/layer3d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vispy/layerlist.py` & `magic_class-0.7.3/magicclass/ext/vispy/layerlist.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vispy/plot_api.py` & `magic_class-0.7.3/magicclass/ext/vispy/plot_api.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vispy/widgets2d.py` & `magic_class-0.7.3/magicclass/ext/vispy/widgets2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vispy/widgets3d.py` & `magic_class-0.7.3/magicclass/ext/vispy/widgets3d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vispy/tests/test_vispy2d.py` & `magic_class-0.7.3/magicclass/ext/vispy/tests/test_vispy2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vtk/components.py` & `magic_class-0.7.3/magicclass/ext/vtk/components.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vtk/const.py` & `magic_class-0.7.3/magicclass/ext/vtk/const.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vtk/volume.py` & `magic_class-0.7.3/magicclass/ext/vtk/volume.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/ext/vtk/widgets.py` & `magic_class-0.7.3/magicclass/ext/vtk/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/fields/_define.py` & `magic_class-0.7.3/magicclass/fields/_define.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/fields/_fields.py` & `magic_class-0.7.3/magicclass/fields/_fields.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/fields/_group.py` & `magic_class-0.7.3/magicclass/fields/_group.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/fields/_property.py` & `magic_class-0.7.3/magicclass/fields/_property.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/functools/_dispatch.py` & `magic_class-0.7.3/magicclass/functools/_dispatch.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/functools/_partial.py` & `magic_class-0.7.3/magicclass/functools/_partial.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/functools/_wraps.py` & `magic_class-0.7.3/magicclass/functools/_wraps.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/logging/core.py` & `magic_class-0.7.3/magicclass/logging/core.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/stylesheets/__init__.py` & `magic_class-0.7.3/magicclass/stylesheets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/testing/_function_gui_test.py` & `magic_class-0.7.3/magicclass/testing/_function_gui_test.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/testing/_gui_test.py` & `magic_class-0.7.3/magicclass/testing/_gui_test.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/types/__init__.py` & `magic_class-0.7.3/magicclass/types/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/types/_bound.py` & `magic_class-0.7.3/magicclass/types/_bound.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/types/_choices.py` & `magic_class-0.7.3/magicclass/types/_choices.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/types/_const.py` & `magic_class-0.7.3/magicclass/types/_const.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/types/_expr.py` & `magic_class-0.7.3/magicclass/types/_expr.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/types/_optional.py` & `magic_class-0.7.3/magicclass/types/_optional.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/types/_path.py` & `magic_class-0.7.3/magicclass/types/_path.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/types/_union.py` & `magic_class-0.7.3/magicclass/types/_union.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/utils/__init__.py` & `magic_class-0.7.3/magicclass/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/utils/_click.py` & `magic_class-0.7.3/magicclass/utils/_click.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/utils/_functions.py` & `magic_class-0.7.3/magicclass/utils/_functions.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/utils/_recent.py` & `magic_class-0.7.3/magicclass/utils/_recent.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/utils/qt.py` & `magic_class-0.7.3/magicclass/utils/qt.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/utils/qthreading.py` & `magic_class-0.7.3/magicclass/utils/qthreading.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/__init__.py` & `magic_class-0.7.3/magicclass/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/_html.py` & `magic_class-0.7.3/magicclass/widgets/_html.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/_mpl_canvas.py` & `magic_class-0.7.3/magicclass/widgets/_mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/_union.py` & `magic_class-0.7.3/magicclass/widgets/_union.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/codeedit.py` & `magic_class-0.7.3/magicclass/widgets/codeedit.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/color.py` & `magic_class-0.7.3/magicclass/widgets/color.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/colormap.py` & `magic_class-0.7.3/magicclass/widgets/colormap.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/containers.py` & `magic_class-0.7.3/magicclass/widgets/containers.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/eval.py` & `magic_class-0.7.3/magicclass/widgets/eval.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/logger.py` & `magic_class-0.7.3/magicclass/widgets/logger.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/misc.py` & `magic_class-0.7.3/magicclass/widgets/misc.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/plot.py` & `magic_class-0.7.3/magicclass/widgets/plot.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/separator.py` & `magic_class-0.7.3/magicclass/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/toggle_switch.py` & `magic_class-0.7.3/magicclass/widgets/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/utils.py` & `magic_class-0.7.3/magicclass/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/pywidgets/__init__.py` & `magic_class-0.7.3/magicclass/widgets/pywidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/pywidgets/dict.py` & `magic_class-0.7.3/magicclass/widgets/pywidgets/dict.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/pywidgets/list.py` & `magic_class-0.7.3/magicclass/widgets/pywidgets/list.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/pywidgets/object.py` & `magic_class-0.7.3/magicclass/widgets/pywidgets/object.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/pywidgets/tree.py` & `magic_class-0.7.3/magicclass/widgets/pywidgets/tree.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/widgets/tests/test_eval.py` & `magic_class-0.7.3/magicclass/widgets/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/wrappers/__init__.py` & `magic_class-0.7.3/magicclass/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/wrappers/_abstractapi.py` & `magic_class-0.7.3/magicclass/wrappers/_abstractapi.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/wrappers/_confirm.py` & `magic_class-0.7.3/magicclass/wrappers/_confirm.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/wrappers/_misc.py` & `magic_class-0.7.3/magicclass/wrappers/_misc.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/magicclass/wrappers/_preview.py` & `magic_class-0.7.3/magicclass/wrappers/_preview.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/.gitignore` & `magic_class-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/LICENSE` & `magic_class-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/README.md` & `magic_class-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.2/pyproject.toml` & `magic_class-0.7.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -51,16 +51,22 @@
 Download = "https://github.com/hanjinliu/magic-class"
 
 [tool.hatch.version]
 path = "magicclass/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = ["/magicclass"]
+exclude = ["/examples", "/rst", "/tests", "setup.py"]
+
+[tool.hatch.build.targets.sdist.force-include]
+"magicclass/core.pyi" = "magicclass/core.pyi"
+"magicclass/testing" = "magicclass/testing"
 
 [tool.hatch.build.targets.wheel]
+include = ["/magicclass"]
 exclude = ["/examples", "/rst", "/tests", "setup.py"]
 
 [tool.hatch.build.targets.wheel.force-include]
 "magicclass/core.pyi" = "magicclass/core.pyi"
 "magicclass/testing" = "magicclass/testing"
 
 [tool.pytest.ini_options]
```

### Comparing `magic_class-0.7.2/PKG-INFO` & `magic_class-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-class
-Version: 0.7.2
+Version: 0.7.3
 Summary: Generate multifunctional GUIs from classes
 Project-URL: Download, https://github.com/hanjinliu/magic-class
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, hanjinliu
         All rights reserved.
```

