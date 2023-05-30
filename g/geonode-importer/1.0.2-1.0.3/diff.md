# Comparing `tmp/geonode_importer-1.0.2-py3-none-any.whl.zip` & `tmp/geonode_importer-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 89165 bytes, number of entries: 77
--rw-r--r--  2.0 unx     1132 b- defN 23-May-25 08:32 importer/__init__.py
+Zip file size: 89258 bytes, number of entries: 77
+-rw-r--r--  2.0 unx     1132 b- defN 23-May-30 11:50 importer/__init__.py
 -rw-r--r--  2.0 unx      891 b- defN 23-May-16 14:04 importer/apps.py
 -rw-r--r--  2.0 unx      301 b- defN 23-May-16 14:04 importer/celery_app.py
 -rw-r--r--  2.0 unx    25673 b- defN 23-May-16 14:04 importer/celery_tasks.py
 -rw-r--r--  2.0 unx     1142 b- defN 23-May-16 14:04 importer/datastore.py
 -rw-r--r--  2.0 unx     2137 b- defN 23-May-16 14:04 importer/db_router.py
 -rw-r--r--  2.0 unx     1533 b- defN 23-May-16 14:04 importer/models.py
 -rw-r--r--  2.0 unx    13953 b- defN 23-May-16 14:04 importer/orchestrator.py
@@ -20,15 +20,15 @@
 -rw-r--r--  2.0 unx    10650 b- defN 23-May-16 14:04 importer/api/views.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-16 14:04 importer/handlers/__init__.py
 -rw-r--r--  2.0 unx     2627 b- defN 23-May-16 14:04 importer/handlers/apps.py
 -rw-r--r--  2.0 unx     5126 b- defN 23-May-16 14:04 importer/handlers/base.py
 -rw-r--r--  2.0 unx     2786 b- defN 23-May-16 14:04 importer/handlers/tests.py
 -rw-r--r--  2.0 unx     5291 b- defN 23-May-16 14:04 importer/handlers/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-16 14:04 importer/handlers/common/__init__.py
--rw-r--r--  2.0 unx    20243 b- defN 23-May-16 14:04 importer/handlers/common/raster.py
+-rw-r--r--  2.0 unx    20407 b- defN 23-May-30 11:50 importer/handlers/common/raster.py
 -rw-r--r--  2.0 unx     3184 b- defN 23-May-16 14:04 importer/handlers/common/tests_raster.py
 -rw-r--r--  2.0 unx    10000 b- defN 23-May-16 14:04 importer/handlers/common/tests_vector.py
 -rw-r--r--  2.0 unx    34026 b- defN 23-May-17 09:15 importer/handlers/common/vector.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-16 14:04 importer/handlers/csv/__init__.py
 -rw-r--r--  2.0 unx      284 b- defN 23-May-16 14:04 importer/handlers/csv/exceptions.py
 -rw-r--r--  2.0 unx     8993 b- defN 23-May-16 14:04 importer/handlers/csv/handler.py
 -rw-r--r--  2.0 unx     7043 b- defN 23-May-16 14:04 importer/handlers/csv/tests.py
@@ -55,25 +55,25 @@
 -rw-r--r--  2.0 unx     1039 b- defN 23-May-16 14:04 importer/handlers/shapefile/serializer.py
 -rw-r--r--  2.0 unx     5650 b- defN 23-May-16 14:04 importer/handlers/shapefile/tests.py
 -rw-r--r--  2.0 unx     1031 b- defN 23-May-16 14:04 importer/migrations/0001_initial.py
 -rw-r--r--  2.0 unx      455 b- defN 23-May-16 14:04 importer/migrations/0002_resourcehandlerinfo_kwargs.py
 -rw-r--r--  2.0 unx      595 b- defN 23-May-16 14:04 importer/migrations/0003_resourcehandlerinfo_execution_id.py
 -rw-r--r--  2.0 unx      409 b- defN 23-May-16 14:04 importer/migrations/0004_rename_execution_id_resourcehandlerinfo_execution_request.py
 -rw-r--r--  2.0 unx     1106 b- defN 23-May-16 14:04 importer/migrations/0005_fixup_dynamic_shema_table_names.py
--rw-r--r--  2.0 unx     1333 b- defN 23-May-16 14:04 importer/migrations/0006_dataset_migration.py
+-rw-r--r--  2.0 unx     1584 b- defN 23-May-30 11:50 importer/migrations/0006_dataset_migration.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-16 14:04 importer/migrations/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-16 14:04 importer/tests/__init__.py
 -rw-r--r--  2.0 unx     1815 b- defN 23-May-16 14:04 importer/tests/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-16 14:04 importer/tests/end2end/__init__.py
 -rw-r--r--  2.0 unx     6095 b- defN 23-May-16 14:04 importer/tests/end2end/test_end2end.py
 -rw-r--r--  2.0 unx     7707 b- defN 23-May-16 14:04 importer/tests/end2end/test_end2end_copy.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-16 14:04 importer/tests/unit/__init__.py
 -rw-r--r--  2.0 unx     1234 b- defN 23-May-16 14:04 importer/tests/unit/test_models.py
 -rw-r--r--  2.0 unx    13739 b- defN 23-May-16 14:04 importer/tests/unit/test_orchestrator.py
 -rw-r--r--  2.0 unx     3606 b- defN 23-May-16 14:04 importer/tests/unit/test_publisher.py
 -rw-r--r--  2.0 unx    23904 b- defN 23-May-16 14:04 importer/tests/unit/test_task.py
--rw-r--r--  2.0 unx     1069 b- defN 23-May-25 08:33 geonode_importer-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      712 b- defN 23-May-25 08:33 geonode_importer-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 08:33 geonode_importer-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-25 08:33 geonode_importer-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6809 b- defN 23-May-25 08:33 geonode_importer-1.0.2.dist-info/RECORD
-77 files, 293343 bytes uncompressed, 78227 bytes compressed:  73.3%
+-rw-r--r--  2.0 unx     1069 b- defN 23-May-30 11:51 geonode_importer-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      712 b- defN 23-May-30 11:51 geonode_importer-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 11:51 geonode_importer-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-30 11:51 geonode_importer-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6809 b- defN 23-May-30 11:51 geonode_importer-1.0.3.dist-info/RECORD
+77 files, 293758 bytes uncompressed, 78320 bytes compressed:  73.3%
```

## zipnote {}

```diff
@@ -210,23 +210,23 @@
 
 Filename: importer/tests/unit/test_publisher.py
 Comment: 
 
 Filename: importer/tests/unit/test_task.py
 Comment: 
 
-Filename: geonode_importer-1.0.2.dist-info/LICENSE
+Filename: geonode_importer-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: geonode_importer-1.0.2.dist-info/METADATA
+Filename: geonode_importer-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: geonode_importer-1.0.2.dist-info/WHEEL
+Filename: geonode_importer-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: geonode_importer-1.0.2.dist-info/top_level.txt
+Filename: geonode_importer-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: geonode_importer-1.0.2.dist-info/RECORD
+Filename: geonode_importer-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## importer/__init__.py

```diff
@@ -16,13 +16,13 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 #########################################################################
 import os
 
 project_dir = os.path.dirname(os.path.abspath(__file__))
 
-VERSION = (1, 0, 2)
+VERSION = (1, 0, 3)
 __version__ = ".".join([str(i) for i in VERSION])
 __author__ = "geosolutions-it"
 __email__ = "info@geosolutionsgroup.com"
 __url__ = "https://github.com/GeoNode/geonode-importer"
 default_app_config = "importer.apps.ImporterConfig"
```

## importer/handlers/common/raster.py

```diff
@@ -500,14 +500,17 @@
 
     original_dataset = ResourceBase.objects.filter(alternate=alternate)
     if not original_dataset.exists():
         raise InvalidGeoTiffException("Dataset required does not exists")
 
     original_dataset = original_dataset.first()
 
+    if not original_dataset.files:
+        raise InvalidGeoTiffException("The original file of the dataset is not available, Is not possible to copy the dataset")
+
     new_file_location = orchestrator.load_handler(handler_module_path).copy_original_file(original_dataset)
 
     new_dataset_alternate = create_alternate(original_dataset.title, exec_id)
 
     additional_kwargs = {
         "original_dataset_alternate": original_dataset.alternate,
         "new_dataset_alternate": new_dataset_alternate,
```

## importer/migrations/0006_dataset_migration.py

```diff
@@ -6,15 +6,21 @@
 
 def dataset_migration(apps, _):
     NewResources = apps.get_model('importer', 'ResourceHandlerInfo')
     for old_resource in Dataset.objects\
         .exclude(pk__in=NewResources.objects.values_list('resource_id', flat=True))\
         .exclude(subtype__in=['remote', None]):        
         # generating orchestrator expected data file
-        converted_files = [{"base_file": x} for x in old_resource.files]
+        if not old_resource.files:
+            if old_resource.is_vector():
+                converted_files = [{"base_file": "placeholder.shp"}]
+            else:
+                converted_files = [{"base_file": "placeholder.tiff"}]
+        else:
+            converted_files = [{"base_file": x} for x in old_resource.files]
         # try to get the handler for the file of the old resource
         # when is found, we can exit
         handler_to_use = None
         for _input in converted_files:
             handler = orchestrator.get_handler(_input)
             if handler is not None:
                 handler_to_use = handler
```

## Comparing `geonode_importer-1.0.2.dist-info/LICENSE` & `geonode_importer-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `geonode_importer-1.0.2.dist-info/METADATA` & `geonode_importer-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geonode-importer
-Version: 1.0.2
+Version: 1.0.3
 Home-page: https://github.com/GeoNode/geonode-importer
 Author: geosolutions-it
 Author-email: info@geosolutionsgroup.com
 Project-URL: Bug Tracker, https://github.com/geosolutions-it/geonode-importer/issues
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.0
```

## Comparing `geonode_importer-1.0.2.dist-info/RECORD` & `geonode_importer-1.0.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-importer/__init__.py,sha256=N7SGyQz8PbnSVAe_Och2MoImoVhkeHpd4g0gMCxR8lM,1132
+importer/__init__.py,sha256=mSMvUe1vcXbgioIg-h-G46y0ftjWGZkBHoOCOK0t5Vg,1132
 importer/apps.py,sha256=nym_44W069KBuqrWbDw64y7CetrA8xFPVgEBcP7F1_A,891
 importer/celery_app.py,sha256=vXVNHq_WntdNstgbKbVVJsOhTllf__ZWr-skmDohJvE,301
 importer/celery_tasks.py,sha256=rbx_r7w9K5MPJh_gIkdLF4lgDMgAh_D9Vcv7_0LoG_A,25673
 importer/datastore.py,sha256=OejV7R8G5fmvSGW3fJPGoE5DE3C_GZylYUIYOz2kbFg,1142
 importer/db_router.py,sha256=zY65wik8Z6ptJ3MggYxp4isFt11ohmk_5t2pIS9MBeA,2137
 importer/models.py,sha256=MuLxhMp8MnFT3J00dPX1gigk1K-ol6fmcpIJ1D6QvMg,1533
 importer/orchestrator.py,sha256=Lsljy5kA0VTeg1oS-0ok55CtFUNUt_L8hOLWxtvam00,13953
@@ -19,15 +19,15 @@
 importer/api/views.py,sha256=IJFZdDzKmKduxYp3CWHS0agaTUoapXTd71eML1JmI-g,10650
 importer/handlers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 importer/handlers/apps.py,sha256=1sr3cX-SOq0pIk_MCpv9Gzvncruwg7m4fWc-QjwUOMk,2627
 importer/handlers/base.py,sha256=7acaVWIe-qBawmk09DciqE-HIXdlvOMZE7UM6LWTFCE,5126
 importer/handlers/tests.py,sha256=ov4UXqVw7r1FzKn356-fXqukLWRNI1Eya9fPpKGGmsE,2786
 importer/handlers/utils.py,sha256=_jPg0oZBwE9o0dmQRfwsDYBYjapdrLARMo2nuMZQxX4,5291
 importer/handlers/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-importer/handlers/common/raster.py,sha256=B7drNzJ_VGzvFcx_5cUnZDUCREmK-7fDx7FWdxO-8xI,20243
+importer/handlers/common/raster.py,sha256=g5VokU0SGZxknRA3aiU4Rs-jbsf-zwBGFGYslNerXUs,20407
 importer/handlers/common/tests_raster.py,sha256=utZSrN3f_cJmoOQwhBpnsC6exslTcO-p6QdLUnUK2BU,3184
 importer/handlers/common/tests_vector.py,sha256=y8fUy_qXAjWpMl5yUwAUc_umNjSkb4JP7KzhA6YaOCA,10000
 importer/handlers/common/vector.py,sha256=qyLZkdWHD_pXKuFxu2vT5WUNzBd8Os3wJYP7vcCM9rg,34026
 importer/handlers/csv/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 importer/handlers/csv/exceptions.py,sha256=WKpt-dN1O1OroyUJx7jztuJPxe0FRks5qGpoZlKVucM,284
 importer/handlers/csv/handler.py,sha256=ch0YgWx1DH-tpb1UIwRRgZewxdR8R9-_Jhp9TaGbonw,8993
 importer/handlers/csv/tests.py,sha256=oe6g9YS12owzHHxDyGu0PjJswV1uW_vNuqX0XNnFh2A,7043
@@ -54,24 +54,24 @@
 importer/handlers/shapefile/serializer.py,sha256=mMQrfe6p3jcEIWIP1XBidzXaEMhkmEwehCXwE50tyvU,1039
 importer/handlers/shapefile/tests.py,sha256=boFIlI0eBeh8L5nrdhsx2OWJI39APtKA9fWMin33Y3k,5650
 importer/migrations/0001_initial.py,sha256=S7oonhRfSMiquei800v5umCSrqkNvfX7hqrGCWXi34U,1031
 importer/migrations/0002_resourcehandlerinfo_kwargs.py,sha256=fT3ncsBvO5LAJRhN4ECIL9WsLKXDNZ1AwFMpu9IqRYY,455
 importer/migrations/0003_resourcehandlerinfo_execution_id.py,sha256=V7Ow2Gaq3YdKGQcRM6XKifT4cIpM6ZbiTRb2MkuKWzQ,595
 importer/migrations/0004_rename_execution_id_resourcehandlerinfo_execution_request.py,sha256=_TwrOC_6ORRMWEa9fg8CqRPC6vDy2Hnbh6Wg9Jtq2kE,409
 importer/migrations/0005_fixup_dynamic_shema_table_names.py,sha256=9B2Me4Tkx3gnLBTP7UpjdUD0YVF6qUtVWLAm0EsO-hg,1106
-importer/migrations/0006_dataset_migration.py,sha256=YnLPxWm7DehCJh2vFtTdHZI82E_kkuM8R0aNAZRvVtU,1333
+importer/migrations/0006_dataset_migration.py,sha256=Jn14JxlGL2FFTSwC-hcm7gJcESd_c62aTT9y6os_njo,1584
 importer/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 importer/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 importer/tests/utils.py,sha256=biJXuf-Tyhzly_SklA4YzxsllGm50Vmqwm0HIPqGzWU,1815
 importer/tests/end2end/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 importer/tests/end2end/test_end2end.py,sha256=Qh4P3o9LChneY-pKdpP459EzmBv1XwGwYfiWWXT1-_s,6095
 importer/tests/end2end/test_end2end_copy.py,sha256=QDmUCZOuhYcB8ie_NDWAw2NIJhcAenlnWimpWzzrIA8,7707
 importer/tests/unit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 importer/tests/unit/test_models.py,sha256=cykml2VUVbiCmdeTTG7pqKAdZiCu0kAALxH7AVSWrC0,1234
 importer/tests/unit/test_orchestrator.py,sha256=M5KueNjjCC3hPfQRepZZD7oo58tDbM7sakmYx-ffUo8,13739
 importer/tests/unit/test_publisher.py,sha256=u6juJPEWoQoKGhfjt6h4D160PDkF8dKuZiiPwwN3XZU,3606
 importer/tests/unit/test_task.py,sha256=AYl0z7IvUMfHKt_bmIdsCaLL0Rn6M6pXHF4zxD8MdsI,23904
-geonode_importer-1.0.2.dist-info/LICENSE,sha256=gMS2YAekulHmzbeQAk-e6U1_unOcCszd6aKY5bQJXO0,1069
-geonode_importer-1.0.2.dist-info/METADATA,sha256=-iNFdy_l_me7uHQatPFjW7C236qC8oJO5_sn6sEGS0Q,712
-geonode_importer-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-geonode_importer-1.0.2.dist-info/top_level.txt,sha256=MRQ0MhtKdXF90IDYri2Z5uPJ8A9O0ITe5bEXA2ZLjM4,9
-geonode_importer-1.0.2.dist-info/RECORD,,
+geonode_importer-1.0.3.dist-info/LICENSE,sha256=gMS2YAekulHmzbeQAk-e6U1_unOcCszd6aKY5bQJXO0,1069
+geonode_importer-1.0.3.dist-info/METADATA,sha256=AgcwitUJ67cib_T_OUXc11vAAbs9ZYce7cGh8zQLitY,712
+geonode_importer-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+geonode_importer-1.0.3.dist-info/top_level.txt,sha256=MRQ0MhtKdXF90IDYri2Z5uPJ8A9O0ITe5bEXA2ZLjM4,9
+geonode_importer-1.0.3.dist-info/RECORD,,
```

