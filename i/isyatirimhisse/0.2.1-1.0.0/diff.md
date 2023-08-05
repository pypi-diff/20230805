# Comparing `tmp/isyatirimhisse-0.2.1.tar.gz` & `tmp/isyatirimhisse-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isyatirimhisse-0.2.1.tar", last modified: Mon Jul 31 11:05:59 2023, max compression
+gzip compressed data, was "isyatirimhisse-1.0.0.tar", last modified: Sat Aug  5 11:45:47 2023, max compression
```

## Comparing `isyatirimhisse-0.2.1.tar` & `isyatirimhisse-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 11:05:59.352568 isyatirimhisse-0.2.1/
--rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyatirimhisse-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      147 2023-07-31 11:05:35.000000 isyatirimhisse-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11144 2023-07-31 11:05:59.350572 isyatirimhisse-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    10574 2023-07-31 11:03:13.000000 isyatirimhisse-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 11:05:59.203101 isyatirimhisse-0.2.1/imgs/
--rw-rw-rw-   0        0        0   111188 2023-07-30 13:15:39.000000 isyatirimhisse-0.2.1/imgs/gorsel_ornek_1.png
--rw-rw-rw-   0        0        0    53435 2023-07-30 13:29:30.000000 isyatirimhisse-0.2.1/imgs/gorsel_ornek_2.png
--rw-rw-rw-   0        0        0   433600 2023-07-30 13:17:48.000000 isyatirimhisse-0.2.1/imgs/gorsel_ornek_3.png
-drwxrwxrwx   0        0        0        0 2023-07-31 11:05:59.253960 isyatirimhisse-0.2.1/isyatirimhisse/
--rw-rw-rw-   0        0        0     4721 2023-07-30 12:56:36.000000 isyatirimhisse-0.2.1/isyatirimhisse/VeriCek.py
--rw-rw-rw-   0        0        0     4784 2023-07-30 13:35:14.000000 isyatirimhisse-0.2.1/isyatirimhisse/VeriGorsel.py
--rw-rw-rw-   0        0        0       66 2023-07-28 15:01:43.000000 isyatirimhisse-0.2.1/isyatirimhisse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:05:59.311679 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/
--rw-rw-rw-   0        0        0    11144 2023-07-31 11:05:58.000000 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2023-07-31 11:05:59.000000 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 11:05:58.000000 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-31 11:05:58.000000 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-31 11:05:58.000000 isyatirimhisse-0.2.1/isyatirimhisse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 11:05:59.352568 isyatirimhisse-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      949 2023-07-31 09:19:32.000000 isyatirimhisse-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:05:59.347582 isyatirimhisse-0.2.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-25 09:00:45.000000 isyatirimhisse-0.2.1/tests/__init__.py
--rw-rw-rw-   0        0        0     5009 2023-07-30 12:17:59.000000 isyatirimhisse-0.2.1/tests/test_veri_cek.py
--rw-rw-rw-   0        0        0     2729 2023-07-30 13:36:49.000000 isyatirimhisse-0.2.1/tests/test_veri_gorsel.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:45:47.888740 isyatirimhisse-1.0.0/
+-rw-rw-rw-   0        0        0     1064 2023-07-23 21:22:22.000000 isyatirimhisse-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      146 2023-08-05 11:43:52.000000 isyatirimhisse-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    24953 2023-08-05 11:45:47.884749 isyatirimhisse-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    24383 2023-08-05 11:30:40.000000 isyatirimhisse-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 11:45:47.808951 isyatirimhisse-1.0.0/imgs/
+-rw-rw-rw-   0        0        0   111417 2023-08-04 20:02:55.000000 isyatirimhisse-1.0.0/imgs/gorsel_ornek_1.png
+-rw-rw-rw-   0        0        0    49704 2023-08-04 20:03:29.000000 isyatirimhisse-1.0.0/imgs/gorsel_ornek_2.png
+-rw-rw-rw-   0        0        0    72598 2023-08-04 20:04:11.000000 isyatirimhisse-1.0.0/imgs/gorsel_ornek_3.png
+drwxrwxrwx   0        0        0        0 2023-08-05 11:45:47.821922 isyatirimhisse-1.0.0/isyatirimhisse/
+-rw-rw-rw-   0        0        0     5093 2023-08-04 21:55:39.000000 isyatirimhisse-1.0.0/isyatirimhisse/DataViz.py
+-rw-rw-rw-   0        0        0    14031 2023-08-05 10:29:09.000000 isyatirimhisse-1.0.0/isyatirimhisse/FetchData.py
+-rw-rw-rw-   0        0        0       88 2023-08-02 11:15:32.000000 isyatirimhisse-1.0.0/isyatirimhisse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:45:47.868805 isyatirimhisse-1.0.0/isyatirimhisse.egg-info/
+-rw-rw-rw-   0        0        0    24953 2023-08-05 11:45:47.000000 isyatirimhisse-1.0.0/isyatirimhisse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-08-05 11:45:47.000000 isyatirimhisse-1.0.0/isyatirimhisse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 11:45:47.000000 isyatirimhisse-1.0.0/isyatirimhisse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-08-05 11:45:47.000000 isyatirimhisse-1.0.0/isyatirimhisse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-08-05 11:45:47.000000 isyatirimhisse-1.0.0/isyatirimhisse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 11:45:47.888740 isyatirimhisse-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-08-02 06:41:59.000000 isyatirimhisse-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:45:47.879762 isyatirimhisse-1.0.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-25 09:00:45.000000 isyatirimhisse-1.0.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     3088 2023-08-04 22:25:40.000000 isyatirimhisse-1.0.0/tests/fetch_data_test.py
+-rw-rw-rw-   0        0        0     2649 2023-08-04 18:34:50.000000 isyatirimhisse-1.0.0/tests/fetch_financials_test.py
+-rw-rw-rw-   0        0        0     2746 2023-08-04 21:54:37.000000 isyatirimhisse-1.0.0/tests/visualize_data_test.py
```

### Comparing `isyatirimhisse-0.2.1/LICENSE.txt` & `isyatirimhisse-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isyatirimhisse-0.2.1/isyatirimhisse/VeriGorsel.py` & `isyatirimhisse-1.0.0/isyatirimhisse/DataViz.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,135 +1,148 @@
 import pandas as pd
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
 plt.style.use('fivethirtyeight')
 
-def veri_gorsel(df=None, gorsel_turu='1', normalizasyon=False, **kwargs):
-    """
-    Veri çerçevesindeki hisse senetlerini görselleştirir.
-
-    Parametreler:
-        df (pandas DataFrame, varsayılan None): Hisse senedi verilerinin bulunduğu pandas DataFrame.
-        gorsel_turu (str, varsayılan '1'): Görselleştirme türü.
-            '1': Çizgi Grafiği
-            '2': Korelasyon Isı Matrisi
-            '3': Dağılım Matrisi
-        normalizasyon (bool, varsayılan False): Veriler normalize (0-1 arasında ölçeklendirme) edilecek mi?
-        **kwargs: Görselleştirme türlerine özel ek seçenekler. Örneğin, '1' türü için `linewidth` gibi.
-        Görselleştirme Türleri için **kwargs Parametreleri:
-            '1' (Çizgi Grafiği):
-                linewidth (float, varsayılan 1.5): Çizgi kalınlığı.
-
-            '2' (Korelasyon Isı Matrisi):
-                cmap (str, varsayılan 'coolwarm'): Renk haritası.
-                vmin (float, varsayılan -1): Renk haritasındaki en küçük değer.
-                vmax (float, varsayılan 1): Renk haritasındaki en büyük değer.
-
-            '3' (Dağılım Matrisi):
-                kind (str, varsayılan 'scatter'): Görselleştirme türü ('scatter' veya 'reg').
-                alpha (float, varsayılan 0.5): Nokta şeffaflığı.
-    """
+def visualize_data(df=None, plot_type='1', normalization=False, language='en', **kwargs):
+
+    error_messages = {
+        'tr': {
+            'df_none': 'DataFrame (df) parametresi belirtilmelidir.',
+            'df_pd_dataframe': 'DataFrame (df) parametresi bir pandas DataFrame olmalıdır.',
+            "df_empty": "DataFrame (df) boş olmamalıdır.",
+            "plot_type": "Geçersiz çizim türü. '1', '2' veya '3' olmalıdır.",
+            "normalization": "Normalizasyon parametresi bir boolean (True/False) değeri olmalıdır."
+        },
+        'en': {
+            'df_none': 'The DataFrame (df) parameter must be specified.',
+            'df_pd_dataframe': 'The DataFrame (df) parameter must be a pandas DataFrame.',
+            "df_empty": "The DataFrame (df) must not be empty.",
+            "plot_type": "Invalid plot type. It must be '1', '2', or '3'",
+            "normalization": "The normalization parameter must be a boolean (True/False) value."
+        }
+    }
+
+    plot_titles = {
+        'tr': {
+            'line_plot': 'Seçilen Hisse Senetlerinin Zaman Serileri',
+            'heatmap': 'Seçilen Hisse Senetleri Arasındaki Korelasyonlar',
+            'scatter_matrix': 'Hisse Senetlerinin İlişkileri ve Dağılımları'
+        },
+        'en': {
+            'line_plot': 'Time Series of Selected Stocks',
+            'heatmap': 'Correlations Between Selected Stocks',
+            'scatter_matrix': 'Relationships and Distributions of Selected Stocks'
+        }
+    }
+
+    annotation_text = {
+        'tr': {
+            'normalization_text': 'Veriler normalize edilmiştir.'
+        },
+        'en': {
+            'normalization_text': 'The data are normalized.'
+        }
+    }
 
     if df is None:
-        raise ValueError("Veri çerçevesi (df) parametresi belirtilmelidir.")
+        raise ValueError(error_messages[language]['df_none'])
 
     if not isinstance(df, pd.DataFrame):
-        raise ValueError("Veri çerçevesi (df) parametresi bir pandas DataFrame olmalıdır.")
+        raise ValueError(error_messages[language]['df_pd_dataframe'])
 
     if df.empty:
-        raise ValueError("Veri çerçevesi (df) boş olmamalıdır.")
+        raise ValueError(error_messages[language]['df_empty'])
 
-    if not isinstance(normalizasyon, bool):
-        raise ValueError("Normalizasyon parametresi bir bool (True/False) değeri olmalıdır.")
+    if not isinstance(normalization, bool):
+        raise ValueError(error_messages[language]['normalization'])
 
-    df = df.set_index('Tarih')
+    df = df.set_index('Date')
 
-    if normalizasyon:
+    if normalization:
         df = (df - df.min()) / (df.max() - df.min())
 
     figsize = kwargs.get('figsize', (10, 6))
 
-    if gorsel_turu == '1':
+    if plot_type == '1':
 
         plt.figure(figsize=figsize)
         for column in df.columns:
             sns.lineplot(
                 x=df.index,
                 y=df[column],
                 label=column,
                 linewidth=kwargs.get('linewidth', 1.5)
             )
-        plt.title("Hisse Senetleri, {}/{}/{} - {}/{}/{}".format(
-            df.index.min().strftime('%d'), df.index.min().strftime('%m'), df.index.min().strftime('%Y'),
-            df.index.max().strftime('%d'), df.index.max().strftime('%m'), df.index.max().strftime('%Y')
-        ))
+        plt.title(f"{plot_titles[language]['line_plot']}, {df.index.min().strftime('%d/%m/%Y')} - {df.index.max().strftime('%d/%m/%Y')}", fontsize=kwargs.get('fontsize', 12))
         plt.xlabel('')
         plt.ylabel('')
         plt.legend(fontsize='small')
-        if normalizasyon:
+        if normalization:
             plt.text(
                 0.99,
                 -0.05,
-                'Veriler normalize edilmiştir.',
+                annotation_text[language]['normalization_text'],
                 ha='right',
                 va='bottom',
                 transform=plt.gcf().transFigure,
                 color='gray',
                 fontsize=10,
                 style='italic'
             )
         plt.show()
 
-    elif gorsel_turu=='2':
+    elif plot_type == '2':
 
         plt.figure(figsize=figsize)
         sns.heatmap(
             df.corr(),
             annot=True,
             cmap=kwargs.get('cmap', 'coolwarm'),
             fmt='.2f',
             vmin=kwargs.get('vmin', -1),
             vmax=kwargs.get('vmax', 1),
             mask=np.triu(df.corr())
         )
-        plt.title('Hisse Senetleri Arasındaki Korelasyonlar')
-        if normalizasyon:
+        plt.title(plot_titles[language]['heatmap'], fontsize=kwargs.get('fontsize', 12))
+        if normalization:
             plt.text(
                 0.99,
                 -0.05,
-                'Veriler normalize edilmiştir.',
+                annotation_text[language]['normalization_text'],
                 ha='right',
                 va='bottom',
                 transform=plt.gcf().transFigure,
                 color='gray',
                 fontsize=10,
                 style='italic'
             )
         plt.show()
 
-    elif gorsel_turu=='3':
+    elif plot_type == '3':
 
-        plt.figure(figsize=figsize)
         sns.pairplot(
             df,
             kind='reg',
             corner=True,
-            plot_kws={'scatter_kws': {'alpha': kwargs.get('alpha', .5)}}
+            plot_kws={'scatter_kws': {'alpha': .5}},
+            height=kwargs.get('height', 2.5),
+            aspect=kwargs.get('aspect', 1)
         )
-        plt.suptitle('Hisse Senetlerine Ait Dağılımlar')
-        if normalizasyon:
+        plt.suptitle(plot_titles[language]['scatter_matrix'], fontsize=kwargs.get('fontsize', 12))
+        if normalization:
             plt.text(
                 0.99,
                 -0.05,
-                'Veriler normalize edilmiştir.',
+                annotation_text[language]['normalization_text'],
                 ha='right',
                 va='bottom',
                 transform=plt.gcf().transFigure,
                 color='gray',
                 fontsize=10,
                 style='italic'
             )
         plt.show()
 
     else:
-        raise ValueError("Geçersiz görselleştirme türü. '1', '2' veya '3' olmalıdır.")
+        raise ValueError(error_messages[language]['plot_type'])
```

### Comparing `isyatirimhisse-0.2.1/setup.py` & `isyatirimhisse-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="isyatirimhisse",
-    version="0.2.1",
+    version="1.0.0",
     packages=find_packages(),
     author="Uraz Akgül",
     author_email="urazdev@gmail.com",
     description="İş Yatırım'ın web sitesinden veri çekme işlemlerini kolaylaştıran ve isteğe göre özelleştirilebilen bir kütüphane.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/urazakgul/isyatirimhisse",
     license="MIT",
     install_requires=[
         "requests",
         "pandas",
         "numpy",
         "matplotlib",
         "seaborn",
+        "selenium",
+        "webdriver_manager",
+        "beautifulsoup4",
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires=">=3.8",
```

