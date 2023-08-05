# Comparing `tmp/sankaku-1.0.3.tar.gz` & `tmp/sankaku-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sankaku-1.0.3.tar", last modified: Sat Jun 17 19:01:45 2023, max compression
+gzip compressed data, was "sankaku-1.0.4.tar", last modified: Sat Aug  5 16:30:46 2023, max compression
```

## Comparing `sankaku-1.0.3.tar` & `sankaku-1.0.4.tar`

### file list

```diff
@@ -1,42 +1,38 @@
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.919839 sankaku-1.0.3/
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1064 2023-05-15 12:04:32.000000 sankaku-1.0.3/LICENSE
--rw-r--r--   0 moldus    (1000) moldus    (1000)       90 2023-06-17 14:43:33.000000 sankaku-1.0.3/MANIFEST.in
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3248 2023-06-17 19:01:45.919839 sankaku-1.0.3/PKG-INFO
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2445 2023-06-17 18:44:48.000000 sankaku-1.0.3/README.md
--rw-r--r--   0 moldus    (1000) moldus    (1000)       81 2023-05-15 15:32:11.000000 sankaku-1.0.3/pyproject.toml
--rw-r--r--   0 moldus    (1000) moldus    (1000)       13 2023-05-31 03:19:49.000000 sankaku-1.0.3/requirements-socks.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)      126 2023-06-17 14:43:33.000000 sankaku-1.0.3/requirements-test.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)       80 2023-06-01 19:36:49.000000 sankaku-1.0.3/requirements.txt
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.916839 sankaku-1.0.3/sankaku/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      120 2023-05-29 15:50:51.000000 sankaku-1.0.3/sankaku/__init__.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.917839 sankaku-1.0.3/sankaku/clients/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      351 2023-05-16 19:34:35.000000 sankaku-1.0.3/sankaku/clients/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1228 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/clients/abc.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)    15472 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/clients/clients.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3258 2023-06-01 20:18:47.000000 sankaku-1.0.3/sankaku/clients/http_client.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1325 2023-05-31 03:19:49.000000 sankaku-1.0.3/sankaku/constants.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1748 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/errors.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.918839 sankaku-1.0.3/sankaku/models/
--rw-r--r--   0 moldus    (1000) moldus    (1000)      104 2023-05-14 06:27:00.000000 sankaku-1.0.3/sankaku/models/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      202 2023-06-17 18:03:24.000000 sankaku-1.0.3/sankaku/models/base.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1935 2023-06-17 17:20:37.000000 sankaku-1.0.3/sankaku/models/books.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      367 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/models/http.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      268 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/models/pages.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3657 2023-06-17 17:35:06.000000 sankaku-1.0.3/sankaku/models/posts.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     4418 2023-06-17 17:43:40.000000 sankaku-1.0.3/sankaku/models/tags.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2469 2023-06-17 17:14:26.000000 sankaku-1.0.3/sankaku/models/users.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.919839 sankaku-1.0.3/sankaku/paginators/
--rw-r--r--   0 moldus    (1000) moldus    (1000)       26 2023-05-13 09:01:36.000000 sankaku-1.0.3/sankaku/paginators/__init__.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      829 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/paginators/abc.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)    10560 2023-05-31 04:05:29.000000 sankaku-1.0.3/sankaku/paginators/paginators.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)      380 2023-05-31 04:05:29.000000 sankaku-1.0.3/sankaku/typedefs.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1986 2023-05-31 04:15:17.000000 sankaku-1.0.3/sankaku/types.py
--rw-r--r--   0 moldus    (1000) moldus    (1000)     2049 2023-06-17 15:58:03.000000 sankaku-1.0.3/sankaku/utils.py
-drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-06-17 19:01:45.917839 sankaku-1.0.3/sankaku.egg-info/
--rw-r--r--   0 moldus    (1000) moldus    (1000)     3248 2023-06-17 19:01:45.000000 sankaku-1.0.3/sankaku.egg-info/PKG-INFO
--rw-r--r--   0 moldus    (1000) moldus    (1000)      773 2023-06-17 19:01:45.000000 sankaku-1.0.3/sankaku.egg-info/SOURCES.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)        1 2023-06-17 19:01:45.000000 sankaku-1.0.3/sankaku.egg-info/dependency_links.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)      242 2023-06-17 19:01:45.000000 sankaku-1.0.3/sankaku.egg-info/requires.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)        8 2023-06-17 19:01:45.000000 sankaku-1.0.3/sankaku.egg-info/top_level.txt
--rw-r--r--   0 moldus    (1000) moldus    (1000)       38 2023-06-17 19:01:45.919839 sankaku-1.0.3/setup.cfg
--rw-r--r--   0 moldus    (1000) moldus    (1000)     1631 2023-06-17 19:00:05.000000 sankaku-1.0.3/setup.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-08-05 16:30:46.777211 sankaku-1.0.4/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1064 2023-05-15 12:04:32.000000 sankaku-1.0.4/LICENSE
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3268 2023-08-05 16:30:46.777211 sankaku-1.0.4/PKG-INFO
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2445 2023-08-05 13:52:42.000000 sankaku-1.0.4/README.md
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2166 2023-08-05 15:54:41.000000 sankaku-1.0.4/pyproject.toml
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-08-05 16:30:46.773211 sankaku-1.0.4/sankaku/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      120 2023-05-29 15:50:51.000000 sankaku-1.0.4/sankaku/__init__.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-08-05 16:30:46.774211 sankaku-1.0.4/sankaku/clients/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      351 2023-05-16 19:34:35.000000 sankaku-1.0.4/sankaku/clients/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1228 2023-05-31 04:15:17.000000 sankaku-1.0.4/sankaku/clients/abc.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)    15472 2023-07-01 20:27:32.000000 sankaku-1.0.4/sankaku/clients/clients.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3258 2023-08-05 13:34:56.000000 sankaku-1.0.4/sankaku/clients/http_client.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1325 2023-07-01 20:27:41.000000 sankaku-1.0.4/sankaku/constants.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1748 2023-05-31 04:15:17.000000 sankaku-1.0.4/sankaku/errors.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-08-05 16:30:46.776211 sankaku-1.0.4/sankaku/models/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      104 2023-05-14 06:27:00.000000 sankaku-1.0.4/sankaku/models/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      185 2023-08-05 15:54:41.000000 sankaku-1.0.4/sankaku/models/base.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1945 2023-08-05 15:54:41.000000 sankaku-1.0.4/sankaku/models/books.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      367 2023-05-31 04:15:17.000000 sankaku-1.0.4/sankaku/models/http.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      268 2023-05-31 04:15:17.000000 sankaku-1.0.4/sankaku/models/pages.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     4658 2023-08-05 15:54:41.000000 sankaku-1.0.4/sankaku/models/posts.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     4418 2023-08-05 13:52:42.000000 sankaku-1.0.4/sankaku/models/tags.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2483 2023-08-05 15:54:41.000000 sankaku-1.0.4/sankaku/models/users.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-08-05 16:30:46.777211 sankaku-1.0.4/sankaku/paginators/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       26 2023-05-13 09:01:36.000000 sankaku-1.0.4/sankaku/paginators/__init__.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      829 2023-05-31 04:15:17.000000 sankaku-1.0.4/sankaku/paginators/abc.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)    10560 2023-08-05 13:35:32.000000 sankaku-1.0.4/sankaku/paginators/paginators.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      380 2023-05-31 04:05:29.000000 sankaku-1.0.4/sankaku/typedefs.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1977 2023-08-05 15:54:41.000000 sankaku-1.0.4/sankaku/types.py
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     2049 2023-06-17 15:58:03.000000 sankaku-1.0.4/sankaku/utils.py
+drwxr-xr-x   0 moldus    (1000) moldus    (1000)        0 2023-08-05 16:30:46.774211 sankaku-1.0.4/sankaku.egg-info/
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     3268 2023-08-05 16:30:46.000000 sankaku-1.0.4/sankaku.egg-info/PKG-INFO
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      699 2023-08-05 16:30:46.000000 sankaku-1.0.4/sankaku.egg-info/SOURCES.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)        1 2023-08-05 16:30:46.000000 sankaku-1.0.4/sankaku.egg-info/dependency_links.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)      278 2023-08-05 16:30:46.000000 sankaku-1.0.4/sankaku.egg-info/requires.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)        8 2023-08-05 16:30:46.000000 sankaku-1.0.4/sankaku.egg-info/top_level.txt
+-rw-r--r--   0 moldus    (1000) moldus    (1000)       38 2023-08-05 16:30:46.777211 sankaku-1.0.4/setup.cfg
+-rw-r--r--   0 moldus    (1000) moldus    (1000)     1631 2023-08-05 16:26:56.000000 sankaku-1.0.4/setup.py
```

### Comparing `sankaku-1.0.3/LICENSE` & `sankaku-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/PKG-INFO` & `sankaku-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sankaku
-Version: 1.0.3
+Version: 1.0.4
 Summary: Asynchronous API wrapper for Sankaku Complex.
 Home-page: https://github.com/zerex290/sankaku
 Author: zerex290
 Author-email: zerex290@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/zerex290/sankaku/issues
 Keywords: sankaku,sankakucomplex,api
@@ -14,15 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: socks
-Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 <h1 align="center">
   <a href="https://github.com/zerex290/sankaku">
     <img src="https://raw.githubusercontent.com/zerex290/sankaku/main/docs/icon.png" alt="Sankaku Complex"
     width="150" height="150"/>
   </a>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: sankaku Version: 1.0.3 Summary: Asynchronous API
+Metadata-Version: 2.1 Name: sankaku Version: 1.0.4 Summary: Asynchronous API
 wrapper for Sankaku Complex. Home-page: https://github.com/zerex290/sankaku
 Author: zerex290 Author-email: zerex290@gmail.com License: MIT Project-URL:
 Issue Tracker, https://github.com/zerex290/sankaku/issues Keywords:
 sankaku,sankakucomplex,api Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-socks Provides-Extra: test License-File: LICENSE
+socks Provides-Extra: dev Provides-Extra: docs License-File: LICENSE
                                [Sankaku_Complex]
                                     sankaku
                             For real men of culture
 ## About Asynchronous API wrapper for [Sankaku Complex](https://
 beta.sankakucomplex.com) with *type-hinting*, pydantic *data validation* and an
 optional *logging support* with loguru. ### Features: - Type-hints -
 Deserialization of raw json data thanks to pydantic models - Enumerations for
```

### Comparing `sankaku-1.0.3/README.md` & `sankaku-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/sankaku/clients/abc.py` & `sankaku-1.0.4/sankaku/clients/abc.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/sankaku/clients/clients.py` & `sankaku-1.0.4/sankaku/clients/clients.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/sankaku/clients/http_client.py` & `sankaku-1.0.4/sankaku/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/sankaku/constants.py` & `sankaku-1.0.4/sankaku/constants.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/sankaku/errors.py` & `sankaku-1.0.4/sankaku/errors.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/sankaku/models/books.py` & `sankaku-1.0.4/sankaku/models/books.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     name_en: Optional[str]
     name_ja: Optional[str]
     description: str
     description_en: Optional[str]
     description_ja: Optional[str]
     created_at: datetime
     updated_at: datetime  # Not sure that update dt isn't optional
-    author: Author
+    author: Optional[Author]
     is_public: bool
     is_active: bool
     is_flagged: bool
     post_count: int
     pages_count: int
     visible_post_count: int
     is_intact: bool
```

### Comparing `sankaku-1.0.3/sankaku/models/posts.py` & `sankaku-1.0.4/sankaku/models/posts.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,48 @@
 from .users import Author
 
 
 __all__ = ["Comment", "Post", "AIPost"]
 
 
 class GenerationDirectives(SankakuResponseModel):
+    # Model fields were tested on 100 pages.
+
+    tags: list[dict]
+    # Possible JSON object properties:
+    #   - id: int
+    #   - name: str
+    #   - type: int
+    #   - count: int
+    #   - rating: str
+    #   - name_en: str
+    #   - name_ja: str
+    #   - tagName: str
+    #   - pool_count: int
+    #   - post_count: int
+    #   - series_count: int
+    #   tag_translations: list[Any]  # IDK list items types
+
+    aspect_ratio: Optional[dict] = None
+    # Possible JSON object properties:
+    #   - type: str
+    #   - width: int
+    #   - height: int
+
+    rating: Optional[dict] = None
+    # Possible JSON object properties:
+    #   - value: str
+    #   - default: str
+
+    negative_prompt: Optional[str] = None
+    natural_input: Optional[str] = None
+    denoising_strength: Optional[int] = None
+
+
+class AIGenerationDirectives(SankakuResponseModel):
     """Model that describes additional fields for AI-generated posts."""
     width: int
     height: int
     prompt: str
     batch_size: int
     batch_count: int
     sampling_steps: int
@@ -38,15 +72,14 @@
     author: Author
     file_url: Optional[str]
     preview_url: Optional[str]
     width: int
     height: int
     file_size: int
     extension: Optional[str] = Field(alias="file_type")
-    generation_directives: Optional[GenerationDirectives]
     md5: str
     tags: List[PostTag]
 
     @property
     def file_type(self) -> Optional[types.FileType]:
         """Get type of the file."""
         if self.extension in ('png', 'jpeg', 'webp'):
@@ -109,26 +142,31 @@
     source: Optional[str]
     in_visible_pool: bool
     is_premium: bool
     is_rating_locked: bool
     is_note_locked: bool
     is_status_locked: bool
     redirect_to_signup: bool
-    sequence: Optional[int]
+
+    # Sequence can be missing when Post model used inside PageBook model
+    sequence: Optional[int] = None
+
     video_duration: Optional[float]
+    generation_directives: Optional[GenerationDirectives]
 
 
 class AIPost(BasePost):
     """Model that describes AI-generated posts.
 
     There is possibility that AI posts have the same fields as common posts,
     but premium account is needed to check it properly. So this model is
     actual for non-premium accounts.
     """
     updated_at: Optional[datetime]
     post_associated_id: Optional[int]
+    generation_directives: Optional[AIGenerationDirectives]
 
     # Validators
     _normalize_datetime = (
         validator("created_at", "updated_at", pre=True, allow_reuse=True)
         (convert_ts_to_datetime)
     )
```

### Comparing `sankaku-1.0.3/sankaku/models/tags.py` & `sankaku-1.0.4/sankaku/models/tags.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/sankaku/models/users.py` & `sankaku-1.0.4/sankaku/models/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     series_update_count: int
     tag_update_count: int
     artist_update_count: int
 
     # The following fields can be missing in server JSON response
     last_logged_in_at: Optional[datetime] = None
     favorite_count: Optional[int] = None
-    post_favorite_count: Optional[int]
-    pool_favorite_count: Optional[int]
+    post_favorite_count: Optional[int] = None
+    pool_favorite_count: Optional[int] = None
     vote_count: Optional[int] = None
     post_vote_count: Optional[int] = None
     pool_vote_count: Optional[int] = None
     recommended_posts_for_user: Optional[int] = None
     subscriptions: List[str] = []
 
     # The following fields was removed from server JSON response
```

### Comparing `sankaku-1.0.3/sankaku/paginators/abc.py` & `sankaku-1.0.4/sankaku/paginators/abc.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/sankaku/paginators/paginators.py` & `sankaku-1.0.4/sankaku/paginators/paginators.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/sankaku/types.py` & `sankaku-1.0.4/sankaku/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     META = 9
     GENRE = 5
     STUDIO = 2
 
 
 class FileType(Enum):
     IMAGE = "image"  # jpeg, png, webp formats
-    GIF = "animated_gif"  # gif format
+    GIF = "gif"  # gif format
     VIDEO = "video"  # mp4, webm formats
 
 
 class FileSize(Enum):
     LARGE = "large_filesize"
     HUGE = "extremely_large_filesize"
     LONG = "long_image"
```

### Comparing `sankaku-1.0.3/sankaku/utils.py` & `sankaku-1.0.4/sankaku/utils.py`

 * *Files identical despite different names*

### Comparing `sankaku-1.0.3/sankaku.egg-info/PKG-INFO` & `sankaku-1.0.4/sankaku.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sankaku
-Version: 1.0.3
+Version: 1.0.4
 Summary: Asynchronous API wrapper for Sankaku Complex.
 Home-page: https://github.com/zerex290/sankaku
 Author: zerex290
 Author-email: zerex290@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/zerex290/sankaku/issues
 Keywords: sankaku,sankakucomplex,api
@@ -14,15 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: socks
-Provides-Extra: test
+Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 <h1 align="center">
   <a href="https://github.com/zerex290/sankaku">
     <img src="https://raw.githubusercontent.com/zerex290/sankaku/main/docs/icon.png" alt="Sankaku Complex"
     width="150" height="150"/>
   </a>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: sankaku Version: 1.0.3 Summary: Asynchronous API
+Metadata-Version: 2.1 Name: sankaku Version: 1.0.4 Summary: Asynchronous API
 wrapper for Sankaku Complex. Home-page: https://github.com/zerex290/sankaku
 Author: zerex290 Author-email: zerex290@gmail.com License: MIT Project-URL:
 Issue Tracker, https://github.com/zerex290/sankaku/issues Keywords:
 sankaku,sankakucomplex,api Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown Provides-Extra:
-socks Provides-Extra: test License-File: LICENSE
+socks Provides-Extra: dev Provides-Extra: docs License-File: LICENSE
                                [Sankaku_Complex]
                                     sankaku
                             For real men of culture
 ## About Asynchronous API wrapper for [Sankaku Complex](https://
 beta.sankakucomplex.com) with *type-hinting*, pydantic *data validation* and an
 optional *logging support* with loguru. ### Features: - Type-hints -
 Deserialization of raw json data thanks to pydantic models - Enumerations for
```

### Comparing `sankaku-1.0.3/sankaku.egg-info/SOURCES.txt` & `sankaku-1.0.4/sankaku.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
-requirements-socks.txt
-requirements-test.txt
-requirements.txt
 setup.py
 sankaku/__init__.py
 sankaku/constants.py
 sankaku/errors.py
 sankaku/typedefs.py
 sankaku/types.py
 sankaku/utils.py
```

### Comparing `sankaku-1.0.3/setup.py` & `sankaku-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     item.group(1): _load_req(item.group(0))
     for item in [_REQ_PATTERN.fullmatch(reqpath) for reqpath in os.listdir()]
     if item
 }
 
 setuptools.setup(
     name="sankaku",
-    version="1.0.3",
+    version="1.0.4",
     author="zerex290",
     author_email="zerex290@gmail.com",
     description="Asynchronous API wrapper for Sankaku Complex.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="sankaku sankakucomplex api".split(),
     url="https://github.com/zerex290/sankaku",
```

