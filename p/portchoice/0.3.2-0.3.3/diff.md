# Comparing `tmp/portchoice-0.3.2.tar.gz` & `tmp/portchoice-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portchoice-0.3.2.tar", max compression
+gzip compressed data, was "portchoice-0.3.3.tar", max compression
```

## Comparing `portchoice-0.3.2.tar` & `portchoice-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2022-10-29 12:06:25.965071 portchoice-0.3.2/portchoice/__init__.py
--rw-r--r--   0        0        0    14724 2023-02-05 19:42:38.209912 portchoice-0.3.2/portchoice/design.py
--rw-r--r--   0        0        0     4735 2023-02-05 19:51:22.664145 portchoice-0.3.2/portchoice/generate.py
--rw-r--r--   0        0        0    44471 2023-02-05 19:53:22.054235 portchoice-0.3.2/portchoice/models.py
--rw-r--r--   0        0        0     6537 2023-02-05 19:46:18.840897 portchoice-0.3.2/portchoice/utils.py
--rw-r--r--   0        0        0      454 2023-06-02 08:49:34.765147 portchoice-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      709 2023-06-02 08:50:29.036122 portchoice-0.3.2/setup.py
--rw-r--r--   0        0        0      535 2023-06-02 08:50:29.036407 portchoice-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-08-04 14:46:35.283731 portchoice-0.3.3/portchoice/__init__.py
+-rw-r--r--   0        0        0    14724 2023-08-04 14:46:35.283911 portchoice-0.3.3/portchoice/design.py
+-rw-r--r--   0        0        0     4735 2023-08-04 14:46:35.284050 portchoice-0.3.3/portchoice/generate.py
+-rw-r--r--   0        0        0    45456 2023-08-05 15:05:05.301162 portchoice-0.3.3/portchoice/models.py
+-rw-r--r--   0        0        0     6537 2023-08-04 14:46:35.284511 portchoice-0.3.3/portchoice/utils.py
+-rw-r--r--   0        0        0      454 2023-08-04 14:58:44.247382 portchoice-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      709 2023-08-05 15:32:50.423727 portchoice-0.3.3/setup.py
+-rw-r--r--   0        0        0      535 2023-08-05 15:32:50.424466 portchoice-0.3.3/PKG-INFO
```

### Comparing `portchoice-0.3.2/portchoice/design.py` & `portchoice-0.3.3/portchoice/design.py`

 * *Files identical despite different names*

### Comparing `portchoice-0.3.2/portchoice/generate.py` & `portchoice-0.3.3/portchoice/generate.py`

 * *Files identical despite different names*

### Comparing `portchoice-0.3.2/portchoice/models.py` & `portchoice-0.3.3/portchoice/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 # Written by Jose Ignacio Hernandez
 # May 2022
 
 # Load required modules
 import numpy as np
 import pandas as pd
 from pyDOE2 import fullfact
-from portchoice.utils import _bfgsmin, numhess
+from portchoice.utils import _bfgsmin #, numhess
+from numdifftools import Hessian
 import time
 
 # Portfolio Logit model
 class PortLogit:
     """Portfolio logit model class.
 
     It contains the routines to prepare the data and estimate a portfolio 
@@ -25,15 +26,17 @@
         A data frame with the alternative-specific variables 
         (e.g., attributes), by default None
     Z : pd.DataFrame, optional
         A data frame with the individual-specific variables, by default None
     C : pd.DataFrame, optional
         A data frame with the costs of each individual alternative for each 
         respondent, by default None
-    B : float, optional
+    B_min : float, optional
+        Minimum expenditure, by default None
+    B_max : float, optional
         Resource constraint, by default None
     B_init : float, optional
         Initial level of consumed resources, 
         by default 0
     interactions : list, optional
         List of alternative-interactions. Each element is a list that marks the 
         alternatives that interact, from 0 to J-1, where J is the number of 
@@ -44,15 +47,15 @@
         set of all possible combinations from a full-factorial design.
     mutually_exclusive : list, optional
         List of mutually-exclusive alternatives. Each element of the list is
         a numpy array of two elements that detail the two mutually-exclusive
         alternatives, by detault None
     """
     # Init function
-    def __init__(self, Y: pd.DataFrame, X: pd.DataFrame = None, Z: pd.DataFrame = None, C: pd.DataFrame = None, B: float = None, B_init: float = 0., interactions: list = None, base_combinations: np.ndarray = None, mutually_exclusive: list = None):
+    def __init__(self, Y: pd.DataFrame, X: pd.DataFrame = None, Z: pd.DataFrame = None, C: pd.DataFrame = None, B_min: float = None, B_max: float = None, B_init: float = 0., interactions: list = None, base_combinations: np.ndarray = None, mutually_exclusive: list = None):
 
         # Array of choices
         self.Y = Y.to_numpy()
         
         # Get scalars N and J
         self.N = self.Y.shape[0]
         self.J = self.Y.shape[1]
@@ -99,35 +102,49 @@
             self.Z = Z.to_numpy()
         else:
             self.M = 0
             self.Z = None
 
         # Define array or budget scalar and feasible combinations (if present)
         self.B_init = B_init
-        if B is not None:
-            if isinstance(B,float):
-                self.B = B
+
+        if B_min is not None:
+            if isinstance(B_min,float):
+                self.B_min = B_min
             else:
-                self.B = B.to_numpy()
+                self.B_min = B_min.to_numpy()
         else:
-            self.B = B
+            self.B_min = B_min
+
+
+        if B_max is not None:
+            if isinstance(B_max,float):
+                self.B_max = B_max
+            else:
+                self.B_max = B_max.to_numpy()
+        else:
+            self.B_max = B_max
 
         # Define arrays of costs and totalcosts (if present)
         if C is not None:
             self.C = C.to_numpy()
             self.Totalcosts = self.C @ self.combinations.T
-            
-            if B is not None:
-                self.Feasible = (self.B_init + self.Totalcosts.T <= self.B).T
-            else:
-                self.Feasible = np.ones(self.Totalcosts.shape)
+
+            self.Feasible = np.ones(self.Totalcosts.shape).astype(bool)
+
+            if B_min is not None:
+                self.Feasible[(self.B_init + self.Totalcosts.T <= self.B_min).T] = False
+
+            if B_max is not None:
+                self.Feasible[(self.B_init + self.Totalcosts.T >= self.B_max).T] = False
+
         else:
             self.C = 0
             self.Totalcosts = 0.
-            self.Feasible = np.ones(self.combinations.shape)  
+            self.Feasible = np.ones((self.N,self.combinations.shape[0])).astype(bool)
 
     # Estimate portfolio logit model
     def estimate(self, startv: np.ndarray, asc: np.ndarray, beta_j: np.ndarray = None, delta_0: float = None, hess: bool = True, tol: float = 1e-6, diffeps: float = (np.finfo(float).eps)**(1/3), verbose: bool = True):
         """Estimate portfolio logit model
 
         It starts the optimisation routine of the portfolio logit model. 
         The user can specify the presence of alternative-specific constants 
@@ -188,43 +205,43 @@
         """
         # Retrieve parameter specifications and store in object
         self.asc = asc
         self.beta_j = beta_j
         self.delta_0 = delta_0
 
         # Set arguments for the estimation routine
-        args = (self.J,self.K,self.M,self.Y,self.C,self.B,self.X,self.Z,self.combinations,self.interactions,self.Totalcosts,self.Feasible,self.asc,self.delta_0,self.beta_j)
+        args = (self.J,self.K,self.M,self.Y,self.C,self.B_min,self.B_max,self.X,self.Z,self.combinations,self.interactions,self.Totalcosts,self.Feasible,self.asc,self.delta_0,self.beta_j)
             
         # Minimise the LL function
         time0 = time.time()
 
         res = _bfgsmin(PortLogit._llf,startv,tol=tol,verbose=verbose,difftype='forward',diffeps=diffeps,args=args)
         
         # Get/compute outputs
         ll = res['fun']
         self.coef = res['x'].flatten()
 
         if verbose:
             print('Computing Hessian')
 
         if hess:
-            hessian = numhess(PortLogit._llf)(self.coef,self.J,self.K,self.M,self.Y,self.C,self.B,self.X,self.Z,self.combinations,self.interactions,self.Totalcosts,self.Feasible,asc,delta_0,beta_j)
+            hessian = Hessian(PortLogit._llf)(self.coef,self.J,self.K,self.M,self.Y,self.C,self.B_min,self.B_max,self.X,self.Z,self.combinations,self.interactions,self.Totalcosts,self.Feasible,asc,delta_0,beta_j)
             se = np.sqrt(np.diag(np.linalg.inv(hessian))).flatten()
         else:
             hessian = res['hessian']
             se = np.sqrt(np.diag(np.linalg.inv(hessian))).flatten()
 
         time1 = time.time()
         diff_time = time1-time0
 
         # Return results
         return ll, self.coef, se, hessian, diff_time
 
     # Optimal portfolio
-    def optimal_portfolio(self,X: pd.Series = None, Z: pd.DataFrame = None, C: pd.Series = None, B: float = None, B_init: float = 0, sims: int = 1000):
+    def optimal_portfolio(self,X: pd.Series = None, Z: pd.DataFrame = None, C: pd.Series = None, B_min: float = None, B_max: float = None, B_init: float = 0, sims: int = 1000):
         """Compute the optimal portfolio
 
         Computes the optimal portfolio based on the estimation results 
         (i.e., obtained from `estimate()`) and user-defined variables. 
         The optimal portfolio is computed by computing the expected 
         utility of all possible combinations of alternatives. The 
         expected utility is computed by simulation using `sims` error 
@@ -234,15 +251,17 @@
         ----------
         X : pd.Series, optional
             Series of alternative-specific variables, by default None
         Z : pd.DataFrame, optional
             Data frame with individual-specific variables, by default None
         C : pd.Series, optional
             Series with individual costs per alternative, by default None
-        B : float, optional
+        B_min : float, optional
+            Minimum expenditure, by default None
+        B_max : float, optional
             Resource constraint, by default None
         B_init : float, optional
             Initial level of consumed resources, 
             by default 0
         sims : int, optional
             Number of Extreme Value random draws, by default 1000
 
@@ -261,35 +280,40 @@
         # Raise error if optimal portfolio is comptued with individual-specific variables
         if Z is not None:
             raise ValueError('Optimal portfolio with individual-specific variables is not implemented yet')
 
         # Define arrays of costs and totalcosts (if present)
         if C is not None:
             Totalcosts = (self.combinations * C.to_numpy()).sum(axis=1)[np.newaxis,:]
-            if B is not None:
-                Feasible = B_init + Totalcosts <= B
-            else:
-                Feasible = np.ones((1,self.combinations.shape[0])).astype(bool)
+
+            Feasible = np.ones(Totalcosts.shape).astype(bool)
+
+            if B_min is not None:
+                Feasible[B_init + Totalcosts <= B_min] = False
+
+            if B_max is not None:
+                Feasible[B_init + Totalcosts >= B_max] = False
+
         else:
             Totalcosts = 0.
-            Feasible = np.ones((1,self.combinations.shape[0]))
+            Feasible = np.ones((1,self.combinations.shape[0])).astype(bool)
 
         # Create random Gumbel draws
         e = np.random.gumbel(size=(sims,self.combinations.shape[0]))
 
         # Get utility of each portfolio
-        Vp = _utility(self.coef,self.J,self.K,self.M,None,C,B,X,Z,self.combinations,self.interactions,Totalcosts,Feasible,self.asc,self.delta_0,self.beta_j,return_chosen=False)
+        Vp = _utility(self.coef,self.J,self.K,self.M,None,C,B_min,B_max,X,Z,self.combinations,self.interactions,Totalcosts,Feasible,self.asc,self.delta_0,self.beta_j,return_chosen=False)
 
         # Compute utility for each simulation and average
         Up_s = Vp + e
         Up = Up_s.mean(axis=0)
 
         # Set utility of unfeasible combinations as -inf
-        if B is not None:
-            Up[~Feasible.flatten()] = -np.inf
+        # if B is not None:
+        #     Up[~Feasible.flatten()] = -np.inf
 
         # Sort portfolios and costs by expected utility
         sort_index = np.argsort(Up)[::-1]
         combinations_sorted = self.combinations[sort_index,:]
         EU_sorted = Up[sort_index]
 
         # If costs are present, add to the frame and drop unfeasible combinations
@@ -309,23 +333,23 @@
             portfolio = pd.concat([portfolio,pd.Series(Totalcosts_sorted,name='Totalcosts')],axis=1)
 
         # Return pandas dataframe
         return portfolio
 
     # Finite-difference Hessian
     def hessian(self, eps: float = (np.finfo(float).eps)**(1/3)):
-        hess = numhess(PortLogit._llf,eps=eps)(self.coef,self.J,self.K,self.Y,self.C,self.B,self.X,self.Z,self.combinations,self.interactions,self.Totalcosts,self.Feasible,self.asc,self.delta_0,self.beta_j)
+        hess = Hessian(PortLogit._llf,eps=eps)(self.coef,self.J,self.K,self.Y,self.C,self.B,self.X,self.Z,self.combinations,self.interactions,self.Totalcosts,self.Feasible,self.asc,self.delta_0,self.beta_j)
         return hess
 
     # Portfolio choice model log-likelihood function
     @staticmethod
-    def _llf(pars,J,K,M,Y,C,B,X,Z,combinations,interactions,Totalcosts,Feasible,asc,delta_0,beta_j):
+    def _llf(pars,J,K,M,Y,C,B_min,B_max,X,Z,combinations,interactions,Totalcosts,Feasible,asc,delta_0,beta_j):
                 
         # Get utility functions of chosen alternatives and of portfolios
-        Vp, Vp_chosen = _utility(pars,J,K,M,Y,C,B,X,Z,combinations,interactions,Totalcosts,Feasible,asc,delta_0,beta_j, return_chosen = True)
+        Vp, Vp_chosen = _utility(pars,J,K,M,Y,C,B_min,B_max,X,Z,combinations,interactions,Totalcosts,Feasible,asc,delta_0,beta_j, return_chosen = True)
 
         # Clip to avoid numerical overflow
         Vp[Vp>700] = 700
         Vp_chosen[Vp_chosen>700] = 700
         
         prob_1 = np.exp(Vp_chosen)
         prob_2 = np.sum(np.exp(Vp),axis=1)
@@ -525,15 +549,15 @@
         ll = res['fun']
         self.coef = res['x'].flatten()
 
         if verbose:
             print('Computing Hessian')
 
         if hess:
-            hessian = numhess(LCPortLogit._llf)(self.coef,self.J,self.K,self.M,self.Y,self.C,self.B,self.X,self.Z,self.combinations,self.interactions,self.Totalcosts,self.Feasible,self.asc,self.delta_0,self.beta_j,self.lc)
+            hessian = Hessian(LCPortLogit._llf)(self.coef,self.J,self.K,self.M,self.Y,self.C,self.B,self.X,self.Z,self.combinations,self.interactions,self.Totalcosts,self.Feasible,self.asc,self.delta_0,self.beta_j,self.lc)
             se = np.sqrt(np.diag(np.linalg.inv(hessian))).flatten()
         else:
             hessian = res['hessian']
             se = np.sqrt(np.diag(np.linalg.inv(hessian))).flatten()
 
         time1 = time.time()
         diff_time = time1-time0
@@ -631,15 +655,15 @@
             portfolio = pd.concat([portfolio,pd.Series(Totalcosts_sorted,name='Totalcosts')],axis=1)
 
         # Return pandas dataframe
         return portfolio
 
     # Finite-difference Hessian
     def hessian(self, eps: float = (np.finfo(float).eps)**(1/3)):
-        hess = numhess(LCPortLogit._llf,eps=eps)(self.coef,self.J,self.K,self.Y,self.C,self.B,self.X,self.Z,self.combinations,self.interactions,self.Totalcosts,self.Feasible,self.asc,self.delta_0,self.beta_j,self.lc)
+        hess = Hessian(LCPortLogit._llf,eps=eps)(self.coef,self.J,self.K,self.Y,self.C,self.B,self.X,self.Z,self.combinations,self.interactions,self.Totalcosts,self.Feasible,self.asc,self.delta_0,self.beta_j,self.lc)
         return hess
 
     # Log-likelihood function
     @staticmethod
     def _llf(pars,J,K,Y,C,B,X,Z,combinations,interactions,Totalcosts,Feasible,asc,delta_0,beta_j,lc):
     
 
@@ -841,29 +865,29 @@
         ll = res['fun']
         self.coef = res['x'].flatten()
 
         if verbose:
             print('Computing Hessian')
 
         if hess:
-            hessian = numhess(PortKT._llf,eps=diffeps)(self.coef,self.N,self.J,self.K,self.Y,self.log_Price,self.Remaining,self.N_nonchosen,self.Case1,self.Case2,self.X,self.Z,self.asc,self.beta_j,self.delta_0,self.sigma,self.alpha_0,self.gamma_0)
+            hessian = Hessian(PortKT._llf,eps=diffeps)(self.coef,self.N,self.J,self.K,self.Y,self.log_Price,self.Remaining,self.N_nonchosen,self.Case1,self.Case2,self.X,self.Z,self.asc,self.beta_j,self.delta_0,self.sigma,self.alpha_0,self.gamma_0)
             se = np.sqrt(np.diag(np.linalg.inv(hessian))).flatten()
         else:
             hessian = res['hessian']
             se = np.sqrt(np.diag(np.linalg.inv(hessian))).flatten()
 
         time1 = time.time()
         diff_time = time1-time0
 
         # Return results
         return ll, self.coef, se, hessian, diff_time
 
     # Finite-difference Hessian
     def hessian(self, eps: float = (np.finfo(float).eps)**(1/3)):
-        hess = numhess(PortKT._llf,eps=eps)(self.coef,self.N,self.J,self.K,self.Y,self.log_Price,self.Remaining,self.N_nonchosen,self.Case1,self.Case2,self.X,self.Z,self.asc,self.beta_j,self.delta_0,self.sigma,self.alpha_0,self.gamma_0)
+        hess = Hessian(PortKT._llf,eps=eps)(self.coef,self.N,self.J,self.K,self.Y,self.log_Price,self.Remaining,self.N_nonchosen,self.Case1,self.Case2,self.X,self.Z,self.asc,self.beta_j,self.delta_0,self.sigma,self.alpha_0,self.gamma_0)
         return hess
 
     def optimal_portfolio(self):
         raise TypeError("Optimal portfolio is not implemented yet")
 
     # Log-likelihood function
     @staticmethod
@@ -1012,15 +1036,15 @@
 
                 ll_n[Case2j_long] = np.log(np.sum(term1*term2,axis=1))
 
         # Return ll
         return -sum(ll_n)
 
 # Utility functions method
-def _utility(pars,J,K,M,Y,C,B,X,Z,combinations,interactions,Totalcosts,Feasible,asc,delta_0,beta_j,return_chosen=True):
+def _utility(pars,J,K,M,Y,C,B_min,B_max,X,Z,combinations,interactions,Totalcosts,Feasible,asc,delta_0,beta_j,return_chosen=True):
 
             # Separate parameters of pars
             par_count = 0
 
             # Alternative-specific constants
             delta_j = np.zeros(J)
             for j in range(J):
@@ -1077,22 +1101,28 @@
                 Vp_chosen = np.sum(Vj*Y,axis=1)
 
                 if interactions is not None:
                     for s in range(len(interactions)):
                         syn = ' & '.join(['(Y[:,' + str(ss) + ']==1)' for ss in interactions[s]])
                         Vp_chosen = Vp_chosen + eval(syn)*delta_ij[s]
 
-            if B is not None:
-                Vp += delta_0*(B-Totalcosts.T).T
-                Vp[~Feasible] = -np.inf
-                if return_chosen:
-                    Vp_chosen += delta_0*(B-np.sum(C*Y,axis=1))
-            else:
-                Vp -= delta_0*Totalcosts
-                if return_chosen:
-                    Vp_chosen -= delta_0*np.sum(C*Y,axis=1)
-        
+            # if B_max is not None:
+            #     Vp += delta_0*(B_max-Totalcosts.T).T
+            #     Vp[~Feasible] = -np.inf
+            #     if return_chosen:
+            #         Vp_chosen += delta_0*(B-np.sum(C*Y,axis=1))
+            # else:
+                # Vp -= delta_0*Totalcosts
+                # if return_chosen:
+                #     Vp_chosen -= delta_0*np.sum(C*Y,axis=1)
+
+            Vp += delta_0*Totalcosts
+            Vp[~Feasible] = -np.inf
+
+            if return_chosen:
+                Vp_chosen += delta_0*np.sum(C*Y,axis=1)
+
             # Return utility functions
             if return_chosen:
                 return Vp, Vp_chosen
             else:
                 return Vp
```

### Comparing `portchoice-0.3.2/portchoice/utils.py` & `portchoice-0.3.3/portchoice/utils.py`

 * *Files identical despite different names*

### Comparing `portchoice-0.3.2/setup.py` & `portchoice-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numdifftools>=0.9.40,<0.10.0', 'pandas>=1.4.2,<2.0.0', 'pyDOE2>=1.3.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'portchoice',
-    'version': '0.3.2',
+    'version': '0.3.3',
     'description': 'Modules to design and estimate portfolio choice models',
     'long_description': None,
     'author': 'Jose Ignacio Hernandez',
     'author_email': 'j.i.hernandez@tudelft.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `portchoice-0.3.2/PKG-INFO` & `portchoice-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portchoice
-Version: 0.3.2
+Version: 0.3.3
 Summary: Modules to design and estimate portfolio choice models
 Author: Jose Ignacio Hernandez
 Author-email: j.i.hernandez@tudelft.nl
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

