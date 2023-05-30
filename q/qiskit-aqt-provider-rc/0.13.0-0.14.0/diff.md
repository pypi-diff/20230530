# Comparing `tmp/qiskit_aqt_provider_rc-0.13.0.tar.gz` & `tmp/qiskit_aqt_provider_rc-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_aqt_provider_rc-0.13.0.tar", max compression
+gzip compressed data, was "qiskit_aqt_provider_rc-0.14.0.tar", max compression
```

## Comparing `qiskit_aqt_provider_rc-0.13.0.tar` & `qiskit_aqt_provider_rc-0.14.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     3214 2023-05-03 09:11:25.184626 qiskit_aqt_provider_rc-0.13.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    14035 2023-05-03 09:11:25.184626 qiskit_aqt_provider_rc-0.13.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11416 2023-05-03 09:11:25.184626 qiskit_aqt_provider_rc-0.13.0/LICENSE.txt
--rw-r--r--   0        0        0     1467 2023-05-03 09:11:25.184626 qiskit_aqt_provider_rc-0.13.0/README.md
--rw-r--r--   0        0        0     6037 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/pyproject.toml
--rw-r--r--   0        0        0      562 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/__init__.py
--rw-r--r--   0        0        0     8241 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/api_models.py
--rw-r--r--   0        0        0    12734 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/api_models_generated.py
--rw-r--r--   0        0        0    16481 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/aqt_job.py
--rw-r--r--   0        0        0     2704 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/aqt_options.py
--rw-r--r--   0        0        0     8730 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/aqt_provider.py
--rw-r--r--   0        0        0    11985 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/aqt_resource.py
--rw-r--r--   0        0        0     3425 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/circuit_to_aqt.py
--rw-r--r--   0        0        0      564 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/primitives/__init__.py
--rw-r--r--   0        0        0     2985 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/primitives/sampler.py
--rw-r--r--   0        0        0        0 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/py.typed
--rw-r--r--   0        0        0      587 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/test/__init__.py
--rw-r--r--   0        0        0     1884 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/test/circuits.py
--rw-r--r--   0        0        0     2676 2023-05-03 09:11:25.188626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/test/fixtures.py
--rw-r--r--   0        0        0     6970 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/test/resources.py
--rw-r--r--   0        0        0     1259 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/test/timeout.py
--rw-r--r--   0        0        0     6483 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/transpiler_plugin.py
--rw-r--r--   0        0        0     1838 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/utils.py
--rw-r--r--   0        0        0     1040 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/versions.py
--rw-r--r--   0        0        0        0 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/test/__init__.py
--rw-r--r--   0        0        0     3822 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/test/test_api_models.py
--rw-r--r--   0        0        0     6142 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/test/test_circuit_to_aqt.py
--rw-r--r--   0        0        0    12067 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/test/test_execution.py
--rw-r--r--   0        0        0     2121 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/test/test_options.py
--rw-r--r--   0        0        0     4643 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/test/test_primitives.py
--rw-r--r--   0        0        0     5139 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/test/test_provider.py
--rw-r--r--   0        0        0    11103 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/test/test_resource.py
--rw-r--r--   0        0        0     8646 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/test/test_transpilation.py
--rw-r--r--   0        0        0     1063 2023-05-03 09:11:25.192626 qiskit_aqt_provider_rc-0.13.0/test/test_utils.py
--rw-r--r--   0        0        0     3111 1970-01-01 00:00:00.000000 qiskit_aqt_provider_rc-0.13.0/PKG-INFO
+-rw-r--r--   0        0        0     3214 2023-05-30 14:32:41.750526 qiskit_aqt_provider_rc-0.14.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    14035 2023-05-30 14:32:41.750526 qiskit_aqt_provider_rc-0.14.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11416 2023-05-30 14:32:41.750526 qiskit_aqt_provider_rc-0.14.0/LICENSE.txt
+-rw-r--r--   0        0        0     1467 2023-05-30 14:32:41.750526 qiskit_aqt_provider_rc-0.14.0/README.md
+-rw-r--r--   0        0        0     6143 2023-05-30 14:32:41.754526 qiskit_aqt_provider_rc-0.14.0/pyproject.toml
+-rw-r--r--   0        0        0      562 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/__init__.py
+-rw-r--r--   0        0        0     8241 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/api_models.py
+-rw-r--r--   0        0        0    12734 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/api_models_generated.py
+-rw-r--r--   0        0        0    16481 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_job.py
+-rw-r--r--   0        0        0     2704 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_options.py
+-rw-r--r--   0        0        0     8826 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_provider.py
+-rw-r--r--   0        0        0    12462 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_resource.py
+-rw-r--r--   0        0        0     3425 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/circuit_to_aqt.py
+-rw-r--r--   0        0        0      564 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/__init__.py
+-rw-r--r--   0        0        0     2476 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/estimator.py
+-rw-r--r--   0        0        0     2286 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/sampler.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/py.typed
+-rw-r--r--   0        0        0      587 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/__init__.py
+-rw-r--r--   0        0        0     1884 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/circuits.py
+-rw-r--r--   0        0        0     2703 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/fixtures.py
+-rw-r--r--   0        0        0     6970 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/resources.py
+-rw-r--r--   0        0        0     1259 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/timeout.py
+-rw-r--r--   0        0        0     7323 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/transpiler_plugin.py
+-rw-r--r--   0        0        0     1838 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/utils.py
+-rw-r--r--   0        0        0     1040 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/versions.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/__init__.py
+-rw-r--r--   0        0        0     3822 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_api_models.py
+-rw-r--r--   0        0        0     6142 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_circuit_to_aqt.py
+-rw-r--r--   0        0        0    13208 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_execution.py
+-rw-r--r--   0        0        0     2121 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_options.py
+-rw-r--r--   0        0        0     6603 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_primitives.py
+-rw-r--r--   0        0        0     5139 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_provider.py
+-rw-r--r--   0        0        0    11103 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_resource.py
+-rw-r--r--   0        0        0     8668 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_transpilation.py
+-rw-r--r--   0        0        0     1063 2023-05-30 14:32:41.758526 qiskit_aqt_provider_rc-0.14.0/test/test_utils.py
+-rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 qiskit_aqt_provider_rc-0.14.0/PKG-INFO
```

### Comparing `qiskit_aqt_provider_rc-0.13.0/CODE_OF_CONDUCT.md` & `qiskit_aqt_provider_rc-0.14.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/CONTRIBUTING.md` & `qiskit_aqt_provider_rc-0.14.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/LICENSE.txt` & `qiskit_aqt_provider_rc-0.14.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/README.md` & `qiskit_aqt_provider_rc-0.14.0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/pyproject.toml` & `qiskit_aqt_provider_rc-0.14.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qiskit-aqt-provider-rc"
-version = "0.13.0"
+version = "0.14.0"
 description = "Qiskit provider for AQT backends"
 authors = ["Qiskit Development Team", "Alpine Quantum Technologies GmbH"]
 repository = "https://github.com/alpine-quantum-technologies/qiskit-aqt-provider-rc/"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers=[
         "Intended Audience :: Developers",
@@ -38,48 +38,48 @@
 [tool.poetry.plugins."qiskit.transpiler.translation"]
 aqt = "qiskit_aqt_provider.transpiler_plugin:AQTTranslationPlugin"
 
 [tool.poetry.plugins.pytest11]
 pytest_qiskit_aqt = "qiskit_aqt_provider.test.fixtures"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.8,<3.11"
 
 httpx = ">=0.24.0"
-pydantic = ">=1.10,<2"
+pydantic = ">=1.10.8,<2"
 python-dotenv = ">=1"
 qiskit-aer = ">=0.11"
-qiskit-terra = ">=0.23.3"
+qiskit-terra = ">=0.23.3,<0.24.0"
 tabulate = ">=0.9.0"
 tqdm = ">=4"
 tweedledum = { version = ">=1", optional = true }
 typing-extensions = ">=4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 coverage = "^7.2.1"
-datamodel-code-generator = { git = "https://github.com/airwoodix/datamodel-code-generator", branch = "annotated-backport" }
+datamodel-code-generator = "^0.19.0"
 hypothesis = "^6.70.0"
 ipykernel = "^6.22.0"
 jupyter-sphinx = "^0.4.0"
 mistletoe = "^1.0.1"
-mypy = "=1.2.0"
+mypy = "=1.3.0"
 poethepoet = "^0.18.1"
 polyfactory = "^2.0.0"
 pre-commit = "^3.1.1"
 pyproject-fmt = "^0.9.2"
-pyright = "=1.1.304"  # also update in workflows/poetry.yml!
+pyright = "=1.1.308"
 pytest = ">=7"
 pytest-httpx = "^0.22.0"
 pytest-sugar = "^0.9.6"
 qiskit-experiments = "^0.4.0"
 qiskit-sphinx-theme = ">=1.7.0"
 qiskit-terra = {version = ">=0.23.2", extras = ["visualization"]}
-ruff = "^0.0.262"
-sphinx = ">=5.3"
+ruff = "^0.0.267"
+sphinx = "^6"
 sympy = "^1.11.1"
 typer = "^0.7.0"
 types-requests = "^2.28.11"
 types-setuptools = "^65.7.0"
 types-tabulate = "^0.9.0.1"
 types-tqdm = "^4.65.0.1"
 
@@ -196,14 +196,17 @@
     "D205",  # allow multiline docstring summaries
     "PT011",  # allow pytest.raises without match=
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
+[tool.coverage.run]
+dynamic_context = "test_function"
+
 [tool.coverage.report]
 fail_under = 98
 
 [tool.poe.tasks.test]
 shell = """
 coverage run ${cov_opts} -m pytest
 coverage report
@@ -215,29 +218,28 @@
 
 [tool.poe.tasks.format]
 shell = """
 black .
 pyproject-fmt .
 """
 
-[tool.poe.tasks.format_check]
-shell = """
-black --check .
-pyproject-fmt --check .
-"""
+[tool.poe.tasks.black_check]
+shell = "black --check ."
+
+[tool.poe.tasks.pyprojectfmt_check]
+shell = "pyproject-fmt --check ."
 
 [tool.poe.tasks.typecheck]
-shell = """
-mypy .
-pyright .
-"""
+shell = "mypy ."
 
-[tool.poe.tasks.lint]
-shell = """
-ruff check .
-./scripts/api_models.py check
-"""
+[tool.poe.tasks.check_api_models]
+shell = "./scripts/api_models.py check"
+
+[tool.poe.tasks.ruff_check]
+shell = "ruff check ."
 
 [tool.poe.tasks]
+lint = ["check_api_models", "ruff_check"]
+format_check = ["black_check", "pyprojectfmt_check"]
 generate-models = "./scripts/api_models.py generate"
 docs = "sphinx-build -b html -W docs docs/_build"
 all = ["format_check", "lint", "typecheck", "test", "docs"]
```

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/__init__.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/api_models.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/api_models.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/api_models_generated.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/api_models_generated.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/aqt_job.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/aqt_options.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/aqt_provider.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 
     noisy: bool
     """Whether the simulator uses a noise model."""
 
 
 OFFLINE_SIMULATORS: Final = [
     OfflineSimulator(id="offline_simulator_no_noise", name="Offline ideal simulator", noisy=False),
+    OfflineSimulator(id="offline_simulator_noise", name="Offline noisy simulator", noisy=True),
 ]
 
 
 class BackendsTable(Sequence[AQTResource]):
     """Pretty-printable list of AQT backends."""
 
     def __init__(self, backends: List[AQTResource]):
```

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/aqt_resource.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/aqt_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 from qiskit.circuit.library import RXGate, RXXGate, RZGate
 from qiskit.circuit.measure import Measure
 from qiskit.circuit.parameter import Parameter
 from qiskit.providers import BackendV2 as Backend
 from qiskit.providers import Options as QiskitOptions
 from qiskit.providers.models import BackendConfiguration
 from qiskit.transpiler import Target
-from qiskit_aer import AerJob, AerSimulator
-from qiskit_aer.noise import NoiseModel
+from qiskit_aer import AerJob, AerSimulator, noise
 
 from qiskit_aqt_provider import api_models
 from qiskit_aqt_provider.aqt_job import AQTJob
 from qiskit_aqt_provider.aqt_options import AQTOptions
 from qiskit_aqt_provider.circuit_to_aqt import circuits_to_aqt_job
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -303,17 +302,29 @@
             resource_id=resource_id,
             resource_name=resource_name,
             resource_type="offline_simulator",
         )
 
         self.job: Optional[SimulatorJob] = None
 
-        noise_model = NoiseModel.from_backend(self) if noisy else None
+        if not noisy:
+            noise_model = None
+        else:
+            # the transpiler lowers all operations to the gate set supported by the AQT API,
+            # not to the resource target's one.
+            noise_model = noise.NoiseModel(basis_gates=["r", "rz", "rxx"])
+            noise_model.add_all_qubit_quantum_error(noise.depolarizing_error(0.003, 1), ["r"])
+            noise_model.add_all_qubit_quantum_error(noise.depolarizing_error(0.01, 2), ["rxx"])
+
         self.simulator = AerSimulator(method="statevector", noise_model=noise_model)
 
+    @property
+    def noisy(self) -> bool:
+        return self.simulator.options.noise_model is not None
+
     def submit(self, circuits: List[QuantumCircuit], shots: int) -> UUID:
         """Submit circuits for execution on the simulator.
 
         Args:
             circuits: circuits to execute
             shots: number of repetitions per circuit.
```

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/circuit_to_aqt.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/circuit_to_aqt.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/primitives/__init__.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/primitives/sampler.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/primitives/estimator.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,71 +9,58 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 from copy import copy
 from typing import Any, Dict, Optional
 
-from qiskit.primitives import BackendSampler
-from qiskit.transpiler.passes import Decompose, Optimize1qGatesDecomposition
-from qiskit.transpiler.passmanager import PassManager
+from qiskit.primitives import BackendEstimator
 
 from qiskit_aqt_provider import transpiler_plugin
 from qiskit_aqt_provider.aqt_resource import AQTResource, make_transpiler_target
 
 
-class AQTSampler(BackendSampler):
-    """Sampler primitive for AQT backends."""
+class AQTEstimator(BackendEstimator):
+    """Estimator primitive for AQT backends."""
 
     _backend: AQTResource
 
     def __init__(
         self,
         backend: AQTResource,
         options: Optional[Dict[str, Any]] = None,
+        abelian_grouping: bool = True,
         skip_transpilation: bool = False,
     ):
-        """Initialize a Sampler primitive for AQT resources.
+        """Initialize an Estimator primitive for AQT resources.
 
         Args:
             backend: AQT resource to evaluate circuits on
             options: options passed to the base sampler
+            abelian_grouping:  whether the observable should be grouped into commuting parts
             skip_transpilation: if true, pass circuits unchanged to the backend.
         """
         # Signal the transpiler to disable passes that require bound
         # parameters.
         # This allows the underlying sampler to apply most of
         # the transpilation passes, and cache the results.
         mod_backend = copy(backend)
         mod_backend._target = make_transpiler_target(
             transpiler_plugin.UnboundParametersTarget, backend.num_qubits
         )
 
-        # Wrap the gate angles after the parameters are bound.
-        bound_pass_manager = PassManager(
-            [
-                # wrap the Rxx angles
-                transpiler_plugin.WrapRxxAngles(),
-                # decompose the substituted Rxx gates
-                Decompose([f"{transpiler_plugin.WrapRxxAngles.SUBSTITUTE_GATE_NAME}*"]),
-                # collapse the single qubit runs as ZXZ
-                Optimize1qGatesDecomposition(target=mod_backend.target),
-                # wrap the Rx angles, rewrite as R
-                transpiler_plugin.RewriteRxAsR(),
-            ]
-        )
-
         # if `with_progress_bar` is not explicitly set in the options, disable it
         options_copy = (options or {}).copy()
         options_copy.update(with_progress_bar=options_copy.get("with_progress_bar", False))
 
         super().__init__(
             mod_backend,
-            bound_pass_manager=bound_pass_manager,
+            bound_pass_manager=transpiler_plugin.bound_pass_manager(mod_backend.target),
             options=options_copy,
+            abelian_grouping=abelian_grouping,
             skip_transpilation=skip_transpilation,
         )
 
     @property
     def backend(self) -> AQTResource:
         """Computing resource used for circuit evaluation."""
         return self._backend
```

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/test/__init__.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/test/circuits.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/circuits.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/test/fixtures.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 from qiskit_aqt_provider.aqt_resource import OfflineSimulatorResource
 from qiskit_aqt_provider.circuit_to_aqt import _qiskit_to_aqt_circuit
 
 
 class MockSimulator(OfflineSimulatorResource):
     """Offline simulator that keeps track of the submitted circuits."""
 
-    def __init__(self) -> None:
+    def __init__(self, *, noisy: bool) -> None:
         super().__init__(
             AQTProvider(""),
             workspace_id="default",
             resource_id="mock_simulator",
             resource_name="mock_simulator",
-            noisy=False,
+            noisy=noisy,
         )
 
         self.submit_call_args: List[Tuple[List[QuantumCircuit], int]] = []
 
     def submit(self, circuits: List[QuantumCircuit], shots: int) -> uuid.UUID:
         """Submit the circuits for execution on the backend.
 
@@ -70,8 +70,8 @@
         """Circuit batches passed to the resource for execution, in submission order."""
         return [circuit for circuit, _ in self.submit_call_args]
 
 
 @pytest.fixture(name="offline_simulator_no_noise")
 def fixture_offline_simulator_no_noise() -> MockSimulator:
     """Noiseless offline simulator resource."""
-    return MockSimulator()
+    return MockSimulator(noisy=False)
```

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/test/resources.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/resources.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/test/timeout.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/test/timeout.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/transpiler_plugin.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/transpiler_plugin.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,26 +19,50 @@
 from qiskit.circuit import Gate, Instruction
 from qiskit.circuit.library import RGate, RXGate, RXXGate, RZGate
 from qiskit.circuit.tools import pi_check
 from qiskit.dagcircuit import DAGCircuit
 from qiskit.transpiler import Target
 from qiskit.transpiler.basepasses import BasePass, TransformationPass
 from qiskit.transpiler.exceptions import TranspilerError
+from qiskit.transpiler.passes import Decompose, Optimize1qGatesDecomposition
 from qiskit.transpiler.passmanager import PassManager
 from qiskit.transpiler.passmanager_config import PassManagerConfig
 from qiskit.transpiler.preset_passmanagers import common
 from qiskit.transpiler.preset_passmanagers.plugin import PassManagerStagePlugin
 
 from qiskit_aqt_provider.utils import map_exceptions
 
 
 class UnboundParametersTarget(Target):
     """Target that disables passes that require bound parameters."""
 
 
+def bound_pass_manager(target: Target) -> PassManager:
+    """Transpilation passes to apply on circuits after the parameters are bound.
+
+    This assumes that a preset pass manager was applied to the unbound circuits
+    (by setting the target to an instance of `UnboundParametersTarget`).
+
+    Args:
+        target: transpilation target.
+    """
+    return PassManager(
+        [
+            # wrap the Rxx angles
+            WrapRxxAngles(),
+            # decompose the substituted Rxx gates
+            Decompose([f"{WrapRxxAngles.SUBSTITUTE_GATE_NAME}*"]),
+            # collapse the single qubit runs as ZXZ
+            Optimize1qGatesDecomposition(target=target),
+            # wrap the Rx angles, rewrite as R
+            RewriteRxAsR(),
+        ]
+    )
+
+
 def rewrite_rx_as_r(theta: float) -> Instruction:
     """Instruction equivalent to Rx(θ) as R(θ, φ) with θ ∈ [0, π] and φ ∈ [0, 2π]."""
     theta = math.atan2(math.sin(theta), math.cos(theta))
     phi = math.pi if theta < 0.0 else 0.0
     return RGate(abs(theta), phi)
```

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/utils.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/qiskit_aqt_provider/versions.py` & `qiskit_aqt_provider_rc-0.14.0/qiskit_aqt_provider/versions.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/test/test_api_models.py` & `qiskit_aqt_provider_rc-0.14.0/test/test_api_models.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/test/test_circuit_to_aqt.py` & `qiskit_aqt_provider_rc-0.14.0/test/test_circuit_to_aqt.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/test/test_execution.py` & `qiskit_aqt_provider_rc-0.14.0/test/test_execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 """Run various circuits on an offline simulator controlled by an AQTResource.
 
 This tests whether the circuit pre-conditioning and results formatting works as
 expected.
 """
 
 import re
+import typing
+from collections import Counter
 from fractions import Fraction
 from math import pi
 from typing import List
 
 import numpy as np
 import pytest
 import qiskit
@@ -28,14 +30,15 @@
 from qiskit.providers.jobstatus import JobStatus
 from qiskit.result import Counts
 from qiskit_aer import AerSimulator
 from qiskit_experiments.library import QuantumVolume
 
 from qiskit_aqt_provider.aqt_resource import AQTResource
 from qiskit_aqt_provider.test.circuits import qft_circuit
+from qiskit_aqt_provider.test.fixtures import MockSimulator
 from qiskit_aqt_provider.test.resources import TestResource
 from qiskit_aqt_provider.test.timeout import timeout
 
 
 @pytest.mark.parametrize("shots", [200])
 def test_empty_circuit(shots: int, offline_simulator_no_noise: AQTResource) -> None:
     """Run an empty circuit."""
@@ -124,14 +127,43 @@
     qc1.measure_all()
 
     # qiskit.execute calls the transpiler automatically
     job = qiskit.execute([qc0, qc1], backend=offline_simulator_no_noise, shots=shots)
     assert job.result().get_counts() == [{"01": shots}, {"10": shots}]
 
 
+@pytest.mark.parametrize("backend", [MockSimulator(noisy=False), MockSimulator(noisy=True)])
+def test_simple_backend_execute_noisy(backend: MockSimulator) -> None:
+    """Execute a simple circuit on a noisy and noiseless backend. Check that the noisy backend
+    is indeed noisy.
+    """
+    qc = QuantumCircuit(1)
+    qc.rx(pi, 0)
+    qc.measure_all()
+
+    # the single qubit error is around 0.1% so to see at least one error, we need to do more than
+    # 1000 shots.
+    total_shots = 4000  # take some margin
+    shots = 200  # maximum shots per submission
+    assert total_shots % shots == 0
+
+    counts: typing.Counter[str] = Counter()
+    for _ in range(total_shots // shots):
+        job = qiskit.execute(qc, backend=backend, shots=shots)
+        counts += Counter(job.result().get_counts())
+
+    assert sum(counts.values()) == total_shots
+
+    if backend.noisy:
+        assert set(counts.keys()) == {"0", "1"}
+        assert counts["0"] < 0.1 * counts["1"]  # very crude
+    else:
+        assert set(counts.keys()) == {"1"}
+
+
 @pytest.mark.parametrize("shots", [100])
 def test_ancilla_qubits_mapping(shots: int, offline_simulator_no_noise: AQTResource) -> None:
     """Run a circuit with two quantum registers, with only one mapped to the classical memory."""
     qr = QuantumRegister(2)
     qr_aux = QuantumRegister(3)
     memory = ClassicalRegister(2)
```

### Comparing `qiskit_aqt_provider_rc-0.13.0/test/test_options.py` & `qiskit_aqt_provider_rc-0.14.0/test/test_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/test/test_primitives.py` & `qiskit_aqt_provider_rc-0.14.0/test/test_primitives.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 import importlib.metadata
-from math import pi
+from math import isclose, pi
 from typing import Callable
 
 import pytest
 import qiskit
 from qiskit.circuit import Parameter, QuantumCircuit
 from qiskit.primitives import BackendSampler, BaseSampler, Sampler
 from qiskit.providers import Backend
+from qiskit.quantum_info import SparsePauliOp
 from qiskit.transpiler.exceptions import TranspilerError
 
 from qiskit_aqt_provider.aqt_resource import AQTResource
 from qiskit_aqt_provider.primitives import AQTSampler
+from qiskit_aqt_provider.primitives.estimator import AQTEstimator
 from qiskit_aqt_provider.test.circuits import assert_circuits_equal
 from qiskit_aqt_provider.test.fixtures import MockSimulator
 
 
 @pytest.mark.skipif(
     importlib.metadata.version("qiskit-terra") >= "0.24.0",
     reason="qiskit.opflow is deprecated in qiskit-terra>=0.24",
@@ -87,14 +89,69 @@
     assert qc.num_parameters > 0
 
     sampler = get_sampler(offline_simulator_no_noise)
     sampled = sampler.run(qc, [pi]).result().quasi_dists
     assert sampled == [{3: 1.0}]
 
 
+@pytest.mark.parametrize("theta", [0.0, pi])
+def test_operator_estimator_primitive_trivial_pauli_x(
+    theta: float, offline_simulator_no_noise: MockSimulator
+) -> None:
+    """Use the Estimator primitive to verify that <0|X|0> = <1|X|1> = 0.
+
+    Define the parametrized circuit that consists of the single gate Rx(θ) with
+    θ=0,π. Applied to |0>, this creates the states |0>,|1>. The Estimator primitive
+    is then used to evaluate the expectation value of the Pauli X operator on the
+    state produced by the circuit.
+    """
+    offline_simulator_no_noise.simulator.options.seed_simulator = 0
+
+    estimator = AQTEstimator(offline_simulator_no_noise, options={"shots": 200})
+
+    qc = QuantumCircuit(1)
+    qc.rx(theta, 0)
+
+    op = SparsePauliOp("X")
+    result = estimator.run(qc, op).result()
+
+    assert abs(result.values[0]) < 0.1
+
+
+def test_operator_estimator_primitive_trivial_pauli_z(
+    offline_simulator_no_noise: MockSimulator,
+) -> None:
+    """Use the Estimator primitive to verify that:
+    <0|Z|0> = 1
+    <1|Z|1> = -1
+    <ψ|Z|ψ> = 0 with |ψ> = (|0> + |1>)/√2.
+
+    The sampled circuit is always Rx(θ) with θ=0,π,π/2 respectively.
+
+    The θ values are passed into a single call to the estimator, thus also checking
+    that the AQTEstimator can deal with parametrized circuits.
+    """
+    offline_simulator_no_noise.simulator.options.seed_simulator = 0
+
+    estimator = AQTEstimator(offline_simulator_no_noise, options={"shots": 200})
+
+    theta = Parameter("θ")
+    qc = QuantumCircuit(1)
+    qc.rx(theta, 0)
+
+    op = SparsePauliOp("Z")
+    result = estimator.run([qc] * 3, [op] * 3, [[0], [pi], [pi / 2]]).result()
+
+    z0, z1, z01 = result.values
+
+    assert isclose(z0, 1.0)  # <0|Z|0>
+    assert isclose(z1, -1.0)  # <1|Z|1>
+    assert abs(z01) < 0.1  # <ψ|Z|ψ>, |ψ> = (|0> + |1>)/√2
+
+
 @pytest.mark.parametrize(
     "theta",
     [
         pi / 3,
         -pi / 3,
         pi / 2,
         -pi / 2,
```

### Comparing `qiskit_aqt_provider_rc-0.13.0/test/test_provider.py` & `qiskit_aqt_provider_rc-0.14.0/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/test/test_resource.py` & `qiskit_aqt_provider_rc-0.14.0/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/test/test_transpilation.py` & `qiskit_aqt_provider_rc-0.14.0/test/test_transpilation.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     optimization_level: int,
     test_gate: Union[RXGate, RYGate],
 ) -> None:
     """Test the rewrite rule: Rx(θ), Ry(θ) → R(θ, φ), θ ∈ [0, π], φ ∈ [0, 2π]."""
     assume(abs(theta) > pi / 200)
 
     # we only need the backend's transpiler target for this test
-    backend = MockSimulator()
+    backend = MockSimulator(noisy=False)
 
     qc = QuantumCircuit(1)
     qc.append(test_gate(theta), (0,))
 
     trans_qc = transpile(qc, backend, optimization_level=optimization_level)
     assert isinstance(trans_qc, QuantumCircuit)
 
@@ -207,15 +207,15 @@
     """Check that Rxx angles are wrapped by the transpiler."""
     assume(abs(angle) > pi / 200)
 
     qc = QuantumCircuit(qubits)
     qc.rxx(angle, 0, 1)
 
     # we only need the backend's transpilation target for this test
-    backend = MockSimulator()
+    backend = MockSimulator(noisy=False)
     trans_qc = transpile(qc, backend, optimization_level=optimization_level)
     assert isinstance(trans_qc, QuantumCircuit)
 
     assert_circuits_equivalent(trans_qc, qc)
 
     assert set(trans_qc.count_ops()) <= set(backend.configuration().basis_gates)
     num_rxx = trans_qc.count_ops().get("rxx")
```

### Comparing `qiskit_aqt_provider_rc-0.13.0/test/test_utils.py` & `qiskit_aqt_provider_rc-0.14.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.13.0/PKG-INFO` & `qiskit_aqt_provider_rc-0.14.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 2.1
 Name: qiskit-aqt-provider-rc
-Version: 0.13.0
+Version: 0.14.0
 Summary: Qiskit provider for AQT backends
 Home-page: https://github.com/alpine-quantum-technologies/qiskit-aqt-provider-rc/
 License: Apache-2.0
 Keywords: qiskit,sdk,quantum
 Author: Qiskit Development Team
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: examples
 Requires-Dist: httpx (>=0.24.0)
-Requires-Dist: pydantic (>=1.10,<2)
+Requires-Dist: pydantic (>=1.10.8,<2)
 Requires-Dist: python-dotenv (>=1)
 Requires-Dist: qiskit-aer (>=0.11)
-Requires-Dist: qiskit-terra (>=0.23.3)
+Requires-Dist: qiskit-terra (>=0.23.3,<0.24.0)
 Requires-Dist: tabulate (>=0.9.0)
 Requires-Dist: tqdm (>=4)
 Requires-Dist: tweedledum (>=1) ; extra == "examples"
 Requires-Dist: typing-extensions (>=4.0.0)
 Project-URL: Repository, https://github.com/alpine-quantum-technologies/qiskit-aqt-provider-rc/
 Description-Content-Type: text/markdown
```

