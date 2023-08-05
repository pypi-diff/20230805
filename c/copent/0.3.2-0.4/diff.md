# Comparing `tmp/copent-0.3.2.tar.gz` & `tmp/copent-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copent-0.3.2.tar", last modified: Sun Sep 11 06:32:38 2022, max compression
+gzip compressed data, was "copent-0.4.tar", last modified: Fri Aug  4 21:42:34 2023, max compression
```

## Comparing `copent-0.3.2.tar` & `copent-0.4.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-09-11 06:32:38.064126 copent-0.3.2/
--rw-rw-rw-   0        0        0    35149 2022-07-17 07:28:25.000000 copent-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     4487 2022-09-11 06:32:38.064126 copent-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     4061 2022-09-11 01:49:56.000000 copent-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2022-09-11 06:32:38.064126 copent-0.3.2/copent/
--rw-rw-rw-   0        0        0       84 2022-07-17 07:28:25.000000 copent-0.3.2/copent/__init__.py
--rw-rw-rw-   0        0        0     3122 2022-09-11 06:32:18.000000 copent-0.3.2/copent/copent.py
-drwxrwxrwx   0        0        0        0 2022-09-11 06:32:38.064126 copent-0.3.2/copent.egg-info/
--rw-rw-rw-   0        0        0     4487 2022-09-11 06:32:37.000000 copent-0.3.2/copent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2022-09-11 06:32:37.000000 copent-0.3.2/copent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-11 06:32:37.000000 copent-0.3.2/copent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-09-11 06:32:37.000000 copent-0.3.2/copent.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-11 06:32:37.000000 copent-0.3.2/copent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-11 06:32:38.064126 copent-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      555 2022-09-11 05:48:08.000000 copent-0.3.2/setup.py
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2023-08-04 21:42:34.814870 copent-0.4/
+-rw-rw-r--   0 majian    (1000) majian    (1000)     5858 2023-08-04 21:42:34.814870 copent-0.4/PKG-INFO
+-rw-rw-r--   0 majian    (1000) majian    (1000)     4740 2023-08-04 21:41:10.000000 copent-0.4/README.md
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2023-08-04 21:42:34.814870 copent-0.4/copent/
+-rw-rw-r--   0 majian    (1000) majian    (1000)       88 2023-08-04 13:27:32.000000 copent-0.4/copent/__init__.py
+-rw-rw-r--   0 majian    (1000) majian    (1000)     3702 2023-08-04 21:41:18.000000 copent-0.4/copent/copent.py
+drwxrwxr-x   0 majian    (1000) majian    (1000)        0 2023-08-04 21:42:34.814870 copent-0.4/copent.egg-info/
+-rw-rw-r--   0 majian    (1000) majian    (1000)     5858 2023-08-04 21:42:33.000000 copent-0.4/copent.egg-info/PKG-INFO
+-rw-rw-r--   0 majian    (1000) majian    (1000)      203 2023-08-04 21:42:33.000000 copent-0.4/copent.egg-info/SOURCES.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)        1 2023-08-04 21:42:33.000000 copent-0.4/copent.egg-info/dependency_links.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)       12 2023-08-04 21:42:33.000000 copent-0.4/copent.egg-info/requires.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)        7 2023-08-04 21:42:33.000000 copent-0.4/copent.egg-info/top_level.txt
+-rw-rw-r--   0 majian    (1000) majian    (1000)       38 2023-08-04 21:42:34.814870 copent-0.4/setup.cfg
+-rw-rw-r--   0 majian    (1000) majian    (1000)      553 2023-08-04 13:36:09.000000 copent-0.4/setup.py
```

### Comparing `copent-0.3.2/PKG-INFO` & `copent-0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,100 @@
-Metadata-Version: 2.1
-Name: copent
-Version: 0.3.2
-Summary: Estimating Copula Entropy and Transfer Entropy
-Home-page: https://github.com/majianthu/pycopent
-Author: MA Jian
-Author-email: majian03@gmail.com
-License: GPL License
-Platform: UNKNOWN
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![PyPI version](https://badge.fury.io/py/copent.svg)](https://pypi.org/project/copent)
-# copent
-Estimating Copula Entropy and Transfer Entropy
-
-#### Introduction
-The nonparametric methods for estimating copula entropy, transfer entropy, and the statistic for multivariate normality test are implemented. 
-
-The method for estimating copula entropy composes of two simple steps: estimating empirical copula by rank statistic and estimating copula entropy with the KSG method. Copula Entropy is a mathematical concept for multivariate statistical independence measuring and testing, and proved to be equivalent to mutual information. Different from Pearson Correlation Coefficient, Copula Entropy is defined for non-linear, high-order and multivariate cases, which makes it universally applicable. Estimating copula entropy can be applied to many cases, including but not limited to variable selection and causal discovery (by estimating transfer entropy). Please refer to Ma and Sun (2011) <[doi:10.1016/S1007-0214(11)70008-6](http://www.doi.org/10.1016/S1007-0214(11)70008-6)> for more information.
-
-The nonparametric method for estimating transfer entropy composes of two steps: estimating three copula entropy and calculating transfer entropy from the estimated copula entropies. A function for conditional independence testing is also provided. Please refer to Ma (2019) <[arXiv:1910.04375](https://arxiv.org/abs/1910.04375)> for more information.
-
-The copula entropy based statistic for multivariate normality test is implemented. Please refer to Ma (2022) <[arXiv:2206.05956](https://arxiv.org/abs/2206.05956)> for more details.
-
-#### Functions
-* copent -- estimating copula entropy;
-* construct_empirical_copula -- the first step of the copent function, which estimates empirical copula for data by rank statistics;
-* entknn -- the second step of the copent function, which estimates copula entropy from empirical copula with kNN method;
-* ci -- conditional independence testing based on copula entropy 
-* transent -- estimating transfer entropy via copula entropy
-* mvnt -- the copula entropy-based statistic for multivariate normality test
-
-#### Parameters
-* x: N * d data, N samples, d dimensions
-* k: kth nearest neighbour, parameter for kNN entropy estimation. default = 3
-* dtype: distance type, can be 'euclidean' or 'chebychev' (for Maximum Distance)
-* lag: time lag. default = 1
-
-
-#### Installation
-The package can be installed from PyPI directly:
-```
-pip install copent
-```
-The package can be installed from Github:
-```
-pip install git+https://github.com/majianthu/pycopent.git
-```
-#### Usage Examples
-##### estimating copula entropy 
-```python
-from numpy.random import multivariate_normal as mnorm
-import copent
-rho = 0.6
-mean1 = [0,0]
-cov1 = [ [1,rho],[rho,1] ]
-x = mnorm(mean1,cov1,200) # bivariate gaussian 
-ce1 = copent.copent(x) # estimated copula entropy
-```
-
-##### estimating transfer entropy 
-```python
-from copent import transent
-from pandas import read_csv
-import numpy as np
-url = "https://archive.ics.uci.edu/ml/machine-learning-databases/00381/PRSA_data_2010.1.1-2014.12.31.csv"
-prsa2010 = read_csv(url)
-# index: 5(PM2.5),6(Dew Point),7(Temperature),8(Pressure),10(Cumulative Wind Speed)
-data = prsa2010.iloc[2200:2700,[5,8]].values
-te = np.zeros(24)
-for lag in range(1,25):
-	te[lag-1] = transent(data[:,0],data[:,1],lag)
-	str = "TE from pressure to PM2.5 at %d hours lag : %f" %(lag,te[lag-1])
-	print(str)
-```
-
-##### multivariate normality test
-```python
-from numpy.random import multivariate_normal as mnorm
-from copent import mvnt
-mean1 = [0,0]
-cov1 = [[1,0.65],[0.65,1]]
-data = mnorm(mean1, cov1, 500) # bivariate gaussian 
-stat1 = mvnt(data)
-```
-
-#### References
-1. Jian Ma and Zengqi Sun. Mutual information is copula entropy. Tsinghua Science & Technology, 2011, 16(1): 51-54. See also arXiv preprint arXiv:0808.0845, 2008.
-2. Jian Ma. Estimating Transfer Entropy via Copula Entropy. arXiv preprint arXiv:1910.04375, 2019.
-3. Jian Ma. Multivariate Normality Test with Copula Entropy. arXiv preprint arXiv:2206.05956, 2022.
-
-
-
+[![PyPI version](https://badge.fury.io/py/copent.svg)](https://pypi.org/project/copent)
+# copent
+Estimating Copula Entropy and Transfer Entropy
+
+#### Introduction
+The nonparametric methods for estimating copula entropy, transfer entropy, and the statistics for multivariate normality test and two-sample test are implemented. 
+
+The method for estimating copula entropy composes of two simple steps: estimating empirical copula by rank statistic and estimating copula entropy with the KSG method. Copula Entropy is a mathematical concept for multivariate statistical independence measuring and testing, and proved to be equivalent to mutual information. Different from Pearson Correlation Coefficient, Copula Entropy is defined for non-linear, high-order and multivariate cases, which makes it universally applicable. Estimating copula entropy can be applied to many cases, including but not limited to variable selection and causal discovery (by estimating transfer entropy). Please refer to Ma and Sun (2011) <[doi:10.1016/S1007-0214(11)70008-6](http://www.doi.org/10.1016/S1007-0214(11)70008-6)> for more information.
+
+The nonparametric method for estimating transfer entropy composes of two steps: estimating three copula entropy and calculating transfer entropy from the estimated copula entropies. A function for conditional independence testing is also provided. Please refer to Ma (2019) <[arXiv:1910.04375](https://arxiv.org/abs/1910.04375)> for more information.
+
+The copula entropy based statistics for multivariate normality test and two-sample test are implemented. Please refer to Ma (2022) <[arXiv:2206.05956](https://arxiv.org/abs/2206.05956)> and Ma (2023) <[arXiv:2307.07247](https://arxiv.org/abs/2307.07247)> for more details.
+
+#### Functions
+* copent -- estimating copula entropy;
+* construct_empirical_copula -- the first step of the copent function, which estimates empirical copula for data by rank statistics;
+* entknn -- the second step of the copent function, which estimates copula entropy from empirical copula with kNN method;
+* ci -- conditional independence testing based on copula entropy 
+* transent -- estimating transfer entropy via copula entropy
+* mvnt -- estimating the copula entropy-based statistic for multivariate normality test
+* tst -- estimating the copula entropy-based statistic for two-sample test
+
+#### Parameters
+* x: N * d data, N samples, d dimensions
+* k: kth nearest neighbour, parameter for kNN entropy estimation. default = 3
+* dtype: distance type, can be 'euclidean' or 'chebychev' (for Maximum Distance)
+* lag: time lag. default = 1
+* s0,s1: two samples with same dimension
+* n: repeat time of estimation
+
+#### Installation
+The package can be installed from PyPI directly:
+```
+pip install copent
+```
+The package can be installed from Github:
+```
+pip install git+https://github.com/majianthu/pycopent.git
+```
+#### Usage Examples
+##### estimating copula entropy 
+```python
+from numpy.random import multivariate_normal as mnorm
+import copent
+rho = 0.6
+mean1 = [0,0]
+cov1 = [ [1,rho],[rho,1] ]
+x = mnorm(mean1,cov1,200) # bivariate gaussian 
+ce1 = copent.copent(x) # estimated copula entropy
+```
+
+##### estimating transfer entropy 
+```python
+from copent import transent
+from pandas import read_csv
+import numpy as np
+url = "https://archive.ics.uci.edu/ml/machine-learning-databases/00381/PRSA_data_2010.1.1-2014.12.31.csv"
+prsa2010 = read_csv(url)
+# index: 5(PM2.5),6(Dew Point),7(Temperature),8(Pressure),10(Cumulative Wind Speed)
+data = prsa2010.iloc[2200:2700,[5,8]].values
+te = np.zeros(24)
+for lag in range(1,25):
+	te[lag-1] = transent(data[:,0],data[:,1],lag)
+	str = "TE from pressure to PM2.5 at %d hours lag : %f" %(lag,te[lag-1])
+	print(str)
+```
+
+##### multivariate normality test
+```python
+from numpy.random import multivariate_normal as mnorm
+from copent import mvnt
+mean1 = [0,0]
+cov1 = [[1,0.65],[0.65,1]]
+data = mnorm(mean1, cov1, 500)
+stat1 = mvnt(data)
+```
+
+##### two-sample test
+```python
+from copent import tst
+from numpy import zeros
+from numpy.random import multivariate_normal as mnorm
+m0 = [0,0]
+rho1 = 0.5
+v0 = [[1,rho1],[rho1,1]]
+s0 = mnorm(m0, v0, 500) # bivariate gaussian 
+stat1 = zeros(9)
+for i in range(0,9):
+	m1 = [i,i]
+	s1 = mnorm(m1,v0,500)
+	stat1[i] = tst(s0,s1)
+	print(stat1[i])
+```
+
+#### References
+1. Jian Ma and Zengqi Sun. Mutual information is copula entropy. Tsinghua Science & Technology, 2011, 16(1): 51-54. See also arXiv preprint arXiv:0808.0845, 2008.
+2. Jian Ma. Estimating Transfer Entropy via Copula Entropy. arXiv preprint arXiv:1910.04375, 2019.
+3. Jian Ma. Multivariate Normality Test with Copula Entropy. arXiv preprint arXiv:2206.05956, 2022.
+4. Jian Ma. Two-Sample Test with Copula Entropy. arXiv preprint arXiv:2307.07247, 2023.
+
```

### Comparing `copent-0.3.2/copent/copent.py` & `copent-0.4/copent/copent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 ##################################################################################
 ###  Estimating Copula Entropy and Transfer Entropy 
-###  2022-09-11
+###  2023-08-05
 ###  by Ma Jian (Email: majian03@gmail.com)
 ###
 ###  Parameters
 ###	x    	: N * d data, N samples, d dimensions
 ###	k    	: kth nearest neighbour, parameter for kNN entropy estimation. default = 3
 ###	dtype	: distance type ['euclidean', 'chebychev' (i.e Maximum distance)]
 ###	lag	: time lag. default = 1
+###	s0,s1	: two samples with same dimension
+###	n	: repeat time of estimation. default = 12
 ###
 ###  References
 ###  [1] Ma Jian, Sun Zengqi. Mutual information is copula entropy. 
 ###      arXiv:0808.0845, 2008.
 ###  [2] Kraskov A, Stögbauer H, Grassberger P. Estimating mutual information. 
 ###      Physical review E, 2004, 69(6): 066138.
 ###  [3] Ma, Jian. Estimating Transfer Entropy via Copula Entropy. 
 ###      arXiv preprint arXiv:1910.04375, 2019.
 ###  [4] Ma, Jian. Multivariate Normality Test with Copula Entropy.
 ###      arXiv preprint arXiv:2206.05956, 2022.
+###  [5] Ma, Jian. Two-Sample Test with Copula Entropy.
+###      arXiv preprint arXiv:2307.07247, 2023.
 ##################################################################################
 
 from scipy.special import digamma
 from scipy.stats import rankdata as rank 
 from scipy.spatial.distance import cdist
 from math import gamma, log, pi
-from numpy import array, abs, max, vstack, zeros, cov
-from numpy.random import normal as rnorm
+from numpy import array, abs, max, hstack, vstack, ones, zeros, cov
+from numpy.random import uniform, normal as rnorm
 from numpy.linalg import det
 
 ##### constructing empirical copula density [1]
 def construct_empirical_copula(x):
 	(N,d) = x.shape	
 	xc = zeros([N,d]) 
 	for i in range(0,d):
@@ -98,8 +102,21 @@
 	x1 = x[0:(l-lag)]
 	x2 = x[lag:l]
 	y = y[0:(l-lag)]
 	return ci(x2,y,x1,k,dtype)
 
 ##### multivariate normality test [4]
 def mvnt(x, k = 3, dtype = 'chebychev'):
-	return -0.5 * log(det(cov(x.T))) - copent(x,k,dtype)
+	return -0.5 * log(det(cov(x.T))) - copent(x,k,dtype)
+
+##### two-sample test [5]
+def tst(s0,s1,n=12):
+	(N0,d0) = s0.shape
+	(N1,d1) = s1.shape
+	x = vstack((s0,s1))
+	stat1 = 0
+	for i in range(0,n):
+		y1 = vstack((ones([N0,1]),ones([N1,1])*2)) + uniform(0, 0.0000001,[N0+N1,1])
+		y0 = ones([N0+N1,1]) + uniform(0,0.0000001,[N0+N1,1])
+		stat1 = stat1 + copent(hstack((x,y1))) - copent(hstack((x,y0)))
+	return stat1/n
+
```

### Comparing `copent-0.3.2/setup.py` & `copent-0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="copent",
-    version="0.3.2",
+    version="0.4",
     author="MA Jian",
     author_email="majian03@gmail.com",
     description="Estimating Copula Entropy and Transfer Entropy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license = 'GPL License',
     url="https://github.com/majianthu/pycopent",
```

