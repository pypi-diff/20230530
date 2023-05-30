# Comparing `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230523171328.tar.gz` & `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230530192335.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230523171328.tar", last modified: Tue May 23 17:14:09 2023, max compression
+gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230530192335.tar", last modified: Tue May 30 19:24:16 2023, max compression
```

## Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523171328.tar` & `echofish-aws-indexing-lambda-1.0.0.dev20230530192335.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:14:09.609365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-23 17:13:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-23 17:14:09.609365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2101 2023-05-23 17:13:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 17:14:09.609365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-23 17:14:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:14:09.605365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:14:09.605365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 17:13:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12138 2023-05-23 17:13:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-05-23 17:13:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 17:14:09.605365 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2444 2023-05-23 17:14:09.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-05-23 17:14:09.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 17:14:09.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-23 17:14:09.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-23 17:14:09.000000 echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 19:24:16.163167 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-30 19:23:28.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-30 19:24:16.163167 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-05-30 19:23:28.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 19:24:16.163167 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      703 2023-05-30 19:24:13.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 19:24:16.163167 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 19:24:16.163167 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 19:23:28.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10281 2023-05-30 19:23:28.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-05-30 19:23:28.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 19:24:16.163167 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-05-30 19:24:16.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-05-30 19:24:16.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 19:24:16.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-30 19:24:16.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-30 19:24:16.000000 echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/LICENSE` & `echofish-aws-indexing-lambda-1.0.0.dev20230530192335/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230530192335/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230523171328
+Version: 1.0.0.dev20230530192335
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/README.md` & `echofish-aws-indexing-lambda-1.0.0.dev20230530192335/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/setup.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230530192335/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-indexing-lambda",
-  version="1.0.0.dev20230523171328",
+  version="1.0.0.dev20230530192335",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-indexing-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda/lambda_executor.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda/lambda_executor.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,49 +9,46 @@
 from datetime import datetime
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import as_completed
 
 class LambdaExecutor:
 
     def __init__(self, index_ek60_table_name, bucket_name, calibration_bucket, calibration_key):
-        self.session = boto3.Session()
-        self.dynamodb = self.session.client(service_name='dynamodb')
-        self.max_pool_connections = 64
-        self.client_config = botocore.config.Config(max_pool_connections=self.max_pool_connections)
-        self.s3 = self.session.client(service_name='s3', config=self.client_config)
         self.index_ek60_table_name = index_ek60_table_name
         self.bucket_name = bucket_name
         self.calibration_bucket = calibration_bucket
         self.calibration_key = calibration_key
+        self.max_pool_connections = 64
 
     def __find_child_objects(
             self,
-            sub_prefix: str
+            s3,
+            sub_prefix
         ) -> list:
         # Given a cruise sub_prefix, return all the children objects
-        paginator = self.s3.get_paginator('list_objects_v2')
+        paginator = s3.get_paginator('list_objects_v2')
         page_iterator = paginator.paginate(Bucket=self.bucket_name, Prefix=sub_prefix)
         objects = []
         for page in page_iterator:
             objects.extend(page['Contents'])
         return objects
 
-    def __get_all_objects(self) -> pd.DataFrame:
+    def __get_all_objects(self, s3) -> pd.DataFrame:
         # Get all objects in data/raw/ s3 folder.
         # Returns pandas dataframe with ['Key', 'LastModified', 'ETag', 'Size', 'StorageClass']
         # Threaded by cruise to decrease time.
         print("getting all objects")
         cruises = []
-        for ship in self.s3.list_objects(Bucket=self.bucket_name, Prefix='data/raw/', Delimiter='/').get('CommonPrefixes'):
-            for cruise in self.s3.list_objects(Bucket=self.bucket_name, Prefix=ship.get('Prefix'), Delimiter='/').get(
+        for ship in s3.list_objects(Bucket=self.bucket_name, Prefix='data/raw/', Delimiter='/').get('CommonPrefixes'):
+            for cruise in s3.list_objects(Bucket=self.bucket_name, Prefix=ship.get('Prefix'), Delimiter='/').get(
                     'CommonPrefixes'):
                 cruises.append(cruise.get('Prefix'))
         all_objects = []
         with ThreadPoolExecutor(max_workers=self.max_pool_connections) as executor:
-            futures = [executor.submit(self.__find_child_objects, cruise) for cruise in cruises]
+            futures = [executor.submit(self.__find_child_objects, s3, cruise) for cruise in cruises]
             for future in as_completed(futures):
                 all_objects.extend(future.result())
         return pd.DataFrame(all_objects)
 
     def __get_subset_ek60_prefix(
             self,
             df: pd.DataFrame
@@ -90,15 +87,15 @@
         return pd.DataFrame(objects)
 
     def __scan_datagram(self, select_key: str) -> list:
         # Reads the first 8 bytes of S3 file. Used to determine if ek60 or ek80
         # Note: uses boto3 session instead of boto3 client: https://github.com/boto/boto3/issues/801
         # select_key = 'data/raw/Albatross_Iv/AL0403/EK60/L0005-D20040302-T200108-EK60.raw'
         session_thread_pool = boto3.Session()  # remove for lambda
-        s3_thread_pool = session_thread_pool.resource(service_name='s3', config=self.client_config)
+        s3_thread_pool = session_thread_pool.resource(service_name='s3', config=botocore.config.Config(max_pool_connections=self.max_pool_connections))
         obj = s3_thread_pool.Object(bucket_name=self.bucket_name, key=select_key)  # XML0
         first_datagram = obj.get(Range='bytes=3-7')['Body'].read().decode().strip('\x00')
         return [{'KEY': select_key, 'DATAGRAM': first_datagram}]
 
     def __get_subset_datagrams(self, df: pd.DataFrame) -> list:
         print("getting subset of datagrams")
         select_keys = list(df[['KEY', 'CRUISE']].drop_duplicates(subset='CRUISE')['KEY'].values)
@@ -117,123 +114,83 @@
         # for each key write datagram value to all other files in same cruise
         for subset_datagram in subset_datagrams:
             if subset_datagram['DATAGRAM'] == 'CON0':
                 select_cruise = df.loc[df['KEY'] == subset_datagram['KEY']]['CRUISE'].iloc[0]
                 df.loc[df['CRUISE'] == select_cruise, ['DATAGRAM']] = subset_datagram['DATAGRAM']
         return df.loc[df['DATAGRAM'] == 'CON0']
 
-    def __create_table(
-            self
-    ) -> None:
-        params = {
-            'TableName': self.index_ek60_table_name,
-            'KeySchema': [
-                {'AttributeName': 'CRUISE', 'KeyType': 'HASH'},
-                {'AttributeName': 'SHIP', 'KeyType': 'RANGE'}
-            ],
-            'AttributeDefinitions': [
-                {'AttributeName': 'CRUISE', 'AttributeType': 'S'},
-                {'AttributeName': 'SHIP', 'AttributeType': 'S'}
-            ],
-            'BillingMode': 'PAY_PER_REQUEST',
-            'Tags': [
-                {
-                    'Key': 'project',
-                    'Value': 'echofish'
-                },
-            ],
-        }
-        # TODO: create_table returns a dict for validation
-        table = self.dynamodb.create_table(**params)
-        waiter = self.dynamodb.get_waiter('table_exists')
-        waiter.wait(TableName=self.index_ek60_table_name)
-        print(f"table: {self.index_ek60_table_name} created")
-
-    def __delete_table(
-            self
-    ) -> None:
-        # Attempts to delete an existing table.
-        try:
-            self.dynamodb.delete_table(TableName=self.index_ek60_table_name)
-            waiter = self.dynamodb.get_waiter('table_not_exists')
-            waiter.wait(TableName=self.index_ek60_table_name)
-            print(f"table: {self.index_ek60_table_name} deleted")
-        except self.dynamodb.exceptions.ClientError as err:
-            # logger.error(
-            #     "Could not delete table. Reason: %s: %s",
-            #     err.response['Error']['Code'], err.response['Error']['Message']
-            # )
-            raise err
-        except self.dynamodb.exceptions.ParamValidationError as error:
-            raise ValueError('The parameters provided are incorrect: {}'.format(error))
 
     def __get_calibration_information(
-            self
+            self, s3
     ) -> pd.DataFrame:
         # Calibration data generated by Chuck currently located here:
         #      https://noaa-wcsd-pds-index.s3.amazonaws.com/calibrated_crusies.csv
-        response = self.s3.get_object(Bucket=self.calibration_bucket, Key=self.calibration_key)
+        response = s3.get_object(Bucket=self.calibration_bucket, Key=self.calibration_key)
         status = response.get("ResponseMetadata", {}).get("HTTPStatusCode")
         calibration_status = pd.DataFrame(columns=["DATASET_NAME", "INSTRUMENT_NAME", "CAL_STATE"])
         if status == 200:
             calibration_status = pd.read_csv(response.get("Body"))
             calibration_status['DATASET_NAME'] = calibration_status['DATASET_NAME'].apply(lambda x: x.split('_EK60')[0])
             # Note: Data are either:
             #      [1] Calibrated w/ calibration data
             #      [2] Calibrated w/o calibration data
             #      [3] uncalibrated
             calibration_status['CAL_STATE'] = calibration_status['CAL_STATE'].apply(lambda x: x.find('Calibrated') >= 0)
         else:
             print(f"Unsuccessful S3 get_object response. Status - {status}")
         return calibration_status
 
-    def execute(self):
+    def execute(self, message):
+        session = boto3.Session()
+        dynamodb = session.client(service_name='dynamodb')
+        s3 = session.client(service_name='s3', config=botocore.config.Config(max_pool_connections=self.max_pool_connections))
+
+
+
         start = datetime.now()  # used for benchmarking
         # Get all object in public dataset bucket
-        all_objects = self.__get_all_objects()
+        all_objects = self.__get_all_objects(s3)
         #
         subset_ek60_by_prefix = self.__get_subset_ek60_prefix(
             df=all_objects[all_objects['Key'].str.contains('EK60')][['Key', 'Size']]
         )
         subset_datagrams = self.__get_subset_datagrams(df=subset_ek60_by_prefix)
         ek60_objects = self.__get_ek60_objects(subset_ek60_by_prefix, subset_datagrams)
         print(start)  # 1:26:57 to 1:39:??
         #
-        current_tables = self.dynamodb.list_tables()
-        if self.index_ek60_table_name in current_tables['TableNames']:
-            print('deleting existing table')
-            self.__delete_table()
-
-        # create new index table
-        self.__create_table()
-        calibration_status = self.__get_calibration_information()
+        # current_tables = self.dynamodb.list_tables()
+        # if self.index_ek60_table_name in current_tables['TableNames']:
+        #     print('deleting existing table')
+        #     self.__delete_table()
+
+        calibration_status = self.__get_calibration_information(s3)
         #
         # TODO: melt calibration_status with
         # ek60_objects['CALIBRATED'] = np.repeat(False, ek60_objects.shape[0])
         # cruises = list(set(ek60_objects['CRUISE']))
         # for i in cruises:
         #     print(i)
         #     if i in list(calibration_status['DATASET_NAME']):
         #         ek60_objects.loc[ek60_objects['CRUISE'] == i, 'CALIBRATED'] = True
         # ek60_objects['CALIBRATED'].value_counts()
         #
-        cruise_names = list(set(ek60_objects['CRUISE']));
+        cruise_names = list(set(ek60_objects['CRUISE']))
         cruise_names.sort()
         for cruise_name in cruise_names:  # ~322 cruises
             cruise_data = ek60_objects.groupby('CRUISE').get_group(cruise_name)
             ship = cruise_data['SHIP'].iloc[0]
             sensor = cruise_data['SENSOR'].iloc[0]
             datagram = cruise_data['DATAGRAM'].iloc[0]
             file_count = cruise_data.shape[0]
             total_size = np.sum(cruise_data['SIZE'])
             calibrated = cruise_name in calibration_status['DATASET_NAME'].unique()  # ~276 entries
             start_date = np.min(cruise_data['DATE']).isoformat(timespec="seconds") + "Z"
             end_date = np.max(cruise_data['DATE']).isoformat(timespec="seconds") + "Z"
             #
-            self.dynamodb.put_item(  # TODO: verify status_code['ResponseMetadata']['HTTPStatusCode'] == 200
+            dynamodb.put_item(  # TODO: verify status_code['ResponseMetadata']['HTTPStatusCode'] == 200
                 TableName=self.index_ek60_table_name,
                 Item={
                     'CRUISE': {'S': cruise_name},
                     'SHIP': {'S': ship},
                     'SENSOR': {'S': sensor},
                     'DATAGRAM': {'S': datagram},
                     'FILE_COUNT': {'N': str(file_count)},
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230523171328/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230530192335/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230523171328
+Version: 1.0.0.dev20230530192335
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

