# Comparing `tmp/rdpy3-1.3.6.tar.gz` & `tmp/rdpy3-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdpy3-1.3.6.tar", last modified: Sat Aug  5 14:07:09 2023, max compression
+gzip compressed data, was "rdpy3-1.3.7.tar", last modified: Sat Aug  5 14:16:58 2023, max compression
```

## Comparing `rdpy3-1.3.6.tar` & `rdpy3-1.3.7.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.850000 rdpy3-1.3.6/
--rwxr-xr-x   0 root         (0) root         (0)    35121 2023-08-05 10:09:26.000000 rdpy3-1.3.6/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)     9577 2023-08-05 14:07:09.840000 rdpy3-1.3.6/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     9290 2023-08-05 13:16:36.000000 rdpy3-1.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.760000 rdpy3-1.3.6/bin/
--rwxr-xr-x   0 root         (0) root         (0)    10243 2023-08-05 14:06:11.000000 rdpy3-1.3.6/bin/rdpy3-rdpclient.py
--rwxr-xr-x   0 root         (0) root         (0)     7339 2023-08-05 14:06:11.000000 rdpy3-1.3.6/bin/rdpy3-rdphoneypot.py
--rwxr-xr-x   0 root         (0) root         (0)    11902 2023-08-05 14:06:11.000000 rdpy3-1.3.6/bin/rdpy3-rdpmitm.py
--rwxr-xr-x   0 root         (0) root         (0)     8077 2023-08-05 14:06:11.000000 rdpy3-1.3.6/bin/rdpy3-rdpscreenshot.py
--rwxr-xr-x   0 root         (0) root         (0)     4405 2023-08-05 14:06:11.000000 rdpy3-1.3.6/bin/rdpy3-rssplayer.py
--rwxr-xr-x   0 root         (0) root         (0)     3344 2023-08-05 14:06:11.000000 rdpy3-1.3.6/bin/rdpy3-vncclient.py
--rwxr-xr-x   0 root         (0) root         (0)     6164 2023-08-05 14:06:11.000000 rdpy3-1.3.6/bin/rdpy3-vncscreenshot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.760000 rdpy3-1.3.6/ext/
--rwxr-xr-x   0 root         (0) root         (0)    19035 2023-08-05 13:03:01.000000 rdpy3-1.3.6/ext/rle.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.760000 rdpy3-1.3.6/rdpy3/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.770000 rdpy3-1.3.6/rdpy3/core/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/core/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2505 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/core/const.py
--rwxr-xr-x   0 root         (0) root         (0)     3014 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/core/error.py
--rwxr-xr-x   0 root         (0) root         (0)     3507 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/core/filetimes.py
--rwxr-xr-x   0 root         (0) root         (0)     8950 2023-08-05 12:56:32.000000 rdpy3-1.3.6/rdpy3/core/layer.py
--rwxr-xr-x   0 root         (0) root         (0)     1976 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/core/log.py
--rwxr-xr-x   0 root         (0) root         (0)     9547 2023-08-05 12:56:32.000000 rdpy3-1.3.6/rdpy3/core/rss.py
--rwxr-xr-x   0 root         (0) root         (0)     1443 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/core/scancode.py
--rwxr-xr-x   0 root         (0) root         (0)    40003 2023-08-05 12:56:52.000000 rdpy3-1.3.6/rdpy3/core/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.780000 rdpy3-1.3.6/rdpy3/protocol/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.780000 rdpy3-1.3.6/rdpy3/protocol/rdp/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14313 2023-08-05 12:56:52.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/lic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.790000 rdpy3-1.3.6/rdpy3/protocol/rdp/nla/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/nla/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    13391 2023-08-05 12:56:32.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/nla/cssp.py
--rwxr-xr-x   0 root         (0) root         (0)    24730 2023-08-05 12:56:52.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/nla/ntlm.py
--rwxr-xr-x   0 root         (0) root         (0)     2808 2023-08-05 12:56:32.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/nla/sspi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.800000 rdpy3-1.3.6/rdpy3/protocol/rdp/pdu/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/pdu/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    19191 2023-08-05 12:56:52.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/pdu/caps.py
--rwxr-xr-x   0 root         (0) root         (0)    51908 2023-08-05 12:58:17.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/pdu/data.py
--rwxr-xr-x   0 root         (0) root         (0)    27792 2023-08-05 12:58:17.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/pdu/layer.py
--rwxr-xr-x   0 root         (0) root         (0)     4840 2023-08-05 12:56:32.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/pdu/order.py
--rwxr-xr-x   0 root         (0) root         (0)    28629 2023-08-05 12:58:17.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/rdp.py
--rwxr-xr-x   0 root         (0) root         (0)    27591 2023-08-05 12:58:17.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/sec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.800000 rdpy3-1.3.6/rdpy3/protocol/rdp/t125/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/t125/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7574 2023-08-05 12:56:32.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/t125/ber.py
--rwxr-xr-x   0 root         (0) root         (0)    23674 2023-08-05 12:58:17.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/t125/gcc.py
--rwxr-xr-x   0 root         (0) root         (0)    24771 2023-08-05 12:58:17.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/t125/mcs.py
--rwxr-xr-x   0 root         (0) root         (0)     7966 2023-08-05 12:56:32.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/t125/per.py
--rwxr-xr-x   0 root         (0) root         (0)     8063 2023-08-05 12:56:32.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/tpkt.py
--rwxr-xr-x   0 root         (0) root         (0)    13551 2023-08-05 12:56:32.000000 rdpy3-1.3.6/rdpy3/protocol/rdp/x224.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.800000 rdpy3-1.3.6/rdpy3/protocol/rfb/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/protocol/rfb/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    25997 2023-08-05 12:56:52.000000 rdpy3-1.3.6/rdpy3/protocol/rfb/rfb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.810000 rdpy3-1.3.6/rdpy3/security/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/security/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    32292 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/security/pyDes.py
--rwxr-xr-x   0 root         (0) root         (0)     1756 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/security/rc4.py
--rwxr-xr-x   0 root         (0) root         (0)     3155 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/security/rsa_wrapper.py
--rwxr-xr-x   0 root         (0) root         (0)     6529 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/security/x509.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.810000 rdpy3-1.3.6/rdpy3/ui/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.6/rdpy3/ui/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14892 2023-08-05 12:56:52.000000 rdpy3-1.3.6/rdpy3/ui/qt5.py
--rwxr-xr-x   0 root         (0) root         (0)     8382 2023-08-05 12:56:32.000000 rdpy3-1.3.6/rdpy3/ui/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.760000 rdpy3-1.3.6/rdpy3.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)     9577 2023-08-05 14:07:09.000000 rdpy3-1.3.6/rdpy3.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1777 2023-08-05 14:07:09.000000 rdpy3-1.3.6/rdpy3.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2023-08-05 14:07:09.000000 rdpy3-1.3.6/rdpy3.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-08-05 14:07:09.000000 rdpy3-1.3.6/rdpy3.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)       10 2023-08-05 14:07:09.000000 rdpy3-1.3.6/rdpy3.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-08-05 14:07:09.850000 rdpy3-1.3.6/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1685 2023-08-05 14:06:46.000000 rdpy3-1.3.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:07:09.840000 rdpy3-1.3.6/test/
--rwxr-xr-x   0 root         (0) root         (0)     1843 2023-08-05 12:56:52.000000 rdpy3-1.3.6/test/test_core_const.py
--rwxr-xr-x   0 root         (0) root         (0)     2636 2023-08-05 12:56:52.000000 rdpy3-1.3.6/test/test_core_layer.py
--rwxr-xr-x   0 root         (0) root         (0)    15634 2023-08-05 12:56:52.000000 rdpy3-1.3.6/test/test_core_type.py
--rwxr-xr-x   0 root         (0) root         (0)     2608 2023-08-05 12:56:52.000000 rdpy3-1.3.6/test/test_protocol_rdp_ber.py
--rwxr-xr-x   0 root         (0) root         (0)     5262 2023-08-05 12:56:32.000000 rdpy3-1.3.6/test/test_protocol_rdp_cssp_ntlm.py
--rwxr-xr-x   0 root         (0) root         (0)     5626 2023-08-05 12:56:52.000000 rdpy3-1.3.6/test/test_protocol_rdp_lic.py
--rwxr-xr-x   0 root         (0) root         (0)     1017 2023-08-05 10:09:26.000000 rdpy3-1.3.6/test/test_protocol_rdp_mcs.py
--rwxr-xr-x   0 root         (0) root         (0)     3604 2023-08-05 12:56:52.000000 rdpy3-1.3.6/test/test_protocol_rdp_per.py
--rwxr-xr-x   0 root         (0) root         (0)     1935 2023-08-05 12:56:52.000000 rdpy3-1.3.6/test/test_protocol_rdp_rc4.py
--rwxr-xr-x   0 root         (0) root         (0)     4098 2023-08-05 12:56:52.000000 rdpy3-1.3.6/test/test_protocol_rdp_tpkt.py
--rwxr-xr-x   0 root         (0) root         (0)     8087 2023-08-05 12:56:52.000000 rdpy3-1.3.6/test/test_protocol_rdp_x224.py
--rwxr-xr-x   0 root         (0) root         (0)      990 2023-08-05 10:09:26.000000 rdpy3-1.3.6/test/test_protocol_rfb_rfb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:58.010000 rdpy3-1.3.7/
+-rwxr-xr-x   0 root         (0) root         (0)    35121 2023-08-05 10:09:26.000000 rdpy3-1.3.7/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)     9578 2023-08-05 14:16:58.000000 rdpy3-1.3.7/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     9291 2023-08-05 14:15:58.000000 rdpy3-1.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.940000 rdpy3-1.3.7/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    10243 2023-08-05 14:06:11.000000 rdpy3-1.3.7/bin/rdpy3-rdpclient.py
+-rwxr-xr-x   0 root         (0) root         (0)     7339 2023-08-05 14:06:11.000000 rdpy3-1.3.7/bin/rdpy3-rdphoneypot.py
+-rwxr-xr-x   0 root         (0) root         (0)    11902 2023-08-05 14:06:11.000000 rdpy3-1.3.7/bin/rdpy3-rdpmitm.py
+-rwxr-xr-x   0 root         (0) root         (0)     8077 2023-08-05 14:06:11.000000 rdpy3-1.3.7/bin/rdpy3-rdpscreenshot.py
+-rwxr-xr-x   0 root         (0) root         (0)     4405 2023-08-05 14:06:11.000000 rdpy3-1.3.7/bin/rdpy3-rssplayer.py
+-rwxr-xr-x   0 root         (0) root         (0)     3344 2023-08-05 14:06:11.000000 rdpy3-1.3.7/bin/rdpy3-vncclient.py
+-rwxr-xr-x   0 root         (0) root         (0)     6164 2023-08-05 14:06:11.000000 rdpy3-1.3.7/bin/rdpy3-vncscreenshot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.940000 rdpy3-1.3.7/ext/
+-rwxr-xr-x   0 root         (0) root         (0)    19035 2023-08-05 13:03:01.000000 rdpy3-1.3.7/ext/rle.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.940000 rdpy3-1.3.7/rdpy3/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.950000 rdpy3-1.3.7/rdpy3/core/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/core/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2505 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/core/const.py
+-rwxr-xr-x   0 root         (0) root         (0)     3014 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/core/error.py
+-rwxr-xr-x   0 root         (0) root         (0)     3507 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/core/filetimes.py
+-rwxr-xr-x   0 root         (0) root         (0)     8950 2023-08-05 12:56:32.000000 rdpy3-1.3.7/rdpy3/core/layer.py
+-rwxr-xr-x   0 root         (0) root         (0)     1976 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/core/log.py
+-rwxr-xr-x   0 root         (0) root         (0)     9547 2023-08-05 12:56:32.000000 rdpy3-1.3.7/rdpy3/core/rss.py
+-rwxr-xr-x   0 root         (0) root         (0)     1443 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/core/scancode.py
+-rwxr-xr-x   0 root         (0) root         (0)    40003 2023-08-05 12:56:52.000000 rdpy3-1.3.7/rdpy3/core/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.950000 rdpy3-1.3.7/rdpy3/protocol/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.960000 rdpy3-1.3.7/rdpy3/protocol/rdp/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14313 2023-08-05 12:56:52.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/lic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.970000 rdpy3-1.3.7/rdpy3/protocol/rdp/nla/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/nla/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    13391 2023-08-05 12:56:32.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/nla/cssp.py
+-rwxr-xr-x   0 root         (0) root         (0)    24730 2023-08-05 12:56:52.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/nla/ntlm.py
+-rwxr-xr-x   0 root         (0) root         (0)     2808 2023-08-05 12:56:32.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/nla/sspi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.980000 rdpy3-1.3.7/rdpy3/protocol/rdp/pdu/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/pdu/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    19191 2023-08-05 12:56:52.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/pdu/caps.py
+-rwxr-xr-x   0 root         (0) root         (0)    51908 2023-08-05 12:58:17.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/pdu/data.py
+-rwxr-xr-x   0 root         (0) root         (0)    27792 2023-08-05 12:58:17.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/pdu/layer.py
+-rwxr-xr-x   0 root         (0) root         (0)     4840 2023-08-05 12:56:32.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/pdu/order.py
+-rwxr-xr-x   0 root         (0) root         (0)    28629 2023-08-05 12:58:17.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/rdp.py
+-rwxr-xr-x   0 root         (0) root         (0)    27591 2023-08-05 12:58:17.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/sec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.980000 rdpy3-1.3.7/rdpy3/protocol/rdp/t125/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/t125/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7574 2023-08-05 12:56:32.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/t125/ber.py
+-rwxr-xr-x   0 root         (0) root         (0)    23674 2023-08-05 12:58:17.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/t125/gcc.py
+-rwxr-xr-x   0 root         (0) root         (0)    24771 2023-08-05 12:58:17.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/t125/mcs.py
+-rwxr-xr-x   0 root         (0) root         (0)     7966 2023-08-05 12:56:32.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/t125/per.py
+-rwxr-xr-x   0 root         (0) root         (0)     8063 2023-08-05 12:56:32.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/tpkt.py
+-rwxr-xr-x   0 root         (0) root         (0)    13551 2023-08-05 12:56:32.000000 rdpy3-1.3.7/rdpy3/protocol/rdp/x224.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.990000 rdpy3-1.3.7/rdpy3/protocol/rfb/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/protocol/rfb/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    25997 2023-08-05 12:56:52.000000 rdpy3-1.3.7/rdpy3/protocol/rfb/rfb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.990000 rdpy3-1.3.7/rdpy3/security/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/security/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    32292 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/security/pyDes.py
+-rwxr-xr-x   0 root         (0) root         (0)     1756 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/security/rc4.py
+-rwxr-xr-x   0 root         (0) root         (0)     3155 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/security/rsa_wrapper.py
+-rwxr-xr-x   0 root         (0) root         (0)     6529 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/security/x509.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:58.000000 rdpy3-1.3.7/rdpy3/ui/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.7/rdpy3/ui/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14892 2023-08-05 12:56:52.000000 rdpy3-1.3.7/rdpy3/ui/qt5.py
+-rwxr-xr-x   0 root         (0) root         (0)     8382 2023-08-05 12:56:32.000000 rdpy3-1.3.7/rdpy3/ui/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:57.940000 rdpy3-1.3.7/rdpy3.egg-info/
+-rwxr-xr-x   0 root         (0) root         (0)     9578 2023-08-05 14:16:57.000000 rdpy3-1.3.7/rdpy3.egg-info/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     1777 2023-08-05 14:16:57.000000 rdpy3-1.3.7/rdpy3.egg-info/SOURCES.txt
+-rwxr-xr-x   0 root         (0) root         (0)        1 2023-08-05 14:16:57.000000 rdpy3-1.3.7/rdpy3.egg-info/dependency_links.txt
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-08-05 14:16:57.000000 rdpy3-1.3.7/rdpy3.egg-info/requires.txt
+-rwxr-xr-x   0 root         (0) root         (0)       10 2023-08-05 14:16:57.000000 rdpy3-1.3.7/rdpy3.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)       38 2023-08-05 14:16:58.010000 rdpy3-1.3.7/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1685 2023-08-05 14:16:31.000000 rdpy3-1.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:16:58.000000 rdpy3-1.3.7/test/
+-rwxr-xr-x   0 root         (0) root         (0)     1850 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_core_const.py
+-rwxr-xr-x   0 root         (0) root         (0)     2642 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_core_layer.py
+-rwxr-xr-x   0 root         (0) root         (0)    15731 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_core_type.py
+-rwxr-xr-x   0 root         (0) root         (0)     2609 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_protocol_rdp_ber.py
+-rwxr-xr-x   0 root         (0) root         (0)     5263 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_protocol_rdp_cssp_ntlm.py
+-rwxr-xr-x   0 root         (0) root         (0)     5627 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_protocol_rdp_lic.py
+-rwxr-xr-x   0 root         (0) root         (0)     1018 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_protocol_rdp_mcs.py
+-rwxr-xr-x   0 root         (0) root         (0)     3605 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_protocol_rdp_per.py
+-rwxr-xr-x   0 root         (0) root         (0)     1936 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_protocol_rdp_rc4.py
+-rwxr-xr-x   0 root         (0) root         (0)     4099 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_protocol_rdp_tpkt.py
+-rwxr-xr-x   0 root         (0) root         (0)     8088 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_protocol_rdp_x224.py
+-rwxr-xr-x   0 root         (0) root         (0)      991 2023-08-05 14:15:58.000000 rdpy3-1.3.7/test/test_protocol_rfb_rfb.py
```

### Comparing `rdpy3-1.3.6/LICENSE` & `rdpy3-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/PKG-INFO` & `rdpy3-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdpy3
-Version: 1.3.6
+Version: 1.3.7
 Summary: Remote Desktop Protocol in Python3
 Home-page: https://github.com/james4ever0/rdpy3
 Author: Sylvain Peyrefitte
 Author-email: citronneur@gmail.com
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -123,15 +123,15 @@
 
 ```
 $ rdpy3-rssplayer.py rss_file_path
 ```
 
 ## RDPY Qt Widget
 
-RDPY can also be used as Qt widget through rdpy.ui.qt5.QRemoteDesktop class. It can be embedded in your own Qt application. qt5reactor must be used in your app for Twisted and Qt to work together. For more details, see sources of rdpy3-rdpclient.
+RDPY can also be used as Qt widget through rdpy3.ui.qt5.QRemoteDesktop class. It can be embedded in your own Qt application. qt5reactor must be used in your app for Twisted and Qt to work together. For more details, see sources of rdpy3-rdpclient.
 
 ## RDPY library
 
 In a nutshell RDPY can be used as a protocol library with a twisted engine.
 
 ### Simple RDP Client
```

### Comparing `rdpy3-1.3.6/README.md` & `rdpy3-1.3.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 ```
 $ rdpy3-rssplayer.py rss_file_path
 ```
 
 ## RDPY Qt Widget
 
-RDPY can also be used as Qt widget through rdpy.ui.qt5.QRemoteDesktop class. It can be embedded in your own Qt application. qt5reactor must be used in your app for Twisted and Qt to work together. For more details, see sources of rdpy3-rdpclient.
+RDPY can also be used as Qt widget through rdpy3.ui.qt5.QRemoteDesktop class. It can be embedded in your own Qt application. qt5reactor must be used in your app for Twisted and Qt to work together. For more details, see sources of rdpy3-rdpclient.
 
 ## RDPY library
 
 In a nutshell RDPY can be used as a protocol library with a twisted engine.
 
 ### Simple RDP Client
```

### Comparing `rdpy3-1.3.6/bin/rdpy3-rdpclient.py` & `rdpy3-1.3.7/bin/rdpy3-rdpclient.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/bin/rdpy3-rdphoneypot.py` & `rdpy3-1.3.7/bin/rdpy3-rdphoneypot.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/bin/rdpy3-rdpmitm.py` & `rdpy3-1.3.7/bin/rdpy3-rdpmitm.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/bin/rdpy3-rdpscreenshot.py` & `rdpy3-1.3.7/bin/rdpy3-rdpscreenshot.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/bin/rdpy3-rssplayer.py` & `rdpy3-1.3.7/bin/rdpy3-rssplayer.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/bin/rdpy3-vncclient.py` & `rdpy3-1.3.7/bin/rdpy3-vncclient.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/bin/rdpy3-vncscreenshot.py` & `rdpy3-1.3.7/bin/rdpy3-vncscreenshot.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/ext/rle.c` & `rdpy3-1.3.7/ext/rle.c`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/core/const.py` & `rdpy3-1.3.7/rdpy3/core/const.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/core/error.py` & `rdpy3-1.3.7/rdpy3/core/error.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/core/filetimes.py` & `rdpy3-1.3.7/rdpy3/core/filetimes.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/core/layer.py` & `rdpy3-1.3.7/rdpy3/core/layer.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/core/log.py` & `rdpy3-1.3.7/rdpy3/core/log.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/core/rss.py` & `rdpy3-1.3.7/rdpy3/core/rss.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/core/scancode.py` & `rdpy3-1.3.7/rdpy3/core/scancode.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/core/type.py` & `rdpy3-1.3.7/rdpy3/core/type.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/lic.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/lic.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/nla/cssp.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/nla/cssp.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/nla/ntlm.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/nla/ntlm.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/nla/sspi.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/nla/sspi.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/pdu/caps.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/pdu/caps.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/pdu/data.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/pdu/data.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/pdu/layer.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/pdu/layer.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/pdu/order.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/pdu/order.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/rdp.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/rdp.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/sec.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/sec.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/t125/ber.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/t125/ber.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/t125/gcc.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/t125/gcc.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/t125/mcs.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/t125/mcs.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/t125/per.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/t125/per.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/tpkt.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/tpkt.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rdp/x224.py` & `rdpy3-1.3.7/rdpy3/protocol/rdp/x224.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/protocol/rfb/rfb.py` & `rdpy3-1.3.7/rdpy3/protocol/rfb/rfb.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/security/pyDes.py` & `rdpy3-1.3.7/rdpy3/security/pyDes.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/security/rc4.py` & `rdpy3-1.3.7/rdpy3/security/rc4.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/security/rsa_wrapper.py` & `rdpy3-1.3.7/rdpy3/security/rsa_wrapper.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/security/x509.py` & `rdpy3-1.3.7/rdpy3/security/x509.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/ui/qt5.py` & `rdpy3-1.3.7/rdpy3/ui/qt5.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3/ui/view.py` & `rdpy3-1.3.7/rdpy3/ui/view.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/rdpy3.egg-info/PKG-INFO` & `rdpy3-1.3.7/rdpy3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdpy3
-Version: 1.3.6
+Version: 1.3.7
 Summary: Remote Desktop Protocol in Python3
 Home-page: https://github.com/james4ever0/rdpy3
 Author: Sylvain Peyrefitte
 Author-email: citronneur@gmail.com
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -123,15 +123,15 @@
 
 ```
 $ rdpy3-rssplayer.py rss_file_path
 ```
 
 ## RDPY Qt Widget
 
-RDPY can also be used as Qt widget through rdpy.ui.qt5.QRemoteDesktop class. It can be embedded in your own Qt application. qt5reactor must be used in your app for Twisted and Qt to work together. For more details, see sources of rdpy3-rdpclient.
+RDPY can also be used as Qt widget through rdpy3.ui.qt5.QRemoteDesktop class. It can be embedded in your own Qt application. qt5reactor must be used in your app for Twisted and Qt to work together. For more details, see sources of rdpy3-rdpclient.
 
 ## RDPY library
 
 In a nutshell RDPY can be used as a protocol library with a twisted engine.
 
 ### Simple RDP Client
```

### Comparing `rdpy3-1.3.6/rdpy3.egg-info/SOURCES.txt` & `rdpy3-1.3.7/rdpy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.6/setup.py` & `rdpy3-1.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 import setuptools
 from distutils.core import setup, Extension
 
 setup(name='rdpy3',
-      version='1.3.6',
+      version='1.3.7',
       description='Remote Desktop Protocol in Python3',
       long_description_content_type="text/markdown",
       python_requires=">=3",
       long_description=open("README.md").read(),
       # long_description="""
       # RDPY is a pure Python implementation of the Microsoft RDP (Remote Desktop Protocol) protocol (Client and Server side). RDPY is built over the event driven network engine Twisted.
```

### Comparing `rdpy3-1.3.6/test/test_core_const.py` & `rdpy3-1.3.7/test/test_core_const.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,45 +14,45 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.core.const module
+unit test for rdpy3.core.const module
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
 import rdpy3.core.const
 import rdpy3.core.type
 
 class ConstTest(unittest.TestCase):
     '''
     represent test case for all classes and function
-    present in rdpy.base.const
+    present in rdpy3.base.const
     '''
     def test_type_attributes(self):
         '''
         test if type attributes decorator works
         '''
-        @rdpy.core.const.TypeAttributes(rdpy.core.type.UInt16Le)
+        @rdpy3.core.const.TypeAttributes(rdpy3.core.type.UInt16Le)
         class Test:
             MEMBER_1 = 1
             MEMBER_2 = 2
         
-        self.assertIsInstance(Test.MEMBER_1, rdpy.core.type.UInt16Le, "MEMBER_1 is not in correct type")
-        self.assertIsInstance(Test.MEMBER_2, rdpy.core.type.UInt16Le, "MEMBER_2 is not in correct type")
+        self.assertIsInstance(Test.MEMBER_1, rdpy3.core.type.UInt16Le, "MEMBER_1 is not in correct type")
+        self.assertIsInstance(Test.MEMBER_2, rdpy3.core.type.UInt16Le, "MEMBER_2 is not in correct type")
         
     def test_const(self):
         '''
         test if get on const class member generate new object each
         '''
-        @rdpy.core.const.ConstAttributes
+        @rdpy3.core.const.ConstAttributes
         class Test:
             MEMBER_1 = 1
             MEMBER_2 = 2
             
         self.assertEquals(Test.MEMBER_1, Test.MEMBER_1, "handle same type of object")
```

### Comparing `rdpy3-1.3.6/test/test_core_layer.py` & `rdpy3-1.3.7/test/test_core_layer.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,64 +14,64 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.network.layer module
+unit test for rdpy3.network.layer module
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
 import rdpy3.core.layer
 
 class LayerTest(unittest.TestCase):
     """
     @summary:  represent test case for all classes and function
-                present in rdpy.core.layer
+                present in rdpy3.core.layer
     """
     
     class LayerCaseException(Exception):
         """
         @summary: exception use for event base test
         """
         pass
     
     def test_layer_connect_event(self):
         """
         @summary: test if connect event is send from transport to presentation
         """
-        class TestConnect(rdpy.core.layer.Layer):
+        class TestConnect(rdpy3.core.layer.Layer):
             def connect(self):
                 raise LayerTest.LayerCaseException()
             
-        self.assertRaises(LayerTest.LayerCaseException, rdpy.core.layer.Layer(presentation = TestConnect()).connect)
+        self.assertRaises(LayerTest.LayerCaseException, rdpy3.core.layer.Layer(presentation = TestConnect()).connect)
         
     def test_layer_automata_more_than_expected(self):
         """
         @summary: test layer automata mechanism if data received is more than expected
         """
-        class TestAutomata(rdpy.core.layer.RawLayer):
+        class TestAutomata(rdpy3.core.layer.RawLayer):
             def expectedCallBack(self, data):
                 if data.dataLen() == 4:
                     raise LayerTest.LayerCaseException()
             
         t = TestAutomata()
         t.expect(4, t.expectedCallBack)
         self.assertRaises(LayerTest.LayerCaseException, t.dataReceived, "\x00\x00\x00\x00\x00")
         
     def test_layer_automata_less_than_expected(self):
         """
         @summary: test layer automata mechanism
         """
-        class TestAutomata(rdpy.core.layer.RawLayer):
+        class TestAutomata(rdpy3.core.layer.RawLayer):
             def expectedCallBack(self, data):
                 if data.dataLen() == 4:
                     raise LayerTest.LayerCaseException()
             
         t = TestAutomata()
         t.expect(4, t.expectedCallBack)
         self.assertEqual(t.dataReceived("\x00\x00\x00"), None, "Not enough dada")
```

### Comparing `rdpy3-1.3.6/test/test_core_type.py` & `rdpy3-1.3.7/test/test_core_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,378 +14,378 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.network.type module
+unit test for rdpy3.network.type module
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
 import rdpy3.core.type
 from rdpy3.core.error import InvalidSize
 
 class TypeTest(unittest.TestCase):
     """
     @summary: represent test case for all classes and function
-                present in rdpy.network.type
+                present in rdpy3.network.type
     """
     def test_callable_value_const(self):
         """
         @summary: test if callable value with const ctor doesn't change value
         """
-        c = rdpy.core.type.CallableValue(5)
+        c = rdpy3.core.type.CallableValue(5)
         self.assertEqual(c.value, 5, "invalid callable const")
         
     def test_callable_value_lambda(self):
         """
         @summary: test if callable value with lambda ctor return dynamic value
         """
-        c = rdpy.core.type.CallableValue(lambda:5)
+        c = rdpy3.core.type.CallableValue(lambda:5)
         self.assertEqual(c.value, 5, "invalid callable lambda")
     
     def test_type_write_conditional_true(self):
         """
         @summary: test when write is obligatory call write function
         """
-        class TestType(rdpy.core.type.Type):
+        class TestType(rdpy3.core.type.Type):
             def __write__(self, s):
                 raise Exception()
-        s = rdpy.core.type.Stream()
+        s = rdpy3.core.type.Stream()
         self.assertRaises(Exception, s.writeType, TestType(conditional = lambda:True))
     
     @unittest.expectedFailure
     def test_type_write_conditional_false(self):
         """
         @summary: test when write doesn't needed, doesn't call write function
         """
-        class TestType(rdpy.core.type.Type):
+        class TestType(rdpy3.core.type.Type):
             def __write__(self, s):
                 raise Exception()
-        s = rdpy.core.type.Stream()
+        s = rdpy3.core.type.Stream()
         self.assertRaises(Exception, s.writeType, TestType(conditional = lambda:False))
         
     def test_type_read_conditional_true(self):
         """
         @summary: test when read is obligatory call write function
         """
-        class TestType(rdpy.core.type.Type):
+        class TestType(rdpy3.core.type.Type):
             def __read__(self, s):
                 raise Exception()
-        s = rdpy.core.type.Stream()
+        s = rdpy3.core.type.Stream()
         self.assertRaises(Exception, s.readType, TestType(conditional = lambda:True))
     
     @unittest.expectedFailure
     def test_type_read_conditional_false(self):
         """
         @summary: test when read doesn't needed, doesn't call read function
         """
-        class TestType(rdpy.core.type.Type):
+        class TestType(rdpy3.core.type.Type):
             def __read__(self, s):
                 raise Exception()
-        s = rdpy.core.type.Stream()
+        s = rdpy3.core.type.Stream()
         self.assertRaises(Exception, s.readType, TestType(conditional = lambda:False))
         
     
     def test_sizeof_conditional_true(self):
         """
         @summary: test if sizeof of simple type is init value(4) when type is conditional true
         """
-        v = rdpy.core.type.SimpleType("I", 4, False, 0, conditional = lambda:True)
-        self.assertEqual(rdpy.core.type.sizeof(v), 4, "invalid sizeof")
+        v = rdpy3.core.type.SimpleType("I", 4, False, 0, conditional = lambda:True)
+        self.assertEqual(rdpy3.core.type.sizeof(v), 4, "invalid sizeof")
         
     def test_sizeof_conditional_false(self):
         """
         @summary: test if sizeof of simple type is 0 when type is conditional false
         """
-        v = rdpy.core.type.SimpleType("I", 4, False, 0, conditional = lambda:False)
-        self.assertEqual(rdpy.core.type.sizeof(v), 0, "invalid sizeof")
+        v = rdpy3.core.type.SimpleType("I", 4, False, 0, conditional = lambda:False)
+        self.assertEqual(rdpy3.core.type.sizeof(v), 0, "invalid sizeof")
         
     def test_sizeof_list(self):
         """
         @summary: test call sizeof on list of type
         """
-        v = [rdpy.core.type.UInt8(), rdpy.core.type.UInt16Le(), rdpy.core.type.UInt32Le()]
-        self.assertEqual(rdpy.core.type.sizeof(v), 7, "invalid sizeof")
+        v = [rdpy3.core.type.UInt8(), rdpy3.core.type.UInt16Le(), rdpy3.core.type.UInt32Le()]
+        self.assertEqual(rdpy3.core.type.sizeof(v), 7, "invalid sizeof")
         
     def test_sizeof_list_conditional(self):
         """
         @summary: test call sizeof on list of type with one type hidden
         """
-        v = [rdpy.core.type.UInt8(), rdpy.core.type.UInt16Le(conditional = lambda:False), rdpy.core.type.UInt32Le()]
-        self.assertEqual(rdpy.core.type.sizeof(v), 5, "invalid sizeof")
+        v = [rdpy3.core.type.UInt8(), rdpy3.core.type.UInt16Le(conditional = lambda:False), rdpy3.core.type.UInt32Le()]
+        self.assertEqual(rdpy3.core.type.sizeof(v), 5, "invalid sizeof")
         
     def test_sizeof_tuple(self):
         """
         @summary: test call sizeof on tuple of type
         """
-        v = [rdpy.core.type.UInt8(), rdpy.core.type.UInt16Le(), rdpy.core.type.UInt32Le()]
-        self.assertEqual(rdpy.core.type.sizeof(v), 7, "invalid sizeof")
+        v = [rdpy3.core.type.UInt8(), rdpy3.core.type.UInt16Le(), rdpy3.core.type.UInt32Le()]
+        self.assertEqual(rdpy3.core.type.sizeof(v), 7, "invalid sizeof")
         
     def test_sizeof_tuple_conditional(self):
         """
         @summary: test call sizeof on tuple of type with one type hidden
         """
-        v = (rdpy.core.type.UInt8(), rdpy.core.type.UInt16Le(), rdpy.core.type.UInt32Le(conditional = lambda:False))
-        self.assertEqual(rdpy.core.type.sizeof(v), 3, "invalid sizeof")
+        v = (rdpy3.core.type.UInt8(), rdpy3.core.type.UInt16Le(), rdpy3.core.type.UInt32Le(conditional = lambda:False))
+        self.assertEqual(rdpy3.core.type.sizeof(v), 3, "invalid sizeof")
         
     def test_stream_write_uint8_type(self):
         """
         @summary: test write uint8 in stream
         """
-        s = rdpy.core.type.Stream()
-        s.writeType(rdpy.core.type.UInt8(1))
+        s = rdpy3.core.type.Stream()
+        s.writeType(rdpy3.core.type.UInt8(1))
         self.assertEqual(''.join(s.buflist), '\x01', "invalid stream write")
         
     def test_stream_write_uint16Le_type(self):
         """
         @summary: test write UInt16Le in stream
         """
-        s = rdpy.core.type.Stream()
-        s.writeType(rdpy.core.type.UInt16Le(1))
+        s = rdpy3.core.type.Stream()
+        s.writeType(rdpy3.core.type.UInt16Le(1))
         self.assertEqual(''.join(s.buflist), '\x01\x00', "invalid stream write")
     
     def test_stream_write_uint16Be_type(self):
         """
         @summary: test write UInt16Be in stream
         """
-        s = rdpy.core.type.Stream()
-        s.writeType(rdpy.core.type.UInt16Be(1))
+        s = rdpy3.core.type.Stream()
+        s.writeType(rdpy3.core.type.UInt16Be(1))
         self.assertEqual(''.join(s.buflist), '\x00\x01', "invalid stream write")
         
     def test_stream_write_uint24Le_type(self):
         """
         @summary: test write UInt24Le in stream
         """
-        s = rdpy.core.type.Stream()
-        s.writeType(rdpy.core.type.UInt24Le(1))
+        s = rdpy3.core.type.Stream()
+        s.writeType(rdpy3.core.type.UInt24Le(1))
         self.assertEqual(''.join(s.buflist), '\x01\x00\x00', "invalid stream write")
     
     def test_stream_write_uint24Be_type(self):
         """
         @summary: test write uint24Be in stream
         """
-        s = rdpy.core.type.Stream()
-        s.writeType(rdpy.core.type.UInt24Be(1))
+        s = rdpy3.core.type.Stream()
+        s.writeType(rdpy3.core.type.UInt24Be(1))
         self.assertEqual(''.join(s.buflist), '\x00\x00\x01', "invalid stream write")
         
     def test_stream_write_uint32Le_type(self):
         """
         @summary: test write UInt32Le in stream
         """
-        s = rdpy.core.type.Stream()
-        s.writeType(rdpy.core.type.UInt32Le(1))
+        s = rdpy3.core.type.Stream()
+        s.writeType(rdpy3.core.type.UInt32Le(1))
         self.assertEqual(''.join(s.buflist), '\x01\x00\x00\x00', "invalid stream write")
     
     def test_stream_write_uint32Be_type(self):
         """
         @summary: test write UInt32Be in stream
         """
-        s = rdpy.core.type.Stream()
-        s.writeType(rdpy.core.type.UInt32Be(1))
+        s = rdpy3.core.type.Stream()
+        s.writeType(rdpy3.core.type.UInt32Be(1))
         self.assertEqual(''.join(s.buflist), '\x00\x00\x00\x01', "invalid stream write")
         
     def test_stream_read_uint8_type(self):
         """
         @summary: test read UInt8 type from stream
         """
-        s = rdpy.core.type.Stream('\x01')
-        t = rdpy.core.type.UInt8()
+        s = rdpy3.core.type.Stream('\x01')
+        t = rdpy3.core.type.UInt8()
         s.readType(t)
         self.assertEqual(t.value, 1, "invalid stream read value")
         self.assertEqual(s.dataLen(), 0, "not read all stream")
         
     def test_stream_read_uint16Le_type(self):
         """
         @summary: test read UInt16Le type from stream
         """
-        s = rdpy.core.type.Stream('\x01\x00')
-        t = rdpy.core.type.UInt16Le()
+        s = rdpy3.core.type.Stream('\x01\x00')
+        t = rdpy3.core.type.UInt16Le()
         s.readType(t)
         self.assertEqual(t.value, 1, "invalid stream read value")
         self.assertEqual(s.dataLen(), 0, "not read all stream")
         
     def test_stream_read_uint16Be_type(self):
         """
         @summary: test read UInt16Be type from stream
         """
-        s = rdpy.core.type.Stream('\x00\x01')
-        t = rdpy.core.type.UInt16Be()
+        s = rdpy3.core.type.Stream('\x00\x01')
+        t = rdpy3.core.type.UInt16Be()
         s.readType(t)
         self.assertEqual(t.value, 1, "invalid stream read value")
         self.assertEqual(s.dataLen(), 0, "not read all stream")
         
     def test_stream_read_uint24Le_type(self):
         """
         @summary: test read UInt24Le type from stream
         """
-        s = rdpy.core.type.Stream('\x01\x00\x00')
-        t = rdpy.core.type.UInt24Le()
+        s = rdpy3.core.type.Stream('\x01\x00\x00')
+        t = rdpy3.core.type.UInt24Le()
         s.readType(t)
         self.assertEqual(t.value, 1, "invalid stream read value")
         self.assertEqual(s.dataLen(), 0, "not read all stream")
         
     def test_stream_read_uint24Be_type(self):
         """
         @summary: test read UInt24Be type from stream
         """
-        s = rdpy.core.type.Stream('\x00\x00\x01')
-        t = rdpy.core.type.UInt24Be()
+        s = rdpy3.core.type.Stream('\x00\x00\x01')
+        t = rdpy3.core.type.UInt24Be()
         s.readType(t)
         self.assertEqual(t.value, 1, "invalid stream read")
         self.assertEqual(s.dataLen(), 0, "not read all stream")
         
     def test_stream_read_uint32Le_type(self):
         """
         @summary: test read UInt32Le type from stream
         """
-        s = rdpy.core.type.Stream('\x01\x00\x00\x00')
-        t = rdpy.core.type.UInt32Le()
+        s = rdpy3.core.type.Stream('\x01\x00\x00\x00')
+        t = rdpy3.core.type.UInt32Le()
         s.readType(t)
         self.assertEqual(t.value, 1, "invalid stream read value")
         self.assertEqual(s.dataLen(), 0, "not read all stream")
         
     def test_stream_read_uint32Be_type(self):
         """
         @summary: test read UInt32Be type from stream
         """
-        s = rdpy.core.type.Stream('\x00\x00\x00\x01')
-        t = rdpy.core.type.UInt32Be()
+        s = rdpy3.core.type.Stream('\x00\x00\x00\x01')
+        t = rdpy3.core.type.UInt32Be()
         s.readType(t)
         self.assertEqual(t.value, 1, "invalid stream read")
         self.assertEqual(s.dataLen(), 0, "not read all stream")
         
     def test_stream_read_optional_singletype(self):
         """
         @summary: test optional option in case of simple type reading
         """
         #unsigned int case
-        t = rdpy.core.type.SimpleType("I", 4, False, 0, optional = True)
+        t = rdpy3.core.type.SimpleType("I", 4, False, 0, optional = True)
         #empty stream
-        s1 = rdpy.core.type.Stream()
+        s1 = rdpy3.core.type.Stream()
         s1.readType(t)
         self.assertEqual(t.value, 0, "invalid stream read optional value")
         
     def test_stream_read_conditional_singletype_false(self):
         """
         @summary: test conditional option in case of simple type reading and when condition is false (not read)
         """
         #unsigned int case
-        t = rdpy.core.type.SimpleType("I", 4, False, 0, conditional = lambda:False)
-        s1 = rdpy.core.type.Stream("\x01\x00\x00\x00")
+        t = rdpy3.core.type.SimpleType("I", 4, False, 0, conditional = lambda:False)
+        s1 = rdpy3.core.type.Stream("\x01\x00\x00\x00")
         s1.readType(t)
         self.assertEqual(t.value, 0, "invalid stream read conditional value")
         
     def test_stream_read_conditional_singletype_true(self):
         """
         @summary: test conditional option in case of simple type reading and when condition is true (must be read)
         """
         #unsigned int case
-        t = rdpy.core.type.SimpleType("I", 4, False, 0, conditional = lambda:True)
-        s1 = rdpy.core.type.Stream("\x01\x00\x00\x00")
+        t = rdpy3.core.type.SimpleType("I", 4, False, 0, conditional = lambda:True)
+        s1 = rdpy3.core.type.Stream("\x01\x00\x00\x00")
         s1.readType(t)
         self.assertEqual(t.value, 1, "invalid stream read conditional value")
         
     def test_stream_read_rollback_constant_constraint(self):
         """
         @summary: test if constant constraint fail, the reading stream is correctly rollback
         """
-        class TestComposite(rdpy.core.type.CompositeType):
+        class TestComposite(rdpy3.core.type.CompositeType):
             def __init__(self):
-                rdpy.core.type.CompositeType.__init__(self)
-                self.padding = rdpy.core.type.UInt32Le(0)
-                self.constraint = rdpy.core.type.UInt32Le(1, constant = True)
+                rdpy3.core.type.CompositeType.__init__(self)
+                self.padding = rdpy3.core.type.UInt32Le(0)
+                self.constraint = rdpy3.core.type.UInt32Le(1, constant = True)
                 
-        s = rdpy.core.type.Stream("\x00\x00\x00\x00\x00\x00\x00\x00")
+        s = rdpy3.core.type.Stream("\x00\x00\x00\x00\x00\x00\x00\x00")
         try:
             s.readType(TestComposite())
         except Exception:
             self.assertEqual(s.readLen(), 0, "invalid stream roll back operation")
             return
         self.assertTrue(False, "Constant constraint fail")
         
     def test_stream_read_rollback_constant_constraint_recurcive(self):
         """
         @summary: test if constant constraint fail even in recurcive composite type, 
         the reading stream is correctly rollback
         """
-        class TestSubComposite(rdpy.core.type.CompositeType):
+        class TestSubComposite(rdpy3.core.type.CompositeType):
             def __init__(self):
-                rdpy.core.type.CompositeType.__init__(self)
-                self.padding = rdpy.core.type.UInt32Le(0)
-                self.constraint = rdpy.core.type.UInt32Le(1, constant = True)
+                rdpy3.core.type.CompositeType.__init__(self)
+                self.padding = rdpy3.core.type.UInt32Le(0)
+                self.constraint = rdpy3.core.type.UInt32Le(1, constant = True)
                 
-        class TestComposite(rdpy.core.type.CompositeType):
+        class TestComposite(rdpy3.core.type.CompositeType):
             def __init__(self):
-                rdpy.core.type.CompositeType.__init__(self)
-                self.padding = rdpy.core.type.UInt32Le(0)
+                rdpy3.core.type.CompositeType.__init__(self)
+                self.padding = rdpy3.core.type.UInt32Le(0)
                 self.recurcive = TestSubComposite()
                 
-        s = rdpy.core.type.Stream("\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00")
+        s = rdpy3.core.type.Stream("\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00")
         try:
             s.readType(TestComposite())
         except Exception:
             self.assertEqual(s.readLen(), 0, "invalid stream roll back operation")
             return
         self.assertTrue(False, "Constant constraint fail")
     
     def test_stream_read_rollback_not_enough_data(self):
         """
         @summary: test if constant constraint fail even in recurcive composite type, 
         the reading stream is correctly rollback
         """
-        class TestSubComposite(rdpy.core.type.CompositeType):
+        class TestSubComposite(rdpy3.core.type.CompositeType):
             def __init__(self):
-                rdpy.core.type.CompositeType.__init__(self)
-                self.padding = rdpy.core.type.UInt32Le(0)
-                self.constraint = rdpy.core.type.UInt32Le(1)
+                rdpy3.core.type.CompositeType.__init__(self)
+                self.padding = rdpy3.core.type.UInt32Le(0)
+                self.constraint = rdpy3.core.type.UInt32Le(1)
                 
-        class TestComposite(rdpy.core.type.CompositeType):
+        class TestComposite(rdpy3.core.type.CompositeType):
             def __init__(self):
-                rdpy.core.type.CompositeType.__init__(self)
-                self.padding = rdpy.core.type.UInt32Le(0)
+                rdpy3.core.type.CompositeType.__init__(self)
+                self.padding = rdpy3.core.type.UInt32Le(0)
                 self.recurcive = TestSubComposite()
                 
-        s = rdpy.core.type.Stream("\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00")
+        s = rdpy3.core.type.Stream("\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00")
         try:
             s.readType(TestComposite())
         except Exception:
             self.assertEqual(s.readLen(), 0, "invalid stream roll back operation")
             return
         self.assertTrue(False, "Constant constraint fail")
         
     def test_stream_read_with_static_length_superior(self):
         """
         @summary: test read stream with a length forced
                     if total stream read length < to forced read length 
                     the trash must be read as padding
         """
-        class TestReadLength(rdpy.core.type.CompositeType):
+        class TestReadLength(rdpy3.core.type.CompositeType):
             def __init__(self, readLen):
-                rdpy.core.type.CompositeType.__init__(self, readLen = readLen)
-                self.padding = rdpy.core.type.UInt32Le(0)
-        s = rdpy.core.type.Stream("\x00" * 10)
-        s.readType(TestReadLength(rdpy.core.type.UInt8(10)))
+                rdpy3.core.type.CompositeType.__init__(self, readLen = readLen)
+                self.padding = rdpy3.core.type.UInt32Le(0)
+        s = rdpy3.core.type.Stream("\x00" * 10)
+        s.readType(TestReadLength(rdpy3.core.type.UInt8(10)))
         self.assertEqual(s.dataLen(), 0, "invalid stream read trash data as padding")
         
     def test_stream_read_with_static_length_inferior(self):
         """
         @summary: test read stream with a length forced
                     if total stream read length > to forced read length 
                     an InvalidSize exception is throw
         """
-        class TestReadLength(rdpy.core.type.CompositeType):
+        class TestReadLength(rdpy3.core.type.CompositeType):
             def __init__(self, readLen):
-                rdpy.core.type.CompositeType.__init__(self, readLen = readLen)
-                self.padding = rdpy.core.type.UInt32Le(0)
-        s = rdpy.core.type.Stream("\x00" * 10)
-        self.assertRaises(InvalidSize, s.readType, TestReadLength(rdpy.core.type.UInt8(2)))
+                rdpy3.core.type.CompositeType.__init__(self, readLen = readLen)
+                self.padding = rdpy3.core.type.UInt32Le(0)
+        s = rdpy3.core.type.Stream("\x00" * 10)
+        self.assertRaises(InvalidSize, s.readType, TestReadLength(rdpy3.core.type.UInt8(2)))
         
     def test_stream_read_string(self):
         """
         @summary: read stream as string buffer
         """
```

### Comparing `rdpy3-1.3.6/test/test_protocol_rdp_ber.py` & `rdpy3-1.3.7/test/test_protocol_rdp_ber.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.protocol.rdp.ber module
+unit test for rdpy3.protocol.rdp.ber module
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
```

### Comparing `rdpy3-1.3.6/test/test_protocol_rdp_cssp_ntlm.py` & `rdpy3-1.3.7/test/test_protocol_rdp_cssp_ntlm.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.protocol.rdp.nla.cssp and ntlm module
+unit test for rdpy3.protocol.rdp.nla.cssp and ntlm module
 """
 import unittest
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 from rdpy3.protocol.rdp.nla import cssp, ntlm
```

### Comparing `rdpy3-1.3.6/test/test_protocol_rdp_lic.py` & `rdpy3-1.3.7/test/test_protocol_rdp_lic.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.protocol.rdp.lic automata
+unit test for rdpy3.protocol.rdp.lic automata
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
```

### Comparing `rdpy3-1.3.6/test/test_protocol_rdp_mcs.py` & `rdpy3-1.3.7/test/test_protocol_rdp_mcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.protocol.rdp.mcs automata
+unit test for rdpy3.protocol.rdp.mcs automata
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
```

### Comparing `rdpy3-1.3.6/test/test_protocol_rdp_per.py` & `rdpy3-1.3.7/test/test_protocol_rdp_per.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.protocol.rdp.per module
+unit test for rdpy3.protocol.rdp.per module
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
```

### Comparing `rdpy3-1.3.6/test/test_protocol_rdp_rc4.py` & `rdpy3-1.3.7/test/test_protocol_rdp_rc4.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.protocol.rdp.rc4 module
+unit test for rdpy3.protocol.rdp.rc4 module
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
```

### Comparing `rdpy3-1.3.6/test/test_protocol_rdp_tpkt.py` & `rdpy3-1.3.7/test/test_protocol_rdp_tpkt.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.protocol.rdp.tpkt module
+unit test for rdpy3.protocol.rdp.tpkt module
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
```

### Comparing `rdpy3-1.3.6/test/test_protocol_rdp_x224.py` & `rdpy3-1.3.7/test/test_protocol_rdp_x224.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.protocol.rdp.x224 module
+unit test for rdpy3.protocol.rdp.x224 module
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
```

### Comparing `rdpy3-1.3.6/test/test_protocol_rfb_rfb.py` & `rdpy3-1.3.7/test/test_protocol_rfb_rfb.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
-unit test for rdpy.protocol.rfb.rfb module
+unit test for rdpy3.protocol.rfb.rfb module
 """
 
 import os, sys
 # Change path so we find rdpy
 sys.path.insert(1, os.path.join(sys.path[0], '..'))
 
 import unittest
```

