# Comparing `tmp/mitmproxy_rs-0.2.0b9.tar.gz` & `tmp/mitmproxy_rs-0.2.1.tar.gz`

## Comparing `mitmproxy_rs-0.2.0b9.tar` & `mitmproxy_rs-0.2.1.tar`

### file list

```diff
@@ -1,63 +1,96 @@
--rw-r--r--   0        0        0     1995 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/Cargo.toml
--rw-r--r--   0     1001      123       84 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.cargo/config.toml
--rw-r--r--   0     1001      123       28 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/FUNDING.yml
--rw-r--r--   0     1001      123      511 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/dependabot.yml
--rw-r--r--   0     1001      123        5 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/python-version.txt
--rw-r--r--   0     1001      123     1158 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/autofix.yml
--rw-r--r--   0     1001      123     4222 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/ci.yml
--rw-r--r--   0     1001      123     1869 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/docs.yml
--rw-r--r--   0     1001      123       57 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.gitignore
--rw-r--r--   0     1001      123     4472 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/CHANGELOG.md
--rwxr-xr-x   0     1001      123     2085 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1080 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/LICENSE
--rw-r--r--   0     1001      123     3271 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/README.md
--rw-r--r--   0     1001      123   243520 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/architecture.png
--rw-r--r--   0     1001      123       22 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/.gitignore
--rw-r--r--   0     1001      123      220 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/local.conf
--rw-r--r--   0     1001      123      214 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/nonlocal.conf
--rw-r--r--   0     1001      123    67352 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/openvpnserv.exe
--rw-r--r--   0     1001      123    10121 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/plot.py
--rwxr-xr-x   0     1001      123     1730 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/process.rs
--rw-r--r--   0     1001      123     2375 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/py_echo_client.py
--rw-r--r--   0     1001      123     1246 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/py_echo_server.py
--rw-r--r--   0     1001      123     2346 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/wg_echo_client.py
--rw-r--r--   0     1001      123     2036 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/wg_echo_server.py
--rwxr-xr-x   0     1001      123      264 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/coverage.sh
--rwxr-xr-x   0     1001      123     4188 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/intercept_conf.rs
--rwxr-xr-x   0     1001      123      202 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/lib.rs
--rwxr-xr-x   0     1001      123     3863 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/messages.rs
--rwxr-xr-x   0     1001      123      126 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/mod.rs
--rwxr-xr-x   0     1001      123    26177 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/task.rs
--rwxr-xr-x   0     1001      123    26991 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/tests.rs
--rwxr-xr-x   0     1001      123     2705 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/virtual_device.rs
--rwxr-xr-x   0     1001      123      662 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/mod.rs
--rwxr-xr-x   0     1001      123     7813 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/windows.rs
--rwxr-xr-x   0     1001      123    13781 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs
--rw-r--r--   0     1001      123      243 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/processes.rs
--rwxr-xr-x   0     1001      123     3721 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/shutdown.rs
--rwxr-xr-x   0     1001      123        1 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/util.rs
--rw-r--r--   0     1001      123     5276 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/icons.rs
--rw-r--r--   0     1001      123       51 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/mod.rs
--rw-r--r--   0     1001      123     6828 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/network.rs
--rw-r--r--   0     1001      123    10928 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/processes.rs
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.0b9/Cargo.toml
--rw-r--r--   0     1001      123       97 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/.gitignore
--rw-r--r--   0     1001      123     2850 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/README.md
--rwxr-xr-x   0     1001      123     1919 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/build.rs
--rw-r--r--   0     1001      123      132 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/mitmproxy_rs/__init__.py
--rw-r--r--   0     1001      123     2296 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/mitmproxy_rs/__init__.pyi
--rw-r--r--   0     1001      123      121 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/mitmproxy_rs/_pyinstaller/__init__.py
--rw-r--r--   0     1001      123       99 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/mitmproxy_rs/_pyinstaller/hook-mitmproxy_rs.py
--rw-r--r--   0     1001      123        0 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/mitmproxy_rs/py.typed
--rw-r--r--   0     1001      123      745 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/pyproject.toml
--rwxr-xr-x   0     1001      123     3575 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/datagram_transport.rs
--rwxr-xr-x   0     1001      123     1737 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/lib.rs
--rw-r--r--   0     1001      123     2054 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/process_info.rs
--rwxr-xr-x   0     1001      123    10062 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/server.rs
--rwxr-xr-x   0     1001      123     7234 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/task.rs
--rwxr-xr-x   0     1001      123     5452 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/tcp_stream.rs
--rwxr-xr-x   0     1001      123     2036 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/src/util.rs
--rwxr-xr-x   0     1001      123       70 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/stubtest-allowlist.txt
--rw-r--r--   0     1001      123      125 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/test.py
--rw-r--r--   0     1001      123    69220 2023-06-13 14:17:34.000000 mitmproxy_rs-0.2.0b9/Cargo.lock
--rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.0b9/PKG-INFO
+-rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/Cargo.toml
+-rw-r--r--   0     1001      123       84 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.cargo/config.toml
+-rw-r--r--   0     1001      123       28 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/FUNDING.yml
+-rw-r--r--   0     1001      123      511 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/dependabot.yml
+-rw-r--r--   0     1001      123        5 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/python-version.txt
+-rwxr-xr-x   0     1001      123     2437 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/scripts/build-macos-redirector.sh
+-rw-r--r--   0     1001      123     1158 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/autofix.yml
+-rw-r--r--   0     1001      123     5072 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123     1869 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/docs.yml
+-rw-r--r--   0     1001      123       71 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.gitignore
+-rw-r--r--   0     1001      123     4472 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/CHANGELOG.md
+-rwxr-xr-x   0     1001      123     2085 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1080 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/LICENSE
+-rw-r--r--   0     1001      123     3271 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/README.md
+-rw-r--r--   0     1001      123   243520 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/architecture.png
+-rw-r--r--   0     1001      123       22 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/.gitignore
+-rw-r--r--   0     1001      123      220 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/local.conf
+-rw-r--r--   0     1001      123      214 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/nonlocal.conf
+-rw-r--r--   0     1001      123    67352 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/openvpnserv.exe
+-rw-r--r--   0     1001      123    10121 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/plot.py
+-rwxr-xr-x   0     1001      123     1730 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/process.rs
+-rw-r--r--   0     1001      123     2375 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/py_echo_client.py
+-rw-r--r--   0     1001      123     1246 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/py_echo_server.py
+-rw-r--r--   0     1001      123     2346 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/wg_echo_client.py
+-rw-r--r--   0     1001      123     2036 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/wg_echo_server.py
+-rw-r--r--   0     1001      123      306 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/build.rs
+-rwxr-xr-x   0     1001      123      264 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/coverage.sh
+-rw-r--r--   0     1001      123      431 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/Info.plist
+-rw-r--r--   0     1001      123      690 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/MitmproxyAppleExtension.entitlements
+-rw-r--r--   0     1001      123     5141 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/PacketTunnelProvider.swift
+-rw-r--r--   0     1001      123     5628 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleExtension/ipc.pb.swift
+-rw-r--r--   0     1001      123   345532 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/1024.png
+-rw-r--r--   0     1001      123    13181 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/128.png
+-rw-r--r--   0     1001      123      902 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/16.png
+-rw-r--r--   0     1001      123    36415 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/256.png
+-rw-r--r--   0     1001      123     2205 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/32.png
+-rw-r--r--   0     1001      123   116514 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/512.png
+-rw-r--r--   0     1001      123     5379 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/64.png
+-rw-r--r--   0     1001      123     1358 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0     1001      123       63 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Assets.xcassets/Contents.json
+-rw-r--r--   0     1001      123      171 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Constants.swift
+-rw-r--r--   0     1001      123     1509 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Controller/AppDelegate.swift
+-rw-r--r--   0     1001      123      218 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Controller/ViewController.swift
+-rw-r--r--   0     1001      123      690 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/MitmproxyAppleTunnel.entitlements
+-rw-r--r--   0     1001      123     6048 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/Model/Proxy.swift
+-rw-r--r--   0     1001      123    60507 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel/View/Base.lproj/Main.storyboard
+-rw-r--r--   0     1001      123    26319 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.pbxproj
+-rw-r--r--   0     1001      123      135 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+-rw-r--r--   0     1001      123      238 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-r--r--   0     1001      123      181 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcshareddata/WorkspaceSettings.xcsettings
+-rw-r--r--   0     1001      123      311 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcshareddata/swiftpm/Package.resolved
+-rw-r--r--   0     1001      123      182 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcuserdata/emanuelemicheletti.xcuserdatad/IDEFindNavigatorScopes.plist
+-rw-r--r--   0     1001      123      453 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/project.xcworkspace/xcuserdata/emanuelemicheletti.xcuserdatad/WorkspaceSettings.xcsettings
+-rw-r--r--   0     1001      123     3869 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcshareddata/xcschemes/MitmproxyAppleExtension.xcscheme
+-rw-r--r--   0     1001      123     4638 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcshareddata/xcschemes/MitmproxyAppleTunnel.xcscheme
+-rw-r--r--   0     1001      123      872 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcuserdata/emanuelemicheletti.xcuserdatad/xcdebugger/Breakpoints_v2.xcbkptlist
+-rw-r--r--   0     1001      123      719 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/macos-redirector/MitmproxyAppleTunnel.xcodeproj/xcuserdata/emanuelemicheletti.xcuserdatad/xcschemes/xcschememanagement.plist
+-rwxr-xr-x   0     1001      123     4410 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/intercept_conf.rs
+-rwxr-xr-x   0     1001      123      202 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/lib.rs
+-rwxr-xr-x   0     1001      123     3863 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/messages.rs
+-rwxr-xr-x   0     1001      123      126 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/mod.rs
+-rwxr-xr-x   0     1001      123    26233 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/task.rs
+-rwxr-xr-x   0     1001      123    26991 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/tests.rs
+-rwxr-xr-x   0     1001      123     2705 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/virtual_device.rs
+-rw-r--r--   0     1001      123      322 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/ipc.proto
+-rwxr-xr-x   0     1001      123      740 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/mod.rs
+-rwxr-xr-x   0     1001      123     7965 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/windows.rs
+-rwxr-xr-x   0     1001      123    13781 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs
+-rw-r--r--   0     1001      123      243 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/processes.rs
+-rwxr-xr-x   0     1001      123     3721 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/shutdown.rs
+-rwxr-xr-x   0     1001      123        1 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/util.rs
+-rw-r--r--   0     1001      123     5276 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/icons.rs
+-rw-r--r--   0     1001      123       51 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/mod.rs
+-rw-r--r--   0     1001      123     6828 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/network.rs
+-rw-r--r--   0     1001      123    10928 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/processes.rs
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123       97 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/.gitignore
+-rw-r--r--   0     1001      123     2850 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/README.md
+-rwxr-xr-x   0     1001      123     1919 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/build.rs
+-rw-r--r--   0     1001      123      132 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/mitmproxy_rs/__init__.py
+-rw-r--r--   0     1001      123     2296 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/mitmproxy_rs/__init__.pyi
+-rw-r--r--   0     1001      123      121 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/mitmproxy_rs/_pyinstaller/__init__.py
+-rw-r--r--   0     1001      123       99 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/mitmproxy_rs/_pyinstaller/hook-mitmproxy_rs.py
+-rw-r--r--   0     1001      123        0 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/mitmproxy_rs/py.typed
+-rw-r--r--   0     1001      123      745 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/pyproject.toml
+-rwxr-xr-x   0     1001      123     3575 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/datagram_transport.rs
+-rwxr-xr-x   0     1001      123     1737 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123     2054 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/process_info.rs
+-rwxr-xr-x   0     1001      123    10121 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/server.rs
+-rwxr-xr-x   0     1001      123     7234 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/task.rs
+-rwxr-xr-x   0     1001      123     5452 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/tcp_stream.rs
+-rwxr-xr-x   0     1001      123     2048 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/src/util.rs
+-rwxr-xr-x   0     1001      123       70 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/stubtest-allowlist.txt
+-rw-r--r--   0     1001      123      125 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/test.py
+-rw-r--r--   0     1001      123    70506 2023-08-04 22:48:35.000000 mitmproxy_rs-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 mitmproxy_rs-0.2.1/PKG-INFO
```

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/Cargo.toml` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -7,56 +7,51 @@
 ]
 
 [workspace.package]
 authors = [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version = "0.2.0-beta.9"
+version = "0.2.1"
 publish = false
 repository = "https://github.com/mitmproxy/mitmproxy-rs"
 edition = "2021"
 rust-version = "1.65.0"
 
-[workspace.dependencies]
-bincode = "2.0.0-rc.3"
-
 [package]
 name = "mitmproxy"
 license = "MIT"
 authors= [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version= "0.2.0-beta.9"
+version= "0.2.1"
 repository= "https://github.com/mitmproxy/mitmproxy-rs"
 edition= "2021"
 rust-version= "1.65.0"
 publish= false
 
 [dependencies]
 anyhow = { version = "1.0.71", features = ["backtrace"] }
 log = "0.4.18"
 once_cell = "1"
 pretty-hex = "0.3.0"
 rand_core = { version = "0.6.4", features = ["getrandom"] }
-smoltcp = "0.9"
-tokio = { version = "1.28.2", features = ["macros", "net", "rt-multi-thread", "sync", "time", "io-util"] }
+smoltcp = "0.10"
+tokio = { version = "1.29.1", features = ["macros", "net", "rt-multi-thread", "sync", "time", "io-util"] }
 boringtun = { version = "0.5", default-features = false }
-x25519-dalek = "=2.0.0-pre.1"
+x25519-dalek = "=2.0.0-rc.3"
 async-trait = "0.1.68"
 console-subscriber = { version = "0.1.9", optional = true }
 image = "0.24.6"
+prost = "0.11.9"
 
 [patch.crates-io]
 # tokio = { path = "../tokio/tokio" }
-smoltcp = { git = 'https://github.com/mhils/smoltcp', rev = 'f65351adfa92db5193f368368cb668bac721fe43' }
-
-[target.'cfg(windows)'.dependencies]
-bincode= "2.0.0-rc.3"
+# smoltcp = { git = 'https://github.com/mhils/smoltcp', rev = 'f65351adfa92db5193f368368cb668bac721fe43' }
 
 [target.'cfg(windows)'.dependencies.windows]
 version = "0.48.0"
 features = [
     "Win32_Foundation",
     "Win32_Graphics_Dwm",
     "Win32_Graphics_Gdi",
@@ -66,14 +61,18 @@
     "Win32_System_LibraryLoader",
     "Win32_System_ProcessStatus",
     "Win32_System_Threading",
     "Win32_UI_Shell",
     "Win32_UI_WindowsAndMessaging",
 ]
 
+[build-dependencies]
+prost-build = "0.11.9"
+protoc-bin-vendored = "3"
+
 [[bench]]
 name = "process"
 harness = false
 
 [profile.release]
 codegen-units = 1
 lto = true
```

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/autofix.yml` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/autofix.yml`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/ci.yml` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/ci.yml`

 * *Files 13% similar despite different names*

```diff
@@ -47,14 +47,21 @@
       - uses: actions/setup-python@v4
         with:
           python-version-file: .github/python-version.txt
 
       - if: runner.os == 'Windows'
         # workaround for https://github.com/rust-lang/cargo/issues/9096
         run: cargo build --package windows-redirector
+      - if: runner.os == 'macOS'
+        run: .github/scripts/build-macos-redirector.sh
+        env:
+          BUILD_CERTIFICATE_BASE64: ${{ secrets.BUILD_CERTIFICATE_BASE64 }}
+          P12_PASSWORD: ${{ secrets.P12_PASSWORD }}
+          BUILD_PROVISION_PROFILE_BASE64: ${{ secrets.BUILD_PROVISION_PROFILE_BASE64 }}
+          BUILD_PROVISION_PROFILE_EXTENSION_BASE64: ${{ secrets.BUILD_PROVISION_PROFILE_EXTENSION_BASE64 }}
 
       - name: Run "cargo check"
         # the action-rs/cargo action adds inline annotations for "cargo check" output
         uses: actions-rs/cargo@9e120dd99b0fbad1c065f686657e914e76bd7b72
         with:
           toolchain: ${{ matrix.rust }}
           command: check
@@ -105,22 +112,29 @@
 
       - name: Install maturin[zig] from PyPI
         uses: install-pinned/maturin-with-zig@59341946682d2f69df7150f6941f53e026e344fd
 
       - if: runner.os == 'Windows'
         # workaround for https://github.com/rust-lang/cargo/issues/9096
         run: cargo build --release --package windows-redirector
+      - if: runner.os == 'macOS'
+        run: .github/scripts/build-macos-redirector.sh
+        env:
+          BUILD_CERTIFICATE_BASE64: ${{ secrets.BUILD_CERTIFICATE_BASE64 }}
+          P12_PASSWORD: ${{ secrets.P12_PASSWORD }}
+          BUILD_PROVISION_PROFILE_BASE64: ${{ secrets.BUILD_PROVISION_PROFILE_BASE64 }}
+          BUILD_PROVISION_PROFILE_EXTENSION_BASE64: ${{ secrets.BUILD_PROVISION_PROFILE_EXTENSION_BASE64 }}
 
       - run: maturin build --release ${{ matrix.args }}
         working-directory: ./ffi
+
       - uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: target/wheels
-
   deploy:
     uses: mhils/workflows/.github/workflows/python-deploy.yml@main
     needs: [test, build]
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     with:
       artifact: wheels
       # repository: testpypi
```

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/.github/workflows/docs.yml` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/.github/workflows/docs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,17 @@
             ~/.cargo/git/db/
             target/
           key: ${{ runner.os }}-cargo-${{ hashFiles('**/Cargo.lock') }}
 
       - name: Install maturin[zig] from PyPI
         uses: install-pinned/maturin-with-zig@59341946682d2f69df7150f6941f53e026e344fd
       - name: Install mypy from PyPI
-        uses: install-pinned/mypy@c581c551e8cff8b305445a9c8375b5d08f330887
+        uses: install-pinned/mypy@0ac9691d218a55b59b345debcd9d4b3ca17b391b
       - name: Install pdoc from PyPI
-        uses: install-pinned/pdoc@fac9037f8ea1d23a645d9ffe26f67877834518c8
+        uses: install-pinned/pdoc@7ed463fdd937004663bcdd7b43c303e9df472c92
 
       - run: maturin build
         working-directory: ./ffi
       - run: pip install --no-index --find-links target/wheels/ mitmproxy_rs
 
       - run: stubtest --allowlist ffi/stubtest-allowlist.txt --mypy-config-file ffi/pyproject.toml mitmproxy_rs
```

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/CHANGELOG.md` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/CONTRIBUTING.md` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/LICENSE` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/LICENSE`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/README.md` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/README.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/architecture.png` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/architecture.png`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/openvpnserv.exe` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/openvpnserv.exe`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/plot.py` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/plot.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/process.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/process.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/py_echo_client.py` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/py_echo_client.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/py_echo_server.py` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/py_echo_server.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/wg_echo_client.py` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/wg_echo_client.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/benches/wg_echo_server.py` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/benches/wg_echo_server.py`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/intercept_conf.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/intercept_conf.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-use anyhow::bail;
-#[cfg(windows)]
-use bincode::{Decode, Encode};
 use std::collections::HashSet;
-use std::path::PathBuf;
+
+use anyhow::bail;
 
 pub type PID = u32;
 
 #[derive(Debug, Clone)]
 pub struct ProcessInfo {
     pub pid: PID,
-    pub process_name: Option<PathBuf>,
+    pub process_name: Option<String>,
 }
 
-#[cfg_attr(windows, derive(Decode, Encode))]
 #[derive(PartialEq, Eq, Debug, Clone)]
 pub struct InterceptConf {
     pids: HashSet<PID>,
     process_names: Vec<String>,
     /// if true, matching items are the ones which are not intercepted.
     invert: bool,
 }
@@ -48,14 +45,32 @@
                 Err(_) => procs.push(part.to_string()),
             }
         }
         Ok(InterceptConf::new(pids, procs, invert))
     }
 }
 
+impl ToString for InterceptConf {
+    fn to_string(&self) -> String {
+        let spec = self
+            .pids
+            .iter()
+            .map(|x| x.to_string())
+            .chain(self.process_names.clone())
+            .collect::<Vec<String>>()
+            .join(",");
+
+        if self.invert {
+            format!("!{}", spec)
+        } else {
+            spec
+        }
+    }
+}
+
 impl InterceptConf {
     pub fn new(pids: Vec<PID>, process_names: Vec<String>, invert: bool) -> Self {
         let pids = HashSet::from_iter(pids.into_iter());
         if invert {
             assert!(!pids.is_empty() || !process_names.is_empty());
         }
         Self {
@@ -68,15 +83,14 @@
     pub fn should_intercept(&self, process_info: &ProcessInfo) -> bool {
         self.invert ^ {
             if self.pids.contains(&process_info.pid) {
                 true
             } else if self.process_names.is_empty() {
                 false // fast path to avoid conversion below.
             } else if let Some(name) = &process_info.process_name {
-                let name = name.to_string_lossy();
                 self.process_names.iter().any(|n| name.contains(n))
             } else {
                 false
             }
         }
     }
```

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/messages.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/messages.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/task.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/task.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 use anyhow::Result;
 use pretty_hex::pretty_hex;
 use smoltcp::iface::{Config, SocketSet};
 use smoltcp::socket::{tcp, Socket};
 
 use smoltcp::wire::{
-    Icmpv4Message, Icmpv4Packet, Icmpv4Repr, Icmpv6Message, Icmpv6Packet, Icmpv6Repr,
+    HardwareAddress, Icmpv4Message, Icmpv4Packet, Icmpv4Repr, Icmpv6Message, Icmpv6Packet,
+    Icmpv6Repr,
 };
 use smoltcp::{
     iface::{Interface, SocketHandle},
     phy::ChecksumCapabilities,
     time::{Duration, Instant},
     wire::{
         IpAddress, IpCidr, IpProtocol, IpRepr, Ipv4Address, Ipv4Packet, Ipv4Repr, Ipv6Address,
@@ -61,16 +62,16 @@
     next_connection_id: ConnectionId,
 }
 
 impl<'a> NetworkIO<'a> {
     fn new(net_tx: Sender<NetworkCommand>) -> Self {
         let mut device = VirtualDevice::new(net_tx.clone());
 
-        let config = Config::new();
-        let mut iface = Interface::new(config, &mut device);
+        let config = Config::new(HardwareAddress::Ip);
+        let mut iface = Interface::new(config, &mut device, Instant::now());
 
         iface.set_any_ip(true);
 
         iface.update_ip_addrs(|ip_address| {
             ip_address
                 .push(IpCidr::new(IpAddress::v4(0, 0, 0, 1), 0))
                 .unwrap();
```

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/tests.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/tests.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/network/virtual_device.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/network/virtual_device.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/mod.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/mod.rs`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 use crate::messages::{NetworkCommand, NetworkEvent};
 
 #[cfg(windows)]
 pub mod windows;
 pub mod wireguard;
 
+pub mod ipc {
+    include!(concat!(env!("OUT_DIR"), "/mitmproxy.ipc.rs"));
+}
+
 #[async_trait]
 pub trait PacketSourceConf {
     type Task: PacketSourceTask + Send + 'static;
     type Data: Send + 'static;
 
     fn name(&self) -> &'static str;
```

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/windows.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/windows.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,42 @@
+use std::io::Cursor;
 use std::iter;
 use std::os::windows::ffi::OsStrExt;
 use std::path::PathBuf;
 
 use anyhow::{anyhow, Context, Result};
 use async_trait::async_trait;
-use bincode::{Decode, Encode};
 use tokio::io::{AsyncReadExt, AsyncWriteExt};
 use tokio::net::windows::named_pipe::{NamedPipeServer, PipeMode, ServerOptions};
 use tokio::sync::broadcast;
 use tokio::sync::mpsc::Sender;
 use tokio::sync::mpsc::{unbounded_channel, Receiver, UnboundedReceiver, UnboundedSender};
 use windows::core::PCWSTR;
 use windows::w;
 use windows::Win32::UI::Shell::ShellExecuteW;
 use windows::Win32::UI::Shell::SE_ERR_ACCESSDENIED;
 use windows::Win32::UI::WindowsAndMessaging::{SW_HIDE, SW_SHOWNORMAL};
 
-use crate::intercept_conf::InterceptConf;
 use crate::messages::{IpPacket, NetworkCommand, NetworkEvent, TunnelInfo};
 use crate::network::MAX_PACKET_SIZE;
-use crate::packet_sources::{PacketSourceConf, PacketSourceTask};
+use crate::packet_sources::ipc::from_redirector::Message::Packet;
+use crate::packet_sources::ipc::{FromRedirector, PacketWithMeta};
+use crate::packet_sources::{ipc, PacketSourceConf, PacketSourceTask};
+use prost::Message;
 
-pub const CONF: bincode::config::Configuration = bincode::config::standard();
-pub const IPC_BUF_SIZE: usize = MAX_PACKET_SIZE + 4;
-
-#[derive(Decode, Encode, PartialEq, Eq, Debug)]
-pub enum WindowsIpcRecv {
-    Packet {
-        data: Vec<u8>,
-        pid: u32,
-        process_name: Option<PathBuf>,
-    },
-}
-
-#[derive(Decode, Encode, PartialEq, Eq, Debug)]
-pub enum WindowsIpcSend {
-    Packet(Vec<u8>),
-    SetIntercept(InterceptConf),
-}
+pub const IPC_BUF_SIZE: usize = MAX_PACKET_SIZE + 1024;
 
 pub struct WindowsConf {
     pub executable_path: PathBuf,
 }
 
 #[async_trait]
 impl PacketSourceConf for WindowsConf {
     type Task = WindowsTask;
-    type Data = UnboundedSender<WindowsIpcSend>;
+    type Data = UnboundedSender<ipc::FromProxy>;
 
     fn name(&self) -> &'static str {
         "Windows proxy"
     }
 
     async fn build(
         self,
@@ -133,15 +119,15 @@
 
 pub struct WindowsTask {
     ipc_server: NamedPipeServer,
     buf: [u8; IPC_BUF_SIZE],
 
     net_tx: Sender<NetworkEvent>,
     net_rx: Receiver<NetworkCommand>,
-    conf_rx: UnboundedReceiver<WindowsIpcSend>,
+    conf_rx: UnboundedReceiver<ipc::FromProxy>,
     sd_watcher: broadcast::Receiver<()>,
 }
 
 #[async_trait]
 impl PacketSourceTask for WindowsTask {
     async fn run(mut self) -> Result<()> {
         log::debug!("Waiting for IPC connection...");
@@ -150,16 +136,18 @@
 
         loop {
             tokio::select! {
                 // wait for graceful shutdown
                 _ = self.sd_watcher.recv() => break,
                 // pipe through changes to the intercept list
                 Some(cmd) = self.conf_rx.recv() => {
-                    assert!(matches!(cmd, WindowsIpcSend::SetIntercept(_)));
-                    let len = bincode::encode_into_slice(&cmd, &mut self.buf, CONF)?;
+                    assert!(matches!(cmd, ipc::FromProxy { message: Some(ipc::from_proxy::Message::InterceptSpec(_)) }));
+                    cmd.encode(&mut self.buf.as_mut_slice())?;
+                    let len = cmd.encoded_len();
+
                     self.ipc_server.write_all(&self.buf[..len]).await?;
                 },
                 // read packets from the IPC pipe into our network stack.
                 r = self.ipc_server.read(&mut self.buf) => {
                     let len = r.context("IPC read error.")?;
                     if len == 0 {
                         // https://learn.microsoft.com/en-us/windows/win32/ipc/named-pipe-client
@@ -167,18 +155,25 @@
                         // possible for the ReadFile operation to return zero after reading a partial
                         // message. This happens when the message is larger than the read buffer.
                         //
                         // We don't support messages larger than the buffer, so this cannot happen.
                         // Instead, empty reads indicate that the IPC client has disconnected.
                         return Err(anyhow!("redirect daemon exited prematurely."));
                     }
-                    let Ok((WindowsIpcRecv::Packet { data, pid, process_name }, n)) = bincode::decode_from_slice(&self.buf[..len], CONF) else {
+
+                    let mut cursor = Cursor::new(&self.buf[..len]);
+                    let Ok(FromRedirector { message: Some(message)}) = FromRedirector::decode(&mut cursor) else {
                         return Err(anyhow!("Received invalid IPC message: {:?}", &self.buf[..len]));
                     };
-                    assert_eq!(n, len);
+                    assert_eq!(cursor.position(), len as u64);
+
+                    let (data, pid, process_name) = match message {
+                        Packet(PacketWithMeta { data, pid, process_name}) => (data, pid, process_name.map(PathBuf::from)),
+                    };
+
                     let Ok(mut packet) = IpPacket::try_from(data) else {
                         log::error!("Skipping invalid packet: {:?}", &self.buf[..len]);
                         continue;
                     };
                     // WinDivert packets do not have correct IP checksums yet, we need fix that here
                     // otherwise smoltcp will be unhappy with us.
                     packet.fill_ip_checksum();
@@ -194,16 +189,17 @@
                         log::warn!("Dropping incoming packet, TCP channel is full.")
                     };
                 },
                 // write packets from the network stack to the IPC pipe to be reinjected.
                 Some(e) = self.net_rx.recv() => {
                     match e {
                         NetworkCommand::SendPacket(packet) => {
-                            let packet = WindowsIpcSend::Packet(packet.into_inner());
-                            let len = bincode::encode_into_slice(&packet, &mut self.buf, CONF)?;
+                            let packet = ipc::FromProxy { message: Some(ipc::from_proxy::Message::Packet(packet.into_inner()))};
+                            packet.encode(&mut self.buf.as_mut_slice())?;
+                            let len = packet.encoded_len();
                             self.ipc_server.write_all(&self.buf[..len]).await?;
                         }
                     }
                 }
             }
         }
```

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/packet_sources/wireguard.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/shutdown.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/shutdown.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/icons.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/icons.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/network.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/network.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/local_dependencies/mitmproxy/src/windows/processes.rs` & `mitmproxy_rs-0.2.1/local_dependencies/mitmproxy/src/windows/processes.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/Cargo.toml` & `mitmproxy_rs-0.2.1/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [package]
 name = "mitmproxy_rs"
 license = "MIT"
 authors= [
     "Fabio Valentini <decathorpe@gmail.com>",
     "Maximilian Hils <cargo@maximilianhils.com>",
 ]
-version= "0.2.0-beta.9"
+version= "0.2.1"
 repository= "https://github.com/mitmproxy/mitmproxy-rs"
 edition= "2021"
 rust-version= "1.65.0"
 publish= false
 
 [lib]
 name = "mitmproxy_rs"
@@ -21,15 +21,15 @@
 data-encoding = "2.4.0"
 log = "0.4.18"
 once_cell = "1"
 pyo3 = { version = "0.18.2", features = ["abi3", "abi3-py310", "extension-module", "anyhow"] }
 pyo3-asyncio = { version = "0.18.0", features = ["tokio-runtime"] }
 pyo3-log = "0.8.1"
 rand_core = { version = "0.6.4", features = ["getrandom"] }
-tokio = { version = "1.27", features = ["macros", "net", "rt-multi-thread", "sync"] }
+tokio = { version = "1.29", features = ["macros", "net", "rt-multi-thread", "sync"] }
 x25519-dalek = "2.0.0-pre.1"
 
 # optional dependencies for tracing support
 console-subscriber = { version = "0.1.9", optional = true }
 
 [features]
 tracing = ["console-subscriber"]
```

### Comparing `mitmproxy_rs-0.2.0b9/README.md` & `mitmproxy_rs-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/build.rs` & `mitmproxy_rs-0.2.1/build.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/mitmproxy_rs/__init__.pyi` & `mitmproxy_rs-0.2.1/mitmproxy_rs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/pyproject.toml` & `mitmproxy_rs-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/src/datagram_transport.rs` & `mitmproxy_rs-0.2.1/src/datagram_transport.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/src/lib.rs` & `mitmproxy_rs-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/src/process_info.rs` & `mitmproxy_rs-0.2.1/src/process_info.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/src/server.rs` & `mitmproxy_rs-0.2.1/src/server.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 use pyo3::prelude::*;
 use tokio::{sync::broadcast, sync::mpsc, sync::Notify};
 use x25519_dalek::PublicKey;
 
 use mitmproxy::intercept_conf::InterceptConf;
 use mitmproxy::network::NetworkTask;
 #[cfg(windows)]
-use mitmproxy::packet_sources::windows::{WindowsConf, WindowsIpcSend};
+use mitmproxy::packet_sources::windows::WindowsConf;
 
 use mitmproxy::packet_sources::wireguard::WireGuardConf;
-use mitmproxy::packet_sources::{PacketSourceConf, PacketSourceTask};
+use mitmproxy::packet_sources::{ipc, PacketSourceConf, PacketSourceTask};
 use mitmproxy::shutdown::ShutdownTask;
 
 use crate::task::PyInteropTask;
 use crate::util::{socketaddr_to_py, string_to_key};
 
 #[derive(Debug)]
 pub struct Server {
@@ -143,34 +143,36 @@
 }
 
 #[pyclass(module = "mitmproxy_rs")]
 #[derive(Debug)]
 pub struct OsProxy {
     server: Server,
     #[cfg(windows)]
-    conf_tx: mpsc::UnboundedSender<WindowsIpcSend>,
+    conf_tx: mpsc::UnboundedSender<ipc::FromProxy>,
 }
 
 #[pymethods]
 impl OsProxy {
     /// Return a textual description of the given spec,
     /// or raise a ValueError if the spec is invalid.
     #[staticmethod]
     fn describe_spec(spec: &str) -> PyResult<String> {
         InterceptConf::try_from(spec)
             .map(|conf| conf.description())
             .map_err(|e| pyo3::exceptions::PyValueError::new_err(e.to_string()))
     }
 
     /// Set a new intercept spec.
-    pub fn set_intercept(&self, spec: &str) -> PyResult<()> {
-        let _conf = InterceptConf::try_from(spec)?;
+    pub fn set_intercept(&self, spec: String) -> PyResult<()> {
+        InterceptConf::try_from(spec.as_str())?;
         #[cfg(windows)]
         self.conf_tx
-            .send(WindowsIpcSend::SetIntercept(_conf))
+            .send(ipc::FromProxy {
+                message: Some(ipc::from_proxy::Message::InterceptSpec(spec)),
+            })
             .map_err(crate::util::event_queue_unavailable)?;
         Ok(())
     }
 
     /// Close the OS proxy server.
     pub fn close(&mut self) {
         self.server.close()
```

### Comparing `mitmproxy_rs-0.2.0b9/src/task.rs` & `mitmproxy_rs-0.2.1/src/task.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/src/tcp_stream.rs` & `mitmproxy_rs-0.2.1/src/tcp_stream.rs`

 * *Files identical despite different names*

### Comparing `mitmproxy_rs-0.2.0b9/src/util.rs` & `mitmproxy_rs-0.2.1/src/util.rs`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 pub fn event_queue_unavailable<T>(_: mpsc::error::SendError<T>) -> PyErr {
     PyOSError::new_err("Server has been shut down.")
 }
 
 /// Generate a WireGuard private key, analogous to the `wg genkey` command.
 #[pyfunction]
 pub fn genkey() -> String {
-    BASE64.encode(&StaticSecret::new(OsRng).to_bytes())
+    BASE64.encode(&StaticSecret::random_from_rng(OsRng).to_bytes())
 }
 
 /// Derive a WireGuard public key from a private key, analogous to the `wg pubkey` command.
 #[pyfunction]
 pub fn pubkey(private_key: String) -> PyResult<String> {
     let private_key: StaticSecret = string_to_key(private_key)?;
     Ok(BASE64.encode(PublicKey::from(&private_key).as_bytes()))
```

### Comparing `mitmproxy_rs-0.2.0b9/Cargo.lock` & `mitmproxy_rs-0.2.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "addr2line"
-version = "0.19.0"
+version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a76fd60b23679b7d19bd066031410fb7e458ccc5e958eb5c325888ce4baedc97"
+checksum = "f4fa78e18c64fce05e902adecd7a5eed15a5e0a3439f7b0e169f0252214865e3"
 dependencies = [
  "gimli",
 ]
 
 [[package]]
 name = "adler"
 version = "1.0.2"
@@ -39,80 +39,75 @@
 [[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
+name = "anstyle"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
+
+[[package]]
 name = "anyhow"
-version = "1.0.71"
+version = "1.0.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
 dependencies = [
  "backtrace",
 ]
 
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
 name = "arrayvec"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8868f09ff8cea88b079da74ae569d9b8c62a23c68c746240b704ee6f7525c89c"
+checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "async-trait"
-version = "0.1.68"
+version = "0.1.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
+checksum = "a564d521dd56509c4c47480d00b80ee55f7e385ae48db5744c67ad50c92d2ebf"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "atomic-polyfill"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3ff7eb3f316534d83a8a2c3d1674ace8a5a71198eba31e2e2b597833f699b28"
 dependencies = [
  "critical-section",
 ]
 
 [[package]]
-name = "atty"
-version = "0.2.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
-]
-
-[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "axum"
-version = "0.6.18"
+version = "0.6.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8175979259124331c1d7bf6586ee7e0da434155e4b2d48ec2c8386281d8df39"
+checksum = "a6a1de45611fdb535bfde7b7de4fd54f4fd2b17b1737c0a59b69bf9b92074b8c"
 dependencies = [
  "async-trait",
  "axum-core",
- "bitflags",
+ "bitflags 1.3.2",
  "bytes",
  "futures-util",
  "http",
  "http-body",
  "hyper",
  "itoa",
  "matchit",
@@ -143,23 +138,23 @@
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
 name = "backtrace"
-version = "0.3.67"
+version = "0.3.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "233d376d6d185f2a3093e58f283f60f880315b6c60075b01f36b3b85154564ca"
+checksum = "4319208da049c43661739c5fade2ba182f09d1dc2299b32298d3a31692b17e12"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
- "miniz_oxide 0.6.2",
+ "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
 version = "0.13.1"
@@ -169,80 +164,67 @@
 [[package]]
 name = "base64"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
-name = "bincode"
-version = "2.0.0-rc.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f11ea1a0346b94ef188834a65c068a03aec181c94896d481d7a0a40d85b0ce95"
-dependencies = [
- "bincode_derive",
- "serde",
-]
-
-[[package]]
-name = "bincode_derive"
-version = "2.0.0-rc.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e30759b3b99a1b802a7a3aa21c85c3ded5c28e1c83170d82d70f08bbf7f3e4c"
-dependencies = [
- "virtue",
-]
-
-[[package]]
 name = "bit_field"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc827186963e592360843fb5ba4b973e145841266c1357f7180c43526f2e5b61"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
 name = "blake2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
- "digest 0.10.7",
+ "digest",
 ]
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "boringtun"
-version = "0.5.2"
+version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "51d23af4567b268583ccc30a983a0f937fb5fc05e71e9de96012a72ad10d1a45"
+checksum = "e720f5e53d68bd7abfbcd315c70d1ce1bebeba2154a34de4e63860a36a241d59"
 dependencies = [
  "aead",
  "base64 0.13.1",
  "blake2",
  "chacha20poly1305",
  "hex",
  "hmac",
  "ip_network",
  "ip_network_table",
  "libc",
  "nix",
  "parking_lot",
- "rand_core 0.6.4",
+ "rand_core",
  "ring",
  "tracing",
  "untrusted 0.9.0",
  "x25519-dalek",
 ]
 
 [[package]]
@@ -347,34 +329,38 @@
  "crypto-common",
  "inout",
  "zeroize",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.25"
+version = "4.3.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
+checksum = "74bb1b4028935821b2d6b439bba2e970bdcf740832732437ead910c632e30d7d"
 dependencies = [
- "bitflags",
- "clap_lex",
- "indexmap",
- "textwrap",
+ "clap_builder",
 ]
 
 [[package]]
-name = "clap_lex"
-version = "0.2.4"
+name = "clap_builder"
+version = "4.3.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
+checksum = "5ae467cbb0111869b765e13882a1dbbd6cb52f58203d8b80c44f667d4dd19843"
 dependencies = [
- "os_str_bytes",
+ "anstyle",
+ "clap_lex",
 ]
 
 [[package]]
+name = "clap_lex"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
+
+[[package]]
 name = "color_quant"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
 
 [[package]]
 name = "console-api"
@@ -386,17 +372,17 @@
  "prost-types",
  "tonic",
  "tracing-core",
 ]
 
 [[package]]
 name = "console-subscriber"
-version = "0.1.9"
+version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57ab2224a0311582eb03adba4caaf18644f7b1f10a760803a803b9b605187fc7"
+checksum = "d4cf42660ac07fcebed809cfe561dd8730bcd35b075215e6479c516bcd0d11cb"
 dependencies = [
  "console-api",
  "crossbeam-channel",
  "crossbeam-utils",
  "futures",
  "hdrhistogram",
  "humantime",
@@ -410,17 +396,17 @@
  "tracing",
  "tracing-core",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.7"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
+checksum = "a17b76ff3a4162b0b27f354a0c87015ddad39d35f9c0c36607a3bdd175dde1f1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -428,27 +414,27 @@
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "criterion"
-version = "0.4.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
+checksum = "f2b12d017a929603d80db1831cd3a24082f8137ce19c69e6447f54f5fc8d692f"
 dependencies = [
  "anes",
- "atty",
  "cast",
  "ciborium",
  "clap",
  "criterion-plot",
+ "is-terminal",
  "itertools",
- "lazy_static",
  "num-traits",
+ "once_cell",
  "oorandom",
  "plotters",
  "rayon",
  "regex",
  "serde",
  "serde_derive",
  "serde_json",
@@ -524,80 +510,85 @@
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
- "rand_core 0.6.4",
+ "rand_core",
  "typenum",
 ]
 
 [[package]]
 name = "curve25519-dalek"
-version = "3.2.0"
+version = "4.0.0-rc.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b9fdf9972b2bd6af2d913799d9ebc165ea4d2e65878e329d9c6b372c4491b61"
+checksum = "436ace70fc06e06f7f689d2624dc4e2f0ea666efb5aa704215f7249ae6e047a7"
 dependencies = [
- "byteorder",
- "digest 0.9.0",
- "rand_core 0.5.1",
+ "cfg-if",
+ "cpufeatures",
+ "curve25519-dalek-derive",
+ "fiat-crypto",
+ "platforms",
+ "rustc_version",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
+name = "curve25519-dalek-derive"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83fdaf97f4804dcebfa5862639bc9ce4121e82140bec2a987ac5140294865b5b"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.26",
+]
+
+[[package]]
 name = "data-encoding"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
 
 [[package]]
 name = "defmt"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "956673bd3cb347512bf988d1e8d89ac9a82b64f6eec54d3c01c3529dac019882"
+checksum = "a8a2d011b2fee29fb7d659b83c43fce9a2cb4df453e16d441a51448e448f3f98"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "defmt-macros",
 ]
 
 [[package]]
 name = "defmt-macros"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4abc4821bd84d3d8f49945ddb24d029be9385ed9b77c99bf2f6296847a6a9f0"
+checksum = "54f0216f6c5acb5ae1a47050a6645024e6edafc2ee32d421955eccfef12ef92e"
 dependencies = [
  "defmt-parser",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "defmt-parser"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "269924c02afd7f94bc4cecbfa5c379f6ffcf9766b3408fe63d22c728654eccd0"
 dependencies = [
  "thiserror",
 ]
 
 [[package]]
 name = "digest"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3dd60d1080a57a05ab032377049e0591415d2b31afd7028356dbf3cc6dcb066"
-dependencies = [
- "generic-array",
-]
-
-[[package]]
-name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
  "subtle",
@@ -650,45 +641,66 @@
 checksum = "827292ea592108849932ad8e30218f8b1f21c0dfd0696698a18b5d0aed62d990"
 dependencies = [
  "arrayvec",
 ]
 
 [[package]]
 name = "exr"
-version = "1.6.4"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "279d3efcc55e19917fff7ab3ddd6c14afb6a90881a0078465196fe2f99d08c56"
+checksum = "d1e481eb11a482815d3e9d618db8c42a93207134662873809335a92327440c18"
 dependencies = [
  "bit_field",
  "flume",
  "half 2.2.1",
  "lebe",
- "miniz_oxide 0.7.1",
+ "miniz_oxide",
  "rayon-core",
  "smallvec",
  "zune-inflate",
 ]
 
 [[package]]
+name = "fastrand"
+version = "1.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
+dependencies = [
+ "instant",
+]
+
+[[package]]
 name = "fdeflate"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d329bdeac514ee06249dabc27877490f17f5d371ec693360768b838e19f3ae10"
 dependencies = [
  "simd-adler32",
 ]
 
 [[package]]
+name = "fiat-crypto"
+version = "0.1.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e825f6987101665dea6ec934c09ec6d721de7bc1bf92248e1d5810c8cd636b77"
+
+[[package]]
+name = "fixedbitset"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
+
+[[package]]
 name = "flate2"
 version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
- "miniz_oxide 0.7.1",
+ "miniz_oxide",
 ]
 
 [[package]]
 name = "flume"
 version = "0.10.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1657b4441c3403d9f7b3409e47575237dac27b1b5726df654a6ecbf92f0f7577"
@@ -758,15 +770,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -803,33 +815,22 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.1.16"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fc3cb4d91f53b50155bdcfd23f6a4c39ae1969c2ae85982b135750cccaf5fce"
-dependencies = [
- "cfg-if",
- "libc",
- "wasi 0.9.0+wasi-snapshot-preview1",
-]
-
-[[package]]
-name = "getrandom"
 version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
- "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "gif"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -837,23 +838,23 @@
 dependencies = [
  "color_quant",
  "weezl",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.27.2"
+version = "0.27.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad0a93d233ebf96623465aad4046a8d3aa4da22d4f4beba5388838c8a434bbb4"
+checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
 
 [[package]]
 name = "h2"
-version = "0.3.19"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
+checksum = "97ec8491ebaf99c8eaa73058b045fe58073cd6be7f596ac993ced0b0a0c01049"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -917,50 +918,38 @@
  "hash32",
  "rustc_version",
  "spin 0.9.8",
  "stable_deref_trait",
 ]
 
 [[package]]
-name = "hermit-abi"
-version = "0.1.19"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "hermit-abi"
-version = "0.2.6"
+name = "heck"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "hmac"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
- "digest 0.10.7",
+ "digest",
 ]
 
 [[package]]
 name = "http"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
@@ -997,17 +986,17 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "hyper"
-version = "0.14.26"
+version = "0.14.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -1076,14 +1065,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
+name = "instant"
+version = "0.1.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "internet-checksum"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc6d6206008e25125b1f97fbe5d309eb7b85141cf9199d52dbd3729a1584dd16"
 
 [[package]]
 name = "internet-packet"
@@ -1095,15 +1093,15 @@
 
 [[package]]
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
- "hermit-abi 0.3.1",
+ "hermit-abi",
  "libc",
  "windows-sys",
 ]
 
 [[package]]
 name = "ip_network"
 version = "0.4.1"
@@ -1124,38 +1122,37 @@
 name = "ip_network_table-deps-treebitmap"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e537132deb99c0eb4b752f0346b6a836200eaaa3516dd7e5514b63930a09e5d"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.7"
+version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
+checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
 dependencies = [
- "hermit-abi 0.3.1",
- "io-lifetimes",
- "rustix",
+ "hermit-abi",
+ "rustix 0.38.4",
  "windows-sys",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
+checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
 
 [[package]]
 name = "jpeg-decoder"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
 dependencies = [
@@ -1181,25 +1178,31 @@
 name = "lebe"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03087c2bad5e1034e8cace5926dec053fb3790248370865f5117a7d0213354c8"
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
+
+[[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -1225,15 +1228,15 @@
 
 [[package]]
 name = "matchers"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
- "regex-automata",
+ "regex-automata 0.1.10",
 ]
 
 [[package]]
 name = "matchit"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b87248edafb776e59e6ee64a79086f65890d3510f2c656c000bf2a7e8a0aea40"
@@ -1281,23 +1284,14 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
-dependencies = [
- "adler",
-]
-
-[[package]]
-name = "miniz_oxide"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
  "simd-adler32",
 ]
@@ -1305,88 +1299,96 @@
 [[package]]
 name = "mio"
 version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
- "wasi 0.11.0+wasi-snapshot-preview1",
+ "wasi",
  "windows-sys",
 ]
 
 [[package]]
 name = "mitm-wg-test-client"
-version = "0.2.0-beta.9"
+version = "0.2.1"
 dependencies = [
  "anyhow",
  "boringtun",
  "data-encoding",
  "hex",
  "smoltcp",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "mitmproxy"
-version = "0.2.0-beta.9"
+version = "0.2.1"
 dependencies = [
  "anyhow",
  "async-trait",
- "bincode",
  "boringtun",
  "console-subscriber",
  "criterion",
  "env_logger",
  "image",
  "log",
  "once_cell",
  "pretty-hex",
+ "prost",
+ "prost-build",
+ "protoc-bin-vendored",
  "rand",
- "rand_core 0.6.4",
+ "rand_core",
  "smoltcp",
  "tokio",
- "windows 0.48.0",
+ "windows",
  "x25519-dalek",
 ]
 
 [[package]]
 name = "mitmproxy_rs"
-version = "0.2.0-beta.9"
+version = "0.2.1"
 dependencies = [
  "anyhow",
  "console-subscriber",
  "data-encoding",
  "env_logger",
  "log",
  "mitmproxy",
  "once_cell",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
- "rand_core 0.6.4",
+ "rand_core",
  "tokio",
  "x25519-dalek",
 ]
 
 [[package]]
+name = "multimap"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
+
+[[package]]
 name = "nanorand"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a51313c5820b0b02bd422f4b44776fbf47961755c74ce64afc73bfad10226c3"
 dependencies = [
- "getrandom 0.2.10",
+ "getrandom",
 ]
 
 [[package]]
 name = "nix"
 version = "0.24.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa52e972a9a719cecb6864fb88568781eb706bac2cd1d4f04a648542dbf78069"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "cfg-if",
  "libc",
  "memoffset 0.6.5",
 ]
 
 [[package]]
 name = "nom"
@@ -1426,27 +1428,27 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.30.4"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03b4680b86d9cfafba8fc491dc9b6df26b68cf40e9e6cd73909194759a63c385"
+checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.18.0"
@@ -1462,20 +1464,14 @@
 [[package]]
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
 [[package]]
-name = "os_str_bytes"
-version = "6.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d5d9eb14b174ee9aa2ef96dc2b94637a2d4b6e7cb873c7e171f0c20c6cf3eac"
-
-[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -1497,84 +1493,100 @@
 [[package]]
 name = "percent-encoding"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
+name = "petgraph"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
+dependencies = [
+ "fixedbitset",
+ "indexmap",
+]
+
+[[package]]
 name = "pin-project"
-version = "1.1.0"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
+checksum = "030ad2bc4db10a8944cb0d837f158bdfec4d4a4873ab701a95046770d11f8842"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.1.0"
+version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
+checksum = "ec2e072ecce94ec471b13398d5402c188e76ac03cf74dd1a975161b23a3f6d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
+checksum = "4c40d25201921e5ff0c862a505c6557ea88568a4e3ace775ab55e93f2f4f9d57"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
+name = "platforms"
+version = "3.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e3d7ddaed09e0eb771a79ab0fd64609ba0afb0a8366421957936ad14cbd13630"
+
+[[package]]
 name = "plotters"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2538b639e642295546c50fcd545198c9d64ee2a38620a628724a3b266d5fbf97"
+checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
 dependencies = [
  "num-traits",
  "plotters-backend",
  "plotters-svg",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "plotters-backend"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "193228616381fecdc1224c62e96946dfbc73ff4384fba576e052ff8c1bea8142"
+checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
 
 [[package]]
 name = "plotters-svg"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9a81d2759aae1dae668f783c308bc5c8ebd191ff4184aaa1b37f65a6ae5a56f"
+checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
 name = "png"
 version = "0.17.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "59871cc5b6cce7eaccca5a802b4173377a1c2ba90654246789a8fa2334426d11"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "crc32fast",
  "fdeflate",
  "flate2",
- "miniz_oxide 0.7.1",
+ "miniz_oxide",
 ]
 
 [[package]]
 name = "poly1305"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8159bd90725d2df49889a078b54f4f79e87f1f8a8444194cdca81d38f5393abf"
@@ -1593,14 +1605,24 @@
 [[package]]
 name = "pretty-hex"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa0831dd7cc608c38a5e323422a0077678fa5744aa2be4ad91c4ece8eec8d5"
 
 [[package]]
+name = "prettyplease"
+version = "0.1.25"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c8646e95016a7a6c4adea95bafa8a16baab64b583356217f2c85db4a39d9a86"
+dependencies = [
+ "proc-macro2",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
@@ -1618,17 +1640,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
 version = "0.11.9"
@@ -1636,14 +1658,36 @@
 checksum = "0b82eaa1d779e9a4bc1c3217db8ffbeabaae1dca241bf70183242128d48681cd"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
+name = "prost-build"
+version = "0.11.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "119533552c9a7ffacc21e099c24a0ac8bb19c2a2a3f363de84cd9b844feab270"
+dependencies = [
+ "bytes",
+ "heck",
+ "itertools",
+ "lazy_static",
+ "log",
+ "multimap",
+ "petgraph",
+ "prettyplease",
+ "prost",
+ "prost-types",
+ "regex",
+ "syn 1.0.109",
+ "tempfile",
+ "which",
+]
+
+[[package]]
 name = "prost-derive"
 version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
 dependencies = [
  "anyhow",
  "itertools",
@@ -1658,14 +1702,64 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "213622a1460818959ac1181aaeb2dc9c7f63df720db7d788b3e24eacd1983e13"
 dependencies = [
  "prost",
 ]
 
 [[package]]
+name = "protoc-bin-vendored"
+version = "3.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "005ca8623e5633e298ad1f917d8be0a44bcf406bf3cde3b80e63003e49a3f27d"
+dependencies = [
+ "protoc-bin-vendored-linux-aarch_64",
+ "protoc-bin-vendored-linux-ppcle_64",
+ "protoc-bin-vendored-linux-x86_32",
+ "protoc-bin-vendored-linux-x86_64",
+ "protoc-bin-vendored-macos-x86_64",
+ "protoc-bin-vendored-win32",
+]
+
+[[package]]
+name = "protoc-bin-vendored-linux-aarch_64"
+version = "3.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8fb9fc9cce84c8694b6ea01cc6296617b288b703719b725b8c9c65f7c5874435"
+
+[[package]]
+name = "protoc-bin-vendored-linux-ppcle_64"
+version = "3.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02d2a07dcf7173a04d49974930ccbfb7fd4d74df30ecfc8762cf2f895a094516"
+
+[[package]]
+name = "protoc-bin-vendored-linux-x86_32"
+version = "3.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d54fef0b04fcacba64d1d80eed74a20356d96847da8497a59b0a0a436c9165b0"
+
+[[package]]
+name = "protoc-bin-vendored-linux-x86_64"
+version = "3.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8782f2ce7d43a9a5c74ea4936f001e9e8442205c244f7a3d4286bd4c37bc924"
+
+[[package]]
+name = "protoc-bin-vendored-macos-x86_64"
+version = "3.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b5de656c7ee83f08e0ae5b81792ccfdc1d04e7876b1d9a38e6876a9e09e02537"
+
+[[package]]
+name = "protoc-bin-vendored-win32"
+version = "3.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9653c3ed92974e34c5a6e0a510864dab979760481714c172e0a34e437cb98804"
+
+[[package]]
 name = "pyo3"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "anyhow",
  "cfg-if",
@@ -1710,17 +1804,17 @@
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c94ff6535a6bae58d7d0b85e60d4c53f7f84d0d0aa35d6a28c3f3e70bfe51444"
+checksum = "f47b0777feb17f61eea78667d61103758b243a871edc09a7786500a50467b605"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
@@ -1753,58 +1847,49 @@
 checksum = "7f6d64c71eb498fe9eae14ce4ec935c555749aef511cca85b5568910d6e48001"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.28"
+version = "1.0.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
+checksum = "5fe8a65d69dd0808184ebb5f836ab526bb259db23c657efa38711b1072ee47f0"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
 dependencies = [
  "libc",
  "rand_chacha",
- "rand_core 0.6.4",
+ "rand_core",
 ]
 
 [[package]]
 name = "rand_chacha"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
 dependencies = [
  "ppv-lite86",
- "rand_core 0.6.4",
-]
-
-[[package]]
-name = "rand_core"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90bde5296fc891b0cef12a6d03ddccc162ce7b2aff54160af9338f8d40df6d19"
-dependencies = [
- "getrandom 0.1.16",
+ "rand_core",
 ]
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
- "getrandom 0.2.10",
+ "getrandom",
 ]
 
 [[package]]
 name = "rayon"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
@@ -1827,48 +1912,60 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.4"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
+checksum = "b2eae68fc220f7cf2532e4494aded17545fce192d59cd996e0fe7887f4ceb575"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.7.2",
+ "regex-automata 0.3.3",
+ "regex-syntax 0.7.4",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
  "regex-syntax 0.6.29",
 ]
 
 [[package]]
+name = "regex-automata"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-syntax 0.7.4",
+]
+
+[[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.2"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "ring"
 version = "0.16.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
 dependencies = [
@@ -1894,84 +1991,97 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.20"
+version = "0.37.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
+checksum = "4d69718bf81c6127a49dc64e44a742e8bb9213c0ff8869a22c308f84c1d4ab06"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
- "linux-raw-sys",
+ "linux-raw-sys 0.3.8",
+ "windows-sys",
+]
+
+[[package]]
+name = "rustix"
+version = "0.38.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0a962918ea88d644592894bc6dc55acc6c0956488adcebbfb6e273506b7fd6e5"
+dependencies = [
+ "bitflags 2.3.3",
+ "errno",
+ "libc",
+ "linux-raw-sys 0.4.3",
  "windows-sys",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.12"
+version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
+checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
-version = "1.0.13"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
+checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+checksum = "b0293b4b29daaf487284529cc2f5675b8e57c61f70167ba415a463651fd6a918"
 
 [[package]]
 name = "serde"
-version = "1.0.164"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
+checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.164"
+version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
+checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.103"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "d03b412469450d4404fe8499a268edd7f8b79fecb074b0d812ad64ca21f4031b"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1996,24 +2106,25 @@
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
 
 [[package]]
 name = "smoltcp"
-version = "0.9.1"
-source = "git+https://github.com/mhils/smoltcp?rev=f65351adfa92db5193f368368cb668bac721fe43#f65351adfa92db5193f368368cb668bac721fe43"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8d2e3a36ac8fea7b94e666dfa3871063d6e0a5c9d5d4fec9a1a6b7b6760f0229"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "byteorder",
  "cfg-if",
  "defmt",
  "heapless",
  "libc",
  "log",
  "managed",
@@ -2065,68 +2176,76 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
+
+[[package]]
+name = "tempfile"
+version = "3.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
+dependencies = [
+ "autocfg",
+ "cfg-if",
+ "fastrand",
+ "redox_syscall",
+ "rustix 0.37.23",
+ "windows-sys",
+]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
-name = "textwrap"
-version = "0.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
-
-[[package]]
 name = "thiserror"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+checksum = "a35fc5b8971143ca348fa6df4f024d4d55264f3468c71ad1c2f365b0a4d58c42"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.40"
+version = "1.0.43"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+checksum = "463fe12d7993d3b327787537ce8dd4dfa058de32fc2b195ef3cde03dc4771e8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
@@ -2154,19 +2273,20 @@
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.28.2"
+version = "1.29.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
+checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
+ "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
@@ -2188,15 +2308,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
@@ -2299,21 +2419,21 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.24"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
+checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -2347,17 +2467,17 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -2392,47 +2512,34 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
-name = "virtue"
-version = "0.0.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9dcc60c0624df774c82a0ef104151231d37da4962957d691c011c852b2473314"
-
-[[package]]
 name = "walkdir"
 version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
- "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
-version = "0.9.0+wasi-snapshot-preview1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cccddf32554fecc6acb585f82a32a72e28b48f8c4c1883ddfeeeaa96f7d8e519"
-
-[[package]]
-name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
 version = "0.2.87"
@@ -2450,15 +2557,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2472,15 +2579,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
@@ -2500,14 +2607,25 @@
 [[package]]
 name = "weezl"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9193164d4de03a926d909d3bc7c30543cecb35400c02114792c2cae20d5e2dbb"
 
 [[package]]
+name = "which"
+version = "4.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2441c784c52b289a054b7201fc93253e288f094e2f4be9058343127c4226a269"
+dependencies = [
+ "either",
+ "libc",
+ "once_cell",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -2532,71 +2650,56 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windivert"
-version = "0.5.5"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "697021beae81b1bc48ff5492bdb93bd38475bc27b587b2589334dff674775df0"
+checksum = "fc6b6833a760d1c36b489314a5541a12a39d162dc8341d8f6f400212b96d3df1"
 dependencies = [
  "etherparse",
  "thiserror",
  "windivert-sys",
- "windows 0.43.0",
+ "windows",
 ]
 
 [[package]]
 name = "windivert-sys"
-version = "0.9.3"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "779ea0aef29d77f02df94ca639ba00ee287b563e2a388ca894e4201797d92366"
+checksum = "832bc4af9272458a8a64395b3aabe10dc4089546486fcbd0e19b9b6d28ba6e54"
 dependencies = [
  "cc",
  "thiserror",
- "windows 0.43.0",
-]
-
-[[package]]
-name = "windows"
-version = "0.43.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04662ed0e3e5630dfa9b26e4cb823b817f1a9addda855d973a9458c236556244"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows",
 ]
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-redirector"
-version = "0.2.0-beta.9"
+version = "0.2.1"
 dependencies = [
  "anyhow",
- "bincode",
  "env_logger",
  "hex",
  "internet-packet",
  "log",
  "lru_time_cache",
  "mitmproxy",
+ "prost",
  "tokio",
  "windivert",
  "winres",
 ]
 
 [[package]]
 name = "windows-sys"
@@ -2605,107 +2708,65 @@
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.0"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winres"
 version = "0.1.12"
@@ -2713,20 +2774,21 @@
 checksum = "b68db261ef59e9e52806f688020631e987592bd83619edccda9c47d42cde4f6c"
 dependencies = [
  "toml",
 ]
 
 [[package]]
 name = "x25519-dalek"
-version = "2.0.0-pre.1"
+version = "2.0.0-rc.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5da623d8af10a62342bcbbb230e33e58a63255a58012f8653c578e54bab48df"
+checksum = "ec7fae07da688e17059d5886712c933bb0520f15eff2e09cfa18e30968f4e63a"
 dependencies = [
  "curve25519-dalek",
- "rand_core 0.6.4",
+ "rand_core",
+ "serde",
  "zeroize",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2739,15 +2801,15 @@
 name = "zeroize_derive"
 version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce36e65b0d2999d2aafac989fb249189a141aee1f53c612c1f37d72631959f69"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "zune-inflate"
 version = "0.2.54"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73ab332fe2f6680068f3582b16a24f90ad7096d5d39b974d1c0aff0125116f02"
```

### Comparing `mitmproxy_rs-0.2.0b9/PKG-INFO` & `mitmproxy_rs-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitmproxy_rs
-Version: 0.2.0b9
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

