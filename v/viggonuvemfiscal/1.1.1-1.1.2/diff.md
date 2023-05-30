# Comparing `tmp/viggonuvemfiscal-1.1.1.tar.gz` & `tmp/viggonuvemfiscal-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggonuvemfiscal-1.1.1.tar", last modified: Fri May 19 12:05:28 2023, max compression
+gzip compressed data, was "viggonuvemfiscal-1.1.2.tar", last modified: Tue May 30 16:45:22 2023, max compression
```

## Comparing `viggonuvemfiscal-1.1.1.tar` & `viggonuvemfiscal-1.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    18422 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-19 12:04:26.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 12:05:28.822647 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-19 12:05:28.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-19 12:05:28.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 12:05:28.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-19 12:05:28.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-19 12:05:28.000000 viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.572012 viggonuvemfiscal-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-30 16:45:22.572012 viggonuvemfiscal-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:45:22.572012 viggonuvemfiscal-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.568011 viggonuvemfiscal-1.1.2/viggonuvemfiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.568011 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.568011 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.568011 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.572012 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22598 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18828 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-05-30 16:44:23.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:45:22.568011 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-30 16:45:22.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-30 16:45:22.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:45:22.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 16:45:22.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 16:45:22.000000 viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/top_level.txt
```

### Comparing `viggonuvemfiscal-1.1.1/viggonuvemfiscal/__init__.py` & `viggonuvemfiscal-1.1.2/viggonuvemfiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.1/viggonuvemfiscal/resources.py` & `viggonuvemfiscal-1.1.2/viggonuvemfiscal/resources.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py` & `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py` & `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py` & `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,23 @@
 
 
 class BaixarXmlNfe(operation.List):
 
     def do(self, session, **kwargs):
         ambiente = kwargs.pop('api_fiscal', cnf_tipo.HOMOLOGACAO)
         nfe_id = self.manager.get_nfe_id(**kwargs)
+        url = self.manager.get_endpoint(f'/nfe/{nfe_id}/xml', ambiente)
+        return self.manager.executar_requisicao('GET', url, ambiente=ambiente)
+
+
+class BaixarXmlNotaNfe(operation.List):
+
+    def do(self, session, **kwargs):
+        ambiente = kwargs.pop('api_fiscal', cnf_tipo.HOMOLOGACAO)
+        nfe_id = self.manager.get_nfe_id(**kwargs)
         url = self.manager.get_endpoint(f'/nfe/{nfe_id}/xml/nota', ambiente)
         return self.manager.executar_requisicao('GET', url, ambiente=ambiente)
 
 
 class BaixarPdfDanfeNfe(operation.List):
 
     def do(self, session, **kwargs):
@@ -367,14 +376,15 @@
         # rotas de nfe
         self.emitir_nfe = EmitirNfe(self)
         self.listar_nfe = ListarNfe(self)
         self.consulta_status_do_servico_na_sefaz_autorizadora_nfe = \
             ConsultaStatusDoServicoNaSefazAutorizadoraNfe(self)
         self.consultar_nfe = ConsultarNfe(self)
         self.baixar_xml_nfe = BaixarXmlNfe(self)
+        self.baixar_xml_nota_nfe = BaixarXmlNotaNfe(self)
         self.baixar_pdf_danfe_nfe = BaixarPdfDanfeNfe(self)
         self.consultar_cancelamento_nfe = ConsultarCancelamentoNfe(self)
         self.baixar_xml_cancelamento_nfe = BaixarXmlCancelamentoNfe(self)
         self.cancelar_nfe_autorizada = CancelarNfeAutorizada(self)
         self.inutilizar_seq_num_nfe = InutilizarSeqNumNfe(self)
         # rotas de nfce
         self.emitir_nfce = EmitirNfce(self)
```

### Comparing `viggonuvemfiscal-1.1.1/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py` & `viggonuvemfiscal-1.1.2/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.1.1/viggonuvemfiscal.egg-info/SOURCES.txt` & `viggonuvemfiscal-1.1.2/viggonuvemfiscal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

