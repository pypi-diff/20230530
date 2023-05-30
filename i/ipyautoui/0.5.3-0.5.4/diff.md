# Comparing `tmp/ipyautoui-0.5.3.tar.gz` & `tmp/ipyautoui-0.5.4.tar.gz`

## Comparing `ipyautoui-0.5.3.tar` & `ipyautoui-0.5.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/_dev_sys_path_append.py
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/_utils.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/_utils_debounce.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/_version.py
--rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autodisplay.py
--rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autodisplay_renderers.py
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autoipywidget.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/automapschema-0.yaml
--rw-r--r--   0        0        0    21750 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/automapschema.py
--rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autoui.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autovjsf.py
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/autowidgets.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/basemodel.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/constants.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/env.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/mydocstring_display.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/test_schema.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/vjsf.vue
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/__init__.py
--rw-r--r--   0        0        0    40894 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/autogrid.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/buttonbars.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/decision_branch.py
--rw-r--r--   0        0        0    25263 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/editgrid.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/filechooser.py
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/filesindir.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/fileupload.py
--rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/iterable.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/loadproject.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/markdown_widget.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/modelrun.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/multiselect_search.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/outputlogging.py
--rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/selectdir.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/showhide.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/showopenurl.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/title_description.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/urlimagelink.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/widgetcaller_error.py
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/custom/workingdir.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/complex_serialization.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/core_ipywidgets.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/editable_datagrid.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nested.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/override_ipywidgets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_array.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_array_enum.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_enum.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_simple.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/src/ipyautoui/demo_schemas/ruleset.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/LICENSE
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/README.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/_dev_sys_path_append.py
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/_utils.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/_utils_debounce.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/_version.py
+-rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autodisplay.py
+-rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autodisplay_renderers.py
+-rw-r--r--   0        0        0    29199 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autoipywidget.py
+-rw-r--r--   0        0        0    21750 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/automapschema.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/automapschema.yaml
+-rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autoui.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autovjsf.py
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/autowidgets.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/basemodel.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/constants.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/env.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/mydocstring_display.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/test_schema.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/vjsf.vue
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/__init__.py
+-rw-r--r--   0        0        0    41006 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/autogrid.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/buttonbars.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/decision_branch.py
+-rw-r--r--   0        0        0    25595 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/editgrid.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/filechooser.py
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/filesindir.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/fileupload.py
+-rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/iterable.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/loadproject.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/markdown_widget.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/modelrun.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/multiselect_search.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/outputlogging.py
+-rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/selectdir.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/showhide.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/showopenurl.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/title_description.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/urlimagelink.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/widgetcaller_error.py
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/custom/workingdir.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/complex_serialization.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/core_ipywidgets.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/editable_datagrid.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nested.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/override_ipywidgets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_array.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_array_enum.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_enum.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_simple.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/src/ipyautoui/demo_schemas/ruleset.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/LICENSE
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/README.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.4/PKG-INFO
```

### Comparing `ipyautoui-0.5.3/src/ipyautoui/__init__.py` & `ipyautoui-0.5.4/src/ipyautoui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/_dev_sys_path_append.py` & `ipyautoui-0.5.4/src/ipyautoui/_dev_sys_path_append.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/_utils.py` & `ipyautoui-0.5.4/src/ipyautoui/_utils.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/_utils_debounce.py` & `ipyautoui-0.5.4/src/ipyautoui/_utils_debounce.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/autodisplay.py` & `ipyautoui-0.5.4/src/ipyautoui/autodisplay.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/autodisplay_renderers.py` & `ipyautoui-0.5.4/src/ipyautoui/autodisplay_renderers.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/autoipywidget.py` & `ipyautoui-0.5.4/src/ipyautoui/autoipywidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,40 +132,47 @@
             return caller
         else:
             return caller
     else:
         raise ValueError(f"ERROR add_fdir_to_widgetcallers self.fdir = {fdir}")
 
 
-def horizontal_row_nested(widget, label, auto_open=False):
+SPACER = w.HBox(layout={"width": "45px"})
+
+
+def horizontal_row_nested(widget, label, auto_open=False, contains_nullable=False):
     # BUG: Reported defects -@jovyan at 8/23/2022, 10:30:52 PM
     # ^ buggy behaviour associated to ShowHide class for nested objects observed in
     # example form linked to `horizontal_row_nested`
-    return ShowHide(
+    wi = ShowHide(
         fn_display=lambda: widget,
         title=label,
         auto_open=auto_open,
         button_width="300px",
     )
+    if contains_nullable:
+        return w.HBox([SPACER, wi])
+    else:
+        return wi
 
 
 def add_spacer_to_form_with_nullables(children, widget, contains_nullable):
     if contains_nullable and not isinstance(widget, Nullable):
-        children = [w.HBox(layout={"width": "45px"})] + children
+        children = [SPACER] + children
     return children
 
 
 def horizontal_row_simple(widget, label, contains_nullable=False):
     children = [widget, w.HTML(label)]
     children = add_spacer_to_form_with_nullables(children, widget, contains_nullable)
     return w.HBox(children)
 
 
 def vertical_row(widget, label, auto_open=None, contains_nullable=False):
-    children = [w.HBox(layout={"width": "40px"}), widget]
+    children = [SPACER, widget]
     children = add_spacer_to_form_with_nullables(children, widget, contains_nullable)
     return w.VBox(
         [
             w.HTML(label),
             w.HBox(children),
         ]
     )
@@ -191,15 +198,15 @@
     Returns:
         _type_: a widget box that is added to the list of children in AutoObject
     """
     if nested_widgets is None:
         nested_widgets = []
     if align_horizontal:
         if True in [isinstance(widget, w) for w in nested_widgets]:
-            return horizontal_row_nested(widget, label, auto_open=auto_open)
+            return horizontal_row_nested(widget, label, auto_open=auto_open, contains_nullable=contains_nullable)
         else:
             return horizontal_row_simple(
                 widget, label, contains_nullable=contains_nullable
             )
     else:
         return vertical_row(widget, label, contains_nullable=contains_nullable)
 
@@ -319,15 +326,14 @@
         return self.savebuttonbar.fns_onsave
 
     @tr.default("fns_onrevert")
     def _default_fns_onrevert(self):
         return self.savebuttonbar.fns_onsave
 
     def __init__(self, **kwargs):
-
         self._init_form()
         self._init_bn_showraw_controls()
         super().__init__(
             layout=w.Layout(
                 width="100%",
                 display="flex",
                 flex="flex-grow",
@@ -390,14 +396,15 @@
         return '{"test": "json"}'
 
 
 if __name__ == "__main__":
     ui = AutoObjectFormLayout(description="description", show_savebuttonbar=True)
     display(ui)
 
+
 # +
 def demo_autoobject_form(title="test", description="a description of the title"):
     """for docs and testing only..."""
     from ipyautoui.custom.buttonbars import SaveButtonBar
 
     form = AutoObjectFormLayout()
     form.title = make_bold(title)
@@ -765,15 +772,18 @@
         #       -@jovyan at 7/18/2022, 12:45:48 PMsavebuttonbar
 
     def _update_widgets_from_value(self):
         for k, v in self.value.items():
             if k in self.di_widgets.keys():
                 if v is None and not isinstance(self.di_widgets[k], Nullable):
                     v = _get_value_trait(self.di_widgets[k]).default()
-                self.di_widgets[k].value = v
+                try:
+                    self.di_widgets[k].value = v
+                except tr.TraitError as err:
+                    logging.warning(err)
             else:
                 logging.critical(
                     f"no widget created for {k}, with value {str(v)}. fix this in the schema!"
                 )
 
     @property
     def di_widgets_value(self):
```

### Comparing `ipyautoui-0.5.3/src/ipyautoui/automapschema-0.yaml` & `ipyautoui-0.5.4/src/ipyautoui/automapschema.yaml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/automapschema.py` & `ipyautoui-0.5.4/src/ipyautoui/automapschema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/autoui.py` & `ipyautoui-0.5.4/src/ipyautoui/autoui.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/autovjsf.py` & `ipyautoui-0.5.4/src/ipyautoui/autovjsf.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/autowidgets.py` & `ipyautoui-0.5.4/src/ipyautoui/autowidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/basemodel.py` & `ipyautoui-0.5.4/src/ipyautoui/basemodel.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/constants.py` & `ipyautoui-0.5.4/src/ipyautoui/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,24 @@
 BUTTON_WIDTH_MEDIUM = "90px"
 BUTTON_HEIGHT_MIN = "25px"
 ROW_WIDTH_MEDIUM = "120px"
 ROW_WIDTH_MIN = "60px"
 BUTTON_MIN_SIZE = frozenmap(width=BUTTON_WIDTH_MIN, height=BUTTON_HEIGHT_MIN)
 # ---------------------------
 
+MAGIC_BUTTON_KWARGS = frozenmap(
+    {
+        "disabled": False,
+        "layout": {"width": "44px"},
+        "button_style": "warning",
+        "icon": "magic",
+        "style": {},
+        "tooltip": "add many",
+    }
+)
 TRUE_BUTTON_KWARGS = frozenmap(
     icon="check",
     style={"button_color": "lightgreen"},
     # button_style="success",
     tooltip="true",
     layout={"width": BUTTON_WIDTH_MIN, "height": BUTTON_HEIGHT_MIN},
     disabled=True,
```

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo.py` & `ipyautoui-0.5.4/src/ipyautoui/demo.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/env.py` & `ipyautoui-0.5.4/src/ipyautoui/env.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/mydocstring_display.py` & `ipyautoui-0.5.4/src/ipyautoui/mydocstring_display.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/test_schema.py` & `ipyautoui-0.5.4/src/ipyautoui/test_schema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/vjsf.vue` & `ipyautoui-0.5.4/src/ipyautoui/vjsf.vue`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/autogrid.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/autogrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,14 +229,18 @@
         {
             setattr(self, k, v)
             for k, v in self.schema.items()
             if k not in ignore_schema_keys
         }
         self.default_row = self._get_default_row()
 
+    @property
+    def types(self):
+        return {k: v["type"] for k, v in self.schema["items"]["properties"].items()}
+
     def set_renderers(self, **kwargs):
         {
             setattr(self, k, v)
             for k, v in get_global_renderers_from_schema(self.schema, **kwargs).items()
         }
         # ^ sets: ["default_renderer", "header_renderer", "corner_renderer"]
         self.renderers = get_column_renderers_from_schema(
@@ -1152,21 +1156,14 @@
 
     grid = AutoGrid(schema=TestDataFrame, by_title=True)
     display(grid)
 
 # +
 
 
-
-
-
-
-
-
-
 if __name__ == "__main__":
     grid.data = pd.DataFrame(grid.data.to_dict(orient="records") * 4)  # .T
 
 if __name__ == "__main__":
     print(grid.is_transposed)
 
 if __name__ == "__main__":
@@ -1223,9 +1220,7 @@
 
 if __name__ == "__main__":
     grid.transposed = False
 
 if __name__ == "__main__":
     grid.set_item_value(0, {"string": "check", "integer": 2, "floater": 3.0})
 # -
-
-
```

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/buttonbars.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/buttonbars.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/decision_branch.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/decision_branch.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/editgrid.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/editgrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -662,14 +662,27 @@
 
 if __name__ == "__main__":
     editgrid.grid.order = ("floater", "string")
     # ^ NOTE: this will result in a value change in the grid
 
 
 if __name__ == "__main__":
+    # list column
+    class TestListCol(BaseModel):
+        li_col: list[str] = ["a"]
+        stringy: str = "as"
+        num: int = 1
+
+    class Test(BaseModel):
+        __root__: list[TestListCol]
+
+    gr = EditGrid(Test, value=[{"li_col": ["a", "b"], "stringy": "string", "num": 23}])
+    display(gr)
+
+if __name__ == "__main__":
     import random
 
     datahandler = DataHandler(
         fn_get_all_data=lambda: AUTO_GRID_DEFAULT_VALUE * random.randint(1, 5),
         fn_post=lambda v: print(v),
         fn_patch=lambda v: v,
         fn_delete=lambda v: print(v),
```

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/filechooser.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/filechooser.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/filesindir.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/filesindir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/fileupload.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/fileupload.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/iterable.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/iterable.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/loadproject.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/loadproject.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/markdown_widget.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/markdown_widget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/modelrun.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/modelrun.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/multiselect_search.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/multiselect_search.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/outputlogging.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/outputlogging.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/selectdir.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/selectdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/showhide.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/showhide.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/showopenurl.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/showopenurl.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/title_description.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/title_description.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/urlimagelink.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/urlimagelink.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/widgetcaller_error.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/widgetcaller_error.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/custom/workingdir.py` & `ipyautoui-0.5.4/src/ipyautoui/custom/workingdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/__init__.py` & `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/complex_serialization.py` & `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/complex_serialization.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/core_ipywidgets.py` & `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/editable_datagrid.py` & `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nested.py` & `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nested.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nested_editable_datagrid.py` & `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nested_editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py` & `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_array_enum.py` & `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_array_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/root_enum.py` & `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/root_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/src/ipyautoui/demo_schemas/ruleset.py` & `ipyautoui-0.5.4/src/ipyautoui/demo_schemas/ruleset.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/.gitignore` & `ipyautoui-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/LICENSE` & `ipyautoui-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/README.md` & `ipyautoui-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/pyproject.toml` & `ipyautoui-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.3/PKG-INFO` & `ipyautoui-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyautoui
-Version: 0.5.3
+Version: 0.5.4
 Summary: wrapper that sits on top of ipywidgets and other ipy widget libraries to template / automate the creation of widget forms. Uses pydantic to create defined data-container and serialisation to JSON. Includes example patterns for adding new custom widgets.
 Project-URL: Homepage, https://github.com/maxfordham/ipyautoui
 Author-email: John Gunstone <gunstone.john@gmail.com>
 License-File: LICENSE
 Keywords: ipyautoui
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

