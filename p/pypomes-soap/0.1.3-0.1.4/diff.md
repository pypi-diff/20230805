# Comparing `tmp/pypomes_soap-0.1.3.tar.gz` & `tmp/pypomes_soap-0.1.4.tar.gz`

## Comparing `pypomes_soap-0.1.3.tar` & `pypomes_soap-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/src/pypomes_soap/__init__.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/src/pypomes_soap/soap_pomes.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/README.md
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pypomes_soap-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pypomes_soap-0.1.4/src/pypomes_soap/__init__.py
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 pypomes_soap-0.1.4/src/pypomes_soap/soap_pomes.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_soap-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_soap-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_soap-0.1.4/README.md
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pypomes_soap-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pypomes_soap-0.1.4/PKG-INFO
```

### Comparing `pypomes_soap-0.1.3/src/pypomes_soap/soap_pomes.py` & `pypomes_soap-0.1.4/src/pypomes_soap/soap_pomes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import ast
 import json
 import requests
 from lxml import etree
-from pypomes_core import json_normalize_dict, xml_to_dict
+from pathlib import Path
+from pypomes_core import HTTP_GET_TIMEOUT, json_normalize_dict, xml_to_dict
 from zeep import Client
 
 
-def soap_build_envelope(zeep_client: Client, service: str, payload: dict, file_path: str = None) -> bytes:
+def soap_build_envelope(zeep_client: Client, service: str, payload: dict, file_path: Path = None) -> bytes:
     """
     Constrói e retorna o envelope SOAP para um dado serviço. Esse envelope não contem os *headers*.
 
     :param zeep_client: o cliente zeep
     :param payload: os dados a serem enviados
     :param service: o nome do serviço
     :param file_path: Path to store the soap envelope.
@@ -20,55 +21,58 @@
     root = zeep_client.create_message(zeep_client.service, service, **payload)
     result: bytes = etree.tostring(element_or_tree=root,
                                    pretty_print=True)
 
     # salva o envelope em arquivo ?
     if file_path is not None:
         # sim
-        with open(file_path, "wb") as f:
+        with Path.open(file_path, "wb") as f:
             f.write(result)
 
     return result
 
 
-def soap_post(ws_url: str, soap_envelope: bytes, extra_headers: dict = None, file_path: str = None) -> bytes:
+def soap_post(ws_url: str, soap_envelope: bytes, extra_headers: dict = None,
+              file_path: Path = None, timeout: int = HTTP_GET_TIMEOUT) -> bytes:
     """
     Encaminha a solicitação SOAP, e retorna a resposta recebida.
 
     :param ws_url: a URL da solicitação
     :param soap_envelope: o envelope SOAP
     :param extra_headers: cabeçalho adicional
     :param file_path: Path to store the response to the request.
+    :param timeout: timeout, in seconds (defaults to HTTP_GET_TIMEOUT - use None to omit)
     :return: a resposta à solicitação
     """
     # constrói o cabeçalho do envelope SOAP
     headers: dict = {"SOAPAction": '""',
                      "content-type": "application/soap+xml; charset=utf-8"}
 
     # um cabeçalho adicional foi definido ?
     if extra_headers is not None:
         # sim, contabilize-o
         headers.update(extra_headers)
 
     # envia o request
     response: requests.Response = requests.post(url=ws_url,
                                                 data=soap_envelope,
-                                                headers=headers)
+                                                headers=headers,
+                                                timeout=timeout)
     result: bytes = response.content
 
     # salva o response em arquivo ?
     if file_path is not None:
         # sim
-        with open(file_path, "wb") as f:
+        with Path.open(file_path, "wb") as f:
             f.write(result)
 
     return result
 
 
-def soap_post_zeep(zeep_service: callable, payload: dict, file_path: str = None) -> dict:
+def soap_post_zeep(zeep_service: callable, payload: dict, file_path: Path = None) -> dict:
     """
     Encaminha a solicitação SOAP utilizando o pacote *zeep*, e retorna a resposta recebida.
 
     :param zeep_service: o serviço de referência
     :param payload: os dados a serem enviados
     :param file_path: Path to store the JSON corresponding to the returned response.
     :return: a resposta à solicitação
@@ -80,21 +84,21 @@
     # converte o conteúdo retornado em dict e o prepara para descarga em JSON
     result: dict = ast.literal_eval(str(response))
     json_normalize_dict(result)
 
     # salva o retorno em arquivo ?
     if file_path is not None:
         # sim
-        with open(file_path, "w") as f:
+        with Path.open(file_path, "w") as f:
             f.write(json.dumps(result, ensure_ascii=False))
 
     return result
 
 
-def soap_get_dict(soap_response: bytes, xml_path: str = None, json_path: str = None) -> dict:
+def soap_get_dict(soap_response: bytes, xml_path: Path = None, json_path: Path = None) -> dict:
     """
     Recupera o objeto *dict* contendo os dados retornados pela solicitação SOAP.
 
     Esse objeto é retornado em condições de ser descarregado em formato JSON.
 
     :param soap_response: o conteúdo retornado pela solicitação SOAP
     :param xml_path: Path to store the XML correspondinge to the returned response.
@@ -105,25 +109,25 @@
     pos_1: int = soap_response.find(b"<soap:Body>") + 11
     pos_2: int = soap_response.find(b"</soap:Body>", pos_1)
     content: bytes = soap_response[pos_1:pos_2]
 
     # salva o conteúdo XML retornado em arquivo ?
     if xml_path is not None:
         # sim
-        with open(xml_path, "wb") as f:
+        with Path.open(xml_path, "wb") as f:
             f.write(content)
 
     # converte o conteúdo XML em dict e o prepara para descarga em JSON
     result: dict = xml_to_dict(content)
     json_normalize_dict(result)
 
     # salva o retorno em arquivo ?
     if json_path is not None:
         # sim
-        with open(json_path, "w") as f:
+        with Path.open(json_path, "w") as f:
             f.write(json.dumps(result, ensure_ascii=False))
 
     return result
 
 
 def soap_get_cids(soap_response: bytes) -> list[bytes]:
     """
@@ -153,15 +157,15 @@
         pos_2: int = soap_response.find(b'"', pos_1)
         result.append(soap_response[pos_1:pos_2])
         pos_1 = soap_response.find(prefix, pos_1)
 
     return result
 
 
-def soap_get_attachment(soap_response: bytes, cid: bytes, file_path: str = None) -> bytes:
+def soap_get_attachment(soap_response: bytes, cid: bytes, file_path: Path = None) -> bytes:
     """
     Obtem e retorna o anexo contido no *response* da solicitação *SOAP*, no padrão *MTOM*.
 
     Nesse padrão (*Message Transmission Optimization Mechanism*), o anexo é identificado pelo *cid* (Content-ID).
 
     :param soap_response: o conteúdo retornado pela solicitação SOAP
     :param cid: a identificação do anexo
@@ -194,11 +198,11 @@
 
         # obtem o anexo
         result: bytes = soap_response[pos_1:pos_2]
 
         # salva o attachment em arquivo ?
         if file_path is not None:
             # sim
-            with open(file_path, "wb") as f:
+            with Path.open(file_path, "wb") as f:
                 f.write(result)
 
     return result
```

### Comparing `pypomes_soap-0.1.3/LICENSE` & `pypomes_soap-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_soap-0.1.3/PKG-INFO` & `pypomes_soap-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pypomes_soap
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of Python pomes, pennyeach (SOAP module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-SOAP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-SOAP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: lxml>=4.9.3
 Requires-Dist: pip>=23.2.1
-Requires-Dist: pypomes-core>=0.2.1
+Requires-Dist: pypomes-core>=0.2.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.41.0
 Requires-Dist: zeep>=4.2.1
```

