# Comparing `tmp/pyrestoolbox-1.4.0.tar.gz` & `tmp/pyrestoolbox-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestoolbox-1.4.0.tar", last modified: Tue Aug  1 08:53:07 2023, max compression
+gzip compressed data, was "pyrestoolbox-1.4.1.tar", last modified: Fri Aug  4 10:25:52 2023, max compression
```

## Comparing `pyrestoolbox-1.4.0.tar` & `pyrestoolbox-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:53:07.344916 pyrestoolbox-1.4.0/
--rw-rw-rw-   0        0        0    33092 2021-12-19 10:23:37.000000 pyrestoolbox-1.4.0/LICENSE
--rw-rw-rw-   0        0        0       37 2022-01-30 04:13:11.000000 pyrestoolbox-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5663 2023-08-01 08:53:07.344916 pyrestoolbox-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    20319 2023-08-01 08:10:22.000000 pyrestoolbox-1.4.0/README.rst
--rw-rw-rw-   0        0        0      121 2022-01-07 02:09:05.000000 pyrestoolbox-1.4.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-01 08:53:07.331912 pyrestoolbox-1.4.0/pyrestoolbox/
--rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.4.0/pyrestoolbox/__init__.py
--rw-rw-rw-   0        0        0    41658 2022-01-30 01:52:14.000000 pyrestoolbox-1.4.0/pyrestoolbox/component_library.xlsx
--rw-rw-rw-   0        0        0   165393 2023-08-01 08:40:42.000000 pyrestoolbox-1.4.0/pyrestoolbox/pyrestoolbox.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:53:07.342914 pyrestoolbox-1.4.0/pyrestoolbox/simtools/
--rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.4.0/pyrestoolbox/simtools/__init__.py
--rw-rw-rw-   0        0        0    37326 2022-04-19 07:29:27.000000 pyrestoolbox-1.4.0/pyrestoolbox/simtools/simtools.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:53:07.339912 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/
--rw-rw-rw-   0        0        0     5663 2023-08-01 08:53:07.000000 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-08-01 08:53:07.000000 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:53:07.000000 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-01 08:53:07.000000 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-01 08:53:07.000000 pyrestoolbox-1.4.0/pyrestoolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-08-01 08:53:07.345923 pyrestoolbox-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1205 2023-08-01 08:06:36.000000 pyrestoolbox-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 10:25:52.369062 pyrestoolbox-1.4.1/
+-rw-rw-rw-   0        0        0    33092 2021-12-19 10:23:37.000000 pyrestoolbox-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0       37 2022-01-30 04:13:11.000000 pyrestoolbox-1.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5783 2023-08-04 10:25:52.370059 pyrestoolbox-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    20436 2023-08-04 10:23:54.000000 pyrestoolbox-1.4.1/README.rst
+-rw-rw-rw-   0        0        0      121 2022-01-07 02:09:05.000000 pyrestoolbox-1.4.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-04 10:25:52.357060 pyrestoolbox-1.4.1/pyrestoolbox/
+-rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.4.1/pyrestoolbox/__init__.py
+-rw-rw-rw-   0        0        0    41658 2022-01-30 01:52:14.000000 pyrestoolbox-1.4.1/pyrestoolbox/component_library.xlsx
+-rw-rw-rw-   0        0        0   169430 2023-08-04 10:10:37.000000 pyrestoolbox-1.4.1/pyrestoolbox/pyrestoolbox.py
+drwxrwxrwx   0        0        0        0 2023-08-04 10:25:52.367061 pyrestoolbox-1.4.1/pyrestoolbox/simtools/
+-rw-rw-rw-   0        0        0        0 2022-01-07 01:15:07.000000 pyrestoolbox-1.4.1/pyrestoolbox/simtools/__init__.py
+-rw-rw-rw-   0        0        0    37326 2022-04-19 07:29:27.000000 pyrestoolbox-1.4.1/pyrestoolbox/simtools/simtools.py
+drwxrwxrwx   0        0        0        0 2023-08-04 10:25:52.365059 pyrestoolbox-1.4.1/pyrestoolbox.egg-info/
+-rw-rw-rw-   0        0        0     5783 2023-08-04 10:25:52.000000 pyrestoolbox-1.4.1/pyrestoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      401 2023-08-04 10:25:52.000000 pyrestoolbox-1.4.1/pyrestoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 10:25:52.000000 pyrestoolbox-1.4.1/pyrestoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-04 10:25:52.000000 pyrestoolbox-1.4.1/pyrestoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-04 10:25:52.000000 pyrestoolbox-1.4.1/pyrestoolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-08-04 10:25:52.371059 pyrestoolbox-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1205 2023-08-04 10:24:14.000000 pyrestoolbox-1.4.1/setup.py
```

### Comparing `pyrestoolbox-1.4.0/LICENSE` & `pyrestoolbox-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.4.0/PKG-INFO` & `pyrestoolbox-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestoolbox
-Version: 1.4.0
+Version: 1.4.1
 Summary: pyResToolbox - A collection of Reservoir Engineering Utilities
 Home-page: https://github.com/mwburgoyne/pyResToolbox
 Author: Mark W. Burgoyne
 Author-email: mark.w.burgoyne@gmail.com
 Keywords: restoolbox,petroleum,reservoir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -41,14 +41,17 @@
 -   Creation of Corey and LET relative permeability tables in Eclipse
     format
 -   Calculation of Methane and CO2 saturated brine properties
 
 Apologies in advance that it is only in oilfield
 units with no current plans to add universal multi-unit support.
 
+Changelist in 1.4.1:
+- Added calculation of Ezrokhi coefficients for brine density and viscosity with dissolved CO2
+
 Changelist in 1.4.0:
 - Introduced CO2 saturated brine calculations using Spycher & Pruess modified SRK EOS method
 - Rectified an error introduced in Gas Z-Factor calculations due to errant indentation
 
 Changelist in 1.3.9:
 - Tweaks to speed DAK and Hall & Yarborough Z-Factor calculations
```

### Comparing `pyrestoolbox-1.4.0/README.rst` & `pyrestoolbox-1.4.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 - Creation of Black Oil Table information
 - Creation of layered permeability distribution consistent with a Lorenze heterogeneity factor
 - Extract problem cells information from Intesect (IX) print files
 - Generation of AQUTAB include file influence functions for use in ECLIPSE
 - Creation of Corey and LET relative permeability tables in Eclipse format
 - Calculation of Methane and CO2 saturated brine properties
 
+Changelist in 1.4.1:
+
+- Added calculation of Ezrokhi coefficients for brine density and viscosity with dissolved CO2
 
 Changelist in 1.4.0:
 
 - Introduced CO2 saturated brine calculations using Spycher & Pruess modified SRK EOS method
 - Rectified an error introduced in Gas Z-Factor calculations due to errant indentation
 
 Changelist in 1.3.9:
```

### Comparing `pyrestoolbox-1.4.0/pyrestoolbox/component_library.xlsx` & `pyrestoolbox-1.4.1/pyrestoolbox/component_library.xlsx`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.4.0/pyrestoolbox/pyrestoolbox.py` & `pyrestoolbox-1.4.1/pyrestoolbox/pyrestoolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -3531,27 +3531,37 @@
                 .rhoGas  : CO2 rich gas density (gm/cm3)
                 .bDen    : Brine density (gm/cm3) [CO2 Saturated, Pure Brine]
                 .bVis    : Brine viscosity (cP)   [CO2 Saturated, Pure Brine]
                 .bVisblty: CO2 Saturated brine viscosibility (1/Bar or 1/psi)
                 .bw      : Brine formation volume factor (rm3/smr / rb/stb) [CO2 Saturated, Pure Brine]
                 .Rs      : CO2 Saturated Brine solution gas ratio (sm3/sm3 or scf/stb)
                 .Cf_usat : Brine undersaturated compressibility (1/Bar or 1/psi)
+            
+            Additional function available to calculate Ezrokhi coefficients for effects of dissolved CO2 on brine density and viscosity
+                .ezrokhi(lower_degC, upper_degC)
+            
+                Calculates and populates the following additional attributes;
+                .EzrokhiDenA : List of A_CO2's for equation Ai(T) = A[0] + A[1] * degC + A[2] * degC**2, for Ezrokhi density adjustment
+                .EzrokhiVisB : List of B_CO2's for equation Bi(T) = B[0] + B[1] * degC + B[2] * degC**2, for Ezrokhi viscosity adjustment
                 
             Usage example for 5000 psia x 275 deg F and 3% NaCl brine:
                 mix = rtb.CO2_Brine_Mixture(pres = 5000, temp = 275, ppm = 30000, metric = False)
                 mix.bw  # Returns [CO2 Saturated Brine Bw, Pure Brine Bw]
                 >> [1.1085535365828796, 1.0543051557116332]
                 
             Usage example for 175 Bara x 85 degC and 0% NaCl brine:
                 mix = rtb.CO2_Brine_Mixture(pres = 175, temp = 85)
                 mix.Rs  # Returns sm3 dissolved CO2 / sm3 Brine
                 >> 24.502168045494223
                 
+                mix.ezrokhi(lower_degC = 70, upper_degC = 140)
+                mix.EzrokhiDenA, mix.EzrokhiVisB
+                >> ([0.05812057460992598, 0.0007985131535236179, -5.863680161690182e-06], [0.7819371846535907, 0, 0])
+                
     """
-    
     def __init__(self, pres, temp, ppm = 0, metric = True):
         self.metric = metric              # Units. FIELD or METRIC
         self.ppm = ppm                    # Parts per million (wt fraction) NaCl in brine
         self.tKel = None                  # Deg K
         self.P0 = None                    # Standard pressure (Bar)
         self.fugPi = [None, None]         # Fugacity * Pressure for species i
         self.K = [None, None]             # yi/xi at reservoir pressure
@@ -3566,46 +3576,80 @@
         self.xSalt = None                 # Mole fraction salt in aqueous mixture
         self.molaL = None                 #--Brine Molality (gmol/kg)
         self.MolarVol = np.array([0.0, 0.0])  #--Molar Volumes from RK-EOS (cm3/gmol)
         self.GASZ = None                  # Vapor phase Z-Factor
         self.MwGas = None                 #--Mole weight  [gm/gmol]
         self.MwBrine = None               #--Mole weight of CO2 free brine (gm/gmol)
         self.rhoGas = None                #--Density of Gas Mixture (gm/cm3)
-        self.Amix = None                  # RK-EOS A_mix parameter
+        self.aMix = None                  # RK-EOS A_mix parameter
         self.aij = None                   # RK-EOS aij
         self.kij = None                   # RK-EOS kij
         self.bMix = None                  # RK-EOS B_mix parameter
         self.b = None                     # RK-EOS bij
         self.vBar = [0, 0]                # Avg partial molar volume of pure condensed phase over the pressure interval P0 to pBar
         self.bDen = None                  # CO2 laden Brine density (gm/cm3) [CO2 Saturated, CO2 Free]
         self.bVis = None                  # Brine viscosity (cP)  [CO2 Saturated, CO2 Free]
         self.bVisblty = None              # CO2 laden viscosibility (1/Bar or 1/psi) (at pressures above Psat)
         self.bw = None                    # Brine formation volume factor (res vol/std vol) [CO2 Saturated, CO2 Free]
         self.Rs = None                    # Solution gwr CO2 (sm3/sm3 or scf/stb brine)
         self.Cf_usat = None               # Undersaturated brine compressibility (1/Bar or 1/psi)
         self.CO2_sat = False              # Flag to determine if in P-T range for saturated liquid CO2 K values
-        
+        self.EzrokhiDenA = None           # Ezrokhi coefficient array for density (to be calculated with ezrokhi() function)
+        self.EzrokhiVisB = None           # Ezrokhi coefficient array for viscosity (to be calculated with ezrokhi() function)
+
         if self.metric:
             self.pBar = pres              # Pressure (Bar)
             self.degC = temp              # Deg C
         else:
             self.pBar = pres/14.5038      # Pressure (psia -> Bar)
             self.degC = (temp - 32)/1.8   # Temperature (degF -> deg C)
         self.tKel = self.degC + CEL2KEL
         
         if self.degC <= 31:
             # Below saturated CO2 pressure equation emprically fit to data at https://www.ohio.edu/mechanical/thermo/property_tables/CO2/CO2_TempSat1.html
-            #if self.pBar >= 10**-15.90106469 * self.tKel**7.157992919: # Above CO2 Psat 
-            if self.pBar >= 26.481*self.degC**0.2827: # Alternate fit to discontinuity peak seen in calculated xCO2 at low temperatures
+            if self.pBar >= 10**-15.90106469 * self.tKel**7.157992919: # Above CO2 Psat 
                 self.CO2_sat = True
 
-
         self.co2BrineSolubility()         # Calculate mutual solubilities
         self.brine()                      # Calculate Brine properties            
-        
+    
+    def ezrokhi(self, lower_degC, upper_degC):
+        # Function to regress on Ezrokhi coefficients for the mixture over the temperature range
+        # Will return arrays Ai and Bi for density and viscosity impact of dissolved CO2 in brine respectively
+        # Uses given sample pressure
+        
+        # Ensure reversed temperatures, or identical values don't fall over
+        if lower_degC <= upper_degC: 
+            lower_degC, upper_degC = min(lower_degC, upper_degC), max(lower_degC, upper_degC)
+            lower_degC -= 10
+            lower_degC = max(10, lower_degC) # Ensure doesn't get below 10 deg C
+            upper_degC += 10
+        
+        wt_co2 = self.x[0] * MWCO2 / (self.x[0] * MWCO2 + self.x[1] * self.MwBrine) # Weight fraction of dissolved CO2
+        temps = np.linspace(lower_degC, upper_degC)
+        As = []
+        Bs = []
+        
+        for temp in temps:
+            results = brine_props(self.pBar, temp, self.ppm, self.x[0], self.MwBrine)
+            bDen, bVis, bVisblty, bw, Rs, Cf_usat = results
+            As.append(np.log10(bDen[0]/bDen[1])/wt_co2)
+            Bs.append(np.log10(bVis[0]/bVis[1])/wt_co2)
+        
+        # Because of the form of the Akand W. Islam and Eric S. Carlson viscosity adjustment, 
+        # the Ezrokhi B coefficient for viscosity will be a constant value for a given xCO2
+        self.EzrokhiVisB = [Bs[0], 0, 0]
+        
+        # Fit density data to quadratic form
+        z = np.polyfit(temps, np.array(As), 2)
+        # Numpy fits coefficients in reverse order to what is expected for Ezrokhi equation as follows
+        # Ai = ao + a1 * T + a2 * T**2
+        z = list(z)[::-1]  # Reverse order of fitted coefficients
+        self.EzrokhiDenA = z 
+    
     def calc_type(self):
         # == Figure out which calculation method to employ ==========================
         # deg C <= 99: Non-iterative solution employed assuming negligible xCO2 for mixing rules
         # deg C > 109: An iterative solution is employed with more robust mixing rules application
         # 99 < deg C < 109: An iterative solution is employed. Partitioning factors and fugacity coefficients are blended between low temp and high temp relationships.
         self.low_temp = True      # Use the simple approach for temp < 99 deg C
         self.scaled = False       # No blending
@@ -3613,41 +3657,38 @@
             self.low_temp = False # Use the iteretaive robust approach
             self.scaled = True    # Also use the simpler < 99 degC approach for equilibrium factors and fugacities and scale the result
         elif self.degC > 109:
             self.low_temp = False # Only perform the more robust > 99 degC approach
             self.scaled = False
 
     # Vapor pressure of water with Buck equation
-    # https://en.wikipedia.org/wiki/Arden_Buck_equation
+    # https://en.wikipedia.org/wiki/Vapour_pressure_of_water#:~:text=The%20saturation%20vapour%20pressure%20of,pressure%20equals%20the%20ambient%20pressure.
     def water_vap_p(self):
         kpa = 0.61121 * np.exp((18.678 - (self.degC/234.5))*(self.degC/(257.14+self.degC)))
-        return 0.145038 * kpa # Convert to psia
-        
-    def FT(self, t, x):                                       # Spycher Equation 6
-        return sum([x[i]*t**i for i in range(len(x))])
+        return 0.145038 * kpa # psia
     
     # Initial estimate for yH2O in saturated Brine / CO2 system
-    # Unpublished empirical fit by Mark Burgoyne (Jul 2023) against data generated with modified Whitson PR-EOS method
+    # Empirical fit by Mark Burgoyne against data generated with modified Whitson PR-EOS method, July 2023
     def est_yH2O(self):
-        # Slope and intercept of ppH20/PPatm - 1 = slope * psia + intercept
+        # Slope and intercept of ppH20/PPatm - 1
         # Slope as function of deg F
-        # Y = (A+B*X)**C+D <--- Bleasdale (Shifted power) + c
+        # N.  98:   Y = (A+B*X)**C+D <--- Bleasdale (Shifted power) + c
         A, B, C, D = 0.1939E+01, 0.8913E-02, -.4844E+01, 0.2551E-03
         degf = self.degC * 1.8 + 32
         p = self.pBar * 14.5038
         slope = (A+B*degf)**C+D
         
         # Intercept as a function of degF
-        # Y = -1/(A+B*X**2)**C <--- Inv pow
+        # N. 107:   Y = -1/(A+B*X**2)**C <--- Inv pow
         A, B, C = 0.3097E+00, 0.9136E-05, 0.1719E+01
         intcpt = -1/(A+B*degf**2)**C
         
-        pp_ratio = slope*p + intcpt + 1.0
+        pp_ratio = slope*p + intcpt + 1
         atm_pvap = self.water_vap_p()
-        pp = pp_ratio * atm_pvap          # Partial pressure of water (yH2O * Pressure)
+        pp = pp_ratio * atm_pvap
         if pp < atm_pvap:
             pp = atm_pvap
         return max(min(pp/p, 1-EPS),0)
         
     def ppm2Molality(self):
     #=======================================================================
     #  Whitson & Brule, SPE Phase Behaviour Monograph, Equation (9.2c)
@@ -3682,19 +3723,27 @@
     #  Spycher, N., and Pruess, K.,
     #  "A Phase-Partitioning Model for CO2-Brine Mixtures ..."
     #  Transp Porous Med (2010), 82, pp. 173-196
     #=======================================================================
     
         cL = [0.0002217, 1.074, 2648.0]
         cZ = [0.000013, -20.12, 5259.0]
-      
+        
         #--(lamB,zetA) from Spycher & Pruess Equation (19) and Table 1---------------
-        lamB = cL[0] * self.tKel + cL[1] / self.tKel + cL[2] / self.tKel ** 2
-        zetA = cZ[0] * self.tKel + cZ[1] / self.tKel + cZ[2] / self.tKel ** 2
-      
+        #lamB = cL[0] * self.tKel + cL[1] / self.tKel + cL[2] / self.tKel ** 2
+        #zetA = cZ[0] * self.tKel + cZ[1] / self.tKel + cZ[2] / self.tKel ** 2
+        
+        T, p = self.tKel, self.pBar
+        # Try method from Duan & Sun
+        c = [0, -0.411370585, 6.08E-02, 97.5347708, -0.023762247, 0.017065624, 1.41E-05]
+        lamB = c[1] + c[2]*T + c[3]/T + c[4]*p/T + c[5]*p / (630-T) + c[6]*T*np.log(p)
+        
+        c = [0, 3.36E-04, -1.98E-02, 0, 2.12E-03, -5.25E-03, 0]
+        zetA = c[1] + c[2]*T + c[3]/T + c[4]*p/T + c[5]*p / (630-T) + c[6]*T*np.log(p)
+        
         #==Hassanzadeh Equation (12)============================================
         self.gamma_prime = (1.0 + self.molaL / CONMOLA) * np.exp(self.molaL * (2.0 * lamB + self.molaL * zetA))
     
     
     def aMix_RK(self):
     #=======================================================================
     #  a-Coefficient of CO2-H2O Mixture for RK-EoS
@@ -3858,15 +3907,17 @@
             t3 /= aMix
             t3 -= b[k] / bMix
             t4 = (aMix / (bMix * RGASCON * self.tKel ** 1.5)) * np.log(vMol / (vMol + bMix))
          
             #==CO2 Fugacity Coefficient=============================================
             logPhi = t1 + t2 + t3 * t4  # Eq. A-8
       
-            #==Pressure * Fugacity Coefficient=============================================
+            #=======================================================================
+            #  Pressure * Fugacity Coefficient
+            #=======================================================================
             self.fugPi[k] = self.pBar * np.exp(logPhi)
     
     def Ktp(self, K0, Vbar):              # Equation 5
         return K0 * np.exp(self.pRT0 * Vbar)
     
     def K_CO2(self): # Units: bar
     #=======================================================================
@@ -3900,19 +3951,22 @@
         
         if self.scaled:
             K0_lt = 10**self.FT(self.degC, [-2.209, 3.097e-2, -1.098e-4, 2.048e-7])
             K0 = self.blended_val(K0_lt, K0)
             
         self.K[1] =  self.Ktp(K0, self.vBar[1])
     
-    def mixMolar(self, x, P1, P2):
+    def mixMolar(self, x1, P1, P2):
     #=======================================================================
     #  Calculate Mixture Property of two Molar Species
     #=======================================================================
-        return x * P1 + (1 - x) * P2
+        return x1 * P1 + (1 - x1) * P2
+    
+    def FT(self, t, x):                        # Equation 6
+        return sum([x[i]*t**i for i in range(len(x))])
     
     def calc_gammas(self):
         if self.low_temp:
             return [1,1]
         Am = -3.084e-2*(self.tKel - 373.15) + 1.927e-5*(self.tKel - 373.15)**2                                 # Eq 15
         self.gamma = [np.exp(2*Am*self.x[0]*(1-self.x[0])**2), np.exp((Am - 2*Am*(1-self.x[0]))*self.x[0]**2)] # Eq 12, 13
         
@@ -3927,37 +3981,47 @@
     #  A Phase-Partitioning Model for CO2–Brine Mixtures at Elevated Temperatures 
     #  and Pressures: Application to CO2-Enhanced Geothermal Systems
     #  Nicolas Spycher & Karsten Pruess, Transp Porous Med (2010) 82:173–196
     #  DOI 10.1007/s11242-009-9425-y
     #============================================================================
     
     def co2BrineSolubility(self):
-        # Calculates CO2 saturated Brine mutual solubilities
-
+        """ Calculates CO2 saturated Brine mutual solubilities
+    
+            Inputs:
+                pBar: Pressure (Bar)
+                degC: Temperature (deg C)
+                ppm: NaCL equivalent concentration in brine
+    
+            Returns tuple of:
+                xCO2: Mole fraction CO2 in brine at pBar
+                yH2O: Mole fraction H2O in CO2 rich gas
+                rhoGas: CO2 rich gas density (gm/cm3)
+        """
         pBar = self.pBar
         degC = self.degC
         ppm = self.ppm
         
         #  Initialisation       
         if pBar <= 1.0:
             pBar = 1+EPS
         
         self.tKel = degC + CEL2KEL
         self.pRT = pBar / (RGASCON * self.tKel)
 
         
         if ppm == None:
-            if self.ppm == None:      # If salt concentration not defined, set to zero
-                self.ppm = 0          # If previously defined, but not redefined here, then leave as it was
+            if self.ppm == None: # If salt concentration not defined, set to zero
+                self.ppm = 0     # If previously defined, but not redefined here, then leave as it was
         else:
-            self.ppm = ppm            # Else if explcitly defined as function parameters, overwrite
+            self.ppm = ppm       # Else if explcitly defined as function parameters, overwrite
         
         if self.degC <= 100:          # Reference pressures delineated by 100 deg C cutoff. 
-            self.P0 = 1.0             # Reference Pressure (1 bar at < 100 degC)
-        else:                         # Ref Pressure (Water saturation pressure Bar at >= 100 degC)
+            self.P0 = 1.0              # Reference Pressure (1 bar at < 100 degC)
+        else:                     # Ref Pressure (Water saturation pressure Bar at >= 100 degC)
             self.P0 = self.FT(self.degC, [-1.9906e-1, 2.0471e-3, 1.0152e-4, -1.4234e-6, 1.4168e-8]) 
     
         self.pRT0 = (self.pBar - self.P0) / (RGASCON * self.tKel)
         self.pRT = self.pBar / (RGASCON * self.tKel)
         
         fppM = PPM2MFR * ppm                                              #--Weight Fraction from PPM
         self.molaL = self.ppm2Molality()                                  #--Molality [gmol/kg]
@@ -3990,14 +4054,16 @@
         self.y = np.array([yCO2, 1.0-yCO2])
         self.x = np.array([xCO2, 1.0-xCO2])
         
         # Trigger mixing rules
         self.aMix_RK()
         self.bMix_RK()
         
+        
+        
         #--Solve the Cubic Equation A-2 --------------------------------------------
         self.MolarVolume()
         
         #--Calculate Fugacity Coefficients*Pressure---------------------------------------
         self.fugP()
         
         if self.scaled: # Recalculate mixing rules and fugacity pressure products with low temp relationships
@@ -4010,14 +4076,18 @@
             self.fugPi[0] = self.blended_val(self.fugPi[0], phiP_ht[0])
             self.fugPi[1] = self.blended_val(self.fugPi[1], phiP_ht[1])
             self.low_temp = False # Reset low temp flag
 
         self.calc_gammas()
         self.A_B()
         
+        #print(self.K)
+        #print(self.gamma_prime, self.gamma, self.A, self.Bprime)      
+        
+        
         # Calculate results. 
         self.y[1] = (1 - self.Bprime) * CONMOLA / ((1/self.A - self.Bprime) * (2.0 * self.molaL + CONMOLA) + 2 * self.molaL * self.Bprime) # Eq B-7
         self.x[0] = self.Bprime * (1.0 - self.y[1])
         self.y[0] = 1.0 - self.y[1]
 
         mCO2 = min(max((1.0 - self.x[0]), EPS),1) * (CONMOLA + 2.0 * self.molaL) / min(max((1.0 - self.x[0]), EPS),1)
         self.xSalt = 2.0 * self.molaL / (2.0 * self.molaL + CONMOLA + mCO2)  # Eq B-3. The 2.0x is stoichiometric ions for NaCl
@@ -4087,24 +4157,24 @@
         self.MolarVolume()                                   #--Molar Volume [cm3/gmol]
         self.MwGas = self.mixMolar(self.y[0], MWCO2, MWWAT)  #--Mole weight  [gm/gmol]
         self.rhoGas = self.MwGas / self.MolarVol[0]          #--Density of Gas Mixture [gm/cm3]
         self.GASZ = self.MolarVol[0] * self.pRT
 
         
     def brine(self):
-        results = co2_brine_props(self.pBar, self.degC, self.ppm, self.x[0], self.MwBrine)
+        results = brine_props(self.pBar, self.degC, self.ppm, self.x[0], self.MwBrine)
         self.bDen, self.bVis, self.bVisblty, self.bw, self.Rs, self.Cf_usat = results
         
         if not self.metric:
             self.bVisblty = self.bVisblty / 14.5038   # CO2 laden viscosibility (1/psi) (at pressures above Psat)
             self.Rs = self.Rs * 35.3147 / 6.28981     # Solution gwr CO2 (scf/stb brine)
             self.Cf_usat = self.Cf_usat / 14.5038     # Undersaturated brine compressibility (1/psi)
 
         
-def co2_brine_props(pBar, degc, ppm, xCO2, MwB):
+def brine_props(pBar, degc, ppm, xCO2, MwB):
     """ Calculates CO2 saturated Brine properties
         1. Pure Brine Density:            Spivey et al. (modified)
         2. Pure Brine viscosity:          Mao-Duan (2009)
         3. CO2 Corrected Brine Density:   Garcia (2001)
         4. CO2 Corrected Brine Viscosity: Islam-Carlson (2012)
         
         pBar: Pressure (Bar)
@@ -4125,15 +4195,15 @@
     MwG = MWCO2
     wt = ppm / 10000 # Wt % (0 - 100)
     m = (1000 * (wt / 100) / (58.4428 * (1 - (wt / 100))))  # Molar concentration of NaCl from wt % in gram mol/kg 
     
     Mpa = pBar * 0.1                    # Pressure in mPa
     tKel = degc + CEL2KEL               # Temperature in deg K
     
-    def Eq41(t, input_array):           # From McCain Petroleum Reservoir Fluid Properties
+    def Eq41(t, input_array):  # From McCain Petroleum Reservoir Fluid Properties
         t2 = t / 100
         return (input_array[1] * t2 ** 2 + input_array[2] * t2 + input_array[3]) / (input_array[4] * t2 ** 2 + input_array[5] * t2 + 1)
 
     # Table 4-6 Coefficients
     rhow_t70_arr = [0, -0.127213, 0.645486, 1.03265, -0.070291, 0.639589]
     Ewt_arr = [0, 4.221, -3.478, 6.221, 0.5182, -0.4405]
     Fwt_arr = [0, -11.403, 29.932, 27.952, 0.20684, 0.3768]
@@ -4153,21 +4223,29 @@
     # Table 4-14 Mao-Duan Coefficients
     d = [0, 2885310, -11072.577, -9.0834095, 0.030925651, -0.0000274071, -1928385.1, 5621.6046, 13.82725, -0.047609523, 0.000035545041]
     
     # Table 4-14 Mao-Duan Coefficients
     a = [-0.21319213, 0.0013651589, -0.0000012191756]
     b = [0.069161945, -0.00027292263, 0.0000002085244]
     c = [-0.0025988855, 0.0000077989227]
-            
-    def calc_props(degc):
-        arrays = [rhow_t70_arr, Ewt_arr, Fwt_arr, Dm2t_arr, Dm32t_arr, Dm1t_arr, Dm12t_arr, Emt_arr, Fm32t_arr, Fm1t_arr, Fm12t_arr]
-        return [Eq41(degc, x) for x in arrays]
     
-    # Calculate properties from steps 1, 2 and  4
-    rhow_t70, Ewt, Fwt, Dm2t, Dm32t, Dm1t, Dm12t, Emt, Fm32t, Fm1t, Fm12t = calc_props(degc)
+    # Density of pure water at the reference pressure of 70 MPa, ?w(T, 70 MPa), in g/cm3,
+    rhow_t70 = Eq41(degc, rhow_t70_arr)                 # Step 1
+    
+    Ewt, Fwt = Eq41(degc, Ewt_arr), Eq41(degc, Fwt_arr) # Step 2
+    
+    Dm2t = Eq41(degc, Dm2t_arr)                         # Step 4
+    Dm32t = Eq41(degc, Dm32t_arr)
+    Dm1t = Eq41(degc, Dm1t_arr)
+    Dm12t = Eq41(degc, Dm12t_arr)
+    
+    Emt = Eq41(degc, Emt_arr)
+    Fm32t = Eq41(degc, Fm32t_arr)
+    Fm1t = Eq41(degc, Fm1t_arr)
+    Fm12t = Eq41(degc, Fm12t_arr)
     
     # -- CO2-Free Brine Density (gm/cm3)
     def brine_denw(Mpa):
         # cw(T, p), in MPa–1, of pure water at temperature T and pressure p,
         cwtp = (1 / 70) * (1 / (Ewt * (Mpa / 70) + Fwt))        # Eq 4.2
 
         #Density of pure water at temperature T and pressure p.
@@ -4178,19 +4256,19 @@
         # Density of brine at temperature T and the reference pressure of 70 MPa
         rhobt70 = (rhow_t70 + Dm2t * m **2 + Dm32t * m ** 1.5 + Dm1t * m + Dm12t * m ** 0.5)  # Eq 4.6
         
         # Brine compressibility coefficients Eb(T,m) and Fb(T,m) from equations (4.7) and (4.8).
         Ebtm = Ewt + Emt * m                                                                  # Eq 4.7
         Fbtm = Fwt + Fm32t * m ** 1.5 + Fm1t * m + Fm12t * m ** 0.5                           # Eq 4.8
         
-        # Return methane-free brine density Rhob(T,p,m), in g/cm3
+        # Return methane-free brine density ?b(T,p,m), in g/cm3
         cbtpm = (1 / 70) * (1 / (Ebtm * (Mpa / 70) + Fbtm))                                   # Eq 4.9 (Step 6)
         Ibt70 = (1 / Ebtm) * np.log(abs(Ebtm + Fbtm))                                         # Eq 4.10 (Step 7)
         Ibtpm = (1 / Ebtm) * np.log(abs(Ebtm * (Mpa / 70) + Fbtm))                            # Eq 4.11
-        return rhobt70 * np.exp(Ibtpm - Ibt70), rhowtp                                        # Eq 4.12
+        return rhobt70 * np.exp(Ibtpm - Ibt70), rhowtp                                                # Eq 4.12
     
     # -- CO2 free brine viscosity Mao-Duan (2009)
     def vis_brine(Mpa, rhowtp):
         
         #-- Viscosity of pure water - Eq 4.41 - 4.42
         lnuw_tp = sum([d[i] * np.power(tKel, (i - 3)) for i in range(1, 6)])
         
@@ -4248,33 +4326,43 @@
     dvdpsi = (cP_CO2_brine_ - cP_CO2_brine)  #-- d[Viscosity/dp [cP/bar]
     viscosblty = dvdpsi * 2 / (cP_CO2_brine + cP_CO2_brine_)  # (1/bar)
     
     # Re-evaluate at reservoir temperature and 1 atmosphere (Rhob_atm)
     Rhob_atm, rhowtp_atm_ = brine_denw(0.101325)
 
     # Re-evaluate at standard conditions
-    # CO2-Free Brine Density at standard conditions (gm/cm3)
     degc = (60 - 32)/1.8 # 60 deg F
-    rhow_t70, Ewt, Fwt, Dm2t, Dm32t, Dm1t, Dm12t, Emt, Fm32t, Fm1t, Fm12t = calc_props(degc)
+    rhow_t70 = Eq41(degc, rhow_t70_arr)
+    Ewt = Eq41(degc, Ewt_arr)
+    Fwt = Eq41(degc, Fwt_arr)
+    Dm2t = Eq41(degc, Dm2t_arr)
+    Dm32t = Eq41(degc, Dm32t_arr)
+    Dm1t = Eq41(degc, Dm1t_arr)
+    Dm12t = Eq41(degc, Dm12t_arr)
+    Emt = Eq41(degc, Emt_arr)
+    Fm32t = Eq41(degc, Fm32t_arr)
+    Fm1t = Eq41(degc, Fm1t_arr)
+    Fm12t = Eq41(degc, Fm12t_arr)
+    
+    # -- CO2-Free Brine Density at standard conditions (gm/cm3)
     sg_SC_Brine, rhowSC = brine_denw(0.101325)
 
-    # Calculate mass, moles and reservoir volume of 1 sm3 of brine without CO2
+    # Calculate mass of 1 sm3 of brine without CO2
     brine_mass = sg_SC_Brine * 1000              # kg brine / sm3 (No CO2)
-    brine_moles = brine_mass / MwB               # Moles of brine per sm3
-    brine_res_vol = brine_mass / (sg_brine*1000) # reservoir volume of brine (res m3 No CO2)
+    brine_moles = brine_mass / MwB               # kg Moles of brine per sm3
     
-    # Calculate moles and mass of CO2 using xCO2 and moles of brine
-    co2_moles = xCO2 / (1 - xCO2) * brine_moles  # Moles of dissolved CO2 per sm3
-    co2_mass = co2_moles * MWCO2                 # kg co2 / sm3 brine
+    # Rearrange: xCO2 = co2_moles / (co2_moles + brine_moles)
+    co2_moles = brine_moles * xCO2 / (1 - xCO2)  # kg Moles of dissolved CO2 per sm3
     
-    # Calculate CO2 volume associated with moles of CO2 in each sm3 of brine
+    co2_mass = co2_moles * MWCO2                 # kg co2 / sm3 brine
     rs = 22.413962 * co2_moles                   # sm3 CO2 per sm3 Brine
+    brine_res_vol = brine_mass / (sg_brine*1000) # reservoir volume of brine (res m3 No CO2)
     
     # Mass balance to work out reservoir volume of dissolved CO2
-    # sg_CO2_Brine = (mass_co2 + mass_brine)/(brine_res_vol + co2_res_vol). Rearranging yields following equation
+    # sg_CO2_Brine = (mass_co2 + mass_brine)/(brine_res_vol + co2_res_vol)
     co2_res_vol = ((co2_mass + brine_mass) - (sg_CO2_Brine * 1000 * brine_res_vol)) / (sg_CO2_Brine * 1000)
-    bw = co2_res_vol + brine_res_vol # rm3 / sm3
+    bw = co2_res_vol + brine_res_vol
     
-    # Undersaturated compressibility = 1/V dV/dP
+    # Understaurated compressibility = 1/V dV/dP
     c_usat = 1 - sg_CO2_Brine / sg_CO2_Brine_ # 1/Bar    
     
-    return ([sg_CO2_Brine, sg_brine], [cP_CO2_brine, cP_brine], viscosblty, [bw, brine_res_vol], rs, c_usat)
+    return ([sg_CO2_Brine, sg_brine], [cP_CO2_brine, cP_brine], viscosblty, [bw, brine_res_vol], rs, c_usat)
```

### Comparing `pyrestoolbox-1.4.0/pyrestoolbox/simtools/simtools.py` & `pyrestoolbox-1.4.1/pyrestoolbox/simtools/simtools.py`

 * *Files identical despite different names*

### Comparing `pyrestoolbox-1.4.0/pyrestoolbox.egg-info/PKG-INFO` & `pyrestoolbox-1.4.1/pyrestoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrestoolbox
-Version: 1.4.0
+Version: 1.4.1
 Summary: pyResToolbox - A collection of Reservoir Engineering Utilities
 Home-page: https://github.com/mwburgoyne/pyResToolbox
 Author: Mark W. Burgoyne
 Author-email: mark.w.burgoyne@gmail.com
 Keywords: restoolbox,petroleum,reservoir
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -41,14 +41,17 @@
 -   Creation of Corey and LET relative permeability tables in Eclipse
     format
 -   Calculation of Methane and CO2 saturated brine properties
 
 Apologies in advance that it is only in oilfield
 units with no current plans to add universal multi-unit support.
 
+Changelist in 1.4.1:
+- Added calculation of Ezrokhi coefficients for brine density and viscosity with dissolved CO2
+
 Changelist in 1.4.0:
 - Introduced CO2 saturated brine calculations using Spycher & Pruess modified SRK EOS method
 - Rectified an error introduced in Gas Z-Factor calculations due to errant indentation
 
 Changelist in 1.3.9:
 - Tweaks to speed DAK and Hall & Yarborough Z-Factor calculations
```

### Comparing `pyrestoolbox-1.4.0/setup.cfg` & `pyrestoolbox-1.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6465 7363  [metadata]..desc
 00000010: 7269 7074 696f 6e5f 6669 6c65 203d 2052  ription_file = R
 00000020: 4541 444d 452e 6d64 0d0a 6e61 6d65 203d  EADME.md..name =
 00000030: 2070 7972 6573 746f 6f6c 626f 780d 0a76   pyrestoolbox..v
-00000040: 6572 7369 6f6e 203d 2031 2e34 2e30 0d0a  ersion = 1.4.0..
+00000040: 6572 7369 6f6e 203d 2031 2e34 2e31 0d0a  ersion = 1.4.1..
 00000050: 6175 7468 6f72 203d 204d 6172 6b20 572e  author = Mark W.
 00000060: 2042 7572 676f 796e 650d 0a61 7574 686f   Burgoyne..autho
 00000070: 725f 656d 6169 6c20 3d20 6d61 726b 2e77  r_email = mark.w
 00000080: 2e62 7572 676f 796e 6540 676d 6169 6c2e  .burgoyne@gmail.
 00000090: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 000000a0: 203d 2070 7952 6573 546f 6f6c 626f 7820   = pyResToolbox 
 000000b0: 2d20 4120 636f 6c6c 6563 7469 6f6e 206f  - A collection o
```

### Comparing `pyrestoolbox-1.4.0/setup.py` & `pyrestoolbox-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 f = open('C:\\Users\\vinom\OneDrive - Santos\\Work in progress\\Python\\0-ResEng\\pyResToolbox\\source_dir\\README.md', 'r').read()
 long_description= f #markdown.markdown( f.read() )
 
 setup(
     name = 'pyrestoolbox',
     packages = find_packages(),
     include_package_data=True,
-    version = '1.4.0',  # Ideally should be same as your GitHub release tag varsion
+    version = '1.4.1',  # Ideally should be same as your GitHub release tag varsion
     description = 'pyResToolbox - A collection of Reservoir Engineering Utilities',
     long_description= long_description,
     long_description_content_type = 'text/markdown',
     author = 'Mark W. Burgoyne',
     author_email = 'mark.w.burgoyne@gmail.com',
     url = 'https://github.com/mwburgoyne/pyResToolbox',
     keywords = ['restoolbox', 'petroleum', 'reservoir'],
```

