# Comparing `tmp/ipc_worker-0.0.8-py3-none-any.whl.zip` & `tmp/ipc_worker-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,19 @@
-Zip file size: 26938 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat    17213 b- defN 23-Feb-01 12:01 ipc_worker/.__data__.pys
--rw-rw-rw-  2.0 fat      414 b- defN 22-Apr-07 07:42 ipc_worker/__init__.py
--rw-rw-rw-  2.0 fat      125 b- defN 21-Dec-02 10:54 ipc_worker/ipc_shm_loader.py
--rw-rw-rw-  2.0 fat      127 b- defN 21-Dec-02 10:54 ipc_worker/ipc_zmq_loader.py
--rw-rw-rw-  2.0 fat     2656 b- defN 21-Dec-02 10:54 ipc_worker/test_shm_ipc.py
--rw-rw-rw-  2.0 fat     2428 b- defN 21-Dec-02 10:54 ipc_worker/test_zmq_ipc.py
--rw-rw-rw-  2.0 fat      748 b- defN 23-Feb-01 11:01 ipc_worker/utils.py
--rw-rw-rw-  2.0 fat      126 b- defN 21-Nov-30 10:42 ipc_worker/shm_module/__init__.py
--rw-rw-rw-  2.0 fat     4423 b- defN 22-Jun-23 14:35 ipc_worker/shm_module/ipc_shm.py
--rw-rw-rw-  2.0 fat      126 b- defN 21-Nov-30 10:42 ipc_worker/zmq_module/__init__.py
--rw-rw-rw-  2.0 fat     3276 b- defN 21-Dec-02 10:54 ipc_worker/zmq_module/ipc_zmq.py
--rw-rw-rw-  2.0 fat     6408 b- defN 23-Feb-01 12:02 ipc_worker-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-01 12:02 ipc_worker-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       55 b- defN 23-Feb-01 12:02 ipc_worker-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1235 b- defN 23-Feb-01 12:02 ipc_worker-0.0.8.dist-info/RECORD
-15 files, 39452 bytes uncompressed, 24890 bytes compressed:  36.9%
+Zip file size: 16840 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat       58 b- defN 23-Jun-09 02:25 ipc_worker/__init__.py
+-rw-rw-rw-  2.0 fat      124 b- defN 23-Jun-09 02:21 ipc_worker/ipc_shm_loader.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Jun-09 02:21 ipc_worker/ipc_zmq_loader.py
+-rw-rw-rw-  2.0 fat      747 b- defN 23-Jun-09 02:21 ipc_worker/utils.py
+-rw-rw-rw-  2.0 fat      126 b- defN 21-Nov-29 07:10 ipc_worker/shm_module/__init__.py
+-rw-rw-rw-  2.0 fat     4423 b- defN 22-Jun-08 06:11 ipc_worker/shm_module/ipc_shm.py
+-rw-rw-rw-  2.0 fat     6058 b- defN 23-Jun-09 02:21 ipc_worker/shm_module/ipc_shm_utils.py
+-rw-rw-rw-  2.0 fat     2177 b- defN 23-Jun-09 02:21 ipc_worker/shm_module/ipc_utils_func.py
+-rw-rw-rw-  2.0 fat      126 b- defN 21-Nov-29 07:19 ipc_worker/zmq_module/__init__.py
+-rw-rw-rw-  2.0 fat      876 b- defN 23-Jun-09 02:21 ipc_worker/zmq_module/ipc_utils_func.py
+-rw-rw-rw-  2.0 fat     3253 b- defN 23-Jun-09 02:21 ipc_worker/zmq_module/ipc_zmq.py
+-rw-rw-rw-  2.0 fat     7350 b- defN 21-Dec-01 06:10 ipc_worker/zmq_module/ipc_zmq_utils.py
+-rw-rw-rw-  2.0 fat    11357 b- defN 23-Jul-21 02:29 ipc_worker-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6449 b- defN 23-Jul-21 02:29 ipc_worker-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 02:29 ipc_worker-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-21 02:29 ipc_worker-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1459 b- defN 23-Jul-21 02:29 ipc_worker-0.0.9.dist-info/RECORD
+17 files, 44812 bytes uncompressed, 14416 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,46 +1,52 @@
-Filename: ipc_worker/.__data__.pys
-Comment: 
-
 Filename: ipc_worker/__init__.py
 Comment: 
 
 Filename: ipc_worker/ipc_shm_loader.py
 Comment: 
 
 Filename: ipc_worker/ipc_zmq_loader.py
 Comment: 
 
-Filename: ipc_worker/test_shm_ipc.py
+Filename: ipc_worker/utils.py
 Comment: 
 
-Filename: ipc_worker/test_zmq_ipc.py
+Filename: ipc_worker/shm_module/__init__.py
 Comment: 
 
-Filename: ipc_worker/utils.py
+Filename: ipc_worker/shm_module/ipc_shm.py
 Comment: 
 
-Filename: ipc_worker/shm_module/__init__.py
+Filename: ipc_worker/shm_module/ipc_shm_utils.py
 Comment: 
 
-Filename: ipc_worker/shm_module/ipc_shm.py
+Filename: ipc_worker/shm_module/ipc_utils_func.py
 Comment: 
 
 Filename: ipc_worker/zmq_module/__init__.py
 Comment: 
 
+Filename: ipc_worker/zmq_module/ipc_utils_func.py
+Comment: 
+
 Filename: ipc_worker/zmq_module/ipc_zmq.py
 Comment: 
 
-Filename: ipc_worker-0.0.8.dist-info/METADATA
+Filename: ipc_worker/zmq_module/ipc_zmq_utils.py
+Comment: 
+
+Filename: ipc_worker-0.0.9.dist-info/LICENSE
+Comment: 
+
+Filename: ipc_worker-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: ipc_worker-0.0.8.dist-info/WHEEL
+Filename: ipc_worker-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: ipc_worker-0.0.8.dist-info/top_level.txt
+Filename: ipc_worker-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ipc_worker-0.0.8.dist-info/RECORD
+Filename: ipc_worker-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipc_worker/__init__.py

```diff
@@ -1,11 +1,3 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/23 10:32
 
-import os
-from se_imports import se_register_module
-__is_ready__ = False
-project_data_dir =  os.path.abspath(os.path.join(os.path.dirname(__file__),'.__data__.pys'))
-if not __is_ready__ and os.path.exists(project_data_dir):
-    __is_ready__ = True
-    root_dir = os.path.abspath(os.path.dirname(__file__))
-    se_register_module(root_dir=root_dir)
```

## ipc_worker/ipc_shm_loader.py

```diff
@@ -1,5 +1,5 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/12/1 11:01
-# @Author  : wyw
+# @Author  : tk
 
 from .shm_module import IPC_shm,SHM_process_worker
```

## ipc_worker/ipc_zmq_loader.py

```diff
@@ -1,6 +1,6 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/12/1 11:00
-# @Author  : wyw
+# @Author  : tk
 
 
 from .zmq_module import IPC_zmq,ZMQ_process_worker
```

## ipc_worker/utils.py

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/30 10:22
-# @Author  : wyw
+# @Author  : tk
 
 import logging
 
 def set_logger(context, verbose=False):
     # if os.name == 'nt':  # for Windows
     #     return NTLogger(context, verbose)
```

## ipc_worker/zmq_module/ipc_zmq.py

```diff
@@ -1,20 +1,19 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/29 13:45
-# @Author  : wyw
+# @Author  : tk
 
 #coding: utf-8
-
 import multiprocessing
 import random
 import time
 
 from .ipc_zmq_utils import ZMQ_manager,ZMQ_sink,ZMQ_worker
 import pickle
-# import numpy as np
+
 
 
 class ZMQ_process_worker(ZMQ_worker):
     def __init__(self,*args,**kwargs):
         super(ZMQ_process_worker,self).__init__(*args,**kwargs)
 
     #Process begin trigger this func
```

## Comparing `ipc_worker-0.0.8.dist-info/METADATA` & `ipc_worker-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ipc-worker
-Version: 0.0.8
+Version: 0.0.9
 Summary: ipc-worker: Inter-Process Communication , muti Process Woker works by share memory or MQ.
-Home-page: https://github.com/ssbuild
+Home-page: https://github.com/ssbuild/ipc_worker
 Author: ssbuild
 Author-email: 9727464@qq.com
 License: Apache 2.0
 Keywords: ipc-worker,ipc_worker,ipc,process worker,ipc,ipc mq,fast-ipc,process ipc
 Platform: win32_AMD64
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,23 +14,24 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3, <4
 Description-Content-Type: text/markdown
-Requires-Dist: se-imports (>=0.1.1)
+Requires-Dist: termcolor
 
 ipc-worker: Inter-Process Communication , muti Process Woker works by share memory or MQ.
 
 ```py
 support share memory (py>=3.8 and linux) and mq process worker (py >=3.6)
 
 ```
@@ -48,19 +49,18 @@
     RuntimeError:
             An attempt has been made to start a new process before the
             current process has finished its bootstrapping phase.
 
 '''
 
 import multiprocessing
-import time,os
+import os
 from ipc_worker.ipc_shm_loader import IPC_shm,SHM_process_worker
 
 
-
 class My_worker(SHM_process_worker):
     def __init__(self,config,*args,**kwargs):
         super(My_worker,self).__init__(*args,**kwargs)
         #config info , use by yourself
 
         self._logger.info('Process id {}, group name {} ,shm name {}'.format(self._idx,self._group_name,self._shm_name))
         self._logger.info(config)
@@ -127,24 +127,23 @@
         instance.terminate()
 
     del evt_quit
 ```
 ```py
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/29 15:06
-# @Author  : wyw
-
+# @Author  : tk
 
 import multiprocessing
 import os
 from ipc_worker.ipc_zmq_loader import IPC_zmq,ZMQ_process_worker
 '''
     demo ZMQ depend zmq
     pip install pyzmq
-    
+
     test pass >= python3.6
 '''
 
 tmp_dir = './tmp'
 if not os.path.exists(tmp_dir):
     os.mkdir(tmp_dir)
 
@@ -212,7 +211,9 @@
     try:
         instance.join()
     except Exception as e:
         evt_quit.set()
         instance.terminate()
     del evt_quit
 ```
+
+
```

## Comparing `ipc_worker-0.0.8.dist-info/RECORD` & `ipc_worker-0.0.9.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-ipc_worker/.__data__.pys,sha256=L1Vb3duMKjeX0gEmGii42uYiixQ7MTxH7YwILvdJYTw,17213
-ipc_worker/__init__.py,sha256=TW_DQJalCgt887vT-3w-1qNjo5e-Vj5Ubr-1mwvdIIw,414
-ipc_worker/ipc_shm_loader.py,sha256=cQJFvg6YCJI6h-aMlAXkc5oQeH0AMM77khPTs2IVo_0,125
-ipc_worker/ipc_zmq_loader.py,sha256=UWSjT3sHpY5vQwNd5tpZlFCxBvHJnrJWe6as5BKaPn8,127
-ipc_worker/test_shm_ipc.py,sha256=gtqqEb7A9IRV1nJFJsQSafKwIdxn51yGoY-yzyCl3MY,2656
-ipc_worker/test_zmq_ipc.py,sha256=sN6MEAnMte91ngOslaqFmHMXgRX_eYOe87yva4-rleM,2428
-ipc_worker/utils.py,sha256=jE0soeqEX7q9djPY2n0uS5pNwT9W3htdqc3inc6Msg0,748
+ipc_worker/__init__.py,sha256=ruMRfWWdrQrctlcYRmigcgHlWq4EEtre5W3KIeLKl54,58
+ipc_worker/ipc_shm_loader.py,sha256=qloEFkmb0v7Ttp3ANo5A1gy26zvkrq-Ey40FC71cQlE,124
+ipc_worker/ipc_zmq_loader.py,sha256=eGAAxWe19H51mWZsW675sGY2YrMXI1m6e4L1VjjRqPY,126
+ipc_worker/utils.py,sha256=w8s14j211ZKOnPkkPFFoeEOtzS7xTIYB_ddrVSPuzjM,747
 ipc_worker/shm_module/__init__.py,sha256=xiptFd-Wn-CHHHrn76PjheyxuIQKmTfEbPKejYxb84Q,126
 ipc_worker/shm_module/ipc_shm.py,sha256=P63p-tnanvkDX0NlNBPcpxbeozbBRAhhx0_f6A1jIjA,4423
+ipc_worker/shm_module/ipc_shm_utils.py,sha256=b2UbaB8FNP6oeaWGQmJC38jLDrSEJIafg9OXbrlYoo0,6058
+ipc_worker/shm_module/ipc_utils_func.py,sha256=KwSnmVTOIc1UfadUoeuTBm33AR5jNqBhPLRhgB39jYc,2177
 ipc_worker/zmq_module/__init__.py,sha256=4HM8jgaXuGG3APy0jqsqcT-edJ09KBfTO64YKO0XMlg,126
-ipc_worker/zmq_module/ipc_zmq.py,sha256=QMYwV1BV5QXnDQYEbd4imJ7P-euOxVRqalA_Bz9vMUw,3276
-ipc_worker-0.0.8.dist-info/METADATA,sha256=C1ki6f2C6BJ5U3of7yyaWLTV43yH7uL2q24pOP_28G8,6408
-ipc_worker-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-ipc_worker-0.0.8.dist-info/top_level.txt,sha256=tR46tFNt1q7uxE4o9UFDLYFdnKz3ED3_l5eKQVeGiz4,55
-ipc_worker-0.0.8.dist-info/RECORD,,
+ipc_worker/zmq_module/ipc_utils_func.py,sha256=qjW3yBhKE6w-BY1hTQYrXOSgCf3Fy1K2A93AVTanpic,876
+ipc_worker/zmq_module/ipc_zmq.py,sha256=863cVUcw8CxbzKtW2G1yWw3R6NPldA81_4PEQO00JlQ,3253
+ipc_worker/zmq_module/ipc_zmq_utils.py,sha256=gkss8abSBkMoBxyi2Nbi8M-4p20BN1ncC9dAJJScky0,7350
+ipc_worker-0.0.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+ipc_worker-0.0.9.dist-info/METADATA,sha256=eeSThkS9OlKWnRtj0wXupcqEmpowI2BnPqtNEwCQssU,6449
+ipc_worker-0.0.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+ipc_worker-0.0.9.dist-info/top_level.txt,sha256=Nt7KccWqNby43j5fBuu3aSszZ17RHYqfHNdgT3LkfgQ,11
+ipc_worker-0.0.9.dist-info/RECORD,,
```

