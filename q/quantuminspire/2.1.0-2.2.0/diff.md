# Comparing `tmp/quantuminspire-2.1.0.tar.gz` & `tmp/quantuminspire-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantuminspire-2.1.0.tar", last modified: Thu Jan  5 09:24:57 2023, max compression
+gzip compressed data, was "dist\quantuminspire-2.2.0.tar", last modified: Tue May 30 13:17:38 2023, max compression
```

## Comparing `quantuminspire-2.1.0.tar` & `quantuminspire-2.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-01-05 09:24:57.336718 quantuminspire-2.1.0/
--rw-rw-rw-   0        0        0    10354 2023-01-05 08:57:36.000000 quantuminspire-2.1.0/LICENSE.md
--rw-rw-rw-   0        0        0      746 2023-01-05 08:57:36.000000 quantuminspire-2.1.0/NOTICE.md
--rw-rw-rw-   0        0        0     9297 2023-01-05 09:24:57.335717 quantuminspire-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8476 2023-01-05 08:57:36.000000 quantuminspire-2.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-01-05 09:24:57.336718 quantuminspire-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2591 2023-01-05 09:12:07.000000 quantuminspire-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-05 09:24:57.300713 quantuminspire-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-01-05 09:24:57.313728 quantuminspire-2.1.0/src/quantuminspire/
--rw-rw-rw-   0        0        0       34 2023-01-05 08:57:36.000000 quantuminspire-2.1.0/src/quantuminspire/__init__.py
--rw-rw-rw-   0        0        0    58510 2023-01-05 09:12:07.000000 quantuminspire-2.1.0/src/quantuminspire/api.py
--rw-rw-rw-   0        0        0     8170 2023-01-05 09:12:07.000000 quantuminspire-2.1.0/src/quantuminspire/credentials.py
--rw-rw-rw-   0        0        0     1101 2023-01-05 08:57:36.000000 quantuminspire-2.1.0/src/quantuminspire/exceptions.py
--rw-rw-rw-   0        0        0     3501 2023-01-05 08:57:36.000000 quantuminspire-2.1.0/src/quantuminspire/job.py
-drwxrwxrwx   0        0        0        0 2023-01-05 09:24:57.324724 quantuminspire-2.1.0/src/quantuminspire/projectq/
--rw-rw-rw-   0        0        0        0 2023-01-05 08:57:36.000000 quantuminspire-2.1.0/src/quantuminspire/projectq/__init__.py
--rw-rw-rw-   0        0        0    37411 2023-01-05 09:12:07.000000 quantuminspire-2.1.0/src/quantuminspire/projectq/backend_qx.py
-drwxrwxrwx   0        0        0        0 2023-01-05 09:24:57.334717 quantuminspire-2.1.0/src/quantuminspire/qiskit/
--rw-rw-rw-   0        0        0      116 2023-01-05 08:57:36.000000 quantuminspire-2.1.0/src/quantuminspire/qiskit/__init__.py
--rw-rw-rw-   0        0        0    32100 2023-01-05 09:12:07.000000 quantuminspire-2.1.0/src/quantuminspire/qiskit/backend_qx.py
--rw-rw-rw-   0        0        0    34396 2023-01-05 09:12:07.000000 quantuminspire-2.1.0/src/quantuminspire/qiskit/circuit_parser.py
--rw-rw-rw-   0        0        0    10929 2023-01-05 08:57:36.000000 quantuminspire-2.1.0/src/quantuminspire/qiskit/measurements.py
--rw-rw-rw-   0        0        0     9550 2023-01-05 09:12:07.000000 quantuminspire-2.1.0/src/quantuminspire/qiskit/qi_job.py
--rw-rw-rw-   0        0        0     9215 2023-01-05 09:12:07.000000 quantuminspire-2.1.0/src/quantuminspire/qiskit/qi_result.py
--rw-rw-rw-   0        0        0     8785 2023-01-05 09:12:07.000000 quantuminspire-2.1.0/src/quantuminspire/qiskit/quantum_inspire_provider.py
--rw-rw-rw-   0        0        0       23 2023-01-05 09:12:07.000000 quantuminspire-2.1.0/src/quantuminspire/version.py
-drwxrwxrwx   0        0        0        0 2023-01-05 09:24:57.320721 quantuminspire-2.1.0/src/quantuminspire.egg-info/
--rw-rw-rw-   0        0        0     9297 2023-01-05 09:24:57.000000 quantuminspire-2.1.0/src/quantuminspire.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      803 2023-01-05 09:24:57.000000 quantuminspire-2.1.0/src/quantuminspire.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-05 09:24:57.000000 quantuminspire-2.1.0/src/quantuminspire.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      257 2023-01-05 09:24:57.000000 quantuminspire-2.1.0/src/quantuminspire.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-01-05 09:24:57.000000 quantuminspire-2.1.0/src/quantuminspire.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 13:17:38.607157 quantuminspire-2.2.0/
+-rw-rw-rw-   0        0        0    10354 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0      746 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/NOTICE.md
+-rw-rw-rw-   0        0        0     9349 2023-05-30 13:17:38.607157 quantuminspire-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8476 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 13:17:38.608159 quantuminspire-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     2644 2023-05-30 13:02:12.000000 quantuminspire-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:17:38.579168 quantuminspire-2.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 13:17:38.593158 quantuminspire-2.2.0/src/quantuminspire/
+-rw-rw-rw-   0        0        0       34 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/src/quantuminspire/__init__.py
+-rw-rw-rw-   0        0        0    58497 2023-05-30 13:02:12.000000 quantuminspire-2.2.0/src/quantuminspire/api.py
+-rw-rw-rw-   0        0        0     8170 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/src/quantuminspire/credentials.py
+-rw-rw-rw-   0        0        0     1101 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/src/quantuminspire/exceptions.py
+-rw-rw-rw-   0        0        0     3501 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/src/quantuminspire/job.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:17:38.600161 quantuminspire-2.2.0/src/quantuminspire/projectq/
+-rw-rw-rw-   0        0        0        0 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/src/quantuminspire/projectq/__init__.py
+-rw-rw-rw-   0        0        0    37411 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/src/quantuminspire/projectq/backend_qx.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:17:38.606157 quantuminspire-2.2.0/src/quantuminspire/qiskit/
+-rw-rw-rw-   0        0        0      116 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/src/quantuminspire/qiskit/__init__.py
+-rw-rw-rw-   0        0        0    32901 2023-05-30 13:02:12.000000 quantuminspire-2.2.0/src/quantuminspire/qiskit/backend_qx.py
+-rw-rw-rw-   0        0        0    32997 2023-05-30 13:02:12.000000 quantuminspire-2.2.0/src/quantuminspire/qiskit/circuit_parser.py
+-rw-rw-rw-   0        0        0    10929 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/src/quantuminspire/qiskit/measurements.py
+-rw-rw-rw-   0        0        0     9550 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/src/quantuminspire/qiskit/qi_job.py
+-rw-rw-rw-   0        0        0     9215 2023-05-30 12:58:49.000000 quantuminspire-2.2.0/src/quantuminspire/qiskit/qi_result.py
+-rw-rw-rw-   0        0        0     8767 2023-05-30 13:02:12.000000 quantuminspire-2.2.0/src/quantuminspire/qiskit/quantum_inspire_provider.py
+-rw-rw-rw-   0        0        0       23 2023-05-30 13:02:12.000000 quantuminspire-2.2.0/src/quantuminspire/version.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:17:38.599157 quantuminspire-2.2.0/src/quantuminspire.egg-info/
+-rw-rw-rw-   0        0        0     9349 2023-05-30 13:17:38.000000 quantuminspire-2.2.0/src/quantuminspire.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2023-05-30 13:17:38.000000 quantuminspire-2.2.0/src/quantuminspire.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:17:38.000000 quantuminspire-2.2.0/src/quantuminspire.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      257 2023-05-30 13:17:38.000000 quantuminspire-2.2.0/src/quantuminspire.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-30 13:17:38.000000 quantuminspire-2.2.0/src/quantuminspire.egg-info/top_level.txt
```

### Comparing `quantuminspire-2.1.0/LICENSE.md` & `quantuminspire-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.1.0/NOTICE.md` & `quantuminspire-2.2.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.1.0/PKG-INFO` & `quantuminspire-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: quantuminspire
-Version: 2.1.0
+Version: 2.2.0
 Summary: SDK for the Quantum Inspire platform
 Home-page: https://qutech.nl
 Author: QuantumInspire
 Author-email: support@quantum-inspire.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: qiskit
 Provides-Extra: projectq
 Provides-Extra: dev
 Provides-Extra: rtd
```

### Comparing `quantuminspire-2.1.0/README.md` & `quantuminspire-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.1.0/setup.py` & `quantuminspire-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,18 +52,19 @@
       classifiers=[
           'Development Status :: 4 - Beta',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'License :: OSI Approved :: Apache Software License'],
       license='Apache 2.0',
       packages=['quantuminspire', 'quantuminspire.qiskit', 'quantuminspire.projectq'],
       install_requires=['coverage>=4.5.1', 'matplotlib>=2.1', 'pylatexenc', 'coreapi>=2.3.3', 'numpy>=1.20', 'jupyter',
                         'nbimporter', 'qilib'],
       extras_require={
-          'qiskit': ["qiskit>=0.20.0"],
+          'qiskit': ["qiskit>=0.40.0"],
           'projectq': ["projectq>=0.4"],
           'dev': ['pytest>=3.3.1', "pylint", "mypy>=0.670"],
           'rtd': ['sphinx', 'sphinx_rtd_theme', 'nbsphinx', 'sphinx-automodapi', 'recommonmark'],
       })
```

### Comparing `quantuminspire-2.1.0/src/quantuminspire/api.py` & `quantuminspire-2.2.0/src/quantuminspire/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,15 +634,15 @@
         return dict(result)
 
     def get_raw_data_from_result(self, result_id: int) -> List[List[Any]]:
         """ Gets the raw data from the result.
 
         Gets the raw data from the result of the executed job, given the result_id.
         The raw data consists of a list of measurements for each shot (job.number_of_shots).
-        The measurements contains a list of data for each measurement in the job (len(measurement_mask)).
+        The measurements contain a list of data for each measurement in the job (len(measurement_mask)).
         The data consist of integer state values (0 or 1) for each measured qubit, else None (see measurement_mask).
         Actual type is: List[List[List[Optional[int]]]] with least significant qubit first.
 
         Example for :code:`"measurement_mask": [[0, 1], [1, 1]]` the raw_data for 6 shots is structured as follows:
 
         .. code-block::
 
@@ -869,18 +869,17 @@
             'project': project['url'],
             'content': content,
         }
         return dict(self._action(['assets', 'create'], params=payload))
 
     #  other  #
 
-    @staticmethod
-    def _wait_for_completed_job(quantum_inspire_job: QuantumInspireJob, collect_max_tries: Optional[int] = None,
-                                sec_retry_delay: float = 0.5) -> Tuple[bool, str]:
-        """Wait for job completion.
+    def wait_for_completed_job(self, quantum_inspire_job: QuantumInspireJob, collect_max_tries: Optional[int] = None,
+                               sec_retry_delay: float = 0.5) -> Tuple[bool, str]:
+        """ Wait for job completion.
 
         Delays the process and requests the job status. The waiting loop is broken when the job status is
         completed or cancelled, or when the maximum number of tries is set and has been reached.
 
         :param quantum_inspire_job: A job object.
         :param collect_max_tries: The maximum number of times the job status is checked. When set, the value should
             be > 0. When not set, the method waits until the job status is either completed or cancelled.
@@ -933,15 +932,15 @@
         maximum waiting time (collect_tries x 0.5 seconds). When the job takes longer to finish no results
         are returned. When set, the value of collect_tries must be > 0. When collect_tries is not set,
         the waiting time for completion is not limited.
 
         :param qasm: The cQASM code as string object.
         :param backend_type: The backend_type to execute the algorithm on.
         :param number_of_shots: Execution times of the algorithm before collecting the results.
-        :param collect_tries: The number of times the status of the job is check for completion before returning.
+        :param collect_tries: The number of times the status of the job is checked for completion before returning.
         :param default_number_of_shots: The default used number of shots for the project.
         :param identifier: The identifier to generate names for the project, asset and job when necessary.
         :param full_state_projection: Do not use full state projection with simulations when set to False (default).
         :param user_data: Data that the user wants to pass along with the job.
 
         :return:
             The results of the executed cQASM if successful else an error result if
@@ -954,15 +953,15 @@
             quantum_inspire_job = self.execute_qasm_async(qasm, backend_type=backend_type,
                                                           number_of_shots=number_of_shots,
                                                           default_number_of_shots=default_number_of_shots,
                                                           identifier=identifier,
                                                           full_state_projection=full_state_projection,
                                                           user_data=user_data)
 
-            has_results, message = self._wait_for_completed_job(quantum_inspire_job, collect_tries)
+            has_results, message = self.wait_for_completed_job(quantum_inspire_job, collect_tries)
             return dict(quantum_inspire_job.retrieve_results()) if has_results else \
                 dict(self._generate_error_result(message))
         except (CoreAPIException, TypeError, ValueError, ApiError) as err_msg:
             message = f'Error raised while executing qasm: {err_msg}'
             return dict(self._generate_error_result(message))
         finally:
             if delete_project_afterwards and quantum_inspire_job is not None:
@@ -977,15 +976,15 @@
         """With this method a cQASM program (job) is scheduled to be executed asynchronously.
 
         The method returns
         directly without waiting for the job to complete, as opposed to method :meth:`~.execute_qasm` which waits for
         the job to finish and returns the result.
 
         To execute a cQASM program a job is scheduled on a backend of type `backend type` as given by the
-        parameter backend_type. Currently there are 3 backend types available:
+        parameter backend_type. Currently, there are 3 backend types available:
 
             1. QX single-node simulator (default for anonymous accounts)
             2. QX single-node simulator SurfSara (advanced account credentials needed)
             3. QX multi-node simulator SurfSara (advanced account credentials needed)
 
         When no `backend_type` is given, the default backend type currently being `QX single-node simulator`, is used.
```

### Comparing `quantuminspire-2.1.0/src/quantuminspire/credentials.py` & `quantuminspire-2.2.0/src/quantuminspire/credentials.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.1.0/src/quantuminspire/exceptions.py` & `quantuminspire-2.2.0/src/quantuminspire/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.1.0/src/quantuminspire/job.py` & `quantuminspire-2.2.0/src/quantuminspire/job.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.1.0/src/quantuminspire/projectq/backend_qx.py` & `quantuminspire-2.2.0/src/quantuminspire/projectq/backend_qx.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.1.0/src/quantuminspire/qiskit/backend_qx.py` & `quantuminspire-2.2.0/src/quantuminspire/qiskit/backend_qx.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 class QuantumInspireBackend(Backend):  # type: ignore
     DEFAULT_CONFIGURATION = QasmBackendConfiguration(
         backend_name='qi_simulator',
         backend_version=quantum_inspire_version,
         n_qubits=26,
-        basis_gates=['x', 'y', 'z', 'h', 'rx', 'ry', 'rz', 's', 'sdg', 't', 'tdg', 'cx', 'ccx', 'u1', 'p', 'u2', 'u3',
+        basis_gates=['x', 'y', 'z', 'h', 'rx', 'ry', 'rz', 's', 'sdg', 't', 'tdg', 'cx', 'ccx', 'p',
                      'id', 'swap', 'cz', 'snapshot', 'delay', 'barrier'],
         gates=[GateConfig(name='NotUsed', parameters=['NaN'], qasm_def='NaN')],
         local=False,
         simulator=True,
         conditional=True,
         open_pulse=False,
         memory=True,
@@ -128,14 +128,30 @@
                 run_config_dict[key] = val
         return run_config_dict
 
     @property
     def backend_name(self) -> str:
         return self.name()  # type: ignore
 
+    @staticmethod
+    def strtobool(value: str) -> bool:
+        """Convert a string representation of truth to true (1) or false (0).
+        True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
+        are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
+        'val' is anything else.
+        From source code python 3.11.2 (distutils/util.py) which is deprecated from 3.12
+        """
+        val = value.lower()
+        if val in ('y', 'yes', 't', 'true', 'on', '1'):
+            return bool(1)
+        elif val in ('n', 'no', 'f', 'false', 'off', '0'):
+            return bool(0)
+        else:
+            raise ValueError(f"invalid truth value {value}")
+
     def run(self,
             run_input: Union[QasmQobj, QuantumCircuit, List[QuantumCircuit]],
             shots: Optional[int] = None,
             memory: Optional[bool] = None,
             allow_fsp: bool = True,
             **run_config: Dict[str, Any]
             ) -> QIJob:
@@ -171,14 +187,17 @@
                               "instead.", DeprecationWarning,
                               stacklevel=3)
                 self.qobj_warning_issued = True
             qobj = run_input
         else:
             qobj = assemble(run_input, self, **run_config_dict)
 
+        if isinstance(allow_fsp, str):
+            allow_fsp = QuantumInspireBackend.strtobool(allow_fsp)
+
         number_of_shots = qobj.config.shots
         self.__validate_number_of_shots(number_of_shots)
 
         identifier = uuid.uuid1()
         project_name = f'qi-sdk-project-{identifier}'
         project: Optional[Dict[str, Any]]
         project = self.__api.create_project(project_name, number_of_shots, self.__backend)
```

### Comparing `quantuminspire-2.1.0/src/quantuminspire/qiskit/circuit_parser.py` & `quantuminspire-2.2.0/src/quantuminspire/qiskit/circuit_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -449,30 +449,30 @@
         CircuitToString._c_u3(stream, instruction, binary_control)
 
     @staticmethod
     def _u1(stream: StringIO, instruction: QasmQobjInstruction) -> None:
         """ Translates the U1(lambda) element to U3(0, 0, lambda).
 
         A copy of the circuit is made to prevent
-        side-effects for the caller.
+        side effects for the caller.
 
         :param stream: The string-io stream to where the resulting cQASM is written.
         :param instruction: The Qiskit instruction to translate to cQASM.
 
         """
         temp_instruction = copy.deepcopy(instruction)
         temp_instruction.params[0:0] = (0, 0)
         CircuitToString._u3(stream, temp_instruction)
 
     @staticmethod
     def _c_u1(stream: StringIO, instruction: QasmQobjInstruction, binary_control: str) -> None:
         """ Translates the binary-controlled U1(lambda) element to U3(0, 0, lambda).
 
         A copy of the circuit is
-        made to prevent side-effects for the caller.
+        made to prevent side effects for the caller.
 
         :param stream: The string-io stream to where the resulting cQASM is written.
         :param instruction: The Qiskit instruction to translate to cQASM.
         :param binary_control: The multi-bits control string. The gate is executed when all specified classical bits
         are 1.
 
         """
@@ -499,46 +499,14 @@
         :param binary_control: The multi-bits control string. The gate is executed when all specified classical bits
         are 1.
 
         """
         CircuitToString._c_u1(stream, instruction, binary_control)
 
     @staticmethod
-    def _u2(stream: StringIO, instruction: QasmQobjInstruction) -> None:
-        """ Translates the U2(phi, lambda) element to U3(pi/2, phi, lambda).
-
-        A copy of the circuit is made to prevent
-        side-effects for the caller.
-
-        :param stream: The string-io stream to where the resulting cQASM is written.
-        :param instruction: The Qiskit instruction to translate to cQASM.
-
-        """
-        temp_instruction = copy.deepcopy(instruction)
-        temp_instruction.params.insert(0, np.pi/2)
-        CircuitToString._u3(stream, temp_instruction)
-
-    @staticmethod
-    def _c_u2(stream: StringIO, instruction: QasmQobjInstruction, binary_control: str) -> None:
-        """ Translates the binary-controlled U2(phi, lambda) element to U3(pi/2, phi, lambda).
-
-        A copy of the
-        circuit is made to prevent side-effects for the caller.
-
-        :param stream: The string-io stream to where the resulting cQASM is written.
-        :param instruction: The Qiskit instruction to translate to cQASM.
-        :param binary_control: The multi-bits control string. The gate is executed when all specified classical bits
-        are 1.
-
-        """
-        temp_instruction = copy.deepcopy(instruction)
-        temp_instruction.params.insert(0, np.pi/2)
-        CircuitToString._c_u3(stream, temp_instruction, binary_control)
-
-    @staticmethod
     def _u3(stream: StringIO, instruction: QasmQobjInstruction) -> None:
         """ Translates the U3(theta, phi, lambda) element to 3 rotation gates.
 
         Any single qubit operation (a 2x2 unitary matrix) can be written as the product of rotations.
         As an example, a unitary single-qubit gate can be expressed as a combination of
         Rz and Ry rotations (Nielsen and Chuang, 10th edition, section 4.2).
         U(theta, phi, lambda) = Rz(phi)Ry(theta)Rz(lambda).
```

### Comparing `quantuminspire-2.1.0/src/quantuminspire/qiskit/measurements.py` & `quantuminspire-2.2.0/src/quantuminspire/qiskit/measurements.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.1.0/src/quantuminspire/qiskit/qi_job.py` & `quantuminspire-2.2.0/src/quantuminspire/qiskit/qi_job.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.1.0/src/quantuminspire/qiskit/qi_result.py` & `quantuminspire-2.2.0/src/quantuminspire/qiskit/qi_result.py`

 * *Files identical despite different names*

### Comparing `quantuminspire-2.1.0/src/quantuminspire/qiskit/quantum_inspire_provider.py` & `quantuminspire-2.2.0/src/quantuminspire/qiskit/quantum_inspire_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                         elif gate == 'tdag':
                             config.basis_gates += ['tdg']
                         elif gate == 'cnot':
                             config.basis_gates += ['cx']
                         elif gate == 'toffoli':
                             config.basis_gates += ['ccx']
             if 'rz' in config.basis_gates and 'ry' in config.basis_gates:
-                config.basis_gates += ['u1', 'p', 'u2', 'u3']
+                config.basis_gates += ['p']
 
         config.simulator = not backend['is_hardware_backend']
         config.conditional = not backend['is_hardware_backend']
         config.max_shots = backend['max_number_of_shots']
         max_experiments = backend['max_number_of_simultaneous_jobs']
         config.max_experiments = max_experiments if max_experiments else 1
         coupling_map = []
```

### Comparing `quantuminspire-2.1.0/src/quantuminspire.egg-info/PKG-INFO` & `quantuminspire-2.2.0/src/quantuminspire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: quantuminspire
-Version: 2.1.0
+Version: 2.2.0
 Summary: SDK for the Quantum Inspire platform
 Home-page: https://qutech.nl
 Author: QuantumInspire
 Author-email: support@quantum-inspire.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: qiskit
 Provides-Extra: projectq
 Provides-Extra: dev
 Provides-Extra: rtd
```

### Comparing `quantuminspire-2.1.0/src/quantuminspire.egg-info/SOURCES.txt` & `quantuminspire-2.2.0/src/quantuminspire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

