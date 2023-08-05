# Comparing `tmp/statprocon-0.1.1.tar.gz` & `tmp/statprocon-0.2.0.tar.gz`

## Comparing `statprocon-0.1.1.tar` & `statprocon-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 statprocon-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 statprocon-0.1.1/CODEOWNERS
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 statprocon-0.1.1/requirements-dev.txt
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 statprocon-0.1.1/tox.ini
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/dataSources.local.xml
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/vcs.xml
--rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/workspace.xml
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/xmr.iml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/charts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/charts/xmr/__init__.py
--rw-r--r--   0        0        0    12222 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/charts/xmr/base.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/charts/xmr/constants.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 statprocon-0.1.1/statprocon/charts/xmr/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 statprocon-0.1.1/tests/test_xmr.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 statprocon-0.1.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.1.1/LICENSE
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 statprocon-0.1.1/README.md
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 statprocon-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5906 2020-02-02 00:00:00.000000 statprocon-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 statprocon-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 statprocon-0.2.0/CODEOWNERS
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 statprocon-0.2.0/requirements-dev.txt
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 statprocon-0.2.0/tox.ini
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 statprocon-0.2.0/.idea/.gitignore
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 statprocon-0.2.0/.idea/dataSources.local.xml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 statprocon-0.2.0/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 statprocon-0.2.0/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 statprocon-0.2.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     9568 2020-02-02 00:00:00.000000 statprocon-0.2.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 statprocon-0.2.0/.idea/xmr.iml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 statprocon-0.2.0/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 statprocon-0.2.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 statprocon-0.2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 statprocon-0.2.0/statprocon/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.2.0/statprocon/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.2.0/statprocon/charts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.2.0/statprocon/charts/xmr/__init__.py
+-rw-r--r--   0        0        0    12165 2020-02-02 00:00:00.000000 statprocon-0.2.0/statprocon/charts/xmr/base.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 statprocon-0.2.0/statprocon/charts/xmr/constants.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 statprocon-0.2.0/statprocon/charts/xmr/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.2.0/statprocon/charts/xmr/limits/__init__.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 statprocon-0.2.0/statprocon/charts/xmr/limits/trending.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 statprocon-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     3387 2020-02-02 00:00:00.000000 statprocon-0.2.0/tests/test_trending.py
+-rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 statprocon-0.2.0/tests/test_xmr.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 statprocon-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 statprocon-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 statprocon-0.2.0/README.md
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 statprocon-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 statprocon-0.2.0/PKG-INFO
```

### Comparing `statprocon-0.1.1/CHANGELOG.md` & `statprocon-0.2.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Release History
 
 ---
 
+## 0.2.0
+
+- Add `XmRTrending()` class to compute trending X central line and natural process limits
+
 ## 0.1.1
 
 - Add parameter `x_central_line_uses` to accept `median` and return the median for the X central line
 
 ## 0.1.0
 
 - Add parameter `moving_range_uses` to accept `median` and compute the limits using the median moving range
```

### Comparing `statprocon-0.1.1/requirements-dev.txt` & `statprocon-0.2.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `statprocon-0.1.1/.idea/workspace.xml` & `statprocon-0.2.0/.idea/workspace.xml`

 * *Files 16% similar despite different names*

#### Comparing `statprocon-0.1.1/.idea/workspace.xml` & `statprocon-0.2.0/.idea/workspace.xml`

```diff
@@ -1,19 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="6b007249-c07a-402d-ab76-cd0adebb4623" name="Default Changelist" comment="">
-      <change beforePath="$PROJECT_DIR$/CHANGELOG.md" beforeDir="false" afterPath="$PROJECT_DIR$/CHANGELOG.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/README.md" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/statprocon/charts/xmr/base.py" beforeDir="false" afterPath="$PROJECT_DIR$/statprocon/charts/xmr/base.py" afterDir="false"/>
-      <change beforePath="$PROJECT_DIR$/tests/test_xmr.py" beforeDir="false" afterPath="$PROJECT_DIR$/tests/test_xmr.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/statprocon/charts/xmr/limits/trending.py" beforeDir="false" afterPath="$PROJECT_DIR$/statprocon/charts/xmr/limits/trending.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -61,15 +59,15 @@
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/statprocon/charts/xmr"/>
       <recent name="$PROJECT_DIR$/statprocon/charts"/>
       <recent name="$PROJECT_DIR$"/>
     </key>
   </component>
-  <component name="RunManager">
+  <component name="RunManager" selected="Python tests.Unittests for test_xmr.XmRTestCase.test_trending_limits_subset">
     <configuration name="Unittests for test_xmr.XmRTestCase.test_rule_1_points_beyond_both_limits" type="tests" factoryName="Unittests" temporary="true" nameIsGenerated="true">
       <module name="xmr"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
@@ -77,16 +75,48 @@
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;test_xmr.XmRTestCase.test_rule_1_points_beyond_both_limits&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
+    <configuration name="Unittests for test_xmr.XmRTestCase.test_trended_limits" type="tests" factoryName="Unittests" temporary="true" nameIsGenerated="true">
+      <module name="xmr"/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
+      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
+      <option name="_new_additionalArguments" value="&quot;&quot;"/>
+      <option name="_new_target" value="&quot;test_xmr.XmRTestCase.test_trended_limits&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
+      <method v="2"/>
+    </configuration>
+    <configuration name="Unittests for test_xmr.XmRTestCase.test_trending_limits_subset" type="tests" factoryName="Unittests" temporary="true" nameIsGenerated="true">
+      <module name="xmr"/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
+      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
+      <option name="_new_additionalArguments" value="&quot;&quot;"/>
+      <option name="_new_target" value="&quot;test_xmr.XmRTestCase.test_trending_limits_subset&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
+      <method v="2"/>
+    </configuration>
     <recent_temporary>
       <list>
+        <item itemvalue="Python tests.Unittests for test_xmr.XmRTestCase.test_trending_limits_subset"/>
+        <item itemvalue="Python tests.Unittests for test_xmr.XmRTestCase.test_trended_limits"/>
         <item itemvalue="Python tests.Unittests for test_xmr.XmRTestCase.test_rule_1_points_beyond_both_limits"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
@@ -95,15 +125,15 @@
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1688827023388</updated>
       <workItem from="1688827024910" duration="1917000"/>
       <workItem from="1688848868641" duration="17704000"/>
       <workItem from="1688944372544" duration="17391000"/>
       <workItem from="1690054614395" duration="31231000"/>
-      <workItem from="1690685043590" duration="13677000"/>
+      <workItem from="1690685043590" duration="29063000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
@@ -127,10 +157,12 @@
           </value>
         </entry>
       </map>
     </option>
     <option name="oldMeFiltersMigrated" value="true"/>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
+    <SUITE FILE_PATH="coverage/statprocon$Unittests_for_test_xmr_XmRTestCase_test_trended_limits.coverage" NAME="Unittests for test_xmr.XmRTestCase.test_trended_limits Coverage Results" MODIFIED="1691119043818" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
+    <SUITE FILE_PATH="coverage/statprocon$Unittests_for_test_xmr_XmRTestCase_test_trending_limits_subset.coverage" NAME="Unittests for test_xmr.XmRTestCase.test_trending_limits_subset Coverage Results" MODIFIED="1691121663149" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
     <SUITE FILE_PATH="coverage/statprocon$Unittests_for_test_xmr_XmRTestCase_test_rule_1_points_beyond_both_limits.coverage" NAME="Unittests for test_xmr.XmRTestCase.test_rule_1_points_beyond_both_limits Coverage Results" MODIFIED="1688952580683" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
   </component>
 </project>
```

### Comparing `statprocon-0.1.1/.idea/xmr.iml` & `statprocon-0.2.0/.idea/xmr.iml`

 * *Files identical despite different names*

### Comparing `statprocon-0.1.1/statprocon/charts/xmr/base.py` & `statprocon-0.2.0/statprocon/charts/xmr/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,22 +43,23 @@
 
         :param counts: list of data to be used by the X chart
         :param x_central_line_uses: Whether to use the 'average' or 'median' for computing the X
             central line.  Defaults to average.  If set to median, moving_range_uses will also be
             set to median.
         :param moving_range_uses: Whether to use the 'average' or 'median' moving range.
             Defaults to average.
-        :param subset_start_index: Optional starting index of counts to calculate limits from
-        :param subset_end_index: Optional ending index of counts to calculate limits to
+        :param subset_start_index: Optional starting index of counts to calculate limits from.
+            Defaults to 0
+        :param subset_end_index: Optional ending index + 1 of counts to calculate limits to.
+            Defaults to len(n)
         """
         assert x_central_line_uses in [AVERAGE, MEDIAN]
         assert moving_range_uses in [AVERAGE, MEDIAN]
 
         self.counts = cast(TYPE_COUNTS, self.to_decimal_list(counts))
-        self._mr: TYPE_MOVING_RANGES = []
         self.i = max(0, subset_start_index)
         self.j = len(counts)
         if subset_end_index:
             self.j = min(self.j, subset_end_index)
 
         assert self.i <= self.j
 
@@ -128,26 +129,22 @@
         return output.getvalue()
 
     def moving_ranges(self) -> TYPE_MOVING_RANGES:
         """
         Moving ranges are the absolute differences between successive count values.
         The first element will always be None
         """
-        if self._mr:
-            return self._mr
-
         result: list[TYPE_MOVING_RANGE_VALUE] = []
         for i, c in enumerate(self.counts):
             if i == 0:
                 result.append(None)
             else:
                 value = cast(Union[Decimal, int], abs(c - self.counts[i - 1]))
                 result.append(value)
-        self._mr = result
-        return self._mr
+        return result
 
     def x_central_line(self) -> Sequence[Decimal]:
         valid_values = self.counts[self.i:self.j]
         if self._x_central_line_uses == AVERAGE:
             value = self._mean(valid_values)
         elif self._x_central_line_uses == MEDIAN:
             value = statistics.median(valid_values)  # type: ignore[type-var,assignment]
```

### Comparing `statprocon-0.1.1/statprocon/charts/xmr/types.py` & `statprocon-0.2.0/statprocon/charts/xmr/types.py`

 * *Files identical despite different names*

### Comparing `statprocon-0.1.1/tests/test_xmr.py` & `statprocon-0.2.0/tests/test_xmr.py`

 * *Files identical despite different names*

### Comparing `statprocon-0.1.1/LICENSE` & `statprocon-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `statprocon-0.1.1/README.md` & `statprocon-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -85,14 +85,28 @@
 1. Click the 3 dot menu on the right next to `LNPL`
 1. Click `Remove`
 
 The LNPL line will be removed from the X Chart.
 
 ## Advanced Usage
 
+### Trending Limits
+
+With data points that trend upwards or downwards over time, use Trending Limits to calculate a sloping X central line, upper natural process limits and lower natural process limits.
+
+```python
+from statprocon import XmRTrending
+
+counts = [...]  # data from TrendingTestCase.test_trending_limits
+
+source = XmR(counts)
+trending = XmRTrending(source)
+pd.DataFrame(trending.x_to_dict()).astype(float).plot()
+```
+
 ### Use the Median Moving Range
 
 If your data contains extreme outliers, it may be better to compute the limits using the median moving range.
 
 ```python
 xmr = XmR(counts, moving_range_uses='median')
 ```
```

### Comparing `statprocon-0.1.1/pyproject.toml` & `statprocon-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statprocon"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Matt McCormick", email="mattmccor@gmail.com" },
 ]
 description = "A Python helper library for generating Process Behaviour Charts"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `statprocon-0.1.1/PKG-INFO` & `statprocon-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statprocon
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Python helper library for generating Process Behaviour Charts
 Project-URL: Homepage, https://github.com/mattmccormick/statprocon
 Project-URL: Bug Tracker, https://github.com/mattmccormick/statprocon/issues
 Project-URL: Changelog, https://github.com/mattmccormick/statprocon/blob/main/CHANGELOG.md
 Author-email: Matt McCormick <mattmccor@gmail.com>
 License-File: LICENSE
 Keywords: Process Behavior Chart,Process Behaviour Chart,QCC,Quality Control Chart,SPC,Shewhart,Statistical Process Control,Wheeler,XmR
@@ -103,14 +103,28 @@
 1. Click the 3 dot menu on the right next to `LNPL`
 1. Click `Remove`
 
 The LNPL line will be removed from the X Chart.
 
 ## Advanced Usage
 
+### Trending Limits
+
+With data points that trend upwards or downwards over time, use Trending Limits to calculate a sloping X central line, upper natural process limits and lower natural process limits.
+
+```python
+from statprocon import XmRTrending
+
+counts = [...]  # data from TrendingTestCase.test_trending_limits
+
+source = XmR(counts)
+trending = XmRTrending(source)
+pd.DataFrame(trending.x_to_dict()).astype(float).plot()
+```
+
 ### Use the Median Moving Range
 
 If your data contains extreme outliers, it may be better to compute the limits using the median moving range.
 
 ```python
 xmr = XmR(counts, moving_range_uses='median')
 ```
```

