# Comparing `tmp/esse-2022.9.6.post0.tar.gz` & `tmp/esse-2023.5.29.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esse-2022.9.6.post0.tar", last modified: Tue Sep  6 13:58:37 2022, max compression
+gzip compressed data, was "esse-2023.5.29.post0.tar", last modified: Mon May 29 23:51:50 2023, max compression
```

## Comparing `esse-2022.9.6.post0.tar` & `esse-2023.5.29.post0.tar`

### file list

```diff
@@ -1,1230 +1,1262 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.063581 esse-2022.9.6.post0/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/.babelrc
--rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/.eslintrc.json
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.931571 esse-2022.9.6.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.951573 esse-2022.9.6.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2796 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     5489 2022-09-06 13:58:37.063581 esse-2022.9.6.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4933 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/build_schemas.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.951573 esse-2022.9.6.post0/example/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.951573 esse-2022.9.6.post0/example/core/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.951573 esse-2022.9.6.post0/example/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/abstract/2d_data.json
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/abstract/2d_plot.json
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/abstract/3d_grid.json
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/abstract/3d_tensor.json
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/abstract/3d_vector_basis.json
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/abstract/point.json
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/abstract/vector.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.951573 esse-2022.9.6.post0/example/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/primitive/1d_data_series.json
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/primitive/3d_lattice.json
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/primitive/array_of_3_booleans.json
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/primitive/array_of_3_numbers.json
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/primitive/array_of_ids.json
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/primitive/axis.json
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/primitive/scalar.json
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/primitive/string.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/core/reference/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reference/experiment/condition.json
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reference/experiment/location.json
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reference/experiment.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reference/literature/name.json
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reference/literature/pages.json
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reference/literature.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reference/modeling/exabyte.json
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reference/modeling.json
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reference.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/core/reusable/
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reusable/atomic_vectors.json
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reusable/band_gap.json
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reusable/energy.json
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reusable/file_metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/core/reusable/object_storage_container_data.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/element.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/job/
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/job/compute.json
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/job.json
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/material.json
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/method.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/methods_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/local-orbital.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/methods_directory/pseudopotential/
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/pseudopotential/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/methods_directory/pseudopotential/file/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/pseudopotential/file/energy_cutoff.json
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/pseudopotential/file/exchange_correlation.json
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/pseudopotential/file/radii.json
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/pseudopotential/file.json
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/pseudopotential/precision.json
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/pseudopotential.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/methods_directory/regression/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/regression/data_per_feature.json
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/regression/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/methods_directory/regression/kernel_ridge/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/regression/kernel_ridge/data_per_property.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/methods_directory/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/regression/linear/data_per_property.json
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/regression/precision.json
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/regression/precision_per_property.json
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/methods_directory/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/model/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/model/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/model.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.931571 esse-2022.9.6.post0/example/models_directory/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.931571 esse-2022.9.6.post0/example/models_directory/pb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/models_directory/pb/qm/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/models_directory/pb/qm/abin/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/abin/configuration_interaction.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.955573 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/functional/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/functional/component.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/functional/components_directory/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/gga/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/gga/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/lda/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/lda/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/lda.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/mgga/
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/mgga/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft.json
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/pb/qm/semp.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.931571 esse-2022.9.6.post0/example/models_directory/st/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/models_directory/st/det/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/models_directory/st/det/ml.json
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/new_model.json
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/project.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/electronic_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/elemental/atomic_radius.json
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/elemental/electronegativity.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/elemental/ionization_potential.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.959573 esse-2022.9.6.post0/example/properties_directory/non-scalar/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/band_gaps.json
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/band_structure.json
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/charge_density_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/density_of_states.json
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/file_content.json
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/phonon_dispersions.json
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/phonon_dos.json
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/reaction_energy_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/stress_tensor.json
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/total_energy_contributions.json
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/non-scalar/vibrational_spectrum.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.963574 esse-2022.9.6.post0/example/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/scalar/electron_affinity.json
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/scalar/fermi_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/scalar/formation_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/scalar/ionization_potential.json
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/scalar/pressure.json
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/scalar/reaction_energy_barrier.json
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/scalar/surface_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/scalar/total_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/scalar/total_force.json
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/scalar/zero_point_energy.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.963574 esse-2022.9.6.post0/example/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/atomic_forces.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.963574 esse-2022.9.6.post0/example/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/basis/atomic_constraints.json
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/basis/atomic_coordinate.json
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/basis/atomic_coordinates.json
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/basis/atomic_element.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/basis/bonds.json
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/basis.json
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/density.json
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/elemental_ratio.json
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/inchi.json
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/inchi_key.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.963574 esse-2022.9.6.post0/example/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/lattice/lattice_bravais.json
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/lattice/lattice_vectors.json
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/lattice.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/magnetic_moments.json
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/molecular_pattern.json
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/p-norm.json
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/symmetry.json
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/structural/volume.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.931571 esse-2022.9.6.post0/example/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.963574 esse-2022.9.6.post0/example/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/workflow/convergence/electronic.json
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/workflow/convergence/ionic.json
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/properties_directory/workflow/convergence/kpoint.json
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/property.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.963574 esse-2022.9.6.post0/example/software/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software/application.json
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software/executable.json
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software/flavor.json
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software/template.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.935571 esse-2022.9.6.post0/example/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.963574 esse-2022.9.6.post0/example/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/ml/exabyteml.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.931571 esse-2022.9.6.post0/example/software_directory/ml/unit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.963574 esse-2022.9.6.post0/example/software_directory/ml/unit/execution/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.963574 esse-2022.9.6.post0/example/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/ml/unit/execution/evaluate/cross-validate.json
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/ml/unit/execution/initialize.json
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/ml/unit/execution/score.json
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/ml/unit/execution/train.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.935571 esse-2022.9.6.post0/example/software_directory/ml/unit/processing/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.963574 esse-2022.9.6.post0/example/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/ml/unit/processing/data_transformation/manipulation.json
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/ml/unit/processing/feature_selection/filter_based.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/software_directory/modeling/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/modeling/espresso/arguments.json
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/modeling/espresso.json
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/modeling/nwchem.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/modeling/unit/execution.json
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/modeling/vasp.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/scripting/jupyter-lab.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/scripting/python.json
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/scripting/shell.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/software_directory/scripting/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/system/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/system/_material.json
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/system/_parent_job.json
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/system/_project.json
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/system/creator.json
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/system/entity_reference.json
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/system/file_source.json
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/system/message.json
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/system/owner.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/new_subworkflow.json
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/subworkflow.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/assignment.json
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/condition.json
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/input/_inputItemScope.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/io/api.json
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/io/db.json
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/io/object_storage.json
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/io.json
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/map.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/processing.json
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.967574 esse-2022.9.6.post0/example/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit/runtime/runtime_items.json
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow/unit.json
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/example/workflow.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.971574 esse-2022.9.6.post0/manifest/
--rw-r--r--   0 runner    (1001) docker     (121)     7807 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/manifest/dft_unit_functionals.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13108 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/manifest/functional_lookup_table.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     9551 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/manifest/models.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4773 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/manifest/properties.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/npmignore
--rw-r--r--   0 runner    (1001) docker     (121)   269461 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/package.json
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)      340 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/refactor.sh
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     1489 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/run-tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.971574 esse-2022.9.6.post0/schema/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.971574 esse-2022.9.6.post0/schema/core/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.971574 esse-2022.9.6.post0/schema/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/abstract/2d_data.json
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/abstract/2d_plot.json
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/abstract/3d_grid.json
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/abstract/3d_tensor.json
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/abstract/3d_vector_basis.json
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/abstract/point.json
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/abstract/vector.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.971574 esse-2022.9.6.post0/schema/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/1d_data_series.json
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/3d_lattice.json
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/array_of_3_booleans.json
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/array_of_3_numbers.json
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/array_of_ids.json
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/array_of_strings.json
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/axis.json
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/scalar.json
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/slugified_entry.json
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/slugified_entry_or_slug.json
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/primitive/string.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.971574 esse-2022.9.6.post0/schema/core/reference/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.971574 esse-2022.9.6.post0/schema/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reference/experiment/condition.json
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reference/experiment/location.json
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reference/experiment.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reference/literature/name.json
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reference/literature/pages.json
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reference/literature.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reference/modeling/exabyte.json
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reference/modeling.json
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reference.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/core/reusable/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reusable/atomic_scalars.json
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reusable/atomic_strings.json
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reusable/atomic_vectors.json
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reusable/band_gap.json
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reusable/energy.json
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reusable/file_metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/core/reusable/object_storage_container_data.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/definitions/
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/definitions/units.json
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/element.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/job/
--rw-r--r--   0 runner    (1001) docker     (121)     5299 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/job/compute.json
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/job.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/material/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/material/conventional.json
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/material.json
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/method.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/methods_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/local-orbital.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.935571 esse-2022.9.6.post0/schema/methods_directory/local_orbital/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/methods_directory/local_orbital/definitions/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/local_orbital/definitions/basis_sets.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/methods_directory/pseudopotential/
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/pseudopotential/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/methods_directory/pseudopotential/file/
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/pseudopotential/file/energy_cutoff.json
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/pseudopotential/file/exchange_correlation.json
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/pseudopotential/file/radii.json
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/pseudopotential/file.json
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/pseudopotential/precision.json
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/pseudopotential.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/methods_directory/regression/
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/regression/data.json
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/regression/data_per_feature.json
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/regression/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/methods_directory/regression/kernel_ridge/
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/regression/kernel_ridge/data_per_property.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/methods_directory/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/regression/linear/data_per_property.json
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/regression/precision.json
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/regression/precision_per_property.json
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/regression.json
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/methods_directory/unknown.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.975574 esse-2022.9.6.post0/schema/model/
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/model/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/model/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/model/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/model.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.979575 esse-2022.9.6.post0/schema/models_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.979575 esse-2022.9.6.post0/schema/models_directory/pb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.979575 esse-2022.9.6.post0/schema/models_directory/pb/qm/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.979575 esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.979575 esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/configuration_interaction/
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/configuration_interaction/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/configuration_interaction/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/configuration_interaction.json
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/abin.json
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.979575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/
--rw-r--r--   0 runner    (1001) docker     (121)    36659 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals.json
--rw-r--r--   0 runner    (1001) docker     (121)     8190 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_model.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.979575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.979575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.979575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/component.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.983575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/dispersion_correction.json
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_gga.json
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_mgga.json
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/local_functional_components.json
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.983575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.983575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.983575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/gga/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/gga/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/gga/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/gga/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/gga.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.983575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.983575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/lda/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/lda/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/lda/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/lda/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/lda.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.987575 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/mgga.json
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft.json
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/dft.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.987575 esse-2022.9.6.post0/schema/models_directory/pb/qm/semp/
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/semp/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/semp/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/semp/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/semp/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/semp.json
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb/qm.json
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/pb.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.987575 esse-2022.9.6.post0/schema/models_directory/st/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.987575 esse-2022.9.6.post0/schema/models_directory/st/det/
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/st/det/ml.json
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/st/det.json
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/st.json
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/models_directory/unknown.json
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/new_model.json
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/project.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.987575 esse-2022.9.6.post0/schema/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/derived_properties.json
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/electronic_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.987575 esse-2022.9.6.post0/schema/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/elemental/atomic_radius.json
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/elemental/electronegativity.json
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/elemental/ionization_potential.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.987575 esse-2022.9.6.post0/schema/properties_directory/non-scalar/
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/band_gaps.json
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/band_structure.json
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/charge_density_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)     2143 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/density_of_states.json
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/file_content.json
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/phonon_dispersions.json
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/phonon_dos.json
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/reaction_energy_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/stress_tensor.json
--rw-r--r--   0 runner    (1001) docker     (121)     6033 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/total_energy_contributions.json
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/non-scalar/vibrational_spectrum.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.991576 esse-2022.9.6.post0/schema/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/scalar/electron_affinity.json
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/scalar/fermi_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/scalar/formation_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/scalar/ionization_potential.json
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/scalar/pressure.json
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/scalar/reaction_energy_barrier.json
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/scalar/surface_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/scalar/total_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/scalar/total_force.json
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/scalar/zero_point_energy.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.991576 esse-2022.9.6.post0/schema/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/atomic_forces.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.991576 esse-2022.9.6.post0/schema/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/basis/atomic_constraints.json
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/basis/atomic_coordinate.json
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/basis/atomic_coordinates.json
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/basis/atomic_element.json
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/basis/bonds.json
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/basis.json
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/density.json
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/elemental_ratio.json
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/inchi.json
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/inchi_key.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.991576 esse-2022.9.6.post0/schema/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/lattice/lattice_bravais.json
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/lattice/lattice_vectors.json
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/lattice.json
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/magnetic_moments.json
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/molecular_pattern.json
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/p-norm.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.991576 esse-2022.9.6.post0/schema/properties_directory/structural/patterns/
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/patterns/functional_group.json
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/patterns/ring.json
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/patterns/special_bond.json
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/symmetry.json
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/structural/volume.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.935571 esse-2022.9.6.post0/schema/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.991576 esse-2022.9.6.post0/schema/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/workflow/convergence/electronic.json
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/workflow/convergence/ionic.json
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/properties_directory/workflow/convergence/kpoint.json
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/property.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.991576 esse-2022.9.6.post0/schema/software/
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software/application.json
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software/executable.json
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software/flavor.json
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software/template.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.939572 esse-2022.9.6.post0/schema/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.991576 esse-2022.9.6.post0/schema/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/exabyteml.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.991576 esse-2022.9.6.post0/schema/software_directory/ml/unit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.995576 esse-2022.9.6.post0/schema/software_directory/ml/unit/execution/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.995576 esse-2022.9.6.post0/schema/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/execution/initialize.json
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/execution/score.json
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/execution/train.json
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.995576 esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.995576 esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/data_transformation.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.995576 esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/feature_selection.json
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/ml/unit/processing.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.995576 esse-2022.9.6.post0/schema/software_directory/modeling/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.995576 esse-2022.9.6.post0/schema/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/modeling/espresso/arguments.json
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/modeling/espresso.json
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/modeling/nwchem.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.995576 esse-2022.9.6.post0/schema/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/modeling/unit/execution.json
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/modeling/vasp.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.995576 esse-2022.9.6.post0/schema/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/scripting/jupyter-lab.json
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/scripting/python.json
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/scripting/shell.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.995576 esse-2022.9.6.post0/schema/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/software_directory/scripting/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.999576 esse-2022.9.6.post0/schema/system/
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/_material.json
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/_parent_job.json
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/_project.json
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/bankable.json
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/bankable_entity.json
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/base_entity_set.json
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/creator.json
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/creator_account.json
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/database_source.json
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/defaultable.json
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/description_object.json
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/entity.json
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/entity_reference.json
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/file_source.json
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/history.json
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/is_multi_material.json
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/is_outdated.json
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/job_extended.json
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/message.json
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/name.json
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/owner.json
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/schema_version.json
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/scope.json
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/sharing.json
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/soft_removable.json
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/status.json
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/system_name.json
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/timestampable.json
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/unit_extended.json
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/system/use_values.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.999576 esse-2022.9.6.post0/schema/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/base_flow.json
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/new_subworkflow.json
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/subworkflow.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.999576 esse-2022.9.6.post0/schema/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/assertion.json
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/assignment.json
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/condition.json
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.999576 esse-2022.9.6.post0/schema/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/input/_input.json
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/input/_inputItem.json
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/input/_inputItemId.json
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/input/_inputItemScope.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.999576 esse-2022.9.6.post0/schema/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/io/api.json
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/io/db.json
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/io/object_storage.json
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/io.json
--rw-r--r--   0 runner    (1001) docker     (121)     2183 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/map.json
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/processing.json
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.999576 esse-2022.9.6.post0/schema/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/runtime/_runtime_item_full_object.json
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/runtime/_runtime_item_name_object.json
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/runtime/_runtime_item_string.json
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/runtime/runtime_item.json
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit/runtime/runtime_items.json
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow/unit.json
--rw-r--r--   0 runner    (1001) docker     (121)     2959 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/schema/workflow.json
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 13:58:37.063581 esse-2022.9.6.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.939572 esse-2022.9.6.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.939572 esse-2022.9.6.post0/src/js/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.003576 esse-2022.9.6.post0/src/js/esse/
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/js/esse/index.js
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/js/esse/settings.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.003576 esse-2022.9.6.post0/src/js/esse/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/js/esse/tests/validate.js
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/js/esse/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.003576 esse-2022.9.6.post0/src/js/json_include/
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/js/json_include/index.js
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/js/json_include/settings.js
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/js/json_include/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.003576 esse-2022.9.6.post0/src/js/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/js/scripts/setSchemaIds.mjs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.939572 esse-2022.9.6.post0/src/py/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.003576 esse-2022.9.6.post0/src/py/esse/
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-06 13:58:36.000000 esse-2022.9.6.post0/src/py/esse/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.943572 esse-2022.9.6.post0/src/py/esse/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.003576 esse-2022.9.6.post0/src/py/esse/data/example/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.003576 esse-2022.9.6.post0/src/py/esse/data/example/core/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.003576 esse-2022.9.6.post0/src/py/esse/data/example/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/abstract/2d_data.json
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/abstract/2d_plot.json
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/abstract/3d_grid.json
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/abstract/3d_tensor.json
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/abstract/3d_vector_basis.json
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/abstract/point.json
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/abstract/vector.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/primitive/1d_data_series.json
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/primitive/3d_lattice.json
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/primitive/array_of_3_booleans.json
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/primitive/array_of_3_numbers.json
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/primitive/array_of_ids.json
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/primitive/axis.json
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/primitive/scalar.json
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/primitive/string.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/experiment/condition.json
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/experiment/location.json
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/experiment.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/literature/name.json
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/literature/pages.json
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/literature.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/modeling/exabyte.json
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reference/modeling.json
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reference.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/core/reusable/
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reusable/atomic_vectors.json
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reusable/band_gap.json
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reusable/energy.json
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reusable/file_metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/core/reusable/object_storage_container_data.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/element.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/job/
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/job/compute.json
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/job.json
--rw-r--r--   0 runner    (1001) docker     (121)     2167 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/material.json
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/method.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/local-orbital.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/pseudopotential/
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/pseudopotential/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/energy_cutoff.json
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/exchange_correlation.json
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/radii.json
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/pseudopotential/file.json
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/pseudopotential/precision.json
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/pseudopotential.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression/data_per_feature.json
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.007577 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression/kernel_ridge/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression/kernel_ridge/data_per_property.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression/linear/data_per_property.json
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression/precision.json
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression/precision_per_property.json
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/model/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/model/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/model.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.939572 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.939572 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/abin/
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/abin/configuration_interaction.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/component.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/components_directory/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/gga/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/gga/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/mgga/
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/mgga/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft.json
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/semp.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.939572 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/st/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/st/det/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/models_directory/st/det/ml.json
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/new_model.json
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/project.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/electronic_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.011577 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/elemental/atomic_radius.json
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/elemental/electronegativity.json
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/elemental/ionization_potential.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.015577 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/band_gaps.json
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/band_structure.json
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/charge_density_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/density_of_states.json
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/file_content.json
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dispersions.json
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dos.json
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/reaction_energy_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/stress_tensor.json
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/total_energy_contributions.json
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/vibrational_spectrum.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.015577 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/electron_affinity.json
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/fermi_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/formation_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/ionization_potential.json
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/pressure.json
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/reaction_energy_barrier.json
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/surface_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/total_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/total_force.json
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/scalar/zero_point_energy.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.015577 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/atomic_forces.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.015577 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_constraints.json
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_coordinate.json
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_coordinates.json
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_element.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/basis/bonds.json
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/basis.json
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/density.json
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/elemental_ratio.json
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/inchi.json
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/inchi_key.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.015577 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/lattice/lattice_bravais.json
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/lattice/lattice_vectors.json
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/lattice.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/magnetic_moments.json
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/molecular_pattern.json
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/p-norm.json
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/symmetry.json
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/volume.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.943572 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/workflow/convergence/electronic.json
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/workflow/convergence/ionic.json
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/workflow/convergence/kpoint.json
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/property.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software/application.json
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software/executable.json
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software/flavor.json
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software/template.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.943572 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/exabyteml.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.943572 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/execution/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/execution/evaluate/cross-validate.json
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/execution/initialize.json
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/execution/score.json
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/execution/train.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.943572 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/processing/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/manipulation.json
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/processing/feature_selection/filter_based.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/modeling/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/modeling/espresso/arguments.json
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/modeling/espresso.json
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/modeling/nwchem.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/modeling/unit/execution.json
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/modeling/vasp.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/scripting/jupyter-lab.json
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/scripting/python.json
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/scripting/shell.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/software_directory/scripting/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/system/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/system/_material.json
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/system/_parent_job.json
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/system/_project.json
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/system/creator.json
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/system/entity_reference.json
--rw-r--r--   0 runner    (1001) docker     (121)      620 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/system/file_source.json
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/system/message.json
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/system/owner.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.019578 esse-2022.9.6.post0/src/py/esse/data/example/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/new_subworkflow.json
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/subworkflow.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.023578 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/assignment.json
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/condition.json
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.023578 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/input/_inputItemScope.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.023578 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/io/api.json
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/io/db.json
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/io/object_storage.json
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/io.json
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/map.json
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/processing.json
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.023578 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/runtime/runtime_items.json
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit.json
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/example/workflow.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.023578 esse-2022.9.6.post0/src/py/esse/data/manifest/
--rw-r--r--   0 runner    (1001) docker     (121)     7807 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/manifest/dft_unit_functionals.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13108 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/manifest/functional_lookup_table.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     9551 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/manifest/models.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4773 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/manifest/properties.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.023578 esse-2022.9.6.post0/src/py/esse/data/schema/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.023578 esse-2022.9.6.post0/src/py/esse/data/schema/core/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.023578 esse-2022.9.6.post0/src/py/esse/data/schema/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/abstract/2d_data.json
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/abstract/2d_plot.json
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/abstract/3d_grid.json
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/abstract/3d_tensor.json
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/abstract/3d_vector_basis.json
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/abstract/point.json
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/abstract/vector.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.027578 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/1d_data_series.json
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/3d_lattice.json
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/array_of_3_booleans.json
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/array_of_3_numbers.json
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/array_of_ids.json
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/array_of_strings.json
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/axis.json
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/scalar.json
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/slugified_entry.json
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/slugified_entry_or_slug.json
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/string.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.027578 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.027578 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/experiment/condition.json
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/experiment/location.json
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/experiment.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.027578 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/literature/name.json
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/literature/pages.json
--rw-r--r--   0 runner    (1001) docker     (121)     2745 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/literature.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.027578 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/modeling/exabyte.json
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/modeling.json
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reference.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.027578 esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/atomic_scalars.json
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/atomic_strings.json
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/atomic_vectors.json
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/band_gap.json
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/energy.json
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/file_metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/object_storage_container_data.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.027578 esse-2022.9.6.post0/src/py/esse/data/schema/definitions/
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/definitions/units.json
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/element.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.027578 esse-2022.9.6.post0/src/py/esse/data/schema/job/
--rw-r--r--   0 runner    (1001) docker     (121)     5299 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/job/compute.json
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/job.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.027578 esse-2022.9.6.post0/src/py/esse/data/schema/material/
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/material/conventional.json
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/material.json
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/method.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.027578 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/local-orbital.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.943572 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/local_orbital/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.031579 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/basis_sets.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.031579 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/
--rw-r--r--   0 runner    (1001) docker     (121)     1926 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.031579 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/energy_cutoff.json
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/exchange_correlation.json
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/radii.json
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file.json
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/precision.json
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.031579 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/data.json
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/data_per_feature.json
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.031579 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/data_per_property.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.031579 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/linear/data_per_property.json
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/precision.json
--rw-r--r--   0 runner    (1001) docker     (121)      521 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/precision_per_property.json
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression.json
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/unknown.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.031579 esse-2022.9.6.post0/src/py/esse/data/schema/model/
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/model/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/model/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/model/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/model.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.031579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.031579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.035579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.035579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.035579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      630 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction.json
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin.json
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.035579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/
--rw-r--r--   0 runner    (1001) docker     (121)    36659 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals.json
--rw-r--r--   0 runner    (1001) docker     (121)     8190 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_model.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.039579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.039579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/
--rw-r--r--   0 runner    (1001) docker     (121)      530 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json
--rw-r--r--   0 runner    (1001) docker     (121)      531 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
--rw-r--r--   0 runner    (1001) docker     (121)      823 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.039579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/
--rw-r--r--   0 runner    (1001) docker     (121)      631 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/component.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.039579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/dispersion_correction.json
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_gga.json
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_mgga.json
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/local_functional_components.json
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.043579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.043579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      712 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.043579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.043579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.043579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      669 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.043579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/functional.json
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga.json
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft.json
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.043579 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/definitions.json
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (121)      398 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/semp.json
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm.json
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.047580 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/st/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.047580 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/st/det/
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/st/det/ml.json
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/st/det.json
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/st.json
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/unknown.json
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/new_model.json
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/project.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.047580 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/derived_properties.json
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/electronic_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.047580 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/elemental/atomic_radius.json
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/elemental/electronegativity.json
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/elemental/ionization_potential.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.047580 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_gaps.json
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_structure.json
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/charge_density_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)     2143 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/density_of_states.json
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/file_content.json
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dispersions.json
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dos.json
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/reaction_energy_profile.json
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/stress_tensor.json
--rw-r--r--   0 runner    (1001) docker     (121)     6033 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/total_energy_contributions.json
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/vibrational_spectrum.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.051580 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/electron_affinity.json
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/fermi_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/formation_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/ionization_potential.json
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/pressure.json
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/reaction_energy_barrier.json
--rw-r--r--   0 runner    (1001) docker     (121)      381 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/surface_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/total_energy.json
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/total_force.json
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/scalar/zero_point_energy.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.051580 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/atomic_forces.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.051580 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_constraints.json
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinate.json
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinates.json
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_element.json
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis/bonds.json
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis.json
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/density.json
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/elemental_ratio.json
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/inchi.json
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/inchi_key.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.051580 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_bravais.json
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_vectors.json
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/lattice.json
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/magnetic_moments.json
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/molecular_pattern.json
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/p-norm.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.051580 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/patterns/
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/patterns/functional_group.json
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/patterns/ring.json
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/patterns/special_bond.json
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/symmetry.json
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/volume.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.947572 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.051580 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/electronic.json
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/ionic.json
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/kpoint.json
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/property.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.051580 esse-2022.9.6.post0/src/py/esse/data/schema/software/
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software/application.json
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software/executable.json
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software/flavor.json
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software/template.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:36.947572 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.051580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/exabyteml.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.051580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.055580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.055580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json
--rw-r--r--   0 runner    (1001) docker     (121)      996 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/initialize.json
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/score.json
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/train.json
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.055580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.055580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.055580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection.json
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.055580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.055580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (121)     2456 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/espresso/arguments.json
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/espresso.json
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/nwchem.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.055580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/unit/execution.json
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/vasp.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.055580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (121)      783 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/scripting/jupyter-lab.json
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/scripting/python.json
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/scripting/shell.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.055580 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/scripting/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.059581 esse-2022.9.6.post0/src/py/esse/data/schema/system/
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/_material.json
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/_parent_job.json
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/_project.json
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/bankable.json
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/bankable_entity.json
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/base_entity_set.json
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/creator.json
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/creator_account.json
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/database_source.json
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/defaultable.json
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/description_object.json
--rw-r--r--   0 runner    (1001) docker     (121)     1294 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/entity.json
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/entity_reference.json
--rw-r--r--   0 runner    (1001) docker     (121)      780 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/file_source.json
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/history.json
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/is_multi_material.json
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/is_outdated.json
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/job_extended.json
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/message.json
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/name.json
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/owner.json
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/schema_version.json
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/scope.json
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/sharing.json
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/soft_removable.json
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/status.json
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/system_name.json
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/tags.json
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/timestampable.json
--rw-r--r--   0 runner    (1001) docker     (121)      283 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/unit_extended.json
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/system/use_values.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.059581 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/base_flow.json
--rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/new_subworkflow.json
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/subworkflow.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.059581 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/assertion.json
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/assignment.json
--rw-r--r--   0 runner    (1001) docker     (121)     1407 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/condition.json
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.059581 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/input/_input.json
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/input/_inputItem.json
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemId.json
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemScope.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.059581 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/io/api.json
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/io/db.json
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/io/object_storage.json
--rw-r--r--   0 runner    (1001) docker     (121)     1137 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/io.json
--rw-r--r--   0 runner    (1001) docker     (121)     2183 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/map.json
--rw-r--r--   0 runner    (1001) docker     (121)      875 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/processing.json
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.063581 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_full_object.json
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_name_object.json
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_string.json
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_item.json
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_items.json
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit.json
--rw-r--r--   0 runner    (1001) docker     (121)     2959 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/data/schema/workflow.json
--rw-r--r--   0 runner    (1001) docker     (121)     1348 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/functionals.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.063581 esse-2022.9.6.post0/src/py/esse/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/tests/validate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2878 2022-09-06 13:58:12.000000 esse-2022.9.6.post0/src/py/esse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:58:37.003576 esse-2022.9.6.post0/src/py/esse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5489 2022-09-06 13:58:36.000000 esse-2022.9.6.post0/src/py/esse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    54571 2022-09-06 13:58:36.000000 esse-2022.9.6.post0/src/py/esse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 13:58:36.000000 esse-2022.9.6.post0/src/py/esse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-09-06 13:58:36.000000 esse-2022.9.6.post0/src/py/esse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-09-06 13:58:36.000000 esse-2022.9.6.post0/src/py/esse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-06 13:58:36.000000 esse-2022.9.6.post0/src/py/esse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.221775 esse-2023.5.29.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/.eslintrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.057772 esse-2023.5.29.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.093773 esse-2023.5.29.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-29 23:51:50.221775 esse-2023.5.29.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/build_schemas.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.093773 esse-2023.5.29.post0/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.093773 esse-2023.5.29.post0/example/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.093773 esse-2023.5.29.post0/example/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/abstract/2d_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/abstract/2d_plot.json
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/abstract/3d_grid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/abstract/3d_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/abstract/3d_vector_basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/abstract/point.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/abstract/vector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/primitive/1d_data_series.json
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/primitive/3d_lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/primitive/array_of_3_booleans.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/primitive/array_of_3_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/primitive/array_of_ids.json
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/primitive/axis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/primitive/scalar.json
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/primitive/string.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/core/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reference/experiment/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reference/experiment/location.json
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reference/experiment.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reference/literature/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reference/literature/pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reference/literature.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reference/modeling/exabyte.json
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reference/modeling.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reference.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/core/reusable/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reusable/atomic_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reusable/band_gap.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reusable/energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reusable/file_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/core/reusable/object_storage_container_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/element.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/job/compute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/job.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/method.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/methods_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/local-orbital.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/methods_directory/pseudopotential/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/pseudopotential/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/methods_directory/pseudopotential/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/pseudopotential/file/energy_cutoff.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/pseudopotential/file/exchange_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/pseudopotential/file/radii.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/pseudopotential/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/pseudopotential/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/pseudopotential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.097773 esse-2023.5.29.post0/example/methods_directory/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/regression/data_per_feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/regression/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/methods_directory/regression/kernel_ridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/regression/kernel_ridge/data_per_property.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/methods_directory/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/regression/linear/data_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/regression/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/regression/precision_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/methods_directory/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/model/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.069772 esse-2023.5.29.post0/example/models_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.065772 esse-2023.5.29.post0/example/models_directory/pb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/abin/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/abin/configuration_interaction.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/functional/component.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/functional/components_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/gga/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/gga/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/lda/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/lda/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/lda.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/mgga/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/mgga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/pb/qm/semp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.069772 esse-2023.5.29.post0/example/models_directory/st/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/models_directory/st/det/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/models_directory/st/det/ml.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/new_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/project.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/electronic_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.101773 esse-2023.5.29.post0/example/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/elemental/atomic_radius.json
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/elemental/electronegativity.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/elemental/ionization_potential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.105773 esse-2023.5.29.post0/example/properties_directory/non-scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/band_gaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/band_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/charge_density_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/density_of_states.json
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/file_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/phonon_dispersions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/phonon_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/reaction_energy_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/stress_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/total_energy_contributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/non-scalar/vibrational_spectrum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.105773 esse-2023.5.29.post0/example/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/electron_affinity.json
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/fermi_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/formation_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/ionization_potential.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/pressure.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/reaction_energy_barrier.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/surface_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/total_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/total_force.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/valence_band_offset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/scalar/zero_point_energy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.105773 esse-2023.5.29.post0/example/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/atomic_forces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/basis/atomic_constraints.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/basis/atomic_coordinate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/basis/atomic_coordinates.json
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/basis/atomic_element.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/basis/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/density.json
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/elemental_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/inchi.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/inchi_key.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/lattice/lattice_bravais.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/lattice/lattice_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/magnetic_moments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/molecular_pattern.json
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/p-norm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/symmetry.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/structural/volume.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.073773 esse-2023.5.29.post0/example/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/workflow/convergence/electronic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/workflow/convergence/ionic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/properties_directory/workflow/convergence/kpoint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/property/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/property/best.json
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/property/raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/property/refined.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software/executable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software/flavor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.073773 esse-2023.5.29.post0/example/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/ml/exabyteml.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.073773 esse-2023.5.29.post0/example/software_directory/ml/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software_directory/ml/unit/execution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/ml/unit/execution/evaluate/cross-validate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/ml/unit/execution/initialize.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/ml/unit/execution/score.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/ml/unit/execution/train.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.073773 esse-2023.5.29.post0/example/software_directory/ml/unit/processing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/ml/unit/processing/data_transformation/manipulation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/ml/unit/processing/feature_selection/filter_based.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software_directory/modeling/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/modeling/espresso/arguments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/modeling/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/modeling/nwchem.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/modeling/unit/execution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/modeling/vasp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/scripting/jupyter-lab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/scripting/python.json
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/scripting/shell.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/software_directory/scripting/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.109773 esse-2023.5.29.post0/example/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/system/_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/system/_parent_job.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/system/_project.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/system/creator.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/system/entity_reference.json
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/system/file_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/system/message.json
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/system/owner.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.113773 esse-2023.5.29.post0/example/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/new_subworkflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/subworkflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.113773 esse-2023.5.29.post0/example/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/assignment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.113773 esse-2023.5.29.post0/example/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/input/_inputItemScope.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.113773 esse-2023.5.29.post0/example/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/io/api.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/io/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/io/object_storage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/io.json
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.113773 esse-2023.5.29.post0/example/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit/runtime/runtime_items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow/unit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/example/workflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.113773 esse-2023.5.29.post0/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/manifest/dft_unit_functionals.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/manifest/functional_lookup_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/manifest/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/manifest/properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/npmignore
+-rw-r--r--   0 runner    (1001) docker     (123)   269811 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      340 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/refactor.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/run-tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.113773 esse-2023.5.29.post0/schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.113773 esse-2023.5.29.post0/schema/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.117773 esse-2023.5.29.post0/schema/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/abstract/2d_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/abstract/2d_plot.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/abstract/3d_grid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/abstract/3d_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/abstract/3d_vector_basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/abstract/point.json
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/abstract/vector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.117773 esse-2023.5.29.post0/schema/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/1d_data_series.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/3d_lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/array_of_3_booleans.json
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/array_of_3_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/array_of_ids.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/array_of_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/array_of_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/axis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/scalar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/slugified_entry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/slugified_entry_or_slug.json
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/primitive/string.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.117773 esse-2023.5.29.post0/schema/core/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reference/exabyte.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.117773 esse-2023.5.29.post0/schema/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reference/experiment/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reference/experiment/location.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reference/experiment.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.117773 esse-2023.5.29.post0/schema/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reference/literature/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reference/literature/pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reference/literature.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.117773 esse-2023.5.29.post0/schema/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reference/modeling/exabyte.json
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reference/modeling.json
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reference.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.117773 esse-2023.5.29.post0/schema/core/reusable/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reusable/atomic_scalars.json
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reusable/atomic_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reusable/atomic_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reusable/band_gap.json
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reusable/energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reusable/file_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/core/reusable/object_storage_container_data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.117773 esse-2023.5.29.post0/schema/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/definitions/units.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/element.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/in_memory_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/in_memory_entity/base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/in_memory_entity/defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/in_memory_entity/named.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/in_memory_entity/named_defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/in_memory_entity/named_defaultable_has_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/in_memory_entity/named_defaultable_runtime_items.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/job/compute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/job.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/material/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/material/conventional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/method.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/methods_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/local-orbital.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.077772 esse-2023.5.29.post0/schema/methods_directory/local_orbital/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/methods_directory/local_orbital/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/local_orbital/definitions/basis_sets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/methods_directory/pseudopotential/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/pseudopotential/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/methods_directory/pseudopotential/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/pseudopotential/file/energy_cutoff.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/pseudopotential/file/exchange_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/pseudopotential/file/radii.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/pseudopotential/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/pseudopotential/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/pseudopotential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/methods_directory/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/regression/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/regression/data_per_feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/regression/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/methods_directory/regression/kernel_ridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/regression/kernel_ridge/data_per_property.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/methods_directory/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/regression/linear/data_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/regression/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/regression/precision_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/methods_directory/unknown.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/model/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/model/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/model/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.121773 esse-2023.5.29.post0/schema/models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.125773 esse-2023.5.29.post0/schema/models_directory/pb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.125773 esse-2023.5.29.post0/schema/models_directory/pb/qm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.125773 esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.125773 esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/configuration_interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/configuration_interaction/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/configuration_interaction/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/configuration_interaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.125773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)    36659 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.125773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.125773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.125773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/component.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.129773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/dispersion_correction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_gga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_mgga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/local_functional_components.json
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.129773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.129773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.129773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/gga/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/gga/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/gga/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/gga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/gga.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.129773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.133773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/lda/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/lda/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/lda/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/lda/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/lda.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.133773 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/mgga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/dft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.133773 esse-2023.5.29.post0/schema/models_directory/pb/qm/semp/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/semp/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/semp/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/semp/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/semp/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/semp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb/qm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/pb.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.133773 esse-2023.5.29.post0/schema/models_directory/st/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.133773 esse-2023.5.29.post0/schema/models_directory/st/det/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/st/det/ml.json
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/st/det.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/st.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/models_directory/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/new_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/project.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.133773 esse-2023.5.29.post0/schema/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/derived_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/electronic_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.133773 esse-2023.5.29.post0/schema/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/elemental/atomic_radius.json
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/elemental/electronegativity.json
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/elemental/ionization_potential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.137774 esse-2023.5.29.post0/schema/properties_directory/non-scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/average_potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/band_gaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/band_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/charge_density_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/density_of_states.json
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/file_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/phonon_dispersions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/phonon_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/reaction_energy_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/stress_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/total_energy_contributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/non-scalar/vibrational_spectrum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.137774 esse-2023.5.29.post0/schema/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/electron_affinity.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/fermi_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/formation_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/ionization_potential.json
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/pressure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/reaction_energy_barrier.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/surface_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/total_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/total_force.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/valence_band_offset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/scalar/zero_point_energy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.137774 esse-2023.5.29.post0/schema/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/atomic_forces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.137774 esse-2023.5.29.post0/schema/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/basis/atomic_constraints.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/basis/atomic_coordinate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/basis/atomic_coordinates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/basis/atomic_element.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/basis/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/density.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/elemental_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/inchi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/inchi_key.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.137774 esse-2023.5.29.post0/schema/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/lattice/lattice_bravais.json
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/lattice/lattice_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/magnetic_moments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/molecular_pattern.json
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/p-norm.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/properties_directory/structural/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/patterns/functional_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/patterns/ring.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/patterns/special_bond.json
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/symmetry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/structural/volume.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.077772 esse-2023.5.29.post0/schema/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/workflow/convergence/electronic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/workflow/convergence/ionic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/properties_directory/workflow/convergence/kpoint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/property/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/property/best.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/property/raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/property/refined.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/property/source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software/executable.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software/flavor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.081773 esse-2023.5.29.post0/schema/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/exabyteml.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/ml/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/ml/unit/execution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/execution/initialize.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/execution/score.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/execution/train.json
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/data_transformation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/feature_selection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/ml/unit/processing.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/modeling/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/modeling/espresso/arguments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/modeling/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/modeling/nwchem.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/modeling/unit/execution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/modeling/vasp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.141774 esse-2023.5.29.post0/schema/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/scripting/jupyter-lab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/scripting/python.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/scripting/shell.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.145774 esse-2023.5.29.post0/schema/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/software_directory/scripting/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.145774 esse-2023.5.29.post0/schema/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/_parent_job.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/_project.json
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/bankable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/creator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/creator_account.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/database_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/entity_reference.json
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/file_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/history.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/in_set.json
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/is_multi_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/is_outdated.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/job_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/message.json
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/owner.json
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/schema_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/scope.json
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/set.json
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/sharing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/soft_removable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/status.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/timestampable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/system/use_values.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.149774 esse-2023.5.29.post0/schema/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/base_flow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/new_subworkflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/subworkflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.149774 esse-2023.5.29.post0/schema/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/assertion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/assignment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.149774 esse-2023.5.29.post0/schema/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/input/_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/input/_inputItem.json
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/input/_inputItemId.json
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/input/_inputItemScope.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.149774 esse-2023.5.29.post0/schema/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/io/api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/io/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/io/object_storage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/io.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.149774 esse-2023.5.29.post0/schema/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/runtime/_runtime_item_full_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/runtime/_runtime_item_name_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/runtime/_runtime_item_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/runtime/runtime_item.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit/runtime/runtime_items.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow/unit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/schema/workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:51:50.221775 esse-2023.5.29.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.081773 esse-2023.5.29.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.081773 esse-2023.5.29.post0/src/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.149774 esse-2023.5.29.post0/src/js/esse/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/js/esse/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/js/esse/settings.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.149774 esse-2023.5.29.post0/src/js/esse/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/js/esse/tests/validate.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/js/esse/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.149774 esse-2023.5.29.post0/src/js/json_include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/js/json_include/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/js/json_include/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/js/json_include/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.149774 esse-2023.5.29.post0/src/js/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/js/scripts/setSchemaIds.mjs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.081773 esse-2023.5.29.post0/src/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.149774 esse-2023.5.29.post0/src/py/esse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-29 23:51:49.000000 esse-2023.5.29.post0/src/py/esse/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.085773 esse-2023.5.29.post0/src/py/esse/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.153774 esse-2023.5.29.post0/src/py/esse/data/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.153774 esse-2023.5.29.post0/src/py/esse/data/example/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.153774 esse-2023.5.29.post0/src/py/esse/data/example/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/abstract/2d_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/abstract/2d_plot.json
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/abstract/3d_grid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/abstract/3d_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/abstract/3d_vector_basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/abstract/point.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/abstract/vector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.157774 esse-2023.5.29.post0/src/py/esse/data/example/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/primitive/1d_data_series.json
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/primitive/3d_lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/primitive/array_of_3_booleans.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/primitive/array_of_3_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/primitive/array_of_ids.json
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/primitive/axis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/primitive/scalar.json
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/primitive/string.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.157774 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.157774 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/experiment/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/experiment/location.json
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/experiment.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.157774 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/literature/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/literature/pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/literature.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.157774 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/modeling/exabyte.json
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reference/modeling.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reference.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.157774 esse-2023.5.29.post0/src/py/esse/data/example/core/reusable/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reusable/atomic_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reusable/band_gap.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reusable/energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reusable/file_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/core/reusable/object_storage_container_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/element.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.157774 esse-2023.5.29.post0/src/py/esse/data/example/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/job/compute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/job.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/method.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.157774 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/local-orbital.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.157774 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/pseudopotential/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/pseudopotential/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/energy_cutoff.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/exchange_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/radii.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/pseudopotential/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/pseudopotential/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/pseudopotential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression/data_per_feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression/kernel_ridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression/kernel_ridge/data_per_property.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression/linear/data_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression/precision_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/model/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.085773 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.081773 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/abin/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/abin/configuration_interaction.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/component.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/components_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.161774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.165774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/gga/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/gga/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.165774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.165774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.165774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/mgga/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/mgga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/semp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.085773 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/st/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.165774 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/st/det/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/models_directory/st/det/ml.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/new_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/project.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.165774 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/electronic_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.165774 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/elemental/atomic_radius.json
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/elemental/electronegativity.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/elemental/ionization_potential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.165774 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/band_gaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/band_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/charge_density_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/density_of_states.json
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/file_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dispersions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/reaction_energy_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/stress_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/total_energy_contributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/vibrational_spectrum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.169774 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/electron_affinity.json
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/fermi_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/formation_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/ionization_potential.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/pressure.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/reaction_energy_barrier.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/surface_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/total_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/total_force.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/valence_band_offset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/scalar/zero_point_energy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.169774 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/atomic_forces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.169774 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_constraints.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_coordinate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_coordinates.json
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_element.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/basis/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/density.json
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/elemental_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/inchi.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/inchi_key.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/lattice/lattice_bravais.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/lattice/lattice_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/magnetic_moments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/molecular_pattern.json
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/p-norm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/symmetry.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/volume.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.085773 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/workflow/convergence/electronic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/workflow/convergence/ionic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/workflow/convergence/kpoint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/property/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/property/best.json
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/property/raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/property/refined.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software/executable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software/flavor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.085773 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/exabyteml.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.085773 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/execution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/execution/evaluate/cross-validate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/execution/initialize.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/execution/score.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/execution/train.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.085773 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/processing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/manipulation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/processing/feature_selection/filter_based.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/modeling/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/modeling/espresso/arguments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/modeling/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/modeling/nwchem.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/modeling/unit/execution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/modeling/vasp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/scripting/jupyter-lab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/scripting/python.json
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/scripting/shell.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.173774 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/software_directory/scripting/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.177774 esse-2023.5.29.post0/src/py/esse/data/example/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/system/_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/system/_parent_job.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/system/_project.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/system/creator.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/system/entity_reference.json
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/system/file_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/system/message.json
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/system/owner.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.177774 esse-2023.5.29.post0/src/py/esse/data/example/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/new_subworkflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/subworkflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.177774 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/assignment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.177774 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/input/_inputItemScope.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.177774 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/io/api.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/io/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/io/object_storage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/io.json
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.177774 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/runtime/runtime_items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/example/workflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.177774 esse-2023.5.29.post0/src/py/esse/data/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/manifest/dft_unit_functionals.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/manifest/functional_lookup_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/manifest/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/manifest/properties.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.181774 esse-2023.5.29.post0/src/py/esse/data/schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.181774 esse-2023.5.29.post0/src/py/esse/data/schema/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.181774 esse-2023.5.29.post0/src/py/esse/data/schema/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/abstract/2d_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/abstract/2d_plot.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/abstract/3d_grid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/abstract/3d_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/abstract/3d_vector_basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/abstract/point.json
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/abstract/vector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.181774 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/1d_data_series.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/3d_lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/array_of_3_booleans.json
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/array_of_3_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/array_of_ids.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/array_of_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/array_of_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/axis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/scalar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/slugified_entry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/slugified_entry_or_slug.json
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/string.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.181774 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/exabyte.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.181774 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/experiment/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/experiment/location.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/experiment.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.181774 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/literature/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/literature/pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/literature.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.181774 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/modeling/exabyte.json
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/modeling.json
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reference.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/atomic_scalars.json
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/atomic_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/atomic_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/band_gap.json
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/file_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/object_storage_container_data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/definitions/units.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/element.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/in_memory_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/in_memory_entity/base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/in_memory_entity/defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/in_memory_entity/named.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/in_memory_entity/named_defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/in_memory_entity/named_defaultable_has_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/in_memory_entity/named_defaultable_runtime_items.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/job/compute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/job.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/material/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/material/conventional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/method.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/local-orbital.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.085773 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/local_orbital/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/basis_sets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/energy_cutoff.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/exchange_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/radii.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/data_per_feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/data_per_property.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.185774 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/linear/data_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/precision_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/unknown.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.189774 esse-2023.5.29.post0/src/py/esse/data/schema/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/model/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/model/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/model/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.189774 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.189774 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.189774 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.189774 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.189774 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.189774 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)    36659 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.189774 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.189774 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.189774 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/component.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.193775 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/dispersion_correction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_gga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_mgga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/local_functional_components.json
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.193775 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.193775 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.193775 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.193775 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.197775 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.197775 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.197775 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/semp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.197775 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/st/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.197775 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/st/det/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/st/det/ml.json
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/st/det.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/st.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/new_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/project.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.197775 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/derived_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/electronic_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.197775 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/elemental/atomic_radius.json
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/elemental/electronegativity.json
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/elemental/ionization_potential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.197775 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/average_potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_gaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/charge_density_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/density_of_states.json
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/file_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dispersions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/reaction_energy_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/stress_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/total_energy_contributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/vibrational_spectrum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.201775 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/electron_affinity.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/fermi_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/formation_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/ionization_potential.json
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/pressure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/reaction_energy_barrier.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/surface_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/total_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/total_force.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/valence_band_offset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/scalar/zero_point_energy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.201775 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/atomic_forces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.201775 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_constraints.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_element.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/density.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/elemental_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/inchi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/inchi_key.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.201775 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_bravais.json
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/magnetic_moments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/molecular_pattern.json
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/p-norm.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.201775 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/patterns/functional_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/patterns/ring.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/patterns/special_bond.json
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/symmetry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/volume.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.089773 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.201775 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/electronic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/ionic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/kpoint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.201775 esse-2023.5.29.post0/src/py/esse/data/schema/property/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/property/best.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/property/raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/property/refined.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/property/source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.201775 esse-2023.5.29.post0/src/py/esse/data/schema/software/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software/executable.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software/flavor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.089773 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/exabyteml.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/initialize.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/score.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/train.json
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/espresso/arguments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/nwchem.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/unit/execution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/vasp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/scripting/jupyter-lab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/scripting/python.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/scripting/shell.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.205775 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/scripting/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.213775 esse-2023.5.29.post0/src/py/esse/data/schema/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/_parent_job.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/_project.json
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/bankable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/creator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/creator_account.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/database_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/entity_reference.json
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/file_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/history.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/in_set.json
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/is_multi_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/is_outdated.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/job_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/message.json
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/owner.json
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/schema_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/scope.json
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/set.json
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/sharing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/soft_removable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/status.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/timestampable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/system/use_values.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.213775 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/base_flow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/new_subworkflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/subworkflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.217775 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/assertion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/assignment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.217775 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/input/_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/input/_inputItem.json
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemId.json
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemScope.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.217775 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/io/api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/io/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/io/object_storage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/io.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.221775 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_full_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_name_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_item.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_items.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/data/schema/workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/functionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.221775 esse-2023.5.29.post0/src/py/esse/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/tests/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-29 23:51:29.000000 esse-2023.5.29.post0/src/py/esse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:51:50.153774 esse-2023.5.29.post0/src/py/esse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-29 23:51:49.000000 esse-2023.5.29.post0/src/py/esse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    55948 2023-05-29 23:51:50.000000 esse-2023.5.29.post0/src/py/esse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:51:49.000000 esse-2023.5.29.post0/src/py/esse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-29 23:51:49.000000 esse-2023.5.29.post0/src/py/esse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 23:51:49.000000 esse-2023.5.29.post0/src/py/esse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 23:51:49.000000 esse-2023.5.29.post0/src/py/esse.egg-info/top_level.txt
```

### Comparing `esse-2022.9.6.post0/.github/workflows/cicd.yml` & `esse-2023.5.29.post0/.github/workflows/cicd.yml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}
   cancel-in-progress: true
 
 jobs:
 
   run-py-tests:
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
     strategy:
       matrix:
         python-version: [3.6, 3.7, 3.8]
 
     steps:
       - name: Checkout this repository
         uses: actions/checkout@v2
@@ -48,14 +48,19 @@
       - name: Checkout actions repository
         uses: actions/checkout@v2
         with:
           repository: Exabyte-io/actions
           token: ${{ secrets.BOT_GITHUB_TOKEN }}
           path: actions
 
+      - name: Run JS validate
+        uses: ./actions/js/validate
+        with:
+          node-version: '14.x'
+      
       - name: Run JS tests
         uses: ./actions/js/test
         with:
           node-version: ${{ matrix.node-version }}
 
   publish-js-package:
     needs: [run-py-tests, run-js-tests]
```

### Comparing `esse-2022.9.6.post0/.gitignore` & `esse-2023.5.29.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/LICENSE.md` & `esse-2023.5.29.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/PKG-INFO` & `esse-2023.5.29.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esse
-Version: 2022.9.6.post0
+Version: 2023.5.29.post0
 Summary: Exabyte Source of Schemas and Examples
 Home-page: https://github.com/Exabyte-io/exabyte-esse
 Author: Exabyte Inc.
 Author-email: info@exabyte.io
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `esse-2022.9.6.post0/README.md` & `esse-2023.5.29.post0/README.md`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/job/compute.json` & `esse-2023.5.29.post0/example/job/compute.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/job.json` & `esse-2023.5.29.post0/example/job.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/material.json` & `esse-2023.5.29.post0/example/material.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/methods_directory/pseudopotential/file.json` & `esse-2023.5.29.post0/example/methods_directory/pseudopotential/file.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/methods_directory/regression.json` & `esse-2023.5.29.post0/example/methods_directory/regression.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/models_directory/pb/qm/abin/configuration_interaction.json` & `esse-2023.5.29.post0/example/models_directory/pb/qm/abin/configuration_interaction.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json` & `esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json` & `esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json` & `esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json` & `esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft/lda.json` & `esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft/lda.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/models_directory/pb/qm/dft/ksdft.json` & `esse-2023.5.29.post0/example/models_directory/pb/qm/dft/ksdft.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/properties_directory/non-scalar/band_structure.json` & `esse-2023.5.29.post0/example/properties_directory/non-scalar/band_structure.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/properties_directory/non-scalar/density_of_states.json` & `esse-2023.5.29.post0/example/properties_directory/non-scalar/density_of_states.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/properties_directory/non-scalar/phonon_dispersions.json` & `esse-2023.5.29.post0/example/properties_directory/non-scalar/phonon_dispersions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/properties_directory/non-scalar/phonon_dos.json` & `esse-2023.5.29.post0/example/properties_directory/non-scalar/phonon_dos.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/properties_directory/non-scalar/potential_profile.json` & `esse-2023.5.29.post0/example/properties_directory/non-scalar/potential_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/properties_directory/non-scalar/reaction_energy_profile.json` & `esse-2023.5.29.post0/example/properties_directory/non-scalar/reaction_energy_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/properties_directory/non-scalar/total_energy_contributions.json` & `esse-2023.5.29.post0/example/properties_directory/non-scalar/total_energy_contributions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/properties_directory/structural/molecular_pattern.json` & `esse-2023.5.29.post0/example/properties_directory/structural/molecular_pattern.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/software_directory/ml/unit/execution/train.json` & `esse-2023.5.29.post0/example/software_directory/ml/unit/execution/train.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json` & `esse-2023.5.29.post0/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/system/file_source.json` & `esse-2023.5.29.post0/example/system/file_source.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/workflow/unit/execution.json` & `esse-2023.5.29.post0/example/workflow/unit/execution.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/workflow/unit/io/api.json` & `esse-2023.5.29.post0/example/workflow/unit/io/api.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/workflow/unit/io.json` & `esse-2023.5.29.post0/example/workflow/unit/io.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/example/workflow.json` & `esse-2023.5.29.post0/example/workflow.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/manifest/dft_unit_functionals.yaml` & `esse-2023.5.29.post0/manifest/dft_unit_functionals.yaml`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/manifest/functional_lookup_table.yaml` & `esse-2023.5.29.post0/manifest/functional_lookup_table.yaml`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/manifest/models.yaml` & `esse-2023.5.29.post0/manifest/models.yaml`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/manifest/properties.yaml` & `esse-2023.5.29.post0/manifest/properties.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,239 +1,255 @@
 convergence_ionic:
   defaults:
     units: eV
-  schemaId: properties-directory-workflow-convergence-ionic
+  schemaId: properties-directory/workflow/convergence/ionic 
   isMonitor: true
 
 convergence_electronic:
   defaults:
     units: eV
-  schemaId: properties-directory-workflow-convergence-electronic
+  schemaId: properties-directory/workflow/convergence/electronic
   isMonitor: true
 
 # SCALAR
 pressure:
   defaults:
     units: kbar
-  schemaId: properties-directory-scalar-pressure
+  schemaId: properties-directory/scalar/pressure
   isResult: true
 
 total_energy:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-total-energy
+  schemaId: properties-directory/scalar/total-energy
   isResult: true
 
 surface_energy:
   defaults:
     units: eV/A^2
-  schemaId: properties-directory-scalar-surface-energy
+  schemaId: properties-directory/scalar/surface-energy
   isResult: true
 
 fermi_energy:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-fermi-energy
+  schemaId: properties-directory/scalar/fermi-energy
   isResult: true
 
 total_force:
   defaults:
     units: eV/angstrom
-  schemaId: properties-directory-scalar-total-force
+  schemaId: properties-directory/scalar/total-force
   isResult: true
 
 zero_point_energy:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-zero-point-energy
+  schemaId: properties-directory/scalar/zero-point-energy
   isResult: true
 
 reaction_energy_barrier:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-reaction-energy-barrier
+  schemaId: properties-directory/scalar/reaction-energy-barrier
   isResult: true
 
 electron_affinity:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-electron-affinity
+  schemaId: properties-directory/scalar/electron-affinity
   isResult: true
 
 ionization_potential:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-ionization-potential
+  schemaId: properties-directory/scalar/ionization-potential
   isResult: true
 
+valence_band_offset:
+  defaults:
+    units: eV
+  schemaId: properties-directory/scalar/valence-band-offset
+
 # NON-SCALAR
 phonon_dos:
   defaults:
     xAxis:
       label: frequency
       units: cm-1
     yAxis:
       label: Phonon DOS
       units: states/cm-1
-  schemaId: properties-directory-non-scalar-phonon-dos
+  schemaId: properties-directory/non-scalar/phonon-dos
   isResult: true
 
 phonon_dispersions:
   defaults:
     xAxis:
       label: qpoints
       units: crystal
     yAxis:
       label: frequency
       units: cm-1
-  schemaId: properties-directory-non-scalar-phonon-dispersions
+  schemaId: properties-directory/non-scalar/phonon-dispersions
   isResult: true
 
 total_energy_contributions:
   defaults:
     units: eV
-  schemaId: properties-directory-non-scalar-total-energy-contributions
+  schemaId: properties-directory/non-scalar/total-energy-contributions
   isResult: true
 
 band_gaps:
   types:
     - direct
     - indirect
   defaults:
     units: eV
-  schemaId: properties-directory-non-scalar-band-gaps
+  schemaId: properties-directory/non-scalar/band-gaps
   isResult: true
 
 stress_tensor:
   defaults:
     units: kbar
-  schemaId: properties-directory-non-scalar-stress-tensor
+  schemaId: properties-directory/non-scalar/stress-tensor
   isResult: true
 
 band_structure:
   defaults:
     xAxis:
       label: kpoints
       units: crystal
     yAxis:
       label: energy
       units: eV
 
-  schemaId: properties-directory-non-scalar-band-structure
+  schemaId: properties-directory/non-scalar/band-structure
   isResult: true
 
 density_of_states:
   defaults:
     xAxis:
       label: energy
       units: eV
     yAxis:
       label: density of states
       units: states/unitcell
-  schemaId: properties-directory-non-scalar-density-of-states
+  schemaId: properties-directory/non-scalar/density-of-states
   isResult: true
 
 reaction_energy_profile:
   defaults:
     xAxis:
       label: reaction coordinate
     yAxis:
       label: energy
       units: eV
-  schemaId: properties-directory-non-scalar-reaction-energy-profile
+  schemaId: properties-directory/non-scalar/reaction-energy-profile
   isResult: true
 
 potential_profile:
   defaults:
     xAxis:
       label: z coordinate
     yAxis:
       label: energy
       units: eV
-  schemaId: properties-directory-non-scalar-potential-profile
+  schemaId: properties-directory/non-scalar/potential-profile
   isResult: true
 
 charge_density_profile:
   defaults:
     xAxis:
       label: z coordinate
     yAxis:
       label: charge density
       units: e/A
-  schemaId: properties-directory-non-scalar-charge-density-profile
+  schemaId: properties-directory/non-scalar/charge-density-profile
   isResult: true
 
 vibrational_spectrum:
   defaults:
     xAxis:
       label: wavenumber
       units: cm-1
     yAxis:
       label: Absorption coefficient
       units: km/mol
-  schemaId: properties-directory-non-scalar-vibrational-spectrum
+  schemaId: properties-directory/non-scalar/vibrational-spectrum
   isResult: true
 
 file_content:
-  schemaId: properties-directory-file-content
+  schemaId: properties-directory/non-scalar/file-content
+  isResult: true
+
+average_potential_profile:
+  defaults:
+    xAxis:
+      label: z coordinate
+      units: angstrom
+    yAxis:
+      label: energy
+      units: eV
+  schemaId: properties-directory/non-scalar/average-potential-profile
   isResult: true
 
 # STRUCTURAL
 basis:
   defaults:
     units: angstrom
-  schemaId: properties-directory-structural-basis
+  schemaId: properties-directory/structural/basis
 
 lattice:
   defaults:
     units: angstrom
-  schemaId: properties-directory-structural-lattice
+  schemaId: properties-directory/structural/lattice
 
 atomic_forces:
   defaults:
     units: eV/angstrom
-  schemaId: properties-directory-structural-atomic-forces
+  schemaId: properties-directory/structural/atomic-forces
   isResult: true
 
 atomic_constraints:
-  schemaId: properties-directory-structural-basis-atomic-constraints
+  schemaId: properties-directory/structural/basis/atomic-constraints
 
 p-norm:
-  schemaId: properties-directory-structural-p-norm
+  schemaId: properties-directory/structural/p-norm
 
 volume:
   defaults:
     units: angstrom^3
-  schemaId: properties-directory-structural-volume
+  schemaId: properties-directory/structural/volume
 
 symmetry:
   defaults:
     units: angstrom
-  schemaId: properties-directory-structural-symmetry
+  schemaId: properties-directory/structural/symmetry
 
 elemental_ratio:
-  schemaId: properties-directory-structural-elemental-ratio
+  schemaId: properties-directory/structural/elemental-ratio
 
 density:
   defaults:
     units: g/cm^3
-  schemaId: properties-directory-structural-density
+  schemaId: properties-directory/structural/density
 
 magnetic_moments:
   defaults:
     units: uB
-  schemaId: properties-directory-structural-magnetic-moments
+  schemaId: properties-directory/structural/magnetic-moments
   isResult: true
 
-covalent_bonds:
+bonds:
   defaults:
     units: angstrom
-  schemaId: properties-directory-structural-covalent-bonds
+  schemaId: properties-directory/structural/basis/bonds
 
 inchi:
-  schemaId: properties-directory-structural-inchi
+  schemaId: properties-directory/structural/inchi
 
 inchi_key:
-  schemaId: properties-directory-structural-inchi_key
+  schemaId: properties-directory/structural/inchi-key
 
 material:
   schemaId: material
```

### Comparing `esse-2022.9.6.post0/package-lock.json` & `esse-2023.5.29.post0/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997830802603037%*

 * *Differences: {"'dependencies'": "{'@exabyte-io/eslint-config': OrderedDict([('version', '2022.11.17-0'), "*

 * *                   "('resolved', "*

 * *                   "'https://registry.npmjs.org/@exabyte-io/eslint-config/-/eslint-config-2022.11.17-0.tgz'), "*

 * *                   "('integrity', "*

 * *                   "'sha512-BYTDSqvjj6ZiWb8l46T5BKrVfkelct+vK2mh7joHu5UWtJMUzLkb0KQMV1+6SUy4xHFnws33XS7/+JSW1yeZOQ=='), "*

 * *                   "('dev', True)])}"}*

```diff
@@ -1486,14 +1486,20 @@
                 "js-yaml": "^3.13.1",
                 "minimatch": "^3.0.4",
                 "strip-json-comments": "^3.1.1"
             },
             "resolved": "https://registry.npmjs.org/@eslint/eslintrc/-/eslintrc-0.4.3.tgz",
             "version": "0.4.3"
         },
+        "@exabyte-io/eslint-config": {
+            "dev": true,
+            "integrity": "sha512-BYTDSqvjj6ZiWb8l46T5BKrVfkelct+vK2mh7joHu5UWtJMUzLkb0KQMV1+6SUy4xHFnws33XS7/+JSW1yeZOQ==",
+            "resolved": "https://registry.npmjs.org/@exabyte-io/eslint-config/-/eslint-config-2022.11.17-0.tgz",
+            "version": "2022.11.17-0"
+        },
         "@humanwhocodes/config-array": {
             "dev": true,
             "integrity": "sha512-FagtKFz74XrTl7y6HCzQpwDfXP0yhxe9lHLD1UZxjvZIcbyRz8zTFF/yYNfSfzU414eDwZ1SrO0Qvtyf+wFMQg==",
             "requires": {
                 "@humanwhocodes/object-schema": "^1.2.0",
                 "debug": "^4.1.1",
                 "minimatch": "^3.0.4"
```

### Comparing `esse-2022.9.6.post0/package.json` & `esse-2023.5.29.post0/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981481481481481%*

 * *Differences: {"'devDependencies'": "{'@exabyte-io/eslint-config': '^2022.11.17-0'}"}*

```diff
@@ -13,14 +13,15 @@
         "file": "^0.2.2",
         "json-schema-deref-sync": "0.14.0",
         "lodash": "4.17.21",
         "yamljs": "^0.3.0"
     },
     "description": "Exabyte Source of Schemas and Examples",
     "devDependencies": {
+        "@exabyte-io/eslint-config": "^2022.11.17-0",
         "chai": "4.3.4",
         "eslint": "^7.32.0",
         "eslint-config-airbnb": "^19.0.2",
         "eslint-config-prettier": "^8.3.0",
         "eslint-plugin-import": "^2.25.3",
         "eslint-plugin-jsdoc": "^37.1.0",
         "eslint-plugin-jsx-a11y": "^6.5.1",
```

### Comparing `esse-2022.9.6.post0/run-tests.sh` & `esse-2023.5.29.post0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/abstract/2d_plot.json` & `esse-2023.5.29.post0/schema/core/abstract/2d_plot.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/abstract/3d_vector_basis.json` & `esse-2023.5.29.post0/schema/core/abstract/3d_vector_basis.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/primitive/3d_lattice.json` & `esse-2023.5.29.post0/schema/core/primitive/3d_lattice.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/primitive/slugified_entry.json` & `esse-2023.5.29.post0/schema/core/primitive/slugified_entry.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/reference/experiment/condition.json` & `esse-2023.5.29.post0/schema/core/reference/experiment/condition.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/reference/experiment.json` & `esse-2023.5.29.post0/schema/core/reference/experiment.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/reference/literature.json` & `esse-2023.5.29.post0/schema/core/reference/literature.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/reference/modeling/exabyte.json` & `esse-2023.5.29.post0/schema/core/reference/modeling/exabyte.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/reusable/band_gap.json` & `esse-2023.5.29.post0/schema/property/raw.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6041666666666666%*

 * *Differences: {"'allOf'": "{0: {'$ref': '../in_memory_entity/base.json', 'description': 'entity schema'}}",*

 * * "'properties'": "{replace: OrderedDict([('slug', OrderedDict([('description', 'property slug, "*

 * *                 "e.g. total_energy'), ('type', 'string')])), ('group', "*

 * *                 "OrderedDict([('description', 'property group, e.g. qe:dft:gga:pbe'), ('type', "*

 * *                 "'string')])), ('data', OrderedDict([('description', 'container of the "*

 * *                 "information, specific to each property'), […]*

```diff
@@ -1,33 +1,32 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "../primitive/scalar.json"
+            "$ref": "../in_memory_entity/base.json",
+            "description": "entity schema"
         }
     ],
     "properties": {
-        "kpointConduction": {
-            "$ref": "../abstract/point.json",
-            "description": "kpoint inside conduction band in crystal coordinates"
+        "data": {
+            "description": "container of the information, specific to each property",
+            "type": "object"
         },
-        "kpointValence": {
-            "$ref": "../abstract/point.json",
-            "description": "kpoint inside valence band in crystal coordinates"
+        "group": {
+            "description": "property group, e.g. qe:dft:gga:pbe",
+            "type": "string"
         },
-        "type": {
-            "enum": [
-                "direct",
-                "indirect"
-            ],
+        "slug": {
+            "description": "property slug, e.g. total_energy",
             "type": "string"
         },
-        "units": {
-            "$ref": "../../definitions/units.json#/energy"
+        "source": {
+            "$ref": "source.json"
         }
     },
     "required": [
-        "type"
+        "data",
+        "source"
     ],
-    "schemaId": "core/reusable/band-gap",
-    "title": "band gap schema"
+    "schemaId": "property/raw",
+    "title": "Schema of material's preliminary property"
 }
```

### Comparing `esse-2022.9.6.post0/schema/core/reusable/energy.json` & `esse-2023.5.29.post0/schema/core/reusable/energy.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/reusable/file_metadata.json` & `esse-2023.5.29.post0/schema/core/reusable/file_metadata.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/core/reusable/object_storage_container_data.json` & `esse-2023.5.29.post0/schema/core/reusable/object_storage_container_data.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/definitions/units.json` & `esse-2023.5.29.post0/schema/definitions/units.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/element.json` & `esse-2023.5.29.post0/schema/element.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/job/compute.json` & `esse-2023.5.29.post0/schema/job/compute.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935897435897436%*

 * *Differences: {"'properties'": "{'isRestartable': OrderedDict([('description', 'Job is allowed to restart on "*

 * *                 "termination.'), ('type', 'boolean'), ('default', True)])}"}*

```diff
@@ -61,14 +61,19 @@
             },
             "type": "array"
         },
         "excludeFilesPattern": {
             "description": "A Python compatible regex to exclude files from upload. e.g. ^.*.txt& excludes all files with .txt suffix",
             "type": "string"
         },
+        "isRestartable": {
+            "default": true,
+            "description": "Job is allowed to restart on termination.",
+            "type": "boolean"
+        },
         "maxCPU": {
             "description": "Maximum CPU count per node. This parameter is used to let backend job submission infrastructure know that this job is to be charged for the maximum CPU per node instead of the actual ppn. For premium/fast queues where resources are provisioned on-demand and exclusively per user.",
             "type": "integer"
         },
         "nodes": {
             "description": "number of nodes used for the job inside the RMS.",
             "type": "integer",
```

### Comparing `esse-2022.9.6.post0/schema/job.json` & `esse-2023.5.29.post0/schema/job.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'allOf'": "{0: {'description': 'in-memory entity', '$ref': "*

 * *            "'in_memory_entity/named_defaultable_has_metadata.json'}}"}*

```diff
@@ -1,13 +1,13 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "system/entity.json",
-            "description": "entity schema"
+            "$ref": "in_memory_entity/named_defaultable_has_metadata.json",
+            "description": "in-memory entity"
         }
     ],
     "properties": {
         "_material": {
             "$ref": "system/entity_reference.json",
             "description": "Subset of the full information about the materials used inside this job."
         },
```

### Comparing `esse-2022.9.6.post0/schema/material.json` & `esse-2023.5.29.post0/schema/material.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'allOf'": "{0: {'description': 'in-memory entity', '$ref': "*

 * *            "'in_memory_entity/named_defaultable_has_metadata.json'}}"}*

```diff
@@ -1,13 +1,13 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "system/bankable_entity.json",
-            "description": "bankable entity schema"
+            "$ref": "in_memory_entity/named_defaultable_has_metadata.json",
+            "description": "in-memory entity"
         }
     ],
     "properties": {
         "basis": {
             "$ref": "properties_directory/structural/basis.json",
             "description": "object containing an array of elements and coordinates in the supercell"
         },
```

### Comparing `esse-2022.9.6.post0/schema/method.json` & `esse-2023.5.29.post0/schema/method.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/local-orbital.json` & `esse-2023.5.29.post0/schema/methods_directory/local-orbital.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/local_orbital/definitions/basis_sets.json` & `esse-2023.5.29.post0/schema/methods_directory/local_orbital/definitions/basis_sets.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/pseudopotential/dataset.json` & `esse-2023.5.29.post0/schema/methods_directory/pseudopotential/dataset.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/pseudopotential/file/energy_cutoff.json` & `esse-2023.5.29.post0/schema/methods_directory/pseudopotential/file/energy_cutoff.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/pseudopotential/file/radii.json` & `esse-2023.5.29.post0/schema/methods_directory/pseudopotential/file/radii.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/pseudopotential/file.json` & `esse-2023.5.29.post0/schema/methods_directory/pseudopotential/file.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/pseudopotential/precision.json` & `esse-2023.5.29.post0/schema/methods_directory/pseudopotential/precision.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/pseudopotential.json` & `esse-2023.5.29.post0/schema/methods_directory/pseudopotential.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/regression/dataset.json` & `esse-2023.5.29.post0/schema/methods_directory/regression/dataset.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/regression/kernel_ridge/data_per_property.json` & `esse-2023.5.29.post0/schema/methods_directory/regression/kernel_ridge/data_per_property.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/regression/linear/data_per_property.json` & `esse-2023.5.29.post0/schema/methods_directory/regression/linear/data_per_property.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/regression/precision_per_property.json` & `esse-2023.5.29.post0/schema/methods_directory/regression/precision_per_property.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/methods_directory/regression.json` & `esse-2023.5.29.post0/schema/methods_directory/regression.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/model.json` & `esse-2023.5.29.post0/schema/model.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/abin/configuration_interaction.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/abin/configuration_interaction.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/definitions.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/definitions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_model.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_model.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/component.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/component.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/functional/definitions.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/functional/definitions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/gga.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/gga.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/lda.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/lda.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/mgga.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/mgga.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/modifiers.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft/tags.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft/ksdft.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft/ksdft.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/dft.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/dft.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/pb/qm/semp.json` & `esse-2023.5.29.post0/schema/models_directory/pb/qm/semp.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/st/det/ml.json` & `esse-2023.5.29.post0/schema/models_directory/st/det/ml.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/models_directory/unknown.json` & `esse-2023.5.29.post0/schema/models_directory/unknown.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/new_model.json` & `esse-2023.5.29.post0/schema/new_model.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/project.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/object_storage_container_data.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.42857142857142855%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('CONTAINER', OrderedDict([('description', 'Object "*

 * *                 "storage container for the file'), ('type', 'string')])), ('NAME', "*

 * *                 "OrderedDict([('description', 'Name of the file inside the object storage "*

 * *                 "bucket'), ('type', 'string')])), ('PROVIDER', OrderedDict([('description', "*

 * *                 "'Object storage provider'), ('type', 'string')])), ('REGION', "*

 * *                 "OrderedDict([('description', 'Region for the […]*

```diff
@@ -1,31 +1,37 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
-    "allOf": [
-        {
-            "$ref": "system/defaultable.json",
-            "description": "defaultable entity schema"
-        }
-    ],
     "properties": {
-        "chargeRate": {
-            "description": "project charge rate",
-            "properties": {
-                "rate": {
-                    "type": "number"
-                }
-            },
-            "type": "object"
+        "CONTAINER": {
+            "description": "Object storage container for the file",
+            "type": "string"
+        },
+        "NAME": {
+            "description": "Name of the file inside the object storage bucket",
+            "type": "string"
+        },
+        "PROVIDER": {
+            "description": "Object storage provider",
+            "type": "string"
+        },
+        "REGION": {
+            "description": "Region for the object container specified in Container",
+            "type": "string"
+        },
+        "SIZE": {
+            "description": "Size of the file in bytes",
+            "type": "integer"
         },
-        "gid": {
-            "description": "project GID",
-            "type": "number"
+        "TIMESTAMP": {
+            "description": "Unix timestamp showing when the file was last modified",
+            "type": "string"
         }
     },
     "required": [
-        "gid",
-        "chargeRate"
+        "CONTAINER",
+        "NAME",
+        "PROVIDER",
+        "REGION"
     ],
-    "schemaId": "project",
-    "title": "project schema",
-    "type": "object"
+    "schemaId": "core/reusable/object-storage-container-data",
+    "title": "Object Storage Container Data"
 }
```

### Comparing `esse-2022.9.6.post0/schema/properties_directory/derived_properties.json` & `esse-2023.5.29.post0/schema/properties_directory/derived_properties.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/elemental/ionization_potential.json` & `esse-2023.5.29.post0/schema/properties_directory/elemental/ionization_potential.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/band_gaps.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/band_gaps.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/band_structure.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/band_structure.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/charge_density_profile.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/charge_density_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/density_of_states.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/density_of_states.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/file_content.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/phonon_dos.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.321875%*

 * *Differences: {"'allOf'": "[OrderedDict([('$ref', '../../core/abstract/2d_plot.json')])]",*

 * * "'properties'": "{'name': {'enum': ['phonon_dos']}, 'xAxis': OrderedDict([('properties', "*

 * *                 "OrderedDict([('label', OrderedDict([('enum', ['frequency'])])), ('units', "*

 * *                 "OrderedDict([('$ref', '../../definitions/units.json#/frequency')]))]))]), "*

 * *                 "'yAxis': OrderedDict([('properties', OrderedDict([('label', "*

 * *                 "OrderedDict([('enum', ['Phonon DOS'])])), ('units', Order […]*

```diff
@@ -1,33 +1,42 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
-    "allof": [
+    "allOf": [
         {
-            "$ref": "../../core/reusable/file_metadata.json"
+            "$ref": "../../core/abstract/2d_plot.json"
         }
     ],
     "properties": {
-        "filetype": {
-            "description": "What kind of file this is, e.g. image / text",
-            "enum": [
-                "image",
-                "text",
-                "csv"
-            ],
-            "type": "string"
-        },
         "name": {
             "enum": [
-                "file_content"
+                "phonon_dos"
             ]
         },
-        "objectData": {
-            "$ref": "../../core/reusable/object_storage_container_data.json"
+        "xAxis": {
+            "properties": {
+                "label": {
+                    "enum": [
+                        "frequency"
+                    ]
+                },
+                "units": {
+                    "$ref": "../../definitions/units.json#/frequency"
+                }
+            }
+        },
+        "yAxis": {
+            "properties": {
+                "label": {
+                    "enum": [
+                        "Phonon DOS"
+                    ]
+                },
+                "units": {
+                    "$ref": "../../definitions/units.json#/phononDOS"
+                }
+            }
         }
     },
-    "required": [
-        "name",
-        "objectData"
-    ],
-    "schemaId": "properties-directory/non-scalar/file-content",
-    "title": "file_content"
+    "schemaId": "properties-directory/non-scalar/phonon-dos",
+    "title": "Phonon density of states schema",
+    "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/phonon_dispersions.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/phonon_dispersions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/phonon_dos.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dos.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/potential_profile.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/potential_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/reaction_energy_profile.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/reaction_energy_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/total_energy_contributions.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/total_energy_contributions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/non-scalar/vibrational_spectrum.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/vibrational_spectrum.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/atomic_forces.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/atomic_forces.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/basis/atomic_coordinates.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/basis/atomic_coordinates.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/basis/atomic_element.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/basis/atomic_element.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/basis/bonds.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/basis/bonds.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/basis.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/basis.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/elemental_ratio.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/elemental_ratio.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/lattice/lattice_bravais.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/lattice/lattice_bravais.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/lattice/lattice_vectors.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/lattice/lattice_vectors.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/lattice.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/lattice.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/magnetic_moments.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/magnetic_moments.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/p-norm.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/p-norm.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/patterns/functional_group.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/patterns/functional_group.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/patterns/ring.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/patterns/ring.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/patterns/special_bond.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/patterns/special_bond.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/structural/symmetry.json` & `esse-2023.5.29.post0/schema/properties_directory/structural/symmetry.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/workflow/convergence/electronic.json` & `esse-2023.5.29.post0/schema/properties_directory/workflow/convergence/electronic.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/workflow/convergence/ionic.json` & `esse-2023.5.29.post0/schema/properties_directory/workflow/convergence/ionic.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/properties_directory/workflow/convergence/kpoint.json` & `esse-2023.5.29.post0/schema/properties_directory/workflow/convergence/kpoint.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/property.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/property/raw.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'allOf'": "{0: {'$ref': '../in_memory_entity/base.json'}}",*

 * * "'properties'": "{'source': {'$ref': 'source.json'}, delete: ['exabyteId']}",*

 * * "'required'": '{delete: [2, 1]}',*

 * * "'schemaId'": "'property/raw'",*

 * * "'title'": '"Schema of material\'s preliminary property"'}*

```diff
@@ -1,38 +1,32 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "system/entity.json",
+            "$ref": "../in_memory_entity/base.json",
             "description": "entity schema"
         }
     ],
     "properties": {
         "data": {
             "description": "container of the information, specific to each property",
             "type": "object"
         },
-        "exabyteId": {
-            "description": "identity of the corresponding material inside exabyte materials bank",
-            "type": "string"
-        },
         "group": {
             "description": "property group, e.g. qe:dft:gga:pbe",
             "type": "string"
         },
         "slug": {
             "description": "property slug, e.g. total_energy",
             "type": "string"
         },
         "source": {
-            "$ref": "core/reference.json"
+            "$ref": "source.json"
         }
     },
     "required": [
         "data",
-        "slug",
-        "group",
         "source"
     ],
-    "schemaId": "property",
-    "title": "property schema"
+    "schemaId": "property/raw",
+    "title": "Schema of material's preliminary property"
 }
```

### Comparing `esse-2022.9.6.post0/schema/software/application.json` & `esse-2023.5.29.post0/schema/software/application.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software/executable.json` & `esse-2023.5.29.post0/schema/software/executable.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software/flavor.json` & `esse-2023.5.29.post0/schema/software/flavor.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software/template.json` & `esse-2023.5.29.post0/schema/software/template.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/ml/exabyteml.json` & `esse-2023.5.29.post0/schema/software_directory/ml/exabyteml.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json` & `esse-2023.5.29.post0/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/ml/unit/execution/initialize.json` & `esse-2023.5.29.post0/schema/software_directory/ml/unit/execution/initialize.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/ml/unit/execution/train.json` & `esse-2023.5.29.post0/schema/software_directory/ml/unit/execution/train.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json` & `esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json` & `esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json` & `esse-2023.5.29.post0/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/modeling/espresso/arguments.json` & `esse-2023.5.29.post0/schema/software_directory/modeling/espresso/arguments.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/modeling/espresso.json` & `esse-2023.5.29.post0/schema/software_directory/modeling/espresso.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/modeling/nwchem.json` & `esse-2023.5.29.post0/schema/software_directory/modeling/nwchem.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/modeling/vasp.json` & `esse-2023.5.29.post0/schema/software_directory/modeling/vasp.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/scripting/jupyter-lab.json` & `esse-2023.5.29.post0/schema/software_directory/scripting/jupyter-lab.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/scripting/python.json` & `esse-2023.5.29.post0/schema/software_directory/scripting/python.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/software_directory/scripting/shell.json` & `esse-2023.5.29.post0/schema/software_directory/scripting/shell.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/system/base_entity_set.json` & `esse-2023.5.29.post0/schema/system/job_extended.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.625%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('mode', OrderedDict([('type', 'string')])), "*

 * *                 "('isExternal', OrderedDict([('type', 'boolean')])), ('_materials', "*

 * *                 "OrderedDict([('type', 'array'), ('items', OrderedDict([('allOf', "*

 * *                 "[OrderedDict([('$ref', 'entity_reference.json')])])]))])), ('_materialsSet', "*

 * *                 "OrderedDict([('allOf', [OrderedDict([('$ref', 'entity_reference.json')])])])), "*

 * *                 "('purged', OrderedDict([('type', 'bool […]*

```diff
@@ -1,34 +1,39 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "properties": {
-        "entitySetType": {
-            "type": "string"
-        },
-        "inSet": {
+        "_materials": {
             "items": {
                 "allOf": [
                     {
-                        "$ref": "../system/entity_reference.json"
-                    },
-                    {
-                        "properties": {
-                            "index": {
-                                "type": "number"
-                            },
-                            "type": {
-                                "type": "string"
-                            }
-                        },
-                        "type": "object"
+                        "$ref": "entity_reference.json"
                     }
                 ]
             },
             "type": "array"
         },
-        "isEntitySet": {
+        "_materialsSet": {
+            "allOf": [
+                {
+                    "$ref": "entity_reference.json"
+                }
+            ]
+        },
+        "dataset": {
+            "type": "object"
+        },
+        "isExternal": {
             "type": "boolean"
+        },
+        "mode": {
+            "type": "string"
+        },
+        "purged": {
+            "type": "boolean"
+        },
+        "purgedAt": {
+            "type": "number"
         }
     },
-    "schemaId": "system/base-entity-set",
-    "title": "extended base entity set schema"
+    "schemaId": "system/job-extended",
+    "title": "extended job schema"
 }
```

### Comparing `esse-2022.9.6.post0/schema/system/database_source.json` & `esse-2023.5.29.post0/schema/system/database_source.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/system/entity.json` & `esse-2023.5.29.post0/schema/workflow/subworkflow.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4321428571428571%*

 * *Differences: {"'allOf'": "{0: {'$ref': 'base_flow.json', delete: ['description']}, delete: [3, 2, 1, 0]}",*

 * * "'properties'": "{replace: OrderedDict([('units', OrderedDict([('description', 'Contains the "*

 * *                 "Units of the subworkflow'), ('type', 'array'), ('items', OrderedDict([('$ref', "*

 * *                 "'unit.json')]))])), ('model', OrderedDict([('description', 'Model used inside "*

 * *                 "the subworkflow'), ('$ref', '../model.json')])), ('application', "*

 * *                 "OrderedDict([('descrip […]*

```diff
@@ -1,45 +1,37 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "timestampable.json",
-            "description": "entity timestampable schema"
-        },
-        {
-            "$ref": "soft_removable.json",
-            "description": "entity removable schema"
-        },
-        {
-            "$ref": "name.json",
-            "description": "entity name schema"
-        },
-        {
-            "$ref": "tags.json",
-            "description": "entity tags schema"
-        },
-        {
-            "$ref": "schema_version.json",
-            "description": "entity schema version"
+            "$ref": "base_flow.json"
         }
     ],
     "properties": {
-        "_id": {
-            "description": "entity identity",
-            "type": "string"
-        },
-        "creator": {
-            "$ref": "entity_reference.json",
-            "description": "Subset of the full information about the user who created the entity."
-        },
-        "description": {
-            "description": "entity description",
-            "type": "string"
-        },
-        "owner": {
-            "$ref": "entity_reference.json",
-            "description": "Subset of the full information about the account who owns the entity."
+        "application": {
+            "$ref": "../software/application.json",
+            "description": "information about the simulation engine/application."
+        },
+        "isDraft": {
+            "default": false,
+            "description": "Defines whether to store the results/properties extracted in this unit to properties collection",
+            "type": "boolean"
+        },
+        "model": {
+            "$ref": "../model.json",
+            "description": "Model used inside the subworkflow"
+        },
+        "units": {
+            "description": "Contains the Units of the subworkflow",
+            "items": {
+                "$ref": "unit.json"
+            },
+            "type": "array"
         }
     },
-    "schemaId": "system/entity",
-    "title": "entity schema"
+    "required": [
+        "model",
+        "application"
+    ],
+    "schemaId": "workflow/subworkflow",
+    "title": "subworkflow schema",
+    "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/schema/system/file_source.json` & `esse-2023.5.29.post0/schema/system/file_source.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/system/history.json` & `esse-2023.5.29.post0/schema/system/history.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/system/job_extended.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/system/job_extended.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/system/message.json` & `esse-2023.5.29.post0/schema/system/message.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/system/status.json` & `esse-2023.5.29.post0/schema/system/status.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/base_flow.json` & `esse-2023.5.29.post0/schema/workflow/base_flow.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/new_subworkflow.json` & `esse-2023.5.29.post0/schema/workflow/new_subworkflow.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/subworkflow.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/subworkflow.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/assertion.json` & `esse-2023.5.29.post0/schema/workflow/unit/assertion.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/assignment.json` & `esse-2023.5.29.post0/schema/workflow/unit/assignment.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/condition.json` & `esse-2023.5.29.post0/schema/workflow/unit/condition.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/execution.json` & `esse-2023.5.29.post0/schema/workflow/unit/execution.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/input/_input.json` & `esse-2023.5.29.post0/schema/workflow/unit/input/_input.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/input/_inputItem.json` & `esse-2023.5.29.post0/schema/workflow/unit/input/_inputItem.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/input/_inputItemId.json` & `esse-2023.5.29.post0/schema/workflow/unit/input/_inputItemId.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/input/_inputItemScope.json` & `esse-2023.5.29.post0/schema/workflow/unit/input/_inputItemScope.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/io/api.json` & `esse-2023.5.29.post0/schema/workflow/unit/io/api.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/io/db.json` & `esse-2023.5.29.post0/schema/workflow/unit/io/db.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/io/object_storage.json` & `esse-2023.5.29.post0/schema/workflow/unit/io/object_storage.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/io.json` & `esse-2023.5.29.post0/schema/workflow/unit/io.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/map.json` & `esse-2023.5.29.post0/schema/workflow/unit/map.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/processing.json` & `esse-2023.5.29.post0/schema/workflow/unit/processing.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/reduce.json` & `esse-2023.5.29.post0/schema/workflow/unit/reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit/runtime/runtime_items.json` & `esse-2023.5.29.post0/schema/workflow/unit/runtime/runtime_items.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/schema/workflow/unit.json` & `esse-2023.5.29.post0/schema/workflow/unit.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95625%*

 * *Differences: {"'allOf'": "{0: {'$ref': '../in_memory_entity/named_defaultable_runtime_items.json'}}",*

 * * "'properties'": "{'_id': OrderedDict([('type', 'string')]), 'isDraft': OrderedDict([('type', "*

 * *                 "'boolean')])}"}*

```diff
@@ -1,16 +1,19 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "additionalProperties": true,
     "allOf": [
         {
-            "$ref": "../system/tags.json"
+            "$ref": "../in_memory_entity/named_defaultable_runtime_items.json"
         }
     ],
     "properties": {
+        "_id": {
+            "type": "string"
+        },
         "context": {
             "type": "object"
         },
         "enableRender": {
             "description": "Whether Rupy should attempt to use Jinja templating to add context variables into the unit",
             "type": "boolean"
         },
@@ -18,14 +21,17 @@
             "description": "Identity of the unit in the workflow. Used to trace the execution flow of the workflow.",
             "type": "string"
         },
         "head": {
             "description": "Whether this unit is the first one to be executed.",
             "type": "boolean"
         },
+        "isDraft": {
+            "type": "boolean"
+        },
         "name": {
             "description": "name of the unit. e.g. pw_scf",
             "type": "string"
         },
         "next": {
             "description": "Next unit's flowchartId. If empty, the current unit is the last.",
             "type": "string"
```

### Comparing `esse-2022.9.6.post0/schema/workflow.json` & `esse-2023.5.29.post0/schema/workflow.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'allOf'": "{0: {'$ref': 'in_memory_entity/named_defaultable_has_metadata.json', delete: "*

 * *            "['description']}, delete: [0]}"}*

```diff
@@ -1,17 +1,12 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "system/bankable_entity.json",
-            "description": "bankable entity schema"
-        },
-        {
-            "$ref": "system/defaultable.json",
-            "description": "defaultable entity schema"
+            "$ref": "in_memory_entity/named_defaultable_has_metadata.json"
         }
     ],
     "properties": {
         "isUsingDataset": {
             "description": "Whether to use the dataset tab in the job designer. Mutually exclusive with using the materials tab.",
             "type": "boolean"
         },
```

### Comparing `esse-2022.9.6.post0/setup.py` & `esse-2023.5.29.post0/setup.py`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/js/esse/index.js` & `esse-2023.5.29.post0/src/js/esse/index.js`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/js/esse/tests/validate.js` & `esse-2023.5.29.post0/src/js/esse/tests/validate.js`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/js/esse/utils.js` & `esse-2023.5.29.post0/src/js/esse/utils.js`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/js/json_include/index.js` & `esse-2023.5.29.post0/src/js/json_include/index.js`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/js/scripts/setSchemaIds.mjs` & `esse-2023.5.29.post0/src/js/scripts/setSchemaIds.mjs`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/__init__.py` & `esse-2023.5.29.post0/src/py/esse/__init__.py`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/job/compute.json` & `esse-2023.5.29.post0/src/py/esse/data/example/job/compute.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/job.json` & `esse-2023.5.29.post0/src/py/esse/data/example/job.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/material.json` & `esse-2023.5.29.post0/src/py/esse/data/example/material.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/pseudopotential/file.json` & `esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/pseudopotential/file.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/methods_directory/regression.json` & `esse-2023.5.29.post0/src/py/esse/data/example/methods_directory/regression.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/abin/configuration_interaction.json` & `esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/abin/configuration_interaction.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json` & `esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json` & `esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json` & `esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json` & `esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda.json` & `esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft.json` & `esse-2023.5.29.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/band_structure.json` & `esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/band_structure.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/density_of_states.json` & `esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/density_of_states.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dispersions.json` & `esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dispersions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dos.json` & `esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dos.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/potential_profile.json` & `esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/potential_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/reaction_energy_profile.json` & `esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/reaction_energy_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/non-scalar/total_energy_contributions.json` & `esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/non-scalar/total_energy_contributions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/properties_directory/structural/molecular_pattern.json` & `esse-2023.5.29.post0/src/py/esse/data/example/properties_directory/structural/molecular_pattern.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/execution/train.json` & `esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/execution/train.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json` & `esse-2023.5.29.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/system/file_source.json` & `esse-2023.5.29.post0/src/py/esse/data/example/system/file_source.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/execution.json` & `esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/execution.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/io/api.json` & `esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/io/api.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/workflow/unit/io.json` & `esse-2023.5.29.post0/src/py/esse/data/example/workflow/unit/io.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/example/workflow.json` & `esse-2023.5.29.post0/src/py/esse/data/example/workflow.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/manifest/dft_unit_functionals.yaml` & `esse-2023.5.29.post0/src/py/esse/data/manifest/dft_unit_functionals.yaml`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/manifest/functional_lookup_table.yaml` & `esse-2023.5.29.post0/src/py/esse/data/manifest/functional_lookup_table.yaml`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/manifest/models.yaml` & `esse-2023.5.29.post0/src/py/esse/data/manifest/models.yaml`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/manifest/properties.yaml` & `esse-2023.5.29.post0/src/py/esse/data/manifest/properties.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,239 +1,255 @@
 convergence_ionic:
   defaults:
     units: eV
-  schemaId: properties-directory-workflow-convergence-ionic
+  schemaId: properties-directory/workflow/convergence/ionic 
   isMonitor: true
 
 convergence_electronic:
   defaults:
     units: eV
-  schemaId: properties-directory-workflow-convergence-electronic
+  schemaId: properties-directory/workflow/convergence/electronic
   isMonitor: true
 
 # SCALAR
 pressure:
   defaults:
     units: kbar
-  schemaId: properties-directory-scalar-pressure
+  schemaId: properties-directory/scalar/pressure
   isResult: true
 
 total_energy:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-total-energy
+  schemaId: properties-directory/scalar/total-energy
   isResult: true
 
 surface_energy:
   defaults:
     units: eV/A^2
-  schemaId: properties-directory-scalar-surface-energy
+  schemaId: properties-directory/scalar/surface-energy
   isResult: true
 
 fermi_energy:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-fermi-energy
+  schemaId: properties-directory/scalar/fermi-energy
   isResult: true
 
 total_force:
   defaults:
     units: eV/angstrom
-  schemaId: properties-directory-scalar-total-force
+  schemaId: properties-directory/scalar/total-force
   isResult: true
 
 zero_point_energy:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-zero-point-energy
+  schemaId: properties-directory/scalar/zero-point-energy
   isResult: true
 
 reaction_energy_barrier:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-reaction-energy-barrier
+  schemaId: properties-directory/scalar/reaction-energy-barrier
   isResult: true
 
 electron_affinity:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-electron-affinity
+  schemaId: properties-directory/scalar/electron-affinity
   isResult: true
 
 ionization_potential:
   defaults:
     units: eV
-  schemaId: properties-directory-scalar-ionization-potential
+  schemaId: properties-directory/scalar/ionization-potential
   isResult: true
 
+valence_band_offset:
+  defaults:
+    units: eV
+  schemaId: properties-directory/scalar/valence-band-offset
+
 # NON-SCALAR
 phonon_dos:
   defaults:
     xAxis:
       label: frequency
       units: cm-1
     yAxis:
       label: Phonon DOS
       units: states/cm-1
-  schemaId: properties-directory-non-scalar-phonon-dos
+  schemaId: properties-directory/non-scalar/phonon-dos
   isResult: true
 
 phonon_dispersions:
   defaults:
     xAxis:
       label: qpoints
       units: crystal
     yAxis:
       label: frequency
       units: cm-1
-  schemaId: properties-directory-non-scalar-phonon-dispersions
+  schemaId: properties-directory/non-scalar/phonon-dispersions
   isResult: true
 
 total_energy_contributions:
   defaults:
     units: eV
-  schemaId: properties-directory-non-scalar-total-energy-contributions
+  schemaId: properties-directory/non-scalar/total-energy-contributions
   isResult: true
 
 band_gaps:
   types:
     - direct
     - indirect
   defaults:
     units: eV
-  schemaId: properties-directory-non-scalar-band-gaps
+  schemaId: properties-directory/non-scalar/band-gaps
   isResult: true
 
 stress_tensor:
   defaults:
     units: kbar
-  schemaId: properties-directory-non-scalar-stress-tensor
+  schemaId: properties-directory/non-scalar/stress-tensor
   isResult: true
 
 band_structure:
   defaults:
     xAxis:
       label: kpoints
       units: crystal
     yAxis:
       label: energy
       units: eV
 
-  schemaId: properties-directory-non-scalar-band-structure
+  schemaId: properties-directory/non-scalar/band-structure
   isResult: true
 
 density_of_states:
   defaults:
     xAxis:
       label: energy
       units: eV
     yAxis:
       label: density of states
       units: states/unitcell
-  schemaId: properties-directory-non-scalar-density-of-states
+  schemaId: properties-directory/non-scalar/density-of-states
   isResult: true
 
 reaction_energy_profile:
   defaults:
     xAxis:
       label: reaction coordinate
     yAxis:
       label: energy
       units: eV
-  schemaId: properties-directory-non-scalar-reaction-energy-profile
+  schemaId: properties-directory/non-scalar/reaction-energy-profile
   isResult: true
 
 potential_profile:
   defaults:
     xAxis:
       label: z coordinate
     yAxis:
       label: energy
       units: eV
-  schemaId: properties-directory-non-scalar-potential-profile
+  schemaId: properties-directory/non-scalar/potential-profile
   isResult: true
 
 charge_density_profile:
   defaults:
     xAxis:
       label: z coordinate
     yAxis:
       label: charge density
       units: e/A
-  schemaId: properties-directory-non-scalar-charge-density-profile
+  schemaId: properties-directory/non-scalar/charge-density-profile
   isResult: true
 
 vibrational_spectrum:
   defaults:
     xAxis:
       label: wavenumber
       units: cm-1
     yAxis:
       label: Absorption coefficient
       units: km/mol
-  schemaId: properties-directory-non-scalar-vibrational-spectrum
+  schemaId: properties-directory/non-scalar/vibrational-spectrum
   isResult: true
 
 file_content:
-  schemaId: properties-directory-file-content
+  schemaId: properties-directory/non-scalar/file-content
+  isResult: true
+
+average_potential_profile:
+  defaults:
+    xAxis:
+      label: z coordinate
+      units: angstrom
+    yAxis:
+      label: energy
+      units: eV
+  schemaId: properties-directory/non-scalar/average-potential-profile
   isResult: true
 
 # STRUCTURAL
 basis:
   defaults:
     units: angstrom
-  schemaId: properties-directory-structural-basis
+  schemaId: properties-directory/structural/basis
 
 lattice:
   defaults:
     units: angstrom
-  schemaId: properties-directory-structural-lattice
+  schemaId: properties-directory/structural/lattice
 
 atomic_forces:
   defaults:
     units: eV/angstrom
-  schemaId: properties-directory-structural-atomic-forces
+  schemaId: properties-directory/structural/atomic-forces
   isResult: true
 
 atomic_constraints:
-  schemaId: properties-directory-structural-basis-atomic-constraints
+  schemaId: properties-directory/structural/basis/atomic-constraints
 
 p-norm:
-  schemaId: properties-directory-structural-p-norm
+  schemaId: properties-directory/structural/p-norm
 
 volume:
   defaults:
     units: angstrom^3
-  schemaId: properties-directory-structural-volume
+  schemaId: properties-directory/structural/volume
 
 symmetry:
   defaults:
     units: angstrom
-  schemaId: properties-directory-structural-symmetry
+  schemaId: properties-directory/structural/symmetry
 
 elemental_ratio:
-  schemaId: properties-directory-structural-elemental-ratio
+  schemaId: properties-directory/structural/elemental-ratio
 
 density:
   defaults:
     units: g/cm^3
-  schemaId: properties-directory-structural-density
+  schemaId: properties-directory/structural/density
 
 magnetic_moments:
   defaults:
     units: uB
-  schemaId: properties-directory-structural-magnetic-moments
+  schemaId: properties-directory/structural/magnetic-moments
   isResult: true
 
-covalent_bonds:
+bonds:
   defaults:
     units: angstrom
-  schemaId: properties-directory-structural-covalent-bonds
+  schemaId: properties-directory/structural/basis/bonds
 
 inchi:
-  schemaId: properties-directory-structural-inchi
+  schemaId: properties-directory/structural/inchi
 
 inchi_key:
-  schemaId: properties-directory-structural-inchi_key
+  schemaId: properties-directory/structural/inchi-key
 
 material:
   schemaId: material
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/abstract/2d_plot.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/abstract/2d_plot.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/abstract/3d_vector_basis.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/abstract/3d_vector_basis.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/3d_lattice.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/3d_lattice.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/primitive/slugified_entry.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/primitive/slugified_entry.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/experiment/condition.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/experiment/condition.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/experiment.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/experiment.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/literature.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/literature.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/reference/modeling/exabyte.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/reference/modeling/exabyte.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/band_gap.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software/template.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5357142857142857%*

 * *Differences: {"'allOf'": "{0: {'$ref': '../workflow/unit/input/_inputItem.json'}}",*

 * * "'properties'": "{replace: OrderedDict([('applicationName', OrderedDict([('type', 'string')])), "*

 * *                 "('applicationVersion', OrderedDict([('type', 'string')])), ('executableName', "*

 * *                 "OrderedDict([('type', 'string')])), ('contextProviders', OrderedDict([('type', "*

 * *                 "'array'), ('items', OrderedDict([('description', 'render context provider "*

 * *                 "names'), ('$ref', "*

 * *              […]*

```diff
@@ -1,33 +1,33 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "../primitive/scalar.json"
+            "$ref": "../workflow/unit/input/_inputItem.json"
         }
     ],
     "properties": {
-        "kpointConduction": {
-            "$ref": "../abstract/point.json",
-            "description": "kpoint inside conduction band in crystal coordinates"
-        },
-        "kpointValence": {
-            "$ref": "../abstract/point.json",
-            "description": "kpoint inside valence band in crystal coordinates"
+        "applicationName": {
+            "type": "string"
         },
-        "type": {
-            "enum": [
-                "direct",
-                "indirect"
-            ],
+        "applicationVersion": {
             "type": "string"
         },
-        "units": {
-            "$ref": "../../definitions/units.json#/energy"
+        "contextProviders": {
+            "items": {
+                "$ref": "../workflow/unit/runtime/_runtime_item_name_object.json",
+                "description": "render context provider names"
+            },
+            "type": "array"
+        },
+        "executableName": {
+            "type": "string"
         }
     },
     "required": [
-        "type"
+        "name",
+        "content"
     ],
-    "schemaId": "core/reusable/band-gap",
-    "title": "band gap schema"
+    "schemaId": "software/template",
+    "title": "template schema",
+    "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/energy.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/energy.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/file_metadata.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/core/reusable/file_metadata.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/core/reusable/object_storage_container_data.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/data_per_property.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('xFit', OrderedDict([('description', 'training data'), "*

 * *                 "('type', 'array')])), ('dualCoefficients', OrderedDict([('description', 'dual "*

 * *                 "coefficients'), ('type', 'array')])), ('perFeature', OrderedDict([('type', "*

 * *                 "'array'), ('description', 'per-feature (property used for training the ML "*

 * *                 "method/model) parameters'), ('items', OrderedDict([('type', 'object'), ('allOf', "*

 * *                 "[Ordere […]*

```diff
@@ -1,37 +1,35 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "properties": {
-        "CONTAINER": {
-            "description": "Object storage container for the file",
-            "type": "string"
+        "dualCoefficients": {
+            "description": "dual coefficients",
+            "type": "array"
         },
-        "NAME": {
-            "description": "Name of the file inside the object storage bucket",
-            "type": "string"
+        "perFeature": {
+            "description": "per-feature (property used for training the ML method/model) parameters",
+            "items": {
+                "allOf": [
+                    {
+                        "$ref": "../data_per_feature.json"
+                    }
+                ],
+                "required": [
+                    "name"
+                ],
+                "type": "object"
+            },
+            "type": "array"
         },
-        "PROVIDER": {
-            "description": "Object storage provider",
-            "type": "string"
-        },
-        "REGION": {
-            "description": "Region for the object container specified in Container",
-            "type": "string"
-        },
-        "SIZE": {
-            "description": "Size of the file in bytes",
-            "type": "integer"
-        },
-        "TIMESTAMP": {
-            "description": "Unix timestamp showing when the file was last modified",
-            "type": "string"
+        "xFit": {
+            "description": "training data",
+            "type": "array"
         }
     },
     "required": [
-        "CONTAINER",
-        "NAME",
-        "PROVIDER",
-        "REGION"
+        "xFit",
+        "dualCoefficients",
+        "perFeature"
     ],
-    "schemaId": "core/reusable/object-storage-container-data",
-    "title": "Object Storage Container Data"
+    "schemaId": "methods-directory/regression/kernel-ridge/data-per-property",
+    "title": "linear regression parameters schema"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/definitions/units.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/definitions/units.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/element.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/element.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/job/compute.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/job/compute.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935897435897436%*

 * *Differences: {"'properties'": "{'isRestartable': OrderedDict([('description', 'Job is allowed to restart on "*

 * *                 "termination.'), ('type', 'boolean'), ('default', True)])}"}*

```diff
@@ -61,14 +61,19 @@
             },
             "type": "array"
         },
         "excludeFilesPattern": {
             "description": "A Python compatible regex to exclude files from upload. e.g. ^.*.txt& excludes all files with .txt suffix",
             "type": "string"
         },
+        "isRestartable": {
+            "default": true,
+            "description": "Job is allowed to restart on termination.",
+            "type": "boolean"
+        },
         "maxCPU": {
             "description": "Maximum CPU count per node. This parameter is used to let backend job submission infrastructure know that this job is to be charged for the maximum CPU per node instead of the actual ppn. For premium/fast queues where resources are provisioned on-demand and exclusively per user.",
             "type": "integer"
         },
         "nodes": {
             "description": "number of nodes used for the job inside the RMS.",
             "type": "integer",
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/job.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/job.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'allOf'": "{0: {'description': 'in-memory entity', '$ref': "*

 * *            "'in_memory_entity/named_defaultable_has_metadata.json'}}"}*

```diff
@@ -1,13 +1,13 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "system/entity.json",
-            "description": "entity schema"
+            "$ref": "in_memory_entity/named_defaultable_has_metadata.json",
+            "description": "in-memory entity"
         }
     ],
     "properties": {
         "_material": {
             "$ref": "system/entity_reference.json",
             "description": "Subset of the full information about the materials used inside this job."
         },
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/material.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/material.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'allOf'": "{0: {'description': 'in-memory entity', '$ref': "*

 * *            "'in_memory_entity/named_defaultable_has_metadata.json'}}"}*

```diff
@@ -1,13 +1,13 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "system/bankable_entity.json",
-            "description": "bankable entity schema"
+            "$ref": "in_memory_entity/named_defaultable_has_metadata.json",
+            "description": "in-memory entity"
         }
     ],
     "properties": {
         "basis": {
             "$ref": "properties_directory/structural/basis.json",
             "description": "object containing an array of elements and coordinates in the supercell"
         },
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/method.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/method.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/local-orbital.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/local-orbital.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/basis_sets.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/basis_sets.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/dataset.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/dataset.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/energy_cutoff.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/energy_cutoff.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/radii.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/radii.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential/precision.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential/precision.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/pseudopotential.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/pseudopotential.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/dataset.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/dataset.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/data_per_property.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/linear/data_per_property.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.74921875%*

 * *Differences: {"'properties'": "{'perFeature': {'items': {'required': ['coefficient'], 'properties': "*

 * *                 "OrderedDict([('coefficient', OrderedDict([('description', 'coefficient in linear "*

 * *                 "regression'), ('type', 'number')]))])}}, 'intercept': "*

 * *                 "OrderedDict([('description', 'intercept (shift) from the linear or non-linear "*

 * *                 "fit of data points'), ('type', 'number')]), delete: ['xFit', "*

 * *                 "'dualCoefficients']}",*

 * * "'required'": "{insert: [(0 […]*

```diff
@@ -1,35 +1,36 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "properties": {
-        "dualCoefficients": {
-            "description": "dual coefficients",
-            "type": "array"
+        "intercept": {
+            "description": "intercept (shift) from the linear or non-linear fit of data points",
+            "type": "number"
         },
         "perFeature": {
             "description": "per-feature (property used for training the ML method/model) parameters",
             "items": {
                 "allOf": [
                     {
                         "$ref": "../data_per_feature.json"
                     }
                 ],
+                "properties": {
+                    "coefficient": {
+                        "description": "coefficient in linear regression",
+                        "type": "number"
+                    }
+                },
                 "required": [
-                    "name"
+                    "coefficient"
                 ],
                 "type": "object"
             },
             "type": "array"
-        },
-        "xFit": {
-            "description": "training data",
-            "type": "array"
         }
     },
     "required": [
-        "xFit",
-        "dualCoefficients",
+        "intercept",
         "perFeature"
     ],
-    "schemaId": "methods-directory/regression/kernel-ridge/data-per-property",
+    "schemaId": "methods-directory/regression/linear/data-per-property",
     "title": "linear regression parameters schema"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/linear/data_per_property.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis/bonds.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25%*

 * *Differences: {"'items'": "OrderedDict([('type', 'object'), ('properties', OrderedDict([('atomPair', "*

 * *            "OrderedDict([('description', 'indices of the two connected atoms'), ('allOf', "*

 * *            "[OrderedDict([('$ref', '../../../core/primitive/array_of_ids.json')])]), ('minItems', "*

 * *            "2), ('maxItems', 2)])), ('bondType', OrderedDict([('type', 'string'), ('enum', "*

 * *            "['single', 'double', 'triple', 'quadruple', 'aromatic', 'tautomeric', 'dative', "*

 * *            "'other'])]))]))])",*

 * * "'sche […]*

```diff
@@ -1,36 +1,35 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
-    "properties": {
-        "intercept": {
-            "description": "intercept (shift) from the linear or non-linear fit of data points",
-            "type": "number"
-        },
-        "perFeature": {
-            "description": "per-feature (property used for training the ML method/model) parameters",
-            "items": {
+    "items": {
+        "properties": {
+            "atomPair": {
                 "allOf": [
                     {
-                        "$ref": "../data_per_feature.json"
-                    }
-                ],
-                "properties": {
-                    "coefficient": {
-                        "description": "coefficient in linear regression",
-                        "type": "number"
+                        "$ref": "../../../core/primitive/array_of_ids.json"
                     }
-                },
-                "required": [
-                    "coefficient"
                 ],
-                "type": "object"
+                "description": "indices of the two connected atoms",
+                "maxItems": 2,
+                "minItems": 2
             },
-            "type": "array"
-        }
+            "bondType": {
+                "enum": [
+                    "single",
+                    "double",
+                    "triple",
+                    "quadruple",
+                    "aromatic",
+                    "tautomeric",
+                    "dative",
+                    "other"
+                ],
+                "type": "string"
+            }
+        },
+        "type": "object"
     },
-    "required": [
-        "intercept",
-        "perFeature"
-    ],
-    "schemaId": "methods-directory/regression/linear/data-per-property",
-    "title": "linear regression parameters schema"
+    "schemaId": "properties-directory/structural/basis/bonds",
+    "title": "bonds schema",
+    "type": "array",
+    "uniqueItems": true
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression/precision_per_property.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression/precision_per_property.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/methods_directory/regression.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/methods_directory/regression.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/model.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/model.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/definitions.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/definitions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_model.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_model.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/component.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/component.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/definitions.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/definitions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/modifiers.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/tags.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/dft.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/dft.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/pb/qm/semp.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/pb/qm/semp.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/st/det/ml.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/st/det/ml.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/models_directory/unknown.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/models_directory/unknown.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/new_model.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/new_model.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/project.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/system/database_source.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'description'": "'information about a database source'",*

 * * "'properties'": "{replace: OrderedDict([('id', OrderedDict([('description', 'ID string for the "*

 * *                 'materials uploaded from a third party source inside the third party source. For '*

 * *                 "materialsproject.org an example ID is mp-32'), ('type', 'string')])), ('source', "*

 * *                 "OrderedDict([('description', 'Third party source name.'), ('type', 'string')])), "*

 * *                 "('origin', OrderedDict([('descripti […]*

```diff
@@ -1,31 +1,30 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
-    "allOf": [
-        {
-            "$ref": "system/defaultable.json",
-            "description": "defaultable entity schema"
-        }
-    ],
+    "description": "information about a database source",
     "properties": {
-        "chargeRate": {
-            "description": "project charge rate",
-            "properties": {
-                "rate": {
-                    "type": "number"
-                }
-            },
+        "data": {
+            "description": "Original response from external source",
             "type": "object"
         },
-        "gid": {
-            "description": "project GID",
-            "type": "number"
+        "id": {
+            "description": "ID string for the materials uploaded from a third party source inside the third party source. For materialsproject.org an example ID is mp-32",
+            "type": "string"
+        },
+        "origin": {
+            "description": "A flag that is true when material is initially imported from a third party * (as opposed to being independently designed from scratch).",
+            "type": "boolean"
+        },
+        "source": {
+            "description": "Third party source name.",
+            "type": "string"
         }
     },
     "required": [
-        "gid",
-        "chargeRate"
+        "id",
+        "source",
+        "origin"
     ],
-    "schemaId": "project",
-    "title": "project schema",
+    "schemaId": "system/database-source",
+    "title": "database source schema",
     "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/derived_properties.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/derived_properties.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/elemental/ionization_potential.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/elemental/ionization_potential.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_gaps.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_gaps.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_structure.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_structure.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/charge_density_profile.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/charge_density_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/density_of_states.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/density_of_states.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/file_content.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/file_content.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7142857142857143%*

 * *Differences: {"'allOf'": "[OrderedDict([('$ref', '../../core/reusable/file_metadata.json')])]",*

 * * 'delete': "['allof']"}*

```diff
@@ -1,10 +1,10 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
-    "allof": [
+    "allOf": [
         {
             "$ref": "../../core/reusable/file_metadata.json"
         }
     ],
     "properties": {
         "filetype": {
             "description": "What kind of file this is, e.g. image / text",
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dispersions.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dispersions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dos.json` & `esse-2023.5.29.post0/schema/properties_directory/non-scalar/average_potential_profile.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.65625%*

 * *Differences: {"'properties'": "{'xAxis': {'properties': {'label': {'enum': ['z coordinate']}, 'units': {'$ref': "*

 * *                 "'../../definitions/units.json#/length'}}}, 'yAxis': {'properties': {'label': "*

 * *                 "{'enum': ['energy']}, 'units': {'$ref': "*

 * *                 "'../../definitions/units.json#/energy'}}}, 'name': {'enum': "*

 * *                 "['average_potential_profile']}}",*

 * * "'schemaId'": "'properties-directory/non-scalar/average-potential-profile'",*

 * * "'title'": "'average potential profile sche […]*

```diff
@@ -4,39 +4,38 @@
         {
             "$ref": "../../core/abstract/2d_plot.json"
         }
     ],
     "properties": {
         "name": {
             "enum": [
-                "phonon_dos"
+                "average_potential_profile"
             ]
         },
         "xAxis": {
             "properties": {
                 "label": {
                     "enum": [
-                        "frequency"
+                        "z coordinate"
                     ]
                 },
                 "units": {
-                    "$ref": "../../definitions/units.json#/frequency"
+                    "$ref": "../../definitions/units.json#/length"
                 }
             }
         },
         "yAxis": {
             "properties": {
                 "label": {
                     "enum": [
-                        "Phonon DOS"
+                        "energy"
                     ]
                 },
                 "units": {
-                    "$ref": "../../definitions/units.json#/phononDOS"
+                    "$ref": "../../definitions/units.json#/energy"
                 }
             }
         }
     },
-    "schemaId": "properties-directory/non-scalar/phonon-dos",
-    "title": "Phonon density of states schema",
-    "type": "object"
+    "schemaId": "properties-directory/non-scalar/average-potential-profile",
+    "title": "average potential profile schema"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/potential_profile.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/potential_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/reaction_energy_profile.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/reaction_energy_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/total_energy_contributions.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/total_energy_contributions.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/non-scalar/vibrational_spectrum.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/vibrational_spectrum.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/atomic_forces.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/atomic_forces.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinates.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinates.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_element.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_element.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis/bonds.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/train.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25%*

 * *Differences: {"'allOf'": "[OrderedDict([('$ref', '../../../../workflow/unit/execution.json')])]",*

 * * "'properties'": "OrderedDict([('input', OrderedDict([('description', 'model train unit (NOTE: "*

 * *                 "info about method, eg. regression/linear is taken from (sub)workflow)'), "*

 * *                 "('type', 'object'), ('properties', OrderedDict([('features', "*

 * *                 "OrderedDict([('description', 'material features used for model fitting'), "*

 * *                 '(\'type\', \'array\'), (\'items\', OrderedDi […]*

```diff
@@ -1,35 +1,38 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
-    "items": {
-        "properties": {
-            "atomPair": {
-                "allOf": [
-                    {
-                        "$ref": "../../../core/primitive/array_of_ids.json"
-                    }
-                ],
-                "description": "indices of the two connected atoms",
-                "maxItems": 2,
-                "minItems": 2
+    "allOf": [
+        {
+            "$ref": "../../../../workflow/unit/execution.json"
+        }
+    ],
+    "properties": {
+        "input": {
+            "description": "model train unit (NOTE: info about method, eg. regression/linear is taken from (sub)workflow)",
+            "properties": {
+                "features": {
+                    "description": "material features used for model fitting",
+                    "items": {
+                        "description": "material features (properties) in a 'flattened' format",
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "targets": {
+                    "description": "target properties to train for",
+                    "items": {
+                        "description": "material features (properties) in a 'flattened' format",
+                        "type": "string"
+                    },
+                    "type": "array"
+                }
             },
-            "bondType": {
-                "enum": [
-                    "single",
-                    "double",
-                    "triple",
-                    "quadruple",
-                    "aromatic",
-                    "tautomeric",
-                    "dative",
-                    "other"
-                ],
-                "type": "string"
-            }
-        },
-        "type": "object"
+            "required": [
+                "features",
+                "targets"
+            ],
+            "type": "object"
+        }
     },
-    "schemaId": "properties-directory/structural/basis/bonds",
-    "title": "bonds schema",
-    "type": "array",
-    "uniqueItems": true
+    "schemaId": "software-directory/ml/unit/execution/train",
+    "title": "train unit schema"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/basis.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/basis.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/elemental_ratio.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/elemental_ratio.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_bravais.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_bravais.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_vectors.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_vectors.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/lattice.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/lattice.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/magnetic_moments.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/magnetic_moments.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/p-norm.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/p-norm.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/patterns/functional_group.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/patterns/functional_group.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/patterns/ring.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/patterns/ring.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/patterns/special_bond.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/patterns/special_bond.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/structural/symmetry.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/structural/symmetry.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/electronic.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/electronic.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/ionic.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/ionic.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/kpoint.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/kpoint.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/property.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/io/db.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25%*

 * *Differences: {"'oneOf'": "[OrderedDict([('properties', OrderedDict([('ids', OrderedDict([('description', 'IDs "*

 * *            "of item to retrieve from db'), ('type', 'array'), ('items', OrderedDict([('type', "*

 * *            "'string')]))]))])), ('required', ['ids'])]), OrderedDict([('properties', "*

 * *            "OrderedDict([('collection', OrderedDict([('description', 'db collection name'), "*

 * *            "('type', 'string')])), ('draft', OrderedDict([('description', 'whether the result "*

 * *            "should be saved as draf […]*

```diff
@@ -1,38 +1,39 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
-    "allOf": [
+    "oneOf": [
         {
-            "$ref": "system/entity.json",
-            "description": "entity schema"
-        }
-    ],
-    "properties": {
-        "data": {
-            "description": "container of the information, specific to each property",
-            "type": "object"
-        },
-        "exabyteId": {
-            "description": "identity of the corresponding material inside exabyte materials bank",
-            "type": "string"
+            "properties": {
+                "ids": {
+                    "description": "IDs of item to retrieve from db",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                }
+            },
+            "required": [
+                "ids"
+            ]
         },
-        "group": {
-            "description": "property group, e.g. qe:dft:gga:pbe",
-            "type": "string"
-        },
-        "slug": {
-            "description": "property slug, e.g. total_energy",
-            "type": "string"
-        },
-        "source": {
-            "$ref": "core/reference.json"
+        {
+            "properties": {
+                "collection": {
+                    "description": "db collection name",
+                    "type": "string"
+                },
+                "draft": {
+                    "default": true,
+                    "description": "whether the result should be saved as draft",
+                    "type": "boolean"
+                }
+            },
+            "required": [
+                "collection",
+                "draft"
+            ]
         }
-    },
-    "required": [
-        "data",
-        "slug",
-        "group",
-        "source"
     ],
-    "schemaId": "property",
-    "title": "property schema"
+    "schemaId": "workflow/unit/io/db",
+    "title": "data IO database input/output schema",
+    "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software/application.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software/application.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software/executable.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software/executable.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software/flavor.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software/flavor.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software/template.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/assertion.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7023809523809524%*

 * *Differences: {"'allOf'": "{0: {'$ref': '../unit.json'}}",*

 * * "'properties'": "{replace: OrderedDict([('type', OrderedDict([('enum', ['assertion'])])), "*

 * *                 "('statement', OrderedDict([('type', 'string')])), ('errorMessage', "*

 * *                 "OrderedDict([('type', 'string')]))])}",*

 * * "'required'": "{insert: [(1, 'statement')], delete: [1]}",*

 * * "'schemaId'": "'workflow/unit/assertion'",*

 * * "'title'": "'assignment unit schema'"}*

```diff
@@ -1,33 +1,28 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "../workflow/unit/input/_inputItem.json"
+            "$ref": "../unit.json"
         }
     ],
     "properties": {
-        "applicationName": {
+        "errorMessage": {
             "type": "string"
         },
-        "applicationVersion": {
+        "statement": {
             "type": "string"
         },
-        "contextProviders": {
-            "items": {
-                "$ref": "../workflow/unit/runtime/_runtime_item_name_object.json",
-                "description": "render context provider names"
-            },
-            "type": "array"
-        },
-        "executableName": {
-            "type": "string"
+        "type": {
+            "enum": [
+                "assertion"
+            ]
         }
     },
     "required": [
         "name",
-        "content"
+        "statement"
     ],
-    "schemaId": "software/template",
-    "title": "template schema",
+    "schemaId": "workflow/unit/assertion",
+    "title": "assignment unit schema",
     "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/exabyteml.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/exabyteml.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/initialize.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/initialize.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/train.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5416666666666666%*

 * *Differences: {"'allOf'": "{0: {'$ref': '../../../../../workflow/unit/processing.json'}}",*

 * * "'properties'": "{replace: OrderedDict([('operation', OrderedDict([('type', 'string'), ('enum', "*

 * *                 "['data_transformation'])])), ('operationType', OrderedDict([('type', 'string'), "*

 * *                 "('enum', ['manipulation'])])), ('inputData', OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('cleanMissingData', OrderedDict([('description', "*

 * *                 "'whether to clean miss […]*

```diff
@@ -1,38 +1,50 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "../../../../workflow/unit/execution.json"
+            "$ref": "../../../../../workflow/unit/processing.json"
         }
     ],
     "properties": {
-        "input": {
-            "description": "model train unit (NOTE: info about method, eg. regression/linear is taken from (sub)workflow)",
+        "inputData": {
             "properties": {
-                "features": {
-                    "description": "material features used for model fitting",
-                    "items": {
-                        "description": "material features (properties) in a 'flattened' format",
-                        "type": "string"
-                    },
-                    "type": "array"
+                "cleanMissingData": {
+                    "default": true,
+                    "description": "whether to clean missing data, eg. NaN",
+                    "type": "boolean"
                 },
-                "targets": {
-                    "description": "target properties to train for",
-                    "items": {
-                        "description": "material features (properties) in a 'flattened' format",
-                        "type": "string"
-                    },
-                    "type": "array"
+                "removeDuplicateRows": {
+                    "default": true,
+                    "description": "whether to remove duplicate rows",
+                    "type": "boolean"
+                },
+                "replaceNoneValuesWith": {
+                    "default": 0,
+                    "description": "replace None values with a given value",
+                    "type": "number"
                 }
             },
             "required": [
-                "features",
-                "targets"
+                "cleanMissingData",
+                "removeDuplicateRows",
+                "replaceNoneValuesWith"
             ],
             "type": "object"
+        },
+        "operation": {
+            "enum": [
+                "data_transformation"
+            ],
+            "type": "string"
+        },
+        "operationType": {
+            "enum": [
+                "manipulation"
+            ],
+            "type": "string"
         }
     },
-    "schemaId": "software-directory/ml/unit/execution/train",
-    "title": "train unit schema"
+    "schemaId": "software-directory/ml/unit/processing/data-transformation/manipulation",
+    "title": "scale and reduce unit schema",
+    "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9085648148148149%*

 * *Differences: {"'properties'": "{'operationType': {'enum': ['scale_and_reduce']}, 'inputData': {'properties': "*

 * *                 "{replace: OrderedDict([('scaler', OrderedDict([('description', 'type of scaler "*

 * *                 "to be applied'), ('type', 'string'), ('default', 'standard_scaler'), ('enum', "*

 * *                 "['standard_scaler'])])), ('perFeature', OrderedDict([('decription', 'per-feature "*

 * *                 "scaling data'), ('type', 'array'), ('items', OrderedDict([('type', 'object'), "*

 * *                 " […]*

```diff
@@ -4,47 +4,67 @@
         {
             "$ref": "../../../../../workflow/unit/processing.json"
         }
     ],
     "properties": {
         "inputData": {
             "properties": {
-                "cleanMissingData": {
-                    "default": true,
-                    "description": "whether to clean missing data, eg. NaN",
-                    "type": "boolean"
+                "perFeature": {
+                    "decription": "per-feature scaling data",
+                    "items": {
+                        "properties": {
+                            "mean": {
+                                "description": "mean value of the original training data",
+                                "type": "number"
+                            },
+                            "name": {
+                                "description": "feature/property name in 'flattened' format",
+                                "type": "string"
+                            },
+                            "scale": {
+                                "description": "scale multiplier for this feature/property",
+                                "type": "number"
+                            },
+                            "variance": {
+                                "description": "variance in original training data",
+                                "type": "number"
+                            }
+                        },
+                        "required": [
+                            "name",
+                            "scale"
+                        ],
+                        "type": "object"
+                    },
+                    "type": "array"
                 },
-                "removeDuplicateRows": {
-                    "default": true,
-                    "description": "whether to remove duplicate rows",
-                    "type": "boolean"
-                },
-                "replaceNoneValuesWith": {
-                    "default": 0,
-                    "description": "replace None values with a given value",
-                    "type": "number"
+                "scaler": {
+                    "default": "standard_scaler",
+                    "description": "type of scaler to be applied",
+                    "enum": [
+                        "standard_scaler"
+                    ],
+                    "type": "string"
                 }
             },
             "required": [
-                "cleanMissingData",
-                "removeDuplicateRows",
-                "replaceNoneValuesWith"
+                "scaler"
             ],
             "type": "object"
         },
         "operation": {
             "enum": [
                 "data_transformation"
             ],
             "type": "string"
         },
         "operationType": {
             "enum": [
-                "manipulation"
+                "scale_and_reduce"
             ],
             "type": "string"
         }
     },
-    "schemaId": "software-directory/ml/unit/processing/data-transformation/manipulation",
+    "schemaId": "software-directory/ml/unit/processing/data-transformation/scale-and-reduce",
     "title": "scale and reduce unit schema",
     "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/map.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6071428571428571%*

 * *Differences: {"'allOf'": "{0: {'$ref': '../unit.json'}}",*

 * * "'properties'": "{replace: OrderedDict([('type', OrderedDict([('enum', ['map'])])), "*

 * *                 "('workflowId', OrderedDict([('description', 'Id of workflow to run inside map'), "*

 * *                 "('type', 'string')])), ('input', OrderedDict([('description', 'Input information "*

 * *                 "for map.'), ('type', 'object'), ('properties', OrderedDict([('target', "*

 * *                 "OrderedDict([('description', 'Name of the target variable to substitu […]*

```diff
@@ -1,70 +1,67 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "../../../../../workflow/unit/processing.json"
+            "$ref": "../unit.json"
         }
     ],
     "properties": {
-        "inputData": {
+        "input": {
+            "description": "Input information for map.",
             "properties": {
-                "perFeature": {
-                    "decription": "per-feature scaling data",
+                "name": {
+                    "description": "Name of the variable inside the scope to retrieve `values` from. Optional if `values` is given.",
+                    "type": "string"
+                },
+                "scope": {
+                    "description": "Scope to retrieve `values` from, global or flowchartId. Optional if `values` is given.",
+                    "type": "string"
+                },
+                "target": {
+                    "description": "Name of the target variable to substitute using the values below. e.g. K_POINTS",
+                    "type": "string"
+                },
+                "useValues": {
+                    "type": "boolean"
+                },
+                "values": {
+                    "description": "Sequence of values for the target Jinja variable. Optional if `scope` and `name` are given. This can be used for map-reduce type parallel execution",
                     "items": {
-                        "properties": {
-                            "mean": {
-                                "description": "mean value of the original training data",
-                                "type": "number"
-                            },
-                            "name": {
-                                "description": "feature/property name in 'flattened' format",
+                        "oneOf": [
+                            {
                                 "type": "string"
                             },
-                            "scale": {
-                                "description": "scale multiplier for this feature/property",
+                            {
                                 "type": "number"
                             },
-                            "variance": {
-                                "description": "variance in original training data",
-                                "type": "number"
+                            {
+                                "type": "object"
                             }
-                        },
-                        "required": [
-                            "name",
-                            "scale"
-                        ],
-                        "type": "object"
+                        ]
                     },
                     "type": "array"
-                },
-                "scaler": {
-                    "default": "standard_scaler",
-                    "description": "type of scaler to be applied",
-                    "enum": [
-                        "standard_scaler"
-                    ],
-                    "type": "string"
                 }
             },
             "required": [
-                "scaler"
+                "target"
             ],
             "type": "object"
         },
-        "operation": {
+        "type": {
             "enum": [
-                "data_transformation"
-            ],
-            "type": "string"
+                "map"
+            ]
         },
-        "operationType": {
-            "enum": [
-                "scale_and_reduce"
-            ],
+        "workflowId": {
+            "description": "Id of workflow to run inside map",
             "type": "string"
         }
     },
-    "schemaId": "software-directory/ml/unit/processing/data-transformation/scale-and-reduce",
-    "title": "scale and reduce unit schema",
+    "required": [
+        "input",
+        "workflowId"
+    ],
+    "schemaId": "workflow/unit/map",
+    "title": "map unit schema",
     "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/espresso/arguments.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/espresso/arguments.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/espresso.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/espresso.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/nwchem.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/nwchem.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/modeling/vasp.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/modeling/vasp.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/scripting/jupyter-lab.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/scripting/jupyter-lab.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/scripting/python.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/scripting/python.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/software_directory/scripting/shell.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/software_directory/scripting/shell.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/system/base_entity_set.json` & `esse-2023.5.29.post0/schema/core/reference/exabyte.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('materialId', OrderedDict([('description', "*

 * *                 '"Material\'s identity. Used for protoProperties."), (\'type\', \'string\')])), '*

 * *                 '(\'jobId\', OrderedDict([(\'description\', "Job\'s identity"), (\'type\', '*

 * *                 "'string')])), ('unitId', OrderedDict([('description', 'Id of the unit that "*

 * *                 "extracted the result'), ('type', 'string')]))])}",*

 * * "'schemaId'": "'core/reference/exabyte'",*

 * * "'type'": "'object'",*

 * * ' […]*

```diff
@@ -1,34 +1,19 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "properties": {
-        "entitySetType": {
+        "jobId": {
+            "description": "Job's identity",
             "type": "string"
         },
-        "inSet": {
-            "items": {
-                "allOf": [
-                    {
-                        "$ref": "../system/entity_reference.json"
-                    },
-                    {
-                        "properties": {
-                            "index": {
-                                "type": "number"
-                            },
-                            "type": {
-                                "type": "string"
-                            }
-                        },
-                        "type": "object"
-                    }
-                ]
-            },
-            "type": "array"
+        "materialId": {
+            "description": "Material's identity. Used for protoProperties.",
+            "type": "string"
         },
-        "isEntitySet": {
-            "type": "boolean"
+        "unitId": {
+            "description": "Id of the unit that extracted the result",
+            "type": "string"
         }
     },
-    "schemaId": "system/base-entity-set",
-    "title": "extended base entity set schema"
+    "schemaId": "core/reference/exabyte",
+    "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/system/database_source.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/new_subworkflow.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5714285714285714%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('_id', OrderedDict([('description', 'subworkflow "*

 * *                 "identity'), ('type', 'string')])), ('name', OrderedDict([('description', "*

 * *                 "'Human-readable name of the subworkflow. e.g. Total-energy'), ('type', "*

 * *                 "'string')])), ('model', OrderedDict([('description', 'Model used inside the "*

 * *                 "subworkflow'), ('oneOf', [OrderedDict([('$ref', "*

 * *                 "'../models_directory/pb/qm/dft/ksdft.json')]), Ordere […]*

```diff
@@ -1,30 +1,66 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
-    "description": "information about a database source",
     "properties": {
-        "data": {
-            "description": "Original response from external source",
-            "type": "object"
-        },
-        "id": {
-            "description": "ID string for the materials uploaded from a third party source inside the third party source. For materialsproject.org an example ID is mp-32",
+        "_id": {
+            "description": "subworkflow identity",
             "type": "string"
         },
-        "origin": {
-            "description": "A flag that is true when material is initially imported from a third party * (as opposed to being independently designed from scratch).",
+        "application": {
+            "$ref": "../software/application.json",
+            "description": "information about the simulation engine/application."
+        },
+        "compute": {
+            "$ref": "../job/compute.json",
+            "description": "compute parameters"
+        },
+        "isDraft": {
+            "default": false,
+            "description": "Defines whether to store the results/properties extracted in this unit to properties collection",
             "type": "boolean"
         },
-        "source": {
-            "description": "Third party source name.",
+        "model": {
+            "description": "Model used inside the subworkflow",
+            "oneOf": [
+                {
+                    "$ref": "../models_directory/pb/qm/dft/ksdft.json"
+                },
+                {
+                    "$ref": "../models_directory/st/det/ml.json"
+                },
+                {
+                    "$ref": "../models_directory/unknown.json"
+                }
+            ]
+        },
+        "name": {
+            "description": "Human-readable name of the subworkflow. e.g. Total-energy",
             "type": "string"
+        },
+        "properties": {
+            "description": "Array of characteristic properties calculated by this subworkflow",
+            "items": {
+                "description": "property names, eg. `band_gaps`, `band_structure`",
+                "type": "string"
+            },
+            "type": "array"
+        },
+        "units": {
+            "description": "Contains the Units of the subworkflow",
+            "items": {
+                "$ref": "unit.json"
+            },
+            "type": "array"
         }
     },
     "required": [
-        "id",
-        "source",
-        "origin"
+        "_id",
+        "name",
+        "units",
+        "model",
+        "application",
+        "properties"
     ],
-    "schemaId": "system/database-source",
-    "title": "database source schema",
+    "schemaId": "workflow/new-subworkflow",
+    "title": "subworkflow schema",
     "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/system/file_source.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/system/file_source.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/system/history.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/system/history.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/system/job_extended.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/io.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.35714285714285715%*

 * *Differences: {"'allOf'": "[OrderedDict([('$ref', '../unit.json')])]",*

 * * "'properties'": "{replace: OrderedDict([('type', OrderedDict([('enum', ['io'])])), ('subtype', "*

 * *                 "OrderedDict([('enum', ['input', 'output', 'dataFrame'])])), ('source', "*

 * *                 "OrderedDict([('enum', ['api', 'db', 'object_storage'])])), ('input', "*

 * *                 "OrderedDict([('type', 'array'), ('items', OrderedDict([('anyOf', "*

 * *                 "[OrderedDict([('$ref', 'io/api.json')]), OrderedDict([('$ref', 'io/db.json […]*

```diff
@@ -1,39 +1,53 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
+    "allOf": [
+        {
+            "$ref": "../unit.json"
+        }
+    ],
     "properties": {
-        "_materials": {
+        "input": {
             "items": {
-                "allOf": [
+                "anyOf": [
+                    {
+                        "$ref": "io/api.json"
+                    },
                     {
-                        "$ref": "entity_reference.json"
+                        "$ref": "io/db.json"
+                    },
+                    {
+                        "$ref": "io/object_storage.json"
                     }
                 ]
             },
             "type": "array"
         },
-        "_materialsSet": {
-            "allOf": [
-                {
-                    "$ref": "entity_reference.json"
-                }
+        "source": {
+            "enum": [
+                "api",
+                "db",
+                "object_storage"
             ]
         },
-        "dataset": {
-            "type": "object"
-        },
-        "isExternal": {
-            "type": "boolean"
-        },
-        "mode": {
-            "type": "string"
-        },
-        "purged": {
-            "type": "boolean"
+        "subtype": {
+            "enum": [
+                "input",
+                "output",
+                "dataFrame"
+            ]
         },
-        "purgedAt": {
-            "type": "number"
+        "type": {
+            "enum": [
+                "io"
+            ]
         }
     },
-    "schemaId": "system/job-extended",
-    "title": "extended job schema"
+    "required": [
+        "subtype",
+        "source",
+        "input"
+    ],
+    "schemaId": "workflow/unit/io",
+    "title": "data IO unit schema",
+    "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/system/message.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/system/message.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/system/status.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/system/status.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/base_flow.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/base_flow.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/new_subworkflow.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5926355390641105%*

 * *Differences: {"'allOf'": "[OrderedDict([('$ref', 'in_memory_entity/named_defaultable_has_metadata.json')])]",*

 * * "'properties'": "{'properties': {'description': 'Array of characteristic properties calculated by "*

 * *                 "this workflow (TODO: add enums)', 'items': {'oneOf': [OrderedDict([('type', "*

 * *                 "'string')]), OrderedDict([('type', 'object')])], delete: ['type']}}, 'units': "*

 * *                 "{'description': 'Contains the Units of the Workflow', 'items': {replace: "*

 * *                 "OrderedDi […]*

```diff
@@ -1,66 +1,89 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
+    "allOf": [
+        {
+            "$ref": "in_memory_entity/named_defaultable_has_metadata.json"
+        }
+    ],
     "properties": {
-        "_id": {
-            "description": "subworkflow identity",
-            "type": "string"
-        },
-        "application": {
-            "$ref": "../software/application.json",
-            "description": "information about the simulation engine/application."
-        },
-        "compute": {
-            "$ref": "../job/compute.json",
-            "description": "compute parameters"
-        },
-        "isDraft": {
-            "default": false,
-            "description": "Defines whether to store the results/properties extracted in this unit to properties collection",
+        "isUsingDataset": {
+            "description": "Whether to use the dataset tab in the job designer. Mutually exclusive with using the materials tab.",
             "type": "boolean"
         },
-        "model": {
-            "description": "Model used inside the subworkflow",
-            "oneOf": [
-                {
-                    "$ref": "../models_directory/pb/qm/dft/ksdft.json"
-                },
-                {
-                    "$ref": "../models_directory/st/det/ml.json"
-                },
-                {
-                    "$ref": "../models_directory/unknown.json"
-                }
-            ]
-        },
-        "name": {
-            "description": "Human-readable name of the subworkflow. e.g. Total-energy",
-            "type": "string"
-        },
         "properties": {
-            "description": "Array of characteristic properties calculated by this subworkflow",
+            "description": "Array of characteristic properties calculated by this workflow (TODO: add enums)",
             "items": {
                 "description": "property names, eg. `band_gaps`, `band_structure`",
-                "type": "string"
+                "oneOf": [
+                    {
+                        "type": "string"
+                    },
+                    {
+                        "type": "object"
+                    }
+                ]
+            },
+            "type": "array"
+        },
+        "subworkflows": {
+            "description": "Array of subworkflows. Subworkflow can be an instance of workflow to allow for nesting",
+            "items": {
+                "anyOf": [
+                    {
+                        "$ref": "workflow/subworkflow.json"
+                    }
+                ]
             },
             "type": "array"
         },
         "units": {
-            "description": "Contains the Units of the subworkflow",
+            "description": "Contains the Units of the Workflow",
+            "items": {
+                "oneOf": [
+                    {
+                        "$ref": "workflow/unit.json"
+                    },
+                    {
+                        "$ref": "workflow/unit/io.json"
+                    },
+                    {
+                        "$ref": "workflow/unit/map.json"
+                    },
+                    {
+                        "$ref": "workflow/unit/reduce.json"
+                    },
+                    {
+                        "$ref": "workflow/unit/condition.json"
+                    },
+                    {
+                        "$ref": "workflow/unit/assertion.json"
+                    },
+                    {
+                        "$ref": "workflow/unit/execution.json"
+                    },
+                    {
+                        "$ref": "workflow/unit/assignment.json"
+                    },
+                    {
+                        "$ref": "workflow/unit/processing.json"
+                    }
+                ]
+            },
+            "type": "array"
+        },
+        "workflows": {
+            "description": "Array of workflows with the same schema as the current one.",
             "items": {
-                "$ref": "unit.json"
+                "type": "object"
             },
             "type": "array"
         }
     },
     "required": [
-        "_id",
-        "name",
         "units",
-        "model",
-        "application",
-        "properties"
+        "subworkflows"
     ],
-    "schemaId": "workflow/new-subworkflow",
-    "title": "subworkflow schema",
+    "schemaId": "workflow",
+    "title": "workflow schema",
     "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/assertion.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/io/api.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5714285714285714%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('endpoint', OrderedDict([('description', 'rest API "*

 * *                 "endpoint'), ('type', 'string')])), ('endpoint_options', "*

 * *                 "OrderedDict([('description', 'rest API endpoint options'), ('type', "*

 * *                 "'object')])), ('name', OrderedDict([('description', 'the name of the variable in "*

 * *                 "local scope to save the data under'), ('type', 'string')]))])}",*

 * * "'required'": "['endpoint', 'endpoint_options']",*

 * * "'schemaId'": "'w […]*

```diff
@@ -1,28 +1,24 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
-    "allOf": [
-        {
-            "$ref": "../unit.json"
-        }
-    ],
     "properties": {
-        "errorMessage": {
+        "endpoint": {
+            "description": "rest API endpoint",
             "type": "string"
         },
-        "statement": {
-            "type": "string"
+        "endpoint_options": {
+            "description": "rest API endpoint options",
+            "type": "object"
         },
-        "type": {
-            "enum": [
-                "assertion"
-            ]
+        "name": {
+            "description": "the name of the variable in local scope to save the data under",
+            "type": "string"
         }
     },
     "required": [
-        "name",
-        "statement"
+        "endpoint",
+        "endpoint_options"
     ],
-    "schemaId": "workflow/unit/assertion",
-    "title": "assignment unit schema",
+    "schemaId": "workflow/unit/io/api",
+    "title": "data IO rest API input schema",
     "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/assignment.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/assignment.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/condition.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/condition.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/execution.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/execution.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/input/_input.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/input/_input.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/input/_inputItem.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/input/_inputItem.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemId.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemId.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemScope.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemScope.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/io/api.json` & `esse-2023.5.29.post0/schema/project.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'allOf'": "[OrderedDict([('description', 'in-memory entity'), ('$ref', "*

 * *            "'in_memory_entity/named_defaultable_has_metadata.json')])]",*

 * * "'properties'": "{replace: OrderedDict([('gid', OrderedDict([('description', 'project GID'), "*

 * *                 "('type', 'number')])), ('clusterBasedChargeRates', OrderedDict([('description', "*

 * *                 "'charge rates info for project'), ('type', 'array'), ('items', "*

 * *                 "OrderedDict([('type', 'object'), ('properties', OrderedDict([('rat […]*

```diff
@@ -1,24 +1,40 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
+    "allOf": [
+        {
+            "$ref": "in_memory_entity/named_defaultable_has_metadata.json",
+            "description": "in-memory entity"
+        }
+    ],
     "properties": {
-        "endpoint": {
-            "description": "rest API endpoint",
-            "type": "string"
+        "clusterBasedChargeRates": {
+            "description": "charge rates info for project",
+            "items": {
+                "properties": {
+                    "hostname": {
+                        "type": "string"
+                    },
+                    "rate": {
+                        "type": "number"
+                    },
+                    "timestamp": {
+                        "type": "number"
+                    }
+                },
+                "type": "object"
+            },
+            "type": "array"
         },
-        "endpoint_options": {
-            "description": "rest API endpoint options",
-            "type": "object"
+        "gid": {
+            "description": "project GID",
+            "type": "number"
         },
-        "name": {
-            "description": "the name of the variable in local scope to save the data under",
-            "type": "string"
+        "isExternal": {
+            "default": false,
+            "type": "boolean"
         }
     },
-    "required": [
-        "endpoint",
-        "endpoint_options"
-    ],
-    "schemaId": "workflow/unit/io/api",
-    "title": "data IO rest API input schema",
+    "schemaId": "project",
+    "title": "project schema",
     "type": "object"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/io/db.json` & `esse-2023.5.29.post0/schema/system/timestampable.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'properties'": "OrderedDict([('createdAt', OrderedDict([('description', 'entity creation time'), "*

 * *                 "('type', 'string'), ('format', 'date-time')])), ('updatedAt', "*

 * *                 "OrderedDict([('description', 'entity last modification time'), ('type', "*

 * *                 "'string'), ('format', 'date-time')])), ('createdBy', OrderedDict([('oneOf', "*

 * *                 "[OrderedDict([('type', 'string')]), OrderedDict([('type', 'number')])])])), "*

 * *                 "('updatedBy', OrderedDict([ […]*

```diff
@@ -1,39 +1,37 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
-    "oneOf": [
-        {
-            "properties": {
-                "ids": {
-                    "description": "IDs of item to retrieve from db",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
+    "properties": {
+        "createdAt": {
+            "description": "entity creation time",
+            "format": "date-time",
+            "type": "string"
+        },
+        "createdBy": {
+            "oneOf": [
+                {
+                    "type": "string"
+                },
+                {
+                    "type": "number"
                 }
-            },
-            "required": [
-                "ids"
             ]
         },
-        {
-            "properties": {
-                "collection": {
-                    "description": "db collection name",
+        "updatedAt": {
+            "description": "entity last modification time",
+            "format": "date-time",
+            "type": "string"
+        },
+        "updatedBy": {
+            "oneOf": [
+                {
                     "type": "string"
                 },
-                "draft": {
-                    "default": true,
-                    "description": "whether the result should be saved as draft",
-                    "type": "boolean"
+                {
+                    "type": "number"
                 }
-            },
-            "required": [
-                "collection",
-                "draft"
             ]
         }
-    ],
-    "schemaId": "workflow/unit/io/db",
-    "title": "data IO database input/output schema",
-    "type": "object"
+    },
+    "schemaId": "system/timestampable",
+    "title": "timestampable entity schema"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/io/object_storage.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/io/object_storage.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/io.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/properties_directory/non-scalar/average_potential_profile.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4642857142857143%*

 * *Differences: {"'allOf'": "{0: {'$ref': '../../core/abstract/2d_plot.json'}}",*

 * * "'properties'": "{replace: OrderedDict([('xAxis', OrderedDict([('properties', "*

 * *                 "OrderedDict([('label', OrderedDict([('enum', ['z coordinate'])])), ('units', "*

 * *                 "OrderedDict([('$ref', '../../definitions/units.json#/length')]))]))])), "*

 * *                 "('yAxis', OrderedDict([('properties', OrderedDict([('label', "*

 * *                 "OrderedDict([('enum', ['energy'])])), ('units', OrderedDict([('$ref', "*

 * *       […]*

```diff
@@ -1,53 +1,41 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "allOf": [
         {
-            "$ref": "../unit.json"
+            "$ref": "../../core/abstract/2d_plot.json"
         }
     ],
     "properties": {
-        "input": {
-            "items": {
-                "anyOf": [
-                    {
-                        "$ref": "io/api.json"
-                    },
-                    {
-                        "$ref": "io/db.json"
-                    },
-                    {
-                        "$ref": "io/object_storage.json"
-                    }
-                ]
-            },
-            "type": "array"
-        },
-        "source": {
+        "name": {
             "enum": [
-                "api",
-                "db",
-                "object_storage"
+                "average_potential_profile"
             ]
         },
-        "subtype": {
-            "enum": [
-                "input",
-                "output",
-                "dataFrame"
-            ]
+        "xAxis": {
+            "properties": {
+                "label": {
+                    "enum": [
+                        "z coordinate"
+                    ]
+                },
+                "units": {
+                    "$ref": "../../definitions/units.json#/length"
+                }
+            }
         },
-        "type": {
-            "enum": [
-                "io"
-            ]
+        "yAxis": {
+            "properties": {
+                "label": {
+                    "enum": [
+                        "energy"
+                    ]
+                },
+                "units": {
+                    "$ref": "../../definitions/units.json#/energy"
+                }
+            }
         }
     },
-    "required": [
-        "subtype",
-        "source",
-        "input"
-    ],
-    "schemaId": "workflow/unit/io",
-    "title": "data IO unit schema",
-    "type": "object"
+    "schemaId": "properties-directory/non-scalar/average-potential-profile",
+    "title": "average potential profile schema"
 }
```

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/processing.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/processing.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/reduce.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_items.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_items.json`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/data/schema/workflow/unit.json` & `esse-2023.5.29.post0/src/py/esse/data/schema/workflow/unit.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95625%*

 * *Differences: {"'allOf'": "{0: {'$ref': '../in_memory_entity/named_defaultable_runtime_items.json'}}",*

 * * "'properties'": "{'_id': OrderedDict([('type', 'string')]), 'isDraft': OrderedDict([('type', "*

 * *                 "'boolean')])}"}*

```diff
@@ -1,16 +1,19 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "additionalProperties": true,
     "allOf": [
         {
-            "$ref": "../system/tags.json"
+            "$ref": "../in_memory_entity/named_defaultable_runtime_items.json"
         }
     ],
     "properties": {
+        "_id": {
+            "type": "string"
+        },
         "context": {
             "type": "object"
         },
         "enableRender": {
             "description": "Whether Rupy should attempt to use Jinja templating to add context variables into the unit",
             "type": "boolean"
         },
@@ -18,14 +21,17 @@
             "description": "Identity of the unit in the workflow. Used to trace the execution flow of the workflow.",
             "type": "string"
         },
         "head": {
             "description": "Whether this unit is the first one to be executed.",
             "type": "boolean"
         },
+        "isDraft": {
+            "type": "boolean"
+        },
         "name": {
             "description": "name of the unit. e.g. pw_scf",
             "type": "string"
         },
         "next": {
             "description": "Next unit's flowchartId. If empty, the current unit is the last.",
             "type": "string"
```

### Comparing `esse-2022.9.6.post0/src/py/esse/functionals.py` & `esse-2023.5.29.post0/src/py/esse/functionals.py`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/tests/validate.py` & `esse-2023.5.29.post0/src/py/esse/tests/validate.py`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse/utils.py` & `esse-2023.5.29.post0/src/py/esse/utils.py`

 * *Files identical despite different names*

### Comparing `esse-2022.9.6.post0/src/py/esse.egg-info/PKG-INFO` & `esse-2023.5.29.post0/src/py/esse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esse
-Version: 2022.9.6.post0
+Version: 2023.5.29.post0
 Summary: Exabyte Source of Schemas and Examples
 Home-page: https://github.com/Exabyte-io/exabyte-esse
 Author: Exabyte Inc.
 Author-email: info@exabyte.io
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `esse-2022.9.6.post0/src/py/esse.egg-info/SOURCES.txt` & `esse-2023.5.29.post0/src/py/esse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 example/element.json
 example/job.json
 example/material.json
 example/method.json
 example/model.json
 example/new_model.json
 example/project.json
-example/property.json
 example/workflow.json
 example/core/reference.json
 example/core/abstract/2d_data.json
 example/core/abstract/2d_plot.json
 example/core/abstract/3d_grid.json
 example/core/abstract/3d_tensor.json
 example/core/abstract/3d_vector_basis.json
@@ -111,14 +110,15 @@
 example/properties_directory/scalar/formation_energy.json
 example/properties_directory/scalar/ionization_potential.json
 example/properties_directory/scalar/pressure.json
 example/properties_directory/scalar/reaction_energy_barrier.json
 example/properties_directory/scalar/surface_energy.json
 example/properties_directory/scalar/total_energy.json
 example/properties_directory/scalar/total_force.json
+example/properties_directory/scalar/valence_band_offset.json
 example/properties_directory/scalar/zero_point_energy.json
 example/properties_directory/structural/atomic_forces.json
 example/properties_directory/structural/basis.json
 example/properties_directory/structural/density.json
 example/properties_directory/structural/elemental_ratio.json
 example/properties_directory/structural/inchi.json
 example/properties_directory/structural/inchi_key.json
@@ -134,14 +134,17 @@
 example/properties_directory/structural/basis/atomic_element.json
 example/properties_directory/structural/basis/bonds.json
 example/properties_directory/structural/lattice/lattice_bravais.json
 example/properties_directory/structural/lattice/lattice_vectors.json
 example/properties_directory/workflow/convergence/electronic.json
 example/properties_directory/workflow/convergence/ionic.json
 example/properties_directory/workflow/convergence/kpoint.json
+example/property/best.json
+example/property/raw.json
+example/property/refined.json
 example/software/application.json
 example/software/executable.json
 example/software/flavor.json
 example/software/template.json
 example/software_directory/ml/exabyteml.json
 example/software_directory/ml/unit/execution/initialize.json
 example/software_directory/ml/unit/execution/score.json
@@ -189,35 +192,36 @@
 schema/element.json
 schema/job.json
 schema/material.json
 schema/method.json
 schema/model.json
 schema/new_model.json
 schema/project.json
-schema/property.json
 schema/workflow.json
 schema/core/reference.json
 schema/core/abstract/2d_data.json
 schema/core/abstract/2d_plot.json
 schema/core/abstract/3d_grid.json
 schema/core/abstract/3d_tensor.json
 schema/core/abstract/3d_vector_basis.json
 schema/core/abstract/point.json
 schema/core/abstract/vector.json
 schema/core/primitive/1d_data_series.json
 schema/core/primitive/3d_lattice.json
 schema/core/primitive/array_of_3_booleans.json
 schema/core/primitive/array_of_3_numbers.json
 schema/core/primitive/array_of_ids.json
+schema/core/primitive/array_of_numbers.json
 schema/core/primitive/array_of_strings.json
 schema/core/primitive/axis.json
 schema/core/primitive/scalar.json
 schema/core/primitive/slugified_entry.json
 schema/core/primitive/slugified_entry_or_slug.json
 schema/core/primitive/string.json
+schema/core/reference/exabyte.json
 schema/core/reference/experiment.json
 schema/core/reference/literature.json
 schema/core/reference/modeling.json
 schema/core/reference/experiment/condition.json
 schema/core/reference/experiment/location.json
 schema/core/reference/literature/name.json
 schema/core/reference/literature/pages.json
@@ -226,14 +230,20 @@
 schema/core/reusable/atomic_strings.json
 schema/core/reusable/atomic_vectors.json
 schema/core/reusable/band_gap.json
 schema/core/reusable/energy.json
 schema/core/reusable/file_metadata.json
 schema/core/reusable/object_storage_container_data.json
 schema/definitions/units.json
+schema/in_memory_entity/base.json
+schema/in_memory_entity/defaultable.json
+schema/in_memory_entity/named.json
+schema/in_memory_entity/named_defaultable.json
+schema/in_memory_entity/named_defaultable_has_metadata.json
+schema/in_memory_entity/named_defaultable_runtime_items.json
 schema/job/compute.json
 schema/material/conventional.json
 schema/methods_directory/local-orbital.json
 schema/methods_directory/pseudopotential.json
 schema/methods_directory/regression.json
 schema/methods_directory/unknown.json
 schema/methods_directory/local_orbital/definitions/basis_sets.json
@@ -338,14 +348,15 @@
 schema/models_directory/st/det.json
 schema/models_directory/st/det/ml.json
 schema/properties_directory/derived_properties.json
 schema/properties_directory/electronic_configuration.json
 schema/properties_directory/elemental/atomic_radius.json
 schema/properties_directory/elemental/electronegativity.json
 schema/properties_directory/elemental/ionization_potential.json
+schema/properties_directory/non-scalar/average_potential_profile.json
 schema/properties_directory/non-scalar/band_gaps.json
 schema/properties_directory/non-scalar/band_structure.json
 schema/properties_directory/non-scalar/charge_density_profile.json
 schema/properties_directory/non-scalar/density_of_states.json
 schema/properties_directory/non-scalar/file_content.json
 schema/properties_directory/non-scalar/phonon_dispersions.json
 schema/properties_directory/non-scalar/phonon_dos.json
@@ -359,14 +370,15 @@
 schema/properties_directory/scalar/formation_energy.json
 schema/properties_directory/scalar/ionization_potential.json
 schema/properties_directory/scalar/pressure.json
 schema/properties_directory/scalar/reaction_energy_barrier.json
 schema/properties_directory/scalar/surface_energy.json
 schema/properties_directory/scalar/total_energy.json
 schema/properties_directory/scalar/total_force.json
+schema/properties_directory/scalar/valence_band_offset.json
 schema/properties_directory/scalar/zero_point_energy.json
 schema/properties_directory/structural/atomic_forces.json
 schema/properties_directory/structural/basis.json
 schema/properties_directory/structural/density.json
 schema/properties_directory/structural/elemental_ratio.json
 schema/properties_directory/structural/inchi.json
 schema/properties_directory/structural/inchi_key.json
@@ -385,14 +397,18 @@
 schema/properties_directory/structural/lattice/lattice_vectors.json
 schema/properties_directory/structural/patterns/functional_group.json
 schema/properties_directory/structural/patterns/ring.json
 schema/properties_directory/structural/patterns/special_bond.json
 schema/properties_directory/workflow/convergence/electronic.json
 schema/properties_directory/workflow/convergence/ionic.json
 schema/properties_directory/workflow/convergence/kpoint.json
+schema/property/best.json
+schema/property/raw.json
+schema/property/refined.json
+schema/property/source.json
 schema/software/application.json
 schema/software/executable.json
 schema/software/flavor.json
 schema/software/template.json
 schema/software_directory/ml/exabyteml.json
 schema/software_directory/ml/unit/execution.json
 schema/software_directory/ml/unit/processing.json
@@ -414,41 +430,38 @@
 schema/software_directory/scripting/python.json
 schema/software_directory/scripting/shell.json
 schema/software_directory/scripting/unit/execution.json
 schema/system/_material.json
 schema/system/_parent_job.json
 schema/system/_project.json
 schema/system/bankable.json
-schema/system/bankable_entity.json
-schema/system/base_entity_set.json
 schema/system/creator.json
 schema/system/creator_account.json
 schema/system/database_source.json
 schema/system/defaultable.json
-schema/system/description_object.json
-schema/system/entity.json
+schema/system/description.json
 schema/system/entity_reference.json
 schema/system/file_source.json
 schema/system/history.json
+schema/system/in_set.json
 schema/system/is_multi_material.json
 schema/system/is_outdated.json
 schema/system/job_extended.json
 schema/system/message.json
 schema/system/metadata.json
 schema/system/name.json
 schema/system/owner.json
 schema/system/schema_version.json
 schema/system/scope.json
+schema/system/set.json
 schema/system/sharing.json
 schema/system/soft_removable.json
 schema/system/status.json
-schema/system/system_name.json
 schema/system/tags.json
 schema/system/timestampable.json
-schema/system/unit_extended.json
 schema/system/use_values.json
 schema/workflow/base_flow.json
 schema/workflow/new_subworkflow.json
 schema/workflow/subworkflow.json
 schema/workflow/unit.json
 schema/workflow/unit/assertion.json
 schema/workflow/unit/assignment.json
@@ -495,15 +508,14 @@
 src/py/esse/data/example/element.json
 src/py/esse/data/example/job.json
 src/py/esse/data/example/material.json
 src/py/esse/data/example/method.json
 src/py/esse/data/example/model.json
 src/py/esse/data/example/new_model.json
 src/py/esse/data/example/project.json
-src/py/esse/data/example/property.json
 src/py/esse/data/example/workflow.json
 src/py/esse/data/example/core/reference.json
 src/py/esse/data/example/core/abstract/2d_data.json
 src/py/esse/data/example/core/abstract/2d_plot.json
 src/py/esse/data/example/core/abstract/3d_grid.json
 src/py/esse/data/example/core/abstract/3d_tensor.json
 src/py/esse/data/example/core/abstract/3d_vector_basis.json
@@ -588,14 +600,15 @@
 src/py/esse/data/example/properties_directory/scalar/formation_energy.json
 src/py/esse/data/example/properties_directory/scalar/ionization_potential.json
 src/py/esse/data/example/properties_directory/scalar/pressure.json
 src/py/esse/data/example/properties_directory/scalar/reaction_energy_barrier.json
 src/py/esse/data/example/properties_directory/scalar/surface_energy.json
 src/py/esse/data/example/properties_directory/scalar/total_energy.json
 src/py/esse/data/example/properties_directory/scalar/total_force.json
+src/py/esse/data/example/properties_directory/scalar/valence_band_offset.json
 src/py/esse/data/example/properties_directory/scalar/zero_point_energy.json
 src/py/esse/data/example/properties_directory/structural/atomic_forces.json
 src/py/esse/data/example/properties_directory/structural/basis.json
 src/py/esse/data/example/properties_directory/structural/density.json
 src/py/esse/data/example/properties_directory/structural/elemental_ratio.json
 src/py/esse/data/example/properties_directory/structural/inchi.json
 src/py/esse/data/example/properties_directory/structural/inchi_key.json
@@ -611,14 +624,17 @@
 src/py/esse/data/example/properties_directory/structural/basis/atomic_element.json
 src/py/esse/data/example/properties_directory/structural/basis/bonds.json
 src/py/esse/data/example/properties_directory/structural/lattice/lattice_bravais.json
 src/py/esse/data/example/properties_directory/structural/lattice/lattice_vectors.json
 src/py/esse/data/example/properties_directory/workflow/convergence/electronic.json
 src/py/esse/data/example/properties_directory/workflow/convergence/ionic.json
 src/py/esse/data/example/properties_directory/workflow/convergence/kpoint.json
+src/py/esse/data/example/property/best.json
+src/py/esse/data/example/property/raw.json
+src/py/esse/data/example/property/refined.json
 src/py/esse/data/example/software/application.json
 src/py/esse/data/example/software/executable.json
 src/py/esse/data/example/software/flavor.json
 src/py/esse/data/example/software/template.json
 src/py/esse/data/example/software_directory/ml/exabyteml.json
 src/py/esse/data/example/software_directory/ml/unit/execution/initialize.json
 src/py/esse/data/example/software_directory/ml/unit/execution/score.json
@@ -666,35 +682,36 @@
 src/py/esse/data/schema/element.json
 src/py/esse/data/schema/job.json
 src/py/esse/data/schema/material.json
 src/py/esse/data/schema/method.json
 src/py/esse/data/schema/model.json
 src/py/esse/data/schema/new_model.json
 src/py/esse/data/schema/project.json
-src/py/esse/data/schema/property.json
 src/py/esse/data/schema/workflow.json
 src/py/esse/data/schema/core/reference.json
 src/py/esse/data/schema/core/abstract/2d_data.json
 src/py/esse/data/schema/core/abstract/2d_plot.json
 src/py/esse/data/schema/core/abstract/3d_grid.json
 src/py/esse/data/schema/core/abstract/3d_tensor.json
 src/py/esse/data/schema/core/abstract/3d_vector_basis.json
 src/py/esse/data/schema/core/abstract/point.json
 src/py/esse/data/schema/core/abstract/vector.json
 src/py/esse/data/schema/core/primitive/1d_data_series.json
 src/py/esse/data/schema/core/primitive/3d_lattice.json
 src/py/esse/data/schema/core/primitive/array_of_3_booleans.json
 src/py/esse/data/schema/core/primitive/array_of_3_numbers.json
 src/py/esse/data/schema/core/primitive/array_of_ids.json
+src/py/esse/data/schema/core/primitive/array_of_numbers.json
 src/py/esse/data/schema/core/primitive/array_of_strings.json
 src/py/esse/data/schema/core/primitive/axis.json
 src/py/esse/data/schema/core/primitive/scalar.json
 src/py/esse/data/schema/core/primitive/slugified_entry.json
 src/py/esse/data/schema/core/primitive/slugified_entry_or_slug.json
 src/py/esse/data/schema/core/primitive/string.json
+src/py/esse/data/schema/core/reference/exabyte.json
 src/py/esse/data/schema/core/reference/experiment.json
 src/py/esse/data/schema/core/reference/literature.json
 src/py/esse/data/schema/core/reference/modeling.json
 src/py/esse/data/schema/core/reference/experiment/condition.json
 src/py/esse/data/schema/core/reference/experiment/location.json
 src/py/esse/data/schema/core/reference/literature/name.json
 src/py/esse/data/schema/core/reference/literature/pages.json
@@ -703,14 +720,20 @@
 src/py/esse/data/schema/core/reusable/atomic_strings.json
 src/py/esse/data/schema/core/reusable/atomic_vectors.json
 src/py/esse/data/schema/core/reusable/band_gap.json
 src/py/esse/data/schema/core/reusable/energy.json
 src/py/esse/data/schema/core/reusable/file_metadata.json
 src/py/esse/data/schema/core/reusable/object_storage_container_data.json
 src/py/esse/data/schema/definitions/units.json
+src/py/esse/data/schema/in_memory_entity/base.json
+src/py/esse/data/schema/in_memory_entity/defaultable.json
+src/py/esse/data/schema/in_memory_entity/named.json
+src/py/esse/data/schema/in_memory_entity/named_defaultable.json
+src/py/esse/data/schema/in_memory_entity/named_defaultable_has_metadata.json
+src/py/esse/data/schema/in_memory_entity/named_defaultable_runtime_items.json
 src/py/esse/data/schema/job/compute.json
 src/py/esse/data/schema/material/conventional.json
 src/py/esse/data/schema/methods_directory/local-orbital.json
 src/py/esse/data/schema/methods_directory/pseudopotential.json
 src/py/esse/data/schema/methods_directory/regression.json
 src/py/esse/data/schema/methods_directory/unknown.json
 src/py/esse/data/schema/methods_directory/local_orbital/definitions/basis_sets.json
@@ -815,14 +838,15 @@
 src/py/esse/data/schema/models_directory/st/det.json
 src/py/esse/data/schema/models_directory/st/det/ml.json
 src/py/esse/data/schema/properties_directory/derived_properties.json
 src/py/esse/data/schema/properties_directory/electronic_configuration.json
 src/py/esse/data/schema/properties_directory/elemental/atomic_radius.json
 src/py/esse/data/schema/properties_directory/elemental/electronegativity.json
 src/py/esse/data/schema/properties_directory/elemental/ionization_potential.json
+src/py/esse/data/schema/properties_directory/non-scalar/average_potential_profile.json
 src/py/esse/data/schema/properties_directory/non-scalar/band_gaps.json
 src/py/esse/data/schema/properties_directory/non-scalar/band_structure.json
 src/py/esse/data/schema/properties_directory/non-scalar/charge_density_profile.json
 src/py/esse/data/schema/properties_directory/non-scalar/density_of_states.json
 src/py/esse/data/schema/properties_directory/non-scalar/file_content.json
 src/py/esse/data/schema/properties_directory/non-scalar/phonon_dispersions.json
 src/py/esse/data/schema/properties_directory/non-scalar/phonon_dos.json
@@ -836,14 +860,15 @@
 src/py/esse/data/schema/properties_directory/scalar/formation_energy.json
 src/py/esse/data/schema/properties_directory/scalar/ionization_potential.json
 src/py/esse/data/schema/properties_directory/scalar/pressure.json
 src/py/esse/data/schema/properties_directory/scalar/reaction_energy_barrier.json
 src/py/esse/data/schema/properties_directory/scalar/surface_energy.json
 src/py/esse/data/schema/properties_directory/scalar/total_energy.json
 src/py/esse/data/schema/properties_directory/scalar/total_force.json
+src/py/esse/data/schema/properties_directory/scalar/valence_band_offset.json
 src/py/esse/data/schema/properties_directory/scalar/zero_point_energy.json
 src/py/esse/data/schema/properties_directory/structural/atomic_forces.json
 src/py/esse/data/schema/properties_directory/structural/basis.json
 src/py/esse/data/schema/properties_directory/structural/density.json
 src/py/esse/data/schema/properties_directory/structural/elemental_ratio.json
 src/py/esse/data/schema/properties_directory/structural/inchi.json
 src/py/esse/data/schema/properties_directory/structural/inchi_key.json
@@ -862,14 +887,18 @@
 src/py/esse/data/schema/properties_directory/structural/lattice/lattice_vectors.json
 src/py/esse/data/schema/properties_directory/structural/patterns/functional_group.json
 src/py/esse/data/schema/properties_directory/structural/patterns/ring.json
 src/py/esse/data/schema/properties_directory/structural/patterns/special_bond.json
 src/py/esse/data/schema/properties_directory/workflow/convergence/electronic.json
 src/py/esse/data/schema/properties_directory/workflow/convergence/ionic.json
 src/py/esse/data/schema/properties_directory/workflow/convergence/kpoint.json
+src/py/esse/data/schema/property/best.json
+src/py/esse/data/schema/property/raw.json
+src/py/esse/data/schema/property/refined.json
+src/py/esse/data/schema/property/source.json
 src/py/esse/data/schema/software/application.json
 src/py/esse/data/schema/software/executable.json
 src/py/esse/data/schema/software/flavor.json
 src/py/esse/data/schema/software/template.json
 src/py/esse/data/schema/software_directory/ml/exabyteml.json
 src/py/esse/data/schema/software_directory/ml/unit/execution.json
 src/py/esse/data/schema/software_directory/ml/unit/processing.json
@@ -891,41 +920,38 @@
 src/py/esse/data/schema/software_directory/scripting/python.json
 src/py/esse/data/schema/software_directory/scripting/shell.json
 src/py/esse/data/schema/software_directory/scripting/unit/execution.json
 src/py/esse/data/schema/system/_material.json
 src/py/esse/data/schema/system/_parent_job.json
 src/py/esse/data/schema/system/_project.json
 src/py/esse/data/schema/system/bankable.json
-src/py/esse/data/schema/system/bankable_entity.json
-src/py/esse/data/schema/system/base_entity_set.json
 src/py/esse/data/schema/system/creator.json
 src/py/esse/data/schema/system/creator_account.json
 src/py/esse/data/schema/system/database_source.json
 src/py/esse/data/schema/system/defaultable.json
-src/py/esse/data/schema/system/description_object.json
-src/py/esse/data/schema/system/entity.json
+src/py/esse/data/schema/system/description.json
 src/py/esse/data/schema/system/entity_reference.json
 src/py/esse/data/schema/system/file_source.json
 src/py/esse/data/schema/system/history.json
+src/py/esse/data/schema/system/in_set.json
 src/py/esse/data/schema/system/is_multi_material.json
 src/py/esse/data/schema/system/is_outdated.json
 src/py/esse/data/schema/system/job_extended.json
 src/py/esse/data/schema/system/message.json
 src/py/esse/data/schema/system/metadata.json
 src/py/esse/data/schema/system/name.json
 src/py/esse/data/schema/system/owner.json
 src/py/esse/data/schema/system/schema_version.json
 src/py/esse/data/schema/system/scope.json
+src/py/esse/data/schema/system/set.json
 src/py/esse/data/schema/system/sharing.json
 src/py/esse/data/schema/system/soft_removable.json
 src/py/esse/data/schema/system/status.json
-src/py/esse/data/schema/system/system_name.json
 src/py/esse/data/schema/system/tags.json
 src/py/esse/data/schema/system/timestampable.json
-src/py/esse/data/schema/system/unit_extended.json
 src/py/esse/data/schema/system/use_values.json
 src/py/esse/data/schema/workflow/base_flow.json
 src/py/esse/data/schema/workflow/new_subworkflow.json
 src/py/esse/data/schema/workflow/subworkflow.json
 src/py/esse/data/schema/workflow/unit.json
 src/py/esse/data/schema/workflow/unit/assertion.json
 src/py/esse/data/schema/workflow/unit/assignment.json
```

