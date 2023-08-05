# Comparing `tmp/barcodes_uc-0.6.2.tar.gz` & `tmp/barcodes_uc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barcodes_uc-0.6.2.tar", max compression
+gzip compressed data, was "barcodes_uc-0.7.0.tar", max compression
```

## Comparing `barcodes_uc-0.6.2.tar` & `barcodes_uc-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
--rw-r--r--   0        0        0     1154 2023-08-02 07:23:12.167972 barcodes_uc-0.6.2/README.md
--rw-r--r--   0        0        0        0 2023-07-09 21:52:22.989605 barcodes_uc-0.6.2/barcodes_uc/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 21:53:12.077870 barcodes_uc-0.6.2/barcodes_uc/barcodes/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 09:46:15.448895 barcodes_uc-0.6.2/barcodes_uc/barcodes/__main__.py
--rw-r--r--   0        0        0        0 2023-07-09 21:53:18.670296 barcodes_uc-0.6.2/barcodes_uc/qrcodes/__init__.py
--rw-r--r--   0        0        0     1983 2023-08-03 10:12:15.529960 barcodes_uc-0.6.2/barcodes_uc/qrcodes/__main__.py
--rw-r--r--   0        0        0    15074 2023-08-03 10:45:48.988272 barcodes_uc-0.6.2/barcodes_uc/qrcodes/qrgenerator.py
--rw-r--r--   0        0        0    51328 2023-08-03 10:06:59.755532 barcodes_uc-0.6.2/barcodes_uc/qrcodes/qrutils.py
--rw-r--r--   0        0        0     1843 2023-07-14 14:45:54.180606 barcodes_uc-0.6.2/data/GF256.csv
--rw-r--r--   0        0        0      664 2023-07-18 09:25:40.467529 barcodes_uc-0.6.2/data/alignment_locations.csv
--rw-r--r--   0        0        0    10948 2023-07-14 13:23:50.352025 barcodes_uc-0.6.2/data/capabilities.csv
--rw-r--r--   0        0        0     3824 2023-07-14 14:37:48.262264 barcodes_uc-0.6.2/data/error_correction_table.csv
--rw-r--r--   0        0        0      766 2023-07-26 21:12:31.179696 barcodes_uc-0.6.2/data/format_table.csv
--rw-r--r--   0        0        0      780 2023-07-26 08:54:25.882026 barcodes_uc-0.6.2/data/version_table.csv
--rw-r--r--   0        0        0      647 2023-08-03 10:49:18.185011 barcodes_uc-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    10174 2023-07-30 21:54:01.391050 barcodes_uc-0.6.2/requirements.txt
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 barcodes_uc-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     2205 2023-08-03 12:22:12.415990 barcodes_uc-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 21:52:22.989605 barcodes_uc-0.7.0/barcodes_uc/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:53:12.077870 barcodes_uc-0.7.0/barcodes_uc/barcodes/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:46:15.448895 barcodes_uc-0.7.0/barcodes_uc/barcodes/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:53:18.670296 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__init__.py
+-rw-r--r--   0        0        0     3115 2023-08-03 11:22:38.779125 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__main__.py
+-rw-r--r--   0        0        0      189 2023-07-13 15:35:12.454179 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      171 2023-07-14 13:34:11.240069 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4345 2023-08-03 11:22:41.098823 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0        0        0    21823 2023-08-05 07:20:03.074297 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrgenerator.cpython-311.pyc
+-rw-r--r--   0        0        0     8909 2023-08-03 08:10:47.508145 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrgenerator.cpython-39.pyc
+-rw-r--r--   0        0        0    26257 2023-07-14 13:33:49.056641 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrinfo.cpython-311.pyc
+-rw-r--r--   0        0        0    15979 2023-07-25 21:47:17.851848 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrinfo.cpython-39.pyc
+-rw-r--r--   0        0        0    55776 2023-08-05 07:20:03.036280 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrutils.cpython-311.pyc
+-rw-r--r--   0        0        0    20967 2023-08-03 08:54:56.822508 barcodes_uc-0.7.0/barcodes_uc/qrcodes/__pycache__/qrutils.cpython-39.pyc
+-rw-r--r--   0        0        0    15054 2023-08-05 07:19:23.305411 barcodes_uc-0.7.0/barcodes_uc/qrcodes/qrgenerator.py
+-rw-r--r--   0        0        0    51478 2023-08-05 07:19:58.290195 barcodes_uc-0.7.0/barcodes_uc/qrcodes/qrutils.py
+-rw-r--r--   0        0        0     1843 2023-07-14 14:45:54.180606 barcodes_uc-0.7.0/data/GF256.csv
+-rw-r--r--   0        0        0      664 2023-07-18 09:25:40.467529 barcodes_uc-0.7.0/data/alignment_locations.csv
+-rw-r--r--   0        0        0    10948 2023-07-14 13:23:50.352025 barcodes_uc-0.7.0/data/capabilities.csv
+-rw-r--r--   0        0        0     3824 2023-07-14 14:37:48.262264 barcodes_uc-0.7.0/data/error_correction_table.csv
+-rw-r--r--   0        0        0      766 2023-07-26 21:12:31.179696 barcodes_uc-0.7.0/data/format_table.csv
+-rw-r--r--   0        0        0      780 2023-07-26 08:54:25.882026 barcodes_uc-0.7.0/data/version_table.csv
+-rw-r--r--   0        0        0      671 2023-08-05 07:20:50.235659 barcodes_uc-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10489 2023-08-05 06:51:06.168501 barcodes_uc-0.7.0/requirements.txt
+-rw-r--r--   0        0        0     2916 1970-01-01 00:00:00.000000 barcodes_uc-0.7.0/PKG-INFO
```

### Comparing `barcodes_uc-0.6.2/barcodes_uc/qrcodes/__main__.py` & `barcodes_uc-0.7.0/barcodes_uc/qrcodes/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,33 +20,58 @@
 
     # Add the arguments
     parser.add_argument('message', metavar='message', type=str, help='Message to encode')
     parser.add_argument('-e', '--encoding', type=str, help='Encoding of the message', choices=['byte', 'numeric', 'alphanumeric', 'kanji'])
     parser.add_argument('-V', '--qr-version', type=int, help='QR version, 1-40')
     parser.add_argument('-E', '--qr-error-correction', help='QR error correction', choices=['L', 'M', 'Q', 'H'])
     parser.add_argument('--save', help='Save the QR code to a file', type=str)
+    parser.add_argument('--no-show', help='Do not show the QR code', action='store_true')
 
     # Execute the parse_args() method
     args = parser.parse_args()
+
+    if args.qr_version:
+        if args.qr_version < 1 or args.qr_version > 40:
+                print(TerminalColors.FAIL + 'Error: QR version must be between 1 and 40' + TerminalColors.ENDC)
+                exit(1)
     
     if args.encoding:
         encoding = qrutils.QREncoding[args.encoding]
+        print('Encoding: ' + TerminalColors.OKGREEN + f'{encoding.name}' + TerminalColors.ENDC)
     else:
         encoding = qrgenerator.get_encoding(args.message)
         print('Encoding detected: ' + TerminalColors.OKGREEN + f'{encoding.name}' + TerminalColors.ENDC)
 
-    if args.qr_version and args.qr_error_correction:
-        version = qrutils.QRVersion[args.qr_version]
-        error_correction = qrutils.QRErrorCorrectionLevels[args.qr_error_correction]
+    # print(args)
+    if args.qr_version != None:
+        # print(0)
+
+        version = qrutils.QRVersion(args.qr_version)
+        # print(version)
+
+        if args.qr_error_correction:
+            error_correction = qrutils.QRErrorCorrectionLevels[args.qr_error_correction]
+        else:
+            error_correction = qrutils.QRErrorCorrectionLevels.Q
         generator = qrgenerator.QRGenerator(args.message, encoding, version, error_correction)
+    # elif args.qr_version and args.qr_error_correction:
+    #     print(1)
+    #     version = qrutils.QRVersion[args.qr_version]
+    #     error_correction = qrutils.QRErrorCorrectionLevels[args.qr_error_correction]
+    #     generator = qrgenerator.QRGenerator(args.message, encoding, version, error_correction)
     else:
+        # print(2)
         version, error_correction = qrgenerator.get_min_version(args.message, encoding, qrutils.QRErrorCorrectionLevels.Q)
         generator = qrgenerator.QRGenerator(args.message, encoding, version, error_correction)
 
+    print(f'QR version: ' + TerminalColors.OKGREEN + f'{version.value}' + TerminalColors.ENDC)
+    print(f'QR error correction: ' + TerminalColors.OKGREEN + f'{error_correction}' + TerminalColors.ENDC)
+
     qr = generator.generate()
-    qr.show()
+    if not args.no_show:
+        qr.show()
 
     if args.save:
         qr.save(f'{args.save}.png')
 
 if __name__ == '__main__':
     main()
```

### Comparing `barcodes_uc-0.6.2/barcodes_uc/qrcodes/qrgenerator.py` & `barcodes_uc-0.7.0/barcodes_uc/qrcodes/qrgenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,19 +73,15 @@
         self.reserved_positions = [[0 for i in range(self.size)] for j in range(self.size)]
 
     # def set_size(self, size: int):
     #     self.size = size
     #     self.matrix = [[0 for i in range(size)] for j in range(size)]
 
     def __str__(self): #TODO: Make this look better
-        buildString = ""
-        for row in self.matrix:
-            for col in row:
-                buildString += str(col)
-            buildString += "\n"
+        buildString = f'QR(version={self.version}, encoding={self.encoding}, error_correction={self.error_correction})\n'
 
         return buildString
     
     def show(self):
         #Add quiet zone
         for _ in range(4):
             for _ in range(self.size + 8):
@@ -366,15 +362,15 @@
 
 #Function to get the correct encoding for the message
 def get_encoding(msg: str):
     #Check if message is numeric
     if msg.isnumeric():
         return qrutils.QREncoding.numeric
     #Check if message is alphanumeric
-    elif msg.isalnum():
+    elif qrutils.is_alphanumeric(msg):
         return qrutils.QREncoding.alphanumeric
     #Check if message is kanji
     elif qrutils.is_byte(msg):
         return qrutils.QREncoding.byte
     elif qrutils.is_kanji(msg):
         return qrutils.QREncoding.kanji
```

### Comparing `barcodes_uc-0.6.2/barcodes_uc/qrcodes/qrutils.py` & `barcodes_uc-0.7.0/barcodes_uc/qrcodes/qrutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1546,8 +1546,15 @@
         return False
     
 def is_byte(data: str) -> bool:
     try:
         data.encode('ISO-8859-1')
         return True
     except:
-        return False
+        return False
+    
+def is_alphanumeric(data: str) -> bool:
+    for char in data:
+        if char not in AlphanumericVals:
+            return False
+
+    return True
```

### Comparing `barcodes_uc-0.6.2/data/GF256.csv` & `barcodes_uc-0.7.0/data/GF256.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.2/data/alignment_locations.csv` & `barcodes_uc-0.7.0/data/alignment_locations.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.2/data/capabilities.csv` & `barcodes_uc-0.7.0/data/capabilities.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.2/data/error_correction_table.csv` & `barcodes_uc-0.7.0/data/error_correction_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.2/data/format_table.csv` & `barcodes_uc-0.7.0/data/format_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.2/data/version_table.csv` & `barcodes_uc-0.7.0/data/version_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.2/pyproject.toml` & `barcodes_uc-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "barcodes-uc"
-version = "0.6.2"
+version = "0.7.0"
 description = "A library to generate barcodes"
 authors = ["Pedro Juan Royo <pedro.juan.royo@gmail.com>"]
 readme = "README.md"
 packages = [{include = "barcodes_uc"}]
 include = ["data/*","requirements.txt"]
+exclude = ["fastapi/*"]
 repository = "https://github.com/Parzival1918/barcodes-uc"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.25.1"
 pandas = "^2.0.3"
 pillow = "^10.0.0"
```

### Comparing `barcodes_uc-0.6.2/requirements.txt` & `barcodes_uc-0.7.0/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-numpy==1.25.1 ; python_version >= "3.11" and python_version < "4.0" \
-    --hash=sha256:012097b5b0d00a11070e8f2e261128c44157a8689f7dedcf35576e525893f4fe \
-    --hash=sha256:0d3fe3dd0506a28493d82dc3cf254be8cd0d26f4008a417385cbf1ae95b54004 \
-    --hash=sha256:0def91f8af6ec4bb94c370e38c575855bf1d0be8a8fbfba42ef9c073faf2cf19 \
-    --hash=sha256:1a180429394f81c7933634ae49b37b472d343cccb5bb0c4a575ac8bbc433722f \
-    --hash=sha256:1d5d3c68e443c90b38fdf8ef40e60e2538a27548b39b12b73132456847f4b631 \
-    --hash=sha256:20e1266411120a4f16fad8efa8e0454d21d00b8c7cee5b5ccad7565d95eb42dd \
-    --hash=sha256:247d3ffdd7775bdf191f848be8d49100495114c82c2bd134e8d5d075fb386a1c \
-    --hash=sha256:35a9527c977b924042170a0887de727cd84ff179e478481404c5dc66b4170009 \
-    --hash=sha256:38eb6548bb91c421261b4805dc44def9ca1a6eef6444ce35ad1669c0f1a3fc5d \
-    --hash=sha256:3d7abcdd85aea3e6cdddb59af2350c7ab1ed764397f8eec97a038ad244d2d105 \
-    --hash=sha256:41a56b70e8139884eccb2f733c2f7378af06c82304959e174f8e7370af112e09 \
-    --hash=sha256:4a90725800caeaa160732d6b31f3f843ebd45d6b5f3eec9e8cc287e30f2805bf \
-    --hash=sha256:6b82655dd8efeea69dbf85d00fca40013d7f503212bc5259056244961268b66e \
-    --hash=sha256:6c6c9261d21e617c6dc5eacba35cb68ec36bb72adcff0dee63f8fbc899362588 \
-    --hash=sha256:77d339465dff3eb33c701430bcb9c325b60354698340229e1dff97745e6b3efa \
-    --hash=sha256:791f409064d0a69dd20579345d852c59822c6aa087f23b07b1b4e28ff5880fcb \
-    --hash=sha256:9a3a9f3a61480cc086117b426a8bd86869c213fc4072e606f01c4e4b66eb92bf \
-    --hash=sha256:c1516db588987450b85595586605742879e50dcce923e8973f79529651545b57 \
-    --hash=sha256:c40571fe966393b212689aa17e32ed905924120737194b5d5c1b20b9ed0fb171 \
-    --hash=sha256:d412c1697c3853c6fc3cb9751b4915859c7afe6a277c2bf00acf287d56c4e625 \
-    --hash=sha256:d5154b1a25ec796b1aee12ac1b22f414f94752c5f94832f14d8d6c9ac40bcca6 \
-    --hash=sha256:d736b75c3f2cb96843a5c7f8d8ccc414768d34b0a75f466c05f3a739b406f10b \
-    --hash=sha256:e8f6049c4878cb16960fbbfb22105e49d13d752d4d8371b55110941fb3b17800 \
-    --hash=sha256:f76aebc3358ade9eacf9bc2bb8ae589863a4f911611694103af05346637df1b7 \
-    --hash=sha256:fd67b306320dcadea700a8f79b9e671e607f8696e98ec255915c0c6d6b818503
-pandas==2.0.3 ; python_version >= "3.11" and python_version < "4.0" \
+aenum==3.1.15 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:27b1710b9d084de6e2e695dab78fe9f269de924b51ae2850170ee7e1ca6288a5 \
+    --hash=sha256:8cbd76cd18c4f870ff39b24284d3ea028fbe8731a58df3aa581e434c575b9559 \
+    --hash=sha256:e0dfaeea4c2bd362144b87377e2c61d91958c5ed0b4daf89cb6f45ae23af6288
+numpy==1.25.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0d60fbae8e0019865fc4784745814cff1c421df5afee233db6d88ab4f14655a2 \
+    --hash=sha256:1a1329e26f46230bf77b02cc19e900db9b52f398d6722ca853349a782d4cff55 \
+    --hash=sha256:1b9735c27cea5d995496f46a8b1cd7b408b3f34b6d50459d9ac8fe3a20cc17bf \
+    --hash=sha256:2792d23d62ec51e50ce4d4b7d73de8f67a2fd3ea710dcbc8563a51a03fb07b01 \
+    --hash=sha256:3e0746410e73384e70d286f93abf2520035250aad8c5714240b0492a7302fdca \
+    --hash=sha256:4c3abc71e8b6edba80a01a52e66d83c5d14433cbcd26a40c329ec7ed09f37901 \
+    --hash=sha256:5883c06bb92f2e6c8181df7b39971a5fb436288db58b5a1c3967702d4278691d \
+    --hash=sha256:5c97325a0ba6f9d041feb9390924614b60b99209a71a69c876f71052521d42a4 \
+    --hash=sha256:60e7f0f7f6d0eee8364b9a6304c2845b9c491ac706048c7e8cf47b83123b8dbf \
+    --hash=sha256:76b4115d42a7dfc5d485d358728cdd8719be33cc5ec6ec08632a5d6fca2ed380 \
+    --hash=sha256:7dc869c0c75988e1c693d0e2d5b26034644399dd929bc049db55395b1379e044 \
+    --hash=sha256:834b386f2b8210dca38c71a6e0f4fd6922f7d3fcff935dbe3a570945acb1b545 \
+    --hash=sha256:8b77775f4b7df768967a7c8b3567e309f617dd5e99aeb886fa14dc1a0791141f \
+    --hash=sha256:90319e4f002795ccfc9050110bbbaa16c944b1c37c0baeea43c5fb881693ae1f \
+    --hash=sha256:b79e513d7aac42ae918db3ad1341a015488530d0bb2a6abcbdd10a3a829ccfd3 \
+    --hash=sha256:bb33d5a1cf360304754913a350edda36d5b8c5331a8237268c48f91253c3a364 \
+    --hash=sha256:bec1e7213c7cb00d67093247f8c4db156fd03075f49876957dca4711306d39c9 \
+    --hash=sha256:c5462d19336db4560041517dbb7759c21d181a67cb01b36ca109b2ae37d32418 \
+    --hash=sha256:c5652ea24d33585ea39eb6a6a15dac87a1206a692719ff45d53c5282e66d4a8f \
+    --hash=sha256:d7806500e4f5bdd04095e849265e55de20d8cc4b661b038957354327f6d9b295 \
+    --hash=sha256:db3ccc4e37a6873045580d413fe79b68e47a681af8db2e046f1dacfa11f86eb3 \
+    --hash=sha256:dfe4a913e29b418d096e696ddd422d8a5d13ffba4ea91f9f60440a3b759b0187 \
+    --hash=sha256:eb942bfb6f84df5ce05dbf4b46673ffed0d3da59f13635ea9b926af3deb76926 \
+    --hash=sha256:f08f2e037bba04e707eebf4bc934f1972a315c883a9e0ebfa8a7756eabf9e357 \
+    --hash=sha256:fd608e19c8d7c55021dffd43bfe5492fab8cc105cc8986f813f8c3c048b38760
+pandas==2.0.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:04dbdbaf2e4d46ca8da896e1805bc04eb85caa9a82e259e8eed00254d5e0c682 \
     --hash=sha256:1168574b036cd8b93abc746171c9b4f1b83467438a5e45909fed645cf8692dbc \
     --hash=sha256:1994c789bf12a7c5098277fb43836ce090f1073858c10f9220998ac74f37c69b \
     --hash=sha256:258d3624b3ae734490e4d63c430256e716f488c4fcb7c8e9bde2d3aa46c29089 \
     --hash=sha256:32fca2ee1b0d93dd71d979726b12b61faa06aeb93cf77468776287f41ff8fdc5 \
     --hash=sha256:37673e3bdf1551b95bf5d4ce372b37770f9529743d2498032439371fc7b7eb26 \
     --hash=sha256:3ef285093b4fe5058eefd756100a367f27029913760773c8bf1d2d8bebe5d210 \
@@ -46,15 +50,15 @@
     --hash=sha256:ba619e410a21d8c387a1ea6e8a0e49bb42216474436245718d7f2e88a2f8d7c0 \
     --hash=sha256:c02f372a88e0d17f36d3093a644c73cfc1788e876a7c4bcb4020a77512e2043c \
     --hash=sha256:ce0c6f76a0f1ba361551f3e6dceaff06bde7514a374aa43e33b588ec10420183 \
     --hash=sha256:d9cd88488cceb7635aebb84809d087468eb33551097d600c6dad13602029c2df \
     --hash=sha256:e4c7c9f27a4185304c7caf96dc7d91bc60bc162221152de697c98eb0b2648dd8 \
     --hash=sha256:f167beed68918d62bffb6ec64f2e1d8a7d297a038f86d4aed056b9493fca407f \
     --hash=sha256:f3421a7afb1a43f7e38e82e844e2bca9a6d793d66c1a7f9f0ff39a795bbc5e02
-pillow==10.0.0 ; python_version >= "3.11" and python_version < "4.0" \
+pillow==10.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:00e65f5e822decd501e374b0650146063fbb30a7264b4d2744bdd7b913e0cab5 \
     --hash=sha256:040586f7d37b34547153fa383f7f9aed68b738992380ac911447bb78f2abe530 \
     --hash=sha256:0b6eb5502f45a60a3f411c63187db83a3d3107887ad0d036c13ce836f8a36f1d \
     --hash=sha256:1ce91b6ec08d866b14413d3f0bbdea7e24dfdc8e59f562bb77bc3fe60b6144ca \
     --hash=sha256:1f62406a884ae75fb2f818694469519fb685cc7eaff05d3451a9ebe55c646891 \
     --hash=sha256:22c10cc517668d44b211717fd9775799ccec4124b9a7f7b3635fc5386e584992 \
     --hash=sha256:3400aae60685b06bb96f99a21e1ada7bc7a413d5f49bce739828ecd9391bb8f7 \
@@ -103,19 +107,19 @@
     --hash=sha256:dbc02381779d412145331789b40cc7b11fdf449e5d94f6bc0b080db0a56ea3f0 \
     --hash=sha256:dffe31a7f47b603318c609f378ebcd57f1554a3a6a8effbc59c3c69f804296de \
     --hash=sha256:edf4392b77bdc81f36e92d3a07a5cd072f90253197f4a52a55a8cec48a12483b \
     --hash=sha256:efe8c0681042536e0d06c11f48cebe759707c9e9abf880ee213541c5b46c5bf3 \
     --hash=sha256:f31f9fdbfecb042d046f9d91270a0ba28368a723302786c0009ee9b9f1f60199 \
     --hash=sha256:f88a0b92277de8e3ca715a0d79d68dc82807457dae3ab8699c758f07c20b3c51 \
     --hash=sha256:faaf07ea35355b01a35cb442dd950d8f1bb5b040a7787791a535de13db15ed90
-python-dateutil==2.8.2 ; python_version >= "3.11" and python_version < "4.0" \
+python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
     --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
-pytz==2023.3 ; python_version >= "3.11" and python_version < "4.0" \
+pytz==2023.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588 \
     --hash=sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb
-six==1.16.0 ; python_version >= "3.11" and python_version < "4.0" \
+six==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-tzdata==2023.3 ; python_version >= "3.11" and python_version < "4.0" \
+tzdata==2023.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a \
     --hash=sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda
```

