# Comparing `tmp/pymod112-0.1.1.tar.gz` & `tmp/pymod112-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymod112-0.1.1.tar", last modified: Sun Jul  2 03:29:15 2023, max compression
+gzip compressed data, was "pymod112-0.1.2.tar", last modified: Sat Aug  5 06:05:04 2023, max compression
```

## Comparing `pymod112-0.1.1.tar` & `pymod112-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 03:29:15.284884 pymod112-0.1.1/
--rw-rw-rw-   0        0        0     1535 2023-06-24 01:55:06.000000 pymod112-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1996 2023-07-02 03:29:15.284884 pymod112-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-07-02 03:24:34.000000 pymod112-0.1.1/README.md
--rw-rw-rw-   0        0        0      622 2023-07-02 03:28:24.000000 pymod112-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-02 03:29:15.285884 pymod112-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 03:29:15.267883 pymod112-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-02 03:29:15.275883 pymod112-0.1.1/src/pymod112/
--rw-rw-rw-   0        0        0      214 2023-07-02 03:26:32.000000 pymod112-0.1.1/src/pymod112/__init__.py
--rw-rw-rw-   0        0        0     7198 2023-07-02 03:27:48.000000 pymod112-0.1.1/src/pymod112/mod112.py
-drwxrwxrwx   0        0        0        0 2023-07-02 03:29:15.281883 pymod112-0.1.1/src/pymod112.egg-info/
--rw-rw-rw-   0        0        0     1996 2023-07-02 03:29:15.000000 pymod112-0.1.1/src/pymod112.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-07-02 03:29:15.000000 pymod112-0.1.1/src/pymod112.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 03:29:15.000000 pymod112-0.1.1/src/pymod112.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-02 03:29:15.000000 pymod112-0.1.1/src/pymod112.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 03:29:15.283883 pymod112-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-27 15:26:13.000000 pymod112-0.1.1/tests/test_basic.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:05:04.870772 pymod112-0.1.2/
+-rw-rw-rw-   0        0        0     1084 2023-06-24 11:23:02.000000 pymod112-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2882 2023-08-05 06:05:04.870772 pymod112-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2340 2023-08-05 06:02:30.000000 pymod112-0.1.2/README.md
+-rw-rw-rw-   0        0        0      624 2023-07-22 15:54:26.000000 pymod112-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 06:05:04.870772 pymod112-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 06:05:04.854712 pymod112-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 06:05:04.870772 pymod112-0.1.2/src/pymod112/
+-rw-rw-rw-   0        0        0      225 2023-07-21 09:02:10.000000 pymod112-0.1.2/src/pymod112/__init__.py
+-rw-rw-rw-   0        0        0     9807 2023-07-30 05:30:18.000000 pymod112-0.1.2/src/pymod112/mod112.py
+drwxrwxrwx   0        0        0        0 2023-08-05 06:05:04.870772 pymod112-0.1.2/src/pymod112.egg-info/
+-rw-rw-rw-   0        0        0     2882 2023-08-05 06:05:04.000000 pymod112-0.1.2/src/pymod112.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-08-05 06:05:04.000000 pymod112-0.1.2/src/pymod112.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 06:05:04.000000 pymod112-0.1.2/src/pymod112.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 06:05:04.000000 pymod112-0.1.2/src/pymod112.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 06:05:04.870772 pymod112-0.1.2/tests/
+-rw-rw-rw-   0        0        0     1128 2023-08-05 05:57:11.000000 pymod112-0.1.2/tests/test_Pymod112.py
```

### Comparing `pymod112-0.1.1/PKG-INFO` & `pymod112-0.1.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,113 @@
 Metadata-Version: 2.1
 Name: pymod112
-Version: 0.1.1
+Version: 0.1.2
 Summary: 一个可以离线检验公民身份号码是否合法的程序
 Author-email: HoshsL <HoshsL@outlook.com>
-Project-URL: Homepage, https://gitee.com/HoshsL/PyMOD11-2
-Project-URL: Bug Tracker, https://gitee.com/HoshsL/PyMOD11-2/issues
+Project-URL: Homepage, https://github.com/HoshsL/PyMOD11-2
+Project-URL: Bug Tracker, https://github.com/HoshsL/PyMOD11-2/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pymod112
 
 一个基于Python开发的公民身份号码检验与地区代码查找程序
 
-## 安装 Installation
+by HoshsL
 
-[PyPi](https://pypi.org/project/pymod112/) 使用pip安装
+## 安装
+
+[PyPI](https://pypi.org/project/pymod112/) 
+
+使用pip安装，仅支持Python 3.10及以上版本
 
 ```sh
 pip install pymod112
 ```
 
-## 使用 Usage
+## 使用
 
-身份证号码校验
+校验身份证号码(隐藏详情)
 
 ```python
-import pymod112
+>>> import pymod112
+>>> pymod112.mod112('11010519491231002X')
+True
+```
 
-pymod112.mod112('11010519491231002X', details=True)
-'''返回值为(dict)
-{'id': '11010519491231002X', 
- 'province': ['11', '北京市'], 
- 'city': ['01', ''], 
- 'county': ['05', '朝阳区'], 
- 'birth_date': ['1949', '12', '31'], 
- 'gender': 0, 
- 'result': True, 
- 'problem': '000'}
-'''
+校验身份证号码(显示详情)
 
+```python
+>>> import pymod112
+>>> pymod112.mod112('11010519491231002X', details=True)
+{'id': '11010519491231002X',
+ 'province': ['11', '北京市'],
+ 'city': ['01', ''],
+ 'county': ['05', '朝阳区'],
+ 'birth_date': ['1949', '12', '31'],
+ 'gender': '女',
+ 'result': True,
+ 'problem': '000'}
 ```
 
 查询地区代码对应的地区名
 
 ```python
-import pymod112
+>>> import pymod112
+>>> pymod112.code2location('110105')
+['北京市', '', '朝阳区']
+```
+
+查询地区名对应的地区代码
 
-pymod112.code_to_location(['51', '01', '06'])
-'''返回值为(list)
-['四川省', '成都市', '金牛区']
-'''
+```python
+>>> import pymod112
+>>> pymod112.location2code(['北京市', '朝阳区'])
+'110105'
 ```
 
 返回全部错误代码及其对应内容
 
 ```python
-import pymod112
-
-pymod112.code_to_error
-'''dict
+>>> import pymod112
+>>> pymod112.CODE2ERROR
 {'000':'不存在问题',
-'001':'<未定义>',
-'002':'<未定义>',
-'003':'<未定义>',
-'004':'参数id长度错误',
-'005':'参数id内容包含非法字符',
-'006':'参数id不合法',
-'007':'参数id中包含不存在的地区',
-'008':'参数id中包含不存在的时间'
-}
-'''
+ '002':'参数location长度错误',
+ '003':'参数code长度错误',
+ '004':'参数id长度错误',
+ '005':'参数id内容包含非法字符',
+ '006':'参数id不合法',
+ '007':'参数id中包含不存在的地区',
+ '008':'参数id中包含不存在的时间'}
 ```
 
-## 许可证 License
-BSD 3-Clause License
+## 许可证
+MIT License
+
+## 更新日志
+
+### **0.1.2(2023-8-5)**
+ - 错误修复
+     - 修复了参数id来自同年的未来时间也可能通过时间校验的问题
+     - 修复了参数id最后一位不合法但不会返回错误代码005的问题
+ - 新增
+     - 新增函数location2code以方便查询行政区划代码
+ - 改进
+     - 修改了一个函数名(code_to_location -> code2location)
+     - 修改了一个常量名(code_to_error -> CODE2ERROR)
+     - 函数code2location参数code要求类型由list变为code
+     - 更新了CODE2ERROR
+     - 函数mod112返回中'gender'的值变为'男'或'女'
+ - 其它
+    - 开源许可证更改为MIT License
 
-## 更新日志 Changelog
-### **0.1.1**
+### **0.1.1(2023-7-2)**
  - 加入参数类型检查
  - 优化错误代码（停用001 002 003）
  - 删除函数problem()
 
 ### **0.1.0(2023-6-24)**
 - 这是第一个正式发行版
```

### Comparing `pymod112-0.1.1/README.md` & `pymod112-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,99 @@
 # pymod112
 
 一个基于Python开发的公民身份号码检验与地区代码查找程序
 
-## 安装 Installation
+by HoshsL
 
-[PyPi](https://pypi.org/project/pymod112/) 使用pip安装
+## 安装
+
+[PyPI](https://pypi.org/project/pymod112/) 
+
+使用pip安装，仅支持Python 3.10及以上版本
 
 ```sh
 pip install pymod112
 ```
 
-## 使用 Usage
+## 使用
 
-身份证号码校验
+校验身份证号码(隐藏详情)
 
 ```python
-import pymod112
+>>> import pymod112
+>>> pymod112.mod112('11010519491231002X')
+True
+```
 
-pymod112.mod112('11010519491231002X', details=True)
-'''返回值为(dict)
-{'id': '11010519491231002X', 
- 'province': ['11', '北京市'], 
- 'city': ['01', ''], 
- 'county': ['05', '朝阳区'], 
- 'birth_date': ['1949', '12', '31'], 
- 'gender': 0, 
- 'result': True, 
- 'problem': '000'}
-'''
+校验身份证号码(显示详情)
 
+```python
+>>> import pymod112
+>>> pymod112.mod112('11010519491231002X', details=True)
+{'id': '11010519491231002X',
+ 'province': ['11', '北京市'],
+ 'city': ['01', ''],
+ 'county': ['05', '朝阳区'],
+ 'birth_date': ['1949', '12', '31'],
+ 'gender': '女',
+ 'result': True,
+ 'problem': '000'}
 ```
 
 查询地区代码对应的地区名
 
 ```python
-import pymod112
+>>> import pymod112
+>>> pymod112.code2location('110105')
+['北京市', '', '朝阳区']
+```
+
+查询地区名对应的地区代码
 
-pymod112.code_to_location(['51', '01', '06'])
-'''返回值为(list)
-['四川省', '成都市', '金牛区']
-'''
+```python
+>>> import pymod112
+>>> pymod112.location2code(['北京市', '朝阳区'])
+'110105'
 ```
 
 返回全部错误代码及其对应内容
 
 ```python
-import pymod112
-
-pymod112.code_to_error
-'''dict
+>>> import pymod112
+>>> pymod112.CODE2ERROR
 {'000':'不存在问题',
-'001':'<未定义>',
-'002':'<未定义>',
-'003':'<未定义>',
-'004':'参数id长度错误',
-'005':'参数id内容包含非法字符',
-'006':'参数id不合法',
-'007':'参数id中包含不存在的地区',
-'008':'参数id中包含不存在的时间'
-}
-'''
+ '002':'参数location长度错误',
+ '003':'参数code长度错误',
+ '004':'参数id长度错误',
+ '005':'参数id内容包含非法字符',
+ '006':'参数id不合法',
+ '007':'参数id中包含不存在的地区',
+ '008':'参数id中包含不存在的时间'}
 ```
 
-## 许可证 License
-BSD 3-Clause License
+## 许可证
+MIT License
+
+## 更新日志
+
+### **0.1.2(2023-8-5)**
+ - 错误修复
+     - 修复了参数id来自同年的未来时间也可能通过时间校验的问题
+     - 修复了参数id最后一位不合法但不会返回错误代码005的问题
+ - 新增
+     - 新增函数location2code以方便查询行政区划代码
+ - 改进
+     - 修改了一个函数名(code_to_location -> code2location)
+     - 修改了一个常量名(code_to_error -> CODE2ERROR)
+     - 函数code2location参数code要求类型由list变为code
+     - 更新了CODE2ERROR
+     - 函数mod112返回中'gender'的值变为'男'或'女'
+ - 其它
+    - 开源许可证更改为MIT License
 
-## 更新日志 Changelog
-### **0.1.1**
+### **0.1.1(2023-7-2)**
  - 加入参数类型检查
  - 优化错误代码（停用001 002 003）
  - 删除函数problem()
 
 ### **0.1.0(2023-6-24)**
 - 这是第一个正式发行版
```

### Comparing `pymod112-0.1.1/src/pymod112.egg-info/PKG-INFO` & `pymod112-0.1.2/src/pymod112.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,113 @@
 Metadata-Version: 2.1
 Name: pymod112
-Version: 0.1.1
+Version: 0.1.2
 Summary: 一个可以离线检验公民身份号码是否合法的程序
 Author-email: HoshsL <HoshsL@outlook.com>
-Project-URL: Homepage, https://gitee.com/HoshsL/PyMOD11-2
-Project-URL: Bug Tracker, https://gitee.com/HoshsL/PyMOD11-2/issues
+Project-URL: Homepage, https://github.com/HoshsL/PyMOD11-2
+Project-URL: Bug Tracker, https://github.com/HoshsL/PyMOD11-2/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pymod112
 
 一个基于Python开发的公民身份号码检验与地区代码查找程序
 
-## 安装 Installation
+by HoshsL
 
-[PyPi](https://pypi.org/project/pymod112/) 使用pip安装
+## 安装
+
+[PyPI](https://pypi.org/project/pymod112/) 
+
+使用pip安装，仅支持Python 3.10及以上版本
 
 ```sh
 pip install pymod112
 ```
 
-## 使用 Usage
+## 使用
 
-身份证号码校验
+校验身份证号码(隐藏详情)
 
 ```python
-import pymod112
+>>> import pymod112
+>>> pymod112.mod112('11010519491231002X')
+True
+```
 
-pymod112.mod112('11010519491231002X', details=True)
-'''返回值为(dict)
-{'id': '11010519491231002X', 
- 'province': ['11', '北京市'], 
- 'city': ['01', ''], 
- 'county': ['05', '朝阳区'], 
- 'birth_date': ['1949', '12', '31'], 
- 'gender': 0, 
- 'result': True, 
- 'problem': '000'}
-'''
+校验身份证号码(显示详情)
 
+```python
+>>> import pymod112
+>>> pymod112.mod112('11010519491231002X', details=True)
+{'id': '11010519491231002X',
+ 'province': ['11', '北京市'],
+ 'city': ['01', ''],
+ 'county': ['05', '朝阳区'],
+ 'birth_date': ['1949', '12', '31'],
+ 'gender': '女',
+ 'result': True,
+ 'problem': '000'}
 ```
 
 查询地区代码对应的地区名
 
 ```python
-import pymod112
+>>> import pymod112
+>>> pymod112.code2location('110105')
+['北京市', '', '朝阳区']
+```
+
+查询地区名对应的地区代码
 
-pymod112.code_to_location(['51', '01', '06'])
-'''返回值为(list)
-['四川省', '成都市', '金牛区']
-'''
+```python
+>>> import pymod112
+>>> pymod112.location2code(['北京市', '朝阳区'])
+'110105'
 ```
 
 返回全部错误代码及其对应内容
 
 ```python
-import pymod112
-
-pymod112.code_to_error
-'''dict
+>>> import pymod112
+>>> pymod112.CODE2ERROR
 {'000':'不存在问题',
-'001':'<未定义>',
-'002':'<未定义>',
-'003':'<未定义>',
-'004':'参数id长度错误',
-'005':'参数id内容包含非法字符',
-'006':'参数id不合法',
-'007':'参数id中包含不存在的地区',
-'008':'参数id中包含不存在的时间'
-}
-'''
+ '002':'参数location长度错误',
+ '003':'参数code长度错误',
+ '004':'参数id长度错误',
+ '005':'参数id内容包含非法字符',
+ '006':'参数id不合法',
+ '007':'参数id中包含不存在的地区',
+ '008':'参数id中包含不存在的时间'}
 ```
 
-## 许可证 License
-BSD 3-Clause License
+## 许可证
+MIT License
+
+## 更新日志
+
+### **0.1.2(2023-8-5)**
+ - 错误修复
+     - 修复了参数id来自同年的未来时间也可能通过时间校验的问题
+     - 修复了参数id最后一位不合法但不会返回错误代码005的问题
+ - 新增
+     - 新增函数location2code以方便查询行政区划代码
+ - 改进
+     - 修改了一个函数名(code_to_location -> code2location)
+     - 修改了一个常量名(code_to_error -> CODE2ERROR)
+     - 函数code2location参数code要求类型由list变为code
+     - 更新了CODE2ERROR
+     - 函数mod112返回中'gender'的值变为'男'或'女'
+ - 其它
+    - 开源许可证更改为MIT License
 
-## 更新日志 Changelog
-### **0.1.1**
+### **0.1.1(2023-7-2)**
  - 加入参数类型检查
  - 优化错误代码（停用001 002 003）
  - 删除函数problem()
 
 ### **0.1.0(2023-6-24)**
 - 这是第一个正式发行版
```

