# Comparing `tmp/vertex2tex-0.3.3.tar.gz` & `tmp/vertex2tex-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertex2tex-0.3.3.tar", last modified: Fri Mar 11 20:54:20 2022, max compression
+gzip compressed data, was "vertex2tex-0.3.4.tar", last modified: Fri Aug  4 21:58:42 2023, max compression
```

## Comparing `vertex2tex-0.3.3.tar` & `vertex2tex-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2022-03-11 20:54:20.598462 vertex2tex-0.3.3/
--rw-r--r--   0 skieffer   (501) staff       (20)     1075 2022-02-13 19:49:11.000000 vertex2tex-0.3.3/LICENSE
--rw-r--r--   0 skieffer   (501) staff       (20)    14839 2022-03-11 20:54:20.598053 vertex2tex-0.3.3/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)    14360 2022-03-11 20:31:22.000000 vertex2tex-0.3.3/README.md
--rw-r--r--   0 skieffer   (501) staff       (20)       38 2022-03-11 20:54:20.598620 vertex2tex-0.3.3/setup.cfg
--rw-r--r--   0 skieffer   (501) staff       (20)      675 2022-03-11 20:45:44.000000 vertex2tex-0.3.3/setup.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2022-03-11 20:54:20.593541 vertex2tex-0.3.3/vertex2tex/
--rw-r--r--   0 skieffer   (501) staff       (20)      191 2022-03-11 19:22:33.000000 vertex2tex-0.3.3/vertex2tex/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)     4954 2022-03-11 19:22:33.000000 vertex2tex-0.3.3/vertex2tex/config.py
--rw-r--r--   0 skieffer   (501) staff       (20)     4673 2022-03-11 19:22:33.000000 vertex2tex-0.3.3/vertex2tex/document.py
--rw-r--r--   0 skieffer   (501) staff       (20)      266 2022-03-11 19:22:33.000000 vertex2tex-0.3.3/vertex2tex/excep.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2022-03-11 20:54:20.597307 vertex2tex-0.3.3/vertex2tex/test/
--rw-r--r--   0 skieffer   (501) staff       (20)        0 2022-02-13 19:48:35.000000 vertex2tex-0.3.3/vertex2tex/test/__init__.py
--rw-r--r--   0 skieffer   (501) staff       (20)      226 2022-03-11 19:22:33.000000 vertex2tex-0.3.3/vertex2tex/test/test_compress.py
--rw-r--r--   0 skieffer   (501) staff       (20)     1522 2022-03-11 20:00:13.000000 vertex2tex-0.3.3/vertex2tex/test/test_tokenize.py
--rw-r--r--   0 skieffer   (501) staff       (20)     3054 2022-03-11 20:45:21.000000 vertex2tex-0.3.3/vertex2tex/test/test_translate.py
--rw-r--r--   0 skieffer   (501) staff       (20)    15240 2022-03-11 19:52:04.000000 vertex2tex-0.3.3/vertex2tex/v2t.py
-drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2022-03-11 20:54:20.595430 vertex2tex-0.3.3/vertex2tex.egg-info/
--rw-r--r--   0 skieffer   (501) staff       (20)    14839 2022-03-11 20:54:20.000000 vertex2tex-0.3.3/vertex2tex.egg-info/PKG-INFO
--rw-r--r--   0 skieffer   (501) staff       (20)      395 2022-03-11 20:54:20.000000 vertex2tex-0.3.3/vertex2tex.egg-info/SOURCES.txt
--rw-r--r--   0 skieffer   (501) staff       (20)        1 2022-03-11 20:54:20.000000 vertex2tex-0.3.3/vertex2tex.egg-info/dependency_links.txt
--rw-r--r--   0 skieffer   (501) staff       (20)       11 2022-03-11 20:54:20.000000 vertex2tex-0.3.3/vertex2tex.egg-info/top_level.txt
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-08-04 21:58:42.759729 vertex2tex-0.3.4/
+-rw-r--r--   0 skieffer   (501) staff       (20)     1075 2022-02-13 19:49:11.000000 vertex2tex-0.3.4/LICENSE
+-rw-r--r--   0 skieffer   (501) staff       (20)    15050 2023-08-04 21:58:42.759950 vertex2tex-0.3.4/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)    14624 2023-08-04 21:29:15.000000 vertex2tex-0.3.4/README.md
+-rw-r--r--   0 skieffer   (501) staff       (20)       81 2023-01-19 20:31:13.000000 vertex2tex-0.3.4/pyproject.toml
+-rw-r--r--   0 skieffer   (501) staff       (20)      557 2023-08-04 21:58:42.760982 vertex2tex-0.3.4/setup.cfg
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-08-04 21:58:42.754345 vertex2tex-0.3.4/vertex2tex/
+-rw-r--r--   0 skieffer   (501) staff       (20)      215 2023-08-04 20:48:56.000000 vertex2tex-0.3.4/vertex2tex/__init__.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     4954 2022-03-11 19:22:33.000000 vertex2tex-0.3.4/vertex2tex/config.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     4426 2023-08-04 18:22:29.000000 vertex2tex-0.3.4/vertex2tex/document.py
+-rw-r--r--   0 skieffer   (501) staff       (20)      266 2022-03-11 19:22:33.000000 vertex2tex-0.3.4/vertex2tex/excep.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-08-04 21:58:42.759003 vertex2tex-0.3.4/vertex2tex/test/
+-rw-r--r--   0 skieffer   (501) staff       (20)        0 2022-02-13 19:48:35.000000 vertex2tex-0.3.4/vertex2tex/test/__init__.py
+-rw-r--r--   0 skieffer   (501) staff       (20)      226 2022-03-11 19:22:33.000000 vertex2tex-0.3.4/vertex2tex/test/test_compress.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     1522 2022-03-11 20:00:13.000000 vertex2tex-0.3.4/vertex2tex/test/test_tokenize.py
+-rw-r--r--   0 skieffer   (501) staff       (20)     3435 2023-08-04 20:49:07.000000 vertex2tex-0.3.4/vertex2tex/test/test_translate.py
+-rw-r--r--   0 skieffer   (501) staff       (20)    16259 2023-08-04 20:48:56.000000 vertex2tex-0.3.4/vertex2tex/v2t.py
+drwxr-xr-x   0 skieffer   (501) staff       (20)        0 2023-08-04 21:58:42.756779 vertex2tex-0.3.4/vertex2tex.egg-info/
+-rw-r--r--   0 skieffer   (501) staff       (20)    15050 2023-08-04 21:58:42.000000 vertex2tex-0.3.4/vertex2tex.egg-info/PKG-INFO
+-rw-r--r--   0 skieffer   (501) staff       (20)      444 2023-08-04 21:58:42.000000 vertex2tex-0.3.4/vertex2tex.egg-info/SOURCES.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)        1 2023-08-04 21:58:42.000000 vertex2tex-0.3.4/vertex2tex.egg-info/dependency_links.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       33 2023-08-04 21:58:42.000000 vertex2tex-0.3.4/vertex2tex.egg-info/requires.txt
+-rw-r--r--   0 skieffer   (501) staff       (20)       11 2023-08-04 21:58:42.000000 vertex2tex-0.3.4/vertex2tex.egg-info/top_level.txt
```

### Comparing `vertex2tex-0.3.3/LICENSE` & `vertex2tex-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vertex2tex-0.3.3/PKG-INFO` & `vertex2tex-0.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: vertex2tex
-Version: 0.3.3
-Summary: VerTeX: Verbal TeX
-Home-page: https://github.com/skieffer/VerTeX
-Author: Steve Kieffer
-Author-email: sk@skieffer.info
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Text Processing :: Markup :: LaTeX
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # VerTeX: Verbal TeX
 
 Do you find anything cumbersome about TeX syntax? For example, 
 
 | If instead of this...       | you'd prefer to type this...   |
 |:----------------------------|:-------------------------------|
 | a_0, a_1, \ldots, a_{n-1}   | a0, a1, ddd, an-1              |
@@ -46,49 +30,55 @@
 
 However, another feature of VerTeX is that -- with a few key exceptions
 (see below) -- ordinary TeX syntax passes through unaltered, so that you may
 use as many or as few of the features of VerTeX as you wish.
 
 # Usage
 
-There are just two main functions that you'll make use of:
-`translate_snippet`, and `translate_document`.
-
-Apply `translate_snippet` directly to math mode contents written in VerTeX,
-in order to translate them into plain TeX:
+Translate `VerTeX --> TeX` using the `translate_snippet` function:
 
-    >>> from vertex2tex import *
+    >>> from vertex2tex import translate_snippet
     >>> translate_snippet('bbQ(alp)')
     '\\mathbb{Q}(\\alpha)'
 
-When working on an entire document, use `translate_document`.
-The default behavior of `translate_document` is to translate
-the contents of math modes _only if they begin or end (or both) with a `@` character
-inside the usual dollar sign delimiters_.
-(The `@` char(s) are then omitted from the output.)
-This allows you to be selective about where VerTeX is used, and where it isn't.
-
-In particular, this means you can begin typing your math mode expressions as usual, and
-only when you're done decide if you used any VerTeX or not. If so, include a `@` before
-the final `$` or `$$`. If not, leave it out. Thus
-
-    >>> translate_document('$alp@$')
-    '$\\alpha$'
-
-but
-
-    >>> translate_document('$alp$')
-    '$alp$'
-
-Alternatively, this behavior can be modified by using the `translate_document` function's
-keyword argument `keychar`. Setting `keychar=None` means that VerTeX translation will be
-applied to _all_ text occurring within math modes:
+You can also process an entire document with `translate_document`.
+The contents of each math mode will be
+translated *conditionally*: If the math mode begins or ends (or both) with a "@"
+character, then we translate `VerTeX --> TeX`, after stripping the "@" char(s).
+
+    >>> from vertex2tex import translate_document
+    >>> translate_document('Would you prefer $pie$ or $pie@$?')
+    'Would you prefer $pie$ or $\\pi$?'
+
+The purpose of the indicator character "@" is to let you decide in each
+math mode whether you want to use VerTeX or not. Since it can come last
+(just before the closing "$"), you can decide after the fact whether you
+needed VerTeX or not.
+
+If you are certain that you want VerTeX translation to be applied in *every*
+math mode, and don't want to have to add "@" characters, you can pass `None`
+to the `keychar` argument of `translate_document`:
+
+    >>> translate_document('Would you like $pie$?', keychar=None)
+    'Would you like $\\pi$?'
+
+Finally, with `cond_translate_snippet` you can translate a single snippet of
+math mode text, but according to the same conditional rules about "@"
+characters used by `translate_document`:
+
+    >>> from vertex2tex import cond_translate_snippet
+    >>> cond_translate_snippet('@alp')
+    '\\alpha'
+    >>> cond_translate_snippet('alp@')
+    '\\alpha'
+    >>> cond_translate_snippet('@alp@')
+    '\\alpha'
+    >>> cond_translate_snippet('alp')
+    'alp'
 
-    >>> translate_document('$alp$', keychar=None)
-    '$\\alpha$'
 
 
 # The VerTeX Language
 
 ## Slash the Backslashes!
 
 When you are writing mathematics, how often do you want a Greek letter alpha, and how
@@ -365,13 +355,11 @@
 
     \\w  -->  w
     \\   -->  \\
     \w   -->  \w
 
 where `w` is a word at least one character long.
 
-But you probably won't need to use this anyway. In using VerTeX for ten years,
+But you probably won't need to use this anyway. In using VerTeX for over ten years,
 I cannot recall needing it once.
 
 Enjoy!
-
-
```

### Comparing `vertex2tex-0.3.3/README.md` & `vertex2tex-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: vertex2tex
+Version: 0.3.4
+Summary: VerTeX: Verbal TeX
+Home-page: https://github.com/skieffer/VerTeX
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Text Processing :: Markup :: LaTeX
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # VerTeX: Verbal TeX
 
 Do you find anything cumbersome about TeX syntax? For example, 
 
 | If instead of this...       | you'd prefer to type this...   |
 |:----------------------------|:-------------------------------|
 | a_0, a_1, \ldots, a_{n-1}   | a0, a1, ddd, an-1              |
@@ -30,49 +44,55 @@
 
 However, another feature of VerTeX is that -- with a few key exceptions
 (see below) -- ordinary TeX syntax passes through unaltered, so that you may
 use as many or as few of the features of VerTeX as you wish.
 
 # Usage
 
-There are just two main functions that you'll make use of:
-`translate_snippet`, and `translate_document`.
-
-Apply `translate_snippet` directly to math mode contents written in VerTeX,
-in order to translate them into plain TeX:
+Translate `VerTeX --> TeX` using the `translate_snippet` function:
 
-    >>> from vertex2tex import *
+    >>> from vertex2tex import translate_snippet
     >>> translate_snippet('bbQ(alp)')
     '\\mathbb{Q}(\\alpha)'
 
-When working on an entire document, use `translate_document`.
-The default behavior of `translate_document` is to translate
-the contents of math modes _only if they begin or end (or both) with a `@` character
-inside the usual dollar sign delimiters_.
-(The `@` char(s) are then omitted from the output.)
-This allows you to be selective about where VerTeX is used, and where it isn't.
-
-In particular, this means you can begin typing your math mode expressions as usual, and
-only when you're done decide if you used any VerTeX or not. If so, include a `@` before
-the final `$` or `$$`. If not, leave it out. Thus
-
-    >>> translate_document('$alp@$')
-    '$\\alpha$'
-
-but
-
-    >>> translate_document('$alp$')
-    '$alp$'
-
-Alternatively, this behavior can be modified by using the `translate_document` function's
-keyword argument `keychar`. Setting `keychar=None` means that VerTeX translation will be
-applied to _all_ text occurring within math modes:
+You can also process an entire document with `translate_document`.
+The contents of each math mode will be
+translated *conditionally*: If the math mode begins or ends (or both) with a "@"
+character, then we translate `VerTeX --> TeX`, after stripping the "@" char(s).
+
+    >>> from vertex2tex import translate_document
+    >>> translate_document('Would you prefer $pie$ or $pie@$?')
+    'Would you prefer $pie$ or $\\pi$?'
+
+The purpose of the indicator character "@" is to let you decide in each
+math mode whether you want to use VerTeX or not. Since it can come last
+(just before the closing "$"), you can decide after the fact whether you
+needed VerTeX or not.
+
+If you are certain that you want VerTeX translation to be applied in *every*
+math mode, and don't want to have to add "@" characters, you can pass `None`
+to the `keychar` argument of `translate_document`:
+
+    >>> translate_document('Would you like $pie$?', keychar=None)
+    'Would you like $\\pi$?'
+
+Finally, with `cond_translate_snippet` you can translate a single snippet of
+math mode text, but according to the same conditional rules about "@"
+characters used by `translate_document`:
+
+    >>> from vertex2tex import cond_translate_snippet
+    >>> cond_translate_snippet('@alp')
+    '\\alpha'
+    >>> cond_translate_snippet('alp@')
+    '\\alpha'
+    >>> cond_translate_snippet('@alp@')
+    '\\alpha'
+    >>> cond_translate_snippet('alp')
+    'alp'
 
-    >>> translate_document('$alp$', keychar=None)
-    '$\\alpha$'
 
 
 # The VerTeX Language
 
 ## Slash the Backslashes!
 
 When you are writing mathematics, how often do you want a Greek letter alpha, and how
@@ -349,11 +369,11 @@
 
     \\w  -->  w
     \\   -->  \\
     \w   -->  \w
 
 where `w` is a word at least one character long.
 
-But you probably won't need to use this anyway. In using VerTeX for ten years,
+But you probably won't need to use this anyway. In using VerTeX for over ten years,
 I cannot recall needing it once.
 
 Enjoy!
```

### Comparing `vertex2tex-0.3.3/vertex2tex/config.py` & `vertex2tex-0.3.4/vertex2tex/config.py`

 * *Files identical despite different names*

### Comparing `vertex2tex-0.3.3/vertex2tex/document.py` & `vertex2tex-0.3.4/vertex2tex/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,21 +125,15 @@
     n = 0
     seg = segs.next()
     while seg:
         t = seg.getStr()
         # Math mode contents occur precisely on the segments of index 2 mod 4.
         if n == 2 and t:
             try:
-                if keychar is None:
-                    t = translate_snippet(t)
-                else:
-                    i0 = 1 if t[0] == keychar else 0
-                    i1 = 1 if t[-1] == keychar else 0
-                    if i0 + i1:
-                        t = translate_snippet(t[i0:len(t)-i1])
+                t = translate_snippet(t, keychar=keychar)
             except VerTeXError as ve:
                 # Note the segment where the error occurred, and re-raise.
                 ve.set_segment(seg)
                 raise ve
         out += t
         # Increment n mod 4, and get next segment.
         n = (n + 1) % 4
```

### Comparing `vertex2tex-0.3.3/vertex2tex/test/test_tokenize.py` & `vertex2tex-0.3.4/vertex2tex/test/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `vertex2tex-0.3.3/vertex2tex/test/test_translate.py` & `vertex2tex-0.3.4/vertex2tex/test/test_translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,27 @@
     """
     for t, expected in zip(text2, out2):
         out = translate_document(t)
         print(out)
         assert out == expected
 
 
+def test_translate_2b():
+    """
+    Test that, with the default keychar of "@", cond_translate_snippet maps vertex to tex
+    iff the keychar appears first, or last, or both.
+    """
+    for t, expected in zip(text2, out2):
+        t = t.strip("$")
+        expected = expected.strip("$")
+        out = cond_translate_snippet(t)
+        print(out)
+        assert out == expected
+
+
 @pytest.mark.parametrize('raw, expected', [
     ['a1, a2, ddd, an+1', 'a_{1}, a_{2},\\ldots, a_{n+1}'],
     ['xivv1, xivv2, ddd, xivvm', 'x_{i_{1}}, x_{i_{2}},\\ldots, x_{i_{ m}}'],
     ['aijuu2', 'a_{i j}^{2}'],
 
     ['pi', 'p_{i}'],
     ['alphan', '\\alpha_{n}'],
```

### Comparing `vertex2tex-0.3.3/vertex2tex/v2t.py` & `vertex2tex-0.3.4/vertex2tex/v2t.py`

 * *Files 2% similar despite different names*

```diff
@@ -523,19 +523,47 @@
     """
     Delete all whitespace characters except those followed by an upper or lowercase letter.
     :param text: The text to be compressed.
     :return: The compressed text.
     """
     return re.sub(r'\s+(?![a-zA-Z])', '', text)
 
-def translate_snippet(text):
+def translate_snippet(text, keychar=None):
     """
-    Translate a single "snippet" (i.e. the contents of a TeX math mode) from VerTeX into plain TeX.
+    Translate a single "snippet" (i.e. the contents of a TeX math mode) from
+    VerTeX into plain TeX.
+
+    If you have not yet checked keychars, you should pass keychar.
+
     :param text: The text of the snippet.
+    :param keychar: Must be either None or a single character (but not $ or \).
+                    Pass None if you want VerTeX to be applied directly to `text`,
+                    as is.
+                    Otherwise VerTeX is applied only when `text` begins or ends
+                    with the keychar (or both), and after stripping any
+                    occurrences of it.
     :return: The translated text.
     """
-    tokens = tokenize(text)
-    ts = TokenStream(tokens)
-    root = Node(ts)
-    out = root.xlat()
-    out = compress(out)
-    return out
+    if not text:
+        return ''
+
+    if keychar is None:
+        tokens = tokenize(text)
+        ts = TokenStream(tokens)
+        root = Node(ts)
+        out = root.xlat()
+        out = compress(out)
+        return out
+    elif text.startswith(keychar) or text.endswith(keychar):
+        text = text.strip(keychar)
+        return translate_snippet(text, keychar=None)
+    else:
+        return text
+
+
+def cond_translate_snippet(text):
+    """
+    Convenience function to translate math mode contents conditionally, i.e.
+    iff it begins or ends with the standard keychar "@" (then stripping the
+    "@" chars before translating).
+    """
+    return translate_snippet(text, keychar="@")
```

### Comparing `vertex2tex-0.3.3/vertex2tex.egg-info/PKG-INFO` & `vertex2tex-0.3.4/vertex2tex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: vertex2tex
-Version: 0.3.3
+Version: 0.3.4
 Summary: VerTeX: Verbal TeX
 Home-page: https://github.com/skieffer/VerTeX
-Author: Steve Kieffer
-Author-email: sk@skieffer.info
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: LaTeX
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # VerTeX: Verbal TeX
 
 Do you find anything cumbersome about TeX syntax? For example, 
 
 | If instead of this...       | you'd prefer to type this...   |
@@ -46,49 +44,55 @@
 
 However, another feature of VerTeX is that -- with a few key exceptions
 (see below) -- ordinary TeX syntax passes through unaltered, so that you may
 use as many or as few of the features of VerTeX as you wish.
 
 # Usage
 
-There are just two main functions that you'll make use of:
-`translate_snippet`, and `translate_document`.
+Translate `VerTeX --> TeX` using the `translate_snippet` function:
 
-Apply `translate_snippet` directly to math mode contents written in VerTeX,
-in order to translate them into plain TeX:
-
-    >>> from vertex2tex import *
+    >>> from vertex2tex import translate_snippet
     >>> translate_snippet('bbQ(alp)')
     '\\mathbb{Q}(\\alpha)'
 
-When working on an entire document, use `translate_document`.
-The default behavior of `translate_document` is to translate
-the contents of math modes _only if they begin or end (or both) with a `@` character
-inside the usual dollar sign delimiters_.
-(The `@` char(s) are then omitted from the output.)
-This allows you to be selective about where VerTeX is used, and where it isn't.
-
-In particular, this means you can begin typing your math mode expressions as usual, and
-only when you're done decide if you used any VerTeX or not. If so, include a `@` before
-the final `$` or `$$`. If not, leave it out. Thus
-
-    >>> translate_document('$alp@$')
-    '$\\alpha$'
-
-but
-
-    >>> translate_document('$alp$')
-    '$alp$'
-
-Alternatively, this behavior can be modified by using the `translate_document` function's
-keyword argument `keychar`. Setting `keychar=None` means that VerTeX translation will be
-applied to _all_ text occurring within math modes:
+You can also process an entire document with `translate_document`.
+The contents of each math mode will be
+translated *conditionally*: If the math mode begins or ends (or both) with a "@"
+character, then we translate `VerTeX --> TeX`, after stripping the "@" char(s).
+
+    >>> from vertex2tex import translate_document
+    >>> translate_document('Would you prefer $pie$ or $pie@$?')
+    'Would you prefer $pie$ or $\\pi$?'
+
+The purpose of the indicator character "@" is to let you decide in each
+math mode whether you want to use VerTeX or not. Since it can come last
+(just before the closing "$"), you can decide after the fact whether you
+needed VerTeX or not.
+
+If you are certain that you want VerTeX translation to be applied in *every*
+math mode, and don't want to have to add "@" characters, you can pass `None`
+to the `keychar` argument of `translate_document`:
+
+    >>> translate_document('Would you like $pie$?', keychar=None)
+    'Would you like $\\pi$?'
+
+Finally, with `cond_translate_snippet` you can translate a single snippet of
+math mode text, but according to the same conditional rules about "@"
+characters used by `translate_document`:
+
+    >>> from vertex2tex import cond_translate_snippet
+    >>> cond_translate_snippet('@alp')
+    '\\alpha'
+    >>> cond_translate_snippet('alp@')
+    '\\alpha'
+    >>> cond_translate_snippet('@alp@')
+    '\\alpha'
+    >>> cond_translate_snippet('alp')
+    'alp'
 
-    >>> translate_document('$alp$', keychar=None)
-    '$\\alpha$'
 
 
 # The VerTeX Language
 
 ## Slash the Backslashes!
 
 When you are writing mathematics, how often do you want a Greek letter alpha, and how
@@ -365,13 +369,11 @@
 
     \\w  -->  w
     \\   -->  \\
     \w   -->  \w
 
 where `w` is a word at least one character long.
 
-But you probably won't need to use this anyway. In using VerTeX for ten years,
+But you probably won't need to use this anyway. In using VerTeX for over ten years,
 I cannot recall needing it once.
 
 Enjoy!
-
-
```

