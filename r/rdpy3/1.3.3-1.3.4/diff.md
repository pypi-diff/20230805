# Comparing `tmp/rdpy3-1.3.3.tar.gz` & `tmp/rdpy3-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdpy3-1.3.3.tar", last modified: Sat Aug  5 13:44:59 2023, max compression
+gzip compressed data, was "rdpy3-1.3.4.tar", last modified: Sat Aug  5 13:53:37 2023, max compression
```

## Comparing `rdpy3-1.3.3.tar` & `rdpy3-1.3.4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.110000 rdpy3-1.3.3/
--rwxr-xr-x   0 root         (0) root         (0)    35121 2023-08-05 10:09:26.000000 rdpy3-1.3.3/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)     9555 2023-08-05 13:44:59.110000 rdpy3-1.3.3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     9290 2023-08-05 13:16:36.000000 rdpy3-1.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.050000 rdpy3-1.3.3/bin/
--rwxr-xr-x   0 root         (0) root         (0)    10240 2023-08-05 13:04:36.000000 rdpy3-1.3.3/bin/rdpy3-rdpclient.py
--rwxr-xr-x   0 root         (0) root         (0)     7337 2023-08-05 12:56:32.000000 rdpy3-1.3.3/bin/rdpy3-rdphoneypot.py
--rwxr-xr-x   0 root         (0) root         (0)    11900 2023-08-05 12:56:32.000000 rdpy3-1.3.3/bin/rdpy3-rdpmitm.py
--rwxr-xr-x   0 root         (0) root         (0)     8074 2023-08-05 13:04:36.000000 rdpy3-1.3.3/bin/rdpy3-rdpscreenshot.py
--rwxr-xr-x   0 root         (0) root         (0)     4403 2023-08-05 13:04:36.000000 rdpy3-1.3.3/bin/rdpy3-rssplayer.py
--rwxr-xr-x   0 root         (0) root         (0)     3342 2023-08-05 13:04:36.000000 rdpy3-1.3.3/bin/rdpy3-vncclient.py
--rwxr-xr-x   0 root         (0) root         (0)     6161 2023-08-05 13:04:36.000000 rdpy3-1.3.3/bin/rdpy3-vncscreenshot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.050000 rdpy3-1.3.3/ext/
--rwxr-xr-x   0 root         (0) root         (0)    19035 2023-08-05 13:03:01.000000 rdpy3-1.3.3/ext/rle.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.050000 rdpy3-1.3.3/rdpy3/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.060000 rdpy3-1.3.3/rdpy3/core/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/core/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2505 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/core/const.py
--rwxr-xr-x   0 root         (0) root         (0)     3014 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/core/error.py
--rwxr-xr-x   0 root         (0) root         (0)     3507 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/core/filetimes.py
--rwxr-xr-x   0 root         (0) root         (0)     8950 2023-08-05 12:56:32.000000 rdpy3-1.3.3/rdpy3/core/layer.py
--rwxr-xr-x   0 root         (0) root         (0)     1976 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/core/log.py
--rwxr-xr-x   0 root         (0) root         (0)     9547 2023-08-05 12:56:32.000000 rdpy3-1.3.3/rdpy3/core/rss.py
--rwxr-xr-x   0 root         (0) root         (0)     1443 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/core/scancode.py
--rwxr-xr-x   0 root         (0) root         (0)    40003 2023-08-05 12:56:52.000000 rdpy3-1.3.3/rdpy3/core/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.060000 rdpy3-1.3.3/rdpy3/protocol/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.070000 rdpy3-1.3.3/rdpy3/protocol/rdp/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14313 2023-08-05 12:56:52.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/lic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.070000 rdpy3-1.3.3/rdpy3/protocol/rdp/nla/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/nla/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    13391 2023-08-05 12:56:32.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/nla/cssp.py
--rwxr-xr-x   0 root         (0) root         (0)    24730 2023-08-05 12:56:52.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/nla/ntlm.py
--rwxr-xr-x   0 root         (0) root         (0)     2808 2023-08-05 12:56:32.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/nla/sspi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.080000 rdpy3-1.3.3/rdpy3/protocol/rdp/pdu/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/pdu/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    19191 2023-08-05 12:56:52.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/pdu/caps.py
--rwxr-xr-x   0 root         (0) root         (0)    51908 2023-08-05 12:58:17.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/pdu/data.py
--rwxr-xr-x   0 root         (0) root         (0)    27792 2023-08-05 12:58:17.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/pdu/layer.py
--rwxr-xr-x   0 root         (0) root         (0)     4840 2023-08-05 12:56:32.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/pdu/order.py
--rwxr-xr-x   0 root         (0) root         (0)    28629 2023-08-05 12:58:17.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/rdp.py
--rwxr-xr-x   0 root         (0) root         (0)    27591 2023-08-05 12:58:17.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/sec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.080000 rdpy3-1.3.3/rdpy3/protocol/rdp/t125/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/t125/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7574 2023-08-05 12:56:32.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/t125/ber.py
--rwxr-xr-x   0 root         (0) root         (0)    23674 2023-08-05 12:58:17.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/t125/gcc.py
--rwxr-xr-x   0 root         (0) root         (0)    24771 2023-08-05 12:58:17.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/t125/mcs.py
--rwxr-xr-x   0 root         (0) root         (0)     7966 2023-08-05 12:56:32.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/t125/per.py
--rwxr-xr-x   0 root         (0) root         (0)     8063 2023-08-05 12:56:32.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/tpkt.py
--rwxr-xr-x   0 root         (0) root         (0)    13551 2023-08-05 12:56:32.000000 rdpy3-1.3.3/rdpy3/protocol/rdp/x224.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.090000 rdpy3-1.3.3/rdpy3/protocol/rfb/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/protocol/rfb/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    25997 2023-08-05 12:56:52.000000 rdpy3-1.3.3/rdpy3/protocol/rfb/rfb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.090000 rdpy3-1.3.3/rdpy3/security/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/security/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    32292 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/security/pyDes.py
--rwxr-xr-x   0 root         (0) root         (0)     1756 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/security/rc4.py
--rwxr-xr-x   0 root         (0) root         (0)     3155 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/security/rsa_wrapper.py
--rwxr-xr-x   0 root         (0) root         (0)     6529 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/security/x509.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.090000 rdpy3-1.3.3/rdpy3/ui/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.3/rdpy3/ui/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14892 2023-08-05 12:56:52.000000 rdpy3-1.3.3/rdpy3/ui/qt5.py
--rwxr-xr-x   0 root         (0) root         (0)     8382 2023-08-05 12:56:32.000000 rdpy3-1.3.3/rdpy3/ui/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.050000 rdpy3-1.3.3/rdpy3.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)     9555 2023-08-05 13:44:58.000000 rdpy3-1.3.3/rdpy3.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1777 2023-08-05 13:44:59.000000 rdpy3-1.3.3/rdpy3.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2023-08-05 13:44:58.000000 rdpy3-1.3.3/rdpy3.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-08-05 13:44:58.000000 rdpy3-1.3.3/rdpy3.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)       10 2023-08-05 13:44:58.000000 rdpy3-1.3.3/rdpy3.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-08-05 13:44:59.110000 rdpy3-1.3.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1456 2023-08-05 13:44:41.000000 rdpy3-1.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:44:59.110000 rdpy3-1.3.3/test/
--rwxr-xr-x   0 root         (0) root         (0)     1843 2023-08-05 12:56:52.000000 rdpy3-1.3.3/test/test_core_const.py
--rwxr-xr-x   0 root         (0) root         (0)     2636 2023-08-05 12:56:52.000000 rdpy3-1.3.3/test/test_core_layer.py
--rwxr-xr-x   0 root         (0) root         (0)    15634 2023-08-05 12:56:52.000000 rdpy3-1.3.3/test/test_core_type.py
--rwxr-xr-x   0 root         (0) root         (0)     2608 2023-08-05 12:56:52.000000 rdpy3-1.3.3/test/test_protocol_rdp_ber.py
--rwxr-xr-x   0 root         (0) root         (0)     5262 2023-08-05 12:56:32.000000 rdpy3-1.3.3/test/test_protocol_rdp_cssp_ntlm.py
--rwxr-xr-x   0 root         (0) root         (0)     5626 2023-08-05 12:56:52.000000 rdpy3-1.3.3/test/test_protocol_rdp_lic.py
--rwxr-xr-x   0 root         (0) root         (0)     1017 2023-08-05 10:09:26.000000 rdpy3-1.3.3/test/test_protocol_rdp_mcs.py
--rwxr-xr-x   0 root         (0) root         (0)     3604 2023-08-05 12:56:52.000000 rdpy3-1.3.3/test/test_protocol_rdp_per.py
--rwxr-xr-x   0 root         (0) root         (0)     1935 2023-08-05 12:56:52.000000 rdpy3-1.3.3/test/test_protocol_rdp_rc4.py
--rwxr-xr-x   0 root         (0) root         (0)     4098 2023-08-05 12:56:52.000000 rdpy3-1.3.3/test/test_protocol_rdp_tpkt.py
--rwxr-xr-x   0 root         (0) root         (0)     8087 2023-08-05 12:56:52.000000 rdpy3-1.3.3/test/test_protocol_rdp_x224.py
--rwxr-xr-x   0 root         (0) root         (0)      990 2023-08-05 10:09:26.000000 rdpy3-1.3.3/test/test_protocol_rfb_rfb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.210000 rdpy3-1.3.4/
+-rwxr-xr-x   0 root         (0) root         (0)    35121 2023-08-05 10:09:26.000000 rdpy3-1.3.4/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)     9577 2023-08-05 13:53:37.210000 rdpy3-1.3.4/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     9290 2023-08-05 13:16:36.000000 rdpy3-1.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.150000 rdpy3-1.3.4/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    10240 2023-08-05 13:04:36.000000 rdpy3-1.3.4/bin/rdpy3-rdpclient.py
+-rwxr-xr-x   0 root         (0) root         (0)     7337 2023-08-05 12:56:32.000000 rdpy3-1.3.4/bin/rdpy3-rdphoneypot.py
+-rwxr-xr-x   0 root         (0) root         (0)    11900 2023-08-05 12:56:32.000000 rdpy3-1.3.4/bin/rdpy3-rdpmitm.py
+-rwxr-xr-x   0 root         (0) root         (0)     8074 2023-08-05 13:04:36.000000 rdpy3-1.3.4/bin/rdpy3-rdpscreenshot.py
+-rwxr-xr-x   0 root         (0) root         (0)     4403 2023-08-05 13:04:36.000000 rdpy3-1.3.4/bin/rdpy3-rssplayer.py
+-rwxr-xr-x   0 root         (0) root         (0)     3342 2023-08-05 13:04:36.000000 rdpy3-1.3.4/bin/rdpy3-vncclient.py
+-rwxr-xr-x   0 root         (0) root         (0)     6161 2023-08-05 13:04:36.000000 rdpy3-1.3.4/bin/rdpy3-vncscreenshot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.150000 rdpy3-1.3.4/ext/
+-rwxr-xr-x   0 root         (0) root         (0)    19035 2023-08-05 13:03:01.000000 rdpy3-1.3.4/ext/rle.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.150000 rdpy3-1.3.4/rdpy3/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.160000 rdpy3-1.3.4/rdpy3/core/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2505 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/const.py
+-rwxr-xr-x   0 root         (0) root         (0)     3014 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/error.py
+-rwxr-xr-x   0 root         (0) root         (0)     3507 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/filetimes.py
+-rwxr-xr-x   0 root         (0) root         (0)     8950 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/core/layer.py
+-rwxr-xr-x   0 root         (0) root         (0)     1976 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/log.py
+-rwxr-xr-x   0 root         (0) root         (0)     9547 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/core/rss.py
+-rwxr-xr-x   0 root         (0) root         (0)     1443 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/scancode.py
+-rwxr-xr-x   0 root         (0) root         (0)    40003 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/core/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.160000 rdpy3-1.3.4/rdpy3/protocol/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.170000 rdpy3-1.3.4/rdpy3/protocol/rdp/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14313 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/lic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.170000 rdpy3-1.3.4/rdpy3/protocol/rdp/nla/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/nla/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    13391 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/nla/cssp.py
+-rwxr-xr-x   0 root         (0) root         (0)    24730 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/nla/ntlm.py
+-rwxr-xr-x   0 root         (0) root         (0)     2808 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/nla/sspi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.180000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    19191 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/caps.py
+-rwxr-xr-x   0 root         (0) root         (0)    51908 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/data.py
+-rwxr-xr-x   0 root         (0) root         (0)    27792 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/layer.py
+-rwxr-xr-x   0 root         (0) root         (0)     4840 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/order.py
+-rwxr-xr-x   0 root         (0) root         (0)    28629 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/rdp.py
+-rwxr-xr-x   0 root         (0) root         (0)    27591 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/sec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.190000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7574 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/ber.py
+-rwxr-xr-x   0 root         (0) root         (0)    23674 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/gcc.py
+-rwxr-xr-x   0 root         (0) root         (0)    24771 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/mcs.py
+-rwxr-xr-x   0 root         (0) root         (0)     7966 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/per.py
+-rwxr-xr-x   0 root         (0) root         (0)     8063 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/tpkt.py
+-rwxr-xr-x   0 root         (0) root         (0)    13551 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/x224.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.190000 rdpy3-1.3.4/rdpy3/protocol/rfb/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/rfb/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    25997 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/protocol/rfb/rfb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.200000 rdpy3-1.3.4/rdpy3/security/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/security/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    32292 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/security/pyDes.py
+-rwxr-xr-x   0 root         (0) root         (0)     1756 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/security/rc4.py
+-rwxr-xr-x   0 root         (0) root         (0)     3155 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/security/rsa_wrapper.py
+-rwxr-xr-x   0 root         (0) root         (0)     6529 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/security/x509.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.200000 rdpy3-1.3.4/rdpy3/ui/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/ui/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14892 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/ui/qt5.py
+-rwxr-xr-x   0 root         (0) root         (0)     8382 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/ui/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.150000 rdpy3-1.3.4/rdpy3.egg-info/
+-rwxr-xr-x   0 root         (0) root         (0)     9577 2023-08-05 13:53:37.000000 rdpy3-1.3.4/rdpy3.egg-info/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     1777 2023-08-05 13:53:37.000000 rdpy3-1.3.4/rdpy3.egg-info/SOURCES.txt
+-rwxr-xr-x   0 root         (0) root         (0)        1 2023-08-05 13:53:37.000000 rdpy3-1.3.4/rdpy3.egg-info/dependency_links.txt
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-08-05 13:53:37.000000 rdpy3-1.3.4/rdpy3.egg-info/requires.txt
+-rwxr-xr-x   0 root         (0) root         (0)       10 2023-08-05 13:53:37.000000 rdpy3-1.3.4/rdpy3.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)       38 2023-08-05 13:53:37.220000 rdpy3-1.3.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1682 2023-08-05 13:51:08.000000 rdpy3-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.210000 rdpy3-1.3.4/test/
+-rwxr-xr-x   0 root         (0) root         (0)     1843 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_core_const.py
+-rwxr-xr-x   0 root         (0) root         (0)     2636 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_core_layer.py
+-rwxr-xr-x   0 root         (0) root         (0)    15634 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_core_type.py
+-rwxr-xr-x   0 root         (0) root         (0)     2608 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_ber.py
+-rwxr-xr-x   0 root         (0) root         (0)     5262 2023-08-05 12:56:32.000000 rdpy3-1.3.4/test/test_protocol_rdp_cssp_ntlm.py
+-rwxr-xr-x   0 root         (0) root         (0)     5626 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_lic.py
+-rwxr-xr-x   0 root         (0) root         (0)     1017 2023-08-05 10:09:26.000000 rdpy3-1.3.4/test/test_protocol_rdp_mcs.py
+-rwxr-xr-x   0 root         (0) root         (0)     3604 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_per.py
+-rwxr-xr-x   0 root         (0) root         (0)     1935 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_rc4.py
+-rwxr-xr-x   0 root         (0) root         (0)     4098 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_tpkt.py
+-rwxr-xr-x   0 root         (0) root         (0)     8087 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_x224.py
+-rwxr-xr-x   0 root         (0) root         (0)      990 2023-08-05 10:09:26.000000 rdpy3-1.3.4/test/test_protocol_rfb_rfb.py
```

### Comparing `rdpy3-1.3.3/LICENSE` & `rdpy3-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/PKG-INFO` & `rdpy3-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: rdpy3
-Version: 1.3.3
-Summary: Remote Desktop Protocol in Python
+Version: 1.3.4
+Summary: Remote Desktop Protocol in Python3
 Home-page: https://github.com/james4ever0/rdpy3
 Author: Sylvain Peyrefitte
 Author-email: citronneur@gmail.com
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RDPY - for Python3 
 
 **this is a fork for porting RDPY to Python3**
```

### Comparing `rdpy3-1.3.3/README.md` & `rdpy3-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/bin/rdpy3-rdpclient.py` & `rdpy3-1.3.4/bin/rdpy3-rdpclient.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/bin/rdpy3-rdphoneypot.py` & `rdpy3-1.3.4/bin/rdpy3-rdphoneypot.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/bin/rdpy3-rdpmitm.py` & `rdpy3-1.3.4/bin/rdpy3-rdpmitm.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/bin/rdpy3-rdpscreenshot.py` & `rdpy3-1.3.4/bin/rdpy3-rdpscreenshot.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/bin/rdpy3-rssplayer.py` & `rdpy3-1.3.4/bin/rdpy3-rssplayer.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/bin/rdpy3-vncclient.py` & `rdpy3-1.3.4/bin/rdpy3-vncclient.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/bin/rdpy3-vncscreenshot.py` & `rdpy3-1.3.4/bin/rdpy3-vncscreenshot.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/ext/rle.c` & `rdpy3-1.3.4/ext/rle.c`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/core/const.py` & `rdpy3-1.3.4/rdpy3/core/const.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/core/error.py` & `rdpy3-1.3.4/rdpy3/core/error.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/core/filetimes.py` & `rdpy3-1.3.4/rdpy3/core/filetimes.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/core/layer.py` & `rdpy3-1.3.4/rdpy3/core/layer.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/core/log.py` & `rdpy3-1.3.4/rdpy3/core/log.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/core/rss.py` & `rdpy3-1.3.4/rdpy3/core/rss.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/core/scancode.py` & `rdpy3-1.3.4/rdpy3/core/scancode.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/core/type.py` & `rdpy3-1.3.4/rdpy3/core/type.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/lic.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/lic.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/nla/cssp.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/nla/cssp.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/nla/ntlm.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/nla/ntlm.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/nla/sspi.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/nla/sspi.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/pdu/caps.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/caps.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/pdu/data.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/data.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/pdu/layer.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/layer.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/pdu/order.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/order.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/rdp.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/rdp.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/sec.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/sec.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/t125/ber.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/t125/ber.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/t125/gcc.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/t125/gcc.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/t125/mcs.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/t125/mcs.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/t125/per.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/t125/per.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/tpkt.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/tpkt.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rdp/x224.py` & `rdpy3-1.3.4/rdpy3/protocol/rdp/x224.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/protocol/rfb/rfb.py` & `rdpy3-1.3.4/rdpy3/protocol/rfb/rfb.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/security/pyDes.py` & `rdpy3-1.3.4/rdpy3/security/pyDes.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/security/rc4.py` & `rdpy3-1.3.4/rdpy3/security/rc4.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/security/rsa_wrapper.py` & `rdpy3-1.3.4/rdpy3/security/rsa_wrapper.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/security/x509.py` & `rdpy3-1.3.4/rdpy3/security/x509.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/ui/qt5.py` & `rdpy3-1.3.4/rdpy3/ui/qt5.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3/ui/view.py` & `rdpy3-1.3.4/rdpy3/ui/view.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/rdpy3.egg-info/PKG-INFO` & `rdpy3-1.3.4/rdpy3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: rdpy3
-Version: 1.3.3
-Summary: Remote Desktop Protocol in Python
+Version: 1.3.4
+Summary: Remote Desktop Protocol in Python3
 Home-page: https://github.com/james4ever0/rdpy3
 Author: Sylvain Peyrefitte
 Author-email: citronneur@gmail.com
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RDPY - for Python3 
 
 **this is a fork for porting RDPY to Python3**
```

### Comparing `rdpy3-1.3.3/rdpy3.egg-info/SOURCES.txt` & `rdpy3-1.3.4/rdpy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_core_const.py` & `rdpy3-1.3.4/test/test_core_const.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_core_layer.py` & `rdpy3-1.3.4/test/test_core_layer.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_core_type.py` & `rdpy3-1.3.4/test/test_core_type.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_protocol_rdp_ber.py` & `rdpy3-1.3.4/test/test_protocol_rdp_ber.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_protocol_rdp_cssp_ntlm.py` & `rdpy3-1.3.4/test/test_protocol_rdp_cssp_ntlm.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_protocol_rdp_lic.py` & `rdpy3-1.3.4/test/test_protocol_rdp_lic.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_protocol_rdp_mcs.py` & `rdpy3-1.3.4/test/test_protocol_rdp_mcs.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_protocol_rdp_per.py` & `rdpy3-1.3.4/test/test_protocol_rdp_per.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_protocol_rdp_rc4.py` & `rdpy3-1.3.4/test/test_protocol_rdp_rc4.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_protocol_rdp_tpkt.py` & `rdpy3-1.3.4/test/test_protocol_rdp_tpkt.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_protocol_rdp_x224.py` & `rdpy3-1.3.4/test/test_protocol_rdp_x224.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.3/test/test_protocol_rfb_rfb.py` & `rdpy3-1.3.4/test/test_protocol_rfb_rfb.py`

 * *Files identical despite different names*

