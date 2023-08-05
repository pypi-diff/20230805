# Comparing `tmp/jmcomic-2.1.8.tar.gz` & `tmp/jmcomic-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.1.8.tar", last modified: Thu Aug  3 14:58:19 2023, max compression
+gzip compressed data, was "jmcomic-2.1.9.tar", last modified: Sat Aug  5 11:24:46 2023, max compression
```

## Comparing `jmcomic-2.1.8.tar` & `jmcomic-2.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:58:19.707510 jmcomic-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 14:58:07.000000 jmcomic-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-03 14:58:19.707510 jmcomic-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-03 14:58:07.000000 jmcomic-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 14:58:19.707510 jmcomic-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-03 14:58:07.000000 jmcomic-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:58:19.703510 jmcomic-2.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:58:19.703510 jmcomic-2.1.8/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-03 14:58:07.000000 jmcomic-2.1.8/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 14:58:07.000000 jmcomic-2.1.8/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13616 2023-08-03 14:58:07.000000 jmcomic-2.1.8/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-08-03 14:58:07.000000 jmcomic-2.1.8/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-08-03 14:58:07.000000 jmcomic-2.1.8/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-08-03 14:58:07.000000 jmcomic-2.1.8/src/jmcomic/jm_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-08-03 14:58:07.000000 jmcomic-2.1.8/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-08-03 14:58:07.000000 jmcomic-2.1.8/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11858 2023-08-03 14:58:07.000000 jmcomic-2.1.8/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 14:58:19.707510 jmcomic-2.1.8/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-03 14:58:19.000000 jmcomic-2.1.8/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-03 14:58:19.000000 jmcomic-2.1.8/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 14:58:19.000000 jmcomic-2.1.8/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-03 14:58:19.000000 jmcomic-2.1.8/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 14:58:19.000000 jmcomic-2.1.8/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:46.577999 jmcomic-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-05 11:24:38.000000 jmcomic-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-05 11:24:46.577999 jmcomic-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-08-05 11:24:38.000000 jmcomic-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 11:24:46.577999 jmcomic-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-05 11:24:38.000000 jmcomic-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:46.577999 jmcomic-2.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:46.577999 jmcomic-2.1.9/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-05 11:24:38.000000 jmcomic-2.1.9/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-05 11:24:38.000000 jmcomic-2.1.9/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-08-05 11:24:38.000000 jmcomic-2.1.9/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-08-05 11:24:38.000000 jmcomic-2.1.9/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-08-05 11:24:38.000000 jmcomic-2.1.9/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-08-05 11:24:38.000000 jmcomic-2.1.9/src/jmcomic/jm_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-08-05 11:24:38.000000 jmcomic-2.1.9/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9559 2023-08-05 11:24:38.000000 jmcomic-2.1.9/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-08-05 11:24:38.000000 jmcomic-2.1.9/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:24:46.577999 jmcomic-2.1.9/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-08-05 11:24:46.000000 jmcomic-2.1.9/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-05 11:24:46.000000 jmcomic-2.1.9/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:24:46.000000 jmcomic-2.1.9/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-05 11:24:46.000000 jmcomic-2.1.9/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-05 11:24:46.000000 jmcomic-2.1.9/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.1.8/LICENSE` & `jmcomic-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.8/PKG-INFO` & `jmcomic-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.1.8/README.md` & `jmcomic-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.8/setup.py` & `jmcomic-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.8/src/jmcomic/api.py` & `jmcomic-2.1.9/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.8/src/jmcomic/jm_client_impl.py` & `jmcomic-2.1.9/src/jmcomic/jm_client_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,37 +59,36 @@
             )
             jm_debug('api', url)
         else:
             # 图片url
             pass
 
         if domain_index != 0 or retry_count != 0:
-            jm_debug(
-                f'request_retry',
-                ', '.join([
-                    f'次数: [{retry_count}/{self.retry_times}]',
-                    f'域名: [{domain_index} of {self.domain_list}]',
-                    f'路径: [{url}]',
-                    f'参数: [{kwargs if "login" not in url else "#login_form#"}]'
-                ])
-            )
+            jm_debug(f'req.retry',
+                     ', '.join([
+                         f'次数: [{retry_count}/{self.retry_times}]',
+                         f'域名: [{domain_index} of {self.domain_list}]',
+                         f'路径: [{url}]',
+                         f'参数: [{kwargs if "login" not in url else "#login_form#"}]'
+                     ])
+                     )
 
         try:
             return request(url, **kwargs)
         except Exception as e:
             self.before_retry(e, kwargs, retry_count, url)
 
         if retry_count < self.retry_times:
             return self.request_with_retry(request, url, domain_index, retry_count + 1, **kwargs)
         else:
             return self.request_with_retry(request, url, domain_index + 1, 0, **kwargs)
 
     # noinspection PyMethodMayBeStatic, PyUnusedLocal
     def before_retry(self, e, kwargs, retry_count, url):
-        jm_debug('retry', str(e))
+        jm_debug('req.err', str(e))
 
     def enable_cache(self, debug=False):
         def wrap_func_cache(func_name, cache_dict_name):
             import common
             if common.VERSION > '0.4.8':
                 if hasattr(self, cache_dict_name):
                     return
@@ -130,15 +129,15 @@
 
     def get_jmcomic_domain_all(self, postman=None):
         return JmModuleConfig.get_jmcomic_domain_all(postman or self.get_root_postman())
 
     # noinspection PyUnusedLocal
     def fallback(self, request, url, domain_index, retry_count, **kwargs):
         msg = f"请求重试全部失败: [{url}], {self.domain_list}"
-        jm_debug('fallback', "msg")
+        jm_debug('fallback', msg)
         raise AssertionError(msg)
 
 
 # 基于网页实现的JmClient
 class JmHtmlClient(AbstractJmClient):
 
     def get_album_detail(self, album_id) -> JmAlbumDetail:
@@ -282,26 +281,26 @@
         # 处理回复评论
         if comment_id is not None:
             data.pop('status')
             data['comment_id'] = comment_id
             data['is_reply'] = 1
             data['forum_subject'] = 1
 
-        jm_debug('album_comment',
+        jm_debug('album.comment',
                  f'{video_id}: [{comment}]' +
                  (f' to ({comment_id})' if comment_id is not None else '')
                  )
 
         resp = self.post('https://18comic.vip/ajax/album_comment',
                          headers=JmModuleConfig.album_comment_headers,
                          data=data,
                          )
 
         ret = JmAcResp(resp)
-        jm_debug('album_comment', f'{video_id}: [{comment}] ← ({ret.model().cid})')
+        jm_debug('album.comment', f'{video_id}: [{comment}] ← ({ret.model().cid})')
 
         return ret
 
     @classmethod
     def require_resp_success_else_raise(cls, resp, req_url):
         # 1. 检查是否 album_missing
         error_album_missing = '/error/album_missing'
```

### Comparing `jmcomic-2.1.8/src/jmcomic/jm_client_interface.py` & `jmcomic-2.1.9/src/jmcomic/jm_client_interface.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.8/src/jmcomic/jm_config.py` & `jmcomic-2.1.9/src/jmcomic/jm_config.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.8/src/jmcomic/jm_downloader.py` & `jmcomic-2.1.9/src/jmcomic/jm_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,47 +5,47 @@
     pass
 
 
 # noinspection PyMethodMayBeStatic
 class DownloadCallback:
 
     def before_album(self, album: JmAlbumDetail):
-        jm_debug('album-before',
+        jm_debug('album.before',
                  f'本子获取成功: [{album.id}], '
                  f'作者: [{album.author}], '
                  f'章节数: [{len(album)}], '
                  f'标题: [{album.title}], '
                  )
 
     def after_album(self, album: JmAlbumDetail):
-        jm_debug('album-after', f'本子下载完成: [{album.id}]')
+        jm_debug('album.after', f'本子下载完成: [{album.id}]')
 
     def before_photo(self, photo: JmPhotoDetail):
-        jm_debug('photo-before',
+        jm_debug('photo.before',
                  f'开始下载章节: {photo.id} ({photo.album_id}[{photo.index}/{len(photo.from_album)}]), '
                  f'标题: [{photo.title}], '
                  f'图片数为[{len(photo)}]'
                  )
 
     def after_photo(self, photo: JmPhotoDetail):
-        jm_debug('photo-after',
+        jm_debug('photo.after',
                  f'章节下载完成: {photo.id} ({photo.album_id}[{photo.index}/{len(photo.from_album)}])')
 
     def before_image(self, image: JmImageDetail, img_save_path):
         if image.is_exists:
-            jm_debug('image-before',
+            jm_debug('image.before',
                      f'图片已存在: {image.tag} ← [{img_save_path}]'
                      )
         else:
-            jm_debug('image-before',
+            jm_debug('image.before',
                      f'图片准备下载: {image.tag}, [{image.img_url}] → [{img_save_path}]'
                      )
 
     def after_image(self, image: JmImageDetail, img_save_path):
-        jm_debug('image-after',
+        jm_debug('image.after',
                  f'图片下载完成: {image.tag}, [{image.img_url}] → [{img_save_path}]')
 
 
 class JmDownloader(DownloadCallback):
     """
     JmDownloader = JmOption + 调度逻辑
     """
@@ -135,10 +135,10 @@
         return self.option.build_jm_client()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_type is not None:
-            jm_debug('exception',
+            jm_debug('dler.exception',
                      f'{self.__class__.__name__} Exit with exception: {exc_type, exc_val}'
                      )
```

### Comparing `jmcomic-2.1.8/src/jmcomic/jm_entity.py` & `jmcomic-2.1.9/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.8/src/jmcomic/jm_option.py` & `jmcomic-2.1.9/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.1.8/src/jmcomic/jm_toolkit.py` & `jmcomic-2.1.9/src/jmcomic/jm_toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .jm_entity import *
+from PIL import Image
 
 
 class JmcomicText:
     pattern_jm_domain = compile('https://([\w.-]+)')
     pattern_jm_pa_id = compile('/(photos?|album)/(\d+)')
     pattern_html_jm_pub_domain = compile('[\w-]+\.\w+/?\w+')
 
@@ -210,15 +211,15 @@
         @param resp: Response对象
         @param filepath: 响应数据保存的绝对路径
         @param need_convert: True 使用PIL打开图片再保存; False 直接保存resp.content;
         如果需要改变图片的格式，比如 .jpg → .png，则需要neet_convert=True。
         如果不需要改变文件的格式，使用need_convert=False可以跳过PIL解析图片，效率更高。
         """
         if need_convert is True:
-            cls.open_Image(resp.content).save(filepath)
+            cls.save_image(cls.open_Image(resp.content), filepath)
         else:
             save_resp_content(resp, filepath)
 
     @classmethod
     def save_resp_decoded_img(cls,
                               resp: Any,
                               image: JmImageDetail,
@@ -279,24 +280,27 @@
 
             img_decode.paste(
                 img_src.crop((0, y, copyW, y + copyH)),
                 (0, py, copyW, py + copyH)
             )
 
         # 保存到新的解密文件
-        img_decode.save(decoded_save_path)
+        cls.save_image(img_decode, decoded_save_path)
 
     @classmethod
     def open_Image(cls, fp: Union[str, bytes]):
-        from PIL import Image
         from io import BytesIO
         fp = fp if isinstance(fp, str) else BytesIO(fp)
         return Image.open(fp)
 
     @classmethod
+    def save_image(cls, image: Image, filepath: str):
+        image.save(filepath)
+
+    @classmethod
     def get_num(cls, scramble_id, aid, filename: str) -> int:
         """
         获得图片分割数
         """
 
         scramble_id = int(scramble_id)
         aid = int(aid)
```

### Comparing `jmcomic-2.1.8/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.1.9/src/jmcomic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

