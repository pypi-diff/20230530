# Comparing `tmp/circuit-knitting-toolbox-0.1.0.tar.gz` & `tmp/circuit_knitting_toolbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuit-knitting-toolbox-0.1.0.tar", last modified: Fri May  5 23:57:12 2023, max compression
+gzip compressed data, was "circuit_knitting_toolbox-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `circuit-knitting-toolbox-0.1.0.tar` & `circuit_knitting_toolbox-0.2.0.tar`

### file list

```diff
@@ -1,90 +1,129 @@
--rw-r--r--   0        0        0       21 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.dockerignore
--rw-r--r--   0        0        0      118 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     3711 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/README.md
--rw-r--r--   0        0        0     2092 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/citation.yml
--rw-r--r--   0        0        0     1112 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      562 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/docker.yml
--rw-r--r--   0        0        0      923 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      608 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      997 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1175 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/test_development_versions.yml
--rw-r--r--   0        0        0     1495 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/test_latest_versions.yml
--rw-r--r--   0        0        0     1218 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.github/workflows/test_minimum_versions.yml
--rw-r--r--   0        0        0      580 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.gitignore
--rw-r--r--   0        0        0       79 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.mypy.ini
--rw-r--r--   0        0        0      199 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/.ruff.toml
--rw-r--r--   0        0        0      664 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/CITATION.bib
--rw-r--r--   0        0        0     6153 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      619 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/Dockerfile
--rw-r--r--   0        0        0     3707 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/INSTALL.rst
--rw-r--r--   0        0        0    11416 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     4687 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/README.md
--rw-r--r--   0        0        0      927 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/__init__.py
--rw-r--r--   0        0        0      923 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/__init__.py
--rw-r--r--   0        0        0     1020 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/__init__.py
--rw-r--r--   0        0        0    22382 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/mip_model.py
--rw-r--r--   0        0        0    37295 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting.py
--rw-r--r--   0        0        0    14798 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_evaluation.py
--rw-r--r--   0        0        0    18166 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_post_processing.py
--rw-r--r--   0        0        0     5902 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_verification.py
--rw-r--r--   0        0        0     1617 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/__init__.py
--rw-r--r--   0        0        0    15773 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/cholesky_decomposition.py
--rw-r--r--   0        0        0     6793 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ansatz.py
--rw-r--r--   0        0        0    15253 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ground_state_solver.py
--rw-r--r--   0        0        0    29419 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_knitter.py
--rw-r--r--   0        0        0     3137 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_operator.py
--rw-r--r--   0        0        0      717 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/__init__.py
--rw-r--r--   0        0        0     3875 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/conversion.py
--rw-r--r--   0        0        0     7993 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/metrics.py
--rw-r--r--   0        0        0     1347 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/orbital_reduction.py
--rw-r--r--   0        0        0      365 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/docker-compose.yml
--rw-r--r--   0        0        0     4062 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/docs/_static/gallery.css
--rw-r--r--   0        0        0     5285 2023-05-05 23:57:07.625493 circuit-knitting-toolbox-0.1.0/docs/_static/no_image.png
--rw-r--r--   0        0        0      194 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/apidocs/circuit_cutting.rst
--rw-r--r--   0        0        0      219 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/apidocs/entanglement_forging.rst
--rw-r--r--   0        0        0      271 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/apidocs/index.rst
--rw-r--r--   0        0        0      156 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/apidocs/utils.rst
--rw-r--r--   0        0        0      347 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/explanation/index.rst
--rw-r--r--   0        0        0      102 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/how-tos/index.rst
--rw-r--r--   0        0        0      550 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/README.rst
--rw-r--r--   0        0        0      146 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/index.rst
--rw-r--r--   0        0        0   164415 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_1_automatic_cut_finding.ipynb
--rw-r--r--   0        0        0   262634 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_2_manual_cutting.ipynb
--rw-r--r--   0        0        0   171432 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_3_cutting_with_quantum_serverless.ipynb
--rw-r--r--   0        0        0     2041 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/conf.py
--rw-r--r--   0        0        0    19307 2023-05-05 23:57:07.629493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/figs/Fig_5_c.png
--rw-r--r--   0        0        0   200296 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/figs/forging_info_graphic.png
--rw-r--r--   0        0        0    12930 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/index.rst
--rw-r--r--   0        0        0    11722 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/freeze-orbitals.ipynb
--rw-r--r--   0        0        0      310 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/index.rst
--rw-r--r--   0        0        0     1354 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/specify-problem.rst
--rw-r--r--   0        0        0    18145 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/use-asymmetric-bitstrings.ipynb
--rw-r--r--   0        0        0     1686 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/data/reactant_2mo.npz
--rw-r--r--   0        0        0      239 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/index.rst
--rw-r--r--   0        0        0    81343 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/tutorial_1_getting_started.ipynb
--rw-r--r--   0        0        0   100607 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/tutorial_2_forging_with_quantum_serverless.ipynb
--rw-r--r--   0        0        0     2927 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/index.rst
--rw-r--r--   0        0        0       28 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/install.rst
--rw-r--r--   0        0        0       53 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/docs/release-notes.rst
--rw-r--r--   0        0        0     2611 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       40 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/releasenotes/config.yaml
--rw-r--r--   0        0        0      401 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/releasenotes/notes/0.1/dep-versions-383f4a21044cf599.yaml
--rw-r--r--   0        0        0      177 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/releasenotes/notes/0.1/deprecate-py37-5ef642682641aeb8.yaml
--rw-r--r--   0        0        0     1060 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/releasenotes/notes/0.1/migrate-to-qiskit-nature-0.5.0-96e90cd48f36d731.yaml
--rw-r--r--   0        0        0      140 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/releasenotes/notes/0.1/optional-cplex-f578dabd9d1a83f8.yaml
--rw-r--r--   0        0        0       38 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/setup.py
--rw-r--r--   0        0        0      475 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/__init__.py
--rw-r--r--   0        0        0      475 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/circuit_cutting/__init__.py
--rw-r--r--   0        0        0     2630 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/circuit_cutting/test_circuit_cutting.py
--rw-r--r--   0        0        0      475 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/__init__.py
--rw-r--r--   0        0        0      416 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CH3_one_body.npy
--rw-r--r--   0        0        0    10496 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CH3_two_body.npy
--rw-r--r--   0        0        0      640 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CN_one_body.npy
--rw-r--r--   0        0        0    32896 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CN_two_body.npy
--rw-r--r--   0        0        0      640 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/O2_one_body.npy
--rw-r--r--   0        0        0    32896 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/O2_two_body.npy
--rw-r--r--   0        0        0     2575 2023-05-05 23:57:07.633493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_entanglement_forging_ground_state_solver.py
--rw-r--r--   0        0        0    13312 2023-05-05 23:57:07.637493 circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_entanglement_forging_knitter.py
--rwxr-xr-x   0        0        0     2818 2023-05-05 23:57:07.637493 circuit-knitting-toolbox-0.1.0/tools/extremal_dependency_versions.py
--rw-r--r--   0        0        0     1904 2023-05-05 23:57:07.637493 circuit-knitting-toolbox-0.1.0/tox.ini
--rw-r--r--   0        0        0     7801 1970-01-01 00:00:00.000000 circuit-knitting-toolbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.dockerignore
+-rw-r--r--   0        0        0      298 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3711 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/workflows/README.md
+-rw-r--r--   0        0        0     2092 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/workflows/citation.yml
+-rw-r--r--   0        0        0     1112 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      562 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/workflows/docker.yml
+-rw-r--r--   0        0        0      923 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      608 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1000 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1205 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/workflows/test_development_versions.yml
+-rw-r--r--   0        0        0     1521 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/workflows/test_latest_versions.yml
+-rw-r--r--   0        0        0     1248 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.github/workflows/test_minimum_versions.yml
+-rw-r--r--   0        0        0      621 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.gitignore
+-rw-r--r--   0        0        0       79 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.mypy.ini
+-rw-r--r--   0        0        0      199 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/.ruff.toml
+-rw-r--r--   0        0        0      735 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/CITATION.bib
+-rw-r--r--   0        0        0     6153 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      619 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/Dockerfile
+-rw-r--r--   0        0        0     3707 2023-05-30 21:15:50.807435 circuit_knitting_toolbox-0.2.0/INSTALL.rst
+-rw-r--r--   0        0        0    11416 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     5413 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/README.md
+-rw-r--r--   0        0        0      534 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/__init__.py
+-rw-r--r--   0        0        0     1396 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/__init__.py
+-rw-r--r--   0        0        0     1013 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/__init__.py
+-rw-r--r--   0        0        0    20945 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/mip_model.py
+-rw-r--r--   0        0        0    36237 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/wire_cutting.py
+-rw-r--r--   0        0        0    14295 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/wire_cutting_evaluation.py
+-rw-r--r--   0        0        0    17673 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/wire_cutting_post_processing.py
+-rw-r--r--   0        0        0     5584 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/wire_cutting_verification.py
+-rw-r--r--   0        0        0     9627 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutting_decomposition.py
+-rw-r--r--   0        0        0    18772 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutting_evaluation.py
+-rw-r--r--   0        0        0     6617 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutting_reconstruction.py
+-rw-r--r--   0        0        0     1266 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/qpd/__init__.py
+-rw-r--r--   0        0        0      921 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/qpd/instructions/__init__.py
+-rw-r--r--   0        0        0     6561 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/qpd/instructions/qpd_gate.py
+-rw-r--r--   0        0        0      919 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/qpd/instructions/qpd_measure.py
+-rw-r--r--   0        0        0    17999 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/qpd/qpd.py
+-rw-r--r--   0        0        0     4779 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/qpd/qpd_basis.py
+-rw-r--r--   0        0        0      852 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting.py
+-rw-r--r--   0        0        0     1617 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/__init__.py
+-rw-r--r--   0        0        0    14880 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/cholesky_decomposition.py
+-rw-r--r--   0        0        0     5135 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ansatz.py
+-rw-r--r--   0        0        0    15102 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ground_state_solver.py
+-rw-r--r--   0        0        0    27727 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_knitter.py
+-rw-r--r--   0        0        0     2555 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_operator.py
+-rw-r--r--   0        0        0     2684 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0      979 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/bitwise.py
+-rw-r--r--   0        0        0     3976 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/conversion.py
+-rw-r--r--   0        0        0     2320 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/iteration.py
+-rw-r--r--   0        0        0     7856 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/metrics.py
+-rw-r--r--   0        0        0    11231 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/observable_grouping.py
+-rw-r--r--   0        0        0     1405 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/orbital_reduction.py
+-rw-r--r--   0        0        0     7486 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/simulation.py
+-rw-r--r--   0        0        0     8689 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/transforms.py
+-rw-r--r--   0        0        0      365 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/docker-compose.yml
+-rw-r--r--   0        0        0     5285 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/docs/_static/no_image.png
+-rw-r--r--   0        0        0      126 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/docs/_static/style.css
+-rw-r--r--   0        0        0      194 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/docs/apidocs/circuit_cutting.rst
+-rw-r--r--   0        0        0      219 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/docs/apidocs/entanglement_forging.rst
+-rw-r--r--   0        0        0      271 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/docs/apidocs/index.rst
+-rw-r--r--   0        0        0      156 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/docs/apidocs/utils.rst
+-rw-r--r--   0        0        0      534 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/cutqc/README.rst
+-rw-r--r--   0        0        0     1076 2023-05-30 21:15:50.811436 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/cutqc/index.rst
+-rw-r--r--   0        0        0   164393 2023-05-30 21:15:50.815436 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/cutqc/tutorials/tutorial_1_automatic_cut_finding.ipynb
+-rw-r--r--   0        0        0   262612 2023-05-30 21:15:50.815436 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/cutqc/tutorials/tutorial_2_manual_cutting.ipynb
+-rw-r--r--   0        0        0   171430 2023-05-30 21:15:50.815436 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/cutqc/tutorials/tutorial_3_cutting_with_quantum_serverless.ipynb
+-rw-r--r--   0        0        0     6245 2023-05-30 21:15:50.815436 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/explanation/index.rst
+-rw-r--r--   0        0        0      508 2023-05-30 21:15:50.815436 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/how-tos/README.rst
+-rw-r--r--   0        0        0     3015 2023-05-30 21:15:50.819435 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/how-tos/how_to_generate_exact_quasi_dists_from_sampler.ipynb
+-rw-r--r--   0        0        0    43277 2023-05-30 21:15:50.819435 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/how-tos/how_to_generate_exact_sampling_coefficients.ipynb
+-rw-r--r--   0        0        0      148 2023-05-30 21:15:50.819435 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/how-tos/index.rst
+-rw-r--r--   0        0        0      358 2023-05-30 21:15:50.819435 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/tutorials/README.rst
+-rw-r--r--   0        0        0   236891 2023-05-30 21:15:50.819435 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/tutorials/gate_cutting_to_reduce_circuit_depth.ipynb
+-rw-r--r--   0        0        0    54564 2023-05-30 21:15:50.819435 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/tutorials/gate_cutting_to_reduce_circuit_width.ipynb
+-rw-r--r--   0        0        0      168 2023-05-30 21:15:50.819435 circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/tutorials/index.rst
+-rw-r--r--   0        0        0     2039 2023-05-30 21:15:50.819435 circuit_knitting_toolbox-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0    19307 2023-05-30 21:15:50.819435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/explanation/figs/Fig_5_c.png
+-rw-r--r--   0        0        0   200296 2023-05-30 21:15:50.819435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/explanation/figs/forging_info_graphic.png
+-rw-r--r--   0        0        0    12930 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/explanation/index.rst
+-rw-r--r--   0        0        0    11722 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/how-tos/freeze-orbitals.ipynb
+-rw-r--r--   0        0        0      310 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/how-tos/index.rst
+-rw-r--r--   0        0        0     1354 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/how-tos/specify-problem.rst
+-rw-r--r--   0        0        0    18145 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/how-tos/use-asymmetric-bitstrings.ipynb
+-rw-r--r--   0        0        0     1686 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/tutorials/data/reactant_2mo.npz
+-rw-r--r--   0        0        0      239 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/tutorials/index.rst
+-rw-r--r--   0        0        0    81343 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/tutorials/tutorial_1_getting_started.ipynb
+-rw-r--r--   0        0        0   100607 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/tutorials/tutorial_2_forging_with_quantum_serverless.ipynb
+-rw-r--r--   0        0        0     3274 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0       28 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/install.rst
+-rw-r--r--   0        0        0       53 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/docs/release-notes.rst
+-rw-r--r--   0        0        0     2807 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/releasenotes/config.yaml
+-rw-r--r--   0        0        0      401 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/releasenotes/notes/0.1/dep-versions-383f4a21044cf599.yaml
+-rw-r--r--   0        0        0      177 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/releasenotes/notes/0.1/deprecate-py37-5ef642682641aeb8.yaml
+-rw-r--r--   0        0        0     1060 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/releasenotes/notes/0.1/migrate-to-qiskit-nature-0.5.0-96e90cd48f36d731.yaml
+-rw-r--r--   0        0        0      140 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/releasenotes/notes/0.1/optional-cplex-f578dabd9d1a83f8.yaml
+-rw-r--r--   0        0        0      510 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/releasenotes/notes/0.2/cutqc-package-98dc0e9a3f81ff16.yaml
+-rw-r--r--   0        0        0     3632 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/releasenotes/notes/0.2/gate-cutting-workflow-ebbedbdb1313b258.yaml
+-rw-r--r--   0        0        0      165 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/releasenotes/notes/0.2/remove-py37-0ca8b41847e64d43.yaml
+-rw-r--r--   0        0        0       38 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/setup.py
+-rw-r--r--   0        0        0      475 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/__init__.py
+-rw-r--r--   0        0        0      475 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/__init__.py
+-rw-r--r--   0        0        0      475 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/qpd/__init__.py
+-rw-r--r--   0        0        0     3919 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/qpd/instructions/test_qpd_gate.py
+-rw-r--r--   0        0        0      758 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/qpd/instructions/test_qpd_measure.py
+-rw-r--r--   0        0        0    12261 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/qpd/test_qpd.py
+-rw-r--r--   0        0        0     6681 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/qpd/test_qpd_basis.py
+-rw-r--r--   0        0        0     2623 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/test_cutqc.py
+-rw-r--r--   0        0        0    10851 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/test_cutting_decomposition.py
+-rw-r--r--   0        0        0    15182 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/test_cutting_evaluation.py
+-rw-r--r--   0        0        0     3956 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/test_cutting_reconstruction.py
+-rw-r--r--   0        0        0     4098 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/circuit_cutting/test_cutting_roundtrip.py
+-rw-r--r--   0        0        0     1304 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/conftest.py
+-rw-r--r--   0        0        0      475 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/entanglement_forging/__init__.py
+-rw-r--r--   0        0        0      416 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/CH3_one_body.npy
+-rw-r--r--   0        0        0    10496 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/CH3_two_body.npy
+-rw-r--r--   0        0        0      640 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/CN_one_body.npy
+-rw-r--r--   0        0        0    32896 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/CN_two_body.npy
+-rw-r--r--   0        0        0      640 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/O2_one_body.npy
+-rw-r--r--   0        0        0    32896 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/O2_two_body.npy
+-rw-r--r--   0        0        0     2575 2023-05-30 21:15:50.823435 circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_entanglement_forging_ground_state_solver.py
+-rw-r--r--   0        0        0    13371 2023-05-30 21:15:50.827436 circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_entanglement_forging_knitter.py
+-rw-r--r--   0        0        0     1141 2023-05-30 21:15:50.827436 circuit_knitting_toolbox-0.2.0/test/utils/test_iteration.py
+-rw-r--r--   0        0        0     4226 2023-05-30 21:15:50.827436 circuit_knitting_toolbox-0.2.0/test/utils/test_observable_grouping.py
+-rw-r--r--   0        0        0     4436 2023-05-30 21:15:50.827436 circuit_knitting_toolbox-0.2.0/test/utils/test_simulation.py
+-rw-r--r--   0        0        0    16822 2023-05-30 21:15:50.827436 circuit_knitting_toolbox-0.2.0/test/utils/test_transforms.py
+-rwxr-xr-x   0        0        0     2818 2023-05-30 21:15:50.827436 circuit_knitting_toolbox-0.2.0/tools/extremal_dependency_versions.py
+-rw-r--r--   0        0        0     1932 2023-05-30 21:15:50.827436 circuit_knitting_toolbox-0.2.0/tox.ini
+-rw-r--r--   0        0        0     8672 1970-01-01 00:00:00.000000 circuit_knitting_toolbox-0.2.0/PKG-INFO
```

### Comparing `circuit-knitting-toolbox-0.1.0/.github/workflows/README.md` & `circuit_knitting_toolbox-0.2.0/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/.github/workflows/citation.yml` & `circuit_knitting_toolbox-0.2.0/.github/workflows/citation.yml`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/.github/workflows/coverage.yml` & `circuit_knitting_toolbox-0.2.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/.github/workflows/docker.yml` & `circuit_knitting_toolbox-0.2.0/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/.github/workflows/docs.yml` & `circuit_knitting_toolbox-0.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/.github/workflows/lint.yml` & `circuit_knitting_toolbox-0.2.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/.github/workflows/release.yml` & `circuit_knitting_toolbox-0.2.0/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     runs-on: ubuntu-latest
     steps:
       - name: Checkout tag
         uses: actions/checkout@v3
         with:
           ref: ${{ github.ref_name }}
       - name: Publish release
-        uses: eloquent/github-release-action@v3
+        uses: ghalactic/github-release-from-tag@v4
         if: github.ref_type == 'tag'
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
           generateReleaseNotes: "true"
 
   pypi:
     name: pypi
```

### Comparing `circuit-knitting-toolbox-0.1.0/.github/workflows/test_development_versions.yml` & `circuit_knitting_toolbox-0.2.0/.github/workflows/test_minimum_versions.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-name: Development version tests
+name: Minimum version tests
 
 on:
   push:
     branches:
       - main
       - 'stable/**'
   pull_request:
     branches:
       - main
       - 'stable/**'
-  schedule:
-    - cron: '0 1 * * *'
 
 jobs:
   tests:
     runs-on: ubuntu-latest
     timeout-minutes: 30
     strategy:
       max-parallel: 4
       matrix:
-        python-version: [3.9]
+        python-version: [3.8]
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Install dependencies (development versions)
+      - name: Install dependencies (minimum versions)
         shell: bash
         run: |
-          python -m pip install --upgrade pip tox
+          python -m pip install --upgrade pip
           python -m pip install toml fire
-          python tools/extremal_dependency_versions.py pin_dependencies dev --inplace
+          pip install "tox==$(./tools/extremal_dependency_versions.py get_tox_minversion)"
+          python tools/extremal_dependency_versions.py pin_dependencies min --inplace
       - name: Modify tox.ini for more thorough check
         shell: bash
         run: |
           sed -i.bak -E '/#.*CI:[[:space:]]*skip-next-line/I{N;d;}' tox.ini
           cat tox.ini
       - name: Test using tox environment
         shell: bash
         run: |
           pver=${{ matrix.python-version }}
-          tox -epy${pver/./},py${pver/./}-notebook
+          tox -epy${pver/./} -- --run-slow
+          tox -epy${pver/./}-notebook
```

### Comparing `circuit-knitting-toolbox-0.1.0/.github/workflows/test_latest_versions.yml` & `circuit_knitting_toolbox-0.2.0/.github/workflows/test_latest_versions.yml`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
   tests:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 30
     strategy:
       max-parallel: 4
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.7", "3.11"]
+        python-version: ["3.8", "3.11"]
         include:
           - os: macos-latest
-            python-version: "3.7"
+            python-version: "3.8"
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
@@ -39,14 +39,14 @@
         run: |
           sed -i.bak -E '/#.*CI:[[:space:]]*skip-next-line/I{N;d;}' tox.ini
           cat tox.ini
       - name: Test using tox environment
         shell: bash
         run: |
           pver=${{ matrix.python-version }}
-          tox -epy${pver/./}
+          tox -epy${pver/./} -- --run-slow
           if [ "$pver" = "3.11" ]; then
             echo Skipping tutorials that require cplex
-            tox -epy${pver/./}-notebook  -- --ignore=docs/circuit_cutting/tutorials/tutorial_1_automatic_cut_finding.ipynb --ignore=docs/circuit_cutting/tutorials/tutorial_3_cutting_with_quantum_serverless.ipynb
+            tox -epy${pver/./}-notebook  -- --ignore=docs/circuit_cutting/cutqc/tutorials/tutorial_1_automatic_cut_finding.ipynb --ignore=docs/circuit_cutting/cutqc/tutorials/tutorial_3_cutting_with_quantum_serverless.ipynb
           else
             tox -epy${pver/./}-notebook
           fi
```

### Comparing `circuit-knitting-toolbox-0.1.0/.gitignore` & `circuit_knitting_toolbox-0.2.0/.gitignore`

 * *Files 21% similar despite different names*

```diff
@@ -51,7 +51,10 @@
 
 # virtualenv
 ENV/
 
 # Sphinx documentation
 docs/_build/
 docs/stubs/
+
+# Algorithm artifacts
+docplex_cutter.lp
```

### Comparing `circuit-knitting-toolbox-0.1.0/CITATION.bib` & `circuit_knitting_toolbox-0.2.0/CITATION.bib`

 * *Files 13% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 @misc{circuit-knitting-toolbox,
-  author = {Luciano Bello and Agata M. Bra\'{n}czyk and Sergey Bravyi and Andrew Eddins and Bryce Fuller and Julien Gacon and James R. Garrison and Jennifer R. Glick and Tanvi P. Gujarati and Ikko Hamamura and Areeq I. Hasan and Takashi Imamichi and Caleb Johnson and Ieva Liepuoniute and Owen Lockwood and Mario Motta and Pedro Rivero and Max Rossmannek and Travis L. Scholten and Seetharami Seelam and Iskandar Sitdikov and Dharmashankar Subramanian and Wei Tang and Stefan Woerner},
+  author = {Luciano Bello and Agata M. Bra\'{n}czyk and Sergey Bravyi and Almudena {Carrera Vazquez} and Andrew Eddins and Daniel J. Egger and Bryce Fuller and Julien Gacon and James R. Garrison and Jennifer R. Glick and Tanvi P. Gujarati and Ikko Hamamura and Areeq I. Hasan and Takashi Imamichi and Caleb Johnson and Ieva Liepuoniute and Owen Lockwood and Mario Motta and C. D. Pemmaraju and Pedro Rivero and Max Rossmannek and Travis L. Scholten and Seetharami Seelam and Iskandar Sitdikov and Dharmashankar Subramanian and Wei Tang and Stefan Woerner},
   title = {{Circuit Knitting Toolbox}},
   howpublished = {\url{https://github.com/Qiskit-Extensions/circuit-knitting-toolbox}},
-  year = {2022}
+  year = {2023}
 }
```

### Comparing `circuit-knitting-toolbox-0.1.0/CODE_OF_CONDUCT.md` & `circuit_knitting_toolbox-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/Dockerfile` & `circuit_knitting_toolbox-0.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/INSTALL.rst` & `circuit_knitting_toolbox-0.2.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/LICENSE.txt` & `circuit_knitting_toolbox-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/README.md` & `circuit_knitting_toolbox-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!-- SHIELDS -->
 <div align="left">
 
   [![Stability](https://img.shields.io/badge/Stability-alpha-f4d03f.svg)](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/releases)
   ![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS-informational)
-  [![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational)](https://www.python.org/)
-  [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.42.1-6133BD)](https://github.com/Qiskit/qiskit)
+  [![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational)](https://www.python.org/)
+  [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.43.0-6133BD)](https://github.com/Qiskit/qiskit)
   [![Qiskit Nature](https://img.shields.io/badge/Qiskit%20Nature-%E2%89%A5%200.5.2-6133BD)](https://github.com/Qiskit/qiskit-nature)
 <br />
   [![License](https://img.shields.io/github/license/Qiskit-Extensions/circuit-knitting-toolbox?label=License)](LICENSE.txt)
   [![Code style: Black](https://img.shields.io/badge/Code%20style-Black-000.svg)](https://github.com/psf/black)
   [![Tests](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/actions/workflows/test_latest_versions.yml/badge.svg)](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/actions/workflows/test_latest_versions.yml)
   [![Coverage](https://coveralls.io/repos/github/Qiskit-Extensions/circuit-knitting-toolbox/badge.svg?branch=main)](https://coveralls.io/github/Qiskit-Extensions/circuit-knitting-toolbox?branch=main)
 
@@ -30,15 +30,15 @@
 
 Each tool in the CKT partitions a user's problem into quantum and classical components to enable efficient use of resources constrained by scaling limits, i.e. size of quantum processors and classical compute capability. It can assign the execution of "quantum code" to QPUs or QPU simulators and "classical code" to various heterogeneous classical resources such as CPUs, GPUs, and TPUs made available via hybrid cloud, on-prem, data centers, etc. 
 
 The toolbox enables users to run parallelized and hybrid (quantum + classical) workloads without worrying about allocating and managing underlying infrastructure.
 
 The toolbox currently contains the following tools:
 - Entanglement Forging [[1]](#references)
-- Circuit Cutting [[2]](#references)
+- Circuit Cutting [[2-6]](#references)
   
 ----------------------------------------------------------------------------------------------------
   
 ### Documentation
 
 The documentation, including installation instructions, is available at https://qiskit-extensions.github.io/circuit-knitting-toolbox/.
 
@@ -48,16 +48,24 @@
 
 This project is meant to evolve rapidly and, as such, does not follow [Qiskit's deprecation policy](https://qiskit.org/documentation/contributing_to_qiskit.html#deprecation-policy).  We may occasionally make breaking changes in order to improve the user experience.  When possible, we will keep old interfaces and mark them as deprecated, as long as they can co-exist with the new ones.  Each substantial improvement, breaking change, or deprecation will be documented in the [release notes](https://qiskit-extensions.github.io/circuit-knitting-toolbox/release-notes.html).
 
 ----------------------------------------------------------------------------------------------------
 
 ### References
 
-[1] Andrew Eddins, Mario Motta, Tanvi P. Gujarati, Sergey Bravyi, Antonio Mezzacapo, Charles Hadfield, Sarah Sheldon, [Doubling the size of quantum simulators by entanglement forging](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.3.010309). PRX Quantum 3, 010309 (2022).
+[1] Andrew Eddins, Mario Motta, Tanvi P. Gujarati, Sergey Bravyi, Antonio Mezzacapo, Charles Hadfield, Sarah Sheldon, [Doubling the size of quantum simulators by entanglement forging](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.3.010309), PRX Quantum 3, 010309 (2022).
 
-[2] Wei Tang, Teague Tomesh, Martin Suchara, Jeffrey Larson, Margaret Martonosi, [CutQC: Using Small Quantum Computers for Large Quantum Circuit Evaluations](https://doi.org/10.1145/3445814.3446758), Proceedings of the 26th ACM International Conference on Architectural Support for Programming Languages and Operating Systems. pp. 473 (2021).
+[2] Kosuke Mitarai, Keisuke Fujii, [Constructing a virtual two-qubit gate by sampling single-qubit operations](https://iopscience.iop.org/article/10.1088/1367-2630/abd7bc), New J. Phys. 23 023021.
 
+[3] Christophe Piveteau, David Sutter, [Circuit knitting with classical communication](https://arxiv.org/abs/2205.00016), arXiv:2205.00016 [quant-ph].
+
+[4] Lukas Brenner, Christophe Piveteau, David Sutter, [Optimal wire cutting with classical communication](https://arxiv.org/abs/2302.03366), arXiv:2302.03366 [quant-ph].
+
+[5] Wei Tang, Teague Tomesh, Martin Suchara, Jeffrey Larson, Margaret Martonosi, [CutQC: Using small quantum computers for large quantum circuit evaluations](https://doi.org/10.1145/3445814.3446758), Proceedings of the 26th ACM International Conference on Architectural Support for Programming Languages and Operating Systems. pp. 473 (2021).
+  
+[6] K. Temme, S. Bravyi, and J. M. Gambetta, [Error mitigation for short-depth quantum circuits](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.119.180509), Physical Review Letters, 119(18), (2017).
+  
 ----------------------------------------------------------------------------------------------------
 
 <!-- LICENSE -->
 ### License
 [Apache License 2.0](LICENSE.txt)
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/__init__.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Code to initialize the wire cutting imports."""
+"""Code to initialize the cutqc imports."""
 
 from .wire_cutting_evaluation import run_subcircuit_instances
 from .wire_cutting_post_processing import generate_summation_terms, build
 from .wire_cutting_verification import verify
 from .wire_cutting import (
     cut_circuit_wires,
     evaluate_subcircuits,
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/mip_model.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/mip_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,33 +33,14 @@
 
     This class represents circuit cutting as a Mixed Integer Programming (MIP) problem
     that can then be solved (provably) optimally using a MIP solver. This is integrated
     with CPLEX, a fast commercial solver sold by IBM. There are free and open source MIP
     solvers, but they come with substantial slowdowns (often many orders of magnitude).
     By representing the original circuit as a Directed Acyclic Graph (DAG), this class
     can find the optimal wire cuts in the circuit.
-
-    Attributes:
-        - n_vertices (int): the number of vertices in the circuit DAG
-        - edges (list): the list of edges of the circuit DAG
-        - n_edges (int): the number of edges
-        - vertex_ids (dict): dictionary mapping vertices (i.e. two qubit gates) to the vertex
-            id (i.e. a number)
-        - id_vertices (dict): the inverse dictionary of vertex_ids, which has keys of vertex ids
-            and values of the vertices
-        - num_subcircuit (int): the number of subcircuits
-        - max_subcircuit_width (int): maximum number of qubits per subcircuit
-        - max_subcircuit_cuts (int): maximum number of cuts in each subcircuit
-        - max_subcircuit_size (int): maximum number of gates in a subcircuit
-        - num_qubits (int): the number of qubits in the circuit
-        - max_cuts (int): the maximum total number of cuts
-        - subcircuit_counter (dict): a tracker for the information regarding subcircuits
-        - vertex_weight (dict): keep track of the number of input qubits directly connected
-            to each node
-        - model (docplex model): the model interface for CPLEX
     """
 
     def __init__(
         self,
         n_vertices: int,
         edges: Sequence[tuple[int]],
         vertex_ids: dict[str, int],
@@ -71,30 +52,30 @@
         num_qubits: int,
         max_cuts: int,
     ):
         """
         Initialize member variables.
 
         Args:
-            - n_vertices (int): the number of vertices in the circuit DAG
-            - edges (list): the list of edges of the circuit DAG
-            - n_edges (int): the number of edges
-            - vertex_ids (dict): dictionary mapping vertices (i.e. two qubit gates) to the vertex
+            n_vertices: The number of vertices in the circuit DAG
+            edges: The list of edges of the circuit DAG
+            n_edges: The number of edges
+            vertex_ids: Dictionary mapping vertices (i.e. two qubit gates) to the vertex
                 id (i.e. a number)
-            - id_vertices (dict): the inverse dictionary of vertex_ids, which has keys of vertex ids
+            id_vertices: The inverse dictionary of vertex_ids, which has keys of vertex ids
                 and values of the vertices
-            - num_subcircuit (int): the number of subcircuits
-            - max_subcircuit_width (int): maximum number of qubits per subcircuit
-            - max_subcircuit_cuts (int): maximum number of cuts in each subcircuit
-            - max_subcircuit_size (int): maximum number of gates in a subcircuit
-            - num_qubits (int): the number of qubits in the circuit
-            - max_cuts (int): the maximum total number of cuts
+            num_subcircuit: The number of subcircuits
+            max_subcircuit_width: Maximum number of qubits per subcircuit
+            max_subcircuit_cuts: Maximum number of cuts in each subcircuit
+            max_subcircuit_size: Maximum number of gates in a subcircuit
+            num_qubits: The number of qubits in the circuit
+            max_cuts: The maximum total number of cuts
 
         Returns:
-            - None
+            None
         """
         self.check_graph(n_vertices, edges)
         self.n_vertices = n_vertices
         self.edges = edges
         self.n_edges = len(edges)
         self.vertex_ids = vertex_ids
         self.id_vertices = id_vertices
@@ -121,20 +102,15 @@
 
         self.model = Model("docplex_cutter")
         self.model.log_output = False
         self._add_variables()
         self._add_constraints()
 
     def _add_variables(self) -> None:
-        """
-        Add the necessary variables to the CPLEX model.
-
-        Returns:
-            - None
-        """
+        """Add the necessary variables to the CPLEX model."""
         """
         Indicate if a vertex is in some subcircuit
         """
         self.vertex_var = []
         for i in range(self.num_subcircuit):
             subcircuit_y = []
             for j in range(self.n_vertices):
@@ -217,20 +193,15 @@
                 self.subcircuit_counter[subcircuit][
                     "build_cost_exponent"
                 ] = self.model.integer_var(
                     lb=lb, ub=ub, name="build_cost_exponent_%d" % subcircuit
                 )
 
     def _add_constraints(self) -> None:
-        """
-        Add all contraints and objectives to MIP model.
-
-        Returns:
-            - None
-        """
+        """Add all contraints and objectives to MIP model."""
         """
         each vertex in exactly one subcircuit
         """
         for v in range(self.n_vertices):
             ctName = "cons_vertex_" + str(v)
             self.model.add_constraint(
                 self.model.sum(
@@ -417,27 +388,26 @@
 
         # self.model.setObjective(self.num_cuts,gp.GRB.MINIMIZE)
         self.model.set_objective("min", self.num_cuts)
 
     def pwl_exp(
         self, lb: int, ub: int, base: int, coefficient: int, integer_only: bool
     ) -> tuple[list[int], list[int]]:
-        """
+        r"""
         Approximate a nonlinear exponential function via a piecewise linear function.
 
         Args:
-            - lb (int): lower bound
-            - ub (int): upper bound
-            - base (int): the base of the input exponential
-            - coefficient (int): the coefficient of the original exponential
-            - integer_only (bool): whether the input x's are only integers
+            lb: Lower bound
+            ub: Upper bound
+            base: The base of the input exponential
+            coefficient: The coefficient of the original exponential
+            integer_only: Whether the input x's are only integers
 
         Returns:
-            - (list): the x's of the piecewise approximation
-            - (list): the f(x)'s of the piecewise approximation
+            A tuple containing the :math:`x`\ s and :math:`f(x)`\ s of the piecewise approximation
         """
         # Piecewise linear approximation of coefficient*base**x
         ptx = []
         ptf = []
 
         x_range = range(lb, ub + 1) if integer_only else list(np.linspace(lb, ub, 200))
         # print('x_range : {}, integer_only : {}'.format(x_range,integer_only))
@@ -451,22 +421,22 @@
         """
         Ensure circuit DAG is viable.
 
         This means that there are no oversized edges, that all edges are from viable nodes,
         and that the graph is otherwise a valid graph.
 
         Args:
-            - n_vertices (int): the number of vertices
-            - edges (list): the edge list
+            n_vertices: The number of vertices
+            edges: The edge list
 
         Returns:
-            - None
+            None
 
         Raises:
-            - ValueError: if the graph is invalid
+            ValueError: The graph is invalid
         """
         # 1. edges must include all vertices
         # 2. all u,v must be ordered and smaller than n_vertices
         vertices = set([i for (i, _) in edges])  # type: ignore
         vertices |= set([i for (_, i) in edges])  # type: ignore
         assert vertices == set(range(n_vertices))
         for edge in edges:
@@ -482,19 +452,19 @@
                 )
 
     def solve(self, min_postprocessing_cost: float) -> bool:
         """
         Solve the MIP model.
 
         Args:
-            - min_post_processing_cost (float): the predicted minimum post-processing cost,
+            min_post_processing_cost: The predicted minimum post-processing cost,
                 often is inf
 
         Returns:
-            - (bool): whether or not the model found a solution
+            Flag denoting whether or not the model found a solution
         """
         # print('solving for %d subcircuits'%self.num_subcircuit)
         # print('model has %d variables, %d linear constraints,%d quadratic constraints, %d general constraints'
         # % (self.model.NumVars,self.model.NumConstrs, self.model.NumQConstrs, self.model.NumGenConstrs))
         print(
             "Exporting as a LP file to let you check the model that will be solved : ",
             min_postprocessing_cost,
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/wire_cutting.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,30 +38,31 @@
     num_subcircuits: Sequence[int] | None = None,
     verbose: bool = True,
 ) -> dict[str, Any]:
     """
     Decompose the circuit into a collection of subcircuits.
 
     Args:
-        - method (str): whether to have the cuts be 'automatically' found, in a
+        method: Whether to have the cuts be 'automatically' found, in a
             provably optimal way, or whether to 'manually' specify the cuts
-        - subcircuit_vertices (Sequence[Sequence[int]]): the vertices to be used in
-            the subcircuits. Note that these are not the indices of the qubits, but
-            the nodes in the circuit DAG
-        - max_subcircuit_width (int): max number of qubits in each subcircuit
-        - max_cuts (int): max total number of cuts allowed
-        - num_subcircuits (Sequence[int]): list of number of subcircuits to try
-        - max_subcircuit_cuts (int, optional): max number of cuts for a subcircuit
-        - max_subcircuit_size (int, optional): max number of gates in a subcircuit
-        - verbose (bool, optional): flag for printing output of cutting
+        subcircuit_vertices: The vertices to be used in the subcircuits. Note
+            that these are not the indices of the qubits, but the nodes in the circuit DAG
+        max_subcircuit_width: Max number of qubits in each subcircuit
+        max_cuts: Max total number of cuts allowed
+        num_subcircuits: List of number of subcircuits to try
+        max_subcircuit_cuts: Max number of cuts for a subcircuit
+        max_subcircuit_size: Max number of gates in a subcircuit
+        verbose: Flag for printing output of cutting
+
     Returns:
-        (dict[str, Any]): A dictionary containing information on the cuts,
-        including the subcircuits themselves (key: 'subcircuits')
+        A dictionary containing information on the cuts, including the subcircuits
+        themselves (key: 'subcircuits')
+
     Raises:
-        - ValueError: if the input method does not match the other provided arguments
+        ValueError: The input method does not match the other provided arguments
     """
     cuts = {}
     if method == "automatic":
         if max_subcircuit_width is None:
             raise ValueError(
                 "The max_subcircuit_width argument must be set if using automatic cut finding."
             )
@@ -96,21 +97,21 @@
     backend_names: str | Sequence[str] | None = None,
     options: Options | Sequence[Options] | None = None,
 ) -> dict[int, dict[int, np.ndarray]]:
     """
     Evaluate the subcircuits.
 
     Args:
-        - cuts (dict): the results of cutting
-        - service (QiskitRuntimeService | None): A service for connecting to Qiskit Runtime Service
-        - options (Options | Sequence[Options] | None): Options to use on each backend
-        - backend_names (str | Sequence[str] | None): The name(s) of the backend(s) to be used
+        cuts: The results of cutting
+        service: A service for connecting to Qiskit Runtime Service
+        options: Options to use on each backend
+        backend_names: The name(s) of the backend(s) to be used
+
     Returns:
-        (dict): the dictionary containing the results from running
-        each of the subcircuits
+        The dictionary containing the results from running each of the subcircuits
     """
     # Put backend_names and options in lists to ensure it is unambiguous how to sync them
     backends_list: Sequence[str] = []
     options_list: Sequence[Options] = []
     if backend_names is None or isinstance(backend_names, str):
         if isinstance(options, Options):
             options_list = [options]
@@ -126,15 +127,17 @@
             options_list = [None] * len(backends_list)
         else:
             options_list = options
 
     if backend_names:
         if len(backends_list) != len(options_list):
             raise AttributeError(
-                f"The list of backend names is length ({len(backends_list)}), but the list of options is length ({len(options_list)}). It is ambiguous how these options should be applied."
+                f"The list of backend names is length ({len(backends_list)}), "
+                f"but the list of options is length ({len(options_list)}). "
+                "It is ambiguous how these options should be applied."
             )
 
     _, _, subcircuit_instances = _generate_metadata(cuts)
 
     subcircuit_instance_probabilities = _run_subcircuits(
         cuts,
         subcircuit_instances,
@@ -152,20 +155,21 @@
     cuts: dict[str, Any],
     num_threads: int = 1,
 ) -> np.ndarray:
     """
     Reconstruct the full probabilities from the subcircuit evaluations.
 
     Args:
-        - circuit (QuantumCircuit): the original full circuit
-        - subcircuit_instance_probabilities (dict): the probability vectors from each
+        circuit: The original full circuit
+        subcircuit_instance_probabilities: The probability vectors from each
             of the subcircuit instances, as output by the _run_subcircuits function
-        - num_threads (int): the number of threads to use to parallelize the recomposing
+        num_threads: The number of threads to use to parallelize the recomposing
+
     Returns:
-        - (np.ndarray): the reconstructed probability vector
+        The reconstructed probability vector
     """
     summation_terms, subcircuit_entries, _ = _generate_metadata(cuts)
 
     subcircuit_entry_probabilities = _attribute_shots(
         subcircuit_entries, subcircuit_instance_probabilities
     )
 
@@ -194,19 +198,20 @@
     dict[int, dict[tuple[str, str], tuple[int, Sequence[tuple[int, int]]]]],
     dict[int, dict[tuple[tuple[str, ...], tuple[Any, ...]], int]],
 ]:
     """
     Generate metadata used to execute subcircuits and reconstruct probabilities of original circuit.
 
     Args:
-        - cuts (dict[str, Any]): results from the cutting step
+        cuts: Results from the cutting step
+
     Returns:
-        - (tuple): information about the 4^(num cuts) summation terms used to reconstruct original
-            probabilities, a dictionary with information on each of the subcircuits, and a dictionary
-            containing indexes for each of the subcircuits
+        Information about the 4^(num cuts) summation terms used to reconstruct original
+        probabilities, a dictionary with information on each of the subcircuits, and a dictionary
+        containing indexes for each of the subcircuits
     """
     (
         summation_terms,
         subcircuit_entries,
         subcircuit_instances,
     ) = generate_summation_terms(
         subcircuits=cuts["subcircuits"],
@@ -225,22 +230,23 @@
 ) -> dict[int, dict[int, np.ndarray]]:
     """
     Execute all the subcircuit instances.
 
     task['subcircuit_instance_probs'][subcircuit_idx][subcircuit_instance_idx] = measured prob
 
     Args:
-        - cuts (dict[str, Any]): results from the cutting step
-        - subcircuit_instances (dict): the dictionary containing the index information for each
+        cuts: Results from the cutting step
+        subcircuit_instances: The dictionary containing the index information for each
             of the subcircuit instances
-        - service (QiskitRuntimeService | None): the arguments for the runtime service
-        - backend_names (Sequence[str] | None): the backend(s) used to run the subcircuits
-        - options (Options | None): options for the runtime execution of subcircuits
+        service: The arguments for the runtime service
+        backend_names: The backend(s) used to run the subcircuits
+        options: Options for the runtime execution of subcircuits
+
     Returns:
-        - (dict): the resulting probabilities from each of the subcircuit instances
+        The resulting probabilities from each of the subcircuit instances
     """
     subcircuit_instance_probs = run_subcircuit_instances(
         subcircuits=cuts["subcircuits"],
         subcircuit_instances=subcircuit_instances,
         service=service,
         backend_names=backend_names,
         options=options,
@@ -257,23 +263,25 @@
 ) -> dict[int, dict[int, np.ndarray]]:
     """
     Attribute the shots into respective subcircuit entries.
 
     task['subcircuit_entry_probs'][subcircuit_idx][subcircuit_entry_idx] = prob
 
     Args:
-        - subcircuit_entries (dict): dictionary containing information about each of the
+        subcircuit_entries: Dictionary containing information about each of the
             subcircuit instances
-        - subcircuit_instance_probs (dict): the probability vectors from each of the subcircuit
+        subcircuit_instance_probs: The probability vectors from each of the subcircuit
             instances, as output by the _run_subcircuits function
+
     Returns:
-        - (dict): a dictionary containing the probability results to each of the appropriate subcircuits
+        A dictionary containing the probability results to each of the appropriate subcircuits
+
     Raises:
-        - ValueError: if each of the kronecker terms are not of size two or if there are no subcircuit
-            probs provided
+        ValueError: A kronecker term is not size two
+        ValueError: There are no subcircuit probs provided
     """
     subcircuit_entry_probs: dict[int, dict[int, np.ndarray]] = {}
     for subcircuit_idx in subcircuit_entries:
         subcircuit_entry_probs[subcircuit_idx] = {}
         for label in subcircuit_entries[subcircuit_idx]:
             subcircuit_entry_idx, kronecker_term = subcircuit_entries[subcircuit_idx][
                 label
@@ -319,24 +327,25 @@
     """
     Find optimal cuts for the wires.
 
     Will print if the model cannot find a solution at all, and will print whether
     the found solution is optimal or not.
 
     Args:
-        - circuit (QuantumCircuit): original quantum circuit to be cut into subcircuits
-        - max_subcircuit_width (int): max number of qubits in each subcircuit
-        - max_cuts (int, optional): max total number of cuts allowed
-        - num_subcircuits (list, optional): list of number of subcircuits to try
-        - max_subcircuit_cuts (int, optional): max number of cuts for a subcircuit
-        - max_subcircuit_size (int, optional): the maximum number of two qubit gates in each
+        circuit: Original quantum circuit to be cut into subcircuits
+        max_subcircuit_width: Max number of qubits in each subcircuit
+        max_cuts: Max total number of cuts allowed
+        num_subcircuits: List of number of subcircuits to try
+        max_subcircuit_cuts: Max number of cuts for a subcircuit
+        max_subcircuit_size: The maximum number of two qubit gates in each
             subcircuit
-        - verbose (bool): whether to print information about the cut finding or not
+        verbose: Whether to print information about the cut finding or not
+
     Returns:
-        - (dict): the solution found for the cuts
+        The solution found for the cuts
     """
     stripped_circ = _circuit_stripping(circuit=circuit)
     n_vertices, edges, vertex_ids, id_vertices = _read_circuit(circuit=stripped_circ)
     num_qubits = circuit.num_qubits
     cut_solution = {}
     min_cost = float("inf")
 
@@ -429,19 +438,20 @@
 ) -> dict[str, Any]:
     """
     Perform the provided cuts.
 
     Used when cut locations are chosen manually.
 
     Args:
-        - circuit (QuantumCircuit): original quantum circuit to be cut into subcircuits
-        - subcircuit_vertices (list): the list of vertices to apply the cuts to
-        - verbose (bool): whether to print the details of cutting or not
+        circuit: Original quantum circuit to be cut into subcircuits
+        subcircuit_vertices: The list of vertices to apply the cuts to
+        verbose: Whether to print the details of cutting or not
+
     Returns:
-        - (dict): the solution calculated from the provided cuts
+        The solution calculated from the provided cuts
     """
     stripped_circ = _circuit_stripping(circuit=circuit)
     n_vertices, edges, vertex_ids, id_vertices = _read_circuit(circuit=stripped_circ)
 
     subcircuit_list = []
     for vertices in subcircuit_vertices:
         subcircuit = []
@@ -493,22 +503,23 @@
     counter: dict[int, dict[str, int]],
     classical_cost: float,
 ) -> None:
     """
     Pretty print the results.
 
     Args:
-        - num_subciruit (int): the number of subcircuits
-        - num_cuts (int): the number of cuts
-        - subcircuits (list): the list of subcircuits
-        - counter (dict): the dictionary containing all meta information regarding
+        num_subciruit: The number of subcircuits
+        num_cuts: The number of cuts
+        subcircuits: The list of subcircuits
+        counter: The dictionary containing all meta information regarding
             each of the subcircuits
-        - classical_cost (float): the estimated processing cost
+        classical_cost: The estimated processing cost
+
     Returns:
-        - None
+        None
     """
     for subcircuit_idx in range(num_subcircuit):
         print("subcircuit %d" % subcircuit_idx)
         print(
             "\u03C1 qubits = %d, O qubits = %d, width = %d, effective = %d, depth = %d, size = %d"
             % (
                 counter[subcircuit_idx]["rho"],
@@ -526,19 +537,20 @@
 def _cuts_parser(
     cuts: Sequence[tuple[str]], circ: QuantumCircuit
 ) -> list[tuple[Qubit, int]]:
     """
     Convert cuts to wires.
 
     Args:
-        - cuts (list): the cuts found by the model (or provided by the user)
-        - circ (QuantumCircuit): the quantum circuit the cuts are from
+        cuts: The cuts found by the model (or provided by the user)
+        circ: The quantum circuit the cuts are from
+
     Returns:
-        - (list): the list containing the wires that were cut and the gates
-            that are affected by these cuts
+        The list containing the wires that were cut and the gates
+        that are affected by these cuts
     """
     dag = circuit_to_dag(circ)
     positions = []
     for position in cuts:
         if len(position) != 2:
             raise ValueError(
                 "position variable should be a length 2 sequence: {position}"
@@ -598,19 +610,19 @@
 def _subcircuits_parser(
     subcircuit_gates: list[list[str]], circuit: QuantumCircuit
 ) -> tuple[Sequence[QuantumCircuit], dict[Qubit, list[dict[str, int | Qubit]]]]:
     """
     Convert the subcircuit gates into quantum circuits and path out the DAGs to enable conversion.
 
     Args:
-        - subcircuit_gates (list): the gates in the subcircuits
-        - circuit (QuantumCircuit): the original circuit
+        subcircuit_gates: The gates in the subcircuits
+        circuit: The original circuit
+
     Returns:
-        - (list): the subcircuits
-        - (dict): the paths in the quantum circuit DAGs
+        A tuple containing he subcircuits and the paths in the quantum circuit DAGs
     """
     """
     Assign the single qubit gates to the closest two-qubit gates
     """
 
     def calculate_distance_between_gate(gate_A, gate_B):
         if len(gate_A.split(" ")) >= len(gate_B.split(" ")):
@@ -738,20 +750,21 @@
     """
     Generate the subcircuits from given nodes and paths.
 
     Called in the subcircuit_parser function to convert the found paths and nodes
     into actual quantum circuit objects.
 
     Args:
-        - subcircuit_op_nodes (dict): the nodes of each of the subcircuits
-        - complete_path_map (dict): the complete path through the subcircuits
-        - subcircuit_sizes (list): the number of qubits in each of the subcircuits
-        - dag (DAGCircuit): the dag representation of the input quantum circuit
+        subcircuit_op_nodes: The nodes of each of the subcircuits
+        complete_path_map: The complete path through the subcircuits
+        subcircuit_sizes: The number of qubits in each of the subcircuits
+        dag: The dag representation of the input quantum circuit
+
     Returns:
-        - (list): the subcircuits
+        The subcircuits
     """
     qubit_pointers = {x: 0 for x in complete_path_map}
     subcircuits = [QuantumCircuit(x, name="q") for x in subcircuit_sizes]
     for op_node in dag.topological_op_nodes():
         subcircuit_idx_list = list(
             filter(
                 lambda x: op_node in subcircuit_op_nodes[x], subcircuit_op_nodes.keys()
@@ -786,19 +799,19 @@
     subcircuits: Sequence[QuantumCircuit],
     O_rho_pairs: list[tuple[dict[str, int | Qubit], dict[str, int | Qubit]]],
 ) -> dict[int, dict[str, int]]:
     """
     Create information regarding each of the subcircuit parameters (qubits, width, etc.).
 
     Args:
-        - subcircuits (list): the list of subcircuits
-        - O_rho_pairs (list): the pairs for each qubit path as generated in the _get_pairs
-            function
+        subcircuits: The list of subcircuits
+        O_rho_pairs: The pairs for each qubit path as generated in the _get_pairs function
+
     Returns:
-        - (dict): the resulting dictionary with all parameter information
+        The resulting dictionary with all parameter information
     """
     counter = {}
     for subcircuit_idx, subcircuit in enumerate(subcircuits):
         counter[subcircuit_idx] = {
             "effective": subcircuit.num_qubits,
             "rho": 0,
             "O": 0,
@@ -818,18 +831,18 @@
 
 
 def _cost_estimate(counter: dict[int, dict[str, int]]) -> float:
     """
     Estimate the cost of processing the subcircuits.
 
     Args:
-        - counter (dict): dictionary containing information for each of the
-            subcircuits
+        counter: Dictionary containing information for each of the subcircuits
+
     Returns:
-        - (float): the estimated cost for classical processing
+        The estimated cost for classical processing
     """
     num_cuts = sum([counter[subcircuit_idx]["rho"] for subcircuit_idx in counter])
     subcircuit_indices = list(counter.keys())
     num_effective_qubits_list = [
         counter[subcircuit_idx]["effective"] for subcircuit_idx in subcircuit_indices
     ]
     num_effective_qubits, _ = zip(
@@ -850,17 +863,18 @@
     """
     Get all pairs through each path.
 
     Iterates through the path for each of the qubits and keeps track of the
     each pair of neigbors.
 
     Args:
-        - complete_path_map (dict): the dictionary containing all path information
+        complete_path_map: The dictionary containing all path information
+
     Returns:
-        - (list): all pairs for each of the qubit paths
+        All pairs for each of the qubit paths
     """
     O_rho_pairs = []
     for input_qubit in complete_path_map:
         path = complete_path_map[input_qubit]
         if len(path) > 1:
             for path_ctr, item in enumerate(path[:-1]):
                 O_qubit_tuple = item
@@ -870,17 +884,18 @@
 
 
 def _circuit_stripping(circuit: QuantumCircuit) -> QuantumCircuit:
     """
     Remove all single qubit and barrier type gates.
 
     Args:
-        - circuit (QuantumCircuit): the circuit to strip
+        circuit: The circuit to strip
+
     Returns:
-        - (QuantumCircuit): the stripped circuit
+        The stripped circuit
     """
     # Remove all single qubit gates and barriers in the circuit
     dag = circuit_to_dag(circuit)
     stripped_dag = DAGCircuit()
     [stripped_dag.add_qreg(x) for x in circuit.qregs]
     for vertex in dag.topological_op_nodes():
         if len(vertex.qargs) == 2 and vertex.op.name != "barrier":
@@ -891,21 +906,19 @@
 def _read_circuit(
     circuit: QuantumCircuit,
 ) -> tuple[int, list[tuple[int, int]], dict[str, int], dict[int, str]]:
     """
     Read the input circuit to a graph based representation for the MIP model.
 
     Args:
-        - circuit (QuantumCircuit): a stripped circuit to be converted into a
-            DAG like representation
+        circuit: A stripped circuit to be converted into a DAG like representation
+
     Returns:
-        - (int): number of vertices
-        - (list): edge list
-        - (dict): the dictionary mapping vertices to vertex numbers
-        - (dict): the dictionary mapping vertex numbers to vertex information
+        A tuple containing the number of vertices, edge list, vertex to vertex id mapping,
+        and vertex id to vertex mapping.
     """
     dag = circuit_to_dag(circuit)
     edges = []
     node_name_ids = {}
     id_node_names = {}
     vertex_ids = {}
     curr_node_id = 0
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_evaluation.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/wire_cutting_evaluation.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,28 +38,30 @@
     Execute all provided subcircuits.
 
     Using the backend(s) provided, this executes all the subcircuits to generate the
     resultant probability vectors.
     subcircuit_instance_probs[subcircuit_idx][subcircuit_instance_idx] = measured probability
 
     Args:
-        - subcircuits (Sequence[QuantumCircuit]): the list of subcircuits to execute
-        - subcircuit_instances (dict): dictionary containing information about each of the
+        subcircuits: The list of subcircuits to execute
+        subcircuit_instances: Dictionary containing information about each of the
             subcircuit instances
-        - service (QiskitRuntimeService | None): the runtime service
-        - backend_names (Sequence[str] | None): the backend(s) used to execute the subcircuits
-        - options (Sequence[Options] | None): options for the runtime execution of subcircuits
+        service: The runtime service
+        backend_names: The backend(s) used to execute the subcircuits
+        options: Options for the runtime execution of subcircuits
 
     Returns:
-        - (dict): the probability vectors from each of the subcircuit instances
+        The probability vectors from each of the subcircuit instances
     """
     if backend_names and options:
         if len(backend_names) != len(options):
             raise AttributeError(
-                f"The list of backend names is length ({len(backend_names)}), but the list of options is length ({len(options)}). It is ambiguous how these options should be applied."
+                f"The list of backend names is length ({len(backend_names)}), "
+                f"but the list of options is length ({len(options)}). It is ambiguous "
+                "how these options should be applied."
             )
     if service:
         if backend_names:
             backend_names_repeated: list[str | None] = [
                 backend_names[i % len(backend_names)] for i, _ in enumerate(subcircuits)
             ]
             if options is None:
@@ -104,18 +106,18 @@
     """
     Change of basis for all identity measurements.
 
     For every identity measurement, it is split into an I and Z measurement.
     I and Z measurement basis correspond to the same logical circuit.
 
     Args:
-        - meas (tuple): the current measurement bases
+        meas: The current measurement bases
 
     Returns:
-        - (tuple): the update measurement bases
+        The update measurement bases
     """
     if all(x != "I" for x in meas):
         return [meas]
     else:
         mutated_meas = []
         for x in meas:
             if x != "I":
@@ -130,24 +132,24 @@
 def modify_subcircuit_instance(
     subcircuit: QuantumCircuit, init: tuple[str, ...], meas: tuple[str, ...]
 ) -> QuantumCircuit:
     """
     Modify the initialization and measurement bases for a given subcircuit.
 
     Args:
-        - subcircuit (QuantumCircuit): the subcircuit to be modified
-        - init (tuple): the current initializations
-        - meas (tuple): the current measement bases
+        subcircuit: The subcircuit to be modified
+        init: The current initializations
+        meas: The current measement bases
 
     Returns:
-        - (QuantumCircuit): the updated circuit, modified so the initialziation
-            and measurement operators are all in the standard computational basis
+        The updated circuit, modified so the initialziation
+        and measurement operators are all in the standard computational basis
 
     Raises:
-        - Exeption: if one of the init's or meas's are not an acceptable string
+        Exeption: One of the inits or meas's are not an acceptable string
     """
     subcircuit_dag = circuit_to_dag(subcircuit)
     subcircuit_instance_dag = copy.deepcopy(subcircuit_dag)
     for i, x in enumerate(init):
         q = subcircuit.qubits[i]
         if x == "zero":
             continue
@@ -211,19 +213,19 @@
     subcircuits: Sequence[QuantumCircuit],
     sampler: BaseSampler,
 ) -> list[np.ndarray]:
     """
     Execute the subcircuit(s).
 
     Args:
-        - subcircuit (QuantumCircuit): the subcircuits to be executed
-        - sampler (BaseSampler): the Sampler to use for executions
+        subcircuit: The subcircuits to be executed
+        sampler: The Sampler to use for executions
 
     Returns:
-        - (np.ndarray): the probability distributions
+        The probability distributions
     """
     for subcircuit in subcircuits:
         if subcircuit.num_clbits == 0:
             subcircuit.measure_all()
 
     quasi_dists = sampler.run(circuits=subcircuits).result().quasi_dists
 
@@ -245,21 +247,21 @@
     backend_name: str | None = None,
     options: Options | None = None,
 ) -> list[np.ndarray]:
     """
     Execute the subcircuit(s).
 
     Args:
-        - subcircuit (QuantumCircuit): the subcircuits to be executed
-        - service (QiskitRuntimeService | None): the runtime service
-        - backend_name (str | None): the backend used to execute the subcircuits
-        - options (Options | None): options for the runtime execution of subcircuits
+        subcircuit: The subcircuits to be executed
+        service: The runtime service
+        backend_name: The backend used to execute the subcircuits
+        options: Options for the runtime execution of subcircuits
 
     Returns:
-        - (np.ndarray): the probability distributions
+        The probability distributions
     """
     if service is not None:
         session = Session(service=service, backend=backend_name)
         sampler = Sampler(session=session, options=options)
     else:
         sampler = TestSampler(options=options)
 
@@ -267,19 +269,19 @@
 
 
 def measure_prob(unmeasured_prob: np.ndarray, meas: tuple[Any, ...]) -> np.ndarray:
     """
     Compute the effective probability distribution from the subcircuit distribution.
 
     Args:
-        - unmeasured_prob (Sequence[float]): the outputs of the subcircuit execution
-        - meas (tuple): the measurement bases
+        unmeasured_prob: The outputs of the subcircuit execution
+        meas: The measurement bases
 
     Returns:
-        - (np.ndarray): the updated measured probability distribution
+        The updated measured probability distribution
     """
     if meas.count("comp") == len(meas):
         return np.array(unmeasured_prob)
     else:
         measured_prob = np.zeros(int(2 ** meas.count("comp")))
         for full_state, p in enumerate(unmeasured_prob):
             sigma, effective_state = measure_state(full_state=full_state, meas=meas)
@@ -292,20 +294,20 @@
 def measure_state(full_state: int, meas: tuple[Any, ...]) -> tuple[int, int]:
     """
     Compute the corresponding effective_state for the given full_state.
 
     Measured in basis `meas`. Returns sigma (int), effective_state (int) where sigma = +-1
 
     Args:
-        - full_state (int): the current state (in decimal form)
-        - meas (tuple): the measurement bases
+        full_state: The current state (in decimal form)
+        meas: The measurement bases
 
     Returns:
-        - (tuple): sigma (defined by the parity of non computational basis 1 measurements) and
-            the effective state (defined by the measurements in the computational basis)
+        Sigma (defined by the parity of non computational basis 1 measurements) and
+        the effective state (defined by the measurements in the computational basis)
     """
     bin_full_state = bin(full_state)[2:].zfill(len(meas))
     sigma = 1
     bin_effective_state = ""
     for meas_bit, meas_basis in zip(bin_full_state, meas[::-1]):
         if meas_bit == "1" and meas_basis != "I" and meas_basis != "comp":
             sigma *= -1
@@ -323,24 +325,24 @@
     backend_name: str | None = None,
     options: Options | None = None,
 ):
     """
     Execute a circuit using qiskit runtime.
 
     Args:
-        - subcircuit_instances (dict): dictionary containing information about each of the
+        subcircuit_instances: Dictionary containing information about each of the
             subcircuit instances
-        - subcircuit (QuantumCircuit): the subcircuit to execute
-        - service (QiskitRuntimeService): the runtime service
-        - backend_name (str): the backends used to execute the subcircuit
-        - options (Options): options for the runtime execution of subcircuit
+        subcircuit: The subcircuit to execute
+        service: The runtime service
+        backend_name: The backends used to execute the subcircuit
+        options: Options for the runtime execution of subcircuit
 
     Returns:
-        - (dict): the measurement probabilities for the subcircuit batch, as calculated from the
-            runtime execution
+        The measurement probabilities for the subcircuit batch, as calculated from the
+        runtime execution
     """
     subcircuit_instance_probs = {}
     circuits_to_run = []
 
     # For each circuit associated with a given subcircuit
     for init_meas in subcircuit_instance:
         subcircuit_instance_idx = subcircuit_instance[init_meas]
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_post_processing.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/wire_cutting_post_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,18 +28,18 @@
     """
     Get O-rho cut qubit pairs.
 
     Iterates through the path for each of the qubits and keeps track of the
     each pair of neigbors.
 
     Args:
-        - complete_path_map (dict): the dictionary containing all path information
+        complete_path_map: The dictionary containing all path information
 
     Returns:
-        - (list): all pairs for each of the qubit paths
+        All pairs for each of the qubit paths
     """
     O_rho_pairs = []
     for input_qubit in complete_path_map:
         path = complete_path_map[input_qubit]
         if len(path) > 1:
             for path_ctr, item in enumerate(path[:-1]):
                 O_qubit_tuple = item
@@ -50,19 +50,19 @@
 
 
 def get_label(label_idx: int, num_cuts: int) -> Sequence[str]:
     """
     Get the basis label for each cut point.
 
     Args:
-        - label_idx (int): the label to be applied for the current basis
-        - num_cuts (int): the number of cuts
+        label_idx: The label to be applied for the current basis
+        num_cuts: The number of cuts
 
     Returns:
-        - (list): the list of the labels
+        The list of the labels
     """
     assert label_idx < 4**num_cuts
     basis = ["I", "X", "Y", "Z"]
     label = []
     for position in range(num_cuts):
         digit = label_idx % 4
         label.append(basis[digit])
@@ -78,22 +78,22 @@
     """
     Get the label attributed to each subcircuit.
 
     subcircuit_label[subcircuit_idx]['init'] = str of init for the cut qubits.
     subcircuit_label[subcircuit_idx]['meas'] = str of meas for the cut qubits.
 
     Args:
-        - label (list): the labels of bases for each cut point, as generated by the
+        label: The labels of bases for each cut point, as generated by the
             get_label function
-        - O_rho_paris (list): the pairs of cut qubits, as generated by the get_cut_qubit_pairs
+        O_rho_paris: The pairs of cut qubits, as generated by the get_cut_qubit_pairs
             function
-        - num_subcircuits (int): the number of subcircuits
+        num_subcircuits: The number of subcircuits
 
     Returns:
-        - (dict): the dictionary containing the labels applied to each of the subcircuits
+        The dictionary containing the labels applied to each of the subcircuits
     """
     subcircuit_label = {
         subcircuit_idx: {"init": "", "meas": ""}
         for subcircuit_idx in range(num_subcircuits)
     }
     for c, pair in zip(label, O_rho_pairs):
         if len(pair) != 2:
@@ -113,22 +113,21 @@
     subcircuit_label: dict[str, str],
     O_rho_pairs: list[tuple[dict[str, Any], dict[str, Any]]],
 ) -> tuple[list[str], list[str]]:
     """
     Given a subcircuit, its label and O-rho cut qubit pairs fill the full init, meas strings.
 
     Args:
-        - subcircuit_idx (int): the subcircuit index
-        - subcircuit (QuantumCircuit): the subcircuit
-        - subcircuit_label (dict): the dictionary containing the applied labels for the bases
-        - O_rho_pairs (list): the list of cut pair qubits
+        subcircuit_idx: The subcircuit index
+        subcircuit: The subcircuit
+        subcircuit_label: The dictionary containing the applied labels for the bases
+        O_rho_pairs: The list of cut pair qubits
 
     Returns:
-        - (list): the initial input bases
-        - (list): the measurements required
+        A tuple containing the initial input bases and the measurements required
     """
     subcircuit_init_label_counter = 0
     subcircuit_meas_label_counter = 0
     init = ["zero" for q in range(subcircuit.num_qubits)]
     meas = ["comp" for q in range(subcircuit.num_qubits)]
     for pair in O_rho_pairs:
         if len(pair) != 2:
@@ -149,19 +148,19 @@
 def get_init_meas(
     init_label: Sequence[str], meas_label: Sequence[str]
 ) -> list[tuple[tuple[str, ...], tuple[str, ...]]]:
     """
     Generate the initial measurements.
 
     Args:
-        - init_label (list): the list of initial bases
-        - meas (list): the list of measurement bases
+        init_label: The list of initial bases
+        meas: The list of measurement bases
 
     Returns:
-        - (list): all subcircuit initial measurements required
+        All subcircuit initial measurements required
     """
     init_combinations = []
     for x in init_label:
         if x == "zero":
             init_combinations.append(["zero"])
         elif x == "I":
             init_combinations.append(["+zero", "+one"])
@@ -188,19 +187,19 @@
 
 
 def convert_to_physical_init(init: list[str]) -> tuple[int, tuple[str, ...]]:
     """
     Convert the initial measurements to the physical representations.
 
     Args:
-        - init (list): the initial measurements, e.g. ["zero", "2plus"]
+        init: The initial measurements, e.g. ["zero", "2plus"]
 
     Returns:
-        - (int): the coefficient of the physical measurements
-        - (tuple): the physical measurement bases
+        A tuple containing the coefficient of the physical measurements
+        and the physical measurement bases
     """
     coefficient = 1
     for idx, x in enumerate(init):
         if x == "zero":
             continue
         elif x == "+zero":
             init[idx] = "zero"
@@ -245,25 +244,21 @@
     | subcircuit_entries[subcircuit_idx][init_label,meas_label] = subcircuit_entry_idx, kronecker_term.
     | kronecker_term (list): (coefficient, subcircuit_instance_idx).
     | Add coefficient*subcircuit_instance to subcircuit_entry.
 
     subcircuit_instances[subcircuit_idx][init,meas] = subcircuit_instance_idx.
 
     Args:
-        - subcircuits (list): the list of subcircuits
-        - complete_path_map (dict): the paths of all the qubits through the circuit DAGs
-        - num_cuts (int): the number of cuts
+        subcircuits: The list of subcircuits
+        complete_path_map: The paths of all the qubits through the circuit DAGs
+        num_cuts: The number of cuts
 
     Returns:
-        a tuple
-        containing:
-
-        - (dict): dictionary containing information on the summation terms
-        - (dict): dictionary containing the subcircuits entry information
-        - (dict): dictionary containing subcircuit instances
+        A tuple containing a summation term dict, a subcircuit entry dict,
+        and a subcircuit instances dict
     """
     summation_terms = []
     subcircuit_entries: dict[
         int, dict[tuple[str, str], tuple[int, Sequence[tuple[int, int]]]]
     ] = {subcircuit_idx: {} for subcircuit_idx in range(len(subcircuits))}
     subcircuit_instances: dict[
         int, dict[tuple[tuple[str, ...], tuple[Any, ...]], int]
@@ -346,23 +341,23 @@
     """
     Reconstruct the full probability distribution from the subcircuits.
 
     This function is called within the build function, meant to be used
     in a multipooling manner.
 
     Args:
-        - subcircuit_order (list): the order of the subcircuit inputs
-        - summation_terms (list): the summation terms, as generated
+        subcircuit_order: The order of the subcircuit inputs
+        summation_terms: The summation terms, as generated
             from generate_summation_terms
-        - subcircuit_entry_probs (dict): the input probabilities from each of
+        subcircuit_entry_probs: The input probabilities from each of
             the subcircuit executions
 
     Returns:
-        - (np.ndarray): the reconstructed probability distribution
-        - (dict): the approximate computational overhead of the function
+        A tuple containing the reconstructed probability distribution
+        and the approximate computational overhead of the function
     """
     reconstructed_prob = None
     overhead = {"additions": 0, "multiplications": 0}
     for summation_term in summation_terms:
         summation_term_prob = None
         for subcircuit_idx in subcircuit_order:
             subcircuit_entry_idx = summation_term[subcircuit_idx]
@@ -390,29 +385,25 @@
     num_cuts: int,
     num_threads: int,
 ) -> tuple[np.ndarray, list[int], dict[str, int]]:
     """
     Reconstruct the full probability distribution from the subcircuits.
 
     Args:
-        - summation_terms (list): the summation terms used to generate the full
+        summation_terms: The summation terms used to generate the full
             vector, as generated in generate_summation_terms
-        - subcircuit_entry_probs (dict): the probabilities vectors from the
+        subcircuit_entry_probs: The probabilities vectors from the
             subcircuit executions
-        - num_cuts (int): the number of cuts
-        - num_threads (int): the number of threads to use for multithreading
+        num_cuts: The number of cuts
+        num_threads: The number of threads to use for multithreading
 
     Returns:
-        a tuple
-        containing:
-
-        - (np.ndarray): the reconstructed probability distribution of the full
-          circuit
-        - (list): the ordering of the distribution
-        - (dict): the computational post-processing overhead
+        A tuple containing the reconstructed probability distribution of the full
+        circuit, the ordering of the distribution, and the computational
+        post-processing overhead
     """
     smart_order = sorted(
         list(subcircuit_entry_probs.keys()),
         key=lambda subcircuit_idx: len(subcircuit_entry_probs[subcircuit_idx][0]),
     )
     args = []
     for i in range(num_threads * 5):
@@ -447,21 +438,20 @@
 def _find_process_jobs(
     jobs: Sequence[dict[int, int]], rank: int, num_workers: int
 ) -> Sequence[dict[int, int]]:
     """
     Split up the total jobs into subjobs to be multithreaded.
 
     Args:
-        - jobs (list): all summation terms to be used
-        - rank (int): the input thread
-        - num_workers (int): 5 * the number of threads
-
-    Returngs:
-        - (list): the sublist of jobs to be executed on the
-            given thread
+        jobs: All summation terms to be used
+        rank: The input thread
+        num_workers: 5 * the number of threads
+
+    Returns:
+        The sublist of jobs to be executed on the given thread
     """
     count = int(len(jobs) / num_workers)
     remainder = len(jobs) % num_workers
     if rank < remainder:
         jobs_start = rank * (count + 1)
         jobs_stop = jobs_start + count + 1
     else:
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting/wire_cutting_verification.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/cutqc/wire_cutting_verification.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,25 +41,20 @@
     Compare the reconstructed probabilities to the ground truth.
 
     Executes the original circuit, then measures the distributional differences between this exact
     result (ground truth) and the reconstructed result from the subcircuits.
     Provides a variety of metrics to evaluate the differences in the distributions.
 
     Args:
-        - full_circuit (QuantumCircuit): the original quantum circuit that was cut
-        - reconstructed_output (np.ndarray): the reconstructed probability distribution from the
+        full_circuit: The original quantum circuit that was cut
+        reconstructed_output: The reconstructed probability distribution from the
             execution of the subcircuits
 
     Returns:
-        a tuple
-        containing:
-
-        - a dictionary containing a variety of distributional difference
-          metrics for the ground truth and reconstructed distributions; and,
-        - the true probability distribution of the full circuit
+        A tuple containing metrics for the ground truth and reconstructed distributions
     """
     ground_truth = _evaluate_circuit(circuit=full_circuit)
     metrics = {}
     for quasi_conversion_mode in ["nearest", "naive"]:
         real_probability = quasi_to_real(
             quasiprobability=reconstructed_output, mode=quasi_conversion_mode
         )
@@ -86,24 +81,24 @@
     smart_order: Sequence[int],
     complete_path_map: dict[Qubit, Sequence[dict[str, int | Qubit]]],
 ) -> np.ndarray:
     """
     Reorder the probability distribution.
 
     Args:
-        - full_circuit (QuantumCircuit): the original uncut circuit
-        - subcircuits (list): the cut subcircuits
-        - unordered (np.ndarray): the unordered results of the subcircuits
-        - smart_order (list): the correct ordering of the subcircuits
-        - complete_path_map (dict): the path map of the cuts, as defined from the
+        full_circuit: The original uncut circuit
+        subcircuits: The cut subcircuits
+        unordered: The unordered results of the subcircuits
+        smart_order: The correct ordering of the subcircuits
+        complete_path_map: The path map of the cuts, as defined from the
             cutting function
 
     Returns:
-        - (np.ndarray): the reordered and reconstructed probability distribution over the
-            full circuit
+        The reordered and reconstructed probability distribution over the
+        full circuit
     """
     subcircuit_out_qubits: dict[int, list[Qubit]] = {
         subcircuit_idx: [] for subcircuit_idx in smart_order
     }
     for input_qubit in complete_path_map:
         path = complete_path_map[input_qubit]
         output_qubit = path[-1]
@@ -140,18 +135,18 @@
 
 
 def _evaluate_circuit(circuit: QuantumCircuit) -> Sequence[float]:
     """
     Compute exact probability vector of given circuit.
 
     Args:
-        - circuit (QuantumCircuit): the circuit to simulate
+        circuit: The circuit to simulate
 
     Returns:
-        - (Sequence[float]): the final probability vector of the circuit
+        The final probability vector of the circuit
     """
     max_memory_mb = psutil.virtual_memory().total >> 20
     max_memory_mb = int(max_memory_mb / 4 * 3)
     simulator = Aer.get_backend(
         "aer_simulator_statevector", max_memory_mb=max_memory_mb
     )
     circuit = copy.deepcopy(circuit)
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/__init__.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/__init__.py`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/cholesky_decomposition.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/cholesky_decomposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 from __future__ import annotations
 
 import copy
 from typing import Sequence
 
 import numpy as np
-from qiskit.opflow import ListOp, PauliSumOp
+
+from qiskit.opflow import PauliSumOp
 from qiskit.quantum_info import Pauli
 from qiskit_nature.second_q.problems import ElectronicStructureProblem
 from qiskit_nature.second_q.mappers import QubitConverter, JordanWignerMapper
 from qiskit_nature.second_q.operators import (
     FermionicOp,
     PolynomialTensor,
 )
@@ -37,55 +38,51 @@
 def get_cholesky_op(
     l_op: np.ndarray, g: int, converter: QubitConverter, opname: str
 ) -> PauliSumOp:
     """
     Convert a two-body term into a cholesky operator.
 
     Args:
-        - l_op: Two body integrals
-        - g: integral index
-        - converter: Qubit converter to be used
-        - opname: Prefix for output cholesky operator name
+        l_op: Two body integrals
+        g: Integral index
+        converter: Qubit converter to be used
+        opname: Prefix for output cholesky operator name
 
     Returns:
-        - cholesky_operator: The converted operator
+        The converted Cholesky operator
     """
     pt = PolynomialTensor({"+-": l_op[:, :, g]})
     fer_op = FermionicOp.from_polynomial_tensor(pt)
     cholesky_op = converter.convert(fer_op)
     cholesky_op._name = opname + "_chol" + str(g)
 
     return cholesky_op
 
 
 def cholesky_decomposition(
     problem: ElectronicStructureProblem,
     mo_coeff: np.ndarray | None = None,
     orbitals_to_reduce: Sequence[int] | None = None,
-) -> tuple[ListOp, float]:
+) -> tuple[list[PauliSumOp], float]:
     """
     Construct the decomposed Hamiltonian from an input ``ElectronicStructureProblem``.
 
     Args:
-        - problem (ElectronicStructureProblem): An ``ElectronicStructureProblem`` from which the decomposed Hamiltonian will be
-            calculated.
-        - mo_coeff (np.ndarray | None): The coefficients for mapping to the MO basis. If ``None``, the input integrals will be
-            assumed to be in the MO basis.
-        - orbitals_to_reduce (Sequence[int] | None): A list of orbital indices to remove from the problem before decomposition.
+        problem: An ``ElectronicStructureProblem`` from which the decomposed Hamiltonian
+            will be calculated
+        mo_coeff: The coefficients for mapping to the MO basis. If ``None``, the input
+            integrals will be assumed to be in the MO basis
+        orbitals_to_reduce: A list of orbital indices to remove from the problem
+            before decomposition
 
     Returns:
-        - Tuple containing
-            - cholesky_operator (ListOp): A list of operators representing the decomposed Hamiltonian.
-              shape: [single-body hamiltonian, cholesky_0, ..., cholesky_N]
-            - freeze_shift (float): An energy shift resulting from the decomposition. This shift should be re-applied after
-              calculating properties of the decomposed operator (i.e. ground state energy).
+        Tuple containing the cholesky operator and the energy shift resulting from decomposition
 
     Raises:
-        - ValueError:
-            The input ElectronicStructureProblem contains no particle number information.
+        ValueError: The input ElectronicStructureProblem contains no particle number information.
     """
     hcore = np.array(problem.hamiltonian.electronic_integrals.one_body.alpha["+-"])
     eri = to_chemist_ordering(
         problem.hamiltonian.electronic_integrals.two_body.alpha["++--"]
     )
     num_alpha = problem.num_alpha
     if num_alpha is None:
@@ -117,37 +114,36 @@
         opname="H",
         halve_transformed_h2=True,
         occupied_orbitals_to_reduce=orbitals_to_reduce_dict["occupied"],
         virtual_orbitals_to_reduce=orbitals_to_reduce_dict["virtual"],
     )
 
     op_list = [h_1_op] + h_chol_ops
-    operator = ListOp(op_list)
+    operator = op_list
 
     return operator, nuclear_repulsion_energy + freeze_shift
 
 
 def convert_cholesky_operator(
-    operator: ListOp,
+    operator: list[PauliSumOp],
     ansatz: EntanglementForgingAnsatz,
 ) -> EntanglementForgingOperator:
     """
-    Convert the Cholesky operator (ListOp) into the entanglement forging format.
+    Convert the Cholesky operator (List[PauliSumOp]) into the entanglement forging format.
 
     Args:
-        - operator: A `ListOp` containing the single-body Hamiltonian followed
-            by the Cholesky operators.
+        operator: A `List[PauliSumOp]` containing the single-body Hamiltonian followed
+            by the Cholesky operators
             shape: [single-body hamiltonian, cholesky_0, ..., cholesky_N]
-        - ansatz:
-            The ansatz for which to compute expectation values of operator. The
-            `EntanglementForgingAnsatz` also contains the bitstrings for each subsystem..
+        ansatz: The ansatz for which to compute expectation values of operator. The
+            `EntanglementForgingAnsatz` also contains the bitstrings for each subsystem
 
     Returns:
-        - forged_operator: An `EntanglementForgingOperator` object describing the
-            decomposed operator.
+        An `EntanglementForgingOperator` object describing the
+        decomposed operator
     """
     calculate_hybrid_cross_terms = len(set(ansatz.bitstrings_u)) < len(
         ansatz.bitstrings_u
     ) or len(set(ansatz.bitstrings_v)) < len(ansatz.bitstrings_v)
 
     op1 = operator[0]
     cholesky_ops = operator[1:]
@@ -247,33 +243,28 @@
     virtual_orbitals_to_reduce: np.ndarray | None = None,
     epsilon_cholesky: float = 1e-10,
 ) -> tuple[PauliSumOp, list[PauliSumOp], float, np.ndarray, np.ndarray,]:
     r"""
     Decompose the Hamiltonian operators into a form appropriate for entanglement forging.
 
     Args:
-        - mo_coeff (np.ndarray): 2D array representing coefficients for converting from AO to MO basis.
-        - h1 (np.ndarray): 2D array representing operator
-            coefficients of one-body integrals in the AO basis.
-        - h2 (np.ndarray): 4D array representing operator coefficients
-            of two-body integrals in the AO basis.
-        - halve_transformed_h2 (bool | None): Should be set to True for Hamiltonian
-            operator to agree with Qiskit conventions.
-        - occupied_orbitals_to_reduce (np.ndarray | None): A list of occupied orbitals that will be removed.
-        - virtual_orbitals_to_reduce (np.ndarray | None): A list of virtual orbitals that will be removed.
-        - epsilon_cholesky (float | None): The threshold for the decomposition (typically a number close to 0).
+        mo_coeff: 2D array representing coefficients for converting from AO to MO basis
+        h1: 2D array representing operator
+            coefficients of one-body integrals in the AO basis
+        h2: 4D array representing operator coefficients
+            of two-body integrals in the AO basis
+        halve_transformed_h2: Should be set to True for Hamiltonian
+            operator to agree with Qiskit conventions
+        occupied_orbitals_to_reduce: A list of occupied orbitals that will be removed
+        virtual_orbitals_to_reduce: A list of virtual orbitals that will be removed
+        epsilon_cholesky: The threshold for the decomposition (typically a number close to 0)
 
     Returns:
-        - qubit_op (PauliSumOp): H_1 in the Cholesky decomposition.
-        - cholesky_ops (list[PauliSumOp]): L_\\gamma in the Cholesky decomposition
-        - freeze_shift (float): Energy shift due to freezing.
-        - h1 (np.ndarray): 2D array representing operator coefficients of one-body
-            integrals in the MO basis.
-        - h2 (np.ndarray): 4D array representing operator coefficients of
-            two-body integrals in the MO basis.
+        A tuple containing the single and two-body integrals, the energy shift, and the
+        one and two body integrals in the MO basis
     """
     if virtual_orbitals_to_reduce is None:
         virtual_orbitals_to_reduce = np.array([])
     if occupied_orbitals_to_reduce is None:
         occupied_orbitals_to_reduce = np.array([])
 
     coeff_mo = copy.copy(mo_coeff)
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ansatz.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ansatz.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,58 +26,44 @@
     optimized using a VQE. The computational basis states of each subsystem that
     contribute to the Schmidt decomposition can be specified by a list of
     bitstrings. This list can be chosen differently for each subsystem.
 
     For a 2N-qubit operator, the circuit should act on N qubits and the bitstrings
     should be of length N. This class functions as a container for information about
     the circuit and bitstrings, and is required for the EntanglementForgingGroundStateSolver.
-
-    Attributes:
-        - circuit_u (QuantumCircuit): the parameterized circuit that is optimized to
-            find the minimum energy of the original problem. It represents the
-            unitary U for both N-qubit subsystems in the Schmidt decomposition.
-        - bitstrings_u (list[tuple[Int]]): the input bitstrings for each N-qubit
-            subsystem. The bitstrings represent the computational basis states
-            contributing to the Schmidt decomposition. List must contain less than
-            or equal to 2^N elements and each bitstring must have length N. These
-            bitstrings are used for each subsystem unless bitstrings_v is provided.
-        - bitstrings_v (list[tuple[Int]], optional): specifies the bitstrings to be
-            used for the second subsystem in the Schmidt decomposition. Must be the
-            same shape as bitstrings_u. If not provided, then bitstrings_u is used
-            for both subsystems.
     """
 
     def __init__(
         self,
         circuit_u: QuantumCircuit,
         bitstrings_u: list[tuple[int, ...]],
         bitstrings_v: list[tuple[int, ...]] | None = None,
     ):
         """
         Assign the necessary member variables and check for shaping errors.
 
         Args:
-            - circuit_u (QuantumCircuit): the parameterized circuit that is optimized to
+            circuit_u: the parameterized circuit that is optimized to
                 find the minimum energy of the original problem. It represents the
                 unitary U for both N-qubit subsystems in the Schmidt decomposition.
-            - bitstrings_u (list[tuple[Int]]): the input bitstrings for each N-qubit
+            bitstrings_u: the input bitstrings for each N-qubit
                 subsystem. The bitstrings represent the computational basis states
                 contributing to the Schmidt decomposition. List must contain less than
                 or equal to 2^N elements and each bitstring must have length N. These
                 bitstrings are used for each subsystem unless bitstrings_v is provided.
-            - bitstrings_v (list[tuple[Int]], optional): specifies the bitstrings to be
+            bitstrings_v: specifies the bitstrings to be
                 used for the second subsystem in the Schmidt decomposition. Must be the
                 same shape as bitstrings_u. If not provided, then bitstrings_u is used
                 for both subsystems.
 
         Returns:
-            - None
+            None
 
         Raises:
-            - ValueError: If the input bitstrings are of incorrect shapes (as defined above).
+            ValueError: The input bitstrings are of incorrect shapes.
         """
         if any(len(bitstring) != circuit_u.num_qubits for bitstring in bitstrings_u):
             raise ValueError(
                 "Length of every U bitstring must be the same as the number of qubits in the ansatz."
             )
 
         if bitstrings_v and bitstrings_v != bitstrings_u:
@@ -95,69 +81,39 @@
 
         self._circuit_u: QuantumCircuit = circuit_u
         self._bitstrings_u: list[tuple[int, ...]] = bitstrings_u
         self._bitstrings_v: list[tuple[int, ...]] = bitstrings_v or bitstrings_u
 
     @property
     def circuit_u(self) -> QuantumCircuit:
-        """
-        Property function for the circuit.
-
-        Returns:
-            - (QuantumCircuit): the _circuit_u member variable
-        """
+        """Property function for the circuit."""
         return self._circuit_u
 
     @property
     def bitstrings_u(self) -> list[tuple[int, ...]]:
-        """
-        Property function for the first bitstrings.
-
-        Returns:
-            - (list[tuple[int, ...]]): the _bitstrings_u member variable
-        """
+        """Property function for the first bitstrings."""
         return self._bitstrings_u
 
     @property
     def bitstrings_v(self) -> list[tuple[int, ...]]:
-        """
-        Property function for the second bitstrings.
-
-        Returns:
-            - (list[tuple[int, ...]]): the _bitstrings_v member variable
-        """
+        """Property function for the second bitstrings."""
         return self._bitstrings_v
 
     @property
     def bitstrings_are_symmetric(self) -> bool:
-        """
-        Property function for the symmetry of bitstrings.
-
-        Returns:
-            - (bool): whether the first and second set of bitstrings are the same
-        """
+        """Property function for the symmetry of bitstrings."""
         return self._bitstrings_v == self._bitstrings_u
 
     @property
     def subspace_dimension(self) -> int:
-        """
-        Property function for the length of bitstrings.
-
-        Returns:
-            - (int): the number of bitstrings
-        """
+        """Property function for the length of bitstrings."""
         return len(self._bitstrings_u)
 
     def __repr__(self) -> str:
-        """
-        Representation function for EntanglementForgingAnsatz.
-
-        Returns:
-            - (str): printable repesentation of class
-        """
+        """Representation function for EntanglementForgingAnsatz."""
         repr = "EntanglementForgingAnsatz\nCircuit:\n"
         repr += str(self._circuit_u.draw())
         repr += "\nBitstrings U:\n"
         repr += str(self.bitstrings_u)
         repr += "\nBitstrings V:\n"
         repr += str(self._bitstrings_v)
         repr += f"\nBitstring are symmetric: {self.bitstrings_are_symmetric}\n"
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ground_state_solver.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_ground_state_solver.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 )
 
 import scipy
 import numpy as np
 
 from qiskit.algorithms.minimum_eigensolvers import MinimumEigensolverResult
 from qiskit.algorithms.optimizers import SPSA, Optimizer, OptimizerResult
-from qiskit.opflow import ListOp
 from qiskit_nature.second_q.problems import (
     ElectronicStructureProblem,
     EigenstateResult,
     ElectronicBasis,
 )
 from qiskit_ibm_runtime import QiskitRuntimeService, Options
+from qiskit.opflow import PauliSumOp
 
 from .entanglement_forging_ansatz import EntanglementForgingAnsatz
 from .entanglement_forging_knitter import EntanglementForgingKnitter
 from .entanglement_forging_operator import EntanglementForgingOperator
 from .cholesky_decomposition import cholesky_decomposition, convert_cholesky_operator
 
 
@@ -131,26 +131,26 @@
         options: Options | list[Options] | None = None,
         mo_coeff: np.ndarray | None = None,
     ):
         """
         Assign the necessary class variables and initialize any defaults.
 
         Args:
-            - ansatz: Class which holds the ansatz circuit and bitstrings
-            - service: The service used to spawn Qiskit primitives
-            - optimizer: Optimizer to use to optimize the ansatz circuit parameters
-            - initial_point: Initial values for ansatz parameters
-            - orbitals_to_reduce: List of orbital indices to remove from the problem before
+            ansatz: Class which holds the ansatz circuit and bitstrings
+            service: The service used to spawn Qiskit primitives
+            optimizer: Optimizer to use to optimize the ansatz circuit parameters
+            initial_point: Initial values for ansatz parameters
+            orbitals_to_reduce: List of orbital indices to remove from the problem before
                 decomposition.
-            - backend_names: Backend name or list of backend names to use during parallel computation
-            - options: Options or list of options to be applied to the backends
-            - mo_coeff: Coefficients for converting an input problem to MO basis
+            backend_names: Backend name or list of backend names to use during parallel computation
+            options: Options or list of options to be applied to the backends
+            mo_coeff: Coefficients for converting an input problem to MO basis
 
         Returns:
-            - None
+            None
         """
         # Set class fields
         self._knitter: EntanglementForgingKnitter | None = None
         self._history: EntanglementForgingHistory = EntanglementForgingHistory()
         self._energy_shift = 0.0
         self._ansatz: EntanglementForgingAnsatz | None = ansatz
         self._service: QiskitRuntimeService | None = service
@@ -247,36 +247,36 @@
         """Set the coefficients for converting integrals to the MO basis."""
         self._mo_coeff = mo_coeff
 
     def solve(
         self,
         problem: ElectronicStructureProblem,
     ) -> EntanglementForgingResult:
-        """Compute Ground State properties.
+        """Compute ground state properties.
 
         Args:
-            - problem: a class encoding a problem to be solved
+            problem: A class encoding a problem to be solved
 
         Returns:
-            - A result object
+            A result object
 
         Raises:
-            - ValueError:
-                The ``backend_names`` and ``options`` lists are of incompatible lengths
-            - AttributeError:
-                Ansatz must be set before calling `solve` method
+            ValueError: The ``backend_names`` and ``options`` lists are of
+                incompatible lengths
+            AttributeError: Ansatz must be set before calling `solve` method
         """
         if self._backend_names and self._options:
             if len(self._backend_names) != len(self._options):
                 if len(self._options) == 1:
                     self._options = [self._options[0]] * len(self._backend_names)
                 else:
                     raise AttributeError(
-                        f"The list of backend names is length ({len(self._backend_names)}), but the list of options is "
-                        f"length ({len(self._options)}). It is ambiguous how to combine the options with the backends."
+                        f"The list of backend names is length ({len(self._backend_names)}), "
+                        f"but the list of options is length ({len(self._options)}). It is "
+                        "ambiguous how to combine the options with the backends."
                     )
         if self._ansatz is None:
             raise AttributeError("Ansatz must be set before calling solve.")
         if self._initial_point is None:
             self._initial_point = np.array(
                 [0.0 for i in range(len(self._ansatz.circuit_u.parameters))]
             )
@@ -331,21 +331,22 @@
         self._knitter.close_sessions()
 
         return result
 
     def get_eigenvalue_evaluation(
         self, operator: EntanglementForgingOperator
     ) -> Callable[[Sequence[float]], float | Iterable[float]]:
-        """Produce a callable function which provides an estimation of the minimum eigenvalue of the input operator.
+        """
+        Produce a callable which provides an estimation of the min eigenvalue of an operator.
 
         Args:
-          - operator (EntanglementForgingOperator): The decomposed Hamiltonian in entanglement forging format
+            operator: The decomposed Hamiltonian in entanglement forging format
         Returns:
-          - callable (Callable):  Callable function which provides an estimation of the mihnimum eigenvalue
-              of the input operator given some ansatz circuit parameters.
+            Callable function which provides an estimation of the mihnimum eigenvalue
+            of the input operator given some ansatz circuit parameters.
         """
 
         def evaluate_eigenvalue(parameters: Sequence[float]) -> float:
             if self._knitter is None:
                 raise RuntimeError("Knitter must be set before evaluating eigenvalue.")
 
             eigenvalue, schmidt_coeffs, _ = self._knitter(
@@ -358,30 +359,27 @@
             return eigenvalue
 
         return evaluate_eigenvalue
 
     def get_qubit_operators(
         self,
         problem: ElectronicStructureProblem,
-    ) -> ListOp:
+    ) -> list[PauliSumOp]:
         """Construct decomposed qubit operators from an ``ElectronicStructureProblem``.
 
         Args:
-          - problem (ElectronicStructureProblem): A class encoding a problem to be solved.
+            problem: A class encoding a problem to be solved
 
         Returns:
-          - hamiltonian_ops: qubit operator representing the decomposed Hamiltonian.
+            hamiltonian_ops: Qubit operator representing the decomposed Hamiltonian
 
         Raises:
-            - ValueError:
-                The input problem is not in MO basis, and ``mo_coeff`` is set to ``None``
-            - ValueError:
-                The ``mo_coeff`` and input problem integrals are of incompatible shapes
-            - ValueError:
-                The input integrals are ``None``
+            ValueError: The input problem is not in MO basis, and ``mo_coeff`` is set to ``None``
+            ValueError: The ``mo_coeff`` and input problem integrals are of incompatible shapes
+            ValueError: The input integrals are ``None``
         """
         self._validate_problem_and_coeffs(problem, self.mo_coeff)
 
         hamiltonian_ops, self._energy_shift = cholesky_decomposition(
             problem, self.mo_coeff, self._orbitals_to_reduce  # type: ignore
         )
         return hamiltonian_ops
@@ -389,25 +387,25 @@
     @staticmethod
     def _validate_problem_and_coeffs(
         problem: ElectronicStructureProblem, mo_coeff: np.ndarray | None
     ):
         """Ensure the input problem can be translated to the MO basis."""
         if (problem.basis != ElectronicBasis.MO) and (mo_coeff is None):
             raise ValueError(
-                f"Cannot transform integrals to MO basis. The input problem is in the ({problem.basis}) basis, "
-                "and the mo_coeff class field is None."
+                "Cannot transform integrals to MO basis. The input problem is "
+                f"in the ({problem.basis}) basis, and the mo_coeff class field is None."
             )
 
         h1 = np.array(problem.hamiltonian.electronic_integrals.one_body.alpha["+-"])
         if h1.shape == ():
             raise ValueError("The input integrals are empty.")
 
         # First two lines of this conditional are already implied by passing above checks, but alas, mypy :)
         if (
             problem.basis != ElectronicBasis.MO
             and mo_coeff is not None
             and mo_coeff.shape != h1.shape
         ):
             raise ValueError(
-                f"The mo_coeff class field has shape ({mo_coeff.shape}), but the input one body integral "
-                f"has shape ({h1.shape})."
+                f"The mo_coeff class field has shape ({mo_coeff.shape}), but "
+                f"the input one body integral has shape ({h1.shape})."
             )
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_knitter.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_knitter.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,22 +46,22 @@
         backend_names: str | list[str] | None = None,
         options: Options | list[Options] | None = None,
     ):
         """
         Assign the necessary member variables.
 
         Args:
-            - ansatz (EntanglementForgingAnsatz): The container for the circuit structure and bitstrings
-                to be used (and generate the stateprep circuits)
-            - service (QiskitRuntimeService): The service used to spawn Qiskit primitives and runtime jobs
-            - backend_names (list[str]): Names of the backends to use for calculating expectation values
-            - options (list[Options]): Options to use with the backends
+            ansatz: The container for the circuit structure and bitstrings to be used
+                (and generate the stateprep circuits)
+            service: The service used to spawn Qiskit primitives and runtime jobs
+            backend_names: Names of the backends to use for calculating expectation values
+            options: Options to use with the backends
 
         Returns:
-            - None
+            None
         """
         # Call backend_names setter to update the session_ids hidden class field
         self._session_ids: list[str | None] | None = None
         self._backend_names: list[str] | None = None
         self._options: list[Options] | None = None
         # Call constructors
         self.backend_names = backend_names  # type: ignore
@@ -100,97 +100,53 @@
                 self._superposition_circuits_v,
             ) = _construct_stateprep_circuits(
                 self._ansatz.bitstrings_v  # type: ignore
             )
 
     @property
     def ansatz(self) -> EntanglementForgingAnsatz:
-        """
-        Property function for the ansatz.
-
-        Returns:
-            - (EntanglementForgingAnsatz): the ansatz member variable
-        """
+        """Property function for the ansatz."""
         return self._ansatz
 
     @property
     def backend_names(self) -> list[str] | None:
-        """
-        List of backend names to be used.
-
-        Returns:
-            - (list[str]): the backend_names member variable
-        """
+        """List of backend names to be used."""
         return self._backend_names
 
     @backend_names.setter
     def backend_names(self, backend_names: str | list[str] | None) -> None:
-        """
-        Change the backend_names class field.
-
-        Args:
-            - backend_names (list[str]): the list of backends to use
-
-        Returns:
-            - None
-        """
+        """Change the backend_names class field."""
         if isinstance(backend_names, str):
             self._backend_names = [backend_names]
         else:
             self._backend_names = backend_names
         if backend_names:
             self._session_ids = [None] * len(backend_names)
 
     @property
     def options(self) -> list[Options] | None:
-        """
-        List of options to be used.
-
-        Returns:
-            - (list[Options]): the options member variable
-        """
+        """List of options to be used."""
         return self._options
 
     @options.setter
     def options(self, options: Options | list[Options] | None) -> None:
-        """
-        Change the options class field.
-
-        Args:
-            - options (list[Options]): the list of options to use
-
-        Returns:
-            - None
-        """
+        """Change the options class field."""
         if isinstance(options, Options):
             self._options = [options]
         else:
             self._options = options
 
     @property
     def service(self) -> QiskitRuntimeService | None:
-        """
-        Property function for service class field.
-
-        Returns:
-            - (QiskitRuntimeService): the service member variable
-        """
+        """Property function for service class field."""
         return QiskitRuntimeService(**self._service)
 
     @service.setter
     def service(self, service: QiskitRuntimeService | None) -> None:
-        """
-        Change the service class field.
-
-        Args:
-            - service (QiskitRuntimeService): the service used to spawn Qiskit primitives
-
-        Returns:
-            - None
-        """
+        """Change the service class field."""
         self._service = service.active_account() if service is not None else service
 
     def __call__(
         self,
         ansatz_parameters: Sequence[float],
         forged_operator: EntanglementForgingOperator,
     ) -> tuple[float, np.ndarray, np.ndarray]:
@@ -208,32 +164,31 @@
         Energy = $ \sum_{n=1}^{2^N} \left ( h_{n, n} + \sum_{m=1}^{n-1} h_{n, m} \right ) $
 
         For now, we are only using $p \in \{0, 2 \} $ as opposed to $ p \in \{ 0, 1, 2, 3 \} $.
 
         Additionally, U = V is currently required, but may change in future versions.
 
         Args:
-            - self
-            - ansatz_parameters (Sequence[float]): the parameters to be used by the ansatz circuit,
+            ansatz_parameters: the parameters to be used by the ansatz circuit,
                 must be the same length as the circuit's parameters
-            - forged_operator (EntanglementForgingOperator): the operator to forge the expectation
-                value from
+            forged_operator: the operator from which to forge the expectation value
 
         Returns:
-            - (tuple[float, np.ndarray, np.ndarray]): a tuple
-                containing the energy (i.e. forged expectation value), the Schmidt coefficients,
-                and the full Schmidt decomposition matrix
+            A tuple containing the energy (i.e. forged expectation value), the Schmidt
+            coefficients, and the full Schmidt decomposition matrix
         """
         if self._backend_names and self._options:
             if len(self._backend_names) != len(self._options):
                 if len(self._options) == 1:
                     self._options = [self._options[0]] * len(self._backend_names)
                 else:
                     raise AttributeError(
-                        f"The list of backend names is length ({len(self._backend_names)}), but the list of options is length ({len(self._options)}). It is ambiguous how to combine the options with the backends."
+                        f"The list of backend names is length ({len(self._backend_names)}), "
+                        f"but the list of options is length ({len(self._options)}). It is "
+                        "ambiguous how to combine the options with the backends."
                     )
         # For now, we only assign the parameters to a copy of the ansatz
         circuit_u = self._ansatz.circuit_u.bind_parameters(ansatz_parameters)
 
         # Create the tensor and superposition stateprep circuits
         # tensor_ansatze   = [U|bi⟩      for |bi⟩       in  tensor_circuits]
         # superposition_ansatze = [U|𝜙^𝑝_𝑏𝑛𝑏𝑚⟩ for |𝜙^𝑝_𝑏𝑛𝑏𝑚⟩ in superposition_circuits]
@@ -322,15 +277,16 @@
             ) = partitioned_expval_future.result()
             tensor_expvals.extend(partition_tensor_expvals)
             superposition_expvals.extend(partition_superposition_expvals)
             # Start a session for each thread if this is the first run
             if job_id and (session_ids[i] is None):
                 if self._session_ids is None:
                     raise ValueError(
-                        "Something unexpected happened. The session_ids field must be set when a job_id is present."
+                        "Something unexpected happened. The session_ids field must "
+                        "be set when a job_id is present."
                     )
                 self._session_ids[i] = job_id
 
         # Compute the Schmidt matrix
         h_schmidt = self._compute_h_schmidt(
             forged_operator, np.array(tensor_expvals), np.array(superposition_expvals)
         )
@@ -346,23 +302,23 @@
         tensor_expvals: np.ndarray,
         superpos_expvals: np.ndarray,
     ) -> np.ndarray:
         """
         Compute the Schmidt decomposition of the Hamiltonian.
 
         Args:
-            - forged_operator (EntanglementForgingOperator): the operator that the
-                forged expectation values are computed with
-            - tensor_expvals (np.ndarray): the expectation values
-                for the tensor circuits (i.e. same Schmidt coefficients)
-            - superpos_expvals (np.ndarray): the expectation values
-                for the superposition circuits (i.e. different Schmidt coefficients)
+            forged_operator: The operator with which the forged expectation values are
+                computed
+            tensor_expvals: The expectation values for the tensor circuits
+                (i.e. same Schmidt coefficients)
+            superpos_expvals: The expectation values for the superposition circuits
+                (i.e. different Schmidt coefficients)
 
         Returns:
-           - (np.ndarray): the Schmidt matrix
+           The Schmidt matrix
         """
         # Calculate the diagonal entries of the Schmidt matrix by
         # summing the expectation values associated with the tensor terms
         # h𝑛𝑛 = Σ_ab 𝑤𝑎𝑏•[ 𝜆𝑛^2•⟨b𝑛|U^t•P𝑎•U|b𝑛⟩⟨b𝑛|V^t•P𝑏•V|b𝑛⟩ ]
         if self._ansatz.bitstrings_are_symmetric:
             h_schmidt_diagonal = np.einsum(
                 "ij, xi, xj->x",
@@ -423,30 +379,23 @@
         #                                   ⟨𝜙^𝑝_𝑏𝑛𝑏𝑚|V^t•𝑃𝑏•V|𝜙^𝑝_𝑏𝑛𝑏𝑚⟩ ]
         for element, indices in zip(h_schmidt_off_diagonals, superpos_indices):
             h_schmidt[indices] = element
 
         return h_schmidt
 
     def close_sessions(self) -> None:
-        """
-        Close all the sessions opened by this object.
-
-        Args:
-            - None
-
-        Returns:
-            - None
-        """
+        """Close all the sessions opened by this object."""
         if self._session_ids is None:
             return
         else:
             for i, session_id in enumerate(self._session_ids):
                 if self._backend_names is None:
                     raise ValueError(
-                        f"There was a problem closing session id ({session_id}). No backend to associate with session."
+                        f"There was a problem closing session id ({session_id}). "
+                        "No backend to associate with session."
                     )
                 session = Session(service=self.service, backend=self._backend_names[i])
                 session._session_id = session_id
                 session.close()
 
         return
 
@@ -504,21 +453,20 @@
          ┌───┐┌───┐
     q_0: ┤ H ├┤ Z ├──■──
          ├───┤└───┘┌─┴─┐
     q_1: ┤ X ├─────┤ X ├
          └───┘     └───┘
 
     Args:
-        - bitstrings (list[tuple[int, ...]]): the input list of bitstrings used to generate the state preparation circuits
-        - subsystem_id (str | None): the subsystem the bitstring reflects ("u" or "v")
+        bitstrings: The input list of bitstrings used to generate the state preparation circuits
+        subsystem_id: The subsystem the bitstring reflects ("u" or "v")
 
     Returns:
-        - (tuple[list[QuantumCircuit], list[QuantumCircuit]]): A tuple containing the tensor (i.e., non-superposition
-            or bitstring) circuits in the first index (length = len(bitstrings)) and the super-position circuits
-            as the second element
+        A tuple containing the tensor (i.e., non-superposition or bitstring) circuits in the first
+        index (length = len(bitstrings)) and the super-position circuits as the second element
     """
     # If empty, just return
     if not bitstrings:
         return [], []
 
     if subsystem_id is None:
         subsystem_id = "u"
@@ -583,21 +531,20 @@
 ) -> QuantumCircuit:
     """Prepare the bitstring circuits.
 
     Generate a computational basis state from the input bitstring by applying an X gate to
     every qubit that has a 1 in the bitstring.
 
     Args:
-        - bitstring (np.ndarray | tuple[int, ...]): the container for the
-            bitstring information. Must contain 0s and 1s and the 1s are used to determine
-            where to put the X gates
-        - name (str, optional): the name of the circuit
+        bitstring: The container for the bitstring information. Must contain 0s and 1s, and
+            the 1s are used to determine where to put the X gates
+        name: The name of the circuit
 
     Returns:
-        - (QuantumCircuit): the prepared circuit
+        The prepared circuit
     """
     qcirc = QuantumCircuit(len(bitstring), name=name)
     for qb_idx, bit in enumerate(bitstring):
         if bit:
             qcirc.x(qb_idx)
     return qcirc
 
@@ -607,18 +554,19 @@
 
     Function that partitions the input, a, into a generator containing
     n sub-partitions of a (that are the same type as a).
     Example:
     _partition([1, 2, 3], 2) -> (i for i in [[1, 2], [3]])
 
     Args:
-        - a (iterable): an object with length and indexing to be partitioned
-        - n (int): the number of partitions
+        a: An object with length and indexing to be partitioned
+        n: The number of partitions
+
     Returns:
-        - (generator): the generator containing the paritions
+        The generator containing the paritions
     """
     k, m = divmod(len(a), n)
     return (a[i * k + min(i, m) : (i + 1) * k + min(i + 1, m)] for i in range(n))
 
 
 def _estimate_expvals(
     tensor_ansatze: list[QuantumCircuit],
@@ -628,38 +576,32 @@
     service_args: dict[str, Any] | None = None,
     backend_name: str | None = None,
     options: Options | None = None,
     session_id: str | None = None,
 ) -> tuple[list[np.ndarray], list[np.ndarray], str | None]:
     """Run quantum circuits to generate the expectation values.
 
-    Function to estimate the exepctation value of some observables on the
+    Function to estimate the expectation value of some observables on the
     tensor and superposition circuits used for reconstructing the full
-    expectation value from the Schmidt decomposed circuit. The ray decorator
-    indicates that this is an actor function (that runs its own python
-    process).
+    expectation value from the Schmidt decomposed circuit.
 
     Args:
-        - tensor_ansatze (list[QuantumCircuit]): the circuits that have the same
-            Schmidt coefficient
-        - tensor_paulis (list[Pauli]): the pauli operators to measure and calculate
+        tensor_ansatze: The circuits that have the same Schmidt coefficient
+        tensor_paulis: The pauli operators to measure and calculate
             the expectation values from for the circuits with the same Schmidt coefficient
-        - superposition_ansatze (list[QuantumCircuit]): the circuits with different
-            Schmidt coefficients
-        - superposition_paulis (list[Pauli]): the pauli operators to measure and calculate
-            the expectation values from for the circuits with different Schmidt
-            coefficients
-        - service_args (dict[str, Any]): The service account used to spawn Qiskit primitives
-        - backend_name (str): The backend to use to evaluate the grouped experiments
-        - options (Options): The options to use with the backend
-        - session_id (str): The session id to use when calling primitive programs
+        superposition_ansatze: The circuits with different Schmidt coefficients
+        superposition_paulis: The pauli operators to measure and calculate
+            the expectation values from for the circuits with different Schmidt coefficients
+        service_args: The service account used to spawn Qiskit primitives
+        backend_name: The backend to use to evaluate the grouped experiments
+        options: The options to use with the backend
+        session_id: The session id to use when calling primitive programs
 
     Returns:
-        - (tuple[list[np.ndarray], list[np.ndarray], str | None]): the expectation values for the
-            tensor circuits and superposition circuits
+        The expectation values for the tensor circuits and superposition circuits
     """
     ansatz_t: list[QuantumCircuit] = []
     observables_t: list[Pauli] = []
     for i, circuit in enumerate(tensor_ansatze):
         ansatz_t += [circuit] * len(tensor_paulis)
         observables_t += tensor_paulis
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_operator.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/entanglement_forging/entanglement_forging_operator.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,56 +21,45 @@
 @dataclass
 class EntanglementForgingOperator:  # noqa: D301
     r"""Operator class for Entanglement Forging.
 
     A class that contains the :math:`2N` qubit Pauli operator :math:`\hat{O} = \sum_{i, j} w_{i, j} \hat{T}_{i, j} \otimes \sum_{a, b} \hat{S}_{a, b}`
     and associated weights. These operators are knitted by the :class:`EntanglementForgingKnitter` to provide esimates of the
     energy for the :class:`EntanglementForgingVQE`.
-
-    Attributes:
-        - tensor_paulis (Sequence[PauliOp]): The operators acting on the subsystems that have the same
-            Schmidt coefficients
-        - superposition_paulis (Sequence[PauliOp]): The operators acting on subsystems that have different
-            Schmidt coefficients
-        - w_ij (np.ndarray): The weight matrix associated with the tensor paulis
-        - w_ab (np.ndarray): The weight matrix associated with the superposition paulis
     """
 
     def __init__(
         self,
         tensor_paulis: Sequence[Pauli],
         superposition_paulis: Sequence[Pauli],
         w_ij: np.ndarray,
         w_ab: np.ndarray,
     ):
         r"""
         Assign the necessary member variables.
 
         Args:
-            - tensor_paulis (Sequence[PauliOp]): The operators acting on the subsystems that have the same
-                Schmidt coefficients
-            - superposition_paulis (Sequence[PauliOp]): The operators acting on subsystems that have different
-                Schmidt coefficients
-            - w_ij (np.ndarray): The weight matrix associated with the tensor paulis
-            - w_ab (np.ndarray): The weight matrix associated with the superposition paulis
-
-        Returns:
-            - None
+            tensor_paulis: The operators acting on the subsystems that have the
+                same Schmidt coefficients
+            superposition_paulis: The operators acting on subsystems that have
+                different Schmidt coefficients
+            w_ij: The weight matrix associated with the tensor paulis
+            w_ab: The weight matrix associated with the superposition paulis
         """
         self.tensor_paulis = tensor_paulis
         self.superposition_paulis = superposition_paulis
         self.w_ij = w_ij
         self.w_ab = w_ab
 
     def __repr__(self) -> str:
         """
         Representation function for EntanglementForgingOperator.
 
         Returns:
-            - (str): printable repesentation of class
+            Printable repesentation of class
         """
         repr = "EntanglementForgingOperator\nTensor Paulis:\n"
         repr += str(self.tensor_paulis)
         repr += "\nSuperposition Paulis:\n"
         repr += str(self.superposition_paulis)
         repr += "\nTensor Weight Matrix:\n"
         repr += np.array_str(self.w_ij, precision=4, suppress_small=True)
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/__init__.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/circuit_cutting/wire_cutting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # This code is a Qiskit project.
 
-# (C) Copyright IBM 2022.
+# (C) Copyright IBM 2023.
 
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""
-Utility functions.
+"""Code to initialize the deprecated cutqc wire cutting imports."""
 
-.. autosummary::
-   :toctree: ../stubs/
-   :nosignatures:
-
-   conversion
-   metrics
-   orbital_reduction.reduce_bitstrings
-"""
-
-from .orbital_reduction import reduce_bitstrings
-
-__all__ = [
-    "reduce_bitstrings",
-]
+from warnings import warn
+
+from .cutqc import *  # noqa: F403
+
+warn(
+    f"The package namespace {__name__} is deprecated and will be removed in "
+    "Circuit Knitting Toolbox 0.3.0. Use namespace "
+    "circuit_knitting_toolbox.circuit_cutting.cutqc instead.",
+    DeprecationWarning,
+    stacklevel=2,
+)
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/conversion.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/conversion.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,54 +5,65 @@
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Code for converting types of distributions."""
+"""
+Code for converting types of distributions.
+
+.. currentmodule:: circuit_knitting_toolbox.utils.conversion
+
+.. autosummary::
+   :toctree: ../stubs/
+
+   quasi_to_real
+   nearest_probability_distribution
+   naive_probability_distribution
+   dict_to_array
+"""
 
 import numpy as np
 
 
 def quasi_to_real(quasiprobability, mode):
     """
     Convert a quasi probability to a valid probability distribution.
 
     Args:
-        - quasiprobability (NDArray): the array of quasiprobabilities
-        - mode (str): how to compute the new distribution, either 'nearest'
-            or 'naive'
+        quasiprobability: The array of quasiprobabilities
+        mode: How to compute the new distribution, either 'nearest' or 'naive'
 
     Returns:
-        - (NDArray) the converted probability distribution
+        The converted probability distribution
     """
     if mode == "nearest":
         return nearest_probability_distribution(quasiprobability=quasiprobability)
     elif mode == "naive":
         return naive_probability_distribution(quasiprobability=quasiprobability)
     else:
         raise NotImplementedError("%s conversion is not implemented" % mode)
 
 
 def nearest_probability_distribution(quasiprobability):
     """
-    Convert quasiprobability dist to the nearest probability dist.
+    Convert quasiprobability distribution to the nearest probability distribution.
 
     Takes a quasiprobability distribution and maps
     it to the closest probability distribution as defined by
     the L2-norm.
 
     Method from Smolin et al., Phys. Rev. Lett. 108, 070502 (2012).
 
     Args:
-        - quasiprobability (NDArray): the input quasiprobabilities
+        quasiprobability: The input quasiprobabilities
 
     Returns:
-        - (NDArray): the converted probability distribution
+        The converted probability distribution
     """
     sorted_probs, states = zip(
         *sorted(zip(quasiprobability, range(len(quasiprobability))))
     )
     num_elems = len(sorted_probs)
     new_probs = np.zeros(num_elems)
     beta = 0
@@ -74,35 +85,35 @@
     Convert quasiprobability dist to probability dist by zero-ing out negative values.
 
     Takes a quasiprobability distribution and does the following two steps:
     1. Update all negative probabilities to 0
     2. Normalize
 
     Args:
-        - quasiprobability (NDArray): the input quasiprobabilities
+        quasiprobability: The input quasiprobabilities
 
     Returns:
-        - (NDArray): the converted probability distribution
+        The converted probability distribution
     """
     new_probs = np.where(quasiprobability < 0, 0, quasiprobability)
     new_probs /= np.sum(new_probs)
     return new_probs
 
 
 def dict_to_array(distribution_dict, force_prob):
     """
     Convert dictionary of shot results to array of distribution.
 
     Args:
-        - distribution_dict (dict): the dictionary containing the shot information
+        distribution_dict: The dictionary containing the shot information
             from circuit execution
-        - force_prob (bool): whether to force the distribution to be normalized
+        force_prob: Whether to force the distribution to be normalized
 
     Returns:
-        - (NDarray): the resulting probability information
+        The resulting probability information
     """
     state = list(distribution_dict.keys())[0]
     num_qubits = len(state)
     num_shots = sum(distribution_dict.values())
     cnts = np.zeros(2**num_qubits, dtype=float)
     for state in distribution_dict:
         cnts[int(state, 2)] = distribution_dict[state]
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/metrics.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,28 @@
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Functions for comparing array distances."""
+"""
+Functions for comparing array distances.
+
+.. currentmodule:: circuit_knitting_toolbox.utils.metrics
+
+.. autosummary::
+   :toctree: ../stubs
+
+   chi2_distance
+   MSE
+   MAPE
+   cross_entropy
+   HOP
+"""
 
 import copy
 
 import numpy as np
 
 
 def chi2_distance(target, obs):  # noqa: D301
@@ -27,23 +40,22 @@
     >>> chi2_distance(np.array([0.1, 0.1, 0.3, 0.5]), np.array([0.25, 0.25, 0.25, 0.25]))
     0.21645021645021645
 
     >>> chi2_distance(np.array([0.25, 0.25, 0.25, 0.25]), np.array([0.25, 0.25, 0.25, 0.25]))
     0
 
     Args:
-        - target (NDArray): the target feature vector
-        - obs (NDArray): the actually observed feature vector
+        target: The target feature vector
+        obs: The actually observed feature vector
 
     Returns:
-        - (float): the computed distance
+        The computed distance
 
     Raises:
-        - Exception: if the target is not a numpy array or dictionary, an exception
-            is raised
+        Exception: The target is not a numpy array or dictionary
     """
     target = copy.deepcopy(target)
     obs = copy.deepcopy(obs)
     obs = np.absolute(obs)
     if isinstance(target, np.ndarray):
         assert len(target) == len(obs)
         distance = 0
@@ -73,24 +85,24 @@
     $\sum_i (x_i - y_i)^2$.
 
     Example:
     >>> MSE(np.array([0.1, 0.1, 0.3, 0.5]), np.array([0.25, 0.25, 0.25, 0.25]))
     0.0275
 
     Args:
-        - target (NDArray): the target feature vector
-        - obs (NDArray): the actually observed feature vector
+        target: The target feature vector
+        obs: The actually observed feature vector
 
     Returns:
-        - (float): the computed MSE
+        The computed MSE
 
     Raises:
-        - Exception: if the target is not a dict, or if the target and obs are not
-            numpy arrays or if the target is not a numpy array and the obs are not
-            a dict an expection is raised
+        Exception: The target is not a dict
+        Exception: The target and obs are not numpy arrays
+        Exception: The target is not a numpy array and the obs are not a dict
     """
     target = copy.deepcopy(target)
     obs = copy.deepcopy(obs)
     if isinstance(target, dict):
         se = 0
         for t_idx in target:
             t = target[t_idx]
@@ -124,24 +136,24 @@
     $ \sum_i \frac{x_i - y_i}{x_i} $.
 
     Example:
     >>> MAPE(np.array([0.1, 0.1, 0.3, 0.5]), np.array([0.25, 0.25, 0.25, 0.25]))
     91.66666666666659
 
     Args:
-        - target (NDArray): the target feature vector
-        - obs (NDArray): the actually observed feature vector
+        target: The target feature vector
+        obs: The actually observed feature vector
 
     Returns:
-        - (float): the computed MAPE
+        The computed MAPE
 
     Raises:
-        - Exception: if the target is not a dict, or if the target and obs are not
-            numpy arrays or if the target is not a numpy array and the obs are not
-            a dict an expection is raised
+        Exception: The target is not a dict
+        Exception: The target and obs are not numpy arrays
+        Exception: The target is not a numpy array and the obs are not a dict
     """
     target = copy.deepcopy(target)
     obs = copy.deepcopy(obs)
     epsilon = 1e-16
     if isinstance(target, dict):
         curr_sum = np.sum(list(target.values()))
         new_sum = curr_sum + epsilon * len(target)
@@ -172,35 +184,35 @@
     else:
         raise Exception("target type : %s" % type(target))
     return mape * 100
 
 
 def cross_entropy(target, obs):  # noqa: D301
     r"""
-    Compue the cross entropy between two distributions.
+    Compute the cross entropy between two distributions.
 
     The cross entropy is a measure of the difference between two probability
     distributions, defined via:
     $ -\sum_i x_i \log y_i $.
 
     Example:
     >>> cross_entropy(np.array([0.1, 0.1, 0.3, 0.5]), np.array([0.25, 0.25, 0.25, 0.25]))
     1.3862943611198906
 
     Args:
-        - target (NDArray): the target feature vector
-        - obs (NDArray): the actually observed feature vector
+        target: The target feature vector
+        obs: The actually observed feature vector
 
     Returns:
-        - (float): the computed cross entropy
+        The computed cross entropy
 
     Raises:
-        - Exception: if the target is not a dict, or if the target and obs are not
-            numpy arrays or if the target is not a numpy array and the obs are not
-            a dict an expection is raised
+        Exception: The target is not a dict
+        Exception: The target and obs are not numpy arrays
+        Exception: The target is not a numpy array and the obs are not a dict
     """
     target = copy.deepcopy(target)
     obs = copy.deepcopy(obs)
     if isinstance(target, dict):
         CE = 0
         for t_idx in target:
             t = target[t_idx]
@@ -222,29 +234,29 @@
         return CE
     else:
         raise Exception("target type : %s, obs type : %s" % (type(target), type(obs)))
 
 
 def HOP(target, obs):
     """
-    Compue the Heavy Output Probability (HOP).
+    Compute the Heavy Output Probability (HOP).
 
     The HOP is an important metric for quantum volume experiments and is defined at the
     probability that one measures a bitstring above the median target probability.
 
     Example:
     >>> HOP(np.array([0.1, 0.1, 0.3, 0.5]), np.array([0.25, 0.25, 0.25, 0.25]))
     0.5
 
     Args:
-        - target (NDArray): the target feature vector
-        - obs (NDArray): the actually observed feature vector
+        target: The target feature vector
+        obs: The actually observed feature vector
 
     Returns:
-        - (float): the computed HOP
+        The computed HOP
     """
     target = copy.deepcopy(target)
     obs = copy.deepcopy(obs)
     target_median = np.median(target)
     hop = 0
     for t, o in zip(target, obs):
         if t > target_median:
```

### Comparing `circuit-knitting-toolbox-0.1.0/circuit_knitting_toolbox/utils/orbital_reduction.py` & `circuit_knitting_toolbox-0.2.0/circuit_knitting_toolbox/utils/orbital_reduction.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 # This code is licensed under the Apache License, Version 2.0. You may
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Helper functions for reducing orbitals."""
+"""
+Helper functions for reducing orbitals.
+
+.. currentmodule:: circuit_knitting_toolbox.utils.orbital_reduction
+
+.. autosummary::
+   :toctree: ../stubs
+
+   reduce_bitstrings
+"""
 
 import numpy as np
 
 
 def reduce_bitstrings(bitstrings, orbitals_to_reduce):
     """
     Eliminates the specified orbitals in the bitstrings.
@@ -22,20 +31,18 @@
     elements of the bitstrings.
 
     Example:
     >>> reduce_bitstrings([[1, 0, 0, 1, 0], [1, 0, 0, 0, 1], [1, 1, 1, 1, 0]], [0, 1])
     [(0, 1, 0), (0, 0, 1), (1, 1, 0)]
 
     Args:
-        - bitstrings (List[List[Int]]): the list of bitstrings to be
-            reduced
-        - orbitals_to_reduce (List[Int]): the positions/orbitals to
-            remove from the bitstrings
+        bitstrings: The list of bitstrings to be reduced
+        orbitals_to_reduce: The positions/orbitals to remove from the bitstrings
 
     Returns:
-        - (List[Tuple]): the list of reduced bitstrings
+        The list of reduced bitstrings
 
     """
     reduced_bitstrings_list = np.delete(
         bitstrings, orbitals_to_reduce, axis=-1
     ).tolist()
     return [tuple(bs) for bs in reduced_bitstrings_list]
```

### Comparing `circuit-knitting-toolbox-0.1.0/docs/_static/no_image.png` & `circuit_knitting_toolbox-0.2.0/docs/_static/no_image.png`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_1_automatic_cut_finding.ipynb` & `circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/cutqc/tutorials/tutorial_1_automatic_cut_finding.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996135461760463%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# CutQC Tutorial 1: Circuit Cutting with Automatic Cut "*

 * *            "Finding\\n')], delete: [0]}}, 4: {'source': {insert: [(2, 'from "*

 * *            "circuit_knitting_toolbox.circuit_cutting.cutqc import cut_circuit_wires\\n')], "*

 * *            "delete: [2]}}, 16: {'source': {insert: [(0, 'from "*

 * *            "circuit_knitting_toolbox.circuit_cutting.cutqc import evaluate_subcircuits\\n')], "*

 * *            "delete: [0]}}, 24: {'source': {insert: [(2, 'from "*

 * *             […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "c6cd641f",
             "metadata": {},
             "source": [
-                "# Tutorial 1: Circuit Cutting with Automatic Cut Finding\n",
+                "# CutQC Tutorial 1: Circuit Cutting with Automatic Cut Finding\n",
                 "\n",
                 "Circuit cutting is a technique to decompose a quantum circuit into smaller circuits, whose results can be knitted together to reconstruct the original circuit output. \n",
                 "\n",
                 "The circuit knitting toolbox implements a wire cutting method presented in [CutQC](https://doi.org/10.1145/3445814.3446758) (Tang et al.). This method allows a circuit wire to be cut such that the generated subcircuits are amended by measurements in the Pauli bases and by state preparation of four Pauli eigenstates (see Fig. 4 of [CutQC](https://doi.org/10.1145/3445814.3446758)).\n",
                 "\n",
                 "This wire cutting technique is comprised of the following basic steps:\n",
                 "\n",
@@ -85,15 +85,15 @@
             "execution_count": 6,
             "id": "8c11457a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%%capture\n",
                 "\n",
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import cut_circuit_wires\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import cut_circuit_wires\n",
                 "\n",
                 "cuts = cut_circuit_wires(\n",
                 "    circuit=circuit,\n",
                 "    method=\"automatic\",\n",
                 "    max_subcircuit_width=5,\n",
                 "    max_cuts=2,\n",
                 "    num_subcircuits=[2],\n",
@@ -259,15 +259,15 @@
         {
             "cell_type": "code",
             "execution_count": 12,
             "id": "2ae5160c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import evaluate_subcircuits\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import evaluate_subcircuits\n",
                 "\n",
                 "subcircuit_instance_probabilities = evaluate_subcircuits(cuts)\n",
                 "\n",
                 "# Uncomment the following lines to instead use Qiskit Runtime Service as configured above.\n",
                 "# subcircuit_instance_probabilities = evaluate_subcircuits(cuts,\n",
                 "#                                                          service_args=service.active_account(),\n",
                 "#                                                          backend_names=backend_names,\n",
@@ -387,15 +387,15 @@
             "execution_count": 16,
             "id": "5aceecc0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%%capture\n",
                 "\n",
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import (\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import (\n",
                 "    reconstruct_full_distribution,\n",
                 ")\n",
                 "\n",
                 "reconstructed_probabilities = reconstruct_full_distribution(\n",
                 "    circuit, subcircuit_instance_probabilities, cuts\n",
                 ")"
             ]
@@ -441,15 +441,15 @@
         {
             "cell_type": "code",
             "execution_count": 18,
             "id": "5353b0c8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import verify\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import verify\n",
                 "\n",
                 "metrics, exact_probabilities = verify(circuit, reconstructed_probabilities)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "03f63d3b",
```

### Comparing `circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_2_manual_cutting.ipynb` & `circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/cutqc/tutorials/tutorial_2_manual_cutting.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995202020202021%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# CutQC Tutorial 2: Circuit Cutting with Manual Wire "*

 * *            "Cutting\\n')], delete: [0]}}, 8: {'source': {insert: [(2, 'from "*

 * *            "circuit_knitting_toolbox.circuit_cutting.cutqc import cut_circuit_wires\\n')], "*

 * *            "delete: [2]}}, 18: {'source': {insert: [(0, 'from "*

 * *            "circuit_knitting_toolbox.circuit_cutting.cutqc import evaluate_subcircuits\\n')], "*

 * *            "delete: [0]}}, 21: {'source': {insert: [(2, 'from "*

 * *            "c […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "c6cd641f",
             "metadata": {},
             "source": [
-                "# Tutorial 2: Circuit Cutting with Manual Wire Cutting\n",
+                "# CutQC Tutorial 2: Circuit Cutting with Manual Wire Cutting\n",
                 "\n",
                 "Circuit cutting is a technique to decompose a quantum circuit into smaller circuits, whose results can be knitted together to reconstruct the original circuit output. \n",
                 "\n",
                 "The circuit knitting toolbox implements a wire cutting method presented in [CutQC](https://doi.org/10.1145/3445814.3446758) (Tang et al.). This method allows a circuit wire to be cut such that the generated subcircuits are amended by measurements in the Pauli bases and by state preparation of four Pauli eigenstates (see Fig. 4 of [CutQC](https://doi.org/10.1145/3445814.3446758)).\n",
                 "\n",
                 "This wire cutting technique is comprised of the following basic steps:\n",
                 "\n",
@@ -151,15 +151,15 @@
             "execution_count": 7,
             "id": "8c11457a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%%capture\n",
                 "\n",
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import cut_circuit_wires\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import cut_circuit_wires\n",
                 "\n",
                 "cuts = cut_circuit_wires(\n",
                 "    circuit=circuit, method=\"manual\", subcircuit_vertices=[[0, 1], [2, 3]]\n",
                 ")"
             ]
         },
         {
@@ -291,15 +291,15 @@
         {
             "cell_type": "code",
             "execution_count": 12,
             "id": "2ae5160c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import evaluate_subcircuits\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import evaluate_subcircuits\n",
                 "\n",
                 "subcircuit_instance_probabilities = evaluate_subcircuits(cuts)\n",
                 "\n",
                 "# Uncomment the following lines to instead use Qiskit Runtime Service as configured above.\n",
                 "# subcircuit_instance_probabilities = evaluate_subcircuits(cuts,\n",
                 "#                                                          service_args=service.active_account(),\n",
                 "#                                                          backend_names=backend_names,\n",
@@ -330,15 +330,15 @@
             "execution_count": 13,
             "id": "5aceecc0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "%%capture\n",
                 "\n",
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import (\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import (\n",
                 "    reconstruct_full_distribution,\n",
                 ")\n",
                 "\n",
                 "reconstructed_probabilities = reconstruct_full_distribution(\n",
                 "    circuit, subcircuit_instance_probabilities, cuts\n",
                 ")"
             ]
@@ -356,15 +356,15 @@
         {
             "cell_type": "code",
             "execution_count": 14,
             "id": "5353b0c8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import verify\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import verify\n",
                 "\n",
                 "metrics, exact_probabilities = verify(circuit, reconstructed_probabilities)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b220335e",
```

### Comparing `circuit-knitting-toolbox-0.1.0/docs/circuit_cutting/tutorials/tutorial_3_cutting_with_quantum_serverless.ipynb` & `circuit_knitting_toolbox-0.2.0/docs/circuit_cutting/cutqc/tutorials/tutorial_3_cutting_with_quantum_serverless.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996504417276353%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# CutQC Tutorial 3: Circuit Cutting with Quantum "*

 * *            "Serverless\\n')], delete: [0]}}, 6: {'source': {insert: [(2, 'from "*

 * *            "circuit_knitting_toolbox.circuit_cutting.cutqc import cut_circuit_wires\\n'), (4, "*

 * *            "'\\n')], delete: [2]}}, 13: {'source': {insert: [(1, 'from "*

 * *            "circuit_knitting_toolbox.circuit_cutting.cutqc import evaluate_subcircuits\\n'), (2, "*

 * *            "'\\n')], delete: [1]}}, 21: {'source': {insert: [(0, […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "c6cd641f",
             "metadata": {},
             "source": [
-                "# Tutorial 3: Circuit Cutting with Quantum Serverless\n",
+                "# CutQC Tutorial 3: Circuit Cutting with Quantum Serverless\n",
                 "\n",
                 "**Circuit cutting** is a technique to decompose a quantum circuit into smaller circuits, whose results can be knitted together to reconstruct the original circuit output. \n",
                 "\n",
                 "The circuit knitting toolbox implements a wire cutting method presented in [CutQC](https://doi.org/10.1145/3445814.3446758) (Tang et al.). This method allows a circuit wire to be cut such that the generated subcircuits are amended by measurements in the Pauli bases and by state preparation of four Pauli eigenstates (see Fig. 4 of [CutQC](https://doi.org/10.1145/3445814.3446758)).\n",
                 "\n",
                 "This wire cutting technique is comprised of the following basic steps:\n",
                 "\n",
@@ -122,17 +122,18 @@
             "execution_count": 3,
             "id": "8c11457a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from typing import Sequence, Any\n",
                 "from qiskit import QuantumCircuit\n",
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import cut_circuit_wires\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import cut_circuit_wires\n",
                 "from quantum_serverless import distribute_task, get\n",
                 "\n",
+                "\n",
                 "# Create a wrapper function to be sent to remote cluster\n",
                 "@distribute_task()\n",
                 "def cut_circuit_wires_remote(\n",
                 "    circuit: QuantumCircuit,\n",
                 "    method: str,\n",
                 "    subcircuit_vertices: Sequence[Sequence[int]] | None = None,\n",
                 "    max_subcircuit_width: int | None = None,\n",
@@ -297,15 +298,16 @@
             "cell_type": "code",
             "execution_count": 7,
             "id": "3234f5f8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from qiskit_ibm_runtime import Options\n",
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import evaluate_subcircuits\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import evaluate_subcircuits\n",
+                "\n",
                 "\n",
                 "# Create a wrapper function to be sent to remote cluster\n",
                 "@distribute_task()\n",
                 "def evaluate_subcircuits_remote(\n",
                 "    cuts: dict[str, Any],\n",
                 "    service_args: dict[str, Any] | None = None,\n",
                 "    backend_names: Sequence[str] | None = None,\n",
@@ -429,15 +431,15 @@
         {
             "cell_type": "code",
             "execution_count": 11,
             "id": "9a74644d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import (\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import (\n",
                 "    reconstruct_full_distribution,\n",
                 ")\n",
                 "\n",
                 "\n",
                 "@distribute_task()\n",
                 "def reconstruct_full_distribution_remote(\n",
                 "    circuit: QuantumCircuit,\n",
@@ -491,15 +493,15 @@
         {
             "cell_type": "code",
             "execution_count": 13,
             "id": "5353b0c8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from circuit_knitting_toolbox.circuit_cutting.wire_cutting import verify\n",
+                "from circuit_knitting_toolbox.circuit_cutting.cutqc import verify\n",
                 "\n",
                 "metrics, exact_probabilities = verify(circuit, reconstructed_probabilities)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "03f63d3b",
```

### Comparing `circuit-knitting-toolbox-0.1.0/docs/conf.py` & `circuit_knitting_toolbox-0.2.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 templates_path = ["_templates"]
 numfig = True
 numfig_format = {"table": "Table %s"}
 language = "en"
 pygments_style = "colorful"
 add_module_names = False
 modindex_common_prefix = ["circuit_knitting_toolbox."]
-html_css_files = ["gallery.css"]
+html_css_files = ["style.css"]
 
 # html theme options
 html_static_path = ["_static"]
 # html_logo = "_static/images/logo.png"
 
 # autodoc/autosummary options
 autosummary_generate = True
```

### Comparing `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/figs/Fig_5_c.png` & `circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/explanation/figs/Fig_5_c.png`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/figs/forging_info_graphic.png` & `circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/explanation/figs/forging_info_graphic.png`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/explanation/index.rst` & `circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/explanation/index.rst`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/freeze-orbitals.ipynb` & `circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/how-tos/freeze-orbitals.ipynb`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/specify-problem.rst` & `circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/how-tos/specify-problem.rst`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/how-tos/use-asymmetric-bitstrings.ipynb` & `circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/how-tos/use-asymmetric-bitstrings.ipynb`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/data/reactant_2mo.npz` & `circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/tutorials/data/reactant_2mo.npz`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/tutorial_1_getting_started.ipynb` & `circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/tutorials/tutorial_1_getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/docs/entanglement_forging/tutorials/tutorial_2_forging_with_quantum_serverless.ipynb` & `circuit_knitting_toolbox-0.2.0/docs/entanglement_forging/tutorials/tutorial_2_forging_with_quantum_serverless.ipynb`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/docs/index.rst` & `circuit_knitting_toolbox-0.2.0/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -11,28 +11,37 @@
 - Circuit Cutting
 - Entanglement Forging
 
 The source code to the toolbox is available `on GitHub <https://github.com/Qiskit-Extensions/circuit-knitting-toolbox>`_.
 
 .. note::
 
-   The `Quantum Serverless <https://qiskit-extensions.github.io/quantum-serverless/>`_ framework is documented separately, as it lives in its own repository.  Check out `Tutorial 2: Forging with Quantum Serverless <./entanglement_forging/tutorials/tutorial_2_forging_with_quantum_serverless.ipynb>`_  and `Tutorial 3: Circuit Cutting with Quantum Serverless <./circuit_cutting/tutorials/tutorial_3_cutting_with_quantum_serverless.ipynb>`_ for examples on how to integrate Quantum Serverless into circuit knitting workflows.
+   The `Quantum Serverless <https://qiskit-extensions.github.io/quantum-serverless/>`_ framework is documented separately, as it lives in its own repository.  Check out `Entanglement Forging Tutorial 2: Forging with Quantum Serverless <./entanglement_forging/tutorials/tutorial_2_forging_with_quantum_serverless.ipynb>`_  and `CutQC Tutorial 3: Circuit Cutting with Quantum Serverless <./circuit_cutting/tutorials/cutqc/tutorial_3_cutting_with_quantum_serverless.ipynb>`_ for examples on how to integrate Quantum Serverless into circuit knitting workflows.
 
 This project is meant to evolve rapidly and, as such, does not follow `Qiskit's deprecation policy <https://qiskit.org/documentation/contributing_to_qiskit.html#deprecation-policy>`_.  We may occasionally make breaking changes in order to improve the user experience.  When possible, we will keep old interfaces and mark them as deprecated, as long as they can co-exist with the new ones.  Each substantial improvement, breaking change, or deprecation will be documented in the :ref:`release notes`.
 
+Citing this project
+-------------------
+
+If you use the Circuit Knitting Toolbox in your research, please cite it according to ``CITATON.bib`` file included in this repository:
+
+.. literalinclude:: ../CITATION.bib
+   :language: bibtex
+
 Contents
 --------
 
 .. toctree::
   :maxdepth: 2
 
   Installation Instructions <install>
   Circuit Cutting Tutorials <circuit_cutting/tutorials/index>
   Circuit Cutting Explanatory Material <circuit_cutting/explanation/index>
   Circuit Cutting How-To Guides <circuit_cutting/how-tos/index>
+  CutQC (legacy circuit cutting implementation) <circuit_cutting/cutqc/index>
   Entanglement Forging Tutorials <entanglement_forging/tutorials/index>
   Entanglement Forging Explanatory Material <entanglement_forging/explanation/index>
   Entanglement Forging How-To Guides <entanglement_forging/how-tos/index>
   API References <apidocs/index>
   Release Notes <release-notes>
 
 .. Hiding - Indices and tables
```

### Comparing `circuit-knitting-toolbox-0.1.0/pyproject.toml` & `circuit_knitting_toolbox-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "circuit-knitting-toolbox"
-version = "0.1.0"
+version = "0.2.0"
 description = "A software prototype for a circuit knitting toolbox which connects user applications with runtime primitives"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 dependencies = [
     "qiskit-aer>=0.12.0",
-    "qiskit-terra>=0.23.3",
+    "qiskit-terra>=0.24.0",
     "qiskit-nature>=0.5.2",
     "qiskit-ibm-runtime>=0.9.2",
 ]
 
 [project.optional-dependencies]
 cplex = [
     # We use the same restrictions in both of the following lines, as there
@@ -40,31 +39,37 @@
     "docplex>=2.23.222; python_version < '3.11' and platform_machine != 'arm64'",
     "cplex>=22.1.0.0; python_version < '3.11' and platform_machine != 'arm64'",
 ]
 pyscf = [
     "pyscf>=2.0.1; sys_platform != 'win32'",
 ]
 dev = [
-    "circuit-knitting-toolbox[test,lint]",
-    "nbmake",
+    "circuit-knitting-toolbox[test,nbtest,lint]",
 ]
-test = [
-    "circuit-knitting-toolbox[pyscf]",
+basetest = [
     "pytest>=6.2.5",
     "pytest-randomly>=1.2.0",
 ]
+test = [
+    "circuit-knitting-toolbox[basetest,pyscf]",
+    "ddt>=1.4.4",
+]
+nbtest = [
+    "circuit-knitting-toolbox[basetest]",
+    "nbmake>=1.3.4"
+]
 style = [
-    "autoflake==1.7.6",
-    "black[jupyter]==22.10.0",
+    "autoflake==2.1.1",
+    "black[jupyter]==23.3.0",
     "ruff>=0.0.246",
 ]
 lint = [
     "circuit-knitting-toolbox[style]",
-    "pydocstyle==6.1.1",
-    "mypy==0.982",
+    "pydocstyle==6.3.0",
+    "mypy==1.3.0",
     "reno>=3.4.0",
     # pydocstyle prefers to parse our pyproject.toml, hence the following line
     "toml",
 ]
 docs = [
     "Sphinx>=3.0.0",
     "sphinx-autodoc-typehints>=1.12.0",
@@ -86,9 +91,15 @@
 "Documentation" = "https://qiskit-extensions.github.io/circuit-knitting-toolbox/"
 "Repository" = "https://github.com/Qiskit-Extensions/circuit-knitting-toolbox"
 
 [tool.autoflake]
 remove-unused-variables = true
 remove-all-unused-imports = true
 
+[tool.coverage.run]
+omit = [
+    # deprecated import location(s)
+    "circuit_knitting_toolbox/circuit_cutting/wire_cutting.py",
+]
+
 [tool.flit.module]
 name = "circuit_knitting_toolbox"
```

### Comparing `circuit-knitting-toolbox-0.1.0/releasenotes/notes/0.1/migrate-to-qiskit-nature-0.5.0-96e90cd48f36d731.yaml` & `circuit_knitting_toolbox-0.2.0/releasenotes/notes/0.1/migrate-to-qiskit-nature-0.5.0-96e90cd48f36d731.yaml`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/test/circuit_cutting/test_circuit_cutting.py` & `circuit_knitting_toolbox-0.2.0/test/circuit_cutting/test_cutqc.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import unittest
 import importlib.util
 
 import numpy as np
 from qiskit import QuantumCircuit
 
-from circuit_knitting_toolbox.circuit_cutting.wire_cutting import (
+from circuit_knitting_toolbox.circuit_cutting.cutqc import (
     cut_circuit_wires,
     evaluate_subcircuits,
     reconstruct_full_distribution,
     verify,
 )
 
 cplex_available = importlib.util.find_spec("cplex") is not None
```

### Comparing `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CH3_two_body.npy` & `circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/CH3_two_body.npy`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CN_one_body.npy` & `circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/CN_one_body.npy`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/CN_two_body.npy` & `circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/CN_two_body.npy`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/O2_one_body.npy` & `circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/O2_one_body.npy`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_data/O2_two_body.npy` & `circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_data/O2_two_body.npy`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_entanglement_forging_ground_state_solver.py` & `circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_entanglement_forging_ground_state_solver.py`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/test/entanglement_forging/test_entanglement_forging_knitter.py` & `circuit_knitting_toolbox-0.2.0/test/entanglement_forging/test_entanglement_forging_knitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Tests for EntanglementForgingKnitter module."""
 
 import os
 import unittest
+import pytest
+
 import numpy as np
 from qiskit.circuit import Parameter, QuantumCircuit
 from qiskit.circuit.library import TwoLocal
 from qiskit_nature.second_q.drivers import PySCFDriver
 from qiskit_nature.second_q.problems import ElectronicStructureProblem, ElectronicBasis
 from qiskit_nature.second_q.hamiltonians import ElectronicEnergy
 from qiskit_nature.second_q.formats import get_ao_to_mo_from_qcschema
@@ -104,15 +106,15 @@
         energy, _, _ = forging_knitter(ansatz_params, forged_hamiltonian)
 
         # Ensure ground state energy output is within tolerance
         self.assertAlmostEqual(energy + energy_shift, -1.121936544469326)
 
     def test_entanglement_forging_H2O(self):  # pylint: disable=too-many-locals
         """
-        Test to apply Entanglement Forging to compute the energy of a H20 molecule,
+        Test to apply Entanglement Forging to compute the energy of a H2O molecule,
         given optimal ansatz parameters.
         """
         # setup problem
         radius_1 = 0.958  # position for the first H atom
         radius_2 = 0.958  # position for the second H atom
         thetas_in_deg = 104.478  # bond angles.
 
@@ -222,14 +224,15 @@
         ansatz_params = [0.0, np.pi / 2]
 
         energy, _, _ = forging_knitter(ansatz_params, forged_hamiltonian)
 
         # Ensure ground state energy output is within tolerance
         self.assertAlmostEqual(energy + energy_shift, -1.1219365445030705)
 
+    @pytest.mark.slow
     def test_asymmetric_bitstrings_O2(self):
         """Test for entanglement forging driver."""
         hamiltonian = ElectronicEnergy.from_raw_integrals(self.hcore_o2, self.eri_o2)
         hamiltonian.nuclear_repulsion_energy = self.energy_shift_o2
         problem = ElectronicStructureProblem(hamiltonian)
         problem.num_particles = (6, 6)
 
@@ -296,14 +299,15 @@
         ansatz_params = [0.0]
 
         energy, _, _ = forging_knitter(ansatz_params, forged_hamiltonian)
 
         # Ensure ground state energy output is within tolerance
         self.assertAlmostEqual(energy + energy_shift, -39.09031477502881)
 
+    @pytest.mark.slow
     def test_asymmetric_bitstrings_CN(self):
         """Test for asymmetric bitstrings with hybrid cross terms."""
         hamiltonian = ElectronicEnergy.from_raw_integrals(self.hcore_cn, self.eri_cn)
         hamiltonian.nuclear_repulsion_energy = self.energy_shift_cn
         problem = ElectronicStructureProblem(hamiltonian)
         problem.num_particles = (5, 4)
```

### Comparing `circuit-knitting-toolbox-0.1.0/tools/extremal_dependency_versions.py` & `circuit_knitting_toolbox-0.2.0/tools/extremal_dependency_versions.py`

 * *Files identical despite different names*

### Comparing `circuit-knitting-toolbox-0.1.0/tox.ini` & `circuit_knitting_toolbox-0.2.0/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 minversion = 3.25
-envlist = py{37,38,39,310,311}{,-notebook}, lint, coverage, docs
+envlist = py{38,39,310,311}{,-notebook}, lint, coverage, docs
 isolated_build = True
 
 [testenv]
 extras =
   test
   cplex
 commands =
@@ -26,39 +26,39 @@
   ruff check circuit_knitting_toolbox/ docs/ test/ tools/
   autoflake --check --recursive circuit_knitting_toolbox/ docs/ test/ tools/
   black --check circuit_knitting_toolbox/ docs/ test/ tools/
   pydocstyle circuit_knitting_toolbox/
   mypy circuit_knitting_toolbox/
   reno lint
 
-[testenv:{,py37-,py38-,py39-,py310-,py311-}notebook]
-deps =
-  nbmake
+[testenv:{,py38-,py39-,py310-,py311-}notebook]
 extras =
+  nbtest
   notebook-dependencies
 commands =
   pytest --nbmake --nbmake-timeout=3000 {posargs} docs/
 
 [testenv:coverage]
+basepython = python3.10
 deps =
   coverage>=5.5
 extras =
   test
   cplex
 commands =
   coverage3 run --source circuit_knitting_toolbox --parallel-mode -m pytest test/ {posargs}
   coverage3 combine
   coverage3 html
-  coverage3 report --fail-under=100 --show-missing --omit="circuit_knitting_toolbox/circuit_cutting/wire_cutting/**/*,circuit_knitting_toolbox/entanglement_forging/**/*,circuit_knitting_toolbox/utils/conversion.py,circuit_knitting_toolbox/utils/metrics.py,circuit_knitting_toolbox/utils/orbital_reduction.py"
+  coverage3 report --fail-under=100 --show-missing --omit="circuit_knitting_toolbox/circuit_cutting/cutqc/**/*,circuit_knitting_toolbox/entanglement_forging/**/*,circuit_knitting_toolbox/utils/conversion.py,circuit_knitting_toolbox/utils/metrics.py,circuit_knitting_toolbox/utils/orbital_reduction.py"
   coverage3 report --fail-under=80
 
 [testenv:docs]
 extras =
   docs
   notebook-dependencies
 commands =
   python -c 'import shutil, pathlib; shutil.rmtree(pathlib.Path("docs") / "stubs", ignore_errors=True)'
   python -c 'import shutil, pathlib; shutil.rmtree(pathlib.Path("docs") / "_build" / "html" / ".doctrees", ignore_errors=True)'
-  sphinx-build -b html -W -T --keep-going {posargs} docs/ docs/_build/html
+  sphinx-build -j auto -b html -W -T --keep-going {posargs} docs/ docs/_build/html
 
 [pytest]
-addopts = --doctest-modules
+addopts = --doctest-modules -rs --durations=10
```

### Comparing `circuit-knitting-toolbox-0.1.0/PKG-INFO` & `circuit_knitting_toolbox-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 Metadata-Version: 2.1
 Name: circuit-knitting-toolbox
-Version: 0.1.0
+Version: 0.2.0
 Summary: A software prototype for a circuit knitting toolbox which connects user applications with runtime primitives
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: qiskit-aer>=0.12.0
-Requires-Dist: qiskit-terra>=0.23.3
+Requires-Dist: qiskit-terra>=0.24.0
 Requires-Dist: qiskit-nature>=0.5.2
 Requires-Dist: qiskit-ibm-runtime>=0.9.2
+Requires-Dist: pytest>=6.2.5 ; extra == "basetest"
+Requires-Dist: pytest-randomly>=1.2.0 ; extra == "basetest"
 Requires-Dist: docplex>=2.23.222 ; extra == "cplex" and ( python_version < '3.11' and platform_machine != 'arm64')
 Requires-Dist: cplex>=22.1.0.0 ; extra == "cplex" and ( python_version < '3.11' and platform_machine != 'arm64')
-Requires-Dist: circuit-knitting-toolbox[test,lint] ; extra == "dev"
-Requires-Dist: nbmake ; extra == "dev"
+Requires-Dist: circuit-knitting-toolbox[test,nbtest,lint] ; extra == "dev"
 Requires-Dist: Sphinx>=3.0.0 ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints>=1.12.0 ; extra == "docs"
 Requires-Dist: jupyter-sphinx>=0.3.2 ; extra == "docs"
 Requires-Dist: nbsphinx>=0.8.8 ; extra == "docs"
 Requires-Dist: sphinx-copybutton>=0.5.0 ; extra == "docs"
 Requires-Dist: reno>=3.4.0 ; extra == "docs"
 Requires-Dist: circuit-knitting-toolbox[style] ; extra == "lint"
-Requires-Dist: pydocstyle==6.1.1 ; extra == "lint"
-Requires-Dist: mypy==0.982 ; extra == "lint"
+Requires-Dist: pydocstyle==6.3.0 ; extra == "lint"
+Requires-Dist: mypy==1.3.0 ; extra == "lint"
 Requires-Dist: reno>=3.4.0 ; extra == "lint"
 Requires-Dist: toml ; extra == "lint"
+Requires-Dist: circuit-knitting-toolbox[basetest] ; extra == "nbtest"
+Requires-Dist: nbmake>=1.3.4 ; extra == "nbtest"
 Requires-Dist: circuit-knitting-toolbox[cplex,pyscf] ; extra == "notebook-dependencies"
 Requires-Dist: quantum-serverless>=0.0.7 ; extra == "notebook-dependencies"
 Requires-Dist: matplotlib ; extra == "notebook-dependencies"
 Requires-Dist: ipywidgets ; extra == "notebook-dependencies"
 Requires-Dist: pylatexenc ; extra == "notebook-dependencies"
 Requires-Dist: qiskit-nature<0.6.0 ; extra == "notebook-dependencies"
 Requires-Dist: pyscf>=2.0.1 ; extra == "pyscf" and ( sys_platform != 'win32')
-Requires-Dist: autoflake==1.7.6 ; extra == "style"
-Requires-Dist: black[jupyter]==22.10.0 ; extra == "style"
+Requires-Dist: autoflake==2.1.1 ; extra == "style"
+Requires-Dist: black[jupyter]==23.3.0 ; extra == "style"
 Requires-Dist: ruff>=0.0.246 ; extra == "style"
-Requires-Dist: circuit-knitting-toolbox[pyscf] ; extra == "test"
-Requires-Dist: pytest>=6.2.5 ; extra == "test"
-Requires-Dist: pytest-randomly>=1.2.0 ; extra == "test"
+Requires-Dist: circuit-knitting-toolbox[basetest,pyscf] ; extra == "test"
+Requires-Dist: ddt>=1.4.4 ; extra == "test"
 Project-URL: Documentation, https://qiskit-extensions.github.io/circuit-knitting-toolbox/
 Project-URL: Repository, https://github.com/Qiskit-Extensions/circuit-knitting-toolbox
+Provides-Extra: basetest
 Provides-Extra: cplex
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: lint
+Provides-Extra: nbtest
 Provides-Extra: notebook-dependencies
 Provides-Extra: pyscf
 Provides-Extra: style
 Provides-Extra: test
 
 <!-- SHIELDS -->
 <div align="left">
 
   [![Stability](https://img.shields.io/badge/Stability-alpha-f4d03f.svg)](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/releases)
   ![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS-informational)
-  [![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational)](https://www.python.org/)
-  [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.42.1-6133BD)](https://github.com/Qiskit/qiskit)
+  [![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational)](https://www.python.org/)
+  [![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.43.0-6133BD)](https://github.com/Qiskit/qiskit)
   [![Qiskit Nature](https://img.shields.io/badge/Qiskit%20Nature-%E2%89%A5%200.5.2-6133BD)](https://github.com/Qiskit/qiskit-nature)
 <br />
   [![License](https://img.shields.io/github/license/Qiskit-Extensions/circuit-knitting-toolbox?label=License)](LICENSE.txt)
   [![Code style: Black](https://img.shields.io/badge/Code%20style-Black-000.svg)](https://github.com/psf/black)
   [![Tests](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/actions/workflows/test_latest_versions.yml/badge.svg)](https://github.com/Qiskit-Extensions/circuit-knitting-toolbox/actions/workflows/test_latest_versions.yml)
   [![Coverage](https://coveralls.io/repos/github/Qiskit-Extensions/circuit-knitting-toolbox/badge.svg?branch=main)](https://coveralls.io/github/Qiskit-Extensions/circuit-knitting-toolbox?branch=main)
 
@@ -92,15 +95,15 @@
 
 Each tool in the CKT partitions a user's problem into quantum and classical components to enable efficient use of resources constrained by scaling limits, i.e. size of quantum processors and classical compute capability. It can assign the execution of "quantum code" to QPUs or QPU simulators and "classical code" to various heterogeneous classical resources such as CPUs, GPUs, and TPUs made available via hybrid cloud, on-prem, data centers, etc. 
 
 The toolbox enables users to run parallelized and hybrid (quantum + classical) workloads without worrying about allocating and managing underlying infrastructure.
 
 The toolbox currently contains the following tools:
 - Entanglement Forging [[1]](#references)
-- Circuit Cutting [[2]](#references)
+- Circuit Cutting [[2-6]](#references)
   
 ----------------------------------------------------------------------------------------------------
   
 ### Documentation
 
 The documentation, including installation instructions, is available at https://qiskit-extensions.github.io/circuit-knitting-toolbox/.
 
@@ -110,17 +113,25 @@
 
 This project is meant to evolve rapidly and, as such, does not follow [Qiskit's deprecation policy](https://qiskit.org/documentation/contributing_to_qiskit.html#deprecation-policy).  We may occasionally make breaking changes in order to improve the user experience.  When possible, we will keep old interfaces and mark them as deprecated, as long as they can co-exist with the new ones.  Each substantial improvement, breaking change, or deprecation will be documented in the [release notes](https://qiskit-extensions.github.io/circuit-knitting-toolbox/release-notes.html).
 
 ----------------------------------------------------------------------------------------------------
 
 ### References
 
-[1] Andrew Eddins, Mario Motta, Tanvi P. Gujarati, Sergey Bravyi, Antonio Mezzacapo, Charles Hadfield, Sarah Sheldon, [Doubling the size of quantum simulators by entanglement forging](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.3.010309). PRX Quantum 3, 010309 (2022).
+[1] Andrew Eddins, Mario Motta, Tanvi P. Gujarati, Sergey Bravyi, Antonio Mezzacapo, Charles Hadfield, Sarah Sheldon, [Doubling the size of quantum simulators by entanglement forging](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.3.010309), PRX Quantum 3, 010309 (2022).
 
-[2] Wei Tang, Teague Tomesh, Martin Suchara, Jeffrey Larson, Margaret Martonosi, [CutQC: Using Small Quantum Computers for Large Quantum Circuit Evaluations](https://doi.org/10.1145/3445814.3446758), Proceedings of the 26th ACM International Conference on Architectural Support for Programming Languages and Operating Systems. pp. 473 (2021).
+[2] Kosuke Mitarai, Keisuke Fujii, [Constructing a virtual two-qubit gate by sampling single-qubit operations](https://iopscience.iop.org/article/10.1088/1367-2630/abd7bc), New J. Phys. 23 023021.
 
+[3] Christophe Piveteau, David Sutter, [Circuit knitting with classical communication](https://arxiv.org/abs/2205.00016), arXiv:2205.00016 [quant-ph].
+
+[4] Lukas Brenner, Christophe Piveteau, David Sutter, [Optimal wire cutting with classical communication](https://arxiv.org/abs/2302.03366), arXiv:2302.03366 [quant-ph].
+
+[5] Wei Tang, Teague Tomesh, Martin Suchara, Jeffrey Larson, Margaret Martonosi, [CutQC: Using small quantum computers for large quantum circuit evaluations](https://doi.org/10.1145/3445814.3446758), Proceedings of the 26th ACM International Conference on Architectural Support for Programming Languages and Operating Systems. pp. 473 (2021).
+  
+[6] K. Temme, S. Bravyi, and J. M. Gambetta, [Error mitigation for short-depth quantum circuits](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.119.180509), Physical Review Letters, 119(18), (2017).
+  
 ----------------------------------------------------------------------------------------------------
 
 <!-- LICENSE -->
 ### License
 [Apache License 2.0](LICENSE.txt)
```

