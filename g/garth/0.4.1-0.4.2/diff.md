# Comparing `tmp/garth-0.4.1.tar.gz` & `tmp/garth-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garth-0.4.1.tar", last modified: Fri Aug  4 20:53:46 2023, max compression
+gzip compressed data, was "garth-0.4.2.tar", last modified: Fri Aug  4 21:43:39 2023, max compression
```

## Comparing `garth-0.4.1.tar` & `garth-0.4.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.1/LICENSE
--rw-r--r--   0        0        0    13332 2023-08-01 00:53:50.423067 garth-0.4.1/README.md
--rw-r--r--   0        0        0      679 2023-08-01 00:53:18.694307 garth-0.4.1/garth/__init__.py
--rw-r--r--   0        0        0      796 2023-08-04 15:13:28.651836 garth-0.4.1/garth/auth_tokens.py
--rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.4.1/garth/exc.py
--rw-r--r--   0        0        0     4922 2023-08-04 05:03:14.761571 garth-0.4.1/garth/http.py
--rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.1/garth/py.typed
--rw-r--r--   0        0        0     4565 2023-08-04 20:40:51.804547 garth-0.4.1/garth/sso.py
--rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.1/garth/stats/__init__.py
--rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.1/garth/stats/_base.py
--rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.1/garth/stats/hrv.py
--rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.1/garth/stats/intensity_minutes.py
--rw-r--r--   0        0        0     3523 2023-08-01 01:10:51.104099 garth-0.4.1/garth/stats/sleep.py
--rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.1/garth/stats/steps.py
--rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.1/garth/stats/stress.py
--rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.1/garth/utils.py
--rw-r--r--   0        0        0       22 2023-08-04 20:53:30.325813 garth-0.4.1/garth/version.py
--rw-r--r--   0        0        0     1221 2023-08-04 20:53:46.447734 garth-0.4.1/pyproject.toml
--rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.1/tests/cassettes/test_client_request.yaml
--rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.1/tests/cassettes/test_connectapi.yaml
--rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.1/tests/cassettes/test_exchange.yaml
--rw-r--r--   0        0        0    50571 2023-08-04 01:10:15.051257 garth-0.4.1/tests/cassettes/test_login_email_password_fail.yaml
--rw-r--r--   0        0        0    71237 2023-08-04 20:44:41.137445 garth-0.4.1/tests/cassettes/test_login_success_mfa.yaml
--rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.1/tests/cassettes/test_username.yaml
--rw-r--r--   0        0        0     3605 2023-08-04 15:10:55.580644 garth-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.1/tests/stats/cassettes/test_daily_hrv.yaml
--rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.1/tests/stats/cassettes/test_daily_hrv_no_results.yaml
--rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.1/tests/stats/cassettes/test_daily_hrv_paginate.yaml
--rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.1/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
--rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.1/tests/stats/cassettes/test_daily_intensity_minutes.yaml
--rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.1/tests/stats/cassettes/test_daily_sleep.yaml
--rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.1/tests/stats/cassettes/test_daily_steps.yaml
--rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.1/tests/stats/cassettes/test_daily_stress.yaml
--rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.1/tests/stats/cassettes/test_daily_stress_pagination.yaml
--rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.1/tests/stats/cassettes/test_sleep_data_get.yaml
--rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.1/tests/stats/cassettes/test_sleep_data_list.yaml
--rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.1/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
--rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.1/tests/stats/cassettes/test_weekly_steps.yaml
--rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.1/tests/stats/cassettes/test_weekly_stress.yaml
--rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.1/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
--rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.1/tests/stats/cassettes/test_weekly_stress_pagination.yaml
--rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.1/tests/stats/test_hrv.py
--rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.1/tests/stats/test_intensity_minutes.py
--rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.4.1/tests/stats/test_sleep.py
--rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.1/tests/stats/test_steps.py
--rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.1/tests/stats/test_stress.py
--rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.1/tests/test_auth_tokens.py
--rw-r--r--   0        0        0     3335 2023-08-04 20:42:44.643135 garth-0.4.1/tests/test_http.py
--rw-r--r--   0        0        0     2402 2023-08-04 20:44:58.232522 garth-0.4.1/tests/test_sso.py
--rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.1/tests/test_utils.py
--rw-r--r--   0        0        0    13784 1970-01-01 00:00:00.000000 garth-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 12:44:00.130760 garth-0.4.2/LICENSE
+-rw-r--r--   0        0        0    13332 2023-08-01 00:53:50.423067 garth-0.4.2/README.md
+-rw-r--r--   0        0        0      679 2023-08-01 00:53:18.694307 garth-0.4.2/garth/__init__.py
+-rw-r--r--   0        0        0      796 2023-08-04 15:13:28.651836 garth-0.4.2/garth/auth_tokens.py
+-rw-r--r--   0        0        0      145 2023-07-18 22:32:58.010661 garth-0.4.2/garth/exc.py
+-rw-r--r--   0        0        0     4922 2023-08-04 05:03:14.761571 garth-0.4.2/garth/http.py
+-rw-r--r--   0        0        0        0 2023-07-27 13:16:10.642595 garth-0.4.2/garth/py.typed
+-rw-r--r--   0        0        0     4656 2023-08-04 21:42:16.200457 garth-0.4.2/garth/sso.py
+-rw-r--r--   0        0        0      434 2023-07-30 01:10:27.575730 garth-0.4.2/garth/stats/__init__.py
+-rw-r--r--   0        0        0     1531 2023-08-01 00:53:16.612824 garth-0.4.2/garth/stats/_base.py
+-rw-r--r--   0        0        0     1726 2023-07-30 04:26:19.317148 garth-0.4.2/garth/stats/hrv.py
+-rw-r--r--   0        0        0      611 2023-08-01 00:53:21.402342 garth-0.4.2/garth/stats/intensity_minutes.py
+-rw-r--r--   0        0        0     3523 2023-08-01 01:10:51.104099 garth-0.4.2/garth/stats/sleep.py
+-rw-r--r--   0        0        0      653 2023-08-01 00:53:20.538257 garth-0.4.2/garth/stats/steps.py
+-rw-r--r--   0        0        0      652 2023-08-01 00:53:19.922467 garth-0.4.2/garth/stats/stress.py
+-rw-r--r--   0        0        0     1767 2023-08-04 01:10:15.047656 garth-0.4.2/garth/utils.py
+-rw-r--r--   0        0        0       22 2023-08-04 21:43:18.587257 garth-0.4.2/garth/version.py
+-rw-r--r--   0        0        0     1221 2023-08-04 21:43:39.480141 garth-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0   100792 2023-08-04 01:10:15.050440 garth-0.4.2/tests/cassettes/test_client_request.yaml
+-rw-r--r--   0        0        0     2602 2023-08-04 01:10:15.050693 garth-0.4.2/tests/cassettes/test_connectapi.yaml
+-rw-r--r--   0        0        0     3102 2023-08-04 03:43:23.879883 garth-0.4.2/tests/cassettes/test_exchange.yaml
+-rw-r--r--   0        0        0    50571 2023-08-04 01:10:15.051257 garth-0.4.2/tests/cassettes/test_login_email_password_fail.yaml
+-rw-r--r--   0        0        0    71303 2023-08-04 21:42:47.426240 garth-0.4.2/tests/cassettes/test_login_success_mfa.yaml
+-rw-r--r--   0        0        0     4883 2023-08-04 01:10:15.052284 garth-0.4.2/tests/cassettes/test_username.yaml
+-rw-r--r--   0        0        0     3605 2023-08-04 15:10:55.580644 garth-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0     8412 2023-08-04 01:10:15.052774 garth-0.4.2/tests/stats/cassettes/test_daily_hrv.yaml
+-rw-r--r--   0        0        0     1893 2023-08-04 01:10:15.052978 garth-0.4.2/tests/stats/cassettes/test_daily_hrv_no_results.yaml
+-rw-r--r--   0        0        0    16982 2023-08-04 01:10:15.053232 garth-0.4.2/tests/stats/cassettes/test_daily_hrv_paginate.yaml
+-rw-r--r--   0        0        0     1897 2023-08-04 01:10:15.053481 garth-0.4.2/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml
+-rw-r--r--   0        0        0     3926 2023-08-04 01:10:15.053705 garth-0.4.2/tests/stats/cassettes/test_daily_intensity_minutes.yaml
+-rw-r--r--   0        0        0     2759 2023-08-04 01:10:15.053918 garth-0.4.2/tests/stats/cassettes/test_daily_sleep.yaml
+-rw-r--r--   0        0        0     4067 2023-08-04 01:10:15.054145 garth-0.4.2/tests/stats/cassettes/test_daily_steps.yaml
+-rw-r--r--   0        0        0     6085 2023-08-04 01:10:15.054397 garth-0.4.2/tests/stats/cassettes/test_daily_stress.yaml
+-rw-r--r--   0        0        0    18594 2023-08-04 01:10:15.054680 garth-0.4.2/tests/stats/cassettes/test_daily_stress_pagination.yaml
+-rw-r--r--   0        0        0     8588 2023-08-04 01:10:15.054936 garth-0.4.2/tests/stats/cassettes/test_sleep_data_get.yaml
+-rw-r--r--   0        0        0    78725 2023-08-04 01:10:15.055303 garth-0.4.2/tests/stats/cassettes/test_sleep_data_list.yaml
+-rw-r--r--   0        0        0     3259 2023-08-04 01:10:15.055564 garth-0.4.2/tests/stats/cassettes/test_weekly_intensity_minutes.yaml
+-rw-r--r--   0        0        0    12946 2023-08-04 01:10:15.055800 garth-0.4.2/tests/stats/cassettes/test_weekly_steps.yaml
+-rw-r--r--   0        0        0     4552 2023-08-04 01:10:15.056039 garth-0.4.2/tests/stats/cassettes/test_weekly_stress.yaml
+-rw-r--r--   0        0        0    15357 2023-08-04 01:10:15.056262 garth-0.4.2/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml
+-rw-r--r--   0        0        0     7120 2023-08-04 01:10:15.056491 garth-0.4.2/tests/stats/cassettes/test_weekly_stress_pagination.yaml
+-rw-r--r--   0        0        0     1001 2023-07-30 04:28:17.698327 garth-0.4.2/tests/stats/test_hrv.py
+-rw-r--r--   0        0        0      748 2023-07-29 23:40:27.912636 garth-0.4.2/tests/stats/test_intensity_minutes.py
+-rw-r--r--   0        0        0      849 2023-07-28 12:22:22.098284 garth-0.4.2/tests/stats/test_sleep.py
+-rw-r--r--   0        0        0      667 2023-07-29 17:53:35.423973 garth-0.4.2/tests/stats/test_steps.py
+-rw-r--r--   0        0        0     1437 2023-07-27 13:31:20.424008 garth-0.4.2/tests/stats/test_stress.py
+-rw-r--r--   0        0        0      455 2023-08-04 01:10:15.056632 garth-0.4.2/tests/test_auth_tokens.py
+-rw-r--r--   0        0        0     3335 2023-08-04 20:54:03.315578 garth-0.4.2/tests/test_http.py
+-rw-r--r--   0        0        0     2402 2023-08-04 21:43:02.079480 garth-0.4.2/tests/test_sso.py
+-rw-r--r--   0        0        0     1655 2023-08-04 04:10:40.202147 garth-0.4.2/tests/test_utils.py
+-rw-r--r--   0        0        0    13784 1970-01-01 00:00:00.000000 garth-0.4.2/PKG-INFO
```

### Comparing `garth-0.4.1/LICENSE` & `garth-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/README.md` & `garth-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/garth/__init__.py` & `garth-0.4.2/garth/__init__.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/garth/auth_tokens.py` & `garth-0.4.2/garth/auth_tokens.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/garth/http.py` & `garth-0.4.2/garth/http.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/garth/sso.py` & `garth-0.4.2/garth/sso.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,18 +111,20 @@
 
 
 def exchange(oauth1: OAuth1Token, client: "http.Client") -> OAuth2Token:
     sess = GarminOAuth1Session(
         resource_owner_key=oauth1.oauth_token,
         resource_owner_secret=oauth1.oauth_token_secret,
     )
+    data = dict(mfa_token=oauth1.mfa_token) if oauth1.mfa_token else {}
     token = sess.post(
         "https://connectapi.garmin.com/oauth-service/oauth/exchange/user/2.0",
         headers=USER_AGENT
         | {"Content-Type": "application/x-www-form-urlencoded"},
+        data=data,
     ).json()
 
     return OAuth2Token(**set_expirations(token))
 
 
 def handle_mfa(client: "http.Client", signin_params: dict) -> None:
     csrf_token = get_csrf_token(client.last_resp.text)
```

### Comparing `garth-0.4.1/garth/stats/_base.py` & `garth-0.4.2/garth/stats/_base.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/garth/stats/hrv.py` & `garth-0.4.2/garth/stats/hrv.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/garth/stats/intensity_minutes.py` & `garth-0.4.2/garth/stats/intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/garth/stats/sleep.py` & `garth-0.4.2/garth/stats/sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/garth/stats/steps.py` & `garth-0.4.2/garth/stats/steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/garth/stats/stress.py` & `garth-0.4.2/garth/stats/stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/garth/utils.py` & `garth-0.4.2/garth/utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/pyproject.toml` & `garth-0.4.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
 ]
 packages = [
     { include = "garth" },
 ]
-version = "0.4.1"
+version = "0.4.2"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `garth-0.4.1/tests/cassettes/test_client_request.yaml` & `garth-0.4.2/tests/cassettes/test_client_request.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/cassettes/test_connectapi.yaml` & `garth-0.4.2/tests/cassettes/test_connectapi.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/cassettes/test_exchange.yaml` & `garth-0.4.2/tests/cassettes/test_exchange.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/cassettes/test_login_email_password_fail.yaml` & `garth-0.4.2/tests/cassettes/test_login_email_password_fail.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/cassettes/test_login_success_mfa.yaml` & `garth-0.4.2/tests/cassettes/test_login_success_mfa.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         a multi factor authentication check. (Only valid for an already logged in
         user.)\n\trememberMyBrowserShown          No  true/false (Default value is
         false)                      Whether the \"Remember My Browser\" check box
         is shown in the GAuth login widget MFA verification screen.\n\trememberMyBrowserChecked
         \       No  true/false (Default value is false)                      Whether
         the \"Remember My Browser\" check box feature is checked by default.\n\tconsentTypeIds\t\t\t\t\tNo\tconsent_types
         ids\t\t \t\t\t\t\t\t\t\t multiple consent types ids can be passed as consentTypeIds=type1&consentTypeIds=type2\n\t</pre>\n</div>\n\n\n\t<script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7f19a351192546a1'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f19f84d2d2047a4'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -155,49 +155,49 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7f19a351192546a1-DFW
+      - 7f19f84d2d2047a4-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Fri, 04 Aug 2023 20:44:22 GMT
+      - Fri, 04 Aug 2023 21:42:23 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=ytG3iKzcFS5%2B99VJD7%2FtqNm2w0E8GcBl0PO%2FS5qsCmdfQkBSJ6ekYSPKRo4ICSZ7qTGOe0aGYYvlGTJhYzx4Z5A46RMoBaAS2EdJ0JfNbriBi4n6TElpPegnmwjqc7Hj"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=zvXYngpt%2FM66%2Fz9gI0xFgQkzoTIocpc3OGEfkncJ37tBwN57jD%2B09JoWPKA%2BcR75KbtbFv7%2FwUMueVpsMUkKalOfkWJqWd9CZJvR9dmZYBgUP2HbcZR8pURmJPN48%2F9J"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - __cf_bm=SANITIZED; path=SANITIZED; expires=SANITIZED; domain=SANITIZED; HttpOnly;
         Secure; SameSite=SANITIZED
       - __cflb=SANITIZED; SameSite=SANITIZED; Secure; path=SANITIZED; expires=SANITIZED;
         HttpOnly
       - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
       X-Application-Context:
-      - casServer:cloud,prod,prod-US_1102:2
+      - casServer:cloud,prod,prod-US_1102:5
       X-B3-Traceid:
-      - 7de36dd29fa2d733290a6725dc47dfb8
+      - 6ca6b8ec7d365a895ef418b6319455ad
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - f780910f-ccdf-4771-49c7-aad225e3c68d
+      - ce3465b6-c1f7-4274-7cea-5812380e0fc9
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
@@ -307,15 +307,15 @@
         \                           <label for=\"password\">Password</label>\n                            <a
         id=\"loginforgotpassword\" class=\"login-forgot-password\" style=\"cursor:pointer\">(Forgot?)</a>\n
         \                           <input type=\"password\" name=\"password\" id=\"password\"
         spellcheck=\"false\" autocorrect=\"off\" autocapitalize=\"off\" />\n                             <strong
         id=\"capslock-warning\" class=\"information\" title=\"Caps lock is on.\" style=\"display:
         none;\">Caps lock is on.</strong>\n\t\t\t\t\t    </div>\n                        <input
         type=\"hidden\" name=\"embed\" value=\"false\"/>\n                        <input
-        type=\"hidden\" name=\"_csrf\" value=\"884C8386EF425D4BA55B54C0B893A3B750BFD7FC791A34EC0BA934444EC04CE6B1FA7484E35E2DF94006783318F9980B7A3A\"
+        type=\"hidden\" name=\"_csrf\" value=\"8FD1312E0D2A8A6D81CFF06E3ECFC06500351F8735530EBCE4F75FCB1A63EF6E8444F31A1CB9774C56E57C2C363807E8FF33\"
         />\n                        <button type=\"submit\" id=\"login-btn-signin\"
         class=\"btn1\" accesskey=\"l\">Sign In</button>\n                        \n\n\n
         \                       <!-- The existence of the \"rememberme\" parameter
         at all will remember the user! -->\n                        \n\n                    </form>\n
         \               </div>\n                <!-- end login form -->\n\n                <!--
         begin Create Account message -->\n\t            <div id=\"login-create-account\">\n\t
         \               \n\t            </div>\n\t            <!-- end Create Account
@@ -333,15 +333,15 @@
         Otherwise focus them in the username field of the login dialog.\n                    jQuery(\"#username\").focus();\n
         \               }\n\n                // Scroll to top of iframe to fix problem
         where Firefox 3.0-3.6 browsers initially show top of iframe cutoff.\n                location.href=\"#\";\n\n
         \               if(!embedWidget){\n                \tjQuery('.createAccountLink').click(function(){\n\t
         \                   send({'openLiteBox':'createAccountLink', 'popupUrl': createAccountConfigURL,
         'popupTitle':'Create An Account', 'clientId':clientId});\n\t                });\n
         \               }\n            });\n        </script>\n    <script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7f19a3536a19468a'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f19f84e7fa8b6e8'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -357,53 +357,53 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7f19a3536a19468a-DFW
+      - 7f19f84e7fa8b6e8-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Fri, 04 Aug 2023 20:44:23 GMT
+      - Fri, 04 Aug 2023 21:42:23 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=%2FFRtmPmaDfGDypVhatXfunnrGA%2BA8%2FxV6e%2BuekUdoE5fp2JNEw4bdoizvGG90r1BbOkbo3Ux5ybFDdoX4bKGqoKZWemHOBRFCYnaxHW3Ewoy9EHnNXohVMAu47T3dGnV"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=vC5EgD2UglMkkfFYe73MTEAE%2Ba%2BwXEfO1fjtmIdd0szIyodAnJpcate6PdHLtQdup9QOd%2F3QsAS5I0UwloNcZnT3gCBvs%2BOglqOmgC2YYJhOHmbrNHAlh%2FhQdk0Bc4XV"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - SESSION=SANITIZED; Path=SANITIZED; Secure; HttpOnly
       - __VCAP_ID__=SANITIZED; Path=SANITIZED; HttpOnly; Secure
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Application-Context:
       - casServer:cloud,prod,prod-US_1102:7
       X-B3-Traceid:
-      - 66c4d064ee4981291e470a27733c75c8
+      - 23e25790497950af53ad870cb9a288b8
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 97a74fb2-172b-46bf-69fb-dc6d6ac7ca6b
+      - 0790e6ab-9635-4d69-6b8a-244cf044e56c
     status:
       code: 200
       message: OK
 - request:
-    body: username=SANITIZED&password=SANITIZED&embed=true&_csrf=884C8386EF425D4BA55B54C0B893A3B750BFD7FC791A34EC0BA934444EC04CE6B1FA7484E35E2DF94006783318F9980B7A3A
+    body: username=SANITIZED&password=SANITIZED&embed=true&_csrf=8FD1312E0D2A8A6D81CFF06E3ECFC06500351F8735530EBCE4F75FCB1A63EF6E8444F31A1CB9774C56E57C2C363807E8FF33
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
@@ -433,45 +433,45 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7f19a354dcda1547-QRO
+      - 7f19f84fd8d5154b-QRO
       Connection:
       - keep-alive
       Content-Language:
       - en
       Content-Length:
       - '0'
       Date:
-      - Fri, 04 Aug 2023 20:44:24 GMT
+      - Fri, 04 Aug 2023 21:42:25 GMT
       Location:
       - https://sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=tT3Bm66IlHoACTPEW5aaWCih7nnzM48aWyyucJvJmXCHD6IH9yzYzqrcuZRsM3bzCgO5iQl0GWdKr4pSX%2Bbww%2F1QQ2HgTgnaYSYzYE9M9%2BiXwO8Z9zPyD5ShoR5IaGGZ"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=tFguDXcU1G6XJJv%2BBcpNv3veY3trRFFdHZIhw4TIp60D4GyisC1Rp3K1v%2Bj%2Fcq4FuGh4LJaZA8UQLxCLAuJfHezU7jFSlTbZvV2qXbNxQ%2F7n0OtnJh2FuSrZzYLtIXUZ"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - __cfruid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Vary:
       - Accept-Encoding
       X-Application-Context:
       - casServer:cloud,prod,prod-US_1102:7
       X-B3-Traceid:
-      - 55b92cb20bd883142b4f3a21212f1a1c
+      - 2306946bb772deae0299aca0881a0afe
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 2993f7d4-157a-412b-4177-8315cd0e0f50
+      - 90ed387d-cabf-4049-4122-09090680db2b
     status:
       code: 302
       message: Found
 - request:
     body: null
     headers:
       Accept:
@@ -550,21 +550,21 @@
         \                       <div id=\"requestNewCodeWrapper\" class=\"requestNewCode\">\n
         \                           <a href=\"#\" id=\"newCode\">Request a new code</a>\n
         \                       </div>\n                        \n                        \n
         \                       <br>\n                            \n                        <br/>\n
         \                       <button type=\"submit\" id=\"mfa-verification-code-submit\"
         class=\"btn1\">Next</button>\n                    </div>\n                    <input
         type=\"hidden\" name=\"embed\"            value=\"\"/>\n                    <input
-        type=\"hidden\" name=\"_csrf\"            value=\"89E48A5A52FDC9A4B5C29D2918F619B337621D199A534539AAD83C0AA2AB17DAF3C4CF9F56195AEE3BCE4B6866A34928D8BF\"
+        type=\"hidden\" name=\"_csrf\"            value=\"F9C17B99B345D1989FF8805BC611547BEC7C8F3C4C3DD4EC32AB8B766A27731265986903FD84CB56F1A1CA270D1D598F1D6F\"
         />\n                    <input type=\"hidden\" name=\"fromPage\"            value=\"setupEnterMfaCode\"/>\n
         \                   <br/>\n                </form>\n            </div>\n            <div
         class=\"clearfix\"></div> <!-- Ensure that GAuth-component div's height is
         computed correctly. -->\n        </div>\n    </div>\n    <script type=\"text/javascript\">\n
         \       resizePageOnLoad(jQuery(\"#GAuth-component\").height());\n    </script>\n<script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7f19a35eadf64797'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f19f85a8a0846d4'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -580,49 +580,49 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7f19a35eadf64797-DFW
+      - 7f19f85a8a0846d4-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Fri, 04 Aug 2023 20:44:24 GMT
+      - Fri, 04 Aug 2023 21:42:25 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=Cx2KhXZ92%2Fc38BjEH2TJ8bKkuzKrXn7G4k2KBB4F77VUlfrRtd3Ma36EuNIuEwPKt0MbbTBkiKz6cmCVpLHL78Grb1yaW4qioaOhRpKmselHhTiRADUtZ986y6gwrMzF"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=vlAIfwLdw1RDwdV2miJoXWzSRPUIP0vka2ZV3M%2BpTKxZz%2F2bv%2FBHlFw0eOQ767Weo7hVAd9dM0d9VkbqussSgEMIYQ268IuyC8EfS2AzRvnQYhcWPAvkZuw%2Fxl6HzYh9"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       Transfer-Encoding:
       - chunked
       X-Application-Context:
       - casServer:cloud,prod,prod-US_1102:7
       X-B3-Traceid:
-      - 7af5fbfce51e803d25255d01c1881b84
+      - 0a3e2d17f07851c273668f7d119fdd2e
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - b3ef8bab-184d-4715-4701-3c7749dfb38d
+      - be07a1e9-4b86-4a15-4a39-c26e2e86dd49
     status:
       code: 200
       message: OK
 - request:
-    body: mfa-code=577212&embed=true&_csrf=89E48A5A52FDC9A4B5C29D2918F619B337621D199A534539AAD83C0AA2AB17DAF3C4CF9F56195AEE3BCE4B6866A34928D8BF&fromPage=setupEnterMfaCode
+    body: mfa-code=195893&embed=true&_csrf=F9C17B99B345D1989FF8805BC611547BEC7C8F3C4C3DD4EC32AB8B766A27731265986903FD84CB56F1A1CA270D1D598F1D6F&fromPage=setupEnterMfaCode
     headers:
       Accept:
       - '*/*'
       Accept-Encoding:
       - gzip, deflate
       Connection:
       - keep-alive
@@ -652,42 +652,42 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7f19a3b10f7a475e-DFW
+      - 7f19f8c8aff41557-QRO
       Connection:
       - keep-alive
       Content-Language:
       - en
       Content-Length:
       - '0'
       Date:
-      - Fri, 04 Aug 2023 20:44:38 GMT
+      - Fri, 04 Aug 2023 21:42:44 GMT
       Location:
-      - https://sso.garmin.com/sso/login?logintoken=VuQcJ7ivPg&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
+      - https://sso.garmin.com/sso/login?logintoken=PFID9Y5XoQ&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=NGgvN3mY6mMbca0W6oPgP77yYti09%2FRuMFbc%2B3TANMVXaqj0LqEANMWpu2bhQ3eP7bUp%2FJHcPil5lor7r%2FZj%2FeqlikvJC40NazuUT3fD0gr%2FhpkVtHuFxfupzOnFljZr"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=cUvppW2Waaho4sVepx4f%2BpBXljwio9Mr5vgx73I%2F2Z0A8qBX1eiBnQz%2Fi24%2BbKl74JW8QBFec2n4hSbX2xJgLE9ud3f1xdREl9jbvaIngvRcXsD4cUuqoLgm%2BP1f4iof"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       X-Application-Context:
       - casServer:cloud,prod,prod-US_1102:7
       X-B3-Traceid:
-      - 2da2090d89494ce45f9fac6d04602be8
+      - 0339eee8eb299f1c0626712d33b7683c
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - e7305dea-ccb7-422a-4d05-8e07ecb69277
+      - 013c5c74-8192-4e87-7be3-d293d92aa83e
     status:
       code: 302
       message: Found
 - request:
     body: null
     headers:
       Accept:
@@ -701,31 +701,31 @@
         __VCAP_ID__=SANITIZED; __cflb=SANITIZED; org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
       User-Agent:
       - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X) AppleWebKit/605.1.15
         (KHTML, like Gecko) Mobile/15E148
       referer:
       - https://sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
     method: GET
-    uri: https://sso.garmin.com/sso/login?logintoken=VuQcJ7ivPg&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
+    uri: https://sso.garmin.com/sso/login?logintoken=PFID9Y5XoQ&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
   response:
     body:
       string: "<!DOCTYPE html>\n<html class=\"no-js\">\n\t<head>\n\t\t<title>Success</title>\n\t\t<meta
         charset=\"utf-8\">\n\t\t<meta http-equiv=\"X-UA-Compatible\" content=\"IE=edge;\"
         />\n\t\t<meta name=\"description\" content=\"\">\n\t\t<meta name=\"viewport\"
         content=\"width=device-width, initial-scale=1\">\n\t\t<meta http-equiv=\"cleartype\"
         content=\"on\">\n\t\t<script type=\"text/javascript\" src=\"/sso/js/jquery/3.1.1/jquery.min.js?20210319\"></script>\n\t\t<script
         type=\"text/javascript\">jQuery.noConflict();</script>\n\t\t<script type=\"text/javascript\"
         src=\"/sso/js/json2.js\"></script>\n\t\t<script type=\"text/javascript\" src=\"/sso/js/consoleUtils.js?20210319\"></script>\n\t\t<script
         type=\"text/javascript\" src=\"/sso/js/postmessage.js?20210319\"></script>\n\t\t<script
         type=\"text/javascript\">\n\t\t\tvar redirectAfterAccountLoginUrl \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed\";\n\t\t\tvar
         redirectAfterAccountCreationUrl = \"\";\n\t\t\tvar consumeServiceTicket         \t
         \ = \"true\";\n\t\t\tvar service_url                  \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed\";\n\t\t\tvar
         parent_url                   \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed\";\n\t\t\tvar
-        response_url                 \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed?ticket=ST-2435197-JpeHGkPdeOMWbeob04zU-cas\";\n\t\t\tvar
-        logintoken                   \t  = \"VuQcJ7ivPg\";\n\t\t\tvar socialLogin
+        response_url                 \t  = \"https:\\/\\/sso.garmin.com\\/sso\\/embed?ticket=ST-2438674-btozWOKhrVdRH4PKUwah-cas\";\n\t\t\tvar
+        logintoken                   \t  = \"PFID9Y5XoQ\";\n\t\t\tvar socialLogin
         \                  \t  = \"\";\n\t\t\tvar performMFACheck                 =
         \"\";\n\n\t\t\t// Decode url if it's encoded unnecessarily (which is happening
         when SSO GAuth logins redisplay the login page due to session timeouts.)\n\t\t\tif
         (response_url.indexOf('%3A%2F%2F') != -1) {\n\t\t\t\tresponse_url = decodeURIComponent(response_url);\n\t\t\t}\n\t\t\tresponse_url
         = response_url.replace(new RegExp(\"&amp;\", 'g'),\"&\");\n\n\t\t\tvar service_ticket
         = response_url.substring(response_url.indexOf('ticket=') + 7, response_url.length);\n\n\t\t\tif
         (redirectAfterAccountLoginUrl) {\n\t\t\t\tconsoleInfo('casEmbedSuccess.html:
@@ -810,15 +810,15 @@
         userdata.country,\n\t\t\t\t\t\t\t\t\t\t\t'passwordChangeRequired' : userdata.passwordChangeRequired,\n\t\t\t\t\t\t\t\t\t\t\t'lastLogin'
         \             : userdata.lastLogin,\n\t\t\t\t\t\t\t\t\t\t\t'erpCustomerNumber'
         \     : userdata.erpCustomerNumber\n\t\t\t\t\t\t\t\t});\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t});\n\t\t\t\t\t}\n\t\t\t\t}\n\t\t\t}\n\t\t</script>\n\t</head>\n\t<body>\n\t\t<div
         id=\"GAuth-component\">\n\t\t\t<img src='/sso/images/ajax-loader.gif' class=\"loaderImage\"/>\n\t\t</div>\n\t\t<script
         type=\"text/javascript\">\n\t\t\tjQuery(document).ready(function(){\n\t\t\t\tvar
         service = \"https:\\/\\/sso.garmin.com\\/sso\\/embed\";\n\t\t\t\tconsoleInfo(\"casEmbedSuccess.html:
         ready, calling redirect('\" + service + \"')...\");\n\t\t\t\tredirect(service);\n\t\t\t});\n\t\t</script>\n\t<script>(function(){var
-        js = \"window['__CF$cv$params']={r:'7f19a3b83f801549'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
+        js = \"window['__CF$cv$params']={r:'7f19f8d24c9745e8'};_cpo=document.createElement('script');_cpo.nonce='',_cpo.src='/cdn-cgi/challenge-platform/scripts/invisible.js',document.getElementsByTagName('head')[0].appendChild(_cpo);\";var
         _0xh = document.createElement('iframe');_0xh.height = 1;_0xh.width = 1;_0xh.style.position
         = 'absolute';_0xh.style.top = 0;_0xh.style.left = 0;_0xh.style.border = 'none';_0xh.style.visibility
         = 'hidden';document.body.appendChild(_0xh);function handler() {var _0xi =
         _0xh.contentDocument || _0xh.contentWindow.document;if (_0xi) {var _0xj =
         _0xi.createElement('script');_0xj.innerHTML = js;_0xi.getElementsByTagName('head')[0].appendChild(_0xj);}}if
         (document.readyState !== 'loading') {handler();} else if (window.addEventListener)
         {document.addEventListener('DOMContentLoaded', handler);} else {var prev =
@@ -834,29 +834,29 @@
       Access-Control-Allow-Methods:
       - GET,POST,OPTIONS
       Access-Control-Allow-Origin:
       - https://www.garmin.com
       CF-Cache-Status:
       - DYNAMIC
       CF-Ray:
-      - 7f19a3b83f801549-QRO
+      - 7f19f8d24c9745e8-DFW
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Language:
       - en
       Content-Type:
       - text/html;charset=UTF-8
       Date:
-      - Fri, 04 Aug 2023 20:44:39 GMT
+      - Fri, 04 Aug 2023 21:42:45 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=imfmx6AwwEBoeOxkjGZH0%2Fuo7TerKPfAo3lexzqusMZoSuUvTb9NcJ%2ByyJcQ2tpq2ir22LFjOMkQL1I3GIaG3fryTvPe4zy0OUoN6zviNS23J9BNLEXkCIiTx381dS8m"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=mkKV3UBsbSn3e2rQHCFQRE14OiBbFa6u7cpCIcXy3QvaEvbDu8dCCamDRgjKkU%2FElrNOIvq2IG3JogUVOk2XT6UoxD4O59Nk0XIMOi4wHBKjb1GrAc5I34cz7VNebdaf"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
         Path=SANITIZED
       - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly
       - CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
@@ -883,19 +883,19 @@
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Application-Context:
       - casServer:cloud,prod,prod-US_1102:7
       X-B3-Traceid:
-      - 4fcf72f20e7a66dc13e58e89d1664544
+      - 782920201f8436216612583f8f870378
       X-Robots-Tag:
       - noindex
       X-Vcap-Request-Id:
-      - 6feb25a6-e44a-4549-47fa-75badeb102f8
+      - c796ecd4-094e-4657-479b-b1ab8bc1b185
     status:
       code: 200
       message: OK
 - request:
     body: null
     headers:
       Accept:
@@ -915,25 +915,25 @@
       Accept-Ranges:
       - bytes
       Content-Length:
       - '124'
       Content-Type:
       - application/json
       Date:
-      - Fri, 04 Aug 2023 20:44:40 GMT
+      - Fri, 04 Aug 2023 21:42:47 GMT
       ETag:
       - '"20240b1013cb35419bb5b2cff1407a4e"'
       Last-Modified:
       - Thu, 03 Aug 2023 00:16:11 GMT
       Server:
       - AmazonS3
       x-amz-id-2:
-      - /eMqmlK8obld8yP0MiiccJ5jEcyJNyjP5NUEl5p0NQ6WmCSo+GNI0sthWE+8i64u6u61lY+iJr4=
+      - cBp5mKgmX+Tjt0vISDuygu6J3/f6qZBCBlJCFl1gmUtHNNKgCK2hu4TiOCmoyIX+Hx16w5mDCeA=
       x-amz-request-id:
-      - 29FWE9MM7JBZB8MM
+      - WTDF5S9E2EP14K4Z
       x-amz-server-side-encryption:
       - AES256
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -949,64 +949,63 @@
       Connection:
       - !!binary |
         a2VlcC1hbGl2ZQ==
       User-Agent:
       - !!binary |
         Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ==
     method: GET
-    uri: https://connectapi.garmin.com/oauth-service/oauth/preauthorized?ticket=ST-2435197-JpeHGkPdeOMWbeob04zU-cas&login-url=https://sso.garmin.com/sso/embed&accepts-mfa-tokens=true
+    uri: https://connectapi.garmin.com/oauth-service/oauth/preauthorized?ticket=ST-2438674-btozWOKhrVdRH4PKUwah-cas&login-url=https://sso.garmin.com/sso/embed&accepts-mfa-tokens=true
   response:
     body:
       string: oauth_token=SANITIZED&oauth_token_secret=SANITIZED&mfa_token=SANITIZED&mfa_expiration_timestamp=2024-08-03
-        20:44:39.000
+        21:42:45.000
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7f19a3beb9b71557-QRO
+      - 7f19f8daecc2155f-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - text/plain;charset=utf-8
       Date:
-      - Fri, 04 Aug 2023 20:44:40 GMT
+      - Fri, 04 Aug 2023 21:42:46 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=cG8UfEpttvW4gX8RkcgEbc%2Fjz0MOIm5YWeo68x2UdO4WGG3DSY1lC1dGGocc%2BZj7p%2BqZy2yZNbmtfxjXlFnSxBfQJ0RE1907rivdo8lAIeNjlyk35y6acqUmJCio9gc9xyTMxWZkSA%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=AwBdGlGunrRQ4HgAAKD04iQqlLixnUaZ%2BIiNeadv9QCozM%2FwAoeCZ8YyQrD7x2J1c1JpLNaGsq8EDNxKrFCxQNh9tCgG4rt7GL7skaSruW%2BcEiDbenbXD8UlQDGQFx4yHcZcEW8nDg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
       alt-svc:
       - h3=":443"; ma=86400
     status:
       code: 200
       message: OK
 - request:
-    body: ''
+    body: mfa_token=MFA-1536-goMvl9PeE1QlH6JSJX1f5hqZk4ccycCbkdy6nxF3WTOg5inTfx-cas
     headers:
       Accept:
       - !!binary |
         Ki8q
       Accept-Encoding:
       - !!binary |
         Z3ppcCwgZGVmbGF0ZQ==
       Authorization:
       - Bearer SANITIZED
       Connection:
       - !!binary |
         a2VlcC1hbGl2ZQ==
       Content-Length:
-      - !!binary |
-        MA==
+      - '73'
       Content-Type:
       - !!binary |
         YXBwbGljYXRpb24veC13d3ctZm9ybS11cmxlbmNvZGVk
       User-Agent:
       - !!binary |
         Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ==
     method: POST
@@ -1014,32 +1013,32 @@
   response:
     body:
       string: '{"scope": "COMMUNITY_COURSE_READ GARMINPAY_WRITE GOLF_API_READ ATP_READ
         GHS_SAMD GHS_UPLOAD INSIGHTS_READ COMMUNITY_COURSE_WRITE CONNECT_WRITE GCOFFER_WRITE
         GARMINPAY_READ DT_CLIENT_ANALYTICS_WRITE GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ
         GCOFFER_READ CONNECT_READ ATP_WRITE", "jti": "SANITIZED", "access_token":
         "SANITIZED", "token_type": "Bearer", "refresh_token": "SANITIZED", "expires_in":
-        90758, "refresh_token_expires_in": 2591999}'
+        86606, "refresh_token_expires_in": 2591999}'
     headers:
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 7f19a3c2d926479c-DFW
+      - 7f19f8de88e8b6e2-QRO
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Fri, 04 Aug 2023 20:44:41 GMT
+      - Fri, 04 Aug 2023 21:42:47 GMT
       NEL:
       - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=iIakQJY4Wz4BRd8mQXfQOMjElxMfZq5J4gzbTACzNHp9kt41Bxc9H%2BBRkdEbAGQPKU08O%2Bb0x67cPAQq1%2FhiQVtxLq%2FrWxUY68hK0Jt4npTqoiIUeHLjsYph3hpIQlEbligc2nhR0w%3D%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v3?s=%2Bvsjzm2UP5VPvfHrSEgS%2FMFxJs3GC4%2FoPObBG3tEuBguxri1QtILCfVGEjYpJA09T8cTXeSsVkZcSCc2Kf6PtL4luax0IhsRSKPsBrCR1FYBrMCpKHInwe3m%2FX5mUKL%2FlNn4Q42ilg%3D%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Set-Cookie:
       - _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED
       Transfer-Encoding:
       - chunked
       alt-svc:
```

#### html2text {}

```diff
@@ -249,30 +249,30 @@
 \n
 \n\n\n\t
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f19a351192546a1-
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f19f84d2d2047a4-
 DFW Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 20:44:22 GMT
+Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 21:42:23 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=ytG3iKzcFS5%2B99VJD7%2FtqNm2w0E8GcBl0PO%2FS5qsCmdfQkBSJ6ekYSPKRo4ICSZ7qTGOe0aGYYvlGTJhYzx4Z5A46RMoBaAS2EdJ0JfNbriBi4n6TElpPegnmwjqc7Hj"}],"group":
+v3?s=zvXYngpt%2FM66%2Fz9gI0xFgQkzoTIocpc3OGEfkncJ37tBwN57jD%2B09JoWPKA%2BcR75KbtbFv7%2FwUMueVpsMUkKalOfkWJqWd9CZJvR9dmZYBgUP2HbcZR8pURmJPN48%2F9J"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - __cf_bm=SANITIZED; path=SANITIZED; expires=SANITIZED;
 domain=SANITIZED; HttpOnly; Secure; SameSite=SANITIZED - __cflb=SANITIZED;
 SameSite=SANITIZED; Secure; path=SANITIZED; expires=SANITIZED; HttpOnly -
 _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
 SameSite=SANITIZED Transfer-Encoding: - chunked X-Application-Context: -
-casServer:cloud,prod,prod-US_1102:2 X-B3-Traceid: -
-7de36dd29fa2d733290a6725dc47dfb8 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
-f780910f-ccdf-4771-49c7-aad225e3c68d status: code: 200 message: OK - request:
+casServer:cloud,prod,prod-US_1102:5 X-B3-Traceid: -
+6ca6b8ec7d365a895ef418b6319455ad X-Robots-Tag: - noindex X-Vcap-Request-Id: -
+ce3465b6-c1f7-4274-7cea-5812380e0fc9 status: code: 200 message: OK - request:
 body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
 Connection: - keep-alive Cookie: - __cf_bm=SANITIZED; _cfuvid=SANITIZED;
 __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/embed?id=gauth-
@@ -333,29 +333,29 @@
 \n\t\t\n\n
 \n
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f19a3536a19468a-
-DFW Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 20:44:23 GMT
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f19f84e7fa8b6e8-
+QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
+Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 21:42:23 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=%2FFRtmPmaDfGDypVhatXfunnrGA%2BA8%2FxV6e%2BuekUdoE5fp2JNEw4bdoizvGG90r1BbOkbo3Ux5ybFDdoX4bKGqoKZWemHOBRFCYnaxHW3Ewoy9EHnNXohVMAu47T3dGnV"}],"group":
+v3?s=vC5EgD2UglMkkfFYe73MTEAE%2Ba%2BwXEfO1fjtmIdd0szIyodAnJpcate6PdHLtQdup9QOd%2F3QsAS5I0UwloNcZnT3gCBvs%2BOglqOmgC2YYJhOHmbrNHAlh%2FhQdk0Bc4XV"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - SESSION=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
 __VCAP_ID__=SANITIZED; Path=SANITIZED; HttpOnly; Secure Transfer-Encoding: -
 chunked Vary: - Accept-Encoding X-Application-Context: - casServer:
-cloud,prod,prod-US_1102:7 X-B3-Traceid: - 66c4d064ee4981291e470a27733c75c8 X-
-Robots-Tag: - noindex X-Vcap-Request-Id: - 97a74fb2-172b-46bf-69fb-dc6d6ac7ca6b
+cloud,prod,prod-US_1102:7 X-B3-Traceid: - 23e25790497950af53ad870cb9a288b8 X-
+Robots-Tag: - noindex X-Vcap-Request-Id: - 0790e6ab-9635-4d69-6b8a-244cf044e56c
 status: code: 200 message: OK - request: body:
-username=SANITIZED&password=SANITIZED&embed=true&_csrf=884C8386EF425D4BA55B54C0B893A3B750BFD7FC791A34EC0BA934444EC04CE6B1FA7484E35E2DF94006783318F9980B7A3A
+username=SANITIZED&password=SANITIZED&embed=true&_csrf=8FD1312E0D2A8A6D81CFF06E3ECFC06500351F8735530EBCE4F75FCB1A63EF6E8444F31A1CB9774C56E57C2C363807E8FF33
 headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate Connection: - keep-
 alive Content-Length: - '177' Content-Type: - application/x-www-form-urlencoded
 Cookie: - SESSION=SANITIZED; __cf_bm=SANITIZED; _cfuvid=SANITIZED;
 __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
@@ -364,28 +364,28 @@
 method: POST uri: https://sso.garmin.com/sso/signin?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
 response: body: string: '' headers: Access-Control-Allow-Credentials: - 'true'
 Access-Control-Allow-Headers: - Access-Control-Allow-Headers, Origin,Accept, X-
 Requested-With, Content-Type, Access-Control-Request-Method, Access-Control-
 Request-Headers Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-
 Control-Allow-Origin: - https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-
-Ray: - 7f19a354dcda1547-QRO Connection: - keep-alive Content-Language: - en
-Content-Length: - '0' Date: - Fri, 04 Aug 2023 20:44:24 GMT Location: - https:/
+Ray: - 7f19f84fd8d5154b-QRO Connection: - keep-alive Content-Language: - en
+Content-Length: - '0' Date: - Fri, 04 Aug 2023 21:42:25 GMT Location: - https:/
 /sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=tT3Bm66IlHoACTPEW5aaWCih7nnzM48aWyyucJvJmXCHD6IH9yzYzqrcuZRsM3bzCgO5iQl0GWdKr4pSX%2Bbww%2F1QQ2HgTgnaYSYzYE9M9%2BiXwO8Z9zPyD5ShoR5IaGGZ"}],"group":
+v3?s=tFguDXcU1G6XJJv%2BBcpNv3veY3trRFFdHZIhw4TIp60D4GyisC1Rp3K1v%2Bj%2Fcq4FuGh4LJaZA8UQLxCLAuJfHezU7jFSlTbZvV2qXbNxQ%2F7n0OtnJh2FuSrZzYLtIXUZ"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - __cfruid=SANITIZED; path=SANITIZED; domain=SANITIZED;
 HttpOnly; Secure; SameSite=SANITIZED Vary: - Accept-Encoding X-Application-
 Context: - casServer:cloud,prod,prod-US_1102:7 X-B3-Traceid: -
-55b92cb20bd883142b4f3a21212f1a1c X-Robots-Tag: - noindex X-Vcap-Request-Id: -
-2993f7d4-157a-412b-4177-8315cd0e0f50 status: code: 302 message: Found -
+2306946bb772deae0299aca0881a0afe X-Robots-Tag: - noindex X-Vcap-Request-Id: -
+90ed387d-cabf-4049-4122-09090680db2b status: code: 302 message: Found -
 request: body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
 Connection: - keep-alive Cookie: - SESSION=SANITIZED; __cf_bm=SANITIZED;
 _cfuvid=SANITIZED; __cfruid=SANITIZED; __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/signin?id=gauth-
@@ -459,27 +459,27 @@
 \n
 \n
 \n
 " headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f19a35eadf64797-
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-RAY: - 7f19f85a8a0846d4-
 DFW Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 20:44:24 GMT
+Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 21:42:25 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=Cx2KhXZ92%2Fc38BjEH2TJ8bKkuzKrXn7G4k2KBB4F77VUlfrRtd3Ma36EuNIuEwPKt0MbbTBkiKz6cmCVpLHL78Grb1yaW4qioaOhRpKmselHhTiRADUtZ986y6gwrMzF"}],"group":
+v3?s=vlAIfwLdw1RDwdV2miJoXWzSRPUIP0vka2ZV3M%2BpTKxZz%2F2bv%2FBHlFw0eOQ767Weo7hVAd9dM0d9VkbqussSgEMIYQ268IuyC8EfS2AzRvnQYhcWPAvkZuw%2Fxl6HzYh9"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED Transfer-Encoding: - chunked X-Application-Context: - casServer:
-cloud,prod,prod-US_1102:7 X-B3-Traceid: - 7af5fbfce51e803d25255d01c1881b84 X-
-Robots-Tag: - noindex X-Vcap-Request-Id: - b3ef8bab-184d-4715-4701-3c7749dfb38d
+cloud,prod,prod-US_1102:7 X-B3-Traceid: - 0a3e2d17f07851c273668f7d119fdd2e X-
+Robots-Tag: - noindex X-Vcap-Request-Id: - be07a1e9-4b86-4a15-4a39-c26e2e86dd49
 status: code: 200 message: OK - request: body: mfa-
-code=577212&embed=true&_csrf=89E48A5A52FDC9A4B5C29D2918F619B337621D199A534539AAD83C0AA2AB17DAF3C4CF9F56195AEE3BCE4B6866A34928D8BF&fromPage=setupEnterMfaCode
+code=195893&embed=true&_csrf=F9C17B99B345D1989FF8805BC611547BEC7C8F3C4C3DD4EC32AB8B766A27731265986903FD84CB56F1A1CA270D1D598F1D6F&fromPage=setupEnterMfaCode
 headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate Connection: - keep-
 alive Content-Length: - '160' Content-Type: - application/x-www-form-urlencoded
 Cookie: - SESSION=SANITIZED; __cf_bm=SANITIZED; __cfruid=SANITIZED;
 _cfuvid=SANITIZED; __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
@@ -489,37 +489,37 @@
 loginEnterMfaCode?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
 response: body: string: '' headers: Access-Control-Allow-Credentials: - 'true'
 Access-Control-Allow-Headers: - Access-Control-Allow-Headers, Origin,Accept, X-
 Requested-With, Content-Type, Access-Control-Request-Method, Access-Control-
 Request-Headers Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-
 Control-Allow-Origin: - https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-
-RAY: - 7f19a3b10f7a475e-DFW Connection: - keep-alive Content-Language: - en
-Content-Length: - '0' Date: - Fri, 04 Aug 2023 20:44:38 GMT Location: - https:/
+RAY: - 7f19f8c8aff41557-QRO Connection: - keep-alive Content-Language: - en
+Content-Length: - '0' Date: - Fri, 04 Aug 2023 21:42:44 GMT Location: - https:/
 /sso.garmin.com/sso/
-login?logintoken=VuQcJ7ivPg&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
+login?logintoken=PFID9Y5XoQ&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=NGgvN3mY6mMbca0W6oPgP77yYti09%2FRuMFbc%2B3TANMVXaqj0LqEANMWpu2bhQ3eP7bUp%2FJHcPil5lor7r%2FZj%2FeqlikvJC40NazuUT3fD0gr%2FhpkVtHuFxfupzOnFljZr"}],"group":
+v3?s=cUvppW2Waaho4sVepx4f%2BpBXljwio9Mr5vgx73I%2F2Z0A8qBX1eiBnQz%2Fi24%2BbKl74JW8QBFec2n4hSbX2xJgLE9ud3f1xdREl9jbvaIngvRcXsD4cUuqoLgm%2BP1f4iof"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED X-Application-Context: - casServer:cloud,prod,prod-US_1102:7 X-
-B3-Traceid: - 2da2090d89494ce45f9fac6d04602be8 X-Robots-Tag: - noindex X-Vcap-
-Request-Id: - e7305dea-ccb7-422a-4d05-8e07ecb69277 status: code: 302 message:
+B3-Traceid: - 0339eee8eb299f1c0626712d33b7683c X-Robots-Tag: - noindex X-Vcap-
+Request-Id: - 013c5c74-8192-4e87-7be3-d293d92aa83e status: code: 302 message:
 Found - request: body: null headers: Accept: - '*/*' Accept-Encoding: - gzip,
 deflate Connection: - keep-alive Cookie: - SESSION=SANITIZED;
 __cf_bm=SANITIZED; __cfruid=SANITIZED; _cfuvid=SANITIZED;
 __VCAP_ID__=SANITIZED; __cflb=SANITIZED;
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED
 User-Agent: - Mozilla/5.0 (iPhone; CPU iPhone OS 16_5 like Mac OS X)
 AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15E148 referer: - https://
 sso.garmin.com/sso/verifyMFA/loginEnterMfaCode?id=gauth-
 widget&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountCreationUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&gauthHost=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed
 method: GET uri: https://sso.garmin.com/sso/
-login?logintoken=VuQcJ7ivPg&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
+login?logintoken=PFID9Y5XoQ&service=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&locale=en&embed=true&source=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&redirectAfterAccountLoginUrl=https%3A%2F%2Fsso.garmin.com%2Fsso%2Fembed&embedWidget=true
 response: body: string: "
 \n
 \n\t
 \n\t\t
 \n\t\t
 \n\t\t
 \n\t\t
@@ -538,20 +538,20 @@
 \n\t\t
 \n\t
 \n
 \n" headers: Access-Control-Allow-Credentials: - 'true' Access-Control-Allow-
 Headers: - Access-Control-Allow-Headers, Origin,Accept, X-Requested-With,
 Content-Type, Access-Control-Request-Method, Access-Control-Request-Headers
 Access-Control-Allow-Methods: - GET,POST,OPTIONS Access-Control-Allow-Origin: -
-https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f19a3b83f801549-
-QRO Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
-Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 20:44:39 GMT
+https://www.garmin.com CF-Cache-Status: - DYNAMIC CF-Ray: - 7f19f8d24c9745e8-
+DFW Connection: - keep-alive Content-Encoding: - gzip Content-Language: - en
+Content-Type: - text/html;charset=UTF-8 Date: - Fri, 04 Aug 2023 21:42:45 GMT
 NEL: - '{"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}'
 Report-To: - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=imfmx6AwwEBoeOxkjGZH0%2Fuo7TerKPfAo3lexzqusMZoSuUvTb9NcJ%2ByyJcQ2tpq2ir22LFjOMkQL1I3GIaG3fryTvPe4zy0OUoN6zviNS23J9BNLEXkCIiTx381dS8m"}],"group":
+v3?s=mkKV3UBsbSn3e2rQHCFQRE14OiBbFa6u7cpCIcXy3QvaEvbDu8dCCamDRgjKkU%2FElrNOIvq2IG3JogUVOk2XT6UoxD4O59Nk0XIMOi4wHBKjb1GrAc5I34cz7VNebdaf"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 org.springframework.web.servlet.i18n.CookieLocaleResolver.LOCALE=SANITIZED;
 Path=SANITIZED - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
 CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
 HttpOnly - GARMIN-SSO=SANITIZED; Domain=SANITIZED; Path=SANITIZED - GARMIN-
 SSO=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Domain=SANITIZED;
 Path=SANITIZED - GarminNoCache=SANITIZED; Domain=SANITIZED; Path=SANITIZED -
@@ -564,59 +564,60 @@
 Expires=SANITIZED; Domain=SANITIZED; Path=SANITIZED - GARMIN-SSO-CUST-
 GUID=SANITIZED; Domain=SANITIZED; Path=SANITIZED - GARMIN-SSO-CUST-
 GUID=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Domain=SANITIZED;
 Path=SANITIZED - CASTGC=SANITIZED; Path=SANITIZED; Secure; HttpOnly -
 CASTGC=SANITIZED; Max-Age=SANITIZED; Expires=SANITIZED; Path=SANITIZED; Secure;
 HttpOnly Transfer-Encoding: - chunked Vary: - Accept-Encoding X-Application-
 Context: - casServer:cloud,prod,prod-US_1102:7 X-B3-Traceid: -
-4fcf72f20e7a66dc13e58e89d1664544 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
-6feb25a6-e44a-4549-47fa-75badeb102f8 status: code: 200 message: OK - request:
+782920201f8436216612583f8f870378 X-Robots-Tag: - noindex X-Vcap-Request-Id: -
+c796ecd4-094e-4657-479b-b1ab8bc1b185 status: code: 200 message: OK - request:
 body: null headers: Accept: - '*/*' Accept-Encoding: - gzip, deflate
 Connection: - keep-alive User-Agent: - python-requests/2.31.0 method: GET uri:
 https://thegarth.s3.amazonaws.com/oauth_consumer.json response: body: string: '
 {"consumer_key": "SANITIZED", "consumer_secret": "SANITIZED"}' headers: Accept-
 Ranges: - bytes Content-Length: - '124' Content-Type: - application/json Date:
-- Fri, 04 Aug 2023 20:44:40 GMT ETag: - '"20240b1013cb35419bb5b2cff1407a4e"'
+- Fri, 04 Aug 2023 21:42:47 GMT ETag: - '"20240b1013cb35419bb5b2cff1407a4e"'
 Last-Modified: - Thu, 03 Aug 2023 00:16:11 GMT Server: - AmazonS3 x-amz-id-2: -
-/eMqmlK8obld8yP0MiiccJ5jEcyJNyjP5NUEl5p0NQ6WmCSo+GNI0sthWE+8i64u6u61lY+iJr4= x-
-amz-request-id: - 29FWE9MM7JBZB8MM x-amz-server-side-encryption: - AES256
+cBp5mKgmX+Tjt0vISDuygu6J3/f6qZBCBlJCFl1gmUtHNNKgCK2hu4TiOCmoyIX+Hx16w5mDCeA= x-
+amz-request-id: - WTDF5S9E2EP14K4Z x-amz-server-side-encryption: - AES256
 status: code: 200 message: OK - request: body: null headers: Accept: - !!binary
 | Ki8q Accept-Encoding: - !!binary | Z3ppcCwgZGVmbGF0ZQ== Authorization: -
 Bearer SANITIZED Connection: - !!binary | a2VlcC1hbGl2ZQ== User-Agent: -
 !!binary | Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ== method: GET
 uri: https://connectapi.garmin.com/oauth-service/oauth/preauthorized?ticket=ST-
-2435197-JpeHGkPdeOMWbeob04zU-cas&login-url=https://sso.garmin.com/sso/
+2438674-btozWOKhrVdRH4PKUwah-cas&login-url=https://sso.garmin.com/sso/
 embed&accepts-mfa-tokens=true response: body: string:
 oauth_token=SANITIZED&oauth_token_secret=SANITIZED&mfa_token=SANITIZED&mfa_expiration_timestamp=2024-
-08-03 20:44:39.000 headers: CF-Cache-Status: - DYNAMIC CF-RAY: -
-7f19a3beb9b71557-QRO Connection: - keep-alive Content-Encoding: - gzip Content-
-Type: - text/plain;charset=utf-8 Date: - Fri, 04 Aug 2023 20:44:40 GMT NEL: - '
+08-03 21:42:45.000 headers: CF-Cache-Status: - DYNAMIC CF-RAY: -
+7f19f8daecc2155f-QRO Connection: - keep-alive Content-Encoding: - gzip Content-
+Type: - text/plain;charset=utf-8 Date: - Fri, 04 Aug 2023 21:42:46 GMT NEL: - '
 {"success_fraction":0.01,"report_to":"cf-nel","max_age":604800}' Report-To: - '
 {"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/
-v3?s=cG8UfEpttvW4gX8RkcgEbc%2Fjz0MOIm5YWeo68x2UdO4WGG3DSY1lC1dGGocc%2BZj7p%2BqZy2yZNbmtfxjXlFnSxBfQJ0RE1907rivdo8lAIeNjlyk35y6acqUmJCio9gc9xyTMxWZkSA%3D%3D"}],"group":
+v3?s=AwBdGlGunrRQ4HgAAKD04iQqlLixnUaZ%2BIiNeadv9QCozM%2FwAoeCZ8YyQrD7x2J1c1JpLNaGsq8EDNxKrFCxQNh9tCgG4rt7GL7skaSruW%2BcEiDbenbXD8UlQDGQFx4yHcZcEW8nDg%3D%3D"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
 SameSite=SANITIZED Transfer-Encoding: - chunked alt-svc: - h3=":443"; ma=86400
-status: code: 200 message: OK - request: body: '' headers: Accept: - !!binary |
-Ki8q Accept-Encoding: - !!binary | Z3ppcCwgZGVmbGF0ZQ== Authorization: - Bearer
-SANITIZED Connection: - !!binary | a2VlcC1hbGl2ZQ== Content-Length: - !!binary
-| MA== Content-Type: - !!binary | YXBwbGljYXRpb24veC13d3ctZm9ybS11cmxlbmNvZGVk
-User-Agent: - !!binary | Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ==
-method: POST uri: https://connectapi.garmin.com/oauth-service/oauth/exchange/
-user/2.0 response: body: string: '{"scope": "COMMUNITY_COURSE_READ
-GARMINPAY_WRITE GOLF_API_READ ATP_READ GHS_SAMD GHS_UPLOAD INSIGHTS_READ
-COMMUNITY_COURSE_WRITE CONNECT_WRITE GCOFFER_WRITE GARMINPAY_READ
-DT_CLIENT_ANALYTICS_WRITE GOLF_API_WRITE INSIGHTS_WRITE PRODUCT_SEARCH_READ
-GCOFFER_READ CONNECT_READ ATP_WRITE", "jti": "SANITIZED", "access_token":
-"SANITIZED", "token_type": "Bearer", "refresh_token": "SANITIZED",
-"expires_in": 90758, "refresh_token_expires_in": 2591999}' headers: CF-Cache-
-Status: - DYNAMIC CF-RAY: - 7f19a3c2d926479c-DFW Connection: - keep-alive
-Content-Encoding: - gzip Content-Type: - application/json Date: - Fri, 04 Aug
-2023 20:44:41 GMT NEL: - '{"success_fraction":0.01,"report_to":"cf-
-nel","max_age":604800}' Report-To: - '{"endpoints":[{"url":"https:\/\/
-a.nel.cloudflare.com\/report\/
-v3?s=iIakQJY4Wz4BRd8mQXfQOMjElxMfZq5J4gzbTACzNHp9kt41Bxc9H%2BBRkdEbAGQPKU08O%2Bb0x67cPAQq1%2FhiQVtxLq%2FrWxUY68hK0Jt4npTqoiIUeHLjsYph3hpIQlEbligc2nhR0w%3D%3D"}],"group":
+status: code: 200 message: OK - request: body: mfa_token=MFA-1536-
+goMvl9PeE1QlH6JSJX1f5hqZk4ccycCbkdy6nxF3WTOg5inTfx-cas headers: Accept: -
+!!binary | Ki8q Accept-Encoding: - !!binary | Z3ppcCwgZGVmbGF0ZQ==
+Authorization: - Bearer SANITIZED Connection: - !!binary | a2VlcC1hbGl2ZQ==
+Content-Length: - '73' Content-Type: - !!binary |
+YXBwbGljYXRpb24veC13d3ctZm9ybS11cmxlbmNvZGVk User-Agent: - !!binary |
+Y29tLmdhcm1pbi5hbmRyb2lkLmFwcHMuY29ubmVjdG1vYmlsZQ== method: POST uri: https://
+connectapi.garmin.com/oauth-service/oauth/exchange/user/2.0 response: body:
+string: '{"scope": "COMMUNITY_COURSE_READ GARMINPAY_WRITE GOLF_API_READ
+ATP_READ GHS_SAMD GHS_UPLOAD INSIGHTS_READ COMMUNITY_COURSE_WRITE CONNECT_WRITE
+GCOFFER_WRITE GARMINPAY_READ DT_CLIENT_ANALYTICS_WRITE GOLF_API_WRITE
+INSIGHTS_WRITE PRODUCT_SEARCH_READ GCOFFER_READ CONNECT_READ ATP_WRITE", "jti":
+"SANITIZED", "access_token": "SANITIZED", "token_type": "Bearer",
+"refresh_token": "SANITIZED", "expires_in": 86606, "refresh_token_expires_in":
+2591999}' headers: CF-Cache-Status: - DYNAMIC CF-RAY: - 7f19f8de88e8b6e2-QRO
+Connection: - keep-alive Content-Encoding: - gzip Content-Type: - application/
+json Date: - Fri, 04 Aug 2023 21:42:47 GMT NEL: - '{"success_fraction":
+0.01,"report_to":"cf-nel","max_age":604800}' Report-To: - '{"endpoints":[
+{"url":"https:\/\/a.nel.cloudflare.com\/report\/
+v3?s=%2Bvsjzm2UP5VPvfHrSEgS%2FMFxJs3GC4%2FoPObBG3tEuBguxri1QtILCfVGEjYpJA09T8cTXeSsVkZcSCc2Kf6PtL4luax0IhsRSKPsBrCR1FYBrMCpKHInwe3m%2FX5mUKL%2FlNn4Q42ilg%3D%3D"}],"group":
 "cf-nel","max_age":604800}' Server: - cloudflare Set-Cookie: -
 _cfuvid=SANITIZED; path=SANITIZED; domain=SANITIZED; HttpOnly; Secure;
 SameSite=SANITIZED Transfer-Encoding: - chunked alt-svc: - h3=":443"; ma=86400
 cache-control: - no-cache, no-store, private pragma: - no-cache status: code:
 200 message: OK version: 1
```

### Comparing `garth-0.4.1/tests/cassettes/test_username.yaml` & `garth-0.4.2/tests/cassettes/test_username.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/conftest.py` & `garth-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_daily_hrv.yaml` & `garth-0.4.2/tests/stats/cassettes/test_daily_hrv.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_daily_hrv_no_results.yaml` & `garth-0.4.2/tests/stats/cassettes/test_daily_hrv_no_results.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_daily_hrv_paginate.yaml` & `garth-0.4.2/tests/stats/cassettes/test_daily_hrv_paginate.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml` & `garth-0.4.2/tests/stats/cassettes/test_daily_hrv_paginate_no_results.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_daily_intensity_minutes.yaml` & `garth-0.4.2/tests/stats/cassettes/test_daily_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_daily_sleep.yaml` & `garth-0.4.2/tests/stats/cassettes/test_daily_sleep.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_daily_steps.yaml` & `garth-0.4.2/tests/stats/cassettes/test_daily_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_daily_stress.yaml` & `garth-0.4.2/tests/stats/cassettes/test_daily_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_daily_stress_pagination.yaml` & `garth-0.4.2/tests/stats/cassettes/test_daily_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_sleep_data_get.yaml` & `garth-0.4.2/tests/stats/cassettes/test_sleep_data_get.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_sleep_data_list.yaml` & `garth-0.4.2/tests/stats/cassettes/test_sleep_data_list.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_weekly_intensity_minutes.yaml` & `garth-0.4.2/tests/stats/cassettes/test_weekly_intensity_minutes.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_weekly_steps.yaml` & `garth-0.4.2/tests/stats/cassettes/test_weekly_steps.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_weekly_stress.yaml` & `garth-0.4.2/tests/stats/cassettes/test_weekly_stress.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml` & `garth-0.4.2/tests/stats/cassettes/test_weekly_stress_beyond_data.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/cassettes/test_weekly_stress_pagination.yaml` & `garth-0.4.2/tests/stats/cassettes/test_weekly_stress_pagination.yaml`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/test_hrv.py` & `garth-0.4.2/tests/stats/test_hrv.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/test_intensity_minutes.py` & `garth-0.4.2/tests/stats/test_intensity_minutes.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/test_sleep.py` & `garth-0.4.2/tests/stats/test_sleep.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/test_steps.py` & `garth-0.4.2/tests/stats/test_steps.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/stats/test_stress.py` & `garth-0.4.2/tests/stats/test_stress.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/test_http.py` & `garth-0.4.2/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/test_sso.py` & `garth-0.4.2/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/tests/test_utils.py` & `garth-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `garth-0.4.1/PKG-INFO` & `garth-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garth
-Version: 0.4.1
+Version: 0.4.2
 Summary: Garmin SSO auth + Connect client
 Author-Email: Matin Tamizi <mtamizi@duck.com>
 License: MIT
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

