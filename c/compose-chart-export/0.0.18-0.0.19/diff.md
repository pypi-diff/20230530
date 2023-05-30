# Comparing `tmp/compose_chart_export-0.0.18-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13241 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-May-11 13:03 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2534 b- defN 23-May-11 13:03 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    14424 b- defN 23-May-11 13:03 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4967 b- defN 23-May-11 13:03 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2211 b- defN 23-May-11 13:03 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     9544 b- defN 23-May-11 13:03 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2359 b- defN 23-May-11 13:03 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-May-11 13:03 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      583 b- defN 23-May-11 13:03 compose_chart_export-0.0.18.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-11 13:03 compose_chart_export-0.0.18.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-11 13:03 compose_chart_export-0.0.18.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-11 13:03 compose_chart_export-0.0.18.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1199 b- defN 23-May-11 13:03 compose_chart_export-0.0.18.dist-info/RECORD
-13 files, 38126 bytes uncompressed, 11185 bytes compressed:  70.7%
+Zip file size: 13357 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-May-30 12:37 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2448 b- defN 23-May-30 12:37 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    14564 b- defN 23-May-30 12:37 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4974 b- defN 23-May-30 12:37 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2285 b- defN 23-May-30 12:37 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     9604 b- defN 23-May-30 12:37 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2365 b- defN 23-May-30 12:37 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-May-30 12:37 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      626 b- defN 23-May-30 12:37 compose_chart_export-0.0.19.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 12:37 compose_chart_export-0.0.19.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-30 12:37 compose_chart_export-0.0.19.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-30 12:37 compose_chart_export-0.0.19.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1199 b- defN 23-May-30 12:37 compose_chart_export-0.0.19.dist-info/RECORD
+13 files, 38370 bytes uncompressed, 11301 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.18.dist-info/METADATA
+Filename: compose_chart_export-0.0.19.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.18.dist-info/WHEEL
+Filename: compose_chart_export-0.0.19.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.18.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.19.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.18.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.19.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.18.dist-info/RECORD
+Filename: compose_chart_export-0.0.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## compose_chart_export/chart_export.py

```diff
@@ -38,45 +38,39 @@
 SERVICE_DEPLOYMENT = "service_deployment"
 DEPLOYMENT_ONLY = "deployment_only"
 DAEMONSET = "daemonset"
 
 
 def _export_chart(
     spec: ChartTemplateSpec,
-    chart_path: Optional[Path] = None,
+    chart_path: Path,
     skip_generators: Optional[List[str]] = None,
 ) -> Path:
     clean_dir(chart_path)
     skip_generators = skip_generators or []
     for rel_path, content_generator in PATH_TO_GENERATORS.items():
         if rel_path in skip_generators:
             continue
         dest = chart_path / rel_path
         if content := content_generator(spec):
             ensure_parents_write_text(dest, content)
     return chart_path
 
 
-def export_service_deployment(
-    spec: ChartTemplateSpec, chart_path: Optional[Path] = None
-) -> Path:
+def export_service_deployment(spec: ChartTemplateSpec, chart_path: Path) -> Path:
     return _export_chart(spec, chart_path, skip_generators=[daemonset_path])
 
 
-def export_deployment_only(
-    spec: ChartTemplateSpec, chart_path: Optional[Path] = None
-) -> Path:
+def export_deployment_only(spec: ChartTemplateSpec, chart_path: Path) -> Path:
     return _export_chart(
         spec, chart_path, skip_generators=[service_path, daemonset_path]
     )
 
 
-def export_daemonset(
-    spec: ChartTemplateSpec, chart_path: Optional[Path] = None
-) -> Path:
+def export_daemonset(spec: ChartTemplateSpec, chart_path: Path) -> Path:
     return _export_chart(
         spec, chart_path, skip_generators=[service_path, deployment_path]
     )
 
 
 def export_chart(spec: ChartTemplateSpec, template_name: str, chart_path: Path) -> None:
     export = globals().get(f"export_{template_name}")
```

## compose_chart_export/chart_file_templates.py

```diff
@@ -1,14 +1,15 @@
 # flake8: noqa
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Dict, List, Tuple
+from typing import Dict, List, Tuple, cast
 
 from model_lib.serialize.yaml_serialize import edit_helm_template
 from pydantic import Field, constr, validator
+from typing_extensions import TypeAlias
 from zero_3rdparty.enum_utils import StrEnum
 
 from model_lib import Event
 
 
 class ReplaceStr(StrEnum):
     APP_NAME = "APP_NAME"
@@ -26,18 +27,18 @@
 version: {ReplaceStr.CHART_VERSION}
 appVersion: {ReplaceStr.APP_VERSION}
 """
 
 
 # start with number or character ". -_" allowed, + and / not allowed
 # https://atomist.github.io/sdm-pack-k8s/modules/_lib_kubernetes_labels_.html
-kubernetes_label_regex = constr(
-    regex=r"^([a-zA-Z0-9][-a-zA-Z0-9_\.]*[a-zA-Z0-9])?$", max_length=63
+kubernetes_label_regex: TypeAlias = cast(
+    str, constr(regex=r"^([a-zA-Z0-9][-a-zA-Z0-9_\.]*[a-zA-Z0-9])?$", max_length=63)
 )
-dns_safe = constr(regex=r"^[a-z-]+$")
+dns_safe: TypeAlias = cast(str, constr(regex=r"^[a-z-]+$"))
 
 
 class TemplateReplacements(Event):
     """
     >>> TemplateReplacements(REPO_NAME="py-hooks", REPO_OWNER="wheelme-devops", CHART_VERSION="0.0.1")
     TemplateReplacements(APP_VERSION='', CHART_VERSION='0.0.1', REPO_NAME='py-hooks', REPO_OWNER='wheelme-devops', APP_NAME='py-hooks')
     >>> TemplateReplacements(REPO_NAME="py-hooks._ok", REPO_OWNER="wheelme-devops", CHART_VERSION="0.0.1")
@@ -324,15 +325,17 @@
                     resources="{{- toYaml .Values.resources | nindent 10 }}"
                     if spec.use_resource_limits
                     else {},
                     ports=[],  # override by artifacts plugin
                     # command=[],  # override by artifacts plugin
                     env=[],  # override by artifacts plugin
                 )
-                volume_mounts: list = container_spec.setdefault("volumeMounts", [])
+                volume_mounts: list = cast(
+                    list, container_spec.setdefault("volumeMounts", [])
+                )
                 if volumes := spec.container_host_path_volumes.get(name):
                     volume_mounts.extend(
                         dict(name=mount.name, mountPath=mount.container_path)
                         for mount in volumes
                     )
                 if pv_volumes := spec.persistence_volumes:
                     volume_mounts.extend(
```

## compose_chart_export/chart_mods.py

```diff
@@ -123,12 +123,12 @@
     if not service_path.exists():
         raise Exception(f"No service yaml found in chart: {chart_dir}")
     with edit_helm_template(service_path, yaml_path="spec.ports") as svc_ports:
         assert isinstance(svc_ports, list)
         not_found: Dict[int, PrefixPort] = {port.port: port for port in ports}
         for i, port_dict in enumerate(deepcopy(svc_ports)):
             port_number: int = port_dict.get("port")
-            new: PrefixPort = not_found.pop(port_number, None)
+            new: PrefixPort | None = not_found.pop(port_number, None)
             if new:
                 svc_ports[i] = port_name(new, container_name, "port")
         for port_prefix in not_found.values():
             svc_ports.append(port_name(port_prefix, container_name, "port"))
```

## compose_chart_export/chart_read.py

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from pathlib import Path
-from typing import Any
+from typing import Any, cast
 
 from model_lib.serialize.yaml_serialize import edit_helm_template, edit_yaml
 
 from model_lib import parse_payload
 
 
 def target_name_underscore(name: str) -> str:
@@ -21,20 +21,20 @@
         rel_path = f"templates/{filename}"
         if (chart_path / rel_path).exists():
             break
     assert rel_path, f"no env_template_file found in {chart_path}/templates"
     return rel_path
 
 
-def read_chart_version(path: Path):
-    return parse_payload(path / "Chart.yaml")["version"]
+def read_chart_version(path: Path) -> str:
+    return parse_payload(path / "Chart.yaml")["version"]  # type: ignore
 
 
-def read_app_version(path: Path):
-    return parse_payload(path / "Chart.yaml")["appVersion"]
+def read_app_version(path: Path) -> str:
+    return parse_payload(path / "Chart.yaml")["appVersion"]  # type: ignore
 
 
 def set_chart_version(chart: Path, version: str, app_version: str = ""):
     with edit_yaml(chart / "Chart.yaml") as chart_yaml:
         chart_yaml["version"] = version
         if app_version:
             chart_yaml["appVersion"] = app_version
@@ -44,15 +44,15 @@
     template_rel_path = container_template(chart_path)
     new = (chart_path / template_rel_path).read_text().strip()
     old = (online_chart_path / template_rel_path).read_text().strip()
     return old == new
 
 
 def read_values(chart_path: Path) -> dict[str, Any]:
-    return parse_payload(chart_path / "values.yaml")
+    return cast(dict[str, Any], parse_payload(chart_path / "values.yaml"))
 
 
 def read_env_vars(chart_path: Path, target_name: str) -> dict[str, str]:
     chart_values = read_values(chart_path)
     key = target_name_underscore(target_name)
     return chart_values[key]
```

## compose_chart_export/compose_export.py

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Callable, Iterable
+from typing import Callable, Iterable, cast
 
-import semver
+import semver  # type: ignore
 from compose_chart_export.chart_export import export_chart
 from compose_chart_export.chart_file_templates import (
     ChartTemplateSpec,
     HostPathContainerPath,
     PersistentVolume,
     TemplateReplacements,
     kubernetes_label_regex,
@@ -237,21 +237,22 @@
     chart_name: str,
     container_name: str,
     chart_version: str,
     service_name: str,
     info: ComposeServiceInfo,
 ) -> tuple[str, ChartTemplateSpec]:
     compose_labels = info.labels
-    template_name = parse_template_name(compose_labels)
     ports = list(info.host_container_ports)
-    if ports:
-        template_name = template_name or ChartTemplate.SERVICE_DEPLOYMENT
+    if name := parse_template_name(compose_labels):
+        template_name = cast(ChartTemplate, name)
+    elif ports:
+        template_name = ChartTemplate.SERVICE_DEPLOYMENT
     else:
-        logger.info(f"no ports for {service_name}")
-        template_name = template_name or ChartTemplate.DEPLOYMENT_ONLY
+        template_name = ChartTemplate.DEPLOYMENT_ONLY
+    logger.info(f"using template name: {template_name} for {service_name}")
     target_volumes = parse_target_volumes(compose_labels)
     persistent_volumes = parse_persistent_volumes(compose_labels)
     use_resource_limits = parse_use_resource_limits(compose_labels)
     repo_name = parse_repo_name(compose_labels) or container_name
     repo_owner = parse_repo_owner(compose_labels) or "unknown"
     service_account_name = parse_service_account_name(compose_labels)
     return template_name, ChartTemplateSpec(
```

## compose_chart_export/ports.py

```diff
@@ -62,15 +62,15 @@
     @classmethod
     def as_kub_port_name(cls, value: PrefixPort):
         protocol = value.protocol
         prefix = value.prefix
         return cls.as_kub_port_name_raw(protocol, prefix)
 
     @classmethod
-    def as_kub_port_name_raw(cls, protocol: PortProtocol, prefix: str):
+    def as_kub_port_name_raw(cls, protocol: PortProtocol | str, prefix: str):
         protocol_with_underscore = protocol.replace("-", "_")
         prefix = prefix.replace(protocol_with_underscore, "")
         if prefix == "/":
             prefix = "root"
         elif prefix.startswith("/"):
             prefix = prefix.lstrip("/")
         parts = [part for part in prefix.split("_") if part]
```

## Comparing `compose_chart_export-0.0.18.dist-info/METADATA` & `compose_chart_export-0.0.19.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.18
+Version: 0.0.19
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
-Requires-Dist: docker-compose-parser (==0.0.17)
-Requires-Dist: model-lib (==0.0.17)
+Requires-Dist: docker-compose-parser (==0.0.18)
+Requires-Dist: model-lib (==0.0.18)
 Requires-Dist: pydantic (>=1.10.2)
 Requires-Dist: semver (==2.13.0)
-Requires-Dist: zero-3rdparty (==0.0.17)
+Requires-Dist: typing-extensions (>=4.3.0)
+Requires-Dist: zero-3rdparty (==0.0.18)
 
 # Compose Chart Export
 - Uses `docker-compose.yaml` to generate a helm chart
 - Supports various customizations using labels
```

## Comparing `compose_chart_export-0.0.18.dist-info/RECORD` & `compose_chart_export-0.0.19.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 compose_chart_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-compose_chart_export/chart_export.py,sha256=oDgolV_QNeF12D2xh2D9xhn45IQSbKDMmj2WRZ2UTaI,2534
-compose_chart_export/chart_file_templates.py,sha256=_bAhDNMUfbV4pBMb9WlVN-8XOS0urLF7HuFee4Sd798,14424
-compose_chart_export/chart_mods.py,sha256=Zn-NSYhv7jJfUtGs6V--fquIolVqFT3bwL8mSWrwgOI,4967
-compose_chart_export/chart_read.py,sha256=chwkPcucA6dLWStADbP2kpAGNbhYVMms9zmPjNIQrLs,2211
-compose_chart_export/compose_export.py,sha256=bExlBsswEkLbbt21NGC0B5QEzPPX-VjN6L92gdmDnPM,9544
-compose_chart_export/ports.py,sha256=06WBSFYTUEPUYh9x4U5BjjUeE-EPNCs1Pot6MO7zxD4,2359
+compose_chart_export/chart_export.py,sha256=tg2QiDVn29_Uic_3WPKWkaAhMMN3HQ6jALSG8-Lfv-s,2448
+compose_chart_export/chart_file_templates.py,sha256=sQMgnbhaCgppTOO5XZD72YbshNJS90INvCENukeNY3w,14564
+compose_chart_export/chart_mods.py,sha256=6eaO7tuccQWcZDc_yoi3p7aIOO2YQ4vAb2aqKZ5qBzc,4974
+compose_chart_export/chart_read.py,sha256=5A7mcFdq1lnD7fitj5-evHE9A0zJ6aAlY0KEYPmeRZo,2285
+compose_chart_export/compose_export.py,sha256=zCMO0r4-9ZwaVPNmcadu6F5lvzF0wMP7Hb_7PZ8tLZI,9604
+compose_chart_export/ports.py,sha256=ubPaqe31gwDqPj8s4Bd6pZf8qB02hylpoQpYpbFkYwc,2365
 compose_chart_export/settings.py,sha256=-vo5OY1ttQUeGQwihuX2YTD-qHRgvBdMuRwP_BelWQY,191
-compose_chart_export-0.0.18.dist-info/METADATA,sha256=Yks01r0gqhwxu33RNWMbJZ74Ggf3ehXgpJBOoFGfULw,583
-compose_chart_export-0.0.18.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-compose_chart_export-0.0.18.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-compose_chart_export-0.0.18.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
-compose_chart_export-0.0.18.dist-info/RECORD,,
+compose_chart_export-0.0.19.dist-info/METADATA,sha256=OcL4cu7dYQGY2yhneG4qyYKdARwVZzRqJpD7OnrINuc,626
+compose_chart_export-0.0.19.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+compose_chart_export-0.0.19.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+compose_chart_export-0.0.19.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
+compose_chart_export-0.0.19.dist-info/RECORD,,
```

