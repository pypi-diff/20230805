# Comparing `tmp/froog-0.2.0.tar.gz` & `tmp/froog-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froog-0.2.0.tar", last modified: Wed Aug  2 01:29:54 2023, max compression
+gzip compressed data, was "froog-0.2.1.tar", last modified: Fri Aug  4 18:25:53 2023, max compression
```

## Comparing `froog-0.2.0.tar` & `froog-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-02 01:29:54.071290 froog-0.2.0/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.2.0/LICENSE
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2995 2023-08-02 01:29:54.071153 froog-0.2.0/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2670 2023-08-02 00:11:34.000000 froog-0.2.0/README.md
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-02 01:29:54.069563 froog-0.2.0/froog/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       57 2023-07-26 06:32:22.000000 froog-0.2.0/froog/__init__.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2417 2023-07-30 06:46:05.000000 froog-0.2.0/froog/gradcheck.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1882 2023-07-28 16:42:26.000000 froog-0.2.0/froog/nn.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)    14381 2023-07-30 19:25:09.000000 froog-0.2.0/froog/ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     4902 2023-07-30 21:07:16.000000 froog-0.2.0/froog/ops_gpu.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2355 2023-07-30 06:46:05.000000 froog-0.2.0/froog/optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     7230 2023-08-02 01:26:16.000000 froog-0.2.0/froog/tensor.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3079 2023-07-30 01:43:20.000000 froog-0.2.0/froog/utils.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-02 01:29:54.070204 froog-0.2.0/froog.egg-info/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2995 2023-08-02 01:29:54.000000 froog-0.2.0/froog.egg-info/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      416 2023-08-02 01:29:54.000000 froog-0.2.0/froog.egg-info/SOURCES.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-08-02 01:29:54.000000 froog-0.2.0/froog.egg-info/dependency_links.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-08-02 01:29:54.000000 froog-0.2.0/froog.egg-info/requires.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        6 2023-08-02 01:29:54.000000 froog-0.2.0/froog.egg-info/top_level.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-08-02 01:29:54.071326 froog-0.2.0/setup.cfg
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      851 2023-08-02 01:29:38.000000 froog-0.2.0/setup.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-02 01:29:54.070968 froog-0.2.0/tests/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3172 2023-07-28 03:44:46.000000 froog-0.2.0/tests/test_conv_speed.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     4256 2023-07-28 03:41:52.000000 froog-0.2.0/tests/test_mnist.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1043 2023-07-28 04:44:12.000000 froog-0.2.0/tests/test_nn.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     4717 2023-07-30 19:28:07.000000 froog-0.2.0/tests/test_ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1987 2023-07-27 02:40:39.000000 froog-0.2.0/tests/test_optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2618 2023-07-30 06:46:05.000000 froog-0.2.0/tests/test_tensor.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-04 18:25:53.991429 froog-0.2.1/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.2.1/LICENSE
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3149 2023-08-04 18:25:53.991315 froog-0.2.1/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2829 2023-08-04 16:09:24.000000 froog-0.2.1/README.md
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-04 18:25:53.988827 froog-0.2.1/froog/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       57 2023-07-26 06:32:22.000000 froog-0.2.1/froog/__init__.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2415 2023-08-04 17:46:53.000000 froog-0.2.1/froog/gradcheck.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1880 2023-08-04 17:50:10.000000 froog-0.2.1/froog/nn.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)    14379 2023-08-04 17:42:33.000000 froog-0.2.1/froog/ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     8723 2023-08-04 18:00:54.000000 froog-0.2.1/froog/ops_gpu.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2450 2023-08-04 17:45:44.000000 froog-0.2.1/froog/optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     7713 2023-08-04 17:40:03.000000 froog-0.2.1/froog/tensor.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3142 2023-08-04 17:41:11.000000 froog-0.2.1/froog/utils.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-04 18:25:53.989512 froog-0.2.1/froog.egg-info/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3149 2023-08-04 18:25:53.000000 froog-0.2.1/froog.egg-info/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      396 2023-08-04 18:25:53.000000 froog-0.2.1/froog.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-08-04 18:25:53.000000 froog-0.2.1/froog.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-08-04 18:25:53.000000 froog-0.2.1/froog.egg-info/requires.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        6 2023-08-04 18:25:53.000000 froog-0.2.1/froog.egg-info/top_level.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-08-04 18:25:53.991465 froog-0.2.1/setup.cfg
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      846 2023-08-04 17:48:51.000000 froog-0.2.1/setup.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-04 18:25:53.990941 froog-0.2.1/tests/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3172 2023-07-28 03:44:46.000000 froog-0.2.1/tests/test_conv_speed.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1043 2023-07-28 04:44:12.000000 froog-0.2.1/tests/test_nn.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     4791 2023-08-04 17:47:26.000000 froog-0.2.1/tests/test_ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1987 2023-07-27 02:40:39.000000 froog-0.2.1/tests/test_optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2618 2023-07-30 06:46:05.000000 froog-0.2.1/tests/test_tensor.py
```

### Comparing `froog-0.2.0/PKG-INFO` & `froog-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.2.0
-Summary: a beautifully compact machine-learning library
+Version: 0.2.1
+Summary: A SUPER SIMPLE MACHINE LEARNING FRAMEWORK
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # froog <img src="https://github.com/kevbuh/froog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
   <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="200">
   <br/>
@@ -28,14 +28,16 @@
 <!-- machine learning is like making a lego. you combine standardized pieces, of all shapes and sizes, to create anything you imagine -->
 <!-- froog is making those essential building blocks. -->
 <!-- grug say never be not improving tooling  -->
 <!-- ml toolkit -->
 
 FROOG is a neural network framework that is actually **SIMPLE** with the goal of running machine learning on any device --> easily and efficiently.
 
+<!-- This project should be art. Code is art. Machine learning should be easy to use, why do you need PHD's to able to create anything awesome with it?   -->
+
 # Installation
 ```bash
 pip install froog
 ```
 
 ### Overview of Features
 - Tensors
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: froog Version: 0.2.0 Summary: a beautifully compact
-machine-learning library Author: Kevin Buhler License: MIT Classifier:
+Metadata-Version: 2.1 Name: froog Version: 0.2.1 Summary: A SUPER SIMPLE
+MACHINE LEARNING FRAMEWORK Author: Kevin Buhler License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
+License Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE # froog [unit test badge]
                                [froog the frog]
                FROOG: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
                         homepage | documentation | pip
 
       FROOG is a neural network framework that is actually **SIMPLE** with the
-goal of running machine learning on any device --> easily and efficiently. #
+goal of running machine learning on any device --> easily and efficiently.  #
 Installation ```bash pip install froog ``` ### Overview of Features - Tensors -
 Automatic Differentiation - Forward and backward passes - Input/gradient shape-
 tracking - MNIST example - 2D Convolutions (im2col) - Numerical gradient
 checking - The most common optimizers (SGD, Adam, RMSProp) ### Math Operations
 - Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D
 Convolutions - Avg & Max pooling - More ### Ready-to-Go Models - EfficientNet-
 B0  # Bounties Want to help but don't know where to start? Here are some
```

### Comparing `froog-0.2.0/README.md` & `froog-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 <!-- machine learning is like making a lego. you combine standardized pieces, of all shapes and sizes, to create anything you imagine -->
 <!-- froog is making those essential building blocks. -->
 <!-- grug say never be not improving tooling  -->
 <!-- ml toolkit -->
 
 FROOG is a neural network framework that is actually **SIMPLE** with the goal of running machine learning on any device --> easily and efficiently.
 
+<!-- This project should be art. Code is art. Machine learning should be easy to use, why do you need PHD's to able to create anything awesome with it?   -->
+
 # Installation
 ```bash
 pip install froog
 ```
 
 ### Overview of Features
 - Tensors
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # froog [unit test badge]
                                [froog the frog]
                FROOG: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
                         homepage | documentation | pip
 
       FROOG is a neural network framework that is actually **SIMPLE** with the
-goal of running machine learning on any device --> easily and efficiently. #
+goal of running machine learning on any device --> easily and efficiently.  #
 Installation ```bash pip install froog ``` ### Overview of Features - Tensors -
 Automatic Differentiation - Forward and backward passes - Input/gradient shape-
 tracking - MNIST example - 2D Convolutions (im2col) - Numerical gradient
 checking - The most common optimizers (SGD, Adam, RMSProp) ### Math Operations
 - Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D
 Convolutions - Avg & Max pooling - More ### Ready-to-Go Models - EfficientNet-
 B0  # Bounties Want to help but don't know where to start? Here are some
```

### Comparing `froog-0.2.0/froog/gradcheck.py` & `froog-0.2.1/froog/gradcheck.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #  _______  ______    _______  _______  _______ 
 # |       ||    _ |  |       ||       ||       |
 # |    ___||   | ||  |   _   ||   _   ||    ___|
 # |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
 # |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
 # |   |    |   |  | ||       ||       ||   |_| |
 # |___|    |___|  |_||_______||_______||_______|
-#
 
 import numpy as np
 from froog.tensor import Tensor
 from froog.utils import mask_like
 
 def jacobian(model, input):
   output = model(input)
```

### Comparing `froog-0.2.0/froog/nn.py` & `froog-0.2.1/froog/nn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #  _______  ______    _______  _______  _______ 
 # |       ||    _ |  |       ||       ||       |
 # |    ___||   | ||  |   _   ||   _   ||    ___|
 # |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
 # |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
 # |   |    |   |  | ||       ||       ||   |_| |
 # |___|    |___|  |_||_______||_______||_______|
-#
 
 from froog.tensor import Tensor
 
 def swish(x):
   return x.mul(x.sigmoid())
 
 # *************************************
```

### Comparing `froog-0.2.0/froog/ops.py` & `froog-0.2.1/froog/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     ctx.save_for_backward(input, weight)
     return input.dot(weight)
 
   @staticmethod
   def backward(ctx, grad_output):
     input, weight = ctx.saved_tensors
     grad_input = grad_output.dot(weight.T)
-    grad_weight = grad_output.T.dot(input).T
+    grad_weight = input.T.dot(grad_output)
     return grad_input, grad_weight
 register('dot', Dot)
 register('matmul', Dot)
 
 
 # ***********************************************************
 #    _____ ______  _______  __    ______   ____  ____  _____
@@ -181,15 +181,15 @@
     output = input - logsumexp(input).reshape((-1, 1))
     ctx.save_for_backward(output)
     return output
 
   @staticmethod
   def backward(ctx, grad_output):
     (output,) = ctx.saved_tensors
-    return grad_output - np.exp(output) * grad_output.sum(axis=1).reshape((-1, 1))
+    return grad_output - np.exp(output)*(grad_output.sum(axis=1).reshape((-1, 1)))
 register("logsoftmax", LogSoftmax)
 
 
 # *************************************************
 #    __________  _   ___    __   ____  ____  _____
 #   / ____/ __ \/ | / / |  / /  / __ \/ __ \/ ___/
 #  / /   / / / /  |/ /| | / /  / / / / /_/ /\__ \
```

### Comparing `froog-0.2.0/froog/optim.py` & `froog-0.2.1/froog/optim.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 # |    ___||   | ||  |   _   ||   _   ||    ___|
 # |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
 # |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
 # |   |    |   |  | ||       ||       ||   |_| |
 # |___|    |___|  |_||_______||_______||_______|
 
 import numpy as np
+from froog.tensor import Tensor, GPU
 
 class Optimizer:
-   def __init__(self, params):
-      self.params = params
+  def __init__(self, params):
+    self.params = params
 
 class SGD(Optimizer):
+  """
+  Stochastic Gradient Descent
+  """
   def __init__(self, params, lr=0.001):
     super(SGD, self).__init__(params)
-    self.lr = lr
+    self.lr = Tensor([lr], gpu=params[0].gpu)
 
   def step(self):
     for t in self.params:
-      t.data -= self.lr * t.grad.data
+      t -= t.grad * self.lr
 
 class Adam(Optimizer):  
   """
   Default ADAM opimizer from https://arxiv.org/pdf/1412.6980.pdf algorithm
   """
   def __init__(self, params, lr=0.001, b1=0.9, b2=0.999, eps=10e-8):
     super(Adam, self).__init__(params)
```

### Comparing `froog-0.2.0/froog/tensor.py` & `froog-0.2.1/froog/tensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,19 @@
 cl_ctx, cl_queue = None, None
 def init_gpu():
   """
   creates global OpenCL context and queue
   """
   global cl_ctx, cl_queue
   if cl_queue is None:
-    cl_ctx = cl.create_some_context(answers=[0,2])   # CHANGE IF YOU HAVE MULTIPLE COMPUTE DEVICES
+    try:
+      # if you have an m2 mac 
+      cl_ctx = cl.create_some_context(answers=[0]) 
+    except (cl._cl.RuntimeError, TypeError):
+      cl_ctx = cl.create_some_context(interactive=False)
     cl_queue = cl.CommandQueue(cl_ctx)
 
 # ************ Main Classes ************
 # ********** Tensor, Function **********
 #   _____________   _______ ____  ____ 
 #  /_  __/ ____/ | / / ___// __ \/ __ \
 #   / / / __/ /  |/ /\__ \/ / / / /_/ /
@@ -65,14 +69,17 @@
       self.gpu_()
 
     # internal variables used for autograd graph construction
     self._ctx = None # these are where the backward gradient computation are saved
 
   def __repr__(self):
     return f"Tensor data: {self.data}, gradients: {self.grad.data if self.grad else None}" 
+  
+  def assign(self, x):
+    self.data = x.data
 
   @property
   def shape(self):
     return self.data.shape
   
   @staticmethod
   def zeros(*shape):
@@ -116,33 +123,39 @@
 
   # ****** cpu/gpu ******
     
   def to_cpu(self):
     if self.gpu:
       data = np.empty(self.shape, dtype=np.float32)
       cl.enqueue_copy(cl_queue, data, self.data) # copy data from cpu to gpu (queue, dest, src)
-      return Tensor(data)
+      ret = Tensor(data)
+      if self.grad:
+        ret.grad = self.grad.to_cpu()
+      return ret
     else: 
       return self
     
   def gpu_(self):
     self.data = self.to_gpu().data
     self.gpu = True
   
   def to_gpu(self):
     if not GPU:
-      raise Exception("no gpu support 4 u")
+      raise Exception("no gpu support! install pyopencl")
     if not self.gpu:
       init_gpu()
       assert self.data.dtype == np.float32 # GPU only allows float32
       # hostbuf is the data buffer on host machine with the data to be copied to the OpenCL buffer
       data = cl.Buffer(cl_ctx, cl.mem_flags.READ_ONLY | cl.mem_flags.COPY_HOST_PTR, hostbuf=self.data) # from pyopencl docs
       data.shape = self.shape
       data.dtype = self.data.dtype
-      return Tensor(data)
+      ret = Tensor(data)
+      if self.grad:
+        ret.grad = self.grad.to_gpu()
+      return ret
     else:
       return self 
 
   ops = {}     # stores operations that are done on the CPU
   ops_gpu = {} # stores operations that are done on the GPU
 
   # ****** basic tensor math ops ******
@@ -155,15 +168,14 @@
     root = Tensor(np.zeros(self.shape, dtype=self.data.dtype)+0.5, gpu=self.gpu)
     return self.pow(root)
 
   def div(self, y):
     root = Tensor(np.zeros(self.shape, dtype=self.data.dtype)-1, gpu=self.gpu)
     return self.mul(y.pow(root))
 
-
 #     ________  ___   ______________________  _   __
 #    / ____/ / / / | / / ____/_  __/  _/ __ \/ | / /
 #   / /_  / / / /  |/ / /     / /  / // / / /  |/ / 
 #  / __/ / /_/ / /|  / /___  / / _/ // /_/ / /|  /  
 # /_/    \____/_/ |_/\____/ /_/ /___/\____/_/ |_/     
                     
 class Function:
@@ -209,12 +221,17 @@
   else:
     Tensor.ops[name] = fxn
 
   def dispatch(self, *x, **kwargs):
     op_func = (Tensor.ops_gpu if self.gpu else Tensor.ops)[name]
     op_func.cl_ctx, op_func.cl_queue = cl_ctx, cl_queue
     return op_func.apply(op_func, self, *x, **kwargs)
+  
   setattr(Tensor, name, dispatch)
 
+  if name in ['add', 'sub', 'mul', 'div']:
+    setattr(Tensor, "__%s__" % name, dispatch)
+    setattr(Tensor, "__i%s__" % name, lambda self,x: self.assign(dispatch(self,x)))
+
 import froog.ops # this registers all the operations
 if GPU:
   import froog.ops_gpu
```

### Comparing `froog-0.2.0/froog/utils.py` & `froog-0.2.1/froog/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 # |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
 # |   |    |   |  | ||       ||       ||   |_| |
 # |___|    |___|  |_||_______||_______||_______|
 
 import numpy as np
 from functools import lru_cache
 
-def dense_layer(*tensor_size):
+def Linear(*tensor_size):
   # TODO: why dividing by sqrt?
   ret = np.random.uniform(-1., 1., size=tensor_size)/np.sqrt(np.prod(tensor_size)) # random init weights
   return ret.astype(np.float32)
 
 def fetch(url):
-  print(f"fetching {url}...")
   import requests, os, hashlib, tempfile
   fp = os.path.join(tempfile.gettempdir(), hashlib.md5(url.encode('utf-8')).hexdigest())
   if os.path.isfile(fp):
+    print(f"opening cache from {url}...")
     with open(fp, "rb") as f:
       dat = f.read()
   else:
-    with open(fp, "wb") as f:
+    print(f"fetching {url}")
+    with open(fp+".tmp", "wb") as f:
       dat = requests.get(url).content
       f.write(dat)
+    os.rename(fp+".tmp", fp)
   return dat
 
 def fetch_mnist():
   import gzip
   parse = lambda dat: np.frombuffer(gzip.decompress(dat), dtype=np.uint8).copy()
   X_train = parse(fetch("http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz"))[0x10:].reshape((-1, 28, 28))
   Y_train = parse(fetch("http://yann.lecun.com/exdb/mnist/train-labels-idx1-ubyte.gz"))[8:]
@@ -58,15 +60,15 @@
   for i,x in enumerate(idx):
     for j in range(H*W):
       if r_idx[x,j] == -1:
         r_idx[x,j] = i
         break
   return r_idx
 
-# matlab uses these to speed up convs
+# im2col convolution helpers
 def im2col(x, H, W):
   bs, cin, oy, ox = x.shape[0], x.shape[1], x.shape[2]-(H-1), x.shape[3]-(W-1)
   idx = get_im2col_index(oy, ox, cin, H, W)
   tx = x.reshape(bs, -1)[:, idx]
 
   # all the time is spent here
   tx = tx.ravel() # TODO: whats the purpose of ravel ???
```

### Comparing `froog-0.2.0/froog.egg-info/PKG-INFO` & `froog-0.2.1/froog.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.2.0
-Summary: a beautifully compact machine-learning library
+Version: 0.2.1
+Summary: A SUPER SIMPLE MACHINE LEARNING FRAMEWORK
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # froog <img src="https://github.com/kevbuh/froog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
   <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="200">
   <br/>
@@ -28,14 +28,16 @@
 <!-- machine learning is like making a lego. you combine standardized pieces, of all shapes and sizes, to create anything you imagine -->
 <!-- froog is making those essential building blocks. -->
 <!-- grug say never be not improving tooling  -->
 <!-- ml toolkit -->
 
 FROOG is a neural network framework that is actually **SIMPLE** with the goal of running machine learning on any device --> easily and efficiently.
 
+<!-- This project should be art. Code is art. Machine learning should be easy to use, why do you need PHD's to able to create anything awesome with it?   -->
+
 # Installation
 ```bash
 pip install froog
 ```
 
 ### Overview of Features
 - Tensors
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: froog Version: 0.2.0 Summary: a beautifully compact
-machine-learning library Author: Kevin Buhler License: MIT Classifier:
+Metadata-Version: 2.1 Name: froog Version: 0.2.1 Summary: A SUPER SIMPLE
+MACHINE LEARNING FRAMEWORK Author: Kevin Buhler License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
+License Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE # froog [unit test badge]
                                [froog the frog]
                FROOG: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
                         homepage | documentation | pip
 
       FROOG is a neural network framework that is actually **SIMPLE** with the
-goal of running machine learning on any device --> easily and efficiently. #
+goal of running machine learning on any device --> easily and efficiently.  #
 Installation ```bash pip install froog ``` ### Overview of Features - Tensors -
 Automatic Differentiation - Forward and backward passes - Input/gradient shape-
 tracking - MNIST example - 2D Convolutions (im2col) - Numerical gradient
 checking - The most common optimizers (SGD, Adam, RMSProp) ### Math Operations
 - Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D
 Convolutions - Avg & Max pooling - More ### Ready-to-Go Models - EfficientNet-
 B0  # Bounties Want to help but don't know where to start? Here are some
```

### Comparing `froog-0.2.0/setup.py` & `froog-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from setuptools import setup
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='froog',
-      version='0.2.0',
-      description='a beautifully compact machine-learning library',
+      version='0.2.1',
+      description='A SUPER SIMPLE MACHINE LEARNING FRAMEWORK',
       author='Kevin Buhler',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages = ['froog'],
       classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
       ],
       install_requires=['numpy', 'requests'],
-      python_requires='>=3.6',
+      python_requires='>=3.8',
       include_package_data=True)
```

### Comparing `froog-0.2.0/tests/test_conv_speed.py` & `froog-0.2.1/tests/test_conv_speed.py`

 * *Files identical despite different names*

### Comparing `froog-0.2.0/tests/test_nn.py` & `froog-0.2.1/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `froog-0.2.0/tests/test_ops.py` & `froog-0.2.1/tests/test_ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,42 +36,38 @@
   else:
     torch_fbp, froog_fbp = np.nan, np.nan
 
   print(f"shape: {repr(shape) : >32} torch/froog fwd: {torch_fwd:.2f}/{froog_fwd:.2f} ms ({float(froog_fwd/torch_fwd):.2f}x slower) bp: {torch_fbp - torch_fwd:.2f}/{froog_fbp - froog_fwd:.2f} ms ({float((froog_fbp - froog_fwd)/(torch_fbp - torch_fwd)):.2f}x slower)")
 
 
 class TestOps(unittest.TestCase):
+  gpu = False
   # **************** Add ****************
   def test_add(self):
-    helper_test_op([(45,65), (45,65)], lambda x,y: x+y, Tensor.add)
-  @unittest.skipUnless(GPU, "Requires GPU")
-  def test_gpu_add(self):
-    helper_test_op([(45,65), (45,65)], lambda x,y: x+y, Tensor.add, gpu=True)
+    helper_test_op([(45,65), (45,65)], lambda x,y: x+y, Tensor.add, gpu=self.gpu)
+  def test_sum(self):
+    helper_test_op([(45,3)], lambda x: x.sum(), Tensor.sum, atol=1e-4, gpu=self.gpu)
   # **************** Sub ****************
   def test_sub(self):
-    helper_test_op([(45,65), (45,65)], lambda x,y: x-y, Tensor.sub)
+    helper_test_op([(45,65), (45,65)], lambda x,y: x-y, Tensor.sub, gpu=self.gpu)
   # **************** Mul ****************
   def test_mul(self):
-    helper_test_op([(45,65), (45,65)], lambda x,y: x*y, Tensor.mul)
-  @unittest.skipUnless(GPU, "Requires GPU")
-  def test_gpu_mul(self):
-    helper_test_op([(45,65), (45,65)], lambda x,y: x*y, Tensor.mul, gpu=True)
+    helper_test_op([(45,65), (45,65)], lambda x,y: x*y, Tensor.mul, gpu=self.gpu)
   # **************** Dot ****************
-  @unittest.skipUnless(GPU, "Requires GPU")
-  def test_gpu_dot(self):
-    helper_test_op([(3,4), (4,5)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-5, gpu=True)
+  def test_dot(self):
+    helper_test_op([(45,65), (65,100)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-5, gpu=self.gpu)
   # **************** Div ****************
   def test_div(self):
-    helper_test_op([(45,65), (45,65)], lambda x,y: x/y, Tensor.div, atol=1e-3, grad_atol=1e-3)
+    helper_test_op([(45,65), (45,65)], lambda x,y: x/y, Tensor.div, atol=1e-3, grad_atol=1e-3, gpu=self.gpu)
   # **************** Pow ****************
   def test_pow(self):
-    helper_test_op([(45,65), (45,65)], lambda x,y: x**y, Tensor.pow)
+    helper_test_op([(45,65), (45,65)], lambda x,y: x**y, Tensor.pow, gpu=self.gpu)
   # **************** Sqrt ****************
   def test_sqrt(self):
-    helper_test_op([(45,65)], lambda x: x.sqrt(), Tensor.sqrt)
+    helper_test_op([(45,65)], lambda x: x.sqrt(), Tensor.sqrt, gpu=self.gpu)
   # **************** Conv ****************
   def test_conv2d(self):
     for bs in [1,8]:
       for cin in [1,2,3]:
         for groups in [1,3] if cin == 3 else [1]:
           for H in [2,5]:
             for W in [2,3,5]:
@@ -80,15 +76,15 @@
                 lambda x,w: Tensor.conv2d(x,w,groups=groups).relu(), atol=2e-5, grad_atol=2e-6)
   def test_strided_conv2d(self):
     bs = 4
     cin = 3
     H,W = 3,3
     helper_test_op([(bs,cin,11,28), (4,cin,H,W)],
                     lambda x,w: torch.nn.functional.conv2d(x,w,stride=2).relu(),
-                    lambda x,w: Tensor.conv2d(x,w,stride=2).relu(),
+                    lambda x,w: Tensor.conv2d(x,w,stride=2).relu(), 
                     atol=2e-5, grad_atol=2e-6)
     helper_test_op([(bs,cin,11,28), (4,cin,H,W)],
                     lambda x,w: torch.nn.functional.conv2d(x,w,stride=(2,1)).relu(),
                     lambda x,w: Tensor.conv2d(x,w,stride=(2,1)).relu(),
                     atol=2e-5, grad_atol=2e-6)
 
   # **************** Max Pool ****************
@@ -98,10 +94,17 @@
         lambda x: torch.nn.functional.max_pool2d(x, kernel_size=size),
         lambda x: Tensor.max_pool2d(x, kernel_size=size))
   def test_maxpool2x2(self):
     helper_test_op([(32,2,110,28)], lambda x: torch.nn.functional.max_pool2d(x, (2,2)), Tensor.max_pool2d)
   # **************** Avg Pool ****************
   def test_avgpool2x2(self):
     helper_test_op([(32,2,111,28)], lambda x: torch.nn.functional.avg_pool2d(x, (2,2)), Tensor.avg_pool2d)
+  # **************** Activations ****************
+  def test_relu(self):
+    helper_test_op([(45,65)], lambda x: x.relu(), Tensor.relu, gpu=self.gpu)
+
+if GPU:
+  class TestOpsGPU(TestOps):
+    gpu = True
 
 if __name__ == '__main__':
   unittest.main(verbosity=2)
```

### Comparing `froog-0.2.0/tests/test_optim.py` & `froog-0.2.1/tests/test_optim.py`

 * *Files identical despite different names*

### Comparing `froog-0.2.0/tests/test_tensor.py` & `froog-0.2.1/tests/test_tensor.py`

 * *Files identical despite different names*

