# Comparing `tmp/xj_behavior-1.0.6.tar.gz` & `tmp/xj_behavior-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_behavior-1.0.6.tar", last modified: Mon Jul 31 08:48:23 2023, max compression
+gzip compressed data, was "dist\xj_behavior-1.0.7.tar", last modified: Sat Aug  5 07:13:48 2023, max compression
```

## Comparing `xj_behavior-1.0.6.tar` & `xj_behavior-1.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/
--rw-rw-rw-   0        0        0     1092 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-03-24 00:39:21.000000 xj_behavior-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      529 2023-07-31 08:48:14.000000 xj_behavior-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/xj_behavior/
--rw-rw-rw-   0        0        0        0 2023-01-12 05:45:43.000000 xj_behavior-1.0.6/xj_behavior/__init__.py
--rw-rw-rw-   0        0        0       22 2023-03-24 00:43:30.000000 xj_behavior-1.0.6/xj_behavior/admin.py
-drwxrwxrwx   0        0        0        0 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/xj_behavior/apis/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.6/xj_behavior/apis/__init__.py
--rw-rw-rw-   0        0        0      982 2023-07-28 02:53:16.000000 xj_behavior-1.0.6/xj_behavior/apis/standing_book_apis.py
--rw-rw-rw-   0        0        0      207 2023-03-24 00:43:09.000000 xj_behavior-1.0.6/xj_behavior/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/xj_behavior/services/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.6/xj_behavior/services/__init__.py
--rw-rw-rw-   0        0        0    13693 2023-07-31 08:47:53.000000 xj_behavior-1.0.6/xj_behavior/services/standing_book_services.py
--rw-rw-rw-   0        0        0      307 2023-07-28 02:26:27.000000 xj_behavior-1.0.6/xj_behavior/urls.py
-drwxrwxrwx   0        0        0        0 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/xj_behavior/utils/
--rw-rw-rw-   0        0        0        0 2023-07-28 01:18:09.000000 xj_behavior-1.0.6/xj_behavior/utils/__init__.py
--rw-rw-rw-   0        0        0     1076 2023-07-28 01:18:09.000000 xj_behavior-1.0.6/xj_behavior/utils/custom_authorization.py
--rw-rw-rw-   0        0        0     4628 2023-07-11 05:41:09.000000 xj_behavior-1.0.6/xj_behavior/utils/custom_response.py
--rw-rw-rw-   0        0        0    39226 2023-07-17 06:47:39.000000 xj_behavior-1.0.6/xj_behavior/utils/custom_tool.py
--rw-rw-rw-   0        0        0      429 2022-11-29 06:32:59.000000 xj_behavior-1.0.6/xj_behavior/utils/j_dict.py
--rw-rw-rw-   0        0        0     8365 2023-07-28 01:18:09.000000 xj_behavior-1.0.6/xj_behavior/utils/j_recur.py
--rw-rw-rw-   0        0        0      464 2023-07-28 01:18:09.000000 xj_behavior-1.0.6/xj_behavior/utils/join_list.py
--rw-rw-rw-   0        0        0     7050 2022-10-27 09:44:29.000000 xj_behavior-1.0.6/xj_behavior/utils/model_handle.py
--rw-rw-rw-   0        0        0     6182 2023-06-05 06:33:17.000000 xj_behavior-1.0.6/xj_behavior/utils/service_manager.py
--rw-rw-rw-   0        0        0     2682 2023-07-28 01:18:09.000000 xj_behavior-1.0.6/xj_behavior/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/xj_behavior.egg-info/
--rw-rw-rw-   0        0        0     1092 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/xj_behavior.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      723 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/xj_behavior.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/xj_behavior.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-31 08:48:23.000000 xj_behavior-1.0.6/xj_behavior.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:48.000000 xj_behavior-1.0.7/
+-rw-rw-rw-   0        0        0     1092 2023-08-05 07:13:48.000000 xj_behavior-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-03-24 00:39:21.000000 xj_behavior-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 07:13:48.000000 xj_behavior-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      529 2023-08-05 07:12:35.000000 xj_behavior-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:48.000000 xj_behavior-1.0.7/xj_behavior/
+-rw-rw-rw-   0        0        0        0 2023-01-12 05:45:43.000000 xj_behavior-1.0.7/xj_behavior/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-03-24 00:43:30.000000 xj_behavior-1.0.7/xj_behavior/admin.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:48.000000 xj_behavior-1.0.7/xj_behavior/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.7/xj_behavior/apis/__init__.py
+-rw-rw-rw-   0        0        0      982 2023-07-28 02:53:16.000000 xj_behavior-1.0.7/xj_behavior/apis/standing_book_apis.py
+-rw-rw-rw-   0        0        0      207 2023-03-24 00:43:09.000000 xj_behavior-1.0.7/xj_behavior/apps.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:48.000000 xj_behavior-1.0.7/xj_behavior/services/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.7/xj_behavior/services/__init__.py
+-rw-rw-rw-   0        0        0    14590 2023-08-05 07:13:11.000000 xj_behavior-1.0.7/xj_behavior/services/standing_book_services.py
+-rw-rw-rw-   0        0        0      307 2023-07-28 02:26:27.000000 xj_behavior-1.0.7/xj_behavior/urls.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:48.000000 xj_behavior-1.0.7/xj_behavior/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-28 01:18:09.000000 xj_behavior-1.0.7/xj_behavior/utils/__init__.py
+-rw-rw-rw-   0        0        0     1076 2023-07-28 01:18:09.000000 xj_behavior-1.0.7/xj_behavior/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     4628 2023-07-11 05:41:09.000000 xj_behavior-1.0.7/xj_behavior/utils/custom_response.py
+-rw-rw-rw-   0        0        0    39226 2023-07-17 06:47:39.000000 xj_behavior-1.0.7/xj_behavior/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      429 2022-11-29 06:32:59.000000 xj_behavior-1.0.7/xj_behavior/utils/j_dict.py
+-rw-rw-rw-   0        0        0     8365 2023-07-28 01:18:09.000000 xj_behavior-1.0.7/xj_behavior/utils/j_recur.py
+-rw-rw-rw-   0        0        0      464 2023-07-28 01:18:09.000000 xj_behavior-1.0.7/xj_behavior/utils/join_list.py
+-rw-rw-rw-   0        0        0     7050 2022-10-27 09:44:29.000000 xj_behavior-1.0.7/xj_behavior/utils/model_handle.py
+-rw-rw-rw-   0        0        0     6182 2023-06-05 06:33:17.000000 xj_behavior-1.0.7/xj_behavior/utils/service_manager.py
+-rw-rw-rw-   0        0        0     2682 2023-07-28 01:18:09.000000 xj_behavior-1.0.7/xj_behavior/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:48.000000 xj_behavior-1.0.7/xj_behavior.egg-info/
+-rw-rw-rw-   0        0        0     1092 2023-08-05 07:13:47.000000 xj_behavior-1.0.7/xj_behavior.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-08-05 07:13:47.000000 xj_behavior-1.0.7/xj_behavior.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 07:13:47.000000 xj_behavior-1.0.7/xj_behavior.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-05 07:13:47.000000 xj_behavior-1.0.7/xj_behavior.egg-info/top_level.txt
```

### Comparing `xj_behavior-1.0.6/PKG-INFO` & `xj_behavior-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_behavior
-Version: 1.0.6
+Version: 1.0.7
 Summary: 行为模块
 License: apache 3.0
 Description-Content-Type: text/markdown
 
 # xj-behavior
 
 #### 介绍
```

### Comparing `xj_behavior-1.0.6/README.md` & `xj_behavior-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.6/setup.py` & `xj_behavior-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_behavior',  # 模块名称
-    version='1.0.6',  # 模块版本
+    version='1.0.7',  # 模块版本
     description='行为模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     packages=find_packages(),  # 系统自动从当前目录开始找包
     license="apache 3.0",
     install_requires=[]
 )
```

### Comparing `xj_behavior-1.0.6/xj_behavior/apis/standing_book_apis.py` & `xj_behavior-1.0.7/xj_behavior/apis/standing_book_apis.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.6/xj_behavior/services/standing_book_services.py` & `xj_behavior-1.0.7/xj_behavior/services/standing_book_services.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,20 +90,48 @@
         # 资金相关的数据
         finance_list, err = FinanceTransactsService.finance_standing_book(params={"enroll_id_list": enroll_id_list})
         JoinList.left_join(l_list=enroll_result['list'], r_list=finance_list, l_key="id", r_key="enroll_id")
 
         return enroll_result, None
 
     @staticmethod
+    def __get_beneficiary_level(user_id, invite_relate_type_id):
+        invite_user_map = {}
+        first_invite_user = db.table("user_relate_to_user"). \
+            where("user_relate_to_user.user_id", '=', user_id). \
+            where("user_relate_type_id", invite_relate_type_id). \
+            pluck('with_user_id')
+        if first_invite_user:
+            invite_user_map[first_invite_user] = 1
+
+        second_invite_user = None
+        if first_invite_user:
+            second_invite_user = db.table("user_relate_to_user"). \
+                where("user_relate_to_user.user_id", first_invite_user). \
+                where("user_relate_type_id", invite_relate_type_id). \
+                pluck('with_user_id')
+            if second_invite_user:
+                invite_user_map[second_invite_user] = 2
+
+        if second_invite_user:
+            third_invite_user = db.table("user_relate_to_user"). \
+                where("user_relate_to_user.user_id", second_invite_user). \
+                where("user_relate_type_id", invite_relate_type_id). \
+                pluck('with_user_id')
+            if third_invite_user:
+                invite_user_map[third_invite_user] = 3
+
+        return invite_user_map
+
+    @staticmethod
     def standing_book_v2(params: dict):
         params, err = force_transform_type(variable=params, var_type="dict", default={})
         # 获取项目信息
         enroll_result, err = EnrollAPI.list_handle(request_params=params)
         enroll_list = enroll_result['list']
-        enroll_list[0]["user_id"] = 680
 
         # 获取业务员相关信息
         enroll_to_user_map = {i["id"]: i["user_id"] for i in enroll_list}
         invite_relate_type_id = db.table("user_relate_type").where("relate_key", "invite").pluck('id')
         beneficiary_relate_type_id = db.table("user_relate_type").where("relate_key", "beneficiary").pluck('id')
         # ------------------------------- section 找到这一批人的业务人员的相关信息 start -------------------------------------------
         # 第一步、获取客户绑定的业务人员列表，找到了业务人员
@@ -135,47 +163,37 @@
         group_user_map = {}
         for i in group_user_set:
             if group_user_map.get(i["user_id"]):
                 group_user_map[i["user_id"]].append(i)
             else:
                 group_user_map[i["user_id"]] = [i]
 
-        # 第三步、找到这批客户的一、二、三级邀请人。来判断业务的分成比例
-        first_invite_users = db.table("user_relate_to_user"). \
-            where_in("user_relate_to_user.user_id", list(set(enroll_to_user_map.values()))). \
-            where("user_relate_type_id", invite_relate_type_id). \
-            lists('with_user_id')
-
-        second_invite_users = db.table("user_relate_to_user"). \
-            where_in("user_relate_to_user.user_id", first_invite_users). \
-            where("user_relate_type_id", invite_relate_type_id). \
-            lists('with_user_id')
-
-        third_invite_users = db.table("user_relate_to_user"). \
-            where_in("user_relate_to_user.user_id", second_invite_users). \
-            where("user_relate_type_id", invite_relate_type_id). \
-            lists('with_user_id')
-
         # 第四步、获取资金相关的信息
         bid_user_pay_map = db.table("finance_transact"). \
             where("income", '>', 0). \
             where_in("enroll_id", list(enroll_to_user_map.keys())).lists('bookkeeping_type', 'enroll_id')
 
         # 第五步、拼接业务信息
         for i in enroll_result['list']:
-            i["beneficiary"] = beneficiary_real_name_map.get(i['user_id'], "--")
-            beneficiary_id = beneficiary_id_map.get(i['user_id'], 0)
-            i["beneficiary_group_name"] = group_user_map.get(beneficiary_id, [])
-            i["beneficiary_percentage"] = 0
-            if beneficiary_id in first_invite_users:
+            i["beneficiary"] = beneficiary_real_name_map.get(i['user_id'], "--")  # 业务员
+            beneficiary_id = beneficiary_id_map.get(i['user_id'], 0)  # 业务员的用户ID
+            i["beneficiary_group_name"] = group_user_map.get(beneficiary_id, [])  # 业务人员所属部门
+            i["beneficiary_percentage"] = 0  # 业务员提成默认值
+            # 获取该用户前三及的邀请人，判断他的业务员是第几级
+            invite_relate_level_map = StandingBookServices.__get_beneficiary_level(
+                user_id=i["user_id"],
+                invite_relate_type_id=invite_relate_type_id
+            )
+            if beneficiary_id and invite_relate_level_map.get(beneficiary_id) == 1:
                 i["beneficiary_percentage"] = float(i["amount"] or 0) * 0.06
-            elif beneficiary_id in second_invite_users:
+            elif beneficiary_id and invite_relate_level_map.get(beneficiary_id) == 2:
                 i["beneficiary_percentage"] = float(i["amount"] or 0) * 0.04
-            elif beneficiary_id in third_invite_users:
+            elif beneficiary_id and invite_relate_level_map.get(beneficiary_id) == 3:
                 i["beneficiary_percentage"] = float(i["amount"] or 0) * 0.02
+
             i["bookkeeping_type"] = bid_user_pay_map.get(i['id'], "-")
         # ------------------------------- section 找到这一批人的业务人员的相关信息 end   -------------------------------------------
 
         # ------------------------------- section 获取开票信息 start -------------------------------------------
         # 第一步、查询
         invoice_set_list = db.table("invoice_to_enroll"). \
             left_join('invoice_invoice', 'invoice_invoice.id', '=', 'invoice_to_enroll.invoice_id'). \
@@ -222,15 +240,16 @@
                 user_base_info.full_name as record_full_name,
                 user_detail_info.real_name as record_real_name
             """). \
             where_in("enroll_record.enroll_id", list(enroll_to_user_map.keys())). \
             where_not_in("enroll_record.enroll_status_code", [124, 234]). \
             get()
         enroll_record_user_map = {i["enroll_id"]: i for i in enroll_record_user}
-        # 获取资金相关的信息
+
+        # 获取资金相关的信息,286 为平台用户
         bid_worker_pay_record = db.table("finance_transact"). \
             select('transact_time', 'enroll_id', 'account_id', 'income', 'outgo', 'pay_mode_id', 'bookkeeping_type'). \
             where("account_id", '=', 286). \
             where("income", '=', 0). \
             where_in("enroll_id", list(enroll_record_user_map.keys())).get()
         bid_worker_pay_record_map = {i["enroll_id"]: i for i in bid_worker_pay_record}
         # 拼接数据
@@ -239,11 +258,11 @@
             i["record_nickname"] = enroll_record_user_map.get(i["id"], {}).get("record_nickname")
             i["record_full_name"] = enroll_record_user_map.get(i["id"], {}).get("record_full_name")
             i["record_real_name"] = enroll_record_user_map.get(i["id"], {}).get("record_real_name")
             # 资金余额相关的逻辑
             i["pay_mode_id"] = bid_worker_pay_record_map.get(i["id"], {}).get("pay_mode_id")
             i["record_transact_time"] = bid_worker_pay_record_map.get(i["id"], {}).get("transact_time")
             i["record_outgo"] = bid_worker_pay_record_map.get(i["id"], {}).get("outgo")
-            i["record_bookkeeping_type"] = bid_worker_pay_record_map.get(i["id"], {}).get("bookkeeping_type", '-')
+            i["record_bookkeeping_type"] = bid_worker_pay_record_map.get(i["id"], {}).get("bookkeeping_type", '-')  # 镖师佣金的线上和线下支付
         # ------------------------------- section 获取镖师信息 end   -------------------------------------------
 
         return enroll_result, None
```

### Comparing `xj_behavior-1.0.6/xj_behavior/utils/custom_authorization.py` & `xj_behavior-1.0.7/xj_behavior/utils/custom_authorization.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.6/xj_behavior/utils/custom_response.py` & `xj_behavior-1.0.7/xj_behavior/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.6/xj_behavior/utils/custom_tool.py` & `xj_behavior-1.0.7/xj_behavior/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.6/xj_behavior/utils/j_recur.py` & `xj_behavior-1.0.7/xj_behavior/utils/j_recur.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.6/xj_behavior/utils/model_handle.py` & `xj_behavior-1.0.7/xj_behavior/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.6/xj_behavior/utils/service_manager.py` & `xj_behavior-1.0.7/xj_behavior/utils/service_manager.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.6/xj_behavior/utils/validator.py` & `xj_behavior-1.0.7/xj_behavior/utils/validator.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.6/xj_behavior.egg-info/PKG-INFO` & `xj_behavior-1.0.7/xj_behavior.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-behavior
-Version: 1.0.6
+Version: 1.0.7
 Summary: 行为模块
 License: apache 3.0
 Description-Content-Type: text/markdown
 
 # xj-behavior
 
 #### 介绍
```

### Comparing `xj_behavior-1.0.6/xj_behavior.egg-info/SOURCES.txt` & `xj_behavior-1.0.7/xj_behavior.egg-info/SOURCES.txt`

 * *Files identical despite different names*

