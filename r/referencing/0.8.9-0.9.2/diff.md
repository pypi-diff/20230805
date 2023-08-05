# Comparing `tmp/referencing-0.8.9.tar.gz` & `tmp/referencing-0.9.2.tar.gz`

## Comparing `referencing-0.8.9.tar` & `referencing-0.9.2.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 referencing-0.8.9/.coveragerc
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 referencing-0.8.9/.flake8
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 referencing-0.8.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 referencing-0.8.9/.readthedocs.yml
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 referencing-0.8.9/noxfile.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 referencing-0.8.9/.github/FUNDING.yml
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 referencing-0.8.9/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 referencing-0.8.9/.github/dependabot.yml
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 referencing-0.8.9/.github/workflows/ci.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 referencing-0.8.9/docs/Makefile
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 referencing-0.8.9/docs/api.rst
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 referencing-0.8.9/docs/conf.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 referencing-0.8.9/docs/index.rst
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 referencing-0.8.9/docs/requirements.in
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 referencing-0.8.9/docs/requirements.txt
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 referencing-0.8.9/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 referencing-0.8.9/referencing/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 referencing-0.8.9/referencing/_attrs.py
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 referencing-0.8.9/referencing/_core.py
--rw-r--r--   0        0        0     7039 2020-02-02 00:00:00.000000 referencing-0.8.9/referencing/jsonschema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 referencing-0.8.9/referencing/py.typed
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 referencing-0.8.9/referencing/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 referencing-0.8.9/referencing/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 referencing-0.8.9/tests/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 referencing-0.8.9/tests/test_integration.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 referencing-0.8.9/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 referencing-0.8.9/COPYING
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 referencing-0.8.9/README.rst
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 referencing-0.8.9/pyproject.toml
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 referencing-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 referencing-0.9.2/.flake8
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 referencing-0.9.2/.gitmodules
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 referencing-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 referencing-0.9.2/.readthedocs.yml
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 referencing-0.9.2/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 referencing-0.9.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 referencing-0.9.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 referencing-0.9.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 referencing-0.9.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 referencing-0.9.2/docs/Makefile
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 referencing-0.9.2/docs/api.rst
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 referencing-0.9.2/docs/conf.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 referencing-0.9.2/docs/index.rst
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 referencing-0.9.2/docs/requirements.in
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 referencing-0.9.2/docs/requirements.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 referencing-0.9.2/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/_attrs.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/_attrs.pyi
+-rw-r--r--   0        0        0    15169 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/_core.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/exceptions.py
+-rw-r--r--   0        0        0     8527 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/jsonschema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/py.typed
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/tests/__init__.py
+-rw-r--r--   0        0        0    22265 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/tests/test_core.py
+-rw-r--r--   0        0        0     6287 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/tests/test_jsonschema.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 referencing-0.9.2/referencing/tests/test_referencing_suite.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 referencing-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 referencing-0.9.2/COPYING
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 referencing-0.9.2/README.rst
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 referencing-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 referencing-0.9.2/PKG-INFO
```

### Comparing `referencing-0.8.9/.pre-commit-config.yaml` & `referencing-0.9.2/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
   - repo: https://github.com/PyCQA/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/pycqa/flake8
     rev: "6.0.0"
     hooks:
       - id: flake8
   - repo: https://github.com/asottile/pyupgrade
```

### Comparing `referencing-0.8.9/noxfile.py` & `referencing-0.9.2/noxfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import nox
 
 ROOT = Path(__file__).parent
+PYPROJECT = ROOT / "pyproject.toml"
 DOCS = ROOT / "docs"
 REFERENCING = ROOT / "referencing"
-TESTS = ROOT / "tests"
 
 
 nox.options.sessions = []
 
 
 def session(default=True, **kwargs):
     def _session(fn):
@@ -18,62 +18,58 @@
         return nox.session(**kwargs)(fn)
 
     return _session
 
 
 @session(python=["3.8", "3.9", "3.10", "3.11", "pypy3"])
 def tests(session):
-    session.install("pytest", str(ROOT))
-    session.run("pytest")
+    dependencies = ["pytest", ROOT]
+    if session.posargs == ["coverage"]:
+        dependencies.append("coverage[toml]")
+        session.install(*dependencies)
+        session.run("coverage", "run", "-m", "pytest")
+        session.run("coverage", "report")
+    else:
+        session.install(*dependencies)
+        session.run("pytest", *session.posargs, REFERENCING)
 
 
 @session(tags=["build"])
 def build(session):
     session.install("build")
     tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", str(ROOT), "--outdir", tmpdir)
+    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
 
 
 @session(tags=["style"])
 def readme(session):
     session.install("build", "twine")
     tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", str(ROOT), "--outdir", tmpdir)
+    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
     session.run("python", "-m", "twine", "check", tmpdir + "/*")
 
 
 @session(tags=["style"])
 def style(session):
     session.install(
         "flake8",
         "flake8-broken-line",
         "flake8-bugbear",
         "flake8-commas",
+        "flake8-docstrings",
         "flake8-quotes",
         "flake8-tidy-imports",
     )
-    session.run(
-        "python",
-        "-m",
-        "flake8",
-        str(REFERENCING),
-        str(TESTS),
-        __file__,
-    )
+    session.run("python", "-m", "flake8", REFERENCING, __file__)
 
 
 @session()
 def typing(session):
-    session.install(  # FIXME: Don't repeat dependencies.
-        "attrs",
-        "mypy",
-        "pyrsistent",
-        str(ROOT),
-    )
-    session.run("python", "-m", "mypy", str(REFERENCING))
+    session.install("pyright", ROOT)
+    session.run("pyright", REFERENCING)
 
 
 @session(tags=["docs"])
 @nox.parametrize(
     "builder",
     [
         nox.param(name, id=name)
@@ -83,32 +79,32 @@
             "linkcheck",
             "man",
             "spelling",
         ]
     ],
 )
 def docs(session, builder):
-    session.install("-r", str(DOCS / "requirements.txt"))
+    session.install("-r", DOCS / "requirements.txt")
     tmpdir = Path(session.create_tmp())
     argv = ["-n", "-T", "-W"]
     if builder != "spelling":
         argv += ["-q"]
     session.run(
         "python",
         "-m",
         "sphinx",
         "-b",
         builder,
-        str(DOCS),
-        str(tmpdir / builder),
+        DOCS,
+        tmpdir / builder,
         *argv,
     )
 
 
 @session(tags=["docs", "style"], name="docs(style)")
 def docs_style(session):
     session.install(
         "doc8",
         "pygments",
         "pygments-github-lexers",
     )
-    session.run("python", "-m", "doc8", "--max-line-length", "1000", str(DOCS))
+    session.run("python", "-m", "doc8", "--config", PYPROJECT, DOCS)
```

### Comparing `referencing-0.8.9/.github/SECURITY.md` & `referencing-0.9.2/.github/SECURITY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 # Security Policy
 
 ## Supported Versions
 
-In general, only the latest released `referencing` version is supported
-and will receive updates.
+In general, only the latest released `referencing` version is supported and will receive updates.
 
 ## Reporting a Vulnerability
 
-To report a security vulnerability, please send an email to
-`Julian+Security` at `GrayVines.com` with subject line `SECURITY (referencing)`.
+To report a security vulnerability, please send an email to `Julian+Security` at `GrayVines.com` with subject line `SECURITY (referencing)`.
 
-I will do my best to respond within 48 hours to acknowledge the message
-and discuss further steps.
+I will do my best to respond within 48 hours to acknowledge the message and discuss further steps.
 
-If the vulnerability is accepted, an advisory will be sent out via
-GitHub's security advisory functionality.
+If the vulnerability is accepted, an advisory will be sent out via GitHub's security advisory functionality.
 
-For non-sensitive discussion related to this policy itself, feel free to
-open an issue on the issue tracker.
+For non-sensitive discussion related to this policy itself, feel free to open an issue on the issue tracker.
```

### Comparing `referencing-0.8.9/docs/Makefile` & `referencing-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `referencing-0.8.9/docs/api.rst` & `referencing-0.9.2/docs/api.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 API Reference
 =============
 
 .. automodule:: referencing
    :members:
    :undoc-members:
    :imported-members:
+   :special-members: __iter__, __getitem__, __len__
 
-.. autoclass:: referencing._core.Resolver
+
+.. autoclass:: referencing._core.Resolved
    :members:
    :undoc-members:
 
-.. autoclass:: referencing._core.Specification
+
+.. autoclass:: referencing._core.Resolver
    :members:
    :undoc-members:
 
 
 Submodules
 ----------
 
@@ -22,13 +25,21 @@
 ^^^^^^^^^^^^^^^^^^^^^^
 
 .. automodule:: referencing.jsonschema
    :members:
    :undoc-members:
 
 
+referencing.exceptions
+^^^^^^^^^^^^^^^^^^^^^^
+
+.. automodule:: referencing.exceptions
+   :members:
+   :undoc-members:
+
+
 referencing.typing
 ^^^^^^^^^^^^^^^^^^
 
 .. automodule:: referencing.typing
    :members:
    :undoc-members:
```

### Comparing `referencing-0.8.9/docs/conf.py` & `referencing-0.9.2/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from pathlib import Path
 import importlib.metadata
 import re
 
-from hyperlink import URL
-from sphinx.ext.intersphinx import resolve_reference_in_inventory
+from yarl import URL
 
 DOCS = Path(__file__).parent
 
-GITHUB = URL.from_text("https://github.com/")
-HOMEPAGE = GITHUB.child("python-jsonschema", "referencing")
+GITHUB = URL("https://github.com/")
+HOMEPAGE = GITHUB / "python-jsonschema/referencing"
 
 project = "referencing"
 author = "Julian Berman"
 copyright = "2022, " + author
 
 release = importlib.metadata.version("referencing")
 version = release.partition("-")[0]
@@ -35,41 +34,33 @@
     "sphinxcontrib.spelling",
 ]
 
 pygments_style = "lovelace"
 pygments_dark_style = "one-dark"
 
 html_theme = "furo"
-html_static_path = []
 
 # See sphinx-doc/sphinx#10785
 _TYPE_ALIASES = dict(
     AnchorType=("class", "Anchor"),
+    D=("data", "D"),
     ObjectSchema=("data", "ObjectSchema"),
     Schema=("data", "Schema"),
+    URI=("attr", "URI"),  # ?!?!?! Sphinx...
 )
 
 
 def _resolve_broken_refs(app, env, node, contnode):
     if node["refdomain"] != "py":
         return
 
-    # Evade tobgu/pyrsistent#267
-    if node["reftarget"].startswith("pyrsistent.typing."):
-        node["reftarget"] = node["reftarget"].replace(".typing.", ".")
-        return resolve_reference_in_inventory(
-            env, "pyrsistent", node, contnode
-        )
-    elif node["reftarget"] == "PList":
-        node["reftarget"] = "pyrsistent.PList"
-        return resolve_reference_in_inventory(
-            env, "pyrsistent", node, contnode
-        )
-
-    kind, target = _TYPE_ALIASES.get(node["reftarget"], (None, None))
+    if node["reftarget"].startswith("referencing.typing."):
+        kind, target = "data", node["reftarget"]
+    else:
+        kind, target = _TYPE_ALIASES.get(node["reftarget"], (None, None))
     if kind is not None:
         return app.env.get_domain("py").resolve_xref(
             env,
             node["refdoc"],
             app.builder,
             kind,
             target,
@@ -101,29 +92,29 @@
     "pyrsistent": ("https://pyrsistent.readthedocs.io/en/latest/", None),
     "python": ("https://docs.python.org/", None),
 }
 
 # -- Options for extlinks extension ------------------------------------------
 
 extlinks = {
-    "gh": (str(HOMEPAGE.child("%s")), None),
-    "github": (str(GITHUB.child("%s")), None),
+    "gh": (str(HOMEPAGE) + "/%s", None),
+    "github": (str(GITHUB) + "/%s", None),
 }
 
 # -- Options for the linkcheck builder ---------------------------------------
 
 
 def entire_domain(host):
     return r"http.?://" + re.escape(host) + r"($|/.*)"
 
 
 linkcheck_ignore = [
     entire_domain("codecov.io"),
     entire_domain("img.shields.io"),
     f"{GITHUB}.*#.*",
-    str(HOMEPAGE.child("actions")),
-    str(HOMEPAGE.child("python-jsonschema/workflows/CI/badge.svg")),
+    str(HOMEPAGE / "actions"),
+    str(HOMEPAGE / "python-jsonschema/workflows/CI/badge.svg"),
 ]
 
 # -- Options for spelling extension ------------------------------------------
 
 spelling_show_suggestions = True
```

### Comparing `referencing-0.8.9/docs/requirements.txt` & `referencing-0.9.2/docs/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with python 3.11
 # To update, run:
 #
 #    pip-compile docs/requirements.in
 #
 alabaster==0.7.12
     # via sphinx
-attrs==22.1.0
+attrs==22.2.0
     # via referencing
 babel==2.11.0
     # via sphinx
 beautifulsoup4==4.11.1
     # via furo
 certifi==2022.12.7
     # via requests
@@ -20,55 +20,52 @@
     # via sphinx-click
 docutils==0.19
     # via
     #   sphinx
     #   sphinx-click
 furo==2022.12.7
     # via -r docs/requirements.in
-hyperlink==21.0.0
-    # via -r docs/requirements.in
 idna==3.4
     # via
-    #   hyperlink
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via sphinx
 lxml==4.9.2
     # via sphinx-json-schema-spec
 markupsafe==2.1.1
     # via jinja2
-multidict==6.0.3
+multidict==6.0.4
     # via yarl
 packaging==22.0
     # via sphinx
 pyenchant==3.2.2
     # via sphinxcontrib-spelling
-pygments==2.13.0
+pygments==2.14.0
     # via
     #   furo
     #   pygments-github-lexers
     #   sphinx
 pygments-github-lexers==0.0.5
     # via -r docs/requirements.in
-pyrsistent==0.19.2
+pyrsistent==0.19.3
     # via referencing
 pytz==2022.7
     # via babel
 file:.#egg=referencing
     # via -r docs/requirements.in
 requests==2.28.1
     # via sphinx
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.3.2.post1
     # via beautifulsoup4
-sphinx==5.3.0
+sphinx==6.1.1
     # via
     #   -r docs/requirements.in
     #   furo
     #   sphinx-basic-ng
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-json-schema-spec
@@ -94,8 +91,10 @@
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
 sphinxcontrib-spelling==7.7.0
     # via -r docs/requirements.in
 urllib3==1.26.13
     # via requests
 yarl==1.8.2
-    # via referencing
+    # via
+    #   -r docs/requirements.in
+    #   referencing
```

### Comparing `referencing-0.8.9/referencing/_attrs.py` & `referencing-0.9.2/referencing/_attrs.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-from typing import TYPE_CHECKING
+from __future__ import annotations
 
-if TYPE_CHECKING:
-    from attrs import define, frozen
-else:
-    from attrs import define as _define, frozen as _frozen
-
-    def define(cls):
-        cls.__init_subclass__ = UnsupportedSubclassing.complain
-        return _define(cls)
-
-    def frozen(cls):
-        cls.__init_subclass__ = UnsupportedSubclassing.complain
-        return _frozen(cls)
+from typing import NoReturn, TypeVar
+
+from attrs import define as _define, frozen as _frozen
+
+_T = TypeVar("_T")
+
+
+def define(cls: type[_T]) -> type[_T]:  # pragma: no cover
+    cls.__init_subclass__ = _do_not_subclass
+    return _define(cls)
+
+
+def frozen(cls: type[_T]) -> type[_T]:
+    cls.__init_subclass__ = _do_not_subclass
+    return _frozen(cls)
 
 
 class UnsupportedSubclassing(Exception):
-    @classmethod
-    def complain(this):
-        raise UnsupportedSubclassing(
-            "Subclassing is not part of referencing's public API. "
-            "If no other suitable API exists for what you're trying to do, "
-            "feel free to file an issue asking for one.",
-        )
+    pass
+
+
+@staticmethod
+def _do_not_subclass() -> NoReturn:  # pragma: no cover
+    raise UnsupportedSubclassing(
+        "Subclassing is not part of referencing's public API. "
+        "If no other suitable API exists for what you're trying to do, "
+        "feel free to file an issue asking for one.",
+    )
```

### Comparing `referencing-0.8.9/.gitignore` & `referencing-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `referencing-0.8.9/COPYING` & `referencing-0.9.2/COPYING`

 * *Files identical despite different names*

### Comparing `referencing-0.8.9/README.rst` & `referencing-0.9.2/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -21,14 +21,14 @@
    :target: https://referencing.readthedocs.io/en/stable/
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/python-jsonschema/referencing/main.svg
   :alt: pre-commit.ci status
   :target: https://results.pre-commit.ci/latest/github/python-jsonschema/referencing/main
 
 
-A (very early) playground for exploring:
+An implementation-agnostic implementation of JSON reference resolution.
 
-    * the budding JSON `reference specification(s) <https://github.com/json-schema-org/referencing>`_ (currently housed within the JSON Schema organization but intended to be more broadly applicable)
+In other words, a way for e.g. JSON Schema tooling to resolve the ``$ref`` keyword across all drafts (without needing to implement support themselves).
 
-    * a newer / better integration of reference resolution into `jsonschema <https://pypi.org/project/jsonschema/>`_, likely built on top of the more generic interface which will come out of the above
+What's here is inspired in part by the budding JSON `reference specification(s) <https://github.com/json-schema-org/referencing>`_ (currently housed within the JSON Schema organization but intended to be more broadly applicable), which intend to detach some of the referencing behavior from JSON Schema's own specifications.
 
-What's here (if any of it even functions) is highly experimental and will change.
+See `the documentation <https://referencing.readthedocs.io/>`_ for more details.
```

### Comparing `referencing-0.8.9/pyproject.toml` & `referencing-0.9.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 source = "vcs"
 
 [project]
 name = "referencing"
 description = "JSON Referencing + Python"
 readme = "README.rst"
 license = {text = "MIT"}
+requires-python = ">=3.8"
 keywords = []
 authors = [
   {email = "Julian+referencing@GrayVines.com"},
   {name = "Julian Berman"},
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -27,22 +28,42 @@
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 
 ]
 dynamic = ["version"]
 dependencies = [
-  "attrs",
+  "attrs>=22.2.0",
   "pyrsistent",
   "yarl",
 ]
 
 [project.urls]
 Homepage = "https://github.com/python-jsonschema/referencing"
 Issues = "https://github.com/python-jsonschema/referencing/issues/"
 Source = "https://github.com/python-jsonschema/referencing"
 
+[tool.coverage.run]
+branch = true
+source = ["referencing"]
+dynamic_context = "test_function"
+
+[tool.coverage.report]
+fail_under = 100
+
+[tool.doc8]
+ignore = [
+    "D001",  # one sentence per line, so max length doesn't make sense
+]
+
 [tool.isort]
 combine_as_imports = true
 from_first = true
 include_trailing_comma = true
 multi_line_output = 3
+
+[tool.pyright]
+strict = ["**/*"]
+exclude = [
+    "**/tests/__init__.py",
+    "**/tests/test_*.py",
+]
```

### Comparing `referencing-0.8.9/PKG-INFO` & `referencing-0.9.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: referencing
-Version: 0.8.9
+Version: 0.9.2
 Summary: JSON Referencing + Python
 Project-URL: Homepage, https://github.com/python-jsonschema/referencing
 Project-URL: Issues, https://github.com/python-jsonschema/referencing/issues/
 Project-URL: Source, https://github.com/python-jsonschema/referencing
 Author: Julian Berman
 Author-email: Julian+referencing@GrayVines.com
 License: MIT
@@ -16,15 +16,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: attrs
+Requires-Python: >=3.8
+Requires-Dist: attrs>=22.2.0
 Requires-Dist: pyrsistent
 Requires-Dist: yarl
 Description-Content-Type: text/x-rst
 
 ===============
 ``referencing``
 ===============
@@ -48,14 +49,14 @@
    :target: https://referencing.readthedocs.io/en/stable/
 
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/python-jsonschema/referencing/main.svg
   :alt: pre-commit.ci status
   :target: https://results.pre-commit.ci/latest/github/python-jsonschema/referencing/main
 
 
-A (very early) playground for exploring:
+An implementation-agnostic implementation of JSON reference resolution.
 
-    * the budding JSON `reference specification(s) <https://github.com/json-schema-org/referencing>`_ (currently housed within the JSON Schema organization but intended to be more broadly applicable)
+In other words, a way for e.g. JSON Schema tooling to resolve the ``$ref`` keyword across all drafts (without needing to implement support themselves).
 
-    * a newer / better integration of reference resolution into `jsonschema <https://pypi.org/project/jsonschema/>`_, likely built on top of the more generic interface which will come out of the above
+What's here is inspired in part by the budding JSON `reference specification(s) <https://github.com/json-schema-org/referencing>`_ (currently housed within the JSON Schema organization but intended to be more broadly applicable), which intend to detach some of the referencing behavior from JSON Schema's own specifications.
 
-What's here (if any of it even functions) is highly experimental and will change.
+See `the documentation <https://referencing.readthedocs.io/>`_ for more details.
```

