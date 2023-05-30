# Comparing `tmp/docker_compose_parser-0.0.17-py3-none-any.whl.zip` & `tmp/docker_compose_parser-0.0.18-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3893 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-May-09 17:50 docker_compose_parser/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 23-May-09 17:50 docker_compose_parser/file_models.py
--rw-r--r--  2.0 unx      452 b- defN 23-May-09 17:50 docker_compose_parser-0.0.17.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 17:50 docker_compose_parser-0.0.17.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-09 17:50 docker_compose_parser-0.0.17.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       22 b- defN 23-May-09 17:50 docker_compose_parser-0.0.17.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      652 b- defN 23-May-09 17:50 docker_compose_parser-0.0.17.dist-info/RECORD
-7 files, 7965 bytes uncompressed, 2703 bytes compressed:  66.1%
+Zip file size: 3908 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-May-30 12:37 docker_compose_parser/__init__.py
+-rw-r--r--  2.0 unx     6879 b- defN 23-May-30 12:37 docker_compose_parser/file_models.py
+-rw-r--r--  2.0 unx      452 b- defN 23-May-30 12:37 docker_compose_parser-0.0.18.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 12:37 docker_compose_parser-0.0.18.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-30 12:37 docker_compose_parser-0.0.18.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-May-30 12:37 docker_compose_parser-0.0.18.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      652 b- defN 23-May-30 12:37 docker_compose_parser-0.0.18.dist-info/RECORD
+7 files, 8098 bytes uncompressed, 2718 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: docker_compose_parser/__init__.py
 Comment: 
 
 Filename: docker_compose_parser/file_models.py
 Comment: 
 
-Filename: docker_compose_parser-0.0.17.dist-info/METADATA
+Filename: docker_compose_parser-0.0.18.dist-info/METADATA
 Comment: 
 
-Filename: docker_compose_parser-0.0.17.dist-info/WHEEL
+Filename: docker_compose_parser-0.0.18.dist-info/WHEEL
 Comment: 
 
-Filename: docker_compose_parser-0.0.17.dist-info/namespace_packages.txt
+Filename: docker_compose_parser-0.0.18.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: docker_compose_parser-0.0.17.dist-info/top_level.txt
+Filename: docker_compose_parser-0.0.18.dist-info/top_level.txt
 Comment: 
 
-Filename: docker_compose_parser-0.0.17.dist-info/RECORD
+Filename: docker_compose_parser-0.0.18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docker_compose_parser/file_models.py

```diff
@@ -109,15 +109,16 @@
             raise TypeError
         return other.depends_on(self.name) or self.index < other.index
 
 
 def iter_sorted_services(compose_payload: str | Path) -> list[tuple[str, dict]]:
     """`depends_on` if used if it exists, otherwise services are sorted by
     their order in the file."""
-    parsed: dict = parse_payload(compose_payload, FileFormat.yaml)
+    parsed = parse_payload(compose_payload, FileFormat.yaml)
+    assert isinstance(parsed, dict)
     services: dict = parsed["services"]
     services_sorted = sorted(
         _NameDict(name, d, i) for i, (name, d) in enumerate(services.items())
     )
     return [(service.name, service.service_dict) for service in services_sorted]
 
 
@@ -126,30 +127,30 @@
     image = read_nested_or_none(parsed, f"services.{service_name}.image")
     labels = read_nested_or_none(parsed, f"services.{service_name}.labels") or {}
     env = read_nested_or_none(parsed, f"services.{service_name}.environment") or {}
     ports = read_nested_or_none(parsed, f"services.{service_name}.ports") or []
     command = read_nested_or_none(parsed, f"services.{service_name}.command") or []
     volumes = read_nested_or_none(parsed, f"services.{service_name}.volumes") or []
     return ComposeServiceInfo(
-        image=image,
-        labels=labels,
-        default_env=env,
-        default_ports=ports,
-        command=command,
-        default_volumes=volumes,
+        image=image,  # type: ignore
+        labels=labels,  # type: ignore
+        default_env=env,  # type: ignore
+        default_ports=ports,  # type: ignore
+        command=command,  # type: ignore
+        default_volumes=volumes,  # type: ignore
     )
 
 
 def export_compose_dict(
     service_dict: dict,
     service_name: str,
     env_overrides: Optional[Dict[str, str]] = None,
     network_name: str | None = NETWORK_NAME_DEFAULT,
     volumes: Optional[List[str]] = None,
-    add_labels: Dict[str, str] = None,
+    add_labels: Dict[str, str] | None = None,
     command: Optional[List[str]] = None,
     only_override_existing_env_vars: bool = True,
     network_external: bool = True,
 ) -> dict:
     """Valid dictionary for a docker-compose.yaml file."""
     service_dict.pop("depends_on", "")
     if network_name:
```

