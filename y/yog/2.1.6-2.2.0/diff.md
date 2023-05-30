# Comparing `tmp/yog-2.1.6.tar.gz` & `tmp/yog-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yog-2.1.6.tar", max compression
+gzip compressed data, was "yog-2.2.0.tar", max compression
```

## Comparing `yog-2.1.6.tar` & `yog-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.1.6/README.md
--rw-r--r--   0        0        0      541 2023-05-01 02:05:05.613161 yog-2.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.1.6/yog/__init__.py
--rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.1.6/yog/command.py
--rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.1.6/yog/git_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.1.6/yog/host/__init__.py
--rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.1.6/yog/host/docker_attrs.py
--rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.1.6/yog/host/main.py
--rw-r--r--   0        0        0     7453 2023-05-01 02:04:55.579539 yog-2.1.6/yog/host/manage.py
--rw-r--r--   0        0        0     8557 2023-04-17 17:47:42.812155 yog-2.1.6/yog/host/necronomicon.py
--rw-r--r--   0        0        0    11317 2023-02-22 22:13:28.278626 yog-2.1.6/yog/host/pki.py
--rw-r--r--   0        0        0      492 2023-02-22 04:11:12.414451 yog-2.1.6/yog/host/pki_model.py
--rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.1.6/yog/host/test_docker_attrs.py
--rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.1.6/yog/logging_utils.py
--rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.1.6/yog/model_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.1.6/yog/repo/__init__.py
--rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.1.6/yog/repo/main.py
--rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.1.6/yog/res/__init__.py
--rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.1.6/yog/res/cas.yml
--rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.1.6/yog/res/docker_test.yml
--rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.1.6/yog/res/sample_necronomicon.yml
--rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.1.6/yog/res/sample_needs_tunnel_back.yml
--rw-r--r--   0        0        0      185 2023-02-22 04:11:12.414451 yog-2.1.6/yog/res/sample_pki_necronomicon.yml
--rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.1.6/yog/res/sample_site_necronomicon.yml
--rw-r--r--   0        0        0    10283 2023-02-22 04:11:12.414451 yog-2.1.6/yog/ssh_utils.py
--rw-r--r--   0        0        0    11384 2023-05-01 02:06:23.207026 yog-2.1.6/setup.py
--rw-r--r--   0        0        0    10753 2023-05-01 02:06:23.207974 yog-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.2.0/README.md
+-rw-r--r--   0        0        0      541 2023-05-30 01:28:33.283278 yog-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.2.0/yog/__init__.py
+-rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.2.0/yog/command.py
+-rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.2.0/yog/git_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.2.0/yog/host/__init__.py
+-rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.2.0/yog/host/docker_attrs.py
+-rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.2.0/yog/host/main.py
+-rw-r--r--   0        0        0     7454 2023-05-30 01:28:33.283278 yog-2.2.0/yog/host/manage.py
+-rw-r--r--   0        0        0     8791 2023-05-30 01:28:33.283278 yog-2.2.0/yog/host/necronomicon.py
+-rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.283278 yog-2.2.0/yog/host/os_utils.py
+-rw-r--r--   0        0        0    12621 2023-05-30 01:28:33.283278 yog-2.2.0/yog/host/pki.py
+-rw-r--r--   0        0        0      775 2023-05-30 01:28:33.283278 yog-2.2.0/yog/host/pki_model.py
+-rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.2.0/yog/host/test_docker_attrs.py
+-rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.2.0/yog/logging_utils.py
+-rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.2.0/yog/model_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.2.0/yog/repo/__init__.py
+-rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.2.0/yog/repo/main.py
+-rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.2.0/yog/res/__init__.py
+-rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.2.0/yog/res/cas.yml
+-rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.2.0/yog/res/docker_test.yml
+-rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.2.0/yog/res/sample_necronomicon.yml
+-rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.2.0/yog/res/sample_needs_tunnel_back.yml
+-rw-r--r--   0        0        0      185 2023-02-22 04:11:12.414451 yog-2.2.0/yog/res/sample_pki_necronomicon.yml
+-rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.2.0/yog/res/sample_site_necronomicon.yml
+-rw-r--r--   0        0        0    11024 2023-05-30 01:28:33.283278 yog-2.2.0/yog/ssh_utils.py
+-rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.0/PKG-INFO
```

### Comparing `yog-2.1.6/README.md` & `yog-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `yog-2.1.6/pyproject.toml` & `yog-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yog"
-version = "2.1.6"
+version = "2.2.0"
 description = "The Gate and Key"
 authors = ["Josh Hertlein <jmhertlein@gmail.com>"]
 license = "AGPLv3"
 readme = "README.md"
 
 [tool.poetry.scripts]
 yog = "yog.host.main:main"
```

### Comparing `yog-2.1.6/yog/git_utils.py` & `yog-2.2.0/yog/git_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.6/yog/host/docker_attrs.py` & `yog-2.2.0/yog/host/docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.6/yog/host/manage.py` & `yog-2.2.0/yog/host/manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,13 +184,14 @@
             if f.root:
                 cmd_prefix = "sudo "
             else:
                 cmd_prefix = ""
 
             check_call(ssh, f"{cmd_prefix}mkdir -p \"{dirname(f.dest)}\"")
             check_call(ssh, f"{cmd_prefix}bash -c 'cat - > \"{f.dest}\"'", send_stdin=content)
+
     for c in hupcmds:
         log.info(f"[{host}][files][hup]: {c}")
         check_call(ssh, c)
```

### Comparing `yog-2.1.6/yog/host/necronomicon.py` & `yog-2.2.0/yog/host/necronomicon.py`

 * *Files 6% similar despite different names*

```diff
@@ -257,26 +257,32 @@
 
 class NeededTunnelsSection(t.NamedTuple):
     tunnels: t.List[NeededTunnel]
 
 
 class CertEntry(t.NamedTuple):
     storage: str
-    validity_years: int
-    refresh_at: int
+    validity_period: str
+    refresh_at_period: str
     names: t.List[str]
     authority: str
+    hupcmd: t.Optional[str]
+    chmod: t.Optional[str]
+    chown: t.Optional[str]
 
     @staticmethod
     def from_parsed(o: t.Any):
         return CertEntry(
             o['storage'],
-            int(o['validity_years']),
-            int(o['refresh_at']),
+            str(o['validity_period']),
+            str(o['refresh_at_period']),
             o['names'],
             o['authority'],
+            o['hupcmd'] if 'hupcmd' in o else None,
+            o['chmod'] if 'chmod' in o else "rw-r--r--",
+            o['chown'] if 'chown' in o else "root:root",
         )
 
+
 class PKI(t.NamedTuple):
     certs: t.List[CertEntry]
-    # authorities: t.List[str]
```

### Comparing `yog-2.1.6/yog/host/pki.py` & `yog-2.2.0/yog/host/pki.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurvePrivateKey
 from cryptography.hazmat.primitives.serialization import load_pem_private_key
 from cryptography.x509 import Certificate, GeneralName
 from cryptography.x509.oid import NameOID
 from paramiko.client import SSHClient
 
 from yog.host.necronomicon import CertEntry, Necronomicon
-from yog.host.pki_model import CAEntry, load_cas
-from yog.model_utils import HostPathStr
-from yog.ssh_utils import mkdirp, cat, exists, put
+from yog.host.os_utils import Perms, Owner, RWXBits
+from yog.host.pki_model import CAEntry, load_cas, parse_validity_period
+from yog.ssh_utils import mkdirp, cat, exists, put, check_call, check_output, stat
 
 log = logging.getLogger(__name__)
 
 class KeyMaterial(t.NamedTuple):
     fname: str
     mattype: str
     body: str
+    owner: t.Optional[Owner]
+    perms: t.Optional[Perms]
 
 
 class KeyPairDataItem(t.NamedTuple):
     field_name: str
     fname: str
     material_type: str
 
@@ -36,14 +38,15 @@
     KeyPairDataItem("private_openssl", "key.pem.openssl", "private"),
     KeyPairDataItem("private_ssh", "key.ssh", "private"),
     KeyPairDataItem("public_pkcs", "key.pem.pkcs1.public", "public"),
     KeyPairDataItem("public_ssh", "key.ssh.public", "public"),
     KeyPairDataItem("certificate", "key.crt", "cert"),
 ]
 
+
 class KeyPairData(t.NamedTuple):
     serial: uuid.UUID
     issuer_serial: uuid.UUID
     private_ssh: KeyMaterial
     private_openssl: KeyMaterial
 
     public_pkcs: KeyMaterial
@@ -66,19 +69,21 @@
     def cert_names(self) -> t.List[str]:
         e: x509.SubjectAlternativeName = self.crt().extensions.get_extension_for_class(x509.SubjectAlternativeName).value
         return e.get_values_for_type(x509.DNSName)
 
     def issuer_cn(self) -> str:
         return self.crt().issuer.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value
 
-    def write(self, ssh: SSHClient, path: str):
+    def write(self, ssh: SSHClient, path: str, owner: t.Optional[Owner], perms: t.Optional[Perms]):
         mkdirp(ssh, path, "root")
         for km in self.materials():
-            put(ssh, os.path.join(path, km.fname), km.body, "root",
-                mode=("600" if km.mattype == "private" else "644"))
+            put(ssh, os.path.join(path, km.fname), km.body,
+                user=owner.user if owner else None,
+                group=owner.group if owner else None,
+                mode=("600" if km.mattype == "private" else perms.to_chmod_expr() if perms else "644"))
         put(ssh, os.path.join(path, "issuer_serial.txt"), str(self.issuer_serial), "root")
         put(ssh, os.path.join(path, "serial.txt"), str(self.serial), "root")
 
     @staticmethod
     def load(ssh: SSHClient, path: str) -> 'KeyPairData':
         serial_path = os.path.join(path, "serial.txt")
         issuer_serial_path = os.path.join(path, "issuer_serial.txt")
@@ -91,19 +96,19 @@
         args = {}
         for i in KEY_PAIR_DATA_ITEMS:
             if not exists(ssh, os.path.join(path, i.fname)):
                 raise ValueError(f"Unable to load {path} (missing key data)")
             args[i.field_name] = KeyMaterial(
                 i.fname,
                 i.material_type,
-                cat(ssh, os.path.join(path, i.fname), i.material_type == "private")
+                cat(ssh, os.path.join(path, i.fname), i.material_type == "private"),
+                *stat(ssh, os.path.join(path, i.fname))
             )
 
-
-        return KeyPairData(serial, issuer_serial, **args)
+        return KeyPairData(serial, issuer_serial, **args) # TODO these Nones
 
 
 def _gen_ca(ca: CAEntry):
     private_key = ec.generate_private_key(
         curve = ec.SECP384R1(),
         backend=default_backend()
     )
@@ -113,15 +118,15 @@
     builder = builder.subject_name(x509.Name([
         x509.NameAttribute(NameOID.COMMON_NAME, ca.ident),
     ]))
     builder = builder.issuer_name(x509.Name([
         x509.NameAttribute(NameOID.COMMON_NAME, ca.ident),
     ]))
     builder = builder.not_valid_before(datetime.datetime.utcnow())
-    builder = builder.not_valid_after(datetime.datetime.utcnow()+datetime.timedelta(days=365*ca.validity_years))
+    builder = builder.not_valid_after(datetime.datetime.utcnow()+datetime.timedelta(days=ca.validity_days))
     serial_no = uuid.uuid4()
     builder = builder.serial_number(int(serial_no))
     builder = builder.public_key(public_key)
     builder = builder.add_extension(
         x509.BasicConstraints(ca=True, path_length=None), critical=True,
     )
     certificate = builder.sign(
@@ -132,34 +137,34 @@
     material = KeyPairData(
         serial_no,
         serial_no,
         KeyMaterial("key.ssh", "private", private_key.private_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PrivateFormat.OpenSSH,
             encryption_algorithm=serialization.NoEncryption(),
-            ).decode("utf-8")),
+            ).decode("utf-8"), None, None),
         KeyMaterial("key.pem.openssl", "private", private_key.private_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PrivateFormat.TraditionalOpenSSL,
             encryption_algorithm=serialization.NoEncryption(),
-        ).decode("utf-8")),
+        ).decode("utf-8"), None, None),
         KeyMaterial("key.pem.pkcs1.public", "public",
             public_key.public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.SubjectPublicKeyInfo,
-            ).decode("utf-8")),
+            ).decode("utf-8"), None, None),
         KeyMaterial("key.ssh.public", "public",
             public_key.public_bytes(
             encoding=serialization.Encoding.OpenSSH,
             format=serialization.PublicFormat.OpenSSH,
-            ).decode("utf-8")),
+            ).decode("utf-8"), None, None),
         KeyMaterial("key.crt", "cert",
             certificate.public_bytes(
             encoding=serialization.Encoding.PEM,
-            ).decode("utf-8")),
+            ).decode("utf-8"), None, None),
     )
 
     return material
 
 
 def _gen_cert(ce: CertEntry, ca_data: KeyPairData, ca: CAEntry):
     private_key = ec.generate_private_key(
@@ -172,15 +177,15 @@
     builder = builder.subject_name(x509.Name([
         x509.NameAttribute(NameOID.COMMON_NAME, ce.names[0]),
     ]))
     builder = builder.issuer_name(x509.Name([
         x509.NameAttribute(NameOID.COMMON_NAME, ca.ident),
     ]))
     builder = builder.not_valid_before(datetime.datetime.utcnow())
-    builder = builder.not_valid_after(datetime.datetime.utcnow()+datetime.timedelta(days=365*ce.validity_years))
+    builder = builder.not_valid_after(datetime.datetime.utcnow()+datetime.timedelta(days=parse_validity_period(ce.validity_period)))
     serial_no = uuid.uuid4()
     builder = builder.serial_number(int(serial_no))
     builder = builder.public_key(public_key)
     builder = builder.add_extension(
         x509.SubjectAlternativeName([x509.DNSName(n) for n in ce.names]), critical=False
     )
     certificate = builder.sign(
@@ -191,34 +196,34 @@
     material = KeyPairData(
         serial_no,
         ca_data.issuer_serial,
         KeyMaterial("key.ssh", "private", private_key.private_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PrivateFormat.OpenSSH,
             encryption_algorithm=serialization.NoEncryption(),
-        ).decode("utf-8")),
+        ).decode("utf-8"), None, None),
         KeyMaterial("key.pem.openssl", "private", private_key.private_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PrivateFormat.TraditionalOpenSSL,
             encryption_algorithm=serialization.NoEncryption(),
-            ).decode("utf-8")),
+            ).decode("utf-8"), None, None),
         KeyMaterial("key.pem.pkcs1.public", "public",
             public_key.public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.SubjectPublicKeyInfo,
-            ).decode("utf-8")),
+            ).decode("utf-8"), None, None),
         KeyMaterial("key.ssh.public", "public",
             public_key.public_bytes(
             encoding=serialization.Encoding.OpenSSH,
             format=serialization.PublicFormat.OpenSSH,
-            ).decode("utf-8")),
+            ).decode("utf-8"), None, None),
         KeyMaterial("key.crt", "cert",
             certificate.public_bytes(
             encoding=serialization.Encoding.PEM,
-            ).decode("utf-8")),
+            ).decode("utf-8"), None, None),
     )
 
     return material
 
 
 
 
@@ -257,14 +262,16 @@
     cadata = _gen_ca(ca)
     cadata.write(ssh, ca.storage.path)
 
 
 def apply_pki_section(host: str, n: Necronomicon, ssh: SSHClient, root_dir):
     cas = load_cas(os.path.join(root_dir, "cas.yml"))
 
+    hupcmds = set()
+
     for ce in n.pki.certs:
         generate = False
 
         root = [ca for ca in cas if ca.ident == ce.authority]
         if not root:
             raise ValueError(f"No such CA: {ce.authority}")
         ca = root[0]
@@ -274,40 +281,53 @@
         ssh_ca.connect(ca.storage.host)
         try:
             ca_data = KeyPairData.load(ssh_ca, ca.storage.path)
         finally:
             ssh_ca.close()
 
         try:
-            trust = KeyPairData.load(ssh, ce.storage)
-            cert: Certificate = trust.crt()
+            cur_trust = KeyPairData.load(ssh, ce.storage)
+            cert: Certificate = cur_trust.crt()
             expiry = cert.not_valid_after
-            if (expiry - datetime.timedelta(days=365 * ce.refresh_at)) <= datetime.datetime.utcnow():
+            if (expiry - datetime.timedelta(days=parse_validity_period(ce.refresh_at_period))) <= datetime.datetime.utcnow():
                 generate = True
                 log.debug("Expiry too soon")
-            elif set(ce.names) != set(trust.cert_names()):
+            elif set(ce.names) != set(cur_trust.cert_names()):
                 generate = True
                 log.debug("Set of names != cert names")
-            elif trust.issuer_cn() != ce.authority:
+            elif cur_trust.issuer_cn() != ce.authority:
                 generate = True
                 log.debug("Issuer CN != authority ident")
-            elif expiry > (datetime.datetime.utcnow() + datetime.timedelta(days=365 * ce.validity_years)):
+            elif expiry > (datetime.datetime.utcnow() + datetime.timedelta(days=parse_validity_period(ce.validity_period))):
                 generate = True
                 log.debug("expiry too far out")
             elif cert.subject.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value != ce.names[0]:
                 generate = True
                 log.debug("CN != cert CN")
-            elif ca_data.serial != trust.issuer_serial:
+            elif ca_data.serial != cur_trust.issuer_serial:
                 generate = True
                 log.debug("CA serial != cert issuer serial")
+            elif ce.chown and any(ce.chown != m.owner for m in cur_trust.materials() if m.mattype != "private"):
+                generate = True
+                log.debug("chown != current ownership")
+            elif ce.chmod and any(Perms(*RWXBits.from_stat(ce.chmod)) != m.perms for m in cur_trust.materials() if m.mattype != "private"):
+                generate = True
+                log.debug("chmod != current perms")
         except ValueError:
             generate = True
             log.debug("no cert found")
 
         if not generate:
             log.info(f"[{host}][pki]: OK [{ce.storage}]")
             continue
 
         log.info(f"[{host}][pki]: stale [{ce.storage}]")
 
         trust_new = _gen_cert(ce, ca_data, ca)
-        trust_new.write(ssh, ce.storage)
+        trust_new.write(ssh, ce.storage, None if not ce.chown else Owner.from_str(ce.chown), None if not ce.chmod else Perms(*RWXBits.from_stat(ce.chmod)))
+
+        if ce.hupcmd:
+            hupcmds.add(ce.hupcmd)
+
+    for cmd in hupcmds:
+        log.info(f"[{host}][pki][hup]: {cmd}")
+        check_call(ssh, cmd)
```

### Comparing `yog-2.1.6/yog/host/test_docker_attrs.py` & `yog-2.2.0/yog/host/test_docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.6/yog/logging_utils.py` & `yog-2.2.0/yog/logging_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.6/yog/repo/main.py` & `yog-2.2.0/yog/repo/main.py`

 * *Files identical despite different names*

### Comparing `yog-2.1.6/yog/res/docker_test.yml` & `yog-2.2.0/yog/res/docker_test.yml`

 * *Files identical despite different names*

### Comparing `yog-2.1.6/yog/ssh_utils.py` & `yog-2.2.0/yog/ssh_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import getpass
 import typing as t
 import logging
 import os
 import re
 import subprocess
 from hashlib import sha512
 from random import randrange
@@ -9,14 +10,16 @@
 from tempfile import NamedTemporaryFile
 from time import sleep
 from typing import Tuple, List, Optional, Set
 
 from paramiko import SSHClient, PKey
 import shlex
 
+from yog.host.os_utils import Owner, RWXBits, Perms
+
 log = logging.getLogger(__name__)
 
 
 def check_call(ssh: SSHClient, command: str, assert_stderr_empty: bool = False, send_stdin: Optional[t.AnyStr] = None, ):
     stdin, stdout, stderr = ssh.exec_command(command)
     if send_stdin is not None:
         stdin.write(send_stdin)
@@ -277,29 +280,52 @@
     log.debug(f"mkdir -p {path}")
     path = shlex.quote(path)
     cmd = f"mkdir -p {path}"
     cmd = _as_user(cmd, user)
     check_call(ssh, cmd)
 
 
+def stat(ssh: SSHClient, path: str) -> t.Tuple[Owner, Perms]:
+    path = shlex.quote(path)
+    # stat -c '%A %U:%G'
+    raw = check_output(ssh, f"stat -c {shlex.quote('%A %U:%G')} {path}")[0][0]
+    log.debug(f"stat: {path}: {raw}")
+    perms, owner = raw.split(" ", 1)
+    perms = perms[-9:]
+
+    return Owner.from_str(owner), Perms(*RWXBits.from_stat(perms))
+
+
 def _as_user(cmd: str, user: t.Optional[str]) -> str:
     user = shlex.quote(user)
     if user is None:
         return cmd
     elif user == "root":
         return "sudo " + cmd
     else:
         return f"sudo -u {user} {cmd}"
 
+
 def exists(ssh: SSHClient, path: str) -> bool:
     log.debug(f"exists? {path}")
     path = shlex.quote(path)
     ret = check_code(ssh, f"test -e {path}")
     log.debug(f"exists? {path} = {ret}")
     return ret
 
-def put(ssh: SSHClient, path: str, content: t.AnyStr, user: t.Optional[str] = None, mode: t.Optional[str] = "644"):
-    log.debug(f"put {path} {mode}")
+
+def put(ssh: SSHClient, path: str, content: t.AnyStr, user: t.Optional[str] = None, group: t.Optional[str]=None, mode: t.Optional[str] = "644"):
+    log.debug(f"put {path} {user}:{group} {mode}")
+    mode = shlex.quote(mode)
     path = shlex.quote(path)
-    check_call(ssh, _as_user(f"install -m {mode} /dev/null {path}", user))
+
+    install_opts = [f"-m {mode}"]
+    if user:
+        user = shlex.quote(user)
+        install_opts.append(f"-o {user}")
+    if group:
+        group = shlex.quote(group)
+        install_opts.append(f"-g {group}")
+    check_call(ssh, _as_user(f"install {' '.join(install_opts)} /dev/null {path}", "root"))
+
     subcommand = shlex.quote(f"cat - > {path}")
-    check_call(ssh, _as_user(f"bash -c {subcommand}", user), send_stdin=content)
+    check_call(ssh, _as_user(f"bash -c {subcommand}", "root"), send_stdin=content)
```

### Comparing `yog-2.1.6/setup.py` & `yog-2.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,316 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: yog
+Version: 2.2.0
+Summary: The Gate and Key
+License: AGPLv3
+Author: Josh Hertlein
+Author-email: jmhertlein@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: docker (>=5.0.3,<6.0.0)
+Requires-Dist: paramiko (>=2.8.0,<3.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['yog', 'yog.host', 'yog.repo', 'yog.res']
+# Overview
 
-package_data = \
-{'': ['*']}
+An opinionated docker-and-ssh-centric declarative system management tool.
 
-install_requires = \
-['PyYAML>=6.0,<7.0', 'docker>=5.0.3,<6.0.0', 'paramiko>=2.8.0,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['yog = yog.host.main:main',
-                     'yog-pki = yog.command:ca_main',
-                     'yog-repo = yog.repo.main:main']}
-
-setup_kwargs = {
-    'name': 'yog',
-    'version': '2.1.6',
-    'description': 'The Gate and Key',
-    'long_description': '# Overview\n\nAn opinionated docker-and-ssh-centric declarative system management tool.\n\n`pip3 install yog`\n\nFeatures:\n\n* Like puppet or ansible but a lot smaller and focused on docker, files, and cron\n* agentless - runs entirely on top of ssh\n* entirely defers auth(z/n) to ssh and the remote system\'s user permissions\n\nNon-features:\n\n* No intentional ipv6 support. I don\'t have anything against IPv6, but my ISP doesn\'t give me a v6 address and as such I\n  don\'t run ipv6 on my lan. So since I can\'t test it at all, I just kind of disregard it, especially where it lets me\n  make the ipv4 UX better.\n\nCommand summary:\n\n* `yog`: Applies configurations to hosts. e.g. `yog myhost.mytld` applies the config from `./domains/mytld/myhost.yml`.\n* `yog-repo`: Manages a docker repository. `yog-repo push` uses the contents of `./yog-repo.conf` to build an image and\n  push it to the configured registry with the configured name and tag.\n\nExample run:\n\n[usage.webm](https://user-images.githubusercontent.com/1287152/209723654-e78b5283-60b5-4894-b5a1-3d2d71bfcc45.webm)\n\n# Setup\n\n1. Configure docker to listen on localhost\'s port 4243 (which is the default). See below.\n2. Use `ssh-copy-id` to copy your ssh key to all the servers you wish to manage. You can look into ssh certificates if\n   you want a more general ssh PKI solution.\n3. Configure the target system to allow you to use sudo without a password. [2]\n4. That\'s it. You now serve the nameless mist. Do you hear whippoorwills?\n\n## Docker port listening setup (step 1)\n\n```bash\nssh myhost\nsudo systemctl edit docker\n```\n\nAnd add `-H tcp://127.0.0.1:4243` to the command. So for me, that file looks like:\n\n```text\n[Service]\nExecStart=\nExecStart=/usr/bin/dockerd -H fd:// -H tcp://127.0.0.1:4243\n```\n\nYog will apply files before docker containers, so you might also want to add a yog file entry like so:\n\n```yaml\nfiles:\n  - src: docker-override.conf\n    dest: /etc/systemd/system/docker.service.d/override.conf\n    root: yes\n    hupcmd: sudo systemctl restart docker\n```\n\n# Usage\n\nYog uses YML files that it calls "necronomicons" for configuration of hosts. It\'s organized hierarchically so\nthat a necronomicon for "mytld" will be applied to all hosts under that TLD.\n\nLet\'s learn by example:\n\nSuppose we have a folder, that can be named whatever we want, at `~/projects/my-config`. This is the root of a\ngit repo, and is also the root of our yog configuration. Make this your current working dir, or pass `--root-dir`.\n\n`$ cd ~/projects/my-config`\n\n```text\n.\n├── domains\n│      ├── com\n│      │      └── example\n│      │          └── myhost.yml\n│      └── com.yml\n└── files\n    ├── example.txt\n    ├── hello_world.html\n    └── helloworld-nginx.conf\n\n4 directories, 5 files\n```\n\nFiles that can be sent to hosts are stored under `files`.\n\nHost configurations - necronomicons - are stored under `domains`.\n\nIf we want to apply `myhost.yml`, we run:\n\n`yog myhost.example.com`\n\nExample output:\n\n```text\n$ yog myhost.example.com\n[2022-12-26 11:01:52,514] [INFO]: [myhost.example.com]\n[2022-12-26 11:01:59,121] [INFO]: [myhost.example.com][files]: OK [hello_world.html]\n[2022-12-26 11:01:59,274] [INFO]: [myhost.example.com][files]: OK [helloworld-nginx.conf]\n[2022-12-26 11:02:07,117] [INFO]: [myhost.example.com][docker]: OK registry@sha256:8be26f81ffea54106bae012c6f349df70f4d5e7e2ec01b143c46e2c03b9e551d\n```\n\n## Necronomicon format\n\nLet\'s look at a necronomicon.\n\n```yml\nfiles:\n  - src: hello_world.html\n    dest: /srv/hello_world/hello_world.html\n    root: yes\n  - src: helloworld-nginx.conf\n    dest: /etc/nginx/conf.d/helloworld.conf\n    root: yes\n    hupcmd: sudo systemctl restart nginx\n\n\ndocker:\n  - image: registry\n    name: my-registry\n    fingerprint: sha256:8be26f81ffea54106bae012c6f349df70f4d5e7e2ec01b143c46e2c03b9e551d\n    volumes:\n      images: /var/lib/registry\n    ports:\n      - container: 5000\n        host: [ 5000 ]\n    env:\n      REGISTRY_STORAGE_DELETE_ENABLED: true\n\npki:\n  certs:\n    - authority: my-ca\n      storage: /srv/pki/myhost/\n      validity_years: 2\n      refresh_at: 1\n      names:\n        - myhost.local\n        - myapp.local\n```\n\n### Files\n\nFiles are checked for equality via hash-comparison. I\'ve found this a useful way to manage:\n\n* cron files in /etc/cron.d/\n* Root certificates to put in the system trust store[1]\n* random config files\n\nAttributes:\n\n* `src`: the source. This is a _relative_ path rooted at the `files` directory in the hierarchy. You can use\n  intermediate dirs.\n* `dest`: the destination filepath on the managed host. This is an absolute path.\n* `root`: whether to `sudo` to root for the file put. This mainly picks who owns the file + can access files, but this\n  might have other useful properties for your use case. If set to `no`, the put operation is run as your ssh user.\n* `hupcmd`: a command to run after the file is placed. A common thing in ye olde days was to send SIGHUP to a process\n  which would handle it by reloading the config. Commonly nowadays you might be\n  using `hupcmd: sudo systemctl reload nginx`\n\n### Docker containers\n\nDocker containers are compared on all specified attributes and won\'t unnecessarily restart containers.\n\nAttributes:\n\n* `image`: the docker repository name. e.g. `itzg/minecraft-server` or `dockerrepo.local:5000/mything`\n* `name`: the container name.\n* `fingerprint`: sha digest of the desired version. Tags are bad news bears so we don\'t support them. This is called\n  fingerprint instead of digest because I didn\'t know they were called digests when I first coded this and then never\n  changed it once I did.\n* `volumes`: volumes to attach. see below.\n* `ports`: ports to open. see below.\n* `env`: environment variables to set.\n\n#### Volumes\n\nFor volumes, the key is the volume name and the value is the mount point.\n\nFor bind mounts, the key is the host path and the value is the container path.\n\n#### Ports\n\nIt\'s a list of:\n\n```text\ncontainer: port/protocol\nhost: [interface_ip:port, interface_ip:port]\n```\n\nFor the container, you can omit the protocol to get tcp by default.\n\nFor the host, you can omit the interface ip to get `0.0.0.0` which binds all interfaces.\n\nExamples:\n\n```yml\n- container: 53/tcp\n  host: [ 192.168.1.103:53, 127.0.0.1:53 ]\n- container: 53/udp\n  host: [ 192.168.1.103:53, 127.0.0.1:53 ]\n- container: 33200 # tcp is implicit default, this is the same behavior as docker\n  host: [ 33200 ] # binds 0.0.0.0\n- container: 3000\n  host: [ 8080 ]\n```\n\n### Public Key Infrastructure (PKI)\n\nYog supports low-fuss local/private PKI management.\n\nYou\'ll define certificate authories in `cas.yml` which is in your yog root (so, right next to `domains` and `files`).\n\nExample `cas.yml`:\n\n```yaml\n- ident: my-ca\n  storage: "myhost.local:/srv/yog/ca/my-ca/"\n  validity_years: 3\n```\n\nAs you can see, yog tries to keep you out of the crypto weeds.\n\n`ident` is both how you\'ll refer to this CA in necronomicons, and also the X.509 Common Name.\n`storage` is a string of format `<host>:<path>` where the trust material will be stored. More on that below.\n`validity_years` is how long the cert will be valid for upon generation.\n\nOnce you\'ve defined `cas.yml`, you can run `yog-pki`.\n\n```text\n$ yog-pki\nGenerating new CA...\n```\n\nNow you can use it in necronomicons.\n\n```yaml\npki:\n  certs:\n    - authority: my-ca # this has to refer to an "ident" in cas.yml\n      storage: /srv/pki/myhost/\n      validity_years: 2\n      refresh_at: 1 # yog runs will only renew a cert once the remaining validity time is < this number of years\n      names:\n        - myhost.local # first entry becomes X.509 Common Name\n        - myapp.local # subsequent names are X.509 Alternative Names\n```\n\n#### Trust Material Formats and Storage\n\nWhen yog or yog-pki write trust material to disk, it will restrict read access for private material but allow it for\npublic.\n\nYog writes multiple formats to facilitate as many use-cases as possible with the same PKI:\n\n| Filename             | Format              | Encoding | Public/Private | Notes                 |\n|:---------------------|:--------------------|:---------|:--------------:|-----------------------|\n| key.pem.openssl      | Traditional OpenSSL | PEM      |    private     | good for nginx        |\n| key.ssh              | SSH                 | SSH      |    private     |                       |\n| key.pem.pkcs1.public | PEM                 | PKCS1    |     public     | java\'s JCE likes this |\n| key.ssh.public       | SSH                 | SSH      |     public     |                       |\n| key.crt              | X.509 Certificate   | PEM      |     public     | good for nginx        |\n\n#### Crypto Remarks\n\nYog tries to keep you out of the weeds and also to be a good, expressive, concise tool for what it considers itself good at.\n\nYou don\'t need to, and shouldn\'t want to, read this section. It is here to help reassure anyone who knows\ntoo much about cryptography and wants to know some details.\n\nYog-pki uses Python\'s Rust-based cryptography module and doesn\'t do anything clever at all (which is dangerous in crypto).\n\nIt uses elliptic-curve keys, and uses the NIST P-384 R1 curve (known as `SECP384R1` in python\'s cryptography module).\nThis is a 384-bit key, roughly equivalent to the hardness of a 7000-bit RSA key. \n\nIt uses CN and Alternative Names to set the "names" that certificates represent. \n\nNothing else is configurable. Small tweaks come in the future but generally speaking,\nI don\'t intend for yog-pki to handle huge, complicated PKIs. If you need to do so, \nyou might want to look at https://smallstep.com/. (You can use Yog\'s docker and file capabilities to\ndeploy a smallstep installation!)\n\n# Footnotes\n\n[1] This is one of those things where I feel like you probably shouldn\'t manage root certs like this but I have yet to\nregret it? It\'s not a cryptographic secret, so.\n\n[2] Also something that people say you probably shouldn\'t do but I\'ve yet to regret. If your user is in the docker group\nit\'s basically root anyway from a threat modeling perspective.\n\n# `yog-repo`\n\nYog also includes a tool for pushing images to your local docker registry. I haven\'t documented it yet, apologies. \n',
-    'author': 'Josh Hertlein',
-    'author_email': 'jmhertlein@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+`pip3 install yog`
 
+Features:
+
+* Like puppet or ansible but a lot smaller and focused on docker, files, and cron
+* agentless - runs entirely on top of ssh
+* entirely defers auth(z/n) to ssh and the remote system's user permissions
+
+Non-features:
+
+* No intentional ipv6 support. I don't have anything against IPv6, but my ISP doesn't give me a v6 address and as such I
+  don't run ipv6 on my lan. So since I can't test it at all, I just kind of disregard it, especially where it lets me
+  make the ipv4 UX better.
+
+Command summary:
+
+* `yog`: Applies configurations to hosts. e.g. `yog myhost.mytld` applies the config from `./domains/mytld/myhost.yml`.
+* `yog-repo`: Manages a docker repository. `yog-repo push` uses the contents of `./yog-repo.conf` to build an image and
+  push it to the configured registry with the configured name and tag.
+
+Example run:
+
+[usage.webm](https://user-images.githubusercontent.com/1287152/209723654-e78b5283-60b5-4894-b5a1-3d2d71bfcc45.webm)
+
+# Setup
+
+1. Configure docker to listen on localhost's port 4243 (which is the default). See below.
+2. Use `ssh-copy-id` to copy your ssh key to all the servers you wish to manage. You can look into ssh certificates if
+   you want a more general ssh PKI solution.
+3. Configure the target system to allow you to use sudo without a password. [2]
+4. That's it. You now serve the nameless mist. Do you hear whippoorwills?
+
+## Docker port listening setup (step 1)
+
+```bash
+ssh myhost
+sudo systemctl edit docker
+```
+
+And add `-H tcp://127.0.0.1:4243` to the command. So for me, that file looks like:
+
+```text
+[Service]
+ExecStart=
+ExecStart=/usr/bin/dockerd -H fd:// -H tcp://127.0.0.1:4243
+```
+
+Yog will apply files before docker containers, so you might also want to add a yog file entry like so:
+
+```yaml
+files:
+  - src: docker-override.conf
+    dest: /etc/systemd/system/docker.service.d/override.conf
+    root: yes
+    hupcmd: sudo systemctl restart docker
+```
+
+# Usage
+
+Yog uses YML files that it calls "necronomicons" for configuration of hosts. It's organized hierarchically so
+that a necronomicon for "mytld" will be applied to all hosts under that TLD.
+
+Let's learn by example:
+
+Suppose we have a folder, that can be named whatever we want, at `~/projects/my-config`. This is the root of a
+git repo, and is also the root of our yog configuration. Make this your current working dir, or pass `--root-dir`.
+
+`$ cd ~/projects/my-config`
+
+```text
+.
+├── domains
+│      ├── com
+│      │      └── example
+│      │          └── myhost.yml
+│      └── com.yml
+└── files
+    ├── example.txt
+    ├── hello_world.html
+    └── helloworld-nginx.conf
+
+4 directories, 5 files
+```
+
+Files that can be sent to hosts are stored under `files`.
+
+Host configurations - necronomicons - are stored under `domains`.
+
+If we want to apply `myhost.yml`, we run:
+
+`yog myhost.example.com`
+
+Example output:
+
+```text
+$ yog myhost.example.com
+[2022-12-26 11:01:52,514] [INFO]: [myhost.example.com]
+[2022-12-26 11:01:59,121] [INFO]: [myhost.example.com][files]: OK [hello_world.html]
+[2022-12-26 11:01:59,274] [INFO]: [myhost.example.com][files]: OK [helloworld-nginx.conf]
+[2022-12-26 11:02:07,117] [INFO]: [myhost.example.com][docker]: OK registry@sha256:8be26f81ffea54106bae012c6f349df70f4d5e7e2ec01b143c46e2c03b9e551d
+```
+
+## Necronomicon format
+
+Let's look at a necronomicon.
+
+```yml
+files:
+  - src: hello_world.html
+    dest: /srv/hello_world/hello_world.html
+    root: yes
+  - src: helloworld-nginx.conf
+    dest: /etc/nginx/conf.d/helloworld.conf
+    root: yes
+    hupcmd: sudo systemctl restart nginx
+
+
+docker:
+  - image: registry
+    name: my-registry
+    fingerprint: sha256:8be26f81ffea54106bae012c6f349df70f4d5e7e2ec01b143c46e2c03b9e551d
+    volumes:
+      images: /var/lib/registry
+    ports:
+      - container: 5000
+        host: [ 5000 ]
+    env:
+      REGISTRY_STORAGE_DELETE_ENABLED: true
+
+pki:
+  certs:
+    - authority: my-ca
+      storage: /srv/pki/myhost/
+      validity_years: 2
+      refresh_at: 1
+      names:
+        - myhost.local
+        - myapp.local
+```
+
+### Files
+
+Files are checked for equality via hash-comparison. I've found this a useful way to manage:
+
+* cron files in /etc/cron.d/
+* Root certificates to put in the system trust store[1]
+* random config files
+
+Attributes:
+
+* `src`: the source. This is a _relative_ path rooted at the `files` directory in the hierarchy. You can use
+  intermediate dirs.
+* `dest`: the destination filepath on the managed host. This is an absolute path.
+* `root`: whether to `sudo` to root for the file put. This mainly picks who owns the file + can access files, but this
+  might have other useful properties for your use case. If set to `no`, the put operation is run as your ssh user.
+* `hupcmd`: a command to run after the file is placed. A common thing in ye olde days was to send SIGHUP to a process
+  which would handle it by reloading the config. Commonly nowadays you might be
+  using `hupcmd: sudo systemctl reload nginx`
+
+### Docker containers
+
+Docker containers are compared on all specified attributes and won't unnecessarily restart containers.
+
+Attributes:
+
+* `image`: the docker repository name. e.g. `itzg/minecraft-server` or `dockerrepo.local:5000/mything`
+* `name`: the container name.
+* `fingerprint`: sha digest of the desired version. Tags are bad news bears so we don't support them. This is called
+  fingerprint instead of digest because I didn't know they were called digests when I first coded this and then never
+  changed it once I did.
+* `volumes`: volumes to attach. see below.
+* `ports`: ports to open. see below.
+* `env`: environment variables to set.
+
+#### Volumes
+
+For volumes, the key is the volume name and the value is the mount point.
+
+For bind mounts, the key is the host path and the value is the container path.
+
+#### Ports
+
+It's a list of:
+
+```text
+container: port/protocol
+host: [interface_ip:port, interface_ip:port]
+```
+
+For the container, you can omit the protocol to get tcp by default.
+
+For the host, you can omit the interface ip to get `0.0.0.0` which binds all interfaces.
+
+Examples:
+
+```yml
+- container: 53/tcp
+  host: [ 192.168.1.103:53, 127.0.0.1:53 ]
+- container: 53/udp
+  host: [ 192.168.1.103:53, 127.0.0.1:53 ]
+- container: 33200 # tcp is implicit default, this is the same behavior as docker
+  host: [ 33200 ] # binds 0.0.0.0
+- container: 3000
+  host: [ 8080 ]
+```
+
+### Public Key Infrastructure (PKI)
+
+Yog supports low-fuss local/private PKI management.
+
+You'll define certificate authories in `cas.yml` which is in your yog root (so, right next to `domains` and `files`).
+
+Example `cas.yml`:
+
+```yaml
+- ident: my-ca
+  storage: "myhost.local:/srv/yog/ca/my-ca/"
+  validity_years: 3
+```
+
+As you can see, yog tries to keep you out of the crypto weeds.
+
+`ident` is both how you'll refer to this CA in necronomicons, and also the X.509 Common Name.
+`storage` is a string of format `<host>:<path>` where the trust material will be stored. More on that below.
+`validity_years` is how long the cert will be valid for upon generation.
+
+Once you've defined `cas.yml`, you can run `yog-pki`.
+
+```text
+$ yog-pki
+Generating new CA...
+```
+
+Now you can use it in necronomicons.
+
+```yaml
+pki:
+  certs:
+    - authority: my-ca # this has to refer to an "ident" in cas.yml
+      storage: /srv/pki/myhost/
+      validity_years: 2
+      refresh_at: 1 # yog runs will only renew a cert once the remaining validity time is < this number of years
+      names:
+        - myhost.local # first entry becomes X.509 Common Name
+        - myapp.local # subsequent names are X.509 Alternative Names
+```
+
+#### Trust Material Formats and Storage
+
+When yog or yog-pki write trust material to disk, it will restrict read access for private material but allow it for
+public.
+
+Yog writes multiple formats to facilitate as many use-cases as possible with the same PKI:
+
+| Filename             | Format              | Encoding | Public/Private | Notes                 |
+|:---------------------|:--------------------|:---------|:--------------:|-----------------------|
+| key.pem.openssl      | Traditional OpenSSL | PEM      |    private     | good for nginx        |
+| key.ssh              | SSH                 | SSH      |    private     |                       |
+| key.pem.pkcs1.public | PEM                 | PKCS1    |     public     | java's JCE likes this |
+| key.ssh.public       | SSH                 | SSH      |     public     |                       |
+| key.crt              | X.509 Certificate   | PEM      |     public     | good for nginx        |
+
+#### Crypto Remarks
+
+Yog tries to keep you out of the weeds and also to be a good, expressive, concise tool for what it considers itself good at.
+
+You don't need to, and shouldn't want to, read this section. It is here to help reassure anyone who knows
+too much about cryptography and wants to know some details.
+
+Yog-pki uses Python's Rust-based cryptography module and doesn't do anything clever at all (which is dangerous in crypto).
+
+It uses elliptic-curve keys, and uses the NIST P-384 R1 curve (known as `SECP384R1` in python's cryptography module).
+This is a 384-bit key, roughly equivalent to the hardness of a 7000-bit RSA key. 
+
+It uses CN and Alternative Names to set the "names" that certificates represent. 
+
+Nothing else is configurable. Small tweaks come in the future but generally speaking,
+I don't intend for yog-pki to handle huge, complicated PKIs. If you need to do so, 
+you might want to look at https://smallstep.com/. (You can use Yog's docker and file capabilities to
+deploy a smallstep installation!)
+
+# Footnotes
+
+[1] This is one of those things where I feel like you probably shouldn't manage root certs like this but I have yet to
+regret it? It's not a cryptographic secret, so.
+
+[2] Also something that people say you probably shouldn't do but I've yet to regret. If your user is in the docker group
+it's basically root anyway from a threat modeling perspective.
+
+# `yog-repo`
+
+Yog also includes a tool for pushing images to your local docker registry. I haven't documented it yet, apologies. 
 
-setup(**setup_kwargs)
```

