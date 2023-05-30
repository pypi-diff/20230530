# Comparing `tmp/tabulous-0.5.2.tar.gz` & `tmp/tabulous-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabulous-0.5.2.tar", last modified: Fri Apr 14 14:02:52 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `tabulous-0.5.2.tar` & `tabulous-0.5.3.tar`

### file list

```diff
@@ -1,416 +1,205 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:51.905140 tabulous-0.5.2/
--rw-rw-rw-   0        0        0     1547 2022-05-31 07:07:35.000000 tabulous-0.5.2/LICENSE
--rw-rw-rw-   0        0        0       81 2022-08-18 11:35:12.000000 tabulous-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2394 2023-04-14 14:02:51.896357 tabulous-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     1965 2023-04-09 14:02:29.000000 tabulous-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:37.906768 tabulous-0.5.2/docs/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:39.057584 tabulous-0.5.2/docs/_images/
--rw-rw-rw-   0        0        0     8521 2023-04-09 14:02:30.000000 tabulous-0.5.2/docs/_images/cell_labels.png
--rw-rw-rw-   0        0        0    54466 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/colormap.png
--rw-rw-rw-   0        0        0    28354 2023-04-09 14:02:30.000000 tabulous-0.5.2/docs/_images/colormap_interpolate.png
--rw-rw-rw-   0        0        0    35913 2023-04-09 14:02:30.000000 tabulous-0.5.2/docs/_images/column_filter.png
--rw-rw-rw-   0        0        0    72490 2023-04-09 14:02:30.000000 tabulous-0.5.2/docs/_images/command_palette.png
--rw-rw-rw-   0        0        0     1116 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/copy.svg
--rw-rw-rw-   0        0        0     1487 2023-04-14 14:01:38.000000 tabulous-0.5.2/docs/_images/copy_as_spreadsheet.svg
--rw-rw-rw-   0        0        0     1186 2023-04-14 14:01:38.000000 tabulous-0.5.2/docs/_images/copy_as_table.svg
--rw-rw-rw-   0        0        0     1319 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/cut.svg
--rw-rw-rw-   0        0        0    46434 2023-04-09 14:02:30.000000 tabulous-0.5.2/docs/_images/dock_with_table_data_annotation.png
--rw-rw-rw-   0        0        0    28476 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/edit_cell.png
--rw-rw-rw-   0        0        0     1694 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/eval.svg
--rw-rw-rw-   0        0        0      702 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/filter.svg
--rw-rw-rw-   0        0        0      646 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/find_item.svg
--rw-rw-rw-   0        0        0    29909 2023-04-09 14:02:30.000000 tabulous-0.5.2/docs/_images/formatter.png
--rw-rw-rw-   0        0        0     1135 2023-04-14 14:01:38.000000 tabulous-0.5.2/docs/_images/groupby.svg
--rw-rw-rw-   0        0        0     1354 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/hist.svg
--rw-rw-rw-   0        0        0      939 2023-04-14 14:01:39.000000 tabulous-0.5.2/docs/_images/melt.svg
--rw-rw-rw-   0        0        0     1169 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/new_figure.svg
--rw-rw-rw-   0        0        0     1501 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/open_sample.svg
--rw-rw-rw-   0        0        0     1741 2023-04-14 14:01:39.000000 tabulous-0.5.2/docs/_images/open_spreadsheet.svg
--rw-rw-rw-   0        0        0     1416 2023-04-14 14:01:38.000000 tabulous-0.5.2/docs/_images/open_table.svg
--rw-rw-rw-   0        0        0      820 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/optimize.svg
--rw-rw-rw-   0        0        0     2016 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/palette.svg
--rw-rw-rw-   0        0        0     1090 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/paste.svg
--rw-rw-rw-   0        0        0     1166 2023-04-14 14:01:39.000000 tabulous-0.5.2/docs/_images/pivot.svg
--rw-rw-rw-   0        0        0      720 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/plot.svg
--rw-rw-rw-   0        0        0     1045 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/redo.svg
--rw-rw-rw-   0        0        0     1243 2023-04-14 14:01:38.000000 tabulous-0.5.2/docs/_images/save_table.svg
--rw-rw-rw-   0        0        0     4229 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/scatter.svg
--rw-rw-rw-   0        0        0     3472 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/sklearn_analysis.svg
--rw-rw-rw-   0        0        0      795 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/sort_table.svg
--rw-rw-rw-   0        0        0     6345 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/spreadsheet.png
--rw-rw-rw-   0        0        0     1254 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/stats_test.svg
--rw-rw-rw-   0        0        0     1070 2023-04-14 14:01:38.000000 tabulous-0.5.2/docs/_images/summarize_table.svg
--rw-rw-rw-   0        0        0     1633 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/switch_header.svg
--rw-rw-rw-   0        0        0     1195 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/switch_layout.svg
--rw-rw-rw-   0        0        0     5885 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/table.png
--rw-rw-rw-   0        0        0     1109 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/tile.svg
--rw-rw-rw-   0        0        0    32696 2023-04-09 14:02:30.000000 tabulous-0.5.2/docs/_images/tile_tables.png
--rw-rw-rw-   0        0        0      988 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/toggle_console.svg
--rw-rw-rw-   0        0        0      985 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/undo.svg
--rw-rw-rw-   0        0        0      820 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_images/untile.svg
--rw-rw-rw-   0        0        0    28693 2023-04-09 14:02:30.000000 tabulous-0.5.2/docs/_images/validator.png
--rw-rw-rw-   0        0        0      804 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/view_dual_h.svg
--rw-rw-rw-   0        0        0      849 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/view_dual_v.svg
--rw-rw-rw-   0        0        0      847 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/view_popup.svg
--rw-rw-rw-   0        0        0      688 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_images/view_reset.svg
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:39.076094 tabulous-0.5.2/docs/_sources/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:39.177539 tabulous-0.5.2/docs/_sources/apidoc/
--rw-rw-rw-   0        0        0       68 2023-01-08 16:07:50.000000 tabulous-0.5.2/docs/_sources/apidoc/modules.rst.txt
--rw-rw-rw-   0        0        0     1716 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/apidoc/tabulous.commands.rst.txt
--rw-rw-rw-   0        0        0     1180 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/apidoc/tabulous.rst.txt
--rw-rw-rw-   0        0        0      175 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/apidoc/tabulous.style.rst.txt
--rw-rw-rw-   0        0        0      181 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/apidoc/tabulous.widgets.rst.txt
--rw-rw-rw-   0        0        0      282 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/font.rst.txt
--rw-rw-rw-   0        0        0     1061 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:39.485163 tabulous-0.5.2/docs/_sources/main/
--rw-rw-rw-   0        0        0     1269 2022-08-18 11:35:12.000000 tabulous-0.5.2/docs/_sources/main/cheat_sheet.rst.txt
--rw-rw-rw-   0        0        0     9765 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/main/columnwise_settings.rst.txt
--rw-rw-rw-   0        0        0     4319 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/main/customize.rst.txt
--rw-rw-rw-   0        0        0     3720 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/main/integrate_custom_widgets.rst.txt
--rw-rw-rw-   0        0        0     3339 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/main/non_mainwindow.rst.txt
--rw-rw-rw-   0        0        0     7179 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/main/quickstart.rst.txt
--rw-rw-rw-   0        0        0     5078 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/main/register_action.rst.txt
--rw-rw-rw-   0        0        0     2890 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/main/selections.rst.txt
--rw-rw-rw-   0        0        0     5196 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/main/sort_filter.rst.txt
--rw-rw-rw-   0        0        0     6196 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/main/table_fields.rst.txt
--rw-rw-rw-   0        0        0     2937 2023-04-09 14:02:29.000000 tabulous-0.5.2/docs/_sources/main/table_view_mode.rst.txt
--rw-rw-rw-   0        0        0    13494 2023-04-09 14:02:30.000000 tabulous-0.5.2/docs/_sources/main/user_interface.rst.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:39.620755 tabulous-0.5.2/docs/_static/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:37.913763 tabulous-0.5.2/docs/_static/css/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:39.809886 tabulous-0.5.2/docs/_static/css/fonts/
--rw-rw-rw-   0        0        0   443670 2023-04-14 14:01:42.000000 tabulous-0.5.2/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0      286 2022-09-17 09:06:46.000000 tabulous-0.5.2/docs/_static/file.png
--rw-rw-rw-   0        0        0       90 2022-09-17 09:06:46.000000 tabulous-0.5.2/docs/_static/minus.png
--rw-rw-rw-   0        0        0       90 2022-09-17 09:06:46.000000 tabulous-0.5.2/docs/_static/plus.png
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:40.277961 tabulous-0.5.2/image/
--rw-rw-rw-   0        0        0    46061 2023-04-09 14:02:30.000000 tabulous-0.5.2/image/colormap_example.png
--rw-rw-rw-   0        0        0    51506 2023-04-09 14:02:30.000000 tabulous-0.5.2/image/command_palette_example.png
--rw-rw-rw-   0        0        0    43269 2023-04-09 14:02:30.000000 tabulous-0.5.2/image/custom_widget_example.png
--rw-rw-rw-   0        0        0    47699 2023-04-09 14:02:30.000000 tabulous-0.5.2/image/eval_example.png
--rw-rw-rw-   0        0        0    46306 2023-04-09 14:02:30.000000 tabulous-0.5.2/image/filter_example.png
--rw-rw-rw-   0        0        0    36605 2023-04-09 14:02:30.000000 tabulous-0.5.2/image/sort_example.png
--rw-rw-rw-   0        0        0    60682 2023-04-09 14:02:30.000000 tabulous-0.5.2/image/viewer_example.png
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:37.967920 tabulous-0.5.2/rst/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:37.936883 tabulous-0.5.2/rst/_build/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:37.956933 tabulous-0.5.2/rst/_build/html/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:42.063290 tabulous-0.5.2/rst/_build/html/_images/
--rw-rw-rw-   0        0        0   137599 2022-08-27 05:30:56.000000 tabulous-0.5.2/rst/_build/html/_images/colormap.png
--rw-rw-rw-   0        0        0     1084 2022-08-18 11:35:13.000000 tabulous-0.5.2/rst/_build/html/_images/concat.svg
--rw-rw-rw-   0        0        0     1486 2022-08-18 11:31:01.000000 tabulous-0.5.2/rst/_build/html/_images/copy_as_spreadsheet.svg
--rw-rw-rw-   0        0        0     1185 2022-08-18 11:31:01.000000 tabulous-0.5.2/rst/_build/html/_images/copy_as_table.svg
--rw-rw-rw-   0        0        0     1694 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/eval.svg
--rw-rw-rw-   0        0        0    88144 2022-08-13 11:18:49.000000 tabulous-0.5.2/rst/_build/html/_images/filter.png
--rw-rw-rw-   0        0        0      702 2022-08-07 04:17:51.000000 tabulous-0.5.2/rst/_build/html/_images/filter.svg
--rw-rw-rw-   0        0        0      646 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/find_item.svg
--rw-rw-rw-   0        0        0     1134 2022-08-18 11:31:01.000000 tabulous-0.5.2/rst/_build/html/_images/groupby.svg
--rw-rw-rw-   0        0        0     1354 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/hist.svg
--rw-rw-rw-   0        0        0      938 2022-08-18 11:31:01.000000 tabulous-0.5.2/rst/_build/html/_images/melt.svg
--rw-rw-rw-   0        0        0     1169 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/new_figure.svg
--rw-rw-rw-   0        0        0      766 2022-09-13 15:15:41.000000 tabulous-0.5.2/rst/_build/html/_images/open_sample.svg
--rw-rw-rw-   0        0        0     1740 2022-08-18 11:31:01.000000 tabulous-0.5.2/rst/_build/html/_images/open_spreadsheet.svg
--rw-rw-rw-   0        0        0     1415 2022-08-18 11:31:01.000000 tabulous-0.5.2/rst/_build/html/_images/open_table.svg
--rw-rw-rw-   0        0        0     1165 2022-08-18 11:31:01.000000 tabulous-0.5.2/rst/_build/html/_images/pivot.svg
--rw-rw-rw-   0        0        0      720 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/plot.svg
--rw-rw-rw-   0        0        0     1242 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/save_table.svg
--rw-rw-rw-   0        0        0     4229 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/scatter.svg
--rw-rw-rw-   0        0        0      795 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/sort_table.svg
--rw-rw-rw-   0        0        0     1069 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/summarize_table.svg
--rw-rw-rw-   0        0        0     1633 2022-10-26 14:58:02.000000 tabulous-0.5.2/rst/_build/html/_images/switch_header.svg
--rw-rw-rw-   0        0        0      988 2022-08-07 04:18:25.000000 tabulous-0.5.2/rst/_build/html/_images/toggle_console.svg
--rw-rw-rw-   0        0        0      804 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/view_dual_h.svg
--rw-rw-rw-   0        0        0      849 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/view_dual_v.svg
--rw-rw-rw-   0        0        0      847 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/view_popup.svg
--rw-rw-rw-   0        0        0      688 2022-08-18 11:35:12.000000 tabulous-0.5.2/rst/_build/html/_images/view_reset.svg
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:42.135667 tabulous-0.5.2/rst/_build/html/_sources/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:42.501161 tabulous-0.5.2/rst/_build/html/_sources/apidoc/
--rw-rw-rw-   0        0        0       68 2022-08-01 17:00:41.000000 tabulous-0.5.2/rst/_build/html/_sources/apidoc/modules.rst.txt
--rw-rw-rw-   0        0        0      835 2022-08-01 17:00:41.000000 tabulous-0.5.2/rst/_build/html/_sources/apidoc/tabulous.rst.txt
--rw-rw-rw-   0        0        0      560 2022-08-27 05:56:25.000000 tabulous-0.5.2/rst/_build/html/_sources/apidoc/tabulous.widgets.rst.txt
--rw-rw-rw-   0        0        0      996 2022-09-14 13:14:23.000000 tabulous-0.5.2/rst/_build/html/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:43.568745 tabulous-0.5.2/rst/_build/html/_sources/main/
--rw-rw-rw-   0        0        0     1374 2022-09-13 15:30:15.000000 tabulous-0.5.2/rst/_build/html/_sources/main/cell_color.rst.txt
--rw-rw-rw-   0        0        0     1269 2022-08-01 17:28:01.000000 tabulous-0.5.2/rst/_build/html/_sources/main/cheat_sheet.rst.txt
--rw-rw-rw-   0        0        0     5314 2022-10-23 04:08:52.000000 tabulous-0.5.2/rst/_build/html/_sources/main/columnwise_settings.rst.txt
--rw-rw-rw-   0        0        0     1309 2022-08-01 17:00:41.000000 tabulous-0.5.2/rst/_build/html/_sources/main/dock_widget.rst.txt
--rw-rw-rw-   0        0        0     1623 2022-10-23 04:05:29.000000 tabulous-0.5.2/rst/_build/html/_sources/main/filter.rst.txt
--rw-rw-rw-   0        0        0       70 2022-08-03 13:49:35.000000 tabulous-0.5.2/rst/_build/html/_sources/main/keycombo.rst.txt
--rw-rw-rw-   0        0        0     3284 2022-08-13 12:30:19.000000 tabulous-0.5.2/rst/_build/html/_sources/main/non_mainwindow.rst.txt
--rw-rw-rw-   0        0        0     6834 2022-09-14 13:25:48.000000 tabulous-0.5.2/rst/_build/html/_sources/main/quickstart.rst.txt
--rw-rw-rw-   0        0        0     2387 2022-08-29 14:15:05.000000 tabulous-0.5.2/rst/_build/html/_sources/main/register_action.rst.txt
--rw-rw-rw-   0        0        0     2883 2022-09-03 02:40:25.000000 tabulous-0.5.2/rst/_build/html/_sources/main/selections.rst.txt
--rw-rw-rw-   0        0        0     5126 2022-10-23 05:07:47.000000 tabulous-0.5.2/rst/_build/html/_sources/main/table_advanced.rst.txt
--rw-rw-rw-   0        0        0     9993 2022-10-23 05:07:47.000000 tabulous-0.5.2/rst/_build/html/_sources/main/user_interface.rst.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:43.615018 tabulous-0.5.2/rst/_build/html/_static/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:37.962883 tabulous-0.5.2/rst/_build/html/_static/css/
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:43.772010 tabulous-0.5.2/rst/_build/html/_static/css/fonts/
--rw-rw-rw-   0        0        0   444379 2022-07-29 08:41:11.000000 tabulous-0.5.2/rst/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0      286 2022-07-29 08:39:26.000000 tabulous-0.5.2/rst/_build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2022-07-29 08:39:26.000000 tabulous-0.5.2/rst/_build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2022-07-29 08:39:26.000000 tabulous-0.5.2/rst/_build/html/_static/plus.png
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:44.390476 tabulous-0.5.2/rst/fig/
--rw-rw-rw-   0        0        0     8521 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/cell_labels.png
--rw-rw-rw-   0        0        0    54466 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/colormap.png
--rw-rw-rw-   0        0        0    28354 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/colormap_interpolate.png
--rw-rw-rw-   0        0        0    35913 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/column_filter.png
--rw-rw-rw-   0        0        0    72490 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/command_palette.png
--rw-rw-rw-   0        0        0    46434 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/dock_with_table_data_annotation.png
--rw-rw-rw-   0        0        0    28476 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/edit_cell.png
--rw-rw-rw-   0        0        0    29909 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/formatter.png
--rw-rw-rw-   0        0        0     6345 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/spreadsheet.png
--rw-rw-rw-   0        0        0     5885 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/table.png
--rw-rw-rw-   0        0        0    32696 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/tile_tables.png
--rw-rw-rw-   0        0        0    28693 2023-04-09 14:02:30.000000 tabulous-0.5.2/rst/fig/validator.png
--rw-rw-rw-   0        0        0       42 2023-04-14 14:02:51.906179 tabulous-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1631 2023-04-13 12:12:18.000000 tabulous-0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:44.704587 tabulous-0.5.2/tabulous/
--rw-rw-rw-   0        0        0      490 2023-04-14 14:01:17.000000 tabulous-0.5.2/tabulous/__init__.py
--rw-rw-rw-   0        0        0     2603 2023-04-11 00:04:09.000000 tabulous-0.5.2/tabulous/__main__.py
--rw-rw-rw-   0        0        0     5310 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_colormap.py
--rw-rw-rw-   0        0        0    11502 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_dtype.py
--rw-rw-rw-   0        0        0     1126 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_fetch_and_install.py
--rw-rw-rw-   0        0        0     1654 2023-04-09 14:21:30.000000 tabulous-0.5.2/tabulous/_io.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:45.190941 tabulous-0.5.2/tabulous/_keymap/
--rw-rw-rw-   0        0        0      138 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_keymap/__init__.py
--rw-rw-rw-   0        0        0     3291 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_keymap/_callback.py
--rw-rw-rw-   0        0        0    22135 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_keymap/_keymap_objects.py
--rw-rw-rw-   0        0        0     5184 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_keymap/_keymapview.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:45.386945 tabulous-0.5.2/tabulous/_magicgui/
--rw-rw-rw-   0        0        0      827 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_magicgui/__init__.py
--rw-rw-rw-   0        0        0     5175 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_magicgui/_color_edit.py
--rw-rw-rw-   0        0        0     5020 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_magicgui/_dialog.py
--rw-rw-rw-   0        0        0     8402 2023-04-14 11:13:41.000000 tabulous-0.5.2/tabulous/_magicgui/_register.py
--rw-rw-rw-   0        0        0     3852 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_magicgui/_selection.py
--rw-rw-rw-   0        0        0     1743 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_magicgui/_table.py
--rw-rw-rw-   0        0        0     7798 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_magicgui/_timedelta.py
--rw-rw-rw-   0        0        0     9735 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_magicgui/_toggle_switch.py
--rw-rw-rw-   0        0        0     8796 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_map_model.py
--rw-rw-rw-   0        0        0     3437 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_pd_index.py
--rw-rw-rw-   0        0        0    66098 2023-04-13 12:11:17.000000 tabulous-0.5.2/tabulous/_psygnal.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:46.040040 tabulous-0.5.2/tabulous/_qt/
--rw-rw-rw-   0        0        0      385 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/__init__.py
--rw-rw-rw-   0        0        0     4510 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_action_registry.py
--rw-rw-rw-   0        0        0     2041 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_app.py
--rw-rw-rw-   0        0        0     1795 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_clickable_label.py
--rw-rw-rw-   0        0        0    10690 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_console.py
--rw-rw-rw-   0        0        0     2073 2022-09-09 08:21:21.000000 tabulous-0.5.2/tabulous/_qt/_dockwidget.py
--rw-rw-rw-   0        0        0     3271 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_filetree.py
--rw-rw-rw-   0        0        0     4692 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_history.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:47.515766 tabulous-0.5.2/tabulous/_qt/_icons/
--rw-rw-rw-   0        0        0      936 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/barplot.svg
--rw-rw-rw-   0        0        0     1739 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/boxenplot.svg
--rw-rw-rw-   0        0        0     1196 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/boxplot.svg
--rw-rw-rw-   0        0        0     1116 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/copy.svg
--rw-rw-rw-   0        0        0     1486 2022-08-18 11:31:01.000000 tabulous-0.5.2/tabulous/_qt/_icons/copy_as_spreadsheet.svg
--rw-rw-rw-   0        0        0     1185 2022-08-18 11:31:01.000000 tabulous-0.5.2/tabulous/_qt/_icons/copy_as_table.svg
--rw-rw-rw-   0        0        0     1319 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/cut.svg
--rw-rw-rw-   0        0        0     1694 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/eval.svg
--rw-rw-rw-   0        0        0      702 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/filter.svg
--rw-rw-rw-   0        0        0      646 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/find_item.svg
--rw-rw-rw-   0        0        0     1134 2022-08-18 11:31:01.000000 tabulous-0.5.2/tabulous/_qt/_icons/groupby.svg
--rw-rw-rw-   0        0        0     1354 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/hist.svg
--rw-rw-rw-   0        0        0      938 2022-08-18 11:31:01.000000 tabulous-0.5.2/tabulous/_qt/_icons/melt.svg
--rw-rw-rw-   0        0        0     1248 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/more.svg
--rw-rw-rw-   0        0        0     1169 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/new_figure.svg
--rw-rw-rw-   0        0        0      860 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/new_spreadsheet.svg
--rw-rw-rw-   0        0        0     1501 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/open_sample.svg
--rw-rw-rw-   0        0        0     1740 2022-08-18 11:31:01.000000 tabulous-0.5.2/tabulous/_qt/_icons/open_spreadsheet.svg
--rw-rw-rw-   0        0        0     1415 2022-08-18 11:31:01.000000 tabulous-0.5.2/tabulous/_qt/_icons/open_table.svg
--rw-rw-rw-   0        0        0      820 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/optimize.svg
--rw-rw-rw-   0        0        0     2016 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/palette.svg
--rw-rw-rw-   0        0        0     1090 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/paste.svg
--rw-rw-rw-   0        0        0     1165 2022-08-18 11:31:01.000000 tabulous-0.5.2/tabulous/_qt/_icons/pivot.svg
--rw-rw-rw-   0        0        0      720 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/plot.svg
--rw-rw-rw-   0        0        0     1704 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/preferences.svg
--rw-rw-rw-   0        0        0     2817 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/random.svg
--rw-rw-rw-   0        0        0     1045 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/redo.svg
--rw-rw-rw-   0        0        0     1293 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/round.svg
--rw-rw-rw-   0        0        0     1242 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/save_table.svg
--rw-rw-rw-   0        0        0     4229 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/scatter.svg
--rw-rw-rw-   0        0        0     1706 2022-10-26 14:58:02.000000 tabulous-0.5.2/tabulous/_qt/_icons/settings.svg
--rw-rw-rw-   0        0        0     3472 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/sklearn_analysis.svg
--rw-rw-rw-   0        0        0      795 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/sort_table.svg
--rw-rw-rw-   0        0        0     1254 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/stats_test.svg
--rw-rw-rw-   0        0        0     1069 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/summarize_table.svg
--rw-rw-rw-   0        0        0     4074 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/swarmplot.svg
--rw-rw-rw-   0        0        0     1633 2022-10-26 14:58:02.000000 tabulous-0.5.2/tabulous/_qt/_icons/switch_header.svg
--rw-rw-rw-   0        0        0     1195 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/switch_layout.svg
--rw-rw-rw-   0        0        0     1109 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/tile.svg
--rw-rw-rw-   0        0        0      988 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/toggle_console.svg
--rw-rw-rw-   0        0        0      985 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/undo.svg
--rw-rw-rw-   0        0        0      820 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_icons/untile.svg
--rw-rw-rw-   0        0        0      804 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/view_dual_h.svg
--rw-rw-rw-   0        0        0      849 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/view_dual_v.svg
--rw-rw-rw-   0        0        0      847 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/view_popup.svg
--rw-rw-rw-   0        0        0      688 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/view_reset.svg
--rw-rw-rw-   0        0        0    12285 2022-08-18 11:35:12.000000 tabulous-0.5.2/tabulous/_qt/_icons/window_icon.png
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:47.880176 tabulous-0.5.2/tabulous/_qt/_mainwindow/
--rw-rw-rw-   0        0        0      258 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_mainwindow/__init__.py
--rw-rw-rw-   0        0        0     8743 2023-04-14 12:46:32.000000 tabulous-0.5.2/tabulous/_qt/_mainwindow/_base.py
--rw-rw-rw-   0        0        0     2433 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_mainwindow/_command_palette.py
--rw-rw-rw-   0        0        0     1832 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_mainwindow/_keycombo.py
--rw-rw-rw-   0        0        0    11441 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_mainwindow/_mainwidgets.py
--rw-rw-rw-   0        0        0     1890 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_mainwindow/_namespace.py
--rw-rw-rw-   0        0        0     5059 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_mainwindow/_titlebar.py
--rw-rw-rw-   0        0        0     1822 2022-10-26 14:58:02.000000 tabulous-0.5.2/tabulous/_qt/_multitips.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:48.000300 tabulous-0.5.2/tabulous/_qt/_plot/
--rw-rw-rw-   0        0        0       71 2022-09-11 14:29:12.000000 tabulous-0.5.2/tabulous/_qt/_plot/__init__.py
--rw-rw-rw-   0        0        0    15100 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_plot/_artist_editors.py
--rw-rw-rw-   0        0        0     1352 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_plot/_artist_types.py
--rw-rw-rw-   0        0        0    10004 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_plot/_mpl_canvas.py
--rw-rw-rw-   0        0        0     4833 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_plot/_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:48.078432 tabulous-0.5.2/tabulous/_qt/_preference/
--rw-rw-rw-   0        0        0       73 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_preference/__init__.py
--rw-rw-rw-   0        0        0     2446 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_preference/_general.py
--rw-rw-rw-   0        0        0     2284 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_preference/_main.py
--rw-rw-rw-   0        0        0      785 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_preference/_shared.py
--rw-rw-rw-   0        0        0     4432 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_preference/_table_config.py
--rw-rw-rw-   0        0        0     3373 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_preference/_theme.py
--rw-rw-rw-   0        0        0     5836 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_progress.py
--rw-rw-rw-   0        0        0    12824 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_proxy_button.py
--rw-rw-rw-   0        0        0      212 2022-10-26 14:58:02.000000 tabulous-0.5.2/tabulous/_qt/_qt_const.py
--rw-rw-rw-   0        0        0     2654 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_svg.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:48.158549 tabulous-0.5.2/tabulous/_qt/_table/
--rw-rw-rw-   0        0        0      370 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:48.634229 tabulous-0.5.2/tabulous/_qt/_table/_base/
--rw-rw-rw-   0        0        0      503 2022-08-19 12:16:19.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/__init__.py
--rw-rw-rw-   0        0        0     5658 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_delegate.py
--rw-rw-rw-   0        0        0    26083 2023-04-14 11:35:13.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_enhanced_table.py
--rw-rw-rw-   0        0        0     9934 2023-04-14 11:38:50.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_header_view.py
--rw-rw-rw-   0        0        0    13511 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_item_model.py
--rw-rw-rw-   0        0        0     4761 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_keycombo.py
--rw-rw-rw-   0        0        0    28363 2023-04-14 11:30:13.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_line_edit.py
--rw-rw-rw-   0        0        0     1291 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_object_holder.py
--rw-rw-rw-   0        0        0     4113 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_overlay.py
--rw-rw-rw-   0        0        0     4275 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_side_area.py
--rw-rw-rw-   0        0        0    58650 2023-04-11 02:54:15.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_table_base.py
--rw-rw-rw-   0        0        0     4497 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_table_group.py
--rw-rw-rw-   0        0        0     3762 2022-10-26 14:58:02.000000 tabulous-0.5.2/tabulous/_qt/_table/_base/_table_wrappers.py
--rw-rw-rw-   0        0        0     8721 2022-09-11 14:29:12.000000 tabulous-0.5.2/tabulous/_qt/_table/_display.py
--rw-rw-rw-   0        0        0     6917 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table/_groupby.py
--rw-rw-rw-   0        0        0    35631 2023-04-11 12:21:04.000000 tabulous-0.5.2/tabulous/_qt/_table/_spreadsheet.py
--rw-rw-rw-   0        0        0     2676 2023-04-11 03:12:36.000000 tabulous-0.5.2/tabulous/_qt/_table/_table.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:48.908041 tabulous-0.5.2/tabulous/_qt/_table_stack/
--rw-rw-rw-   0        0        0       43 2022-08-18 11:31:02.000000 tabulous-0.5.2/tabulous/_qt/_table_stack/__init__.py
--rw-rw-rw-   0        0        0     2669 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table_stack/_eval.py
--rw-rw-rw-   0        0        0    14746 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table_stack/_finder.py
--rw-rw-rw-   0        0        0     9943 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table_stack/_overlay.py
--rw-rw-rw-   0        0        0     3450 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table_stack/_start.py
--rw-rw-rw-   0        0        0     1997 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table_stack/_tabbar.py
--rw-rw-rw-   0        0        0    23682 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table_stack/_tabwidget.py
--rw-rw-rw-   0        0        0     5477 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_table_stack/_utils.py
--rw-rw-rw-   0        0        0     1861 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_titlebar.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:49.006339 tabulous-0.5.2/tabulous/_qt/_toolbar/
--rw-rw-rw-   0        0        0       85 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_toolbar/__init__.py
--rw-rw-rw-   0        0        0     6269 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_toolbar/_corner.py
--rw-rw-rw-   0        0        0    12184 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_toolbar/_toolbar_widget.py
--rw-rw-rw-   0        0        0     2316 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_toolbar/_toolbutton.py
--rw-rw-rw-   0        0        0    11448 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_traceback.py
--rw-rw-rw-   0        0        0     3087 2022-08-19 11:58:39.000000 tabulous-0.5.2/tabulous/_qt/_tree_header.py
--rw-rw-rw-   0        0        0     4717 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_qt/_undo.py
--rw-rw-rw-   0        0        0     9933 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_range.py
--rw-rw-rw-   0        0        0    13505 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_selection_model.py
--rw-rw-rw-   0        0        0    15992 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_selection_op.py
--rw-rw-rw-   0        0        0    14756 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_sort_filter_proxy.py
--rw-rw-rw-   0        0        0    15060 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_text_formatter.py
--rw-rw-rw-   0        0        0     9454 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/_utils.py
--rw-rw-rw-   0        0        0    13695 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/color.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:49.707010 tabulous-0.5.2/tabulous/commands/
--rw-rw-rw-   0        0        0     3731 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/__init__.py
--rw-rw-rw-   0        0        0     6267 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_arange.py
--rw-rw-rw-   0        0        0    11788 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_dialogs.py
--rw-rw-rw-   0        0        0     3135 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_optimizer.py
--rw-rw-rw-   0        0        0    15035 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_plot_models.py
--rw-rw-rw-   0        0        0     4975 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_random_data.py
--rw-rw-rw-   0        0        0     2859 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_regression.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:49.837995 tabulous-0.5.2/tabulous/commands/_sklearn/
--rw-rw-rw-   0        0        0       73 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_sklearn/__init__.py
--rw-rw-rw-   0        0        0    14540 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_sklearn/_models.py
--rw-rw-rw-   0        0        0    10825 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_sklearn/_widget.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:49.990998 tabulous-0.5.2/tabulous/commands/_stats/
--rw-rw-rw-   0        0        0      136 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_stats/__init__.py
--rw-rw-rw-   0        0        0     2847 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_stats/_distribution.py
--rw-rw-rw-   0        0        0     2109 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_stats/_latex.py
--rw-rw-rw-   0        0        0    10460 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_stats/_statstest.py
--rw-rw-rw-   0        0        0     6236 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_stats/_widgets.py
--rw-rw-rw-   0        0        0      491 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_storage.py
--rw-rw-rw-   0        0        0     3670 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/_utils.py
--rw-rw-rw-   0        0        0     3054 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/analysis.py
--rw-rw-rw-   0        0        0     5246 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/column.py
--rw-rw-rw-   0        0        0     2125 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/file.py
--rw-rw-rw-   0        0        0     5650 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/plot.py
--rw-rw-rw-   0        0        0    20073 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/selection.py
--rw-rw-rw-   0        0        0     2752 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/tab.py
--rw-rw-rw-   0        0        0    10070 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/table.py
--rw-rw-rw-   0        0        0      766 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/view.py
--rw-rw-rw-   0        0        0     3260 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/commands/window.py
--rw-rw-rw-   0        0        0     2496 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/core.py
--rw-rw-rw-   0        0        0     1236 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/exceptions.py
--rw-rw-rw-   0        0        0     6494 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/post_init.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:50.082002 tabulous-0.5.2/tabulous/style/
--rw-rw-rw-   0        0        0       82 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/style/__init__.py
--rw-rw-rw-   0        0        0     2043 2023-04-14 13:55:17.000000 tabulous-0.5.2/tabulous/style/_style.py
--rw-rw-rw-   0        0        0    12052 2023-04-14 13:55:17.000000 tabulous-0.5.2/tabulous/style/_style.qss
--rw-rw-rw-   0        0        0     2621 2023-04-14 13:55:17.000000 tabulous-0.5.2/tabulous/style/defaults.json
--rw-rw-rw-   0        0        0     3928 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/threading.py
--rw-rw-rw-   0        0        0     5260 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/types.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:50.548193 tabulous-0.5.2/tabulous/widgets/
--rw-rw-rw-   0        0        0      422 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:50.848245 tabulous-0.5.2/tabulous/widgets/_component/
--rw-rw-rw-   0        0        0     1256 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_component/__init__.py
--rw-rw-rw-   0        0        0     2731 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_component/_base.py
--rw-rw-rw-   0        0        0    10644 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_component/_cell.py
--rw-rw-rw-   0        0        0    13430 2023-04-11 02:50:39.000000 tabulous-0.5.2/tabulous/widgets/_component/_column_setting.py
--rw-rw-rw-   0        0        0     9380 2023-04-14 14:01:46.000000 tabulous-0.5.2/tabulous/widgets/_component/_header.py
--rw-rw-rw-   0        0        0     1596 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_component/_keymap.py
--rw-rw-rw-   0        0        0     4846 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_component/_plot.py
--rw-rw-rw-   0        0        0    10370 2023-04-11 14:15:41.000000 tabulous-0.5.2/tabulous/widgets/_component/_proxy.py
--rw-rw-rw-   0        0        0     4838 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_component/_ranges.py
--rw-rw-rw-   0        0        0    10966 2023-04-11 02:50:39.000000 tabulous-0.5.2/tabulous/widgets/_component/_table_subset.py
--rw-rw-rw-   0        0        0     3406 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_component/_viewer.py
--rw-rw-rw-   0        0        0     1166 2022-08-27 01:33:14.000000 tabulous-0.5.2/tabulous/widgets/_doc.py
--rw-rw-rw-   0        0        0      187 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_keymap_abc.py
--rw-rw-rw-   0        0        0     2330 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_magicgui.py
--rw-rw-rw-   0        0        0    23064 2023-04-11 12:32:56.000000 tabulous-0.5.2/tabulous/widgets/_mainwindow.py
--rw-rw-rw-   0        0        0     4901 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_registry.py
--rw-rw-rw-   0        0        0      976 2022-09-13 14:24:36.000000 tabulous-0.5.2/tabulous/widgets/_sample.py
--rw-rw-rw-   0        0        0      930 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_source.py
--rw-rw-rw-   0        0        0    32982 2023-04-14 12:25:01.000000 tabulous-0.5.2/tabulous/widgets/_table.py
--rw-rw-rw-   0        0        0     7368 2023-04-09 14:02:30.000000 tabulous-0.5.2/tabulous/widgets/_tablelist.py
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:45.112949 tabulous-0.5.2/tabulous.egg-info/
--rw-rw-rw-   0        0        0     2394 2023-04-14 14:02:29.000000 tabulous-0.5.2/tabulous.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12032 2023-04-14 14:02:37.000000 tabulous-0.5.2/tabulous.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 14:02:29.000000 tabulous-0.5.2/tabulous.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-14 14:02:29.000000 tabulous-0.5.2/tabulous.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      315 2023-04-14 14:02:29.000000 tabulous-0.5.2/tabulous.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-14 14:02:29.000000 tabulous-0.5.2/tabulous.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 14:02:51.886350 tabulous-0.5.2/tests/
--rw-rw-rw-   0        0        0     4690 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_cell_eval.py
--rw-rw-rw-   0        0        0    14006 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_cell_ref_eval.py
--rw-rw-rw-   0        0        0     5450 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_colormap.py
--rw-rw-rw-   0        0        0     2844 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_column_dtype.py
--rw-rw-rw-   0        0        0      321 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_commands.py
--rw-rw-rw-   0        0        0      119 2022-10-26 15:27:47.000000 tabulous-0.5.2/tests/test_config.py
--rw-rw-rw-   0        0        0     2889 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_copy_paste.py
--rw-rw-rw-   0        0        0      651 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_core.py
--rw-rw-rw-   0        0        0     3026 2022-08-18 11:35:12.000000 tabulous-0.5.2/tests/test_dock_widgets.py
--rw-rw-rw-   0        0        0     3923 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_finder.py
--rw-rw-rw-   0        0        0     1653 2022-08-18 11:35:12.000000 tabulous-0.5.2/tests/test_groupby.py
--rw-rw-rw-   0        0        0     1894 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_keyboard_ops.py
--rw-rw-rw-   0        0        0     4788 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_keycombo.py
--rw-rw-rw-   0        0        0      918 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_magicwidget.py
--rw-rw-rw-   0        0        0     4083 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_main_window.py
--rw-rw-rw-   0        0        0     8905 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_proxy.py
--rw-rw-rw-   0        0        0     2460 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_range.py
--rw-rw-rw-   0        0        0     1810 2023-04-14 13:58:04.000000 tabulous-0.5.2/tests/test_register.py
--rw-rw-rw-   0        0        0     7769 2022-09-06 11:55:20.000000 tabulous-0.5.2/tests/test_selection_model.py
--rw-rw-rw-   0        0        0     2712 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_selection_op.py
--rw-rw-rw-   0        0        0     4559 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_selections.py
--rw-rw-rw-   0        0        0     1536 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_signal_array.py
--rw-rw-rw-   0        0        0     6667 2023-04-11 02:50:39.000000 tabulous-0.5.2/tests/test_spreadsheet.py
--rw-rw-rw-   0        0        0     9333 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_table.py
--rw-rw-rw-   0        0        0     2554 2022-08-18 11:35:12.000000 tabulous-0.5.2/tests/test_table_group.py
--rw-rw-rw-   0        0        0     2673 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_table_only_usage.py
--rw-rw-rw-   0        0        0     3554 2023-04-14 13:57:55.000000 tabulous-0.5.2/tests/test_table_subset.py
--rw-rw-rw-   0        0        0     1044 2023-04-09 14:02:30.000000 tabulous-0.5.2/tests/test_text_formatter.py
--rw-rw-rw-   0        0        0     1259 2022-08-18 11:35:12.000000 tabulous-0.5.2/tests/test_undo.py
--rw-rw-rw-   0        0        0     1455 2022-09-13 15:15:41.000000 tabulous-0.5.2/tests/test_validator.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/__init__.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/__main__.py
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_colormap.py
+-rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_dtype.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_fetch_and_install.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_io.py
+-rw-r--r--   0        0        0     6407 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_ipython.py
+-rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_map_model.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_pd_index.py
+-rw-r--r--   0        0        0    66229 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_psygnal.py
+-rw-r--r--   0        0        0    11304 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_range.py
+-rw-r--r--   0        0        0    13505 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_selection_model.py
+-rw-r--r--   0        0        0    16024 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_selection_op.py
+-rw-r--r--   0        0        0    14756 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_sort_filter_proxy.py
+-rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_text_formatter.py
+-rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_utils.py
+-rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/color.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/core.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/exceptions.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/post_init.py
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/threading.py
+-rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/types.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_keymap/__init__.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_keymap/_callback.py
+-rw-r--r--   0        0        0    22386 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_keymap/_keymap_objects.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_keymap/_keymapview.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_magicgui/__init__.py
+-rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_magicgui/_color_edit.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_magicgui/_dialog.py
+-rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_magicgui/_register.py
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_magicgui/_selection.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_magicgui/_table.py
+-rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_magicgui/_timedelta.py
+-rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_magicgui/_toggle_switch.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/__init__.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_action_registry.py
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_app.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_clickable_label.py
+-rw-r--r--   0        0        0    11575 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_console.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_dockwidget.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_filetree.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_history.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_jump.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_multitips.py
+-rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_progress.py
+-rw-r--r--   0        0        0    12824 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_proxy_button.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_qt_const.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_svg.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_titlebar.py
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_traceback.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_tree_header.py
+-rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_undo.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/barplot.svg
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/boxenplot.svg
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/boxplot.svg
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/copy.svg
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/copy_as_spreadsheet.svg
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/copy_as_table.svg
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/cut.svg
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/eval.svg
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/filter.svg
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/find_item.svg
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/groupby.svg
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/hist.svg
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/melt.svg
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/more.svg
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/new_figure.svg
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/new_spreadsheet.svg
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/open_sample.svg
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/open_spreadsheet.svg
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/open_table.svg
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/optimize.svg
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/palette.svg
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/paste.svg
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/pivot.svg
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/plot.svg
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/preferences.svg
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/random.svg
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/redo.svg
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/round.svg
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/save_table.svg
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/scatter.svg
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/settings.svg
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/sklearn_analysis.svg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/sort_table.svg
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/stats_test.svg
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/summarize_table.svg
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/swarmplot.svg
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/switch_header.svg
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/switch_layout.svg
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/tabulous.ico
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/tile.svg
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/toggle_console.svg
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/undo.svg
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/untile.svg
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/view_dual_h.svg
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/view_dual_v.svg
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/view_popup.svg
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/view_reset.svg
+-rw-r--r--   0        0        0    12285 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_icons/window_icon.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_mainwindow/__init__.py
+-rw-r--r--   0        0        0     9104 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_mainwindow/_base.py
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_mainwindow/_command_palette.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_mainwindow/_keycombo.py
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_mainwindow/_mainwidgets.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_mainwindow/_namespace.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_mainwindow/_titlebar.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_plot/__init__.py
+-rw-r--r--   0        0        0    15100 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_plot/_artist_editors.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_plot/_artist_types.py
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_plot/_mpl_canvas.py
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_plot/_widget.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_preference/__init__.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_preference/_general.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_preference/_main.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_preference/_shared.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_preference/_table_config.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_preference/_theme.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/__init__.py
+-rw-r--r--   0        0        0     7552 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_animation.py
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_display.py
+-rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_groupby.py
+-rw-r--r--   0        0        0    37792 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_spreadsheet.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_table.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/__init__.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_delegate.py
+-rw-r--r--   0        0        0    26586 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_enhanced_table.py
+-rw-r--r--   0        0        0     9934 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_header_view.py
+-rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_item_model.py
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_keycombo.py
+-rw-r--r--   0        0        0    28527 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_line_edit.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_object_holder.py
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_overlay.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_side_area.py
+-rw-r--r--   0        0        0    58943 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_table_base.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_table_group.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table/_base/_table_wrappers.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table_stack/__init__.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table_stack/_eval.py
+-rw-r--r--   0        0        0    14746 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table_stack/_finder.py
+-rw-r--r--   0        0        0     9943 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table_stack/_overlay.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table_stack/_start.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table_stack/_tabbar.py
+-rw-r--r--   0        0        0    23741 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table_stack/_tabwidget.py
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_table_stack/_utils.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_toolbar/__init__.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_toolbar/_corner.py
+-rw-r--r--   0        0        0    12266 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_toolbar/_toolbar_widget.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/_qt/_toolbar/_toolbutton.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/__init__.py
+-rw-r--r--   0        0        0     6267 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_arange.py
+-rw-r--r--   0        0        0    11788 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_dialogs.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_optimizer.py
+-rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_plot_models.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_random_data.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_regression.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_storage.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_utils.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/analysis.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/column.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/file.py
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/plot.py
+-rw-r--r--   0        0        0    19871 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/selection.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/tab.py
+-rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/table.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/view.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/window.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_sklearn/__init__.py
+-rw-r--r--   0        0        0    14540 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_sklearn/_models.py
+-rw-r--r--   0        0        0    10825 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_sklearn/_widget.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_stats/__init__.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_stats/_distribution.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_stats/_latex.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_stats/_statstest.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/commands/_stats/_widgets.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/style/__init__.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/style/_style.py
+-rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/style/_style.qss
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/style/defaults.json
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/__init__.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_doc.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_keymap_abc.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_magicgui.py
+-rw-r--r--   0        0        0    23897 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_mainwindow.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_registry.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_sample.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_source.py
+-rw-r--r--   0        0        0    35108 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_table.py
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_tablelist.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/_base.py
+-rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/_cell.py
+-rw-r--r--   0        0        0    13602 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/_column_setting.py
+-rw-r--r--   0        0        0     9948 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/_header.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/_keymap.py
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/_plot.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/_proxy.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/_ranges.py
+-rw-r--r--   0        0        0    11531 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/_table_subset.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 tabulous-0.5.3/tabulous/widgets/_component/_viewer.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 tabulous-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 tabulous-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 tabulous-0.5.3/README.md
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 tabulous-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 tabulous-0.5.3/PKG-INFO
```

### Comparing `tabulous-0.5.2/LICENSE` & `tabulous-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/PKG-INFO` & `tabulous-0.5.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,15 @@
-Metadata-Version: 2.1
-Name: tabulous
-Version: 0.5.2
-Summary: A table data viewer for Python
-Download-URL: https://github.com/hanjinliu/tabulous
-Author: Hanjin Liu
-Author-email: liuhanjin-sc@g.ecc.u-tokyo.ac.jp
-License: BSD 3-Clause
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: pyqt5
-Provides-Extra: pyqt6
-Provides-Extra: scikit-learn
-License-File: LICENSE
-
 [![Python package index download statistics](https://img.shields.io/pypi/dm/tabulous.svg)](https://pypistats.org/packages/tabulous)
 [![PyPI version](https://badge.fury.io/py/tabulous.svg)](https://badge.fury.io/py/tabulous)
 
 # tabulous
 
 A table data viewer for Python.
 
-[&rarr;当 Documentation](https://hanjinliu.github.io/tabulous/)
+[&rarr;📖 Documentation](https://hanjinliu.github.io/tabulous/)
 
 ![](https://github.com/hanjinliu/tabulous/blob/main/image/viewer_example.png)
 
 `tabulous` is highly inspired by [napari](https://github.com/napari/napari) in its design and API.
 
 ### Installation
```

### Comparing `tabulous-0.5.2/docs/_images/copy.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/copy.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/copy_as_spreadsheet.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/copy_as_spreadsheet.svg`

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 00000550: 2e30 3233 2031 3030 3520 3636 372e 3931  .023 1005 667.91
 00000560: 3722 2073 7472 6f6b 653d 2223 3030 3030  7" stroke="#0000
 00000570: 3030 2220 7374 726f 6b65 2d77 6964 7468  00" stroke-width
 00000580: 3d22 3822 2073 7472 6f6b 652d 6d69 7465  ="8" stroke-mite
 00000590: 726c 696d 6974 3d22 3822 2066 696c 6c3d  rlimit="8" fill=
 000005a0: 226e 6f6e 6522 2066 696c 6c2d 7275 6c65  "none" fill-rule
 000005b0: 3d22 6576 656e 6f64 6422 2f3e 0d0a 2020  ="evenodd"/>..  
-000005c0: 2020 3c2f 673e 0d0a 3c2f 7376 673e 0a      </g>..</svg>.
+000005c0: 2020 3c2f 673e 0d0a 3c2f 7376 673e         </g>..</svg>
```

### Comparing `tabulous-0.5.2/docs/_images/copy_as_table.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/copy_as_table.svg`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 00000430: 2e39 3332 2220 7374 726f 6b65 3d22 2330  .932" stroke="#0
 00000440: 3030 3030 3022 2073 7472 6f6b 652d 7769  00000" stroke-wi
 00000450: 6474 683d 2238 2220 7374 726f 6b65 2d6d  dth="8" stroke-m
 00000460: 6974 6572 6c69 6d69 743d 2238 2220 6669  iterlimit="8" fi
 00000470: 6c6c 3d22 6e6f 6e65 2220 6669 6c6c 2d72  ll="none" fill-r
 00000480: 756c 653d 2265 7665 6e6f 6464 222f 3e0d  ule="evenodd"/>.
 00000490: 0a20 2020 203c 2f67 3e0d 0a3c 2f73 7667  .    </g>..</svg
-000004a0: 3e0a                                     >.
+000004a0: 3e                                       >
```

### Comparing `tabulous-0.5.2/docs/_images/cut.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/cut.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/eval.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/eval.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/filter.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/filter.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/find_item.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/find_item.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/groupby.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/groupby.svg`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,8 @@
 000003f0: 2e31 3539 2033 3436 2032 3934 2e31 3837  .159 346 294.187
 00000400: 5a22 2073 7472 6f6b 653d 2223 3030 3030  Z" stroke="#0000
 00000410: 3030 2220 7374 726f 6b65 2d77 6964 7468  00" stroke-width
 00000420: 3d22 3822 2073 7472 6f6b 652d 6d69 7465  ="8" stroke-mite
 00000430: 726c 696d 6974 3d22 3822 2066 696c 6c3d  rlimit="8" fill=
 00000440: 226e 6f6e 6522 2066 696c 6c2d 7275 6c65  "none" fill-rule
 00000450: 3d22 6576 656e 6f64 6422 2f3e 0d0a 2020  ="evenodd"/>..  
-00000460: 2020 3c2f 673e 0d0a 3c2f 7376 673e 0a      </g>..</svg>.
+00000460: 2020 3c2f 673e 0d0a 3c2f 7376 673e         </g>..</svg>
```

### Comparing `tabulous-0.5.2/docs/_images/hist.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/hist.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/melt.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/melt.svg`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 00000330: 224d 3932 3620 3534 3120 3932 3620 3631  "M926 541 926 61
 00000340: 302e 3833 3622 2073 7472 6f6b 653d 2223  0.836" stroke="#
 00000350: 3030 3030 3030 2220 7374 726f 6b65 2d77  000000" stroke-w
 00000360: 6964 7468 3d22 3422 2073 7472 6f6b 652d  idth="4" stroke-
 00000370: 6d69 7465 726c 696d 6974 3d22 3822 2066  miterlimit="8" f
 00000380: 696c 6c3d 226e 6f6e 6522 2066 696c 6c2d  ill="none" fill-
 00000390: 7275 6c65 3d22 6576 656e 6f64 6422 2f3e  rule="evenodd"/>
-000003a0: 3c2f 673e 3c2f 7376 673e 0a              </g></svg>.
+000003a0: 3c2f 673e 3c2f 7376 673e                 </g></svg>
```

### Comparing `tabulous-0.5.2/docs/_images/new_figure.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/new_figure.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/open_sample.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/open_sample.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/open_spreadsheet.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/open_spreadsheet.svg`

 * *Files 4% similar despite different names*

```diff
@@ -102,8 +102,8 @@
 00000650: 2037 3737 2e37 3720 3635 312e 3530 3822   777.77 651.508"
 00000660: 2073 7472 6f6b 653d 2223 3030 3030 3030   stroke="#000000
 00000670: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
 00000680: 3822 2073 7472 6f6b 652d 6d69 7465 726c  8" stroke-miterl
 00000690: 696d 6974 3d22 3822 2066 696c 6c3d 226e  imit="8" fill="n
 000006a0: 6f6e 6522 2066 696c 6c2d 7275 6c65 3d22  one" fill-rule="
 000006b0: 6576 656e 6f64 6422 2f3e 0d0a 2020 2020  evenodd"/>..    
-000006c0: 3c2f 673e 0d0a 3c2f 7376 673e 0a         </g>..</svg>.
+000006c0: 3c2f 673e 0d0a 3c2f 7376 673e            </g>..</svg>
```

### Comparing `tabulous-0.5.2/docs/_images/open_table.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/open_table.svg`

 * *Files 0% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 00000510: 3531 2036 3536 2e31 3134 2220 7374 726f  51 656.114" stro
 00000520: 6b65 3d22 2330 3030 3030 3022 2073 7472  ke="#000000" str
 00000530: 6f6b 652d 7769 6474 683d 2238 2220 7374  oke-width="8" st
 00000540: 726f 6b65 2d6d 6974 6572 6c69 6d69 743d  roke-miterlimit=
 00000550: 2238 2220 6669 6c6c 3d22 6e6f 6e65 2220  "8" fill="none" 
 00000560: 6669 6c6c 2d72 756c 653d 2265 7665 6e6f  fill-rule="eveno
 00000570: 6464 222f 3e0d 0a20 2020 203c 2f67 3e0d  dd"/>..    </g>.
-00000580: 0a3c 2f73 7667 3e0a                      .</svg>.
+00000580: 0a3c 2f73 7667 3e                        .</svg>
```

### Comparing `tabulous-0.5.2/docs/_images/optimize.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/optimize.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/palette.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/palette.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/paste.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/paste.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/pivot.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/pivot.svg`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,8 @@
 00000410: 224d 3730 3620 3538 3020 3736 362e 3434  "M706 580 766.44
 00000420: 2036 3338 2e37 3336 2220 7374 726f 6b65   638.736" stroke
 00000430: 3d22 2330 3030 3030 3022 2073 7472 6f6b  ="#000000" strok
 00000440: 652d 7769 6474 683d 2234 2220 7374 726f  e-width="4" stro
 00000450: 6b65 2d6d 6974 6572 6c69 6d69 743d 2238  ke-miterlimit="8
 00000460: 2220 6669 6c6c 3d22 6e6f 6e65 2220 6669  " fill="none" fi
 00000470: 6c6c 2d72 756c 653d 2265 7665 6e6f 6464  ll-rule="evenodd
-00000480: 222f 3e3c 2f67 3e3c 2f73 7667 3e0a       "/></g></svg>.
+00000480: 222f 3e3c 2f67 3e3c 2f73 7667 3e         "/></g></svg>
```

### Comparing `tabulous-0.5.2/docs/_images/plot.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/plot.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/redo.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/redo.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/save_table.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/save_table.svg`

 * *Files 0% similar despite different names*

```diff
@@ -71,8 +71,8 @@
 00000460: 3938 2033 3534 2e31 3820 3339 3822 2073  98 354.18 398" s
 00000470: 7472 6f6b 653d 2223 3030 3030 3030 2220  troke="#000000" 
 00000480: 7374 726f 6b65 2d77 6964 7468 3d22 3422  stroke-width="4"
 00000490: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
 000004a0: 6974 3d22 3822 2066 696c 6c3d 226e 6f6e  it="8" fill="non
 000004b0: 6522 2066 696c 6c2d 7275 6c65 3d22 6576  e" fill-rule="ev
 000004c0: 656e 6f64 6422 2f3e 0d0a 2020 2020 3c2f  enodd"/>..    </
-000004d0: 673e 0d0a 3c2f 7376 673e 0a              g>..</svg>.
+000004d0: 673e 0d0a 3c2f 7376 673e                 g>..</svg>
```

### Comparing `tabulous-0.5.2/docs/_images/scatter.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/scatter.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/sklearn_analysis.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/sklearn_analysis.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/sort_table.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/sort_table.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/stats_test.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/stats_test.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/summarize_table.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/summarize_table.svg`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,8 @@
 000003b0: 3220 3020 3020 3130 2031 325a 2220 6669  2 0 0 10 12Z" fi
 000003c0: 6c6c 3d22 2330 3030 3030 3022 2066 696c  ll="#000000" fil
 000003d0: 6c2d 7275 6c65 3d22 6576 656e 6f64 6422  l-rule="evenodd"
 000003e0: 2074 7261 6e73 666f 726d 3d22 6d61 7472   transform="matr
 000003f0: 6978 282d 3120 312e 3232 3436 3565 2d31  ix(-1 1.22465e-1
 00000400: 3620 312e 3232 3436 3565 2d31 3620 3120  6 1.22465e-16 1 
 00000410: 3437 3620 3630 3929 222f 3e0d 0a20 2020  476 609)"/>..   
-00000420: 203c 2f67 3e0d 0a3c 2f73 7667 3e0a        </g>..</svg>.
+00000420: 203c 2f67 3e0d 0a3c 2f73 7667 3e          </g>..</svg>
```

### Comparing `tabulous-0.5.2/docs/_images/switch_header.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/switch_header.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/switch_layout.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/switch_layout.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/tile.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/tile.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/toggle_console.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/toggle_console.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/undo.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/undo.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/untile.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/untile.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/view_dual_h.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/view_dual_h.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/view_dual_v.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/view_dual_v.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/view_popup.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/view_popup.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/docs/_images/view_reset.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/view_reset.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/rst/_build/html/_images/eval.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/more.svg`

 * *Files 25% similar despite different names*

```diff
@@ -1,106 +1,78 @@
-00000000: 3c73 7667 2077 6964 7468 3d22 3931 2220  <svg width="91" 
-00000010: 6865 6967 6874 3d22 3834 220d 0a20 2020  height="84"..   
+00000000: 3c73 7667 2077 6964 7468 3d22 3336 2220  <svg width="36" 
+00000010: 6865 6967 6874 3d22 3636 220d 0a20 2020  height="66"..   
 00000020: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f77   xmlns="http://w
 00000030: 7777 2e77 332e 6f72 672f 3230 3030 2f73  ww.w3.org/2000/s
 00000040: 7667 220d 0a20 2020 2078 6d6c 6e73 3a78  vg"..    xmlns:x
 00000050: 6c69 6e6b 3d22 6874 7470 3a2f 2f77 7777  link="http://www
 00000060: 2e77 332e 6f72 672f 3139 3939 2f78 6c69  .w3.org/1999/xli
 00000070: 6e6b 2220 6f76 6572 666c 6f77 3d22 6869  nk" overflow="hi
 00000080: 6464 656e 223e 0d0a 2020 2020 3c64 6566  dden">..    <def
 00000090: 733e 0d0a 2020 2020 2020 2020 3c63 6c69  s>..        <cli
 000000a0: 7050 6174 6820 6964 3d22 636c 6970 3022  pPath id="clip0"
 000000b0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-000000c0: 7265 6374 2078 3d22 3735 3522 2079 3d22  rect x="755" y="
-000000d0: 3534 3822 2077 6964 7468 3d22 3931 2220  548" width="91" 
-000000e0: 6865 6967 6874 3d22 3834 222f 3e0d 0a20  height="84"/>.. 
-000000f0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
-00000100: 683e 0d0a 2020 2020 3c2f 6465 6673 3e0d  h>..    </defs>.
-00000110: 0a20 2020 203c 6720 636c 6970 2d70 6174  .    <g clip-pat
-00000120: 683d 2275 726c 2823 636c 6970 3029 2220  h="url(#clip0)" 
-00000130: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00000140: 6c61 7465 282d 3735 3520 2d35 3438 2922  late(-755 -548)"
-00000150: 3e0d 0a20 2020 2020 2020 203c 7061 7468  >..        <path
-00000160: 2064 3d22 4d37 3537 2e32 3620 3536 342e   d="M757.26 564.
-00000170: 3835 3120 3737 312e 3835 3120 3536 342e  851 771.851 564.
-00000180: 3835 3120 3737 312e 3835 3120 3535 302e  851 771.851 550.
-00000190: 3236 2037 3830 2e31 3439 2035 3530 2e32  26 780.149 550.2
-000001a0: 3620 3738 302e 3134 3920 3536 342e 3835  6 780.149 564.85
-000001b0: 3120 3739 342e 3734 2035 3634 2e38 3531  1 794.74 564.851
-000001c0: 2037 3934 2e37 3420 3537 332e 3134 3920   794.74 573.149 
-000001d0: 3738 302e 3134 3920 3537 332e 3134 3920  780.149 573.149 
-000001e0: 3738 302e 3134 3920 3538 372e 3734 2037  780.149 587.74 7
-000001f0: 3731 2e38 3531 2035 3837 2e37 3420 3737  71.851 587.74 77
-00000200: 312e 3835 3120 3537 332e 3134 3920 3735  1.851 573.149 75
-00000210: 372e 3236 2035 3733 2e31 3439 5a22 2073  7.26 573.149Z" s
-00000220: 7472 6f6b 653d 2223 3030 3030 3030 2220  troke="#000000" 
-00000230: 7374 726f 6b65 2d77 6964 7468 3d22 312e  stroke-width="1.
-00000240: 3333 3333 3322 2073 7472 6f6b 652d 6d69  33333" stroke-mi
-00000250: 7465 726c 696d 6974 3d22 3822 2066 696c  terlimit="8" fil
-00000260: 6c3d 2223 3030 3030 3030 2220 6669 6c6c  l="#000000" fill
-00000270: 2d72 756c 653d 2265 7665 6e6f 6464 222f  -rule="evenodd"/
-00000280: 3e0d 0a20 2020 2020 2020 203c 7265 6374  >..        <rect
-00000290: 2078 3d22 3830 372e 3339 3322 2079 3d22   x="807.393" y="
-000002a0: 3536 352e 3135 3922 2077 6964 7468 3d22  565.159" width="
-000002b0: 3338 2e32 3134 3722 2068 6569 6768 743d  38.2147" height=
-000002c0: 2237 2e36 3832 3133 2220 7374 726f 6b65  "7.68213" stroke
-000002d0: 3d22 2330 3030 3030 3022 2073 7472 6f6b  ="#000000" strok
-000002e0: 652d 7769 6474 683d 2231 2e33 3333 3333  e-width="1.33333
-000002f0: 2220 6669 6c6c 3d22 2330 3030 3030 3022  " fill="#000000"
-00000300: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
-00000310: 6974 3d22 3822 2f3e 0d0a 2020 2020 2020  it="8"/>..      
-00000320: 2020 3c70 6174 6820 643d 224d 3735 392e    <path d="M759.
-00000330: 3932 3420 3630 342e 3537 3420 3736 352e  924 604.574 765.
-00000340: 3537 3420 3539 382e 3932 3420 3737 3620  574 598.924 776 
-00000350: 3630 392e 3335 2037 3836 2e34 3236 2035  609.35 786.426 5
-00000360: 3938 2e39 3234 2037 3932 2e30 3736 2036  98.924 792.076 6
-00000370: 3034 2e35 3734 2037 3831 2e36 3520 3631  04.574 781.65 61
-00000380: 3520 3739 322e 3037 3620 3632 352e 3432  5 792.076 625.42
-00000390: 3620 3738 362e 3432 3620 3633 312e 3037  6 786.426 631.07
-000003a0: 3620 3737 3620 3632 302e 3635 2037 3635  6 776 620.65 765
-000003b0: 2e35 3734 2036 3331 2e30 3736 2037 3539  .574 631.076 759
-000003c0: 2e39 3234 2036 3235 2e34 3236 2037 3730  .924 625.426 770
-000003d0: 2e33 3520 3631 355a 2220 7374 726f 6b65  .35 615Z" stroke
-000003e0: 3d22 2330 3030 3030 3022 2073 7472 6f6b  ="#000000" strok
-000003f0: 652d 7769 6474 683d 2231 2e33 3333 3333  e-width="1.33333
-00000400: 2220 7374 726f 6b65 2d6d 6974 6572 6c69  " stroke-miterli
-00000410: 6d69 743d 2238 2220 6669 6c6c 3d22 2330  mit="8" fill="#0
-00000420: 3030 3030 3022 2066 696c 6c2d 7275 6c65  00000" fill-rule
-00000430: 3d22 6576 656e 6f64 6422 2f3e 0d0a 2020  ="evenodd"/>..  
-00000440: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-00000450: 3832 362e 3520 3539 362e 3830 3843 3832  826.5 596.808C82
-00000460: 392e 3138 3420 3539 362e 3830 3820 3833  9.184 596.808 83
-00000470: 312e 3335 3920 3539 382e 3938 3420 3833  1.359 598.984 83
-00000480: 312e 3335 3920 3630 312e 3636 3720 3833  1.359 601.667 83
-00000490: 312e 3335 3920 3630 342e 3335 3120 3832  1.359 604.351 82
-000004a0: 392e 3138 3420 3630 362e 3532 3620 3832  9.184 606.526 82
-000004b0: 362e 3520 3630 362e 3532 3620 3832 332e  6.5 606.526 823.
-000004c0: 3831 3720 3630 362e 3532 3620 3832 312e  817 606.526 821.
-000004d0: 3634 3120 3630 342e 3335 3120 3832 312e  641 604.351 821.
-000004e0: 3634 3120 3630 312e 3636 3720 3832 312e  641 601.667 821.
-000004f0: 3634 3120 3539 382e 3938 3420 3832 332e  641 598.984 823.
-00000500: 3831 3720 3539 362e 3830 3820 3832 362e  817 596.808 826.
-00000510: 3520 3539 362e 3830 385a 4d38 3236 2e35  5 596.808ZM826.5
-00000520: 2036 3330 2e31 3932 4338 3233 2e38 3137   630.192C823.817
-00000530: 2036 3330 2e31 3932 2038 3231 2e36 3431   630.192 821.641
-00000540: 2036 3238 2e30 3136 2038 3231 2e36 3431   628.016 821.641
-00000550: 2036 3235 2e33 3333 2038 3231 2e36 3431   625.333 821.641
-00000560: 2036 3232 2e36 3439 2038 3233 2e38 3137   622.649 823.817
-00000570: 2036 3230 2e34 3734 2038 3236 2e35 2036   620.474 826.5 6
-00000580: 3230 2e34 3734 2038 3239 2e31 3834 2036  20.474 829.184 6
-00000590: 3230 2e34 3734 2038 3331 2e33 3539 2036  20.474 831.359 6
-000005a0: 3232 2e36 3439 2038 3331 2e33 3539 2036  22.649 831.359 6
-000005b0: 3235 2e33 3333 2038 3331 2e33 3539 2036  25.333 831.359 6
-000005c0: 3238 2e30 3136 2038 3239 2e31 3834 2036  28.016 829.184 6
-000005d0: 3330 2e31 3932 2038 3236 2e35 2036 3330  30.192 826.5 630
-000005e0: 2e31 3932 5a4d 3830 372e 3339 3320 3630  .192ZM807.393 60
-000005f0: 392e 3538 3420 3834 352e 3630 3720 3630  9.584 845.607 60
-00000600: 392e 3538 3420 3834 352e 3630 3720 3631  9.584 845.607 61
-00000610: 372e 3431 3620 3830 372e 3339 3320 3631  7.416 807.393 61
-00000620: 372e 3431 365a 2220 7374 726f 6b65 3d22  7.416Z" stroke="
-00000630: 2330 3030 3030 3022 2073 7472 6f6b 652d  #000000" stroke-
-00000640: 7769 6474 683d 2231 2e33 3333 3333 2220  width="1.33333" 
-00000650: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
-00000660: 743d 2238 2220 6669 6c6c 3d22 2330 3030  t="8" fill="#000
-00000670: 3030 3022 2066 696c 6c2d 7275 6c65 3d22  000" fill-rule="
-00000680: 6576 656e 6f64 6422 2f3e 0d0a 2020 2020  evenodd"/>..    
-00000690: 3c2f 673e 0d0a 3c2f 7376 673e 0d0a       </g>..</svg>..
+000000c0: 7265 6374 2078 3d22 3130 3733 2220 793d  rect x="1073" y=
+000000d0: 2235 3039 2220 7769 6474 683d 2233 3622  "509" width="36"
+000000e0: 2068 6569 6768 743d 2236 3622 2f3e 0d0a   height="66"/>..
+000000f0: 2020 2020 2020 2020 3c2f 636c 6970 5061          </clipPa
+00000100: 7468 3e0d 0a20 2020 203c 2f64 6566 733e  th>..    </defs>
+00000110: 0d0a 2020 2020 3c67 2063 6c69 702d 7061  ..    <g clip-pa
+00000120: 7468 3d22 7572 6c28 2363 6c69 7030 2922  th="url(#clip0)"
+00000130: 2074 7261 6e73 666f 726d 3d22 7472 616e   transform="tran
+00000140: 736c 6174 6528 2d31 3037 3320 2d35 3039  slate(-1073 -509
+00000150: 2922 3e0d 0a20 2020 2020 2020 203c 7061  )">..        <pa
+00000160: 7468 2064 3d22 4d31 3037 342e 3938 2035  th d="M1074.98 5
+00000170: 3539 2e36 3735 4331 3037 332e 3438 2035  59.675C1073.48 5
+00000180: 3538 2e31 3735 2031 3037 332e 3438 2035  58.175 1073.48 5
+00000190: 3535 2e37 3433 2031 3037 342e 3938 2035  55.743 1074.98 5
+000001a0: 3534 2e32 3433 4c31 3037 342e 3938 2035  54.243L1074.98 5
+000001b0: 3534 2e32 3433 4331 3037 362e 3438 2035  54.243C1076.48 5
+000001c0: 3532 2e37 3433 2031 3037 382e 3931 2035  52.743 1078.91 5
+000001d0: 3532 2e37 3433 2031 3038 302e 3431 2035  52.743 1080.41 5
+000001e0: 3534 2e32 3433 4c31 3039 322e 3838 2035  54.243L1092.88 5
+000001f0: 3636 2e37 3135 4331 3039 342e 3338 2035  66.715C1094.38 5
+00000200: 3638 2e32 3135 2031 3039 342e 3338 2035  68.215 1094.38 5
+00000210: 3730 2e36 3437 2031 3039 322e 3838 2035  70.647 1092.88 5
+00000220: 3732 2e31 3437 4c31 3039 322e 3838 2035  72.147L1092.88 5
+00000230: 3732 2e31 3437 4331 3039 312e 3338 2035  72.147C1091.38 5
+00000240: 3733 2e36 3437 2031 3038 382e 3935 2035  73.647 1088.95 5
+00000250: 3733 2e36 3437 2031 3038 372e 3435 2035  73.647 1087.45 5
+00000260: 3732 2e31 3437 5a22 2073 7472 6f6b 653d  72.147Z" stroke=
+00000270: 2223 3030 3030 3030 2220 7374 726f 6b65  "#000000" stroke
+00000280: 2d77 6964 7468 3d22 312e 3333 3333 3322  -width="1.33333"
+00000290: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+000002a0: 6974 3d22 3822 2066 696c 6c3d 2223 3030  it="8" fill="#00
+000002b0: 3030 3030 2220 6669 6c6c 2d72 756c 653d  0000" fill-rule=
+000002c0: 2265 7665 6e6f 6464 222f 3e0d 0a20 2020  "evenodd"/>..   
+000002d0: 2020 2020 203c 7061 7468 2064 3d22 4d31       <path d="M1
+000002e0: 3130 302e 3632 2035 3534 2e32 3034 4331  100.62 554.204C1
+000002f0: 3130 322e 3132 2035 3532 2e37 3034 2031  102.12 552.704 1
+00000300: 3130 342e 3536 2035 3532 2e37 3034 2031  104.56 552.704 1
+00000310: 3130 362e 3036 2035 3534 2e32 3034 4c31  106.06 554.204L1
+00000320: 3130 362e 3036 2035 3534 2e32 3034 4331  106.06 554.204C1
+00000330: 3130 372e 3536 2035 3535 2e37 3034 2031  107.56 555.704 1
+00000340: 3130 372e 3536 2035 3538 2e31 3336 2031  107.56 558.136 1
+00000350: 3130 362e 3036 2035 3539 2e36 3336 4c31  106.06 559.636L1
+00000360: 3039 332e 3538 2035 3732 2e31 3038 4331  093.58 572.108C1
+00000370: 3039 322e 3038 2035 3733 2e36 3038 2031  092.08 573.608 1
+00000380: 3038 392e 3635 2035 3733 2e36 3038 2031  089.65 573.608 1
+00000390: 3038 382e 3135 2035 3732 2e31 3038 4c31  088.15 572.108L1
+000003a0: 3038 382e 3135 2035 3732 2e31 3038 4331  088.15 572.108C1
+000003b0: 3038 362e 3635 2035 3730 2e36 3038 2031  086.65 570.608 1
+000003c0: 3038 362e 3635 2035 3638 2e31 3736 2031  086.65 568.176 1
+000003d0: 3038 382e 3135 2035 3636 2e36 3735 5a22  088.15 566.675Z"
+000003e0: 2073 7472 6f6b 653d 2223 3030 3030 3030   stroke="#000000
+000003f0: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
+00000400: 312e 3333 3333 3322 2073 7472 6f6b 652d  1.33333" stroke-
+00000410: 6d69 7465 726c 696d 6974 3d22 3822 2066  miterlimit="8" f
+00000420: 696c 6c3d 2223 3030 3030 3030 2220 6669  ill="#000000" fi
+00000430: 6c6c 2d72 756c 653d 2265 7665 6e6f 6464  ll-rule="evenodd
+00000440: 222f 3e0d 0a20 2020 2020 2020 203c 7061  "/>..        <pa
+00000450: 7468 2064 3d22 4d31 3038 342e 3520 3530  th d="M1084.5 50
+00000460: 392e 3520 3130 3937 2e34 3220 3530 392e  9.5 1097.42 509.
+00000470: 3522 2073 7472 6f6b 653d 2223 3030 3030  5" stroke="#0000
+00000480: 3030 2220 7374 726f 6b65 2d77 6964 7468  00" stroke-width
+00000490: 3d22 3022 2073 7472 6f6b 652d 6d69 7465  ="0" stroke-mite
+000004a0: 726c 696d 6974 3d22 3822 2066 696c 6c3d  rlimit="8" fill=
+000004b0: 226e 6f6e 6522 2066 696c 6c2d 7275 6c65  "none" fill-rule
+000004c0: 3d22 6576 656e 6f64 6422 2f3e 0d0a 2020  ="evenodd"/>..  
+000004d0: 2020 3c2f 673e 0d0a 3c2f 7376 673e 0d0a    </g>..</svg>..
```

### Comparing `tabulous-0.5.2/rst/_build/html/_images/hist.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/boxenplot.svg`

 * *Files 10% similar despite different names*

```diff
@@ -6,80 +6,104 @@
 00000050: 6c69 6e6b 3d22 6874 7470 3a2f 2f77 7777  link="http://www
 00000060: 2e77 332e 6f72 672f 3139 3939 2f78 6c69  .w3.org/1999/xli
 00000070: 6e6b 2220 6f76 6572 666c 6f77 3d22 6869  nk" overflow="hi
 00000080: 6464 656e 223e 0d0a 2020 2020 3c64 6566  dden">..    <def
 00000090: 733e 0d0a 2020 2020 2020 2020 3c63 6c69  s>..        <cli
 000000a0: 7050 6174 6820 6964 3d22 636c 6970 3022  pPath id="clip0"
 000000b0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-000000c0: 7265 6374 2078 3d22 3436 2220 793d 2235  rect x="46" y="5
-000000d0: 3839 2220 7769 6474 683d 2238 3822 2068  89" width="88" h
-000000e0: 6569 6768 743d 2238 3322 2f3e 0d0a 2020  eight="83"/>..  
-000000f0: 2020 2020 2020 3c2f 636c 6970 5061 7468        </clipPath
-00000100: 3e0d 0a20 2020 203c 2f64 6566 733e 0d0a  >..    </defs>..
-00000110: 2020 2020 3c67 2063 6c69 702d 7061 7468      <g clip-path
-00000120: 3d22 7572 6c28 2363 6c69 7030 2922 2074  ="url(#clip0)" t
-00000130: 7261 6e73 666f 726d 3d22 7472 616e 736c  ransform="transl
-00000140: 6174 6528 2d34 3620 2d35 3839 2922 3e0d  ate(-46 -589)">.
-00000150: 0a20 2020 2020 2020 203c 7061 7468 2064  .        <path d
-00000160: 3d22 4d35 3420 3539 3020 3534 2e30 3030  ="M54 590 54.000
-00000170: 3120 3636 372e 3630 3922 2073 7472 6f6b  1 667.609" strok
-00000180: 653d 2223 3030 3030 3030 2220 7374 726f  e="#000000" stro
-00000190: 6b65 2d77 6964 7468 3d22 3822 2073 7472  ke-width="8" str
-000001a0: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
-000001b0: 3822 2066 696c 6c3d 226e 6f6e 6522 2066  8" fill="none" f
-000001c0: 696c 6c2d 7275 6c65 3d22 6576 656e 6f64  ill-rule="evenod
-000001d0: 6422 2f3e 0d0a 2020 2020 2020 2020 3c70  d"/>..        <p
-000001e0: 6174 6820 643d 224d 3020 3020 3832 2e36  ath d="M0 0 82.6
-000001f0: 3034 3420 302e 3030 3031 3034 3938 3722  044 0.000104987"
-00000200: 2073 7472 6f6b 653d 2223 3030 3030 3030   stroke="#000000
-00000210: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
-00000220: 3822 2073 7472 6f6b 652d 6d69 7465 726c  8" stroke-miterl
-00000230: 696d 6974 3d22 3822 2066 696c 6c3d 226e  imit="8" fill="n
-00000240: 6f6e 6522 2066 696c 6c2d 7275 6c65 3d22  one" fill-rule="
-00000250: 6576 656e 6f64 6422 2074 7261 6e73 666f  evenodd" transfo
-00000260: 726d 3d22 6d61 7472 6978 282d 3120 3020  rm="matrix(-1 0 
-00000270: 3020 3120 3133 332e 3630 3420 3636 3329  0 1 133.604 663)
-00000280: 222f 3e0d 0a20 2020 2020 2020 203c 7265  "/>..        <re
-00000290: 6374 2078 3d22 3539 2e35 3030 3122 2079  ct x="59.5001" y
-000002a0: 3d22 3634 302e 3522 2077 6964 7468 3d22  ="640.5" width="
-000002b0: 3134 2220 6865 6967 6874 3d22 3230 2220  14" height="20" 
-000002c0: 7374 726f 6b65 3d22 2330 3030 3030 3022  stroke="#000000"
-000002d0: 2073 7472 6f6b 652d 7769 6474 683d 2231   stroke-width="1
-000002e0: 2e33 3333 3333 2220 6669 6c6c 3d22 2330  .33333" fill="#0
-000002f0: 3030 3030 3022 2073 7472 6f6b 652d 6d69  00000" stroke-mi
-00000300: 7465 726c 696d 6974 3d22 3822 2f3e 0d0a  terlimit="8"/>..
-00000310: 2020 2020 2020 2020 3c72 6563 7420 783d          <rect x=
-00000320: 2237 342e 3530 3031 2220 793d 2236 3134  "74.5001" y="614
-00000330: 2e35 2220 7769 6474 683d 2231 3422 2068  .5" width="14" h
-00000340: 6569 6768 743d 2234 3622 2073 7472 6f6b  eight="46" strok
-00000350: 653d 2223 3030 3030 3030 2220 7374 726f  e="#000000" stro
-00000360: 6b65 2d77 6964 7468 3d22 312e 3333 3333  ke-width="1.3333
-00000370: 3322 2066 696c 6c3d 2223 3030 3030 3030  3" fill="#000000
-00000380: 2220 7374 726f 6b65 2d6d 6974 6572 6c69  " stroke-miterli
-00000390: 6d69 743d 2238 222f 3e0d 0a20 2020 2020  mit="8"/>..     
-000003a0: 2020 203c 7265 6374 2078 3d22 3839 2e35     <rect x="89.5
-000003b0: 3030 3122 2079 3d22 3630 312e 3522 2077  001" y="601.5" w
-000003c0: 6964 7468 3d22 3134 2220 6865 6967 6874  idth="14" height
-000003d0: 3d22 3539 2220 7374 726f 6b65 3d22 2330  ="59" stroke="#0
-000003e0: 3030 3030 3022 2073 7472 6f6b 652d 7769  00000" stroke-wi
-000003f0: 6474 683d 2231 2e33 3333 3333 2220 6669  dth="1.33333" fi
-00000400: 6c6c 3d22 2330 3030 3030 3022 2073 7472  ll="#000000" str
-00000410: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
-00000420: 3822 2f3e 0d0a 2020 2020 2020 2020 3c72  8"/>..        <r
-00000430: 6563 7420 783d 2231 3034 2e35 2220 793d  ect x="104.5" y=
-00000440: 2236 3037 2e35 2220 7769 6474 683d 2231  "607.5" width="1
-00000450: 3522 2068 6569 6768 743d 2235 3322 2073  5" height="53" s
-00000460: 7472 6f6b 653d 2223 3030 3030 3030 2220  troke="#000000" 
-00000470: 7374 726f 6b65 2d77 6964 7468 3d22 312e  stroke-width="1.
-00000480: 3333 3333 3322 2066 696c 6c3d 2223 3030  33333" fill="#00
-00000490: 3030 3030 2220 7374 726f 6b65 2d6d 6974  0000" stroke-mit
-000004a0: 6572 6c69 6d69 743d 2238 222f 3e0d 0a20  erlimit="8"/>.. 
-000004b0: 2020 2020 2020 203c 7265 6374 2078 3d22         <rect x="
-000004c0: 3131 392e 3522 2079 3d22 3633 322e 3522  119.5" y="632.5"
-000004d0: 2077 6964 7468 3d22 3134 2220 6865 6967   width="14" heig
-000004e0: 6874 3d22 3239 2220 7374 726f 6b65 3d22  ht="29" stroke="
-000004f0: 2330 3030 3030 3022 2073 7472 6f6b 652d  #000000" stroke-
-00000500: 7769 6474 683d 2231 2e33 3333 3333 2220  width="1.33333" 
-00000510: 6669 6c6c 3d22 2330 3030 3030 3022 2073  fill="#000000" s
-00000520: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
-00000530: 3d22 3822 2f3e 0d0a 2020 2020 3c2f 673e  ="8"/>..    </g>
-00000540: 0d0a 3c2f 7376 673e 0d0a                 ..</svg>..
+000000c0: 7265 6374 2078 3d22 3337 3122 2079 3d22  rect x="371" y="
+000000d0: 3336 3322 2077 6964 7468 3d22 3838 2220  363" width="88" 
+000000e0: 6865 6967 6874 3d22 3833 222f 3e0d 0a20  height="83"/>.. 
+000000f0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
+00000100: 683e 0d0a 2020 2020 3c2f 6465 6673 3e0d  h>..    </defs>.
+00000110: 0a20 2020 203c 6720 636c 6970 2d70 6174  .    <g clip-pat
+00000120: 683d 2275 726c 2823 636c 6970 3029 2220  h="url(#clip0)" 
+00000130: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
+00000140: 6c61 7465 282d 3337 3120 2d33 3633 2922  late(-371 -363)"
+00000150: 3e0d 0a20 2020 2020 2020 203c 7061 7468  >..        <path
+00000160: 2064 3d22 4d33 3739 2033 3634 2033 3739   d="M379 364 379
+00000170: 2034 3431 2e36 3039 2220 7374 726f 6b65   441.609" stroke
+00000180: 3d22 2330 3030 3030 3022 2073 7472 6f6b  ="#000000" strok
+00000190: 652d 7769 6474 683d 2238 2220 7374 726f  e-width="8" stro
+000001a0: 6b65 2d6d 6974 6572 6c69 6d69 743d 2238  ke-miterlimit="8
+000001b0: 2220 6669 6c6c 3d22 6e6f 6e65 2220 6669  " fill="none" fi
+000001c0: 6c6c 2d72 756c 653d 2265 7665 6e6f 6464  ll-rule="evenodd
+000001d0: 222f 3e0d 0a20 2020 2020 2020 203c 7061  "/>..        <pa
+000001e0: 7468 2064 3d22 4d30 2030 2038 322e 3630  th d="M0 0 82.60
+000001f0: 3434 2030 2e30 3030 3130 3439 3837 2220  44 0.000104987" 
+00000200: 7374 726f 6b65 3d22 2330 3030 3030 3022  stroke="#000000"
+00000210: 2073 7472 6f6b 652d 7769 6474 683d 2238   stroke-width="8
+00000220: 2220 7374 726f 6b65 2d6d 6974 6572 6c69  " stroke-miterli
+00000230: 6d69 743d 2238 2220 6669 6c6c 3d22 6e6f  mit="8" fill="no
+00000240: 6e65 2220 6669 6c6c 2d72 756c 653d 2265  ne" fill-rule="e
+00000250: 7665 6e6f 6464 2220 7472 616e 7366 6f72  venodd" transfor
+00000260: 6d3d 226d 6174 7269 7828 2d31 2030 2030  m="matrix(-1 0 0
+00000270: 2031 2034 3538 2e36 3034 2034 3338 2922   1 458.604 438)"
+00000280: 2f3e 0d0a 2020 2020 2020 2020 3c72 6563  />..        <rec
+00000290: 7420 783d 2233 3838 2e35 2220 793d 2233  t x="388.5" y="3
+000002a0: 3930 2e35 2220 7769 6474 683d 2232 3822  90.5" width="28"
+000002b0: 2068 6569 6768 743d 2231 3122 2073 7472   height="11" str
+000002c0: 6f6b 653d 2223 3030 3030 3030 2220 7374  oke="#000000" st
+000002d0: 726f 6b65 2d77 6964 7468 3d22 312e 3333  roke-width="1.33
+000002e0: 3333 3322 2066 696c 6c3d 2223 3030 3030  333" fill="#0000
+000002f0: 3030 2220 7374 726f 6b65 2d6d 6974 6572  00" stroke-miter
+00000300: 6c69 6d69 743d 2238 222f 3e0d 0a20 2020  limit="8"/>..   
+00000310: 2020 2020 203c 7265 6374 2078 3d22 3432       <rect x="42
+00000320: 322e 3522 2079 3d22 3431 312e 3522 2077  2.5" y="411.5" w
+00000330: 6964 7468 3d22 3238 2220 6865 6967 6874  idth="28" height
+00000340: 3d22 3922 2073 7472 6f6b 653d 2223 3030  ="9" stroke="#00
+00000350: 3030 3030 2220 7374 726f 6b65 2d77 6964  0000" stroke-wid
+00000360: 7468 3d22 312e 3333 3333 3322 2066 696c  th="1.33333" fil
+00000370: 6c3d 2223 3030 3030 3030 2220 7374 726f  l="#000000" stro
+00000380: 6b65 2d6d 6974 6572 6c69 6d69 743d 2238  ke-miterlimit="8
+00000390: 222f 3e0d 0a20 2020 2020 2020 203c 7061  "/>..        <pa
+000003a0: 7468 2064 3d22 4d34 3032 2033 3639 2034  th d="M402 369 4
+000003b0: 3032 2034 3136 2e31 3338 2220 7374 726f  02 416.138" stro
+000003c0: 6b65 3d22 2330 3030 3030 3022 2073 7472  ke="#000000" str
+000003d0: 6f6b 652d 7769 6474 683d 2234 2220 7374  oke-width="4" st
+000003e0: 726f 6b65 2d6d 6974 6572 6c69 6d69 743d  roke-miterlimit=
+000003f0: 2238 2220 6669 6c6c 3d22 6e6f 6e65 2220  "8" fill="none" 
+00000400: 6669 6c6c 2d72 756c 653d 2265 7665 6e6f  fill-rule="eveno
+00000410: 6464 222f 3e0d 0a20 2020 2020 2020 203c  dd"/>..        <
+00000420: 7061 7468 2064 3d22 4d34 3337 2033 3938  path d="M437 398
+00000430: 2034 3337 2034 3330 2e34 3739 2220 7374   437 430.479" st
+00000440: 726f 6b65 3d22 2330 3030 3030 3022 2073  roke="#000000" s
+00000450: 7472 6f6b 652d 7769 6474 683d 2234 2220  troke-width="4" 
+00000460: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+00000470: 743d 2238 2220 6669 6c6c 3d22 6e6f 6e65  t="8" fill="none
+00000480: 2220 6669 6c6c 2d72 756c 653d 2265 7665  " fill-rule="eve
+00000490: 6e6f 6464 222f 3e0d 0a20 2020 2020 2020  nodd"/>..       
+000004a0: 203c 7265 6374 2078 3d22 3339 342e 3522   <rect x="394.5"
+000004b0: 2079 3d22 3338 312e 3522 2077 6964 7468   y="381.5" width
+000004c0: 3d22 3136 2220 6865 6967 6874 3d22 3822  ="16" height="8"
+000004d0: 2073 7472 6f6b 653d 2223 3030 3030 3030   stroke="#000000
+000004e0: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
+000004f0: 312e 3333 3333 3322 2066 696c 6c3d 2223  1.33333" fill="#
+00000500: 3030 3030 3030 2220 7374 726f 6b65 2d6d  000000" stroke-m
+00000510: 6974 6572 6c69 6d69 743d 2238 222f 3e0d  iterlimit="8"/>.
+00000520: 0a20 2020 2020 2020 203c 7265 6374 2078  .        <rect x
+00000530: 3d22 3339 342e 3522 2079 3d22 3430 312e  ="394.5" y="401.
+00000540: 3522 2077 6964 7468 3d22 3136 2220 6865  5" width="16" he
+00000550: 6967 6874 3d22 3522 2073 7472 6f6b 653d  ight="5" stroke=
+00000560: 2223 3030 3030 3030 2220 7374 726f 6b65  "#000000" stroke
+00000570: 2d77 6964 7468 3d22 312e 3333 3333 3322  -width="1.33333"
+00000580: 2066 696c 6c3d 2223 3030 3030 3030 2220   fill="#000000" 
+00000590: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+000005a0: 743d 2238 222f 3e0d 0a20 2020 2020 2020  t="8"/>..       
+000005b0: 203c 7265 6374 2078 3d22 3432 382e 3522   <rect x="428.5"
+000005c0: 2079 3d22 3430 362e 3522 2077 6964 7468   y="406.5" width
+000005d0: 3d22 3137 2220 6865 6967 6874 3d22 3622  ="17" height="6"
+000005e0: 2073 7472 6f6b 653d 2223 3030 3030 3030   stroke="#000000
+000005f0: 2220 7374 726f 6b65 2d77 6964 7468 3d22  " stroke-width="
+00000600: 312e 3333 3333 3322 2066 696c 6c3d 2223  1.33333" fill="#
+00000610: 3030 3030 3030 2220 7374 726f 6b65 2d6d  000000" stroke-m
+00000620: 6974 6572 6c69 6d69 743d 2238 222f 3e0d  iterlimit="8"/>.
+00000630: 0a20 2020 2020 2020 203c 7265 6374 2078  .        <rect x
+00000640: 3d22 3432 392e 3522 2079 3d22 3431 392e  ="429.5" y="419.
+00000650: 3522 2077 6964 7468 3d22 3136 2220 6865  5" width="16" he
+00000660: 6967 6874 3d22 3522 2073 7472 6f6b 653d  ight="5" stroke=
+00000670: 2223 3030 3030 3030 2220 7374 726f 6b65  "#000000" stroke
+00000680: 2d77 6964 7468 3d22 312e 3333 3333 3322  -width="1.33333"
+00000690: 2066 696c 6c3d 2223 3030 3030 3030 2220   fill="#000000" 
+000006a0: 7374 726f 6b65 2d6d 6974 6572 6c69 6d69  stroke-miterlimi
+000006b0: 743d 2238 222f 3e0d 0a20 2020 203c 2f67  t="8"/>..    </g
+000006c0: 3e0d 0a3c 2f73 7667 3e0d 0a              >..</svg>..
```

### Comparing `tabulous-0.5.2/rst/_build/html/_images/pivot.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/round.svg`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,81 @@
-00000000: 3c73 7667 2077 6964 7468 3d22 3935 2220  <svg width="95" 
-00000010: 6865 6967 6874 3d22 3935 2220 786d 6c6e  height="95" xmln
+00000000: 3c73 7667 2077 6964 7468 3d22 3539 2220  <svg width="59" 
+00000010: 6865 6967 6874 3d22 3437 2220 786d 6c6e  height="47" xmln
 00000020: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
 00000030: 2e6f 7267 2f32 3030 302f 7376 6722 2078  .org/2000/svg" x
 00000040: 6d6c 6e73 3a78 6c69 6e6b 3d22 6874 7470  mlns:xlink="http
 00000050: 3a2f 2f77 7777 2e77 332e 6f72 672f 3139  ://www.w3.org/19
 00000060: 3939 2f78 6c69 6e6b 2220 6f76 6572 666c  99/xlink" overfl
 00000070: 6f77 3d22 6869 6464 656e 223e 3c64 6566  ow="hidden"><def
 00000080: 733e 3c63 6c69 7050 6174 6820 6964 3d22  s><clipPath id="
 00000090: 636c 6970 3022 3e3c 7265 6374 2078 3d22  clip0"><rect x="
-000000a0: 3638 3922 2079 3d22 3536 3222 2077 6964  689" y="562" wid
-000000b0: 7468 3d22 3935 2220 6865 6967 6874 3d22  th="95" height="
-000000c0: 3935 222f 3e3c 2f63 6c69 7050 6174 683e  95"/></clipPath>
+000000a0: 3732 3122 2079 3d22 3531 3722 2077 6964  721" y="517" wid
+000000b0: 7468 3d22 3539 2220 6865 6967 6874 3d22  th="59" height="
+000000c0: 3437 222f 3e3c 2f63 6c69 7050 6174 683e  47"/></clipPath>
 000000d0: 3c2f 6465 6673 3e3c 6720 636c 6970 2d70  </defs><g clip-p
 000000e0: 6174 683d 2275 726c 2823 636c 6970 3029  ath="url(#clip0)
 000000f0: 2220 7472 616e 7366 6f72 6d3d 2274 7261  " transform="tra
-00000100: 6e73 6c61 7465 282d 3638 3920 2d35 3632  nslate(-689 -562
-00000110: 2922 3e3c 7061 7468 2064 3d22 4d37 3031  )"><path d="M701
-00000120: 2035 3836 2e35 4337 3031 2035 3830 2e31   586.5C701 580.1
-00000130: 3439 2037 3036 2e31 3439 2035 3735 2037  49 706.149 575 7
-00000140: 3132 2e35 2035 3735 4c37 3538 2e35 2035  12.5 575L758.5 5
-00000150: 3735 4337 3634 2e38 3531 2035 3735 2037  75C764.851 575 7
-00000160: 3730 2035 3830 2e31 3439 2037 3730 2035  70 580.149 770 5
-00000170: 3836 2e35 4c37 3730 2036 3332 2e35 4337  86.5L770 632.5C7
-00000180: 3730 2036 3338 2e38 3531 2037 3634 2e38  70 638.851 764.8
-00000190: 3531 2036 3434 2037 3538 2e35 2036 3434  51 644 758.5 644
-000001a0: 4c37 3132 2e35 2036 3434 4337 3036 2e31  L712.5 644C706.1
-000001b0: 3439 2036 3434 2037 3031 2036 3338 2e38  49 644 701 638.8
-000001c0: 3531 2037 3031 2036 3332 2e35 5a22 2073  51 701 632.5Z" s
-000001d0: 7472 6f6b 653d 2223 3030 3030 3030 2220  troke="#000000" 
-000001e0: 7374 726f 6b65 2d77 6964 7468 3d22 3822  stroke-width="8"
-000001f0: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
-00000200: 6974 3d22 3822 2066 696c 6c3d 226e 6f6e  it="8" fill="non
-00000210: 6522 2066 696c 6c2d 7275 6c65 3d22 6576  e" fill-rule="ev
-00000220: 656e 6f64 6422 2f3e 3c70 6174 6820 643d  enodd"/><path d=
-00000230: 224d 3731 3920 3538 3220 3736 382e 3034  "M719 582 768.04
-00000240: 3320 3538 3222 2073 7472 6f6b 653d 2223  3 582" stroke="#
-00000250: 3030 3030 3030 2220 7374 726f 6b65 2d77  000000" stroke-w
-00000260: 6964 7468 3d22 3822 2073 7472 6f6b 652d  idth="8" stroke-
-00000270: 6d69 7465 726c 696d 6974 3d22 3822 2066  miterlimit="8" f
-00000280: 696c 6c3d 226e 6f6e 6522 2066 696c 6c2d  ill="none" fill-
-00000290: 7275 6c65 3d22 6576 656e 6f64 6422 2f3e  rule="evenodd"/>
-000002a0: 3c70 6174 6820 643d 224d 3731 3920 3538  <path d="M719 58
-000002b0: 3920 3736 382e 3034 3320 3538 3922 2073  9 768.043 589" s
-000002c0: 7472 6f6b 653d 2223 3030 3030 3030 2220  troke="#000000" 
-000002d0: 7374 726f 6b65 2d77 6964 7468 3d22 3822  stroke-width="8"
-000002e0: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
-000002f0: 6974 3d22 3822 2066 696c 6c3d 226e 6f6e  it="8" fill="non
-00000300: 6522 2066 696c 6c2d 7275 6c65 3d22 6576  e" fill-rule="ev
-00000310: 656e 6f64 6422 2f3e 3c70 6174 6820 643d  enodd"/><path d=
-00000320: 224d 3731 3620 3539 3320 3731 3620 3634  "M716 593 716 64
-00000330: 312e 3438 3622 2073 7472 6f6b 653d 2223  1.486" stroke="#
-00000340: 3030 3030 3030 2220 7374 726f 6b65 2d77  000000" stroke-w
-00000350: 6964 7468 3d22 3822 2073 7472 6f6b 652d  idth="8" stroke-
-00000360: 6d69 7465 726c 696d 6974 3d22 3822 2066  miterlimit="8" f
-00000370: 696c 6c3d 226e 6f6e 6522 2066 696c 6c2d  ill="none" fill-
-00000380: 7275 6c65 3d22 6576 656e 6f64 6422 2f3e  rule="evenodd"/>
-00000390: 3c70 6174 6820 643d 224d 3730 3820 3539  <path d="M708 59
-000003a0: 3320 3730 3820 3634 312e 3438 3622 2073  3 708 641.486" s
-000003b0: 7472 6f6b 653d 2223 3030 3030 3030 2220  troke="#000000" 
-000003c0: 7374 726f 6b65 2d77 6964 7468 3d22 3822  stroke-width="8"
-000003d0: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
-000003e0: 6974 3d22 3822 2066 696c 6c3d 226e 6f6e  it="8" fill="non
-000003f0: 6522 2066 696c 6c2d 7275 6c65 3d22 6576  e" fill-rule="ev
-00000400: 656e 6f64 6422 2f3e 3c70 6174 6820 643d  enodd"/><path d=
-00000410: 224d 3730 3620 3538 3020 3736 362e 3434  "M706 580 766.44
-00000420: 2036 3338 2e37 3336 2220 7374 726f 6b65   638.736" stroke
-00000430: 3d22 2330 3030 3030 3022 2073 7472 6f6b  ="#000000" strok
-00000440: 652d 7769 6474 683d 2234 2220 7374 726f  e-width="4" stro
-00000450: 6b65 2d6d 6974 6572 6c69 6d69 743d 2238  ke-miterlimit="8
-00000460: 2220 6669 6c6c 3d22 6e6f 6e65 2220 6669  " fill="none" fi
-00000470: 6c6c 2d72 756c 653d 2265 7665 6e6f 6464  ll-rule="evenodd
-00000480: 222f 3e3c 2f67 3e3c 2f73 7667 3e         "/></g></svg>
+00000100: 6e73 6c61 7465 282d 3732 3120 2d35 3137  nslate(-721 -517
+00000110: 2922 3e3c 7061 7468 2064 3d22 4d37 3335  )"><path d="M735
+00000120: 2035 3139 2037 3335 2035 3539 2e31 3733   519 735 559.173
+00000130: 2220 7374 726f 6b65 3d22 2330 3030 3030  " stroke="#00000
+00000140: 3022 2073 7472 6f6b 652d 7769 6474 683d  0" stroke-width=
+00000150: 2238 2220 7374 726f 6b65 2d6d 6974 6572  "8" stroke-miter
+00000160: 6c69 6d69 743d 2238 2220 6669 6c6c 3d22  limit="8" fill="
+00000170: 6e6f 6e65 2220 6669 6c6c 2d72 756c 653d  none" fill-rule=
+00000180: 2265 7665 6e6f 6464 222f 3e3c 7061 7468  "evenodd"/><path
+00000190: 2064 3d22 4d30 2030 2031 332e 3037 3520   d="M0 0 13.075 
+000001a0: 302e 3234 3131 3535 2220 7374 726f 6b65  0.241155" stroke
+000001b0: 3d22 2330 3030 3030 3022 2073 7472 6f6b  ="#000000" strok
+000001c0: 652d 7769 6474 683d 2238 2220 7374 726f  e-width="8" stro
+000001d0: 6b65 2d6d 6974 6572 6c69 6d69 743d 2238  ke-miterlimit="8
+000001e0: 2220 6669 6c6c 3d22 6e6f 6e65 2220 6669  " fill="none" fi
+000001f0: 6c6c 2d72 756c 653d 2265 7665 6e6f 6464  ll-rule="evenodd
+00000200: 2220 7472 616e 7366 6f72 6d3d 226d 6174  " transform="mat
+00000210: 7269 7828 2d31 2030 2030 2031 2037 3339  rix(-1 0 0 1 739
+00000220: 2e30 3735 2035 3331 2922 2f3e 3c70 6174  .075 531)"/><pat
+00000230: 6820 643d 224d 3733 342e 3939 3920 3532  h d="M734.999 52
+00000240: 302e 3336 3943 3733 352e 3037 3120 3532  0.369C735.071 52
+00000250: 352e 3631 3620 3733 302e 3837 3720 3532  5.616 730.877 52
+00000260: 392e 3932 3720 3732 352e 3633 3120 3532  9.927 725.631 52
+00000270: 392e 3939 3920 3732 352e 3439 3520 3533  9.999 725.495 53
+00000280: 302e 3030 3120 3732 352e 3335 3920 3533  0.001 725.359 53
+00000290: 3020 3732 352e 3232 3420 3532 392e 3939  0 725.224 529.99
+000002a0: 3622 2073 7472 6f6b 653d 2223 3030 3030  6" stroke="#0000
+000002b0: 3030 2220 7374 726f 6b65 2d77 6964 7468  00" stroke-width
+000002c0: 3d22 3822 2073 7472 6f6b 652d 6d69 7465  ="8" stroke-mite
+000002d0: 726c 696d 6974 3d22 3822 2066 696c 6c3d  rlimit="8" fill=
+000002e0: 226e 6f6e 6522 2066 696c 6c2d 7275 6c65  "none" fill-rule
+000002f0: 3d22 6576 656e 6f64 6422 2f3e 3c70 6174  ="evenodd"/><pat
+00000300: 6820 643d 224d 3735 3320 3533 302e 3543  h d="M753 530.5C
+00000310: 3735 3320 3532 352e 3830 3620 3735 362e  753 525.806 756.
+00000320: 3830 3620 3532 3220 3736 312e 3520 3532  806 522 761.5 52
+00000330: 324c 3736 312e 3520 3532 3243 3736 362e  2L761.5 522C766.
+00000340: 3139 3420 3532 3220 3737 3020 3532 352e  194 522 770 525.
+00000350: 3830 3620 3737 3020 3533 302e 354c 3737  806 770 530.5L77
+00000360: 3020 3534 372e 3543 3737 3020 3535 322e  0 547.5C770 552.
+00000370: 3139 3420 3736 362e 3139 3420 3535 3620  194 766.194 556 
+00000380: 3736 312e 3520 3535 364c 3736 312e 3520  761.5 556L761.5 
+00000390: 3535 3643 3735 362e 3830 3620 3535 3620  556C756.806 556 
+000003a0: 3735 3320 3535 322e 3139 3420 3735 3320  753 552.194 753 
+000003b0: 3534 372e 355a 2220 7374 726f 6b65 3d22  547.5Z" stroke="
+000003c0: 2330 3030 3030 3022 2073 7472 6f6b 652d  #000000" stroke-
+000003d0: 7769 6474 683d 2238 2220 7374 726f 6b65  width="8" stroke
+000003e0: 2d6d 6974 6572 6c69 6d69 743d 2238 2220  -miterlimit="8" 
+000003f0: 6669 6c6c 3d22 6e6f 6e65 2220 6669 6c6c  fill="none" fill
+00000400: 2d72 756c 653d 2265 7665 6e6f 6464 222f  -rule="evenodd"/
+00000410: 3e3c 7061 7468 2064 3d22 4d37 3435 2035  ><path d="M745 5
+00000420: 3531 2037 3435 2035 3539 2e35 3739 2220  51 745 559.579" 
+00000430: 7374 726f 6b65 3d22 2330 3030 3030 3022  stroke="#000000"
+00000440: 2073 7472 6f6b 652d 7769 6474 683d 2238   stroke-width="8
+00000450: 2220 7374 726f 6b65 2d6d 6974 6572 6c69  " stroke-miterli
+00000460: 6d69 743d 2238 2220 6669 6c6c 3d22 6e6f  mit="8" fill="no
+00000470: 6e65 2220 6669 6c6c 2d72 756c 653d 2265  ne" fill-rule="e
+00000480: 7665 6e6f 6464 222f 3e3c 7061 7468 2064  venodd"/><path d
+00000490: 3d22 4d37 3434 2035 3230 2037 3737 2e32  ="M744 520 777.2
+000004a0: 2035 3537 2e36 2220 7374 726f 6b65 3d22   557.6" stroke="
+000004b0: 2330 3030 3030 3022 2073 7472 6f6b 652d  #000000" stroke-
+000004c0: 7769 6474 683d 2234 2220 7374 726f 6b65  width="4" stroke
+000004d0: 2d6d 6974 6572 6c69 6d69 743d 2238 2220  -miterlimit="8" 
+000004e0: 6669 6c6c 3d22 6e6f 6e65 2220 6669 6c6c  fill="none" fill
+000004f0: 2d72 756c 653d 2265 7665 6e6f 6464 222f  -rule="evenodd"/
+00000500: 3e3c 2f67 3e3c 2f73 7667 3e0d 0a         ></g></svg>..
```

### Comparing `tabulous-0.5.2/rst/_build/html/_images/summarize_table.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/barplot.svg`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,59 @@
-00000000: 3c73 7667 2077 6964 7468 3d22 3530 2220  <svg width="50" 
-00000010: 6865 6967 6874 3d22 3633 220d 0a20 2020  height="63"..   
+00000000: 3c73 7667 2077 6964 7468 3d22 3838 2220  <svg width="88" 
+00000010: 6865 6967 6874 3d22 3833 220d 0a20 2020  height="83"..   
 00000020: 2078 6d6c 6e73 3d22 6874 7470 3a2f 2f77   xmlns="http://w
 00000030: 7777 2e77 332e 6f72 672f 3230 3030 2f73  ww.w3.org/2000/s
 00000040: 7667 220d 0a20 2020 2078 6d6c 6e73 3a78  vg"..    xmlns:x
 00000050: 6c69 6e6b 3d22 6874 7470 3a2f 2f77 7777  link="http://www
 00000060: 2e77 332e 6f72 672f 3139 3939 2f78 6c69  .w3.org/1999/xli
 00000070: 6e6b 2220 6f76 6572 666c 6f77 3d22 6869  nk" overflow="hi
 00000080: 6464 656e 223e 0d0a 2020 2020 3c64 6566  dden">..    <def
 00000090: 733e 0d0a 2020 2020 2020 2020 3c63 6c69  s>..        <cli
 000000a0: 7050 6174 6820 6964 3d22 636c 6970 3022  pPath id="clip0"
 000000b0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-000000c0: 7265 6374 2078 3d22 3432 3822 2079 3d22  rect x="428" y="
-000000d0: 3535 3922 2077 6964 7468 3d22 3530 2220  559" width="50" 
-000000e0: 6865 6967 6874 3d22 3633 222f 3e0d 0a20  height="63"/>.. 
+000000c0: 7265 6374 2078 3d22 3234 3622 2079 3d22  rect x="246" y="
+000000d0: 3437 3022 2077 6964 7468 3d22 3838 2220  470" width="88" 
+000000e0: 6865 6967 6874 3d22 3833 222f 3e0d 0a20  height="83"/>.. 
 000000f0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
 00000100: 683e 0d0a 2020 2020 3c2f 6465 6673 3e0d  h>..    </defs>.
 00000110: 0a20 2020 203c 6720 636c 6970 2d70 6174  .    <g clip-pat
 00000120: 683d 2275 726c 2823 636c 6970 3029 2220  h="url(#clip0)" 
 00000130: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00000140: 6c61 7465 282d 3432 3820 2d35 3539 2922  late(-428 -559)"
+00000140: 6c61 7465 282d 3234 3620 2d34 3730 2922  late(-246 -470)"
 00000150: 3e0d 0a20 2020 2020 2020 203c 7061 7468  >..        <path
-00000160: 2064 3d22 4d34 3333 2e35 2035 3631 2e35   d="M433.5 561.5
-00000170: 2034 3736 2e32 3035 2035 3631 2e35 2220   476.205 561.5" 
-00000180: 7374 726f 6b65 3d22 2330 3030 3030 3022  stroke="#000000"
-00000190: 2073 7472 6f6b 652d 7769 6474 683d 2233   stroke-width="3
-000001a0: 2220 7374 726f 6b65 2d6d 6974 6572 6c69  " stroke-miterli
-000001b0: 6d69 743d 2238 2220 6669 6c6c 3d22 2330  mit="8" fill="#0
-000001c0: 3030 3030 3022 2066 696c 6c2d 7275 6c65  00000" fill-rule
-000001d0: 3d22 6576 656e 6f64 6422 2f3e 0d0a 2020  ="evenodd"/>..  
-000001e0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-000001f0: 3020 3331 2032 312e 3339 3132 2030 2033  0 31 21.3912 0 3
-00000200: 3420 3020 3132 2e36 3038 3820 3331 5a22  4 0 12.6088 31Z"
-00000210: 2066 696c 6c3d 2223 3030 3030 3030 2220   fill="#000000" 
-00000220: 6669 6c6c 2d72 756c 653d 2265 7665 6e6f  fill-rule="eveno
-00000230: 6464 2220 7472 616e 7366 6f72 6d3d 226d  dd" transform="m
-00000240: 6174 7269 7828 2d31 2030 2030 2031 2034  atrix(-1 0 0 1 4
-00000250: 3632 2035 3630 2922 2f3e 0d0a 2020 2020  62 560)"/>..    
-00000260: 2020 2020 3c70 6174 6820 643d 224d 3436      <path d="M46
-00000270: 3220 3539 3020 3433 392e 3831 3620 3632  2 590 439.816 62
-00000280: 3120 3432 3820 3632 3120 3435 302e 3138  1 428 621 450.18
-00000290: 3420 3539 305a 2220 6669 6c6c 3d22 2330  4 590Z" fill="#0
-000002a0: 3030 3030 3022 2066 696c 6c2d 7275 6c65  00000" fill-rule
-000002b0: 3d22 6576 656e 6f64 6422 2f3e 0d0a 2020  ="evenodd"/>..  
-000002c0: 2020 2020 2020 3c70 6174 6820 643d 224d        <path d="M
-000002d0: 3433 332e 3520 3631 392e 3520 3437 362e  433.5 619.5 476.
-000002e0: 3230 3520 3631 392e 3522 2073 7472 6f6b  205 619.5" strok
-000002f0: 653d 2223 3030 3030 3030 2220 7374 726f  e="#000000" stro
-00000300: 6b65 2d77 6964 7468 3d22 3322 2073 7472  ke-width="3" str
-00000310: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
-00000320: 3822 2066 696c 6c3d 2223 3030 3030 3030  8" fill="#000000
-00000330: 2220 6669 6c6c 2d72 756c 653d 2265 7665  " fill-rule="eve
-00000340: 6e6f 6464 222f 3e0d 0a20 2020 2020 2020  nodd"/>..       
-00000350: 203c 7061 7468 2064 3d22 4d34 3737 2035   <path d="M477 5
-00000360: 3630 2034 3737 2035 3731 2034 3636 2035  60 477 571 466 5
-00000370: 3630 5a22 2066 696c 6c3d 2223 3030 3030  60Z" fill="#0000
-00000380: 3030 2220 6669 6c6c 2d72 756c 653d 2265  00" fill-rule="e
-00000390: 7665 6e6f 6464 222f 3e0d 0a20 2020 2020  venodd"/>..     
-000003a0: 2020 203c 7061 7468 2064 3d22 4d30 2031     <path d="M0 1
-000003b0: 3220 3020 3020 3130 2031 325a 2220 6669  2 0 0 10 12Z" fi
-000003c0: 6c6c 3d22 2330 3030 3030 3022 2066 696c  ll="#000000" fil
-000003d0: 6c2d 7275 6c65 3d22 6576 656e 6f64 6422  l-rule="evenodd"
-000003e0: 2074 7261 6e73 666f 726d 3d22 6d61 7472   transform="matr
-000003f0: 6978 282d 3120 312e 3232 3436 3565 2d31  ix(-1 1.22465e-1
-00000400: 3620 312e 3232 3436 3565 2d31 3620 3120  6 1.22465e-16 1 
-00000410: 3437 3620 3630 3929 222f 3e0d 0a20 2020  476 609)"/>..   
-00000420: 203c 2f67 3e0d 0a3c 2f73 7667 3e          </g>..</svg>
+00000160: 2064 3d22 4d32 3534 2034 3730 2032 3534   d="M254 470 254
+00000170: 2035 3437 2e36 3039 2220 7374 726f 6b65   547.609" stroke
+00000180: 3d22 2330 3030 3030 3022 2073 7472 6f6b  ="#000000" strok
+00000190: 652d 7769 6474 683d 2238 2220 7374 726f  e-width="8" stro
+000001a0: 6b65 2d6d 6974 6572 6c69 6d69 743d 2238  ke-miterlimit="8
+000001b0: 2220 6669 6c6c 3d22 6e6f 6e65 2220 6669  " fill="none" fi
+000001c0: 6c6c 2d72 756c 653d 2265 7665 6e6f 6464  ll-rule="evenodd
+000001d0: 222f 3e0d 0a20 2020 2020 2020 203c 7061  "/>..        <pa
+000001e0: 7468 2064 3d22 4d30 2030 2038 322e 3630  th d="M0 0 82.60
+000001f0: 3434 2030 2e30 3030 3130 3439 3837 2220  44 0.000104987" 
+00000200: 7374 726f 6b65 3d22 2330 3030 3030 3022  stroke="#000000"
+00000210: 2073 7472 6f6b 652d 7769 6474 683d 2238   stroke-width="8
+00000220: 2220 7374 726f 6b65 2d6d 6974 6572 6c69  " stroke-miterli
+00000230: 6d69 743d 2238 2220 6669 6c6c 3d22 6e6f  mit="8" fill="no
+00000240: 6e65 2220 6669 6c6c 2d72 756c 653d 2265  ne" fill-rule="e
+00000250: 7665 6e6f 6464 2220 7472 616e 7366 6f72  venodd" transfor
+00000260: 6d3d 226d 6174 7269 7828 2d31 2030 2030  m="matrix(-1 0 0
+00000270: 2031 2033 3333 2e36 3034 2035 3434 2922   1 333.604 544)"
+00000280: 2f3e 0d0a 2020 2020 2020 2020 3c72 6563  />..        <rec
+00000290: 7420 783d 2232 3633 2e35 2220 793d 2234  t x="263.5" y="4
+000002a0: 3933 2e35 2220 7769 6474 683d 2232 3822  93.5" width="28"
+000002b0: 2068 6569 6768 743d 2234 3922 2073 7472   height="49" str
+000002c0: 6f6b 653d 2223 3030 3030 3030 2220 7374  oke="#000000" st
+000002d0: 726f 6b65 2d77 6964 7468 3d22 312e 3333  roke-width="1.33
+000002e0: 3333 3322 2066 696c 6c3d 2223 3030 3030  333" fill="#0000
+000002f0: 3030 2220 7374 726f 6b65 2d6d 6974 6572  00" stroke-miter
+00000300: 6c69 6d69 743d 2238 222f 3e0d 0a20 2020  limit="8"/>..   
+00000310: 2020 2020 203c 7265 6374 2078 3d22 3239       <rect x="29
+00000320: 372e 3522 2079 3d22 3531 302e 3522 2077  7.5" y="510.5" w
+00000330: 6964 7468 3d22 3238 2220 6865 6967 6874  idth="28" height
+00000340: 3d22 3332 2220 7374 726f 6b65 3d22 2330  ="32" stroke="#0
+00000350: 3030 3030 3022 2073 7472 6f6b 652d 7769  00000" stroke-wi
+00000360: 6474 683d 2231 2e33 3333 3333 2220 6669  dth="1.33333" fi
+00000370: 6c6c 3d22 2330 3030 3030 3022 2073 7472  ll="#000000" str
+00000380: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
+00000390: 3822 2f3e 0d0a 2020 2020 3c2f 673e 0d0a  8"/>..    </g>..
+000003a0: 3c2f 7376 673e 0d0a                      </svg>..
```

### Comparing `tabulous-0.5.2/tabulous/__main__.py` & `tabulous-0.5.3/tabulous/__main__.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_colormap.py` & `tabulous-0.5.3/tabulous/_colormap.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_dtype.py` & `tabulous-0.5.3/tabulous/_dtype.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_fetch_and_install.py` & `tabulous-0.5.3/tabulous/_fetch_and_install.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_io.py` & `tabulous-0.5.3/tabulous/_io.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_keymap/_callback.py` & `tabulous-0.5.3/tabulous/_keymap/_callback.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_keymap/_keymap_objects.py` & `tabulous-0.5.3/tabulous/_keymap/_keymap_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Sequence,
     TYPE_CHECKING,
     TypeVar,
     Union,
     overload,
 )
 
-from qtpy import QtGui
+from qtpy import QtGui, QT6
 from qtpy.QtCore import Qt
 from functools import reduce
 from operator import or_
 
 from tabulous.exceptions import TriggerParent
 
 from ._callback import BoundCallback
@@ -143,14 +143,22 @@
 )
 ALPHA = QtGui.QKeySequence("α")[0]
 OMEGA = QtGui.QKeySequence("ω")[0]
 
 CYR_A = QtGui.QKeySequence("а")[0]
 CYR_YA = QtGui.QKeySequence("я")[0]
 
+if QT6:
+    # Since Qt6, indexing QKeySequence returns a QKeyCombination object, which
+    # does not support comparison with Qt.Key(int).
+    ALPHA = ALPHA.key()
+    OMEGA = OMEGA.key()
+    CYR_A = CYR_A.key()
+    CYR_YA = CYR_YA.key()
+
 
 class QtKeys:
     """A custom class for handling key events."""
 
     def __init__(self, e: KeyType):
         if isinstance(e, QtGui.QKeyEvent):
             self.modifier = _parse_modifiers(e.modifiers())
```

### Comparing `tabulous-0.5.2/tabulous/_keymap/_keymapview.py` & `tabulous-0.5.3/tabulous/_keymap/_keymapview.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_magicgui/__init__.py` & `tabulous-0.5.3/tabulous/_magicgui/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_magicgui/_color_edit.py` & `tabulous-0.5.3/tabulous/_magicgui/_color_edit.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_magicgui/_dialog.py` & `tabulous-0.5.3/tabulous/_magicgui/_dialog.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_magicgui/_register.py` & `tabulous-0.5.3/tabulous/_magicgui/_register.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_magicgui/_selection.py` & `tabulous-0.5.3/tabulous/_magicgui/_selection.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_magicgui/_table.py` & `tabulous-0.5.3/tabulous/_magicgui/_table.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_magicgui/_timedelta.py` & `tabulous-0.5.3/tabulous/_magicgui/_timedelta.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_magicgui/_toggle_switch.py` & `tabulous-0.5.3/tabulous/_magicgui/_toggle_switch.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_map_model.py` & `tabulous-0.5.3/tabulous/_map_model.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_pd_index.py` & `tabulous-0.5.3/tabulous/_pd_index.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_psygnal.py` & `tabulous-0.5.3/tabulous/_psygnal.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,21 +346,22 @@
         elif isinstance(_row, int) and isinstance(_col, int):  # set scalar
             _out = str(_out)
 
         else:
             raise UnreachableError(type(_row), type(_col))
 
         _sel_model = qtable_view._selection_model
-        # fmt: off
-        with _sel_model.blocked(), \
-            qtable_view._table_map.lock_pos(self.pos), \
-            table.undo_manager.merging(lambda _: f"{self.as_literal(dest=True)}"), \
-            table.proxy.released(keep_widgets=True):
+        with (
+            _sel_model.blocked(),
+            qtable_view._table_map.lock_pos(self.pos),
+            table.undo_manager.merging(lambda _: f"{self.as_literal(dest=True)}"),
+            table.proxy.released(keep_widgets=True),
+        ):
             qtable.setDataFrameValue(_row, _col, _out)
-        # fmt: on
+            qtable.model()._background_color_anim.start(_row, _col)
         self.last_destination = (_row, _col)
         return EvalResult(out, (_row, _col))
 
     def after_called(self, out: EvalResult) -> None:
         table = self.table
         qtable = table._qwidget
         qtable_view = qtable._qtable_view
@@ -377,21 +378,23 @@
             else:
                 err_repr = pd.NA
             val = np.full(
                 (rsl.stop - rsl.start, csl.stop - csl.start),
                 err_repr,
                 dtype=object,
             )
-            # fmt: off
-            with qtable_view._selection_model.blocked(), \
-                qtable_view._table_map.lock_pos(self.pos), \
-                table.events.data.blocked(), \
-                table.proxy.released(keep_widgets=True):
-                table._qwidget.setDataFrameValue(rsl, csl, pd.DataFrame(val))
-            # fmt: on
+            # insert error values
+            with (
+                qtable_view._selection_model.blocked(),
+                qtable_view._table_map.lock_pos(self.pos),
+                table.events.data.blocked(),
+                table.proxy.released(keep_widgets=True),
+            ):
+                qtable.setDataFrameValue(rsl, csl, pd.DataFrame(val))
+                qtable.model()._background_color_anim.start(rsl, csl)
         return None
 
     def call(self):
         """Function that will be called when cells changed."""
         out = self.evaluate()
         self.after_called(out)
         return out
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_action_registry.py` & `tabulous-0.5.3/tabulous/_qt/_action_registry.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_app.py` & `tabulous-0.5.3/tabulous/_qt/_app.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_clickable_label.py` & `tabulous-0.5.3/tabulous/_qt/_clickable_label.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_console.py` & `tabulous-0.5.3/tabulous/_qt/_console.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+from functools import lru_cache
 
 from pathlib import Path
 import weakref
 from typing import TYPE_CHECKING, cast
 from contextlib import suppress
 
 from qtpy.QtCore import Signal
@@ -98,38 +99,45 @@
 
             from IPython.paths import get_ipython_dir
             from tabulous._utils import get_config
 
             config = get_config()
             _ns = config.console_namespace
 
+            _exit = _get_exit_auto_call()
+            _exit.set_viewer(widget)
+            self.shell.push({"exit": _exit})  # update the "exit"
+
             # run IPython startup files
             profile_dir = Path(get_ipython_dir()) / "profile_default" / "startup"
             if profile_dir.exists() and _ns.load_startup_file:
                 import runpy
 
                 _globals = {}
                 for startup in profile_dir.glob("*.py"):
                     with suppress(Exception):
-                        _globals.update(runpy.run_path(startup))
+                        _globals.update(runpy.run_path(str(startup)))
 
                 self.shell.push(_globals)
 
             # update namespaces
             import tabulous as tbl
             import numpy as np
             import pandas as pd
+            from tabulous._ipython import install_magics, VIEWER_IDENTIFIER
 
             ns = {
+                VIEWER_IDENTIFIER: widget,
                 _ns.viewer: widget,
                 _ns.numpy: np,
                 _ns.pandas: pd,
                 _ns.tabulous: tbl,
             }
             self.shell.push(ns)
+            install_magics()
 
     def setFocus(self):
         """Set focus to the text edit."""
         self._control.setFocus()
         cursor = self._control.textCursor()
         cursor.clearSelection()
         self._control.setTextCursor(cursor)
@@ -285,7 +293,27 @@
         light_theme = sum(normalize_color(style.background)[:3]) > 382.5
         if light_theme:
             self.syntax_style = "default"
         else:
             self.syntax_style = "vim"
         bracket_color = QtGui.QColor(*normalize_color(style.highlight0))
         self._bracket_matcher.format.setBackground(bracket_color)
+
+
+@lru_cache(maxsize=1)
+def _get_exit_auto_call():
+    from IPython.core.autocall import IPyAutocall
+
+    class ExitAutocall(IPyAutocall):
+        """Overwrite the default 'exit' autocall to close the viewer."""
+
+        def __init__(self, ip=None):
+            super().__init__(ip)
+            self._viewer = None
+
+        def set_viewer(self, viewer: TableViewerBase):
+            self._viewer = weakref.ref(viewer)
+
+        def __call__(self, *args, **kwargs):
+            self._viewer().close()
+
+    return ExitAutocall()
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_dockwidget.py` & `tabulous-0.5.3/tabulous/_qt/_dockwidget.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_filetree.py` & `tabulous-0.5.3/tabulous/_qt/_filetree.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,11 +79,12 @@
         self._file_tree = QFileTreeWidget(self)
         curpath = QtCore.QDir.currentPath()
         self._file_tree.setRoot(curpath)
         self._file_edit.value = Path(curpath)
         self._layout.addWidget(self._file_edit.native)
         self._layout.addWidget(self._file_tree)
         self._file_edit.changed.connect(self._update_root)
+        self._update_root(curpath)
 
     def _update_root(self, path: str):
         if Path(path).exists():
             self._file_tree.setRoot(str(path))
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_history.py` & `tabulous-0.5.3/tabulous/_qt/_history.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_icons/barplot.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/boxplot.svg`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 00000060: 2e77 332e 6f72 672f 3139 3939 2f78 6c69  .w3.org/1999/xli
 00000070: 6e6b 2220 6f76 6572 666c 6f77 3d22 6869  nk" overflow="hi
 00000080: 6464 656e 223e 0d0a 2020 2020 3c64 6566  dden">..    <def
 00000090: 733e 0d0a 2020 2020 2020 2020 3c63 6c69  s>..        <cli
 000000a0: 7050 6174 6820 6964 3d22 636c 6970 3022  pPath id="clip0"
 000000b0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
 000000c0: 7265 6374 2078 3d22 3234 3622 2079 3d22  rect x="246" y="
-000000d0: 3437 3022 2077 6964 7468 3d22 3838 2220  470" width="88" 
+000000d0: 3537 3922 2077 6964 7468 3d22 3838 2220  579" width="88" 
 000000e0: 6865 6967 6874 3d22 3833 222f 3e0d 0a20  height="83"/>.. 
 000000f0: 2020 2020 2020 203c 2f63 6c69 7050 6174         </clipPat
 00000100: 683e 0d0a 2020 2020 3c2f 6465 6673 3e0d  h>..    </defs>.
 00000110: 0a20 2020 203c 6720 636c 6970 2d70 6174  .    <g clip-pat
 00000120: 683d 2275 726c 2823 636c 6970 3029 2220  h="url(#clip0)" 
 00000130: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
-00000140: 6c61 7465 282d 3234 3620 2d34 3730 2922  late(-246 -470)"
+00000140: 6c61 7465 282d 3234 3620 2d35 3739 2922  late(-246 -579)"
 00000150: 3e0d 0a20 2020 2020 2020 203c 7061 7468  >..        <path
-00000160: 2064 3d22 4d32 3534 2034 3730 2032 3534   d="M254 470 254
-00000170: 2035 3437 2e36 3039 2220 7374 726f 6b65   547.609" stroke
+00000160: 2064 3d22 4d32 3534 2035 3830 2032 3534   d="M254 580 254
+00000170: 2036 3537 2e36 3039 2220 7374 726f 6b65   657.609" stroke
 00000180: 3d22 2330 3030 3030 3022 2073 7472 6f6b  ="#000000" strok
 00000190: 652d 7769 6474 683d 2238 2220 7374 726f  e-width="8" stro
 000001a0: 6b65 2d6d 6974 6572 6c69 6d69 743d 2238  ke-miterlimit="8
 000001b0: 2220 6669 6c6c 3d22 6e6f 6e65 2220 6669  " fill="none" fi
 000001c0: 6c6c 2d72 756c 653d 2265 7665 6e6f 6464  ll-rule="evenodd
 000001d0: 222f 3e0d 0a20 2020 2020 2020 203c 7061  "/>..        <pa
 000001e0: 7468 2064 3d22 4d30 2030 2038 322e 3630  th d="M0 0 82.60
@@ -33,27 +33,43 @@
 00000200: 7374 726f 6b65 3d22 2330 3030 3030 3022  stroke="#000000"
 00000210: 2073 7472 6f6b 652d 7769 6474 683d 2238   stroke-width="8
 00000220: 2220 7374 726f 6b65 2d6d 6974 6572 6c69  " stroke-miterli
 00000230: 6d69 743d 2238 2220 6669 6c6c 3d22 6e6f  mit="8" fill="no
 00000240: 6e65 2220 6669 6c6c 2d72 756c 653d 2265  ne" fill-rule="e
 00000250: 7665 6e6f 6464 2220 7472 616e 7366 6f72  venodd" transfor
 00000260: 6d3d 226d 6174 7269 7828 2d31 2030 2030  m="matrix(-1 0 0
-00000270: 2031 2033 3333 2e36 3034 2035 3434 2922   1 333.604 544)"
+00000270: 2031 2033 3333 2e36 3034 2036 3533 2922   1 333.604 653)"
 00000280: 2f3e 0d0a 2020 2020 2020 2020 3c72 6563  />..        <rec
-00000290: 7420 783d 2232 3633 2e35 2220 793d 2234  t x="263.5" y="4
-000002a0: 3933 2e35 2220 7769 6474 683d 2232 3822  93.5" width="28"
-000002b0: 2068 6569 6768 743d 2234 3922 2073 7472   height="49" str
+00000290: 7420 783d 2232 3633 2e35 2220 793d 2235  t x="263.5" y="5
+000002a0: 3939 2e35 2220 7769 6474 683d 2232 3822  99.5" width="28"
+000002b0: 2068 6569 6768 743d 2232 3022 2073 7472   height="20" str
 000002c0: 6f6b 653d 2223 3030 3030 3030 2220 7374  oke="#000000" st
 000002d0: 726f 6b65 2d77 6964 7468 3d22 312e 3333  roke-width="1.33
 000002e0: 3333 3322 2066 696c 6c3d 2223 3030 3030  333" fill="#0000
 000002f0: 3030 2220 7374 726f 6b65 2d6d 6974 6572  00" stroke-miter
 00000300: 6c69 6d69 743d 2238 222f 3e0d 0a20 2020  limit="8"/>..   
 00000310: 2020 2020 203c 7265 6374 2078 3d22 3239       <rect x="29
-00000320: 372e 3522 2079 3d22 3531 302e 3522 2077  7.5" y="510.5" w
+00000320: 382e 3522 2079 3d22 3632 352e 3522 2077  8.5" y="625.5" w
 00000330: 6964 7468 3d22 3238 2220 6865 6967 6874  idth="28" height
-00000340: 3d22 3332 2220 7374 726f 6b65 3d22 2330  ="32" stroke="#0
+00000340: 3d22 3133 2220 7374 726f 6b65 3d22 2330  ="13" stroke="#0
 00000350: 3030 3030 3022 2073 7472 6f6b 652d 7769  00000" stroke-wi
 00000360: 6474 683d 2231 2e33 3333 3333 2220 6669  dth="1.33333" fi
 00000370: 6c6c 3d22 2330 3030 3030 3022 2073 7472  ll="#000000" str
 00000380: 6f6b 652d 6d69 7465 726c 696d 6974 3d22  oke-miterlimit="
-00000390: 3822 2f3e 0d0a 2020 2020 3c2f 673e 0d0a  8"/>..    </g>..
-000003a0: 3c2f 7376 673e 0d0a                      </svg>..
+00000390: 3822 2f3e 0d0a 2020 2020 2020 2020 3c70  8"/>..        <p
+000003a0: 6174 6820 643d 224d 3237 3820 3538 3420  ath d="M278 584 
+000003b0: 3237 3820 3633 312e 3133 3822 2073 7472  278 631.138" str
+000003c0: 6f6b 653d 2223 3030 3030 3030 2220 7374  oke="#000000" st
+000003d0: 726f 6b65 2d77 6964 7468 3d22 3422 2073  roke-width="4" s
+000003e0: 7472 6f6b 652d 6d69 7465 726c 696d 6974  troke-miterlimit
+000003f0: 3d22 3822 2066 696c 6c3d 226e 6f6e 6522  ="8" fill="none"
+00000400: 2066 696c 6c2d 7275 6c65 3d22 6576 656e   fill-rule="even
+00000410: 6f64 6422 2f3e 0d0a 2020 2020 2020 2020  odd"/>..        
+00000420: 3c70 6174 6820 643d 224d 3331 3220 3631  <path d="M312 61
+00000430: 3420 3331 3220 3634 362e 3437 3922 2073  4 312 646.479" s
+00000440: 7472 6f6b 653d 2223 3030 3030 3030 2220  troke="#000000" 
+00000450: 7374 726f 6b65 2d77 6964 7468 3d22 3422  stroke-width="4"
+00000460: 2073 7472 6f6b 652d 6d69 7465 726c 696d   stroke-miterlim
+00000470: 6974 3d22 3822 2066 696c 6c3d 226e 6f6e  it="8" fill="non
+00000480: 6522 2066 696c 6c2d 7275 6c65 3d22 6576  e" fill-rule="ev
+00000490: 656e 6f64 6422 2f3e 0d0a 2020 2020 3c2f  enodd"/>..    </
+000004a0: 673e 0d0a 3c2f 7376 673e 0d0a            g>..</svg>..
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_icons/new_spreadsheet.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/new_spreadsheet.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_icons/preferences.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/preferences.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_icons/random.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/random.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_icons/settings.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/settings.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_icons/swarmplot.svg` & `tabulous-0.5.3/tabulous/_qt/_icons/swarmplot.svg`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_icons/window_icon.png` & `tabulous-0.5.3/tabulous/_qt/_icons/window_icon.png`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_mainwindow/_base.py` & `tabulous-0.5.3/tabulous/_qt/_mainwindow/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,18 +70,23 @@
 
         # update with user namespace
         self._namespace = Namespace()
         self._namespace.update_safely(load_cell_namespace())
 
         # install command palette
         self._command_palette = get_palette("tabulous")
-        self._command_palette.install(self)
-        qcommand_palette = self._command_palette.get_widget(self)
-        qcommand_palette.hidden.connect(self._on_hidden)
-        qcommand_palette.setFont(QtGui.QFont("Arial", 10))
+        try:
+            self._command_palette.install(self)
+        except RuntimeError:
+            # During test, main window might have been destroyed
+            pass
+        else:
+            qcommand_palette = self._command_palette.get_widget(self)
+            qcommand_palette.hidden.connect(self._on_hidden)
+            qcommand_palette.setFont(QtGui.QFont("Arial", 10))
 
     def _on_hidden(self):
         try:
             self.setCellFocus()
         except AttributeError:
             pass
 
@@ -238,7 +243,12 @@
         """Set selection slices to the table selection editor"""
         if table := self._table_viewer.current_table:
             sel = list(table.selections)
             self._toolbar.blockSignals(True)
             sel[-1] = sl
             table.selections = sel
             self._toolbar.blockSignals(False)
+
+    # subclasses will override this method. Just for signature compatibility.
+    def close(self, ask: bool | None = False) -> bool:
+        """Close the window."""
+        return super().close()
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_mainwindow/_command_palette.py` & `tabulous-0.5.3/tabulous/_qt/_mainwindow/_command_palette.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_mainwindow/_keycombo.py` & `tabulous-0.5.3/tabulous/_qt/_mainwindow/_keycombo.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_mainwindow/_mainwidgets.py` & `tabulous-0.5.3/tabulous/_qt/_mainwindow/_mainwidgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from pathlib import Path
-import weakref
 from qtpy import QtWidgets as QtW, QtGui
 from qtpy.QtCore import Qt, QEvent, QTimer
 
 from ._base import _QtMainWidgetBase
 from tabulous._keymap import QtKeyMap
 from tabulous.types import TabPosition
 from tabulous._utils import get_config
 
 if TYPE_CHECKING:
     from tabulous.widgets import TableViewer
     from tabulous._qt._table_stack import QTabbedTableStack
-    from tabulous._qt._dockwidget import QtDockWidget
 
 ICON_DIR = Path(__file__).parent.parent / "_icons"
 
 
 class QMainWidget(QtW.QSplitter, _QtMainWidgetBase):
     _keymap = QtKeyMap()
 
@@ -116,15 +114,14 @@
 # Flag to assert that the new version of tabulous will be notified only once
 _NOTIFIED = False
 
 
 class QMainWindow(QtW.QMainWindow, _QtMainWidgetBase):
     _instances: list[QMainWindow] = []
     _keymap = QtKeyMap()
-    _dock_widgets: weakref.WeakValueDictionary[str, QtDockWidget]
     _is_mainwindow = True
 
     def __init__(
         self,
         tab_position: TabPosition | str = TabPosition.top,
     ):
         from tabulous._qt._toolbar import QTableStackToolBar
@@ -134,15 +131,14 @@
         super().__init__()
         _QtMainWidgetBase.__init__(self, tab_position=tab_position)
         self.setWindowTitle("tabulous")
 
         self.setWindowIcon(QtGui.QIcon(str(ICON_DIR / "window_icon.png")))
 
         self._console_dock_widget = None
-        self._dock_widgets = weakref.WeakValueDictionary()
 
         # ask if it is OK to close
         self._ask_on_close = cfg.window.ask_on_close
 
         self._toolbar = QTableStackToolBar(self)
         self.addToolBar(self._toolbar)
         self._toolbar.setMovable(False)  # nested toolbar causes layout problems
@@ -225,31 +221,33 @@
         return window._table_viewer if window else None
 
     def show(self) -> None:
         global _NOTIFIED
 
         super().show()
 
-        if _NOTIFIED:
+        if _NOTIFIED or not get_config().window.notify_latest:
             return
         _NOTIFIED = True
+
         from tabulous._fetch_and_install import get_worker
 
         worker = get_worker()
 
         @worker.returned.connect
         def _(v: str):
             if v is not None and get_config().window.notify_latest:
                 self._tablestack.notifyLatestVersion(v)
             # NOTE: uncomment the following line to test the notification
             # self._tablestack.notifyLatestVersion("0.X.X")
 
         worker.start()
 
     def close(self, ask: bool | None = False) -> bool:
+        """Close the window. If `ask` is True, ask if it is OK to close."""
         if ask is not None:
             self._ask_on_close = ask
         return super().close()
 
     def event(self, e: QEvent):
         type = e.type()
         if type == QEvent.Type.Close:
@@ -309,15 +307,15 @@
                 if not self._tablestack.isEmpty():
                     if get_config().window.selection_editor:
                         toolbar._corner_widget.show()
                     else:
                         toolbar._corner_widget.hide()
 
             for table in self._table_viewer.tables:
-                table._qwidget._qtable_view.load_config(cfg)
+                table._qwidget.load_config(cfg)
         return None
 
 
 class QRichStatusBar(QtW.QStatusBar):
     """Custom status bar with rich text support."""
 
     def __init__(self, parent: QtW.QWidget | None = None) -> None:
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_mainwindow/_namespace.py` & `tabulous-0.5.3/tabulous/_qt/_mainwindow/_namespace.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_mainwindow/_titlebar.py` & `tabulous-0.5.3/tabulous/_qt/_mainwindow/_titlebar.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_multitips.py` & `tabulous-0.5.3/tabulous/_qt/_multitips.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_plot/_artist_editors.py` & `tabulous-0.5.3/tabulous/_qt/_plot/_artist_editors.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_plot/_artist_types.py` & `tabulous-0.5.3/tabulous/_qt/_plot/_artist_types.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_plot/_mpl_canvas.py` & `tabulous-0.5.3/tabulous/_qt/_plot/_mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_plot/_widget.py` & `tabulous-0.5.3/tabulous/_qt/_plot/_widget.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_preference/_general.py` & `tabulous-0.5.3/tabulous/_qt/_preference/_general.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     def get_updated_config(self):
         cfg = get_config()
         cfg.window.ask_on_close = self._ask_on_close.isChecked()
         cfg.window.notify_latest = self._notify_latest.isChecked()
         cfg.window.selection_editor = self._selection_editor.isChecked()
         cfg.window.show_console = self._show_console.isChecked()
+        cfg.window.animate = self._animate.isChecked()
         cfg.console_namespace.load_startup_file = self._load_startup.isChecked()
         return cfg
 
     def _update_config(self):
         cfg = self.get_updated_config()
         update_config(cfg)
         QMainWindow.reload_config()
@@ -39,25 +40,30 @@
 
         self._selection_editor = QToggleSwitch()
         self._selection_editor.setChecked(cfg.window.selection_editor)
 
         self._show_console = QToggleSwitch()
         self._show_console.setChecked(cfg.window.show_console)
 
+        self._animate = QToggleSwitch()
+        self._animate.setChecked(cfg.window.animate)
+
         self._load_startup = QToggleSwitch()
         self._load_startup.setChecked(cfg.console_namespace.load_startup_file)
 
         _layout = QtW.QFormLayout()
 
         _layout.addRow("Ask before closing window", self._ask_on_close)
         _layout.addRow("Notify latest version", self._notify_latest)
         _layout.addRow("Show selection editor", self._selection_editor)
         _layout.addRow("Show Qt console", self._show_console)
+        _layout.addRow("Enable animations", self._animate)
         _layout.addRow("Load IPython startup files", self._load_startup)
 
         self._ask_on_close.toggled.connect(self._update_config)
         self._notify_latest.toggled.connect(self._update_config)
         self._selection_editor.toggled.connect(self._update_config)
         self._show_console.toggled.connect(self._update_config)
+        self._animate.toggled.connect(self._update_config)
         self._load_startup.toggled.connect(self._update_config)
 
         self.setLayout(_layout)
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_preference/_main.py` & `tabulous-0.5.3/tabulous/_qt/_preference/_main.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_preference/_shared.py` & `tabulous-0.5.3/tabulous/_qt/_preference/_shared.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_preference/_table_config.py` & `tabulous-0.5.3/tabulous/_qt/_preference/_table_config.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_preference/_theme.py` & `tabulous-0.5.3/tabulous/_qt/_preference/_theme.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_progress.py` & `tabulous-0.5.3/tabulous/_qt/_progress.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_proxy_button.py` & `tabulous-0.5.3/tabulous/_qt/_proxy_button.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_svg.py` & `tabulous-0.5.3/tabulous/_qt/_svg.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_delegate.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_delegate.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,9 +132,14 @@
     def initStyleOption(
         self, option: QtW.QStyleOptionViewItem, index: QtCore.QModelIndex
     ):
         super().initStyleOption(option, index)
         if option.state & QtW.QStyle.StateFlag.State_HasFocus:
             option.state = option.state & ~QtW.QStyle.StateFlag.State_HasFocus
 
+    # fmt: off
+    if TYPE_CHECKING:
+        def parent(self) -> _QTableViewEnhanced: ...
+    # fmt: on
+
     def parentTable(self) -> QBaseTable:
         return self.parent().parent()
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_enhanced_table.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_enhanced_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         # header settings
         vheader = QVerticalHeaderView()
         hheader = QHorizontalHeaderView()
         self.setVerticalHeader(vheader)
         self.setHorizontalHeader(hheader)
 
         vheader.resize(36, vheader.height())
+        _valign = Qt.AlignmentFlag.AlignRight | Qt.AlignmentFlag.AlignVCenter
+        vheader.setDefaultAlignment(_valign)
         vheader.setMinimumSectionSize(5)
         hheader.setMinimumSectionSize(5)
 
         vheader.setDefaultSectionSize(self._h_default)
         hheader.setDefaultSectionSize(self._w_default)
 
         self.setVerticalScrollMode(_SCROLL_PER_PIXEL)
@@ -124,22 +126,14 @@
 
         self._table_map = DummySlotRefMapping()
 
         # initialize colors
         self._selection_color = QtGui.QColor(120, 120, 170, 255)
         self._highlight_color = QtGui.QColor(255, 0, 0, 86)
 
-    # fmt: off
-    if TYPE_CHECKING:
-        def model(self) -> AbstractDataFrameModel: ...
-        def itemDelegate(self) -> TableItemDelegate: ...
-        def verticalHeader(self) -> QVerticalHeaderView: ...
-        def horizontalHeader(self) -> QHorizontalHeaderView: ...
-    # fmt: on
-
     def load_config(self, cfg: TabulousConfig | None = None) -> None:
         from tabulous._utils import get_config
 
         if cfg is None:
             cfg = get_config()
 
         table = cfg.table
@@ -598,16 +592,18 @@
             self._rect_from_ranges(self._highlight_model._ranges, map=True)
         ):
             painter.fillRect(rect, h_color)
 
         # draw selections
         s_color = self._get_selection_color()
         for i, rect in enumerate(self._rect_from_ranges(self._selection_model._ranges)):
-            last_one = nsel == i + 1
-            pen = QtGui.QPen(s_color, 2 + int(last_one) * focused)
+            if nsel == i + 1:
+                pen = QtGui.QPen(s_color, 2 + focused)
+            else:
+                pen = QtGui.QPen(s_color, 2)
             painter.setPen(pen)
             painter.drawRect(rect)
 
         # current index
         idx = self._selection_model.current_index
         if idx >= (0, 0):
             rect_cursor = self.visualRect(self.model().index(*idx))
@@ -687,14 +683,30 @@
         if not isinstance(text, str):
             text = ""
         line = QCellLiteralEdit.from_table(self, text)
         line.show()
         line.setFocus()
         return line
 
+    # fmt: off
+    if TYPE_CHECKING:
+        def model(self) -> AbstractDataFrameModel: ...
+        def itemDelegate(self) -> TableItemDelegate: ...
+        def verticalHeader(self) -> QVerticalHeaderView: ...
+        def horizontalHeader(self) -> QHorizontalHeaderView: ...
+        @property
+        def highlightColor(self) -> QtGui.QColor: ...
+        @highlightColor.setter
+        def highlightColor(self, color: QtGui.QColor): ...
+        @property
+        def selectionColor(self) -> QtGui.QColor: ...
+        @selectionColor.setter
+        def selectionColor(self, color: QtGui.QColor): ...
+    # fmt: on
+
 
 def _color_cycle() -> Iterator[QtGui.QColor]:
     """Generate easily distinguishable colors."""
     # This is the default color cycle of matplotlib
     colors = [
         QtGui.QColor(31, 119, 180),
         QtGui.QColor(255, 127, 14),
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_header_view.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_header_view.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_item_model.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_item_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
-from typing import Any, Callable, Hashable, TYPE_CHECKING, cast
+from typing import Any, Callable, Hashable, TYPE_CHECKING, Iterable, cast
 import warnings
 from qtpy import QtCore, QtGui, QtWidgets as QtW
 from qtpy.QtCore import Qt, Signal
 import pandas as pd
 
 from tabulous._dtype import isna
 from tabulous.color import normalize_color, ColorType
 from tabulous._text_formatter import DefaultFormatter
 from tabulous._map_model import TableMapping
 from tabulous._utils import get_config
+from tabulous._qt._table._animation import CellColorAnimation
 
 if TYPE_CHECKING:
     from ._table_base import QBaseTable
 
 # https://ymt-lab.com/post/2020/pyqt5-qtableview-pandas-qabstractitemmodel/
 
 _READ_ONLY = Qt.ItemFlag.ItemIsEnabled | Qt.ItemFlag.ItemIsSelectable
@@ -36,19 +37,21 @@
         self._validator: dict[Hashable, Callable[[Any], None]] = {}
 
         self._data_role_map = {
             Qt.ItemDataRole.DisplayRole: self._data_display,
             Qt.ItemDataRole.EditRole: self._data_edit,
             Qt.ItemDataRole.TextColorRole: self._data_text_color,
             Qt.ItemDataRole.ToolTipRole: self._data_tooltip,
-            Qt.ItemDataRole.BackgroundColorRole: self._data_background_color,
+            Qt.ItemDataRole.BackgroundColorRole: self._data_background_color_rendered,
             Qt.ItemDataRole.DecorationRole: self._data_decoration,
+            Qt.ItemDataRole.SizeHintRole: self._data_size_hint,
         }
 
         self._decorations: TableMapping[tuple[QtGui.QPixmap, str]] = TableMapping()
+        self._background_color_anim = CellColorAnimation(self)
 
     @property
     def df(self) -> pd.DataFrame:
         return self._df
 
     def updateValue(self, r, c, val):
         # pandas warns but no problem
@@ -164,20 +167,43 @@
                     # since this method is called many times, errorous function should
                     # be deleted from the mapper.
                     self._background_colormap.pop(colname)
                     raise e
                 return QtGui.QColor(*rgba)
         return QtCore.QVariant()
 
+    def _data_background_color_rendered(self, index: QtCore.QModelIndex):
+        col = self._data_background_color(index)
+        anim = self._background_color_anim
+        if not anim.contains(index):
+            return col
+        return anim.get_brush(self._data_size_hint(index), anim.value, col)
+
     def _data_decoration(self, index: QtCore.QModelIndex):
         r, c = index.row(), index.column()
         if content := self._decorations.get((r, c), None):
             return content[0]
         return QtCore.QVariant()
 
+    def _data_size_hint(self, index: QtCore.QModelIndex):
+        r, c = index.row(), index.column()
+        tv = self.parent()._qtable_view
+        vsize = tv.verticalHeader()._section_sizes
+        hsize = tv.horizontalHeader()._section_sizes
+        if r < len(vsize):
+            lr = tv.verticalHeader()._section_sizes[r]
+        else:
+            lr = get_config().table.row_size
+        if c < len(hsize):
+            lc = tv.horizontalHeader()._section_sizes[c]
+        else:
+            lc = get_config().table.column_size
+        zoom = self.parent().zoom()
+        return QtCore.QSize(int(lc * zoom), int(lr * zoom))
+
     def set_cell_label(self, index: QtCore.QModelIndex, text: str | None):
         if text is None or text == "":
             self._decorations.pop((index.row(), index.column()), None)
         else:
             qlabel = QtW.QLabel(text, self.parent())
             qlabel.setStyleSheet("background-color: transparent; color: gray;")
             qlabel.setAlignment(Qt.AlignmentFlag.AlignCenter)
@@ -219,15 +245,15 @@
                     return self._column_tooltip(section)
                 return None
 
         if orientation == Qt.Orientation.Vertical:
             if role == Qt.ItemDataRole.DisplayRole:
                 if section >= self.df.index.size:
                     return None
-                text = str(self.df.index[section])
+                text = str(self.df.index[section]) + " "
                 return text
             elif role == Qt.ItemDataRole.ToolTipRole:
                 if section < self.df.index.size:
                     return str(self.df.index[section])
                 return None
 
     def _column_tooltip(self, section: int):
@@ -282,42 +308,62 @@
             self.beginRemoveColumns(parent, c0 + dc, c0 - 1)
             self.removeColumns(c0 + dc, -dc, parent)
             self.endRemoveColumns()
 
         return None
 
     def insertColumns(
-        self, column: int, count: int, parent: QtCore.QModelIndex = None
+        self,
+        column: int,
+        count: int,
+        parent: QtCore.QModelIndex = None,
+        span: int | Iterable[int] | None = None,
     ) -> bool:
         self._decorations.insert_columns(column, count)
-        span = self.data(self.index(0, column - 1), Qt.ItemDataRole.SizeHintRole)
-        if isinstance(span, QtCore.QSize):
-            span = cast(QtCore.QSize, span).width()
+        if span is None:
+            span = self.data(self.index(0, column - 1), Qt.ItemDataRole.SizeHintRole)
+            if isinstance(span, QtCore.QSize):
+                span = cast(QtCore.QSize, span).width()
+            else:
+                span = get_config().table.column_size
+        header = self.parent()._qtable_view.horizontalHeader()
+        if hasattr(span, "__iter__"):
+            for s, r in zip(span, range(column, column + count)):
+                header.insertSection(r, 1, s)
         else:
-            span = get_config().table.column_size
-        self.parent()._qtable_view.horizontalHeader().insertSection(column, count, span)
+            header.insertSection(column, count, span)
         return super().insertColumns(column, count, parent)
 
     def removeColumns(
         self, column: int, count: int, parent: QtCore.QModelIndex = None
     ) -> bool:
         self._decorations.remove_columns(column, count)
         self.parent()._qtable_view.horizontalHeader().removeSection(column, count)
         return super().removeColumns(column, count, parent)
 
     def insertRows(
-        self, row: int, count: int, parent: QtCore.QModelIndex = None
+        self,
+        row: int,
+        count: int,
+        parent: QtCore.QModelIndex = None,
+        span: int | Iterable[int] | None = None,
     ) -> bool:
         self._decorations.insert_rows(row, count)
-        span = self.data(self.index(0, row - 1), Qt.ItemDataRole.SizeHintRole)
-        if isinstance(span, QtCore.QSize):
-            span = cast(QtCore.QSize, span).height()
+        if span is None:
+            span = self.data(self.index(0, row - 1), Qt.ItemDataRole.SizeHintRole)
+            if isinstance(span, QtCore.QSize):
+                span = cast(QtCore.QSize, span).height()
+            else:
+                span = get_config().table.row_size
+        header = self.parent()._qtable_view.verticalHeader()
+        if hasattr(span, "__iter__"):
+            for s, r in zip(span, range(row, row + count)):
+                header.insertSection(r, 1, s)
         else:
-            span = get_config().table.row_size
-        self.parent()._qtable_view.verticalHeader().insertSection(row, count, span)
+            header.insertSection(row, count, span)
         return super().insertRows(row, count, parent)
 
     def removeRows(
         self, row: int, count: int, parent: QtCore.QModelIndex = None
     ) -> bool:
         self._decorations.remove_rows(row, count)
         self.parent()._qtable_view.verticalHeader().removeSection(row, count)
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_keycombo.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_keycombo.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_line_edit.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_line_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -562,18 +562,21 @@
             column_selected=column_selected,
         )
 
         if selop is None:  # out of bound
             return None
 
         # get string that represents the selection
-        if selop.area(_df_ori) > 1:
+        if selop.area(_df_ori) > 1 or column_selected:
             to_be_added = selop.fmt("df")
         else:
-            to_be_added = selop.resolve_indices(_df_ori, (1, 1)).fmt_scalar("df")
+            # NOTE: Selecting an entire column with a single cell is not allowed
+            # by fmt_scalar.
+            resolved = selop.resolve_indices(_df_ori, (1, 1))
+            to_be_added = resolved.fmt_scalar("df")
 
         # add the representation to the text at the proper position
         if cursor_pos == 0:
             self.setText(to_be_added + text)
         elif text[cursor_pos - 1] != "]":
             self.setText(text[:cursor_pos] + to_be_added + text[cursor_pos:])
         else:
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_object_holder.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_object_holder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
-from qtpy import QtWidgets as QtW, QtGui
-from qtpy.QtCore import Signal, Qt
+from qtpy import QtWidgets as QtW
 
 if TYPE_CHECKING:
     from ._overlay import QOverlayFrame
 
 # TODO:
 class QObjectHolder(QtW.QWidget):
     def __init__(self, parent: QtW.QWidget = None):
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_overlay.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_overlay.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from qtpy import QtWidgets as QtW, QtGui
 from qtpy.QtCore import Qt
 
 if TYPE_CHECKING:
-    from ..._table_stack import QTabbedTableStack
-    from .._base import QBaseTable
+    from tabulous._qt._table_stack import QTabbedTableStack
+    from tabulous._qt._table._base import QBaseTable
 
 
 class QOverlayFrame(QtW.QDialog):
     """The overlay frame widget used to display the overlaid widget in tables."""
 
     def __init__(
         self,
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_side_area.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_side_area.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_table_base.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_table_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     QCellLiteralEdit,
 )
 from tabulous._sort_filter_proxy import SortFilterProxy
 from tabulous._dtype import isna
 from tabulous._qt._undo import QtUndoManager, fmt_slice
 from tabulous._qt._svg import QColoredSVGIcon
 from tabulous._keymap import QtKeys, QtKeyMap
+from tabulous._utils import TabulousConfig
 from tabulous._qt._action_registry import QActionRegistry
 from tabulous.types import ProxyType, ItemInfo, HeaderInfo, EvalInfo
 from tabulous.exceptions import (
     SelectionRangeError,
     TableImmutableError,
     UnreachableError,
 )
@@ -122,15 +123,18 @@
 
     def needSave(self) -> bool:
         """Return True if the table is edited."""
         return self._edited
 
     def setOrientation(self, a0: Qt.Orientation) -> None:
         """Set table orientation and the side area orientation."""
-        a1 = 1 - a0  # opposite orientation
+        if a0 == Qt.Orientation.Horizontal:
+            a1 = Qt.Orientation.Vertical
+        else:
+            a1 = Qt.Orientation.Horizontal
         super().setOrientation(a0)
         if self._side_area is not None:
             self._side_area.setOrientation(a1)
         return None
 
     def createHandle(self) -> QTableHandle:
         """Create custom handle."""
@@ -219,14 +223,18 @@
     def dataShapeRaw(self) -> tuple[int, int]:
         return self.getDataFrame().shape
 
     def zoom(self) -> float:
         """Get current zoom factor."""
         return self._qtable_view.zoom()
 
+    def load_config(self, cfg: TabulousConfig | None = None):
+        """Load new config."""
+        return self._qtable_view.load_config(cfg)
+
     def setZoom(self, value: float) -> None:
         """Set zoom factor."""
         return self._qtable_view.setZoom(value)
 
     def itemDelegate(self) -> TableItemDelegate:
         return QtW.QTableView.itemDelegate(self._qtable_view)
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_table_group.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_table_group.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_base/_table_wrappers.py` & `tabulous-0.5.3/tabulous/_qt/_table/_base/_table_wrappers.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_display.py` & `tabulous-0.5.3/tabulous/_qt/_table/_display.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_groupby.py` & `tabulous-0.5.3/tabulous/_qt/_table/_groupby.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_spreadsheet.py` & `tabulous-0.5.3/tabulous/_qt/_table/_spreadsheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 import pandas as pd
 from qtpy import QtCore, QtGui
 from qtpy.QtCore import Qt
 
 from collections_undo import arguments
 
 from ._base import AbstractDataFrameModel, QMutableSimpleTable
+from ._animation import RowAnimation, ColumnAnimation
 from tabulous._dtype import get_converter, get_dtype, DTypeMap, DefaultValidator
+from tabulous._utils import TabulousConfig, get_config
 from tabulous.color import normalize_color
 from tabulous.types import ItemInfo
 from tabulous._text_formatter import DefaultFormatter
 from tabulous import _pd_index
 
 if TYPE_CHECKING:
     from magicgui.widgets._bases import ValueWidget
 
 # More rows/columns will be displayed
-_OUT_OF_BOUND_R = 60
-_OUT_OF_BOUND_C = 10
 _STRING_DTYPE = get_dtype("string")
 _EMPTY = object()
 _EXP_FLOAT = re.compile(r"[-+]?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)")
 
 
 class SpreadSheetModel(AbstractDataFrameModel):
     """A DataFrameModel for a spreadsheet."""
@@ -63,24 +63,18 @@
         return self._df
 
     @df.setter
     def df(self, data: pd.DataFrame):
         self._df = data
 
     def rowCount(self, parent=None):
-        return min(
-            self._df.shape[0] + _OUT_OF_BOUND_R,
-            self._table_config.max_row_count,
-        )
+        return self._table_config.max_row_count
 
     def columnCount(self, parent=None):
-        return min(
-            self._df.shape[1] + _OUT_OF_BOUND_C,
-            self._table_config.max_column_count,
-        )
+        return self._table_config.max_column_count
 
     def _data_display(self, index: QtCore.QModelIndex):
         """Display role."""
         r, c = index.row(), index.column()
         df = self.df
         if r < df.shape[0] and c < df.shape[1]:
             val = df.iat[r, c]
@@ -171,17 +165,41 @@
     is (almost) unbounded.
     """
 
     _DEFAULT_EDITABLE = True
     NaN = ""
 
     def __init__(self, parent=None, data: pd.DataFrame | None = None):
+        from tabulous._utils import get_config
+
+        cfg = get_config()
+
+        if data is not None:
+            if (
+                cfg.table.max_row_count < data.shape[0]
+                or cfg.table.max_column_count < data.shape[1]
+            ):
+                _max_size = (cfg.table.max_row_count, cfg.table.max_column_count)
+                raise ValueError(
+                    f"Input table data size {data.shape} exceeds the maximum "
+                    f"size {_max_size}."
+                )
+
         self._columns_dtype = DTypeMap()
         super().__init__(parent, data)
         self._qtable_view.verticalHeader().setMinimumWidth(20)
+        animate = cfg.window.animate
+        self._anim_row = RowAnimation(self).set_animate(animate)
+        self._anim_col = ColumnAnimation(self).set_animate(animate)
+
+        # initialize section spans
+        rspan, cspan = cfg.table.row_size, cfg.table.column_size
+        nr, nc = self._data_raw.shape
+        self._qtable_view.verticalHeader().insertSection(0, nr, rspan)
+        self._qtable_view.horizontalHeader().insertSection(0, nc, cspan)
 
     if TYPE_CHECKING:
 
         def model(self) -> SpreadSheetModel:
             ...
 
     def getDataFrame(self) -> pd.DataFrame:
@@ -248,29 +266,31 @@
         """Return the shown dataframe (consider filter)."""
         if parse:
             df = self.getDataFrame()
             return self._proxy.apply(df)
         else:
             return self.model().df
 
+    def load_config(self, cfg: TabulousConfig | None = None):
+        """Load new config."""
+        self._anim_row.set_animate(cfg.window.animate)
+        self._anim_col.set_animate(cfg.window.animate)
+        return super().load_config(cfg)
+
     @QMutableSimpleTable._mgr.interface
     def setDataFrame(self, data: pd.DataFrame) -> None:
         """Set data frame as a string table."""
         self._data_raw = data.astype(_STRING_DTYPE)
 
         # SpreadSheet columns should be str if possible. Convert it.
         if isinstance(self._data_raw.columns, pd.RangeIndex):
             self._data_raw.columns = _pd_index.char_arange(self._data_raw.columns.size)
         elif self._data_raw.columns.dtype.kind in "iuf":
             self._data_raw.columns = self._data_raw.columns.astype(str)
 
-        self.model().setShape(
-            data.index.size + _OUT_OF_BOUND_R,
-            data.columns.size + _OUT_OF_BOUND_C,
-        )
         self._data_cache = None
         self.setProxy(None)
         self.refreshTable()
         return
 
     def updateValue(self, r, c, val):
         index = self._data_raw.index[r]
@@ -317,20 +337,15 @@
             else:
                 to_assign[k] = v.astype(_STRING_DTYPE)
         old_value = self._data_raw
         self._data_raw: pd.DataFrame = self._data_raw.assign(**to_assign).drop(
             to_delete, axis=1, inplace=False
         )
 
-        nr, nc = self._data_raw.shape
         self.model().df = self._data_raw
-        self.model().setShape(
-            nr + _OUT_OF_BOUND_R,
-            nc + _OUT_OF_BOUND_C,
-        )
         self.setProxy(None)
         self.refreshTable()
         # NOTE: ItemInfo cannot have list indices.
         self.itemChangedSignal.emit(
             ItemInfo(
                 slice(None),
                 slice(None),
@@ -398,17 +413,14 @@
 
         with self._mgr.merging(formatter=lambda _: self._set_value_fmt(r, c, value)):
             if need_expand:
                 self.expandDataFrame(max(rmax - nr + 1, 0), max(cmax - nc + 1, 0))
             super().setDataFrameValue(r, c, value)
             self._set_proxy(self._proxy)
 
-        self._qtable_view.verticalHeader().resize(
-            self._qtable_view.verticalHeader().sizeHint()
-        )
         return None
 
     def setLabeledData(self, r: slice, c: slice, value: pd.Series):
         nr, nc = self._data_raw.shape
         rmax = _get_limit(r)
         cmax = _get_limit(c)
         need_expand = nr <= rmax or nc <= cmax
@@ -418,17 +430,14 @@
 
         with self._mgr.merging(formatter=lambda cmds: cmds[-2].format()):
             if need_expand:
                 self.expandDataFrame(max(rmax - nr + 1, 0), max(cmax - nc + 1, 0))
             super().setLabeledData(r, c, value)
             self._set_proxy(self._proxy)
 
-        self._qtable_view.verticalHeader().resize(
-            self._qtable_view.verticalHeader().sizeHint()
-        )
         return None
 
     def _pre_set_array(self, r: slice, c: slice, _value: pd.DataFrame):
         """Convert input dataframe for setting to data[r, c]."""
         if len(self.model()._validator) == 0:
             # use faster method if no validator is set
             out = self._data_raw.iloc[r, c].copy()
@@ -445,39 +454,40 @@
         return super()._pre_set_array(r, c, _value)
 
     @QMutableSimpleTable._mgr.undoable
     def expandDataFrame(self, nrows: int, ncols: int):
         """Expand the data frame by adding empty rows and columns."""
         if not self.isEditable():
             return None
+        nr, nc = self._data_raw.shape
         self._data_raw = _pad_dataframe(self._data_raw, nrows, ncols)
         if self._proxy.proxy_type != "none":
             self._set_proxy(self._proxy)  # need update!
-        new_shape = self._data_raw.shape
-        self.model().setShape(
-            new_shape[0] + _OUT_OF_BOUND_R,
-            new_shape[1] + _OUT_OF_BOUND_C,
-        )
+        cfg = get_config()
+
+        rspan, cspan = cfg.table.row_size, cfg.table.column_size
+        self._qtable_view.verticalHeader().insertSection(nr, nrows, rspan)
+        self._qtable_view.horizontalHeader().insertSection(nc, ncols, cspan)
         return None
 
     @expandDataFrame.undo_def
     def expandDataFrame(self, nrows: int, ncols: int):
         nr, nc = self._data_raw.shape
-        model = self.model()
         self._data_raw = self._data_raw.iloc[: nr - nrows, : nc - ncols]
-        model.setShape(
-            self._data_raw.shape[0] + _OUT_OF_BOUND_R,
-            self._data_raw.shape[1] + _OUT_OF_BOUND_C,
-        )
         self._set_proxy(self._proxy)
+
+        self._qtable_view.verticalHeader().removeSection(nr, nrows)
+        self._qtable_view.horizontalHeader().insertSection(nc, ncols)
         self._data_cache = None
         return None
 
     @QMutableSimpleTable._mgr.undoable
-    def insertRows(self, row: int, count: int, value: Any = _EMPTY):
+    def insertRows(
+        self, row: int, count: int, value: Any = _EMPTY, span: int | None = None
+    ):
         """Insert rows at the given row number and count."""
         if self._proxy.proxy_type != "none":
             raise NotImplementedError("Cannot insert rows during filtering/sorting.")
 
         index_existing = self._data_raw.index
 
         if value is _EMPTY:
@@ -505,52 +515,60 @@
                 value,
                 self._data_raw.iloc[row:, :],
             ],
             axis=0,
         )
         if _pd_index.is_ranged(index_existing):
             self._data_raw.index = pd.RangeIndex(0, self._data_raw.index.size)
-        self.model().insertRows(row, count, QtCore.QModelIndex())
-        self._set_proxy(self._proxy)
-        self._data_cache = None
-        self._edited = True
+        self.model().insertRows(row, count, QtCore.QModelIndex(), span=span)
 
-        # update indices
-        self._process_insert_rows(row, count)
+        @self._anim_row.connect
+        def _on_finish():
+            self._set_proxy(self._proxy)
+            self._data_cache = None
+            self._edited = True
 
-        info = ItemInfo(
-            slice(row, row + count),
-            slice(None),
-            value,
-            ItemInfo.INSERTED,
-        )
-        self._qtable_view.setZoom(self._qtable_view.zoom())
-        self.itemChangedSignal.emit(info)
-        return None
+            # update indices
+            self._process_insert_rows(row, count)
+
+            info = ItemInfo(
+                slice(row, row + count),
+                slice(None),
+                value,
+                ItemInfo.INSERTED,
+            )
+            self._qtable_view.setZoom(self._qtable_view.zoom())
+            self.itemChangedSignal.emit(info)
+
+        return self._anim_row.run_insert(row, count, span)
 
     @insertRows.undo_def
-    def insertRows(self, row: int, count: int, value: Any = _EMPTY):
+    def insertRows(self, row: int, count: int, value: Any = _EMPTY, span=None):
         """Insert rows at the given row number and count."""
         return self.removeRows(row, count)
 
     @insertRows.set_formatter
     def _insertRows_fmt(self, row: int, count: int, value: Any = _EMPTY):
         return f"table.index.insert(at={row}, count={count})"
 
-    def insertColumns(self, col: int, count: int, value: Any = _EMPTY):
+    def insertColumns(
+        self, col: int, count: int, value: Any = _EMPTY, span: int | None = None
+    ):
         """Insert columns at the given column number and count."""
         with self._mgr.merging(
             lambda cmds: f"table.columns.insert(at={col}, count={count})"
         ):
-            self._insert_columns(col, count, value)
+            self._insert_columns(col, count, value, span)
             self._process_header_widgets_on_insert(col, count)
         return None
 
     @QMutableSimpleTable._mgr.undoable
-    def _insert_columns(self, col: int, count: int, value: Any = _EMPTY):
+    def _insert_columns(
+        self, col: int, count: int, value: Any = _EMPTY, span: int | None = None
+    ):
         columns_existing = self._data_raw.columns
         _c_ranged = _pd_index.is_ranged(columns_existing)
 
         if value is _EMPTY:
             columns = _remove_duplicate(
                 _pd_index.char_arange(col, col + count), existing=columns_existing
             )
@@ -580,78 +598,91 @@
                 model._background_colormap,
                 model._text_formatter,
                 model._validator,
                 self._columns_dtype,
             ]:
                 _inserte_in_dict(d, col, count)
 
-        self.model().insertColumns(col, count, QtCore.QModelIndex())
-        self._data_cache = None
-        self._edited = True
+        self.model().insertColumns(col, count, QtCore.QModelIndex(), span=span)
 
-        # update indices
-        self._process_insert_columns(col, count)
+        @self._anim_col.connect
+        def _on_finish():
+            self._data_cache = None
+            self._edited = True
 
-        info = ItemInfo(
-            slice(None),
-            slice(col, col + count),
-            value,
-            ItemInfo.INSERTED,
-        )
-        self._qtable_view.setZoom(self._qtable_view.zoom())
-        self.itemChangedSignal.emit(info)
-        return None
+            # update indices
+            self._process_insert_columns(col, count)
+
+            info = ItemInfo(
+                slice(None),
+                slice(col, col + count),
+                value,
+                ItemInfo.INSERTED,
+            )
+            self._qtable_view.setZoom(self._qtable_view.zoom())
+            self.itemChangedSignal.emit(info)
+
+        return self._anim_col.run_insert(col, count, span)
 
     @_insert_columns.undo_def
-    def _insert_columns(self, col: int, count: int, value: Any = _EMPTY):
+    def _insert_columns(self, col: int, count: int, value: Any = _EMPTY, span=None):
         """Insert columns at the given column number and count."""
         self._remove_columns(col, count, self._data_raw.iloc[:, col : col + count])
         self._set_proxy(self._proxy)
         return None
 
     def removeRows(self, row: int, count: int):
         """Remove rows at the given row number and count."""
         df = self.model().df.iloc[row : row + count, :]
-
+        hheader = self._qtable_view.verticalHeader()
+        spans = hheader._section_sizes[row : row + count].copy()
         with self._mgr.merging(
             lambda cmds: f"table.index.remove(at={row}, count={count})"
         ):
             self._clear_incell_slots(
                 slice(row, row + count),
                 slice(0, self._data_raw.shape[1]),
             )
-            self._remove_rows(row, count, df)
+            self._remove_rows(row, count, df, spans)
         return None
 
     @QMutableSimpleTable._mgr.undoable
-    def _remove_rows(self, row: int, count: int, old_values: pd.DataFrame):
+    def _remove_rows(self, row: int, count: int, old_values: pd.DataFrame, spans=None):
         _r_ranged = isinstance(self._data_raw.index, pd.RangeIndex)
-        self._data_raw = pd.concat(
+        _new_data_raw = pd.concat(
             [self._data_raw.iloc[:row, :], self._data_raw.iloc[row + count :, :]],
             axis=0,
         )
         if _r_ranged:
-            self._data_raw.index = pd.RangeIndex(0, self._data_raw.index.size)
-        self.model().removeRows(row, count, QtCore.QModelIndex())
-        self._set_proxy(self._proxy)
-        self.setSelections([(slice(row, row + 1), slice(0, self._data_raw.shape[1]))])
-        self._data_cache = None
-        self._edited = True
+            _new_data_raw.index = pd.RangeIndex(0, _new_data_raw.index.size)
 
-        self._process_remove_rows(row, count)
-        info = ItemInfo(
-            slice(row, row + count), slice(None), ItemInfo.DELETED, old_values
-        )
-        self._qtable_view.setZoom(self._qtable_view.zoom())
-        self.itemChangedSignal.emit(info)
+        @self._anim_row.connect
+        def _on_finish():
+            self._data_raw = _new_data_raw
+            self.model().removeRows(row, count, QtCore.QModelIndex())
+            self._set_proxy(self._proxy)
+            self.setSelections(
+                [(slice(row, row + 1), slice(0, self._data_raw.shape[1]))]
+            )
+            self._data_cache = None
+            self._edited = True
+
+            self._process_remove_rows(row, count)
+            info = ItemInfo(
+                slice(row, row + count), slice(None), ItemInfo.DELETED, old_values
+            )
+            self._qtable_view.setZoom(self._qtable_view.zoom())
+            self.itemChangedSignal.emit(info)
+
+        self._anim_row.run_remove(row, count)
         return None
 
     @_remove_rows.undo_def
-    def _remove_rows(self, row: int, count: int, old_values: pd.DataFrame):
-        self.insertRows(row, count, old_values)
+    def _remove_rows(self, row: int, count: int, old_values: pd.DataFrame, spans=None):
+        self.insertRows(row, count, old_values, spans)
         self.setSelections([(slice(row, row + 1), slice(0, self._data_raw.shape[1]))])
         return None
 
     def removeColumns(self, column: int, count: int):
         """Remove columns at the given column number and count."""
         df = self.model().df.iloc[:, column : column + count]
         with self._mgr.merging(
@@ -659,61 +690,84 @@
         ):
             self._clear_incell_slots(
                 slice(0, self._data_raw.shape[0]),
                 slice(column, column + count),
             )
             self._process_header_widgets_on_remove(column, count)
             model = self.model()
+            hheader = self._qtable_view.horizontalHeader()
             for index in range(column, column + count):
                 colname = model.df.columns[index]
                 self.setForegroundColormap(colname, None)
                 self.setBackgroundColormap(colname, None)
                 self.setTextFormatter(colname, None)
                 self.setDataValidator(colname, None)
                 self.setColumnDtype(colname, None)
-            self._remove_columns(column, count, df)
-            self._set_proxy(self._proxy)
+            section_sizes = hheader._section_sizes[column : column + count].copy()
+            self._remove_columns(column, count, df, section_sizes)
         return None
 
     @QMutableSimpleTable._mgr.undoable
-    def _remove_columns(self, col: int, count: int, old_values: pd.DataFrame):
+    def _remove_columns(
+        self,
+        col: int,
+        count: int,
+        old_values: pd.DataFrame,
+        spans: np.ndarray | None = None,
+    ):
         _c_ranged = _pd_index.is_ranged(self._data_raw.columns)
-        self._data_raw = pd.concat(
+        _new_data_raw = pd.concat(
             [self._data_raw.iloc[:, :col], self._data_raw.iloc[:, col + count :]],
             axis=1,
         )
         if _c_ranged:
-            self._data_raw.columns = _pd_index.char_range_index(
-                self._data_raw.columns.size
+            _new_data_raw.columns = _pd_index.char_range_index(
+                _new_data_raw.columns.size
             )
             model = self.model()
             for d in [
                 model._foreground_colormap,
                 model._background_colormap,
                 model._text_formatter,
                 model._validator,
                 self._columns_dtype,
             ]:
                 _remove_in_dict(d, col, count)
-        self.model().removeColumns(col, count, QtCore.QModelIndex())
-        self.setSelections([(slice(0, self._data_raw.shape[0]), slice(col, col + 1))])
-        self._data_cache = None
-        self._edited = True
 
-        self._process_remove_columns(col, count)
-        info = ItemInfo(
-            slice(None), slice(col, col + count), ItemInfo.DELETED, old_values
-        )
-        self._qtable_view.setZoom(self._qtable_view.zoom())
-        self.itemChangedSignal.emit(info)
+        @self._anim_col.connect
+        def _on_finish():
+            self.model().removeColumns(col, count, QtCore.QModelIndex())
+            self._data_raw = _new_data_raw
+            self.setSelections(
+                [(slice(0, self._data_raw.shape[0]), slice(col, col + 1))]
+            )
+            self._data_cache = None
+            self._edited = True
+
+            self._process_remove_columns(col, count)
+            self._qtable_view.setZoom(self._qtable_view.zoom())
+            info = ItemInfo(
+                slice(None), slice(col, col + count), ItemInfo.DELETED, old_values
+            )
+            self.itemChangedSignal.emit(info)  # relay to the psygnal.Signal
+            self._set_proxy(self._proxy)
+            return
+
+        self._anim_col.run_remove(col, count)
         return None
 
     @_remove_columns.undo_def
-    def _remove_columns(self, col: int, count: int, old_values: pd.DataFrame):
-        self.insertColumns(col, count, old_values)
+    def _remove_columns(
+        self,
+        col: int,
+        count: int,
+        old_values: pd.DataFrame,
+        spans: np.ndarray | None = None,
+    ):
+        self.insertColumns(col, count, old_values, spans)
         self.setSelections([(slice(0, self._data_raw.shape[0]), slice(col, col + 1))])
         return None
 
     @QMutableSimpleTable._mgr.interface
     def _set_widget_at_index(self, r: int, c: int, widget: ValueWidget | None) -> None:
         index = self.model().index(r, c)
         if wdt := self._qtable_view.indexWidget(index):
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_table/_table.py` & `tabulous-0.5.3/tabulous/_qt/_table/_table.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table_stack/_eval.py` & `tabulous-0.5.3/tabulous/_qt/_table_stack/_eval.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
-import ast
 from qtpy import QtWidgets as QtW
-import pandas as pd
 from . import _utils
 
 
 class QAbstractEval(QtW.QWidget):
     _BUTTON_TEXT = ""
     _PLACEHOLDER_TEXT = ""
 
@@ -46,22 +44,15 @@
 
     def callback(self):
         """Evaluate the current text as a Python expression."""
         text = self._line.text()
         if text == "":
             return
         table = self._line.currentPyTable(assert_mutable=True)
-        df = table.data.eval(text, inplace=False, global_dict={"df": table.data})
-        parsed = ast.parse(text.replace("@", "")).body[0]
-        if type(parsed) is not ast.Assign:
-            self._line._qtable_viewer._table_viewer.add_table(df, name=table.name)
-        else:
-            name = parsed.targets[0].id
-            new_ds = df[name]
-            table.assign({name: new_ds})
+        table.query(text)
         self._line.toHistory()
 
 
 class QLiteralFilterWidget(QAbstractEval):
     """
     Apply filter using literal string.
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_table_stack/_finder.py` & `tabulous-0.5.3/tabulous/_qt/_table_stack/_finder.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table_stack/_overlay.py` & `tabulous-0.5.3/tabulous/_qt/_table_stack/_overlay.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table_stack/_start.py` & `tabulous-0.5.3/tabulous/_qt/_table_stack/_start.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table_stack/_tabbar.py` & `tabulous-0.5.3/tabulous/_qt/_table_stack/_tabbar.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_table_stack/_tabwidget.py` & `tabulous-0.5.3/tabulous/_qt/_table_stack/_tabwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
                 else:
                     toolbar._corner_widget.hide()
         self.addTab(table, name)
         table._qtable_view.resizedSignal.connect(self.resizedSignal.emit)
         table.selectionChangedSignal.connect(
             lambda: self.updateSelectionEdit(table.selections())
         )
+        table.setSelections([(slice(0, 1), slice(0, 1))])
         return None
 
     def takeTable(self, index: int) -> QBaseTable:
         """Remove table at `index` and return it."""
         table = self.tableAtIndex(index)
         self.untileTable(index)
         self.removeTab(index)
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_table_stack/_utils.py` & `tabulous-0.5.3/tabulous/_qt/_table_stack/_utils.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_titlebar.py` & `tabulous-0.5.3/tabulous/_qt/_titlebar.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_toolbar/_corner.py` & `tabulous-0.5.3/tabulous/_qt/_toolbar/_corner.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,15 @@
                 return super().event(event)
             if key == Qt.Key.Key_Up:
                 self.increment()
                 return True
             elif key == Qt.Key.Key_Down:
                 self.decrement()
                 return True
+
         return super().event(event)
 
     def wheelEvent(self, a0: QtGui.QWheelEvent) -> None:
         if a0.angleDelta().y() > 0:
             self.increment()
         else:
             self.decrement()
@@ -63,14 +64,15 @@
         metrics = QtGui.QFontMetrics(self.font())
         w = metrics.width("9") * len(text) + 6
         self.setFixedWidth(w)
 
 
 class QSelectionRangeEdit(QtW.QWidget):
     sliceChanged = Signal(object)
+    editingFinished = Signal()
 
     def __init__(self, parent: QtW.QWidget | None = None):
         super().__init__(parent)
         self.setLayout(QtW.QHBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
         inner = QtW.QWidget()
         self.layout().addWidget(inner)
@@ -96,14 +98,19 @@
         layout.addWidget(self._r_colon)
         layout.addWidget(self._r_stop)
         layout.addWidget(_label(", "))
         layout.addWidget(self._c_start)
         layout.addWidget(self._c_colon)
         layout.addWidget(self._c_stop)
 
+        self._r_start.editingFinished.connect(self.editingFinished.emit)
+        self._r_stop.editingFinished.connect(self.editingFinished.emit)
+        self._c_start.editingFinished.connect(self.editingFinished.emit)
+        self._c_stop.editingFinished.connect(self.editingFinished.emit)
+
     def slice(self) -> tuple[slice, slice]:
         rsl = slice(self._r_start.value(), self._r_stop.value())
         csl = slice(self._c_start.value(), self._c_stop.value())
         return rsl, csl
 
     def setSlice(self, sl: tuple[slice, slice]):
         rsl, csl = sl
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_toolbar/_toolbar_widget.py` & `tabulous-0.5.3/tabulous/_qt/_toolbar/_toolbar_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
     @property
     def _corner_widget(self) -> QSelectionRangeEdit:
         if self._tab.cornerWidget() is None:
             corner = QSelectionRangeEdit(self._tab)
             corner.sliceChanged.connect(self.sliceChanged.emit)
 
             self._tab.setCornerWidget(corner)
+            corner.editingFinished.connect(lambda: self.parent().setCellFocus())
             corner.hide()
         return self._tab.cornerWidget()
 
     @property
     def viewer(self) -> TableViewerBase:
         """The parent viewer object."""
         return self.parent()._table_viewer
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_toolbar/_toolbutton.py` & `tabulous-0.5.3/tabulous/_qt/_toolbar/_toolbutton.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_traceback.py` & `tabulous-0.5.3/tabulous/_qt/_traceback.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,15 @@
     """An message box widget for displaying Python exception."""
 
     def __init__(self, title: str, text_or_exception: str | Exception, parent):
         if isinstance(text_or_exception, str):
             text = text_or_exception
             exc = None
         else:
-            if len(text_or_exception.args) == 0:
-                text = ""
-            else:
-                text = text_or_exception.args[0]
+            text = str(text_or_exception)
             exc = text_or_exception
         MBox = QtW.QMessageBox
         super().__init__(
             MBox.Icon.Critical,
             str(title),
             str(text)[:1000],
             MBox.StandardButton.Ok | MBox.StandardButton.Help,
```

### Comparing `tabulous-0.5.2/tabulous/_qt/_tree_header.py` & `tabulous-0.5.3/tabulous/_qt/_tree_header.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_qt/_undo.py` & `tabulous-0.5.3/tabulous/_qt/_undo.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_range.py` & `tabulous-0.5.3/tabulous/_range.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,30 @@
         csl = self._csl
         rlower = rsl.start <= r if rsl.start is not None else True
         rupper = r < rsl.stop if rsl.stop is not None else True
         clower = csl.start <= c if csl.start is not None else True
         cupper = c < csl.stop if csl.stop is not None else True
         return rlower and rupper and clower and cupper
 
+    def intersection(self, other: RectRange) -> RectRange:
+        """Return the intersection of two ranges."""
+        r0_s, r1_s = self._rsl.start, self._rsl.stop
+        c0_s, c1_s = self._csl.start, self._csl.stop
+        r0_o, r1_o = other._rsl.start, other._rsl.stop
+        c0_o, c1_o = other._csl.start, other._csl.stop
+        r0 = _max(r0_s, r0_o)
+        r1 = _min(r1_s, r1_o)
+        if r0 >= r1:
+            return NoRange()
+        c0 = _max(c0_s, c0_o)
+        c1 = _min(c1_s, c1_o)
+        if c0 >= c1:
+            return NoRange()
+        return RectRange(slice(r0, r1), slice(c0, c1))
+
     def includes(self, other: RectRange) -> bool:
         if isinstance(other, MultiRectRange):
             return all(self.includes(rng) for rng in other)
 
         r0_s, r1_s = self._rsl.start, self._rsl.stop
         c0_s, c1_s = self._csl.start, self._csl.stop
         r0_o, r1_o = other._rsl.start, other._rsl.stop
@@ -188,24 +204,40 @@
         self._ranges = ranges
 
     @classmethod
     def from_slices(cls, slices: Iterable[tuple[slice, slice]]):
         """Construct from list of slices."""
         return cls([RectRange(rsl, csl) for rsl, csl in slices])
 
+    def with_slices(self, rsl: slice, csl: slice) -> MultiRectRange:
+        """Create a new MultiRectRange with the given slices added."""
+        return self.__class__(self._ranges + [RectRange(rsl, csl)])
+
+    def intersection(self, other: RectRange) -> MultiRectRange:
+        slices: list[RectRange] = []
+        for rng in self:
+            x = rng.intersection(other)
+            if isinstance(x, NoRange):
+                continue
+            slices.append(x)
+        return self.__class__(slices)
+
     def __repr__(self):
         s = ", ".join(repr(rng) for rng in self)
         return f"MultiRectRange[{s}]"
 
     def __contains__(self, other: tuple[int, int]):
         return any(other in rng for rng in self)
 
     def __iter__(self) -> Iterator[RectRange]:
         return iter(self._ranges)
 
+    def __getitem__(self, idx: int) -> RectRange:
+        return self._ranges[idx]
+
     def includes(self, other: RectRange) -> bool:
         if isinstance(other, MultiRectRange):
             return all(self.includes(rng) for rng in other)
         return any(rng.includes(other) for rng in self)
 
     def overlaps_with(self, other: RectRange) -> bool:
         if isinstance(other, MultiRectRange):
@@ -278,14 +310,26 @@
             return False
         else:
             return r1_o <= r1_s
     else:
         return True
 
 
+def _max(a, b):
+    if _le(a, b):
+        return b
+    return a
+
+
+def _min(a, b):
+    if _le(a, b):
+        return a
+    return b
+
+
 INF = float("inf")
 
 
 def _overlap_1d(
     r0_s: int | None, r1_s: int | None, r0_o: int | None, r1_o: int | None
 ) -> bool:
     if r0_s is None:
```

### Comparing `tabulous-0.5.2/tabulous/_selection_model.py` & `tabulous-0.5.3/tabulous/_selection_model.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_selection_op.py` & `tabulous-0.5.3/tabulous/_selection_op.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,19 +246,19 @@
         rsel, csel = self.args
         return f"{df_expr}.iloc[{_fmt_slice(rsel)}, {_fmt_slice(csel)}]"
 
     def fmt_scalar(self, df_expr: str = "df") -> str:
         rsel, csel = self.args
         if isinstance(rsel, slice):
             if _has_none(rsel) or rsel.start != rsel.stop - 1:
-                raise ValueError("Cannot format as a scalar value.")
+                raise ValueError(f"Cannot format {(rsel, csel)} as a scalar value.")
             rsel = rsel.start
         if isinstance(csel, slice):
             if _has_none(csel) or csel.start != csel.stop - 1:
-                raise ValueError("Cannot format as a scalar value.")
+                raise ValueError(f"Cannot format {(rsel, csel)} as a scalar value.")
             csel = csel.start
         return f"{df_expr}.iloc[{_fmt_slice(rsel)}, {_fmt_slice(csel)}]"
 
     def operate(self, df: pd.DataFrame) -> pd.DataFrame | pd.Series:
         rsel, csel = self.args
         return df.iloc[rsel, csel]
```

### Comparing `tabulous-0.5.2/tabulous/_sort_filter_proxy.py` & `tabulous-0.5.3/tabulous/_sort_filter_proxy.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_text_formatter.py` & `tabulous-0.5.3/tabulous/_text_formatter.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/_utils.py` & `tabulous-0.5.3/tabulous/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 from types import MappingProxyType
-from typing import Any
+from typing import Any, TYPE_CHECKING
 from dataclasses import asdict, dataclass, field
 from functools import wraps
 from pathlib import Path
 from contextlib import contextmanager
 from appdirs import user_config_dir
 
+if TYPE_CHECKING:
+    KeyBinding = dict[str, str | list[str]]
 
 TXT_PATH = Path(user_config_dir("tabulous", "tabulous", "history.txt"))
 CONFIG_PATH = Path(user_config_dir("tabulous", "tabulous", "config.toml"))
 CELL_NAMESPACE_PATH = Path(user_config_dir("tabulous", "tabulous", "cell_namespace.py"))
 POST_INIT_PATH = Path(user_config_dir("tabulous", "tabulous", "post_init.py"))
 
 
@@ -115,25 +117,53 @@
         if isinstance(var, TableInitializer):
             table_initializer.join(var)
         elif isinstance(var, ViewerInitializer):
             viewer_initializer.join(var)
     return viewer_initializer, table_initializer
 
 
-def prep_default_keybindings() -> dict[str, str | list[str]]:
+def prep_default_keybindings() -> KeyBinding:
     from tabulous.commands import DEFAULT_KEYBINDING_SETTING
 
     kb = {}
     for cmd, seq in DEFAULT_KEYBINDING_SETTING:
         mod = cmd.__module__.split(".")[-1]
         name = cmd.__name__
         kb[f"{mod}.{name}"] = seq
     return kb
 
 
+def set_default_keybindings(kb: KeyBinding) -> KeyBinding:
+    from tabulous.commands import DEFAULT_KEYBINDING_SETTING
+
+    existing = set()
+    for seq in kb.values():
+        if isinstance(seq, str):
+            existing.add(seq)
+        elif isinstance(seq, list):
+            existing.update(seq)
+        else:
+            raise RuntimeError(f"Invalid keybinding sequence: {seq}")
+
+    for cmd, seq in DEFAULT_KEYBINDING_SETTING:
+        if isinstance(seq, str):
+            if seq not in existing:
+                mod = cmd.__module__.split(".")[-1]
+                name = cmd.__name__
+                kb[f"{mod}.{name}"] = seq
+
+        else:
+            if not existing.intersection(seq):
+                mod = cmd.__module__.split(".")[-1]
+                name = cmd.__name__
+                kb[f"{mod}.{name}"] = seq
+
+    return kb
+
+
 @dataclass
 class ConsoleNamespace:
     """Default namespace of the console."""
 
     tabulous: str = "tbl"
     viewer: str = "viewer"
     pandas: str = "pd"
@@ -167,28 +197,27 @@
 
     ask_on_close: bool = True
     show_console: bool = False
     theme: str = "light-blue"
     notify_latest: bool = True
     selection_editor: bool = True
     nonmain_style: bool = False
+    animate: bool = True
     title_bar: str = "native"
 
 
 @dataclass
 class TabulousConfig:
     """The config model."""
 
     console_namespace: ConsoleNamespace = field(default_factory=ConsoleNamespace)
     table: Table = field(default_factory=Table)
     cell: Cell = field(default_factory=Cell)
     window: Window = field(default_factory=Window)
-    keybindings: dict[str, str | list[str]] = field(
-        default_factory=prep_default_keybindings
-    )
+    keybindings: KeyBinding = field(default_factory=prep_default_keybindings)
 
     @classmethod
     def from_toml(cls, path: Path = CONFIG_PATH) -> TabulousConfig:
         """Load the config file."""
         import toml
 
         if not path.exists():
@@ -200,16 +229,15 @@
 
     @classmethod
     def from_dict(cls, dict_: dict[str, Any]) -> TabulousConfig:
         console_namespace = dict_.get("console_namespace", {})
         table = dict_.get("table", {})
         cell = dict_.get("cell", {})
         window = dict_.get("window", {})
-        if not (kb := dict_.get("keybindings", {})):
-            kb = prep_default_keybindings()
+        kb = set_default_keybindings(dict_.get("keybindings", {}))
         return cls(
             ConsoleNamespace(**_as_fields(console_namespace, ConsoleNamespace)),
             Table(**_as_fields(table, Table)),
             Cell(**_as_fields(cell, Cell)),
             Window(**_as_fields(window, Window)),
             kb,
         )
```

### Comparing `tabulous-0.5.2/tabulous/color.py` & `tabulous-0.5.3/tabulous/color.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/__init__.py` & `tabulous-0.5.3/tabulous/commands/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     (table.new_spreadsheet, "Ctrl+N"),
     (table.show_finder_widget, "Ctrl+F"),
     (table.show_undo_stack_view, "Ctrl+H"),
     (table.undo_table, "Ctrl+Z"),
     (table.redo_table, "Ctrl+Y"),
     (table.zoom_in, "Ctrl+Shift+>"),
     (table.zoom_out, "Ctrl+Shift+<"),
+    (table.jump_to_cell, "Ctrl+G"),
     (file.open_table, "Ctrl+O"),
     (file.open_spreadsheet, "Ctrl+K, Ctrl+O"),
     (file.save_table, "Ctrl+S"),
     (file.save_table_to_source, "Ctrl+Shift+S"),
     (selection.show_context_menu, "Menu"),
     (selection.raise_slot_error, "F6"),
     (selection.copy_data_tab_separated, "Ctrl+C"),
```

### Comparing `tabulous-0.5.2/tabulous/commands/_arange.py` & `tabulous-0.5.3/tabulous/commands/_arange.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_dialogs.py` & `tabulous-0.5.3/tabulous/commands/_dialogs.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_optimizer.py` & `tabulous-0.5.3/tabulous/commands/_optimizer.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_plot_models.py` & `tabulous-0.5.3/tabulous/commands/_plot_models.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_random_data.py` & `tabulous-0.5.3/tabulous/commands/_random_data.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_regression.py` & `tabulous-0.5.3/tabulous/commands/_regression.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_sklearn/_models.py` & `tabulous-0.5.3/tabulous/commands/_sklearn/_models.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_sklearn/_widget.py` & `tabulous-0.5.3/tabulous/commands/_sklearn/_widget.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_stats/_distribution.py` & `tabulous-0.5.3/tabulous/commands/_stats/_distribution.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_stats/_latex.py` & `tabulous-0.5.3/tabulous/commands/_stats/_latex.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_stats/_statstest.py` & `tabulous-0.5.3/tabulous/commands/_stats/_statstest.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_stats/_widgets.py` & `tabulous-0.5.3/tabulous/commands/_stats/_widgets.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/_utils.py` & `tabulous-0.5.3/tabulous/commands/_utils.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/analysis.py` & `tabulous-0.5.3/tabulous/commands/analysis.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/column.py` & `tabulous-0.5.3/tabulous/commands/column.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/file.py` & `tabulous-0.5.3/tabulous/commands/file.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/plot.py` & `tabulous-0.5.3/tabulous/commands/plot.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/selection.py` & `tabulous-0.5.3/tabulous/commands/selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,72 +264,72 @@
         if formatting:
             sheet._set_default_text_formatter(colname)
     return None
 
 
 def insert_row_above(viewer: TableViewerBase):
     """Insert a row above"""
-    sheet = _utils.get_spreadsheet(viewer)._qwidget
-    if not sheet.isEditable():
+    sheet = _utils.get_spreadsheet(viewer)
+    if not sheet.editable:
         return _notify_editability()
-    row, _ = sheet._qtable_view._selection_model.current_index
-    return sheet.insertRows(row, 1)
+    row, _ = sheet.current_index
+    return sheet.native.insertRows(row, 1)
 
 
 def insert_row_below(viewer: TableViewerBase):
     """Insert a row below"""
-    sheet = _utils.get_spreadsheet(viewer)._qwidget
-    if not sheet.isEditable():
+    sheet = _utils.get_spreadsheet(viewer)
+    if not sheet.editable:
         return _notify_editability()
-    row, _ = sheet._qtable_view._selection_model.current_index
-    return sheet.insertRows(row + 1, 1)
+    row, _ = sheet.current_index
+    return sheet.native.insertRows(row + 1, 1)
 
 
 def insert_column_left(viewer: TableViewerBase):
     """Insert a column left"""
-    sheet = _utils.get_spreadsheet(viewer)._qwidget
-    if not sheet.isEditable():
+    sheet = _utils.get_spreadsheet(viewer)
+    if not sheet.editable:
         return _notify_editability()
-    _, col = sheet._qtable_view._selection_model.current_index
-    return sheet.insertColumns(col, 1)
+    _, col = sheet.current_index
+    return sheet.native.insertColumns(col, 1)
 
 
 def insert_column_right(viewer: TableViewerBase):
     """Insert a column right"""
-    sheet = _utils.get_spreadsheet(viewer)._qwidget
-    if not sheet.isEditable():
+    sheet = _utils.get_spreadsheet(viewer)
+    if not sheet.editable:
         return _notify_editability()
-    _, col = sheet._qtable_view._selection_model.current_index
-    return sheet.insertColumns(col + 1, 1)
+    _, col = sheet.current_index
+    return sheet.native.insertColumns(col + 1, 1)
 
 
 def remove_selected_rows(viewer: TableViewerBase):
     """Remove selected rows"""
-    sheet = _utils.get_spreadsheet(viewer)._qwidget
-    if not sheet.isEditable():
+    sheet = _utils.get_spreadsheet(viewer)
+    if not sheet.editable:
         return _notify_editability()
-    row, col = sheet._qtable_view._selection_model.current_index
-    _, rng = sheet._qtable_view._selection_model.range_under_index(row, col)
+    row, col = sheet.current_index
+    _, rng = sheet.native._qtable_view._selection_model.range_under_index(row, col)
     if rng is not None:
         row_range = rng[0]
-        sheet.removeRows(row_range.start, row_range.stop - row_range.start)
+        sheet.native.removeRows(row_range.start, row_range.stop - row_range.start)
         return None
     raise ValueError("No selection under cursor.")
 
 
 def remove_selected_columns(viewer: TableViewerBase):
     """Remove selected columns"""
-    sheet = _utils.get_spreadsheet(viewer)._qwidget
-    if not sheet.isEditable():
+    sheet = _utils.get_spreadsheet(viewer)
+    if not sheet.editable:
         return _notify_editability()
-    row, col = sheet._qtable_view._selection_model.current_index
-    _, rng = sheet._qtable_view._selection_model.range_under_index(row, col)
+    row, col = sheet.current_index
+    _, rng = sheet.native._qtable_view._selection_model.range_under_index(row, col)
     if rng is not None:
         col_range = rng[1]
-        sheet.removeColumns(col_range.start, col_range.stop - col_range.start)
+        sheet.native.removeColumns(col_range.start, col_range.stop - col_range.start)
         return None
     raise ValueError("No selection under cursor.")
 
 
 def write_data_signal_in_console(viewer: TableViewerBase):
     """Write data signal connection to console"""
     from qtpy import QtCore
```

### Comparing `tabulous-0.5.2/tabulous/commands/tab.py` & `tabulous-0.5.3/tabulous/commands/tab.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/table.py` & `tabulous-0.5.3/tabulous/commands/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     from tabulous.widgets import TableViewerBase, TableBase, SpreadSheet
     from ._arange import _RangeDialog
 
 
 def new_spreadsheet(viewer: TableViewerBase):
     """Add an empty spreadsheet."""
     viewer.add_spreadsheet()
+    viewer.native.setCellFocus()
 
 
 def copy_as_table(viewer: TableViewerBase):
     """Copy current table as a new table"""
     table = _utils.get_table(viewer)
     out = viewer.add_table(table.data, name=f"{table.name}-copy")
     out._source = Source.from_table(table)
@@ -310,7 +311,17 @@
     table.native._qtable_view.zoomIn(1)
 
 
 def zoom_out(viewer: TableViewerBase):
     """Zoom in"""
     table = _utils.get_table(viewer)
     table.native._qtable_view.zoomIn(-1)
+
+
+def jump_to_cell(viewer: TableViewerBase):
+    """Jump to a cell."""
+    from tabulous._qt._jump import QJumpWidget
+
+    if viewer.current_table is None:
+        return
+    jw = QJumpWidget(viewer.native)
+    jw.show()
```

### Comparing `tabulous-0.5.2/tabulous/commands/view.py` & `tabulous-0.5.3/tabulous/commands/view.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/commands/window.py` & `tabulous-0.5.3/tabulous/commands/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def show_keymap(viewer: TableViewerBase):
     """Show key map widget"""
     viewer._qwidget.showKeyMap()
 
 
 def close_window(viewer: TableViewerBase):
     """Close window"""
-    viewer._qwidget.close()
+    viewer._qwidget.close(ask=None)
 
 
 def new_window(viewer: TableViewerBase):
     """Create a new window"""
     new = viewer.__class__()
     pos = viewer._qwidget.pos()
     pos.setX(pos.x() + 20)
```

### Comparing `tabulous-0.5.2/tabulous/core.py` & `tabulous-0.5.3/tabulous/core.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/exceptions.py` & `tabulous-0.5.3/tabulous/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/post_init.py` & `tabulous-0.5.3/tabulous/post_init.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/style/_style.py` & `tabulous-0.5.3/tabulous/style/_style.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/style/_style.qss` & `tabulous-0.5.3/tabulous/style/_style.qss`

 * *Files 1% similar despite different names*

```diff
@@ -536,14 +536,28 @@
 }
 
 QOverlayFrame {
     border: 1px solid #[highlight0];
     background-color: #[background];
 }
 
+QJumpWidget {
+    border: 1px solid #[highlight0];
+    border-radius: 5px;
+    background-color: #[background];
+}
+
+QJumpWidget > QWidget {
+    font-size: 16px;
+}
+
+QJumpWidget > QWidget > QWidget {
+    font-size: 18px;
+}
+
 QCornerButtons {
     background-color: #[background0];
 }
 
 QCornerButtons > QToolButton {
     background-color: #[background0];
     border-radius: 4px;
```

### Comparing `tabulous-0.5.2/tabulous/style/defaults.json` & `tabulous-0.5.3/tabulous/style/defaults.json`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/threading.py` & `tabulous-0.5.3/tabulous/threading.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/types.py` & `tabulous-0.5.3/tabulous/types.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/__init__.py` & `tabulous-0.5.3/tabulous/widgets/_component/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/_base.py` & `tabulous-0.5.3/tabulous/widgets/_component/_base.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/_cell.py` & `tabulous-0.5.3/tabulous/widgets/_component/_cell.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/_column_setting.py` & `tabulous-0.5.3/tabulous/widgets/_component/_column_setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,17 @@
     def _get_dict(self) -> dict[str, _F]:
         """Get dict of colormaps."""
 
     @abstractmethod
     def _set_value(self, key: str, func: _F):
         """Set colormap at key."""
 
+    def _ipython_key_completions_(self):
+        return list(self.parent.columns)
+
     def __getitem__(self, key: str) -> _F:
         return self._get_dict()[key]
 
     def __setitem__(self, key: str, func: _F) -> None:
         self.set(key, func)
         return None
 
@@ -349,14 +352,17 @@
 
 class ColumnDtypeInterface(Component["SpreadSheet"], MutableMapping[str, "_DtypeLike"]):
     """Interface to the column dtype of spreadsheet."""
 
     def _get_dtype_map(self):
         return self.parent._qwidget._columns_dtype
 
+    def _ipython_key_completions_(self):
+        return list(self.parent.columns)
+
     def __getitem__(self, key: str) -> _DtypeLike | None:
         """Get the dtype of the given column name."""
         return self._get_dtype_map().get(key, None)
 
     def __setitem__(self, key: str, dtype: Any) -> None:
         """Set a dtype to the given column name."""
         return self.parent._qwidget.setColumnDtype(key, dtype)
```

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/_header.py` & `tabulous-0.5.3/tabulous/widgets/_component/_header.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,14 +40,22 @@
                     raise ValueError("Size mismatch between destination and spans.")
                 [header.resizeSection(idx, sp) for idx, sp in zip(index, span)]
             else:
                 [header.resizeSection(idx, span) for idx in index]
         else:
             header.resizeSection(index, span)
 
+    def __iter__(self) -> Iterator[int]:
+        return iter(int(a) for a in self.parent._get_header()._section_sizes)
+
+    def __eq__(self, other: Any) -> bool:
+        return np.all(
+            self.parent._get_header()._section_sizes.astype(np.uint16) == other
+        )
+
     def resize_to_content(self):
         from qtpy.QtWidgets import QHeaderView
 
         header = self.parent._get_header()
         header.resizeSections(QHeaderView.ResizeMode.ResizeToContents)
         return None
 
@@ -206,23 +214,25 @@
 
     def _set_value(self, idx: int, val: Any):
         return self.parent._qwidget.setVerticalHeaderValue(idx, val)
 
     def _get_header(self) -> QDataFrameHeaderView:
         return self.parent._qwidget._qtable_view.verticalHeader()
 
-    def insert(self, at: int, count: int):
+    def insert(self, at: int, count: int = 1):
         """Insert `count` rows at the given position."""
         sheet = self._assert_spreadsheet()
-        sheet._qwidget.insertRows(at, count)
+        with sheet._qwidget._anim_row.using_animation(False):
+            sheet._qwidget.insertRows(at, count)
 
-    def remove(self, at: int, count: int):
+    def remove(self, at: int, count: int = 1):
         """Remove `count` rows at the given position."""
         sheet = self._assert_spreadsheet()
-        sheet._qwidget.removeRows(at, count)
+        with sheet._qwidget._anim_row.using_animation(False):
+            sheet._qwidget.removeRows(at, count)
 
     @_HeaderInterface.selected.setter
     def selected(self, slices: int | slice | list[int | slice]):
         """Set the selected ranges."""
         if isinstance(slices, (int, slice)):
             slices = [slices]
         smodel = self.parent._qwidget._qtable_view._selection_model
@@ -244,23 +254,25 @@
 
     def _set_value(self, idx: int, val: Any):
         return self.parent._qwidget.setHorizontalHeaderValue(idx, val)
 
     def _get_header(self) -> QDataFrameHeaderView:
         return self.parent._qwidget._qtable_view.horizontalHeader()
 
-    def insert(self, at: int, count: int):
+    def insert(self, at: int, count: int = 1):
         """Insert `count` columns at the given position."""
         sheet = self._assert_spreadsheet()
-        sheet._qwidget.insertColumns(at, count)
+        with sheet._qwidget._anim_col.using_animation(False):
+            sheet._qwidget.insertColumns(at, count)
 
-    def remove(self, at: int, count: int):
+    def remove(self, at: int, count: int = 1):
         """Remove `count` columns at the given position."""
         sheet = self._assert_spreadsheet()
-        sheet._qwidget.removeColumns(at, count)
+        with sheet._qwidget._anim_col.using_animation(False):
+            sheet._qwidget.removeColumns(at, count)
 
     @_HeaderInterface.selected.setter
     def selected(self, slices: int | slice | list[int | slice]):
         """Set the selected ranges."""
         if isinstance(slices, (int, slice)):
             slices = [slices]
         smodel = self.parent._qwidget._qtable_view._selection_model
```

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/_keymap.py` & `tabulous-0.5.3/tabulous/widgets/_component/_keymap.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/_plot.py` & `tabulous-0.5.3/tabulous/widgets/_component/_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,24 @@
 
     def gcw(self):
         """Get current widget."""
         if self._current_widget is None or isdeleted(self._current_widget):
             self.new_widget()
         return self._current_widget
 
+    def clf(self):
+        """Clear the current figure."""
+        self.gcf().clf()
+        return self.draw()
+
+    def cla(self):
+        """Clear the current axis."""
+        self.gca().cla()
+        return self.draw()
+
     def new_widget(self, nrows: int = 1, ncols: int = 1, style: str | None = None):
         """Create a new plot widget and add it to the table."""
         from tabulous._qt._plot import QtMplPlotCanvas
 
         table = self.parent
         qviewer = table._qwidget._qtable_view.parentViewer()
```

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/_proxy.py` & `tabulous-0.5.3/tabulous/widgets/_component/_proxy.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/_ranges.py` & `tabulous-0.5.3/tabulous/widgets/_component/_ranges.py`

 * *Files 15% similar despite different names*

```diff
@@ -105,15 +105,29 @@
     """A table data specific selection range list."""
 
     def _get_list(self):
         return list(self.parent._qwidget.selections())
 
     def update(self, value: SelectionRanges):
         """Update the selection ranges."""
-        return self.parent._qwidget.setSelections(value)
+        self.parent._qwidget.setSelections(value)
+        sels = self.parent._qwidget.selections()
+        if len(sels) > 0:
+            # update current index
+            rsl, csl = sels[-1]
+            if (
+                rsl.stop is not None
+                and rsl.start is not None
+                and (rsl.stop - rsl.start) == 1
+                and csl.stop is not None
+                and csl.start is not None
+                and (csl.stop - csl.start) == 1
+            ):
+                _smodel = self.parent._qwidget._qtable_view._selection_model
+                _smodel.current_index = (rsl.start, csl.start)
 
 
 class HighlightRanges(_TableRanges):
     """A table data specific highlight list."""
 
     def _get_list(self):
         return list(self.parent._qwidget.highlights())
```

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/_table_subset.py` & `tabulous-0.5.3/tabulous/widgets/_component/_table_subset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Sequence, TypeVar, Union, overload, Callable
+from typing import TYPE_CHECKING, Any, Sequence, TypeVar, Union, overload, Callable
 
 import numpy as np
 from tabulous.exceptions import TableImmutableError
 
 from tabulous.types import ColorMapping
 from ._base import TableComponent
 from ._column_setting import _Void
@@ -117,51 +117,61 @@
             return TableSeries(table, rkey, table.columns[ckey])
         elif isinstance(ckey, (slice, Sequence)):
             return TableSubset(table, rkey, list(table.columns[ckey]))
         else:
             raise TypeError(f"Cannot iloc-slice by {type(ckey)}")
 
 
-class TableSubset(TableComponent):
-    """Object representing a subset of a Table widget."""
-
-    def __init__(
-        self, parent: TableBase, row_slice: slice | list[int], columns: list[str]
-    ):
-        super().__init__(parent)
-        self._row_slice = row_slice
-        self._columns = columns
+class DataProperty:
+    """Internal subset data of the table."""
 
-    @property
-    def data(self) -> pd.DataFrame:
-        """Data of the subset as a pandas DataFrame."""
-        table = self.parent
-        return table.native._get_sub_frame(self._columns).iloc[self._row_slice]
-
-    @data.setter
-    def data(self, val) -> None:
+    def __get__(self, instance: TableSubset, owner) -> pd.DataFrame:
+        if instance is None:
+            raise AttributeError("Cannot access property without instance.")
+        table = instance.parent
+        return table.native._get_sub_frame(instance._columns).iloc[instance._row_slice]
+
+    def __set__(self, instance: TableSubset, val: Any):
+        if instance is None:
+            raise AttributeError("Cannot access property without instance.")
         import pandas as pd
 
-        table = self.parent
+        table = instance.parent
         if not table.mutable:
             raise TableImmutableError(f"Cannot set data on {type(table)}")
         table: Table | SpreadSheet
-        df = table.native._get_sub_frame(self._columns)
+        df = table.native._get_sub_frame(instance._columns)
         to_assign = {}
         if not isinstance(val, pd.DataFrame):
             val = pd.DataFrame(val, columns=df.columns)
         for k, v in df.items():
-            v.values[self._row_slice] = val[k]
+            v.values[instance._row_slice] = val[k]
             to_assign[k] = v
         table.assign(to_assign)
         return None
 
+
+class TableSubset(TableComponent):
+    """Object representing a subset of a Table widget."""
+
+    def __init__(
+        self, parent: TableBase, row_slice: slice | list[int], columns: list[str]
+    ):
+        super().__init__(parent)
+        self._row_slice = row_slice
+        self._columns = columns
+
+    data = DataProperty()
+
     def __repr__(self) -> str:
         return f"<TableSubset of {self.parent!r}> with data:\n{self.data!r}"
 
+    def _ipython_key_completions_(self):
+        return self._columns
+
 
 class TableSeries(TableComponent):
     """Object representing a column series of a Table widget."""
 
     def __init__(self, parent: TableBase, row_slice: slice | list[int], column: str):
         super().__init__(parent)
         self._row_slice = row_slice
@@ -297,20 +307,23 @@
 
 
 class _PartialColormapInterface(_PartialInterface):
     def _get_field(self) -> _ColormapInterface:
         raise NotImplementedError()
 
     def invert(self):
+        """Invert the colormap of the column."""
         return self._get_field().invert(self._column)
 
     def set_opacity(self, opacity: float):
+        """Set the opacity of the colormap of the column."""
         return self._get_field().set_opacity(self._column, opacity)
 
     def adjust_brightness(self, factor: float):
+        """Change the brightness of the colormap of the column."""
         return self._get_field().adjust_brightness(self._column, factor)
 
     def set(
         self,
         colormap: ColorMapping = _Void,
         *,
         interp_from: _Interpolatable | None = None,
```

### Comparing `tabulous-0.5.2/tabulous/widgets/_component/_viewer.py` & `tabulous-0.5.3/tabulous/widgets/_component/_viewer.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_doc.py` & `tabulous-0.5.3/tabulous/widgets/_doc.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_magicgui.py` & `tabulous-0.5.3/tabulous/widgets/_magicgui.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_mainwindow.py` & `tabulous-0.5.3/tabulous/widgets/_mainwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractproperty
 from functools import partial
 from pathlib import Path
 from types import MappingProxyType
 import warnings
 import weakref
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable, Union
+from typing import TYPE_CHECKING, Any, Callable, Generic, Union, TypeVar
 from psygnal import Signal, SignalGroup
 from superqt.utils import thread_worker
 
 from ._table import Table, SpreadSheet, GroupBy, TableDisplay
 from ._tablelist import TableList
 from ._sample import open_sample
 from ._component import Toolbar, Console, CommandPalette
@@ -31,14 +31,15 @@
     from tabulous._qt._mainwindow._namespace import Namespace
     from qtpy.QtWidgets import QWidget
     from magicgui.widgets import Widget
     import numpy as np
     import pandas as pd
 
 PathLike = Union[str, Path, bytes]
+_T = TypeVar("_T")
 
 
 class TableType(Enum):
     table = "table"
     spreadsheet = "spreadsheet"
 
 
@@ -95,14 +96,31 @@
     ) -> None:
         """Paste from clipboard."""
         if selections is not None:
             self.current_table.selections = selections
         return self.current_table._qwidget.pasteFromClipBoard()
 
 
+class IPyProperty(Generic[_T]):
+    """
+    Essentially identical to the getter-only property.
+
+    IPython runtime auto-completion checks if the evaluation has any side effects.
+    If an attribute is a property, it immediately skips the auto-completion check.
+    """
+
+    def __init__(self, fget: Callable[[Any], _T]):
+        self.fget = fget
+
+    def __get__(self, instance, owner=None) -> _T:
+        if instance is None:
+            raise AttributeError("Can only be accessed via an instance.")
+        return self.fget(instance)
+
+
 class TableViewerBase(_AbstractViewer, SupportKeyMap):
     """The base class of a table viewer widget."""
 
     events: TableViewerSignal
     _qwidget_class: type[_QtMainWidgetBase]
 
     toolbar = Toolbar()
@@ -133,20 +151,15 @@
 
         if show:
             self.show(run=False)
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__} widget at {hex(id(self))}>"
 
-    @property
-    def tables(self) -> TableList:
-        """Return the table list object."""
-        return self._tablist
-
-    @property
+    @IPyProperty
     def current_table(self) -> TableBase | None:
         """Return the currently visible table."""
         if len(self.tables) > 0:
             return self.tables[self.current_index]
         return None
 
     @property
@@ -161,14 +174,19 @@
     def current_index(self, index: int | str):
         if isinstance(index, str):
             index = self.tables.index(index)
         elif index < 0:
             index += len(self.tables)
         return self._qwidget._tablestack.setCurrentIndex(index)
 
+    @IPyProperty
+    def tables(self) -> TableList:
+        """Return the table list object."""
+        return self._tablist
+
     @property
     def native(self) -> _QtMainWidgetBase:
         """Return the native widget."""
         return self._qwidget
 
     @property
     def cell_namespace(self) -> Namespace:
@@ -325,27 +343,33 @@
         TableDisplay
             A table display object.
         """
         table = TableDisplay(loader, name=name, metadata=metadata)
         return self.add_layer(table, update=update)
 
     def add_layer(self, input: TableBase, *, update: bool = False):
+        """Add any table object to the viewer."""
+        if table := self.current_table:
+            table_has_focus = table.native._qtable_view.hasFocus()
+        else:
+            table_has_focus = False
         if (
             update
             and (table := self.tables.get(input.name, None))
             and type(table) is type(input)
         ):
             table.data = input.data
             return table
         self.tables.append(input)
         self.current_index = -1  # activate the last table
 
-        self._qwidget.setCellFocus()
         if self._table_initializer is not None:
             self._table_initializer.initialize_table(input)
+        if table_has_focus:
+            self._qwidget.setCellFocus()
         return input
 
     def open(self, path: PathLike, *, type: TableType | str = TableType.table) -> None:
         """
         Read a table data and add to the viewer.
 
         Parameters
@@ -491,15 +515,15 @@
     @size.setter
     def size(self, size: tuple[int, int]):
         """Set the size of the table viewer."""
         w, h = size
         return self._qwidget.resize(int(w), int(h))
 
     def _link_events(self):
-        _tablist = self._tablist
+        _tablist = self.tables
         _qtablist = self._qwidget._tablestack
 
         @_tablist.events.inserted.connect
         def _insert_qtable(i: int):
             table = _tablist[i]
             _qtablist.addTable(table._qwidget, table.name)
 
@@ -526,25 +550,25 @@
                 _qtablist.renameTable(index, name)
 
         @_qtablist.itemMoved.connect
         def _move_pytable(src: int, dst: int):
             """Move evented list when list is moved in GUI."""
             if src < dst:
                 dst += 1
-            with self._tablist.events.blocked():
-                self._tablist.move(src, dst)
+            with self.tables.events.blocked():
+                self.tables.move(src, dst)
 
         @_qtablist.tableRenamed.connect
         def _rename_pytable(index: int, name: str):
-            self._tablist.rename(index, name)
+            self.tables.rename(index, name)
 
         @_qtablist.tableRemoved.connect
         def _remove_pytable(index: int):
-            with self._tablist.events.blocked():
-                del self._tablist[index]
+            with self.tables.events.blocked():
+                del self.tables[index]
 
         @_qtablist.tablePassed.connect
         def _pass_pytable(src, index: int, dst):
             src_ = _find_parent_table(src)
             dst_ = _find_parent_table(dst)
             dst_.tables.append(src_.tables.pop(index))
```

### Comparing `tabulous-0.5.2/tabulous/widgets/_registry.py` & `tabulous-0.5.3/tabulous/widgets/_registry.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_sample.py` & `tabulous-0.5.3/tabulous/widgets/_sample.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_source.py` & `tabulous-0.5.3/tabulous/widgets/_source.py`

 * *Files identical despite different names*

### Comparing `tabulous-0.5.2/tabulous/widgets/_table.py` & `tabulous-0.5.3/tabulous/widgets/_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import logging
 from abc import abstractmethod, abstractstaticmethod
+import ast
 from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, Hashable, TYPE_CHECKING, overload
 import warnings
 import weakref
 from psygnal import SignalGroup, Signal
 
@@ -76,14 +77,50 @@
         return super().__eq__(other)
 
     def __repr__(self) -> str:
         return f"<{type(self).__name__}.{self.name}>"
 
 
 # #####################################################################
+#   Property-like
+# #####################################################################
+
+
+class DataProperty:
+    """Internal data of the table."""
+
+    def __get__(self, instance: TableBase, owner) -> pd.DataFrame:
+        if instance is None:
+            raise AttributeError("Cannot access property without instance.")
+        return instance._qwidget.getDataFrame()
+
+    def __set__(self, instance: TableBase, value: Any):
+        if instance is None:
+            raise AttributeError("Cannot access property without instance.")
+        _data = instance._normalize_data(value)
+        instance._qwidget.setDataFrame(_data)
+
+
+class MetadataProperty:
+    """Metadata dictionary of the table."""
+
+    def __get__(self, instance: TableBase, owner) -> dict[str, Any]:
+        if instance is None:
+            raise AttributeError("Cannot access property without instance.")
+        return instance._metadata
+
+    def __set__(self, instance: TableBase, value: dict[str, Any]):
+        if instance is None:
+            raise AttributeError("Cannot access property without instance.")
+        if not isinstance(value, dict):
+            raise TypeError("metadata must be a dict")
+        instance._metadata = value
+
+
+# #####################################################################
 #   The abstract base class of tables.
 # #####################################################################
 
 
 class TableBase(SupportKeyMap):
     """The base class for a table layer."""
 
@@ -142,14 +179,17 @@
             )
 
             self.events.evaluated.connect(self._emit_evaluated)
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}<{self.name!r}>"
 
+    def _ipython_key_completions_(self):
+        return [name for name in self.columns]
+
     # fmt: off
     @overload
     def __getitem__(self, key: str) -> _comp.TableSeries: ...
     @overload
     def __getitem__(self, key: list[str]) -> _comp.TableSubset: ...
     # fmt: on
 
@@ -169,14 +209,24 @@
         return self.cell.ref
 
     @property
     def source(self) -> Source:
         """The source of the table."""
         return self._source
 
+    @property
+    def current_index(self) -> tuple[int, int]:
+        """The current index of the table."""
+        return self._qwidget._qtable_view._selection_model.current_index
+
+    @current_index.setter
+    def current_index(self, index: tuple[int, int]) -> None:
+        r, c = index
+        return self.move_iloc(r, c)
+
     def _emit_data_changed_signal(self, info: ItemInfo) -> None:
         r, c = info.row, info.column
         if info.value is info.DELETED or info.old_value is info.INSERTED:
             # insertion/deletion emits signal from the next row/column.
             _is_deleted = info.value is info.DELETED
             if r == slice(None):
                 # column is deleted/inserted
@@ -212,24 +262,15 @@
         """Data normalization before setting a new data."""
 
     @property
     def table_type(self) -> str:
         """Return the table type in string."""
         return type(self).__name__
 
-    @property
-    def data(self) -> pd.DataFrame:
-        """Table data."""
-        return self._qwidget.getDataFrame()
-
-    @data.setter
-    def data(self, value: Any):
-        """Set table data."""
-        _data = self._normalize_data(value)
-        self._qwidget.setDataFrame(_data)
+    data = DataProperty()
 
     @property
     def data_shown(self) -> pd.DataFrame:
         """Return the data shown in the table (filter considered)."""
         return self._qwidget.dataShown(parse=True)
 
     @property
@@ -252,14 +293,16 @@
     @metadata.setter
     def metadata(self, value: dict[str, Any]) -> None:
         """Set metadata of the table."""
         if not isinstance(value, dict):
             raise TypeError("metadata must be a dict")
         self._metadata = value
 
+    metadata = MetadataProperty()
+
     @property
     def zoom(self) -> float:
         """Zoom factor of table."""
         return self._qwidget.zoom()
 
     @zoom.setter
     def zoom(self, value: float):
@@ -664,14 +707,28 @@
             serieses: dict[str, pd.Series] = {}
             for k, v in kwargs.items():
                 serieses[str(k)] = pd.Series(v, index=self.data.index, name=k)
 
             self._qwidget.assignColumns(serieses)
         return self
 
+    def query(self, text: str):
+        df = self.data.eval(text, inplace=False, global_dict={"df": self.data})
+        parsed = ast.parse(text.replace("@", "")).body[0]
+        if type(parsed) is not ast.Assign:
+            self._qwidget.parentViewer()._table_viewer.add_table(df, name=self.name)
+        else:
+            obj = parsed.targets[0]
+            if type(obj) is not ast.Name:
+                raise ValueError("Only simple assignment is supported.")
+            name = obj.id
+            new_ds = df[name]
+            self.assign({name: new_ds})
+        return None
+
 
 @_doc.update_doc
 class Table(_DataFrameTableLayer):
     """
     A table implemented with type checking.
 
     Parameters
```

### Comparing `tabulous-0.5.2/tabulous/widgets/_tablelist.py` & `tabulous-0.5.3/tabulous/widgets/_tablelist.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,17 @@
         return self._parent
 
     @property
     def _qcontextmenu(self):
         """The QContextMenu widget."""
         return self.parent.native._tablestack._qt_context_menu
 
+    def _ipython_key_completions_(self):
+        return [table.name for table in self]
+
     def insert(self, index: int, table: TableBase):
         """Insert a table at index `index`."""
         if not isinstance(table, TableBase):
             raise TypeError(
                 f"Cannot insert {type(table)} to {self.__class__.__name__}."
             )
```

