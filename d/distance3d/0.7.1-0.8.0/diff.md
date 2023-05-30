# Comparing `tmp/distance3d-0.7.1.tar.gz` & `tmp/distance3d-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distance3d-0.7.1.tar", last modified: Sat Sep 17 16:04:47 2022, max compression
+gzip compressed data, was "distance3d-0.8.0.tar", last modified: Tue May 30 15:07:35 2023, max compression
```

## Comparing `distance3d-0.7.1.tar` & `distance3d-0.8.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2022-09-17 16:04:47.503122 distance3d-0.7.1/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2885 2022-07-12 13:59:15.000000 distance3d-0.7.1/LICENSE
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5262 2022-09-17 16:04:47.503122 distance3d-0.7.1/PKG-INFO
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4633 2022-08-16 14:43:07.000000 distance3d-0.7.1/README.md
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2022-09-17 16:04:47.499122 distance3d-0.7.1/distance3d/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       82 2022-09-17 16:00:24.000000 distance3d-0.7.1/distance3d/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      607 2022-06-17 22:40:17.000000 distance3d-0.7.1/distance3d/benchmark.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5489 2022-08-02 13:24:00.000000 distance3d-0.7.1/distance3d/broad_phase.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    17665 2022-07-12 13:59:15.000000 distance3d-0.7.1/distance3d/colliders.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5288 2022-07-01 09:00:36.000000 distance3d-0.7.1/distance3d/containment.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8078 2022-08-02 13:24:00.000000 distance3d-0.7.1/distance3d/containment_test.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2022-09-17 16:04:47.499122 distance3d-0.7.1/distance3d/distance/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6004 2022-08-17 20:23:57.000000 distance3d-0.7.1/distance3d/distance/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6021 2022-06-24 14:57:25.000000 distance3d-0.7.1/distance3d/distance/_box.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13274 2022-08-19 09:42:13.000000 distance3d-0.7.1/distance3d/distance/_circle.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1340 2022-05-29 20:34:55.000000 distance3d-0.7.1/distance3d/distance/_cylinder.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5108 2022-08-19 09:43:05.000000 distance3d-0.7.1/distance3d/distance/_disk.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3414 2022-06-24 14:57:25.000000 distance3d-0.7.1/distance3d/distance/_ellipsoid.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    10909 2022-06-17 22:40:17.000000 distance3d-0.7.1/distance3d/distance/_line.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    17666 2022-06-24 14:57:25.000000 distance3d-0.7.1/distance3d/distance/_line_to_box.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    12752 2022-08-17 20:23:57.000000 distance3d-0.7.1/distance3d/distance/_plane.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    12127 2022-06-17 22:40:17.000000 distance3d-0.7.1/distance3d/distance/_rectangle.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13543 2022-06-17 22:40:17.000000 distance3d-0.7.1/distance3d/distance/_triangle.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7844 2022-06-17 22:40:17.000000 distance3d-0.7.1/distance3d/epa.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    15704 2022-08-02 13:24:00.000000 distance3d-0.7.1/distance3d/geometry.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2022-09-17 16:04:47.503122 distance3d-0.7.1/distance3d/gjk/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1150 2022-08-16 08:32:11.000000 distance3d-0.7.1/distance3d/gjk/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    23950 2022-08-02 13:24:00.000000 distance3d-0.7.1/distance3d/gjk/_gjk_jolt.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8388 2022-07-12 13:59:15.000000 distance3d-0.7.1/distance3d/gjk/_gjk_libccd.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    43115 2022-08-19 09:10:43.000000 distance3d-0.7.1/distance3d/gjk/_gjk_original.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2022-09-17 16:04:47.503122 distance3d-0.7.1/distance3d/hydroelastic_contact/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1646 2022-08-23 21:04:07.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/__init__.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      396 2022-08-16 08:16:24.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/_barycentric_transform.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2553 2022-08-20 21:45:07.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/_broad_phase.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5609 2022-09-03 21:36:42.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/_contact_surface.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4679 2022-09-03 21:36:42.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/_forces.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3624 2022-09-03 21:36:42.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/_halfplanes.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3214 2022-08-20 21:41:16.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/_interface.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1620 2022-08-23 21:04:07.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/_mesh_processing.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6716 2022-08-25 19:56:56.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/_rigid_body.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    20269 2022-08-25 19:56:56.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/_tetra_mesh_creation.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    12735 2022-09-03 21:36:42.000000 distance3d-0.7.1/distance3d/hydroelastic_contact/_tetrahedron_intersection.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3229 2022-09-09 08:35:09.000000 distance3d-0.7.1/distance3d/io.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6924 2022-08-04 20:28:00.000000 distance3d-0.7.1/distance3d/mesh.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1910 2022-08-18 21:25:46.000000 distance3d-0.7.1/distance3d/minkowski.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13427 2022-08-19 09:12:04.000000 distance3d-0.7.1/distance3d/mpr.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    12703 2022-09-17 15:58:43.000000 distance3d-0.7.1/distance3d/plotting.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13699 2022-07-12 13:59:15.000000 distance3d-0.7.1/distance3d/random.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2115 2022-07-12 13:59:15.000000 distance3d-0.7.1/distance3d/self_collision.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3792 2022-08-19 09:11:19.000000 distance3d-0.7.1/distance3d/urdf_utils.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9354 2022-08-16 08:16:24.000000 distance3d-0.7.1/distance3d/utils.py
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    10135 2022-09-17 15:52:47.000000 distance3d-0.7.1/distance3d/visualization.py
-drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2022-09-17 16:04:47.499122 distance3d-0.7.1/distance3d.egg-info/
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5262 2022-09-17 16:04:46.000000 distance3d-0.7.1/distance3d.egg-info/PKG-INFO
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1644 2022-09-17 16:04:47.000000 distance3d-0.7.1/distance3d.egg-info/SOURCES.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)        1 2022-09-17 16:04:46.000000 distance3d-0.7.1/distance3d.egg-info/dependency_links.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      129 2022-09-17 16:04:47.000000 distance3d-0.7.1/distance3d.egg-info/requires.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       11 2022-09-17 16:04:47.000000 distance3d-0.7.1/distance3d.egg-info/top_level.txt
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      123 2022-09-17 16:04:47.503122 distance3d-0.7.1/setup.cfg
--rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1281 2022-06-24 14:57:25.000000 distance3d-0.7.1/setup.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-30 15:07:35.466541 distance3d-0.8.0/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2885 2022-07-12 13:59:15.000000 distance3d-0.8.0/LICENSE
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5262 2023-05-30 15:07:35.466541 distance3d-0.8.0/PKG-INFO
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4633 2022-08-16 14:43:07.000000 distance3d-0.8.0/README.md
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-30 15:07:35.466541 distance3d-0.8.0/distance3d/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       82 2023-05-30 15:00:59.000000 distance3d-0.8.0/distance3d/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    16753 2023-05-30 14:57:57.000000 distance3d-0.8.0/distance3d/aabb_tree.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      607 2022-06-17 22:40:17.000000 distance3d-0.8.0/distance3d/benchmark.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8347 2023-04-04 20:34:12.000000 distance3d-0.8.0/distance3d/broad_phase.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    17533 2023-05-26 15:51:11.000000 distance3d-0.8.0/distance3d/colliders.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5288 2023-04-16 14:55:53.000000 distance3d-0.8.0/distance3d/containment.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8078 2022-08-02 13:24:00.000000 distance3d-0.8.0/distance3d/containment_test.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-30 15:07:35.466541 distance3d-0.8.0/distance3d/distance/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6004 2022-08-17 20:23:57.000000 distance3d-0.8.0/distance3d/distance/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6021 2022-06-24 14:57:25.000000 distance3d-0.8.0/distance3d/distance/_box.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13274 2022-08-19 09:42:13.000000 distance3d-0.8.0/distance3d/distance/_circle.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1340 2022-05-29 20:34:55.000000 distance3d-0.8.0/distance3d/distance/_cylinder.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5108 2022-08-19 09:43:05.000000 distance3d-0.8.0/distance3d/distance/_disk.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3414 2022-06-24 14:57:25.000000 distance3d-0.8.0/distance3d/distance/_ellipsoid.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    10909 2022-06-17 22:40:17.000000 distance3d-0.8.0/distance3d/distance/_line.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    17666 2022-06-24 14:57:25.000000 distance3d-0.8.0/distance3d/distance/_line_to_box.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    12752 2022-08-17 20:23:57.000000 distance3d-0.8.0/distance3d/distance/_plane.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    12127 2022-06-17 22:40:17.000000 distance3d-0.8.0/distance3d/distance/_rectangle.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13543 2022-06-17 22:40:17.000000 distance3d-0.8.0/distance3d/distance/_triangle.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7844 2022-06-17 22:40:17.000000 distance3d-0.8.0/distance3d/epa.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    15704 2023-04-16 14:55:53.000000 distance3d-0.8.0/distance3d/geometry.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-30 15:07:35.466541 distance3d-0.8.0/distance3d/gjk/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1150 2023-05-26 15:51:11.000000 distance3d-0.8.0/distance3d/gjk/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    23948 2023-05-26 15:51:11.000000 distance3d-0.8.0/distance3d/gjk/_gjk_jolt.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     8388 2022-07-12 13:59:15.000000 distance3d-0.8.0/distance3d/gjk/_gjk_libccd.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    43115 2023-05-26 15:51:11.000000 distance3d-0.8.0/distance3d/gjk/_gjk_original.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-30 15:07:35.466541 distance3d-0.8.0/distance3d/hydroelastic_contact/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1673 2023-04-04 20:34:12.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      396 2022-08-16 08:16:24.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/_barycentric_transform.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3174 2023-04-04 20:34:12.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/_broad_phase.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5609 2022-09-03 21:36:42.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/_contact_surface.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4850 2022-11-24 19:48:12.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/_forces.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3624 2022-09-03 21:36:42.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/_halfplanes.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3453 2023-04-04 20:34:12.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/_interface.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1620 2022-08-23 21:04:07.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/_mesh_processing.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9026 2023-04-04 20:34:12.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/_rigid_body.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    20269 2022-08-25 19:56:56.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/_tetra_mesh_creation.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13595 2022-11-24 19:48:12.000000 distance3d-0.8.0/distance3d/hydroelastic_contact/_tetrahedron_intersection.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3224 2022-12-30 17:26:30.000000 distance3d-0.8.0/distance3d/io.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6924 2022-08-04 20:28:00.000000 distance3d-0.8.0/distance3d/mesh.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1910 2022-08-18 21:25:46.000000 distance3d-0.8.0/distance3d/minkowski.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13427 2022-08-19 09:12:04.000000 distance3d-0.8.0/distance3d/mpr.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    12837 2022-11-05 16:56:17.000000 distance3d-0.8.0/distance3d/plotting.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    13699 2022-07-12 13:59:15.000000 distance3d-0.8.0/distance3d/random.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2115 2022-10-28 20:00:54.000000 distance3d-0.8.0/distance3d/self_collision.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3792 2022-08-19 09:11:19.000000 distance3d-0.8.0/distance3d/urdf_utils.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9354 2022-08-16 08:16:24.000000 distance3d-0.8.0/distance3d/utils.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    11133 2023-04-04 20:33:55.000000 distance3d-0.8.0/distance3d/visualization.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2023-05-30 15:07:35.466541 distance3d-0.8.0/distance3d.egg-info/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5262 2023-05-30 15:07:35.000000 distance3d-0.8.0/distance3d.egg-info/PKG-INFO
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1668 2023-05-30 15:07:35.000000 distance3d-0.8.0/distance3d.egg-info/SOURCES.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)        1 2023-05-30 15:07:35.000000 distance3d-0.8.0/distance3d.egg-info/dependency_links.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      129 2023-05-30 15:07:35.000000 distance3d-0.8.0/distance3d.egg-info/requires.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       11 2023-05-30 15:07:35.000000 distance3d-0.8.0/distance3d.egg-info/top_level.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      123 2023-05-30 15:07:35.466541 distance3d-0.8.0/setup.cfg
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1281 2022-06-24 14:57:25.000000 distance3d-0.8.0/setup.py
```

### Comparing `distance3d-0.7.1/LICENSE` & `distance3d-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/PKG-INFO` & `distance3d-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distance3d
-Version: 0.7.1
+Version: 0.8.0
 Summary: Distance computation and collision detection in 3D.
 Home-page: https://github.com/AlexanderFabisch/distance3d
 Author: Alexander Fabisch
 Author-email: afabisch@googlemail.com
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: distance3d Version: 0.7.1 Summary: Distance
+Metadata-Version: 2.1 Name: distance3d Version: 0.8.0 Summary: Distance
 computation and collision detection in 3D. Home-page: https://github.com/
 AlexanderFabisch/distance3d Author: Alexander Fabisch Author-email:
 afabisch@googlemail.com License: BSD-3-Clause Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: OS Independent Classifier: Topic :: Scientific/Engineering
 :: Mathematics Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
```

### Comparing `distance3d-0.7.1/README.md` & `distance3d-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/benchmark.py` & `distance3d-0.8.0/distance3d/benchmark.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/colliders.py` & `distance3d-0.8.0/distance3d/colliders.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     support_function_sphere, support_function_cone, support_function_disk,
     support_function_ellipse)
 from .containment import (
     axis_aligned_bounding_box, sphere_aabb, box_aabb, cylinder_aabb,
     capsule_aabb, ellipsoid_aabb, cone_aabb, disk_aabb, ellipse_aabb)
 from .mesh import MeshHillClimbingSupportFunction
 from .utils import plane_basis_from_normal, norm_vector
-from aabbtree import AABB
 
 
 class ConvexCollider(abc.ABC):
     """Convex collider base class.
 
     Parameters
     ----------
@@ -125,15 +124,15 @@
     def center(self):
         return np.mean(self.vertices, axis=0)
 
     def update_pose(self, pose):
         raise NotImplementedError("update_pose is not implemented!")
 
     def aabb(self):
-        return AABB(np.array(axis_aligned_bounding_box(self.vertices)).T)
+        return np.array(axis_aligned_bounding_box(self.vertices)).T
 
 
 class Box(ConvexHullVertices):
     """Box collider.
 
     Parameters
     ----------
@@ -162,15 +161,15 @@
     def update_pose(self, pose):
         self.box2origin = pose
         self.vertices = convert_box_to_vertices(pose, self.size)
         if self.artist_ is not None:
             self.artist_.set_data(pose)
 
     def aabb(self):
-        return AABB(np.array(box_aabb(self.box2origin, self.size)).T)
+        return np.array(box_aabb(self.box2origin, self.size)).T
 
 
 class MeshGraph(ConvexCollider):
     """Mesh collider that uses triangles for hill climbing.
 
     Parameters
     ----------
@@ -213,17 +212,17 @@
     def update_pose(self, mesh2origin):
         self.mesh2origin = mesh2origin
         self._support_function.update_pose(mesh2origin)
         if self.artist_ is not None:
             self.artist_.set_data(mesh2origin)
 
     def aabb(self):
-        return AABB(np.array(axis_aligned_bounding_box(
+        return np.array(axis_aligned_bounding_box(
             self.mesh2origin[np.newaxis, :3, 3] + np.dot(
-                self.vertices, self.mesh2origin[:3, :3].T))).T)
+                self.vertices, self.mesh2origin[:3, :3].T))).T
 
 
 class Sphere(ConvexCollider):
     """Sphere collider.
 
     Parameters
     ----------
@@ -259,15 +258,15 @@
 
     def update_pose(self, pose):
         self.c = pose[:3, 3]
         if self.artist_ is not None:
             self.artist_.set_data(pose)
 
     def aabb(self):
-        return AABB(np.array(sphere_aabb(self.c, self.radius)).T)
+        return np.array(sphere_aabb(self.c, self.radius)).T
 
 
 class Capsule(ConvexCollider):
     """Capsule collider.
 
     Parameters
     ----------
@@ -308,16 +307,16 @@
 
     def update_pose(self, pose):
         self.capsule2origin = pose
         if self.artist_ is not None:
             self.artist_.set_data(pose)
 
     def aabb(self):
-        return AABB(np.array(capsule_aabb(
-            self.capsule2origin, self.radius, self.height)).T)
+        return np.array(capsule_aabb(
+            self.capsule2origin, self.radius, self.height)).T
 
 
 class Ellipsoid(ConvexCollider):
     """Ellipsoid collider.
 
     Parameters
     ----------
@@ -353,16 +352,15 @@
 
     def update_pose(self, pose):
         self.ellipsoid2origin = pose
         if self.artist_ is not None:
             self.artist_.set_data(pose)
 
     def aabb(self):
-        return AABB(
-            np.array(ellipsoid_aabb(self.ellipsoid2origin, self.radii)).T)
+        return np.array(ellipsoid_aabb(self.ellipsoid2origin, self.radii)).T
 
 
 class Cylinder(ConvexCollider):
     """Cylinder collider.
 
     Parameters
     ----------
@@ -403,16 +401,16 @@
 
     def update_pose(self, pose):
         self.cylinder2origin = pose
         if self.artist_ is not None:
             self.artist_.set_data(pose)
 
     def aabb(self):
-        return AABB(np.array(cylinder_aabb(
-            self.cylinder2origin, self.radius, self.length)).T)
+        return np.array(cylinder_aabb(
+            self.cylinder2origin, self.radius, self.length)).T
 
 
 class Disk(ConvexCollider):
     """Disk collider.
 
     Parameters
     ----------
@@ -458,15 +456,15 @@
     def update_pose(self, pose):
         self.c = pose[:3, 3]
         self.normal = pose[:3, 2]
         if self.artist_ is not None:
             self.artist_.set_data(pose)
 
     def aabb(self):
-        return AABB(np.array(disk_aabb(self.c, self.radius, self.normal)).T)
+        return np.array(disk_aabb(self.c, self.radius, self.normal)).T
 
 
 class Ellipse(ConvexCollider):
     """Ellipse collider.
 
     Parameters
     ----------
@@ -505,15 +503,15 @@
     def update_pose(self, pose):
         self.c = pose[:3, 3]
         self.axes = pose[:3, :2].T
         if self.artist_ is not None:
             self.artist_.set_data(pose)
 
     def aabb(self):
-        return AABB(np.array(ellipse_aabb(self.c, self.axes, self.radii)).T)
+        return np.array(ellipse_aabb(self.c, self.axes, self.radii)).T
 
 
 class Cone(ConvexCollider):
     """Cone collider.
 
     Parameters
     ----------
@@ -554,16 +552,15 @@
 
     def update_pose(self, pose):
         self.cone2origin = pose
         if self.artist_ is not None:
             self.artist_.set_data(pose)
 
     def aabb(self):
-        return AABB(np.array(cone_aabb(
-            self.cone2origin, self.radius, self.height)).T)
+        return np.array(cone_aabb(self.cone2origin, self.radius, self.height)).T
 
 
 class Margin(ConvexCollider):
     """Margin around collider.
 
     Parameters
     ----------
@@ -593,17 +590,17 @@
         return self.collider.center()
 
     def update_pose(self, pose):
         self.collider.update_pose(pose)
 
     def aabb(self):
         aabb = self.collider.aabb()
-        mins = aabb.limits[:, 0] - self.margin
-        maxs = aabb.limits[:, 1] + self.margin
-        return AABB(np.array([mins, maxs]).T)
+        mins = aabb[:, 0] - self.margin
+        maxs = aabb[:, 1] + self.margin
+        return np.array([mins, maxs]).T
 
 
 COLLIDERS = {
     "sphere": Sphere,
     "ellipsoid": Ellipsoid,
     "capsule": Capsule,
     "disk": Disk,
```

### Comparing `distance3d-0.7.1/distance3d/containment.py` & `distance3d-0.8.0/distance3d/containment.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/containment_test.py` & `distance3d-0.8.0/distance3d/containment_test.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/__init__.py` & `distance3d-0.8.0/distance3d/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/_box.py` & `distance3d-0.8.0/distance3d/distance/_box.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/_circle.py` & `distance3d-0.8.0/distance3d/distance/_circle.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/_cylinder.py` & `distance3d-0.8.0/distance3d/distance/_cylinder.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/_disk.py` & `distance3d-0.8.0/distance3d/distance/_disk.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/_ellipsoid.py` & `distance3d-0.8.0/distance3d/distance/_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/_line.py` & `distance3d-0.8.0/distance3d/distance/_line.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/_line_to_box.py` & `distance3d-0.8.0/distance3d/distance/_line_to_box.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/_plane.py` & `distance3d-0.8.0/distance3d/distance/_plane.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/_rectangle.py` & `distance3d-0.8.0/distance3d/distance/_rectangle.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/distance/_triangle.py` & `distance3d-0.8.0/distance3d/distance/_triangle.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/epa.py` & `distance3d-0.8.0/distance3d/epa.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/geometry.py` & `distance3d-0.8.0/distance3d/geometry.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/gjk/__init__.py` & `distance3d-0.8.0/distance3d/gjk/__init__.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/gjk/_gjk_jolt.py` & `distance3d-0.8.0/distance3d/gjk/_gjk_jolt.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
             continue
         elif state == GjkState.Clipped:
             return MAX_FLOAT, None, None, None
         else:
             # Get the closest points
             a, b = calculate_closest_points(Y, P, Q, n_points)
 
-            assert abs(np.dot(search_direction, search_direction) - v_len_sq) < EPSILON
+            assert abs(np.dot(search_direction, search_direction) - v_len_sq) < 1e-12
             dist = math.sqrt(v_len_sq)
             if dist < EPSILON:
                 a = b = 0.5 * (a + b)
             return dist, a, b, Y
 
 
 @numba.njit(cache=True)
```

### Comparing `distance3d-0.7.1/distance3d/gjk/_gjk_libccd.py` & `distance3d-0.8.0/distance3d/gjk/_gjk_libccd.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/gjk/_gjk_original.py` & `distance3d-0.8.0/distance3d/gjk/_gjk_original.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/hydroelastic_contact/__init__.py` & `distance3d-0.8.0/distance3d/hydroelastic_contact/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     intersect_halfplanes, plot_halfplanes_and_intersections)
 from ._mesh_processing import (
     center_of_mass_tetrahedral_mesh, tetrahedral_mesh_aabbs,
     tetrahedral_mesh_volumes)
 from ._barycentric_transform import barycentric_transforms
 from ._tetrahedron_intersection import intersect_tetrahedron_pair
 from ._forces import compute_contact_force
-from ._broad_phase import broad_phase_tetrahedra
+from ._broad_phase import HydroelasticBoundingVolumeHierarchy
 
 
 __all__ = [
     "contact_forces", "find_contact_surface", "RigidBody", "ContactSurface",
+    "HydroelasticBoundingVolumeHierarchy",
     # exported for unit tests and specific examples:
     "intersect_halfplanes", "plot_halfplanes_and_intersections",
     "center_of_mass_tetrahedral_mesh", "tetrahedral_mesh_aabbs",
     "tetrahedral_mesh_volumes", "barycentric_transforms",
     "intersect_tetrahedron_pair", "compute_contact_force",
-    "broad_phase_tetrahedra"
 ]
```

### Comparing `distance3d-0.7.1/distance3d/hydroelastic_contact/_contact_surface.py` & `distance3d-0.8.0/distance3d/hydroelastic_contact/_contact_surface.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/hydroelastic_contact/_forces.py` & `distance3d-0.8.0/distance3d/hydroelastic_contact/_forces.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     for intersection_idx, tetrahedron_idx in enumerate(
             contact_surface.intersecting_tetrahedra1):
         coms[intersection_idx], forces[intersection_idx], \
         areas[intersection_idx], triangle = compute_contact_force(
             rigid_body1.tetrahedra_points[tetrahedron_idx],
             tetrahedra_potentials1[tetrahedron_idx],
             contact_surface.contact_planes[intersection_idx],
-            contact_surface.contact_polygons[intersection_idx])
+            contact_surface.contact_polygons[intersection_idx],
+            rigid_body1.youngs_modulus)
 
         triangles.append(triangle)
     return areas, coms, forces, triangles
 
 
 @numba.njit(cache=True)
 def tesselate_ordered_polygon(n_vertices):
@@ -46,15 +47,15 @@
 
 # 8 halfplanes cannot define a polygon with more than 8 vertices
 TRIANGLES = tesselate_ordered_polygon(8)
 
 
 @numba.njit(cache=True)
 def compute_contact_force(
-        tetrahedron, epsilon, contact_plane_hnf, contact_polygon):
+        tetrahedron, epsilon, contact_plane_hnf, contact_polygon, youngs_modulus=1.0):
     """Compute contact force from contact polygon.
 
     Parameters
     ----------
     tetrahedron : array, shape (4, 3)
         Vertices of tetrahedron
 
@@ -64,14 +65,17 @@
     contact_plane_hnf : array, shape (4,)
         Contact plane in Hesse normal form.
 
     contact_polygon : array, shape (n_vertices, 3)
         Contact polygon between two tetrahedra. Points are ordered
         counter-clockwise around their center.
 
+    youngs_modulus : float, optional (default: 1.0)
+        The stiffness of the material.
+
     Returns
     -------
     intersection_com : array, shape (3,)
         Center of the contact polygon.
 
     force_vector : array, shape (3,)
         Force vector of this contact.
@@ -90,15 +94,15 @@
     com = np.empty(4, dtype=np.dtype("float"))
     com[3] = 1.0
     triangles = TRIANGLES[:len(contact_polygon) - 2]
     for triangle in triangles:
         vertices = contact_polygon[triangle]
         com[:3] = (vertices[0] + vertices[1] + vertices[2]) / 3.0
         res = np.linalg.solve(X, com)
-        pressure = np.sum(res * epsilon)
+        pressure = np.sum(res * (epsilon * youngs_modulus))
         area = 0.5 * np.linalg.norm(np.cross(vertices[1] - vertices[0],
                                              vertices[2] - vertices[0]))
         total_force += pressure * area
         total_area += area
         intersection_com += area * com[:3]
 
     if total_area > 0.0:
```

### Comparing `distance3d-0.7.1/distance3d/hydroelastic_contact/_halfplanes.py` & `distance3d-0.8.0/distance3d/hydroelastic_contact/_halfplanes.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/hydroelastic_contact/_interface.py` & `distance3d-0.8.0/distance3d/hydroelastic_contact/_interface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import numpy as np
 from ._forces import contact_surface_forces, accumulate_wrenches
-from ._broad_phase import broad_phase_tetrahedra
 from ._barycentric_transform import barycentric_transforms
 from ._tetrahedron_intersection import intersect_tetrahedron_pairs
 from ._contact_surface import ContactSurface
+from ..aabb_tree import all_aabbs_overlap
 
 
 def contact_forces(rigid_body1, rigid_body2, return_details=False):
     """Contact forces between two objects.
 
     Parameters
     ----------
@@ -46,52 +45,56 @@
             contact_surface.intersection, wrench12_in_world, wrench21_in_world,
             details)
     else:
         return (
             contact_surface.intersection, wrench12_in_world, wrench21_in_world)
 
 
-def find_contact_surface(rigid_body1, rigid_body2):
+def find_contact_surface(rigid_body1, rigid_body2, use_aabb_trees=False):
     """Find contact plane of two rigid bodies.
 
     Note that this function will transform rigid_body1 into the frame of
     rigid_body2.
 
     Parameters
     ----------
     rigid_body1 : RigidBody
         First rigid body.
 
     rigid_body2 : RigidBody
         Second rigid body.
 
+    use_aabb_trees : bool, optional (default: False)
+        Option to specify the usage of aabb_trees.
+
     Returns
     -------
     contact_surface : ContactSurface
         Contact information.
     """
     # We transform vertices of rigid_body1 to rigid_body2 frame to be able to
     # reuse the AABB tree of rigid_body2.
     rigid_body1.express_in(rigid_body2.body2origin_)
 
-    broad_tetrahedra1, broad_tetrahedra2, broad_pairs = broad_phase_tetrahedra(
-        rigid_body1, rigid_body2)
+    if use_aabb_trees:
+        _, broad_tetrahedra1, broad_tetrahedra2, broad_pairs \
+            = rigid_body1.aabbtree_.overlaps_aabb_tree(rigid_body2.aabbtree_)
+    else:
+        broad_tetrahedra1, broad_tetrahedra2, broad_pairs = all_aabbs_overlap(rigid_body1.aabbs, rigid_body2.aabbs)
 
-    unique_indices1 = np.unique(broad_tetrahedra1)
-    unique_indices2 = np.unique(broad_tetrahedra2)
-    X1 = barycentric_transforms(rigid_body1.tetrahedra_points[unique_indices1])
-    X2 = barycentric_transforms(rigid_body2.tetrahedra_points[unique_indices2])
-    X1 = {j: X1[i] for i, j in enumerate(unique_indices1)}
-    X2 = {j: X2[i] for i, j in enumerate(unique_indices2)}
+    X1 = barycentric_transforms(rigid_body1.tetrahedra_points[broad_tetrahedra1])
+    X2 = barycentric_transforms(rigid_body2.tetrahedra_points[broad_tetrahedra2])
+    X1 = {j: X1[i] for i, j in enumerate(broad_tetrahedra1)}
+    X2 = {j: X2[i] for i, j in enumerate(broad_tetrahedra2)}
 
     intersection_result = intersect_tetrahedron_pairs(
         broad_pairs,
         rigid_body1.tetrahedra_points, rigid_body2.tetrahedra_points,
         rigid_body1.tetrahedra_potentials, rigid_body2.tetrahedra_potentials,
-        X1, X2)
+        X1, X2, rigid_body1.youngs_modulus, rigid_body2.youngs_modulus)
     contact_surface = ContactSurface(
         rigid_body2.body2origin_, *intersection_result)
 
     areas, coms, forces, triangles = contact_surface_forces(
         contact_surface, rigid_body1)
     contact_surface.add_polygon_info(areas, coms, forces, triangles)
```

### Comparing `distance3d-0.7.1/distance3d/hydroelastic_contact/_mesh_processing.py` & `distance3d-0.8.0/distance3d/hydroelastic_contact/_mesh_processing.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/hydroelastic_contact/_rigid_body.py` & `distance3d-0.8.0/distance3d/hydroelastic_contact/_rigid_body.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 from ..utils import transform_points, invert_transform
 from ._tetra_mesh_creation import (
     make_tetrahedral_sphere, make_tetrahedral_ellipsoid,
     make_tetrahedral_cube, make_tetrahedral_box, make_tetrahedral_cylinder,
     make_tetrahedral_capsule)
-from ._mesh_processing import center_of_mass_tetrahedral_mesh
+from ._mesh_processing import center_of_mass_tetrahedral_mesh, tetrahedral_mesh_aabbs
+from ..aabb_tree import AabbTree
+from ..visualization import RigidBodyTetrahedralMesh
 
 
 class RigidBody:
     """Rigid body represented by tetrahedral mesh.
 
     Parameters
     ----------
@@ -19,24 +21,34 @@
         Vertices of the mesh.
 
     tetrahedra : array, shape (n_tetrahedra, 4)
         Indices of vertices that form tetrahedra of the mesh.
 
     potentials : array, shape (n_vertices,)
         Potential of each vertex. Shortest distance to surface.
+
+    youngs_modulus : float, optional (default: 1.0)
+        The stiffness of the material the rigidbody is made out of.
     """
-    def __init__(self, body2origin, vertices, tetrahedra, potentials):
+    def __init__(self, body2origin, vertices, tetrahedra, potentials,
+                 youngs_modulus=1.0):
         self.body2origin_ = body2origin
         self.vertices_ = vertices
         self.tetrahedra_ = tetrahedra
         self.potentials_ = potentials
 
         self._tetrahedra_points = None
         self._com = None
 
+        self._aabbs = None
+        self._aabb_tree = None
+
+        self._youngs_modulus = youngs_modulus
+        self._artist = None
+
     @staticmethod
     def make_sphere(center, radius, order=4):
         """Create sphere.
 
         Parameters
         ----------
         center : array, shape (3,)
@@ -217,7 +229,68 @@
         origin2new_body = invert_transform(new_body2origin)
         body2new_body = np.dot(origin2new_body, self.body2origin_)
         self.vertices_ = transform_points(body2new_body, self.vertices_)
         self.body2origin_ = np.copy(new_body2origin)
 
         self._tetrahedra_points = None
         self._com = None
+        self._aabbs = None
+        self._aabb_tree = None
+
+    def update_pose(self, body2origin):
+        """Set new pose.
+
+        Parameters
+        ----------
+        body2origin : array, shape (4, 4)
+            New pose.
+        """
+        # TODO Check if this is correct.
+        self.body2origin_ = body2origin
+        if self.artist_ is not None:
+            self.artist_.set_data(body2origin, vertices=self.vertices_, tetrahedra=self.tetrahedra_)
+
+    def aabb(self):
+        """The aabb of the rigidbody"""
+        return self.aabb_tree.get_root_aabb()
+
+    @property
+    def aabbs(self):
+        """The aabbs for broad phase collision detection"""
+        if self._aabbs is None:
+            self._aabbs = tetrahedral_mesh_aabbs(self.tetrahedra_points)
+        return self._aabbs
+
+    @property
+    def aabb_tree(self):
+        """The aabb_tree for broad phase collision detection"""
+        if self._aabb_tree is None:
+            self._aabb_tree = AabbTree()
+            self._aabb_tree.insert_aabbs(self.aabbs, pre_insertion_methode="sort")
+        return self._aabb_tree
+
+    @property
+    def youngs_modulus(self):
+        """Get the young's modulus of the Object. (stiffness)"""
+        return self._youngs_modulus
+
+    @youngs_modulus.setter
+    def youngs_modulus(self, value):
+        """Set the young's modulus of the Object. (stiffness)"""
+        self._youngs_modulus = value
+
+    @property
+    def artist_(self):
+        """The artist to visualize the rigid body as a wireframe."""
+        if self._artist is None:
+            self.make_artist()
+        return self._artist
+
+    def make_artist(self, c=None):
+        """Creates a new artist.
+
+            Parameters
+            ----------
+            c : array, shape (3
+                The color of the wireframe.
+        """
+        self._artist = RigidBodyTetrahedralMesh(self.body2origin_, self.vertices_, self.tetrahedra_, c)
```

### Comparing `distance3d-0.7.1/distance3d/hydroelastic_contact/_tetra_mesh_creation.py` & `distance3d-0.8.0/distance3d/hydroelastic_contact/_tetra_mesh_creation.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/hydroelastic_contact/_tetrahedron_intersection.py` & `distance3d-0.8.0/distance3d/hydroelastic_contact/_tetrahedron_intersection.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 from ..utils import plane_basis_from_normal, EPSILON
 from ._halfplanes import intersect_halfplanes
 
 
 def intersect_tetrahedron_pairs(
         pairs, tetrahedra_points1, tetrahedra_points2,
-        epsilon1, epsilon2, X1, X2):
+        epsilon1, epsilon2, X1, X2, youngs_modulus1=1.0, youngs_modulus2=1.0):
     """Intersect pairs of tetrahedra.
 
     Parameters
     ----------
     pairs : list
         List of index pairs.
 
@@ -28,14 +28,20 @@
 
     X1 : dict
         Maps tetrahedron indices of first rigid body to barycentric transform.
 
     X2 : dict
         Maps tetrahedron indices of second rigid body to barycentric transform.
 
+    youngs_modulus1 : float, optional (default: 1.0)
+        Young's modulus of the first rigid body
+
+    youngs_modulus2 : float, optional (default: 1.0)
+        Young's modulus of the second rigid body
+
     Returns
     -------
     intersection : bool
         Do both rigid bodies overlap?
 
     contact_planes : array, shape (n_intersections, 4)
         Contact planes of intersection pairs in Hesse normal form.
@@ -53,15 +59,16 @@
     contact_planes = []
     contact_polygons = []
     intersecting_tetrahedra1 = []
     intersecting_tetrahedra2 = []
     for i, j in pairs:
         intersecting, contact_details = intersect_tetrahedron_pair(
             tetrahedra_points1[i], epsilon1[i], X1[i],
-            tetrahedra_points2[j], epsilon2[j], X2[j])
+            tetrahedra_points2[j], epsilon2[j], X2[j],
+            youngs_modulus1, youngs_modulus2)
         if intersecting:
             intersection = True
         else:
             continue
 
         contact_plane_hnf, contact_polygon = contact_details
 
@@ -73,15 +80,16 @@
         contact_planes = np.vstack(contact_planes)
     return (intersection, contact_planes, contact_polygons,
             intersecting_tetrahedra1, intersecting_tetrahedra2)
 
 
 @numba.njit(cache=True)
 def intersect_tetrahedron_pair(tetrahedron1, epsilon1, X1,
-                               tetrahedron2, epsilon2, X2):
+                               tetrahedron2, epsilon2, X2,
+                               youngs_modulus1=1.0, youngs_modulus2=1.0):
     """Intersect a pair of tetrahedra.
 
     Parameters
     ----------
     tetrahedron1 : array, shape (4, 3)
         Vertices of tetrahedron 1.
 
@@ -96,24 +104,30 @@
 
     epsilon2 : array, shape (4,)
         Potentials of the vertices of tetrahedron 2.
 
     X2 : array, shape (4, 4)
         Each row is a halfspace that defines the original tetrahedron.
 
+    youngs_modulus1 : float, optional (default: 1.0)
+        Young's modulus of tetrahedron 1
+
+    youngs_modulus2 : float, optional (default: 1.0)
+        Young's modulus of tetrahedron 2
+
     Returns
     -------
     intersection : bool
         Do both tetrahedra intersect?
 
     contact_info : tuple
         Contact plane in Hesse normal form, contact polygon and triangles of
         contact polygon.
     """
-    contact_plane_hnf, same = contact_plane(X1, X2, epsilon1, epsilon2)
+    contact_plane_hnf, same = contact_plane(X1, X2, epsilon1, epsilon2, youngs_modulus1, youngs_modulus2)
     if same:
         return True, _handle_same_tetrahedron(epsilon2, tetrahedron2)
 
     plane_normal = contact_plane_hnf[:3]
     d = contact_plane_hnf[3]
     if not check_tetrahedra_intersect_contact_plane(
             tetrahedron1, tetrahedron2, plane_normal, d, tolerance=1e-6):
@@ -144,18 +158,19 @@
         plane_normal[0], plane_normal[1], plane_normal[2], d])
     contact_polygon = np.vstack((plane_point, plane_point, plane_point))
     return contact_plane_hnf, contact_polygon
 
 
 @numba.njit(
     numba.types.Tuple((numba.float64[::1], numba.bool_))(
-        numba.float64[:, ::1], numba.float64[:, ::1], numba.float64[::1],
-        numba.float64[::1]),
+        numba.float64[:, ::1], numba.float64[:, ::1],
+        numba.float64[::1], numba.float64[::1],
+        numba.float64, numba.float64),
     cache=True)
-def contact_plane(X1, X2, epsilon1, epsilon2):
+def contact_plane(X1, X2, epsilon1, epsilon2, youngs_modulus1, youngs_modulus2):
     """Compute contact plane.
 
     Parameters
     ----------
     X1 : array, shape (4, 4)
         Each row is a halfspace that defines the original tetrahedron.
 
@@ -164,25 +179,30 @@
 
     epsilon1 : array, shape (4,)
         Potentials of the vertices of tetrahedron 1.
 
     epsilon2 : array, shape (4,)
         Potentials of the vertices of tetrahedron 2.
 
+    youngs_modulus1 : float, optional (default: 1.0)
+        Young's modulus of tetrahedron 1
+
+    youngs_modulus2 : float, optional (default: 1.0)
+        Young's modulus of tetrahedron 2
+
     Returns
     -------
     plane_hnf : array, shape (4,)
         Contact plane in Hesse normal form: plane normal and distance to origin
         along plane normal.
 
     same : bool
         Are both tetrahedrons actually the same tetrahedron (maybe scaled)?
     """
-    # TODO Young's modulus, see Eq. 16 of paper
-    plane_hnf = epsilon1.dot(X1) - epsilon2.dot(X2)
+    plane_hnf = (epsilon1 * youngs_modulus1).dot(X1) - (epsilon2 * youngs_modulus2).dot(X2)
     norm = np.linalg.norm(plane_hnf[:3])
 
     if norm == 0.0:
         return plane_hnf, True
 
     plane_hnf /= norm
     # NOTE in order to obtain proper Hesse normal form of the contact plane
@@ -226,18 +246,18 @@
     -------
     intersection : bool
         Do both tetrahedra intersect the contact plane.
     """
     plane_distances1 = tetrahedron1.dot(plane_normal) - d
     plane_distances2 = tetrahedron2.dot(plane_normal) - d
     return (
-        min(plane_distances1) < -tolerance
-        and max(plane_distances1) > tolerance
-        and min(plane_distances2) < -tolerance
-        and max(plane_distances2) > tolerance)
+            min(plane_distances1) < -tolerance
+            and max(plane_distances1) > tolerance
+            and min(plane_distances2) < -tolerance
+            and max(plane_distances2) > tolerance)
 
 
 @numba.njit(
     numba.float64[:, ::1](numba.float64[:, ::1], numba.float64[::1],
                           numba.float64[:, ::1]),
     cache=True)
 def make_halfplanes(X, plane_point, cart2plane):
```

### Comparing `distance3d-0.7.1/distance3d/io.py` & `distance3d-0.8.0/distance3d/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     tetrahedra : array, shape (n_tetrahedra, 4)
         Indices of vertices that form tetrahedra of the mesh.
     """
     assert filename.endswith(".vtk")
 
     with open(filename, "r") as f:
         content = f.read()
-    lines = content.split(os.linesep)
+    lines = content.splitlines()
     lines = [line.strip() for line in lines]
 
     point_lines = None
     cells_lines = None
     for i, line in enumerate(lines):
         if line.startswith("POINTS"):
             n_points = int(line.split(" ")[1])
```

### Comparing `distance3d-0.7.1/distance3d/mesh.py` & `distance3d-0.8.0/distance3d/mesh.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/minkowski.py` & `distance3d-0.8.0/distance3d/minkowski.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/mpr.py` & `distance3d-0.8.0/distance3d/mpr.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/plotting.py` & `distance3d-0.8.0/distance3d/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Plotting functions for geometric shapes."""
 from collections import deque
 import numpy as np
 from mpl_toolkits import mplot3d
 import pytransform3d.plot_utils as ppu
 import pytransform3d.rotations as pr
 import pytransform3d.transformations as pt
+
+from .aabb_tree import TYPE_INDEX, TYPE_LEAF, TYPE_BRANCH
 from .utils import plane_basis_from_normal
 
 
 def plot_line(ax, line_point, line_direction, length=10):
     """Plot line.
 
     Parameters
@@ -338,31 +340,34 @@
     """Plot tree of axis-aligned bounding boxes.
 
     Parameters
     ----------
     ax : Matplotlib 3d axis
         A matplotlib 3d axis.
 
-    tree : aabbtree.AABBTree
+    tree : AabbTree
         Tree of axis-aligned bounding boxes.
 
     alpha : float, optional (default: 0.5)
         Alpha value of edges.
 
     color : str
         Color of edges.
     """
-    nodes = deque()
-    nodes.append(tree)
-    while nodes:
-        node = nodes.popleft()
-        mins, maxs = np.array(node.aabb.limits).T
-        plot_aabb(ax, mins, maxs, alpha=alpha, color=color)
-        if not node.is_leaf:
-            nodes.extend([node.left, node.right])
+    stack = [tree.root]
+
+    while len(stack) != 0:
+
+        node_index = stack[-1]
+        stack = stack[:-1]
+
+        plot_aabb(ax, tree.aabbs[node_index, :, 0], tree.aabbs[node_index, :, 1], alpha=alpha, color=color)
+
+        if tree.nodes[node_index, TYPE_INDEX] == TYPE_BRANCH:
+            stack.extend([tree.nodes[node_index, 1], tree.nodes[node_index, 2]])
 
 
 def plot_plane(
         ax, plane_point, plane_normal, s=1.0, surface_alpha=0.1, color="b"):
     """Plot rectangle.
 
     Parameters
```

### Comparing `distance3d-0.7.1/distance3d/random.py` & `distance3d-0.8.0/distance3d/random.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/self_collision.py` & `distance3d-0.8.0/distance3d/self_collision.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/urdf_utils.py` & `distance3d-0.8.0/distance3d/urdf_utils.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/utils.py` & `distance3d-0.8.0/distance3d/utils.py`

 * *Files identical despite different names*

### Comparing `distance3d-0.7.1/distance3d/visualization.py` & `distance3d-0.8.0/distance3d/visualization.py`

 * *Files 3% similar despite different names*

```diff
@@ -286,40 +286,76 @@
         Pose of the mesh.
 
     vertices : array, shape (n_vertices, 3)
         Vertices of the mesh.
 
     tetrahedra : array, shape (n_tetrahedra, 4)
         Indices of vertices that form tetrahedra of the mesh.
+
+    c : array-like, shape (3,), optional (default: None)
+        Color(s)
     """
-    def __init__(self, body2origin, vertices, tetrahedra):
+    def __init__(self, body2origin, vertices, tetrahedra, c=None):
         self.mesh = o3d.geometry.TetraMesh()
-        self.set_data(body2origin, vertices, tetrahedra)
+        self.set_data(body2origin, vertices, tetrahedra, c)
 
-    def set_data(self, body2origin, vertices, tetrahedra):
+    def set_data(self, body2origin, vertices, tetrahedra, c=None):
         """Update rigid body.
 
         Parameters
         ----------
         body2origin : array, shape (4, 4)
             Pose of the mesh.
 
         vertices : array, shape (n_vertices, 3)
             Vertices of the mesh.
 
         tetrahedra : array, shape (n_tetrahedra, 4)
             Indices of vertices that form tetrahedra of the mesh.
+
+        c : array-like, shape (3,), optional (default: None)
+            Color(s)
         """
         self.mesh.vertices = o3d.utility.Vector3dVector(vertices)
         self.mesh.tetras = o3d.utility.Vector4iVector(tetrahedra)
         self.mesh.transform(body2origin)
+        if c is not None:
+            self.mesh.paint_uniform_color(c)
 
     @property
     def geometries(self):
         """Expose geometries.
 
         Returns
         -------
         geometries : list
             List of geometries that can be added to the visualizer.
         """
         return [self.mesh]
+
+
+class ColoredVertices(pv.Artist):  # pragma: no cover
+    """Vertices of a mesh without connections with color information.
+
+    Parameters
+    ----------
+    vertices : array, shape (n_vertices, 3)
+        Vertices of the mesh.
+
+    colors : array-like, shape (n_vertices, 3)
+        Colors
+    """
+    def __init__(self, vertices, colors):
+        self.vertices = o3d.geometry.PointCloud(
+            o3d.utility.Vector3dVector(vertices))
+        self.vertices.colors = o3d.utility.Vector3dVector(colors)
+
+    @property
+    def geometries(self):
+        """Expose geometries.
+
+        Returns
+        -------
+        geometries : list
+            List of geometries that can be added to the visualizer.
+        """
+        return [self.vertices]
```

### Comparing `distance3d-0.7.1/distance3d.egg-info/PKG-INFO` & `distance3d-0.8.0/distance3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distance3d
-Version: 0.7.1
+Version: 0.8.0
 Summary: Distance computation and collision detection in 3D.
 Home-page: https://github.com/AlexanderFabisch/distance3d
 Author: Alexander Fabisch
 Author-email: afabisch@googlemail.com
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: distance3d Version: 0.7.1 Summary: Distance
+Metadata-Version: 2.1 Name: distance3d Version: 0.8.0 Summary: Distance
 computation and collision detection in 3D. Home-page: https://github.com/
 AlexanderFabisch/distance3d Author: Alexander Fabisch Author-email:
 afabisch@googlemail.com License: BSD-3-Clause Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: OS Independent Classifier: Topic :: Scientific/Engineering
 :: Mathematics Classifier: Topic :: Scientific/Engineering :: Visualization
 Description-Content-Type: text/markdown Provides-Extra: test Provides-Extra:
```

### Comparing `distance3d-0.7.1/distance3d.egg-info/SOURCES.txt` & `distance3d-0.8.0/distance3d.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 distance3d/__init__.py
+distance3d/aabb_tree.py
 distance3d/benchmark.py
 distance3d/broad_phase.py
 distance3d/colliders.py
 distance3d/containment.py
 distance3d/containment_test.py
 distance3d/epa.py
 distance3d/geometry.py
```

### Comparing `distance3d-0.7.1/setup.py` & `distance3d-0.8.0/setup.py`

 * *Files identical despite different names*

