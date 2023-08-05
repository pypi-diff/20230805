# Comparing `tmp/offat-0.4.0.tar.gz` & `tmp/offat-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offat-0.4.0.tar", max compression
+gzip compressed data, was "offat-0.5.0.tar", max compression
```

## Comparing `offat-0.4.0.tar` & `offat-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-31 18:36:18.784892 offat-0.4.0/LICENSE
--rw-r--r--   0        0        0     5781 2023-07-31 18:36:18.784892 offat-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-07-31 18:36:18.784892 offat-0.4.0/offat/__init__.py
--rw-r--r--   0        0        0     1027 2023-07-31 18:36:18.788892 offat-0.4.0/offat/__main__.py
--rw-r--r--   0        0        0     4327 2023-07-31 18:36:18.788892 offat-0.4.0/offat/http.py
--rw-r--r--   0        0        0     1122 2023-07-31 18:36:18.788892 offat-0.4.0/offat/logger.py
--rw-r--r--   0        0        0     3767 2023-07-31 18:36:18.788892 offat-0.4.0/offat/openapi.py
--rw-r--r--   0        0        0        0 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/__init__.py
--rw-r--r--   0        0        0     1567 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/data_exposure.py
--rw-r--r--   0        0        0     3158 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/fuzzer.py
--rw-r--r--   0        0        0     1617 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/regexs.py
--rw-r--r--   0        0        0    12039 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/test_generator.py
--rw-r--r--   0        0        0     1537 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/test_results.py
--rw-r--r--   0        0        0     4720 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/test_runner.py
--rw-r--r--   0        0        0     2175 2023-07-31 18:36:18.788892 offat-0.4.0/offat/tester/tester_utils.py
--rw-r--r--   0        0        0     3051 2023-07-31 18:36:18.788892 offat-0.4.0/offat/utils.py
--rw-r--r--   0        0        0      873 2023-07-31 18:36:18.788892 offat-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6749 1970-01-01 00:00:00.000000 offat-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-05 20:31:37.299740 offat-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6055 2023-08-05 20:31:37.299740 offat-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 20:31:37.299740 offat-0.5.0/offat/__init__.py
+-rw-r--r--   0        0        0     2224 2023-08-05 20:31:37.299740 offat-0.5.0/offat/__main__.py
+-rw-r--r--   0        0        0     4327 2023-08-05 20:31:37.303740 offat-0.5.0/offat/http.py
+-rw-r--r--   0        0        0     1122 2023-08-05 20:31:37.303740 offat-0.5.0/offat/logger.py
+-rw-r--r--   0        0        0     3767 2023-08-05 20:31:37.303740 offat-0.5.0/offat/openapi.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:31:37.303740 offat-0.5.0/offat/tester/__init__.py
+-rw-r--r--   0        0        0     1567 2023-08-05 20:31:37.303740 offat-0.5.0/offat/tester/data_exposure.py
+-rw-r--r--   0        0        0     3730 2023-08-05 20:31:37.303740 offat-0.5.0/offat/tester/fuzzer.py
+-rw-r--r--   0        0        0     1617 2023-08-05 20:31:37.303740 offat-0.5.0/offat/tester/regexs.py
+-rw-r--r--   0        0        0    17259 2023-08-05 20:31:37.303740 offat-0.5.0/offat/tester/test_generator.py
+-rw-r--r--   0        0        0     2032 2023-08-05 20:31:37.303740 offat-0.5.0/offat/tester/test_results.py
+-rw-r--r--   0        0        0     4961 2023-08-05 20:31:37.303740 offat-0.5.0/offat/tester/test_runner.py
+-rw-r--r--   0        0        0     2859 2023-08-05 20:31:37.303740 offat-0.5.0/offat/tester/tester_utils.py
+-rw-r--r--   0        0        0     4629 2023-08-05 20:31:37.303740 offat-0.5.0/offat/utils.py
+-rw-r--r--   0        0        0      873 2023-08-05 20:31:37.303740 offat-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7023 1970-01-01 00:00:00.000000 offat-0.5.0/PKG-INFO
```

### Comparing `offat-0.4.0/LICENSE` & `offat-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `offat-0.4.0/README.md` & `offat-0.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # OFFAT - OFFensive Api Tester
 
 Automatically Tests for vulnerabilities after generating tests from openapi specification file. Project is in Beta stage, so sometimes it might crash while running.
 
-![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-test-undocumented-api-endpoint-http-method.png)
+![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-v0.5.0.png)
 
 ## Features
 
 - [X] Restricted HTTP Methods
 - [X] SQLi
 - [X] BOLA (Might need few bug fixes)
 - [X] Data Exposure (Detects Common Data Exposures)
@@ -100,14 +100,30 @@
 
 - Run tests only for endpoint paths matching regex pattern
 
   ```bash
   offat -f swagger_file.json -pr '/user'
   ```
 
+- Add headers to requests
+
+  ```bash
+  offat -f swagger_file.json -H 'Accept: application/json' -H 'Authorization: Bearer YourJWTToken'
+  ```
+
+- Run Test with Requests Rate Limited
+
+  ```bash
+  offat -f swagger_file.json -rl 1000 -dr 0.001
+  ```
+
+  > `rl`: requests rate limit, `dr`: delay between requests
+
+
+
 > If you're using Termux or windows, then use `pip` instead of `pip3`.  
 > Few features are only for linux os, hence they might not work on windows and require admin priviliges.
 
 ### Open In Google Cloud Shell
 
 - Temporary Session  
   [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/dmdhrumilmistry/offat.git&ephemeral=true&show=terminal&cloudshell_print=./DISCLAIMER.md)
```

### Comparing `offat-0.4.0/offat/http.py` & `offat-0.5.0/offat/http.py`

 * *Files identical despite different names*

### Comparing `offat-0.4.0/offat/logger.py` & `offat-0.5.0/offat/logger.py`

 * *Files identical despite different names*

### Comparing `offat-0.4.0/offat/openapi.py` & `offat-0.5.0/offat/openapi.py`

 * *Files identical despite different names*

### Comparing `offat-0.4.0/offat/tester/data_exposure.py` & `offat-0.5.0/offat/tester/data_exposure.py`

 * *Files identical despite different names*

### Comparing `offat-0.4.0/offat/tester/regexs.py` & `offat-0.5.0/offat/tester/regexs.py`

 * *Files identical despite different names*

### Comparing `offat-0.4.0/offat/tester/test_generator.py` & `offat-0.5.0/offat/tester/test_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from copy import deepcopy
 from .fuzzer import fill_params
 from .test_runner import TestRunnerFiltersEnum
+from .fuzzer import generate_random_int
 from ..openapi import OpenAPIParser
 
 
 class TestGenerator:
     """
     Class to generate API test checks.
 
@@ -112,50 +113,99 @@
                         'name':prop,
                         'type':prop_type,
                         'required': prop in required_params,
                     })
 
         return payload_data
     
+    def __fuzz_request_params(self, openapi_parser:OpenAPIParser) -> list[dict]:
+        """
+        Fuzzes Request params available in different positions and returns a list
+        of tasks
+
+        Args:
+            openapi_parser (OpenAPIParser): An instance of the OpenAPIParser class
+            containing the parsed OpenAPI specification.
+
+        Returns:
+            list: returns list of dict (tasks) for API testing with fuzzed request params
+        """
+        base_url:str = openapi_parser.base_url
+        request_response_params:list[dict] = openapi_parser.request_response_params
+
+        tasks = []
+        for path_obj in request_response_params:
+            # handle path params from request_params
+            request_params = path_obj.get('request_params',[])
+            request_params = fill_params(request_params)
+
+            # get params based on their position in request
+            request_body_params = list(filter(lambda x: x.get('in') == 'body', request_params))
+            request_query_params = list(filter(lambda x: x.get('in') == 'query', request_params))
+            path_params_in_body = list(filter(lambda x: x.get('in') == 'path', request_params))
+            
+
+            # handle path params from path_params
+            # and replace path params by value in 
+            # endpoint path
+            endpoint_path:str = path_obj.get('path')
+            path_params = path_obj.get('path_params',[])
+            path_params += path_params_in_body
+            path_params = fill_params(path_params)
+            # print(path_params)
+            # print('-'*30)
+
+
+            for path_param in path_params:
+                path_param_name = path_param.get('name')
+                path_param_value = path_param.get('value')
+                endpoint_path = endpoint_path.replace('{' + str(path_param_name) + '}', str(path_param_value))
+
+
+            tasks.append({
+                'test_name':'BOLA Path Test with Fuzzed Params',
+                'url': f'{base_url}{endpoint_path}',
+                'endpoint': path_obj.get('path'),
+                'method': path_obj.get('http_method').upper(),
+                'body_params':request_body_params,
+                'query_params':request_query_params,
+                # 'malicious_payload':path_params,  
+            })
+
+        return tasks
     
+
     def __inject_sqli_payload_in_params(self, request_params:list[dict], sqli_payload:str):
         """
         Injects SQL injection (SQLi) payload into the request parameters.
 
         This method modifies the provided request parameters by injecting the SQLi payload.
 
         Args:
             request_params (list[dict]): A list of dictionaries representing the request parameters.
             sqli_payload (str): The SQL injection payload to be injected into the request parameters.
 
         Returns:
             list: returns list of sqli injection parameters for API testing
         """
-        malicious_params = []
-        request_params = self.__get_request_params_list(request_params)
-
-        # filter params with string value 
-        # TODO: we're missing out required params here, 
-        # required param should be considered
-        request_params = list(filter(lambda param: param.get('required')==True or param.get('type')=='string', request_params))
-
+        request_params = deepcopy(request_params)
+    
         # inject sqli payload as param value
         for request_param_data in request_params:
+            # TODO: inject sqli payloads in other data types as well
             if request_param_data.get('type') == 'string':
-                new_request = deepcopy(request_param_data)
-                new_request['value'] = sqli_payload
-                malicious_params.append(new_request)
+                request_param_data['value'] = sqli_payload
 
-        return malicious_params
+        return request_params
         
 
     def sqli_fuzz_params_test(
             self,
             openapi_parser:OpenAPIParser,
-            success_codes:list[int]=[403,405,500],
+            success_codes:list[int]=[500],
             *args,
             **kwargs
     ):
         '''Performs SQL injection (SQLi) parameter fuzzing based on the provided OpenAPIParser instance.
     
         Args:
             openapi_parser (OpenAPIParser): An instance of the OpenAPIParser class containing the parsed OpenAPI specification.
@@ -165,62 +215,61 @@
         
         Returns:
             List: List of dictionaries containing tests for SQLi
         
         Raises:
             Any exceptions raised during the execution.
         '''
-        base_url:str = openapi_parser.base_url
-        request_response_params:dict = openapi_parser.request_response_params
 
         # APPROACH: first send sqli in all params, if error is generated
         # then enumerate one by one or ask user to pentest manually using
         # sqlmap
         tasks = []
         basic_sqli_payloads = [
             "' OR 1=1 ;--",
             "' UNION SELECT 1,2,3 -- -",
             "' OR '1'='1--",
             "' AND (SELECT * FROM (SELECT(SLEEP(5)))abc)",
             "' AND SLEEP(5) --",
         ]
 
-        # TODO: handle path params in future
-        # NOTE: skip paths containing in path variables and no body params for now!!.
-        request_response_params = list(filter(lambda x: len(x.get('path_params',[]))==0 and len(x.get('request_params',[]))>0, request_response_params))
+        fuzzed_request_list = self.__fuzz_request_params(openapi_parser)
 
         # inject SQLi payloads in string variables
         for sqli_payload in basic_sqli_payloads:
-            for request_obj in request_response_params:
-                request_params = request_obj.get('request_params',[])
-                request_path = request_obj.get('path',[])
-
-                malicious_request_params = self.__inject_sqli_payload_in_params(request_params, sqli_payload)
+            for request_obj in fuzzed_request_list:
+                # handle body request params
+                body_request_params = request_obj.get('body_params',[])
+                malicious_body_request_params = self.__inject_sqli_payload_in_params(body_request_params, sqli_payload)
+
+                # handle query request params
+                query_request_params = request_obj.get('query_params',[])
+                malicious_query_request_params = self.__inject_sqli_payload_in_params(query_request_params, sqli_payload)
 
-                tasks.append({
-                    'test_name':'SQLi Test',
-                    'url': f'{base_url}{request_path}',
-                    'endpoint': request_path,
-                    'method': request_obj.get('http_method').upper(),
-                    'body_params':malicious_request_params,
-                    'malicious_payload':sqli_payload,
-                    'args': args,
-                    'kwargs': kwargs,
-                    'result_details':{
-                        True:'Parameters are not vulnerable to SQLi Payload', # passed
-                        False:'One or more parameter is vulnerable to SQL Injection Attack', # failed
-                    },
-                    'success_codes':success_codes,
-                    'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER.name
-                })
+                request_obj['test_name'] = 'SQLi Test'
+                
+                request_obj['body_params'] = malicious_body_request_params
+                request_obj['query_params'] = malicious_query_request_params
+                request_obj['args'] = args
+                request_obj['kwargs'] = kwargs
+                
+                request_obj['malicious_payload'] = sqli_payload
+                
+                request_obj['result_details'] = {
+                    True:'Parameters are not vulnerable to SQLi Payload', # passed
+                    False:'One or more parameter is vulnerable to SQL Injection Attack', # failed
+                }
+                request_obj['success_codes'] = success_codes
+                request_obj['response_filter'] = TestRunnerFiltersEnum.STATUS_CODE_FILTER.name
+                tasks.append(deepcopy(request_obj))
 
         return tasks
     
 
-    def bola_path_test(
+    def bola_fuzz_path_test(
             self,
             openapi_parser:OpenAPIParser,
             success_codes:list[int]=[200, 201, 301],
             *args,
             **kwargs
     ):
         '''Generate Tests for BOLA in endpoint path
@@ -236,17 +285,14 @@
         
         Raises:
             Any exceptions raised during the execution.
         '''
         base_url:str = openapi_parser.base_url
         request_response_params:list[dict] = openapi_parser.request_response_params
 
-        # get request params list
-        # request_params_list = list(map(lambda x: self.__get_request_params_list(x.get('request_params',[])), request_response_params))
-
         # filter path containing params in path
         endpoints_with_param_in_path = list(filter(lambda path_obj: '/{' in path_obj.get('path'), request_response_params))
 
         tasks = []
         for path_obj in endpoints_with_param_in_path:
             # handle path params from request_params
             request_params = path_obj.get('request_params',[])
@@ -261,27 +307,29 @@
             # endpoint path
             endpoint_path:str = path_obj.get('path')
 
             path_params = path_obj.get('path_params',[])
             path_params_in_body = list(filter(lambda x: x.get('in') == 'path', request_params))
             path_params += path_params_in_body
             path_params = fill_params(path_params)
+            # print(path_params)
+            # print('-'*30)
 
             for path_param in path_params:
                 path_param_name = path_param.get('name')
                 path_param_value = path_param.get('value')
                 endpoint_path = endpoint_path.replace('{' + str(path_param_name) + '}', str(path_param_value))
 
             # TODO: handle request query params
             request_query_params = list(filter(lambda x: x.get('in') == 'query', request_params))
             # print(request_query_params)
             # print('-'*30)
 
             tasks.append({
-                'test_name':'BOLA Path Test',
+                'test_name':'BOLA Path Test with Fuzzed Params',
                 'url': f'{base_url}{endpoint_path}',
                 'endpoint': path_obj.get('path'),
                 'method': path_obj.get('http_method').upper(),
                 'body_params':request_body_params,
                 'query_params':request_query_params,
                 'malicious_payload':path_params,
                 'args': args,
@@ -293,7 +341,87 @@
                 'success_codes':success_codes,
                 'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER.name
             })
 
         return tasks
     
 
+    def bola_fuzz_trailing_slash_path_test(
+            self,
+            openapi_parser:OpenAPIParser,
+            success_codes:list[int]=[200, 201, 301],
+            *args,
+            **kwargs
+    ):
+        '''Generate Tests for BOLA in endpoint path
+        
+        Args:
+            openapi_parser (OpenAPIParser): An instance of the OpenAPIParser class containing the parsed OpenAPI specification.
+            success_codes (list[int], optional): A list of HTTP success codes to consider as successful BOLA responses. Defaults to [200, 201, 301].
+            *args: Variable-length positional arguments.
+            **kwargs: Arbitrary keyword arguments.
+        
+        Returns:
+            list[dict]: list of dict containing test case for endpoint
+        
+        Raises:
+            Any exceptions raised during the execution.
+        '''
+        base_url:str = openapi_parser.base_url
+        request_response_params:list[dict] = openapi_parser.request_response_params
+
+        tasks = []
+        for path_obj in request_response_params:
+            # handle path params from request_params
+            request_params = path_obj.get('request_params',[])
+            request_params = fill_params(request_params)
+
+            # get params based on their position in request
+            request_body_params = list(filter(lambda x: x.get('in') == 'body', request_params))
+            request_query_params = list(filter(lambda x: x.get('in') == 'query', request_params))
+            path_params_in_body = list(filter(lambda x: x.get('in') == 'path', request_params))
+            
+
+            # handle path params from path_params
+            # and replace path params by value in 
+            # endpoint path
+            endpoint_path:str = path_obj.get('path')
+            path_params = path_obj.get('path_params',[])
+            path_params += path_params_in_body
+            path_params = fill_params(path_params)
+            # print(path_params)
+            # print('-'*30)
+
+
+            for path_param in path_params:
+                path_param_name = path_param.get('name')
+                path_param_value = path_param.get('value')
+                endpoint_path = endpoint_path.replace('{' + str(path_param_name) + '}', str(path_param_value))
+
+            # generate URL for BOLA attack
+            url = f'{base_url}{endpoint_path}'
+            if url.endswith('/'):
+                url = f'{url}{generate_random_int()}'
+            else:
+                url = f'{url}/{generate_random_int()}'
+            
+
+            tasks.append({
+                'test_name':'BOLA Path Trailing Slash Test',
+                'url': url,
+                'endpoint': path_obj.get('path'),
+                'method': path_obj.get('http_method').upper(),
+                'body_params':request_body_params,
+                'query_params':request_query_params,
+                'path_params':path_params,
+                'malicious_payload':[],
+                'args': args,
+                'kwargs': kwargs,
+                'result_details':{
+                    True:'Endpoint might not vulnerable to BOLA', # passed
+                    False:'Endpoint might be vulnerable to BOLA', # failed
+                },
+                'success_codes':success_codes,
+                'response_filter': TestRunnerFiltersEnum.STATUS_CODE_FILTER.name
+            })
+
+        return tasks
```

### Comparing `offat-0.4.0/offat/tester/test_runner.py` & `offat-0.5.0/offat/tester/test_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         http_method = test_task.get('method')
         success_codes = test_task.get('success_codes', [200, 301])
         args = test_task.get('args')
         kwargs = test_task.get('kwargs')
         body_params = test_task.get('body_params')
         query_params = test_task.get('query_params')
 
-        if body_params:
+        if body_params and str(http_method).upper() not in ['GET', 'OPTIONS']:
             kwargs['json'] = self._generate_payloads(body_params, payload_for=PayloadFor.BODY)
 
         if query_params:
             kwargs['params'] = self._generate_payloads(query_params, payload_for=PayloadFor.QUERY)
 
         try:
             response = await self._client.request(url=url, method=http_method, *args, **kwargs)
@@ -93,20 +93,24 @@
         test_result = test_task
         if isinstance(response, dict) and response.get('status') in success_codes:
             result = False # test failed
         else:
             result = True # test passed
         test_result['result'] = result
         test_result['result_details'] = test_result['result_details'].get(result)
+
+        # add request headers to result
+        test_result['request_headers'] = response.get('req_headers',[])
         
         # append response headers and body for analyzing data leak
         res_body = response.get('res_body', 'No Response Body Found')
         test_result['response_headers'] = response.get('res_headers')
         test_result['response_body'] = res_body
         test_result['response_status_code'] = response.get('status')
+        test_result['redirection'] = response.get('res_redirection', '')
 
         # run data leak test
         data_exposures_dict = detect_data_exposure(str(res_body))
         test_result['data_leak'] = data_exposures_dict
 
         # if data_exposures_dict:
             # print(res_body)
```

### Comparing `offat-0.4.0/offat/tester/tester_utils.py` & `offat-0.5.0/offat/tester/tester_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 from ..openapi import OpenAPIParser
 from ..utils import write_json_to_file
 
 
 logger = create_logger(__name__)
 
 # create tester objs
-test_runner = TestRunner()
 test_table_generator = TestResultTable()
 test_generator = TestGenerator()
 
 
-def run_test(tests:list[dict], regex_pattern:str=None) -> list:
+def run_test(test_runner:TestRunner, tests:list[dict], regex_pattern:str=None) -> list:
     '''Run tests and print result on console'''
-    global test_runner, test_table_generator
+    global test_table_generator
 
     # filter data if regex is passed
     if regex_pattern:
         tests = list(
             filter(
                 lambda x: regex_search(regex_pattern, x.get('endpoint','')),
                 tests 
@@ -32,34 +31,47 @@
 
     test_results = run(test_runner.run_tests(tests))
     results = test_table_generator.generate_result_table(deepcopy(test_results))
     print(results)
     return test_results
 
  
-def generate_and_run_tests(api_parser:OpenAPIParser, regex_pattern:str=None, output_file:str=None):
-    global test_runner, test_table_generator, logger
+def generate_and_run_tests(api_parser:OpenAPIParser, regex_pattern:str=None, output_file:str=None, rate_limit:int=None,delay:float=None,req_headers:dict=None):
+    global test_table_generator, logger
 
+    test_runner = TestRunner(
+        rate_limit=rate_limit,
+        delay=delay,
+        headers=req_headers
+    )
+    
     results:list = []
 
     # test for unsupported http methods
     logger.info('Checking for Unsupported HTTP methods:')
     unsupported_http_endpoint_tests = test_generator.check_unsupported_http_methods(api_parser.base_url, api_parser._get_endpoints())
-    results += run_test(tests=unsupported_http_endpoint_tests, regex_pattern=regex_pattern)
+    results += run_test(test_runner=test_runner, tests=unsupported_http_endpoint_tests, regex_pattern=regex_pattern)
 
     # sqli fuzz test
     logger.info('Checking for SQLi vulnerability:')
     sqli_fuzz_tests = test_generator.sqli_fuzz_params_test(api_parser)
-    results += run_test(tests=sqli_fuzz_tests, regex_pattern=regex_pattern)
+    results += run_test(test_runner=test_runner, tests=sqli_fuzz_tests, regex_pattern=regex_pattern)
    
-    # BOLA path tests
-    logger.info('Checking for BOLA in PATH:')
-    bola_path_tests = test_generator.bola_path_test(api_parser, success_codes=[200, 201, 301])
-    results += run_test(tests=bola_path_tests, regex_pattern=regex_pattern)
+    # BOLA path tests with fuzzed data
+    logger.info('Checking for BOLA in PATH using fuzzed params:')
+    bola_fuzzed_path_tests = test_generator.bola_fuzz_path_test(api_parser, success_codes=[200, 201, 301])
+    results += run_test(test_runner=test_runner, tests=bola_fuzzed_path_tests, regex_pattern=regex_pattern)
+
+    # BOLA path test with fuzzed data + trailing slash
+    logger.info('Checking for BOLA in PATH with trailing slash and id using fuzzed params :')
+    bola_trailing_slash_path_tests = test_generator.bola_fuzz_trailing_slash_path_test(api_parser, success_codes=[200, 201, 301])
+    results += run_test(test_runner=test_runner, tests=bola_trailing_slash_path_tests, regex_pattern=regex_pattern)
 
     if output_file:
         write_json_to_file(
             json_data={
                 'results':results
             }, 
             file_path=output_file
         )
+
+
```

### Comparing `offat-0.4.0/pyproject.toml` & `offat-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "offat"
-version = "0.4.0"
+version = "0.5.0"
 description = "Offensive API tester tool automates checks for common API vulnerabilities"
 authors = ["Dhrumil Mistry <56185972+dmdhrumilmistry@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `offat-0.4.0/PKG-INFO` & `offat-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: offat
-Version: 0.4.0
+Version: 0.5.0
 Summary: Offensive API tester tool automates checks for common API vulnerabilities
 License: MIT
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 Project-URL: Support, https://github.com/sponsors/dmdhrumilmistry/
 Description-Content-Type: text/markdown
 
 # OFFAT - OFFensive Api Tester
 
 Automatically Tests for vulnerabilities after generating tests from openapi specification file. Project is in Beta stage, so sometimes it might crash while running.
 
-![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-test-undocumented-api-endpoint-http-method.png)
+![UnDocumented petstore API endpoint HTTP method results](./.images/tests/offat-v0.5.0.png)
 
 ## Features
 
 - [X] Restricted HTTP Methods
 - [X] SQLi
 - [X] BOLA (Might need few bug fixes)
 - [X] Data Exposure (Detects Common Data Exposures)
@@ -123,14 +123,30 @@
 
 - Run tests only for endpoint paths matching regex pattern
 
   ```bash
   offat -f swagger_file.json -pr '/user'
   ```
 
+- Add headers to requests
+
+  ```bash
+  offat -f swagger_file.json -H 'Accept: application/json' -H 'Authorization: Bearer YourJWTToken'
+  ```
+
+- Run Test with Requests Rate Limited
+
+  ```bash
+  offat -f swagger_file.json -rl 1000 -dr 0.001
+  ```
+
+  > `rl`: requests rate limit, `dr`: delay between requests
+
+
+
 > If you're using Termux or windows, then use `pip` instead of `pip3`.  
 > Few features are only for linux os, hence they might not work on windows and require admin priviliges.
 
 ### Open In Google Cloud Shell
 
 - Temporary Session  
   [![Open in Cloud Shell](https://gstatic.com/cloudssh/images/open-btn.svg)](https://shell.cloud.google.com/cloudshell/editor?cloudshell_git_repo=https://github.com/dmdhrumilmistry/offat.git&ephemeral=true&show=terminal&cloudshell_print=./DISCLAIMER.md)
```

