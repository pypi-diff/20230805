# Comparing `tmp/vp4jl-0.1.2.tar.gz` & `tmp/vp4jl-0.1.3.tar.gz`

## Comparing `vp4jl-0.1.2.tar` & `vp4jl-0.1.3.tar`

### file list

```diff
@@ -1,70 +1,69 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vp4jl-0.1.2/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 vp4jl-0.1.2/.yarnrc.yml
--rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 vp4jl-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 vp4jl-0.1.2/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 vp4jl-0.1.2/babel.config.js
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 vp4jl-0.1.2/conftest.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 vp4jl-0.1.2/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 vp4jl-0.1.2/jest.config.js
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 vp4jl-0.1.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vp4jl-0.1.2/setup.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 vp4jl-0.1.2/tsconfig.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 vp4jl-0.1.2/tsconfig.test.json
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 vp4jl-0.1.2/untitled.vp4jl
--rw-r--r--   0        0        0   421990 2020-02-02 00:00:00.000000 vp4jl-0.1.2/yarn.lock
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 vp4jl-0.1.2/jupyter-config/nb-config/vp4jl.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 vp4jl-0.1.2/jupyter-config/server-config/vp4jl.json
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/context.ts
--rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/index.ts
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/model-factory.ts
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/model.ts
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/namepace.ts
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/node-extension.tsx
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/request-token.ts
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/request.ts
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/toolbar-factory.ts
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/tracker.ts
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/utils.ts
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/widget-factory.ts
--rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/widget.tsx
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 vp4jl-0.1.2/src/__tests__/vp4jl.spec.ts
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 vp4jl-0.1.2/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 vp4jl-0.1.2/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vp4jl-0.1.2/style/index.js
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 vp4jl-0.1.2/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vp4jl-0.1.2/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 vp4jl-0.1.2/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 vp4jl-0.1.2/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   163960 2020-02-02 00:00:00.000000 vp4jl-0.1.2/ui-tests/yarn.lock
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 vp4jl-0.1.2/ui-tests/tests/vp4jl.spec.ts
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/_version.py
--rw-r--r--   0        0        0     8391 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/handlers.py
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/package.json
--rw-r--r--   0        0        0  2082557 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/126.66641eda4dd704d1f1cc.js
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/126.66641eda4dd704d1f1cc.js.LICENSE.txt
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/155.7f405a8095cea8450e9e.js
--rw-r--r--   0        0        0    22134 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/313.f952284afa306d64a9ff.js
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/518.cee0296c9bdfd0eb851d.js
--rw-r--r--   0        0        0    27416 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/539.fd29c917c181658da4cd.js
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/65.c0057cf84a674e7da6d5.js
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/747.5f00b4009d5740253210.js
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/86.aba30179e86367171d7c.js
--rw-r--r--   0        0        0    79068 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/917.da6458362024da3a7c97.js
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/remoteEntry.94e82f91fd69704b4c87.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/style.js
--rw-r--r--   0        0        0    63046 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/nodeextension/imageio.json
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/tests/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/tests/test_handlers.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/vp_nodes/module.json
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/vp_nodes/package1/__init__.json
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/vp_nodes/package1/module1.json
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/vp_nodes/package1/Level2/__init__.json
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/vp_nodes/package1/Level2/module2.json
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 vp4jl-0.1.2/vp4jl/vp_nodes/package1/Level2/Level3/module3.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 vp4jl-0.1.2/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 vp4jl-0.1.2/LICENSE
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 vp4jl-0.1.2/README.md
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 vp4jl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 vp4jl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vp4jl-0.1.3/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 vp4jl-0.1.3/.yarnrc.yml
+-rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 vp4jl-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 vp4jl-0.1.3/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 vp4jl-0.1.3/babel.config.js
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 vp4jl-0.1.3/conftest.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 vp4jl-0.1.3/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 vp4jl-0.1.3/jest.config.js
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 vp4jl-0.1.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 vp4jl-0.1.3/setup.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 vp4jl-0.1.3/tsconfig.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 vp4jl-0.1.3/tsconfig.test.json
+-rw-r--r--   0        0        0   421990 2020-02-02 00:00:00.000000 vp4jl-0.1.3/yarn.lock
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 vp4jl-0.1.3/jupyter-config/nb-config/vp4jl.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 vp4jl-0.1.3/jupyter-config/server-config/vp4jl.json
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/context.ts
+-rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/index.ts
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/model-factory.ts
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/model.ts
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/namepace.ts
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/node-extension.tsx
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/request-token.ts
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/request.ts
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/toolbar-factory.ts
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/tracker.ts
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/utils.ts
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/widget-factory.ts
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/widget.tsx
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 vp4jl-0.1.3/src/__tests__/vp4jl.spec.ts
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 vp4jl-0.1.3/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 vp4jl-0.1.3/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 vp4jl-0.1.3/style/index.js
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 vp4jl-0.1.3/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vp4jl-0.1.3/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 vp4jl-0.1.3/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 vp4jl-0.1.3/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   163960 2020-02-02 00:00:00.000000 vp4jl-0.1.3/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 vp4jl-0.1.3/ui-tests/tests/vp4jl.spec.ts
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/_version.py
+-rw-r--r--   0        0        0     8391 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/handlers.py
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/package.json
+-rw-r--r--   0        0        0  2082928 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/126.7c83d19240dcfaf4c488.js
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/126.7c83d19240dcfaf4c488.js.LICENSE.txt
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/155.7f405a8095cea8450e9e.js
+-rw-r--r--   0        0        0    22134 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/313.71d37862fe3c5f967528.js
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/518.cee0296c9bdfd0eb851d.js
+-rw-r--r--   0        0        0    27416 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/539.fd29c917c181658da4cd.js
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/65.c0057cf84a674e7da6d5.js
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/747.5f00b4009d5740253210.js
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/86.aba30179e86367171d7c.js
+-rw-r--r--   0        0        0    79068 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/917.da6458362024da3a7c97.js
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/remoteEntry.ca5757684c444f3550a8.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/style.js
+-rw-r--r--   0        0        0    63046 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/nodeextension/imageio.json
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/tests/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/tests/test_handlers.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/vp_nodes/module.json
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/vp_nodes/package1/__init__.json
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/vp_nodes/package1/module1.json
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/vp_nodes/package1/Level2/__init__.json
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/vp_nodes/package1/Level2/module2.json
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 vp4jl-0.1.3/vp4jl/vp_nodes/package1/Level2/Level3/module3.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 vp4jl-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 vp4jl-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 vp4jl-0.1.3/README.md
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 vp4jl-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 vp4jl-0.1.3/PKG-INFO
```

### Comparing `vp4jl-0.1.2/CHANGELOG.md` & `vp4jl-0.1.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.3
+
+([Full Changelog](https://github.com/Max-ChenFei/VisualProgramming4JupyterLab/compare/v0.1.2...1a66fb4a0938eb1e0d4b8d986595f698db398dda))
+
+### Bugs fixed
+
+- Fix/kernel selection when reboot [#108](https://github.com/Max-ChenFei/VisualProgramming4JupyterLab/pull/108) ([@Max-ChenFei](https://github.com/Max-ChenFei))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/Max-ChenFei/VisualProgramming4JupyterLab/graphs/contributors?from=2023-08-04&to=2023-08-05&type=c))
+
+[@Max-ChenFei](https://github.com/search?q=repo%3AMax-ChenFei%2FVisualProgramming4JupyterLab+involves%3AMax-ChenFei+updated%3A2023-08-04..2023-08-05&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.1.2
 
 ([Full Changelog](https://github.com/Max-ChenFei/VisualProgramming4JupyterLab/compare/v0.1.1...0b58e4bc4ad0b53bd2a65b84f1a1f7edc38266d3))
 
 ### Enhancements made
 
 - Cleanup [#105](https://github.com/Max-ChenFei/VisualProgramming4JupyterLab/pull/105) ([@Max-ChenFei](https://github.com/Max-ChenFei))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/Max-ChenFei/VisualProgramming4JupyterLab/graphs/contributors?from=2023-08-04&to=2023-08-04&type=c))
 
 [@Max-ChenFei](https://github.com/search?q=repo%3AMax-ChenFei%2FVisualProgramming4JupyterLab+involves%3AMax-ChenFei+updated%3A2023-08-04..2023-08-04&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.1
 
 ([Full Changelog](https://github.com/Max-ChenFei/VisualProgramming4JupyterLab/compare/308159c55b7a3512b4286d71f3acf96b87c20435...4151f7b1b7427d82dca5f0673b0f762d3ca2150e))
 
 ### Enhancements made
 
 - Fix/node library management [#89](https://github.com/Max-ChenFei/VisualProgramming4JupyterLab/pull/89) ([@Max-ChenFei](https://github.com/Max-ChenFei))
```

### Comparing `vp4jl-0.1.2/RELEASE.md` & `vp4jl-0.1.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/jest.config.js` & `vp4jl-0.1.3/jest.config.js`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/package.json` & `vp4jl-0.1.3/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785539215686274%*

 * *Differences: {"'dependencies'": "{'visual-programming-editor': '^8.5.1'}", "'version'": "'0.1.3'"}*

```diff
@@ -18,15 +18,15 @@
         "filepond": "^4.30.4",
         "react": "^18.2.0",
         "react-dom": "^18.2.0",
         "react-filepond": "^7.1.2",
         "reactflow": "^11.7.0",
         "stream": "^0.0.2",
         "util": "^0.12.5",
-        "visual-programming-editor": "^8.5.0",
+        "visual-programming-editor": "^8.5.1",
         "yjs": "^13.5.40"
     },
     "description": "The JupyterLab extension providing node based visual programming environment",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
         "@jupyterlab/builder": "^4.0.0-beta.0",
@@ -203,9 +203,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `vp4jl-0.1.2/tsconfig.json` & `vp4jl-0.1.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/yarn.lock` & `vp4jl-0.1.3/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1519,23 +1519,23 @@
     "@codemirror/language": ^6.0.0
     "@lezer/rust": ^1.0.0
   checksum: 8a439944cb22159b0b3465ca4fa4294c69843219d5d30e278ae6df8e48f30a7a9256129723c025ec9b5e694d31a3560fb004300b125ffcd81c22d13825845170
   languageName: node
   linkType: hard
 
 "@codemirror/lang-sql@npm:^6.4.1":
-  version: 6.5.2
-  resolution: "@codemirror/lang-sql@npm:6.5.2"
+  version: 6.5.3
+  resolution: "@codemirror/lang-sql@npm:6.5.3"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 29c7f3245271e50707939946e0aa3bae36d2fc392281c5a44bed38c886a5709611a8c68494d1f21c854dd70771ddb2cff2f0f26221b031653278ba2d5678a2b8
+  checksum: dce286eeecf306615a063046bb74d366d840ce3f61f84c08ffb7595f338675c32ada689592446ff61ab2fb0e8c3c011d0558289ee29a98ea3b47717da9beb00a
   languageName: node
   linkType: hard
 
 "@codemirror/lang-wast@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-wast@npm:6.0.1"
   dependencies:
@@ -4006,17 +4006,17 @@
   version: 1.2.2
   resolution: "@types/minimist@npm:1.2.2"
   checksum: b8da83c66eb4aac0440e64674b19564d9d86c80ae273144db9681e5eeff66f238ade9515f5006ffbfa955ceff8b89ad2bd8ec577d7caee74ba101431fb07045d
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 20.4.7
-  resolution: "@types/node@npm:20.4.7"
-  checksum: a40d7003f66b56220a2028179e49f950b46fa6dbf860a4a6ecbd6ba7976f05b2f0b31ced39689ec88a7d9e32d07e088c6a06d270b99d5bc13a28291ac2f30ca7
+  version: 20.4.8
+  resolution: "@types/node@npm:20.4.8"
+  checksum: 86a3963c0c7af3410553d1dfa4b018a20b3cb3ab4d8e8ffe27408b6338c5de0374b0bf379bc705da2205b466daa751ccfe062f453ba9bde34fdb0e5163ca6a68
   languageName: node
   linkType: hard
 
 "@types/normalize-package-data@npm:^2.4.0":
   version: 2.4.1
   resolution: "@types/normalize-package-data@npm:2.4.1"
   checksum: e87bccbf11f95035c89a132b52b79ce69a1e3652fe55962363063c9c0dae0fe2477ebc585e03a9652adc6f381d24ba5589cc5e51849df4ced3d3e004a7d40ed5
@@ -7071,20 +7071,20 @@
     ci-info: ^2.0.0
   bin:
     is-ci: bin.js
   checksum: 77b869057510f3efa439bbb36e9be429d53b3f51abd4776eeea79ab3b221337fe1753d1e50058a9e2c650d38246108beffb15ccfd443929d77748d8c0cc90144
   languageName: node
   linkType: hard
 
-"is-core-module@npm:^2.11.0, is-core-module@npm:^2.5.0":
-  version: 2.12.1
-  resolution: "is-core-module@npm:2.12.1"
+"is-core-module@npm:^2.13.0, is-core-module@npm:^2.5.0":
+  version: 2.13.0
+  resolution: "is-core-module@npm:2.13.0"
   dependencies:
     has: ^1.0.3
-  checksum: f04ea30533b5e62764e7b2e049d3157dc0abd95ef44275b32489ea2081176ac9746ffb1cdb107445cf1ff0e0dfcad522726ca27c27ece64dadf3795428b8e468
+  checksum: 053ab101fb390bfeb2333360fd131387bed54e476b26860dc7f5a700bbf34a0ec4454f7c8c4d43e8a0030957e4b3db6e16d35e1890ea6fb654c833095e040355
   languageName: node
   linkType: hard
 
 "is-date-object@npm:^1.0.1":
   version: 1.0.5
   resolution: "is-date-object@npm:1.0.5"
   dependencies:
@@ -8326,19 +8326,19 @@
   version: 4.3.0
   resolution: "map-obj@npm:4.3.0"
   checksum: fbc554934d1a27a1910e842bc87b177b1a556609dd803747c85ece420692380827c6ae94a95cce4407c054fa0964be3bf8226f7f2cb2e9eeee432c7c1985684e
   languageName: node
   linkType: hard
 
 "markdown-to-jsx@npm:^7.2.1":
-  version: 7.3.1
-  resolution: "markdown-to-jsx@npm:7.3.1"
+  version: 7.3.2
+  resolution: "markdown-to-jsx@npm:7.3.2"
   peerDependencies:
     react: ">= 0.14.0"
-  checksum: 280545b5c1a6aa730817c2d11b2c1dfc80470fbc4f33430b6f705d3dc70aab4d2c79e326ce59f018d2c9cc0face34d21a80067767e053189c729e51ebc9801fb
+  checksum: 8885c6343b71570b0a7ec16cd85a49b853a830234790ee7430e2517ea5d8d361ff138bd52147f650790f3e7b3a28a15c755fc16f8856dd01ddf09a6161782e06
   languageName: node
   linkType: hard
 
 "mathml-tag-names@npm:^2.1.3":
   version: 2.1.3
   resolution: "mathml-tag-names@npm:2.1.3"
   checksum: 1201a25a137d6b9e328facd67912058b8b45b19a6c4cc62641c9476195da28a275ca6e0eca070af5378b905c2b11abc1114676ba703411db0b9ce007de921ad0
@@ -9592,36 +9592,36 @@
   version: 2.0.2
   resolution: "resolve.exports@npm:2.0.2"
   checksum: 1c7778ca1b86a94f8ab4055d196c7d87d1874b96df4d7c3e67bbf793140f0717fd506dcafd62785b079cd6086b9264424ad634fb904409764c3509c3df1653f2
   languageName: node
   linkType: hard
 
 "resolve@npm:^1.10.0, resolve@npm:^1.14.2, resolve@npm:^1.19.0, resolve@npm:^1.20.0":
-  version: 1.22.2
-  resolution: "resolve@npm:1.22.2"
+  version: 1.22.4
+  resolution: "resolve@npm:1.22.4"
   dependencies:
-    is-core-module: ^2.11.0
+    is-core-module: ^2.13.0
     path-parse: ^1.0.7
     supports-preserve-symlinks-flag: ^1.0.0
   bin:
     resolve: bin/resolve
-  checksum: 7e5df75796ebd429445d102d5824482ee7e567f0070b2b45897b29bb4f613dcbc262e0257b8aeedb3089330ccaea0d6a0464df1a77b2992cf331dcda0f4cb549
+  checksum: 23f25174c2736ce24c6d918910e0d1f89b6b38fefa07a995dff864acd7863d59a7f049e691f93b4b2ee29696303390d921552b6d1b841ed4a8101f517e1d0124
   languageName: node
   linkType: hard
 
 "resolve@patch:resolve@^1.10.0#~builtin<compat/resolve>, resolve@patch:resolve@^1.14.2#~builtin<compat/resolve>, resolve@patch:resolve@^1.19.0#~builtin<compat/resolve>, resolve@patch:resolve@^1.20.0#~builtin<compat/resolve>":
-  version: 1.22.2
-  resolution: "resolve@patch:resolve@npm%3A1.22.2#~builtin<compat/resolve>::version=1.22.2&hash=c3c19d"
+  version: 1.22.4
+  resolution: "resolve@patch:resolve@npm%3A1.22.4#~builtin<compat/resolve>::version=1.22.4&hash=c3c19d"
   dependencies:
-    is-core-module: ^2.11.0
+    is-core-module: ^2.13.0
     path-parse: ^1.0.7
     supports-preserve-symlinks-flag: ^1.0.0
   bin:
     resolve: bin/resolve
-  checksum: 66cc788f13b8398de18eb4abb3aed90435c84bb8935953feafcf7231ba4cd191b2c10b4a87b1e9681afc34fb138c705f91f7330ff90bfa36f457e5584076a2b8
+  checksum: c45f2545fdc4d21883861b032789e20aa67a2f2692f68da320cc84d5724cd02f2923766c5354b3210897e88f1a7b3d6d2c7c22faeead8eed7078e4c783a444bc
   languageName: node
   linkType: hard
 
 "retry@npm:^0.12.0":
   version: 0.12.0
   resolution: "retry@npm:0.12.0"
   checksum: 623bd7d2e5119467ba66202d733ec3c2e2e26568074923bc0585b6b99db14f357e79bdedb63cab56cec47491c4a0da7e6021a7465ca6dc4f481d3898fdd3158c
@@ -11013,17 +11013,17 @@
 "validate.io-number@npm:^1.0.3":
   version: 1.0.3
   resolution: "validate.io-number@npm:1.0.3"
   checksum: 42418aeb6c969efa745475154fe576809b02eccd0961aad0421b090d6e7a12d23a3e28b0d5dddd2c6347c1a6bdccb82bba5048c716131cd20207244d50e07282
   languageName: node
   linkType: hard
 
-"visual-programming-editor@npm:^8.5.0":
-  version: 8.5.0
-  resolution: "visual-programming-editor@npm:8.5.0"
+"visual-programming-editor@npm:^8.5.1":
+  version: 8.5.1
+  resolution: "visual-programming-editor@npm:8.5.1"
   dependencies:
     "@emotion/react": ^11.10.6
     "@emotion/styled": ^11.10.6
     "@mui/icons-material": ^5.11.11
     "@mui/lab": ^5.0.0-alpha.125
     "@mui/material": ^5.11.15
     elkjs: ^0.8.2
@@ -11035,15 +11035,15 @@
     react-filepond: ^7.1.2
     react-icons: ^4.8.0
     reactflow: ^11.7.4
     toposort: ^2.0.2
   peerDependencies:
     react: ^18.2.0
     react-dom: ^18.2.0
-  checksum: 2bdc53f78f2649f3f72afaff2d4bb1b221b13b35674e7cab502fdb960b73c7d5877e95aacc11d43e37251f0f6fbd0d1df4cb4d8504157730b6e1de440d9785ca
+  checksum: 0267a9c518bf76b1bb4ec8bc154fd59174e49b28a4171251698f68ca5e86a411a03e416d61e5003e89e9848e6e30d9743c188ec1bd1d432a844933fd189c2253
   languageName: node
   linkType: hard
 
 "vp4jl@workspace:.":
   version: 0.0.0-use.local
   resolution: "vp4jl@workspace:."
   dependencies:
@@ -11085,15 +11085,15 @@
     stylelint-config-prettier: ^9.0.4
     stylelint-config-recommended: ^8.0.0
     stylelint-config-standard: ^26.0.0
     stylelint-prettier: ^2.0.0
     ts-jest: ^26.0.0
     typescript: ~5.0.2
     util: ^0.12.5
-    visual-programming-editor: ^8.5.0
+    visual-programming-editor: ^8.5.1
     yjs: ^13.5.40
   languageName: unknown
   linkType: soft
 
 "vscode-jsonrpc@npm:8.1.0, vscode-jsonrpc@npm:^8.0.2":
   version: 8.1.0
   resolution: "vscode-jsonrpc@npm:8.1.0"
```

### Comparing `vp4jl-0.1.2/src/index.ts` & `vp4jl-0.1.3/src/index.ts`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/src/model-factory.ts` & `vp4jl-0.1.3/src/model-factory.ts`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/src/model.ts` & `vp4jl-0.1.3/src/model.ts`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/src/namepace.ts` & `vp4jl-0.1.3/src/namepace.ts`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/src/node-extension.tsx` & `vp4jl-0.1.3/src/node-extension.tsx`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/src/request-token.ts` & `vp4jl-0.1.3/src/request-token.ts`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/src/request.ts` & `vp4jl-0.1.3/src/request.ts`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/src/toolbar-factory.ts` & `vp4jl-0.1.3/src/toolbar-factory.ts`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/src/tracker.ts` & `vp4jl-0.1.3/src/tracker.ts`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/src/widget-factory.ts` & `vp4jl-0.1.3/src/widget-factory.ts`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/src/widget.tsx` & `vp4jl-0.1.3/src/widget.tsx`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/style/base.css` & `vp4jl-0.1.3/style/base.css`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/ui-tests/README.md` & `vp4jl-0.1.3/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/ui-tests/yarn.lock` & `vp4jl-0.1.3/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/ui-tests/tests/vp4jl.spec.ts` & `vp4jl-0.1.3/ui-tests/tests/vp4jl.spec.ts`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/vp4jl/__init__.py` & `vp4jl-0.1.3/vp4jl/__init__.py`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/vp4jl/handlers.py` & `vp4jl-0.1.3/vp4jl/handlers.py`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/vp4jl/labextension/package.json` & `vp4jl-0.1.3/vp4jl/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9781198937908496%*

 * *Differences: {"'dependencies'": "{'visual-programming-editor': '^8.5.1'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ca5757684c444f3550a8.js'}}",*

 * * "'version'": "'0.1.3'"}*

```diff
@@ -18,15 +18,15 @@
         "filepond": "^4.30.4",
         "react": "^18.2.0",
         "react-dom": "^18.2.0",
         "react-filepond": "^7.1.2",
         "reactflow": "^11.7.0",
         "stream": "^0.0.2",
         "util": "^0.12.5",
-        "visual-programming-editor": "^8.5.0",
+        "visual-programming-editor": "^8.5.1",
         "yjs": "^13.5.40"
     },
     "description": "The JupyterLab extension providing node based visual programming environment",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
         "@jupyterlab/builder": "^4.0.0-beta.0",
@@ -125,15 +125,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/Max-ChenFei/VisualProgramming4JupyterLab",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.94e82f91fd69704b4c87.js",
+            "load": "static/remoteEntry.ca5757684c444f3550a8.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "vp4jl"
                 },
@@ -208,9 +208,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `vp4jl-0.1.2/vp4jl/labextension/static/126.66641eda4dd704d1f1cc.js` & `vp4jl-0.1.3/vp4jl/labextension/static/126.7c83d19240dcfaf4c488.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 126.66641eda4dd704d1f1cc.js.LICENSE.txt */
+/*! For license information please see 126.7c83d19240dcfaf4c488.js.LICENSE.txt */
 (self.webpackChunkvp4jl = self.webpackChunkvp4jl || []).push([
     [126, 155], {
         7187: e => {
             "use strict";
             var t, n = "object" == typeof Reflect ? Reflect : null,
                 i = n && "function" == typeof n.apply ? n.apply : function(e, t, n) {
                     return Function.prototype.apply.call(e, t, n)
@@ -9475,15 +9475,15 @@
                     f = l[1],
                     d = (0, r.useState)(!1),
                     b = d[0],
                     p = d[1],
                     g = (0, r.useRef)(null);
                 (0, r.useEffect)((function() {
                     var e, t;
-                    b ? (null === (e = g.current) || void 0 === e || e.focus(), null == c || c(), document.body.style.cursor = "text") : (null === (t = g.current) || void 0 === t || t.blur(), null == s || s()), m(g.current)
+                    b ? (null === (e = g.current) || void 0 === e || e.focus(), null == c || c()) : (null === (t = g.current) || void 0 === t || t.blur(), null == s || s()), m(g.current)
                 }), [b]), (0, r.useEffect)((function() {
                     b !== a && p(!!a)
                 }), []);
                 var m = (0, r.useCallback)((function(e) {
                     e && (e.style.height = "auto", e.style.height = "".concat(e.scrollHeight, "px"))
                 }), []);
                 return (0, i.jsxs)("div", w({
@@ -9491,15 +9491,15 @@
                         width: "100%",
                         height: "100%",
                         fontFamily: "inherit",
                         fontSize: "inherit",
                         border: "0px"
                     },
                     onDoubleClick: function(e) {
-                        p(!0), document.body.style.cursor = "text"
+                        p(!0)
                     }
                 }, {
                     children: [!b && (0, i.jsx)("div", w({
                         style: {
                             width: "100%",
                             wordWrap: "break-word",
                             userSelect: "none",
@@ -9556,15 +9556,15 @@
                     f = h[0],
                     d = h[1],
                     b = (0, r.useRef)(null);
                 return (0, r.useEffect)((function() {
                     var e, t;
                     f ? (null === (e = b.current) || void 0 === e || e.focus({
                         preventScroll: !0
-                    }), null == o || o(), document.body.style.cursor = "text") : (null === (t = b.current) || void 0 === t || t.blur(), null == a || a())
+                    }), null == o || o()) : (null === (t = b.current) || void 0 === t || t.blur(), null == a || a())
                 }), [f]), (0, i.jsxs)("div", w({
                     style: {
                         width: "100%",
                         height: "100%",
                         fontFamily: "inherit",
                         fontSize: "inherit",
                         color: "inherit",
@@ -18814,15 +18814,15 @@
                 var t = e.onChange,
                     n = e.onArrowDownKeyDown,
                     a = (0, r.useState)(!1),
                     c = a[0],
                     s = a[1],
                     u = o().useRef(null);
                 (0, r.useEffect)((function() {
-                    u.current && (u.current.focus(), document.body.style.cursor = "text")
+                    u.current && u.current.focus()
                 }), []);
                 var l = (0, r.useCallback)((function(e) {
                     "ArrowDown" === e.key && (e.preventDefault(), null == n || n(e))
                 }), []);
                 return (0, i.jsx)(bm, {
                     sx: {
                         width: "100%",
@@ -19465,53 +19465,57 @@
                                     var r = k(i, l.handleType, l.handleDataType);
                                     x(i, r)
                                 }
                                 t()
                             }
                         }), []),
                         I = (0, r.useCallback)((function(e, i) {
-                            if (i && !Array.isArray(i.children))
-                                if ("Enter" === e.key && i.configType) {
-                                    var r = null == a ? void 0 : a(i.configType, n);
-                                    if (p() && r) {
-                                        var o = k(r, l.handleType, l.handleDataType);
-                                        x(r, o)
-                                    }
+                            if (i && !Array.isArray(i.children)) {
+                                if ("Enter" === e.key) {
+                                    if (i.configType) {
+                                        var r = null == a ? void 0 : a(i.configType, n);
+                                        if (p() && r) {
+                                            var o = k(r, l.handleType, l.handleDataType);
+                                            x(r, o)
+                                        }
+                                    } else ! function(e, t) {
+                                        var i = e.find((function(e) {
+                                            return e.name === t
+                                        }));
+                                        i && i.action(void 0, void 0, n)
+                                    }(d, i.name);
                                     t()
-                                } else ! function(e, t) {
-                                    var n = e.find((function(e) {
-                                        return e.name === t
-                                    }));
-                                    n && n.action()
-                                }(d, i.name), t()
-                        }), []),
+                                }
+                                "Escape" === e.key && t()
+                            }
+                        }), [d]),
                         C = (0, r.useCallback)((function(e) {
-                            for (var n = [], i = function(e) {
-                                    var i = {
+                            for (var i = [], r = function(e) {
+                                    var r = {
                                         id: e.name,
                                         name: e.name,
                                         tooltip: e.tooltip,
                                         labelIcon: e.labelIcon,
-                                        onClick: function(n, i) {
-                                            t(), e.action(n, i)
+                                        onClick: function(i, r) {
+                                            t(), e.action(i, r, n)
                                         },
                                         rank: e.rank
                                     };
-                                    if (!e.category) return n.push(i), "continue";
-                                    var r = n.find((function(t) {
+                                    if (!e.category) return i.push(r), "continue";
+                                    var o = i.find((function(t) {
                                         return t.name === e.category
                                     }));
-                                    r ? (r.children || (r.children = []), r.children.push(i)) : n.push({
+                                    o ? (o.children || (o.children = []), o.children.push(r)) : i.push({
                                         id: e.category,
                                         name: e.category,
-                                        children: [i],
+                                        children: [r],
                                         rank: e.categoryRank
                                     })
-                                }, r = 0, o = e; r < o.length; r++) i(o[r]);
-                            return n
+                                }, o = 0, a = e; o < a.length; o++) r(a[o]);
+                            return i
                         }), []);
                     return (0, i.jsx)(Qw, w({
                         transitionDuration: 0,
                         onContextMenu: function(e) {
                             e.preventDefault()
                         },
                         open: !0,
@@ -78139,81 +78143,88 @@
                                 return e.nodes[t.source] && e.nodes[t.target]
                             }));
                             var n = JSON.stringify(e);
                             navigator.clipboard.writeText(n).then((function() {
                                 l((function(e) {
                                     var t = {
                                             name: "Paste",
-                                            action: S,
+                                            action: function(e, t, n) {
+                                                S(n ? _s({
+                                                    clientX: n.left,
+                                                    clientY: n.top
+                                                }, i, b) : void 0)
+                                            },
                                             labelIcon: ij,
                                             labelInfo: "Ctrl+V",
                                             tooltip: "Paste from the clipboard"
                                         },
                                         n = e.findIndex((function(e) {
                                             return "Paste" === e.name
                                         }));
                                     return -1 !== n ? (e[n] = t, e) : v(v([], e, !0), [t], !1)
                                 }))
                             })).catch((function(e) {
                                 console.error("Failed to copy: ", e)
                             }))
                         }
                     },
-                    S = function() {
-                        navigator.clipboard.readText().then((function(n) {
-                            var i = JSON.parse(n);
-                            if (null == i ? void 0 : i.hasNodes) {
-                                var r = {},
-                                    o = c(Object.keys(i.nodes).length);
-                                Object.keys(i.nodes).forEach((function(e) {
-                                    var n = i.nodes[e],
-                                        a = o.shift(),
-                                        c = w(w({}, n), {
-                                            id: a,
+                    S = function(n) {
+                        navigator.clipboard.readText().then((function(i) {
+                            var r, o, a = JSON.parse(i);
+                            if (null == a ? void 0 : a.hasNodes) {
+                                var s = {},
+                                    u = c(Object.keys(a.nodes).length),
+                                    l = null !== (r = null == n ? void 0 : n.x) && void 0 !== r ? r : t.current.mouseX,
+                                    h = null !== (o = null == n ? void 0 : n.y) && void 0 !== o ? o : t.current.mouseY;
+                                Object.keys(a.nodes).forEach((function(e) {
+                                    var t = a.nodes[e],
+                                        n = u.shift(),
+                                        i = w(w({}, t), {
+                                            id: n,
                                             selected: !0,
                                             position: {
-                                                x: n.position.x - (i.minX - t.current.mouseX),
-                                                y: n.position.y - (i.minY - t.current.mouseY)
+                                                x: t.position.x - (a.minX - l),
+                                                y: t.position.y - (a.minY - h)
                                             }
                                         });
-                                    r[e] = c
+                                    s[e] = i
                                 }));
-                                var a = i.edges.map((function(e) {
-                                    var t = r[e.source].id,
-                                        n = r[e.target].id;
+                                var f = a.edges.map((function(e) {
+                                    var t = s[e.source].id,
+                                        n = s[e.target].id;
                                     return w(w({}, e), {
                                         id: "e".concat(t, "-").concat(e.sourceHandle, "-").concat(n, "-").concat(e.targetHandle),
                                         selected: !0,
                                         source: t,
                                         target: n
                                     })
                                 }));
-                                Object.values(r).forEach((function(e) {
+                                Object.values(s).forEach((function(e) {
                                     var t, n;
                                     Object.values(null !== (t = e.data.inputs) && void 0 !== t ? t : {}).forEach((function(e) {
                                         e.connection = 0
                                     })), Object.values(null !== (n = e.data.outputs) && void 0 !== n ? n : {}).forEach((function(e) {
                                         e.connection = 0
                                     }))
                                 }));
-                                for (var s = 0, u = a; s < u.length; s++) {
-                                    var l = u[s],
-                                        h = $j(l.source, Object.values(r)),
-                                        f = $j(l.target, Object.values(r));
-                                    if (h && f) {
-                                        var d = h.data.outputs[l.sourceHandle],
-                                            b = f.data.inputs[l.targetHandle];
-                                        d.connection++, b.connection++
+                                for (var d = 0, b = f; d < b.length; d++) {
+                                    var p = b[d],
+                                        g = $j(p.source, Object.values(s)),
+                                        m = $j(p.target, Object.values(s));
+                                    if (g && m) {
+                                        var v = g.data.outputs[p.sourceHandle],
+                                            y = m.data.inputs[p.targetHandle];
+                                        v.connection++, y.connection++
                                     }
                                 }
-                                Object.values(r).forEach((function(e) {
+                                Object.values(s).forEach((function(e) {
                                     "reroute" === e.data.configType && 0 === e.data.inputs.input.connection && 0 === e.data.outputs.output.connection && (e.data.dataType = "any", e.data.inputs.input.dataType = "any", e.data.outputs.output.dataType = "any")
                                 })), e.selectAll(!1), e.addElements({
-                                    newNodes: Object.values(r),
-                                    newEdges: a
+                                    newNodes: Object.values(s),
+                                    newEdges: f
                                 })
                             }
                         })).catch((function(e) {
                             console.error("Failed to paste: ", e)
                         }))
                     },
                     k = (0, r.useCallback)((function(n, i, r, o) {
@@ -79395,26 +79406,33 @@
                         g = b[1],
                         m = (0, r.useState)(!1),
                         v = m[0],
                         y = m[1],
                         E = (0, r.useState)(u.comment),
                         S = E[0],
                         k = E[1],
-                        T = (0, r.useCallback)((function() {
+                        T = null !== (n = null === (t = ks()) || void 0 === t ? void 0 : t.sceneActions) && void 0 !== n ? n : {},
+                        x = T.setNodes,
+                        _ = T.sortZIndexOfComments,
+                        I = (0, r.useCallback)((function() {
                             y(!1)
                         }), []),
-                        x = (0, r.useCallback)((function() {
-                            y(!0)
+                        C = (0, r.useCallback)((function() {
+                            y(!0), u.defaultEditable && (null == x || x((function(e) {
+                                var t = e.map((function(e) {
+                                    return e.id === s && (e.data = w(w({}, e.data), {
+                                        defaultEditable: !1
+                                    })), e
+                                }));
+                                return t
+                            })))
                         }), []),
-                        _ = (0, r.useCallback)((function(e) {
+                        M = (0, r.useCallback)((function(e) {
                             k(e), u.comment = e
-                        }), []),
-                        I = null !== (n = null === (t = ks()) || void 0 === t ? void 0 : t.sceneActions) && void 0 !== n ? n : {},
-                        C = I.setNodes,
-                        M = I.sortZIndexOfComments;
+                        }), []);
                     if (u.width !== f || u.height !== p) {
                         var O = null !== (o = u.width) && void 0 !== o ? o : 250,
                             j = null !== (a = u.height) && void 0 !== a ? a : 150;
                         d(O), g(j);
                         var A = null === (c = l.current) || void 0 === c ? void 0 : c.parentElement;
                         null == A || A.style.setProperty("width", String(O) + "px"), null == A || A.style.setProperty("height", String(j) + "px")
                     }
@@ -79432,36 +79450,36 @@
                             color: "#ffffff00",
                             handleStyle: {
                                 border: "none"
                             },
                             minWidth: 200,
                             minHeight: 100,
                             onResize: function(e, t) {
-                                d(t.width), g(t.height), null == C || C((function(e) {
+                                d(t.width), g(t.height), null == x || x((function(e) {
                                     var n, i = e.map((function(e) {
                                         return e.id === s && (e.data = w(w({}, e.data), {
                                             width: t.width,
                                             height: t.height
                                         })), e
                                     }));
-                                    return null !== (n = null == M ? void 0 : M(i)) && void 0 !== n ? n : i
+                                    return null !== (n = null == _ ? void 0 : _(i)) && void 0 !== n ? n : i
                                 }))
                             }
                         }), (0, i.jsxs)("div", w({
                             style: {
                                 padding: "4px"
                             },
                             className: v ? "node__header node__header--enabled" : "node__header node__header--disabled"
                         }, {
                             children: [(0, i.jsx)(ms, {
                                 text: u.comment,
                                 defaultEditable: u.defaultEditable,
-                                onStartEdit: T,
-                                onStopEdit: x,
-                                onEditChange: _
+                                onStartEdit: I,
+                                onStopEdit: C,
+                                onEditChange: M
                             }), " "]
                         }))]
                     }))
                 })),
                 tA = (0, r.memo)((function(e) {
                     var t = e.id,
                         n = e.data,
@@ -79623,15 +79641,22 @@
                         x = (0, r.useState)(!1),
                         _ = x[0],
                         I = x[1],
                         C = (0, r.useCallback)((function() {
                             I(!1)
                         }), []),
                         M = (0, r.useCallback)((function() {
-                            I(!k)
+                            I(!k), s.defaultEditable && (null == A || A((function(e) {
+                                var t = e.map((function(e) {
+                                    return e.id === c && (e.data = w(w({}, e.data), {
+                                        defaultEditable: !1
+                                    })), e
+                                }));
+                                return t
+                            })))
                         }), [k]),
                         O = (0, r.useCallback)((function(e) {
                             m(e), s.stickyNote = e
                         }), []),
                         j = (0, r.useCallback)((function() {
                             T(!k), I(k)
                         }), [k]),
```

### Comparing `vp4jl-0.1.2/vp4jl/labextension/static/126.66641eda4dd704d1f1cc.js.LICENSE.txt` & `vp4jl-0.1.3/vp4jl/labextension/static/126.7c83d19240dcfaf4c488.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/vp4jl/labextension/static/155.7f405a8095cea8450e9e.js` & `vp4jl-0.1.3/vp4jl/labextension/static/155.7f405a8095cea8450e9e.js`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/vp4jl/labextension/static/313.f952284afa306d64a9ff.js` & `vp4jl-0.1.3/vp4jl/labextension/static/313.71d37862fe3c5f967528.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
                 u = n(8861),
                 m = n(8833),
                 p = n(6029),
                 h = n.n(p),
                 g = n(8778),
                 v = n(3150),
                 C = n(6322),
-                x = n(3446);
+                x = n(5779);
             n(6250);
             class b extends m.ReactWidget {
                 constructor(e, t) {
                     super(), this._editor_activated = !1, this.id = e, this._model = t, this._model.vpContentChanged.connect(this.update, this)
                 }
                 get model() {
                     return this._model
```

### Comparing `vp4jl-0.1.2/vp4jl/labextension/static/539.fd29c917c181658da4cd.js` & `vp4jl-0.1.3/vp4jl/labextension/static/539.fd29c917c181658da4cd.js`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/vp4jl/labextension/static/747.5f00b4009d5740253210.js` & `vp4jl-0.1.3/vp4jl/labextension/static/747.5f00b4009d5740253210.js`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/vp4jl/labextension/static/86.aba30179e86367171d7c.js` & `vp4jl-0.1.3/vp4jl/labextension/static/86.aba30179e86367171d7c.js`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/vp4jl/labextension/static/917.da6458362024da3a7c97.js` & `vp4jl-0.1.3/vp4jl/labextension/static/917.da6458362024da3a7c97.js`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/vp4jl/labextension/static/remoteEntry.94e82f91fd69704b4c87.js` & `vp4jl-0.1.3/vp4jl/labextension/static/remoteEntry.ca5757684c444f3550a8.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -46,29 +46,29 @@
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
         29: "4958014bab8f74fbd1b4",
         65: "c0057cf84a674e7da6d5",
         86: "aba30179e86367171d7c",
-        126: "66641eda4dd704d1f1cc",
+        126: "7c83d19240dcfaf4c488",
         155: "7f405a8095cea8450e9e",
-        313: "f952284afa306d64a9ff",
+        313: "71d37862fe3c5f967528",
         385: "90b7175465d918e4a87d",
         518: "cee0296c9bdfd0eb851d",
         539: "fd29c917c181658da4cd",
         747: "5f00b4009d5740253210",
         917: "da6458362024da3a7c97"
     } [e] + ".js?v=" + {
         29: "4958014bab8f74fbd1b4",
         65: "c0057cf84a674e7da6d5",
         86: "aba30179e86367171d7c",
-        126: "66641eda4dd704d1f1cc",
+        126: "7c83d19240dcfaf4c488",
         155: "7f405a8095cea8450e9e",
-        313: "f952284afa306d64a9ff",
+        313: "71d37862fe3c5f967528",
         385: "90b7175465d918e4a87d",
         518: "cee0296c9bdfd0eb851d",
         539: "fd29c917c181658da4cd",
         747: "5f00b4009d5740253210",
         917: "da6458362024da3a7c97"
     } [e], x.g = function() {
         if ("object" == typeof globalThis) return globalThis;
@@ -125,15 +125,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("stream", "0.0.2", (() => x.e(86).then((() => () => x(3086))))), l("util", "0.12.5", (() => Promise.all([x.e(539), x.e(155)]).then((() => () => x(9539))))), l("visual-programming-editor", "8.5.0", (() => Promise.all([x.e(126), x.e(385), x.e(29), x.e(518)]).then((() => () => x(1126))))), l("vp4jl", "0.1.2", (() => Promise.all([x.e(917), x.e(29), x.e(313)]).then((() => () => x(9137)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("stream", "0.0.2", (() => x.e(86).then((() => () => x(3086))))), l("util", "0.12.5", (() => Promise.all([x.e(539), x.e(155)]).then((() => () => x(9539))))), l("visual-programming-editor", "8.5.1", (() => Promise.all([x.e(126), x.e(385), x.e(29), x.e(518)]).then((() => () => x(1126))))), l("vp4jl", "0.1.3", (() => Promise.all([x.e(917), x.e(29), x.e(313)]).then((() => () => x(9137)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -247,21 +247,21 @@
     })), w = {}, P = {
         6029: () => y("default", "react", [1, 18, 2, 0]),
         255: () => y("default", "@jupyterlab/services", [1, 7, 0, 4]),
         731: () => y("default", "@jupyterlab/statedb", [1, 4, 0, 4]),
         2196: () => y("default", "@jupyterlab/statusbar", [1, 4, 0, 4]),
         2385: () => y("default", "@jupyterlab/launcher", [1, 4, 0, 4]),
         3150: () => g("default", "@jupyterlab/docregistry", [1, 4, 0, 4]),
-        3446: () => j("default", "visual-programming-editor", [1, 8, 5, 0], (() => Promise.all([x.e(126), x.e(385), x.e(65)]).then((() => () => x(1126))))),
         4151: () => y("default", "@jupyterlab/coreutils", [1, 6, 0, 4]),
         4543: () => y("default", "@jupyterlab/notebook", [1, 4, 0, 4]),
         4664: () => y("default", "@jupyterlab/mainmenu", [1, 4, 0, 4]),
         4901: () => y("default", "@lumino/signaling", [1, 2, 0, 0]),
         5623: () => g("default", "@jupyterlab/docmanager-extension", [1, 4, 0, 4]),
         5633: () => y("default", "@lumino/messaging", [1, 2, 0, 0]),
+        5779: () => j("default", "visual-programming-editor", [1, 8, 5, 1], (() => Promise.all([x.e(126), x.e(385), x.e(65)]).then((() => () => x(1126))))),
         6322: () => g("default", "@jupyterlab/outputarea", [1, 4, 0, 4]),
         6697: () => y("default", "@lumino/algorithm", [1, 2, 0, 0]),
         7930: () => y("default", "@lumino/coreutils", [1, 2, 0, 0]),
         8035: () => y("default", "@jupyterlab/ui-components", [1, 4, 0, 4]),
         8220: () => y("default", "@jupyterlab/application", [1, 4, 0, 4]),
         8314: () => y("default", "@jupyterlab/translation", [1, 4, 0, 4]),
         8778: () => y("default", "@lumino/widgets", [1, 2, 0, 1]),
@@ -269,15 +269,15 @@
         8861: () => y("default", "@jupyterlab/rendermime", [1, 4, 0, 4]),
         8905: () => y("default", "@jupyterlab/filebrowser", [1, 4, 0, 4]),
         150: () => m("default", "stream", (() => x.e(86).then((() => () => x(3086))))),
         7704: () => y("default", "react-dom", [1, 18, 2, 0]),
         8538: () => m("default", "util", (() => x.e(539).then((() => () => x(9539)))))
     }, S = {
         29: [6029],
-        313: [255, 731, 2196, 2385, 3150, 3446, 4151, 4543, 4664, 4901, 5623, 5633, 6322, 6697, 7930, 8035, 8220, 8314, 8778, 8833, 8861, 8905],
+        313: [255, 731, 2196, 2385, 3150, 4151, 4543, 4664, 4901, 5623, 5633, 5779, 6322, 6697, 7930, 8035, 8220, 8314, 8778, 8833, 8861, 8905],
         385: [150, 7704, 8538]
     }, x.f.consumes = (e, r) => {
         x.o(S, e) && S[e].forEach((e => {
             if (x.o(w, e)) return r.push(w[e]);
             var t = r => {
                     w[e] = 0, x.m[e] = t => {
                         delete x.c[e], t.exports = r()
```

### Comparing `vp4jl-0.1.2/vp4jl/labextension/static/third-party-licenses.json` & `vp4jl-0.1.3/vp4jl/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975961538461539%*

 * *Differences: {"'packages'": "{24: {'versionInfo': '8.5.1'}}"}*

```diff
@@ -144,15 +144,15 @@
             "name": "util",
             "versionInfo": "0.12.5"
         },
         {
             "extractedText": "                    GNU GENERAL PUBLIC LICENSE\n                       Version 3, 29 June 2007\n\n Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>\n Everyone is permitted to copy and distribute verbatim copies\n of this license document, but changing it is not allowed.\n\n                            Preamble\n\n  The GNU General Public License is a free, copyleft license for\nsoftware and other kinds of works.\n\n  The licenses for most software and other practical works are designed\nto take away your freedom to share and change the works.  By contrast,\nthe GNU General Public License is intended to guarantee your freedom to\nshare and change all versions of a program--to make sure it remains free\nsoftware for all its users.  We, the Free Software Foundation, use the\nGNU General Public License for most of our software; it applies also to\nany other work released this way by its authors.  You can apply it to\nyour programs, too.\n\n  When we speak of free software, we are referring to freedom, not\nprice.  Our General Public Licenses are designed to make sure that you\nhave the freedom to distribute copies of free software (and charge for\nthem if you wish), that you receive source code or can get it if you\nwant it, that you can change the software or use pieces of it in new\nfree programs, and that you know you can do these things.\n\n  To protect your rights, we need to prevent others from denying you\nthese rights or asking you to surrender the rights.  Therefore, you have\ncertain responsibilities if you distribute copies of the software, or if\nyou modify it: responsibilities to respect the freedom of others.\n\n  For example, if you distribute copies of such a program, whether\ngratis or for a fee, you must pass on to the recipients the same\nfreedoms that you received.  You must make sure that they, too, receive\nor can get the source code.  And you must show them these terms so they\nknow their rights.\n\n  Developers that use the GNU GPL protect your rights with two steps:\n(1) assert copyright on the software, and (2) offer you this License\ngiving you legal permission to copy, distribute and/or modify it.\n\n  For the developers' and authors' protection, the GPL clearly explains\nthat there is no warranty for this free software.  For both users' and\nauthors' sake, the GPL requires that modified versions be marked as\nchanged, so that their problems will not be attributed erroneously to\nauthors of previous versions.\n\n  Some devices are designed to deny users access to install or run\nmodified versions of the software inside them, although the manufacturer\ncan do so.  This is fundamentally incompatible with the aim of\nprotecting users' freedom to change the software.  The systematic\npattern of such abuse occurs in the area of products for individuals to\nuse, which is precisely where it is most unacceptable.  Therefore, we\nhave designed this version of the GPL to prohibit the practice for those\nproducts.  If such problems arise substantially in other domains, we\nstand ready to extend this provision to those domains in future versions\nof the GPL, as needed to protect the freedom of users.\n\n  Finally, every program is threatened constantly by software patents.\nStates should not allow patents to restrict development and use of\nsoftware on general-purpose computers, but in those that do, we wish to\navoid the special danger that patents applied to a free program could\nmake it effectively proprietary.  To prevent this, the GPL assures that\npatents cannot be used to render the program non-free.\n\n  The precise terms and conditions for copying, distribution and\nmodification follow.\n\n                       TERMS AND CONDITIONS\n\n  0. Definitions.\n\n  \"This License\" refers to version 3 of the GNU General Public License.\n\n  \"Copyright\" also means copyright-like laws that apply to other kinds of\nworks, such as semiconductor masks.\n\n  \"The Program\" refers to any copyrightable work licensed under this\nLicense.  Each licensee is addressed as \"you\".  \"Licensees\" and\n\"recipients\" may be individuals or organizations.\n\n  To \"modify\" a work means to copy from or adapt all or part of the work\nin a fashion requiring copyright permission, other than the making of an\nexact copy.  The resulting work is called a \"modified version\" of the\nearlier work or a work \"based on\" the earlier work.\n\n  A \"covered work\" means either the unmodified Program or a work based\non the Program.\n\n  To \"propagate\" a work means to do anything with it that, without\npermission, would make you directly or secondarily liable for\ninfringement under applicable copyright law, except executing it on a\ncomputer or modifying a private copy.  Propagation includes copying,\ndistribution (with or without modification), making available to the\npublic, and in some countries other activities as well.\n\n  To \"convey\" a work means any kind of propagation that enables other\nparties to make or receive copies.  Mere interaction with a user through\na computer network, with no transfer of a copy, is not conveying.\n\n  An interactive user interface displays \"Appropriate Legal Notices\"\nto the extent that it includes a convenient and prominently visible\nfeature that (1) displays an appropriate copyright notice, and (2)\ntells the user that there is no warranty for the work (except to the\nextent that warranties are provided), that licensees may convey the\nwork under this License, and how to view a copy of this License.  If\nthe interface presents a list of user commands or options, such as a\nmenu, a prominent item in the list meets this criterion.\n\n  1. Source Code.\n\n  The \"source code\" for a work means the preferred form of the work\nfor making modifications to it.  \"Object code\" means any non-source\nform of a work.\n\n  A \"Standard Interface\" means an interface that either is an official\nstandard defined by a recognized standards body, or, in the case of\ninterfaces specified for a particular programming language, one that\nis widely used among developers working in that language.\n\n  The \"System Libraries\" of an executable work include anything, other\nthan the work as a whole, that (a) is included in the normal form of\npackaging a Major Component, but which is not part of that Major\nComponent, and (b) serves only to enable use of the work with that\nMajor Component, or to implement a Standard Interface for which an\nimplementation is available to the public in source code form.  A\n\"Major Component\", in this context, means a major essential component\n(kernel, window system, and so on) of the specific operating system\n(if any) on which the executable work runs, or a compiler used to\nproduce the work, or an object code interpreter used to run it.\n\n  The \"Corresponding Source\" for a work in object code form means all\nthe source code needed to generate, install, and (for an executable\nwork) run the object code and to modify the work, including scripts to\ncontrol those activities.  However, it does not include the work's\nSystem Libraries, or general-purpose tools or generally available free\nprograms which are used unmodified in performing those activities but\nwhich are not part of the work.  For example, Corresponding Source\nincludes interface definition files associated with source files for\nthe work, and the source code for shared libraries and dynamically\nlinked subprograms that the work is specifically designed to require,\nsuch as by intimate data communication or control flow between those\nsubprograms and other parts of the work.\n\n  The Corresponding Source need not include anything that users\ncan regenerate automatically from other parts of the Corresponding\nSource.\n\n  The Corresponding Source for a work in source code form is that\nsame work.\n\n  2. Basic Permissions.\n\n  All rights granted under this License are granted for the term of\ncopyright on the Program, and are irrevocable provided the stated\nconditions are met.  This License explicitly affirms your unlimited\npermission to run the unmodified Program.  The output from running a\ncovered work is covered by this License only if the output, given its\ncontent, constitutes a covered work.  This License acknowledges your\nrights of fair use or other equivalent, as provided by copyright law.\n\n  You may make, run and propagate covered works that you do not\nconvey, without conditions so long as your license otherwise remains\nin force.  You may convey covered works to others for the sole purpose\nof having them make modifications exclusively for you, or provide you\nwith facilities for running those works, provided that you comply with\nthe terms of this License in conveying all material for which you do\nnot control copyright.  Those thus making or running the covered works\nfor you must do so exclusively on your behalf, under your direction\nand control, on terms that prohibit them from making any copies of\nyour copyrighted material outside their relationship with you.\n\n  Conveying under any other circumstances is permitted solely under\nthe conditions stated below.  Sublicensing is not allowed; section 10\nmakes it unnecessary.\n\n  3. Protecting Users' Legal Rights From Anti-Circumvention Law.\n\n  No covered work shall be deemed part of an effective technological\nmeasure under any applicable law fulfilling obligations under article\n11 of the WIPO copyright treaty adopted on 20 December 1996, or\nsimilar laws prohibiting or restricting circumvention of such\nmeasures.\n\n  When you convey a covered work, you waive any legal power to forbid\ncircumvention of technological measures to the extent such circumvention\nis effected by exercising rights under this License with respect to\nthe covered work, and you disclaim any intention to limit operation or\nmodification of the work as a means of enforcing, against the work's\nusers, your or third parties' legal rights to forbid circumvention of\ntechnological measures.\n\n  4. Conveying Verbatim Copies.\n\n  You may convey verbatim copies of the Program's source code as you\nreceive it, in any medium, provided that you conspicuously and\nappropriately publish on each copy an appropriate copyright notice;\nkeep intact all notices stating that this License and any\nnon-permissive terms added in accord with section 7 apply to the code;\nkeep intact all notices of the absence of any warranty; and give all\nrecipients a copy of this License along with the Program.\n\n  You may charge any price or no price for each copy that you convey,\nand you may offer support or warranty protection for a fee.\n\n  5. Conveying Modified Source Versions.\n\n  You may convey a work based on the Program, or the modifications to\nproduce it from the Program, in the form of source code under the\nterms of section 4, provided that you also meet all of these conditions:\n\n    a) The work must carry prominent notices stating that you modified\n    it, and giving a relevant date.\n\n    b) The work must carry prominent notices stating that it is\n    released under this License and any conditions added under section\n    7.  This requirement modifies the requirement in section 4 to\n    \"keep intact all notices\".\n\n    c) You must license the entire work, as a whole, under this\n    License to anyone who comes into possession of a copy.  This\n    License will therefore apply, along with any applicable section 7\n    additional terms, to the whole of the work, and all its parts,\n    regardless of how they are packaged.  This License gives no\n    permission to license the work in any other way, but it does not\n    invalidate such permission if you have separately received it.\n\n    d) If the work has interactive user interfaces, each must display\n    Appropriate Legal Notices; however, if the Program has interactive\n    interfaces that do not display Appropriate Legal Notices, your\n    work need not make them do so.\n\n  A compilation of a covered work with other separate and independent\nworks, which are not by their nature extensions of the covered work,\nand which are not combined with it such as to form a larger program,\nin or on a volume of a storage or distribution medium, is called an\n\"aggregate\" if the compilation and its resulting copyright are not\nused to limit the access or legal rights of the compilation's users\nbeyond what the individual works permit.  Inclusion of a covered work\nin an aggregate does not cause this License to apply to the other\nparts of the aggregate.\n\n  6. Conveying Non-Source Forms.\n\n  You may convey a covered work in object code form under the terms\nof sections 4 and 5, provided that you also convey the\nmachine-readable Corresponding Source under the terms of this License,\nin one of these ways:\n\n    a) Convey the object code in, or embodied in, a physical product\n    (including a physical distribution medium), accompanied by the\n    Corresponding Source fixed on a durable physical medium\n    customarily used for software interchange.\n\n    b) Convey the object code in, or embodied in, a physical product\n    (including a physical distribution medium), accompanied by a\n    written offer, valid for at least three years and valid for as\n    long as you offer spare parts or customer support for that product\n    model, to give anyone who possesses the object code either (1) a\n    copy of the Corresponding Source for all the software in the\n    product that is covered by this License, on a durable physical\n    medium customarily used for software interchange, for a price no\n    more than your reasonable cost of physically performing this\n    conveying of source, or (2) access to copy the\n    Corresponding Source from a network server at no charge.\n\n    c) Convey individual copies of the object code with a copy of the\n    written offer to provide the Corresponding Source.  This\n    alternative is allowed only occasionally and noncommercially, and\n    only if you received the object code with such an offer, in accord\n    with subsection 6b.\n\n    d) Convey the object code by offering access from a designated\n    place (gratis or for a charge), and offer equivalent access to the\n    Corresponding Source in the same way through the same place at no\n    further charge.  You need not require recipients to copy the\n    Corresponding Source along with the object code.  If the place to\n    copy the object code is a network server, the Corresponding Source\n    may be on a different server (operated by you or a third party)\n    that supports equivalent copying facilities, provided you maintain\n    clear directions next to the object code saying where to find the\n    Corresponding Source.  Regardless of what server hosts the\n    Corresponding Source, you remain obligated to ensure that it is\n    available for as long as needed to satisfy these requirements.\n\n    e) Convey the object code using peer-to-peer transmission, provided\n    you inform other peers where the object code and Corresponding\n    Source of the work are being offered to the general public at no\n    charge under subsection 6d.\n\n  A separable portion of the object code, whose source code is excluded\nfrom the Corresponding Source as a System Library, need not be\nincluded in conveying the object code work.\n\n  A \"User Product\" is either (1) a \"consumer product\", which means any\ntangible personal property which is normally used for personal, family,\nor household purposes, or (2) anything designed or sold for incorporation\ninto a dwelling.  In determining whether a product is a consumer product,\ndoubtful cases shall be resolved in favor of coverage.  For a particular\nproduct received by a particular user, \"normally used\" refers to a\ntypical or common use of that class of product, regardless of the status\nof the particular user or of the way in which the particular user\nactually uses, or expects or is expected to use, the product.  A product\nis a consumer product regardless of whether the product has substantial\ncommercial, industrial or non-consumer uses, unless such uses represent\nthe only significant mode of use of the product.\n\n  \"Installation Information\" for a User Product means any methods,\nprocedures, authorization keys, or other information required to install\nand execute modified versions of a covered work in that User Product from\na modified version of its Corresponding Source.  The information must\nsuffice to ensure that the continued functioning of the modified object\ncode is in no case prevented or interfered with solely because\nmodification has been made.\n\n  If you convey an object code work under this section in, or with, or\nspecifically for use in, a User Product, and the conveying occurs as\npart of a transaction in which the right of possession and use of the\nUser Product is transferred to the recipient in perpetuity or for a\nfixed term (regardless of how the transaction is characterized), the\nCorresponding Source conveyed under this section must be accompanied\nby the Installation Information.  But this requirement does not apply\nif neither you nor any third party retains the ability to install\nmodified object code on the User Product (for example, the work has\nbeen installed in ROM).\n\n  The requirement to provide Installation Information does not include a\nrequirement to continue to provide support service, warranty, or updates\nfor a work that has been modified or installed by the recipient, or for\nthe User Product in which it has been modified or installed.  Access to a\nnetwork may be denied when the modification itself materially and\nadversely affects the operation of the network or violates the rules and\nprotocols for communication across the network.\n\n  Corresponding Source conveyed, and Installation Information provided,\nin accord with this section must be in a format that is publicly\ndocumented (and with an implementation available to the public in\nsource code form), and must require no special password or key for\nunpacking, reading or copying.\n\n  7. Additional Terms.\n\n  \"Additional permissions\" are terms that supplement the terms of this\nLicense by making exceptions from one or more of its conditions.\nAdditional permissions that are applicable to the entire Program shall\nbe treated as though they were included in this License, to the extent\nthat they are valid under applicable law.  If additional permissions\napply only to part of the Program, that part may be used separately\nunder those permissions, but the entire Program remains governed by\nthis License without regard to the additional permissions.\n\n  When you convey a copy of a covered work, you may at your option\nremove any additional permissions from that copy, or from any part of\nit.  (Additional permissions may be written to require their own\nremoval in certain cases when you modify the work.)  You may place\nadditional permissions on material, added by you to a covered work,\nfor which you have or can give appropriate copyright permission.\n\n  Notwithstanding any other provision of this License, for material you\nadd to a covered work, you may (if authorized by the copyright holders of\nthat material) supplement the terms of this License with terms:\n\n    a) Disclaiming warranty or limiting liability differently from the\n    terms of sections 15 and 16 of this License; or\n\n    b) Requiring preservation of specified reasonable legal notices or\n    author attributions in that material or in the Appropriate Legal\n    Notices displayed by works containing it; or\n\n    c) Prohibiting misrepresentation of the origin of that material, or\n    requiring that modified versions of such material be marked in\n    reasonable ways as different from the original version; or\n\n    d) Limiting the use for publicity purposes of names of licensors or\n    authors of the material; or\n\n    e) Declining to grant rights under trademark law for use of some\n    trade names, trademarks, or service marks; or\n\n    f) Requiring indemnification of licensors and authors of that\n    material by anyone who conveys the material (or modified versions of\n    it) with contractual assumptions of liability to the recipient, for\n    any liability that these contractual assumptions directly impose on\n    those licensors and authors.\n\n  All other non-permissive additional terms are considered \"further\nrestrictions\" within the meaning of section 10.  If the Program as you\nreceived it, or any part of it, contains a notice stating that it is\ngoverned by this License along with a term that is a further\nrestriction, you may remove that term.  If a license document contains\na further restriction but permits relicensing or conveying under this\nLicense, you may add to a covered work material governed by the terms\nof that license document, provided that the further restriction does\nnot survive such relicensing or conveying.\n\n  If you add terms to a covered work in accord with this section, you\nmust place, in the relevant source files, a statement of the\nadditional terms that apply to those files, or a notice indicating\nwhere to find the applicable terms.\n\n  Additional terms, permissive or non-permissive, may be stated in the\nform of a separately written license, or stated as exceptions;\nthe above requirements apply either way.\n\n  8. Termination.\n\n  You may not propagate or modify a covered work except as expressly\nprovided under this License.  Any attempt otherwise to propagate or\nmodify it is void, and will automatically terminate your rights under\nthis License (including any patent licenses granted under the third\nparagraph of section 11).\n\n  However, if you cease all violation of this License, then your\nlicense from a particular copyright holder is reinstated (a)\nprovisionally, unless and until the copyright holder explicitly and\nfinally terminates your license, and (b) permanently, if the copyright\nholder fails to notify you of the violation by some reasonable means\nprior to 60 days after the cessation.\n\n  Moreover, your license from a particular copyright holder is\nreinstated permanently if the copyright holder notifies you of the\nviolation by some reasonable means, this is the first time you have\nreceived notice of violation of this License (for any work) from that\ncopyright holder, and you cure the violation prior to 30 days after\nyour receipt of the notice.\n\n  Termination of your rights under this section does not terminate the\nlicenses of parties who have received copies or rights from you under\nthis License.  If your rights have been terminated and not permanently\nreinstated, you do not qualify to receive new licenses for the same\nmaterial under section 10.\n\n  9. Acceptance Not Required for Having Copies.\n\n  You are not required to accept this License in order to receive or\nrun a copy of the Program.  Ancillary propagation of a covered work\noccurring solely as a consequence of using peer-to-peer transmission\nto receive a copy likewise does not require acceptance.  However,\nnothing other than this License grants you permission to propagate or\nmodify any covered work.  These actions infringe copyright if you do\nnot accept this License.  Therefore, by modifying or propagating a\ncovered work, you indicate your acceptance of this License to do so.\n\n  10. Automatic Licensing of Downstream Recipients.\n\n  Each time you convey a covered work, the recipient automatically\nreceives a license from the original licensors, to run, modify and\npropagate that work, subject to this License.  You are not responsible\nfor enforcing compliance by third parties with this License.\n\n  An \"entity transaction\" is a transaction transferring control of an\norganization, or substantially all assets of one, or subdividing an\norganization, or merging organizations.  If propagation of a covered\nwork results from an entity transaction, each party to that\ntransaction who receives a copy of the work also receives whatever\nlicenses to the work the party's predecessor in interest had or could\ngive under the previous paragraph, plus a right to possession of the\nCorresponding Source of the work from the predecessor in interest, if\nthe predecessor has it or can get it with reasonable efforts.\n\n  You may not impose any further restrictions on the exercise of the\nrights granted or affirmed under this License.  For example, you may\nnot impose a license fee, royalty, or other charge for exercise of\nrights granted under this License, and you may not initiate litigation\n(including a cross-claim or counterclaim in a lawsuit) alleging that\nany patent claim is infringed by making, using, selling, offering for\nsale, or importing the Program or any portion of it.\n\n  11. Patents.\n\n  A \"contributor\" is a copyright holder who authorizes use under this\nLicense of the Program or a work on which the Program is based.  The\nwork thus licensed is called the contributor's \"contributor version\".\n\n  A contributor's \"essential patent claims\" are all patent claims\nowned or controlled by the contributor, whether already acquired or\nhereafter acquired, that would be infringed by some manner, permitted\nby this License, of making, using, or selling its contributor version,\nbut do not include claims that would be infringed only as a\nconsequence of further modification of the contributor version.  For\npurposes of this definition, \"control\" includes the right to grant\npatent sublicenses in a manner consistent with the requirements of\nthis License.\n\n  Each contributor grants you a non-exclusive, worldwide, royalty-free\npatent license under the contributor's essential patent claims, to\nmake, use, sell, offer for sale, import and otherwise run, modify and\npropagate the contents of its contributor version.\n\n  In the following three paragraphs, a \"patent license\" is any express\nagreement or commitment, however denominated, not to enforce a patent\n(such as an express permission to practice a patent or covenant not to\nsue for patent infringement).  To \"grant\" such a patent license to a\nparty means to make such an agreement or commitment not to enforce a\npatent against the party.\n\n  If you convey a covered work, knowingly relying on a patent license,\nand the Corresponding Source of the work is not available for anyone\nto copy, free of charge and under the terms of this License, through a\npublicly available network server or other readily accessible means,\nthen you must either (1) cause the Corresponding Source to be so\navailable, or (2) arrange to deprive yourself of the benefit of the\npatent license for this particular work, or (3) arrange, in a manner\nconsistent with the requirements of this License, to extend the patent\nlicense to downstream recipients.  \"Knowingly relying\" means you have\nactual knowledge that, but for the patent license, your conveying the\ncovered work in a country, or your recipient's use of the covered work\nin a country, would infringe one or more identifiable patents in that\ncountry that you have reason to believe are valid.\n\n  If, pursuant to or in connection with a single transaction or\narrangement, you convey, or propagate by procuring conveyance of, a\ncovered work, and grant a patent license to some of the parties\nreceiving the covered work authorizing them to use, propagate, modify\nor convey a specific copy of the covered work, then the patent license\nyou grant is automatically extended to all recipients of the covered\nwork and works based on it.\n\n  A patent license is \"discriminatory\" if it does not include within\nthe scope of its coverage, prohibits the exercise of, or is\nconditioned on the non-exercise of one or more of the rights that are\nspecifically granted under this License.  You may not convey a covered\nwork if you are a party to an arrangement with a third party that is\nin the business of distributing software, under which you make payment\nto the third party based on the extent of your activity of conveying\nthe work, and under which the third party grants, to any of the\nparties who would receive the covered work from you, a discriminatory\npatent license (a) in connection with copies of the covered work\nconveyed by you (or copies made from those copies), or (b) primarily\nfor and in connection with specific products or compilations that\ncontain the covered work, unless you entered into that arrangement,\nor that patent license was granted, prior to 28 March 2007.\n\n  Nothing in this License shall be construed as excluding or limiting\nany implied license or other defenses to infringement that may\notherwise be available to you under applicable patent law.\n\n  12. No Surrender of Others' Freedom.\n\n  If conditions are imposed on you (whether by court order, agreement or\notherwise) that contradict the conditions of this License, they do not\nexcuse you from the conditions of this License.  If you cannot convey a\ncovered work so as to satisfy simultaneously your obligations under this\nLicense and any other pertinent obligations, then as a consequence you may\nnot convey it at all.  For example, if you agree to terms that obligate you\nto collect a royalty for further conveying from those to whom you convey\nthe Program, the only way you could satisfy both those terms and this\nLicense would be to refrain entirely from conveying the Program.\n\n  13. Use with the GNU Affero General Public License.\n\n  Notwithstanding any other provision of this License, you have\npermission to link or combine any covered work with a work licensed\nunder version 3 of the GNU Affero General Public License into a single\ncombined work, and to convey the resulting work.  The terms of this\nLicense will continue to apply to the part which is the covered work,\nbut the special requirements of the GNU Affero General Public License,\nsection 13, concerning interaction through a network will apply to the\ncombination as such.\n\n  14. Revised Versions of this License.\n\n  The Free Software Foundation may publish revised and/or new versions of\nthe GNU General Public License from time to time.  Such new versions will\nbe similar in spirit to the present version, but may differ in detail to\naddress new problems or concerns.\n\n  Each version is given a distinguishing version number.  If the\nProgram specifies that a certain numbered version of the GNU General\nPublic License \"or any later version\" applies to it, you have the\noption of following the terms and conditions either of that numbered\nversion or of any later version published by the Free Software\nFoundation.  If the Program does not specify a version number of the\nGNU General Public License, you may choose any version ever published\nby the Free Software Foundation.\n\n  If the Program specifies that a proxy can decide which future\nversions of the GNU General Public License can be used, that proxy's\npublic statement of acceptance of a version permanently authorizes you\nto choose that version for the Program.\n\n  Later license versions may give you additional or different\npermissions.  However, no additional obligations are imposed on any\nauthor or copyright holder as a result of your choosing to follow a\nlater version.\n\n  15. Disclaimer of Warranty.\n\n  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY\nAPPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT\nHOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM \"AS IS\" WITHOUT WARRANTY\nOF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,\nTHE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR\nPURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM\nIS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF\nALL NECESSARY SERVICING, REPAIR OR CORRECTION.\n\n  16. Limitation of Liability.\n\n  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING\nWILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS\nTHE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY\nGENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE\nUSE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF\nDATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD\nPARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),\nEVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF\nSUCH DAMAGES.\n\n  17. Interpretation of Sections 15 and 16.\n\n  If the disclaimer of warranty and limitation of liability provided\nabove cannot be given local legal effect according to their terms,\nreviewing courts shall apply local law that most closely approximates\nan absolute waiver of all civil liability in connection with the\nProgram, unless a warranty or assumption of liability accompanies a\ncopy of the Program in return for a fee.\n\n                     END OF TERMS AND CONDITIONS\n\n            How to Apply These Terms to Your New Programs\n\n  If you develop a new program, and you want it to be of the greatest\npossible use to the public, the best way to achieve this is to make it\nfree software which everyone can redistribute and change under these terms.\n\n  To do so, attach the following notices to the program.  It is safest\nto attach them to the start of each source file to most effectively\nstate the exclusion of warranty; and each file should have at least\nthe \"copyright\" line and a pointer to where the full notice is found.\n\n    <one line to give the program's name and a brief idea of what it does.>\n    Copyright (C) <year>  <name of author>\n\n    This program is free software: you can redistribute it and/or modify\n    it under the terms of the GNU General Public License as published by\n    the Free Software Foundation, either version 3 of the License, or\n    (at your option) any later version.\n\n    This program is distributed in the hope that it will be useful,\n    but WITHOUT ANY WARRANTY; without even the implied warranty of\n    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\n    GNU General Public License for more details.\n\n    You should have received a copy of the GNU General Public License\n    along with this program.  If not, see <https://www.gnu.org/licenses/>.\n\nAlso add information on how to contact you by electronic and paper mail.\n\n  If the program does terminal interaction, make it output a short\nnotice like this when it starts in an interactive mode:\n\n    <program>  Copyright (C) <year>  <name of author>\n    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.\n    This is free software, and you are welcome to redistribute it\n    under certain conditions; type `show c' for details.\n\nThe hypothetical commands `show w' and `show c' should show the appropriate\nparts of the General Public License.  Of course, your program's commands\nmight be different; for a GUI interface, you would use an \"about box\".\n\n  You should also get your employer (if you work as a programmer) or school,\nif any, to sign a \"copyright disclaimer\" for the program, if necessary.\nFor more information on this, and how to apply and follow the GNU GPL, see\n<https://www.gnu.org/licenses/>.\n\n  The GNU General Public License does not permit incorporating your program\ninto proprietary programs.  If your program is a subroutine library, you\nmay consider it more useful to permit linking proprietary applications with\nthe library.  If this is what you want to do, use the GNU Lesser General\nPublic License instead of this License.  But first, please read\n<https://www.gnu.org/licenses/why-not-lgpl.html>.\n",
             "licenseId": "GPL-3.0",
             "name": "visual-programming-editor",
-            "versionInfo": "8.5.0"
+            "versionInfo": "8.5.1"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015 Jordan Harband\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n\n",
             "licenseId": "MIT",
             "name": "which-typed-array",
             "versionInfo": "1.1.11"
         }
```

### Comparing `vp4jl-0.1.2/vp4jl/nodeextension/imageio.json` & `vp4jl-0.1.3/vp4jl/nodeextension/imageio.json`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/vp4jl/vp_nodes/package1/__init__.json` & `vp4jl-0.1.3/vp4jl/vp_nodes/package1/__init__.json`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/.gitignore` & `vp4jl-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/LICENSE` & `vp4jl-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/README.md` & `vp4jl-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/pyproject.toml` & `vp4jl-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vp4jl-0.1.2/PKG-INFO` & `vp4jl-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vp4jl
-Version: 0.1.2
+Version: 0.1.3
 Summary: The JupyterLab extension providing node based visual programming environment
 Project-URL: Homepage, https://github.com/Max-ChenFei/VisualProgramming4JupyterLab
 Project-URL: Bug Tracker, https://github.com/Max-ChenFei/VisualProgramming4JupyterLab/issues
 Project-URL: Repository, https://github.com/Max-ChenFei/VisualProgramming4JupyterLab.git
 Author-email: Fei Chen <boxchenfei@gmail.com>
 License: BSD 3-Clause License
```

