# Comparing `tmp/genomehubs-2.7.1.tar.gz` & `tmp/genomehubs-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomehubs-2.7.1.tar", last modified: Tue May 23 15:24:58 2023, max compression
+gzip compressed data, was "genomehubs-2.7.5.tar", last modified: Tue May 30 11:03:54 2023, max compression
```

## Comparing `genomehubs-2.7.1.tar` & `genomehubs-2.7.5.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:58.127168 genomehubs-2.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-23 15:24:51.000000 genomehubs-2.7.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 15:24:51.000000 genomehubs-2.7.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-23 15:24:51.000000 genomehubs-2.7.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-23 15:24:51.000000 genomehubs-2.7.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-23 15:24:51.000000 genomehubs-2.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-23 15:24:51.000000 genomehubs-2.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-23 15:24:58.127168 genomehubs-2.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-23 15:24:51.000000 genomehubs-2.7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 15:24:51.000000 genomehubs-2.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-23 15:24:58.127168 genomehubs-2.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-23 15:24:51.000000 genomehubs-2.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:58.115167 genomehubs-2.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:58.119167 genomehubs-2.7.1/src/genomehubs/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:58.119167 genomehubs-2.7.1/src/genomehubs/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/config/dist.config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/genomehubs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:58.123168 genomehubs-2.7.1/src/genomehubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/btk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/busco.py
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13572 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/es_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    34258 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/gbif.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)    35765 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    37857 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/taxon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/wikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/lib/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:58.123168 genomehubs-2.7.1/src/genomehubs/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/ATTR_busco.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/ATTR_feature.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/ATTR_window_stats.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/analysis.json
--rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/assembly.json
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/assembly.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/btk.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/busco.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/busco_feature.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/feature.json
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/file.json
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/identifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/organelle.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/sample.types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:58.127168 genomehubs-2.7.1/src/genomehubs/templates/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/analysis_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/analysis_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/assembly_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/assembly_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/attribute_types_by_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/attribute_values_by_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/attributes_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/attributes_identifiers_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/attributes_names_by_keyword_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/file_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/file_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/max_nested_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/max_nested_value_by_key_value.json
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/max_nested_value_by_type.json
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/search_by_taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_attributes_by_taxon_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_by_any_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_by_name.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_by_specific_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_lookup.json
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_names.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_names_by_root.json
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_suggest.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/taxonomy_node_by_taxon_id.json
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/scripts/value_by_type_by_lineage.json
--rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/taxon.json
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/taxon.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/taxonomy.json
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/wikidata.names.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/window_full.types.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-23 15:24:51.000000 genomehubs-2.7.1/src/genomehubs/templates/window_stats.types.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:24:58.119167 genomehubs-2.7.1/src/genomehubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-23 15:24:58.000000 genomehubs-2.7.1/src/genomehubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-23 15:24:58.000000 genomehubs-2.7.1/src/genomehubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 15:24:58.000000 genomehubs-2.7.1/src/genomehubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-23 15:24:58.000000 genomehubs-2.7.1/src/genomehubs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 15:24:58.000000 genomehubs-2.7.1/src/genomehubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 15:24:58.000000 genomehubs-2.7.1/src/genomehubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.559165 genomehubs-2.7.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-30 11:03:14.000000 genomehubs-2.7.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-30 11:03:14.000000 genomehubs-2.7.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 11:03:14.000000 genomehubs-2.7.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-30 11:03:14.000000 genomehubs-2.7.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 11:03:14.000000 genomehubs-2.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-30 11:03:14.000000 genomehubs-2.7.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-30 11:03:54.559165 genomehubs-2.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-30 11:03:14.000000 genomehubs-2.7.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-30 11:03:14.000000 genomehubs-2.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-30 11:03:54.559165 genomehubs-2.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-30 11:03:14.000000 genomehubs-2.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.543163 genomehubs-2.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.547164 genomehubs-2.7.5/src/genomehubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.547164 genomehubs-2.7.5/src/genomehubs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/config/dist.config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/genomehubs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.551164 genomehubs-2.7.5/src/genomehubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/btk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/busco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/es_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34258 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/gbif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35765 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22460 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11928 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37857 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/taxon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/lib/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.555164 genomehubs-2.7.5/src/genomehubs/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/ATTR_busco.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/ATTR_feature.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/ATTR_window_stats.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/analysis.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15519 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/assembly.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/assembly.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/attributes.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/btk.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/busco.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/busco_feature.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/identifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/organelle.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10748 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/sample.types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.559165 genomehubs-2.7.5/src/genomehubs/templates/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/analysis_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/analysis_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/assembly_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/assembly_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attribute_types_by_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attribute_values_by_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attributes_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attributes_identifiers_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/attributes_names_by_keyword_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/file_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/file_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value_by_key_value.json
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value_by_type.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/search_by_taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_attributes_by_taxon_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_any_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_specific_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_lookup.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_names.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_names_by_root.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_suggest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/taxonomy_node_by_taxon_id.json
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/scripts/value_by_type_by_lineage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18238 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/taxon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/taxon.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/taxonomy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/wikidata.names.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/window_full.types.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-30 11:03:14.000000 genomehubs-2.7.5/src/genomehubs/templates/window_stats.types.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:03:54.547164 genomehubs-2.7.5/src/genomehubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 11:03:54.000000 genomehubs-2.7.5/src/genomehubs.egg-info/top_level.txt
```

### Comparing `genomehubs-2.7.1/CONTRIBUTING.rst` & `genomehubs-2.7.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/LICENSE` & `genomehubs-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/PKG-INFO` & `genomehubs-2.7.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: genomehubs
-Version: 2.7.1
+Version: 2.7.5
 Summary: GenomeHubs
 Home-page: https://github.com/genomehubs/genomehubs
 Author: genomehubs
 Author-email: genomehubs@genomehubs.org
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/genomehubs/genomehubs/issues
 Project-URL: Source, https://github.com/genomehubs/genomehubs
 Keywords: bioinformatics
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
@@ -69,9 +67,7 @@
 Changelog
 =========
 
 2.0.0 (2020-07-02)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `genomehubs-2.7.1/README.rst` & `genomehubs-2.7.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     :alt: Install with Conda
     :target: https://anaconda.org/tolkit/genomehubs
 
 .. |platforms| image:: https://anaconda.org/tolkit/genomehubs/badges/platforms.svg
     :alt: Conda platforms
     :target: https://anaconda.org/tolkit/genomehubs
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/genomehubs/genomehubs/2.7.1.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/genomehubs/genomehubs/2.7.5.svg
     :alt: Commits since latest release
-    :target: https://github.com/genomehubs/genomehubs/compare/2.7.1...main
+    :target: https://github.com/genomehubs/genomehubs/compare/2.7.5...main
 
 .. |license| image:: https://anaconda.org/tolkit/genomehubs/badges/license.svg
     :alt: MIT License
     :target: https://anaconda.org/tolkit/genomehubs
 
 .. end-badges
```

### Comparing `genomehubs-2.7.1/setup.cfg` & `genomehubs-2.7.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/setup.py` & `genomehubs-2.7.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="genomehubs",  # Required
-    version="2.7.1",
+    version="2.7.5",
     description="GenomeHubs",  # Optional
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
@@ -46,27 +46,27 @@
     #
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         # Indicate who your project is intended for
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         # Pick your license as you wish
         "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate you support Python 3. These classifiers are *not*
         # checked by 'pip install'. See instead 'python_requires' below.
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
```

### Comparing `genomehubs-2.7.1/src/genomehubs/config/dist.config.yaml` & `genomehubs-2.7.5/src/genomehubs/config/dist.config.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/genomehubs.py` & `genomehubs-2.7.5/src/genomehubs/genomehubs.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/attributes.py` & `genomehubs-2.7.5/src/genomehubs/lib/attributes.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/btk.py` & `genomehubs-2.7.5/src/genomehubs/lib/btk.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/busco.py` & `genomehubs-2.7.5/src/genomehubs/lib/busco.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/config.py` & `genomehubs-2.7.5/src/genomehubs/lib/config.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/directory.py` & `genomehubs-2.7.5/src/genomehubs/lib/directory.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/es_functions.py` & `genomehubs-2.7.5/src/genomehubs/lib/es_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 def test_connection(opts, *, log=False):
     """Test connection to Elasticsearch."""
     connected = False
     host = opts["es-host"][0]
     host = f"http://{host}"
     hosts = [host]
-    print(hosts)
     # with tolog.DisableLogger():
     # try:
     es = Elasticsearch(hosts=hosts, timeout=1800, max_retries=10, retry_on_timeout=True)
     connected = es.info()
     #   pass
     if not connected:
         message = "Could not connect to Elasticsearch at '%s'" % ", ".join(hosts)
```

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/files.py` & `genomehubs-2.7.5/src/genomehubs/lib/files.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/fill.py` & `genomehubs-2.7.5/src/genomehubs/lib/fill.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/gbif.py` & `genomehubs-2.7.5/src/genomehubs/lib/gbif.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/geo.py` & `genomehubs-2.7.5/src/genomehubs/lib/geo.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/hub.py` & `genomehubs-2.7.5/src/genomehubs/lib/hub.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/index.py` & `genomehubs-2.7.5/src/genomehubs/lib/index.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/init.py` & `genomehubs-2.7.5/src/genomehubs/lib/init.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/ncbi.py` & `genomehubs-2.7.5/src/genomehubs/lib/ncbi.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/parse.py` & `genomehubs-2.7.5/src/genomehubs/lib/parse.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/run.py` & `genomehubs-2.7.5/src/genomehubs/lib/run.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/sample.py` & `genomehubs-2.7.5/src/genomehubs/lib/sample.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/search.py` & `genomehubs-2.7.5/src/genomehubs/lib/search.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/taxon.py` & `genomehubs-2.7.5/src/genomehubs/lib/taxon.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/taxonomy.py` & `genomehubs-2.7.5/src/genomehubs/lib/taxonomy.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/test.py` & `genomehubs-2.7.5/src/genomehubs/lib/test.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/validate.py` & `genomehubs-2.7.5/src/genomehubs/lib/validate.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/wikidata.py` & `genomehubs-2.7.5/src/genomehubs/lib/wikidata.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/lib/window.py` & `genomehubs-2.7.5/src/genomehubs/lib/window.py`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/ATTR_busco.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/ATTR_busco.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/ATTR_feature.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/ATTR_feature.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/ATTR_window_stats.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/ATTR_window_stats.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/analysis.json` & `genomehubs-2.7.5/src/genomehubs/templates/analysis.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/assembly.json` & `genomehubs-2.7.5/src/genomehubs/templates/assembly.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/assembly.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/assembly.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/attributes.json` & `genomehubs-2.7.5/src/genomehubs/templates/attributes.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/btk.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/btk.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/busco.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/busco.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/busco_feature.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/busco_feature.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/feature.json` & `genomehubs-2.7.5/src/genomehubs/templates/feature.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/file.json` & `genomehubs-2.7.5/src/genomehubs/templates/file.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/identifiers.json` & `genomehubs-2.7.5/src/genomehubs/templates/identifiers.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/organelle.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/organelle.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/sample.json` & `genomehubs-2.7.5/src/genomehubs/templates/sample.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/sample.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/sample.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/assembly_lookup.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/assembly_lookup.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/assembly_suggest.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/assembly_suggest.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/attribute_value_by_primary_id.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/attribute_values_by_taxon.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/attribute_values_by_taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/max_nested_value_by_type.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value_by_type.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/max_nested_value_by_type_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/search_by_ancestral_taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_attributes_by_root_depth.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_by_any_name.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_any_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_any_name_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_by_lineage.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_by_name.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_by_specific_name.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_by_specific_name.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_lookup.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_lookup.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_lookup_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_missing_attribute_by_ancestor_id.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_name_sayt_attribute.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/taxon_suggest.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/taxon_suggest.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/scripts/value_by_type_by_lineage.json` & `genomehubs-2.7.5/src/genomehubs/templates/scripts/value_by_type_by_lineage.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/taxon.json` & `genomehubs-2.7.5/src/genomehubs/templates/taxon.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/taxon.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/taxon.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/taxonomy.json` & `genomehubs-2.7.5/src/genomehubs/templates/taxonomy.json`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/window_full.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/window_full.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs/templates/window_stats.types.yaml` & `genomehubs-2.7.5/src/genomehubs/templates/window_stats.types.yaml`

 * *Files identical despite different names*

### Comparing `genomehubs-2.7.1/src/genomehubs.egg-info/PKG-INFO` & `genomehubs-2.7.5/src/genomehubs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: genomehubs
-Version: 2.7.1
+Version: 2.7.5
 Summary: GenomeHubs
 Home-page: https://github.com/genomehubs/genomehubs
 Author: genomehubs
 Author-email: genomehubs@genomehubs.org
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/genomehubs/genomehubs/issues
 Project-URL: Source, https://github.com/genomehubs/genomehubs
 Keywords: bioinformatics
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
@@ -69,9 +67,7 @@
 Changelog
 =========
 
 2.0.0 (2020-07-02)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `genomehubs-2.7.1/src/genomehubs.egg-info/SOURCES.txt` & `genomehubs-2.7.5/src/genomehubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

