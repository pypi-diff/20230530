# Comparing `tmp/t4flib-0.3.0-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.3.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10963 bytes, number of entries: 12
+Zip file size: 10985 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx      987 b- defN 23-May-24 12:34 t4flib/config.py
 -rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
 -rw-rw-r--  2.0 unx     6145 b- defN 23-May-17 15:49 t4flib/file_helper.py
 -rw-rw-r--  2.0 unx     5621 b- defN 23-May-22 15:34 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
--rw-rw-r--  2.0 unx     2632 b- defN 23-May-30 14:21 t4flib/gcloud_helper.py
+-rw-rw-r--  2.0 unx     2682 b- defN 23-May-30 14:55 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      876 b- defN 23-May-30 14:21 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-30 14:35 t4flib-0.3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-30 14:35 t4flib-0.3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-30 14:35 t4flib-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      919 b- defN 23-May-30 14:35 t4flib-0.3.0.dist-info/RECORD
-12 files, 27435 bytes uncompressed, 9431 bytes compressed:  65.6%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-30 15:07 t4flib-0.3.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-30 15:07 t4flib-0.3.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-30 15:07 t4flib-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      919 b- defN 23-May-30 15:07 t4flib-0.3.1.dist-info/RECORD
+12 files, 27485 bytes uncompressed, 9453 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.3.0.dist-info/METADATA
+Filename: t4flib-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.3.0.dist-info/WHEEL
+Filename: t4flib-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.3.0.dist-info/top_level.txt
+Filename: t4flib-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.3.0.dist-info/RECORD
+Filename: t4flib-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/gcloud_helper.py

```diff
@@ -28,14 +28,17 @@
     credentials = service_account.Credentials.from_service_account_file(GCP_ACCOUNT_SERVICE_FILE)
     if ENVIRONEMENT == 'dev':
         os.environ["HTTPS_PROXY"] = PROXY_AUCHAN
 
     try:
         client = bigquery.Client(credentials=credentials)
         # Exécution de la requête BigQuery
+	
+        logger('DEBUG', f'Query => {query}')
+	
         query_job = client.query(valid_query.query, location='EU')
 
         # Attente de la fin de l'exécution de la requête et récupération des résultats
         results = query_job.result()
 
         # Conversion des résultats en DataFrame
         df = results.to_dataframe()
@@ -65,8 +68,8 @@
         return 0
 
     except FileNotFoundError as e:
         logger('ERROR',f'Le fichier {file_path} est introuvable : {e}')
         return 1
     except Exception as e:
         logger('ERROR',f'Une erreur inattendue s\'est produite : {e}')
-        return 1
+        return 1
```

## Comparing `t4flib-0.3.0.dist-info/METADATA` & `t4flib-0.3.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.3.0
+Version: 0.3.1
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

