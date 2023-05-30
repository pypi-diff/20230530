# Comparing `tmp/concurrent_plugin-0.5.1-py3-none-any.whl.zip` & `tmp/concurrent_plugin-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 31184 bytes, number of entries: 17
+Zip file size: 34437 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx        2 b- defN 22-Sep-22 06:22 concurrent_plugin/__init__.py
--rw-rw-r--  2.0 unx    33825 b- defN 23-May-17 11:18 concurrent_plugin/concurrent_backend.py
+-rw-rw-r--  2.0 unx    42966 b- defN 23-May-26 16:51 concurrent_plugin/concurrent_backend.py
 -rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-12 10:10 concurrent_plugin/concurrent_core.py
 -rw-rw-r--  2.0 unx    15759 b- defN 23-Feb-15 19:34 concurrent_plugin/login.py
 -rw-rw-r--  2.0 unx     3994 b- defN 23-Jan-10 17:33 concurrent_plugin/periodic_run.py
+-rw-rw-r--  2.0 unx     2091 b- defN 23-May-23 18:02 concurrent_plugin/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Sep-22 06:22 concurrent_plugin/infinfs/__init__.py
 -rw-rw-r--  2.0 unx      990 b- defN 22-Oct-18 19:03 concurrent_plugin/infinfs/infin_download.py
 -rw-rw-r--  2.0 unx     1339 b- defN 22-Sep-22 06:22 concurrent_plugin/infinfs/infin_prefetch.py
 -rw-rw-r--  2.0 unx    10783 b- defN 22-Nov-11 07:23 concurrent_plugin/infinfs/infinfs.py
 -rw-rw-r--  2.0 unx     5326 b- defN 22-Oct-18 19:03 concurrent_plugin/infinfs/infinmount.py
 -rw-rw-r--  2.0 unx     1140 b- defN 22-Nov-11 07:23 concurrent_plugin/infinfs/mount_main.py
--rw-rw-r--  2.0 unx    16627 b- defN 23-May-17 11:12 concurrent_plugin/infinfs/mount_service.py
--rw-rw-r--  2.0 unx      307 b- defN 23-May-17 17:44 concurrent_plugin-0.5.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-17 17:44 concurrent_plugin-0.5.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx      181 b- defN 23-May-17 17:44 concurrent_plugin-0.5.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-May-17 17:44 concurrent_plugin-0.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1567 b- defN 23-May-17 17:44 concurrent_plugin-0.5.1.dist-info/RECORD
-17 files, 108770 bytes uncompressed, 28550 bytes compressed:  73.8%
+-rw-rw-r--  2.0 unx    15974 b- defN 23-May-25 20:09 concurrent_plugin/infinfs/mount_service.py
+-rw-rw-r--  2.0 unx      307 b- defN 23-May-30 06:13 concurrent_plugin-0.5.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-30 06:13 concurrent_plugin-0.5.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      181 b- defN 23-May-30 06:13 concurrent_plugin-0.5.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-May-30 06:13 concurrent_plugin-0.5.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1650 b- defN 23-May-30 06:13 concurrent_plugin-0.5.2.dist-info/RECORD
+18 files, 119432 bytes uncompressed, 31675 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -9,14 +9,17 @@
 
 Filename: concurrent_plugin/login.py
 Comment: 
 
 Filename: concurrent_plugin/periodic_run.py
 Comment: 
 
+Filename: concurrent_plugin/utils.py
+Comment: 
+
 Filename: concurrent_plugin/infinfs/__init__.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/infin_download.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/infin_prefetch.py
@@ -30,23 +33,23 @@
 
 Filename: concurrent_plugin/infinfs/mount_main.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/mount_service.py
 Comment: 
 
-Filename: concurrent_plugin-0.5.1.dist-info/METADATA
+Filename: concurrent_plugin-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: concurrent_plugin-0.5.1.dist-info/WHEEL
+Filename: concurrent_plugin-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: concurrent_plugin-0.5.1.dist-info/entry_points.txt
+Filename: concurrent_plugin-0.5.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: concurrent_plugin-0.5.1.dist-info/top_level.txt
+Filename: concurrent_plugin-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: concurrent_plugin-0.5.1.dist-info/RECORD
+Filename: concurrent_plugin-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concurrent_plugin/concurrent_backend.py

```diff
@@ -6,21 +6,23 @@
 import docker
 from os.path import expanduser
 import requests
 from requests.exceptions import HTTPError
 from urllib.parse import urlparse
 import base64
 import uuid
+import concurrent_plugin.utils
 
 # Use lazy % or % formatting in logging functionspylint(logging-format-interpolation)
 # Use lazy % or .format() or % formatting in logging functionspylint(logging-fstring-interpolation)
 # pylint: disable=logging-not-lazy, logging-format-interpolation, logging-fstring-interpolation
 
 from mlflow.projects.backend.abstract_backend import AbstractBackend
 import mlflow.tracking as tracking
+import mlflow.entities
 from mlflow.entities import RunStatus
 from mlflow.utils.git_utils import get_git_commit, get_git_repo_url
 from mlflow.projects.submitted_run import SubmittedRun
 from mlflow.projects.utils import (
     fetch_and_validate_project,
     get_or_create_run,
     load_project,
@@ -37,14 +39,15 @@
         MLFLOW_DOCKER_IMAGE_ID
 )
 import mlflow.projects.kubernetes
 from mlflow.projects.kubernetes import KubernetesSubmittedRun, _get_run_command, _load_kube_context
 import kubernetes
 import kubernetes.client
 from concurrent_plugin.login import get_conf, get_token, get_token_file_obj, get_env_var
+from typing import List
 
 _logger = logging.getLogger(__name__)
 
 verbose = True
 
 CONCURRENT_FUSE_MOUNT_BASE = '/mount_base_dir'
 MOUNT_SERVICE_READY_MARKER_FILE = os.path.join(CONCURRENT_FUSE_MOUNT_BASE,  '__service_ready__')
@@ -158,17 +161,36 @@
                 if (verbose):
                     _logger.info('upload_objects: Uploading ' + src_path + ' to ' + dst_path)
                 tracking.MlflowClient().log_artifact(run_id, src_path, dst_path)
     except Exception as err:
         _logger.info(str(err))
 
 class PluginConcurrentProjectBackend(AbstractBackend):
-    def run(self, project_uri, entry_point, params,
-            version, backend_config, tracking_uri, experiment_id):
+    def run(self, project_uri:str, entry_point:str, params:str,
+            version:str, backend_config:dict, tracking_uri:str, experiment_id:str):
+        """
+        for the specified 'project_uri', fetches the MLproject details into a 'working_dir'.  the fetched MLproject is then run locally or remotely using run_project() REST API
+
+        _extended_summary_
 
+        Args:
+            project_uri (str): the URI for MLFlow project file (MLproject) to be run
+            entry_point (str): entry point specified in the MLFlow project file (MLproject)
+            params (str): params specified in the MLflow project file (MLproject)
+            version (str): _description_
+            backend_config (dict): See run_eks_on_backend() for documentation
+            tracking_uri (str): MLFlow tracking URI
+            experiment_id (str): MLFlow Experiment ID
+
+        Raises:
+            ValueError: _description_
+
+        Returns:
+            _type_: _description_
+        """
         if (verbose):
             _logger.info("PluginConcurrentProjectBackend: Entered. project_uri=" + str(project_uri)\
                 + ", entry_point=" + str(entry_point)\
                 + ", params=" + str(params)\
                 + ", version=" + str(version)\
                 + ", backend_config=" + str(backend_config)\
                 + ", experiment_id=" + str(experiment_id)\
@@ -219,43 +241,71 @@
         else:
             _logger.info('Error. unknown backend type ' + backend_type)
             self.fail_run(run_id)
             rv = ParallelsSubmittedRun(active_run.info.run_id)
             rv.set_status(RunStatus.FAILED)
             return rv
 
-    def run_eks(self, run_id, backend_type, bucket_name, path_in_bucket, work_dir, project_uri, entry_point, params,
-            version, backend_config, tracking_store_uri, experiment_id, project, active_run):
+    def run_eks(self, run_id:str, backend_type:str, bucket_name:str, path_in_bucket:str, work_dir:str, project_uri:str, entry_point:str, params:str,
+            version, backend_config:dict, tracking_store_uri:str, experiment_id:str, project:str, active_run:mlflow.entities.Run):
+        """
+        _summary_
+
+        _extended_summary_
+
+        Args:
+            run_id (str): _description_
+            backend_type (str): gke|aws|HPE
+            bucket_name (str): _description_
+            path_in_bucket (str): _description_
+            work_dir (str): working directory with MLproject and its related files
+            project_uri (str): URI for MLproject file
+            entry_point (str): entry point specified in MLproject file
+            params (str): params specified in MLproject file
+            version (_type_): _description_
+            backend_config (dict): see run_eks_on_backend() for documentation
+            tracking_store_uri (str): _description_
+            experiment_id (str): _description_
+            project (_type_): the MLproject entity
+            active_run (mlflow.entities.Run): _description_
+
+        Raises:
+            ValueError: _description_
+
+        Returns:
+            _type_: _description_
+        """
+        
         kube_client_location = backend_config.get('kube-client-location', 'local')
         if kube_client_location == 'local':
             return self.run_eks_on_local(backend_type, project_uri, entry_point, params, version,
                     backend_config, tracking_store_uri, experiment_id, project, active_run, work_dir)
         elif kube_client_location == 'backend':
             return self.run_eks_on_backend(run_id, backend_type, bucket_name, path_in_bucket, work_dir, project_uri,
                     entry_point, params, version, backend_config, tracking_store_uri, experiment_id,
                     project, active_run)
         else:
             raise ValueError('kube_client_location must be either local or backend')
 
     def run_eks_on_backend(self, run_id, backend_type, bucket_name, path_in_bucket, work_dir, project_uri, entry_point, params,
-            version, backend_config, tracking_store_uri, experiment_id, project, active_run):
+            version, backend_config:dict, tracking_store_uri:str, experiment_id:str, project:str, active_run:mlflow.entities.Run):
         """
-        calls the run_project() REST API to run the MLProject, instead of running the MLProject locally.  
+        calls upload_objects() to upload MLproject and its files.  Then calls run_project() REST API to run the MLProject in the target compute, instead of running the MLProject locally.  run_project() REST API's invocation parameters are derived from 'backend_config'
 
         Args:
             run_id (_type_): _description_
             backend_type (_type_): _description_
             bucket_name (_type_): _description_
             path_in_bucket (_type_): _description_
-            work_dir (_type_): _description_
+            work_dir (_type_): working directory with MLproject and related files that need to be uploaded to the Mlflow Run.   Eventually run_eks_on_local() will use the contents of this artifact directory to run the MLproject
             project_uri (_type_): _description_
             entry_point (_type_): _description_
             params (_type_): _description_
             version (_type_): _description_ 
-            backend_config (_type_): {"backend-type": "HPE", "kube-context": "unused", "kube-namespace": "parallelsns", "resources.requests.memory": "1024Mi", "kube-client-location": "backend"}
+            backend_config (dict): {"backend-type": "HPE|aws|gke", "kube-context": "unused", "kube-namespace": "parallelsns", "kube-client-location": "backend|local", 'kube-job-template-path':xxxx, 'kube-namespace':xxxxx, 'resources.limits.cpu':500m, 'resources.limits.memory':"1024Mi", 'resources.limits.hugepages':xxxxx, 'resources.limits.nvidia.com/gpu':xxxxx, 'resources.requests.cpu':500m, 'resources.requests.memory':"1024Mi", 'resources.requests.hugepages':xxxxx, 'resources.requests.nvidia.com/gpu':xxxxx, 'kube-context':xxxx, 'run-id':xxxxx, 'parent_run_id':xxxxx, 'last_in_chain_of_xforms':xxxxx, 'INPUT_DATA_SPEC': base64(xxxxx), 'repository-uri':'git_repo_uri', 'git-commit':xxxx, 'IMAGE_TAG':'docker_image_with_tag', IMAGE_DIGEST:xxxx, STORAGE_DIR:xxxx}.  
             tracking_store_uri (_type_): _description_
             experiment_id (_type_): _description_
             project (_type_): _description_
             active_run (_type_): _description_
 
         Raises:
             ValueError: _description_
@@ -278,14 +328,15 @@
 
         if 'kube-job-template-path' in backend_config:
             _logger.info('Using kubernetes job template file ' + backend_config['kube-job-template-path'])
             body['kube_job_template_contents'] = base64.b64encode(
                     open(backend_config.get('kube-job-template-path'), "r").read().encode('utf-8')).decode('utf-8')
             with open(backend_config.get('kube-job-template-path'), "r") as yf:
                 yml = yaml.safe_load(yf)
+            _logger.info(f"contents of {backend_config.get('kube-job-template-path')} = {yml}")
             if 'metadata' in yml and 'namespace' in yml['metadata']:
                 body['namespace'] = yml['metadata']['namespace']
                 _logger.info('namespace obtained from job template: ' + body['namespace'])
                 if 'kube-namespace' in backend_config:
                     if body['namespace'] != backend_config['kube-namespace']:
                         _logger.info('Error. mismatch between namespace in backend configuration and job template')
                         self.fail_run(run_id)
@@ -373,15 +424,15 @@
 
         Args:
             backend_type (_type_): _description_
             project_uri (_type_): _description_
             entry_point (_type_): _description_
             params (_type_): _description_
             version (_type_): _description_
-            backend_config (_type_): _description_
+            backend_config (_type_): see run_eks_on_backend() documentation
             tracking_store_uri (_type_): _description_
             experiment_id (_type_): _description_
             project (_type_): _description_
             active_run (_type_): _description_
             work_dir (_type_): _description_
 
         Returns:
@@ -394,25 +445,31 @@
         input_data_spec = backend_config.get('INPUT_DATA_SPEC')
         if (verbose):
             _logger.info("PluginConcurrentProjectBackend.run_eks_on_local: kube-context=" + str(kube_context)\
                 + ", repository-uri=" + str(repository_uri)\
                 + ", git-commit=" + str(git_commit)\
                 + ", kube-job-template-path=" + str(kube_job_template_path)\
                 + ", input_data_spec=" + str(input_data_spec))
+            if kube_job_template_path and os.path.exists(kube_job_template_path):
+                with open(kube_job_template_path, "r") as job_template:
+                    yaml_obj = yaml.safe_load(job_template.read())
+                    _logger.info(f"contents of {kube_job_template_path}={yaml_obj}")
 
         from mlflow.projects.docker import (
             validate_docker_env,
             validate_docker_installation
         )
         
         tracking.MlflowClient().set_tag(active_run.info.run_id, MLFLOW_PROJECT_ENV, "docker")
         validate_docker_env(project)
         validate_docker_installation()
 
+        # kube_config is a copy of backend_config with one additional key: 'kube-job-template', which is contents of backend_config['kube-job-template-path']
         kube_config = mlflow.projects._parse_kubernetes_config(backend_config)
+        _logger.info(f"kube_config={kube_config}")
 
         env_vars:dict = get_run_env_vars(run_id=active_run.info.run_uuid, experiment_id=active_run.info.experiment_id)
         for envvar_name in ['DATABRICKS_HOST', 'DATABRICKS_TOKEN']:
             if os.getenv(envvar_name): env_vars[envvar_name] = os.getenv(envvar_name)
     
         #If a local image has already been created/pulled, kube_config should have it
         if 'IMAGE_TAG' in backend_config and 'IMAGE_DIGEST' in backend_config:
@@ -514,24 +571,59 @@
             _logger.info("Temporary docker context file %s was not deleted.", build_ctx_path)
         tracking.MlflowClient().set_tag(run_id, MLFLOW_DOCKER_IMAGE_URI, image_uri)
         tracking.MlflowClient().set_tag(run_id, MLFLOW_DOCKER_IMAGE_ID, image.id)
         return image
 
     def run_eks_job(
         self,
-        project_name,
-        active_run,
-        image_tag,
-        image_digest,
-        command,
-        env_vars,
-        input_data_spec,
-        kube_context=None,
-        job_template=None
-    ):
+        project_name:str,
+        active_run:mlflow.entities.Run,
+        image_tag:str,
+        image_digest:str,
+        command:List[str],
+        env_vars:dict,
+        input_data_spec:str,
+        kube_context:str=None,
+        job_template:dict=None
+    ) -> KubernetesSubmittedRun:
+        """
+        creates a k8s job using the specified 'job_template' and the arguments to this method and runs it in the k8s cluster.
+
+        
+
+        Args:
+            project_name (str): name of the project
+            active_run (mlflow.entities.Run): the mlflow Run for running this MLProject
+            image_tag (str): the docker image for the MLProject to be used in the k8s job
+            image_digest (str): digtest of the docker image
+            command (List[str]): command to be used in k8s job
+            env_vars (dict): the env vars to be used in the k8s job
+            input_data_spec (str): input_data_spec injected into the k8s job: used to setup inputs to MLProject
+            kube_context (str, optional): trying to load either the context passed as arg or, if None, the one provided as env var `KUBECONFIG` or in `~/.kube/config`
+            job_template (dict, optional): the job_template to use to create the k8s job. Defaults to None.
+
+        Returns:
+            KubernetesSubmittedRun: _description_
+        """
+        # 2023-05-24 05:05:40,641 - 353 - concurrent_plugin.concurrent_backend - INFO - run_eks_job: Entered. project_name=docker-example, 
+        # active_run=<Run: data=<RunData: metrics={}, params={'alpha': '0.62', 'l1_ratio': '0.02'}, tags={'mlflow.gitRepoURL': 'https://github.com/jagane-infinstor/mlflow-example-docker.git',
+        #  'mlflow.project.backend': 'concurrent-backend',
+        #  'mlflow.project.entryPoint': 'main',
+        #  'mlflow.source.git.commit': '5ebaa6d3130fec010e49c19b948468eff0aafe51',
+        #  'mlflow.source.git.repoURL': 'https://github.com/jagane-infinstor/mlflow-example-docker.git',
+        #  'mlflow.source.name': 'https://github.com/jagane-infinstor/mlflow-example-docker.git',
+        #  'mlflow.source.type': 'PROJECT',
+        #  'mlflow.user': 'raj-hpe'}>, info=<RunInfo: artifact_uri='s3://infinstor-mlflow-artifacts-hpe.infinstor.com/mlflow-artifacts/raj-hpe/1/1-16848593352850000000055', end_time=None, experiment_id='1', lifecycle_stage='active', run_id='1-16848593352850000000055', run_name='', run_uuid='1-16848593352850000000055', start_time=1684859335285, status='RUNNING', user_id='raj-hpe'>>, 
+        # image_tag=10.241.17.223:31386/mlflow/raj-hpe/ff16d546a3daeea3469ac955073c96fb4d990e60522d7e6ab03939b331317f21:5ebaa6d, 
+        # image_digest=sha256:1d0f14a49dcb17b304bf5d9ec5680de8494797c4c3d697eaff04166349744fa8, 
+        # command=['python train.py --alpha 0.62 --l1-ratio 0.02'], 
+        # env_vars={'MLFLOW_RUN_ID': '1-16848593352850000000055', 'MLFLOW_TRACKING_URI': 'infinstor://mlflow.hpe.infinstor.com', 'MLFLOW_EXPERIMENT_ID': '1'}, 
+        # input_data_spec=W10=, 
+        # kube_context=None, 
+        # job_template={'apiVersion': 'batch/v1', 'kind': 'Job', 'metadata': {'name': '{replaced with MLflow Project name}', 'namespace': 'parallelsns'}, 'spec': {'backoffLimit': 0, 'template': {'spec': {'shareProcessNamespace': True, 'containers': [{'name': '{replaced with MLflow Project name}', 'image': '{replaced with URI of Docker image created during Project execution}', 'command': ['{replaced with MLflow Project entry point command}'], 'imagePullPolicy': 'IfNotPresent', 'resources': {'limits': {'memory': '1024Mi'}}}, {'name': 'sidecar-1-16848593352850000000055', 'image': '10.241.17.223:31386/mlflow/raj-hpe/ff16d546a3daeea3469ac955073c96fb4d990e60522d7e6ab03939b331317f21:5ebaa6d@sha256:1d0f14a49dcb17b304bf5d9ec5680de8494797c4c3d697eaff04166349744fa8', 'lifecycle': {'type': 'Sidecar'}, 'command': ['python'], 'args': ['-m', 'concurrent_plugin.infinfs.mount_service'], 'imagePullPolicy': 'IfNotPresent', 'env': [{'name': 'MLFLOW_TRACKING_URI', 'value': 'infinstor://mlflow.hpe.infinstor.com'}, {'name': 'MLFLOW_RUN_ID', 'value': '1-16848593352850000000055'}, {'name': 'MLFLOW_CONCURRENT_URI', 'value': 'https://concurrent.hpe.infinstor.com'}, {'name': 'DAG_EXECUTION_ID', 'value': 'None'}, {'name': 'DAGID', 'value': 'None'}, {'name': 'MY_POD_NAME', 'valueFrom': {'fieldRef': {'fieldPath': 'metadata.name'}}}, {'name': 'MY_POD_NAMESPACE', 'valueFrom': {'fieldRef': {'fieldPath': 'metadata.namespace'}}}], 'securityContext': {'privileged': True, 'capabilities': {'add': ['SYS_ADMIN']}}, 'resources': {'limits': {'cpu': '250m', 'memory': '1024Mi'}}}], 'priorityClassName': 'concurrent-high-non-preempt-prio', 'restartPolicy': 'Never'}}}}
         _logger.info('run_eks_job: Entered. project_name=' + str(project_name)\
                 + ', active_run=' + str(active_run) + ', image_tag=' + str(image_tag)\
                 + ', image_digest=' + str(image_digest) + ', command=' + str(command)\
                 + ', env_vars=' + str(env_vars) + ', input_data_spec=' + str(input_data_spec)\
                 + ', kube_context=' + str(kube_context) + ', job_template=' + str(job_template))
         if os.getenv('PERIODIC_RUN_NAME'):
           env_vars['PERIODIC_RUN_NAME'] = os.getenv('PERIODIC_RUN_NAME')
@@ -546,14 +638,19 @@
         env_vars['DAGID'] = os.getenv('DAGID')
         # PYTHONUNBUFFERED is an environment variable in Python that can be used to disable output buffering for all streams. When this variable is set to a non-empty string, Python automatically sets the PYTHONUNBUFFERED flag, which forces Python to disable buffering for sys.stdout and sys.stderr.
         if os.getenv("PYTHONUNBUFFERED"): env_vars['PYTHONUNBUFFERED'] = os.getenv("PYTHONUNBUFFERED")
         
         job_template = mlflow.projects.kubernetes._get_kubernetes_job_definition(
             project_name, image_tag, image_digest, _get_run_command(command), env_vars, job_template
         )
+        if os.getenv("PYTHONUNBUFFERED") and len(job_template["spec"]["template"]["spec"]["containers"]) > 1: # sidecar container is present:
+            if "env" not in job_template["spec"]["template"]["spec"]["containers"][1].keys():
+                job_template["spec"]["template"]["spec"]["containers"][1]["env"] = []
+            job_template["spec"]["template"]["spec"]["containers"][1]["env"] += [{'name':'PYTHONUNBUFFERED', 'value':os.getenv('PYTHONUNBUFFERED')}]
+
         job_name = job_template["metadata"]["name"]
         job_namespace = job_template["metadata"]["namespace"]
         _load_kube_context(context=kube_context)
         kubernetes.client.configuration.retries = 10
         print(f'run_eks_job: Overrode default kubernetes.client.configuration.retries to 10')
 
         core_api_instance = kubernetes.client.CoreV1Api()
@@ -612,15 +709,15 @@
         volume_mounts.append(kubernetes.client.V1VolumeMount(mount_path=CONCURRENT_FUSE_MOUNT_BASE,
                                                              name='sharedmount',
                                                              mount_propagation='HostToContainer'))
         side_car_volume_mounts.append(kubernetes.client.V1VolumeMount(mount_path=CONCURRENT_FUSE_MOUNT_BASE,
                                                     name='sharedmount',
                                                     mount_propagation='Bidirectional'))
 
-        job_template["spec"]["ttlSecondsAfterFinished"] = int(os.getenv("CONCURRENT_KUBE_JOB_TEMPLATE_TTL", "7200"))
+        job_template["spec"]["ttlSecondsAfterFinished"] = int(os.getenv("CONCURRENT_KUBE_JOB_TEMPLATE_TTL", "86400"))
         
         if os.getenv("CONCURRENT_PRIVILEGED_MLFLOW_CONTAINER"): 
             # create 'securityContext' if needed
             if not job_template["spec"]["template"]["spec"]["containers"][0].get('securityContext'):
                 job_template["spec"]["template"]["spec"]["containers"][0]['securityContext'] = {}
             job_template["spec"]["template"]["spec"]["containers"][0]['securityContext']['privileged'] = True
             
@@ -649,22 +746,25 @@
         job_template["spec"]["template"]["spec"]["serviceAccountName"] = 'k8s-serviceaccount-for-users-' + job_namespace
 
         job_template["spec"]["template"]["spec"]["volumes"] = [
                     kubernetes.client.V1Volume(name="parallels-token-file", secret=kubernetes.client.V1SecretVolumeSource(secret_name=token_secret_name)),
                     kubernetes.client.V1Volume(name="aws-creds-file", secret=kubernetes.client.V1SecretVolumeSource(secret_name=awscreds_secret_name)),
                     kubernetes.client.V1Volume(name='sharedmount', empty_dir=kubernetes.client.V1EmptyDirVolumeSource())
                 ]
-        if input_data_spec:
+        if input_data_spec: 
             job_template["spec"]["template"]["spec"]["volumes"].append(
                     kubernetes.client.V1Volume(name=input_spec_name, secret=kubernetes.client.V1SecretVolumeSource(secret_name=input_spec_name)))
         # if AWS IAM Roles Anywhere is configured, set it up
         if os.getenv("IAM_ROLES_ANYWHERE_SECRET_NAME"):
             job_template["spec"]["template"]["spec"]["volumes"].append(
                 kubernetes.client.V1Volume(name="iam-roles-anywhere-volume", secret=kubernetes.client.V1SecretVolumeSource(secret_name=os.getenv("IAM_ROLES_ANYWHERE_SECRET_NAME"))))
-            
-        _logger.info('run_eks_job: job_template=' + str(job_template))
+        
+        _logger.info(f'run_eks_job: job_template before filtering= { job_template }')
+        # Note: job_template is not just a 'dict' containing 'lists' and 'scalars'.  It has other objects like V1Volume and others.  so filter_empty_in_dict_list_scalar() will not filter correctly.  Also yaml.safe_dump() will not be able to dump such a hybrid correctly as a string
+        #_logger.info(f'run_eks_job: job_template after  filtering= { yaml.safe_dump(concurrent_plugin.utils.filter_empty_in_dict_list_scalar(job_template)) }')
         api_instance = kubernetes.client.BatchV1Api()
-        resp = api_instance.create_namespaced_job(namespace=job_namespace, body=job_template, pretty=True)
+        resp:kubernetes.client.V1Job = api_instance.create_namespaced_job(namespace=job_namespace, body=job_template, pretty=True)
         _logger.info( resp.kind + " " + resp.metadata.name +" created." )
+        _logger.info(f'run_eks_job: created job=\n{ yaml.safe_dump(concurrent_plugin.utils.filter_empty_in_dict_list_scalar(resp.to_dict())) }')
         tracking.MlflowClient().log_param(active_run.info.run_id, 'kubernetes.job_name', job_name)
         tracking.MlflowClient().log_param(active_run.info.run_id, 'kubectl.get_pods', 'kubectl -n ' + str(job_namespace) + ' get pods --selector=job-name=' + job_name)
         return KubernetesSubmittedRun(active_run.info.run_id, job_name, job_namespace)
```

## concurrent_plugin/infinfs/mount_service.py

```diff
@@ -1,18 +1,17 @@
 import socket
 import time
 import os
-import traceback
-from typing import Any, Union
 from concurrent_plugin.infinfs import infinmount
 import json
 import yaml
 from mlflow.tracking import MlflowClient
 import psutil
 from concurrent_plugin.concurrent_backend import MOUNT_SERVICE_READY_MARKER_FILE
+import concurrent_plugin.utils
 import logging
 import requests
 import subprocess
 # importing it as kubernetes.client since 'client' is used in the code in some places as the Mlflow client.  this mlflow 'client' conflicts with 'from kubernetes import client'.  Need to cleanup.
 import kubernetes.client
 from kubernetes import client, config
 import dpath
@@ -109,70 +108,27 @@
         client = MlflowClient()
         client.log_artifact(run_id, tmp_log_file, artifact_path='.concurrent/logs')
     except Exception as ex:
         logger.warning("Failed upload logs for {}, {}: {}".format(run_id, pod_name, ex))
 
 
 def update_mlflow_run(run_id, status):
+    logger.info(f"update_mlflow_run(): updating mlflow run-id={run_id} with status={status}")
     client = MlflowClient()
     client.set_terminated(run_id, status)
 
-def _filter_empty_in_dict_list_scalar(dict_list_scalar:Union[list, dict, Any]) -> Union[list, dict, Any]:
-    """
-    given a 'dict' or 'list' as input, removes all elements in these containers that are empty: scalars with None, strings that are '', lists and dicts that are empty.  Note that the filtering is in-place: modifies the passed list or dict
-
-    Args:
-        dict_list_scalar (Union[list, dict, Any]): see above
-    """
-    try:
-        # depth first traveral
-        if isinstance(dict_list_scalar, dict):
-            keys_to_del:list = []
-            for k in dict_list_scalar.keys():  
-                _filter_empty_in_dict_list_scalar(dict_list_scalar[k])
-                
-                # check if the 'key' is now None or empty.  If so, remove the 'key'
-                if not dict_list_scalar[k]: 
-                    # cannont do dict.pop(): RuntimeError: dictionary changed size during iteration
-                    # dict_list_scalar.pop(k)
-                    keys_to_del.append(k)
-            
-            # now delete the keys from the map
-            for k in keys_to_del:
-                dict_list_scalar.pop(k)
-            
-            return dict_list_scalar
-        elif isinstance(dict_list_scalar, list):
-            i = 0; length = len(dict_list_scalar)
-            while i < length: 
-                _filter_empty_in_dict_list_scalar(dict_list_scalar[i])
-            
-                # check if element is now None (if scalar) or empty (if list or dict).  If so, remove the element from the list
-                if not dict_list_scalar[i]:
-                    dict_list_scalar.remove(dict_list_scalar[i])
-                    i -= 1; length -= 1
-                
-                i += 1
-            return dict_list_scalar
-        else: # this must be a non container, like int, str, datatime.datetime
-            return dict_list_scalar
-    except Exception as e:
-        # some excpetion, just log it..
-        print(f"_filter_empty_in_dict_list_scalar(): Caught exception: {e}")
-        traceback.print_exc()
-
 def log_describe_pod(k8s_client:kubernetes.client.CoreV1Api, run_id, pod_name, pod_namespace, pod_info:kubernetes.client.V1Pod):
     describe_file = "/tmp/describe-" + pod_name + ".txt"
     try:
         events:kubernetes.client.V1EventList = k8s_client.list_namespaced_event(pod_namespace, field_selector=f'involvedObject.name={pod_name}')
         with open(describe_file, "w") as fh:
             pod_info_dict:dict = pod_info.to_dict()
             # remove metadata/managed_fields key
             if pod_info_dict.get('metadata') and pod_info_dict.get('metadata').get('managed_fields'): pod_info_dict['metadata'].pop('managed_fields')            
-            _filter_empty_in_dict_list_scalar(pod_info_dict)
+            concurrent_plugin.utils.filter_empty_in_dict_list_scalar(pod_info_dict)
             fh.write(yaml.safe_dump(pod_info_dict))
             
             events_dict:dict = events.to_dict()
             # api_version: v1
             # kind: EventList
             # metadata:
             #   resource_version: '292715'
@@ -209,16 +165,16 @@
             # 
             # remove unwanted fields from the eventList
             for path_to_del in '/metadata/managed_fields','/items/*/metadata', '/items/*/involved_object':
                 try:
                     # Given a obj, delete all elements that match the glob.  Returns the number of deleted objects. Raises PathNotFound if no paths are found to delete.
                     dpath.delete(events_dict, path_to_del)
                 except dpath.PathNotFound as e:
-                    print(f"log_describe_pod(): path_to_del={path_to_del}; exception={e}")
-            _filter_empty_in_dict_list_scalar(events_dict)
+                    print(f"log_describe_pod(): path_to_del={path_to_del}; exception={e}; ignoring exception and continuing..")
+            concurrent_plugin.utils.filter_empty_in_dict_list_scalar(events_dict)
             fh.write(yaml.safe_dump(events_dict))
             
         client = MlflowClient()
         client.log_artifact(run_id, describe_file, artifact_path='.concurrent/logs')
     except Exception as ex:
         logger.warning('Failed to log describe pod, try again later: ' + str(ex))
         return
@@ -235,18 +191,44 @@
         task_container_name = pod_info.spec.containers[task_index].name
         side_car_container_name = pod_info.spec.containers[sidecar_index].name
         log_describe_pod(k8s_client, run_id, pod_name, pod_namespace, pod_info)
         upload_logs_for_pod(k8s_client, run_id, pod_name, pod_namespace, f"/tmp/run-logs-{log_suffix}.txt",
                             container_name=task_container_name)
         upload_logs_for_pod(k8s_client, run_id, pod_name, pod_namespace, f"/tmp/sidecar-logs-{log_suffix}.txt",
                             container_name=side_car_container_name)
-        task_container_status = pod_info.status
-        container_statuses = task_container_status.container_statuses
-        task = container_statuses[task_index]
-        task_container_state = task.state
+        # status:
+        #   conditions:
+        #   - lastProbeTime: null
+        #     .
+        #     .
+        #   containerStatuses:
+        #   - containerID: containerd://9e180784bc5b47d294c022e055b36de7b11b8f297740580ae44ba69b5c56a6b7
+        #     .
+        #     .
+        #     name: sidecar-xxxx
+        #     state:
+        #       running:
+        #         startedAt: "2023-05-26T06:38:17Z"
+        #   - containerID: containerd://23c749e123d44b928429cf4193108976f2f479ad4a830b1745e894a2bb67a34f
+        #     .
+        #     .
+        #     name: userbucket-xxxx
+        #     state:
+        #       terminated:
+        #         containerID: containerd://23c749e123d44b928429cf4193108976f2f479ad4a830b1745e894a2bb67a34f
+        #         exitCode: 0
+        #         .
+        #         .
+        pod_info_status = pod_info.status
+        container_statuses = pod_info_status.container_statuses
+        # recompute task_index and sidecar_index for the array 'status/container_statuses'.  Earlier computed index using 'spec/containers' will not always be valid for this array .
+        task_index=0; sidecar_index=1
+        if container_statuses[0].name.startswith('sidecar-'): sidecar_index=0; task_index=1
+        task_cont_status = container_statuses[task_index]
+        task_container_state = task_cont_status.state
         if task_container_state.running:
             print(f"Task container is in running state. Continuing to loop")
             return True
         elif task_container_state.terminated:
             print(f"Task container is in terminated state. Exiting loop")
             return False
         elif task_container_state.waiting:
@@ -257,17 +239,18 @@
             return True
     except Exception as ex:
         print(f"_fetch_upload_pod_status_logs: caught {ex}. Continuing to loop")
         return True # continue looping
 
 def get_task_exit_code(k8s_client, pod_name, pod_namespace, num_attempt=1):
     max_attempts = 3
-    pod_info = k8s_client.read_namespaced_pod(pod_name, pod_namespace)
+    pod_info:client.V1Pod = k8s_client.read_namespaced_pod(pod_name, pod_namespace)
     try:
-        if pod_info.spec.containers[1].name.startswith('sidecar-'):
+        # see yaml further above for pod/status/containter_statuses structure
+        if pod_info.status.container_statuses[1].name.startswith('sidecar-'):
             exitCode = pod_info.status.container_statuses[0].state.terminated.exit_code
         else:
             exitCode = pod_info.status.container_statuses[1].state.terminated.exit_code
         logger.info("Task container finished with exitCode " + str(exitCode))
         return exitCode
     except Exception as ex:
         logger.error("Exception in getting exit code " + str(ex))
```

## Comparing `concurrent_plugin-0.5.1.dist-info/RECORD` & `concurrent_plugin-0.5.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 concurrent_plugin/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
-concurrent_plugin/concurrent_backend.py,sha256=jtiJST2I56ZNGARles29-grG-D2kk9WFHMlw9MwG9kc,33825
+concurrent_plugin/concurrent_backend.py,sha256=ytxbHgMGTmasGLxQp1Fdtkq9YOaCiEVb5sD7J71NMmU,42966
 concurrent_plugin/concurrent_core.py,sha256=ECXT0b11j8L5kgWAxxyW6gg6gUK9d_TGOf_AibCb27k,16820
 concurrent_plugin/login.py,sha256=yBdoKr_9Uiq4DFPHmQjJEBGS61F2fw79QIL8c3hy5Vg,15759
 concurrent_plugin/periodic_run.py,sha256=Ud66-3AtnonAO6oOhcn2EwJQPfbljcrlCQeR23ELH1c,3994
+concurrent_plugin/utils.py,sha256=NpAWse8mKJkP_cyxLuCFizfVe2JjuyWkQWRGbBRjf9w,2091
 concurrent_plugin/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 concurrent_plugin/infinfs/infin_download.py,sha256=6yILg2brDNDNMFGqayFHIshB4cl25byn5dal0QI7JKQ,990
 concurrent_plugin/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 concurrent_plugin/infinfs/infinfs.py,sha256=3xId2Ocp7UJv7ntBgpr-KCFv5wGJQFw2m8csamIHiYY,10783
 concurrent_plugin/infinfs/infinmount.py,sha256=Y9BPuggy0P9gz-kYH2ZhLy24Z1WTsw7GgU3rgH7JSsY,5326
 concurrent_plugin/infinfs/mount_main.py,sha256=ehL8zXZ1HRviaukp753TjJ6pFCtO9uUfUIjx8yfUHVE,1140
-concurrent_plugin/infinfs/mount_service.py,sha256=iPrGlkx4AS3aauPii77UZ7F09bfynQMnzxyZFOg02B8,16627
-concurrent_plugin-0.5.1.dist-info/METADATA,sha256=q01_DwrFNlEg3r8vIOHu0GT-bWxAmZbeXByq4hTsH0s,307
-concurrent_plugin-0.5.1.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
-concurrent_plugin-0.5.1.dist-info/entry_points.txt,sha256=1x__D3G335a8YKoEFWsCaUHB-H1IqgvVq07ga4TgtGk,181
-concurrent_plugin-0.5.1.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
-concurrent_plugin-0.5.1.dist-info/RECORD,,
+concurrent_plugin/infinfs/mount_service.py,sha256=G6jpVhFClkiwAoUyp4R35wTrhOzg23MA5-XZkyAWHX0,15974
+concurrent_plugin-0.5.2.dist-info/METADATA,sha256=HLWfzuPTFvxoAvlQWfnNC7FMYmfsVz8AqTdCLs7GmNk,307
+concurrent_plugin-0.5.2.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
+concurrent_plugin-0.5.2.dist-info/entry_points.txt,sha256=1x__D3G335a8YKoEFWsCaUHB-H1IqgvVq07ga4TgtGk,181
+concurrent_plugin-0.5.2.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
+concurrent_plugin-0.5.2.dist-info/RECORD,,
```

