# Comparing `tmp/TorchSUL-0.2.3.tar.gz` & `tmp/TorchSUL-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchSUL-0.2.3.tar", last modified: Thu Jul 27 12:27:18 2023, max compression
+gzip compressed data, was "TorchSUL-0.2.4.tar", last modified: Sat Aug  5 01:39:10 2023, max compression
```

## Comparing `TorchSUL-0.2.3.tar` & `TorchSUL-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-27 12:27:18.545262 TorchSUL-0.2.3/
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4199 2023-07-27 12:27:18.542263 TorchSUL-0.2.3/PKG-INFO
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4030 2023-07-27 00:49:09.000000 TorchSUL-0.2.3/README.md
-drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-27 12:27:18.411130 TorchSUL-0.2.3/TorchSUL/
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     3925 2023-07-27 12:26:40.000000 TorchSUL-0.2.3/TorchSUL/Base.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      932 2023-07-27 00:43:05.000000 TorchSUL-0.2.3/TorchSUL/Config.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    22926 2023-07-16 13:09:25.000000 TorchSUL-0.2.3/TorchSUL/Layers.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    16258 2023-07-27 12:26:40.000000 TorchSUL-0.2.3/TorchSUL/Model.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    13358 2023-07-16 13:09:25.000000 TorchSUL-0.2.3/TorchSUL/Quant.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      260 2023-07-15 09:40:38.000000 TorchSUL-0.2.3/TorchSUL/__init__.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     1912 2023-07-16 13:09:25.000000 TorchSUL-0.2.3/TorchSUL/sul_tool.py
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     6446 2023-07-16 13:09:25.000000 TorchSUL-0.2.3/TorchSUL/sulplotter.py
-drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-07-27 12:27:18.505263 TorchSUL-0.2.3/TorchSUL.egg-info/
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4199 2023-07-27 12:27:18.000000 TorchSUL-0.2.3/TorchSUL.egg-info/PKG-INFO
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      333 2023-07-27 12:27:18.000000 TorchSUL-0.2.3/TorchSUL.egg-info/SOURCES.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        1 2023-07-27 12:27:18.000000 TorchSUL-0.2.3/TorchSUL.egg-info/dependency_links.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       45 2023-07-27 12:27:18.000000 TorchSUL-0.2.3/TorchSUL.egg-info/requires.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        9 2023-07-27 12:27:18.000000 TorchSUL-0.2.3/TorchSUL.egg-info/top_level.txt
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       38 2023-07-27 12:27:18.546263 TorchSUL-0.2.3/setup.cfg
--rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      669 2023-07-27 12:27:03.000000 TorchSUL-0.2.3/setup.py
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-08-05 01:39:10.853763 TorchSUL-0.2.4/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4415 2023-08-05 01:39:10.851761 TorchSUL-0.2.4/PKG-INFO
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4251 2023-08-05 01:36:32.000000 TorchSUL-0.2.4/README.md
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-08-05 01:39:10.784671 TorchSUL-0.2.4/TorchSUL/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4034 2023-08-05 01:31:12.000000 TorchSUL-0.2.4/TorchSUL/Base.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      994 2023-08-05 01:31:12.000000 TorchSUL-0.2.4/TorchSUL/Config.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    23562 2023-08-05 01:31:12.000000 TorchSUL-0.2.4/TorchSUL/Layers.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    16250 2023-08-05 01:31:12.000000 TorchSUL-0.2.4/TorchSUL/Model.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)    13358 2023-07-16 13:09:25.000000 TorchSUL-0.2.4/TorchSUL/Quant.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      260 2023-07-15 09:40:38.000000 TorchSUL-0.2.4/TorchSUL/__init__.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     1912 2023-07-16 13:09:25.000000 TorchSUL-0.2.4/TorchSUL/sul_tool.py
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     6446 2023-07-16 13:09:25.000000 TorchSUL-0.2.4/TorchSUL/sulplotter.py
+drwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        0 2023-08-05 01:39:10.839761 TorchSUL-0.2.4/TorchSUL.egg-info/
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)     4415 2023-08-05 01:39:10.000000 TorchSUL-0.2.4/TorchSUL.egg-info/PKG-INFO
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      333 2023-08-05 01:39:10.000000 TorchSUL-0.2.4/TorchSUL.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        1 2023-08-05 01:39:10.000000 TorchSUL-0.2.4/TorchSUL.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       45 2023-08-05 01:39:10.000000 TorchSUL-0.2.4/TorchSUL.egg-info/requires.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)        9 2023-08-05 01:39:10.000000 TorchSUL-0.2.4/TorchSUL.egg-info/top_level.txt
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)       38 2023-08-05 01:39:10.853763 TorchSUL-0.2.4/setup.cfg
+-rwxrwxrwx   0 ddwe_cy   (1000) ddwe_cy   (1000)      669 2023-08-05 01:33:51.000000 TorchSUL-0.2.4/setup.py
```

### Comparing `TorchSUL-0.2.3/PKG-INFO` & `TorchSUL-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchSUL
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple but useful layers for Pytorch
 Home-page: https://github.com/ddddwee1/TorchSUL
 Author: Cheng Yu
 Author-email: chengyu996@gmail.com
 Description-Content-Type: text/markdown
 
 # TorchSUL
@@ -29,14 +29,19 @@
 
 ```
 pip install --upgrade torchsul
 ```
 
 ## Patch Notes
 
+#### 2023-08-05 (0.2.4)
+1. Add "loose_load" flag. Working similarly to the "strict=False"
+2. Fix a bug in sul config that would not support multi-processing
+3. Add more initialization options for conv and fc layers
+
 #### 2023-07-27 (0.2.2)
 1. Add support for loading standard pytorch state dict. Users can set "from_torch" flag to load from standard pytorch state dict.
 
 
 #### 2023-07-16:  Bugfixes (0.2.1)
 1. Now *M.Model.\_laod_from_state_dict2* can normally manipulate state dictionary of its child modules 
 2. Add quantization support for fc layers.
```

### Comparing `TorchSUL-0.2.3/README.md` & `TorchSUL-0.2.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 
 ```
 pip install --upgrade torchsul
 ```
 
 ## Patch Notes
 
+#### 2023-08-05 (0.2.4)
+1. Add "loose_load" flag. Working similarly to the "strict=False"
+2. Fix a bug in sul config that would not support multi-processing
+3. Add more initialization options for conv and fc layers
+
 #### 2023-07-27 (0.2.2)
 1. Add support for loading standard pytorch state dict. Users can set "from_torch" flag to load from standard pytorch state dict.
 
 
 #### 2023-07-16:  Bugfixes (0.2.1)
 1. Now *M.Model.\_laod_from_state_dict2* can normally manipulate state dictionary of its child modules 
 2. Add quantization support for fc layers.
```

### Comparing `TorchSUL-0.2.3/TorchSUL/Base.py` & `TorchSUL-0.2.4/TorchSUL/Base.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,13 +122,19 @@
 
 	def save_tensor(self, out, name):
 		if self.get_flag('save_tensor'):
 			os.makedirs('./layer_dumps/', exist_ok=True)
 			torch.save(out, './layer_dumps/%s.pth'%name.replace('/','_'))
 
 	def _load_from_state_dict(self, state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs):
-		self._load_from_state_dict2(state_dict, prefix)
+		try:
+			self._load_from_state_dict2(state_dict, prefix)
+		except Exception as e:
+			if not self.get_flag('loose_load'):
+				raise e 
+			else:
+				pass
 		super()._load_from_state_dict(state_dict, prefix, local_metadata, strict, missing_keys, unexpected_keys, error_msgs)
 		
 	def _load_from_state_dict2(self, state_dict, prefix):
 		# Conveinient method. Omit infrequent arguments
 		pass
```

### Comparing `TorchSUL-0.2.3/TorchSUL/Config.py` & `TorchSUL-0.2.4/TorchSUL/Config.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 		elif isinstance(d, list):
 			res = [ConfigDict.parse_dict(i) for i in d]
 		else:
 			res = d
 		return res 
 
 	def __getattr__(self, key):
-		return self.dict[key]
+		if not key[0]=='_':
+			return self.dict[key]
+		else:
+			super().__getattr__(key)
 
 	def __str__(self):
 		return self.dict_str
 
 
 def load_yaml(f):
 	with open(f) as f:
```

### Comparing `TorchSUL-0.2.3/TorchSUL/Layers.py` & `TorchSUL-0.2.4/TorchSUL/Layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,23 +65,30 @@
 				obs_type = 'minmax'
 			self.input_quantizer = QQuantizers['uniform'](zero_offset=False, bit_type=bit_type, observer=obs_type)
 			self.w_quantizer = QQuantizers['uniform'](zero_offset=True, mode='channel_wise', is_weight=True)
 
 	def reset_params(self):
 		if self.get_flag('conv_init_mode')=='normal':
 			init.normal_(self.weight, std=0.001)
-		else:
+		elif self.get_flag('conv_init_mode')=='resnet':
 			_resnet_normal(self.weight)
+		else:
+			init.kaiming_uniform_(self.weight, a=math.sqrt(5))
 		if self.bias is not None:
 			if self.get_flag('conv_init_mode')=='normal':
 				init.zeros_(self.bias)
-			else:
+			elif self.get_flag('conv_init_mode')=='resnet':
 				fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
 				bound = 1 / math.sqrt(fan_in)
 				init.uniform_(self.bias, -bound, bound)
+			else:
+				fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
+				if fan_in != 0:
+					bound = 1 / math.sqrt(fan_in)
+					init.uniform_(self.bias, -bound, bound)
 
 	def forward(self, x):
 		weight = self.weight
 		if self._quant:
 			x = self.input_quantizer(x)
 			weight = self.w_quantizer(weight)
 		return F.conv2d(x, weight, self.bias, self.stride, self.pad, self.dilation_rate, self.gropus)
@@ -319,17 +326,24 @@
 			if obs_type is None:
 				obs_type = 'minmax'
 			self.input_quantizer = QQuantizers['uniform'](zero_offset=False, bit_type=bit_type, observer=obs_type)
 			self.w_quantizer = QQuantizers['uniform'](zero_offset=True, mode='channel_wise', is_weight=True)
 
 
 	def reset_params(self):
-		init.normal_(self.weight, std=0.001)
-		if self.bias is not None:
-			init.zeros_(self.bias)
+		if self.get_flag('fc_init_mode')=='normal':
+			init.normal_(self.weight, std=0.001)
+			if self.bias is not None:
+				init.zeros_(self.bias)
+		else:
+			init.kaiming_uniform_(self.weight, a=math.sqrt(5))
+			if self.bias is not None:
+				fan_in, _ = init._calculate_fan_in_and_fan_out(self.weight)
+				bound = 1 / math.sqrt(fan_in) if fan_in > 0 else 0
+				init.uniform_(self.bias, -bound, bound)
 
 	def forward(self, x):
 		if self.norm:
 			with torch.no_grad():
 				norm = x.norm(p=2, dim=1, keepdim=True)
 				wnorm = self.weight.norm(p=2,dim=1, keepdim=True)
 			x = x / norm
```

### Comparing `TorchSUL-0.2.3/TorchSUL/Model.py` & `TorchSUL-0.2.4/TorchSUL/Model.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,22 +186,22 @@
 		if self.activation==PARAM_RELU:
 			relu = nn.ReLU()
 			setattr(self, 'act', relu)
 
 	def _load_from_state_dict2(self, state_dict, prefix):
 		def _load_weight(k):
 			if not k in state_dict:
-				raise Exception('Attenpt to find', k, 'but only exist', state_dict.keys(), '\nCannot find weight in checkpoint for layer:', prefix)
+				raise Exception('Attenpt to find', k, 'but only exist', state_dict.keys(), 'Cannot find weight in checkpoint for layer:', prefix)
 			return state_dict.pop(k)
 		def _load_bias(k):
 			if self.conv.usebias:
 				try:
 					b = state_dict.pop(k)
 				except:
-					raise Exception('Attenpt to find', k, 'but only exist', state_dict.keys(), '\nBias is set for layer', prefix, 'but not found in checkpoint. \nTry to set usebias=False to fix this problem')
+					raise Exception('Attenpt to find', k, 'but only exist', state_dict.keys(), 'Bias is set for layer', prefix, 'but not found in checkpoint. Try to set usebias=False to fix this problem')
 			else:
 				b = None
 			return b 
 
 		# get names for params
 		if prefix+'conv.weight' in state_dict:
 			# normal load 
@@ -370,15 +370,15 @@
 	def _load_from_state_dict2(self, state_dict, prefix):
 		if self.get_flag('from_torch'):
 			w = state_dict.pop(prefix + 'weight')
 			if self.fc.usebias:
 				try:
 					b = state_dict.pop(prefix + 'bias')
 				except:
-					raise Exception('Bias is set for layer', prefix, 'but not found in checkpoint. \nTry to set usebias=False to fix this problem')
+					raise Exception('Bias is set for layer', prefix, 'but not found in checkpoint. Try to set usebias=False to fix this problem')
 			else:
 				b = None
 
 			state_dict[prefix+'fc.weight'] = w
 			if b is not None: 
 				state_dict[prefix+'fc.bias'] = b
```

### Comparing `TorchSUL-0.2.3/TorchSUL/Quant.py` & `TorchSUL-0.2.4/TorchSUL/Quant.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.3/TorchSUL/sul_tool.py` & `TorchSUL-0.2.4/TorchSUL/sul_tool.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.3/TorchSUL/sulplotter.py` & `TorchSUL-0.2.4/TorchSUL/sulplotter.py`

 * *Files identical despite different names*

### Comparing `TorchSUL-0.2.3/TorchSUL.egg-info/PKG-INFO` & `TorchSUL-0.2.4/TorchSUL.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchSUL
-Version: 0.2.3
+Version: 0.2.4
 Summary: Simple but useful layers for Pytorch
 Home-page: https://github.com/ddddwee1/TorchSUL
 Author: Cheng Yu
 Author-email: chengyu996@gmail.com
 Description-Content-Type: text/markdown
 
 # TorchSUL
@@ -29,14 +29,19 @@
 
 ```
 pip install --upgrade torchsul
 ```
 
 ## Patch Notes
 
+#### 2023-08-05 (0.2.4)
+1. Add "loose_load" flag. Working similarly to the "strict=False"
+2. Fix a bug in sul config that would not support multi-processing
+3. Add more initialization options for conv and fc layers
+
 #### 2023-07-27 (0.2.2)
 1. Add support for loading standard pytorch state dict. Users can set "from_torch" flag to load from standard pytorch state dict.
 
 
 #### 2023-07-16:  Bugfixes (0.2.1)
 1. Now *M.Model.\_laod_from_state_dict2* can normally manipulate state dictionary of its child modules 
 2. Add quantization support for fc layers.
```

### Comparing `TorchSUL-0.2.3/setup.py` & `TorchSUL-0.2.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup_args = dict(
     name='TorchSUL',
-    version='0.2.3',
+    version='0.2.4',
     description='Simple but useful layers for Pytorch',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Cheng Yu',
     author_email='chengyu996@gmail.com',
     url='https://github.com/ddddwee1/TorchSUL',
```

