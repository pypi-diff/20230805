# Comparing `tmp/mknodes-0.8.3.tar.gz` & `tmp/mknodes-0.9.0.tar.gz`

## Comparing `mknodes-0.8.3.tar` & `mknodes-0.9.0.tar`

### file list

```diff
@@ -1,92 +1,93 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.8.3/.editorconfig
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.8.3/Makefile
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mknodes-0.8.3/mkdocs.yml
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.8.3/.github/workflows/build.yml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.8.3/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 mknodes-0.8.3/docs/gen_pages.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 mknodes-0.8.3/docs/gen_qt.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkadmonition.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkannotations.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkbinaryimage.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkblock.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkcode.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkcontainer.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkcritic.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkdiagram.py
--rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkdoc.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkdocstrings.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkhtmlblock.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkimage.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkinstallguide.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mklink.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mklist.py
--rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mknav.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mknode.py
--rw-r--r--   0        0        0    13072 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkpage.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkpageinclude.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mkshields.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mksnippet.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mksourceandresult.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mktabcontainer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mktable.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mktabs.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/mktext.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/node.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/__linkreplacer/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/__linkreplacer/linkreplacer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/classnodes/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/classnodes/mkclassdiagram.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/classnodes/mkclasspage.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/classnodes/mkclasstable.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/manual/__init__.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/manual/introduce_nodes.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/manual/page_1.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/manual/page_2.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/manual/page_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/modulenodes/__init__.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/modulenodes/mkmodulepage.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/modulenodes/mkmoduletable.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/resources/codeofconduct.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/__init__.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/classhelpers.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/connectionbuilder.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/debugging.py
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/helpers.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/inventorymanager.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/linkprovider.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/mermaid.py
--rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/noderesolver.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 mknodes-0.8.3/mknodes/utils/packageinfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/conftest.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_admonition.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_annotations.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_block.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_classdiagram.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_docstrings.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_image.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_linkreplacer.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_list.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_manual.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_markdownnode.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_modulepage.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_nav.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_packageinfo.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_page.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_tabblock.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_tabcontainer.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/test_text.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/SUMMARY.md
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_file.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_folder/sub_1.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_folder/sub_2.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_subnav/SUMMARY.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_subnav/subnav_page_1.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.8.3/tests/data/nav_tree/test_subnav/subnav_page_2.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.8.3/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.8.3/LICENSE
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.8.3/README.md
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 mknodes-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 mknodes-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.9.0/.editorconfig
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.9.0/Makefile
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 mknodes-0.9.0/mkdocs.yml
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.9.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 mknodes-0.9.0/docs/gen_pages.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 mknodes-0.9.0/docs/gen_qt.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/__init__.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkadmonition.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkannotations.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkbinaryimage.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkblock.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkcode.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkcontainer.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkcritic.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkdiagram.py
+-rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkdoc.py
+-rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkdocstrings.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkhtmlblock.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkimage.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkinstallguide.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mklink.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mklist.py
+-rw-r--r--   0        0        0     9723 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mknav.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mknode.py
+-rw-r--r--   0        0        0    13075 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkpage.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkpageinclude.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mkshields.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mksnippet.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mktabcontainer.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mktable.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mktabs.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/mktext.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/node.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/__linkreplacer/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/__linkreplacer/linkreplacer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/classnodes/__init__.py
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/classnodes/mkclassdiagram.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/classnodes/mkclasspage.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/classnodes/mkclasstable.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/manual/__init__.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/manual/introduce_nodes.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/manual/page_1.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/manual/page_2.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/manual/page_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/modulenodes/__init__.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/modulenodes/mkmodulepage.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/modulenodes/mkmoduletable.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/resources/codeofconduct.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/utils/__init__.py
+-rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/utils/classhelpers.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/utils/connectionbuilder.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/utils/debugging.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/utils/helpers.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/utils/inventorymanager.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/utils/linkprovider.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/utils/mermaid.py
+-rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/utils/noderesolver.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 mknodes-0.9.0/mknodes/utils/packageinfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_admonition.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_annotations.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_block.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_classdiagram.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_docstrings.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_image.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_inventorymanager.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_linkreplacer.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_list.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_manual.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_markdownnode.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_modulepage.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_nav.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_packageinfo.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_page.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_tabblock.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_tabcontainer.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/test_text.py
+-rw-r--r--   0        0        0    18320 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/data/objects.inv
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/data/nav_tree/SUMMARY.md
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/data/nav_tree/test_file.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/data/nav_tree/test_folder/sub_1.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/data/nav_tree/test_folder/sub_2.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/data/nav_tree/test_subnav/SUMMARY.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/data/nav_tree/test_subnav/subnav_page_1.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.9.0/tests/data/nav_tree/test_subnav/subnav_page_2.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.9.0/README.md
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 mknodes-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 mknodes-0.9.0/PKG-INFO
```

### Comparing `mknodes-0.8.3/.pre-commit-config.yaml` & `mknodes-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/Makefile` & `mknodes-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mkdocs.yml` & `mknodes-0.9.0/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
           show_symbol_type_toc: true
           show_symbol_type_heading: true
           # merge_init_into_class: true
           # ignore_init_summary: true
           # show_if_no_docstring: true
           inherited_members: false
           signature_crossrefs: true
-          # separate_signature: true
+          separate_signature: true
           line_length: 90
 markdown_extensions:
 - codehilite
 - admonition
 - def_list
 - attr_list
 - abbr
```

### Comparing `mknodes-0.8.3/.github/workflows/build.yml` & `mknodes-0.9.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/.github/workflows/documentation.yml` & `mknodes-0.9.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/docs/gen_pages.py` & `mknodes-0.9.0/docs/gen_pages.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/docs/gen_qt.py` & `mknodes-0.9.0/docs/gen_qt.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/__init__.py` & `mknodes-0.9.0/mknodes/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 from .mkcode import MkCode
 from .mkdocstrings import MkDocStrings
 from .mkimage import MkImage
 from .mkbinaryimage import MkBinaryImage
 from .mklist import MkList
 from .mkdiagram import MkDiagram
 from .mktable import MkTable
-from .mktabcontainer import MkTabBlock, MkTabbed
+from .mktabcontainer import MkBlockTabbed, MkTabbed
 from .mksnippet import MkSnippet
 from .mkcritic import MkCritic
 from .mkannotations import MkAnnotations
-from .mksourceandresult import MkSourceAndResult
 from .mkshields import MkShields
 from .mkpage import MkPage
 from .mkpageinclude import MkPageInclude
 from .mkinstallguide import MkInstallGuide
 
 from .classnodes.mkclassdiagram import MkClassDiagram
 from .classnodes.mkclasstable import MkClassTable
@@ -55,18 +54,17 @@
     "MkClassTable",
     "MkList",
     "MkClassPage",
     "MkModulePage",
     "MkModuleTable",
     "MkAnnotations",
     "MkDoc",
-    "MkTabBlock",
+    "MkBlockTabbed",
     "MkTabbed",
-    "MkSourceAndResult",
     "MkSnippet",
     "MkShields",
     "MkPageInclude",
     "MkCritic",
     "MkInstallGuide",
 ]
 
-__version__ = "0.8.3"
+__version__ = "0.9.0"
```

### Comparing `mknodes-0.8.3/mknodes/mkannotations.py` & `mknodes-0.9.0/mknodes/mkannotations.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,36 +7,34 @@
 from mknodes.utils import helpers
 
 
 logger = logging.getLogger(__name__)
 
 
 class MkAnnotation(mkcontainer.MkContainer):
+    """Represents a single annotation. It gets managed by an MkAnnotations node."""
+
     def __init__(self, num: int, item: str | mknode.MkNode, **kwargs):
         super().__init__(items=[item], **kwargs)
         self.num = num
 
     def __repr__(self):
         return helpers.get_repr(self, num=self.num, item=self.items[0])
 
-    @staticmethod
-    def examples():
-        yield from ()
-
     def _to_markdown(self) -> str:
         item_str = "\n\n".join(i.to_markdown() for i in self.items)
         lines = item_str.split("\n")
         space = (3 - len(str(self.num))) * " "
         result = [f"{self.num}.{space}{lines[0]}"]
         result.extend(f"    {i}" for i in lines[1:])
         return "\n".join(result) + "\n"
 
 
 class MkAnnotations(mkcontainer.MkContainer):
-    """Node containing a list of annotations."""
+    """Node containing a list of MkAnnotations."""
 
     items: list[MkAnnotation]
 
     def __init__(
         self,
         annotations: Mapping[int, str | mknode.MkNode]
         | list[MkAnnotation]
@@ -103,19 +101,33 @@
         if index in self:
             pos = self._get_annotation_pos(index)
             self.items[pos] = annotation
         else:
             self.items.append(annotation)
 
     @staticmethod
-    def examples():  # (1)
-        yield dict(annotations=["Item 1"])
+    def create_example_page(page):
+        import mknodes
+
+        page += mknodes.MkCode.for_object(
+            MkAnnotations.create_example_page,
+            extract_body=True,
+        )
+        node = MkAnnotations()
+        page += "The MkAnnotations node aggregates annotations."
+        node[1] = r"Annotations are numbered and can be set via \__setitem__."  # (1)
+        node[2] = mknodes.MkAdmonition("They can also contain other Markdown.")  # (2)
+        page += node
+        page += mknodes.MkCode(str(node), language="markdown", header="Markdown")
 
     def _to_markdown(self) -> str:
         return "".join(str(i) for i in self.items) if self.items else ""
 
 
 if __name__ == "__main__":
+    import mknodes
+
     # ann = MkAnnotation(1, "test")
     # print(ann)
-    section = MkAnnotations(["abcde\nfghi"] * 10, header="Header")
-    print(section.to_markdown())
+    page = mknodes.MkPage()
+    MkAnnotations.create_example_page(page)
+    print(page)
```

### Comparing `mknodes-0.8.3/mknodes/mkblock.py` & `mknodes-0.9.0/mknodes/mkhtmlblock.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 from __future__ import annotations
 
 import logging
+import textwrap
 
-from mknodes import mknode
+from mknodes import mkblock, mknode
 
 
 logger = logging.getLogger(__name__)
 
 
-class MkBlock(mknode.MkNode):
+class MkHtmlBlock(mkblock.MkBlock):
     """pymdownx-based block."""
 
     def __init__(
         self,
-        typ: str,
         content: str | mknode.MkNode = "",
         *,
-        title: str = "",
         attributes: dict[str, str | bool] | None = None,
         **kwargs,
     ):
-        super().__init__(**kwargs)
-        self.typ = typ
-        self.attributes = attributes or {}
-        self.title = title
-        self.content = content
+        super().__init__(name="html", argument="div", content=content, **kwargs)
 
     def _to_markdown(self) -> str:
         block_limiter = "///"
-        lines = [f"{block_limiter} {self.typ} | {self.title}"]
+        lines = [f"{block_limiter} {self.name} | {self.argument}"]
         lines.extend(f"    {k}: {v}" for k, v in self.attributes.items())
-        lines.extend((str(self.content).rstrip("\n"), block_limiter))
+        lines.append("")
+        lines.extend(
+            (textwrap.indent(str(self.content), "    ").rstrip("\n"), block_limiter),
+        )
         return "\n".join(lines) + "\n"
 
 
 if __name__ == "__main__":
-    test = MkBlock("tab", title="abc", content="bcd", attributes=dict(new=True))
+    test = MkHtmlBlock("test")
     print(test)
```

### Comparing `mknodes-0.8.3/mknodes/mkcode.py` & `mknodes-0.9.0/mknodes/mkcode.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,20 +44,26 @@
         self.language = language
         self.title = title
         self.linenums = linenums
         self.highlight_lines = highlight_lines
 
     def _to_markdown(self) -> str:
         title = f" title={self.title!r}" if self.title else ""
+        if self.highlight_lines:
+            title += ' hl_lines="' + " ".join(str(i) for i in self.highlight_lines) + '"'
         return f"``` {self.language}{title}\n{self.text}\n```"
 
     @staticmethod
-    def examples():
-        yield dict(language="python", code="a = 1 + 2")
-        yield dict(language="js", code="var z = x + y;", title="JavaScript")
+    def create_example_page(page):
+        page += "A MkCode node can be used to display a code section"
+        page += MkCode(language="python", code="a = 1 + 2")
+        page += "You can also apply syntax highlighting for different languages"
+        page += MkCode(language="js", code="var z = x + y;", title="JavaScript")
+        page += "Highlighting lines is also possible"
+        page += MkCode(code="1\n2\n3\n4", highlight_lines=[1, 3])
 
     @classmethod
     def for_object(
         cls,
         obj: types.ModuleType
         | type
         | types.MethodType
@@ -65,23 +71,30 @@
         | types.TracebackType
         | types.FrameType
         | types.CodeType
         | Callable[..., Any],
         *,
         dedent: bool = True,
         extract_body: bool = False,
+        title: str | None = None,
         header: str = "",
     ) -> Self:
         if extract_body and isinstance(obj, type | types.FunctionType | types.MethodType):
             code = helpers.get_function_body(obj)
         elif extract_body:
             msg = "Can only extract body from Functions, Methods and classes"
             raise TypeError(msg)
         else:
             code = inspect.getsource(obj)
         code = textwrap.dedent(code) if dedent else code
-        return cls(code=code, header=header)
+        if title is not None:
+            code_title = title
+        elif isinstance(obj, types.TracebackType | types.FrameType | types.CodeType):
+            code_title = ""
+        else:
+            code_title = obj.__name__
+        return cls(code=code, header=header, title=code_title)
 
 
 if __name__ == "__main__":
     code = MkCode.for_object(MkCode, extract_body=True)
     print(code)
```

### Comparing `mknodes-0.8.3/mknodes/mkcontainer.py` & `mknodes-0.9.0/mknodes/mkcontainer.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,18 +26,24 @@
     def __iter__(self) -> Iterator[mknode.MkNode]:  # type: ignore
         return iter(self.items)
 
     def __repr__(self):
         return helpers.get_repr(self, items=self.items)
 
     @staticmethod
-    def examples():
-        from mknodes import mkcode
+    def create_example_page(page):
+        import mknodes
 
-        yield dict(items=[mkcode.MkCode(code="a = 1 + 2"), mktext.MkText("abc")])
+        page += "MkContainers are usually only used as a base class"
+        page += "It basically only carries other nodes and stringifies them sequentially."
+        item_1 = mknodes.MkCode(code="a = 1 + 2")
+        item_2 = mktext.MkText("abc")
+        node = MkContainer(items=[item_1, item_2])
+        node += mknodes.MkHtmlBlock(str(node), header="Markdown")
+        page += node
 
     def _to_markdown(self) -> str:
         return "\n\n".join(i.to_markdown() for i in self.items)
 
     def append(self, other: str | mknode.MkNode):
         match other:
             case str():
```

### Comparing `mknodes-0.8.3/mknodes/mkcritic.py` & `mknodes-0.9.0/mknodes/mkcritic.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,17 @@
             case "comment":
                 left, right = (">>", "<<")
             case _:
                 raise TypeError(self.mark)
         return f"{{{left}\n\n{self.text}\n\n{right}}}"
 
     @staticmethod
-    def examples():
+    def create_example_page(page):
+        page += "The MkCritic node can be used to display text diffs."
         for typ in ["addition", "deletion", "comment", "highlight"]:
-            yield dict(mark=typ, text=f"This is type {typ}")
+            node = MkCritic(mark=typ, text=f"This is type {typ}")
+            page += node
 
 
 if __name__ == "__main__":
     mkcritic = MkCritic("hello")
     print(mkcritic)
```

### Comparing `mknodes-0.8.3/mknodes/mkdiagram.py` & `mknodes-0.9.0/mknodes/mkdiagram.py`

 * *Files 20% similar despite different names*

```diff
@@ -59,18 +59,23 @@
     def _to_markdown(self) -> str:
         items = list(self.items) + [f"{a} --> {b}" for a, b in self.connections]
         item_str = textwrap.indent("\n".join(items), "  ")
         text = f"{self.graph_type} {self.orientation}\n{item_str}"
         return f"```mermaid\n{text}\n```"
 
     @staticmethod
-    def examples():
-        yield dict(
+    def create_example_page(page):
+        import mknodes
+
+        page += "MkDiagrams can be used to create Mermaid diagrams."
+        diagram = MkDiagram(
             graph_type="flow",
             items=["1", "2", "3"],
             connections=[("1", "2"), ("2", "3")],
         )
+        page += diagram
+        page += mknodes.MkHtmlBlock(str(diagram), header="Markdown")
 
 
 if __name__ == "__main__":
     diagram = MkDiagram(graph_type="flow")
     print(diagram)
```

### Comparing `mknodes-0.8.3/mknodes/mkdoc.py` & `mknodes-0.9.0/mknodes/mkdoc.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/mkdocstrings.py` & `mknodes-0.9.0/mknodes/mkdocstrings.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     REQUIRED_PLUGINS = "mkdocstrings"
     OPTIONS_DEFAULT: dict[str, Any] = {}
 
     def __init__(
         self,
         obj: types.ModuleType
         | str
+        | tuple[str, ...]
+        | list[str]
         | os.PathLike
         | type
         | types.FunctionType
         | types.MethodType,
         for_topmost: bool = False,
         allow_inspection: bool | None = None,
         show_bases: bool | None = None,
@@ -175,11 +177,25 @@
     def _to_markdown(self) -> str:
         md = f"::: {self.obj_path}\n"
         if self.options:
             options = "\n".join(f"      {k}: {v!r}" for k, v in self.options.items())
             md = f"{md}    options:\n{options}\n"
         return md
 
+    @staticmethod
+    def create_example_page(page):
+        import mknodes
+
+        page += "The MkDocStrings node shows DocStrings from mkdocstrings addon."
+        node = MkDocStrings(
+            "mknodes.MkDocStrings",
+            show_if_no_docstring=True,
+            header="DocStrings",
+            heading_level=3,
+        )
+        page += mknodes.MkCode(str(node), header="Markdown")
+        page += node
+
 
 if __name__ == "__main__":
     docstrings = MkDocStrings("a.b", show_submodules=True)
     print(docstrings)
```

### Comparing `mknodes-0.8.3/mknodes/mkhtmlblock.py` & `mknodes-0.9.0/mknodes/mkblock.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 from __future__ import annotations
 
 import logging
-import textwrap
 
-from mknodes import mkblock, mknode
+from mknodes import mknode
 
 
 logger = logging.getLogger(__name__)
 
 
-class MkHtmlBlock(mkblock.MkBlock):
+class MkBlock(mknode.MkNode):
     """pymdownx-based block."""
 
     def __init__(
         self,
+        name: str,
         content: str | mknode.MkNode = "",
         *,
+        argument: str = "",
         attributes: dict[str, str | bool] | None = None,
         **kwargs,
     ):
-        super().__init__(typ="html", title="div", content=content)
+        super().__init__(**kwargs)
+        self.name = name
+        self.attributes = attributes or {}
+        self.argument = argument
+        self.content = content
 
     def _to_markdown(self) -> str:
         block_limiter = "///"
-        lines = [f"{block_limiter} {self.typ} | {self.title}"]
+        base = f"{block_limiter} {self.name}"
+        if self.argument:
+            base += f" | {self.argument}"
+        lines = [base]
         lines.extend(f"    {k}: {v}" for k, v in self.attributes.items())
-        lines.append("")
-        lines.extend(
-            (textwrap.indent(str(self.content), "    ").rstrip("\n"), block_limiter),
-        )
+        lines.extend((str(self.content).rstrip("\n"), block_limiter))
         return "\n".join(lines) + "\n"
 
+    @staticmethod
+    def create_example_page(page):
+        import mknodes
+
+        page += "An MkBlock is a base class for pymdownx-style blocks."
+        block = MkBlock("html", content="Some text", argument="div")
+        page += mknodes.MkCode(str(block), header="Markdown")
+
 
 if __name__ == "__main__":
-    test = MkHtmlBlock("test")
+    test = MkBlock("tab", argument="abc", content="bcd", attributes=dict(new=True))
     print(test)
```

### Comparing `mknodes-0.8.3/mknodes/mkimage.py` & `mknodes-0.9.0/mknodes/mkimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/mkinstallguide.py` & `mknodes-0.9.0/mknodes/mkinstallguide.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,14 +27,21 @@
         super().__init__(**kwargs)
         self.project = project
 
     def _to_markdown(self) -> str:
         return TEXT.format(project=self.project)
 
     @staticmethod
-    def examples():
-        yield dict(project="mknodes")
+    def create_example_page(page):
+        import mknodes
+
+        # MkInstallGuide is just a text snippet for a short Install guide
+        # Currently it is only tailored towards PyPi.
+
+        node = MkInstallGuide(project="mknodes")
+        page += node
+        page += mknodes.MkHtmlBlock(str(node), header="Markdown")
 
 
 if __name__ == "__main__":
     installguide = MkInstallGuide(project="mknodes")
     print(installguide)
```

### Comparing `mknodes-0.8.3/mknodes/mklink.py` & `mknodes-0.9.0/mknodes/mklink.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/mklist.py` & `mknodes-0.9.0/mknodes/mklist.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,17 +39,31 @@
             self,
             items=self.items,
             shorten_after=self.shorten_after,
             as_links=self.as_links,
         )
 
     @staticmethod
-    def examples():
-        yield dict(items=["Item 1", "Item 2", "Item 2"])
-        yield dict(items=["Item"] * 6, shorten_after=3)
+    def create_example_page(page):
+        import mknodes
+
+        list_1 = MkList(items=["Item 1", "Item 2", "Item 3"], header="Regular")
+        # list can also have a max length. they will get shortened with a "..." entry.
+        list_2 = MkList(items=["Item"] * 6, shorten_after=3, header="Shortened")
+        # They can also be ordered.
+        list_3 = MkList(
+            items=["Item 1", "Item 2", "Item 3"],
+            ordered=True,
+            header="Ordered",
+        )
+        page += list_1
+        page += list_2
+        page += list_3
+        code = "\n".join(str(i) for i in [list_1, list_2, list_3])
+        page += mknodes.MkCode(code, language="markdown", header="Markdown")
 
     def _prep(self, item) -> str:
         return helpers.linked(item) if self.as_links else str(item)
 
     def _to_markdown(self) -> str:
         if not self.items:
             return ""
```

### Comparing `mknodes-0.8.3/mknodes/mknav.py` & `mknodes-0.9.0/mknodes/mknav.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/mknode.py` & `mknodes-0.9.0/mknodes/mknode.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,14 @@
         super().__init__(parent=parent)
         self.header = header
         self.indent = indent
 
     def __str__(self):
         return self.to_markdown()
 
-    # @staticmethod
-    # def examples():
-    #     yield from ()
-
     def _to_markdown(self) -> str:
         return NotImplemented
 
     def to_markdown(self) -> str:
         """Outputs markdown for self and all children."""
         text = self._to_markdown()
         if self.indent:
```

### Comparing `mknodes-0.8.3/mknodes/mkpage.py` & `mknodes-0.9.0/mknodes/mkpage.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
             data: tab data
             style: Whether to use new-style (tabblock) or old-style (tabbed) tabs.
             kwargs: Keyword arguments passed to Tabs
         """
         if style == "tabbed":
             tabblock = mktabcontainer.MkTabbed(data, parent=self, **kwargs)
         else:
-            tabblock = mktabcontainer.MkTabBlock(data, parent=self, **kwargs)
+            tabblock = mktabcontainer.MkBlockTabbed(data, parent=self, **kwargs)
         self.append(tabblock)
         return tabblock
 
 
 if __name__ == "__main__":
     doc = MkPage(hide_toc=True, search_boost=2)
     doc.add_link("test")
```

### Comparing `mknodes-0.8.3/mknodes/mkpageinclude.py` & `mknodes-0.9.0/mknodes/mkpageinclude.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,16 +34,12 @@
             case os.PathLike() | str():
                 return pathlib.Path(self.page).read_text()
             case mkpage.MkPage():
                 return str(self.page)
             case _:
                 raise TypeError(self.page)
 
-    @staticmethod
-    def examples():
-        yield dict(page=mkpage.MkPage(items=["test"]))
-
 
 if __name__ == "__main__":
     page = mkpage.MkPage(items=["test"])
     include = MkPageInclude(page=__file__)
     print(include)
```

### Comparing `mknodes-0.8.3/mknodes/mkshields.py` & `mknodes-0.9.0/mknodes/mkshields.py`

 * *Files 10% similar despite different names*

```diff
@@ -125,20 +125,24 @@
             s.to_url(user=self.user, project=self.project, branch=self.branch)
             for s in SHIELDS
             if s.identifier in self.shields
         ]
         return "".join(shield_strs)
 
     @staticmethod
-    def examples():
-        yield dict(
+    def create_example_page(page):
+        import mknodes
+
+        node = MkShields(
             shields=["version", "status", "codecov"],
             user="phil65",
             project="mknodes",
         )
+        page += node
+        page += mknodes.MkCode(str(node), language="markdown", header="Markdown")
 
 
 if __name__ == "__main__":
     shields = MkShields(
         shields=["version", "status", "codecov"],
         user="phil65",
         project="prettyqt",
```

### Comparing `mknodes-0.8.3/mknodes/mksnippet.py` & `mknodes-0.9.0/mknodes/mksnippet.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/mktabcontainer.py` & `mknodes-0.9.0/mknodes/mktabcontainer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,140 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
 import logging
-import textwrap
 
 from mknodes import mkcontainer, mknode, mktabs, mktext
 from mknodes.utils import helpers
 
 
 logger = logging.getLogger(__name__)
 
 
 class MkTabContainer(mkcontainer.MkContainer):
-    items: list[mktabs.MkTab]
+    items: list[mktabs.MkTab | mktabs.MkBlockTab]
+    Tab: type[mktabs.MkTab] | type[mktabs.MkBlockTab]
 
     def __init__(
         self,
         tabs: Mapping[str, str | mknode.MkNode] | list[mktabs.MkTab],
         *,
         header: str = "",
         select_tab: int | str | None = None,
         **kwargs,
     ):
         if isinstance(tabs, list):
             items = tabs
         else:
             items = [
-                mktabs.MkTab(
-                    k,
-                    items=[mktext.MkText(v) if isinstance(v, str) else v],
+                self.Tab(
+                    title=k,
+                    content=mktext.MkText(v) if isinstance(v, str) else v,
                 )
                 for k, v in tabs.items()
             ]
         for tab in items:
             tab.parent_item = self
         match select_tab:
             case int():
                 items[select_tab].select = True
             case str():
                 pos = self._get_tab_pos(select_tab)
                 items[pos].select = True
         super().__init__(items=items, header=header, **kwargs)
 
-    def __getitem__(self, item: int | str):
+    def __getitem__(self, item: int | str) -> mktabs.MkTab | mktabs.MkBlockTab:
         match item:
             case int():
                 return self.items[item]
             case str():
                 for tab in self.items:
                     if tab.title == item:
                         return tab
                 raise IndexError(item)
             case _:
                 raise TypeError(item)
 
-    def __contains__(self, tab: str | mktabs.MkTab) -> bool:
+    def __contains__(self, tab: str | mktabs.MkTab | mktabs.MkBlockTab) -> bool:
         match tab:
-            case mktabs.MkTab():
+            case mktabs.MkTab() | mktabs.MkBlockTab():
                 return tab in self.items
             case str():
                 return any(i.title == tab for i in self.items)
             case _:
                 raise TypeError(tab)
 
     def _get_tab_pos(self, tab_title: str) -> int:
         item = next(i for i in self.items if i.title == tab_title)
         return self.items.index(item)
 
-    def __setitem__(self, index: str, value: mktabs.MkTab | str):
+    def __setitem__(self, index: str, value: mktabs.MkTab | mktabs.MkBlockTab | str):
         match value:
             case str():
                 item = mktext.MkText(value)
-                tab = mktabs.MkTab(index, items=[item])
-            case mktabs.MkTab():
+                tab = self.Tab(index, content=item)
+            case mktabs.MkTab() | mktabs.MkBlockTab():
                 tab = value
             case mknode.MkNode():
-                tab = mktabs.MkTab(index, items=[value])
+                tab = self.Tab(index, content=value)
         if index in self:
             pos = self._get_tab_pos(index)
             self.items[pos] = tab
         else:
             self.items.append(tab)
 
     def __repr__(self):
-        return helpers.get_repr(self, items=self.items)
+        return helpers.get_repr(self, tabs=self.items)
 
     def to_dict(self):
         return {tab.title: str(tab) for tab in self.items}
 
-    @staticmethod
-    def examples():
-        yield dict(tabs={"Tab 1": "Some markdown", "Tab 2": "Other Markdown"})
+    def _to_markdown(self) -> str:
+        return "\n".join(str(i) for i in self.items)
 
 
 class MkTabbed(MkTabContainer):
     """pymdownx-based Tab block."""
 
+    items: list[mktabs.MkTab]
     REQUIRED_EXTENSIONS = "pymdownx.tabbed"
+    Tab = mktabs.MkTab
 
-    def _to_markdown(self) -> str:
-        lines: list[str] = []
-        for tab in self.items:
-            indented_text = textwrap.indent(str(tab).rstrip("\n"), prefix="    ")
-            selected = "+" if tab.select else ""
-            lines.extend((f'==={selected} "{tab.title}"', indented_text))
-        return "\n".join(lines) + "\n"
+    @staticmethod
+    def create_example_page(page):
+        import mknodes
+
+        # this node is basically a container and manager for MkTabs nodes.
+        node = MkTabbed(tabs={"Tab 1": "Some markdown", "Tab 2": "Other Markdown"})
+        page += node
+        page += mknodes.MkCode(str(node), language="markdown", header="Markdown")
 
 
-class MkTabBlock(MkTabContainer):
+class MkBlockTabbed(MkTabContainer):
     """New blocks-based Tab block."""
 
+    items: list[mktabs.MkBlockTab]
     REQUIRED_EXTENSIONS = "pymdownx.blocks.tab"
+    Tab = mktabs.MkBlockTab
+
+    @staticmethod
+    def create_example_page(page):
+        import mknodes
+
+        # this one is basically the same as MkTabbed,
+        # but based on new pymdownx block syntax.
+        # i think it is not supported by Material for MkDocs yet.
+        node = MkBlockTabbed(tabs={"Tab 1": "Some markdown", "Tab 2": "Other Markdown"})
+        page += node
+        page += mknodes.MkCode(str(node), language="markdown", header="Markdown")
 
     def _to_markdown(self) -> str:
-        lines: list[str] = []
-        for i, tab in enumerate(self.items):
-            begin = f"/// tab | {tab.title}"
-            if i == 0:
-                begin += "\n    new: True"
-            if tab.select:
-                begin += "\n    select: True"
-            content = str(tab).rstrip("\n")
-            end = "///\n"
-            lines.extend((begin, content, end))
-        return "\n".join(lines) + "\n"
+        if not self.items:
+            return ""
+        self.items[0].new = True
+        return "\n".join(str(i) for i in self.items)
 
 
 if __name__ == "__main__":
     tabs = dict(Tab1="Some text", Tab2="Another text")
-    tabblock = MkTabbed(tabs)
+    tabblock = MkBlockTabbed(tabs)
     print(tabblock)
```

### Comparing `mknodes-0.8.3/mknodes/mktable.py` & `mknodes-0.9.0/mknodes/mktable.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,21 +53,28 @@
         data = [
             [formatters[i].format(k) for i, k in enumerate(row)]
             for row in self._iter_rows()
         ]
         header_txt = "| " + " | ".join(headers) + " |"
         divider_text = "| " + " | ".join(divider) + " |"
         data_txt = ["| " + " | ".join(line) + " |" for line in data]
-        return "\n".join([header_txt, divider_text, *data_txt])
+        return "\n".join([header_txt, divider_text, *data_txt]) + "\n"
 
     @staticmethod
-    def examples():
-        yield dict(data={"Column A": ["A", "B", "C"], "Column B": ["C", "D", "E"]})
+    def create_example_page(page):
+        import mknodes
+
+        node_1 = MkTable(data={"Column A": ["A", "B", "C"], "Column B": ["C", "D", "E"]})
+        # data can be given in different shapes.
         dicts = [{"col 1": "abc", "col 2": "cde"}, {"col 1": "fgh", "col 2": "ijk"}]
-        yield dict(data=dicts)
+        node_2 = MkTable(data=dicts)
+
+        page += node_1
+        page += node_2
+        page += mknodes.MkCode(str(node_1) + "\n" + str(node_2))
 
     def _iter_rows(self):
         length = min(len(i) for i in self.data.values())
         for j, _ in enumerate(range(length)):
             yield [self.data[k][j] or "" for k in self.data]
 
     def width_for_column(self, column: str | int):
```

### Comparing `mknodes-0.8.3/mknodes/mktext.py` & `mknodes-0.9.0/mknodes/mktext.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/node.py` & `mknodes-0.9.0/mknodes/node.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/__linkreplacer/linkreplacer.py` & `mknodes-0.9.0/mknodes/__linkreplacer/linkreplacer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/classnodes/mkclassdiagram.py` & `mknodes-0.9.0/mknodes/classnodes/mkclassdiagram.py`

 * *Files 19% similar despite different names*

```diff
@@ -86,16 +86,39 @@
             self,
             klass=self.klass,
             mode=self.mode,
             orientation=self.orientation,
         )
 
     @staticmethod
-    def examples():
-        yield dict(klass=MkClassDiagram)
+    def create_example_page(page):
+        import mknodes
+
+        parent_diagram = MkClassDiagram(
+            klass=MkClassDiagram,
+            mode="parent_tree",
+            header="Parent class hiearchy for MkClassDiagram",
+        )
+        sub_diagram = MkClassDiagram(
+            klass=mknodes.MkContainer,
+            mode="subclass_tree",
+            header="Subclass hiearchy for MkContainer",
+            orientation="LR",
+        )
+        mro_diagram = MkClassDiagram(
+            klass=mknodes.MkTable,
+            mode="mro",
+            header="Mro for MkTable",
+        )
+        page += parent_diagram
+        page += sub_diagram
+        page += mro_diagram
+        page += mknodes.MkHtmlBlock(parent_diagram, header="Markdown")
+        page += mknodes.MkHtmlBlock(sub_diagram)
+        page += mknodes.MkHtmlBlock(mro_diagram)
 
     def _to_markdown(self) -> str:
         match self.mode:
             case "subclass_tree":
                 builder = SubclassConnectionBuilder(self.klass)
                 item_str = builder.get_graph_connection_text()
             case "parent_tree":
```

### Comparing `mknodes-0.8.3/mknodes/classnodes/mkclasspage.py` & `mknodes-0.9.0/mknodes/classnodes/mkclasspage.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,16 +45,22 @@
                 self.parts = classhelpers.to_module_parts(module_path)
         self._build()
 
     def __repr__(self):
         return helpers.get_repr(self, klass=self.klass, path=str(self.path))
 
     @staticmethod
-    def examples():
-        yield dict(klass=MkClassPage)
+    def create_example_page(page):
+        import mknodes
+
+        # MkClassPages are page templates to display
+        # documentation about a class.
+        node = MkClassPage(klass=MkClassPage)
+        page += str(node)
+        page += mknodes.MkHtmlBlock(str(node), header="Markdown")
 
     def add_class_diagram(
         self,
         mode: mkclassdiagram.DiagramModeStr = "parent_tree",
         *,
         header: str = "",
     ):
```

### Comparing `mknodes-0.8.3/mknodes/classnodes/mkclasstable.py` & `mknodes-0.9.0/mknodes/classnodes/mkclasstable.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,22 +44,31 @@
 
         super().__init__(data=data, **kwargs)
 
     def __repr__(self):
         return helpers.get_repr(self, klasses=self.klasses)
 
     @staticmethod
-    def examples():
-        from mknodes import mknav
+    def create_example_page(page):
+        import mknodes
 
-        yield dict(klasses=[mktable.MkTable, MkClassTable, mknav.MkNav])
-        yield dict(
-            klasses=[mktable.MkTable, MkClassTable, mknav.MkNav],
+        node_1 = MkClassTable(
+            klasses=[mknodes.MkTable, MkClassTable, mknodes.MkNav],
+            layout="compact",
+            header="Compact layout",
+        )
+        node_2 = MkClassTable(
+            klasses=[mknodes.MkTable, MkClassTable, mknodes.MkNav],
             layout="extended",
+            header="Extended layout",
         )
+        page += node_1
+        page += node_2
+        page += mknodes.MkCode(str(node_1), language="markdown", header="Markdown")
+        page += mknodes.MkCode(str(node_2), language="markdown")
 
     def default_row_for_klass(self, kls: type) -> dict[str, str]:
         return dict(
             Class=helpers.link_for_class(kls),
             Module=kls.__module__,
             Description=helpers.get_first_doc_line(kls),
         )
```

### Comparing `mknodes-0.8.3/mknodes/manual/introduce_nodes.py` & `mknodes-0.9.0/mknodes/manual/introduce_nodes.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/manual/page_1.py` & `mknodes-0.9.0/mknodes/manual/page_1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import mknodes
 
-from mknodes.utils import classhelpers, helpers
+from mknodes.utils import classhelpers
 
 
 INTRO_TEXT = """
 Basically everything interesting in this library inherits from MkNode.
 It`s the base class for all tree nodes we are building. The tree goes from the root nav
 down to single markup elements. We can show the subclass tree by using
 the MkClassDiagram Node.
@@ -30,41 +30,25 @@
     # they will get converted to a mknodes.Text node.
     overview += INTRO_TEXT
     create_subclass_page(home_nav)
 
     # let`s take a look at some of the mentioned Markup nodes.
     # Some of them have a `examples` classmethod which yields some example signatures
     #  to show the functionality.
-    for kls in classhelpers.get_subclasses(mknodes.MkNode):
-        # get_subclasses just calls __subclasses__ recursively.
-        create_page_for_class(nodes_nav, kls)
-
-
-def create_page_for_class(nav: mknodes.MkNav, kls: type):
-    subpage = nav.add_page(kls.__name__)
-    subpage += mknodes.MkCode.for_object(create_page_for_class)
-    if hasattr(kls, "examples"):
-        subpage += mknodes.MkCode.for_object(
-            kls.examples,
-            header="Example signatures",
-        )
-        for i, sig in enumerate(kls.examples(), start=1):
-            subpage.add_header(f"Example {i}", level=2)
-            sig_txt = helpers.format_kwargs(sig)
-            text = f"node = mknodes.{kls.__name__}({sig_txt})\nstr(node)"
-            subpage.add_code(code=text, title=f"example_{i}.py")
-            node = kls(**sig)
-            subpage += mknodes.MkText(str(node), header="Preview")
-            subpage += mknodes.MkCode(
-                language="md",
-                code=node,
-                title="Resulting markdown",
+    for kls in classhelpers.iter_subclasses(mknodes.MkNode):
+        # iter_subclasses just calls __subclasses__ recursively.
+        if "create_example_page" in kls.__dict__:
+            subpage = nodes_nav.add_page(kls.__name__)
+            subpage += "## Code for this page"
+            subpage += mknodes.MkCode.for_object(
+                kls.create_example_page,
+                extract_body=True,
             )
-            subpage.add_newlines(3)
-    subpage.add_mkdocstrings(kls)
+            subpage += "## Output"
+            kls.create_example_page(subpage)
 
 
 def create_subclass_page(nav: mknodes.MkNav):
     # Lets take a look at the relations of the included nodes.
     # It`s easy to show different diagrams for classes.
     subcls_page = nav.add_page("Subclass tree", hide_toc=True)
     subcls_page += mknodes.MkCode.for_object(create_subclass_page)
```

### Comparing `mknodes-0.8.3/mknodes/manual/page_2.py` & `mknodes-0.9.0/mknodes/manual/page_2.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/manual/page_3.py` & `mknodes-0.9.0/mknodes/manual/page_3.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/modulenodes/mkmodulepage.py` & `mknodes-0.9.0/mknodes/modulenodes/mkmodulepage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import inspect
 import logging
 import os
 import pathlib
 import types
 
 from mknodes import mkdocstrings, mkpage
 from mknodes.classnodes import mkclasstable
@@ -44,24 +45,28 @@
         self.show_class_table = show_class_table
         self._build()
 
     def __repr__(self):
         return helpers.get_repr(self, module=self.module, path=str(self.path))
 
     @staticmethod
-    def examples():
+    def create_example_page(page):
         import mknodes
 
-        yield dict(module=mknodes)
+        # MkModulePages are page templates to display
+        # documentation about a module.
+        node = MkModulePage(module=mknodes)
+        page += node
+        page += mknodes.MkCode(str(node), language="markdown", header="Markdown")
 
     def _build(self):
-        if doc := self.module.__doc__:
+        if doc := inspect.getdoc(self.module):
             self.append(doc)
         if self.docstrings:
-            item = mkdocstrings.MkDocStrings(f'{".".join(self.parts)}')
+            item = mkdocstrings.MkDocStrings(self.module)
             self.append(item)
         if self.show_class_table:
             table = mkclasstable.MkClassTable(self.klasses)
             self.append(table)
 
 
 if __name__ == "__main__":
```

### Comparing `mknodes-0.8.3/mknodes/modulenodes/mkmoduletable.py` & `mknodes-0.9.0/mknodes/modulenodes/mkmoduletable.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,16 +45,20 @@
             ),
         )
 
     # def __repr__(self):
     #     return helpers.get_repr(self, module=self.module)
 
     @staticmethod
-    def examples():
+    def create_example_page(page):
+        import mkdocstrings
+
         import mknodes
 
-        yield dict(module=mknodes)
+        node = MkModuleTable(module=mkdocstrings)
+        page += node
+        page += mknodes.MkCode(str(node), language="markdown", header="Markdown")
 
 
 if __name__ == "__main__":
     table = MkModuleTable(module=helpers)
     print(table)
```

### Comparing `mknodes-0.8.3/mknodes/resources/codeofconduct.md` & `mknodes-0.9.0/mknodes/resources/codeofconduct.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/utils/classhelpers.py` & `mknodes-0.9.0/mknodes/utils/classhelpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,31 @@
 
 T = typing.TypeVar("T", bound=type)
 
 
 logger = logging.getLogger(__name__)
 
 
-def get_subclasses(klass: type, include_abstract: bool = False) -> typing.Iterator[type]:
+def iter_subclasses(
+    klass: type,
+    include_abstract: bool = False,
+    recursive: bool = True,
+) -> typing.Iterator[type]:
     """Recursively iter all subclasses of given klass.
 
     Arguments:
         klass: class to get subclasses from
         include_abstract: whether abstract base classes should be included.
+        recursive: whether to also get subclasses of subclasses.
     """
     if getattr(klass.__subclasses__, "__self__", None) is None:
         return
     for i in klass.__subclasses__():
-        yield from get_subclasses(i)
+        if recursive:
+            yield from iter_subclasses(i)
         if include_abstract or not inspect.isabstract(i):
             yield i
 
 
 @typing.overload
 def to_module(module, return_none: typing.Literal[False] = ...) -> types.ModuleType:
     ...
@@ -102,14 +108,28 @@
             return tuple(module.__name__.split("."))
         case pathlib.Path() if not module.is_absolute():
             return module.parts
         case _:
             raise TypeError(module)
 
 
+def to_dotted_path(obj: Sequence[str] | str | types.ModuleType | type) -> str:
+    match obj:
+        case (str(), *_):
+            return ".".join(obj)
+        case str():
+            return obj
+        case types.ModuleType():
+            return obj.__name__
+        case type():
+            return f"{obj.__module__}.{obj.__qualname__}"
+        case _:
+            raise TypeError(obj)
+
+
 def iter_classes(
     module: types.ModuleType | str | tuple[str, ...],
     *,
     type_filter: type | None | types.UnionType = None,
     module_filter: str | None = None,
     filter_by___all__: bool = False,
     recursive: bool = False,
```

### Comparing `mknodes-0.8.3/mknodes/utils/connectionbuilder.py` & `mknodes-0.9.0/mknodes/utils/connectionbuilder.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/utils/debugging.py` & `mknodes-0.9.0/mknodes/utils/debugging.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/utils/helpers.py` & `mknodes-0.9.0/mknodes/utils/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -194,16 +194,16 @@
             name = repr(v)
         kw_parts.append(f"{k}={name}")
     return ", ".join(kw_parts)
 
 
 def get_function_body(func: types.MethodType | types.FunctionType | type) -> str:
     # see https://stackoverflow.com/questions/38050649
-    source_lines = inspect.getsourcelines(func)[0]
-    source_lines = itertools.dropwhile(lambda x: x.startswith("@"), source_lines)
+    source_lines, _ = inspect.getsourcelines(func)
+    source_lines = itertools.dropwhile(lambda x: x.strip().startswith("@"), source_lines)
     line = next(source_lines).strip()  # type: ignore
     if not line.startswith(("def ", "class ")):
         return line.rsplit(":")[-1].strip()
     if not line.endswith(":"):
         for line in source_lines:
             line = line.strip()
             if line.endswith(":"):
@@ -212,15 +212,16 @@
 
 
 def get_deprecated_message(obj) -> str | None:
     return obj.__deprecated__ if hasattr(obj, "__deprecated__") else None
 
 
 def get_first_doc_line(obj, escape: bool = False, fallback: str = "") -> str:
-    doc = obj.__doc__.split("\n")[0] if isinstance(obj.__doc__, str) else fallback
+    docstrings = inspect.getdoc(obj)
+    doc = docstrings.split("\n")[0] if isinstance(docstrings, str) else fallback
     if escape:
         doc = escaped(doc)
     return doc
 
 
 if __name__ == "__main__":
     strings = groupby_first_letter([str(i) for i in range(1000)])
```

### Comparing `mknodes-0.8.3/mknodes/utils/linkprovider.py` & `mknodes-0.9.0/mknodes/utils/linkprovider.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/utils/mermaid.py` & `mknodes-0.9.0/mknodes/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/utils/noderesolver.py` & `mknodes-0.9.0/mknodes/utils/noderesolver.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/mknodes/utils/packageinfo.py` & `mknodes-0.9.0/mknodes/utils/packageinfo.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/tests/test_annotations.py` & `mknodes-0.9.0/tests/test_annotations.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/tests/test_nav.py` & `mknodes-0.9.0/tests/test_nav.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/tests/test_page.py` & `mknodes-0.9.0/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/tests/data/nav_tree/test_file.md` & `mknodes-0.9.0/tests/data/nav_tree/test_file.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/.gitignore` & `mknodes-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/LICENSE` & `mknodes-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/README.md` & `mknodes-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/pyproject.toml` & `mknodes-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mknodes-0.8.3/PKG-INFO` & `mknodes-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknodes
-Version: 0.8.3
+Version: 0.9.0
 Summary: Generate docs with ease.
 Project-URL: Documentation, https://phil65.github.io/mknodes/
 Project-URL: Source, https://github.com/phil65/mknodes
 Author-email: mknodes <philipptemminghoff@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: docs,docstrings,documentation,framework,internet,markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mknodes Version: 0.8.3 Summary: Generate docs with
+Metadata-Version: 2.1 Name: mknodes Version: 0.9.0 Summary: Generate docs with
 ease. Project-URL: Documentation, https://phil65.github.io/mknodes/ Project-
 URL: Source, https://github.com/phil65/mknodes Author-email: mknodes
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 docs,docstrings,documentation,framework,internet,markdown Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

