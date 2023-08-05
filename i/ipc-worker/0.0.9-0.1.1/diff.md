# Comparing `tmp/ipc_worker-0.0.9-py3-none-any.whl.zip` & `tmp/ipc_worker-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 16840 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat       58 b- defN 23-Jun-09 02:25 ipc_worker/__init__.py
--rw-rw-rw-  2.0 fat      124 b- defN 23-Jun-09 02:21 ipc_worker/ipc_shm_loader.py
--rw-rw-rw-  2.0 fat      126 b- defN 23-Jun-09 02:21 ipc_worker/ipc_zmq_loader.py
--rw-rw-rw-  2.0 fat      747 b- defN 23-Jun-09 02:21 ipc_worker/utils.py
--rw-rw-rw-  2.0 fat      126 b- defN 21-Nov-29 07:10 ipc_worker/shm_module/__init__.py
--rw-rw-rw-  2.0 fat     4423 b- defN 22-Jun-08 06:11 ipc_worker/shm_module/ipc_shm.py
--rw-rw-rw-  2.0 fat     6058 b- defN 23-Jun-09 02:21 ipc_worker/shm_module/ipc_shm_utils.py
--rw-rw-rw-  2.0 fat     2177 b- defN 23-Jun-09 02:21 ipc_worker/shm_module/ipc_utils_func.py
--rw-rw-rw-  2.0 fat      126 b- defN 21-Nov-29 07:19 ipc_worker/zmq_module/__init__.py
--rw-rw-rw-  2.0 fat      876 b- defN 23-Jun-09 02:21 ipc_worker/zmq_module/ipc_utils_func.py
--rw-rw-rw-  2.0 fat     3253 b- defN 23-Jun-09 02:21 ipc_worker/zmq_module/ipc_zmq.py
--rw-rw-rw-  2.0 fat     7350 b- defN 21-Dec-01 06:10 ipc_worker/zmq_module/ipc_zmq_utils.py
--rw-rw-rw-  2.0 fat    11357 b- defN 23-Jul-21 02:29 ipc_worker-0.0.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6449 b- defN 23-Jul-21 02:29 ipc_worker-0.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 02:29 ipc_worker-0.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-21 02:29 ipc_worker-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1459 b- defN 23-Jul-21 02:29 ipc_worker-0.0.9.dist-info/RECORD
-17 files, 44812 bytes uncompressed, 14416 bytes compressed:  67.8%
+Zip file size: 17553 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat       83 b- defN 23-Aug-05 15:13 ipc_worker/__init__.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-05 15:32 ipc_worker/ipc_shm_loader.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-05 12:22 ipc_worker/ipc_zmq_loader.py
+-rw-rw-rw-  2.0 fat      839 b- defN 23-Aug-05 15:11 ipc_worker/utils.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-05 12:22 ipc_worker/shm_module/__init__.py
+-rw-rw-rw-  2.0 fat     5087 b- defN 23-Aug-05 17:51 ipc_worker/shm_module/ipc_shm.py
+-rw-rw-rw-  2.0 fat     8445 b- defN 23-Aug-05 15:16 ipc_worker/shm_module/ipc_shm_utils.py
+-rw-rw-rw-  2.0 fat     2194 b- defN 23-Aug-05 15:15 ipc_worker/shm_module/ipc_utils_func.py
+-rw-rw-rw-  2.0 fat      126 b- defN 23-Aug-05 12:22 ipc_worker/zmq_module/__init__.py
+-rw-rw-rw-  2.0 fat      878 b- defN 23-Aug-05 15:32 ipc_worker/zmq_module/ipc_utils_func.py
+-rw-rw-rw-  2.0 fat     3409 b- defN 23-Aug-05 18:15 ipc_worker/zmq_module/ipc_zmq.py
+-rw-rw-rw-  2.0 fat     9009 b- defN 23-Aug-05 17:49 ipc_worker/zmq_module/ipc_zmq_utils.py
+-rw-rw-rw-  2.0 fat    11357 b- defN 23-Aug-05 18:20 ipc_worker-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6757 b- defN 23-Aug-05 18:20 ipc_worker-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-05 18:20 ipc_worker-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-05 18:20 ipc_worker-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1459 b- defN 23-Aug-05 18:20 ipc_worker-0.1.1.dist-info/RECORD
+17 files, 50124 bytes uncompressed, 15129 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: ipc_worker/zmq_module/ipc_zmq.py
 Comment: 
 
 Filename: ipc_worker/zmq_module/ipc_zmq_utils.py
 Comment: 
 
-Filename: ipc_worker-0.0.9.dist-info/LICENSE
+Filename: ipc_worker-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: ipc_worker-0.0.9.dist-info/METADATA
+Filename: ipc_worker-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: ipc_worker-0.0.9.dist-info/WHEEL
+Filename: ipc_worker-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ipc_worker-0.0.9.dist-info/top_level.txt
+Filename: ipc_worker-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ipc_worker-0.0.9.dist-info/RECORD
+Filename: ipc_worker-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ipc_worker/__init__.py

```diff
@@ -1,3 +1,4 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/23 10:32
 
+from .utils import logger
```

## ipc_worker/ipc_shm_loader.py

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/12/1 11:01
 # @Author  : tk
 
-from .shm_module import IPC_shm,SHM_process_worker
+from .shm_module import IPC_shm,SHM_process_worker
```

## ipc_worker/utils.py

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/30 10:22
 # @Author  : tk
 
 import logging
+from termcolor import colored
+
 
 def set_logger(context, verbose=False):
     # if os.name == 'nt':  # for Windows
     #     return NTLogger(context, verbose)
 
     logger = logging.getLogger(context)
     logger.setLevel(logging.DEBUG if verbose else logging.INFO)
@@ -14,8 +16,11 @@
         '%(levelname)-.1s:' + context + ':[%(filename)s:%(funcName)s:%(lineno)3d]:%(message)s', datefmt=
         '%m-%d %H:%M:%S')
     console_handler = logging.StreamHandler()
     console_handler.setLevel(logging.DEBUG if verbose else logging.INFO)
     console_handler.setFormatter(formatter)
     logger.handlers = []
     logger.addHandler(console_handler)
-    return logger
+    return logger
+
+
+logger = set_logger(colored('VENTILATOR', 'magenta'))
```

## ipc_worker/shm_module/ipc_shm.py

```diff
@@ -1,16 +1,14 @@
 #coding: utf-8
-
 import multiprocessing
+import time
 from threading import Lock
 from .ipc_shm_utils import SHM_manager,SHM_woker
 import pickle
 # import numpy as np
-
-
 class SHM_process_worker(SHM_woker):
     def __init__(self,*args,**kwargs):
         super(SHM_process_worker,self).__init__(*args,**kwargs)
 
     #Process begin trigger this func
     def run_begin(self):
         raise NotImplementedError
@@ -31,27 +29,28 @@
                  worker_args: tuple,
                  worker_num: int,
                  manager_num: int,
                  group_name,
                  evt_quit=multiprocessing.Manager().Event(),
                  shm_size=1 * 1024 * 1024,
                  queue_size=20,
-                 is_log_time=False
+                 is_log_time=False,
+                 daemon=False
                  ):
         self.__manager_lst = []
         self.__woker_lst = []
         self.__signal_list = []
         self.__shm_name_list = []
 
         self.__input_queue = None
         self.__output_queue = None
 
 
         self.request_id = 0
-        self.pending_request = set()
+        self.pending_request = {}
         self.pending_response = {}
 
         self.locker = Lock()
 
         assert isinstance(worker_args, tuple)
         self.__input_queue = multiprocessing.Manager().Queue(queue_size)
         self.__output_queue = multiprocessing.Manager().Queue(queue_size)
@@ -64,74 +63,93 @@
                 *worker_args,
                 evt_quit,
                 semaphore,
                 shm_name,
                 shm_size,
                 is_log_time=is_log_time,
                 idx=i,
-                group_name=group_name)
+                group_name=group_name,
+                daemon=daemon)
             self.__signal_list.append(worker.get_signal())
             self.__shm_name_list.append(shm_name)
             self.__woker_lst.append(worker)
-            #worker.start()
 
         semaphore = multiprocessing.Manager().Semaphore(manager_num)
         for i in range(manager_num):
             manager = SHM_manager(evt_quit,
                                   self.__signal_list,
                                   semaphore,
                                   self.__shm_name_list,
                                   self.__input_queue,
                                   self.__output_queue,
                                   is_log_time=is_log_time,
                                   idx=i)
             self.__manager_lst.append(manager)
-            #manager.start()
+        self.__last_t = time.time()
     def start(self):
         for w in self.__woker_lst:
             w.start()
         for w in self.__manager_lst:
             w.start()
 
     def put(self,data):
         self.locker.acquire()
         self.request_id += 1
         request_id = self.request_id
-        self.pending_request.add(request_id)
+        self.pending_request[request_id] = time.time()
         self.__input_queue.put((request_id,pickle.dumps(data)))
         self.locker.release()
         return request_id
 
     def get(self,request_id):
-        #data has serializated
+        c_t = time.time()
+        if (c_t - self.__last_t) / 600 > 0:
+            self.__last_t = c_t
+            invalid = set({rid for rid, t in self.pending_request.items() if (c_t - t) / 3600 > 0})
+            for rid in invalid:
+                self.pending_request.pop(rid)
+
         response = None
         while True:
             is_end = False
             self.locker.acquire(blocking=False)
             if request_id in self.pending_request:
+                self.pending_request[request_id] = time.time()
                 if request_id in self.pending_response:
                     response = self.pending_response.pop(request_id)
-                    self.pending_request.remove(request_id)
                     is_end = True
                 else:
-                    r_id, response = self.__output_queue.get()
+                    r_id,_,seq_id, response = self.__output_queue.get()
                     if r_id != request_id:
                         self.pending_response[r_id] = response
                     else:
                         is_end = True
             else:
                 print('bad request_id {}'.format(request_id))
                 is_end = True
-            self.locker.release()
+            if self.locker.locked():
+                self.locker.release()
             if is_end:
                 break
         return response
 
     def join(self):
         for p in self.__manager_lst:
             p.join()
         for p in self.__woker_lst:
             p.join()
 
     def terminate(self):
-        for p in self.__woker_lst:
+        for p in self.__woker_lst + self.__manager_lst:
+            try:
+                p.release()
+            except Exception as e:
+                pass
             p.terminate()
+
+    @property
+    def manager_process_list(self):
+        return self.__manager_lst
+
+    @property
+    def woker_process_list(self):
+        return self.__woker_lst
```

## ipc_worker/shm_module/ipc_shm_utils.py

```diff
@@ -11,27 +11,30 @@
 import struct
 import multiprocessing
 import traceback
 from multiprocessing import Event,Condition,Process
 from datetime import datetime
 import numpy as np
 import pickle
-from .ipc_utils_func import set_logger,C_sharedata
-from termcolor import colored
+import typing
+from .ipc_utils_func import C_sharedata, WorkState
+from ..utils import logger
+
+
 
 class SHM_manager(Process):
     def __init__(self,evt_quit,
                  signal_list,semaphore,
                  shm_name_list,
                  input_queue,
                  output_queue,
                  is_log_time,
-                 idx):
-        super().__init__(daemon=True)
-        self._logger = set_logger(colored('VENTILATOR', 'magenta'))
+                 idx,
+                 daemon=False):
+        super().__init__(daemon=daemon)
         self._evt_quit = evt_quit
         self._signal_list = signal_list
 
         self._semaphore = semaphore
         self._shm_name_list = shm_name_list
 
         self._input_queue = input_queue
@@ -45,82 +48,107 @@
     def get_input_queue(self):
         return self._input_queue
 
     def get_output_queue(self):
         return self._output_queue
 
     def get_real_data(self,buf):
-        len = struct.unpack('i',buf[4:8])[0]
-        d = buf[8:8+len]
+        len = struct.unpack('i',buf[12:16])[0]
+        d = buf[16:16+len]
         #队列不能序列化 bytes
         return pickle.loads(d)
 
+    def release(self):
+        if not getattr(self,'__is_closed',False):
+            self._input_queue.close()
+            self._output_queue.close()
+            setattr(self,'__is_closed',True)
+
     def run(self):
         shm_list = []
         for shm_name in self._shm_name_list:
             s_d = C_sharedata(name=shm_name,create=False)
             shm_list.append(s_d)
         task_queue1 = self._input_queue
         task_queue2 = self._output_queue
 
         s_d_id_list = []
-        while True:
-            request_id,msg = task_queue1.get()
-            if self._evt_quit.is_set():
-                break
-            s_d_id_list.clear()
-            self._semaphore.acquire()
-            for i,node in enumerate(shm_list):
-                flag = struct.unpack("i", node.buf[0:4])[0]
-                if flag == 0:
-                    s_d_id_list.append(i)
-            if len(s_d_id_list) == 0:
-                self._semaphore.release()
-                self._logger.info('service busy  , no worker consume')
-                task_queue1.put((request_id,msg))
-                continue
-            sel_id = random.choices(s_d_id_list)[0]
-            s_d = shm_list[sel_id]
-
-            #if isinstance(msg,dict) else msg
-            # d = pickle.dumps(msg)
-            # print(d)
-
-            d = msg
-            s_d.buf[4:8] = struct.pack("i", len(d))
-            s_d.buf[8:8 + len(d)] = d
-            s_d.buf[0:4] = struct.pack("i", 1)
-            #是否信号，给其他进程
-            self._semaphore.release()
-            self._signal_list[sel_id].set()
-            start_t = datetime.now()
+        try:
             while True:
-                flag = struct.unpack("i", s_d.buf[0:4])[0]
-                if flag == 3:
+                request_id,msg = task_queue1.get()
+                if self._evt_quit.is_set():
                     break
-            p_result = self.get_real_data(s_d.buf)
+                s_d_id_list.clear()
+                self._semaphore.acquire()
+                for i,node in enumerate(shm_list):
+                    flag = struct.unpack("i", node.buf[0:4])[0]
+                    if flag == WorkState.WS_FREE:
+                        s_d_id_list.append(i)
+                if len(s_d_id_list) == 0:
+                    self._semaphore.release()
+                    logger.info('service busy  , no worker consume')
+                    task_queue1.put((request_id,msg))
+                    continue
+                sel_id = random.choices(s_d_id_list)[0]
+                s_d = shm_list[sel_id]
+
+                #if isinstance(msg,dict) else msg
+                # d = pickle.dumps(msg)
+                # print(d)
+
+                d = msg
+                s_d.buf[12:16] = struct.pack("i", len(d))
+                s_d.buf[16:16 + len(d)] = d
+                s_d.buf[0:4] = struct.pack("i", WorkState.WS_REQUEST)
+                #是否信号，给其他进程
+                self._semaphore.release()
+                self._signal_list[sel_id].set()
+                start_t = datetime.now()
+                Flag_step = False
+                while True:
+                    flag = struct.unpack("i", s_d.buf[0:4])[0]
+                    if flag == WorkState.WS_FINISH:
+                        break
+                    elif flag == WorkState.WS_FINISH_STEP:
+                        Flag_step = True
+                        p_result = self.get_real_data(s_d.buf)
+                        worker_id = struct.unpack("i", s_d.buf[4:8])[0]
+                        seq_id = struct.unpack("i", s_d.buf[8:12])[0]
+
+                        s_d.buf[0:4] = struct.pack('i', WorkState.WS_FREE)
+                        task_queue2.put((request_id,worker_id,seq_id, p_result))
+                if not Flag_step:
+                    p_result = self.get_real_data(s_d.buf)
+                    worker_id = struct.unpack("i", s_d.buf[4:8])[0]
+                    seq_id = struct.unpack("i", s_d.buf[8:12])[0]
+
+                    s_d.buf[0:4] = struct.pack('i',WorkState.WS_FREE)
+                    task_queue2.put((request_id,worker_id,seq_id,p_result))
+                else:
+                    s_d.buf[0:4] = struct.pack('i', WorkState.WS_FREE)
 
-            s_d.buf[0:4] = struct.pack('i',0)
-            task_queue2.put((request_id,p_result))
-            if self._is_log_time:
-                deata = datetime.now() - start_t
-                micros = deata.seconds * 1000 + deata.microseconds / 1000
-                self._logger.info('manager workerId {} , runtime {}'.format(sel_id, micros))
+                if self._is_log_time:
+                    deata = datetime.now() - start_t
+                    micros = deata.seconds * 1000 + deata.microseconds / 1000
+                    logger.info('manager workerId {} , runtime {}'.format(sel_id, micros))
+        except Exception as e:
+            print(e)
+        self.release()
 
 class SHM_woker(Process):
     def __init__(self,
                  evt_quit,
                  semaphore,
                  shm_name,
                  shm_size,
                  is_log_time,
                  idx,
-                 group_name):
-        super().__init__(daemon=True)
-        self._logger = set_logger(colored('VENTILATOR', 'magenta'))
+                 group_name,
+                 daemon=False):
+        super().__init__(daemon=daemon)
 
         self._evt_quit = evt_quit
         self._semaphore= semaphore
         self._idx = idx
         self._group_name = group_name
         self._shm_name = shm_name
 
@@ -136,44 +164,68 @@
 
     def run_end(self):
         raise NotImplementedError
 
     def run_once(self,request_data):
         raise NotImplementedError
 
+    def release(self):
+        if not getattr(self, '__is_closed', False):
+            self._evt_signal.set()
+            self._evt_quit.set()
+            setattr(self, '__is_closed', True)
+
     def run(self):
         self.run_begin()
         s_data = self._s_data
         try:
             while True :
                 self._evt_signal.wait()
                 if self._evt_quit.is_set():
                     break
                 self._semaphore.acquire()
                 flag = struct.unpack("i", s_data.buf[0:4])[0]
-                if flag != 1:
+                if flag != WorkState.WS_REQUEST:
                     self._semaphore.release()
                     continue
                 self._evt_signal.clear()
-                #工作者接收任务，修改工作标志
-                s_data.buf[0:4] = struct.pack('i',2)
+
+                s_data.buf[0:4] = struct.pack('i',WorkState.WS_RECIEVE)
                 self._semaphore.release()
-                msg_size = struct.unpack("i", s_data.buf[4:8])[0]
-                msg = s_data.buf[8:8 + msg_size]
+
+                # s_data.buf[8:12] = struct.pack('i',0)
+
+                msg_size = struct.unpack("i", s_data.buf[12:16])[0]
+                msg = s_data.buf[16:16 + msg_size]
                 request_data = pickle.loads(msg)
                 start_t = datetime.now()
-                X = self.run_once(request_data)
-                X = pickle.dumps(X)
-
-                s_data.buf[4:8] = struct.pack("i", len(X))
-                s_data.buf[8:8 + len(X)] = X
-                s_data.buf[0:4] = struct.pack("i", 3)
+                XX = self.run_once(request_data)
+                seq_id = 0
+                if isinstance(XX, typing.Generator):
+                    for X in XX:
+                        seq_id += 1
+                        X = pickle.dumps(X)
+                        s_data.buf[4:8] = struct.pack('i', self._idx)
+                        s_data.buf[8:12] = struct.pack('i', seq_id)
+                        s_data.buf[12:16] = struct.pack("i", len(X))
+                        s_data.buf[16:16 + len(X)] = X
+                        s_data.buf[0:4] = struct.pack("i", WorkState.WS_FINISH_STEP)
+                        while struct.unpack("i", s_data.buf[0:4])[0] != WorkState.WS_FREE:
+                            continue
+                else:
+                    X = pickle.dumps(XX)
+                    s_data.buf[4:8] = struct.pack('i', self._idx)
+                    s_data.buf[8:12] = struct.pack('i', seq_id)
+                    s_data.buf[12:16] = struct.pack("i", len(X))
+                    s_data.buf[16:16 + len(X)] = X
+                    s_data.buf[0:4] = struct.pack("i", WorkState.WS_FINISH)
 
                 if self._is_log_time:
                     deata = datetime.now() - start_t
                     micros = deata.seconds * 1000 + deata.microseconds / 1000
-                    self._logger.info('worker msg_size {} , runtime {}'.format(msg_size,micros))
+                    logger.info('worker msg_size {} , runtime {}'.format(msg_size,micros))
         except Exception as e:
             traceback.print_exc()
-            self._logger.error(e)
+            logger.error(e)
         del s_data
         self.run_end()
+        self.release()
```

## ipc_worker/shm_module/ipc_utils_func.py

```diff
@@ -1,17 +1,20 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/23 10:03
 # @Author  : tk
 
-import os
-from termcolor import colored
 from multiprocessing import shared_memory, Event, Condition
-from ..utils import set_logger
+from ..utils import logger
 
-logger = set_logger(colored('VENTILATOR', 'magenta'))
+class WorkState:
+    WS_FREE = 0
+    WS_REQUEST = 1
+    WS_RECIEVE = 2
+    WS_FINISH = 3
+    WS_FINISH_STEP = 4
 
 # 进程数据交换协议. 标志状态是否空闲（空闲 为0 ， 由数据请求方置为 1 ， 工作者接收该任务置为 2 ,工作完成处理方式置为 3 ， 数据请求方读取万结果后置为0）
 # 数据长度
 # 数据内容
 
 class C_sharedata:
     def __init__(self, name, create=True, size=0):
```

## ipc_worker/zmq_module/ipc_utils_func.py

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/29 9:57
 # @Author  : tk
+
 import os
 import uuid
 import zmq
 
 def auto_bind(socket):
     # socket.bind_to_random_port('tcp://127.0.0.1')
     # return socket.getsockopt(zmq.LAST_ENDPOINT).decode('ascii')
```

## ipc_worker/zmq_module/ipc_zmq.py

```diff
@@ -1,16 +1,13 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2021/11/29 13:45
 # @Author  : tk
-
-#coding: utf-8
 import multiprocessing
 import random
 import time
-
 from .ipc_zmq_utils import ZMQ_manager,ZMQ_sink,ZMQ_worker
 import pickle
 
 
 
 class ZMQ_process_worker(ZMQ_worker):
     def __init__(self,*args,**kwargs):
@@ -35,43 +32,41 @@
                  CLS_worker,
                  worker_args: tuple,
                  worker_num: int,
                  group_name,
                  evt_quit=multiprocessing.Manager().Event(),
                  queue_size=20,
                  is_log_time=False,
+                 daemon=False
                  ):
         self.__manager_lst = []
         self.__woker_lst = []
         self.__group_idenity = []
 
         assert isinstance(worker_args, tuple)
-
-        #ZMQ_worker(identity,evt_quit,ip,port, port_out)
-
         manager = ZMQ_manager(0, queue_size, group_name,evt_quit)
         self.__manager_lst.append(manager)
 
         sink = ZMQ_sink(queue_size,group_name,evt_quit)
         self.__manager_lst.append(sink)
 
         for i in range(worker_num):
             identity = bytes('{}_{}'.format(group_name,i),encoding='utf-8')
             worker = CLS_worker(
                 *worker_args,
-                identity,
-                group_name,
-                evt_quit,
-                is_log_time,
-                i,
+                identity=identity,
+                group_name=group_name,
+                evt_quit=evt_quit,
+                is_log_time=is_log_time,
+                idx=i,
+                daemon=daemon
             )
             self.__group_idenity.append(identity)
             self.__woker_lst.append(worker)
-            #worker.start()
-
+        self.__last_worker_id = len(self.__group_idenity) - 1
     def start(self):
         for w in self.__manager_lst:
             w.start()
 
         for w in self.__manager_lst:
             w.wait_init()
 
@@ -83,37 +78,40 @@
         for w in self.__woker_lst:
             while not w.signal.is_set():
                 pass
             del w.signal
 
 
     def put(self,data):
-        idenity = random.choice(self.__group_idenity)
+        self.__last_worker_id = (self.__last_worker_id + 1 ) % len(self.__group_idenity)
+        idenity = self.__group_idenity[self.__last_worker_id]
         request_id = self.__manager_lst[0].put(idenity,pickle.dumps(data))
         self.__manager_lst[1].add_request_id(request_id)
         return request_id
 
     def get(self,request_id):
-        #data has serializated
         d = self.__manager_lst[1].get(request_id)
         return d if d is None else pickle.loads(d)
 
     def join(self):
         for p in self.__manager_lst:
             p.join()
         time.sleep(1)
         for p in self.__woker_lst:
             p.join()
 
+    @property
+    def manager_process_list(self):
+        return self.__manager_lst
+
+    @property
+    def woker_process_list(self):
+        return self.__woker_lst
+
     def terminate(self):
-        for p in self.__woker_lst:
+        for p in self.__woker_lst + self.__manager_lst:
             try:
-                p.close()
+                p.release()
             except Exception as e:
                 pass
             p.terminate()
-        for p in self.__manager_lst:
-            try:
-                p.close()
-            except Exception as e:
-                pass
-            p.terminate()
+
```

## ipc_worker/zmq_module/ipc_zmq_utils.py

```diff
@@ -1,44 +1,34 @@
 # @Time    : 2021/11/26 21:15
 # @Author  : tk
 # @FileName: zmq_utils.py
 import json
-
-import zmq
+import threading
 import time
-import uuid
-from collections import namedtuple
-# from queue import Queue
+import typing
+import zmq
 from multiprocessing import Queue
 from multiprocessing import Event,Process
 from threading import Lock
-from ..utils import set_logger
-from termcolor import colored
 import pickle
 from datetime import datetime
 from .ipc_utils_func import auto_bind
-
-
+from ..utils import logger
 
 
 class ZMQ_worker(Process):
-    def __init__(self,identity,group_name,evt_quit,is_log_time,idx):
-        super(ZMQ_worker,self).__init__(daemon=True)
-
-        self._logger = set_logger(colored('VENTILATOR', 'magenta'))
-
-        self._identity = identity
+    def __init__(self,identity,group_name,evt_quit,is_log_time,idx,daemon=False):
+        super(ZMQ_worker,self).__init__(daemon=daemon)
+        self.__identity = identity
         self._group_name = group_name
         self._evt_quit = evt_quit
         self._idx = idx
         self._is_log_time = is_log_time
 
-
         self.signal = Event()
-
         self.__is_closed = False
 
 
     def _set_addr(self,addr_sink,addr_pub):
         self._addr_sink = addr_sink
         self._addr_pub = addr_pub
 
@@ -52,156 +42,184 @@
 
     # any data put will trigger this func
     def run_once(self, request_data):
         raise NotImplementedError
 
     def __processinit__(self):
         self._context = zmq.Context()
-        # 消费者 接收代理 数据
         self._receiver = self._context.socket(zmq.SUB)
-        self._receiver.setsockopt(zmq.SUBSCRIBE, self._identity)
+        self._receiver.setsockopt(zmq.SUBSCRIBE, self.__identity)
         # self._receiver.setsockopt(zmq.SUBSCRIBE, b'')
 
         # self._receiver.connect('tcp://{}:{}'.format(self._ip, self._port))
         self._receiver.connect(self._addr_pub)
 
-        # 结果推送
         self._sender = self._context.socket(zmq.PUSH)
         self._sender.setsockopt(zmq.LINGER, 0)
         # self._sender.connect('tcp://{}:{}'.format(self._ip, self._port_out))
         self._sender.connect(self._addr_sink)
 
-    def close(self):
-        if not self.__is_closed:
-            self.__is_closed = True
-            self._receiver.close()
-            self._sender.close()
-            self._context.term()
+    def release(self):
+        try:
+            if not self.__is_closed:
+                self.__is_closed = True
+                self._receiver.close()
+                self._context.term()
+                self._sender.close()
+        except Exception as e:
+            ...
 
     def run(self):
         self.__processinit__()
         self.signal.set()
-
         self.run_begin()
-        while not self._evt_quit.is_set():
-            _,msg,b_request_id = self._receiver.recv_multipart()
-            msg_size = len(msg)
-            request_data = pickle.loads(msg)
-            start_t = datetime.now()
-            X = self.run_once(request_data)
-            X = pickle.dumps(X)
-            self._sender.send_multipart([b_request_id,X])
-            if self._is_log_time:
-                deata = datetime.now() - start_t
-                micros = deata.seconds * 1000 + deata.microseconds / 1000
-                self._logger.info('worker msg_size {} , runtime {}'.format(msg_size, micros))
-        self.close()
-        self.run_end()
-
 
+        try:
+            while not self._evt_quit.is_set():
+                _,msg,b_request_id = self._receiver.recv_multipart()
+                if self.__is_closed:
+                    break
+                msg_size = len(msg)
+                request_data = pickle.loads(msg)
+                start_t = datetime.now()
+                XX = self.run_once(request_data)
+                seq_id = 0
+                if isinstance(XX, typing.Generator):
+                    for X in XX:
+                        seq_id += 1
+                        X = pickle.dumps(X)
+                        self._sender.send_multipart([b_request_id,int.to_bytes(self._idx,4,byteorder="little",signed=False),int.to_bytes(seq_id,4,byteorder="little",signed=False),X])
+                else:
+                    X = pickle.dumps(XX)
+                    self._sender.send_multipart([b_request_id,int.to_bytes(self._idx,4,byteorder="little",signed=False),int.to_bytes(seq_id,4,byteorder="little",signed=False), X])
 
+                if self._is_log_time:
+                    deata = datetime.now() - start_t
+                    micros = deata.seconds * 1000 + deata.microseconds / 1000
+                    logger.debug('worker msg_size {} , runtime {}'.format(msg_size, micros))
+        except Exception as e:
+            print(e)
 
+        self.run_end()
+        self.release()
 
 
 
 
 class ZMQ_sink(Process):
-    def __init__(self,queue_size,group_name,evt_quit):
-        super(ZMQ_sink,self).__init__(daemon=True)
-
-        self.logger = set_logger(colored('VENTILATOR', 'magenta'))
+    def __init__(self,queue_size,group_name,evt_quit,daemon=False):
+        super(ZMQ_sink,self).__init__(daemon=daemon)
 
         self.group_name = group_name
-
-        self.is_closed = False
+        self.__is_closed = False
         self.evt_quit = evt_quit
-        self.pending_request = set()
+        self.pending_request = {}
         self.pending_response = {}
         self.queue = Queue(maxsize=queue_size)
         #
         self.locker = Lock()
         self.signal = Event()
         self.addr = None
     def wait_init(self):
         self.addr = self.queue.get()
 
     def get(self,request_id):
         response = None
         while True:
             is_end = False
-            self.signal.wait(0.01)
-            self.locker.acquire(blocking=False)
+            self.signal.wait(0.005)
+            self.locker.acquire(timeout=0.005)
             if request_id in self.pending_request:
+                self.pending_request[request_id] = time.time()
                 if request_id in self.pending_response:
                     response = self.pending_response.pop(request_id)
-                    self.pending_request.remove(request_id)
                     self.signal.clear()
                     is_end = True
                 else:
-                    r_id,response = self.queue.get()
+                    r_id,w_id,seq_id,response = self.queue.get()
                     if r_id != request_id:
                         self.pending_response[r_id] = response
                     else:
                         is_end = True
             else:
-                self.logger.error('bad request_id {}'.format(request_id))
+                logger.error('bad request_id {}'.format(request_id))
                 is_end = True
-            self.locker.release()
+            if self.locker.locked():
+                self.locker.release()
             if is_end:
                 break
         return response
 
     def __processinit__(self):
         self.context = zmq.Context()
         self.receiver = self.context.socket(zmq.PULL)
         self.receiver.setsockopt(zmq.LINGER, 0)
         # self.receiver.bind('tcp://*:{}'.format(self.port_out))
         self.addr = auto_bind(self.receiver)
-        self.logger.info('group {} sink bind {}'.format(self.group_name,self.addr))
+        logger.debug('group {} sink bind {}'.format(self.group_name,self.addr))
         self.queue.put(self.addr)
 
-    def close(self):
-        if not self.is_closed:
-            self.is_closed = True
-            self.receiver.close()
-            self.context.term()
+    def release(self):
+        try:
+            if not self.__is_closed:
+                self.__is_closed = True
+                self.receiver.close()
+                self.queue.close()
+                self.queue.join_thread()
+                self.context.term()
+        except Exception as e:
+            ...
 
-    def run(self):
-        self.__processinit__()
 
-        while not self.evt_quit.is_set():
-            request_id,response = self.receiver.recv_multipart()
-            r_id = int.from_bytes(request_id, byteorder='little', signed=False)
-            self.queue.put((r_id,response))
-            self.signal.set()
 
-        self.close()
+    def run(self):
+        self.__processinit__()
+        try:
+            last_t = time.time()
+            while not self.evt_quit.is_set():
+                request_id,w_id,seq_id,response = self.receiver.recv_multipart()
+                if self.__is_closed:
+                    break
+
+                c_t = time.time()
+                if (c_t - last_t) / 600 > 0:
+                    last_t = c_t
+                    invalid = set({rid for rid, t in self.pending_request.items() if (c_t - t) / 3600 > 0})
+                    for rid in invalid:
+                        self.pending_request.pop(rid)
+
+                r_id = int.from_bytes(request_id, byteorder='little', signed=False)
+                w_id = int.from_bytes(w_id, byteorder='little', signed=False)
+                seq_id = int.from_bytes(seq_id, byteorder='little', signed=False)
+                self.queue.put((r_id,w_id,seq_id,response))
+                self.signal.set()
+        except Exception as e:
+            print(e)
+        self.release()
 
 
     def add_request_id(self,request_id):
         self.locker.acquire()
-        self.pending_request.add(request_id)
+        self.pending_request[request_id] = time.time()
         self.locker.release()
 
 
-# 数据生产者 , 结果消费者
-class ZMQ_manager(Process):
-    def __init__(self,idx,queue_size,group_name,evt_quit):
-        super(ZMQ_manager, self).__init__(daemon=True)
 
-        self.logger = set_logger(colored('VENTILATOR', 'magenta'))
+class ZMQ_manager(Process):
+    def __init__(self,idx,queue_size,group_name,evt_quit,daemon=False):
+        super(ZMQ_manager, self).__init__(daemon=daemon)
         self.group_name = group_name
         self.request_id = 0
         self.idx = idx
 
         self.queue = Queue(queue_size)
         self.evt_quit = evt_quit
         self.locker = Lock()
         self.addr = None
-        self.is_closed = False
+        self.__is_closed = False
 
     def wait_init(self):
         self.addr = self.queue.get()
 
     def put(self,identity,msg):
         self.locker.acquire()
         self.request_id += 1
@@ -213,23 +231,33 @@
     def __processinit__(self):
         self.context = zmq.Context()
         self.sender = self.context.socket(zmq.PUB)
         self.sender.setsockopt(zmq.LINGER, 0)
         # self.sender.bind('tcp://*:{}'.format(self.port))
         self.addr = auto_bind(self.sender)
         self.queue.put(self.addr)
-    def close(self):
-        if not self.is_closed:
-            self.is_closed = True
-            self.sender.close()
-            self.context.term()
+
+    def release(self):
+        try:
+            if not self.__is_closed:
+                self.__is_closed = True
+                self.queue.close()
+                self.queue.join_thread()
+                self.sender.close()
+                self.context.term()
+        except Exception as e:
+            ...
 
     def run(self):
         self.__processinit__()
-        self.logger.info('group {} manager bind {}'.format(self.group_name,self.addr))
-        while not self.evt_quit.is_set():
-            request_id,identity,msg = self.queue.get()
-            self.sender.send_multipart([identity,msg, request_id.to_bytes(4,byteorder='little',signed=False)])
-
-        self.close()
+        logger.debug('group {} manager bind {}'.format(self.group_name,self.addr))
+        try:
+            while not self.evt_quit.is_set():
+                request_id,identity,msg = self.queue.get()
+                if self.__is_closed:
+                    break
+                self.sender.send_multipart([identity,msg, request_id.to_bytes(4,byteorder='little',signed=False)])
+        except Exception as e:
+            print(e)
+        self.release()
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `ipc_worker-0.0.9.dist-info/LICENSE` & `ipc_worker-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ipc_worker-0.0.9.dist-info/METADATA` & `ipc_worker-0.1.1.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-Metadata-Version: 2.1
-Name: ipc-worker
-Version: 0.0.9
-Summary: ipc-worker: Inter-Process Communication , muti Process Woker works by share memory or MQ.
-Home-page: https://github.com/ssbuild/ipc_worker
-Author: ssbuild
-Author-email: 9727464@qq.com
-License: Apache 2.0
-Keywords: ipc-worker,ipc_worker,ipc,process worker,ipc,ipc mq,fast-ipc,process ipc
-Platform: win32_AMD64
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3, <4
-Description-Content-Type: text/markdown
-Requires-Dist: termcolor
-
-ipc-worker: Inter-Process Communication , muti Process Woker works by share memory or MQ.
-
-```py
-support share memory (py>=3.8 and linux) and mq process worker (py >=3.6)
-
-```
-```py
-# -*- coding: utf-8 -*-
-# @Time    : 2021/11/23 9:35
-
-'''
-demo share memrory
-recommended system linux and python >= 3.8
-    recommended linux
-    python 3.8
-
-Do not recommended run in windows , it will report an error as follow
-    RuntimeError:
-            An attempt has been made to start a new process before the
-            current process has finished its bootstrapping phase.
-
-'''
-
-import multiprocessing
-import os
-from ipc_worker.ipc_shm_loader import IPC_shm,SHM_process_worker
-
-
-class My_worker(SHM_process_worker):
-    def __init__(self,config,*args,**kwargs):
-        super(My_worker,self).__init__(*args,**kwargs)
-        #config info , use by yourself
-
-        self._logger.info('Process id {}, group name {} ,shm name {}'.format(self._idx,self._group_name,self._shm_name))
-        self._logger.info(config)
-        self.config = config
-
-
-    #Process begin trigger this func
-    def run_begin(self):
-        self._logger.info('worker pid {}...'.format(os.getpid()))
-        self.handle = None
-        pass
-
-    # Process end trigger this func
-    def run_end(self):
-        if self.handle is not None:
-            pass
-
-    #any data put will trigger this func
-    def run_once(self,request_data):
-        #process request_data
-        if isinstance(request_data,dict):
-            request_data['b']  = 200
-        if self.handle is not None:
-            #do some thing
-            pass
-        return request_data
-
-
-if __name__ == '__main__':
-    config = {
-        "anything" : "anything",
-        "aa": 100
-    }
-
-    evt_quit = multiprocessing.Manager().Event()
-
-    # group_name 为共享内存组名,需唯一
-    # manager is an agent  and act as a load balancing
-    # worker is real doing your work
-    instance = IPC_shm(
-        CLS_worker=My_worker,
-        worker_args=(config,),  # must be tuple
-        worker_num=10,  # number of worker Process
-        manager_num=2,  # number of agent Process
-        group_name='serving_shm',  # share memory name
-        shm_size=1 * 1024 * 1024,  # share memory size
-        queue_size=20,  # recv queue size
-        is_log_time=True,  # whether log compute time
-    )
-
-    instance.start()
-
-    #demo produce and consume message , you can process by http
-    for i in range(10):
-        print('produce message')
-        data = {"a" : 100}
-        request_id = instance.put(data)
-        data = instance.get(request_id)
-        print('get process result',data)
-    try:
-        instance.join()
-    except Exception as e:
-        evt_quit.set()
-        instance.terminate()
-
-    del evt_quit
-```
-```py
-# -*- coding: utf-8 -*-
-# @Time    : 2021/11/29 15:06
-# @Author  : tk
-
-import multiprocessing
-import os
-from ipc_worker.ipc_zmq_loader import IPC_zmq,ZMQ_process_worker
-'''
-    demo ZMQ depend zmq
-    pip install pyzmq
-
-    test pass >= python3.6
-'''
-
-tmp_dir = './tmp'
-if not os.path.exists(tmp_dir):
-    os.mkdir(tmp_dir)
-
-os.environ['ZEROMQ_SOCK_TMP_DIR'] = tmp_dir
-
-class My_worker(ZMQ_process_worker):
-    def __init__(self,config,*args,**kwargs):
-        super(My_worker,self).__init__(*args,**kwargs)
-        #config info , use by yourself
-        self._logger.info('Process id {}, group name {} , identity {}'.format(self._idx,self._group_name,self._identity))
-        self._logger.info(config)
-        self.config = config
-
-    #Process begin trigger this func
-    def run_begin(self):
-        self._logger.info('worker pid {}...'.format(os.getpid()))
-        self.handle = None
-        pass
-
-    # Process end trigger this func
-    def run_end(self):
-        if self.handle is not None:
-            pass
-
-    #any data put will trigger this func
-    def run_once(self,request_data):
-        #process request_data
-        if isinstance(request_data,dict):
-            request_data['b'] = 200
-        if self.handle is not None:
-            #do some thing
-            pass
-        return request_data
-
-
-if __name__ == '__main__':
-    config = {
-        "anything" : "anything",
-        "aa": 100
-    }
-
-    evt_quit = multiprocessing.Manager().Event()
-
-    # group_name 为共享内存组名,需唯一
-    # manager is an agent  and act as a load balancing
-    # worker is real doing your work
-    instance = IPC_zmq(
-        CLS_worker=My_worker,
-        worker_args=(config,),  # must be tuple
-        worker_num=10,  # number of worker Process
-        group_name='serving_zmq',  # share memory name
-        evt_quit=evt_quit,
-        queue_size=20,  # recv queue size
-        is_log_time=True,  # whether log compute time
-    )
-    instance.start()
-
-    #demo produce and consume message , you can process by http
-    for i in range(10):
-        data = {"a" : 100}
-        request_id = instance.put(data)
-
-        data = instance.get(request_id)
-        print('get process result',request_id,data)
-    try:
-        instance.join()
-    except Exception as e:
-        evt_quit.set()
-        instance.terminate()
-    del evt_quit
-```
-
-
+Metadata-Version: 2.1
+Name: ipc-worker
+Version: 0.1.1
+Summary: ipc-worker: Inter-Process Communication , muti Process Woker works by share memory or MQ.
+Home-page: https://github.com/ssbuild/ipc_worker
+Author: ssbuild
+Author-email: 9727464@qq.com
+License: Apache 2.0
+Keywords: ipc-worker,ipc_worker,ipc,process worker,ipc,ipc mq,fast-ipc,process ipc
+Platform: win32_AMD64
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: termcolor
+
+ipc-worker: Inter-Process Communication , muti Process Woker works by share memory or MQ.
+
+```py
+support share memory (py>=3.8 and linux) and mq process worker (py >=3.6)
+
+```
+```py
+# -*- coding: utf-8 -*-
+# @Time    : 2021/11/23 9:35
+
+'''
+demo share memrory
+recommended system linux and python >= 3.8
+    recommended linux
+    python 3.8
+
+Do not recommended run in windows , it will report an error as follow
+    RuntimeError:
+            An attempt has been made to start a new process before the
+            current process has finished its bootstrapping phase.
+
+'''
+import multiprocessing
+import os
+from ipc_worker import logger
+from ipc_worker.ipc_shm_loader import IPC_shm,SHM_process_worker
+
+class My_worker(SHM_process_worker):
+    def __init__(self,config,*args,**kwargs):
+        super(My_worker,self).__init__(*args,**kwargs)
+        #config info , use by yourself
+
+        logger.info('Process id {}, group name {} ,shm name {}'.format(self._idx,self._group_name,self._shm_name))
+        logger.info(config)
+        self.config = config
+
+
+    #Process begin trigger this func
+    def run_begin(self):
+        logger.info('worker pid {}...'.format(os.getpid()))
+        self.handle = None
+        pass
+
+    # Process end trigger this func
+    def run_end(self):
+        if self.handle is not None:
+            pass
+
+    #any data put will trigger this func
+    def run_once(self,request_data):
+        #process request_data
+        if isinstance(request_data,dict):
+            request_data['b']  = 200
+        if self.handle is not None:
+            #do some thing
+            pass
+        return request_data
+
+
+if __name__ == '__main__':
+    config = {
+        "anything" : "anything",
+        "aa": 100
+    }
+
+    evt_quit = multiprocessing.Manager().Event()
+
+    # group_name 为共享内存组名,需唯一
+    # manager is an agent  and act as a load balancing
+    # worker is real doing your work
+    instance = IPC_shm(
+        CLS_worker=My_worker,
+        worker_args=(config,),  # must be tuple
+        worker_num=10,  # number of worker Process
+        manager_num=2,  # number of agent Process
+        group_name='serving_shm',  # share memory name
+        shm_size=1 * 1024 * 1024,  # share memory size
+        queue_size=20,  # recv queue size
+        is_log_time=True,  # whether log compute time
+        daemon=False,
+    )
+
+    instance.start()
+
+    #demo produce and consume message , you can process by http
+    for i in range(10):
+        print('produce message')
+        data = {"a" : 100}
+        request_id = instance.put(data)
+        data = instance.get(request_id)
+        print('get process result',data)
+    try:
+        instance.join()
+    except Exception as e:
+        evt_quit.set()
+        instance.terminate()
+
+    del evt_quit
+```
+```py
+# -*- coding: utf-8 -*-
+# @Time    : 2021/11/29 15:06
+# @Author  : tk
+import multiprocessing
+import os
+from ipc_worker import logger
+from ipc_worker.ipc_zmq_loader import IPC_zmq,ZMQ_process_worker
+'''
+    demo ZMQ depend zmq
+    pip install pyzmq
+    
+    test pass >= python3.6
+'''
+
+tmp_dir = './tmp'
+if not os.path.exists(tmp_dir):
+    os.mkdir(tmp_dir)
+
+os.environ['ZEROMQ_SOCK_TMP_DIR'] = tmp_dir
+
+class My_worker(ZMQ_process_worker):
+    def __init__(self,config,*args,**kwargs):
+        super(My_worker,self).__init__(*args,**kwargs)
+        #config info , use by yourself
+        logger.info('Process id {}, group name {} , identity {}'.format(self._idx,self._group_name,self._identity))
+        logger.info(config)
+        self.config = config
+
+    #Process begin trigger this func
+    def run_begin(self):
+        logger.info('worker pid {}...'.format(os.getpid()))
+        self.handle = None
+        pass
+
+    # Process end trigger this func
+    def run_end(self):
+        if self.handle is not None:
+            pass
+
+    #any data put will trigger this func
+    def run_once(self,request_data):
+        #process request_data
+        if isinstance(request_data,dict):
+            request_data['b'] = 200
+        if self.handle is not None:
+            #do some thing
+            pass
+        return request_data
+
+
+if __name__ == '__main__':
+    config = {
+        "anything" : "anything",
+        "aa": 100
+    }
+
+    evt_quit = multiprocessing.Manager().Event()
+
+    # group_name 为共享内存组名,需唯一
+    # manager is an agent  and act as a load balancing
+    # worker is real doing your work
+    instance = IPC_zmq(
+        CLS_worker=My_worker,
+        worker_args=(config,),  # must be tuple
+        worker_num=10,  # number of worker Process
+        group_name='serving_zmq',  # share memory name
+        evt_quit=evt_quit,
+        queue_size=20,  # recv queue size
+        is_log_time=True,  # whether log compute time
+        daemon=False,
+    )
+    instance.start()
+
+    #demo produce and consume message , you can process by http
+    for i in range(10):
+        data = {"a" : 100}
+        request_id = instance.put(data)
+
+        data = instance.get(request_id)
+        print('get process result',request_id,data)
+    try:
+        instance.join()
+    except Exception as e:
+        evt_quit.set()
+        instance.terminate()
+    del evt_quit
+```
```

## Comparing `ipc_worker-0.0.9.dist-info/RECORD` & `ipc_worker-0.1.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-ipc_worker/__init__.py,sha256=ruMRfWWdrQrctlcYRmigcgHlWq4EEtre5W3KIeLKl54,58
-ipc_worker/ipc_shm_loader.py,sha256=qloEFkmb0v7Ttp3ANo5A1gy26zvkrq-Ey40FC71cQlE,124
+ipc_worker/__init__.py,sha256=fK3ASYKB5vx3P71YnrPzgFtrrpc0nuv7NrbDXjh0KmA,83
+ipc_worker/ipc_shm_loader.py,sha256=xKqpZQPfNtcUgVVt5iOlEqVWCt7ws5uvU6GsuqT8eeE,126
 ipc_worker/ipc_zmq_loader.py,sha256=eGAAxWe19H51mWZsW675sGY2YrMXI1m6e4L1VjjRqPY,126
-ipc_worker/utils.py,sha256=w8s14j211ZKOnPkkPFFoeEOtzS7xTIYB_ddrVSPuzjM,747
+ipc_worker/utils.py,sha256=UHkLeqz89qK6PCstESVUXHKjHt8isEMbE_ryDlBC2No,839
 ipc_worker/shm_module/__init__.py,sha256=xiptFd-Wn-CHHHrn76PjheyxuIQKmTfEbPKejYxb84Q,126
-ipc_worker/shm_module/ipc_shm.py,sha256=P63p-tnanvkDX0NlNBPcpxbeozbBRAhhx0_f6A1jIjA,4423
-ipc_worker/shm_module/ipc_shm_utils.py,sha256=b2UbaB8FNP6oeaWGQmJC38jLDrSEJIafg9OXbrlYoo0,6058
-ipc_worker/shm_module/ipc_utils_func.py,sha256=KwSnmVTOIc1UfadUoeuTBm33AR5jNqBhPLRhgB39jYc,2177
+ipc_worker/shm_module/ipc_shm.py,sha256=TRW89Lw37Z0IwlmU3JYbEzYFav3PN8qw4h70AsSRaOY,5087
+ipc_worker/shm_module/ipc_shm_utils.py,sha256=UiCuddy0ebVAosR3u5yeVWpKhT1LAKWaPMFBius3VCI,8445
+ipc_worker/shm_module/ipc_utils_func.py,sha256=YNkqqMDFhMFgMSE1GEvBlxNR3g_HIVZGy0PySZU-lCY,2194
 ipc_worker/zmq_module/__init__.py,sha256=4HM8jgaXuGG3APy0jqsqcT-edJ09KBfTO64YKO0XMlg,126
-ipc_worker/zmq_module/ipc_utils_func.py,sha256=qjW3yBhKE6w-BY1hTQYrXOSgCf3Fy1K2A93AVTanpic,876
-ipc_worker/zmq_module/ipc_zmq.py,sha256=863cVUcw8CxbzKtW2G1yWw3R6NPldA81_4PEQO00JlQ,3253
-ipc_worker/zmq_module/ipc_zmq_utils.py,sha256=gkss8abSBkMoBxyi2Nbi8M-4p20BN1ncC9dAJJScky0,7350
-ipc_worker-0.0.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-ipc_worker-0.0.9.dist-info/METADATA,sha256=eeSThkS9OlKWnRtj0wXupcqEmpowI2BnPqtNEwCQssU,6449
-ipc_worker-0.0.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-ipc_worker-0.0.9.dist-info/top_level.txt,sha256=Nt7KccWqNby43j5fBuu3aSszZ17RHYqfHNdgT3LkfgQ,11
-ipc_worker-0.0.9.dist-info/RECORD,,
+ipc_worker/zmq_module/ipc_utils_func.py,sha256=zvz9DZ99RMBvGHsFbAhNQ0LWn-5eIn2K8mh4cJJyCc0,878
+ipc_worker/zmq_module/ipc_zmq.py,sha256=aIQKub_EOgqEj1Zfke9djLliZqfZRw0E7C_fR2W72a0,3409
+ipc_worker/zmq_module/ipc_zmq_utils.py,sha256=LrLgXXx46H3xep1nmtyYg2_aXscYvkviAwCSG90uKDc,9009
+ipc_worker-0.1.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+ipc_worker-0.1.1.dist-info/METADATA,sha256=W591Fgq9RG90AujvN-zVZxbeCaHCtmSHbKSrfY7YAVo,6757
+ipc_worker-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ipc_worker-0.1.1.dist-info/top_level.txt,sha256=Nt7KccWqNby43j5fBuu3aSszZ17RHYqfHNdgT3LkfgQ,11
+ipc_worker-0.1.1.dist-info/RECORD,,
```

