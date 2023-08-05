# Comparing `tmp/django-selenium-test-1.1.0.tar.gz` & `tmp/django-selenium-test-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-selenium-test-1.1.0.tar", last modified: Sun Aug 30 11:12:30 2020, max compression
+gzip compressed data, was "django-selenium-test-2.0.0.tar", last modified: Sat Aug  5 08:38:10 2023, max compression
```

## Comparing `django-selenium-test-1.1.0.tar` & `django-selenium-test-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 twiesing  (1000) users      (100)        0 2020-08-30 11:12:30.048579 django-selenium-test-1.1.0/
--rw-r--r--   0 twiesing  (1000) users      (100)      472 2020-08-30 10:04:09.000000 django-selenium-test-1.1.0/CHANGES.txt
--rw-r--r--   0 twiesing  (1000) users      (100)     1573 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/LICENSE.txt
--rw-r--r--   0 twiesing  (1000) users      (100)       59 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/MANIFEST.in
--rw-r--r--   0 twiesing  (1000) users      (100)    12506 2020-08-30 11:12:30.048579 django-selenium-test-1.1.0/PKG-INFO
--rw-r--r--   0 twiesing  (1000) users      (100)     9265 2020-08-30 11:01:09.000000 django-selenium-test-1.1.0/README.md
-drwxr-xr-x   0 twiesing  (1000) users      (100)        0 2020-08-30 11:12:30.047579 django-selenium-test-1.1.0/django_selenium_test/
--rw-r--r--   0 twiesing  (1000) users      (100)      106 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/django_selenium_test/__init__.py
--rw-r--r--   0 twiesing  (1000) users      (100)    10070 2020-08-30 09:53:53.000000 django-selenium-test-1.1.0/django_selenium_test/core.py
--rw-r--r--   0 twiesing  (1000) users      (100)    17582 2020-08-30 09:53:53.000000 django-selenium-test-1.1.0/django_selenium_test/integration.py
--rw-r--r--   0 twiesing  (1000) users      (100)     1495 2020-08-30 09:53:53.000000 django-selenium-test-1.1.0/django_selenium_test/settings.py
-drwxr-xr-x   0 twiesing  (1000) users      (100)        0 2020-08-30 11:12:30.047579 django-selenium-test-1.1.0/django_selenium_test.egg-info/
--rw-r--r--   0 twiesing  (1000) users      (100)    12506 2020-08-30 11:12:30.000000 django-selenium-test-1.1.0/django_selenium_test.egg-info/PKG-INFO
--rw-r--r--   0 twiesing  (1000) users      (100)      625 2020-08-30 11:12:30.000000 django-selenium-test-1.1.0/django_selenium_test.egg-info/SOURCES.txt
--rw-r--r--   0 twiesing  (1000) users      (100)        1 2020-08-30 11:12:30.000000 django-selenium-test-1.1.0/django_selenium_test.egg-info/dependency_links.txt
--rw-r--r--   0 twiesing  (1000) users      (100)       35 2020-08-30 11:12:30.000000 django-selenium-test-1.1.0/django_selenium_test.egg-info/requires.txt
--rw-r--r--   0 twiesing  (1000) users      (100)       27 2020-08-30 11:12:30.000000 django-selenium-test-1.1.0/django_selenium_test.egg-info/top_level.txt
--rw-r--r--   0 twiesing  (1000) users      (100)       38 2020-08-30 11:12:30.049579 django-selenium-test-1.1.0/setup.cfg
--rwxr-xr-x   0 twiesing  (1000) users      (100)     1298 2020-08-30 11:11:30.000000 django-selenium-test-1.1.0/setup.py
-drwxr-xr-x   0 twiesing  (1000) users      (100)        0 2020-08-30 11:12:30.048579 django-selenium-test-1.1.0/tests/
--rw-r--r--   0 twiesing  (1000) users      (100)        0 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/tests/__init__.py
--rw-r--r--   0 twiesing  (1000) users      (100)      218 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/tests/forms.py
--rwxr-xr-x   0 twiesing  (1000) users      (100)     1299 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/tests/manage.py
--rw-r--r--   0 twiesing  (1000) users      (100)     1320 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/tests/settings.py
-drwxr-xr-x   0 twiesing  (1000) users      (100)        0 2020-08-30 11:12:30.048579 django-selenium-test-1.1.0/tests/tests/
--rw-r--r--   0 twiesing  (1000) users      (100)      167 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/tests/tests/__init__.py
--rw-r--r--   0 twiesing  (1000) users      (100)     8874 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/tests/tests/test_01_core.py
--rw-r--r--   0 twiesing  (1000) users      (100)     4083 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/tests/tests/test_02_integration.py
--rw-r--r--   0 twiesing  (1000) users      (100)      810 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/tests/tests/test_03_user_autologin.py
--rw-r--r--   0 twiesing  (1000) users      (100)      970 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/tests/urls.py
--rw-r--r--   0 twiesing  (1000) users      (100)     1302 2020-08-30 09:46:13.000000 django-selenium-test-1.1.0/tests/views.py
+drwxr-xr-x   0 twiesing   (501) staff       (20)        0 2023-08-05 08:38:10.368674 django-selenium-test-2.0.0/
+-rw-r--r--   0 twiesing   (501) staff       (20)      585 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/CHANGES.txt
+-rw-r--r--   0 twiesing   (501) staff       (20)     1578 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/LICENSE.txt
+-rw-r--r--   0 twiesing   (501) staff       (20)       59 2023-08-02 13:09:30.000000 django-selenium-test-2.0.0/MANIFEST.in
+-rw-r--r--   0 twiesing   (501) staff       (20)    10088 2023-08-05 08:38:10.368739 django-selenium-test-2.0.0/PKG-INFO
+-rw-r--r--   0 twiesing   (501) staff       (20)     9266 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/README.md
+drwxr-xr-x   0 twiesing   (501) staff       (20)        0 2023-08-05 08:38:10.366755 django-selenium-test-2.0.0/django_selenium_test/
+-rw-r--r--   0 twiesing   (501) staff       (20)      106 2023-08-02 13:09:30.000000 django-selenium-test-2.0.0/django_selenium_test/__init__.py
+-rw-r--r--   0 twiesing   (501) staff       (20)    10511 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/django_selenium_test/core.py
+-rw-r--r--   0 twiesing   (501) staff       (20)    17505 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/django_selenium_test/integration.py
+-rw-r--r--   0 twiesing   (501) staff       (20)     1487 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/django_selenium_test/settings.py
+drwxr-xr-x   0 twiesing   (501) staff       (20)        0 2023-08-05 08:38:10.367390 django-selenium-test-2.0.0/django_selenium_test.egg-info/
+-rw-r--r--   0 twiesing   (501) staff       (20)    10088 2023-08-05 08:38:10.000000 django-selenium-test-2.0.0/django_selenium_test.egg-info/PKG-INFO
+-rw-r--r--   0 twiesing   (501) staff       (20)      641 2023-08-05 08:38:10.000000 django-selenium-test-2.0.0/django_selenium_test.egg-info/SOURCES.txt
+-rw-r--r--   0 twiesing   (501) staff       (20)        1 2023-08-05 08:38:10.000000 django-selenium-test-2.0.0/django_selenium_test.egg-info/dependency_links.txt
+-rw-r--r--   0 twiesing   (501) staff       (20)       36 2023-08-05 08:38:10.000000 django-selenium-test-2.0.0/django_selenium_test.egg-info/requires.txt
+-rw-r--r--   0 twiesing   (501) staff       (20)       27 2023-08-05 08:38:10.000000 django-selenium-test-2.0.0/django_selenium_test.egg-info/top_level.txt
+-rw-r--r--   0 twiesing   (501) staff       (20)       81 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/pyproject.toml
+-rw-r--r--   0 twiesing   (501) staff       (20)      874 2023-08-05 08:38:10.369059 django-selenium-test-2.0.0/setup.cfg
+drwxr-xr-x   0 twiesing   (501) staff       (20)        0 2023-08-05 08:38:10.368083 django-selenium-test-2.0.0/tests/
+-rw-r--r--   0 twiesing   (501) staff       (20)        0 2023-08-02 13:09:30.000000 django-selenium-test-2.0.0/tests/__init__.py
+-rw-r--r--   0 twiesing   (501) staff       (20)      218 2023-08-02 13:09:30.000000 django-selenium-test-2.0.0/tests/forms.py
+-rwxr-xr-x   0 twiesing   (501) staff       (20)     1299 2023-08-02 13:09:30.000000 django-selenium-test-2.0.0/tests/manage.py
+-rw-r--r--   0 twiesing   (501) staff       (20)     1320 2023-08-02 13:09:30.000000 django-selenium-test-2.0.0/tests/settings.py
+drwxr-xr-x   0 twiesing   (501) staff       (20)        0 2023-08-05 08:38:10.368561 django-selenium-test-2.0.0/tests/tests/
+-rw-r--r--   0 twiesing   (501) staff       (20)      167 2023-08-02 13:09:30.000000 django-selenium-test-2.0.0/tests/tests/__init__.py
+-rw-r--r--   0 twiesing   (501) staff       (20)     8873 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/tests/tests/test_01_core.py
+-rw-r--r--   0 twiesing   (501) staff       (20)     4076 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/tests/tests/test_02_integration.py
+-rw-r--r--   0 twiesing   (501) staff       (20)      807 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/tests/tests/test_03_user_autologin.py
+-rw-r--r--   0 twiesing   (501) staff       (20)      970 2023-08-02 13:09:30.000000 django-selenium-test-2.0.0/tests/urls.py
+-rw-r--r--   0 twiesing   (501) staff       (20)     1300 2023-08-05 08:37:36.000000 django-selenium-test-2.0.0/tests/views.py
```

### Comparing `django-selenium-test-1.1.0/LICENSE.txt` & `django-selenium-test-2.0.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2020 Tom Wiesing
+Copyright (C) 2020-2023 Tom Wiesing
 
 Copyright (C) 2013-2015 Antonis Christofides
 
 Copyright (C) 2013-2014 Ivan Villanueva, George Vlachos
 
 All rights reserved.
```

### Comparing `django-selenium-test-1.1.0/PKG-INFO` & `django-selenium-test-2.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,324 +1,324 @@
 Metadata-Version: 2.1
 Name: django-selenium-test
-Version: 1.1.0
+Version: 2.0.0
 Summary: Write clean Selenium tests in Django
 Home-page: https://github.com/tkw1536/django_selenium_test
 Author: Tom Wiesing
 Author-email: tkw01536@gmail.com
 License: BSD 3-Clause License
-Description: # django-selenium-test
-        
-        ![CI Status](https://github.com/tkw1536/django_selenium_test/workflows/CI/badge.svg)
-        ![Status](https://img.shields.io/pypi/status/django-selenium-test.svg)
-        [![Latest version](https://img.shields.io/pypi/v/django-selenium-test.svg)](https://pypi.python.org/pypi/django-selenium-test)
-        
-        Write Selenium tests on Django 2.x, Django 3.0, Django 3.1 and Python 3.8. 
-        Based on [django-selenium-clean](https://github.com/aptiko/django-selenium-clean). 
-        
-        This documentation is currently a work-in-progress. 
-        
-        ## Tutorial
-        
-        ### Installation
-        
-        In your virtualenv:
-        
-        ```sh
-        pip install django-selenium-test
-        ```
-        
-        ### Setting up
-        
-        * Create a new django project and app:
-        
-        ```sh
-        django-admin startproject foo
-        cd foo
-        python manage.py startapp bar
-        ```
-        
-        * In ``foo/settings.py``, add ``'bar'`` to ``INSTALLED_APPS``
-        
-        * In ``foo/urls.py``, add ``from bar.views import SimpleView`` to the
-          top, and add ``url(r'^$', SimpleView.as_view())`` to ``urlpatterns``.
-        
-        * Add the SimpleView to ``bar/views.py``:
-        
-        ```python
-        import textwrap
-        
-        from django.http import HttpResponse
-        from django.views.generic.base import View
-        
-        
-        class SimpleView(View):
-        
-            def dispatch(request, *args, **kwargs):
-                response_text = textwrap.dedent('''\
-                    <html>
-                    <head>
-                    <title>Greetings to the world</title>
-                    </head>
-                    <body>
-                    <h1 id="earth">Greetings to earth</h1>
-                    <h1 id="world" style="display: none;">Hello, world!</h1>
-        
-                    <p>We have some javascript here so that when you click the button
-                        the heading above toggles between "Greetings to earth" and
-                        "Hello, world!".</p>
-        
-                    <button onclick="toggle()">Toggle</button>
-        
-                    <script type="text/javascript">
-                        toggle = function () {
-                            var heading_earth = document.getElementById("earth");
-                            var heading_world = document.getElementById("world");
-                            if (heading_earth.style.display == 'none') {
-                                heading_world.style.display = 'none';
-                                heading_earth.style.display = 'block';
-                            } else {
-                                heading_earth.style.display = 'none';
-                                heading_world.style.display = 'block';
-                            }
-                        }
-                    </script>
-                    </body>
-                    </html>
-                ''')
-                return HttpResponse(response_text)
-        ```
-        
-        We're done setting up. If you now run ``python manage.py runserver``
-        in your browser and visit http://localhost:8000/ in your browser, you
-        should see the simple page. Let's now proceed to write a test for it.
-        
-        ### Writing the test
-        
-        Modify ``bar/tests.py`` so that it has the following contents:
-        
-        ```python
-        from unittest import skipUnless
-        
-        from django.conf import settings
-        
-        from django_selenium_test import selenium, SeleniumTestCase, PageElement
-        from selenium.webdriver.common.by import By
-        
-        
-        @skipUnless(getattr(settings, 'SELENIUM_WEBDRIVERS', False),
-                    "Selenium is unconfigured")
-        class HelloTestCase(SeleniumTestCase):
-        
-            heading_earth = PageElement(By.ID, 'earth')
-            heading_world = PageElement(By.ID, 'world')
-            button = PageElement(By.CSS_SELECTOR, 'button')
-        
-            def test_toggle(self):
-                # Visit the page
-                self.selenium.get(self.live_server_url)
-        
-                # Check that the earth heading is visible
-                self.assertTrue(self.heading_earth.is_displayed())
-                self.assertFalse(self.heading_world.is_displayed())
-        
-                # Toggle and check the new condition
-                self.button.click()
-                self.heading_world.wait_until_is_displayed()
-                self.assertFalse(self.heading_earth.is_displayed())
-                self.assertTrue(self.heading_world.is_displayed())
-        
-                # Toggle again and re-check
-                self.button.click()
-                self.heading_earth.wait_until_is_displayed()
-                self.assertTrue(self.heading_earth.is_displayed())
-                self.assertFalse(self.heading_world.is_displayed())
-        ```
-        
-        ### Executing the test
-        
-        Try ``python manage.py test`` and it will skip the test because
-        selenium is unconfigured. You need to configure it by specifying
-        ``SELENIUM_WEBDRIVERS`` in ``foo/settings.py``:
-        
-        ```python
-        from django_selenium_test.settings import make_chrome_driver
-        
-        SELENIUM_WEBDRIVERS = {
-            'default': make_chrome_driver([], {}),
-        }
-        ```
-        
-        Now try again, and it should execute the test. 
-        
-        ### Advanced test running tricks
-        
-        #### Executing a test in many widths
-        
-        Add this to your ``foo/settings.py``:
-        
-        ```python
-        SELENIUM_WIDTHS = [1024, 800, 350]
-        ```
-        
-        This will result in executing all ``SeleniumTestCase``'s three times,
-        one for each specified browser width. Useful for responsive designs.
-        The default is to run them on only one width, 1024.
-        
-        #### Using many selenium drivers
-        
-        You can have many ``SELENIUM_WEBDRIVERS``:
-        
-        ```python
-        from django_selenium_test.settings import make_chrome_driver, make_firefox_driver
-        SELENIUM_WEBDRIVERS = {
-            'default': make_chrome_driver([], {})
-            'firefox': make_firefox_driver([], {})
-        }
-        ```
-        
-        By default, the ``default`` one is used. You can specify another using
-        the ``SELENIUM_WEBDRIVER`` environment variable:
-        
-        ```sh
-        SELENIUM_WEBDRIVER=firefox python manage.py test
-        ```
-        
-        
-        #### Running a headless browser
-        
-        It can be very useful to run the selenium tests with a headless
-        browser, that is, in an invisible browser window. For one thing, it
-        is much faster. 
-        
-        To achieve this, pass headless=True to the make_BRAND_driver() function:
-        
-        ```python
-        from django_selenium_test.settings import make_chrome_driver, make_firefox_driver
-        SELENIUM_WEBDRIVERS = {
-            'default': make_chrome_driver([], {}, headless=True)
-            'firefox': make_firefox_driver([], {}, headless=True)
-        }
-        ```
-        
-        #### Using advanced integration tests
-        
-        (Currently undocumented)
-        
-        
-        ## Reference
-        
-        ### SeleniumTestCase objects
-        
-        .. code:: python
-        
-           from django_selenium_test import SeleniumTestCase
-        
-        ``SeleniumTestCase`` is the same as Django's
-        ``StaticLiveServerTestCase`` but it adds a little bit of Selenium
-        functionality. Derive your Selenium tests from this class instead of
-        ``StaticLiveServerTestCase``.
-        
-        The most important feature of ``SeleniumTestCase`` is the ``selenium``
-        attribute.  Technically it is a wrapper around the selenium driver. In
-        practice, you can think about it as the browser, or as the equivalent
-        of Django's test client. It has all `selenium driver attributes and
-        methods`_, but you will mostly use ``get()``. It also has the
-        following additional methods:
-        
-        * ``self.selenium.login(**credentials)``,
-        ``self.selenium.force_login(user, base_url)``,
-        ``self.selenium.logout()``
-        
-          Similar to the Django test client ``login()``, ``force_login()`` and
-          ``logout()`` methods.  ``login()`` returns ``True`` if login is
-          possible; ``False`` if the provided credentials are incorrect, or the
-          user is inactive, or if the sessions framework is not available.
-        
-          The `force_login()` code was adapted from [django-selenium-login](https://github.com/feffe/django-selenium-login/blob/master/seleniumlogin/__init__.py),
-          which is licensed under the MIT License. 
-        
-        * ``self.selenium.wait_until_n_windows(n, timeout=2)``
-        
-          Useful when a Javascript action has caused the browser to open
-          another window. The typical usage is this:
-        
-        ```python
-        button_that_will_open_a_second_window.click()
-        self.selenium.wait_until_n_windows(n=2, timeout=10)
-        windows = self.selenium.window_handles
-        self.selenium.switch_to.window(windows[1])
-        # continue testing
-        ```
-        
-          If the timeout (in seconds) elapses and the number of browser
-          windows never becomes ``n``, an ``AssertionError`` is raised.
-        
-        - [selenium driver attributes and methods](http://selenium-python.readthedocs.org/api.html#module-selenium.webdriver.remote.webdriver)
-        
-        PageElement objects
-        -------------------
-        
-        ```python
-        from django_selenium_test import PageElement
-        ```
-        
-        ``PageElement`` is a lazy wrapper around WebElement_; it has all its
-        properties and methods. It is initialized with a locator_, but the
-        element is not actually located until needed. In addition to
-        WebElement_ properties and methods, it has these:
-        
-        * ``PageElement.exists()``: Returns True if the element can be located.
-        
-        * ``PageElement.wait_until_exists(timeout=10)``
-        
-          ``PageElement.wait_until_not_exists(timeout=10)``
-        
-          ``PageElement.wait_until_is_displayed(timeout=10)``
-        
-          ``PageElement.wait_until_not_displayed(timeout=10)``
-        
-          ``PageElement.wait_until_contains(text, timeout=10)``
-        
-          ``PageElement.wait_until_not_contains(text, timeout=10)``
-        
-          What these methods do should be self-explanatory from their name. The
-          ones ending in ``contains`` refer to whether the element contains the
-          specified text.  The methods raise an exception if there is a timeout.
-        
-        - [WebElement](http://selenium-python.readthedocs.org/api.html#module-selenium.webdriver.remote.webelement)
-        - [locator](http://selenium-python.readthedocs.org/api.html#locate-elements-by)
-        
-        ### IntegrationTest objects
-        (Currently undocumented)
-        
-        ### Running django-selenium-test's own unit tests
-        
-        By default the unit tests will use Chrome::
-        
-        ```sh
-        ./setup.py test
-        ```
-        
-        Use the ``SELENIUM_BROWSER`` environment variable to use another browser:
-        
-        ```sh
-        SELENIUM_BROWSER=firefox ./setup.py test
-        ```
-        
-        ## License
-        
-        Licensed under the BSD 3-clause license; see `LICENSE.txt` for details.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# django-selenium-test
+
+![CI Status](https://github.com/tkw1536/django_selenium_test/workflows/CI/badge.svg)
+![Status](https://img.shields.io/pypi/status/django-selenium-test.svg)
+[![Latest version](https://img.shields.io/pypi/v/django-selenium-test.svg)](https://pypi.python.org/pypi/django-selenium-test)
+
+Write Selenium tests on Django 3.2, Django 4.0, Django 3.1 and Python 3.8+. 
+Based on [django-selenium-clean](https://github.com/aptiko/django-selenium-clean). 
+
+This documentation is currently a work-in-progress. 
+
+## Tutorial
+
+### Installation
+
+In your virtualenv:
+
+```sh
+pip install django-selenium-test
+```
+
+### Setting up
+
+* Create a new django project and app:
+
+```sh
+django-admin startproject foo
+cd foo
+python manage.py startapp bar
+```
+
+* In ``foo/settings.py``, add ``'bar'`` to ``INSTALLED_APPS``
+
+* In ``foo/urls.py``, add ``from bar.views import SimpleView`` to the
+  top, and add ``url(r'^$', SimpleView.as_view())`` to ``urlpatterns``.
+
+* Add the SimpleView to ``bar/views.py``:
+
+```python
+import textwrap
+
+from django.http import HttpResponse
+from django.views.generic.base import View
+
+
+class SimpleView(View):
+
+    def dispatch(request, *args, **kwargs):
+        response_text = textwrap.dedent('''\
+            <html>
+            <head>
+            <title>Greetings to the world</title>
+            </head>
+            <body>
+            <h1 id="earth">Greetings to earth</h1>
+            <h1 id="world" style="display: none;">Hello, world!</h1>
+
+            <p>We have some javascript here so that when you click the button
+                the heading above toggles between "Greetings to earth" and
+                "Hello, world!".</p>
+
+            <button onclick="toggle()">Toggle</button>
+
+            <script type="text/javascript">
+                toggle = function () {
+                    var heading_earth = document.getElementById("earth");
+                    var heading_world = document.getElementById("world");
+                    if (heading_earth.style.display == 'none') {
+                        heading_world.style.display = 'none';
+                        heading_earth.style.display = 'block';
+                    } else {
+                        heading_earth.style.display = 'none';
+                        heading_world.style.display = 'block';
+                    }
+                }
+            </script>
+            </body>
+            </html>
+        ''')
+        return HttpResponse(response_text)
+```
+
+We're done setting up. If you now run ``python manage.py runserver``
+in your browser and visit http://localhost:8000/ in your browser, you
+should see the simple page. Let's now proceed to write a test for it.
+
+### Writing the test
+
+Modify ``bar/tests.py`` so that it has the following contents:
+
+```python
+from unittest import skipUnless
+
+from django.conf import settings
+
+from django_selenium_test import selenium, SeleniumTestCase, PageElement
+from selenium.webdriver.common.by import By
+
+
+@skipUnless(getattr(settings, 'SELENIUM_WEBDRIVERS', False),
+            "Selenium is unconfigured")
+class HelloTestCase(SeleniumTestCase):
+
+    heading_earth = PageElement(By.ID, 'earth')
+    heading_world = PageElement(By.ID, 'world')
+    button = PageElement(By.CSS_SELECTOR, 'button')
+
+    def test_toggle(self):
+        # Visit the page
+        self.selenium.get(self.live_server_url)
+
+        # Check that the earth heading is visible
+        self.assertTrue(self.heading_earth.is_displayed())
+        self.assertFalse(self.heading_world.is_displayed())
+
+        # Toggle and check the new condition
+        self.button.click()
+        self.heading_world.wait_until_is_displayed()
+        self.assertFalse(self.heading_earth.is_displayed())
+        self.assertTrue(self.heading_world.is_displayed())
+
+        # Toggle again and re-check
+        self.button.click()
+        self.heading_earth.wait_until_is_displayed()
+        self.assertTrue(self.heading_earth.is_displayed())
+        self.assertFalse(self.heading_world.is_displayed())
+```
+
+### Executing the test
+
+Try ``python manage.py test`` and it will skip the test because
+selenium is unconfigured. You need to configure it by specifying
+``SELENIUM_WEBDRIVERS`` in ``foo/settings.py``:
+
+```python
+from django_selenium_test.settings import make_chrome_driver
+
+SELENIUM_WEBDRIVERS = {
+    'default': make_chrome_driver([], {}),
+}
+```
+
+Now try again, and it should execute the test. 
+
+### Advanced test running tricks
+
+#### Executing a test in many widths
+
+Add this to your ``foo/settings.py``:
+
+```python
+SELENIUM_WIDTHS = [1024, 800, 350]
+```
+
+This will result in executing all ``SeleniumTestCase``'s three times,
+one for each specified browser width. Useful for responsive designs.
+The default is to run them on only one width, 1024.
+
+#### Using many selenium drivers
+
+You can have many ``SELENIUM_WEBDRIVERS``:
+
+```python
+from django_selenium_test.settings import make_chrome_driver, make_firefox_driver
+SELENIUM_WEBDRIVERS = {
+    'default': make_chrome_driver([], {})
+    'firefox': make_firefox_driver([], {})
+}
+```
+
+By default, the ``default`` one is used. You can specify another using
+the ``SELENIUM_WEBDRIVER`` environment variable:
+
+```sh
+SELENIUM_WEBDRIVER=firefox python manage.py test
+```
+
+
+#### Running a headless browser
+
+It can be very useful to run the selenium tests with a headless
+browser, that is, in an invisible browser window. For one thing, it
+is much faster. 
+
+To achieve this, pass headless=True to the make_BRAND_driver() function:
+
+```python
+from django_selenium_test.settings import make_chrome_driver, make_firefox_driver
+SELENIUM_WEBDRIVERS = {
+    'default': make_chrome_driver([], {}, headless=True)
+    'firefox': make_firefox_driver([], {}, headless=True)
+}
+```
+
+#### Using advanced integration tests
+
+(Currently undocumented)
+
+
+## Reference
+
+### SeleniumTestCase objects
+
+.. code:: python
+
+   from django_selenium_test import SeleniumTestCase
+
+``SeleniumTestCase`` is the same as Django's
+``StaticLiveServerTestCase`` but it adds a little bit of Selenium
+functionality. Derive your Selenium tests from this class instead of
+``StaticLiveServerTestCase``.
+
+The most important feature of ``SeleniumTestCase`` is the ``selenium``
+attribute.  Technically it is a wrapper around the selenium driver. In
+practice, you can think about it as the browser, or as the equivalent
+of Django's test client. It has all `selenium driver attributes and
+methods`_, but you will mostly use ``get()``. It also has the
+following additional methods:
+
+* ``self.selenium.login(**credentials)``,
+``self.selenium.force_login(user, base_url)``,
+``self.selenium.logout()``
+
+  Similar to the Django test client ``login()``, ``force_login()`` and
+  ``logout()`` methods.  ``login()`` returns ``True`` if login is
+  possible; ``False`` if the provided credentials are incorrect, or the
+  user is inactive, or if the sessions framework is not available.
+
+  The `force_login()` code was adapted from [django-selenium-login](https://github.com/feffe/django-selenium-login/blob/master/seleniumlogin/__init__.py),
+  which is licensed under the MIT License. 
+
+* ``self.selenium.wait_until_n_windows(n, timeout=2)``
+
+  Useful when a Javascript action has caused the browser to open
+  another window. The typical usage is this:
+
+```python
+button_that_will_open_a_second_window.click()
+self.selenium.wait_until_n_windows(n=2, timeout=10)
+windows = self.selenium.window_handles
+self.selenium.switch_to.window(windows[1])
+# continue testing
+```
+
+  If the timeout (in seconds) elapses and the number of browser
+  windows never becomes ``n``, an ``AssertionError`` is raised.
+
+- [selenium driver attributes and methods](http://selenium-python.readthedocs.org/api.html#module-selenium.webdriver.remote.webdriver)
+
+PageElement objects
+-------------------
+
+```python
+from django_selenium_test import PageElement
+```
+
+``PageElement`` is a lazy wrapper around WebElement_; it has all its
+properties and methods. It is initialized with a locator_, but the
+element is not actually located until needed. In addition to
+WebElement_ properties and methods, it has these:
+
+* ``PageElement.exists()``: Returns True if the element can be located.
+
+* ``PageElement.wait_until_exists(timeout=10)``
+
+  ``PageElement.wait_until_not_exists(timeout=10)``
+
+  ``PageElement.wait_until_is_displayed(timeout=10)``
+
+  ``PageElement.wait_until_not_displayed(timeout=10)``
+
+  ``PageElement.wait_until_contains(text, timeout=10)``
+
+  ``PageElement.wait_until_not_contains(text, timeout=10)``
+
+  What these methods do should be self-explanatory from their name. The
+  ones ending in ``contains`` refer to whether the element contains the
+  specified text.  The methods raise an exception if there is a timeout.
+
+- [WebElement](http://selenium-python.readthedocs.org/api.html#module-selenium.webdriver.remote.webelement)
+- [locator](http://selenium-python.readthedocs.org/api.html#locate-elements-by)
+
+### IntegrationTest objects
+(Currently undocumented)
+
+### Running django-selenium-test's own unit tests
+
+By default the unit tests will use Chrome::
+
+```sh
+./setup.py test
+```
+
+Use the ``SELENIUM_BROWSER`` environment variable to use another browser:
+
+```sh
+SELENIUM_BROWSER=firefox ./setup.py test
+```
+
+## License
+
+Licensed under the BSD 3-clause license; see `LICENSE.txt` for details.
```

### Comparing `django-selenium-test-1.1.0/README.md` & `django-selenium-test-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # django-selenium-test
 
 ![CI Status](https://github.com/tkw1536/django_selenium_test/workflows/CI/badge.svg)
 ![Status](https://img.shields.io/pypi/status/django-selenium-test.svg)
 [![Latest version](https://img.shields.io/pypi/v/django-selenium-test.svg)](https://pypi.python.org/pypi/django-selenium-test)
 
-Write Selenium tests on Django 2.x, Django 3.0, Django 3.1 and Python 3.8. 
+Write Selenium tests on Django 3.2, Django 4.0, Django 3.1 and Python 3.8+. 
 Based on [django-selenium-clean](https://github.com/aptiko/django-selenium-clean). 
 
 This documentation is currently a work-in-progress. 
 
 ## Tutorial
 
 ### Installation
```

### Comparing `django-selenium-test-1.1.0/django_selenium_test/core.py` & `django-selenium-test-2.0.0/django_selenium_test/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,46 +20,62 @@
     from django.contrib.auth.models import AbstractUser
 
     from selenium.webdriver.remote.webdriver import WebDriver
 
 
 class SeleniumWrapper(object):
     _instance = None
+    _init_done = None
+    _init_except = None  # was there an error while initializing?
     driver: WebDriver
 
     def __new__(cls, *args: Any, **kwargs: Any) -> SeleniumWrapper:
-        if not cls._instance:
-            cls._instance = super().__new__(cls, *args, **kwargs)
+        # if we aren't yet initialized, do it!
+        if not cls._init_done:
+            try:
+                cls._instance = super().__new__(cls, *args, **kwargs)
+            except Exception as e:
+                cls._init_except = e
+            cls._init_done = True
+
+        # if some error occurred, raise it!
+        if cls._init_except is not None:
+            raise cls._init_except
+
+        # return the instance
         return cls._instance
 
     def __init__(self) -> None:
         SELENIUM_WEBDRIVERS = getattr(settings, "SELENIUM_WEBDRIVERS", {})
         if not SELENIUM_WEBDRIVERS:
             return
         driver_id = os.environ.get("SELENIUM_WEBDRIVER", "default")
         driver = SELENIUM_WEBDRIVERS[driver_id]
         callable = driver["callable"]
         args = driver["args"]
         kwargs = driver["kwargs"]
         self.driver = callable(*args, **kwargs)
 
     def __getattr__(self, name: str) -> Any:
+        # always natively get the driver attribute!
+        if name == "driver":
+            return getattr(super(), name)
+
         return getattr(self.driver, name)
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name == "driver":
-            super(SeleniumWrapper, self).__setattr__(name, value)
-        else:
-            setattr(self.driver, name, value)
+            super().__setattr__(name, value)
+            return
+
+        setattr(self.driver, name, value)
 
     def __bool__(self) -> bool:
         return bool(self.driver)
 
-    __nonzero__ = __bool__  # Python 2 compatibility
-
     def login(self, **credentials: Any) -> bool:
         """
         Sets selenium to appear as if a user has successfully signed in.
 
         Returns True if signin is possible; False if the provided
         credentials are incorrect, or the user is inactive, or if the
         sessions framework is not available.
@@ -85,15 +101,15 @@
 
         The user will have its backend attribute set to the value of the
         backend argument (which should be a dotted Python path string),
         or to settings.AUTHENTICATION_BACKENDS[0] if a value isn't
         provided. The authenticate() function called by login() normally
         annotates the user like this.
 
-        The code is based on https://github.com/feffe/django-selenium-login/blob/master/seleniumlogin/__init__.py. 
+        The code is based on https://github.com/feffe/django-selenium-login/blob/master/seleniumlogin/__init__.py.
         """
 
         # The original code was licensed under:
         #
         #
         # MIT License
         #
@@ -195,16 +211,15 @@
 
 
 class SeleniumTestCase(StaticLiveServerTestCase):
     selenium: SeleniumWrapper
 
     @classmethod
     def setUpClass(cls) -> None:
-
-        super(SeleniumTestCase, cls).setUpClass()
+        super().setUpClass()
         cls.selenium = SeleniumWrapper()
         PageElement.selenium = cls.selenium
 
         # Normally we would just do something like
         #     selenium.live_server_url = self.live_server_url
         # However, there is no "self" at this time, so we
         # essentially duplicate the code from the definition of
@@ -212,28 +227,26 @@
         cls.selenium.live_server_url = "http://%s:%s" % (
             cls.server_thread.host,
             cls.server_thread.port,
         )
 
     @classmethod
     def tearDownClass(cls) -> None:
-
         cls.selenium.quit()
         PageElement.selenium = None
         super().tearDownClass()
 
     def __call__(self, result=None):
         if hasattr(self, "selenium"):
             for width in getattr(settings, "SELENIUM_WIDTHS", [1024]):
                 self.selenium.set_window_size(width, 1024)
         return super().__call__(result)
 
 
 class PageElement(object):
-
     selenium: Optional[WebDriver] = None
 
     def __init__(self, *args: Any) -> None:
         if len(args) == 2:
             self.locator = args
 
     def wait_until_exists(self, timeout: int = 10) -> None:
```

### Comparing `django-selenium-test-1.1.0/django_selenium_test/integration.py` & `django-selenium-test-2.0.0/django_selenium_test/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     from django.contrib.auth.models import User
 
     from django_selenium_clean import SeleniumWrapper
     from selenium.webdriver.remote.webelement import WebElement
 
 
 class DummyTestBase:
-    """ A dummy base class for type-hinting within integration tests """
+    """A dummy base class for type-hinting within integration tests"""
 
     selenium: SeleniumWrapper
     live_server_url: str
 
     def assertTrue(self, expr: bool, msg: Optional[str] = None) -> None:
         ...
 
@@ -48,15 +48,15 @@
 class ElementFindMixins(DummyTestBase):
     find_element_timeout: int
     find_element_selector: str
 
     def find_element(
         self, selector: str, timeout: Optional[int] = None, clickable: bool = False
     ) -> WebElement:
-        """ Finds an element by a selector and waits for it to become available """
+        """Finds an element by a selector and waits for it to become available"""
 
         if timeout is None:
             timeout = self.__class__.find_element_timeout
         if selector is None:
             if self.__class__.find_element_selector is None:
                 raise Exception("find_element_selector may not be None")
             selector = self.__class__.find_element_selector
@@ -67,46 +67,46 @@
             condition = expected_conditions.element_to_be_clickable
         else:
             condition = expected_conditions.visibility_of_element_located
 
         return wait.until(condition((By.CSS_SELECTOR, selector)))
 
     def find_next_sibling(self, element: WebElement) -> Optional[WebElement]:
-        """ Finds the next sibling of an element """
+        """Finds the next sibling of an element"""
         return self.selenium.execute_script(
             "return arguments[0].nextElementSibling; ", element
         )
 
 
 class ElementAssertionMixins(DummyTestBase):
     def _element_exists(self, selector: str) -> bool:
-        """ Checks if an element with the given selector exists on the page """
+        """Checks if an element with the given selector exists on the page"""
         return len(self.selenium.find_elements(By.CSS_SELECTOR, selector)) > 0
 
     def _element_displayed(self, selector: str) -> bool:
-        """ Checks if an element with a given selector exists and is displayed """
+        """Checks if an element with a given selector exists and is displayed"""
 
         for element in self.selenium.find_elements(By.CSS_SELECTOR, selector):
             return element.is_displayed()
         return False
 
     def assert_element_exists(self, selector: str, *args: Any) -> None:
-        """ Asserts that an element exists on the current page """
+        """Asserts that an element exists on the current page"""
         return self.assertTrue(self._element_exists(selector), *args)
 
     def assert_element_not_exists(self, selector: str, *args: Any) -> None:
-        """ Asserts that an element does not exist on the current page """
+        """Asserts that an element does not exist on the current page"""
         return self.assertFalse(self._element_exists(selector), *args)
 
     def assert_element_displayed(self, selector: str, *args: Any) -> None:
-        """ Asserts that an element with the given selector is displayed """
+        """Asserts that an element with the given selector is displayed"""
         return self.assertTrue(self._element_displayed(selector), *args)
 
     def assert_element_not_displayed(self, selector: str, *args: Any) -> None:
-        """ Asserts that an element with the given selector is not displayed """
+        """Asserts that an element with the given selector is not displayed"""
         return self.assertFalse(self._element_displayed(selector), *args)
 
 
 class FormElementMixins(DummyTestBase):
     def fill_out_form(
         self,
         url_pattern: str,
@@ -118,23 +118,23 @@
         selector: Optional[str] = None,
         url_args: Optional[List[str]] = None,
         url_kwargs: Optional[Dict[str, Any]] = None,
         url_reverse_get_params: Optional[Dict[str, Any]] = None,
         selector_timeout: Optional[int] = None,
     ) -> WebElement:
         """
-            Loads a URL using selenium from the live server and waits for the element with the submit_button id to be
-            available.
-            Once available, uses send_keys to send strings to elements with ids as specificed by send_form_keys dict.
-            Next, selects either one item by visible text, or muliple items by value, in dropdowns specified by the
-            select_dropdowns element.
-            Next, sets the selection state of checkboxes of elements with ids as specified by the select_checkboxes
-            dict.
-            Next, directly set the value attribute of elements refered to by the script_value dict.
-            Finally returns the button element.
+        Loads a URL using selenium from the live server and waits for the element with the submit_button id to be
+        available.
+        Once available, uses send_keys to send strings to elements with ids as specificed by send_form_keys dict.
+        Next, selects either one item by visible text, or muliple items by value, in dropdowns specified by the
+        select_dropdowns element.
+        Next, sets the selection state of checkboxes of elements with ids as specified by the select_checkboxes
+        dict.
+        Next, directly set the value attribute of elements refered to by the script_value dict.
+        Finally returns the button element.
         """
         if submit_button is None:
             selector = None
         else:
             selector = "#{}".format(submit_button)
 
         # get the element on the page
@@ -147,34 +147,34 @@
             selector_timeout=selector_timeout,
             selector_clickable=True,
         )
 
         # send_keys to the specified form elements
         if send_form_keys is not None:
             for id_, value in send_form_keys.items():
-                element = self.selenium.find_element_by_id(id_)
+                element = self.selenium.find_element(By.ID, id_)
                 element.clear()
                 element.send_keys(value)
 
         # select inside the specified dropdowns
         if select_dropdowns is not None:
             for id_, value in select_dropdowns.items():
                 self.select_dropdown(id_, value)
 
         # select the checkboxes
         if select_checkboxes is not None:
             for id_, value in select_checkboxes.items():
-                checkbox = self.selenium.find_element_by_id(id_)
+                checkbox = self.selenium.find_element(By.ID, id_)
                 if checkbox.is_selected() != value:
                     checkbox.click()
 
         # set the scripted values
         if script_value is not None:
             for id_, value in script_value.items():
-                element = self.selenium.find_element_by_id(id_)
+                element = self.selenium.find_element(By.ID, id_)
 
                 self.selenium.execute_script(
                     # update the value in the DOM
                     "arguments[0].value = arguments[1];" +
                     # tell input event handlers this happened
                     "arguments[0].dispatchEvent(new Event('input',{bubbles: true,cancelable: true}));"
                     +
@@ -188,17 +188,17 @@
         return button
 
     def submit_form(
         self,
         *args: Any,
         next_selector: Optional[str] = None,
         selector_timeout: Optional[int] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> WebElement:
-        """ Fills out and submit a form, then returns the body element of the submitted page """
+        """Fills out and submit a form, then returns the body element of the submitted page"""
 
         # fill out the form and click the submit button
         button = self.fill_out_form(*args, selector_timeout=selector_timeout, **kwargs)
         button.click()
 
         # wait for next element to be visible
         return self.find_element(next_selector, timeout=selector_timeout)
@@ -214,17 +214,18 @@
         for (var i = 0; i < selects.length; i++) {
             selects[i].removeAttribute('required');
         }
         """
         )
 
     def __intercept_xhr(self, code: str, *args: Any) -> [bool, IO[bytes]]:
-        """ Creates and then executes a script that
-        programatically intercepts the provided file download. 
-        'code' should be a javascript code calling init_xhr_intercept() with appropriate functions. """
+        """Creates and then executes a script that
+        programatically intercepts the provided file download.
+        'code' should be a javascript code calling init_xhr_intercept() with appropriate functions.
+        """
 
         self.selenium.execute_script(
             """
 window.xhr_done = false;
 window.xhr_ok = null;
 window.xhr_data = null;
 
@@ -242,15 +243,15 @@
         reader.readAsDataURL(xhr.response);
     };
 
     callback(xhr);
     return xhr;
 }"""
             + code,
-            *args
+            *args,
         )
 
         xhr_done = False
         while xhr_done == False:
             xhr_done = self.selenium.execute_script("return window.xhr_done;")
             time.sleep(0.1)
 
@@ -268,57 +269,56 @@
         self,
         url: str,
         args: Optional[List[Any]] = None,
         kwargs: Optional[Dict[str, Any]] = None,
         get_params: Option[Dict[str, str]] = None,
         reverse_get_params: Optional[Dict[str, Any]] = None,
     ) -> [bool, IO[bytes]]:
-
         return self.__intercept_xhr(
             """
             var url = arguments[0];
             init_xhr_intercept(function(xhr){
                 xhr.open('GET', url);
                 xhr.send(null);
             });
         """,
             self._resolve_url(url, args, kwargs, get_params, reverse_get_params),
         )
 
     def get_form_download(self, form: WebElement) -> [bool, IO[bytes]]:
-        """ Virtually submits a form and intercepts the resulting downloaded file as a BytesIO """
+        """Virtually submits a form and intercepts the resulting downloaded file as a BytesIO"""
         return self.__intercept_xhr(
             """
             var form = arguments[0].form;
             init_xhr_intercept(function(xhr){
                 var fd = new FormData(form);
                 xhr.open('POST', form.getAttribute('action') || window.location.href);
                 xhr.send(fd);
             });
         """,
             form,
         )
 
     def hover_element(self, id_: str) -> WebElement:
-        """ Hovers over an element with the given ID """
-        element = self.selenium.find_element_by_id(id_)
+        """Hovers over an element with the given ID"""
+        element = self.selenium.find_element(By.ID, id_)
 
         hover = ActionChains(self.selenium).move_to_element(element)
         hover.perform()
 
         return element
 
     def select_dropdown(
         self, id_or_element: Union[str, WebElement], value: str
     ) -> Select:
-        """ Selects text of a dropdown by value """
+        """Selects text of a dropdown by value"""
 
         # if we don't have an element, select it by selector
         if isinstance(id_or_element, str):
-            id_or_element = self.selenium.find_element_by_id(id_or_element)
+            id_or_element = self.selenium.find_element(By.ID, id_or_element)
 
         select = Select(id_or_element)
 
         # if we are a multiple select, deselect all of them
         if select.is_multiple:
             select.deselect_all()
 
@@ -343,15 +343,15 @@
         self,
         url: str,
         args: Optional[List[Any]] = None,
         kwargs: Optional[Dict[str, Any]] = None,
         get_params: Option[Dict[str, str]] = None,
         reverse_get_params: Optional[Dict[str, Any]] = None,
     ) -> str:
-        """ Resolves a url pattern into an actual url """
+        """Resolves a url pattern into an actual url"""
 
         # If it's an absolute url, the test case is wrong
         if url.startswith("/"):
             raise AssertionError(
                 "_resolve_url() does not accept absolute urls, got: {}".format(url)
             )
 
@@ -366,15 +366,15 @@
         if get_params is not None:
             has_extra_args = True
             extra_args.update(get_params)
 
         # reversed get params
         if reverse_get_params is not None:
             has_extra_args = True
-            for (k, v) in reverse_get_params.items():
+            for k, v in reverse_get_params.items():
                 extra_args[k] = reverse(v)
 
         # if we had some extra arguments
         if has_extra_args:
             resolved = (
                 resolved
                 + "?"
@@ -382,15 +382,15 @@
             )
 
         # and return the resolved url
         return resolved
 
     @property
     def _current_url(self) -> str:
-        """ The current url of the server relative to the root """
+        """The current url of the server relative to the root"""
 
         url = str(self.selenium.current_url)
         if url.startswith(self.live_server_url):
             return url[len(self.live_server_url) :]
         return url
 
     def load_live_url(
@@ -401,16 +401,16 @@
         url_kwargs: Optional[Dict[str, Any]] = None,
         url_get_params: Option[Dict[str, str]] = None,
         url_reverse_get_params: Optional[Dict[str, Any]] = None,
         selector_timeout: Optional[int] = None,
         selector_clickable: bool = False,
     ) -> WebElement:
         """
-            Loads an url from the selenium from the live server and waits for the CSS selector (if any) to be available
-            Returns the element selected, None if none is selected, or raises TimeoutException if a timeout occurs.
+        Loads an url from the selenium from the live server and waits for the CSS selector (if any) to be available
+        Returns the element selected, None if none is selected, or raises TimeoutException if a timeout occurs.
         """
 
         # resolve the url and load it
         url = self._resolve_url(
             url_pattern,
             args=url_args,
             kwargs=url_kwargs,
@@ -421,15 +421,15 @@
 
         # wait for the element
         return self.find_element(
             selector, timeout=selector_timeout, clickable=selector_clickable
         )
 
     def assert_url_equal(self, url: str, *args: Any, **kwargs: Any) -> None:
-        """ Asserts that the current url is equal to the (pontially resolvable) url """
+        """Asserts that the current url is equal to the (pontially resolvable) url"""
 
         got = self._current_url
         expected = self._resolve_url(url, **kwargs)
         return self.assertEqual(got, expected, *args)
 
     def assert_url_follow(
         self,
@@ -439,18 +439,18 @@
         url_args=None,
         url_kwargs=None,
         url_reverse_get_params=None,
         new_url_args=None,
         new_url_kwargs=None,
         new_url_reverse_get_params=None,
         url_selector: str = None,
-        url_selector_timeout: int = None
+        url_selector_timeout: int = None,
     ):
         """
-            Asserts that loading url (with selector selector) in the browser redirects to new_url. 
+        Asserts that loading url (with selector selector) in the browser redirects to new_url.
         """
 
         # load the url
         self.load_live_url(
             url,
             url_args=url_args,
             url_kwargs=url_kwargs,
@@ -461,52 +461,52 @@
 
         # and check that it's equal
         return self.assert_url_equal(
             new_url,
             args=new_url_args,
             kwargs=new_url_kwargs,
             reverse_get_params=new_url_reverse_get_params,
-            *args
+            *args,
         )
 
 
 class IntegrationTestBase(
     ElementAssertionMixins,
     ElementFindMixins,
     FormElementMixins,
     URLMixins,
     DummyTestBase,
 ):
-    """ A base class for integration tests """
+    """A base class for integration tests"""
 
     user: Optional[User] = None
     selenium: SeleniumWrapper = None
     live_server_url: str = None
 
     find_element_timeout: int = 10
     find_element_selector: str  # to be overwritten by subclass
 
     def login(self, username: str) -> User:
-        """ Authenticates the user with the given username and returns the user object """
+        """Authenticates the user with the given username and returns the user object"""
 
         # grab the instance of the user we want to login
         user = get_user_model().objects.get(username=username)
 
         # and force the login
         self.selenium.force_login(user, base_url=self.live_server_url)
 
         # return the user
         return user
 
 
 class IntegrationTest(SeleniumTestCase, IntegrationTestBase):
-    """ An integration test base class using Selenium """
+    """An integration test base class using Selenium"""
 
     def setUp(self) -> None:
-        """ Setups up this test class """
+        """Setups up this test class"""
 
         # before each test case, we need to reset the cookies
         self.selenium.delete_all_cookies()
 
         user = self.__class__.user
         if user is not None:
             self.user = self.login(user)  # type: User
```

### Comparing `django-selenium-test-1.1.0/django_selenium_test/settings.py` & `django-selenium-test-2.0.0/django_selenium_test/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,44 +9,44 @@
 if TYPE_CHECKING:
     from typing import Any, Dict, List
 
 
 def make_chrome_driver(
     args: List[Any], kwargs: Dict[str, Any], headless=False
 ) -> Dict[str, Any]:
-    """ Makes a new chrome driver settings instance """
+    """Makes a new chrome driver settings instance"""
     kwargs.update({"options": _make_chrome_options(headless)})
 
     return {
         "callable": webdriver.Chrome,
         "args": args,
         "kwargs": kwargs,
     }
 
 
 def _make_chrome_options(headless: bool) -> ChromeOptions:
-    """ Creates a new options instance for the chrome webdriver """
+    """Creates a new options instance for the chrome webdriver"""
     chrome_options = ChromeOptions()
     if headless:
         chrome_options.add_argument("--headless")
     return chrome_options
 
 
 def make_firefox_driver(
     args: List[Any], kwargs: Dict[str, Any], headless=False
 ) -> Dict[str, Any]:
-    """ Makes a new chrome driver settings instance """
+    """Makes a new chrome driver settings instance"""
     kwargs.update({"options": _make_firefox_options(headless)})
 
     return {
         "callable": webdriver.Firefox,
         "args": args,
         "kwargs": kwargs,
     }
 
 
 def _make_firefox_options(headless: bool) -> FirefoxOptions:
-    """ Creates a new options instance for the firefox webdriver """
+    """Creates a new options instance for the firefox webdriver"""
     firefox_options = FirefoxOptions()
     if headless:
         firefox_options.add_argument("--headless")
     return firefox_options
```

### Comparing `django-selenium-test-1.1.0/django_selenium_test.egg-info/PKG-INFO` & `django-selenium-test-2.0.0/django_selenium_test.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,324 +1,324 @@
 Metadata-Version: 2.1
 Name: django-selenium-test
-Version: 1.1.0
+Version: 2.0.0
 Summary: Write clean Selenium tests in Django
 Home-page: https://github.com/tkw1536/django_selenium_test
 Author: Tom Wiesing
 Author-email: tkw01536@gmail.com
 License: BSD 3-Clause License
-Description: # django-selenium-test
-        
-        ![CI Status](https://github.com/tkw1536/django_selenium_test/workflows/CI/badge.svg)
-        ![Status](https://img.shields.io/pypi/status/django-selenium-test.svg)
-        [![Latest version](https://img.shields.io/pypi/v/django-selenium-test.svg)](https://pypi.python.org/pypi/django-selenium-test)
-        
-        Write Selenium tests on Django 2.x, Django 3.0, Django 3.1 and Python 3.8. 
-        Based on [django-selenium-clean](https://github.com/aptiko/django-selenium-clean). 
-        
-        This documentation is currently a work-in-progress. 
-        
-        ## Tutorial
-        
-        ### Installation
-        
-        In your virtualenv:
-        
-        ```sh
-        pip install django-selenium-test
-        ```
-        
-        ### Setting up
-        
-        * Create a new django project and app:
-        
-        ```sh
-        django-admin startproject foo
-        cd foo
-        python manage.py startapp bar
-        ```
-        
-        * In ``foo/settings.py``, add ``'bar'`` to ``INSTALLED_APPS``
-        
-        * In ``foo/urls.py``, add ``from bar.views import SimpleView`` to the
-          top, and add ``url(r'^$', SimpleView.as_view())`` to ``urlpatterns``.
-        
-        * Add the SimpleView to ``bar/views.py``:
-        
-        ```python
-        import textwrap
-        
-        from django.http import HttpResponse
-        from django.views.generic.base import View
-        
-        
-        class SimpleView(View):
-        
-            def dispatch(request, *args, **kwargs):
-                response_text = textwrap.dedent('''\
-                    <html>
-                    <head>
-                    <title>Greetings to the world</title>
-                    </head>
-                    <body>
-                    <h1 id="earth">Greetings to earth</h1>
-                    <h1 id="world" style="display: none;">Hello, world!</h1>
-        
-                    <p>We have some javascript here so that when you click the button
-                        the heading above toggles between "Greetings to earth" and
-                        "Hello, world!".</p>
-        
-                    <button onclick="toggle()">Toggle</button>
-        
-                    <script type="text/javascript">
-                        toggle = function () {
-                            var heading_earth = document.getElementById("earth");
-                            var heading_world = document.getElementById("world");
-                            if (heading_earth.style.display == 'none') {
-                                heading_world.style.display = 'none';
-                                heading_earth.style.display = 'block';
-                            } else {
-                                heading_earth.style.display = 'none';
-                                heading_world.style.display = 'block';
-                            }
-                        }
-                    </script>
-                    </body>
-                    </html>
-                ''')
-                return HttpResponse(response_text)
-        ```
-        
-        We're done setting up. If you now run ``python manage.py runserver``
-        in your browser and visit http://localhost:8000/ in your browser, you
-        should see the simple page. Let's now proceed to write a test for it.
-        
-        ### Writing the test
-        
-        Modify ``bar/tests.py`` so that it has the following contents:
-        
-        ```python
-        from unittest import skipUnless
-        
-        from django.conf import settings
-        
-        from django_selenium_test import selenium, SeleniumTestCase, PageElement
-        from selenium.webdriver.common.by import By
-        
-        
-        @skipUnless(getattr(settings, 'SELENIUM_WEBDRIVERS', False),
-                    "Selenium is unconfigured")
-        class HelloTestCase(SeleniumTestCase):
-        
-            heading_earth = PageElement(By.ID, 'earth')
-            heading_world = PageElement(By.ID, 'world')
-            button = PageElement(By.CSS_SELECTOR, 'button')
-        
-            def test_toggle(self):
-                # Visit the page
-                self.selenium.get(self.live_server_url)
-        
-                # Check that the earth heading is visible
-                self.assertTrue(self.heading_earth.is_displayed())
-                self.assertFalse(self.heading_world.is_displayed())
-        
-                # Toggle and check the new condition
-                self.button.click()
-                self.heading_world.wait_until_is_displayed()
-                self.assertFalse(self.heading_earth.is_displayed())
-                self.assertTrue(self.heading_world.is_displayed())
-        
-                # Toggle again and re-check
-                self.button.click()
-                self.heading_earth.wait_until_is_displayed()
-                self.assertTrue(self.heading_earth.is_displayed())
-                self.assertFalse(self.heading_world.is_displayed())
-        ```
-        
-        ### Executing the test
-        
-        Try ``python manage.py test`` and it will skip the test because
-        selenium is unconfigured. You need to configure it by specifying
-        ``SELENIUM_WEBDRIVERS`` in ``foo/settings.py``:
-        
-        ```python
-        from django_selenium_test.settings import make_chrome_driver
-        
-        SELENIUM_WEBDRIVERS = {
-            'default': make_chrome_driver([], {}),
-        }
-        ```
-        
-        Now try again, and it should execute the test. 
-        
-        ### Advanced test running tricks
-        
-        #### Executing a test in many widths
-        
-        Add this to your ``foo/settings.py``:
-        
-        ```python
-        SELENIUM_WIDTHS = [1024, 800, 350]
-        ```
-        
-        This will result in executing all ``SeleniumTestCase``'s three times,
-        one for each specified browser width. Useful for responsive designs.
-        The default is to run them on only one width, 1024.
-        
-        #### Using many selenium drivers
-        
-        You can have many ``SELENIUM_WEBDRIVERS``:
-        
-        ```python
-        from django_selenium_test.settings import make_chrome_driver, make_firefox_driver
-        SELENIUM_WEBDRIVERS = {
-            'default': make_chrome_driver([], {})
-            'firefox': make_firefox_driver([], {})
-        }
-        ```
-        
-        By default, the ``default`` one is used. You can specify another using
-        the ``SELENIUM_WEBDRIVER`` environment variable:
-        
-        ```sh
-        SELENIUM_WEBDRIVER=firefox python manage.py test
-        ```
-        
-        
-        #### Running a headless browser
-        
-        It can be very useful to run the selenium tests with a headless
-        browser, that is, in an invisible browser window. For one thing, it
-        is much faster. 
-        
-        To achieve this, pass headless=True to the make_BRAND_driver() function:
-        
-        ```python
-        from django_selenium_test.settings import make_chrome_driver, make_firefox_driver
-        SELENIUM_WEBDRIVERS = {
-            'default': make_chrome_driver([], {}, headless=True)
-            'firefox': make_firefox_driver([], {}, headless=True)
-        }
-        ```
-        
-        #### Using advanced integration tests
-        
-        (Currently undocumented)
-        
-        
-        ## Reference
-        
-        ### SeleniumTestCase objects
-        
-        .. code:: python
-        
-           from django_selenium_test import SeleniumTestCase
-        
-        ``SeleniumTestCase`` is the same as Django's
-        ``StaticLiveServerTestCase`` but it adds a little bit of Selenium
-        functionality. Derive your Selenium tests from this class instead of
-        ``StaticLiveServerTestCase``.
-        
-        The most important feature of ``SeleniumTestCase`` is the ``selenium``
-        attribute.  Technically it is a wrapper around the selenium driver. In
-        practice, you can think about it as the browser, or as the equivalent
-        of Django's test client. It has all `selenium driver attributes and
-        methods`_, but you will mostly use ``get()``. It also has the
-        following additional methods:
-        
-        * ``self.selenium.login(**credentials)``,
-        ``self.selenium.force_login(user, base_url)``,
-        ``self.selenium.logout()``
-        
-          Similar to the Django test client ``login()``, ``force_login()`` and
-          ``logout()`` methods.  ``login()`` returns ``True`` if login is
-          possible; ``False`` if the provided credentials are incorrect, or the
-          user is inactive, or if the sessions framework is not available.
-        
-          The `force_login()` code was adapted from [django-selenium-login](https://github.com/feffe/django-selenium-login/blob/master/seleniumlogin/__init__.py),
-          which is licensed under the MIT License. 
-        
-        * ``self.selenium.wait_until_n_windows(n, timeout=2)``
-        
-          Useful when a Javascript action has caused the browser to open
-          another window. The typical usage is this:
-        
-        ```python
-        button_that_will_open_a_second_window.click()
-        self.selenium.wait_until_n_windows(n=2, timeout=10)
-        windows = self.selenium.window_handles
-        self.selenium.switch_to.window(windows[1])
-        # continue testing
-        ```
-        
-          If the timeout (in seconds) elapses and the number of browser
-          windows never becomes ``n``, an ``AssertionError`` is raised.
-        
-        - [selenium driver attributes and methods](http://selenium-python.readthedocs.org/api.html#module-selenium.webdriver.remote.webdriver)
-        
-        PageElement objects
-        -------------------
-        
-        ```python
-        from django_selenium_test import PageElement
-        ```
-        
-        ``PageElement`` is a lazy wrapper around WebElement_; it has all its
-        properties and methods. It is initialized with a locator_, but the
-        element is not actually located until needed. In addition to
-        WebElement_ properties and methods, it has these:
-        
-        * ``PageElement.exists()``: Returns True if the element can be located.
-        
-        * ``PageElement.wait_until_exists(timeout=10)``
-        
-          ``PageElement.wait_until_not_exists(timeout=10)``
-        
-          ``PageElement.wait_until_is_displayed(timeout=10)``
-        
-          ``PageElement.wait_until_not_displayed(timeout=10)``
-        
-          ``PageElement.wait_until_contains(text, timeout=10)``
-        
-          ``PageElement.wait_until_not_contains(text, timeout=10)``
-        
-          What these methods do should be self-explanatory from their name. The
-          ones ending in ``contains`` refer to whether the element contains the
-          specified text.  The methods raise an exception if there is a timeout.
-        
-        - [WebElement](http://selenium-python.readthedocs.org/api.html#module-selenium.webdriver.remote.webelement)
-        - [locator](http://selenium-python.readthedocs.org/api.html#locate-elements-by)
-        
-        ### IntegrationTest objects
-        (Currently undocumented)
-        
-        ### Running django-selenium-test's own unit tests
-        
-        By default the unit tests will use Chrome::
-        
-        ```sh
-        ./setup.py test
-        ```
-        
-        Use the ``SELENIUM_BROWSER`` environment variable to use another browser:
-        
-        ```sh
-        SELENIUM_BROWSER=firefox ./setup.py test
-        ```
-        
-        ## License
-        
-        Licensed under the BSD 3-clause license; see `LICENSE.txt` for details.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# django-selenium-test
+
+![CI Status](https://github.com/tkw1536/django_selenium_test/workflows/CI/badge.svg)
+![Status](https://img.shields.io/pypi/status/django-selenium-test.svg)
+[![Latest version](https://img.shields.io/pypi/v/django-selenium-test.svg)](https://pypi.python.org/pypi/django-selenium-test)
+
+Write Selenium tests on Django 3.2, Django 4.0, Django 3.1 and Python 3.8+. 
+Based on [django-selenium-clean](https://github.com/aptiko/django-selenium-clean). 
+
+This documentation is currently a work-in-progress. 
+
+## Tutorial
+
+### Installation
+
+In your virtualenv:
+
+```sh
+pip install django-selenium-test
+```
+
+### Setting up
+
+* Create a new django project and app:
+
+```sh
+django-admin startproject foo
+cd foo
+python manage.py startapp bar
+```
+
+* In ``foo/settings.py``, add ``'bar'`` to ``INSTALLED_APPS``
+
+* In ``foo/urls.py``, add ``from bar.views import SimpleView`` to the
+  top, and add ``url(r'^$', SimpleView.as_view())`` to ``urlpatterns``.
+
+* Add the SimpleView to ``bar/views.py``:
+
+```python
+import textwrap
+
+from django.http import HttpResponse
+from django.views.generic.base import View
+
+
+class SimpleView(View):
+
+    def dispatch(request, *args, **kwargs):
+        response_text = textwrap.dedent('''\
+            <html>
+            <head>
+            <title>Greetings to the world</title>
+            </head>
+            <body>
+            <h1 id="earth">Greetings to earth</h1>
+            <h1 id="world" style="display: none;">Hello, world!</h1>
+
+            <p>We have some javascript here so that when you click the button
+                the heading above toggles between "Greetings to earth" and
+                "Hello, world!".</p>
+
+            <button onclick="toggle()">Toggle</button>
+
+            <script type="text/javascript">
+                toggle = function () {
+                    var heading_earth = document.getElementById("earth");
+                    var heading_world = document.getElementById("world");
+                    if (heading_earth.style.display == 'none') {
+                        heading_world.style.display = 'none';
+                        heading_earth.style.display = 'block';
+                    } else {
+                        heading_earth.style.display = 'none';
+                        heading_world.style.display = 'block';
+                    }
+                }
+            </script>
+            </body>
+            </html>
+        ''')
+        return HttpResponse(response_text)
+```
+
+We're done setting up. If you now run ``python manage.py runserver``
+in your browser and visit http://localhost:8000/ in your browser, you
+should see the simple page. Let's now proceed to write a test for it.
+
+### Writing the test
+
+Modify ``bar/tests.py`` so that it has the following contents:
+
+```python
+from unittest import skipUnless
+
+from django.conf import settings
+
+from django_selenium_test import selenium, SeleniumTestCase, PageElement
+from selenium.webdriver.common.by import By
+
+
+@skipUnless(getattr(settings, 'SELENIUM_WEBDRIVERS', False),
+            "Selenium is unconfigured")
+class HelloTestCase(SeleniumTestCase):
+
+    heading_earth = PageElement(By.ID, 'earth')
+    heading_world = PageElement(By.ID, 'world')
+    button = PageElement(By.CSS_SELECTOR, 'button')
+
+    def test_toggle(self):
+        # Visit the page
+        self.selenium.get(self.live_server_url)
+
+        # Check that the earth heading is visible
+        self.assertTrue(self.heading_earth.is_displayed())
+        self.assertFalse(self.heading_world.is_displayed())
+
+        # Toggle and check the new condition
+        self.button.click()
+        self.heading_world.wait_until_is_displayed()
+        self.assertFalse(self.heading_earth.is_displayed())
+        self.assertTrue(self.heading_world.is_displayed())
+
+        # Toggle again and re-check
+        self.button.click()
+        self.heading_earth.wait_until_is_displayed()
+        self.assertTrue(self.heading_earth.is_displayed())
+        self.assertFalse(self.heading_world.is_displayed())
+```
+
+### Executing the test
+
+Try ``python manage.py test`` and it will skip the test because
+selenium is unconfigured. You need to configure it by specifying
+``SELENIUM_WEBDRIVERS`` in ``foo/settings.py``:
+
+```python
+from django_selenium_test.settings import make_chrome_driver
+
+SELENIUM_WEBDRIVERS = {
+    'default': make_chrome_driver([], {}),
+}
+```
+
+Now try again, and it should execute the test. 
+
+### Advanced test running tricks
+
+#### Executing a test in many widths
+
+Add this to your ``foo/settings.py``:
+
+```python
+SELENIUM_WIDTHS = [1024, 800, 350]
+```
+
+This will result in executing all ``SeleniumTestCase``'s three times,
+one for each specified browser width. Useful for responsive designs.
+The default is to run them on only one width, 1024.
+
+#### Using many selenium drivers
+
+You can have many ``SELENIUM_WEBDRIVERS``:
+
+```python
+from django_selenium_test.settings import make_chrome_driver, make_firefox_driver
+SELENIUM_WEBDRIVERS = {
+    'default': make_chrome_driver([], {})
+    'firefox': make_firefox_driver([], {})
+}
+```
+
+By default, the ``default`` one is used. You can specify another using
+the ``SELENIUM_WEBDRIVER`` environment variable:
+
+```sh
+SELENIUM_WEBDRIVER=firefox python manage.py test
+```
+
+
+#### Running a headless browser
+
+It can be very useful to run the selenium tests with a headless
+browser, that is, in an invisible browser window. For one thing, it
+is much faster. 
+
+To achieve this, pass headless=True to the make_BRAND_driver() function:
+
+```python
+from django_selenium_test.settings import make_chrome_driver, make_firefox_driver
+SELENIUM_WEBDRIVERS = {
+    'default': make_chrome_driver([], {}, headless=True)
+    'firefox': make_firefox_driver([], {}, headless=True)
+}
+```
+
+#### Using advanced integration tests
+
+(Currently undocumented)
+
+
+## Reference
+
+### SeleniumTestCase objects
+
+.. code:: python
+
+   from django_selenium_test import SeleniumTestCase
+
+``SeleniumTestCase`` is the same as Django's
+``StaticLiveServerTestCase`` but it adds a little bit of Selenium
+functionality. Derive your Selenium tests from this class instead of
+``StaticLiveServerTestCase``.
+
+The most important feature of ``SeleniumTestCase`` is the ``selenium``
+attribute.  Technically it is a wrapper around the selenium driver. In
+practice, you can think about it as the browser, or as the equivalent
+of Django's test client. It has all `selenium driver attributes and
+methods`_, but you will mostly use ``get()``. It also has the
+following additional methods:
+
+* ``self.selenium.login(**credentials)``,
+``self.selenium.force_login(user, base_url)``,
+``self.selenium.logout()``
+
+  Similar to the Django test client ``login()``, ``force_login()`` and
+  ``logout()`` methods.  ``login()`` returns ``True`` if login is
+  possible; ``False`` if the provided credentials are incorrect, or the
+  user is inactive, or if the sessions framework is not available.
+
+  The `force_login()` code was adapted from [django-selenium-login](https://github.com/feffe/django-selenium-login/blob/master/seleniumlogin/__init__.py),
+  which is licensed under the MIT License. 
+
+* ``self.selenium.wait_until_n_windows(n, timeout=2)``
+
+  Useful when a Javascript action has caused the browser to open
+  another window. The typical usage is this:
+
+```python
+button_that_will_open_a_second_window.click()
+self.selenium.wait_until_n_windows(n=2, timeout=10)
+windows = self.selenium.window_handles
+self.selenium.switch_to.window(windows[1])
+# continue testing
+```
+
+  If the timeout (in seconds) elapses and the number of browser
+  windows never becomes ``n``, an ``AssertionError`` is raised.
+
+- [selenium driver attributes and methods](http://selenium-python.readthedocs.org/api.html#module-selenium.webdriver.remote.webdriver)
+
+PageElement objects
+-------------------
+
+```python
+from django_selenium_test import PageElement
+```
+
+``PageElement`` is a lazy wrapper around WebElement_; it has all its
+properties and methods. It is initialized with a locator_, but the
+element is not actually located until needed. In addition to
+WebElement_ properties and methods, it has these:
+
+* ``PageElement.exists()``: Returns True if the element can be located.
+
+* ``PageElement.wait_until_exists(timeout=10)``
+
+  ``PageElement.wait_until_not_exists(timeout=10)``
+
+  ``PageElement.wait_until_is_displayed(timeout=10)``
+
+  ``PageElement.wait_until_not_displayed(timeout=10)``
+
+  ``PageElement.wait_until_contains(text, timeout=10)``
+
+  ``PageElement.wait_until_not_contains(text, timeout=10)``
+
+  What these methods do should be self-explanatory from their name. The
+  ones ending in ``contains`` refer to whether the element contains the
+  specified text.  The methods raise an exception if there is a timeout.
+
+- [WebElement](http://selenium-python.readthedocs.org/api.html#module-selenium.webdriver.remote.webelement)
+- [locator](http://selenium-python.readthedocs.org/api.html#locate-elements-by)
+
+### IntegrationTest objects
+(Currently undocumented)
+
+### Running django-selenium-test's own unit tests
+
+By default the unit tests will use Chrome::
+
+```sh
+./setup.py test
+```
+
+Use the ``SELENIUM_BROWSER`` environment variable to use another browser:
+
+```sh
+SELENIUM_BROWSER=firefox ./setup.py test
+```
+
+## License
+
+Licensed under the BSD 3-clause license; see `LICENSE.txt` for details.
```

### Comparing `django-selenium-test-1.1.0/django_selenium_test.egg-info/SOURCES.txt` & `django-selenium-test-2.0.0/django_selenium_test.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 CHANGES.txt
 LICENSE.txt
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+setup.cfg
 django_selenium_test/__init__.py
 django_selenium_test/core.py
 django_selenium_test/integration.py
 django_selenium_test/settings.py
 django_selenium_test.egg-info/PKG-INFO
 django_selenium_test.egg-info/SOURCES.txt
 django_selenium_test.egg-info/dependency_links.txt
```

### Comparing `django-selenium-test-1.1.0/tests/manage.py` & `django-selenium-test-2.0.0/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-selenium-test-1.1.0/tests/settings.py` & `django-selenium-test-2.0.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-selenium-test-1.1.0/tests/tests/test_01_core.py` & `django-selenium-test-2.0.0/tests/tests/test_01_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
 
 from django_selenium_test import PageElement, SeleniumTestCase
 
 
 class DjangoSeleniumCleanTestCase(SeleniumTestCase):
-
     heading_earth = PageElement(By.ID, "earth")
     heading_world = PageElement(By.ID, "world")
     user_info = PageElement(By.ID, "user")
     button_toggle_heading = PageElement(By.ID, "toggle-heading")
     button_open_window = PageElement(By.ID, "open-window")
     button_toggle_element = PageElement(By.ID, "toggle-element")
     button_toggle_message = PageElement(By.ID, "toggle-message")
```

### Comparing `django-selenium-test-1.1.0/tests/tests/test_02_integration.py` & `django-selenium-test-2.0.0/tests/tests/test_02_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 from unittest import mock
 
 from django_selenium_test import IntegrationTest
 
 
 class ExampleIntegrationTest(IntegrationTest):
-
     find_element_selector = "main"
 
     def test_element_mixins(self) -> None:
-        """ Checks that the element mixins work as intended """
+        """Checks that the element mixins work as intended"""
 
         self.load_live_url("integration")
 
         test_element = self.find_element("#test")
         self.assertIsNotNone(test_element, "Can find the test element")
 
         test_next_element = self.find_element("#test_next")
@@ -23,27 +22,26 @@
         self.assertEqual(
             self.find_next_sibling(test_element),
             test_next_element,
             "Checks that find_next_sibling works as expected",
         )
 
     def test_element_assertions(self) -> None:
-        """ Checks that the element assertions work as intended """
+        """Checks that the element assertions work as intended"""
 
         self.load_live_url("integration")
 
         self.assert_element_exists("#exists")
         self.assert_element_not_exists("#not_exists")
 
         self.assert_element_displayed("#displayed")
         self.assert_element_not_displayed("#not_displayed")
         self.assert_element_not_displayed("#not_exists")
 
     def test_urls(self) -> None:
-
         # check that load_live_url and assert_url_equal work
         self.load_live_url(
             "integrationparams",
             url_kwargs={"parameter": 12},
             url_reverse_get_params={"next": "integration"},
         )
         self.assert_url_equal(
@@ -53,15 +51,14 @@
         )
 
         # check that the follow function works
         self.assert_url_follow("integrationredirect", "integration")
 
     @mock.patch("tests.views.cleaned_data_check", return_value=1)
     def test_fill_form(self, cmock: mock.Mock) -> None:
-
         # fill in the form normally
         self.submit_form(
             "integration",
             "input_id_submit",
             send_form_keys={"id_a": "Filled in A"},
             select_dropdowns={"id_b": "b"},
             script_value={"id_c": "Filled in C"},
```

### Comparing `django-selenium-test-1.1.0/tests/tests/test_03_user_autologin.py` & `django-selenium-test-2.0.0/tests/tests/test_03_user_autologin.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 from django_selenium_test import IntegrationTest
 
 
 class ExampleIntegrationTest(IntegrationTest):
     user = "alice"
 
     def setUp(self):
-
         # crate the alice user
         from django.contrib.auth.hashers import make_password
         from django.contrib.auth.models import User
 
         alice = User.objects.create(
             username="alice", password=make_password("topsecret"), is_active=True
         )
 
         # create the alice user
         super().setUp()
 
     def test_auto_login(self):
-        """ Checks that the user was actually logged in """
+        """Checks that the user was actually logged in"""
 
         element = self.load_live_url("core", selector="#user")
         self.assertEqual(element.text, "The logged on user is alice.")
         self.assertIsNone(self.user.last_login)
```

### Comparing `django-selenium-test-1.1.0/tests/urls.py` & `django-selenium-test-2.0.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-selenium-test-1.1.0/tests/views.py` & `django-selenium-test-2.0.0/tests/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from .forms import SampleForm
 
 if TYPE_CHECKING:
     from django.http import HttpRequest
 
 
 def cleaned_data_check(data: dict) -> None:
-    """ Function that doesn't do anythingbut is mocked by integration tests to check if cleaned_data is right """
+    """Function that doesn't do anythingbut is mocked by integration tests to check if cleaned_data is right"""
     pass
 
 
 class SampleFormView(FormView):
     template_name = "integration.html"
     form_class = SampleForm
     success_url = "/integration/submit"
```

