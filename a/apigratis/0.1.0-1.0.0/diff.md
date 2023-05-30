# Comparing `tmp/apigratis-0.1.0.tar.gz` & `tmp/apigratis-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apigratis-0.1.0.tar", last modified: Tue May 30 12:37:17 2023, max compression
+gzip compressed data, was "apigratis-1.0.0.tar", last modified: Tue May 30 14:09:44 2023, max compression
```

## Comparing `apigratis-0.1.0.tar` & `apigratis-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 12:37:17.369854 apigratis-0.1.0/
--rw-rw-rw-   0        0        0      454 2023-05-30 12:37:17.368854 apigratis-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2640 2023-05-30 12:37:02.000000 apigratis-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 12:37:17.346848 apigratis-0.1.0/apigratis/
--rw-rw-rw-   0        0        0     1828 2023-05-29 23:03:05.000000 apigratis-0.1.0/apigratis/Service.py
--rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-0.1.0/apigratis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:37:17.366847 apigratis-0.1.0/apigratis.egg-info/
--rw-rw-rw-   0        0        0      454 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 12:37:17.369854 apigratis-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-05-30 12:36:50.000000 apigratis-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:09:44.930466 apigratis-1.0.0/
+-rw-rw-rw-   0        0        0     3927 2023-05-30 14:09:44.930466 apigratis-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2693 2023-05-30 14:06:52.000000 apigratis-1.0.0/README
+drwxrwxrwx   0        0        0        0 2023-05-30 14:09:44.909503 apigratis-1.0.0/apigratis/
+-rw-rw-rw-   0        0        0     1780 2023-05-30 13:12:32.000000 apigratis-1.0.0/apigratis/Service.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-1.0.0/apigratis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:09:44.927950 apigratis-1.0.0/apigratis.egg-info/
+-rw-rw-rw-   0        0        0     3927 2023-05-30 14:09:44.000000 apigratis-1.0.0/apigratis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-30 14:09:44.000000 apigratis-1.0.0/apigratis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 14:09:44.000000 apigratis-1.0.0/apigratis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 14:09:44.000000 apigratis-1.0.0/apigratis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 14:09:44.000000 apigratis-1.0.0/apigratis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1198 2023-05-30 14:09:40.000000 apigratis-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 14:09:44.931467 apigratis-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-05-30 14:09:26.000000 apigratis-1.0.0/setup.py
```

### Comparing `apigratis-0.1.0/README.rst` & `apigratis-1.0.0/README`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,46 @@
-# SDK Python - APIGratis by API BRASIL 🚀
+# SDK Python - APIGratis by API BRASIL
 
 Conjunto de API, para desenvolvedores.
 
-_Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais. Comece agora._
+_Transforme seus projetos em solucoes inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalizacao, rastreamento de encomendas, verificacao de CPF/CNPJ e mais, voce pode criar solucoes eficientes e funcionais._
 
-#Como instalar
+## Como instalar
 
-```pip3 install apigratis==0.0.9```
+```pip3 install apigratis```
 ## Canais de suporte (Comunidade)
 [![WhatsApp Group](https://img.shields.io/badge/WhatsApp-Group-25D366?logo=whatsapp)](https://chat.whatsapp.com/KsxrUGIPWvUBYAjI1ogaGs)
 [![Telegram Group](https://img.shields.io/badge/Telegram-Group-32AFED?logo=telegram)](https://t.me/apigratisoficial)
 
 ## Obtenha suas credenciais
 https://apigratis.com.br
 
-# Mais informações
+## Mais informacoes
 
-https://pypi.org/project/apigratis/0.1.0/
+https://pypi.org/project/apigratis
 
-## Serviços de API disponíveis
+## Servicos de API disponíveis
 
 | Up  | Services available            | Description       | Free    | Beta        | Stable   |
 ------|-------------------------------|-------------------|---------| ------------------------- | ------------------------- |
-| ✅ | WhatsAppService                | API do WhatsApp Gratuita.               |   ✅   | ✅                   | ⌛                   |
-| ✅ | Receita Data CNPJ              | API Dados CNPJ Receita.                 |   ⌛   | ⌛                   | ⌛                   |
-| ✅ | Receita Data CPF               | API Dados de CPF Serasa.                |   ⌛   | ⌛                   | ⌛                   |
-| ✅ | CorreiosService                | API Busca encomendas Correios Brazil.   |   ⌛   | ⌛                   | ⌛                   |
-| ✅ | CEPLocation                    | API CEP Geolocation + IBGE Brazil.      |   ⌛   | ⌛                   | ⌛                   |
-| ✅ | VehiclesService                | API Placa Dados.                        |   ⌛   | ⌛                   | ⌛                   |
-| ✅ | FipeService                    | API Placa FIPE.                         |   ⌛   | ⌛                   | ⌛                   |
+| O | WhatsAppService                | API do WhatsApp Gratuita.               |   O   | O                   | x                   |
+| x | Receita Data CNPJ              | API Dados CNPJ Receita.                 |   x   | x                   | x                   |
+| x | Receita Data CPF               | API Dados de CPF Serasa.                |   x   | x                   | x                   |
+| x | CorreiosService                | API Busca encomendas Correios Brazil.   |   x   | x                   | x                   |
+| x | CEPLocation                    | API CEP Geolocation + IBGE Brazil.      |   x   | x                   | x                   |
+| x | VehiclesService                | API Placa Dados.                        |   x   | x                   | x                   |
+| x | FipeService                    | API Placa FIPE.                         |   x   | x                   | x                   |
+
+## Como utilizar
+
+_Você pode utilizar todos os endpoints da API do WhatsApp, basta mudar o action e o body_
+
+## Documentacoes
+https://apibrasil.com.br/documentacoes
 
-# Como utilizar
 
 ```python
 
 from apigratis.Service import Service
 import json
 
 def main():
```

### Comparing `apigratis-0.1.0/apigratis/Service.py` & `apigratis-1.0.0/apigratis/Service.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,14 @@
             if not data['body']:
                 raise Exception('Body não informado, verifique a documentação')
 
             payload = json.dumps(data['body'])
 
             credentials = data['credentials']
 
-            #valida se os dados foram passados
             if not credentials['SecretKey']:
                 raise Exception('SecretKey não informado')
             if not credentials['PublicToken']:
                 raise Exception('PublicToken não informado')
             if not credentials['BearerToken']:
                 raise Exception('BearerToken não informado')
             if not credentials['DeviceToken']:
```

### Comparing `apigratis-0.1.0/setup.py` & `apigratis-1.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from setuptools import setup
 
-setup(
-    name='apigratis',
-    version='0.1.0',
-    description='Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como  API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais. Comece agora.',
+with open("README.md", "r") as fh:
+    readme = fh.read()
+
+setup(name='apigratis',
+    version='1.0.0',
+    url='https://github.com/APIBrasil/apigratis-sdk-python',
+    license='MIT License',
     author='APIBRASIL',
+    long_description=readme,
+    long_description_content_type="text/markdown",
     author_email='contato@apibrasil.com.br',
+    keywords='whatsapp api, apibrasil, cnpj, sms, cep, consulta, api, brasil, gratis, free, whatsapp, apiwhatsapp, apigratis, apifree',
+    description=u'Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais',
     packages=['apigratis'],
-    install_requires=[
-        # Lista de dependências necessárias
-        'requests',
-    ],
-)
+    install_requires=['requests'])
```

