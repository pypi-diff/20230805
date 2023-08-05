# Comparing `tmp/opsanalyze-1.0.tar.gz` & `tmp/opsanalyze-1.1.tar.gz`

## Comparing `opsanalyze-1.0.tar` & `opsanalyze-1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 opsanalyze-1.0/.pypirc
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opsanalyze-1.0/src/opsanalyze/__init__.py
--rw-r--r--   0        0        0    28481 2020-02-02 00:00:00.000000 opsanalyze-1.0/src/opsanalyze/analyze.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 opsanalyze-1.0/LICENSE
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 opsanalyze-1.0/README.md
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 opsanalyze-1.0/pyproject.toml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 opsanalyze-1.0/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 opsanalyze-1.1/.pypirc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opsanalyze-1.1/src/opsanalyze/__init__.py
+-rw-r--r--   0        0        0    28461 2020-02-02 00:00:00.000000 opsanalyze-1.1/src/opsanalyze/analyze.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 opsanalyze-1.1/LICENSE
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 opsanalyze-1.1/README.md
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 opsanalyze-1.1/pyproject.toml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 opsanalyze-1.1/PKG-INFO
```

### Comparing `opsanalyze-1.0/src/opsanalyze/analyze.py` & `opsanalyze-1.1/src/opsanalyze/analyze.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,28 +538,28 @@
 
             ok = ops.analyze(1)
             if ok != 0:
                 num_suc = 0
                 print('    Analysis failed at step ', str(Nstep))
                 du = du / du_Div
                 if abs(du) < du_min:
-                    print('  Analysis failed: du < dumin =  ', str(du_min), '     Loc = ', str(round(node_location, 6)*1000)
-                          , '    Target = ', str(TargetDisp[i]*1000))
+                    print('  Analysis failed: du < dumin =  ', str(du_min), '     Loc = ', str(round(node_location, 6))
+                          , '    Target = ', str(TargetDisp[i]))
 
                     end_time = datetime.now().replace(microsecond=0)
                     print('End Time: {}'.format(end_time))
                     print('Duration: {}'.format(end_time - start_time))
                     exit()
 
                 print('    Try du = ', str(du))
                 ops.integrator('DisplacementControl', cnodeTag, cdof, du, numIter)
             else:
                 node_location += du
-                print('    Analysis successful at step ', str(Nstep), '     Loc = ', str(round(node_location*1000, 2)),
-                          '    Target = ', str(TargetDisp[i]*1000))
+                print('    Analysis successful at step ', str(Nstep), '     Loc = ', str(round(node_location, 2)),
+                          '    Target = ', str(TargetDisp[i]))
 
                 Nstep += 1
                 num_suc += 1
 
     print('Analysis successful')
 
     end_time = datetime.now().replace(microsecond=0)
```

### Comparing `opsanalyze-1.0/LICENSE` & `opsanalyze-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opsanalyze-1.0/README.md` & `opsanalyze-1.1/README.md`

 * *Files identical despite different names*

### Comparing `opsanalyze-1.0/PKG-INFO` & `opsanalyze-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsanalyze
-Version: 1.0
+Version: 1.1
 Summary: A python package To perform analysis of models created by opensees
 Author-email: Okhtay Alizadeh Arasi <ok.programss@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

