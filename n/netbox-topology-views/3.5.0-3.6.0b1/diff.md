# Comparing `tmp/netbox-topology-views-3.5.0.tar.gz` & `tmp/netbox-topology-views-3.6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-topology-views-3.5.0.tar", last modified: Sun Apr 30 18:15:10 2023, max compression
+gzip compressed data, was "netbox-topology-views-3.6.0b1.tar", last modified: Tue May 30 14:58:04 2023, max compression
```

## Comparing `netbox-topology-views-3.5.0.tar` & `netbox-topology-views-3.6.0b1.tar`

### file list

```diff
@@ -1,100 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.746385 netbox-topology-views-3.5.0/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.746385 netbox-topology-views-3.5.0/netbox_topology_views/api/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.746385 netbox-topology-views-3.5.0/netbox_topology_views/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/migrations/0002_individualoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.742385 netbox-topology-views-3.5.0/netbox_topology_views/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.742385 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.746385 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/css/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/css/app.css
--rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/css/vendor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/
--rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/backup.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/camera.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/database.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/modem.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/phone.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/printer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/router.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/siem.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/storage.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/ups.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/
--rw-r--r--   0 runner    (1001) docker     (123)   349737 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/images.js
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/images.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.742385 netbox-topology-views-3.5.0/netbox_topology_views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/images.html
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/individual_options.html
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/site_button.html
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/toasts.html
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31247 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/netbox_topology_views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:15:10.746385 netbox-topology-views-3.5.0/netbox_topology_views.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-04-30 18:15:10.000000 netbox-topology-views-3.5.0/netbox_topology_views.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-30 18:15:10.000000 netbox-topology-views-3.5.0/netbox_topology_views.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:15:10.000000 netbox-topology-views-3.5.0/netbox_topology_views.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-30 18:15:10.000000 netbox-topology-views-3.5.0/netbox_topology_views.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 18:15:10.754385 netbox-topology-views-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-30 18:14:59.000000 netbox-topology-views-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.392943 netbox-topology-views-3.6.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-30 14:58:04.392943 netbox-topology-views-3.6.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.380943 netbox-topology-views-3.6.0b1/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.384943 netbox-topology-views-3.6.0b1/netbox_topology_views/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.384943 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0002_individualoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0005_individualoptions_save_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.380943 netbox-topology-views-3.6.0b1/netbox_topology_views/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.380943 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.384943 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/css/vendor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.388943 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/backup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/database.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/modem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/printer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/router.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/siem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/storage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/ups.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.388943 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   350175 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/images.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/images.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.380943 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.392943 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinate.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinate_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinate_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinate_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/images.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/individual_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/location_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/site_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/toasts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36634 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.380943 netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-30 14:58:04.000000 netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-30 14:58:04.000000 netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:58:04.000000 netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 14:58:04.000000 netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:58:04.392943 netbox-topology-views-3.6.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/setup.py
```

### Comparing `netbox-topology-views-3.5.0/LICENSE` & `netbox-topology-views-3.6.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/PKG-INFO` & `netbox-topology-views-3.6.0b1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.5.0
+Version: 3.6.0b1
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
@@ -13,26 +13,30 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Netbox Topology Views Plugin
 
 ![Version](https://img.shields.io/pypi/v/netbox-topology-views) ![Downloads](https://img.shields.io/pypi/dm/netbox-topology-views)
 
-Create topology views/maps from your devices in netbox.
-The connections are based on the cables you created in netbox.
-Support to filter on name, site, tag and device role.
+Create topology views/maps from your devices in NetBox.
+The connections are based on the cables you created in NetBox.
+Support to filter on name, site, tag and device role.  
+Options to export to xml (for draw.io/diagrams.net) or png.
 
 ## Preview
 
-![preview image](doc/img/preview_3.1.jpeg?raw=true "preview")
+![Topology with light mode](doc/img/topology_light.png)
+![Topology with dark mode](doc/img/topology_dark.png)
 
 ## Install
 
 **_NOTE:_** For docker please see: [Docker install](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins)
 
+**_NOTE:_** Add `RUN mkdir -p /opt/netbox/netbox/static/netbox_topology_views/img` to the Dockerfile-Plugins file to create the image folder
+
 The plugin is available as a Python package and can be installed with pip.
 
 Run `pip install netbox-topology-views` in your virtual env.
 
 To ensure NetBox Topology Views plugin is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the NetBox root directory (alongside `requirements.txt`) and list the `netbox-topology-views` package:
 
 ```no-highlight
@@ -66,29 +70,32 @@
 | >= 3.3.0       | >= v3.0.0                     |
 | >= 3.2.0       | >= v1.1.0                     |
 | >= 3.1.8       | >= v1.0.0                     |
 | >= 2.11.1      | >= v0.5.3                     |
 | >= 2.10.0      | >= v0.5.0                     |
 | < 2.10.0       | =< v0.4.10                    |
 
-### Custom field: coordinates
+### Update
 
-There is also support for custom fields.
+Run `pip install netbox-topology-views --upgrade` in your venv.
 
-If you create a custom field "coordinates" for "dcim > device" and "Circuits > circuit" with type "text" and name "coordinates" you will see the same layout every time. It is recommended to set this field to "UI visibility" "Hidden" and let the plugin manage it in the background.
+Run `python3 manage.py migrate netbox_topology_views`
 
-The coordinates are stored as: "X;Y".
+Run `python3 manage.py collectstatic --no-input`
 
-Please read the "Configure" chapter to set the `allow_coordinates_saving` option to True.
-You might also set the `always_save_coordinates` option to True.
+Clear you browser cache.
 
 ## Configure
 
+### Individual Options
+
 All individual options can be assigned a default value per user directly in the plugin. The default value can be overridden on the filter page.
 
+![Individual Options](doc/img/topology_individual_options.png)
+
 The remaining options must be configured in the `PLUGINS_CONFIG` section of your `netbox/configuration.py`.
 
 Example:
 ```
 PLUGINS_CONFIG = {
     'netbox_topology_views': {
         'static_image_directory': 'netbox_topology_views/img',
@@ -97,73 +104,113 @@
     }
 }
 ```
 
 | Setting                  | Default value                                                                                                                                  | Description                                                                                                            |
 | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
 | static_image_directory   | netbox_topology_views/img                                                                                                                      | (str or pathlib.Path) Specifies the location that images will be loaded from by default. Must be within `STATIC_ROOT`  |
-| allow_coordinates_saving | False                                                                                                                                          | (bool) Set to true if you use the custom coordinates fields and want to save the coordinates                           |
-| always_save_coordinates  | False                                                                                                                                          | (bool) Set if you want to enable the option to save coordinates by default                                             |
+| allow_coordinates_saving | False                                                                                                                                          | (bool) Set to true if you want to enable the ability to save the coordinates.                           |
+| always_save_coordinates  | False                                                                                                                                          | (bool) Set if you want to enable the option to save coordinates by default. Setting allow_coordinates_saving to true is mandatory.                                             |
+
+### Custom field: coordinates
+
+There is also support for custom fields.
+
+>**_Note:_** The custom field "coordinates" is deprecated and will be removed in the future. Please use Coordinate Groups instead.
+
+If you create a custom field "coordinates" for "dcim > device" and "Circuits > circuit" with type "text" and name "coordinates" you will see the same layout every time. It is recommended to set this field to "UI visibility" "Hidden" and let the plugin manage it in the background.
+
+The coordinates are stored as: "X;Y".
+
+> Please read the "Configure" chapter to set the `allow_coordinates_saving` option to True.
+You might also set the `always_save_coordinates` option to True.
+
+### Convert custom field to Coordinate Groups
+
+Please note that values stored in the custom field "coordinates" are not being converted to Coordinate Groups automatically. A pragmatic way to do this conversion yourself is as follows:
++ Navigate to "Topology" > "Filters".
++ Select "Show Unconnected" and "Show Cables". 
++ Leave all other filter settings alone. We want all entries to be displayed!
++ Click "Search" and wait for the results to be displayed
++ Select all nodes. This can be done by holding down the Shift key and dragging a frame around all icons with the left mouse button.
++ Drag the selection a tiny bit to the side. This causes all coordinates for all devices to be stored in the "default" group.
+> **_Hint_**: Don't wait too long after clicking an icon in order to drag. If you hold the mouse button for too long before dragging starts, the selection is reset._
++ Storing the values might take some time, depending on the number of devices. Please be patient and check "Coordinates" in order to make sure that everthing has been stored.
++ It is save to delete the custom field now.
 
 ### Custom Images
 
-To change image with associated device use the `Images` page - it allows to map a device role with an image found in the netbox static directory (defined by the plugin config `static_image_directory` which defaults to `netbox_topology_views/img`). You can also upload you own custom images to there - these images will automatically be used for a device (if it does not already have a specified image in the settings) if their name is the device role slug.
+To change image with associated device use the `Images` page - it allows to map a device role with an image found in the NetBox static directory (defined by the plugin config `static_image_directory` which defaults to `netbox_topology_views/img`). You can also upload you own custom images to there - these images will automatically be used for a device (if it does not already have a specified image in the settings) if their name is the device role slug.
+
+![Images](doc/img/topology_images.png)
 
 ## Use
 
 Go to the plugins tab in the navbar and click topology or go to `$NETBOX_URL/plugins/netbox_topology_views/` to view your topologies
 
 Select your options for the topology view:
 
-![topology_options](https://user-images.githubusercontent.com/20901110/235302073-234c3ef7-2c2b-4d0c-a674-9909d490d7ea.png)
+![Filter Options](doc/img/topology_filter_options.png)
 
 <dl>
+    <dt>Coordinate Group</dt>
+    <dd>Select Coordinate Group. These groups allow devices to be displayed in different positions depending on the group, thus providing different representations for the same topology. If nothing is selected, the group "default" is set automatically.</dd>
     <dt>Save Coordinates</dt>
     <dd>Save the coordinates of devices in the topology view.</dd>
     <dt>Show Unconnected</dt>
     <dd>Show devices that have no connections or for which no connection is displayed. This option depends on other parameters like 'Show Cables' and 'Show Logical Connections'.</dd>
     <dt>Show Cables</dt>
     <dd>Show connections between interfaces, front / rear ports, etc., that are connected with one or more cables. These connections are displayed as solid lines in the color of the cable.</dd> 
     <dt>Show Logical Connections</dt>
     <dd>Show logical connections between interfaces (referred to as Interface Connections in NetBox) in the topology view. Where the path between
         interfaces includes multiple cables (e.g., via patch panels), only the end interface connections are shown, not the 
         intermediate front / rear port connections, etc. This is similar to what was referred to as 'end-to-end' connections in previous versions. These connections are displayed as yellow dotted lines.</dd>
-    <dt>Show redundant Cable and Locigal Connection</dt>
+    <dt>Show redundant Cable and Logical Connection</dt>
     <dd>Shows a logical connection (in addition to a cable), even if a cable is directly connected. Leaving this option disabled prevents that redundant display. This option only has an effect if 'Show Logical Connections' is activated.</dd>
     <dt>Show Neighbors</dt>
     <dd>Adds neighbors to the filter result set automatically. Link peers will be added if 'Show Cables' is ticked, far-end terminations will be added if 'Show Logical Connections' is ticked.</dd>
     <dt>Show Circuit Terminations</dt>
     <dd>Show connections which end at a circuit termination in the topology view. These connections are displayed as blue dashed lines.</dd>
     <dt>Show Power Feeds</dt>
     <dd>Displays connections between power outlets and power ports. These connections are displayed as solid lines in the color of the cable. This option depends on 'Show Cables'.</dd>
     <dt>Show Wireless Links</dt>
     <dd>Displays wireless connections. These connections are displayed as blue dotted lines.</dd>
 </dl>
     
-### Update
+### Coordinates and Coordinate Groups
 
-Run `pip install netbox-topology-views --upgrade` in your venv.
+Netbox Topology Views stores the position of the devices. In order to allow different representations for the topology, Coordinate Groups are supported.
 
-Run `python3 manage.py migrate netbox_topology_views`
+> Please read the "Configure" chapter to set the `allow_coordinates_saving` option to True.
+You might also set the `always_save_coordinates` option to True.
 
-Run `python3 manage.py collectstatic --no-input`
+Navigate to "Coordinate Groups" in the menu and create as many groups as you like. You can select a group later in the filter pane in order to show icon positions according to this group (see chapter "Use"). You can also omit creating a group if you don't need this feature. Netbox Topology Views automatically creates a group named "default" for you and stores all coordinates in this group, even if you do not select a group in the filter.
 
+By default, the position of the devices are calculated with a physics engine. As soon as a device icon is dragged to another location, its position is saved and excluded from the calculation by the physics engine. All saved coordinates can be viewed and edited under the menu item "Coordinates".
 
-Clear you browser cache.
-
+> **_Note:_** At the time of writing, it is not possible to store the positions of circuit terminations, power panels and power feeds, as these are not devices.
 
 ### Permissions
 
 To view `/plugins/netbox_topology-views/topology` you need the following permissions:
  + dcim | device | can view device
  + dcim | site | can view site
  + extras | tag | can view tag
  + dcim | device role | can view device role
 
-To view `/plugins/netbox_topology-views/image`:
+To save `Coordinates` when moving icons:
+ + netbox_topology_views | coordinate | change
+
+To view `/plugins/netbox_topology-views/images`:
  + dcim | site | view
  + dcim | device role | view
  + dcim | device role | add
  + dcim | device role | change
 
- To view `/plugins/netbox_topology-views/individualoptions`:
- + netbox topology views | individualoptions | change
+To view `/plugins/netbox_topology-views/individualoptions`:
+ + netbox_topology_views | individual options | change
+
+Set `Coordinate Groups` according to your needs:
+ + netbox_topology_views | coordinate groups | view/add/change/delete
+
+Set `Coordinates` according to your needs:
+ + netbox_topology_views | coordinate | view/add/change/delete
```

### Comparing `netbox-topology-views-3.5.0/README.md` & `netbox-topology-views-3.6.0b1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Netbox Topology Views Plugin
 
 ![Version](https://img.shields.io/pypi/v/netbox-topology-views) ![Downloads](https://img.shields.io/pypi/dm/netbox-topology-views)
 
-Create topology views/maps from your devices in netbox.
-The connections are based on the cables you created in netbox.
-Support to filter on name, site, tag and device role.
+Create topology views/maps from your devices in NetBox.
+The connections are based on the cables you created in NetBox.
+Support to filter on name, site, tag and device role.  
+Options to export to xml (for draw.io/diagrams.net) or png.
 
 ## Preview
 
-![preview image](doc/img/preview_3.1.jpeg?raw=true "preview")
+![Topology with light mode](doc/img/topology_light.png)
+![Topology with dark mode](doc/img/topology_dark.png)
 
 ## Install
 
 **_NOTE:_** For docker please see: [Docker install](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins)
 
+**_NOTE:_** Add `RUN mkdir -p /opt/netbox/netbox/static/netbox_topology_views/img` to the Dockerfile-Plugins file to create the image folder
+
 The plugin is available as a Python package and can be installed with pip.
 
 Run `pip install netbox-topology-views` in your virtual env.
 
 To ensure NetBox Topology Views plugin is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the NetBox root directory (alongside `requirements.txt`) and list the `netbox-topology-views` package:
 
 ```no-highlight
@@ -51,29 +55,32 @@
 | >= 3.3.0       | >= v3.0.0                     |
 | >= 3.2.0       | >= v1.1.0                     |
 | >= 3.1.8       | >= v1.0.0                     |
 | >= 2.11.1      | >= v0.5.3                     |
 | >= 2.10.0      | >= v0.5.0                     |
 | < 2.10.0       | =< v0.4.10                    |
 
-### Custom field: coordinates
+### Update
 
-There is also support for custom fields.
+Run `pip install netbox-topology-views --upgrade` in your venv.
 
-If you create a custom field "coordinates" for "dcim > device" and "Circuits > circuit" with type "text" and name "coordinates" you will see the same layout every time. It is recommended to set this field to "UI visibility" "Hidden" and let the plugin manage it in the background.
+Run `python3 manage.py migrate netbox_topology_views`
 
-The coordinates are stored as: "X;Y".
+Run `python3 manage.py collectstatic --no-input`
 
-Please read the "Configure" chapter to set the `allow_coordinates_saving` option to True.
-You might also set the `always_save_coordinates` option to True.
+Clear you browser cache.
 
 ## Configure
 
+### Individual Options
+
 All individual options can be assigned a default value per user directly in the plugin. The default value can be overridden on the filter page.
 
+![Individual Options](doc/img/topology_individual_options.png)
+
 The remaining options must be configured in the `PLUGINS_CONFIG` section of your `netbox/configuration.py`.
 
 Example:
 ```
 PLUGINS_CONFIG = {
     'netbox_topology_views': {
         'static_image_directory': 'netbox_topology_views/img',
@@ -82,73 +89,113 @@
     }
 }
 ```
 
 | Setting                  | Default value                                                                                                                                  | Description                                                                                                            |
 | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
 | static_image_directory   | netbox_topology_views/img                                                                                                                      | (str or pathlib.Path) Specifies the location that images will be loaded from by default. Must be within `STATIC_ROOT`  |
-| allow_coordinates_saving | False                                                                                                                                          | (bool) Set to true if you use the custom coordinates fields and want to save the coordinates                           |
-| always_save_coordinates  | False                                                                                                                                          | (bool) Set if you want to enable the option to save coordinates by default                                             |
+| allow_coordinates_saving | False                                                                                                                                          | (bool) Set to true if you want to enable the ability to save the coordinates.                           |
+| always_save_coordinates  | False                                                                                                                                          | (bool) Set if you want to enable the option to save coordinates by default. Setting allow_coordinates_saving to true is mandatory.                                             |
+
+### Custom field: coordinates
+
+There is also support for custom fields.
+
+>**_Note:_** The custom field "coordinates" is deprecated and will be removed in the future. Please use Coordinate Groups instead.
+
+If you create a custom field "coordinates" for "dcim > device" and "Circuits > circuit" with type "text" and name "coordinates" you will see the same layout every time. It is recommended to set this field to "UI visibility" "Hidden" and let the plugin manage it in the background.
+
+The coordinates are stored as: "X;Y".
+
+> Please read the "Configure" chapter to set the `allow_coordinates_saving` option to True.
+You might also set the `always_save_coordinates` option to True.
+
+### Convert custom field to Coordinate Groups
+
+Please note that values stored in the custom field "coordinates" are not being converted to Coordinate Groups automatically. A pragmatic way to do this conversion yourself is as follows:
++ Navigate to "Topology" > "Filters".
++ Select "Show Unconnected" and "Show Cables". 
++ Leave all other filter settings alone. We want all entries to be displayed!
++ Click "Search" and wait for the results to be displayed
++ Select all nodes. This can be done by holding down the Shift key and dragging a frame around all icons with the left mouse button.
++ Drag the selection a tiny bit to the side. This causes all coordinates for all devices to be stored in the "default" group.
+> **_Hint_**: Don't wait too long after clicking an icon in order to drag. If you hold the mouse button for too long before dragging starts, the selection is reset._
++ Storing the values might take some time, depending on the number of devices. Please be patient and check "Coordinates" in order to make sure that everthing has been stored.
++ It is save to delete the custom field now.
 
 ### Custom Images
 
-To change image with associated device use the `Images` page - it allows to map a device role with an image found in the netbox static directory (defined by the plugin config `static_image_directory` which defaults to `netbox_topology_views/img`). You can also upload you own custom images to there - these images will automatically be used for a device (if it does not already have a specified image in the settings) if their name is the device role slug.
+To change image with associated device use the `Images` page - it allows to map a device role with an image found in the NetBox static directory (defined by the plugin config `static_image_directory` which defaults to `netbox_topology_views/img`). You can also upload you own custom images to there - these images will automatically be used for a device (if it does not already have a specified image in the settings) if their name is the device role slug.
+
+![Images](doc/img/topology_images.png)
 
 ## Use
 
 Go to the plugins tab in the navbar and click topology or go to `$NETBOX_URL/plugins/netbox_topology_views/` to view your topologies
 
 Select your options for the topology view:
 
-![topology_options](https://user-images.githubusercontent.com/20901110/235302073-234c3ef7-2c2b-4d0c-a674-9909d490d7ea.png)
+![Filter Options](doc/img/topology_filter_options.png)
 
 <dl>
+    <dt>Coordinate Group</dt>
+    <dd>Select Coordinate Group. These groups allow devices to be displayed in different positions depending on the group, thus providing different representations for the same topology. If nothing is selected, the group "default" is set automatically.</dd>
     <dt>Save Coordinates</dt>
     <dd>Save the coordinates of devices in the topology view.</dd>
     <dt>Show Unconnected</dt>
     <dd>Show devices that have no connections or for which no connection is displayed. This option depends on other parameters like 'Show Cables' and 'Show Logical Connections'.</dd>
     <dt>Show Cables</dt>
     <dd>Show connections between interfaces, front / rear ports, etc., that are connected with one or more cables. These connections are displayed as solid lines in the color of the cable.</dd> 
     <dt>Show Logical Connections</dt>
     <dd>Show logical connections between interfaces (referred to as Interface Connections in NetBox) in the topology view. Where the path between
         interfaces includes multiple cables (e.g., via patch panels), only the end interface connections are shown, not the 
         intermediate front / rear port connections, etc. This is similar to what was referred to as 'end-to-end' connections in previous versions. These connections are displayed as yellow dotted lines.</dd>
-    <dt>Show redundant Cable and Locigal Connection</dt>
+    <dt>Show redundant Cable and Logical Connection</dt>
     <dd>Shows a logical connection (in addition to a cable), even if a cable is directly connected. Leaving this option disabled prevents that redundant display. This option only has an effect if 'Show Logical Connections' is activated.</dd>
     <dt>Show Neighbors</dt>
     <dd>Adds neighbors to the filter result set automatically. Link peers will be added if 'Show Cables' is ticked, far-end terminations will be added if 'Show Logical Connections' is ticked.</dd>
     <dt>Show Circuit Terminations</dt>
     <dd>Show connections which end at a circuit termination in the topology view. These connections are displayed as blue dashed lines.</dd>
     <dt>Show Power Feeds</dt>
     <dd>Displays connections between power outlets and power ports. These connections are displayed as solid lines in the color of the cable. This option depends on 'Show Cables'.</dd>
     <dt>Show Wireless Links</dt>
     <dd>Displays wireless connections. These connections are displayed as blue dotted lines.</dd>
 </dl>
     
-### Update
+### Coordinates and Coordinate Groups
 
-Run `pip install netbox-topology-views --upgrade` in your venv.
+Netbox Topology Views stores the position of the devices. In order to allow different representations for the topology, Coordinate Groups are supported.
 
-Run `python3 manage.py migrate netbox_topology_views`
+> Please read the "Configure" chapter to set the `allow_coordinates_saving` option to True.
+You might also set the `always_save_coordinates` option to True.
 
-Run `python3 manage.py collectstatic --no-input`
+Navigate to "Coordinate Groups" in the menu and create as many groups as you like. You can select a group later in the filter pane in order to show icon positions according to this group (see chapter "Use"). You can also omit creating a group if you don't need this feature. Netbox Topology Views automatically creates a group named "default" for you and stores all coordinates in this group, even if you do not select a group in the filter.
 
+By default, the position of the devices are calculated with a physics engine. As soon as a device icon is dragged to another location, its position is saved and excluded from the calculation by the physics engine. All saved coordinates can be viewed and edited under the menu item "Coordinates".
 
-Clear you browser cache.
-
+> **_Note:_** At the time of writing, it is not possible to store the positions of circuit terminations, power panels and power feeds, as these are not devices.
 
 ### Permissions
 
 To view `/plugins/netbox_topology-views/topology` you need the following permissions:
  + dcim | device | can view device
  + dcim | site | can view site
  + extras | tag | can view tag
  + dcim | device role | can view device role
 
-To view `/plugins/netbox_topology-views/image`:
+To save `Coordinates` when moving icons:
+ + netbox_topology_views | coordinate | change
+
+To view `/plugins/netbox_topology-views/images`:
  + dcim | site | view
  + dcim | device role | view
  + dcim | device role | add
  + dcim | device role | change
 
- To view `/plugins/netbox_topology-views/individualoptions`:
- + netbox topology views | individualoptions | change
+To view `/plugins/netbox_topology-views/individualoptions`:
+ + netbox_topology_views | individual options | change
+
+Set `Coordinate Groups` according to your needs:
+ + netbox_topology_views | coordinate groups | view/add/change/delete
+
+Set `Coordinates` according to your needs:
+ + netbox_topology_views | coordinate | view/add/change/delete
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/__init__.py` & `netbox-topology-views-3.6.0b1/netbox_topology_views/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from extras.plugins import PluginConfig
 
 
 class TopologyViewsConfig(PluginConfig):
     name = "netbox_topology_views"
     verbose_name = "Topology views"
     description = "An plugin to render topology maps"
-    version = "3.5.0"
+    version = "3.6.0-beta.1"
     author = "Mattijs Vanhaverbeke"
     author_email = "author@example.com"
     base_url = "netbox_topology_views"
     required_settings = []
     default_settings = {
         "static_image_directory": "netbox_topology_views/img",
         "allow_coordinates_saving": False,
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/api/views.py` & `netbox-topology-views-3.6.0b1/netbox_topology_views/api/views.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,33 +10,36 @@
 from rest_framework.response import Response
 from rest_framework.viewsets import ReadOnlyModelViewSet, ViewSet
 
 from netbox_topology_views.api.serializers import (
     RoleImageSerializer,
     TopologyDummySerializer,
 )
-from netbox_topology_views.models import RoleImage, IndividualOptions
+from netbox_topology_views.models import RoleImage, IndividualOptions, CoordinateGroup, Coordinate
 from netbox_topology_views.views import get_topology_data
 from netbox_topology_views.utils import get_image_from_url, export_data_to_xml, get_query_settings
 from netbox_topology_views.filters import DeviceFilterSet
 
-class SaveCoordsViewSet(ReadOnlyModelViewSet):
+class SaveCoordsViewSet(PermissionRequiredMixin, ReadOnlyModelViewSet):
+    permission_required = 'netbox_topology_views.change_coordinate'
+
     queryset = Device.objects.none()
     serializer_class = TopologyDummySerializer
 
     @action(detail=False, methods=["patch"])
     def save_coords(self, request):
         if not settings.PLUGINS_CONFIG["netbox_topology_views"][
             "allow_coordinates_saving"
         ]:
             return Response({"status": "not allowed to save coords"}, status=500)
 
         device_id: str = request.data.get("node_id", None)
         x_coord = request.data.get("x", None)
         y_coord = request.data.get("y", None)
+        group_id = request.data.get("group", "None")
 
         actual_device = None
         if device_id.startswith("c"):
             device_id = device_id.lstrip("c")
             actual_device = Circuit.objects.get(id=device_id)
         elif device_id.startswith("p"):
             device_id = device_id.lstrip("p")
@@ -46,30 +49,45 @@
             actual_device = PowerFeed.objects.get(id=device_id)
         elif device_id.isnumeric():
             actual_device = Device.objects.get(id=device_id)
 
         if not actual_device:
             return Response({"status": "invalid node_id in body"}, status=400)
 
+        if group_id is None or group_id == "default":
+            group_id = Coordinate.get_or_create_default_group(group_id)
+            if not group_id:
+                return Response(
+                    {"status": "Error while creating default group."}, status=500
+                )  
+
         try:
-            actual_device.custom_field_data["coordinates"] = "%s;%s" % (
-                x_coord,
-                y_coord,
-            )
-            actual_device.save()
+            if CoordinateGroup.objects.filter(pk=group_id):
+                group = CoordinateGroup.objects.get(pk=group_id)
+                # Hen-and-egg-problem. Thanks, Django! By default, Django updates records that
+                # already exist and inserts otherwise. This does not work with our 
+                # unique_together key if no pk is given. But: No record, no pk.
+                if not Coordinate.objects.filter(group=group, device=actual_device):
+                    # Unique group/device pair does not exist. Prepare new data set
+                    coords = Coordinate(group=group, device=actual_device, x=x_coord, y=y_coord)
+                else:
+                    # Unique group/device pair already exists. Update data
+                    coords = Coordinate(pk=Coordinate.objects.get(group=group, device=actual_device).pk, group=group, device=actual_device, x=x_coord, y=y_coord)  
+                coords.save()
         except:
             return Response(
-                {"status": "coords custom field could not be saved"}, status=500
+                {"status": "Coordinates could not be saved."}, status=500
             )
 
         return Response({"status": "saved coords"})
 
 class ExportTopoToXML(PermissionRequiredMixin, ViewSet):
-    queryset = Device.objects.none()
     permission_required = ("dcim.view_site", "dcim.view_device")
+
+    queryset = Device.objects.none()
     serializer_class = TopologyDummySerializer
 
     def list(self, request):
 
         self.filterset = DeviceFilterSet
         self.queryset = Device.objects.all().select_related(
             "device_type", "device_role"
@@ -79,44 +97,50 @@
         individualOptions, created = IndividualOptions.objects.get_or_create(
             user_id=request.user.id,
         )
 
         if request.GET:
 
             save_coords, show_unconnected, show_power, show_circuit, show_logical_connections, show_single_cable_logical_conns, show_cables, show_wireless, show_neighbors = get_query_settings(request)
+            if 'group' not in request.query_params:
+                group_id = "default"
+            else:
+                group_id = request.query_params["group"]
             topo_data = get_topology_data(
                 queryset=self.queryset,
                 individualOptions=individualOptions,
                 save_coords=save_coords,
                 show_unconnected=show_unconnected,
                 show_cables=show_cables,
                 show_logical_connections=show_logical_connections,
                 show_single_cable_logical_conns=show_single_cable_logical_conns,
                 show_neighbors=show_neighbors,
                 show_circuit=show_circuit,
                 show_power=show_power,
                 show_wireless=show_wireless,
+                group_id=group_id,
             )
             xml_data = export_data_to_xml(topo_data).decode('utf-8')
 
             return HttpResponse(xml_data, content_type="application/xml; charset=utf-8")
         else:
             return JsonResponse(
                 {"status": "Missing or malformed request parameters"}, status=400
             )
 
-class SaveRoleImageViewSet(PermissionRequiredMixin, ViewSet):
+class SaveRoleImageViewSet(PermissionRequiredMixin, ReadOnlyModelViewSet):
     queryset = DeviceRole.objects.none()
     serializer_class = RoleImageSerializer
     permission_required = (
         "dcim.add_device_role",
         "dcim.change_device_role",
     )
 
-    def create(self, request):
+    @action(detail=False, methods=["post"])
+    def save(self, request):
         if not isinstance(request.data, dict):
             return JsonResponse(
                 {"status": "Missing or malformed request body"}, status=400
             )
 
         device_roles = {k: v for k, v in request.data.items() if k.isnumeric()}
         content_type_ids = {
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/filters.py` & `netbox-topology-views-3.6.0b1/netbox_topology_views/filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import django_filters
 from dcim.choices import DeviceStatusChoices
 from dcim.models import Device, DeviceRole, Location, Rack, Region, Site
 from django.db.models import Q
 from netbox.filtersets import NetBoxModelFilterSet
 from tenancy.filtersets import TenancyFilterSet
 from utilities.filters import TreeNodeMultipleChoiceFilter
-
+from netbox_topology_views.models import CoordinateGroup, Coordinate
 
 class DeviceFilterSet(TenancyFilterSet, NetBoxModelFilterSet):
     q = django_filters.CharFilter(
         method="search",
         label="Search",
     )
     device_role_id = django_filters.ModelMultipleChoiceFilter(
@@ -49,7 +49,29 @@
 
     def search(self, queryset, name, value):
         """Perform the filtered search."""
         if not value.strip():
             return queryset
         qs_filter = Q(name__icontains=value)
         return queryset.filter(qs_filter)
+
+class CoordinatesFilterSet(NetBoxModelFilterSet):
+    group = django_filters.ModelMultipleChoiceFilter(
+        queryset = CoordinateGroup.objects.all(),
+    )
+
+    device = django_filters.ModelMultipleChoiceFilter(
+        queryset = Device.objects.all(),
+    )
+
+    class Meta:
+        model = Coordinate
+        fields = ['id', 'group', 'device', 'x', 'y']
+
+    def search(self, queryset, name, value):
+        """Perform the filtered search."""
+        if not value.strip():
+            return queryset
+        return queryset.filter(
+            Q(group__name__icontains=value) |
+            Q(device__name__icontains=value)
+        )
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/forms.py` & `netbox-topology-views-3.6.0b1/netbox_topology_views/forms.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,32 +8,36 @@
 from dcim.models import Device, Site, Region, DeviceRole, Location, Rack
 
 from django import forms
 from dcim.choices import DeviceStatusChoices
 from tenancy.models import TenantGroup, Tenant
 from tenancy.forms import TenancyFilterForm
 from django.conf import settings
-from netbox.forms import NetBoxModelFilterSetForm, NetBoxModelForm
+from netbox.forms import NetBoxModelFilterSetForm, NetBoxModelForm, NetBoxModelImportForm
 from utilities.forms.fields import (
     TagFilterField,
-    DynamicModelMultipleChoiceField,
-    MultipleChoiceField
+    DynamicModelMultipleChoiceField
 )
 
-
-from .models import IndividualOptions
+from netbox_topology_views.models import IndividualOptions, CoordinateGroup, Coordinate
 
 class DeviceFilterForm(TenancyFilterForm, NetBoxModelFilterSetForm):
     model = Device
     fieldsets = (
         (
             None,
             (
                 "q",
                 "filter_id",
+            ),          
+        ),
+        (
+            None,
+            (
+                "group",
                 "save_coords",
                 "show_unconnected",
                 "show_cables",
                 "show_logical_connections",
                 "show_single_cable_logical_conns",
                 "show_neighbors",
                 "show_circuit",
@@ -55,15 +59,19 @@
                 "device_role_id",
                 "id",
                 "status",
             ),
         ),
         (None, ("tag",)),
     )
-
+    group = forms.ModelChoiceField(
+        queryset=CoordinateGroup.objects.all(),
+        required=False,
+        label=_("Coordinate group"),
+    )
     region_id = DynamicModelMultipleChoiceField(
         queryset=Region.objects.all(), required=False, label=_("Region")
     )
     device_role_id = DynamicModelMultipleChoiceField(
         queryset=DeviceRole.objects.all(), required=False, label=_("Device Role")
     )
     id = DynamicModelMultipleChoiceField(
@@ -100,15 +108,15 @@
         query_params={
             "region_id": "$region_id",
             "site_id": "$site_id",
             "location_id": "$location_id",
         },
         label=_("Rack"),
     )
-    status = MultipleChoiceField(
+    status = forms.MultipleChoiceField(
         choices=DeviceStatusChoices, required=False, label=_("Device Status")
     )
     tag = TagFilterField(model)
 
     # options
     save_coords = forms.BooleanField(
         label=_("Save Coordinates"),
@@ -122,38 +130,92 @@
     show_cables = forms.BooleanField(
         label =_("Show Cables"), required=False, initial=False
     )
     show_logical_connections = forms.BooleanField(
         label =_("Show Logical Connections"), required=False, initial=False
     )
     show_single_cable_logical_conns = forms.BooleanField(
-        label =_("Show redundant Cable and Locigal Connection"), required=False, initial=False
+        label =_("Show redundant Cable and Logical Connection"), required=False, initial=False
     )
     show_neighbors = forms.BooleanField(
         label =_("Show Neighbors"), required=False, initial=False
     )
     show_circuit = forms.BooleanField(
         label=_("Show Circuit Terminations"), required=False, initial=False
     )
     show_power = forms.BooleanField(
         label=_("Show Power Feeds"), required=False, initial=False
     )
     show_wireless = forms.BooleanField(
         label =_("Show Wireless Links"), required=False, initial=False
     )
 
+class CoordinateGroupsForm(NetBoxModelForm):
+    fieldsets = (
+        ('Group Details', ('name', 'description')),
+    )
+
+    class Meta:
+        model = CoordinateGroup
+        fields = ('name', 'description')
+
+class CoordinateGroupsImportForm(NetBoxModelImportForm):
+    class Meta:
+        model = CoordinateGroup
+        fields = ('name', 'description')
+
+class CoordinatesForm(NetBoxModelForm):
+    fieldsets = (
+        ('Coordinate', ('group', 'device', 'x', 'y')),
+    )
+
+    class Meta:
+        model = Coordinate
+        fields = ('group', 'device', 'x', 'y')
+
+class CoordinatesImportForm(NetBoxModelImportForm):
+    class Meta:
+        model = Coordinate
+        fields = ('group', 'device', 'x', 'y')
+
+class CoordinatesFilterForm(NetBoxModelFilterSetForm):
+    model = Coordinate
+    fieldsets = (
+        (None, ('q', 'filter_id')),
+        ('Coordinates', ('group', 'device', 'x', 'y'))
+    )
+
+    group = forms.ModelMultipleChoiceField(
+        queryset=CoordinateGroup.objects.all(),
+        required=False
+    )
+
+    device = DynamicModelMultipleChoiceField(
+        queryset=Device.objects.all(),
+        required=False
+    )
+
+    x = forms.IntegerField(
+        required=False
+    )
+
+    y = forms.IntegerField(
+        required=False
+    )
+
 class IndividualOptionsForm(NetBoxModelForm):
     fieldsets = (
         (
             None,
             (
                 "user_id",
                 "ignore_cable_type",
                 "preselected_device_roles",
                 "preselected_tags",
+                "save_coords",
                 "show_unconnected",
                 "show_cables",
                 "show_logical_connections",
                 "show_single_cable_logical_conns",
                 "show_neighbors",
                 "show_circuit",
                 "show_power",
@@ -161,15 +223,15 @@
                 "draw_default_layout",
             ),
         ),
     )
 
     user_id = forms.CharField(widget=forms.HiddenInput())
 
-    ignore_cable_type = MultipleChoiceField(
+    ignore_cable_type = forms.MultipleChoiceField(
         label=_("Ignore Termination Types"), 
         required=False, 
         choices=IndividualOptions.CHOICES,
         help_text=_("Choose Termination Types that you want to be ignored. "
             "If any ignored Termination Type is part of a connection, the "
             "cable is not displayed.")
     )
@@ -183,14 +245,23 @@
     preselected_tags = forms.ModelMultipleChoiceField(
         label=_("Preselected Tags"),
         queryset=Device.tags.all(),
         required=False,
         help_text=_("Select Tags that you want to have "
             "preselected in the filter tab.")
     )
+    save_coords = forms.BooleanField(
+        label=_("Save Coordinates"), 
+        required=False, 
+        initial=False,
+        help_text=_("Coordinates of nodes will be saved if dragged to a different "
+            "position. This option depends on parameters set in the config file. "
+            "It has no effect if 'allow_coordinates_saving' has not been set or "
+            " 'always_save_coordinates' has been set.")
+    )
     show_unconnected = forms.BooleanField(
         label=_("Show Unconnected"), 
         required=False, 
         initial=False,
         help_text=_("Draws devices that have no connections or for which no "
             "connection is displayed. This option depends on other parameters "
             "like 'Show Cables' and 'Show Logical Connections'.")
@@ -208,15 +279,15 @@
         required=False, 
         initial=False,
         help_text=_("Displays connections between devices that are not "
             "directly connected (e.g. via patch panels). These connections "
             "are displayed as yellow dotted lines.")
     )
     show_single_cable_logical_conns = forms.BooleanField(
-        label = ("Show redundant Cable and Locigal Connection"),
+        label = ("Show redundant Cable and Logical Connection"),
         required = False,
         initial=False,
         help_text=_("Shows a logical connection (in addition to a cable), "
             "even if a cable is directly connected. Leaving this option "
             "disabled prevents that redundant display. This option only "
             "has an effect if 'Show Logical Connections' is activated.")
     )
@@ -257,10 +328,9 @@
         help_text=_("Enable this option if you want to draw the topology on "
             "the initial load (when you go to the topology plugin page).")
     )
 
     class Meta:
         model = IndividualOptions
         fields = [
-            'user_id', 'ignore_cable_type', 'preselected_device_roles', 'preselected_tags', 'show_unconnected', 'show_cables', 'show_logical_connections', 'show_single_cable_logical_conns', 'show_neighbors', 'show_circuit', 'show_power', 'show_wireless', 'draw_default_layout'
-        ]
-        
+            'user_id', 'ignore_cable_type', 'preselected_device_roles', 'preselected_tags', 'save_coords', 'show_unconnected', 'show_cables', 'show_logical_connections', 'show_single_cable_logical_conns', 'show_neighbors', 'show_circuit', 'show_power', 'show_wireless', 'draw_default_layout'
+        ]
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/migrations/0001_initial.py` & `netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/migrations/0002_individualoptions.py` & `netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0002_individualoptions.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/models.py` & `netbox-topology-views-3.6.0b1/netbox_topology_views/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from pathlib import Path
 from typing import Optional
 
-from dcim.models import DeviceRole
+from dcim.models import Device, DeviceRole
 from extras.models import Tag
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.templatetags.static import static
+from django.urls import reverse
 from netbox.models import NetBoxModel
 from netbox.models.features import (
     ChangeLoggingMixin,
     ExportTemplatesMixin,
     WebhooksMixin,
 )
 
@@ -90,14 +91,87 @@
     def get_image_url(self, dir: Path = CONF_IMAGE_DIR) -> str:
         try:
             self.get_image()
         except ValueError:
             return self.get_default_image(dir)
         return static(f"/{self.image}")
 
+class CoordinateGroup(NetBoxModel):
+    """
+    A coordinate group is used to display the topology for a particular group. 
+    This allows different visualizations with the same devices.
+    """
+    name = models.CharField(
+        max_length=100,
+        unique=True,
+    )
+
+    description = models.CharField(
+        max_length=255,
+        blank = True,
+    )
+
+    class Meta:
+        ordering = ['name']
+
+    def __str__(self):
+        return self.name
+
+    def get_absolute_url(self):
+        return reverse('plugins:netbox_topology_views:coordinategroup', args=[self.pk])
+
+class Coordinate(NetBoxModel):
+    """
+    Coordinates are being used to place devices in a topology view onto a certain 
+    position. Devices belong to one or more coordinate groups. They have to 
+    be unique together.
+    """
+    device = models.ForeignKey(Device, on_delete=models.CASCADE)
+    group = models.ForeignKey(CoordinateGroup, on_delete=models.CASCADE)
+    
+    x = models.IntegerField(
+        help_text='X-coordinate of the device (horizontal) on the canvas. '
+            'Smaller values correspond to a position further up on the monitor.',
+    )
+    y = models.IntegerField(
+        help_text='Y-coordinate of the device (vertical) on the canvas. '
+            'Smaller values correspond to a position further to the left on the monitor.',
+    )
+
+    def get_or_create_default_group(group_id):
+        # Default group named "default" must always exist in order to make sure
+        # that coordinate values can be stored even if no coordinate group has been
+        # selected. The default group will be added automatically if it does not exist.
+        try:
+            if CoordinateGroup.objects.filter(name="default"):
+                group = CoordinateGroup.objects.get(name="default")
+                group_id = group.pk
+            else:
+                group = CoordinateGroup(
+                    name="default", 
+                    description="Automatically generated default group. If you delete "
+                        "this group, all default coordinates are gone for good but "
+                        "the group itself will be re-created."
+                )
+                group.save()
+                group_id = group.pk
+        except:
+            return False
+        return group_id
+
+    class Meta:
+        ordering = ['group', 'device']
+        unique_together = ('device', 'group')
+
+    def __str__(self):
+        return f'{self.x};{self.y}'
+
+    def get_absolute_url(self):
+        return reverse('plugins:netbox_topology_views:coordinate', args=[self.pk])
+
 class IndividualOptions(NetBoxModel):
     CHOICES = (
         ('interface', 'interface'),
         ('front port', 'front port'),
         ('rear port', 'rear port'),
         ('power outlet', 'power outlet'),
         ('power port', 'power port'),
@@ -121,14 +195,17 @@
     )
     preselected_tags = models.ManyToManyField(
         to='extras.Tag',
         related_name='+',
         blank=True,
         db_table='netbox_topology_views_individualoptions_preselected_tag',
     )
+    save_coords = models.BooleanField(
+        default=False
+    )
     show_unconnected = models.BooleanField(
         default=False
     )
     show_cables = models.BooleanField(
         default=False
     )
     show_logical_connections = models.BooleanField(
@@ -150,8 +227,8 @@
         default=False
     )
     draw_default_layout = models.BooleanField(
         default=False
     )
 
     def __str___(self):
-        return f"{self.user_id}"
+        return f"{self.user_id}"
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/signals.py` & `netbox-topology-views-3.6.0b1/netbox_topology_views/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/css/vendor.css` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/css/vendor.css`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/LICENSE` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/backup.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/backup.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/camera.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/camera.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/circuit.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/circuit.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/console-server.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/console-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/core-router.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/core-router.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/database-server.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/database-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/database.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/database.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/desktop.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/desktop.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/firewall.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/firewall.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/kvm.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/kvm.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/modem.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/modem.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/notebook.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/notebook.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/pabx.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/pabx.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/pdu.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/pdu.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/phone.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/phone.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/power-units.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/power-units.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/printer.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/printer.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/proxy.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/proxy.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/router.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/router.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/server.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/siem.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/siem.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/storage.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/storage.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/switch.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/ups.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/ups.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/app.js` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/app.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13138,35 +13138,43 @@
         if (!topologyData) return;
 
         function e(s) {
             let o = document.createElement("div");
             return o.innerHTML = s, o
         }
         let t = new Te(topologyData.nodes.map(s => Be(de({}, s), {
-                title: e(s.title)
-            }))),
-            i = new Te(topologyData.edges.map(s => Be(de({}, s), {
-                title: e(s.title)
-            })));
+            title: e(s.title)
+        })));
+        window.nodes = t;
+        let i = new Te(topologyData.edges.map(s => Be(de({}, s), {
+            title: e(s.title)
+        })));
         Ge = new I(kn, {
             nodes: t,
             edges: i
         }, qi), Ge.fit(), Ge.on("dragEnd", s => {
             Sn != null && (!Sn.checked || Promise.allSettled(Object.entries(Ge.getPositions(s.nodes)).map(a => Xi(this, [a], function*([o, r]) {
+                window.nodes.update({
+                    id: parseInt(o),
+                    physics: !1,
+                    x: r.x,
+                    y: r.y
+                });
                 let d = yield fetch("/api/plugins/netbox_topology_views/save-coords/save_coords/", {
                     method: "PATCH",
                     headers: {
                         "X-CSRFToken": Ba,
                         Accept: "application/json",
                         "Content-Type": "application/json"
                     },
                     body: JSON.stringify({
                         node_id: o,
                         x: r.x,
-                        y: r.y
+                        y: r.y,
+                        group: topologyData.group
                     })
                 });
                 console.log(o, d.status, d.statusText)
             }))))
         }), Ge.on("doubleClick", s => {
             s.nodes.length > 0 ? s.nodes.forEach(o => {
                 window.open(t.get(o).href, "_blank")
@@ -13189,20 +13197,33 @@
     }
     var Ra = document.querySelector("#btnDownloadXml");
     Ra.addEventListener("click", n => {
         Ha()
     });
 
     function Ha() {
-        let n = document.createElement("a");
-        fetch("/api/plugins/netbox_topology_views/xml-export/?" + new URLSearchParams(window.location.search)).then(e => e.text()).then(e => {
-            var t = new Blob([e], {
+        let n = document.createElement("a"),
+            e = "";
+        if (typeof is_htmx != "undefined") {
+            var t = window.location.href;
+            let o = "/sites/",
+                r = "/locations/";
+            if (t.includes(o)) {
+                var i = t.split(o)[1];
+                i = i.split("/")[0], e = "site_id=" + i + "&show_cables=on&show_unconnected=on"
+            } else if (t.includes(r)) {
+                var s = t.split(r)[1];
+                s = s.split("/")[0], e = "location_id=" + s + "&show_cables=on&show_unconnected=on"
+            }
+        } else e = new URLSearchParams(window.location.search);
+        fetch("/api/plugins/netbox_topology_views/xml-export/?" + e).then(o => o.text()).then(o => {
+            var r = new Blob([o], {
                 type: "text/plain"
             });
-            n.setAttribute("href", window.URL.createObjectURL(t)), n.setAttribute("download", "topology.xml"), n.dataset.downloadurl = ["text/plain", n.download, n.href].join(":"), n.click()
+            n.setAttribute("href", window.URL.createObjectURL(r)), n.setAttribute("download", "topology.xml"), n.dataset.downloadurl = ["text/plain", n.download, n.href].join(":"), n.click()
         })
     }
     var ja = new MutationObserver(n => n.forEach(e => {
         if (!Ge || e.type !== "attributes" || e.attributeName !== "data-netbox-color-mode" || !(e.target instanceof HTMLElement)) return;
         let {
             netboxColorMode: t
         } = e.target.dataset;
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/images.js` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/images.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -45,15 +45,15 @@
         }
     };
     var g = {},
         p = d("csrftoken");
     document.querySelector("form#images").addEventListener("submit", e => l(void 0, null, function*() {
         e.preventDefault();
         try {
-            let t = yield fetch("/api/plugins/netbox_topology_views/images/", {
+            let t = yield fetch("/api/plugins/netbox_topology_views/images/save/", {
                 method: "POST",
                 body: JSON.stringify(g),
                 headers: {
                     "X-CSRFToken": p,
                     "Content-Type": "application/json"
                 }
             });
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/static/netbox_topology_views/js/images.js.map` & `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/images.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'mappings'": "'mNAAO,GAAM,GAAY,AAAC,GAAS,CAC/B,GAAI,CAAC,SAAS,OAAQ,OAEtB,GAAI,GAAc,KACZ,EAAU,SAAS,OAAO,MAAM,KAEtC,OAAS,GAAI,EAAG,EAAI,EAAQ,OAAQ,IAAK,CACrC,GAAM,GAAS,EAAQ,GAAG,OAE1B,GAAI,EAAO,UAAU,EAAG,EAAK,OAAS,KAAO,EAAO,IAAK,CACrD,EAAc,mBAAmB,EAAO,UAAU,EAAK,OAAS,IAChE,OAIR,MAAO,ICfJ,GAAM,GAAQ,CACjB,QAAS,AAAC,GAAY,CAClB,GAAM,GAAK,SAAS,cAAc,kCAClC,GAAI,CAAC,EAAI,MAAO,SAAQ,MAAM,mCAC9B,GAAM,GAAU,EAAG,cAAc,QACjC,EAAQ,YAAc,EAEtB,AADc,GAAI,QAAO,MAAM,GACzB,QAEV,MAAO,AAAC,GAAY,CAChB,GAAM,GAAK,SAAS,cAAc,gCAClC,GAA […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "mappings": "mNAAO,GAAM,GAAY,AAAC,GAAS,CAC/B,GAAI,CAAC,SAAS,OAAQ,OAEtB,GAAI,GAAc,KACZ,EAAU,SAAS,OAAO,MAAM,KAEtC,OAAS,GAAI,EAAG,EAAI,EAAQ,OAAQ,IAAK,CACrC,GAAM,GAAS,EAAQ,GAAG,OAE1B,GAAI,EAAO,UAAU,EAAG,EAAK,OAAS,KAAO,EAAO,IAAK,CACrD,EAAc,mBAAmB,EAAO,UAAU,EAAK,OAAS,IAChE,OAIR,MAAO,ICfJ,GAAM,GAAQ,CACjB,QAAS,AAAC,GAAY,CAClB,GAAM,GAAK,SAAS,cAAc,kCAClC,GAAI,CAAC,EAAI,MAAO,SAAQ,MAAM,mCAC9B,GAAM,GAAU,EAAG,cAAc,QACjC,EAAQ,YAAc,EAEtB,AADc,GAAI,QAAO,MAAM,GACzB,QAEV,MAAO,AAAC,GAAY,CAChB,GAAM,GAAK,SAAS,cAAc,gCAClC,GAAI,CAAC,EAAI,MAAO,SAAQ,MAAM,mCAC9B,GAAM,GAAU,EAAG,cAAc,QACjC,EAAQ,YAAc,EAEtB,AADc,GAAI,QAAO,MAAM,GACzB,SCZd,GAAM,GAAU,GACV,EAAY,EAAU,aAE5B,SAAS,cAAc,eAAe,iBAAiB,SAAU,AAAO,GAAM,0BAC1E,EAAE,iBACF,GAAI,CACA,GAAM,GAAM,KAAM,OAAM,6CAA8C,CAClE,OAAQ,OACR,KAAM,KAAK,UAAU,GACrB,QAAS,CACL,cAAe,EACf,eAAgB,sBAIxB,GAAI,CAAC,EAAI,GAAI,KAAM,IAAI,OAAM,KAAM,GAAI,QACvC,EAAM,QAAQ,wBACT,EAAP,CACE,QAAQ,IAAI,GACZ,EAAM,MAAM,EAAI,aAIxB,SAAS,iBAAiB,kCAAkC,QAAQ,AAAC,GAAO,CACxE,EAAG,iBAAiB,QAAS,AAAC,GAAM,CA3BxC,MA4BQ,GAAI,CAAE,GAAE,wBAAyB,cAAc,OAC/C,GAAM,CACF,QAAS,CAAE,OAAM,UACjB,EAAE,cAEN,EAAQ,GAAQ,EAEhB,GAAM,GAAS,KAAE,cACZ,QAAQ,eADE,cAET,cAAc,sBAAsB,KAC1C,AAAI,GAAQ,GAAO,UAAY,aAAa",
+    "mappings": "mNAAO,GAAM,GAAY,AAAC,GAAS,CAC/B,GAAI,CAAC,SAAS,OAAQ,OAEtB,GAAI,GAAc,KACZ,EAAU,SAAS,OAAO,MAAM,KAEtC,OAAS,GAAI,EAAG,EAAI,EAAQ,OAAQ,IAAK,CACrC,GAAM,GAAS,EAAQ,GAAG,OAE1B,GAAI,EAAO,UAAU,EAAG,EAAK,OAAS,KAAO,EAAO,IAAK,CACrD,EAAc,mBAAmB,EAAO,UAAU,EAAK,OAAS,IAChE,OAIR,MAAO,ICfJ,GAAM,GAAQ,CACjB,QAAS,AAAC,GAAY,CAClB,GAAM,GAAK,SAAS,cAAc,kCAClC,GAAI,CAAC,EAAI,MAAO,SAAQ,MAAM,mCAC9B,GAAM,GAAU,EAAG,cAAc,QACjC,EAAQ,YAAc,EAEtB,AADc,GAAI,QAAO,MAAM,GACzB,QAEV,MAAO,AAAC,GAAY,CAChB,GAAM,GAAK,SAAS,cAAc,gCAClC,GAAI,CAAC,EAAI,MAAO,SAAQ,MAAM,mCAC9B,GAAM,GAAU,EAAG,cAAc,QACjC,EAAQ,YAAc,EAEtB,AADc,GAAI,QAAO,MAAM,GACzB,SCZd,GAAM,GAAU,GACV,EAAY,EAAU,aAE5B,SAAS,cAAc,eAAe,iBAAiB,SAAU,AAAO,GAAM,0BAC1E,EAAE,iBACF,GAAI,CACA,GAAM,GAAM,KAAM,OAAM,kDAAmD,CACvE,OAAQ,OACR,KAAM,KAAK,UAAU,GACrB,QAAS,CACL,cAAe,EACf,eAAgB,sBAIxB,GAAI,CAAC,EAAI,GAAI,KAAM,IAAI,OAAM,KAAM,GAAI,QACvC,EAAM,QAAQ,wBACT,EAAP,CACE,QAAQ,IAAI,GACZ,EAAM,MAAM,EAAI,aAIxB,SAAS,iBAAiB,kCAAkC,QAAQ,AAAC,GAAO,CACxE,EAAG,iBAAiB,QAAS,AAAC,GAAM,CA3BxC,MA4BQ,GAAI,CAAE,GAAE,wBAAyB,cAAc,OAC/C,GAAM,CACF,QAAS,CAAE,OAAM,UACjB,EAAE,cAEN,EAAQ,GAAQ,EAEhB,GAAM,GAAS,KAAE,cACZ,QAAQ,eADE,cAET,cAAc,sBAAsB,KAC1C,AAAI,GAAQ,GAAO,UAAY,aAAa",
     "names": [],
     "sources": [
         "../../../static_dev/js/csrftoken.js",
         "../../../static_dev/js/toast.js",
         "../../../static_dev/js/images.js"
     ],
     "version": 3
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html` & `netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html`

 * *Files 20% similar despite different names*

```diff
@@ -33,11 +33,12 @@
 <style type="text/css">
     .modal-dialog {
         max-width: 902px !important;
     }
 </style>
 
 <script type="text/javascript">
-    const brokenImage = '{{ broken_image }}';
-    const topologyData = {{ topology_data | safe }};
+    var is_htmx = true;
+    var brokenImage = '{{ broken_image }}';
+    var topologyData = {{ topology_data | safe }};
 </script>
 <script src="{% static 'netbox_topology_views/js/app.js' %}?ver={{ epoch }} " defer></script>
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/images.html` & `netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/images.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/index.html` & `netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 {% block content-wrapper %}
   {% with config=settings.PLUGINS_CONFIG.netbox_topology_views %}
     <div class="tab-content">
 
       {# Applied filters #}
       {% if filter_form %}
         {% applied_filters model filter_form request.GET %}
-        <hr style="margin-top: 0px;">
       {% endif %}
 
       <div class="tab-pane show active" id="networks" role="tabpanel" aria-labelledby="network-tab">
         <div class="panel-body">
           <div id="visgraph"></div>
         </div>
       </div>
```

#### html2text {}

```diff
@@ -13,15 +13,13 @@
     * {% if filter_form %}
     *  Filters {% if filter_form %}{% badge filter_form.changed_data|length
       bg_color="blue" %}{% endif %}
     * {% endif %} {% endblock tab_items %}
 {% endblock tabs %} {% block content-wrapper %} {% with
 config=settings.PLUGINS_CONFIG.netbox_topology_views %}
 {# Applied filters #} {% if filter_form %} {% applied_filters model filter_form
-request.GET %}
-===============================================================================
-{% endif %}
+request.GET %} {% endif %}
 {% if filter_form %}
 {% include 'inc/filter_list.html' %}
 {% endif %}
 {% endwith %} {% endblock content-wrapper %} {% block javascript %}
  {% endblock javascript %}
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/templates/netbox_topology_views/toasts.html` & `netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/toasts.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/utils.py` & `netbox-topology-views-3.6.0b1/netbox_topology_views/utils.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views/views.py` & `netbox-topology-views-3.6.0b1/netbox_topology_views/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,33 +18,52 @@
     PowerPanel,
     RearPort,
 )
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.auth.mixins import PermissionRequiredMixin
 from django.contrib.contenttypes.models import ContentType
-from django.db.models import Q, QuerySet
+from django.db.models import Q, QuerySet, Count
 from django.db.models.functions import Lower
 from django.http import HttpRequest, HttpResponseRedirect, QueryDict
-from django.shortcuts import render
+from django.shortcuts import render, get_object_or_404
 from django.views.generic import View
 from extras.models import Tag
 from wireless.models import WirelessLink
+from netbox.views.generic import (
+    ObjectView, 
+    ObjectListView, 
+    ObjectEditView, 
+    ObjectDeleteView, 
+    ObjectChangeLogView, 
+    BulkImportView
+)
+
 
-from netbox_topology_views.filters import DeviceFilterSet
-from netbox_topology_views.forms import DeviceFilterForm, IndividualOptionsForm
-from netbox_topology_views.models import RoleImage, IndividualOptions
+from netbox_topology_views.filters import DeviceFilterSet, CoordinatesFilterSet
+from netbox_topology_views.forms import (
+    DeviceFilterForm, 
+    IndividualOptionsForm, 
+    CoordinateGroupsForm, 
+    CoordinatesForm, 
+    CoordinatesFilterForm, 
+    CoordinateGroupsImportForm,
+    CoordinatesImportForm
+)
+from netbox_topology_views.models import RoleImage, CoordinateGroup, Coordinate, IndividualOptions
+from netbox_topology_views.tables import CoordinateGroupListTable, CoordinateListTable
 from netbox_topology_views.utils import (
     CONF_IMAGE_DIR,
     find_image_url,
     get_model_role,
     get_model_slug,
     image_static_url,
     LinePattern,
-    get_query_settings
+    get_query_settings,
+    IMAGE_FILETYPES
 )
 
 
 
 def get_image_for_entity(entity: Union[Device, Circuit, PowerPanel, PowerFeed]):
     is_device = isinstance(entity, Device)
     query = (
@@ -58,15 +77,15 @@
     except RoleImage.DoesNotExist:
         return find_image_url(
             entity.device_role.slug if is_device else get_model_slug(entity.__class__)
         )
 
 
 def create_node(
-    device: Union[Device, Circuit, PowerPanel, PowerFeed], save_coords: bool
+    device: Union[Device, Circuit, PowerPanel, PowerFeed], save_coords: bool, group_id="default"
 ):
     node = {}
     node_content = ""
     if isinstance(device, Circuit):
         dev_name = device.cid
         node["id"] = f"c{device.pk}"
 
@@ -140,33 +159,50 @@
                 )
 
         node["id"] = device.pk
 
         if device.device_role.color != "":
             node["color.border"] = "#" + device.device_role.color
 
-    dev_title = "<table><tbody> %s</tbody></table>" % (node_content)
-
-    node["title"] = dev_title
-    node["name"] = dev_name
-    node["label"] = dev_name
-    node["shape"] = "image"
-    node["href"] = device.get_absolute_url()
-    node["image"] = get_image_for_entity(device)
+    if group_id is None or group_id == "default":
+        group_id = Coordinate.get_or_create_default_group(group_id)
+        if not group_id:
+            print('Exception occured while handling default group.')
+            return node
+   
+    group = get_object_or_404(CoordinateGroup, pk=group_id)
 
     node["physics"] = True
-    if "coordinates" in device.custom_field_data:
+    # Coords must be set even if no coords have been stored. Otherwise nodes with coords 
+    # will not be placed correctly by vis-network.
+    node["x"] = 0
+    node["y"] = 0
+    if Coordinate.objects.filter(group=group, device=device.pk).values('x') and Coordinate.objects.filter(group=group, device=device.pk).values('y'):
+        # Coordinates data for the device exists in Coordinates Group. Let's assign them
+        node["x"] = Coordinate.objects.get(group=group, device=device.pk).x
+        node["y"] = Coordinate.objects.get(group=group, device=device.pk).y
+        node["physics"] = False
+    elif "coordinates" in device.custom_field_data:
+        # We prefer the new Coordinate model but leave the deprecated method 
+        # for now as fallback for compatibility reasons
         if device.custom_field_data["coordinates"] is not None:
             if ";" in device.custom_field_data["coordinates"]:
                 cords = device.custom_field_data["coordinates"].split(";")
                 node["x"] = int(cords[0])
                 node["y"] = int(cords[1])
                 node["physics"] = False
-        elif save_coords:
-            node["physics"] = False
+
+    dev_title = "<table><tbody> %s</tbody></table>" % (node_content)
+    node["title"] = dev_title
+    node["name"] = dev_name
+    node["label"] = dev_name
+    node["shape"] = "image"
+    node["href"] = device.get_absolute_url()
+    node["image"] = get_image_for_entity(device)
+
     return node
 
 
 def create_edge(
     edge_id: int,
     termination_a: Dict,
     termination_b: Dict,
@@ -263,14 +299,15 @@
     show_cables: bool,
     show_circuit: bool,
     show_logical_connections: bool,
     show_single_cable_logical_conns: bool,
     show_neighbors: bool,
     show_power: bool,
     show_wireless: bool,
+    group_id,
 ):
     
     supported_termination_types = []
     for t in IndividualOptions.CHOICES:
         supported_termination_types.append(t[1])
 
     if not queryset:
@@ -302,15 +339,15 @@
         rearports = RearPort.objects.filter(
             Q(device_id__in=device_ids)
         )
 
         ports = chain(interfaces, frontports, rearports)
         for port in ports:
             for link_peer in port.link_peers:
-                if link_peer.device.id not in device_ids:
+                if hasattr(link_peer, 'device') and link_peer.device.id not in device_ids:
                     device_ids.append(link_peer.device.id)
 
         if show_logical_connections:
             path_complete_interfaces = Interface.objects.filter(
                 Q(_path__is_complete=True) & Q(device_id__in=device_ids)
             )
             for path_complete_interface in path_complete_interfaces:
@@ -384,15 +421,15 @@
                 if circuit_has_connections and not show_unconnected:
                     if circuit_termination.circuit_id not in nodes_circuits:
                         nodes_circuits[
                             circuit_termination.circuit.pk
                         ] = circuit_termination.circuit
 
         for d in nodes_circuits.values():
-            nodes.append(create_node(d, save_coords))
+            nodes.append(create_node(d, save_coords, group_id))
 
     if show_power:
         power_panels_ids = PowerPanel.objects.filter(
             Q(site_id__in=site_ids)
         ).values_list("pk", flat=True)
         power_feeds: QuerySet[PowerFeed] = PowerFeed.objects.filter(
             Q(power_panel_id__in=power_panels_ids)
@@ -434,18 +471,18 @@
                     )
                 )
 
                 if power_feed.cable_id is not None:
                     cable_ids[power_feed.cable_id][power_feed.cable_end] = termination_b
 
         for d in nodes_powerfeed.values():
-            nodes.append(create_node(d, save_coords))
+            nodes.append(create_node(d, save_coords, group_id))
 
         for d in nodes_powerpanel.values():
-            nodes.append(create_node(d, save_coords))
+            nodes.append(create_node(d, save_coords, group_id))
 
     if show_logical_connections:
         interfaces = Interface.objects.filter(
             Q(_path__is_complete=True) & Q(device_id__in=device_ids)
         )
 
         for interface in interfaces:
@@ -594,18 +631,19 @@
     for qs_device in queryset:
         if qs_device.pk not in nodes_devices and show_unconnected:
             nodes_devices[qs_device.pk] = qs_device
 
     results = {}
 
     for d in nodes_devices.values():
-        nodes.append(create_node(d, save_coords))
+        nodes.append(create_node(d, save_coords, group_id))
 
     results["nodes"] = nodes
     results["edges"] = edges
+    results["group"] = group_id
     return results
 
 
 class TopologyHomeView(PermissionRequiredMixin, View):
     permission_required = ("dcim.view_site", "dcim.view_device")
 
     """
@@ -625,38 +663,45 @@
             user_id=request.user.id,
         )
 
         if request.GET:
 
             save_coords, show_unconnected, show_power, show_circuit, show_logical_connections, show_single_cable_logical_conns, show_cables, show_wireless, show_neighbors = get_query_settings(request)
             
+            if "group" not in request.GET:
+                group_id = "default"
+            else:
+                group_id = request.GET["group"]
+
             if not "draw_init" in request.GET or "draw_init" in request.GET and request.GET["draw_init"].lower() == "true":
                 topo_data = get_topology_data(
                     queryset=self.queryset,
                     individualOptions=individualOptions,
                     save_coords=save_coords,
                     show_unconnected=show_unconnected,
                     show_cables=show_cables,
                     show_logical_connections=show_logical_connections,
                     show_single_cable_logical_conns=show_single_cable_logical_conns,
                     show_neighbors=show_neighbors,
                     show_circuit=show_circuit,
                     show_power=show_power,
                     show_wireless=show_wireless,
+                    group_id=group_id,
                 )
             
         else:
             # No GET-Request in URL. We most likely came here from the navigation menu.
             preselected_device_roles = IndividualOptions.objects.get(id=individualOptions.id).preselected_device_roles.all().values_list('id', flat=True)
             preselected_tags = IndividualOptions.objects.get(id=individualOptions.id).preselected_tags.all().values_list(Lower('name'), flat=True)
 
             q = QueryDict(mutable=True)
             q.setlist("device_role_id", list(preselected_device_roles))
             q.setlist("tag", list(preselected_tags))
 
+            if individualOptions.save_coords: q['save_coords'] = "on"
             if individualOptions.show_unconnected: q['show_unconnected'] = "on"
             if individualOptions.show_cables: q['show_cables'] = "on"
             if individualOptions.show_logical_connections: q['show_logical_connections'] = "on"
             if individualOptions.show_single_cable_logical_conns: q['show_single_cable_logical_conns'] = "on"
             if individualOptions.show_neighbors: q['show_neighbors'] = "on"
             if individualOptions.show_circuit: q['show_circuit'] = "on"
             if individualOptions.show_power: q['show_power'] = "on"
@@ -705,15 +750,15 @@
         "dcim.add_device_role",
         "dcim.change_device_role",
     )
 
     def get(self, request: HttpRequest):
         images = [
             {"url": image_static_url(image), "title": image.stem}
-            for image in CONF_IMAGE_DIR.iterdir()
+            for image in CONF_IMAGE_DIR.iterdir() if image.name.lower().endswith(IMAGE_FILETYPES)
         ]
 
         roles = reduce(
             lambda acc, cur: {
                 **acc,
                 cur.name: {
                     "id": cur.pk,
@@ -747,14 +792,106 @@
             "netbox_topology_views/images.html",
             {
                 "roles": sorted(list(roles.values()), key=lambda r: r["name"]),
                 "images": images,
             },
         )
 
+class CoordinateView(PermissionRequiredMixin, ObjectView):
+    permission_required = 'netbox_topology_views.view_coordinate'
+
+    queryset = Coordinate.objects.all()
+
+class CoordinateAddView(PermissionRequiredMixin, ObjectEditView):
+    permission_required = 'netbox_topology_views.add_coordinate'
+
+    queryset = Coordinate.objects.all()
+    form = CoordinatesForm
+    template_name = 'netbox_topology_views/coordinate_add.html'
+
+class CoordinateBulkImportView(BulkImportView):
+    queryset = Coordinate.objects.all()
+    model_form = CoordinatesImportForm
+
+class CoordinateListView(PermissionRequiredMixin, ObjectListView):
+    permission_required = 'netbox_topology_views.view_coordinate'
+
+    queryset = Coordinate.objects.all()
+    table = CoordinateListTable
+    template_name = 'netbox_topology_views/coordinate_list.html'
+    filterset = CoordinatesFilterSet
+    filterset_form = CoordinatesFilterForm
+
+class CoordinateEditView(PermissionRequiredMixin, ObjectEditView):
+    permission_required = 'netbox_topology_views.change_coordinate'
+
+    queryset = Coordinate.objects.all()
+    form = CoordinatesForm
+    template_name = 'netbox_topology_views/coordinate_edit.html'
+
+class CoordinateDeleteView(PermissionRequiredMixin, ObjectDeleteView):
+    permission_required = 'netbox_topology_views.delete_coordinate'
+
+    queryset = Coordinate.objects.all()
+
+class CoordinateChangeLogView(PermissionRequiredMixin, ObjectChangeLogView):
+    permission_required = 'netbox_topology_views.view_coordinate'
+
+    queryset = Coordinate.objects.all()
+
+class CoordinateGroupView(PermissionRequiredMixin, ObjectView):
+    permission_required = 'netbox_topology_views.view_coordinategroup'
+
+    queryset = CoordinateGroup.objects.all()
+
+    def get_extra_context(self, request, instance):
+        table = CoordinateListTable(instance.coordinate_set.all())
+        table.configure(request)
+
+        return {
+            'coordinates_table': table,
+        }
+
+class CoordinateGroupAddView(PermissionRequiredMixin, ObjectEditView):
+    permission_required = 'netbox_topology_views.add_coordinategroup'
+
+    queryset = CoordinateGroup.objects.all()
+    form = CoordinateGroupsForm
+    template_name = 'netbox_topology_views/coordinategroup_add.html'
+
+class CoordinateGroupBulkImportView(BulkImportView):
+    queryset = CoordinateGroup.objects.all()
+    model_form = CoordinateGroupsImportForm
+
+class CoordinateGroupListView(PermissionRequiredMixin, ObjectListView):
+    permission_required = 'netbox_topology_views.view_coordinategroup'
+
+    queryset = CoordinateGroup.objects.annotate(
+        devices = Count('coordinate')
+    )
+    table = CoordinateGroupListTable
+    template_name = 'netbox_topology_views/coordinategroup_list.html'
+
+class CoordinateGroupEditView(PermissionRequiredMixin, ObjectEditView):
+    permission_required = 'netbox_topology_views.change_coordinategroup'
+
+    queryset = CoordinateGroup.objects.all()
+    form = CoordinateGroupsForm
+    template_name = 'netbox_topology_views/coordinategroup_edit.html'
+
+class CoordinateGroupDeleteView(PermissionRequiredMixin, ObjectDeleteView):
+    permission_required = 'netbox_topology_views.delete_coordinategroup'
+
+    queryset = CoordinateGroup.objects.all()
+
+class CoordinateGroupChangeLogView(PermissionRequiredMixin, ObjectChangeLogView):
+    permission_required = 'netbox_topology_views.view_coordinategroup'
+
+    queryset = CoordinateGroup.objects.all()
+
 class TopologyIndividualOptionsView(PermissionRequiredMixin, View):
     permission_required = 'netbox_topology_views.change_individualoptions'
 
     def post(self, request):
         instance = IndividualOptions.objects.get(user_id=request.user.id)
         form = IndividualOptionsForm(request.POST, instance=instance)
         if form.is_valid():
@@ -772,14 +909,15 @@
 
         form = IndividualOptionsForm(
             initial={
                 'user_id': request.user.id,
                 'ignore_cable_type': tuple(queryset.ignore_cable_type.translate({ord(i): None for i in '[]\''}).split(', ')),
                 'preselected_device_roles': IndividualOptions.objects.get(id=queryset.id).preselected_device_roles.all(),
                 'preselected_tags': IndividualOptions.objects.get(id=queryset.id).preselected_tags.all(),
+                'save_coords': queryset.save_coords,
                 'show_unconnected': queryset.show_unconnected,
                 'show_cables': queryset.show_cables, 
                 'show_logical_connections': queryset.show_logical_connections,
                 'show_single_cable_logical_conns': queryset.show_single_cable_logical_conns,
                 'show_neighbors': queryset.show_neighbors,
                 'show_circuit': queryset.show_circuit,
                 'show_power': queryset.show_power,
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views.egg-info/PKG-INFO` & `netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.5.0
+Version: 3.6.0b1
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
@@ -13,26 +13,30 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Netbox Topology Views Plugin
 
 ![Version](https://img.shields.io/pypi/v/netbox-topology-views) ![Downloads](https://img.shields.io/pypi/dm/netbox-topology-views)
 
-Create topology views/maps from your devices in netbox.
-The connections are based on the cables you created in netbox.
-Support to filter on name, site, tag and device role.
+Create topology views/maps from your devices in NetBox.
+The connections are based on the cables you created in NetBox.
+Support to filter on name, site, tag and device role.  
+Options to export to xml (for draw.io/diagrams.net) or png.
 
 ## Preview
 
-![preview image](doc/img/preview_3.1.jpeg?raw=true "preview")
+![Topology with light mode](doc/img/topology_light.png)
+![Topology with dark mode](doc/img/topology_dark.png)
 
 ## Install
 
 **_NOTE:_** For docker please see: [Docker install](https://github.com/netbox-community/netbox-docker/wiki/Using-Netbox-Plugins)
 
+**_NOTE:_** Add `RUN mkdir -p /opt/netbox/netbox/static/netbox_topology_views/img` to the Dockerfile-Plugins file to create the image folder
+
 The plugin is available as a Python package and can be installed with pip.
 
 Run `pip install netbox-topology-views` in your virtual env.
 
 To ensure NetBox Topology Views plugin is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the NetBox root directory (alongside `requirements.txt`) and list the `netbox-topology-views` package:
 
 ```no-highlight
@@ -66,29 +70,32 @@
 | >= 3.3.0       | >= v3.0.0                     |
 | >= 3.2.0       | >= v1.1.0                     |
 | >= 3.1.8       | >= v1.0.0                     |
 | >= 2.11.1      | >= v0.5.3                     |
 | >= 2.10.0      | >= v0.5.0                     |
 | < 2.10.0       | =< v0.4.10                    |
 
-### Custom field: coordinates
+### Update
 
-There is also support for custom fields.
+Run `pip install netbox-topology-views --upgrade` in your venv.
 
-If you create a custom field "coordinates" for "dcim > device" and "Circuits > circuit" with type "text" and name "coordinates" you will see the same layout every time. It is recommended to set this field to "UI visibility" "Hidden" and let the plugin manage it in the background.
+Run `python3 manage.py migrate netbox_topology_views`
 
-The coordinates are stored as: "X;Y".
+Run `python3 manage.py collectstatic --no-input`
 
-Please read the "Configure" chapter to set the `allow_coordinates_saving` option to True.
-You might also set the `always_save_coordinates` option to True.
+Clear you browser cache.
 
 ## Configure
 
+### Individual Options
+
 All individual options can be assigned a default value per user directly in the plugin. The default value can be overridden on the filter page.
 
+![Individual Options](doc/img/topology_individual_options.png)
+
 The remaining options must be configured in the `PLUGINS_CONFIG` section of your `netbox/configuration.py`.
 
 Example:
 ```
 PLUGINS_CONFIG = {
     'netbox_topology_views': {
         'static_image_directory': 'netbox_topology_views/img',
@@ -97,73 +104,113 @@
     }
 }
 ```
 
 | Setting                  | Default value                                                                                                                                  | Description                                                                                                            |
 | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
 | static_image_directory   | netbox_topology_views/img                                                                                                                      | (str or pathlib.Path) Specifies the location that images will be loaded from by default. Must be within `STATIC_ROOT`  |
-| allow_coordinates_saving | False                                                                                                                                          | (bool) Set to true if you use the custom coordinates fields and want to save the coordinates                           |
-| always_save_coordinates  | False                                                                                                                                          | (bool) Set if you want to enable the option to save coordinates by default                                             |
+| allow_coordinates_saving | False                                                                                                                                          | (bool) Set to true if you want to enable the ability to save the coordinates.                           |
+| always_save_coordinates  | False                                                                                                                                          | (bool) Set if you want to enable the option to save coordinates by default. Setting allow_coordinates_saving to true is mandatory.                                             |
+
+### Custom field: coordinates
+
+There is also support for custom fields.
+
+>**_Note:_** The custom field "coordinates" is deprecated and will be removed in the future. Please use Coordinate Groups instead.
+
+If you create a custom field "coordinates" for "dcim > device" and "Circuits > circuit" with type "text" and name "coordinates" you will see the same layout every time. It is recommended to set this field to "UI visibility" "Hidden" and let the plugin manage it in the background.
+
+The coordinates are stored as: "X;Y".
+
+> Please read the "Configure" chapter to set the `allow_coordinates_saving` option to True.
+You might also set the `always_save_coordinates` option to True.
+
+### Convert custom field to Coordinate Groups
+
+Please note that values stored in the custom field "coordinates" are not being converted to Coordinate Groups automatically. A pragmatic way to do this conversion yourself is as follows:
++ Navigate to "Topology" > "Filters".
++ Select "Show Unconnected" and "Show Cables". 
++ Leave all other filter settings alone. We want all entries to be displayed!
++ Click "Search" and wait for the results to be displayed
++ Select all nodes. This can be done by holding down the Shift key and dragging a frame around all icons with the left mouse button.
++ Drag the selection a tiny bit to the side. This causes all coordinates for all devices to be stored in the "default" group.
+> **_Hint_**: Don't wait too long after clicking an icon in order to drag. If you hold the mouse button for too long before dragging starts, the selection is reset._
++ Storing the values might take some time, depending on the number of devices. Please be patient and check "Coordinates" in order to make sure that everthing has been stored.
++ It is save to delete the custom field now.
 
 ### Custom Images
 
-To change image with associated device use the `Images` page - it allows to map a device role with an image found in the netbox static directory (defined by the plugin config `static_image_directory` which defaults to `netbox_topology_views/img`). You can also upload you own custom images to there - these images will automatically be used for a device (if it does not already have a specified image in the settings) if their name is the device role slug.
+To change image with associated device use the `Images` page - it allows to map a device role with an image found in the NetBox static directory (defined by the plugin config `static_image_directory` which defaults to `netbox_topology_views/img`). You can also upload you own custom images to there - these images will automatically be used for a device (if it does not already have a specified image in the settings) if their name is the device role slug.
+
+![Images](doc/img/topology_images.png)
 
 ## Use
 
 Go to the plugins tab in the navbar and click topology or go to `$NETBOX_URL/plugins/netbox_topology_views/` to view your topologies
 
 Select your options for the topology view:
 
-![topology_options](https://user-images.githubusercontent.com/20901110/235302073-234c3ef7-2c2b-4d0c-a674-9909d490d7ea.png)
+![Filter Options](doc/img/topology_filter_options.png)
 
 <dl>
+    <dt>Coordinate Group</dt>
+    <dd>Select Coordinate Group. These groups allow devices to be displayed in different positions depending on the group, thus providing different representations for the same topology. If nothing is selected, the group "default" is set automatically.</dd>
     <dt>Save Coordinates</dt>
     <dd>Save the coordinates of devices in the topology view.</dd>
     <dt>Show Unconnected</dt>
     <dd>Show devices that have no connections or for which no connection is displayed. This option depends on other parameters like 'Show Cables' and 'Show Logical Connections'.</dd>
     <dt>Show Cables</dt>
     <dd>Show connections between interfaces, front / rear ports, etc., that are connected with one or more cables. These connections are displayed as solid lines in the color of the cable.</dd> 
     <dt>Show Logical Connections</dt>
     <dd>Show logical connections between interfaces (referred to as Interface Connections in NetBox) in the topology view. Where the path between
         interfaces includes multiple cables (e.g., via patch panels), only the end interface connections are shown, not the 
         intermediate front / rear port connections, etc. This is similar to what was referred to as 'end-to-end' connections in previous versions. These connections are displayed as yellow dotted lines.</dd>
-    <dt>Show redundant Cable and Locigal Connection</dt>
+    <dt>Show redundant Cable and Logical Connection</dt>
     <dd>Shows a logical connection (in addition to a cable), even if a cable is directly connected. Leaving this option disabled prevents that redundant display. This option only has an effect if 'Show Logical Connections' is activated.</dd>
     <dt>Show Neighbors</dt>
     <dd>Adds neighbors to the filter result set automatically. Link peers will be added if 'Show Cables' is ticked, far-end terminations will be added if 'Show Logical Connections' is ticked.</dd>
     <dt>Show Circuit Terminations</dt>
     <dd>Show connections which end at a circuit termination in the topology view. These connections are displayed as blue dashed lines.</dd>
     <dt>Show Power Feeds</dt>
     <dd>Displays connections between power outlets and power ports. These connections are displayed as solid lines in the color of the cable. This option depends on 'Show Cables'.</dd>
     <dt>Show Wireless Links</dt>
     <dd>Displays wireless connections. These connections are displayed as blue dotted lines.</dd>
 </dl>
     
-### Update
+### Coordinates and Coordinate Groups
 
-Run `pip install netbox-topology-views --upgrade` in your venv.
+Netbox Topology Views stores the position of the devices. In order to allow different representations for the topology, Coordinate Groups are supported.
 
-Run `python3 manage.py migrate netbox_topology_views`
+> Please read the "Configure" chapter to set the `allow_coordinates_saving` option to True.
+You might also set the `always_save_coordinates` option to True.
 
-Run `python3 manage.py collectstatic --no-input`
+Navigate to "Coordinate Groups" in the menu and create as many groups as you like. You can select a group later in the filter pane in order to show icon positions according to this group (see chapter "Use"). You can also omit creating a group if you don't need this feature. Netbox Topology Views automatically creates a group named "default" for you and stores all coordinates in this group, even if you do not select a group in the filter.
 
+By default, the position of the devices are calculated with a physics engine. As soon as a device icon is dragged to another location, its position is saved and excluded from the calculation by the physics engine. All saved coordinates can be viewed and edited under the menu item "Coordinates".
 
-Clear you browser cache.
-
+> **_Note:_** At the time of writing, it is not possible to store the positions of circuit terminations, power panels and power feeds, as these are not devices.
 
 ### Permissions
 
 To view `/plugins/netbox_topology-views/topology` you need the following permissions:
  + dcim | device | can view device
  + dcim | site | can view site
  + extras | tag | can view tag
  + dcim | device role | can view device role
 
-To view `/plugins/netbox_topology-views/image`:
+To save `Coordinates` when moving icons:
+ + netbox_topology_views | coordinate | change
+
+To view `/plugins/netbox_topology-views/images`:
  + dcim | site | view
  + dcim | device role | view
  + dcim | device role | add
  + dcim | device role | change
 
- To view `/plugins/netbox_topology-views/individualoptions`:
- + netbox topology views | individualoptions | change
+To view `/plugins/netbox_topology-views/individualoptions`:
+ + netbox_topology_views | individual options | change
+
+Set `Coordinate Groups` according to your needs:
+ + netbox_topology_views | coordinate groups | view/add/change/delete
+
+Set `Coordinates` according to your needs:
+ + netbox_topology_views | coordinate | view/add/change/delete
```

### Comparing `netbox-topology-views-3.5.0/netbox_topology_views.egg-info/SOURCES.txt` & `netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 README.md
 setup.py
 netbox_topology_views/__init__.py
 netbox_topology_views/filters.py
 netbox_topology_views/forms.py
 netbox_topology_views/models.py
 netbox_topology_views/navigation.py
+netbox_topology_views/search.py
 netbox_topology_views/signals.py
+netbox_topology_views/tables.py
 netbox_topology_views/template_content.py
 netbox_topology_views/urls.py
 netbox_topology_views/utils.py
 netbox_topology_views/views.py
 netbox_topology_views.egg-info/PKG-INFO
 netbox_topology_views.egg-info/SOURCES.txt
 netbox_topology_views.egg-info/dependency_links.txt
@@ -19,14 +21,16 @@
 netbox_topology_views/api/__init__.py
 netbox_topology_views/api/serializers.py
 netbox_topology_views/api/urls.py
 netbox_topology_views/api/views.py
 netbox_topology_views/migrations/0001_initial.py
 netbox_topology_views/migrations/0002_individualoptions.py
 netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
+netbox_topology_views/migrations/0004_coordinategroup_coordinate.py
+netbox_topology_views/migrations/0005_individualoptions_save_coords.py
 netbox_topology_views/migrations/__init__.py
 netbox_topology_views/static/netbox_topology_views/css/app.css
 netbox_topology_views/static/netbox_topology_views/css/vendor.css
 netbox_topology_views/static/netbox_topology_views/img/LICENSE
 netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
 netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
 netbox_topology_views/static/netbox_topology_views/img/backup.svg
@@ -74,13 +78,22 @@
 netbox_topology_views/static/netbox_topology_views/img/ups.svg
 netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
 netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
 netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
 netbox_topology_views/static/netbox_topology_views/js/app.js
 netbox_topology_views/static/netbox_topology_views/js/images.js
 netbox_topology_views/static/netbox_topology_views/js/images.js.map
+netbox_topology_views/templates/netbox_topology_views/coordinate.html
+netbox_topology_views/templates/netbox_topology_views/coordinate_add.html
+netbox_topology_views/templates/netbox_topology_views/coordinate_edit.html
+netbox_topology_views/templates/netbox_topology_views/coordinate_list.html
+netbox_topology_views/templates/netbox_topology_views/coordinategroup.html
+netbox_topology_views/templates/netbox_topology_views/coordinategroup_add.html
+netbox_topology_views/templates/netbox_topology_views/coordinategroup_edit.html
+netbox_topology_views/templates/netbox_topology_views/coordinategroup_list.html
 netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
 netbox_topology_views/templates/netbox_topology_views/images.html
 netbox_topology_views/templates/netbox_topology_views/index.html
 netbox_topology_views/templates/netbox_topology_views/individual_options.html
+netbox_topology_views/templates/netbox_topology_views/location_button.html
 netbox_topology_views/templates/netbox_topology_views/site_button.html
 netbox_topology_views/templates/netbox_topology_views/toasts.html
```

### Comparing `netbox-topology-views-3.5.0/setup.py` & `netbox-topology-views-3.6.0b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 readme = Path(__file__).parent / "README.md"
 long_description = readme.read_text()
 
 setup(
     name="netbox-topology-views",
-    version="3.5.0",
+    version="3.6.0-beta.1",
     description="An NetBox plugin to create Topology maps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mattieserver/netbox-topology-views",
     author="Mattijs Vanhaverbeke",
     license="Apache 2.0",
     install_requires=[],
```

