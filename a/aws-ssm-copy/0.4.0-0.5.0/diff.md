# Comparing `tmp/aws-ssm-copy-0.4.0.tar.gz` & `tmp/aws-ssm-copy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ssm-copy-0.4.0.tar", last modified: Sat Apr  2 19:32:28 2022, max compression
+gzip compressed data, was "aws-ssm-copy-0.5.0.tar", last modified: Tue May 30 08:58:41 2023, max compression
```

## Comparing `aws-ssm-copy-0.4.0.tar` & `aws-ssm-copy-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2022-04-02 19:32:28.983534 aws-ssm-copy-0.4.0/
--rw-------   0 mvanholsteijn   (502) staff       (20)    11357 2018-02-22 10:44:58.000000 aws-ssm-copy-0.4.0/LICENSE
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     1669 2022-04-02 19:32:28.983405 aws-ssm-copy-0.4.0/PKG-INFO
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     1356 2022-04-02 18:38:55.000000 aws-ssm-copy-0.4.0/README.md
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)       38 2022-04-02 19:32:28.983577 aws-ssm-copy-0.4.0/setup.cfg
--rwxr-xr-x   0 mvanholsteijn   (502) staff       (20)      901 2022-04-02 19:31:49.000000 aws-ssm-copy-0.4.0/setup.py
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2022-04-02 19:32:28.980671 aws-ssm-copy-0.4.0/src/
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2022-04-02 19:32:28.981983 aws-ssm-copy-0.4.0/src/aws_ssm_copy/
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)       39 2020-11-27 08:34:45.000000 aws-ssm-copy-0.4.0/src/aws_ssm_copy/__init__.py
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)       47 2020-11-27 08:34:45.000000 aws-ssm-copy-0.4.0/src/aws_ssm_copy/__main__.py
--rwxr-xr-x   0 mvanholsteijn   (502) staff       (20)     9745 2022-04-02 19:15:16.000000 aws-ssm-copy-0.4.0/src/aws_ssm_copy/ssm_copy.py
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2022-04-02 19:32:28.983228 aws-ssm-copy-0.4.0/src/aws_ssm_copy.egg-info/
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     1669 2022-04-02 19:32:28.000000 aws-ssm-copy-0.4.0/src/aws_ssm_copy.egg-info/PKG-INFO
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      394 2022-04-02 19:32:28.000000 aws-ssm-copy-0.4.0/src/aws_ssm_copy.egg-info/SOURCES.txt
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)        1 2022-04-02 19:32:28.000000 aws-ssm-copy-0.4.0/src/aws_ssm_copy.egg-info/dependency_links.txt
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)       51 2022-04-02 19:32:28.000000 aws-ssm-copy-0.4.0/src/aws_ssm_copy.egg-info/entry_points.txt
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)        1 2022-04-02 18:44:46.000000 aws-ssm-copy-0.4.0/src/aws_ssm_copy.egg-info/not-zip-safe
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)        6 2022-04-02 19:32:28.000000 aws-ssm-copy-0.4.0/src/aws_ssm_copy.egg-info/requires.txt
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)       13 2022-04-02 19:32:28.000000 aws-ssm-copy-0.4.0/src/aws_ssm_copy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:58:41.786480 aws-ssm-copy-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 08:58:39.000000 aws-ssm-copy-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-30 08:58:41.782480 aws-ssm-copy-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-30 08:58:39.000000 aws-ssm-copy-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:58:41.786480 aws-ssm-copy-0.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      900 2023-05-30 08:58:39.000000 aws-ssm-copy-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:58:41.782480 aws-ssm-copy-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:58:41.782480 aws-ssm-copy-0.5.0/src/aws_ssm_copy/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 08:58:39.000000 aws-ssm-copy-0.5.0/src/aws_ssm_copy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 08:58:39.000000 aws-ssm-copy-0.5.0/src/aws_ssm_copy/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11786 2023-05-30 08:58:39.000000 aws-ssm-copy-0.5.0/src/aws_ssm_copy/ssm_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:58:41.782480 aws-ssm-copy-0.5.0/src/aws_ssm_copy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-30 08:58:41.000000 aws-ssm-copy-0.5.0/src/aws_ssm_copy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-30 08:58:41.000000 aws-ssm-copy-0.5.0/src/aws_ssm_copy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:58:41.000000 aws-ssm-copy-0.5.0/src/aws_ssm_copy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 08:58:41.000000 aws-ssm-copy-0.5.0/src/aws_ssm_copy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:58:41.000000 aws-ssm-copy-0.5.0/src/aws_ssm_copy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 08:58:41.000000 aws-ssm-copy-0.5.0/src/aws_ssm_copy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 08:58:41.000000 aws-ssm-copy-0.5.0/src/aws_ssm_copy.egg-info/top_level.txt
```

### Comparing `aws-ssm-copy-0.4.0/LICENSE` & `aws-ssm-copy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ssm-copy-0.4.0/PKG-INFO` & `aws-ssm-copy-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-copy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Copy AWS Parameter Store parameters
 Home-page: https://github.com/binxio/aws-ssm-copy
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: UNKNOWN
 Platform: any
 Description-Content-Type: text/markdown
@@ -34,14 +34,15 @@
 --source-region REGION to get the parameters from
 --source-profile NAME  to obtain the parameters from
 --region REGION        to copy the parameters to
 --profile NAME         to copy the parameters to
 --target-path NAME     to copy the parameters to
 --key-id ID            to use for parameter values in the destination
 --clear-key-id, -C     clear the kms key id associated with the parameter
+--with-tags, -W        copy the tags too, existing tags will be removed
 ```
 
 
 ## Examples
 Copy all parameters under /dev to a new profile:
 ```
 aws-ssm-copy --profile binx-io --recursive /dev
```

### Comparing `aws-ssm-copy-0.4.0/README.md` & `aws-ssm-copy-0.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 --source-region REGION to get the parameters from
 --source-profile NAME  to obtain the parameters from
 --region REGION        to copy the parameters to
 --profile NAME         to copy the parameters to
 --target-path NAME     to copy the parameters to
 --key-id ID            to use for parameter values in the destination
 --clear-key-id, -C     clear the kms key id associated with the parameter
+--with-tags, -W        copy the tags too, existing tags will be removed
 ```
 
 
 ## Examples
 Copy all parameters under /dev to a new profile:
 ```
 aws-ssm-copy --profile binx-io --recursive /dev
```

### Comparing `aws-ssm-copy-0.4.0/setup.py` & `aws-ssm-copy-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), 'r') as f:
     long_description = f.read()
 
-version = "0.4.0"
+version = "0.5.0"
 
 setup(
     name='aws-ssm-copy',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     entry_points={
         'console_scripts': ['aws-ssm-copy = aws_ssm_copy:main']
@@ -25,12 +25,12 @@
     version=version,
     description='Copy AWS Parameter Store parameters',
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     zip_safe=False,
     platforms='any',
-    install_requires=['boto3' ],
+    install_requires=['boto3'],
     author='Mark van Holsteijn',
     author_email='markvanholsteijn@binx.io',
     url='https://github.com/binxio/aws-ssm-copy',
 )
```

### Comparing `aws-ssm-copy-0.4.0/src/aws_ssm_copy/ssm_copy.py` & `aws-ssm-copy-0.5.0/src/aws_ssm_copy/ssm_copy.py`

 * *Files 19% similar despite different names*

```diff
@@ -100,28 +100,68 @@
                 result[parameter["Name"]] = parameter
 
         if len(result) == 0:
             sys.stderr.write("ERROR: {} not found.\n".format(arg))
             sys.exit(1)
         return result
 
+    def copy_tags(self,
+                  name: str,
+                  new_name: str
+                  ):
+        """
+        copy the tags of the parameter `name` to `new_name`. Existing tags on `new_name` will be
+        removed.
+        """
+        source_tag_list = self.source_ssm.list_tags_for_resource(
+            ResourceType='Parameter',
+            ResourceId=name
+        )['TagList']
+        source_tags = {tag['Key']: tag['Value'] for tag in source_tag_list}
+
+        existing_tags_list = self.target_ssm.list_tags_for_resource(
+            ResourceType='Parameter',
+            ResourceId=new_name
+        )['TagList']
+        target_tags = {tag['Key']: tag['Value'] for tag in existing_tags_list}
+
+        to_remove = list(filter(lambda key: key not in source_tags, target_tags.keys()))
+        to_add = list(filter(lambda key: key not in target_tags or source_tags[key] != target_tags[key], source_tags.keys()))
+        if to_remove:
+            sys.stdout.write(f"{'DRY-RUN' if self.dry_run else 'INFO'}: remove tags {','.join(to_remove)} from {new_name}\n")
+
+            self.target_ssm.remove_tags_from_resource(
+                ResourceType='Parameter',
+                ResourceId=new_name,
+                TagKeys=to_remove
+            )
+        if to_add:
+            sys.stdout.write(f"{'DRY-RUN' if self.dry_run else 'INFO'}: adding tags {','.join(to_add)} from {new_name}\n")
+            self.target_ssm.add_tags_to_resource(
+                ResourceType='Parameter',
+                ResourceId=new_name,
+                Tags=[{'Key': key, 'Value': source_tags[key]} for key in to_add]
+            )
+
     def copy(
         self,
         args,
         recursive,
         one_level,
         overwrite,
         key_id=None,
         clear_kms_key=False,
         keep_going=False,
+        with_tags=False,
     ):
         for arg in args:
             parameters = self.load_source_parameters(arg, recursive, one_level)
             for name in parameters:
                 value = self.source_ssm.get_parameter(Name=name, WithDecryption=True)
+
                 parameter = parameters[name]
                 parameter["Value"] = value["Parameter"]["Value"]
 
                 if "KeyId" in parameter and key_id is not None:
                     parameter["KeyId"] = key_id
                 if "KeyId" in parameter and clear_kms_key:
                     del parameter["KeyId"]
@@ -136,19 +176,21 @@
                         # an empty policies list causes an exception
                         del parameter["Policies"]
                 parameter["Overwrite"] = overwrite
                 parameter = rename_parameter(parameter, arg, self.target_path)
                 new_name = parameter["Name"]
                 if self.dry_run:
                     sys.stdout.write(f"DRY-RUN: copying {name} to {new_name}\n")
+                    self.copy_tags(name, new_name)
                 else:
-
                     try:
                         self.target_ssm.put_parameter(**parameter)
                         sys.stdout.write(f"INFO: copied {name} to {new_name}\n")
+                        if with_tags:
+                            self.copy_tags(name, new_name)
                     except self.target_ssm.exceptions.ParameterAlreadyExists as e:
                         if not keep_going:
                             sys.stderr.write(
                                 f"ERROR: failed to copy {name} to {new_name} as it already exists: specify --overwrite or --keep-going\n"
                             )
                             exit(1)
                         else:
@@ -242,14 +284,22 @@
         key_group.add_argument(
             "--clear-key-id",
             "-C",
             dest="clear_key_id",
             action="store_true",
             help="clear the KMS key id associated with the parameter",
         )
+        key_group.add_argument(
+            "--with-tags",
+            "-W",
+            dest="with_tags",
+            action="store_true",
+            help="copy the tags of the parameters too",
+        )
+
         parser.add_argument(
             "parameters", metavar="PARAMETER", type=str, nargs="+", help="source path"
         )
         options = parser.parse_args()
 
         try:
             self.connect_to_source(options.source_profile, options.source_region)
@@ -260,14 +310,15 @@
                 options.parameters,
                 options.recursive,
                 options.one_level,
                 options.overwrite,
                 options.key_id,
                 options.clear_key_id,
                 options.keep_going,
+                options.with_tags
             )
         except ClientError as e:
             sys.stderr.write("ERROR: {}\n".format(e))
             sys.exit(1)
 
 
 def main():
```

### Comparing `aws-ssm-copy-0.4.0/src/aws_ssm_copy.egg-info/PKG-INFO` & `aws-ssm-copy-0.5.0/src/aws_ssm_copy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ssm-copy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Copy AWS Parameter Store parameters
 Home-page: https://github.com/binxio/aws-ssm-copy
 Author: Mark van Holsteijn
 Author-email: markvanholsteijn@binx.io
 License: UNKNOWN
 Platform: any
 Description-Content-Type: text/markdown
@@ -34,14 +34,15 @@
 --source-region REGION to get the parameters from
 --source-profile NAME  to obtain the parameters from
 --region REGION        to copy the parameters to
 --profile NAME         to copy the parameters to
 --target-path NAME     to copy the parameters to
 --key-id ID            to use for parameter values in the destination
 --clear-key-id, -C     clear the kms key id associated with the parameter
+--with-tags, -W        copy the tags too, existing tags will be removed
 ```
 
 
 ## Examples
 Copy all parameters under /dev to a new profile:
 ```
 aws-ssm-copy --profile binx-io --recursive /dev
```

