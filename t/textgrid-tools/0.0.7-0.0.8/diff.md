# Comparing `tmp/textgrid-tools-0.0.7.tar.gz` & `tmp/textgrid-tools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textgrid-tools-0.0.7.tar", last modified: Thu Jan 12 11:42:26 2023, max compression
+gzip compressed data, was "textgrid-tools-0.0.8.tar", last modified: Tue May 30 15:23:38 2023, max compression
```

## Comparing `textgrid-tools-0.0.7.tar` & `textgrid-tools-0.0.8.tar`

### file list

```diff
@@ -1,209 +1,206 @@
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/
--rw-rw-r--   0 mi        (1000) mi        (1000)     1070 2022-04-28 11:12:15.000000 textgrid-tools-0.0.7/LICENSE
--rw-rw-r--   0 mi        (1000) mi        (1000)     9445 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/PKG-INFO
--rw-rw-r--   0 mi        (1000) mi        (1000)     8154 2023-01-12 11:24:41.000000 textgrid-tools-0.0.7/README.md
--rw-rw-r--   0 mi        (1000) mi        (1000)     2698 2023-01-12 11:25:17.000000 textgrid-tools-0.0.7/pyproject.toml
--rw-rw-r--   0 mi        (1000) mi        (1000)       38 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/setup.cfg
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.893993 textgrid-tools-0.0.7/src/
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.897992 textgrid-tools-0.0.7/src/textgrid_tools/
--rw-rw-r--   0 mi        (1000) mi        (1000)      231 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      979 2022-04-29 15:42:16.000000 textgrid-tools-0.0.7/src/textgrid_tools/cloning.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1128 2022-05-06 07:02:01.000000 textgrid-tools-0.0.7/src/textgrid_tools/comparison.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      183 2022-04-29 15:42:16.000000 textgrid-tools-0.0.7/src/textgrid_tools/globals.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.897992 textgrid-tools-0.0.7/src/textgrid_tools/grid/
--rw-rw-r--   0 mi        (1000) mi        (1000)      263 2022-04-29 15:42:16.000000 textgrid-tools-0.0.7/src/textgrid_tools/grid/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3752 2022-05-06 13:47:23.000000 textgrid-tools-0.0.7/src/textgrid_tools/grid/audio_synchronization.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     7843 2022-05-06 13:47:23.000000 textgrid-tools-0.0.7/src/textgrid_tools/grid/creation.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4735 2022-05-06 13:51:32.000000 textgrid-tools-0.0.7/src/textgrid_tools/grid/splitting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3673 2022-05-06 13:47:23.000000 textgrid-tools-0.0.7/src/textgrid_tools/grid/stats_generation.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.897992 textgrid-tools-0.0.7/src/textgrid_tools/grids/
--rw-rw-r--   0 mi        (1000) mi        (1000)      153 2022-04-29 15:42:16.000000 textgrid-tools-0.0.7/src/textgrid_tools/grids/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4128 2022-12-02 11:44:08.000000 textgrid-tools-0.0.7/src/textgrid_tools/grids/dictionary_exporting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)    14705 2023-01-04 16:15:31.000000 textgrid-tools-0.0.7/src/textgrid_tools/grids/durations_labelling.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4081 2022-11-09 10:55:39.000000 textgrid-tools-0.0.7/src/textgrid_tools/grids/durations_plotting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2888 2022-05-06 13:51:59.000000 textgrid-tools-0.0.7/src/textgrid_tools/grids/grid_merging.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1517 2022-11-11 13:24:26.000000 textgrid-tools-0.0.7/src/textgrid_tools/grids/marks_exporting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5179 2022-10-24 15:24:23.000000 textgrid-tools-0.0.7/src/textgrid_tools/grids/stats_generation.py
--rw-rw-r--   0 mi        (1000) mi        (1000)    13418 2022-10-21 12:47:38.000000 textgrid-tools-0.0.7/src/textgrid_tools/helper.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.901992 textgrid-tools-0.0.7/src/textgrid_tools/intervals/
--rw-rw-r--   0 mi        (1000) mi        (1000)      967 2022-12-19 16:19:08.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2979 2022-11-09 11:55:46.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/between_marks_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2841 2022-10-12 10:18:07.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/between_pause_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     7752 2022-10-21 14:10:05.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/boundary_fixing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2756 2022-05-06 13:54:18.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/boundary_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3237 2022-11-09 11:42:03.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/common.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     9805 2022-06-08 15:27:55.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/duration_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3950 2022-06-08 15:27:55.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/durations_plotting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1322 2022-10-11 07:16:17.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2858 2022-05-06 13:56:48.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/mark_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     9791 2022-10-24 15:24:23.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/removing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2503 2022-05-06 13:54:55.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/splitting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5583 2022-12-19 15:44:04.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/symbols_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3514 2022-12-23 11:17:29.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/template_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3529 2023-01-05 09:24:51.000000 textgrid-tools-0.0.7/src/textgrid_tools/intervals/text_replacement.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.901992 textgrid-tools-0.0.7/src/textgrid_tools/tier/
--rw-rw-r--   0 mi        (1000) mi        (1000)      265 2022-05-02 10:53:07.000000 textgrid-tools-0.0.7/src/textgrid_tools/tier/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1515 2022-05-06 13:55:01.000000 textgrid-tools-0.0.7/src/textgrid_tools/tier/cloning.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1179 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools/tier/exporting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1015 2022-05-06 13:55:03.000000 textgrid-tools-0.0.7/src/textgrid_tools/tier/importing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4448 2022-12-19 16:27:28.000000 textgrid-tools-0.0.7/src/textgrid_tools/tier/mapping.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1691 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools/tier/moving.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1189 2022-05-06 13:55:09.000000 textgrid-tools-0.0.7/src/textgrid_tools/tier/renaming.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.901992 textgrid-tools-0.0.7/src/textgrid_tools/tiers/
--rw-rw-r--   0 mi        (1000) mi        (1000)      302 2022-04-29 15:42:16.000000 textgrid-tools-0.0.7/src/textgrid_tools/tiers/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2560 2022-05-11 06:16:28.000000 textgrid-tools-0.0.7/src/textgrid_tools/tiers/marks_mapping.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1388 2022-05-06 13:55:18.000000 textgrid-tools-0.0.7/src/textgrid_tools/tiers/removing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1459 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools/tiers/silence_labeling.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2371 2022-05-06 13:47:23.000000 textgrid-tools-0.0.7/src/textgrid_tools/tiers/symbol_removing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4062 2022-10-26 08:53:39.000000 textgrid-tools-0.0.7/src/textgrid_tools/tiers/transcription.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4957 2022-10-07 07:36:43.000000 textgrid-tools-0.0.7/src/textgrid_tools/validation.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.897992 textgrid-tools-0.0.7/src/textgrid_tools.egg-info/
--rw-rw-r--   0 mi        (1000) mi        (1000)     9445 2023-01-12 11:42:26.000000 textgrid-tools-0.0.7/src/textgrid_tools.egg-info/PKG-INFO
--rw-rw-r--   0 mi        (1000) mi        (1000)     9072 2023-01-12 11:42:26.000000 textgrid-tools-0.0.7/src/textgrid_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)        1 2023-01-12 11:42:26.000000 textgrid-tools-0.0.7/src/textgrid_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)       71 2023-01-12 11:42:26.000000 textgrid-tools-0.0.7/src/textgrid_tools.egg-info/entry_points.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)      137 2023-01-12 11:42:26.000000 textgrid-tools-0.0.7/src/textgrid_tools.egg-info/requires.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)       80 2023-01-12 11:42:26.000000 textgrid-tools-0.0.7/src/textgrid_tools.egg-info/top_level.txt
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.901992 textgrid-tools-0.0.7/src/textgrid_tools_cli/
--rw-rw-r--   0 mi        (1000) mi        (1000)     1677 2022-11-09 11:54:49.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)    10614 2023-01-12 11:19:39.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/cli.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5022 2022-11-25 15:43:01.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/common.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1292 2022-11-04 08:15:00.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/globals.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.901992 textgrid-tools-0.0.7/src/textgrid_tools_cli/grid/
--rw-rw-r--   0 mi        (1000) mi        (1000)      304 2022-05-06 13:16:00.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grid/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4073 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grid/audio_synchronization.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5380 2022-11-25 16:00:17.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grid/creation.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5782 2022-11-25 16:00:49.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grid/splitting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1844 2022-11-25 16:01:00.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grid/stats_generation.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.901992 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/
--rw-rw-r--   0 mi        (1000) mi        (1000)      337 2022-05-02 10:52:12.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1414 2022-11-11 13:24:26.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/audio_paths_exporting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3154 2023-01-02 15:26:47.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/audio_paths_importing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     6927 2023-01-05 11:15:41.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/durations_labelling.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2428 2022-11-25 17:25:05.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/durations_plotting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1930 2022-11-11 13:25:51.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/grid_durations_exporting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1407 2022-11-11 13:24:26.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/grid_paths_exporting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3152 2023-01-02 15:26:37.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/grid_paths_importing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2657 2022-11-25 16:02:50.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/grids_merging.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2455 2022-11-25 16:03:01.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/marks_exporting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5902 2022-10-14 13:58:10.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/pronunciations_exporting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3474 2022-10-24 15:25:30.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/stats_generation.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4580 2023-01-12 09:17:55.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/vocabulary_export.py
--rw-rw-r--   0 mi        (1000) mi        (1000)    12673 2023-01-04 13:24:23.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/helper.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.905993 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/
--rw-rw-r--   0 mi        (1000) mi        (1000)      915 2022-11-09 11:54:47.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2318 2022-11-25 15:52:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/between_marks_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2143 2022-11-25 15:52:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/between_pause_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1931 2022-11-25 16:03:40.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/boundary_fixing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2010 2022-11-25 16:03:47.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/boundary_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      491 2022-04-29 15:42:16.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/common.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2194 2022-11-25 15:52:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/duration_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2714 2022-12-02 10:45:55.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/durations_plotting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1642 2022-11-25 15:52:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2716 2022-11-25 16:06:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/mark_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     6757 2023-01-05 09:13:08.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/removing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1734 2022-11-25 16:08:07.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/splitting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2719 2022-11-25 16:09:25.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/symbols_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2228 2022-12-23 11:19:46.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/template_joining.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2072 2023-01-05 09:25:04.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/text_replacement.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5164 2022-05-06 13:29:39.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/logging_configuration.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     7569 2022-06-08 12:21:14.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/textgrid_io.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.905993 textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/
--rw-rw-r--   0 mi        (1000) mi        (1000)      386 2022-05-02 10:55:02.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1631 2022-11-25 15:52:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/cloning.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2814 2022-11-25 16:09:45.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/exporting.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3538 2022-11-25 16:10:05.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/importing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2950 2022-11-25 15:52:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/mapping.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1609 2022-11-25 15:52:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/moving.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1923 2022-11-25 16:10:33.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/renaming.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.905993 textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/
--rw-rw-r--   0 mi        (1000) mi        (1000)      377 2022-05-02 10:52:07.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2802 2022-11-25 16:11:26.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/marks_mapping.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1397 2022-11-25 15:52:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/removing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2967 2022-11-25 16:12:21.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/silence_labeling.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2111 2022-11-25 16:12:49.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/symbol_removing.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     4433 2022-11-25 15:52:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/transcription.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1064 2022-10-12 14:15:13.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli/validation.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.905993 textgrid-tools-0.0.7/src/textgrid_tools_cli_tests/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:09:17.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli_tests/__init__.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.893993 textgrid-tools-0.0.7/src/textgrid_tools_cli_tests/grids/
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.905993 textgrid-tools-0.0.7/src/textgrid_tools_cli_tests/grids/vocabulary_export_py/
--rw-rw-r--   0 mi        (1000) mi        (1000)     1254 2023-01-04 13:30:42.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli_tests/grids/vocabulary_export_py/test_get_vocabulary.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      572 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli_tests/test_parse_codec.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      552 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_cli_tests/test_parse_float.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.905993 textgrid-tools-0.0.7/src/textgrid_tools_tests/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:09:04.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/__init__.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.893993 textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.905993 textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/
--rw-rw-r--   0 mi        (1000) mi        (1000)     2155 2022-10-07 16:22:39.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_filter_intervals_by_duration.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1442 2022-10-07 16:22:39.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_filter_intervals_by_mark.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1898 2022-10-07 16:22:39.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_get_percentile_boundary.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      900 2022-10-07 16:22:39.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_get_percentual_boundary.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1643 2022-10-11 07:16:16.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_absolute.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1878 2022-11-25 16:22:03.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_all.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2080 2022-11-25 16:26:29.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_separate.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      431 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/helper.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.905993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:09:09.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/__init__.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.905993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_between_pause_joining/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:51.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_between_pause_joining/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2407 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_between_pause_joining/test_get_chunks.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2428 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_between_pause_joining/test_group_adjacent_pauses.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.905993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_common/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:49.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_common/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2829 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_common/test_group_adjacent_content_and_pauses.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      965 2022-04-29 15:42:16.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_common/test_merge_intervals.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:31.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1298 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_chunk_intervals_with_pauses.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1333 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_chunk_intervals_without_pauses.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1551 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_get_duration_chunks.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2578 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_split_pauses.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1290 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_split_pauses_at_end.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1297 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_split_pauses_at_start.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:46.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      870 2022-10-21 08:55:36.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_all.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      732 2022-10-21 08:54:19.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_both.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      637 2022-10-21 08:53:46.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_end.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      641 2022-10-21 08:53:07.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_start.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2178 2022-10-24 08:47:12.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_get_sync_times.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1067 2022-10-21 12:33:46.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_merge_consecutives.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2539 2022-10-21 13:21:15.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_remove_intervals_from_tiers.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_sentence_joining/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_sentence_joining/__init__.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_splitting/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:39.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_splitting/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1128 2022-05-02 15:44:42.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_splitting/test_get_split_intervals.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      951 2022-05-31 09:56:00.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_splitting/test_split_intervals.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2023-01-05 08:37:13.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      903 2023-01-05 08:38:52.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_all.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      674 2023-01-05 09:14:16.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_begin.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      765 2023-01-05 08:40:12.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_both.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      670 2023-01-05 08:40:42.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_end.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1349 2023-01-05 09:07:52.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/test_replace_text.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_splitting_v2_py/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:37.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_splitting_v2_py/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2803 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_splitting_v2_py/test_get_split_intervals_v2.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_symbols_joining_py/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:35.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_symbols_joining_py/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3757 2022-06-08 15:27:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_symbols_joining_py/test_chunk_intervals.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2435 2022-12-19 15:44:11.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_symbols_joining_py/test_merge_right_core2.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_template_joining/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-12-19 15:48:43.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_template_joining/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     6306 2022-12-23 11:17:15.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_template_joining/test_chunk_intervals_boundary.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/py_helper/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:54.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/py_helper/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1030 2022-05-02 15:24:14.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/py_helper/test_check_intervals_are_consecutive copy.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      984 2022-05-02 15:20:29.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/py_helper/test_set_intervals_consecutive.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/tier/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:58.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/tier/__init__.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/tier/py_moving/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:57.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/tier/py_moving/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1569 2022-05-06 14:09:34.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/tier/py_moving/test_move_tier.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/tiers/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:09:03.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/tiers/__init__.py
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-01-12 11:42:26.909993 textgrid-tools-0.0.7/src/textgrid_tools_tests/tiers/py_symbol_removing/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:09:01.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/tiers/py_symbol_removing/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)        0 2022-05-06 07:02:01.000000 textgrid-tools-0.0.7/src/textgrid_tools_tests/tiers/py_symbol_removing/test_get_updated_mark.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1070 2023-05-30 15:10:35.000000 textgrid-tools-0.0.8/LICENSE
+-rw-rw-r--   0 mi        (1000) mi        (1000)     9905 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/PKG-INFO
+-rw-rw-r--   0 mi        (1000) mi        (1000)     8614 2023-05-30 15:09:42.000000 textgrid-tools-0.0.8/README.md
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2698 2023-05-30 15:08:47.000000 textgrid-tools-0.0.8/pyproject.toml
+-rw-rw-r--   0 mi        (1000) mi        (1000)       38 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/setup.cfg
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.835700 textgrid-tools-0.0.8/src/
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.835700 textgrid-tools-0.0.8/src/textgrid_tools/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      231 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      979 2022-04-29 15:42:16.000000 textgrid-tools-0.0.8/src/textgrid_tools/cloning.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1128 2022-05-06 07:02:01.000000 textgrid-tools-0.0.8/src/textgrid_tools/comparison.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      183 2022-04-29 15:42:16.000000 textgrid-tools-0.0.8/src/textgrid_tools/globals.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.835700 textgrid-tools-0.0.8/src/textgrid_tools/grid/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      263 2022-04-29 15:42:16.000000 textgrid-tools-0.0.8/src/textgrid_tools/grid/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3752 2022-05-06 13:47:23.000000 textgrid-tools-0.0.8/src/textgrid_tools/grid/audio_synchronization.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     7843 2022-05-06 13:47:23.000000 textgrid-tools-0.0.8/src/textgrid_tools/grid/creation.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4735 2022-05-06 13:51:32.000000 textgrid-tools-0.0.8/src/textgrid_tools/grid/splitting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3673 2022-05-06 13:47:23.000000 textgrid-tools-0.0.8/src/textgrid_tools/grid/stats_generation.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.835700 textgrid-tools-0.0.8/src/textgrid_tools/grids/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      153 2022-04-29 15:42:16.000000 textgrid-tools-0.0.8/src/textgrid_tools/grids/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4128 2022-12-02 11:44:08.000000 textgrid-tools-0.0.8/src/textgrid_tools/grids/dictionary_exporting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)    14705 2023-01-04 16:15:31.000000 textgrid-tools-0.0.8/src/textgrid_tools/grids/durations_labelling.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4081 2022-11-09 10:55:39.000000 textgrid-tools-0.0.8/src/textgrid_tools/grids/durations_plotting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2888 2022-05-06 13:51:59.000000 textgrid-tools-0.0.8/src/textgrid_tools/grids/grid_merging.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1517 2022-11-11 13:24:26.000000 textgrid-tools-0.0.8/src/textgrid_tools/grids/marks_exporting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     6117 2023-03-08 11:57:15.000000 textgrid-tools-0.0.8/src/textgrid_tools/grids/stats_generation.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)    13418 2022-10-21 12:47:38.000000 textgrid-tools-0.0.8/src/textgrid_tools/helper.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.839700 textgrid-tools-0.0.8/src/textgrid_tools/intervals/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      967 2022-12-19 16:19:08.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2979 2022-11-09 11:55:46.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/between_marks_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2841 2022-10-12 10:18:07.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/between_pause_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     7752 2022-10-21 14:10:05.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/boundary_fixing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2756 2022-05-06 13:54:18.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/boundary_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3237 2022-11-09 11:42:03.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/common.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     9805 2022-06-08 15:27:55.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/duration_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3950 2022-06-08 15:27:55.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/durations_plotting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1322 2022-10-11 07:16:17.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2858 2022-05-06 13:56:48.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/mark_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     9791 2022-10-24 15:24:23.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/removing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2503 2022-05-06 13:54:55.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/splitting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     5583 2022-12-19 15:44:04.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/symbols_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3514 2022-12-23 11:17:29.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/template_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3529 2023-01-05 09:24:51.000000 textgrid-tools-0.0.8/src/textgrid_tools/intervals/text_replacement.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.839700 textgrid-tools-0.0.8/src/textgrid_tools/tier/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      265 2022-05-02 10:53:07.000000 textgrid-tools-0.0.8/src/textgrid_tools/tier/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1515 2022-05-06 13:55:01.000000 textgrid-tools-0.0.8/src/textgrid_tools/tier/cloning.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1179 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools/tier/exporting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1015 2022-05-06 13:55:03.000000 textgrid-tools-0.0.8/src/textgrid_tools/tier/importing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4448 2022-12-19 16:27:28.000000 textgrid-tools-0.0.8/src/textgrid_tools/tier/mapping.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1691 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools/tier/moving.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1189 2022-05-06 13:55:09.000000 textgrid-tools-0.0.8/src/textgrid_tools/tier/renaming.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.839700 textgrid-tools-0.0.8/src/textgrid_tools/tiers/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      302 2022-04-29 15:42:16.000000 textgrid-tools-0.0.8/src/textgrid_tools/tiers/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2560 2022-05-11 06:16:28.000000 textgrid-tools-0.0.8/src/textgrid_tools/tiers/marks_mapping.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1388 2022-05-06 13:55:18.000000 textgrid-tools-0.0.8/src/textgrid_tools/tiers/removing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1459 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools/tiers/silence_labeling.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2371 2022-05-06 13:47:23.000000 textgrid-tools-0.0.8/src/textgrid_tools/tiers/symbol_removing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4062 2022-10-26 08:53:39.000000 textgrid-tools-0.0.8/src/textgrid_tools/tiers/transcription.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4957 2022-10-07 07:36:43.000000 textgrid-tools-0.0.8/src/textgrid_tools/validation.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.835700 textgrid-tools-0.0.8/src/textgrid_tools.egg-info/
+-rw-rw-r--   0 mi        (1000) mi        (1000)     9905 2023-05-30 15:23:38.000000 textgrid-tools-0.0.8/src/textgrid_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 mi        (1000) mi        (1000)     8898 2023-05-30 15:23:38.000000 textgrid-tools-0.0.8/src/textgrid_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)        1 2023-05-30 15:23:38.000000 textgrid-tools-0.0.8/src/textgrid_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)       71 2023-05-30 15:23:38.000000 textgrid-tools-0.0.8/src/textgrid_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)      137 2023-05-30 15:23:38.000000 textgrid-tools-0.0.8/src/textgrid_tools.egg-info/requires.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)       80 2023-05-30 15:23:38.000000 textgrid-tools-0.0.8/src/textgrid_tools.egg-info/top_level.txt
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.839700 textgrid-tools-0.0.8/src/textgrid_tools_cli/
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1677 2022-11-09 11:54:49.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)    10609 2023-04-04 08:41:17.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/cli.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     5022 2022-11-25 15:43:01.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/common.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1292 2022-11-04 08:15:00.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/globals.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.839700 textgrid-tools-0.0.8/src/textgrid_tools_cli/grid/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      304 2022-05-06 13:16:00.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grid/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4073 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grid/audio_synchronization.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     5380 2022-11-25 16:00:17.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grid/creation.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     5782 2022-11-25 16:00:49.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grid/splitting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1844 2022-11-25 16:01:00.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grid/stats_generation.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.839700 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      337 2022-05-02 10:52:12.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1416 2023-04-04 08:41:37.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/audio_paths_exporting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3634 2023-01-16 08:51:34.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/audio_paths_importing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     6927 2023-01-05 11:15:41.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/durations_labelling.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2428 2022-11-25 17:25:05.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/durations_plotting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2781 2023-04-04 08:41:59.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/grid_durations_exporting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1407 2022-11-11 13:24:26.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/grid_paths_exporting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3629 2023-01-16 08:51:34.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/grid_paths_importing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2657 2022-11-25 16:02:50.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/grids_merging.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2455 2022-11-25 16:03:01.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/marks_exporting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     5902 2022-10-14 13:58:10.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/pronunciations_exporting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3474 2022-10-24 15:25:30.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/stats_generation.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4580 2023-01-12 09:17:55.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/vocabulary_export.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)    12673 2023-01-04 13:24:23.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/helper.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      915 2022-11-09 11:54:47.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2318 2022-11-25 15:52:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/between_marks_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2143 2022-11-25 15:52:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/between_pause_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1931 2022-11-25 16:03:40.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/boundary_fixing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2010 2022-11-25 16:03:47.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/boundary_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      491 2022-04-29 15:42:16.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/common.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2194 2022-11-25 15:52:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/duration_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2714 2022-12-02 10:45:55.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/durations_plotting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1642 2022-11-25 15:52:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2716 2022-11-25 16:06:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/mark_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     6757 2023-01-12 15:16:47.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/removing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1734 2022-11-25 16:08:07.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/splitting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2719 2022-11-25 16:09:25.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/symbols_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2228 2022-12-23 11:19:46.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/template_joining.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2072 2023-01-05 09:25:04.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/text_replacement.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     5164 2022-05-06 13:29:39.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/logging_configuration.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     7569 2022-06-08 12:21:14.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/textgrid_io.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      386 2022-05-02 10:55:02.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1631 2022-11-25 15:52:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/cloning.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2814 2022-11-25 16:09:45.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/exporting.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3538 2022-11-25 16:10:05.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/importing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2950 2022-11-25 15:52:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/mapping.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1609 2022-11-25 15:52:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/moving.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1923 2022-11-25 16:10:33.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/renaming.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/
+-rw-rw-r--   0 mi        (1000) mi        (1000)      377 2022-05-02 10:52:07.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2802 2022-11-25 16:11:26.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/marks_mapping.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1397 2022-11-25 15:52:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/removing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2967 2022-11-25 16:12:21.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/silence_labeling.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2111 2022-11-25 16:12:49.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/symbol_removing.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     4433 2022-11-25 15:52:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/transcription.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1064 2022-10-12 14:15:13.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli/validation.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_cli_tests/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:09:17.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli_tests/__init__.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.835700 textgrid-tools-0.0.8/src/textgrid_tools_cli_tests/grids/
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_cli_tests/grids/vocabulary_export_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1254 2023-01-04 13:30:42.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli_tests/grids/vocabulary_export_py/test_get_vocabulary.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      572 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli_tests/test_parse_codec.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      552 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_cli_tests/test_parse_float.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_tests/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:09:04.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/__init__.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.835700 textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2155 2022-10-07 16:22:39.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_filter_intervals_by_duration.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1442 2022-10-07 16:22:39.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_filter_intervals_by_mark.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1898 2022-10-07 16:22:39.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_get_percentile_boundary.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      900 2022-10-07 16:22:39.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_get_percentual_boundary.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1643 2022-10-11 07:16:16.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_absolute.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1878 2022-11-25 16:22:03.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_all.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2080 2022-11-25 16:26:29.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_separate.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      431 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/helper.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_tests/helper_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/helper_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1030 2022-05-02 15:24:14.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/helper_py/test_check_intervals_are_consecutive copy.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      984 2022-05-02 15:20:29.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/helper_py/test_set_intervals_consecutive.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:09:09.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/__init__.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/between_pause_joining_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:51.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/between_pause_joining_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2407 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/between_pause_joining_py/test_get_chunks.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2428 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/between_pause_joining_py/test_group_adjacent_pauses.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/common_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:49.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/common_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2829 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/common_py/test_group_adjacent_content_and_pauses.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      965 2022-04-29 15:42:16.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/common_py/test_merge_intervals.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:31.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1298 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_chunk_intervals_with_pauses.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1333 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_chunk_intervals_without_pauses.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1551 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_get_duration_chunks.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2578 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_split_pauses.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1290 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_split_pauses_at_end.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1297 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_split_pauses_at_start.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.843700 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:46.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      870 2022-10-21 08:55:36.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_all.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      732 2022-10-21 08:54:19.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_both.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      637 2022-10-21 08:53:46.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_end.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      641 2022-10-21 08:53:07.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_start.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2178 2022-10-24 08:47:12.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_get_sync_times.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1067 2022-10-21 12:33:46.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_merge_consecutives.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2539 2022-10-21 13:21:15.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_remove_intervals_from_tiers.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/sentence_joining_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/sentence_joining_py/__init__.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/splitting_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:39.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/splitting_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3824 2023-05-30 15:22:38.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/splitting_py/test_get_split_intervals.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      951 2022-05-31 09:56:00.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/splitting_py/test_split_intervals.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/symbols_joining_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:35.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/symbols_joining_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3757 2022-06-08 15:27:54.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/symbols_joining_py/test_chunk_intervals.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2435 2022-12-19 15:44:11.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/symbols_joining_py/test_merge_right_core2.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/template_joining_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-12-19 15:48:43.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/template_joining_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     6306 2022-12-23 11:17:15.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/template_joining_py/test_chunk_intervals_boundary.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2023-01-05 08:37:13.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      903 2023-01-05 08:38:52.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_all.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      674 2023-01-05 09:14:16.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_begin.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      765 2023-01-05 08:40:12.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_both.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      670 2023-01-05 08:40:42.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_end.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1349 2023-01-05 09:07:52.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/test_replace_text.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/src/textgrid_tools_tests/tier/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:58.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/tier/__init__.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/src/textgrid_tools_tests/tier/moving_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:08:57.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/tier/moving_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1569 2022-05-06 14:09:34.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/tier/moving_py/test_move_tier.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/src/textgrid_tools_tests/tiers/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:09:03.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/tiers/__init__.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 15:23:38.847700 textgrid-tools-0.0.8/src/textgrid_tools_tests/tiers/symbol_removing_py/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-31 12:09:01.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/tiers/symbol_removing_py/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)        0 2022-05-06 07:02:01.000000 textgrid-tools-0.0.8/src/textgrid_tools_tests/tiers/symbol_removing_py/test_get_updated_mark.py
```

### Comparing `textgrid-tools-0.0.7/LICENSE` & `textgrid-tools-0.0.8/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Stefan Taubert
+Copyright (c) 2023 Stefan Taubert
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `textgrid-tools-0.0.7/PKG-INFO` & `textgrid-tools-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgrid-tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Command-line interface (CLI) to modify TextGrids and their corresponding audio files.
 Author-email: Stefan Taubert <pypi@stefantaubert.com>
 Maintainer-email: Stefan Taubert <pypi@stefantaubert.com>
 License: MIT
 Project-URL: Homepage, https://github.com/stefantaubert/textgrid-ipa
 Project-URL: Issues, https://github.com/stefantaubert/textgrid-ipa/issues
 Keywords: Text-to-speech,Speech synthesis,praat,TextGrid,Utils,Language,Linguistics
@@ -30,16 +30,16 @@
 # textgrid-tools
 
 [![PyPI](https://img.shields.io/pypi/v/textgrid-tools.svg)](https://pypi.python.org/pypi/textgrid-tools)
 ![PyPI](https://img.shields.io/pypi/pyversions/textgrid-tools.svg)
 [![MIT](https://img.shields.io/github/license/stefantaubert/textgrid-ipa.svg)](https://github.com/stefantaubert/textgrid-ipa/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/wheel/textgrid-tools.svg)](https://pypi.python.org/pypi/textgrid-tools/#files)
 ![PyPI](https://img.shields.io/pypi/implementation/textgrid-tools.svg)
-[![PyPI](https://img.shields.io/github/commits-since/stefantaubert/textgrid-ipa/latest/main.svg)](https://github.com/stefantaubert/textgrid-ipa/compare/v0.0.7...main)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7528782.svg)](https://doi.org/10.5281/zenodo.7528782)
+[![PyPI](https://img.shields.io/github/commits-since/stefantaubert/textgrid-ipa/latest/main.svg)](https://github.com/stefantaubert/textgrid-ipa/compare/v0.0.8...main)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7986716.svg)](https://doi.org/10.5281/zenodo.7986716)
 
 Command-line interface (CLI) to modify TextGrids and their corresponding audio files.
 
 ## Features
 
 - grids
   - `merge`: merge grids together
@@ -193,22 +193,31 @@
 
 ## Citation
 
 If you want to cite this repo, you can use this BibTeX-entry generated by GitHub (see *About => Cite this repository*).
 
 ## Changelog
 
+- v0.0.8 (2023-05-30)
+  - Fixed:
+    - Bugfix `intervals remove` copying on different in/out-locations
+    - Bugfix `import-paths` and `import-audio-paths` option `--symlink` is now creating symbolic links instead of hard links
+  - Changed:
+    - Improved logging in `import-paths` and `import-audio-paths`
+    - Improved logging of durations in `grids plot-stats`
+  - Added:
+    - Added option to get durations from audio files on `grids export-durations`
 - v0.0.7 (2023-01-12)
-  - Fixed
+  - Fixed:
     - Bugfix `grids import-paths` and `grids import-audio-paths`
-  - Added
+  - Added:
     - Added option `--ignore` to ignore custom marks in `grids export-vocabulary`
     - Added option `--mode` to `intervals replace-text` to replace text on different interval positions
     - Added returning of an exit code
-  - Removed
+  - Removed:
     - Removed `tiers mark-silence` because `grids mark-durations` should be used
     - Removed `tiers remove-symbols` because `intervals replace-text` should be used
     - Removed `intervals join-between-pauses` because `join-between-marks` should be used
 - v0.0.6 (2022-12-23)
   - improved validation for pronunciation dictionary creation
   - bugfix replace text logging
   - added intervals join-template
```

### Comparing `textgrid-tools-0.0.7/README.md` & `textgrid-tools-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # textgrid-tools
 
 [![PyPI](https://img.shields.io/pypi/v/textgrid-tools.svg)](https://pypi.python.org/pypi/textgrid-tools)
 ![PyPI](https://img.shields.io/pypi/pyversions/textgrid-tools.svg)
 [![MIT](https://img.shields.io/github/license/stefantaubert/textgrid-ipa.svg)](https://github.com/stefantaubert/textgrid-ipa/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/wheel/textgrid-tools.svg)](https://pypi.python.org/pypi/textgrid-tools/#files)
 ![PyPI](https://img.shields.io/pypi/implementation/textgrid-tools.svg)
-[![PyPI](https://img.shields.io/github/commits-since/stefantaubert/textgrid-ipa/latest/main.svg)](https://github.com/stefantaubert/textgrid-ipa/compare/v0.0.7...main)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7528782.svg)](https://doi.org/10.5281/zenodo.7528782)
+[![PyPI](https://img.shields.io/github/commits-since/stefantaubert/textgrid-ipa/latest/main.svg)](https://github.com/stefantaubert/textgrid-ipa/compare/v0.0.8...main)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7986716.svg)](https://doi.org/10.5281/zenodo.7986716)
 
 Command-line interface (CLI) to modify TextGrids and their corresponding audio files.
 
 ## Features
 
 - grids
   - `merge`: merge grids together
@@ -164,22 +164,31 @@
 
 ## Citation
 
 If you want to cite this repo, you can use this BibTeX-entry generated by GitHub (see *About => Cite this repository*).
 
 ## Changelog
 
+- v0.0.8 (2023-05-30)
+  - Fixed:
+    - Bugfix `intervals remove` copying on different in/out-locations
+    - Bugfix `import-paths` and `import-audio-paths` option `--symlink` is now creating symbolic links instead of hard links
+  - Changed:
+    - Improved logging in `import-paths` and `import-audio-paths`
+    - Improved logging of durations in `grids plot-stats`
+  - Added:
+    - Added option to get durations from audio files on `grids export-durations`
 - v0.0.7 (2023-01-12)
-  - Fixed
+  - Fixed:
     - Bugfix `grids import-paths` and `grids import-audio-paths`
-  - Added
+  - Added:
     - Added option `--ignore` to ignore custom marks in `grids export-vocabulary`
     - Added option `--mode` to `intervals replace-text` to replace text on different interval positions
     - Added returning of an exit code
-  - Removed
+  - Removed:
     - Removed `tiers mark-silence` because `grids mark-durations` should be used
     - Removed `tiers remove-symbols` because `intervals replace-text` should be used
     - Removed `intervals join-between-pauses` because `join-between-marks` should be used
 - v0.0.6 (2022-12-23)
   - improved validation for pronunciation dictionary creation
   - bugfix replace text logging
   - added intervals join-template
```

### Comparing `textgrid-tools-0.0.7/pyproject.toml` & `textgrid-tools-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "textgrid-tools"
-version = "0.0.7"
+version = "0.0.8"
 description = "Command-line interface (CLI) to modify TextGrids and their corresponding audio files."
 readme = "README.md"
 requires-python = ">=3.8, <4"
 license = {text = "MIT"}
 authors = [
   {name = "Stefan Taubert", email = "pypi@stefantaubert.com"}
 ]
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/cloning.py` & `textgrid-tools-0.0.8/src/textgrid_tools/cloning.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/comparison.py` & `textgrid-tools-0.0.8/src/textgrid_tools/comparison.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/grid/audio_synchronization.py` & `textgrid-tools-0.0.8/src/textgrid_tools/grid/audio_synchronization.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/grid/creation.py` & `textgrid-tools-0.0.8/src/textgrid_tools/grid/creation.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/grid/splitting.py` & `textgrid-tools-0.0.8/src/textgrid_tools/grid/splitting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/grid/stats_generation.py` & `textgrid-tools-0.0.8/src/textgrid_tools/grid/stats_generation.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/grids/dictionary_exporting.py` & `textgrid-tools-0.0.8/src/textgrid_tools/grids/dictionary_exporting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/grids/durations_labelling.py` & `textgrid-tools-0.0.8/src/textgrid_tools/grids/durations_labelling.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/grids/durations_plotting.py` & `textgrid-tools-0.0.8/src/textgrid_tools/grids/durations_plotting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/grids/grid_merging.py` & `textgrid-tools-0.0.8/src/textgrid_tools/grids/grid_merging.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/grids/marks_exporting.py` & `textgrid-tools-0.0.8/src/textgrid_tools/grids/marks_exporting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/grids/stats_generation.py` & `textgrid-tools-0.0.8/src/textgrid_tools/grids/stats_generation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import io
 import logging
-from collections import Counter
+from collections import Counter, OrderedDict
 from logging import Logger, getLogger
 from typing import Dict, List, Optional, Tuple, cast
 
 import numpy as np
 import pandas as pd
 from matplotlib import collections
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.ticker import FixedLocator
+from scipy.stats import kurtosis
 from textgrid import TextGrid
 from textgrid.textgrid import TextGrid
 from tqdm import tqdm
 
 from textgrid_tools.globals import ExecutionResult
 from textgrid_tools.validation import InvalidGridError
 
@@ -50,24 +51,56 @@
       intervals_durations[tier.name].extend(tier_durations)
 
       if tier.name not in intervals_vocabulary:
         intervals_vocabulary[tier.name] = []
       vocabulary = [interval.mark for interval in tier.intervals]
       intervals_vocabulary[tier.name].extend(vocabulary)
 
-  total_duration = sum(durations)
-  logger.info(
-    f"Total duration: {total_duration:.2f}s / {total_duration/60:.2f}min / {total_duration/60/60:.2f}h")
+  durations_df = get_durations_df(np.array(durations))
+  with pd.option_context(
+    'display.max_rows', None,
+    'display.max_columns', None,
+    "display.width", None,
+    "display.precision", 4):
+    logger.info(f"Grid duration statistics:\n{durations_df.to_string(index=False)}")
 
   mark_log = print_mark_stats(intervals_vocabulary)
   fig = get_durations_fig(intervals_durations, durations)
 
   return (None, False), fig, mark_log
 
 
+def get_durations_df(durations: np.ndarray) -> pd.DataFrame:
+  col_count = "#Grids"
+  col_min = "Min (s)"
+  col_median = "Median (s)"
+  col_max = "Max (s)"
+  col_mean = "Mean (s)"
+  col_sd = "SD (s)"
+  col_kurt = "Kurt (s)"
+  col_sum_s = "Sum (s)"
+  col_sum_min = "Sum (min)"
+  col_sum_h = "Sum (h)"
+
+  data = OrderedDict((
+    (col_count, len(durations)),
+    (col_min, np.min(durations)),
+    (col_median, np.median(durations)),
+    (col_max, np.max(durations)),
+    (col_mean, np.mean(durations)),
+    (col_sd, np.std(durations)),
+    (col_kurt, kurtosis(durations)),
+    (col_sum_s, np.sum(durations)),
+    (col_sum_min, np.sum(durations) / 60),
+    (col_sum_h, np.sum(durations) / 3600),
+  ))
+  result = pd.DataFrame.from_records([data])
+  return result
+
+
 def print_mark_stats(vocabulary: Dict[str, List[str]]) -> str:
   result = ""
   for tier, symbols in vocabulary.items():
     df = get_marks_df(symbols)
     result += f"Tier:;\"{tier}\"\n\n"
     with io.StringIO() as stream:
       df.to_csv(stream, sep=";", index=False)
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/helper.py` & `textgrid-tools-0.0.8/src/textgrid_tools/helper.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/__init__.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/__init__.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/between_marks_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/between_marks_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/between_pause_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/between_pause_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/boundary_fixing.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/boundary_fixing.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/boundary_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/boundary_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/common.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/common.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/duration_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/duration_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/durations_plotting.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/durations_plotting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/mark_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/mark_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/removing.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/removing.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/splitting.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/splitting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/symbols_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/symbols_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/template_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/template_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/intervals/text_replacement.py` & `textgrid-tools-0.0.8/src/textgrid_tools/intervals/text_replacement.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tier/cloning.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tier/cloning.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tier/exporting.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tier/exporting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tier/importing.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tier/importing.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tier/mapping.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tier/mapping.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tier/moving.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tier/moving.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tier/renaming.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tier/renaming.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tiers/marks_mapping.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tiers/marks_mapping.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tiers/removing.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tiers/removing.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tiers/silence_labeling.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tiers/silence_labeling.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tiers/symbol_removing.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tiers/symbol_removing.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/tiers/transcription.py` & `textgrid-tools-0.0.8/src/textgrid_tools/tiers/transcription.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools/validation.py` & `textgrid-tools-0.0.8/src/textgrid_tools/validation.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools.egg-info/PKG-INFO` & `textgrid-tools-0.0.8/src/textgrid_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textgrid-tools
-Version: 0.0.7
+Version: 0.0.8
 Summary: Command-line interface (CLI) to modify TextGrids and their corresponding audio files.
 Author-email: Stefan Taubert <pypi@stefantaubert.com>
 Maintainer-email: Stefan Taubert <pypi@stefantaubert.com>
 License: MIT
 Project-URL: Homepage, https://github.com/stefantaubert/textgrid-ipa
 Project-URL: Issues, https://github.com/stefantaubert/textgrid-ipa/issues
 Keywords: Text-to-speech,Speech synthesis,praat,TextGrid,Utils,Language,Linguistics
@@ -30,16 +30,16 @@
 # textgrid-tools
 
 [![PyPI](https://img.shields.io/pypi/v/textgrid-tools.svg)](https://pypi.python.org/pypi/textgrid-tools)
 ![PyPI](https://img.shields.io/pypi/pyversions/textgrid-tools.svg)
 [![MIT](https://img.shields.io/github/license/stefantaubert/textgrid-ipa.svg)](https://github.com/stefantaubert/textgrid-ipa/blob/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/wheel/textgrid-tools.svg)](https://pypi.python.org/pypi/textgrid-tools/#files)
 ![PyPI](https://img.shields.io/pypi/implementation/textgrid-tools.svg)
-[![PyPI](https://img.shields.io/github/commits-since/stefantaubert/textgrid-ipa/latest/main.svg)](https://github.com/stefantaubert/textgrid-ipa/compare/v0.0.7...main)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7528782.svg)](https://doi.org/10.5281/zenodo.7528782)
+[![PyPI](https://img.shields.io/github/commits-since/stefantaubert/textgrid-ipa/latest/main.svg)](https://github.com/stefantaubert/textgrid-ipa/compare/v0.0.8...main)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7986716.svg)](https://doi.org/10.5281/zenodo.7986716)
 
 Command-line interface (CLI) to modify TextGrids and their corresponding audio files.
 
 ## Features
 
 - grids
   - `merge`: merge grids together
@@ -193,22 +193,31 @@
 
 ## Citation
 
 If you want to cite this repo, you can use this BibTeX-entry generated by GitHub (see *About => Cite this repository*).
 
 ## Changelog
 
+- v0.0.8 (2023-05-30)
+  - Fixed:
+    - Bugfix `intervals remove` copying on different in/out-locations
+    - Bugfix `import-paths` and `import-audio-paths` option `--symlink` is now creating symbolic links instead of hard links
+  - Changed:
+    - Improved logging in `import-paths` and `import-audio-paths`
+    - Improved logging of durations in `grids plot-stats`
+  - Added:
+    - Added option to get durations from audio files on `grids export-durations`
 - v0.0.7 (2023-01-12)
-  - Fixed
+  - Fixed:
     - Bugfix `grids import-paths` and `grids import-audio-paths`
-  - Added
+  - Added:
     - Added option `--ignore` to ignore custom marks in `grids export-vocabulary`
     - Added option `--mode` to `intervals replace-text` to replace text on different interval positions
     - Added returning of an exit code
-  - Removed
+  - Removed:
     - Removed `tiers mark-silence` because `grids mark-durations` should be used
     - Removed `tiers remove-symbols` because `intervals replace-text` should be used
     - Removed `intervals join-between-pauses` because `join-between-marks` should be used
 - v0.0.6 (2022-12-23)
   - improved validation for pronunciation dictionary creation
   - bugfix replace text logging
   - added intervals join-template
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools.egg-info/SOURCES.txt` & `textgrid-tools-0.0.8/src/textgrid_tools.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -117,55 +117,53 @@
 src/textgrid_tools_tests/grids/durations_labelling_py/test_filter_intervals_by_duration.py
 src/textgrid_tools_tests/grids/durations_labelling_py/test_filter_intervals_by_mark.py
 src/textgrid_tools_tests/grids/durations_labelling_py/test_get_percentile_boundary.py
 src/textgrid_tools_tests/grids/durations_labelling_py/test_get_percentual_boundary.py
 src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_absolute.py
 src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_all.py
 src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_separate.py
+src/textgrid_tools_tests/helper_py/__init__.py
+src/textgrid_tools_tests/helper_py/test_check_intervals_are_consecutive copy.py
+src/textgrid_tools_tests/helper_py/test_set_intervals_consecutive.py
 src/textgrid_tools_tests/intervals/__init__.py
-src/textgrid_tools_tests/intervals/py_between_pause_joining/__init__.py
-src/textgrid_tools_tests/intervals/py_between_pause_joining/test_get_chunks.py
-src/textgrid_tools_tests/intervals/py_between_pause_joining/test_group_adjacent_pauses.py
-src/textgrid_tools_tests/intervals/py_common/__init__.py
-src/textgrid_tools_tests/intervals/py_common/test_group_adjacent_content_and_pauses.py
-src/textgrid_tools_tests/intervals/py_common/test_merge_intervals.py
-src/textgrid_tools_tests/intervals/py_duration_joining/__init__.py
-src/textgrid_tools_tests/intervals/py_duration_joining/test_chunk_intervals_with_pauses.py
-src/textgrid_tools_tests/intervals/py_duration_joining/test_chunk_intervals_without_pauses.py
-src/textgrid_tools_tests/intervals/py_duration_joining/test_get_duration_chunks.py
-src/textgrid_tools_tests/intervals/py_duration_joining/test_split_pauses.py
-src/textgrid_tools_tests/intervals/py_duration_joining/test_split_pauses_at_end.py
-src/textgrid_tools_tests/intervals/py_duration_joining/test_split_pauses_at_start.py
-src/textgrid_tools_tests/intervals/py_removing/__init__.py
-src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_all.py
-src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_both.py
-src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_end.py
-src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_start.py
-src/textgrid_tools_tests/intervals/py_removing/test_get_sync_times.py
-src/textgrid_tools_tests/intervals/py_removing/test_merge_consecutives.py
-src/textgrid_tools_tests/intervals/py_removing/test_remove_intervals_from_tiers.py
-src/textgrid_tools_tests/intervals/py_sentence_joining/__init__.py
-src/textgrid_tools_tests/intervals/py_splitting/__init__.py
-src/textgrid_tools_tests/intervals/py_splitting/test_get_split_intervals.py
-src/textgrid_tools_tests/intervals/py_splitting/test_split_intervals.py
-src/textgrid_tools_tests/intervals/py_text_replacement/__init__.py
-src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_all.py
-src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_begin.py
-src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_both.py
-src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_end.py
-src/textgrid_tools_tests/intervals/py_text_replacement/test_replace_text.py
-src/textgrid_tools_tests/intervals/test_splitting_v2_py/__init__.py
-src/textgrid_tools_tests/intervals/test_splitting_v2_py/test_get_split_intervals_v2.py
-src/textgrid_tools_tests/intervals/test_symbols_joining_py/__init__.py
-src/textgrid_tools_tests/intervals/test_symbols_joining_py/test_chunk_intervals.py
-src/textgrid_tools_tests/intervals/test_symbols_joining_py/test_merge_right_core2.py
-src/textgrid_tools_tests/intervals/test_template_joining/__init__.py
-src/textgrid_tools_tests/intervals/test_template_joining/test_chunk_intervals_boundary.py
-src/textgrid_tools_tests/py_helper/__init__.py
-src/textgrid_tools_tests/py_helper/test_check_intervals_are_consecutive copy.py
-src/textgrid_tools_tests/py_helper/test_set_intervals_consecutive.py
+src/textgrid_tools_tests/intervals/between_pause_joining_py/__init__.py
+src/textgrid_tools_tests/intervals/between_pause_joining_py/test_get_chunks.py
+src/textgrid_tools_tests/intervals/between_pause_joining_py/test_group_adjacent_pauses.py
+src/textgrid_tools_tests/intervals/common_py/__init__.py
+src/textgrid_tools_tests/intervals/common_py/test_group_adjacent_content_and_pauses.py
+src/textgrid_tools_tests/intervals/common_py/test_merge_intervals.py
+src/textgrid_tools_tests/intervals/duration_joining_py/__init__.py
+src/textgrid_tools_tests/intervals/duration_joining_py/test_chunk_intervals_with_pauses.py
+src/textgrid_tools_tests/intervals/duration_joining_py/test_chunk_intervals_without_pauses.py
+src/textgrid_tools_tests/intervals/duration_joining_py/test_get_duration_chunks.py
+src/textgrid_tools_tests/intervals/duration_joining_py/test_split_pauses.py
+src/textgrid_tools_tests/intervals/duration_joining_py/test_split_pauses_at_end.py
+src/textgrid_tools_tests/intervals/duration_joining_py/test_split_pauses_at_start.py
+src/textgrid_tools_tests/intervals/removing_py/__init__.py
+src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_all.py
+src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_both.py
+src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_end.py
+src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_start.py
+src/textgrid_tools_tests/intervals/removing_py/test_get_sync_times.py
+src/textgrid_tools_tests/intervals/removing_py/test_merge_consecutives.py
+src/textgrid_tools_tests/intervals/removing_py/test_remove_intervals_from_tiers.py
+src/textgrid_tools_tests/intervals/sentence_joining_py/__init__.py
+src/textgrid_tools_tests/intervals/splitting_py/__init__.py
+src/textgrid_tools_tests/intervals/splitting_py/test_get_split_intervals.py
+src/textgrid_tools_tests/intervals/splitting_py/test_split_intervals.py
+src/textgrid_tools_tests/intervals/symbols_joining_py/__init__.py
+src/textgrid_tools_tests/intervals/symbols_joining_py/test_chunk_intervals.py
+src/textgrid_tools_tests/intervals/symbols_joining_py/test_merge_right_core2.py
+src/textgrid_tools_tests/intervals/template_joining_py/__init__.py
+src/textgrid_tools_tests/intervals/template_joining_py/test_chunk_intervals_boundary.py
+src/textgrid_tools_tests/intervals/text_replacement_py/__init__.py
+src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_all.py
+src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_begin.py
+src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_both.py
+src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_end.py
+src/textgrid_tools_tests/intervals/text_replacement_py/test_replace_text.py
 src/textgrid_tools_tests/tier/__init__.py
-src/textgrid_tools_tests/tier/py_moving/__init__.py
-src/textgrid_tools_tests/tier/py_moving/test_move_tier.py
+src/textgrid_tools_tests/tier/moving_py/__init__.py
+src/textgrid_tools_tests/tier/moving_py/test_move_tier.py
 src/textgrid_tools_tests/tiers/__init__.py
-src/textgrid_tools_tests/tiers/py_symbol_removing/__init__.py
-src/textgrid_tools_tests/tiers/py_symbol_removing/test_get_updated_mark.py
+src/textgrid_tools_tests/tiers/symbol_removing_py/__init__.py
+src/textgrid_tools_tests/tiers/symbol_removing_py/test_get_updated_mark.py
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/__init__.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/cli.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from time import perf_counter
 from typing import Callable, Dict, Generator, List, Tuple
 
 from textgrid_tools_cli import *
 from textgrid_tools_cli.grids.audio_paths_exporting import get_audio_paths_exporting_parser
 from textgrid_tools_cli.grids.audio_paths_importing import get_audio_paths_importing_parser
 from textgrid_tools_cli.grids.durations_labelling import get_grids_label_durations_parser
-from textgrid_tools_cli.grids.grid_durations_exporting import get_grid_durations_exporting_parser
+from textgrid_tools_cli.grids.grid_durations_exporting import get_durations_exporting_parser
 from textgrid_tools_cli.grids.grid_paths_exporting import get_grid_paths_exporting_parser
 from textgrid_tools_cli.grids.grid_paths_importing import get_grid_paths_importing_parser
 from textgrid_tools_cli.grids.pronunciations_exporting import get_pronunciations_exporting_parser
 from textgrid_tools_cli.grids.stats_generation import get_grids_plot_stats_parser
 from textgrid_tools_cli.helper import get_optional, parse_path
 from textgrid_tools_cli.intervals.template_joining import get_template_joining_parser
 from textgrid_tools_cli.intervals.text_replacement import get_text_replacement_parser
@@ -46,15 +46,15 @@
   yield "merge", "merge grids together", get_grids_merging_parser
   yield "plot-durations", "plot durations", get_grids_plot_interval_durations_parser
   yield "mark-durations", "mark intervals with specific durations with a text", get_grids_label_durations_parser
   yield "create-dictionary", "create pronunciation dictionary out of a word and a pronunciation tier", get_pronunciations_exporting_parser
   yield "plot-stats", "plot statistics", get_grids_plot_stats_parser
   yield "export-vocabulary", "export vocabulary out of multiple grid files", get_vocabulary_export_parser
   yield "export-marks", "exports marks of a tier to a file", get_marks_exporting_parser
-  yield "export-durations", "exports durations of grids to a file", get_grid_durations_exporting_parser
+  yield "export-durations", "exports durations of grids to a file", get_durations_exporting_parser
   yield "export-paths", "exports grid paths to a file", get_grid_paths_exporting_parser
   yield "export-audio-paths", "exports audio paths to a file", get_audio_paths_exporting_parser
   yield "import-paths", "import grids from paths written in a file", get_grid_paths_importing_parser
   yield "import-audio-paths", "import audio files from paths written in a file", get_audio_paths_importing_parser
 
 
 def get_grid_parsers() -> Parsers:
@@ -207,15 +207,15 @@
       logger.info("Didn't changed anything.")
       flogger.info("Didn't changed anything.")
 
     duration = perf_counter() - start
     flogger.debug(f"Total duration (s): {duration}")
 
     if log_to_file:
-      logger.info(f"Written log to: {ns.log.absolute()}")
+      logger.info(f"Written log to: \"{ns.log.absolute()}\".")
 
     if not success:
       sys.exit(1)
     sys.exit(0)
   else:
     parser.print_help()
     sys.exit(0)
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/common.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/common.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/globals.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/globals.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grid/audio_synchronization.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grid/audio_synchronization.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grid/creation.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grid/creation.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grid/splitting.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grid/splitting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grid/stats_generation.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grid/stats_generation.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/audio_paths_exporting.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/audio_paths_exporting.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
   add_encoding_argument(parser, "OUTPUT encoding")
   return export_audio_paths_ns
 
 
 def export_audio_paths_ns(ns: Namespace) -> ExecutionResult:
   logger = init_and_get_console_logger(__name__)
 
-  grid_files = get_audio_files(ns.directory)
+  audio_files = get_audio_files(ns.directory)
 
   paths: List[str] = []
-  for file_nr, (file_stem, rel_path) in enumerate(tqdm(grid_files.items()), start=1):
+  for file_nr, (file_stem, rel_path) in enumerate(tqdm(audio_files.items()), start=1):
     audio_file_in_abs: Path = ns.directory / rel_path
     paths.append(str(audio_file_in_abs.absolute()))
 
   txt = "\n".join(paths)
 
   ns.output.parent.mkdir(parents=True, exist_ok=True)
   ns.output.write_text(txt, ns.encoding)
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/audio_paths_importing.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/grids_merging.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,83 +1,74 @@
-import os
 from argparse import ArgumentParser, Namespace
-from pathlib import Path
-from shutil import copy
-from typing import cast
+from typing import Callable, List
 
-from ordered_set import OrderedSet
+from textgrid import TextGrid
+from tqdm import tqdm
 
+from textgrid_tools.grids.grid_merging import merge_grids
 from textgrid_tools_cli.globals import ExecutionResult
-from textgrid_tools_cli.helper import (add_encoding_argument, get_optional, parse_path,
-                                       parse_txt_path)
+from textgrid_tools_cli.helper import (add_directory_argument, add_encoding_argument,
+                                       get_grid_files, get_optional, parse_path,
+                                       parse_positive_float, try_load_grid, try_save_grid)
 from textgrid_tools_cli.logging_configuration import get_file_logger, init_and_get_console_logger
 
 
-def get_audio_paths_importing_parser(parser: ArgumentParser):
-  parser.description = "This command imports all files from one text file containing paths."
-  parser.add_argument("path", type=parse_txt_path, metavar="PATH",
-                      help="path to import the paths (*.txt)")
-  parser.add_argument("output_directory", metavar='OUTPUT-PATH', type=parse_path,
-                      help="directory where to copy the audio files")
-  parser.add_argument("--relative-to", type=get_optional(parse_path), metavar="REL-PATH",
-                      help="parse paths in PATHS relative to REL-PATH to import files with the same folder structure", default=None)
-  add_encoding_argument(parser, "PATHS encoding")
-  parser.add_argument("-s", "--symlink", action="store_true",
-                      help="create symbolic links instead of copying")
-  return export_grid_paths_ns
+def get_grids_merging_parser(parser: ArgumentParser) -> Callable:
+  parser.description = "This command merges grid files."
+  add_directory_argument(parser)
+  parser.add_argument("output", type=parse_path, metavar="OUTPUT",
+                      help="file to write the generated grid (.TextGrid)")
+  parser.add_argument("--insert-duration", type=get_optional(parse_positive_float), metavar="DURATION",
+                      help="insert an interval between subsequent grids having this duration and mark as content", default=None)
+  parser.add_argument(
+    "--insert-mark", type=str, help="set this mark in the inserted interval (only if insert-duration > 0)", metavar="MARK", default="")
+  add_encoding_argument(parser)
+  return merge_grids_app
 
 
-def export_grid_paths_ns(ns: Namespace) -> ExecutionResult:
+def merge_grids_app(ns: Namespace) -> ExecutionResult:
   logger = init_and_get_console_logger(__name__)
   flogger = get_file_logger()
 
-  try:
-    text: str = ns.path.read_text(ns.encoding)
-  except Exception as ex:
-    logger.error("PATH couldn't be loaded.")
-    logger.exception(ex)
-    return False, False
+  grid_files = get_grid_files(ns.directory)
+
+  grids: List[TextGrid] = []
+  for file_nr, (file_stem, rel_path) in enumerate(tqdm(grid_files.items()), start=1):
+    flogger.info(f"Processing {file_stem}")
+    grid_file_in_abs = ns.directory / rel_path
+    error, grid = try_load_grid(grid_file_in_abs, ns.encoding)
+
+    if error:
+      flogger.debug(error.exception)
+      flogger.error(error.default_message)
+      flogger.info("Skipped.")
+      continue
+    assert grid is not None
+
+    grids.append(grid)
+
+  success = error is None
 
-  try:
-    paths: OrderedSet[Path] = OrderedSet(Path(path) for path in text.split("\n"))
-  except Exception as ex:
-    logger.error("PATHS couldn't be parsed.")
-    logger.exception(ex)
+  if not success:
+    logger.error(error.default_message)
     return False, False
 
-  logger.info(f"Parsed {len(paths)} unique paths.")
+  (error, changed_anything), merged_grid = merge_grids(
+    grids, ns.insert_duration, ns.insert_mark, flogger)
 
-  path: Path
-  for path in paths:
-    target_dir = cast(Path, ns.output_directory)
-    if not path.is_file():
-      logger.error(f"Path \"{path}\" is no file.")
-      logger.exception(ex)
-      return False, False
-
-    if ns.relative_to is None:
-      target_path = target_dir / path.name
-    else:
-      try:
-        target_path = target_dir / path.relative_to(ns.relative_to)
-      except ValueError as error:
-        logger.error(f"Path \"{ns.relative_to}\" is not relative to \"{path}\"!")
-        logger.exception(error)
-        return False, False
-
-    try:
-      target_path.parent.mkdir(parents=True, exist_ok=True)
-      if ns.symlink:
-        flogger.info(
-          f"Creating symbolic link of \"{path.absolute()}\" at \"{target_path.absolute()}\"")
-        os.link(path, target_path, follow_symlinks=False)
-      else:
-        flogger.info(f"Copying \"{path.absolute()}\" to \"{target_path.absolute()}\"")
-        copy(path, target_path)
-    except Exception as ex:
-      logger.error(f"Couldn't copy \"{path.absolute()}\" to \"{target_path.absolute()}\"!")
-      logger.exception(ex)
-      return False, False
+  success = error is None
+
+  if not success:
+    logger.error(error.default_message)
+    return False, False
+
+  logger.info("Saving grid...")
+  error = try_save_grid(ns.output, merged_grid, ns.encoding)
+  if error is not None:
+    flogger.debug(error.exception)
+    flogger.error(error.default_message)
+    flogger.info("Skipped.")
+    return False, False
 
-  logger.info(f"Imported {len(paths)} path(s) to: \"{ns.output_directory.absolute()}\".")
+  logger.info(f"Written grid to: {ns.output.absolute()}")
 
   return True, True
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/durations_labelling.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/durations_labelling.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/durations_plotting.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/durations_plotting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/grid_durations_exporting.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/grid_durations_exporting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,74 @@
 from argparse import ArgumentParser, Namespace
 from typing import List
 
 from tqdm import tqdm
 
+from textgrid_tools.helper import samples_to_s
 from textgrid_tools_cli.globals import ExecutionResult
 from textgrid_tools_cli.helper import (add_directory_argument, add_encoding_argument,
-                                       get_grid_files, parse_txt_path, try_load_grid)
+                                       get_audio_files, get_grid_files, parse_txt_path, read_audio,
+                                       try_load_grid)
 from textgrid_tools_cli.logging_configuration import get_file_logger, init_and_get_console_logger
 
 
-def get_grid_durations_exporting_parser(parser: ArgumentParser):
-  parser.description = "This command exports the durations of all grid files into one text file."
+def get_durations_exporting_parser(parser: ArgumentParser):
+  parser.description = "This command exports the durations of all grid/audio files into one text file."
   add_directory_argument(parser)
   parser.add_argument("output", type=parse_txt_path, metavar="OUTPUT",
                       help="path to output the durations (*.txt)")
+  parser.add_argument("--mode", type=str, choices=["grid", "audio"],
+                      default="grid", help="from which files the audio should be taken")
   add_encoding_argument(parser, "encoding of input grid files and OUTPUT text file")
-  return export_grid_paths_ns
+  return export_durations_ns
 
 
-def export_grid_paths_ns(ns: Namespace) -> ExecutionResult:
+def export_durations_ns(ns: Namespace) -> ExecutionResult:
   logger = init_and_get_console_logger(__name__)
   flogger = get_file_logger()
 
-  grid_files = get_grid_files(ns.directory)
+  use_grids = True
+  if ns.mode == "grid":
+    files = get_grid_files(ns.directory)
+  else:
+    assert ns.mode == "audio"
+    files = get_audio_files(ns.directory)
+    use_grids = False
 
   durations: List[str] = []
   # TODO all successful false on skipped files
   all_successful = True
-  for file_nr, (file_stem, rel_path) in enumerate(tqdm(grid_files.items()), start=1):
+  for file_nr, (file_stem, rel_path) in enumerate(tqdm(files.items()), start=1):
     flogger.info(f"Processing {file_stem}")
-    grid_file_in_abs = ns.directory / rel_path
-    error, grid = try_load_grid(grid_file_in_abs, ns.encoding)
+    file_in_abs = ns.directory / rel_path
 
-    if error:
-      flogger.debug(error.exception)
-      flogger.error(error.default_message)
-      flogger.info("Skipped.")
-      all_successful = False
-      continue
-    assert grid is not None
-
-    grid_duration = grid.maxTime - grid.minTime
-    durations.append(str(grid_duration))
+    if use_grids:
+      error, grid = try_load_grid(file_in_abs, ns.encoding)
+      if error:
+        flogger.debug(error.exception)
+        flogger.error(error.default_message)
+        flogger.info("Skipped.")
+        all_successful = False
+        continue
+      assert grid is not None
+
+      grid_duration = grid.maxTime - grid.minTime
+      durations.append(str(grid_duration))
+    else:
+      try:
+        sample_rate, audio_in = read_audio(file_in_abs)
+      except Exception as ex:
+        flogger.debug(ex)
+        flogger.error("Audio file couldn't be read!")
+        flogger.info("Skipped.")
+        all_successful = False
+        continue
+      audio_samples_in = audio_in.shape[0]
+      duration_s = samples_to_s(audio_samples_in, sample_rate)
+      durations.append(str(duration_s))
 
   txt = "\n".join(durations)
 
   ns.output.parent.mkdir(parents=True, exist_ok=True)
   ns.output.write_text(txt, ns.encoding)
   logger.info(f"Exported {len(durations)} duration(s) to: \"{ns.output.absolute()}\".")
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/grid_paths_exporting.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/grid_paths_exporting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/grid_paths_importing.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/audio_paths_importing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import os
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 from shutil import copy
 from typing import cast
 
 from ordered_set import OrderedSet
+from tqdm import tqdm
 
 from textgrid_tools_cli.globals import ExecutionResult
 from textgrid_tools_cli.helper import (add_encoding_argument, get_optional, parse_path,
                                        parse_txt_path)
 from textgrid_tools_cli.logging_configuration import get_file_logger, init_and_get_console_logger
 
 
-def get_grid_paths_importing_parser(parser: ArgumentParser):
+def get_audio_paths_importing_parser(parser: ArgumentParser):
   parser.description = "This command imports all files from one text file containing paths."
   parser.add_argument("path", type=parse_txt_path, metavar="PATH",
                       help="path to import the paths (*.txt)")
   parser.add_argument("output_directory", metavar='OUTPUT-PATH', type=parse_path,
-                      help="directory where to copy the grid files")
+                      help="directory where to copy the audio files")
   parser.add_argument("--relative-to", type=get_optional(parse_path), metavar="REL-PATH",
                       help="parse paths in PATHS relative to REL-PATH to import files with the same folder structure", default=None)
+  add_encoding_argument(parser, "PATHS encoding")
   parser.add_argument("-s", "--symlink", action="store_true",
                       help="create symbolic links instead of copying")
-  add_encoding_argument(parser, "PATHS encoding")
-  return export_grid_paths_ns
+  return import_audio_paths_ns
 
 
-def export_grid_paths_ns(ns: Namespace) -> ExecutionResult:
+def import_audio_paths_ns(ns: Namespace) -> ExecutionResult:
   logger = init_and_get_console_logger(__name__)
   flogger = get_file_logger()
 
   try:
     text: str = ns.path.read_text(ns.encoding)
   except Exception as ex:
     logger.error("PATH couldn't be loaded.")
@@ -43,15 +43,15 @@
     logger.error("PATHS couldn't be parsed.")
     logger.exception(ex)
     return False, False
 
   logger.info(f"Parsed {len(paths)} unique paths.")
 
   path: Path
-  for path in paths:
+  for path in tqdm(paths, desc="Importing", unit=" audio(s)"):
     target_dir = cast(Path, ns.output_directory)
     if not path.is_file():
       logger.error(f"Path \"{path}\" is no file.")
       logger.exception(ex)
       return False, False
 
     if ns.relative_to is None:
@@ -62,22 +62,34 @@
       except ValueError as error:
         logger.error(f"Path \"{ns.relative_to}\" is not relative to \"{path}\"!")
         logger.exception(error)
         return False, False
 
     try:
       target_path.parent.mkdir(parents=True, exist_ok=True)
-      if ns.symlink:
+    except Exception as ex:
+      logger.error(f"Target directory \"{target_path.parent.absolute()}\" couldn't be created!")
+      logger.exception(ex)
+      return False, False
+
+    if ns.symlink:
+      try:
         flogger.info(
           f"Creating symbolic link of \"{path.absolute()}\" at \"{target_path.absolute()}\"")
-        os.link(path, target_path, follow_symlinks=False)
-      else:
+        target_path.symlink_to(path, target_is_directory=False)
+      except Exception as ex:
+        logger.error(
+          f"Couldn't create symbolic link from \"{path.absolute()}\" to \"{target_path.absolute()}\"!")
+        logger.exception(ex)
+        return False, False
+    else:
+      try:
         flogger.info(f"Copying \"{path.absolute()}\" to \"{target_path.absolute()}\"")
         copy(path, target_path)
-    except Exception as ex:
-      logger.error(f"Couldn't copy \"{path.absolute()}\" to \"{target_path.absolute()}\"!")
-      logger.exception(ex)
-      return False, False
+      except Exception as ex:
+        logger.error(f"Couldn't copy \"{path.absolute()}\" to \"{target_path.absolute()}\"!")
+        logger.exception(ex)
+        return False, False
 
   logger.info(f"Imported {len(paths)} path(s) to: \"{ns.output_directory.absolute()}\".")
 
   return True, True
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/grids_merging.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/durations_plotting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,72 @@
 from argparse import ArgumentParser, Namespace
-from typing import Callable, List
+from logging import getLogger
 
-from textgrid import TextGrid
 from tqdm import tqdm
 
-from textgrid_tools.grids.grid_merging import merge_grids
+from textgrid_tools import plot_interval_durations_diagram
 from textgrid_tools_cli.globals import ExecutionResult
 from textgrid_tools_cli.helper import (add_directory_argument, add_encoding_argument,
-                                       get_grid_files, get_optional, parse_path,
-                                       parse_positive_float, try_load_grid, try_save_grid)
+                                       add_overwrite_argument, add_tiers_argument, get_grid_files,
+                                       get_optional, parse_path, try_load_grid)
 from textgrid_tools_cli.logging_configuration import get_file_logger, init_and_get_console_logger
 
 
-def get_grids_merging_parser(parser: ArgumentParser) -> Callable:
-  parser.description = "This command merges grid files."
+def get_plot_interval_durations_parser(parser: ArgumentParser):
+  parser.description = "This command creates a violin plot of the interval durations."
   add_directory_argument(parser)
-  parser.add_argument("output", type=parse_path, metavar="OUTPUT",
-                      help="file to write the generated grid (.TextGrid)")
-  parser.add_argument("--insert-duration", type=get_optional(parse_positive_float), metavar="DURATION",
-                      help="insert an interval between subsequent grids having this duration and mark as content", default=None)
-  parser.add_argument(
-    "--insert-mark", type=str, help="set this mark in the inserted interval (only if insert-duration > 0)", metavar="MARK", default="")
+  add_tiers_argument(parser, "tiers containing the intervals that should be plotted")
+  parser.add_argument("-out", "--output-directory", metavar='DIRECTORY', type=get_optional(parse_path),
+                      help="directory where to output the plots if not to the same directory")
   add_encoding_argument(parser)
-  return merge_grids_app
+  add_overwrite_argument(parser)
+  return app_plot_interval_durations
 
 
-def merge_grids_app(ns: Namespace) -> ExecutionResult:
+def app_plot_interval_durations(ns: Namespace) -> ExecutionResult:
   logger = init_and_get_console_logger(__name__)
   flogger = get_file_logger()
 
   grid_files = get_grid_files(ns.directory)
 
-  grids: List[TextGrid] = []
+  output_directory = ns.output_directory
+  if output_directory is None:
+    output_directory = ns.directory
+
+  total_success = True
   for file_nr, (file_stem, rel_path) in enumerate(tqdm(grid_files.items()), start=1):
-    flogger.info(f"Processing {file_stem}")
+    flogger.info(f"Processing \"{file_stem}\"")
+
+    pdf_out = output_directory / f"{rel_path.stem}.pdf"
+    png_out = output_directory / f"{rel_path.stem}.png"
+
+    if not ns.overwrite and (pdf_out.exists() or png_out.exists()):
+      flogger.info("Plot already exists. Skipping...")
+      continue
+
     grid_file_in_abs = ns.directory / rel_path
     error, grid = try_load_grid(grid_file_in_abs, ns.encoding)
 
     if error:
       flogger.debug(error.exception)
       flogger.error(error.default_message)
       flogger.info("Skipped.")
       continue
     assert grid is not None
 
-    grids.append(grid)
-
-  success = error is None
-
-  if not success:
-    logger.error(error.default_message)
-    return False, False
+    (error, changed_anything), figure = plot_interval_durations_diagram(grid, ns.tiers, flogger)
+    assert not changed_anything
+    success = error is None
+    total_success &= success
 
-  (error, changed_anything), merged_grid = merge_grids(
-    grids, ns.insert_duration, ns.insert_mark, flogger)
-
-  success = error is None
-
-  if not success:
-    logger.error(error.default_message)
-    return False, False
-
-  logger.info("Saving grid...")
-  error = try_save_grid(ns.output, merged_grid, ns.encoding)
-  if error is not None:
-    flogger.debug(error.exception)
-    flogger.error(error.default_message)
-    flogger.info("Skipped.")
-    return False, False
+    if not success:
+      flogger.error(error.default_message)
+      flogger.info("Skipped.")
+      continue
 
-  logger.info(f"Written grid to: {ns.output.absolute()}")
+    output_directory.mkdir(parents=True, exist_ok=True)
+    getLogger('matplotlib.backends.backend_pdf').disabled = True
+    figure.savefig(pdf_out)
+    getLogger('matplotlib.backends.backend_pdf').disabled = False
+    figure.savefig(png_out)
 
-  return True, True
+  return total_success, True
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/marks_exporting.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/marks_exporting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/pronunciations_exporting.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/pronunciations_exporting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/stats_generation.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/stats_generation.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/grids/vocabulary_export.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/vocabulary_export.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/helper.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/helper.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/__init__.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/__init__.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/between_marks_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/between_marks_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/between_pause_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/between_pause_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/boundary_fixing.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/boundary_fixing.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/boundary_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/boundary_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/duration_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/duration_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/durations_plotting.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/exporting.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,75 @@
 from argparse import ArgumentParser, Namespace
-from logging import getLogger
 
 from tqdm import tqdm
 
-from textgrid_tools import plot_interval_durations_diagram
+from textgrid_tools import convert_tier_to_text
 from textgrid_tools_cli.globals import ExecutionResult
 from textgrid_tools_cli.helper import (add_directory_argument, add_encoding_argument,
-                                       add_overwrite_argument, add_tiers_argument, get_grid_files,
-                                       get_optional, parse_path, try_load_grid)
+                                       add_overwrite_argument, add_tier_argument, get_grid_files,
+                                       get_optional, parse_path, save_text, try_load_grid)
 from textgrid_tools_cli.logging_configuration import get_file_logger, init_and_get_console_logger
 
 
-def get_plot_interval_durations_parser(parser: ArgumentParser):
-  parser.description = "This command creates a violin plot of the interval durations."
+def get_exporting_parser(parser: ArgumentParser):
+  parser.description = "This command writes the content of a tier into a text file."
+
   add_directory_argument(parser)
-  add_tiers_argument(parser, "tiers containing the intervals that should be plotted")
-  parser.add_argument("-out", "--output-directory", metavar='DIRECTORY', type=get_optional(parse_path),
-                      help="directory where to output the plots if not to the same directory")
-  add_encoding_argument(parser)
+  add_tier_argument(parser, "tier from which the content should be written")
+  add_encoding_argument(parser, "encoding of grid and text files")
+  parser.add_argument("-out", "--output-directory", metavar='OUTPUT-DIRECTORY', type=get_optional(parse_path),
+                      help="directory where to output the text files if not to the same directory", default=None)
+  parser.add_argument('--sep', type=str, metavar="SYMBOL",
+                      help="use this symbol to separate the marks of each interval", default="\n")
   add_overwrite_argument(parser)
-  return app_plot_interval_durations
+  return app_convert_tier_to_text
 
 
-def app_plot_interval_durations(ns: Namespace) -> ExecutionResult:
+def app_convert_tier_to_text(ns: Namespace) -> ExecutionResult:
   logger = init_and_get_console_logger(__name__)
   flogger = get_file_logger()
 
-  grid_files = get_grid_files(ns.directory)
-
   output_directory = ns.output_directory
   if output_directory is None:
     output_directory = ns.directory
 
+  grid_files = get_grid_files(ns.directory)
+
   total_success = True
   for file_nr, (file_stem, rel_path) in enumerate(tqdm(grid_files.items()), start=1):
-    flogger.info(f"Processing \"{file_stem}\"")
-
-    pdf_out = output_directory / f"{rel_path.stem}.pdf"
-    png_out = output_directory / f"{rel_path.stem}.png"
-
-    if not ns.overwrite and (pdf_out.exists() or png_out.exists()):
-      flogger.info("Plot already exists. Skipping...")
+    flogger.info(f"Processing {file_stem}")
+    text_file_out_abs = output_directory / f"{file_stem}.txt"
+    if text_file_out_abs.exists() and not ns.overwrite:
+      flogger.info("Text file already exists. Skipped.")
       continue
 
     grid_file_in_abs = ns.directory / rel_path
     error, grid = try_load_grid(grid_file_in_abs, ns.encoding)
 
     if error:
       flogger.debug(error.exception)
       flogger.error(error.default_message)
       flogger.info("Skipped.")
       continue
     assert grid is not None
 
-    (error, changed_anything), figure = plot_interval_durations_diagram(grid, ns.tiers, flogger)
-    assert not changed_anything
+    (error, _), text = convert_tier_to_text(grid, ns.tier, ns.sep, flogger)
+
     success = error is None
     total_success &= success
 
     if not success:
       flogger.error(error.default_message)
       flogger.info("Skipped.")
       continue
 
-    output_directory.mkdir(parents=True, exist_ok=True)
-    getLogger('matplotlib.backends.backend_pdf').disabled = True
-    figure.savefig(pdf_out)
-    getLogger('matplotlib.backends.backend_pdf').disabled = False
-    figure.savefig(png_out)
+    try:
+      save_text(text_file_out_abs, text, ns.encoding)
+    except Exception as ex:
+      flogger.debug(ex)
+      flogger.error("Text couldn't be saved!")
+      flogger.info("Skipped.")
+      total_success = False
+      continue
 
+  logger.info(f"Written output to: {output_directory.absolute()}")
   return total_success, True
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/mark_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/mark_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/removing.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/removing.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
           flogger.debug(ex)
           flogger.error("Audio couldn't be saved!")
           flogger.info("Skipped.")
           total_success = False
           continue
       elif ns.directory != output_directory:
         try:
-          copy_audio(audio_file_out_abs, audio_file_in_abs)
+          copy_audio(audio_file_in_abs, audio_file_out_abs)
         except Exception as ex:
           flogger.debug(ex)
           flogger.error("Audio couldn't be saved!")
           flogger.info("Skipped.")
           total_success = False
           continue
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/splitting.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/splitting.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/symbols_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/symbols_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/template_joining.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/template_joining.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/intervals/text_replacement.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/intervals/text_replacement.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/logging_configuration.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/textgrid_io.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/textgrid_io.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/cloning.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/cloning.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/exporting.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/importing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,93 @@
 from argparse import ArgumentParser, Namespace
 
 from tqdm import tqdm
 
-from textgrid_tools import convert_tier_to_text
+from textgrid_tools.tier.importing import import_text_to_tier
 from textgrid_tools_cli.globals import ExecutionResult
 from textgrid_tools_cli.helper import (add_directory_argument, add_encoding_argument,
-                                       add_overwrite_argument, add_tier_argument, get_grid_files,
-                                       get_optional, parse_path, save_text, try_load_grid)
+                                       add_overwrite_argument, add_tier_argument, get_optional,
+                                       get_text_files, parse_existing_directory, parse_path,
+                                       try_load_grid, try_save_grid)
 from textgrid_tools_cli.logging_configuration import get_file_logger, init_and_get_console_logger
 
 
-def get_exporting_parser(parser: ArgumentParser):
-  parser.description = "This command writes the content of a tier into a text file."
+def get_importing_parser(parser: ArgumentParser):
+  parser.description = "This command imports a tier from a text file."
 
   add_directory_argument(parser)
-  add_tier_argument(parser, "tier from which the content should be written")
+  add_tier_argument(parser, "new tier to which the content should be written")
   add_encoding_argument(parser, "encoding of grid and text files")
+  parser.add_argument("--text-directory", metavar='TEXT-DIRECTORY', type=get_optional(parse_existing_directory),
+                      help="directory where to read the text files; defaults to dictionary if not set", default=None)
   parser.add_argument("-out", "--output-directory", metavar='OUTPUT-DIRECTORY', type=get_optional(parse_path),
-                      help="directory where to output the text files if not to the same directory", default=None)
+                      help="directory where to output the grid files if not to the same directory", default=None)
   parser.add_argument('--sep', type=str, metavar="SYMBOL",
                       help="use this symbol to separate the marks of each interval", default="\n")
   add_overwrite_argument(parser)
-  return app_convert_tier_to_text
+  return import_text_to_tier_ns
 
 
-def app_convert_tier_to_text(ns: Namespace) -> ExecutionResult:
+def import_text_to_tier_ns(ns: Namespace) -> ExecutionResult:
   logger = init_and_get_console_logger(__name__)
   flogger = get_file_logger()
 
   output_directory = ns.output_directory
   if output_directory is None:
     output_directory = ns.directory
 
-  grid_files = get_grid_files(ns.directory)
+  text_dir = ns.directory
+  if ns.text_directory is not None:
+    text_dir = ns.text_directory
+
+  text_files = get_text_files(text_dir)
 
   total_success = True
-  for file_nr, (file_stem, rel_path) in enumerate(tqdm(grid_files.items()), start=1):
+  for file_nr, (file_stem, rel_path) in enumerate(tqdm(text_files.items()), start=1):
     flogger.info(f"Processing {file_stem}")
-    text_file_out_abs = output_directory / f"{file_stem}.txt"
-    if text_file_out_abs.exists() and not ns.overwrite:
-      flogger.info("Text file already exists. Skipped.")
+    grid_file_in_abs = ns.directory / f"{file_stem}.TextGrid"
+
+    if not grid_file_in_abs.is_file():
+      flogger.warning("No corresponding grid found. Skipped.")
+      continue
+
+    grid_file_out_abs = output_directory / f"{file_stem}.TextGrid"
+    if grid_file_out_abs.exists() and not ns.overwrite:
+      flogger.info("Grid already exists. Skipped.")
       continue
 
-    grid_file_in_abs = ns.directory / rel_path
     error, grid = try_load_grid(grid_file_in_abs, ns.encoding)
 
     if error:
       flogger.debug(error.exception)
       flogger.error(error.default_message)
       flogger.info("Skipped.")
       continue
     assert grid is not None
 
-    (error, _), text = convert_tier_to_text(grid, ns.tier, ns.sep, flogger)
+    try:
+      text = (text_dir / rel_path).read_text(ns.encoding)
+    except Exception as ex:
+      flogger.error("Text couldn't be loaded. Skipped")
+      flogger.exception(ex)
+      continue
+
+    error, _ = import_text_to_tier(grid, ns.tier, text, ns.sep, flogger)
 
     success = error is None
     total_success &= success
 
     if not success:
       flogger.error(error.default_message)
       flogger.info("Skipped.")
       continue
 
-    try:
-      save_text(text_file_out_abs, text, ns.encoding)
-    except Exception as ex:
-      flogger.debug(ex)
-      flogger.error("Text couldn't be saved!")
+    error = try_save_grid(grid_file_out_abs, grid, ns.encoding)
+    if error is not None:
+      flogger.debug(error.exception)
+      flogger.error(error.default_message)
       flogger.info("Skipped.")
       total_success = False
       continue
 
   logger.info(f"Written output to: {output_directory.absolute()}")
   return total_success, True
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/importing.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/grids/grid_paths_importing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,95 @@
 from argparse import ArgumentParser, Namespace
+from pathlib import Path
+from shutil import copy
+from typing import cast
 
+from ordered_set import OrderedSet
 from tqdm import tqdm
 
-from textgrid_tools.tier.importing import import_text_to_tier
 from textgrid_tools_cli.globals import ExecutionResult
-from textgrid_tools_cli.helper import (add_directory_argument, add_encoding_argument,
-                                       add_overwrite_argument, add_tier_argument, get_optional,
-                                       get_text_files, parse_existing_directory, parse_path,
-                                       try_load_grid, try_save_grid)
+from textgrid_tools_cli.helper import (add_encoding_argument, get_optional, parse_path,
+                                       parse_txt_path)
 from textgrid_tools_cli.logging_configuration import get_file_logger, init_and_get_console_logger
 
 
-def get_importing_parser(parser: ArgumentParser):
-  parser.description = "This command imports a tier from a text file."
+def get_grid_paths_importing_parser(parser: ArgumentParser):
+  parser.description = "This command imports all files from one text file containing paths."
+  parser.add_argument("path", type=parse_txt_path, metavar="PATH",
+                      help="path to import the paths (*.txt)")
+  parser.add_argument("output_directory", metavar='OUTPUT-PATH', type=parse_path,
+                      help="directory where to copy the grid files")
+  parser.add_argument("--relative-to", type=get_optional(parse_path), metavar="REL-PATH",
+                      help="parse paths in PATHS relative to REL-PATH to import files with the same folder structure", default=None)
+  parser.add_argument("-s", "--symlink", action="store_true",
+                      help="create symbolic links instead of copying")
+  add_encoding_argument(parser, "PATHS encoding")
+  return import_grid_paths_ns
 
-  add_directory_argument(parser)
-  add_tier_argument(parser, "new tier to which the content should be written")
-  add_encoding_argument(parser, "encoding of grid and text files")
-  parser.add_argument("--text-directory", metavar='TEXT-DIRECTORY', type=get_optional(parse_existing_directory),
-                      help="directory where to read the text files; defaults to dictionary if not set", default=None)
-  parser.add_argument("-out", "--output-directory", metavar='OUTPUT-DIRECTORY', type=get_optional(parse_path),
-                      help="directory where to output the grid files if not to the same directory", default=None)
-  parser.add_argument('--sep', type=str, metavar="SYMBOL",
-                      help="use this symbol to separate the marks of each interval", default="\n")
-  add_overwrite_argument(parser)
-  return import_text_to_tier_ns
 
-
-def import_text_to_tier_ns(ns: Namespace) -> ExecutionResult:
+def import_grid_paths_ns(ns: Namespace) -> ExecutionResult:
   logger = init_and_get_console_logger(__name__)
   flogger = get_file_logger()
 
-  output_directory = ns.output_directory
-  if output_directory is None:
-    output_directory = ns.directory
-
-  text_dir = ns.directory
-  if ns.text_directory is not None:
-    text_dir = ns.text_directory
-
-  text_files = get_text_files(text_dir)
-
-  total_success = True
-  for file_nr, (file_stem, rel_path) in enumerate(tqdm(text_files.items()), start=1):
-    flogger.info(f"Processing {file_stem}")
-    grid_file_in_abs = ns.directory / f"{file_stem}.TextGrid"
-
-    if not grid_file_in_abs.is_file():
-      flogger.warning("No corresponding grid found. Skipped.")
-      continue
-
-    grid_file_out_abs = output_directory / f"{file_stem}.TextGrid"
-    if grid_file_out_abs.exists() and not ns.overwrite:
-      flogger.info("Grid already exists. Skipped.")
-      continue
-
-    error, grid = try_load_grid(grid_file_in_abs, ns.encoding)
-
-    if error:
-      flogger.debug(error.exception)
-      flogger.error(error.default_message)
-      flogger.info("Skipped.")
-      continue
-    assert grid is not None
+  try:
+    text: str = ns.path.read_text(ns.encoding)
+  except Exception as ex:
+    logger.error("PATH couldn't be loaded.")
+    logger.exception(ex)
+    return False, False
+
+  try:
+    paths: OrderedSet[Path] = OrderedSet(Path(path) for path in text.split("\n"))
+  except Exception as ex:
+    logger.error("PATHS couldn't be parsed.")
+    logger.exception(ex)
+    return False, False
+
+  logger.info(f"Parsed {len(paths)} unique paths.")
+
+  path: Path
+  for path in tqdm(paths, desc="Importing", unit=" grid(s)"):
+    target_dir = cast(Path, ns.output_directory)
+    if not path.is_file():
+      logger.error(f"Path \"{path}\" is no file.")
+      logger.exception(ex)
+      return False, False
+
+    if ns.relative_to is None:
+      target_path = target_dir / path.name
+    else:
+      try:
+        target_path = target_dir / path.relative_to(ns.relative_to)
+      except ValueError as error:
+        logger.error(f"Path \"{ns.relative_to}\" is not relative to \"{path}\"!")
+        logger.exception(error)
+        return False, False
 
     try:
-      text = (text_dir / rel_path).read_text(ns.encoding)
+      target_path.parent.mkdir(parents=True, exist_ok=True)
     except Exception as ex:
-      flogger.error("Text couldn't be loaded. Skipped")
-      flogger.exception(ex)
-      continue
-
-    error, _ = import_text_to_tier(grid, ns.tier, text, ns.sep, flogger)
-
-    success = error is None
-    total_success &= success
-
-    if not success:
-      flogger.error(error.default_message)
-      flogger.info("Skipped.")
-      continue
-
-    error = try_save_grid(grid_file_out_abs, grid, ns.encoding)
-    if error is not None:
-      flogger.debug(error.exception)
-      flogger.error(error.default_message)
-      flogger.info("Skipped.")
-      total_success = False
-      continue
+      logger.error(f"Target directory \"{target_path.parent.absolute()}\" couldn't be created!")
+      logger.exception(ex)
+      return False, False
+
+    if ns.symlink:
+      try:
+        flogger.info(
+          f"Creating symbolic link of \"{path.absolute()}\" at \"{target_path.absolute()}\"")
+        target_path.symlink_to(path, target_is_directory=False)
+      except Exception as ex:
+        logger.error(
+          f"Couldn't create symbolic link from \"{path.absolute()}\" to \"{target_path.absolute()}\"!")
+        logger.exception(ex)
+        return False, False
+    else:
+      try:
+        flogger.info(f"Copying \"{path.absolute()}\" to \"{target_path.absolute()}\"")
+        copy(path, target_path)
+      except Exception as ex:
+        logger.error(f"Couldn't copy \"{path.absolute()}\" to \"{target_path.absolute()}\"!")
+        logger.exception(ex)
+        return False, False
+
+  logger.info(f"Imported {len(paths)} path(s) to: \"{ns.output_directory.absolute()}\".")
 
-  logger.info(f"Written output to: {output_directory.absolute()}")
-  return total_success, True
+  return True, True
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/mapping.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/mapping.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/moving.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/moving.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tier/renaming.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tier/renaming.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/marks_mapping.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/marks_mapping.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/removing.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/removing.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/silence_labeling.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/silence_labeling.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/symbol_removing.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/symbol_removing.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/tiers/transcription.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/tiers/transcription.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli/validation.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli/validation.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli_tests/grids/vocabulary_export_py/test_get_vocabulary.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli_tests/grids/vocabulary_export_py/test_get_vocabulary.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli_tests/test_parse_codec.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli_tests/test_parse_codec.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_cli_tests/test_parse_float.py` & `textgrid-tools-0.0.8/src/textgrid_tools_cli_tests/test_parse_float.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_filter_intervals_by_duration.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_filter_intervals_by_duration.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_filter_intervals_by_mark.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_filter_intervals_by_mark.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_get_percentile_boundary.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_get_percentile_boundary.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_get_percentual_boundary.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_get_percentual_boundary.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_absolute.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_absolute.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_all.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_all.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_separate.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/grids/durations_labelling_py/test_label_durations_core_separate.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_between_pause_joining/test_get_chunks.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/between_pause_joining_py/test_get_chunks.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_between_pause_joining/test_group_adjacent_pauses.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/between_pause_joining_py/test_group_adjacent_pauses.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_common/test_group_adjacent_content_and_pauses.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/common_py/test_group_adjacent_content_and_pauses.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_common/test_merge_intervals.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/common_py/test_merge_intervals.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_chunk_intervals_with_pauses.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_chunk_intervals_with_pauses.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_chunk_intervals_without_pauses.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_chunk_intervals_without_pauses.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_get_duration_chunks.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_get_duration_chunks.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_split_pauses.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_split_pauses.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_split_pauses_at_end.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_split_pauses_at_end.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_duration_joining/test_split_pauses_at_start.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/duration_joining_py/test_split_pauses_at_start.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_all.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_all.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_both.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_both.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_end.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_end.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_get_intervals_start.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_get_intervals_start.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_get_sync_times.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_get_sync_times.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_merge_consecutives.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_merge_consecutives.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_removing/test_remove_intervals_from_tiers.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/removing_py/test_remove_intervals_from_tiers.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_splitting/test_split_intervals.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/splitting_py/test_split_intervals.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_all.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_all.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_begin.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_begin.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_both.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_both.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/test_get_intervals_end.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/test_get_intervals_end.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/py_text_replacement/test_replace_text.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/text_replacement_py/test_replace_text.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_splitting_v2_py/test_get_split_intervals_v2.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/splitting_py/test_get_split_intervals.py`

 * *Files 13% similar despite different names*

```diff
@@ -99,7 +99,44 @@
   assert intervals[0] == Interval(0.5, 1.0, "this")
   assert intervals[1] == Interval(1.0, 1.5, " ")
   assert intervals[2] == Interval(1.5, 2.0, "is")
   assert intervals[3] == Interval(2.0, 2.5, " ")
   assert intervals[4] == Interval(2.5, 3.0, "a")
   assert intervals[5] == Interval(3.0, 3.5, " ")
   assert intervals[6] == Interval(3.5, 4, "test")
+
+
+def test_no_space__returns_one_intervals():
+  interval = Interval(0.5, 2, "\"Thistest\"")
+
+  intervals = list(get_split_intervals(interval, " ", False))
+
+  assert len(intervals) == 1
+  assert intervals[0] == Interval(0.5, 2, "\"Thistest\"")
+
+
+def test_one_space__returns_two_intervals():
+  interval = Interval(0.5, 2, "\"This test\"")
+
+  intervals = list(get_split_intervals(interval, " ", False))
+
+  assert len(intervals) == 2
+  assert intervals[0] == Interval(0.5, 1.25, "\"This")
+  assert intervals[1] == Interval(1.25, 2.0, "test\"")
+
+
+def test_double_space__returns_two_intervals():
+  interval = Interval(3, 5, "Is right.")
+
+  intervals = list(get_split_intervals(interval, " ", False))
+
+  assert len(intervals) == 2
+  assert intervals[0] == Interval(3, 4, "Is")
+  assert intervals[1] == Interval(4, 5.0, "right.")
+
+
+def test_component():
+  interval = Interval(3, 5, "Is right and a test and 123 abce: and? \"no\" ??.")
+
+  intervals = list(get_split_intervals(interval, " ", False))
+
+  assert len(intervals) == 11
```

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_symbols_joining_py/test_chunk_intervals.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/symbols_joining_py/test_chunk_intervals.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_symbols_joining_py/test_merge_right_core2.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/symbols_joining_py/test_merge_right_core2.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/intervals/test_template_joining/test_chunk_intervals_boundary.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/intervals/template_joining_py/test_chunk_intervals_boundary.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/py_helper/test_check_intervals_are_consecutive copy.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/helper_py/test_check_intervals_are_consecutive copy.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/py_helper/test_set_intervals_consecutive.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/helper_py/test_set_intervals_consecutive.py`

 * *Files identical despite different names*

### Comparing `textgrid-tools-0.0.7/src/textgrid_tools_tests/tier/py_moving/test_move_tier.py` & `textgrid-tools-0.0.8/src/textgrid_tools_tests/tier/moving_py/test_move_tier.py`

 * *Files identical despite different names*

