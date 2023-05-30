# Comparing `tmp/t4flib-0.2.7-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.3.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11208 bytes, number of entries: 12
+Zip file size: 10963 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx      987 b- defN 23-May-24 12:34 t4flib/config.py
 -rw-rw-r--  2.0 unx      971 b- defN 23-May-17 15:49 t4flib/data_helper.py
 -rw-rw-r--  2.0 unx     6145 b- defN 23-May-17 15:49 t4flib/file_helper.py
 -rw-rw-r--  2.0 unx     5621 b- defN 23-May-22 15:34 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     7420 b- defN 23-May-17 15:49 t4flib/functional_helper.py
--rw-rw-r--  2.0 unx     3235 b- defN 23-May-17 15:49 t4flib/gcloud_helper.py
--rw-rw-r--  2.0 unx     1229 b- defN 23-May-24 12:34 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-24 12:47 t4flib-0.2.7.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-24 12:47 t4flib-0.2.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-24 12:47 t4flib-0.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      920 b- defN 23-May-24 12:47 t4flib-0.2.7.dist-info/RECORD
-12 files, 28392 bytes uncompressed, 9676 bytes compressed:  65.9%
+-rw-rw-r--  2.0 unx     2632 b- defN 23-May-30 14:21 t4flib/gcloud_helper.py
+-rw-rw-r--  2.0 unx      876 b- defN 23-May-30 14:21 t4flib/log_helper.py
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-30 14:35 t4flib-0.3.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-30 14:35 t4flib-0.3.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-30 14:35 t4flib-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      919 b- defN 23-May-30 14:35 t4flib-0.3.0.dist-info/RECORD
+12 files, 27435 bytes uncompressed, 9431 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.2.7.dist-info/METADATA
+Filename: t4flib-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.2.7.dist-info/WHEEL
+Filename: t4flib-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.2.7.dist-info/top_level.txt
+Filename: t4flib-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.2.7.dist-info/RECORD
+Filename: t4flib-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/gcloud_helper.py

```diff
@@ -1,69 +1,56 @@
 import shutil
-
+from pydantic import BaseModel, Field, ValidationError
 from google.cloud import bigquery
 from google.oauth2 import service_account
 from google.cloud import storage
 from google.api_core import exceptions as gcloud_ex
 import pandas as pd
 from .log_helper import logger
 from .config import GCP_ACCOUNT_SERVICE_FILE, ENVIRONEMENT, PROXY_AUCHAN, BQ_PROJECT_ID
 import os
 
+# Modèle de validation pour une requête BigQuery
+class QueryModel(BaseModel):
+    query: str = Field(..., min_length=1)
+
+def run_bq_query(query) -> pd.DataFrame:
+    """
+    Cette fonction exécute une requête BigQuery et retourne un DataFrame sans les en-têtes.
+    """
+    # Vérification de la validité de la requête
+    try:
+        valid_query = QueryModel(query=query)
+    except ValidationError as e:
+        logger('ERROR', f"La requête est invalide : {e}")
+        return None
 
-def run_bq_query(query):
     ENVIRONEMENT='dev'
     credentials = service_account.Credentials.from_service_account_file(GCP_ACCOUNT_SERVICE_FILE)
     if ENVIRONEMENT == 'dev':
         os.environ["HTTPS_PROXY"] = PROXY_AUCHAN
+
     try:
-        logger('DEBUG', query)
         client = bigquery.Client(credentials=credentials)
-        query_job = client.query(query, location='EU')
-        # if len(query_job.errors) > 0:
-        #     return 1, pd.DataFrame()
-
-        response = [dict(row) for row in query_job.result()]
-        response_dataframe = pd.DataFrame.from_records(response)
-        logger('INFO', 'La requete a été executé avec succès !')
-        return 0, response_dataframe
-
-    except gcloud_ex.BadRequest as e:
-        logger('ERROR', f"La requête est mal formée ou comporte des erreurs syntaxiques : {str(e)}")
-        return 1, None
-
-    except gcloud_ex.Forbidden as e:
-        logger('ERROR',
-               f"L'utilisateur n'a pas les autorisations nécessaires pour accéder aux ressources demandées : {str(e)}")
-        return 1, None
-
-    except gcloud_ex.NotFound as e:
-        logger('ERROR', f"La ressource demandée n'a pas été trouvée : {str(e)}")
-        return 1, None
-
-    except gcloud_ex.ServiceUnavailable as e:
-        logger('ERROR', f"Le service BigQuery n'est pas disponible ou inaccessible : {str(e)}")
-        return 1, None
-
-    except gcloud_ex.TooManyRequests as e:
-        logger('ERROR', f"L'utilisateur a dépassé le quota de requêtes autorisé : {str(e)}")
-        return 1, None
-
-    except  gcloud_ex.PermissionDenied as e:
-        logger('ERROR', f"Erreur lors de l'indetification : {str(e)}")
-        return 1, None
-
-    except gcloud_ex.GoogleAPIError as e:
-        logger('ERROR', f"Une erreur s'est produite lors de l'exécution de la requête : {str(e)}")
-        return 1, None
+        # Exécution de la requête BigQuery
+        query_job = client.query(valid_query.query, location='EU')
+
+        # Attente de la fin de l'exécution de la requête et récupération des résultats
+        results = query_job.result()
+
+        # Conversion des résultats en DataFrame
+        df = results.to_dataframe()
+
+        logger('INFO', f"La requête a été exécutée avec succès.")
+
+        return df
 
     except Exception as e:
-        logger('ERROR', f'Une erreur non repertorié est survenue : {str(e)}')
-        return 1, None
-    
+        logger('ERROR', f"Une erreur est survenue lors de l'exécution de la requête : {e}")
+        return None
 
 
 def upload_file_to_gcs(file_path, bucket_name, path_bucket):
     logger('INFO', f'Début de l\'upload du fichier {file_path} vers le bucket {bucket_name}')
     try:
         if ENVIRONEMENT == 'dev':
             os.environ["HTTPS_PROXY"] = PROXY_AUCHAN
```

## t4flib/log_helper.py

```diff
@@ -26,20 +26,7 @@
         color = Fore.BLUE
     else:
         color = Fore.WHITE
 
     print(
         f"|{indentation} [{timestamp}] - [{Fore.CYAN}{inspect.stack()[1].function}{Fore.RESET}] - "
         f"[{color}{severity}{Fore.RESET}] {message}")
-
-
-def setup_logger(name, log_file, level=logging.INFO):
-    formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-    
-    handler = logging.FileHandler(log_file)
-    handler.setFormatter(formatter)
-    
-    logger = logging.getLogger(name)
-    logger.setLevel(level)
-    logger.addHandler(handler)
-    
-    return logger
```

## Comparing `t4flib-0.2.7.dist-info/METADATA` & `t4flib-0.3.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.2.7
+Version: 0.3.0
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

