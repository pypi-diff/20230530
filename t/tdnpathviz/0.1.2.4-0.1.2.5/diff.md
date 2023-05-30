# Comparing `tmp/tdnpathviz-0.1.2.4-py3-none-any.whl.zip` & `tmp/tdnpathviz-0.1.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 378847 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-30 10:02 tdnpathviz/__init__.py
+Zip file size: 379078 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-30 10:18 tdnpathviz/__init__.py
 -rw-rw-rw-  2.0 fat      991 b- defN 23-Jan-02 15:29 tdnpathviz/datasets.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-02 15:29 tdnpathviz/utils.py
--rw-rw-rw-  2.0 fat    10688 b- defN 23-May-30 10:01 tdnpathviz/visualizations.py
+-rw-rw-rw-  2.0 fat    12050 b- defN 23-May-30 10:34 tdnpathviz/visualizations.py
 -rw-rw-rw-  2.0 fat  2179525 b- defN 23-Jan-02 15:29 tdnpathviz/data/train_dataset.csv
--rw-rw-rw-  2.0 fat      266 b- defN 23-May-30 10:07 tdnpathviz-0.1.2.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 10:07 tdnpathviz-0.1.2.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-May-30 10:07 tdnpathviz-0.1.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      724 b- defN 23-May-30 10:07 tdnpathviz-0.1.2.4.dist-info/RECORD
-9 files, 2192320 bytes uncompressed, 377597 bytes compressed:  82.8%
+-rw-rw-rw-  2.0 fat      266 b- defN 23-May-30 10:41 tdnpathviz-0.1.2.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 10:41 tdnpathviz-0.1.2.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-30 10:41 tdnpathviz-0.1.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      724 b- defN 23-May-30 10:41 tdnpathviz-0.1.2.5.dist-info/RECORD
+9 files, 2193682 bytes uncompressed, 377828 bytes compressed:  82.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tdnpathviz/visualizations.py
 Comment: 
 
 Filename: tdnpathviz/data/train_dataset.csv
 Comment: 
 
-Filename: tdnpathviz-0.1.2.4.dist-info/METADATA
+Filename: tdnpathviz-0.1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: tdnpathviz-0.1.2.4.dist-info/WHEEL
+Filename: tdnpathviz-0.1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: tdnpathviz-0.1.2.4.dist-info/top_level.txt
+Filename: tdnpathviz-0.1.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: tdnpathviz-0.1.2.4.dist-info/RECORD
+Filename: tdnpathviz-0.1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tdnpathviz/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.2.4'
+__version__ = '0.1.2.5'
```

## tdnpathviz/visualizations.py

```diff
@@ -43,47 +43,69 @@
         ret.append("rgba(" + str(r) + "," + str(g) + "," + str(b) + "," + str(alpha) + ")")
 
     return ret  # Return the list of generated colors
 
 
 
 def plot_first_main_paths(myPathAnalysis, path_column='mypath', id_column='travelid', nb_paths=15, print_query=False,
-                          font_size=10, width=1200, height=800):
+                          font_size=10, width=1200, height=800, weight_column = None, weight_agg = 'count'):
     """
         Plots the first main paths based on a given output of the teradataml NPATH function or the teradataml dataframe of its result field.
 
         Parameters:
         - myPathAnalysis (DataFrame or tdml.dataframe.dataframe.DataFrame): The input DataFrame containing path analysis data.
         - path_column (str, optional): The column name representing the path. Defaults to 'mypath'.
         - id_column (str or list, optional): The column name(s) representing the unique identifier(s). Defaults to 'travelid'.
         - nb_paths (int, optional): The number of main paths to plot. Defaults to 15.
         - print_query (bool, optional): Whether to print the generated query. Defaults to False.
         - font_size (int, optional): define the size of the font. Defaults is 10.
         - width (int, optional): define the width of the figure. Defaults is 1200.
         - height (int, optional): define the height of the figure. Defaults is 800.
+        - weight_column (str, optional): define the column to aggregate. If None, just count the number of pathes.
+          Default is None.
+        - weight_agg (str, optional): when weight_column is not None, then the weight is the result of the aggregation
+          defined by weight_agg on the weight_column. Permitted values are 'count', 'avg', 'max', 'min', 'sum'.
+          Default is 'count'.
 
         Returns:
         - None (it display an interactive Sankey plot)
     """
     if type(id_column) != list:
         id_column = [id_column]
 
-    if type(myPathAnalysis) != tdml.dataframe.dataframe.DataFrame:
-        df_agg = myPathAnalysis.result.select(id_column+[path_column]).groupby(path_column).count()
-    else:
-        df_agg = myPathAnalysis.select(id_column+[path_column]).groupby(path_column).count()
+    if weight_column == None:
 
-    df_agg._DataFrame__execute_node_and_set_table_name(df_agg._nodeid, df_agg._metaexpr)
+        if type(myPathAnalysis) != tdml.dataframe.dataframe.DataFrame:
+            df_agg = myPathAnalysis.result.select(id_column+[path_column]).groupby(path_column).count()
+        else:
+            df_agg = myPathAnalysis.select(id_column+[path_column]).groupby(path_column).count()
+
+        df_agg._DataFrame__execute_node_and_set_table_name(df_agg._nodeid, df_agg._metaexpr)
+
+        query = f"""SEL
+            row_number() OVER (PARTITION BY 1 ORDER BY count_{id_column[0]} DESC) as id
+        ,	REGEXP_REPLACE(lower(A.{path_column}),'\\[|\\]', '') as str
+        ,	count_{id_column[0]} as weight
+        FROM {df_agg._table_name} A
+        QUALIFY id < {nb_paths}+1"""
 
-    query = f"""SEL
-        row_number() OVER (PARTITION BY 1 ORDER BY count_{id_column[0]} DESC) as id
-    ,	REGEXP_REPLACE(lower(A.{path_column}),'\\[|\\]', '') as str
-    ,	count_{id_column[0]} as weight
-    FROM {df_agg._table_name} A
-    QUALIFY id < {nb_paths}+1"""
+    else:
+        if type(myPathAnalysis) != tdml.dataframe.dataframe.DataFrame:
+            df_agg = myPathAnalysis.result.select(list(set(id_column + [path_column] + [weight_column]))).groupby(path_column).agg({weight_column : weight_agg})
+        else:
+            df_agg = myPathAnalysis.select(list(set(id_column + [path_column] + [weight_column]))).groupby(path_column).agg({weight_column : weight_agg})
+
+        df_agg._DataFrame__execute_node_and_set_table_name(df_agg._nodeid, df_agg._metaexpr)
+
+        query = f"""SEL
+            row_number() OVER (PARTITION BY 1 ORDER BY {weight_agg}_{weight_column} DESC) as id
+        ,	REGEXP_REPLACE(lower(A.{path_column}),'\\[|\\]', '') as str
+        ,	{weight_agg}_{weight_column} as weight
+        FROM {df_agg._table_name} A
+        QUALIFY id < {nb_paths}+1"""
 
     df_selection = tdml.DataFrame.from_query(query)
 
     query2 = f"""
     sel
         CC.id
     ,	CC.node_source
```

