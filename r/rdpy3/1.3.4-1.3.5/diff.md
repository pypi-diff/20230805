# Comparing `tmp/rdpy3-1.3.4.tar.gz` & `tmp/rdpy3-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdpy3-1.3.4.tar", last modified: Sat Aug  5 13:53:37 2023, max compression
+gzip compressed data, was "rdpy3-1.3.5.tar", last modified: Sat Aug  5 14:03:38 2023, max compression
```

## Comparing `rdpy3-1.3.4.tar` & `rdpy3-1.3.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.210000 rdpy3-1.3.4/
--rwxr-xr-x   0 root         (0) root         (0)    35121 2023-08-05 10:09:26.000000 rdpy3-1.3.4/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)     9577 2023-08-05 13:53:37.210000 rdpy3-1.3.4/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     9290 2023-08-05 13:16:36.000000 rdpy3-1.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.150000 rdpy3-1.3.4/bin/
--rwxr-xr-x   0 root         (0) root         (0)    10240 2023-08-05 13:04:36.000000 rdpy3-1.3.4/bin/rdpy3-rdpclient.py
--rwxr-xr-x   0 root         (0) root         (0)     7337 2023-08-05 12:56:32.000000 rdpy3-1.3.4/bin/rdpy3-rdphoneypot.py
--rwxr-xr-x   0 root         (0) root         (0)    11900 2023-08-05 12:56:32.000000 rdpy3-1.3.4/bin/rdpy3-rdpmitm.py
--rwxr-xr-x   0 root         (0) root         (0)     8074 2023-08-05 13:04:36.000000 rdpy3-1.3.4/bin/rdpy3-rdpscreenshot.py
--rwxr-xr-x   0 root         (0) root         (0)     4403 2023-08-05 13:04:36.000000 rdpy3-1.3.4/bin/rdpy3-rssplayer.py
--rwxr-xr-x   0 root         (0) root         (0)     3342 2023-08-05 13:04:36.000000 rdpy3-1.3.4/bin/rdpy3-vncclient.py
--rwxr-xr-x   0 root         (0) root         (0)     6161 2023-08-05 13:04:36.000000 rdpy3-1.3.4/bin/rdpy3-vncscreenshot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.150000 rdpy3-1.3.4/ext/
--rwxr-xr-x   0 root         (0) root         (0)    19035 2023-08-05 13:03:01.000000 rdpy3-1.3.4/ext/rle.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.150000 rdpy3-1.3.4/rdpy3/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.160000 rdpy3-1.3.4/rdpy3/core/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2505 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/const.py
--rwxr-xr-x   0 root         (0) root         (0)     3014 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/error.py
--rwxr-xr-x   0 root         (0) root         (0)     3507 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/filetimes.py
--rwxr-xr-x   0 root         (0) root         (0)     8950 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/core/layer.py
--rwxr-xr-x   0 root         (0) root         (0)     1976 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/log.py
--rwxr-xr-x   0 root         (0) root         (0)     9547 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/core/rss.py
--rwxr-xr-x   0 root         (0) root         (0)     1443 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/core/scancode.py
--rwxr-xr-x   0 root         (0) root         (0)    40003 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/core/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.160000 rdpy3-1.3.4/rdpy3/protocol/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.170000 rdpy3-1.3.4/rdpy3/protocol/rdp/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14313 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/lic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.170000 rdpy3-1.3.4/rdpy3/protocol/rdp/nla/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/nla/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    13391 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/nla/cssp.py
--rwxr-xr-x   0 root         (0) root         (0)    24730 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/nla/ntlm.py
--rwxr-xr-x   0 root         (0) root         (0)     2808 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/nla/sspi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.180000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    19191 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/caps.py
--rwxr-xr-x   0 root         (0) root         (0)    51908 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/data.py
--rwxr-xr-x   0 root         (0) root         (0)    27792 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/layer.py
--rwxr-xr-x   0 root         (0) root         (0)     4840 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/order.py
--rwxr-xr-x   0 root         (0) root         (0)    28629 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/rdp.py
--rwxr-xr-x   0 root         (0) root         (0)    27591 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/sec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.190000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7574 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/ber.py
--rwxr-xr-x   0 root         (0) root         (0)    23674 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/gcc.py
--rwxr-xr-x   0 root         (0) root         (0)    24771 2023-08-05 12:58:17.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/mcs.py
--rwxr-xr-x   0 root         (0) root         (0)     7966 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/t125/per.py
--rwxr-xr-x   0 root         (0) root         (0)     8063 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/tpkt.py
--rwxr-xr-x   0 root         (0) root         (0)    13551 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/protocol/rdp/x224.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.190000 rdpy3-1.3.4/rdpy3/protocol/rfb/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/protocol/rfb/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    25997 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/protocol/rfb/rfb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.200000 rdpy3-1.3.4/rdpy3/security/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/security/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    32292 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/security/pyDes.py
--rwxr-xr-x   0 root         (0) root         (0)     1756 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/security/rc4.py
--rwxr-xr-x   0 root         (0) root         (0)     3155 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/security/rsa_wrapper.py
--rwxr-xr-x   0 root         (0) root         (0)     6529 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/security/x509.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.200000 rdpy3-1.3.4/rdpy3/ui/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.4/rdpy3/ui/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    14892 2023-08-05 12:56:52.000000 rdpy3-1.3.4/rdpy3/ui/qt5.py
--rwxr-xr-x   0 root         (0) root         (0)     8382 2023-08-05 12:56:32.000000 rdpy3-1.3.4/rdpy3/ui/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.150000 rdpy3-1.3.4/rdpy3.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)     9577 2023-08-05 13:53:37.000000 rdpy3-1.3.4/rdpy3.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     1777 2023-08-05 13:53:37.000000 rdpy3-1.3.4/rdpy3.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)        1 2023-08-05 13:53:37.000000 rdpy3-1.3.4/rdpy3.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)       57 2023-08-05 13:53:37.000000 rdpy3-1.3.4/rdpy3.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)       10 2023-08-05 13:53:37.000000 rdpy3-1.3.4/rdpy3.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-08-05 13:53:37.220000 rdpy3-1.3.4/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1682 2023-08-05 13:51:08.000000 rdpy3-1.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 13:53:37.210000 rdpy3-1.3.4/test/
--rwxr-xr-x   0 root         (0) root         (0)     1843 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_core_const.py
--rwxr-xr-x   0 root         (0) root         (0)     2636 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_core_layer.py
--rwxr-xr-x   0 root         (0) root         (0)    15634 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_core_type.py
--rwxr-xr-x   0 root         (0) root         (0)     2608 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_ber.py
--rwxr-xr-x   0 root         (0) root         (0)     5262 2023-08-05 12:56:32.000000 rdpy3-1.3.4/test/test_protocol_rdp_cssp_ntlm.py
--rwxr-xr-x   0 root         (0) root         (0)     5626 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_lic.py
--rwxr-xr-x   0 root         (0) root         (0)     1017 2023-08-05 10:09:26.000000 rdpy3-1.3.4/test/test_protocol_rdp_mcs.py
--rwxr-xr-x   0 root         (0) root         (0)     3604 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_per.py
--rwxr-xr-x   0 root         (0) root         (0)     1935 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_rc4.py
--rwxr-xr-x   0 root         (0) root         (0)     4098 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_tpkt.py
--rwxr-xr-x   0 root         (0) root         (0)     8087 2023-08-05 12:56:52.000000 rdpy3-1.3.4/test/test_protocol_rdp_x224.py
--rwxr-xr-x   0 root         (0) root         (0)      990 2023-08-05 10:09:26.000000 rdpy3-1.3.4/test/test_protocol_rfb_rfb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.230000 rdpy3-1.3.5/
+-rwxr-xr-x   0 root         (0) root         (0)    35121 2023-08-05 10:09:26.000000 rdpy3-1.3.5/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)     9577 2023-08-05 14:03:38.230000 rdpy3-1.3.5/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     9290 2023-08-05 13:16:36.000000 rdpy3-1.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.090000 rdpy3-1.3.5/bin/
+-rwxr-xr-x   0 root         (0) root         (0)    10242 2023-08-05 14:02:32.000000 rdpy3-1.3.5/bin/rdpy3-rdpclient.py
+-rwxr-xr-x   0 root         (0) root         (0)     7338 2023-08-05 14:02:32.000000 rdpy3-1.3.5/bin/rdpy3-rdphoneypot.py
+-rwxr-xr-x   0 root         (0) root         (0)    11901 2023-08-05 14:02:32.000000 rdpy3-1.3.5/bin/rdpy3-rdpmitm.py
+-rwxr-xr-x   0 root         (0) root         (0)     8076 2023-08-05 14:02:32.000000 rdpy3-1.3.5/bin/rdpy3-rdpscreenshot.py
+-rwxr-xr-x   0 root         (0) root         (0)     4404 2023-08-05 14:02:32.000000 rdpy3-1.3.5/bin/rdpy3-rssplayer.py
+-rwxr-xr-x   0 root         (0) root         (0)     3343 2023-08-05 14:02:32.000000 rdpy3-1.3.5/bin/rdpy3-vncclient.py
+-rwxr-xr-x   0 root         (0) root         (0)     6163 2023-08-05 14:02:32.000000 rdpy3-1.3.5/bin/rdpy3-vncscreenshot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.090000 rdpy3-1.3.5/ext/
+-rwxr-xr-x   0 root         (0) root         (0)    19035 2023-08-05 13:03:01.000000 rdpy3-1.3.5/ext/rle.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.090000 rdpy3-1.3.5/rdpy3/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.120000 rdpy3-1.3.5/rdpy3/core/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/core/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2505 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/core/const.py
+-rwxr-xr-x   0 root         (0) root         (0)     3014 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/core/error.py
+-rwxr-xr-x   0 root         (0) root         (0)     3507 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/core/filetimes.py
+-rwxr-xr-x   0 root         (0) root         (0)     8950 2023-08-05 12:56:32.000000 rdpy3-1.3.5/rdpy3/core/layer.py
+-rwxr-xr-x   0 root         (0) root         (0)     1976 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/core/log.py
+-rwxr-xr-x   0 root         (0) root         (0)     9547 2023-08-05 12:56:32.000000 rdpy3-1.3.5/rdpy3/core/rss.py
+-rwxr-xr-x   0 root         (0) root         (0)     1443 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/core/scancode.py
+-rwxr-xr-x   0 root         (0) root         (0)    40003 2023-08-05 12:56:52.000000 rdpy3-1.3.5/rdpy3/core/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.120000 rdpy3-1.3.5/rdpy3/protocol/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.130000 rdpy3-1.3.5/rdpy3/protocol/rdp/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14313 2023-08-05 12:56:52.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/lic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.140000 rdpy3-1.3.5/rdpy3/protocol/rdp/nla/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/nla/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    13391 2023-08-05 12:56:32.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/nla/cssp.py
+-rwxr-xr-x   0 root         (0) root         (0)    24730 2023-08-05 12:56:52.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/nla/ntlm.py
+-rwxr-xr-x   0 root         (0) root         (0)     2808 2023-08-05 12:56:32.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/nla/sspi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.160000 rdpy3-1.3.5/rdpy3/protocol/rdp/pdu/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/pdu/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    19191 2023-08-05 12:56:52.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/pdu/caps.py
+-rwxr-xr-x   0 root         (0) root         (0)    51908 2023-08-05 12:58:17.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/pdu/data.py
+-rwxr-xr-x   0 root         (0) root         (0)    27792 2023-08-05 12:58:17.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/pdu/layer.py
+-rwxr-xr-x   0 root         (0) root         (0)     4840 2023-08-05 12:56:32.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/pdu/order.py
+-rwxr-xr-x   0 root         (0) root         (0)    28629 2023-08-05 12:58:17.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/rdp.py
+-rwxr-xr-x   0 root         (0) root         (0)    27591 2023-08-05 12:58:17.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/sec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.170000 rdpy3-1.3.5/rdpy3/protocol/rdp/t125/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/t125/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7574 2023-08-05 12:56:32.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/t125/ber.py
+-rwxr-xr-x   0 root         (0) root         (0)    23674 2023-08-05 12:58:17.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/t125/gcc.py
+-rwxr-xr-x   0 root         (0) root         (0)    24771 2023-08-05 12:58:17.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/t125/mcs.py
+-rwxr-xr-x   0 root         (0) root         (0)     7966 2023-08-05 12:56:32.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/t125/per.py
+-rwxr-xr-x   0 root         (0) root         (0)     8063 2023-08-05 12:56:32.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/tpkt.py
+-rwxr-xr-x   0 root         (0) root         (0)    13551 2023-08-05 12:56:32.000000 rdpy3-1.3.5/rdpy3/protocol/rdp/x224.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.180000 rdpy3-1.3.5/rdpy3/protocol/rfb/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/protocol/rfb/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    25997 2023-08-05 12:56:52.000000 rdpy3-1.3.5/rdpy3/protocol/rfb/rfb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.190000 rdpy3-1.3.5/rdpy3/security/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/security/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    32292 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/security/pyDes.py
+-rwxr-xr-x   0 root         (0) root         (0)     1756 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/security/rc4.py
+-rwxr-xr-x   0 root         (0) root         (0)     3155 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/security/rsa_wrapper.py
+-rwxr-xr-x   0 root         (0) root         (0)     6529 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/security/x509.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.200000 rdpy3-1.3.5/rdpy3/ui/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 10:09:26.000000 rdpy3-1.3.5/rdpy3/ui/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    14892 2023-08-05 12:56:52.000000 rdpy3-1.3.5/rdpy3/ui/qt5.py
+-rwxr-xr-x   0 root         (0) root         (0)     8382 2023-08-05 12:56:32.000000 rdpy3-1.3.5/rdpy3/ui/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.110000 rdpy3-1.3.5/rdpy3.egg-info/
+-rwxr-xr-x   0 root         (0) root         (0)     9577 2023-08-05 14:03:37.000000 rdpy3-1.3.5/rdpy3.egg-info/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     1777 2023-08-05 14:03:37.000000 rdpy3-1.3.5/rdpy3.egg-info/SOURCES.txt
+-rwxr-xr-x   0 root         (0) root         (0)        1 2023-08-05 14:03:37.000000 rdpy3-1.3.5/rdpy3.egg-info/dependency_links.txt
+-rwxr-xr-x   0 root         (0) root         (0)       57 2023-08-05 14:03:37.000000 rdpy3-1.3.5/rdpy3.egg-info/requires.txt
+-rwxr-xr-x   0 root         (0) root         (0)       10 2023-08-05 14:03:37.000000 rdpy3-1.3.5/rdpy3.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)       38 2023-08-05 14:03:38.230000 rdpy3-1.3.5/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1685 2023-08-05 14:03:17.000000 rdpy3-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 14:03:38.230000 rdpy3-1.3.5/test/
+-rwxr-xr-x   0 root         (0) root         (0)     1843 2023-08-05 12:56:52.000000 rdpy3-1.3.5/test/test_core_const.py
+-rwxr-xr-x   0 root         (0) root         (0)     2636 2023-08-05 12:56:52.000000 rdpy3-1.3.5/test/test_core_layer.py
+-rwxr-xr-x   0 root         (0) root         (0)    15634 2023-08-05 12:56:52.000000 rdpy3-1.3.5/test/test_core_type.py
+-rwxr-xr-x   0 root         (0) root         (0)     2608 2023-08-05 12:56:52.000000 rdpy3-1.3.5/test/test_protocol_rdp_ber.py
+-rwxr-xr-x   0 root         (0) root         (0)     5262 2023-08-05 12:56:32.000000 rdpy3-1.3.5/test/test_protocol_rdp_cssp_ntlm.py
+-rwxr-xr-x   0 root         (0) root         (0)     5626 2023-08-05 12:56:52.000000 rdpy3-1.3.5/test/test_protocol_rdp_lic.py
+-rwxr-xr-x   0 root         (0) root         (0)     1017 2023-08-05 10:09:26.000000 rdpy3-1.3.5/test/test_protocol_rdp_mcs.py
+-rwxr-xr-x   0 root         (0) root         (0)     3604 2023-08-05 12:56:52.000000 rdpy3-1.3.5/test/test_protocol_rdp_per.py
+-rwxr-xr-x   0 root         (0) root         (0)     1935 2023-08-05 12:56:52.000000 rdpy3-1.3.5/test/test_protocol_rdp_rc4.py
+-rwxr-xr-x   0 root         (0) root         (0)     4098 2023-08-05 12:56:52.000000 rdpy3-1.3.5/test/test_protocol_rdp_tpkt.py
+-rwxr-xr-x   0 root         (0) root         (0)     8087 2023-08-05 12:56:52.000000 rdpy3-1.3.5/test/test_protocol_rdp_x224.py
+-rwxr-xr-x   0 root         (0) root         (0)      990 2023-08-05 10:09:26.000000 rdpy3-1.3.5/test/test_protocol_rfb_rfb.py
```

### Comparing `rdpy3-1.3.4/LICENSE` & `rdpy3-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/PKG-INFO` & `rdpy3-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdpy3
-Version: 1.3.4
+Version: 1.3.5
 Summary: Remote Desktop Protocol in Python3
 Home-page: https://github.com/james4ever0/rdpy3
 Author: Sylvain Peyrefitte
 Author-email: citronneur@gmail.com
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rdpy3-1.3.4/README.md` & `rdpy3-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/bin/rdpy3-rdpclient.py` & `rdpy3-1.3.5/bin/rdpy3-rdpclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         #create client observer
         if self._recodedPath is None:
             self._client = RDPClientQt(controller, self._width, self._height)
         else:
             self._client = RDPClientQtRecorder(controller, self._width, self._height, rss.createRecorder(self._recodedPath))
         #create qt widget
         self._w = self._client.getWidget()
-        self._w.setWindowTitle('rdpy-rdpclient')
+        self._w.setWindowTitle('rdpy3-rdpclient')
         if self._fullscreen:
             self._w.showFullScreen()
         else:
             self._w.show()
         
         controller.setUsername(self._username)
         controller.setPassword(self._passwod)
@@ -208,15 +208,15 @@
     except Exception as e:
         log.info("failed to auto detect keyboard layout " + str(e))
         pass
     return "en"
         
 def help():
     print ("""
-    Usage: rdpy-rdpclient [options] ip[:port]"
+    Usage: rdpy3-rdpclient [options] ip[:port]"
     \t-u: user name
     \t-p: password
     \t-d: domain
     \t-w: width of screen [default : 1024]
     \t-l: height of screen [default : 800]
     \t-f: enable full screen mode [default : False]
     \t-k: keyboard layout [en|fr] [default : en]
```

### Comparing `rdpy3-1.3.4/bin/rdpy3-rdphoneypot.py` & `rdpy3-1.3.5/bin/rdpy3-rdphoneypot.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             return e.event.width.value, e.event.height.value
     
 def help():
     """
     @summary: Print help in console
     """
     print("""
-    Usage:  rdpy-rdphoneypot.py 
+    Usage:  rdpy3-rdphoneypot.py 
             [-L logfile]
             [-l listen_port default 3389] 
             [-k private_key_file_path (mandatory for SSL)] 
             [-c certificate_file_path (mandatory for SSL)] 
             rss_filepath(1..n)
     """)
```

### Comparing `rdpy3-1.3.4/bin/rdpy3-rdpmitm.py` & `rdpy3-1.3.5/bin/rdpy3-rdpmitm.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
 """
 RDP proxy with Man in the middle capabilities
 Save RDP events in output RSR file format
-RSR file format can be read by rdpy-rsrplayer.py
+RSR file format can be read by rdpy3-rsrplayer.py
                ----------------------------
 Client RDP -> | ProxyServer | ProxyClient | -> Server RDP
               ----------------------------
                    | Record Session |
                    -----------------
 """
```

### Comparing `rdpy3-1.3.4/bin/rdpy3-rdpscreenshot.py` & `rdpy3-1.3.5/bin/rdpy3-rdpscreenshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,18 +188,18 @@
 
     reactor.runReturn()
     app.exec_()
     return RDPScreenShotFactory.__STATE__
 
 
 def help():
-    print("Usage: rdpy-rdpscreenshot [options] ip[:port]")
+    print("Usage: rdpy3-rdpscreenshot [options] ip[:port]")
     print("\t-w: width of screen default value is 1024")
     print("\t-l: height of screen default value is 800")
-    print("\t-o: file path of screenshot default(/tmp/rdpy-rdpscreenshot.jpg)")
+    print("\t-o: file path of screenshot default(/tmp/rdpy3-rdpscreenshot.jpg)")
     print("\t-t: timeout of connection without any updating order (default is 2s)")
 
 if __name__ == '__main__':
     # default script argument
     width = 1024
     height = 800
     path = "/tmp/"
```

### Comparing `rdpy3-1.3.4/bin/rdpy3-rssplayer.py` & `rdpy3-1.3.5/bin/rdpy3-rssplayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         layout.addWidget(self._text, 2)
         
         self.setLayout(layout)
         
         self.setGeometry(0, 0, 800, 600)
 
 def help():
-    print "Usage: rdpy-rssplayer [-h] rss_filepath"
+    print "Usage: rdpy3-rssplayer [-h] rss_filepath"
 
 def start(widget, rssFile):
     loop(widget, rssFile, rssFile.nextEvent())
   
 def loop(widget, rssFile, nextEvent):
     """
     @summary: timer function
```

### Comparing `rdpy3-1.3.4/bin/rdpy3-vncclient.py` & `rdpy3-1.3.5/bin/rdpy3-vncclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         """
         #set password
         controller.setPassword(self._password)
         #create client observer
         client = RFBClientQt(controller)
         #create qt widget
         self._w = client.getWidget()
-        self._w.setWindowTitle('rdpy-vncclient')
+        self._w.setWindowTitle('rdpy3-vncclient')
         self._w.show()
         return client
         
     def clientConnectionLost(self, connector, reason):
         """
         @summary: Connection lost event
         @param connector: twisted connector use for vnc connection (use reconnect to restart connection)
```

### Comparing `rdpy3-1.3.4/bin/rdpy3-vncscreenshot.py` & `rdpy3-1.3.5/bin/rdpy3-vncscreenshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,16 @@
                 log.info("save screenshot into %s"%self._path)
                 self._buffer.save(self._path)
         
         controller.setPassword(self._password)
         return ScreenShotObserver(controller, self._path)
         
 def help():
-    print("Usage: rdpy-vncscreenshot [options] ip[:port]")
-    print("\t-o: file path of screenshot default(/tmp/rdpy-vncscreenshot.jpg)")
+    print("Usage: rdpy3-vncscreenshot [options] ip[:port]")
+    print("\t-o: file path of screenshot default(/tmp/rdpy3-vncscreenshot.jpg)")
     print("\t-p: password for VNC Session")
         
 if __name__ == '__main__':
     #default script argument
     path = "/tmp/"
     password = ""
```

### Comparing `rdpy3-1.3.4/ext/rle.c` & `rdpy3-1.3.5/ext/rle.c`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/core/const.py` & `rdpy3-1.3.5/rdpy3/core/const.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/core/error.py` & `rdpy3-1.3.5/rdpy3/core/error.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/core/filetimes.py` & `rdpy3-1.3.5/rdpy3/core/filetimes.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/core/layer.py` & `rdpy3-1.3.5/rdpy3/core/layer.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/core/log.py` & `rdpy3-1.3.5/rdpy3/core/log.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/core/rss.py` & `rdpy3-1.3.5/rdpy3/core/rss.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/core/scancode.py` & `rdpy3-1.3.5/rdpy3/core/scancode.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/core/type.py` & `rdpy3-1.3.5/rdpy3/core/type.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/lic.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/lic.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/nla/cssp.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/nla/cssp.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/nla/ntlm.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/nla/ntlm.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/nla/sspi.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/nla/sspi.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/caps.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/pdu/caps.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/data.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/pdu/data.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/layer.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/pdu/layer.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/pdu/order.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/pdu/order.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/rdp.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/rdp.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/sec.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/sec.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/t125/ber.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/t125/ber.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/t125/gcc.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/t125/gcc.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/t125/mcs.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/t125/mcs.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/t125/per.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/t125/per.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/tpkt.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/tpkt.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rdp/x224.py` & `rdpy3-1.3.5/rdpy3/protocol/rdp/x224.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/protocol/rfb/rfb.py` & `rdpy3-1.3.5/rdpy3/protocol/rfb/rfb.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/security/pyDes.py` & `rdpy3-1.3.5/rdpy3/security/pyDes.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/security/rc4.py` & `rdpy3-1.3.5/rdpy3/security/rc4.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/security/rsa_wrapper.py` & `rdpy3-1.3.5/rdpy3/security/rsa_wrapper.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/security/x509.py` & `rdpy3-1.3.5/rdpy3/security/x509.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/ui/qt5.py` & `rdpy3-1.3.5/rdpy3/ui/qt5.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3/ui/view.py` & `rdpy3-1.3.5/rdpy3/ui/view.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/rdpy3.egg-info/PKG-INFO` & `rdpy3-1.3.5/rdpy3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdpy3
-Version: 1.3.4
+Version: 1.3.5
 Summary: Remote Desktop Protocol in Python3
 Home-page: https://github.com/james4ever0/rdpy3
 Author: Sylvain Peyrefitte
 Author-email: citronneur@gmail.com
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rdpy3-1.3.4/rdpy3.egg-info/SOURCES.txt` & `rdpy3-1.3.5/rdpy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/setup.py` & `rdpy3-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 import setuptools
 from distutils.core import setup, Extension
 
 setup(name='rdpy3',
-      version='1.3.4',
+      version='1.3.5',
       description='Remote Desktop Protocol in Python3',
       long_description_content_type="text/markdown",
-	  python_requires=">=3",
+      python_requires=">=3",
       long_description=open("README.md").read(),
       # long_description="""
       # RDPY is a pure Python implementation of the Microsoft RDP (Remote Desktop Protocol) protocol (Client and Server side). RDPY is built over the event driven network engine Twisted.
 
       # RDPY provide RDP and VNC binaries : RDP Man In The Middle proxy which record session, RDP Honeypot, RDP screenshoter, RDP client, VNC client, VNC screenshoter, RSS Player
       # """,
       author='Sylvain Peyrefitte',
```

### Comparing `rdpy3-1.3.4/test/test_core_const.py` & `rdpy3-1.3.5/test/test_core_const.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_core_layer.py` & `rdpy3-1.3.5/test/test_core_layer.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_core_type.py` & `rdpy3-1.3.5/test/test_core_type.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_protocol_rdp_ber.py` & `rdpy3-1.3.5/test/test_protocol_rdp_ber.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_protocol_rdp_cssp_ntlm.py` & `rdpy3-1.3.5/test/test_protocol_rdp_cssp_ntlm.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_protocol_rdp_lic.py` & `rdpy3-1.3.5/test/test_protocol_rdp_lic.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_protocol_rdp_mcs.py` & `rdpy3-1.3.5/test/test_protocol_rdp_mcs.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_protocol_rdp_per.py` & `rdpy3-1.3.5/test/test_protocol_rdp_per.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_protocol_rdp_rc4.py` & `rdpy3-1.3.5/test/test_protocol_rdp_rc4.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_protocol_rdp_tpkt.py` & `rdpy3-1.3.5/test/test_protocol_rdp_tpkt.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_protocol_rdp_x224.py` & `rdpy3-1.3.5/test/test_protocol_rdp_x224.py`

 * *Files identical despite different names*

### Comparing `rdpy3-1.3.4/test/test_protocol_rfb_rfb.py` & `rdpy3-1.3.5/test/test_protocol_rfb_rfb.py`

 * *Files identical despite different names*

