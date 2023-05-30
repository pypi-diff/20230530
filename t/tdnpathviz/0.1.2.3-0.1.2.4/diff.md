# Comparing `tmp/tdnpathviz-0.1.2.3-py3-none-any.whl.zip` & `tmp/tdnpathviz-0.1.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 378773 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-24 07:40 tdnpathviz/__init__.py
+Zip file size: 378847 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-30 10:02 tdnpathviz/__init__.py
 -rw-rw-rw-  2.0 fat      991 b- defN 23-Jan-02 15:29 tdnpathviz/datasets.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-02 15:29 tdnpathviz/utils.py
--rw-rw-rw-  2.0 fat    10360 b- defN 23-May-15 08:26 tdnpathviz/visualizations.py
+-rw-rw-rw-  2.0 fat    10688 b- defN 23-May-30 10:01 tdnpathviz/visualizations.py
 -rw-rw-rw-  2.0 fat  2179525 b- defN 23-Jan-02 15:29 tdnpathviz/data/train_dataset.csv
--rw-rw-rw-  2.0 fat      266 b- defN 23-May-24 08:19 tdnpathviz-0.1.2.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-24 08:19 tdnpathviz-0.1.2.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-May-24 08:19 tdnpathviz-0.1.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      724 b- defN 23-May-24 08:19 tdnpathviz-0.1.2.3.dist-info/RECORD
-9 files, 2191992 bytes uncompressed, 377523 bytes compressed:  82.8%
+-rw-rw-rw-  2.0 fat      266 b- defN 23-May-30 10:07 tdnpathviz-0.1.2.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 10:07 tdnpathviz-0.1.2.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-30 10:07 tdnpathviz-0.1.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      724 b- defN 23-May-30 10:07 tdnpathviz-0.1.2.4.dist-info/RECORD
+9 files, 2192320 bytes uncompressed, 377597 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tdnpathviz/visualizations.py
 Comment: 
 
 Filename: tdnpathviz/data/train_dataset.csv
 Comment: 
 
-Filename: tdnpathviz-0.1.2.3.dist-info/METADATA
+Filename: tdnpathviz-0.1.2.4.dist-info/METADATA
 Comment: 
 
-Filename: tdnpathviz-0.1.2.3.dist-info/WHEEL
+Filename: tdnpathviz-0.1.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: tdnpathviz-0.1.2.3.dist-info/top_level.txt
+Filename: tdnpathviz-0.1.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: tdnpathviz-0.1.2.3.dist-info/RECORD
+Filename: tdnpathviz-0.1.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdnpathviz/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.2.3'
+__version__ = '0.1.2.4'
```

## tdnpathviz/visualizations.py

```diff
@@ -42,24 +42,28 @@
         # Construct the RGBA string and append it to the ret list
         ret.append("rgba(" + str(r) + "," + str(g) + "," + str(b) + "," + str(alpha) + ")")
 
     return ret  # Return the list of generated colors
 
 
 
-def plot_first_main_paths(myPathAnalysis, path_column='mypath', id_column='travelid', nb_paths=15, print_query=False):
+def plot_first_main_paths(myPathAnalysis, path_column='mypath', id_column='travelid', nb_paths=15, print_query=False,
+                          font_size=10, width=1200, height=800):
     """
         Plots the first main paths based on a given output of the teradataml NPATH function or the teradataml dataframe of its result field.
 
         Parameters:
         - myPathAnalysis (DataFrame or tdml.dataframe.dataframe.DataFrame): The input DataFrame containing path analysis data.
         - path_column (str, optional): The column name representing the path. Defaults to 'mypath'.
         - id_column (str or list, optional): The column name(s) representing the unique identifier(s). Defaults to 'travelid'.
         - nb_paths (int, optional): The number of main paths to plot. Defaults to 15.
         - print_query (bool, optional): Whether to print the generated query. Defaults to False.
+        - font_size (int, optional): define the size of the font. Defaults is 10.
+        - width (int, optional): define the width of the figure. Defaults is 1200.
+        - height (int, optional): define the height of the figure. Defaults is 800.
 
         Returns:
         - None (it display an interactive Sankey plot)
     """
     if type(id_column) != list:
         id_column = [id_column]
 
@@ -157,16 +161,16 @@
         link=dict(
             source=df_ready_local.node_source.map(labs),  # indices correspond to labels, eg A1, A2, A2, B1, ...
             target=df_ready_local.node_target.map(labs),
             value=df_ready_local.weight,
             color=df_ready_local.color
         ))])
 
-    fig.update_layout(font_size=10, width=1200,
-                      height=800)
+    fig.update_layout(font_size=font_size, width=width,
+                      height=height)
     fig.show()
 
     return
 
 def create_all_pathes_views(myPathAnalysis, root_name = 'mytest',
                             schema = tdml.get_context().execute('SELECT DATABASE').fetchall()[0][0],
                             path_column='mypath', id_column='travelid'):
```

## Comparing `tdnpathviz-0.1.2.3.dist-info/RECORD` & `tdnpathviz-0.1.2.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tdnpathviz/__init__.py,sha256=-NliaY9zSZZpZVslDvE3vpgy_hnikvd6AkiNMRCDglk,23
+tdnpathviz/__init__.py,sha256=WT5wGPSnxktTfYvr3q-CjYVlUh8VZivoykAhfsaVaDk,23
 tdnpathviz/datasets.py,sha256=XASLSjLtaHMZq-uPArgCLjbGapxDI2CJ2i0gSu9KW8M,991
 tdnpathviz/utils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tdnpathviz/visualizations.py,sha256=be7Rrep0av1O4lFffiRs5q6tkohZlg1aCIsrPqie1R8,10360
+tdnpathviz/visualizations.py,sha256=udc_JsTMNYJIlfM2JT5jDEGUV_ZOyr_nSpEYWWN5HZQ,10688
 tdnpathviz/data/train_dataset.csv,sha256=ko9f4sY4Cglvfii921mOnb01gAqP_EOhgKe12UdX9Pg,2179525
-tdnpathviz-0.1.2.3.dist-info/METADATA,sha256=dYDV2iX_t_AMhxcSo_VDkxF5UXMWNBcnx-pWes7CLNM,266
-tdnpathviz-0.1.2.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-tdnpathviz-0.1.2.3.dist-info/top_level.txt,sha256=zQpyBz_y48B-516T0jpkRU5MQcz1GLgaLohQ2iJTT_c,11
-tdnpathviz-0.1.2.3.dist-info/RECORD,,
+tdnpathviz-0.1.2.4.dist-info/METADATA,sha256=SrI6cBzQetcl-v1OjOg9Ox0tw87HXDXkK8REWZywtuw,266
+tdnpathviz-0.1.2.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+tdnpathviz-0.1.2.4.dist-info/top_level.txt,sha256=zQpyBz_y48B-516T0jpkRU5MQcz1GLgaLohQ2iJTT_c,11
+tdnpathviz-0.1.2.4.dist-info/RECORD,,
```

