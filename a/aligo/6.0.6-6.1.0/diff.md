# Comparing `tmp/aligo-6.0.6.tar.gz` & `tmp/aligo-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligo-6.0.6.tar", last modified: Sun Jul 16 13:43:55 2023, max compression
+gzip compressed data, was "aligo-6.1.0.tar", last modified: Sat Aug  5 04:57:44 2023, max compression
```

## Comparing `aligo-6.0.6.tar` & `aligo-6.1.0.tar`

### file list

```diff
@@ -1,214 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.846749 aligo-6.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-16 13:43:49.000000 aligo-6.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-16 13:43:55.846749 aligo-6.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-07-16 13:43:49.000000 aligo-6.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-16 13:43:49.000000 aligo-6.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-16 13:43:49.000000 aligo-6.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 13:43:55.846749 aligo-6.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.822749 aligo-6.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.822749 aligo-6.0.6/src/aligo/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.826749 aligo-6.0.6/src/aligo/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Album.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Aligo.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/CustomShare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Download.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Move.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Search.py
--rw-r--r--   0 runner    (1001) docker     (123)    23234 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Share.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Star.py
--rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/SyncFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/Video.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.830749 aligo-6.0.6/src/aligo/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Album.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/BaseAligo.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/EMail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/LoginServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Move.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Share.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Star.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Template.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/User.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/Video.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.830749 aligo-6.0.6/src/aligo/error/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.834749 aligo-6.0.6/src/aligo/request/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/AimSearchRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/AlbumListFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/AlbumListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/ArchiveStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/ArchiveUncompressRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchCancelShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchCopyFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchGetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchMoveFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchMoveToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchRestoreRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchStarFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/BatchSubRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CancelShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CompleteFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CopyFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CreateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CreateFolderRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/CreateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetAudioPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetDefaultDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetFilePathRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetRecycleBinListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareLinkDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareLinkListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetShareTokenRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetStarredListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetUploadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetVideoPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/ListToCleanRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/MoveFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/MoveFileToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/PrivateShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/RenameFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/RestoreFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/SearchFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/SearchShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/ShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/StarredFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/TemplateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/UpdateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/UpdateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.838749 aligo-6.0.6/src/aligo/response/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/AimSearchResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/AlbumInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/AlbumListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ArchiveStatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ArchiveUncompressResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/BatchDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/BatchShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/BatchSubResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/CancelShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/CopyFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/CreateFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/CreateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/DuplicateListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetAudioPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetFilePathResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetOfficePreviewUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetPersonalInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetRecycleBinListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetShareFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetShareInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetShareLinkDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetShareLinkListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetShareTokenResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetStarredListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetUploadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetVideoPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ListMyDrivesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ListToCleanResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/MoveFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/MoveFileToTrashResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/PrivateShareResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/RestoreFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/RewardSpaceResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/SearchFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/SearchShareFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ShareItemInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/ShareLinkExtractCodeResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/TemplateResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/UpdateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/UsersVipInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.846749 aligo-6.0.6/src/aligo/types/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/AudioMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/AudioMusicMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/AudioTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/BaseAlbum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/BaseDrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/BaseFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/BaseShareFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/BaseUser.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/CroppingBoundary.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/CroppingSuggestionItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/DataClass.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/DriveCapacityDetail.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/DriveFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/EMailConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/Enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/FaceThumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/FieldsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/FolderSizeInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ImageMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ImageQuality.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ImageTag.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ListAlbumItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/LoginDevice.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/LoginTimout.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/MediaTransCodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/Null.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/PersonalRightsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/PersonalSpaceInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/Privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/RateLimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ShareLinkBaseFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/ShareLinkSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/SystemTag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/UploadPartInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoMediaAudioStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoMediaVideoStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoPreview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoPreviewPlayInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoPreviewSprite.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/VideoTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-16 13:43:49.000000 aligo-6.0.6/src/aligo/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:43:55.822749 aligo-6.0.6/src/aligo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 13:43:55.000000 aligo-6.0.6/src/aligo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.390127 aligo-6.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-05 04:57:36.000000 aligo-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-08-05 04:57:44.390127 aligo-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-08-05 04:57:36.000000 aligo-6.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-05 04:57:36.000000 aligo-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-05 04:57:36.000000 aligo-6.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 04:57:44.390127 aligo-6.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.358125 aligo-6.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.358125 aligo-6.1.0/src/aligo/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-05 04:57:43.000000 aligo-6.1.0/src/aligo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.362125 aligo-6.1.0/src/aligo/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Aligo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/CustomShare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23334 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Star.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/SyncFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.366125 aligo-6.1.0/src/aligo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Album.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19955 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/BaseAligo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12900 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/EMail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/LoginServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Move.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.366125 aligo-6.1.0/src/aligo/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.374126 aligo-6.1.0/src/aligo/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/AimSearchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/AlbumListFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/AlbumListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/ArchiveStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/ArchiveUncompressRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchCancelShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchCopyFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchGetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchMoveFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchMoveToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchRestoreRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchStarFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/BatchSubRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/CancelShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/CompleteFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/CopyFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/CreateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/CreateFolderRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/CreateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetAudioPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetDefaultDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetFilePathRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetRecycleBinListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetShareFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetShareInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetShareLinkDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetShareLinkListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetShareTokenRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetStarredListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetUploadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetVideoPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/ListToCleanRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/MoveFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/MoveFileToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/PrivateShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/RenameFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/RestoreFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/SearchFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/SearchShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/ShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/StarredFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/TemplateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/UpdateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/UpdateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.382126 aligo-6.1.0/src/aligo/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/AimSearchResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/AlbumInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/AlbumListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/ArchiveStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/ArchiveUncompressResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/BatchDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/BatchShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/BatchSubResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/CancelShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/CopyFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/CreateFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/CreateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/DuplicateListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetAudioPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetFilePathResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetOfficePreviewUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetPersonalInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetRecycleBinListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetShareFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetShareInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetShareLinkDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetShareLinkListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetShareTokenResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetStarredListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetUploadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetVideoPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/ListMyDrivesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/ListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/ListToCleanResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/MoveFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/MoveFileToTrashResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/PrivateShareResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/RestoreFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/RewardSpaceResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/SearchFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/SearchShareFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/ShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/ShareItemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/ShareLinkExtractCodeResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/TemplateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/UpdateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/UsersVipInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.386127 aligo-6.1.0/src/aligo/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/AudioMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/AudioMusicMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/AudioTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/BaseAlbum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/BaseDrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/BaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/BaseShareFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/BaseUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/CroppingBoundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/CroppingSuggestionItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/DriveCapacityDetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/DriveFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/EMailConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/Enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/FaceThumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/FieldsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/FolderSizeInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/ImageMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/ImageQuality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/ImageTag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/ListAlbumItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/LoginDevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/MediaTransCodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/Null.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/PersonalRightsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/PersonalSpaceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/Privilege.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/RateLimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/ShareLinkBaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/ShareLinkSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/SystemTag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/Type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/UploadPartInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/VideoMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/VideoMediaAudioStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/VideoMediaVideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/VideoPreview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/VideoPreviewPlayInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/VideoPreviewSprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/VideoTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.390127 aligo-6.1.0/src/aligo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/utils/LoginTimout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:36.000000 aligo-6.1.0/src/aligo/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 04:57:44.358125 aligo-6.1.0/src/aligo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-08-05 04:57:44.000000 aligo-6.1.0/src/aligo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-05 04:57:44.000000 aligo-6.1.0/src/aligo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 04:57:44.000000 aligo-6.1.0/src/aligo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-05 04:57:44.000000 aligo-6.1.0/src/aligo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 04:57:44.000000 aligo-6.1.0/src/aligo.egg-info/top_level.txt
```

### Comparing `aligo-6.0.6/LICENSE` & `aligo-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aligo-6.0.6/PKG-INFO` & `aligo-6.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.0.6
+Version: 6.1.0
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
@@ -115,14 +115,29 @@
 ```
 
 ## 如何彻底删除文件？
 > 无需先移动文件到回收站
 
 此功能太危险，**aligo** 未直接提供。不过 [这里](https://github.com/foyoux/aligo/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E5%8A%9F%E8%83%BD---%E5%BD%BB%E5%BA%95%E5%88%A0%E9%99%A4%E6%96%87%E4%BB%B6) 扩展了该功能，请小心使用！
 
+## 如何操作资源盘
+
+```python
+from aligo import Aligo
+
+if __name__ == '__main__':
+    ali = Aligo()
+    drives = ali.list_my_drives()
+    resource_drive_id = [drive.drive_id for drive in drives if drive.drive_name == 'resource'][0]
+    ll = ali.get_file_list(drive_id=resource_drive_id)
+    for i in ll:
+        print(i)
+
+```
+
 
 ## 关于扩展功能
 
 一般步骤：
 
     1. 使用浏览器或其他抓包工具，观察通信过程；
     2. 获取 url/path + 请求体；
```

### Comparing `aligo-6.0.6/README.md` & `aligo-6.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -95,14 +95,29 @@
 ```
 
 ## 如何彻底删除文件？
 > 无需先移动文件到回收站
 
 此功能太危险，**aligo** 未直接提供。不过 [这里](https://github.com/foyoux/aligo/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E5%8A%9F%E8%83%BD---%E5%BD%BB%E5%BA%95%E5%88%A0%E9%99%A4%E6%96%87%E4%BB%B6) 扩展了该功能，请小心使用！
 
+## 如何操作资源盘
+
+```python
+from aligo import Aligo
+
+if __name__ == '__main__':
+    ali = Aligo()
+    drives = ali.list_my_drives()
+    resource_drive_id = [drive.drive_id for drive in drives if drive.drive_name == 'resource'][0]
+    ll = ali.get_file_list(drive_id=resource_drive_id)
+    for i in ll:
+        print(i)
+
+```
+
 
 ## 关于扩展功能
 
 一般步骤：
 
     1. 使用浏览器或其他抓包工具，观察通信过程；
     2. 获取 url/path + 请求体；
```

### Comparing `aligo-6.0.6/pyproject.toml` & `aligo-6.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aligo-6.0.6/src/aligo/apis/Album.py` & `aligo-6.1.0/src/aligo/apis/Album.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """..."""
 from typing import List, Union
 
-from aligo.core import *
-from aligo.core.Config import *
+from aligo.core import Core
+from aligo.core.Config import (ADRIVE_V1_ALBUM_GET, ADRIVE_V1_ALBUM_CREATE, ADRIVE_V1_ALBUM_DELETE,
+                               ADRIVE_V1_ALBUM_ADD_FILES, ADRIVE_V1_ALBUM_UPDATE)
 from aligo.request import AlbumListRequest, AlbumListFilesRequest
 from aligo.types import ListAlbumItem, BaseAlbum, BaseFile
-from aligo.types.Enum import *
+from aligo.types.Enum import GetShareLinkListOrderBy, OrderDirection
 
 
 class Album(Core):
     """..."""
 
     def list_albums(
             self, album_drive_id: str = None,
@@ -23,42 +24,42 @@
             album_drive_id=album_drive_id, drive_id=drive_id,
             order_by=order_by, order_direction=order_direction
         )
         return list(self._core_list_album(body))
 
     def delete_album(self, album_id: str) -> bool:
         """删除 album"""
-        response = self._post(ADRIVE_V1_ALBUM_DELETE, body={'album_id': album_id})
+        response = self.post(ADRIVE_V1_ALBUM_DELETE, body={'album_id': album_id})
         return response.status_code == 200
 
     def create_album(self, name: str, description: str = None) -> BaseAlbum:
         """创建 album"""
-        response = self._post(ADRIVE_V1_ALBUM_CREATE, body={
+        response = self.post(ADRIVE_V1_ALBUM_CREATE, body={
             'name': name,
             'description': description
         })
         return self._result(response, BaseAlbum)
 
     def get_album(self, album_id: str) -> BaseAlbum:
         """获取相册，通过 album_id"""
-        response = self._post(ADRIVE_V1_ALBUM_GET, body={'album_id': album_id})
+        response = self.post(ADRIVE_V1_ALBUM_GET, body={'album_id': album_id})
         return self._result(response, BaseAlbum)
 
     def add_files_to_album(self, album_id: str, files: List[Union[BaseFile, str]]) -> List[BaseFile]:
-        response = self._post(ADRIVE_V1_ALBUM_ADD_FILES, body={
+        response = self.post(ADRIVE_V1_ALBUM_ADD_FILES, body={
             'album_id': album_id,
             'drive_file_list': [{'drive_id': f.drive_id, 'file_id': f.file_id} for f in files]
         })
         return self._result(response, BaseFile, field='file_list')
 
     def list_album_files(self, album_id: str, order_direction: OrderDirection = 'DESC') -> List[BaseFile]:
         """获取指定相册文件"""
         body = AlbumListFilesRequest(album_id=album_id, order_direction=order_direction)
         result = self._core_list_album_files(body)
         return list(result)
 
     def rename_album(self, album_id: str, name: str):
-        response = self._post(ADRIVE_V1_ALBUM_UPDATE, body={
+        response = self.post(ADRIVE_V1_ALBUM_UPDATE, body={
             'album_id': album_id,
             'name': name
         })
         return self._result(response, BaseAlbum)
```

### Comparing `aligo-6.0.6/src/aligo/apis/Aligo.py` & `aligo-6.1.0/src/aligo/apis/Aligo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""Aligo class"""
+"""..."""
 import json
 import logging
 from typing import Callable, Dict
 
+from aligo.core import aligo_config_folder
+from aligo.types import EMailConfig
 from .Album import Album
 from .Audio import Audio
 from .Compress import Compress
 from .Copy import Copy
-from .Copy import aligo_config_folder
 from .Create import Create
 from .CustomShare import CustomShare
 from .Download import Download
 from .Drive import Drive
 from .Duplicate import Duplicate
 from .File import File
 from .Move import Move
@@ -19,15 +20,14 @@
 from .Recyclebin import Recyclebin
 from .Search import Search
 from .Share import Share
 from .Star import Star
 from .SyncFolder import SyncFolder
 from .Update import Update
 from .Video import Video
-from aligo.types import EMailConfig
 
 
 class Aligo(
     Audio,
     Album,
     Compress,
     Copy,
```

### Comparing `aligo-6.0.6/src/aligo/apis/Audio.py` & `aligo-6.1.0/src/aligo/apis/Audio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-"""Audio class"""
-
-from aligo.core import *
-from aligo.request import *
-from aligo.response import *
+"""..."""
+from aligo.core import Core
+from aligo.request import GetAudioPlayInfoRequest
+from aligo.response import GetAudioPlayInfoResponse
 
 
 class Audio(Core):
     """音频相关"""
 
     def get_audio_play_info(self, file_id: str, drive_id: str = None) -> GetAudioPlayInfoResponse:
         """
```

### Comparing `aligo-6.0.6/src/aligo/apis/Compress.py` & `aligo-6.1.0/src/aligo/apis/Compress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """..."""
-
 from aligo.core import Core
 from aligo.request import ArchiveUncompressRequest, ArchiveStatusRequest
 from aligo.response import ArchiveUncompressResponse, ArchiveStatusResponse
 from aligo.types.Enum import ArchiveType
 
 
 class Compress(Core):
```

### Comparing `aligo-6.0.6/src/aligo/apis/Copy.py` & `aligo-6.1.0/src/aligo/apis/Copy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""Copy class"""
+"""..."""
 from typing import List, overload
 
-from aligo.core import *
-from aligo.request import *
-from aligo.response import *
+from aligo.core import Core
+from aligo.request import CopyFileRequest, BatchCopyFilesRequest
+from aligo.response import CopyFileResponse, BatchSubResponse
 
 
 class Copy(Core):
     """复制文件相关
     说明：官方虽然提供文件（夹）复制接口，但并未公开文件（夹）复制的功能。
         所以后期可能会失效，不过有替代方案，如果此接口失效我会补上。
     """
```

### Comparing `aligo-6.0.6/src/aligo/apis/Create.py` & `aligo-6.1.0/src/aligo/apis/Create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""Create class"""
+"""..."""
 import os
 from typing import List, Callable
 
-from aligo.core import *
-from aligo.request import *
-from aligo.response import *
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.core import Core
+from aligo.request import CreateFolderRequest
+from aligo.response import CreateFileResponse
+from aligo.types import BaseFile
+from aligo.types.Enum import CheckNameMode
 
 
 class Create(Core):
     """创建上传文件相关"""
 
     def create_folder(self,
                       name: str,
```

### Comparing `aligo-6.0.6/src/aligo/apis/CustomShare.py` & `aligo-6.1.0/src/aligo/apis/CustomShare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """自定义分享"""
 import base64
 import json
 from typing import List, Dict
 
-from aligo.core import *
-from aligo.request import *
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.core import Core
+from aligo.request import GetFileListRequest, GetFileRequest, CreateFolderRequest
+from aligo.types import BaseFile
+from aligo.types.Enum import CheckNameMode
 
 
 class CustomShare(Core):
     """..."""
 
     _ALIGO_SHARE_SCHEMA = 'aligo://'
```

### Comparing `aligo-6.0.6/src/aligo/apis/Download.py` & `aligo-6.1.0/src/aligo/apis/Download.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """..."""
 import os
 from typing import List, overload, Callable
 
-from aligo.core import *
+from aligo.core import Core
 from aligo.error import AligoException
-from aligo.request import *
-from aligo.response import *
-from aligo.types import *
+from aligo.request import GetFileRequest, GetFileListRequest, GetDownloadUrlRequest, BatchDownloadUrlRequest
+from aligo.response import GetDownloadUrlResponse, BatchDownloadUrlResponse
+from aligo.types import BaseFile
 
 
 class Download(Core):
     """..."""
 
     def get_download_url(self,
                          file_id: str,
```

### Comparing `aligo-6.0.6/src/aligo/apis/Drive.py` & `aligo-6.1.0/src/aligo/apis/Drive.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """drive"""
-
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.types import *
+from aligo.core import Core
+from aligo.core.Config import ADRIVE_V1_USER_DRIVECAPACITY_DETAILS
+from aligo.request import GetDriveRequest
+from aligo.types import BaseDrive, DriveCapacityDetail
 
 
 class Drive(Core):
     """..."""
 
     def get_drive(self, drive_id: str = None) -> BaseDrive:
         """
@@ -22,9 +21,9 @@
         >>> print(result)
         """
         body = GetDriveRequest(drive_id=drive_id)
         return self._core_get_drive(body)
 
     def drive_capacity_details(self) -> DriveCapacityDetail:
         """获取网盘容量详细信息"""
-        response = self._post(ADRIVE_V1_USER_DRIVECAPACITY_DETAILS)
+        response = self.post(ADRIVE_V1_USER_DRIVECAPACITY_DETAILS)
         return self._result(response, DriveCapacityDetail)
```

### Comparing `aligo-6.0.6/src/aligo/apis/Duplicate.py` & `aligo-6.1.0/src/aligo/apis/Duplicate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """..."""
 import itertools
 from typing import List
 
-from aligo.core import *
-from aligo.request import *
-from aligo.response import *
+from aligo.core import Core
+from aligo.request import ListToCleanRequest
+from aligo.response import DuplicateItem
 from aligo.types import BaseFile
 
 
 class Duplicate(Core):
     """..."""
 
     def duplicate_list(self, drive_id: str = None) -> List[DuplicateItem]:
```

### Comparing `aligo-6.0.6/src/aligo/apis/File.py` & `aligo-6.1.0/src/aligo/apis/File.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """文件相关"""
 import os
 from typing import List, overload, Union, Callable
 
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
+from aligo.core import Core
+from aligo.core.Config import ADRIVE_V1_FILE_GET_FOLDER_SIZE_INFO
+from aligo.request import GetFileRequest, GetFileListRequest, BatchGetFileRequest, CreateFolderRequest
 from aligo.response import *
 from aligo.types import *
 from aligo.types.Enum import *
 
 
 class File(Core):
     """..."""
@@ -221,9 +221,9 @@
             if f.type == 'file':
                 callback(_path, f)
                 continue
             self.walk_files(callback, parent_file_id=f.file_id, drive_id=drive_id, _path=os.path.join(_path, f.name))
 
     def get_folder_size_info(self, file_id: str, drive_id: str = None) -> FolderSizeInfo:
         """获取文件夹信息，文件夹个数，以及文件个数及其大小，不递归"""
-        response = self._post(ADRIVE_V1_FILE_GET_FOLDER_SIZE_INFO, body={'file_id': file_id, 'drive_id': drive_id})
+        response = self.post(ADRIVE_V1_FILE_GET_FOLDER_SIZE_INFO, body={'file_id': file_id, 'drive_id': drive_id})
         return self._result(response, FolderSizeInfo)
```

### Comparing `aligo-6.0.6/src/aligo/apis/Move.py` & `aligo-6.1.0/src/aligo/apis/Move.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """..."""
 from typing import List, overload
 
-from aligo.core import *
-from aligo.request import *
-from aligo.response import *
+from aligo.core import Core
+from aligo.request import MoveFileRequest, BatchMoveFilesRequest
+from aligo.response import MoveFileResponse, BatchSubResponse
 
 
 class Move(Core):
     """..."""
 
     @overload
     def move_file(self, file_id: str,
```

### Comparing `aligo-6.0.6/src/aligo/apis/Other.py` & `aligo-6.1.0/src/aligo/apis/Other.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Other"""
-
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.response import *
+from aligo.core import Core
+from aligo.core.Config import V2_FILE_GET_OFFICE_PREVIEW_URL
+from aligo.request import GetFilePathRequest
+from aligo.response import GetFilePathResponse, GetOfficePreviewUrlResponse
 
 
 class Other(Core):
     """Other"""
 
     def get_path(self, file_id: str, drive_id: str = None) -> GetFilePathResponse:
         """
@@ -24,12 +23,12 @@
         >>> for item in file_path_info.items:
         >>>     assert isinstance(item, BaseFile)
         """
         body = GetFilePathRequest(file_id=file_id, drive_id=drive_id)
         return self._core_get_path(body)
 
     def get_office_preview_url(self, file_id: str, drive_id: str = None):
-        response = self._post(V2_FILE_GET_OFFICE_PREVIEW_URL, body={
+        response = self.post(V2_FILE_GET_OFFICE_PREVIEW_URL, body={
             'file_id': file_id,
             'drive_id': drive_id
         })
         return self._result(response, GetOfficePreviewUrlResponse)
```

### Comparing `aligo-6.0.6/src/aligo/apis/Recyclebin.py` & `aligo-6.1.0/src/aligo/apis/Recyclebin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""Recyclebin class"""
+"""..."""
 from typing import List, overload
 
-from aligo.core import *
-from aligo.request import *
-from aligo.response import *
-from aligo.types import *
+from aligo.core import Core
+from aligo.request import (RestoreFileRequest, GetRecycleBinListRequest, MoveFileToTrashRequest,
+                           BatchMoveToTrashRequest, BatchRestoreRequest)
+from aligo.response import MoveFileToTrashResponse, BatchSubResponse, RestoreFileResponse
+from aligo.types import BaseFile
 
 
 class Recyclebin(Core):
     """删除文件太过危险, 只提供移动文件到回收站的功能"""
 
     def move_file_to_trash(self, file_id: str, drive_id: str = None) -> MoveFileToTrashResponse:
         """
```

### Comparing `aligo-6.0.6/src/aligo/apis/Search.py` & `aligo-6.1.0/src/aligo/apis/Search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Search class"""
+"""..."""
 import warnings
 from typing import List, overload
 
-from aligo.core import *
-from aligo.request import *
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.core import Core
+from aligo.request import SearchFileRequest, AimSearchRequest
+from aligo.types import BaseFile
+from aligo.types.Enum import SearchCategory, BaseFileCategory
 
 
 class Search(Core):
     """搜索相关"""
 
     def search_file(self, *args, **kwargs):
         """请使用 search_files """
```

### Comparing `aligo-6.0.6/src/aligo/apis/Share.py` & `aligo-6.1.0/src/aligo/apis/Share.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """分享相关"""
 import warnings
 from typing import List, overload
 
-from aligo.core import *
+from aligo.core import Core
 from aligo.request import *
 from aligo.response import *
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.types import BaseShareFile, ShareLinkSchema, DriveFile
+from aligo.types.Enum import OrderDirection, SearchFileOrderBy, GetShareLinkListOrderBy
 
 
 def _deprecation_warning(kwargs):
     if 'share_id' in kwargs:
         kwargs.pop('share_id')
         warnings.warn('share 相关方法已删除 `share_id` 参数，因为 share_token 已包含了 share_id 信息',
                       DeprecationWarning, stacklevel=3)
```

### Comparing `aligo-6.0.6/src/aligo/apis/Star.py` & `aligo-6.1.0/src/aligo/apis/Star.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """收藏相关"""
 from typing import List
 
-from aligo.core import *
-from aligo.request import *
-from aligo.response import *
-from aligo.types import *
+from aligo.core import Core
+from aligo.request import StarredFileRequest, BatchStarFilesRequest, GetStarredListRequest
+from aligo.response import BatchSubResponse
+from aligo.types import BaseFile
 
 
 class Star(Core):
     """..."""
     _MAX_STAR_COUNT: int = 500
 
     def starred_file(self,
```

### Comparing `aligo-6.0.6/src/aligo/apis/SyncFolder.py` & `aligo-6.1.0/src/aligo/apis/SyncFolder.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import shutil
 from datetime import datetime
 from typing import Callable
 from typing import Dict, Union
 from typing import Optional
 
-from aligo.core import *
+from aligo.core import Core
 from aligo.request import GetFileListRequest, MoveFileToTrashRequest, CreateFolderRequest
 from aligo.types import BaseFile
 
 
 def utc_str_to_timestamp(utc: str) -> int:
     """'2022-04-16T11:07:03.276Z' -> timestamp"""
     return int(datetime.fromisoformat(utc[:-1]).timestamp()) + 28800
```

### Comparing `aligo-6.0.6/src/aligo/apis/Update.py` & `aligo-6.1.0/src/aligo/apis/Update.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """..."""
 from typing import List
 
-from aligo.core import *
-from aligo.request import *
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.core import Core
+from aligo.request import RenameFileRequest, BatchRequest, BatchSubRequest
+from aligo.types import BaseFile
+from aligo.types.Enum import CheckNameMode
 
 
 class Update(Core):
     """..."""
 
     def rename_file(self,
                     file_id: str,
```

### Comparing `aligo-6.0.6/src/aligo/apis/Video.py` & `aligo-6.1.0/src/aligo/apis/Video.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """..."""
-
-from aligo.core import *
-from aligo.request import *
-from aligo.response import *
+from aligo.core import Core
+from aligo.request import GetVideoPlayInfoRequest, GetVideoPreviewPlayInfoRequest
+from aligo.response import GetVideoPlayInfoResponse, GetVideoPreviewPlayInfoResponse
 from aligo.types.Enum import VideoTemplateID
 
 
 class Video(Core):
     """..."""
 
     def get_video_play_info(self, file_id: str, drive_id: str = None) -> GetVideoPlayInfoResponse:
```

### Comparing `aligo-6.0.6/src/aligo/core/Album.py` & `aligo-6.1.0/src/aligo/core/Album.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Iterator
 
 from aligo.core import *
 from aligo.core.Config import *
 from aligo.request import AlbumListRequest, AlbumListFilesRequest
 from aligo.response import AlbumInfoResponse, AlbumListResponse, ListResponse
-from aligo.types import DataClass, ListAlbumItem
+from aligo.types import ListAlbumItem
 
 
 class Album(BaseAligo):
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._album_info = None
 
     @property
     def album_info(self) -> AlbumInfoResponse:
         if self._album_info is None:
-            response = self._post(ADRIVE_V1_USER_ALBUMS_INFO)
+            response = self.post(ADRIVE_V1_USER_ALBUMS_INFO)
             data = response.json()['data']
-            self._album_info = DataClass.fill_attrs(AlbumInfoResponse, data)
+            self._album_info = AlbumInfoResponse(**data)
         return self._album_info
 
     def _core_list_album(self, body: AlbumListRequest) -> Iterator[ListAlbumItem]:
         yield from self._list_file(ADRIVE_V1_ALBUMHOME_ALBUMLIST, body, AlbumListResponse)
 
     def _core_list_album_files(self, body: AlbumListFilesRequest):
         yield from self._list_file(ADRIVE_V1_ALBUM_LIST_FILES, body, ListResponse)
```

### Comparing `aligo-6.0.6/src/aligo/core/Auth.py` & `aligo-6.1.0/src/aligo/core/Auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import requests
 
 import aligo
 from aligo.core.Config import *
 from aligo.error import AligoStatus500, AligoRefreshFailed, AligoFatalError, AligoShareLinkCreateExceedDailyLimit
 from aligo.types import *
 from aligo.types.Enum import *
+from aligo.utils.LoginTimout import LoginTimeout
 from .EMail import send_email
 from .LoginServer import LoginServer
 
 # 默认配置目录
 aligo_config_folder = Path.home().joinpath('.aligo')
 aligo_config_folder.mkdir(parents=True, exist_ok=True)
 
@@ -101,14 +102,30 @@
             port: int = None,
             email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
     ):
         """refresh_token 登录"""
 
+    @overload
+    def __init__(
+            self, name: str = 'aligo',
+            refresh_token: str = None,
+            show: Callable[[str], None] = None,
+            level: int = logging.DEBUG,
+            proxies: Dict = None,
+            port: int = None,
+            email: EMailConfig = None,
+            request_failed_delay: float = 3,
+            requests_timeout: float = None,
+            login_timeout: float = None,
+            re_login: bool = True,
+    ):
+        """..."""
+
     # noinspection PyPep8Naming,SpellCheckingInspection
     def __init__(
             self, name: str = 'aligo',
             refresh_token: str = None,
             show: Callable[[str], None] = None,
             level: int = logging.DEBUG,
             proxies: Dict = None,
@@ -177,15 +194,15 @@
         self.log.info(self._os_name)
         self._show = show
 
         self._x_device_id = None
 
         if self._name.exists():
             self.log.info(f'加载配置文件 {self._name}')
-            self.token = DataClass.fill_attrs(Token, json.load(self._name.open(encoding='utf8')))
+            self.token = Token(**json.load(self._name.open(encoding='utf8')))
             self.session.headers.update({
                 'Authorization': self.token.access_token,
             })
             self._init_x_headers()
         elif refresh_token is None:
             self.log.info('登录方式 扫描二维码')
             self._login()
@@ -319,15 +336,15 @@
                 'refresh_token': refresh_token,
                 'grant_type': 'refresh_token'
             }
         )
         self._log_response(response)
         if response.status_code == 200:
             self.log.info('刷新 token 成功')
-            self.token = DataClass.fill_attrs(Token, response.json())
+            self.token = Token(**response.json())
             self.session.headers.update({
                 'Authorization': self.token.access_token,
             })
             if not self._x_device_id:
                 self._init_x_headers()
             else:
                 self.token.x_device_id = self._x_device_id
```

### Comparing `aligo-6.0.6/src/aligo/core/BaseAligo.py` & `aligo-6.1.0/src/aligo/core/BaseAligo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """..."""
 import json
 import logging
 import subprocess
 import traceback
 from dataclasses import asdict, is_dataclass
-from typing import Generic, List, Iterator, Dict, Callable, Union, Type
+from typing import Generic, List, Iterator, Dict, Callable, Union
+from typing import Type, Optional
 
 import requests
 
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.response import *
-from aligo.types import *
-from aligo.types.DataClass import DataType
-from aligo.types.Enum import *
+from aligo.core import Auth
+from aligo.core.Config import API_HOST, V2_FILE_GET, V2_DATABOX_GET_PERSONAL_INFO, V3_BATCH
+from aligo.request import GetFileRequest, BatchRequest
+from aligo.response import GetPersonalInfoResponse, BatchSubResponse
+from aligo.types import DatClass, DataType, Null, EMailConfig, BaseUser, BaseDrive, BaseFile
 
 
 class BaseAligo:
     """..."""
 
     def __init__(
             self,
@@ -46,15 +45,15 @@
         :param port: (可选) 开启 http server 端口，用于网页端扫码登录. 提供此值时，将不再弹出或打印二维码
         :param email: (可选) 邮箱配置，参考 EMailConfig
         :param request_failed_delay: 请求失败后，延迟时间，单位：秒
         :param requests_timeout: same as requests timeout
         :param login_timeout: 登录超时时间，单位：秒
         :param re_login: refresh_token 失效后是否继续登录（弹出二维码或邮件，需等待） fix #73
         """
-        self._auth: Auth = Auth(  # type: ignore
+        self._auth = Auth(
             name=name,
             refresh_token=refresh_token,
             show=show,
             level=level,
             proxies=proxies,
             port=port,
             email=email,
@@ -78,35 +77,38 @@
                 self._auth.log.info('发现 aria2c, 将使用 aria2c 下载文件')
             except FileNotFoundError:
                 self._auth.log.warning('未发现 aria2c')
                 self._has_aria2c = False
         else:
             self._has_aria2c = False
 
-    def _post(
+    def post(
             self,
             path: str,
             host: str = API_HOST,
-            body: Union[DataType, Dict] = None,
+            body: Union[DatClass, Dict] = None,
             headers: dict = None,
             ignore_auth: bool = False,
             params: dict = None,
     ) -> requests.Response:
         """统一处理数据类型和 drive_id"""
         if body is None:
             body = {}
-        elif isinstance(body, DataClass):
+        elif isinstance(body, DatClass):
             body = asdict(body)
 
         if 'drive_id' in body and body['drive_id'] is None:
             # 如果存在 attr drive_id 并且它是 None，并将 default_drive_id 设置为它
             body['drive_id'] = self.default_drive_id
 
         return self._auth.post(path=path, host=host, body=body, headers=headers, ignore_auth=ignore_auth, params=params)
 
+    def _post(self, *args, **kwargs):
+        raise DeprecationWarning('请使用 post 方法')
+
     @property
     def default_drive_id(self):
         """默认 drive_id"""
         return self._auth.token.default_drive_id
 
     @property
     def default_sbox_drive_id(self):
@@ -147,25 +149,25 @@
             try:
                 # noinspection PyProtectedMember
                 d = json.loads(text)
                 if field:
                     for i in field.split('.'):
                         d = d[i]
                 if isinstance(d, list):
-                    return [DataClass.fill_attrs(cls, i) for i in d]
-                return DataClass.fill_attrs(cls, d)
+                    return [cls(**i) for i in d]
+                return cls(**d)
             except TypeError:
                 self._auth.debug_log(response)
                 self._auth.log.error(cls)
                 traceback.print_exc()
         self._auth.log.warning(f'{response.status_code} {response.text[:200]}')
         return Null(response)
 
     def _list_file(
-            self, path: str, body: Union[DataClass, Dict],
+            self, path: str, body: Union[DatClass, Dict],
             resp_type: Generic[DataType], headers: dict = None, params: dict = None) -> Iterator[DataType]:
         """
         枚举文件: 用于统一处理 1.文件列表 2.搜索文件列表 3.收藏列表 4.回收站列表
         :param path: [str] 批量处理的路径
         :param body: [DataClass] 批量处理的参数
         :param resp_type: [Callable] 响应类型
         :return: [Iterator[DataType]] 响应结果
@@ -173,38 +175,38 @@
         如何判断请求失败与否（适用于所有使用此方法的上层方法）：
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> result = ali.get_file_list('<file_id>')
         >>> if isinstance(result[-1], Null):
         >>>     print('请求失败')
         """
-        response = self._post(path, body=body, headers=headers, params=params)
+        response = self.post(path, body=body, headers=headers, params=params)
         file_list = self._result(response, resp_type)
         if isinstance(file_list, Null):
             yield file_list
             return
         yield from file_list.items
         if file_list.next_marker != '':
             if isinstance(body, dict):
                 body['marker'] = file_list.next_marker
             else:
                 body.marker = file_list.next_marker
             yield from self._list_file(path=path, body=body, resp_type=resp_type, headers=headers, params=params)
 
     def _core_get_file(self, body: GetFileRequest) -> BaseFile:
         """获取文件信息, 其他类中可能会用到, 所以放到基类中"""
-        response = self._post(V2_FILE_GET, body=body)
+        response = self.post(V2_FILE_GET, body=body)
         return self._result(response, BaseFile)
 
     def get_personal_info(self) -> GetPersonalInfoResponse:
         """
         获取个人信息
         :return: [GetPersonalInfoResponse]
         """
-        response = self._post(V2_DATABOX_GET_PERSONAL_INFO)
+        response = self.post(V2_DATABOX_GET_PERSONAL_INFO)
         return self._result(response, GetPersonalInfoResponse)
 
     _BATCH_COUNT = 100
 
     @staticmethod
     def _list_split(ll: List[DataType], n: int) -> List[List[DataType]]:
         rt = []
@@ -223,15 +225,15 @@
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> result = ali.batch_get_files(['<file1_id>', '<file2_id>'])
         >>> if isinstance(result[-1], Null):
         >>>     print('请求失败')
         """
         for request_list in self._list_split(body.requests, self._BATCH_COUNT):
-            response = self._post(V3_BATCH, body={
+            response = self.post(V3_BATCH, body={
                 "requests": [
                     {
                         "body": asdict(request.body) if is_dataclass(request.body) else request.body,
                         "headers": request.headers,
                         "id": request.id,
                         "method": request.method,
                         "url": request.url
@@ -241,22 +243,22 @@
             })
 
             if response.status_code != 200:
                 yield Null(response)
                 return
 
             for batch in response.json()['responses']:
-                i = DataClass.fill_attrs(BatchSubResponse, batch)
+                i = BatchSubResponse(**batch)
                 if i.body:
                     try:
                         # 不是都会成功
                         # eg: {
                         #       'code': 'AlreadyExist.File',
                         #       'message': "The resource file has already exists. drive has the same file,
                         #                   can't update, file_id 609887cca951bf4feca54c6ebd0a91a03b826949"
                         # }
                         # status 409
-                        i.body = DataClass.fill_attrs(body_type, i.body)
+                        i.body = body_type(**i.body)
                     except TypeError:
                         # self._auth.log.warning(i)
                         pass
                 yield i
```

### Comparing `aligo-6.0.6/src/aligo/core/Compress.py` & `aligo-6.1.0/src/aligo/core/Compress.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 class Compress(BaseAligo):
     """..."""
 
     def _core_archive_uncompress(self, body: ArchiveUncompressRequest) -> ArchiveUncompressResponse:
         """新建在线解压缩任务"""
         if body.target_drive_id is None:
             body.target_drive_id = self.default_drive_id
-        response = self._post(V2_ARCHIVE_UNCOMPRESS, body=body)
+        response = self.post(V2_ARCHIVE_UNCOMPRESS, body=body)
         return self._result(response, ArchiveUncompressResponse, status_code=202)
 
     def _core_archive_status(self, body: ArchiveStatusRequest) -> ArchiveStatusResponse:
         """获取在线解压缩任务状态"""
-        response = self._post(V2_ARCHIVE_STATUS, body=body)
+        response = self.post(V2_ARCHIVE_STATUS, body=body)
         return self._result(response, ArchiveStatusResponse)
```

### Comparing `aligo-6.0.6/src/aligo/core/Config.py` & `aligo-6.1.0/src/aligo/core/Config.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.6/src/aligo/core/Copy.py` & `aligo-6.1.0/src/aligo/core/Copy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """..."""
 from typing import Iterator
 
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.response import *
+from aligo.core import BaseAligo
+from aligo.core.Config import V2_FILE_COPY
+from aligo.request import BatchCopyFilesRequest, CopyFileRequest, BatchRequest, BatchSubRequest
+from aligo.response import BatchSubResponse, CopyFileResponse
 
 
 class Copy(BaseAligo):
     """..."""
 
     def _core_copy_file(self, body: CopyFileRequest) -> CopyFileResponse:
         """..."""
-        response = self._post(V2_FILE_COPY, body=body)
+        response = self.post(V2_FILE_COPY, body=body)
         return self._result(response, CopyFileResponse, [201, 202])
 
     def _core_batch_copy_files(self, body: BatchCopyFilesRequest) -> Iterator[BatchSubResponse[CopyFileResponse]]:
         """..."""
         if body.drive_id is None:
             body.drive_id = self.default_drive_id
```

### Comparing `aligo-6.0.6/src/aligo/core/Core.py` & `aligo-6.1.0/src/aligo/core/Core.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.6/src/aligo/core/Create.py` & `aligo-6.1.0/src/aligo/core/Create.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from dataclasses import asdict
 from typing import Union, List
 
 import requests.exceptions
 from tqdm import tqdm
 
-from aligo.core import *
+from aligo.core import BaseAligo
 from aligo.core.Config import *
 from aligo.request import *
 from aligo.response import *
 from aligo.types import *
 from aligo.types.Enum import *
 
 
@@ -31,15 +31,15 @@
 
         :Example:
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> result = ali.create_file(CreateFileRequest(name='test.txt', parent_file_id='root', type='file', size=1024))
         >>> print(result.file_id)
         """
-        response = self._post(ADRIVE_V2_FILE_CREATEWITHFOLDERS, body=body)
+        response = self.post(ADRIVE_V2_FILE_CREATEWITHFOLDERS, body=body)
         return self._result(response, CreateFileResponse, status_code=201)
 
     def _core_create_folder(self, body: CreateFolderRequest) -> CreateFileResponse:
         """..."""
         return self.create_file(CreateFileRequest(**asdict(body)))
 
     def complete_file(self, body: CompleteFileRequest) -> BaseFile:
@@ -50,15 +50,15 @@
 
         :Example:
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> result = ali.complete_file(CompleteFileRequest(file_id='file_id', part_info_list=[UploadPartInfo(part_number=1)]))
         >>> print(result.file_id)
         """
-        response = self._post(V2_FILE_COMPLETE, body=body)
+        response = self.post(V2_FILE_COMPLETE, body=body)
         return self._result(response, BaseFile)
 
     @staticmethod
     def _get_part_info_list(file_size: int) -> List[UploadPartInfo]:
         """根据文件大小, 返回 part_info_list """
         # 以10MB为一块: 10485760
         return [UploadPartInfo(part_number=i) for i in range(1, math.ceil(file_size / Create.__UPLOAD_CHUNK_SIZE) + 1)]
@@ -74,15 +74,15 @@
             parent_file_id=parent_file_id,
             name=name,
             type='file',
             check_name_mode=check_name_mode,
             size=file_size,
             pre_hash=pre_hash
         )
-        response = self._post(ADRIVE_V2_FILE_CREATEWITHFOLDERS, body=body)
+        response = self.post(ADRIVE_V2_FILE_CREATEWITHFOLDERS, body=body)
         part_info = self._result(response, CreateFileResponse, [201, 409])
         return part_info
 
     def _get_proof_code(self, file_path: str, file_size: int) -> str:
         """计算proof_code"""
         md5_int = int(hashlib.md5(self._auth.token.access_token.encode()).hexdigest()[:16], 16)
         # file_size = os.path.getsize(file_path)
@@ -123,29 +123,29 @@
             check_name_mode=check_name_mode,
             size=file_size,
             content_hash=content_hash,
             content_hash_name="sha1",
             proof_code=proof_code,
             proof_version='v1'
         )
-        response = self._post(ADRIVE_V2_FILE_CREATEWITHFOLDERS, body=body)
+        response = self.post(ADRIVE_V2_FILE_CREATEWITHFOLDERS, body=body)
         # AttributeError: 'Null' object has no attribute 'rapid_upload'
         if response.status_code == 400:
             body.proof_code = self._get_proof_code(file_path, file_size)
-            response = self._post(ADRIVE_V2_FILE_CREATEWITHFOLDERS, body=body)
+            response = self.post(ADRIVE_V2_FILE_CREATEWITHFOLDERS, body=body)
         part_info = self._result(response, CreateFileResponse, 201)
         return part_info
 
     def get_upload_url(self, body: GetUploadUrlRequest) -> GetUploadUrlResponse:
         """
         获取上传文件的url
         :param body: [GetUploadUrlRequest]
         :return: [GetUploadUrlResponse]
         """
-        response = self._post(V2_FILE_GET_UPLOAD_URL, body=body)
+        response = self.post(V2_FILE_GET_UPLOAD_URL, body=body)
         return self._result(response, GetUploadUrlResponse)
 
     def _put_data(self, file_path: str, part_info: CreateFileResponse, file_size: int) -> Union[BaseFile, Null]:
         """上传数据"""
         with open(file_path, 'rb') as f:
             progress_bar = tqdm(total=file_size, unit='B', unit_scale=True, colour='#21d789')
             for i in range(len(part_info.part_info_list)):
@@ -296,9 +296,9 @@
             drive_id=drive_id,
             type='file',
             content_hash_name='sha1',
             check_name_mode=check_name_mode,
             proof_code=proof_code,
             proof_version='v1'
         )
-        response = self._post(ADRIVE_V2_FILE_CREATEWITHFOLDERS, body=body)
+        response = self.post(ADRIVE_V2_FILE_CREATEWITHFOLDERS, body=body)
         return self._result(response, CreateFileResponse, 201)
```

### Comparing `aligo-6.0.6/src/aligo/core/Download.py` & `aligo-6.1.0/src/aligo/core/Download.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """..."""
 import os
 import re
 from typing import Iterator, List
 
 from tqdm import tqdm
 
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.response import *
-from aligo.types import *
+from aligo.core import BaseAligo
+from aligo.core.Config import V2_FILE_GET_DOWNLOAD_URL
+from aligo.request import BatchDownloadUrlRequest, GetDownloadUrlRequest, BatchRequest, BatchSubRequest
+from aligo.response import BatchDownloadUrlResponse, GetDownloadUrlResponse
+from aligo.types import BaseFile
 
 
 class Download(BaseAligo):
     """..."""
     _DOWNLOAD_CHUNK_SIZE = 8388608  # 8 MB
 
     def _core_get_download_url(self, body: GetDownloadUrlRequest) -> GetDownloadUrlResponse:
         """..."""
-        response = self._post(V2_FILE_GET_DOWNLOAD_URL, body=body)
+        response = self.post(V2_FILE_GET_DOWNLOAD_URL, body=body)
         return self._result(response, GetDownloadUrlResponse)
 
     def _core_batch_download_url(self, body: BatchDownloadUrlRequest) -> Iterator[BatchDownloadUrlResponse]:
         """..."""
         if body.drive_id is None:
             body.drive_id = self.default_drive_id
```

### Comparing `aligo-6.0.6/src/aligo/core/Drive.py` & `aligo-6.1.0/src/aligo/core/Drive.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 """..."""
-
 from typing import List
 
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.response import *
-from aligo.types import *
+from aligo.core import BaseAligo
+from aligo.core.Config import V2_DRIVE_GET, V2_DRIVE_GET_DEFAULT_DRIVE, V2_DRIVE_LIST_MY_DRIVES
+from aligo.request import GetDriveRequest, GetDefaultDriveRequest
+from aligo.response import ListMyDrivesResponse
+from aligo.types import BaseDrive
 
 
 class Drive(BaseAligo):
     """..."""
 
     def _core_get_drive(self, body: GetDriveRequest) -> BaseDrive:
         """..."""
-        response = self._post(V2_DRIVE_GET, body=body)
+        response = self.post(V2_DRIVE_GET, body=body)
         return self._result(response, BaseDrive)
 
     def get_default_drive(self) -> BaseDrive:
         """
         Get default drive.
         :return: [BaseDrive]
 
         :Example:
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> drive = ali.get_default_drive()
         >>> print(drive.drive_name)
         """
         if self._default_drive is None:
-            response = self._post(V2_DRIVE_GET_DEFAULT_DRIVE, body=GetDefaultDriveRequest(self._auth.token.user_id))
+            response = self.post(V2_DRIVE_GET_DEFAULT_DRIVE, body=GetDefaultDriveRequest(self._auth.token.user_id))
             self._default_drive = self._result(response, BaseDrive)
         return self._default_drive
 
     def list_my_drives(self) -> List[BaseDrive]:
         """
         List my drives.
         :return: [BaseDrive]
```

### Comparing `aligo-6.0.6/src/aligo/core/Duplicate.py` & `aligo-6.1.0/src/aligo/core/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.6/src/aligo/core/EMail.py` & `aligo-6.1.0/src/aligo/core/EMail.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.6/src/aligo/core/File.py` & `aligo-6.1.0/src/aligo/core/File.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """..."""
 from typing import Iterator
 
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.response import *
-from aligo.types import *
+from aligo.core import BaseAligo
+from aligo.core.Config import ADRIVE_V3_FILE_LIST
+from aligo.request import BatchGetFileRequest, GetFileListRequest, GetFileRequest, BatchRequest, BatchSubRequest
+from aligo.response import BatchSubResponse, GetFileListResponse
+from aligo.types import BaseFile
 
 
 class File(BaseAligo):
     """..."""
 
     def _core_get_file_list(self, body: GetFileListRequest) -> Iterator[BaseFile]:
         """..."""
```

### Comparing `aligo-6.0.6/src/aligo/core/LoginServer.py` & `aligo-6.1.0/src/aligo/core/LoginServer.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from http.server import BaseHTTPRequestHandler
 from typing import Any
 
 
 class LoginServer(BaseHTTPRequestHandler):
     """..."""
 
+    # noinspection PyPep8Naming
     def do_GET(self):
         """..."""
         if self.path == '/':
             self.send_response(200)
             self.send_header("content-type", "text/html")
             self.end_headers()
             self.wfile.write(bytes(
```

### Comparing `aligo-6.0.6/src/aligo/core/Move.py` & `aligo-6.1.0/src/aligo/core/Move.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """..."""
 from typing import Iterator
 
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.response import *
+from aligo.core import BaseAligo
+from aligo.core.Config import V2_FILE_MOVE
+from aligo.request import BatchMoveFilesRequest, MoveFileRequest, BatchRequest, BatchSubRequest
+from aligo.response import BatchSubResponse, MoveFileResponse
 
 
 class Move(BaseAligo):
     """..."""
 
     def _core_move_file(self, body: MoveFileRequest) -> MoveFileResponse:
         """..."""
-        response = self._post(V2_FILE_MOVE, body=body)
+        response = self.post(V2_FILE_MOVE, body=body)
         return self._result(response, MoveFileResponse)
 
     def _core_batch_move_files(self, body: BatchMoveFilesRequest) -> Iterator[BatchSubResponse[MoveFileResponse]]:
         """..."""
         if body.drive_id is None:
             body.drive_id = self.default_drive_id
```

### Comparing `aligo-6.0.6/src/aligo/core/Recyclebin.py` & `aligo-6.1.0/src/aligo/core/Recyclebin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """..."""
 from typing import Iterator
 
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
+from aligo.core import BaseAligo
+from aligo.core.Config import V2_RECYCLEBIN_TRASH, V2_RECYCLEBIN_RESTORE, V2_RECYCLEBIN_LIST
+from aligo.request import (MoveFileToTrashRequest, BatchMoveToTrashRequest, RestoreFileRequest, BatchRequest,
+                           BatchSubRequest, BatchRestoreRequest, GetRecycleBinListRequest)
 from aligo.response import *
 from aligo.types import *
 
 
 class Recyclebin(BaseAligo):
     """删除文件太过危险, 只提供移动文件到回收站的功能"""
 
     def _core_move_file_to_trash(self, body: MoveFileToTrashRequest) -> MoveFileToTrashResponse:
         """移动文件到回收站"""
-        response = self._post(V2_RECYCLEBIN_TRASH, body=body)
+        response = self.post(V2_RECYCLEBIN_TRASH, body=body)
         return self._result(response, MoveFileToTrashResponse, [202, 204])
 
     def _core_batch_move_to_trash(self, body: BatchMoveToTrashRequest) -> Iterator[BatchSubResponse]:
         """..."""
         if body.drive_id is None:
             body.drive_id = self.default_drive_id
 
@@ -29,15 +30,15 @@
                     drive_id=body.drive_id, file_id=file_id
                 )
             ) for file_id in body.file_id_list]
         ), MoveFileToTrashResponse)
 
     def _core_restore_file(self, body: RestoreFileRequest) -> RestoreFileResponse:
         """恢复文件"""
-        response = self._post(V2_RECYCLEBIN_RESTORE, body=body)
+        response = self.post(V2_RECYCLEBIN_RESTORE, body=body)
         return self._result(response, RestoreFileResponse, 204)
 
     def _core_batch_restore_files(self, body: BatchRestoreRequest) -> Iterator[BatchSubResponse]:
         """..."""
         if body.drive_id is None:
             body.drive_id = self.default_drive_id
```

### Comparing `aligo-6.0.6/src/aligo/core/Search.py` & `aligo-6.1.0/src/aligo/core/Search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """..."""
 from typing import Iterator
 
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.response import *
-from aligo.types import *
+from aligo.core import BaseAligo
+from aligo.core.Config import V2_FILE_SEARCH, V2_AIMS_SEARCH
+from aligo.request import SearchFileRequest, AimSearchRequest
+from aligo.response import SearchFileResponse, AimSearchResponse
+from aligo.types import BaseFile
 
 
 class Search(BaseAligo):
     """..."""
 
     def _core_search_files(self, body: SearchFileRequest) -> Iterator[BaseFile]:
         """
```

### Comparing `aligo-6.0.6/src/aligo/core/Share.py` & `aligo-6.1.0/src/aligo/core/Share.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 """分享相关"""
 from dataclasses import asdict
 from typing import Iterator
 
-from aligo.core import *
+from aligo.core import BaseAligo
 from aligo.core.Config import *
 from aligo.request import *
 from aligo.response import *
 from aligo.types import *
 
 
 class Share(BaseAligo):
     """分享相关"""
 
     def share_link_extract_code(self, content: str) -> ShareLinkExtractCodeResponse:
-        response = self._post(ADRIVE_V2_SHARE_LINK_EXTRACT_CODE, body={
+        response = self.post(ADRIVE_V2_SHARE_LINK_EXTRACT_CODE, body={
             'content': content
         })
         return self._result(response, ShareLinkExtractCodeResponse, field='data')
 
     def _core_share_file(self, body: CreateShareLinkRequest) -> CreateShareLinkResponse:
         """分享文件, 支持批量分享
 
         目前(2021年07月17日)官方只开放分享部分类型文件
         """
-        response = self._post(ADRIVE_V2_SHARE_LINK_CREATE, body=body)
+        response = self.post(ADRIVE_V2_SHARE_LINK_CREATE, body=body)
         return self._result(response, CreateShareLinkResponse)
 
     def _core_update_share(self, body: UpdateShareLinkRequest) -> UpdateShareLinkResponse:
         """更新分享, 如更新 密码, 有效期 等"""
-        response = self._post(V2_SHARE_LINK_UPDATE, body=body)
+        response = self.post(V2_SHARE_LINK_UPDATE, body=body)
         return self._result(response, UpdateShareLinkResponse)
 
     def _core_cancel_share(self, body: CancelShareLinkRequest) -> CancelShareLinkResponse:
         """取消分享"""
-        response = self._post(ADRIVE_V2_SHARE_LINK_CANCEL, body=body)
+        response = self.post(ADRIVE_V2_SHARE_LINK_CANCEL, body=body)
         return self._result(response, CancelShareLinkResponse)
 
     def _core_batch_cancel_share(self, body: BatchCancelShareRequest) -> Iterator[BatchSubResponse]:
         """批量取消分享"""
         yield from self.batch_request(BatchRequest(
             requests=[BatchSubRequest(
                 id=share_id,
@@ -55,22 +55,22 @@
         :return: ShareLinkSchema对象的迭代器
         """
         yield from self._list_file(ADRIVE_V3_SHARE_LINK_LIST, body, GetShareLinkListResponse)
 
     # 处理其他人的分享
     def _core_get_share_info(self, body: GetShareInfoRequest) -> GetShareInfoResponse:
         """..."""
-        response = self._post(ADRIVE_V2_SHARE_LINK_GET_SHARE_BY_ANONYMOUS, body=body, ignore_auth=True)
+        response = self.post(ADRIVE_V2_SHARE_LINK_GET_SHARE_BY_ANONYMOUS, body=body, ignore_auth=True)
         share_info = self._result(response, GetShareInfoResponse)
         return share_info
 
     def _core_get_share_token(self, body: GetShareTokenRequest) -> GetShareTokenResponse:
         """..."""
         # noinspection PyProtectedMember
-        response = self._post(V2_SHARE_LINK_GET_SHARE_TOKEN, body=body, ignore_auth=True)
+        response = self.post(V2_SHARE_LINK_GET_SHARE_TOKEN, body=body, ignore_auth=True)
         share_token: GetShareTokenResponse = self._result(response, GetShareTokenResponse)
         share_token.share_id = body.share_id
         share_token.share_pwd = body.share_pwd
         return share_token
 
     def _core_get_share_file_list(
             self,
@@ -183,18 +183,18 @@
             }, headers={'x-share-token': x_share_token})
 
             if response.status_code != 200:
                 yield Null(response)
                 return
 
             for batch in response.json()['responses']:
-                i = DataClass.fill_attrs(BatchSubResponse, batch)
+                i = BatchSubResponse(**batch)
                 if i.body:
                     # noinspection PyArgumentList
-                    i.body = DataClass.fill_attrs(BatchShareFileSaveToDriveResponse, i.body)
+                    i.body = BatchShareFileSaveToDriveResponse(i.body)
                 yield i
 
     def _core_search_share_files(self, body: SearchShareFileRequest, share_token) -> Iterator[BaseShareFile]:
         """
         关于 query 的语法, 参考下段代码
         {
             key: "getPDSSearchQuery", value: function () {
@@ -207,9 +207,9 @@
         eg: 'name match "epub" and category = "image"'
         category : BaseFileCategory
         """
         yield from self._list_file(
             RECOMMEND_V1_SHARELINK_SEARCH, body, SearchShareFileResponse, headers={'x-share-token': share_token})
 
     def _core_private_share_files(self, body: PrivateShareRequest) -> PrivateShareResponse:
-        response = self._post(ADRIVE_V1_SHARE_CREATE, body=body)
+        response = self.post(ADRIVE_V1_SHARE_CREATE, body=body)
         return self._result(response, PrivateShareResponse)
```

### Comparing `aligo-6.0.6/src/aligo/core/Star.py` & `aligo-6.1.0/src/aligo/core/Star.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """收藏相关"""
 from dataclasses import asdict
 from typing import Iterator
 
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.response import *
-from aligo.types import *
+from aligo.core.Config import V2_FILE_LIST_BY_CUSTOM_INDEX_KEY
+from aligo.request import (StarredFileRequest, UpdateFileRequest, BatchStarFilesRequest, BatchRequest, BatchSubRequest,
+                           GetStarredListRequest)
+from aligo.response import GetStarredListResponse, BatchSubResponse
+from aligo.types import BaseFile
 from .Update import Update
 
 
 class Star(Update):
     """..."""
     _MAX_STAR_COUNT: int = 500
```

### Comparing `aligo-6.0.6/src/aligo/core/Update.py` & `aligo-6.1.0/src/aligo/core/Update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """..."""
-
 from dataclasses import asdict
 
-from aligo.core import *
-from aligo.core.Config import *
-from aligo.request import *
-from aligo.types import *
+from aligo.core import BaseAligo
+from aligo.core.Config import V3_FILE_UPDATE
+from aligo.request import UpdateFileRequest, RenameFileRequest
+from aligo.types import BaseFile
 
 
 class Update(BaseAligo):
     """..."""
 
     def update_file(self, body: UpdateFileRequest) -> BaseFile:
         """
@@ -19,13 +18,13 @@
 
         :Example:
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> new_file = ali.update_file(UpdateFileRequest(file_id='file_id', name='new_name'))
         >>> print(new_file.name)
         """
-        response = self._post(V3_FILE_UPDATE, body=body)
+        response = self.post(V3_FILE_UPDATE, body=body)
         return self._result(response, BaseFile)
 
     def _core_rename_file(self, body: RenameFileRequest) -> BaseFile:
         """..."""
         return self.update_file(UpdateFileRequest(**asdict(body)))
```

### Comparing `aligo-6.0.6/src/aligo/core/User.py` & `aligo-6.1.0/src/aligo/core/User.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """..."""
-
 from typing import List
 
-from aligo.core import *
-from aligo.core.Config import *
+from aligo.core import BaseAligo
+from aligo.core.Config import (ADRIVE_V1_USER_CONFIG_GET, MEMBER_HOST, V1_USERS_REWARDS, V2_USER_GET,
+                               BUSINESS_V1_USERS_VIP_INFO, USERS_V2_USERS_DEVICE_LIST)
 from aligo.response import RewardSpaceResponse, UsersVipInfoResponse
-from aligo.types import *
+from aligo.types import BaseUser, UserConfig, LoginDevice
 
 
 class User(BaseAligo):
     """..."""
 
     def get_user(self, f5: bool = False) -> BaseUser:
         """
         获取用户信息
         :param f5: [可选] 是否强制刷新
         :return: [BaseUser]
         """
         if self._user is None or f5:
-            response = self._post(V2_USER_GET)
+            response = self.post(V2_USER_GET)
             # response.status_code == 200 or self._error_log_exit(response)
             # self._user = BaseUser(**response.json())
             self._user = self._result(response, BaseUser)
         return self._user
 
     def rewards_space(self, code: str):
         """
@@ -31,25 +31,25 @@
         :return: [RewardSpaceResponse]
 
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> result = ali.rewards_space('12345678')
         >>> print(result)
         """
-        response = self._post(V1_USERS_REWARDS, MEMBER_HOST, body={
+        response = self.post(V1_USERS_REWARDS, MEMBER_HOST, body={
             'code': code
         })
         return self._result(response, RewardSpaceResponse)
 
     def get_user_config(self) -> UserConfig:
         """获取用户配置信息"""
-        response = self._post(ADRIVE_V1_USER_CONFIG_GET, body={})
+        response = self.post(ADRIVE_V1_USER_CONFIG_GET, body={})
         return self._result(response, UserConfig)
 
     def get_vip_info(self) -> UsersVipInfoResponse:
         """获取用户vip信息"""
-        response = self._post(BUSINESS_V1_USERS_VIP_INFO, body={})
+        response = self.post(BUSINESS_V1_USERS_VIP_INFO, body={})
         return self._result(response, UsersVipInfoResponse)
 
     def list_login_device(self) -> List[LoginDevice]:
-        response = self._post(USERS_V2_USERS_DEVICE_LIST)
+        response = self.post(USERS_V2_USERS_DEVICE_LIST)
         return self._result(response, LoginDevice, field='result.devices')
```

### Comparing `aligo-6.0.6/src/aligo/request/AlbumListFilesRequest.py` & `aligo-6.1.0/src/aligo/request/AlbumListFilesRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """..."""
 from dataclasses import dataclass
 
-from aligo.types import DataClass
+from aligo.types import DatClass
 from aligo.types.Enum import AlbumFileListType, OrderDirection
 
 
 @dataclass
-class AlbumListFilesRequest(DataClass):
+class AlbumListFilesRequest(DatClass):
     """..."""
     album_id: str = None
     fields: str = "*"
     filter: str = ""
     image_thumbnail_process: str = "image/resize,w_400/format,jpeg"
     image_url_process: str = "image/resize,w_1920/format,jpeg"
     limit: int = 100
```

### Comparing `aligo-6.0.6/src/aligo/request/CreateFileRequest.py` & `aligo-6.1.0/src/aligo/request/CreateFileRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """..."""
 from dataclasses import dataclass, field
 from typing import List
 
-from aligo.types import DataClass, UploadPartInfo
-from aligo.types.Enum import *
+from aligo.types import DatClass, UploadPartInfo
+from aligo.types.Enum import BaseFileType, BaseFileContentHashName, CheckNameMode
 
 
 @dataclass
-class CreateFileRequest(DataClass):
+class CreateFileRequest(DatClass):
     """..."""
     name: str
     file_id: str = None
     type: BaseFileType = 'folder'
     parent_file_id: str = 'root'
     size: int = field(default=None, repr=False)
     check_name_mode: CheckNameMode = field(default='auto_rename', repr=False)
```

### Comparing `aligo-6.0.6/src/aligo/request/CreateShareLinkRequest.py` & `aligo-6.1.0/src/aligo/request/CreateShareLinkRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """..."""
 from dataclasses import dataclass
 from typing import List
 
-from aligo.types import DataClass
+from aligo.types import DatClass
 
 
 @dataclass
-class CreateShareLinkRequest(DataClass):
+class CreateShareLinkRequest(DatClass):
     """创建分享链接请求
 
     Attributes:
         drive_id (str):
         file_id_list (List[str]):
         share_pwd (str): 提取码，0-64个字符。长度0表示没有提取码。
         expiration (str): 失效时间点。RFC3339格式，比如："2020-06-28T11:33:00.000+08:00"。永久有效: ""
```

### Comparing `aligo-6.0.6/src/aligo/request/GetFileListRequest.py` & `aligo-6.1.0/src/aligo/request/GetFileListRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """..."""
-
 from dataclasses import dataclass, field
 
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.types import DatClass
+from aligo.types.Enum import BaseFileCategory, BaseFileType, GetFileListFields, GetFileListOrderBy, OrderDirection
 
 
 @dataclass
-class GetFileListRequest(DataClass):
+class GetFileListRequest(DatClass):
     """..."""
     parent_file_id: str = 'root'
     drive_id: str = None
     starred: bool = field(default=None, repr=False)
     all: bool = field(default=False, repr=False)
     category: BaseFileCategory = field(default=None, repr=False)
     fields: GetFileListFields = field(default='*', repr=False)
```

### Comparing `aligo-6.0.6/src/aligo/request/GetFileRequest.py` & `aligo-6.1.0/src/aligo/request/SearchFileRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """..."""
+from dataclasses import field, dataclass
 
-from dataclasses import dataclass, field
-
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.types import DatClass
 
 
 @dataclass
-class GetFileRequest(DataClass):
+class SearchFileRequest(DatClass):
     """..."""
-    file_id: str
+    query: str
     drive_id: str = None
-    url_expire_sec: int = field(default=14400, repr=False)
-    fields: GetFileFields = field(default='*', repr=False)
+    limit: int = field(default=100, repr=False)
     image_thumbnail_process: str = field(default='image/resize,w_160/format,jpeg', repr=False)
     image_url_process: str = field(default='image/resize,w_1920/format,jpeg', repr=False)
+    marker: str = field(default=None, repr=False)
+    order_by: str = field(default=None, repr=False)
+    url_expire_sec: int = field(default=14400, repr=False)
     video_thumbnail_process: str = field(default='video/snapshot,t_0,f_jpg,ar_auto,w_800', repr=False)
```

### Comparing `aligo-6.0.6/src/aligo/request/GetRecycleBinListRequest.py` & `aligo-6.1.0/src/aligo/request/GetRecycleBinListRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """..."""
 from dataclasses import dataclass, field
 
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.types import DatClass
+from aligo.types.Enum import BaseFileType, OrderDirection, GetRecycleBinListOrderBy
 
 
 @dataclass
-class GetRecycleBinListRequest(DataClass):
+class GetRecycleBinListRequest(DatClass):
     """..."""
     drive_id: str = None
     fields: str = field(default=None, repr=False)
     limit: int = field(default=200, repr=False)
     marker: str = field(default=None, repr=False)
     order_direction: OrderDirection = field(default='ASC', repr=False)
     order_by: GetRecycleBinListOrderBy = field(default='name', repr=False)
```

### Comparing `aligo-6.0.6/src/aligo/request/GetShareFileListRequest.py` & `aligo-6.1.0/src/aligo/request/GetShareFileListRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """获取分享文件列表"""
 from dataclasses import dataclass, field
 
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.types import DatClass
+from aligo.types.Enum import BaseFileCategory, BaseFileType, GetShareFileListOrderBy, OrderDirection
 
 
 @dataclass
-class GetShareFileListRequest(DataClass):
+class GetShareFileListRequest(DatClass):
     """..."""
     share_id: str = None
     starred: bool = None
     all: bool = None
     category: BaseFileCategory = None
     fields: str = None
     image_thumbnail_process: str = None
```

### Comparing `aligo-6.0.6/src/aligo/request/GetShareLinkDownloadUrlRequest.py` & `aligo-6.1.0/src/aligo/request/GetShareLinkDownloadUrlRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """分享链接下载链接请求体"""
 from dataclasses import dataclass
 
-from aligo.types import *
+from aligo.types import DatClass
 
 
 @dataclass
-class GetShareLinkDownloadUrlRequest(DataClass):
+class GetShareLinkDownloadUrlRequest(DatClass):
     """..."""
     share_id: str
     file_id: str
-    # {"code":"InvalidParameter.ExpireSec","message":"The input parameter expire_sec is not valid. expire_sec should be less or equal than 600"}
+    # {
+    #   "code":"InvalidParameter.ExpireSec",
+    #   "message":"The input parameter expire_sec is not valid. expire_sec should be less or equal than 600"
+    # }
     # expire_sec: int = 14400
     expire_sec: int = 600
     image_thumbnail_process: str = None
     image_url_process: str = None
     video_thumbnail_process: str = None
     get_video_play_info: bool = None
     get_audio_play_info: bool = None
```

### Comparing `aligo-6.0.6/src/aligo/request/GetShareLinkListRequest.py` & `aligo-6.1.0/src/aligo/request/GetShareLinkListRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """..."""
 from dataclasses import dataclass
 
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.types import DatClass
+from aligo.types.Enum import GetShareLinkListOrderBy, OrderDirection
 
 
 @dataclass
-class GetShareLinkListRequest(DataClass):
+class GetShareLinkListRequest(DatClass):
     """获取自己的分享列表
 
     Attributes:
         creator (str): 一 、管理员：1.1 不传，查所有用户 1.2 传指定user_id，查指定用户的分享。
             * 二、普通用户：2.1 不传，查自己2.2 传指定user_id，只能是自己，否则报403
         limit (int): 返回数据最大条数,范围:[1-100]，默认:100
         marker (str):
```

### Comparing `aligo-6.0.6/src/aligo/request/UpdateFileRequest.py` & `aligo-6.1.0/src/aligo/request/UpdateFileRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """..."""
 from dataclasses import dataclass, field
 from typing import List
 
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.types import DatClass
+from aligo.types.Enum import CheckNameMode
 
 
 @dataclass
-class UpdateFileRequest(DataClass):
+class UpdateFileRequest(DatClass):
     """...."""
     name: str = None
     file_id: str = None
     drive_id: str = None
     check_name_mode: CheckNameMode = field(default='refuse', repr=False)
     custom_index_key: str = field(default=None, repr=False)
     description: str = field(default=None, repr=False)
```

### Comparing `aligo-6.0.6/src/aligo/request/UpdateShareLinkRequest.py` & `aligo-6.1.0/src/aligo/request/UpdateShareLinkRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """更新分享链接请求"""
 from dataclasses import dataclass
 
-from aligo.types import DataClass
+from aligo.types import DatClass
 
 
 @dataclass
-class UpdateShareLinkRequest(DataClass):
+class UpdateShareLinkRequest(DatClass):
     """
     更新分享链接请求
 
     Attributes:
         share_id (str):
         share_pwd (str): 提取码，0-64个字符。长度0表示没有提取码。
         expiration (str): 失效时间点。RFC3339格式，比如："2020-06-28T11:33:00.000+08:00"。永久有效: ""
```

### Comparing `aligo-6.0.6/src/aligo/request/__init__.py` & `aligo-6.1.0/src/aligo/request/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.6/src/aligo/response/CreateFileResponse.py` & `aligo-6.1.0/src/aligo/types/BaseDrive.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 """..."""
 from dataclasses import dataclass, field
-from typing import List, Dict
 
-from aligo.types import *
-from aligo.types.Enum import *
+from .Type import DatClass
 
 
 @dataclass
-class CreateFileResponse(DataClass):
+class BaseDrive(DatClass):
     """..."""
-    file_name: str = None
-    type: BaseFileType = None
-    file_id: str = None
-    parent_file_id: str = None
+    drive_id: str = None
+    used_size: int = None
+    total_size: int = None
+    drive_name: str = field(default=None, repr=False)
+    owner: str = field(default=None, repr=False)
+    description: str = field(default=None, repr=False)
+    drive_type: str = field(default=None, repr=False)
+    creator: str = field(default=None, repr=False)
     domain_id: str = field(default=None, repr=False)
-    drive_id: str = field(default=None, repr=False)
+    status: str = field(default=None, repr=False)
+    store_id: str = field(default=None, repr=False)
+    owner_type: str = field(default=None, repr=False)
+    relative_path: str = field(default=None, repr=False)
     encrypt_mode: str = field(default=None, repr=False)
-    part_info_list: List[UploadPartInfo] = field(default_factory=list, repr=False)
-    rapid_upload: bool = field(default=None, repr=False)
-    status: BaseFileStatus = field(default=None, repr=False)
-    streams_upload_info: Dict = field(default=None, repr=False)
-    upload_id: str = field(default=None, repr=False)
-    exist: bool = field(default=None, repr=False)
-    location: str = field(default=None, repr=False)
-
-    # pre_hash
-    pre_hash: str = field(default=None, repr=False)
-    # 与批量操作中的错误不同, 此处code为是否命中秒传的结果
-    code: str = field(default=None, repr=False)
-    message: str = field(default=None, repr=False)
-    revision_id: str = field(default=None, repr=False)
+    encrypt_data_access: bool = field(default=None, repr=False)
+    permission: str = field(default=None, repr=False)
+    created_at: str = field(default=None, repr=False)
+    subdomain_id: str = field(default=None, repr=False)
+    category: str = field(default=None, repr=False)
+    updated_at: str = field(default=None, repr=False)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aligo-6.0.6/src/aligo/response/CreateShareLinkResponse.py` & `aligo-6.1.0/src/aligo/response/CreateShareLinkResponse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """..."""
 from dataclasses import dataclass, field
 from typing import List
 
-from aligo.types import *
-from aligo.types.Enum import *
+from aligo.types import DatClass, ShareLinkBaseFile
+from aligo.types.Enum import SharePolicy
 
 
 @dataclass
-class CreateShareLinkResponse(DataClass):
+class CreateShareLinkResponse(DatClass):
     """
     分享链接结构对象, 类似 BaseShareFile 的含义
     Attributes:
         created_at (str): 分享创建时间
         updated_at (str): 分享更新时间
         creator (str): 分享创建者
         description (str): 描述
```

### Comparing `aligo-6.0.6/src/aligo/response/DuplicateListResponse.py` & `aligo-6.1.0/src/aligo/response/DuplicateListResponse.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """..."""
 from dataclasses import dataclass, field
 from typing import List
 
-from aligo.types import DataClass
+from aligo.types import DatClass
 
 
 @dataclass
-class DuplicateFileInfo(DataClass):
+class DuplicateFileInfo(DatClass):
     """..."""
     name: str = None
     thumbnail: str = None
     type: str = None
     category: str = None
     size: int = None
     starred: bool = None
@@ -22,18 +22,18 @@
     created_at: str = None
     updated_at: str = None
     trashed_at: str = None
     mime_type: str = None
 
 
 @dataclass
-class DuplicateItem(DataClass):
+class DuplicateItem(DatClass):
     """..."""
     items: List[DuplicateFileInfo] = field(default_factory=list)
     group_id: str = ''
 
 
 @dataclass
-class DuplicateListResponse(DataClass):
+class DuplicateListResponse(DatClass):
     """..."""
     items: List[DuplicateItem] = field(default_factory=list)
     next_marker: str = ''
```

### Comparing `aligo-6.0.6/src/aligo/response/GetShareInfoResponse.py` & `aligo-6.1.0/src/aligo/response/GetShareInfoResponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """..."""
 from dataclasses import dataclass, field
 from typing import List
 
-from aligo.types import DataClass
+from aligo.types import DatClass
 from .ShareItemInfo import ShareItemInfo
 
 
 @dataclass
-class GetShareInfoResponse(DataClass):
+class GetShareInfoResponse(DatClass):
     """..."""
     avatar: str = None
     creator_id: str = None
     creator_name: str = None
     creator_phone: str = None
     expiration: str = None
     file_count: int = None
```

### Comparing `aligo-6.0.6/src/aligo/response/UpdateShareLinkResponse.py` & `aligo-6.1.0/src/aligo/response/UpdateShareLinkResponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """更新分享链接响应"""
-
 from dataclasses import dataclass, field
 from typing import List
 
-from aligo.types import DataClass
-from aligo.types.Enum import *
+from aligo.types import DatClass
+from aligo.types.Enum import SharePolicy
 from aligo.types.ShareLinkBaseFile import ShareLinkBaseFile
 
 
 @dataclass
-class UpdateShareLinkResponse(DataClass):
+class UpdateShareLinkResponse(DatClass):
     """更新分享链接响应"""
-
     share_id: str
     share_name: str = None
     share_pwd: str = None
     expiration: str = None
     created_at: str = field(default=None, repr=False)
     updated_at: str = field(default=None, repr=False)
     creator: str = field(default=None, repr=False)
```

### Comparing `aligo-6.0.6/src/aligo/response/__init__.py` & `aligo-6.1.0/src/aligo/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.6/src/aligo/types/BaseAlbum.py` & `aligo-6.1.0/src/aligo/types/BaseAlbum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """..."""
 from dataclasses import dataclass, field
 from typing import List
 
 from .BaseFile import BaseFile
-from .DataClass import DataClass
+from .Type import DatClass
 
 
 @dataclass
-class _BaseAlbumList(DataClass):
+class _BaseAlbumList(DatClass):
     """..."""
     list: List[BaseFile] = field(default_factory=list)
 
 
 @dataclass
-class BaseAlbum(DataClass):
+class BaseAlbum(DatClass):
     """..."""
     owner: str = None
     name: str = None
     description: str = None
     album_id: str = None
     file_count: int = None
     image_count: int = None
```

### Comparing `aligo-6.0.6/src/aligo/types/BaseDrive.py` & `aligo-6.1.0/src/aligo/types/BaseUser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """..."""
-
 from dataclasses import dataclass, field
 
-from .DataClass import DataClass
+from .Type import DatClass
+
+
+# 1. 只 REPR 能理解的数据
+# 2. 尽可能的少
+# 3. 不知道的不处理, 默认
 
 
 @dataclass
-class BaseDrive(DataClass):
+class BaseUser(DatClass):
     """..."""
-    drive_id: str = None
-    used_size: int = None
-    total_size: int = None
-    drive_name: str = field(default=None, repr=False)
-    owner: str = field(default=None, repr=False)
+    user_name: str = None
+    user_id: str = None
+    default_drive_id: str = None
     description: str = field(default=None, repr=False)
-    drive_type: str = field(default=None, repr=False)
-    creator: str = field(default=None, repr=False)
-    domain_id: str = field(default=None, repr=False)
+    nick_name: str = field(default=None, repr=False)
+    email: str = field(default=None, repr=False)
+    phone: str = field(default=None, repr=False)
+    role: str = field(default=None, repr=False)
     status: str = field(default=None, repr=False)
-    store_id: str = field(default=None, repr=False)
-    owner_type: str = field(default=None, repr=False)
-    relative_path: str = field(default=None, repr=False)
-    encrypt_mode: str = field(default=None, repr=False)
-    encrypt_data_access: bool = field(default=None, repr=False)
+    created_at: int = field(default=None, repr=False)
+    domain_id: str = field(default=None, repr=False)
+    updated_at: int = field(default=None, repr=False)
+    avatar: str = field(default=None, repr=False)
+    user_data: dict = field(default=None, repr=False)
+    deny_change_password_by_self: bool = field(default=False, repr=False)
+    need_change_password_next_login: bool = field(default=False, repr=False)
     permission: str = field(default=None, repr=False)
-    created_at: str = field(default=None, repr=False)
-    subdomain_id: str = field(default=None, repr=False)
-    category: str = field(default=None, repr=False)
+    creator: str = field(default=None, repr=False)
+    expired_at: int = field(default=None, repr=False)
+    default_location: str = field(default=None, repr=False)
+    phone_region: str = field(default=None, repr=False)
+    last_login_time: int = field(default=None, repr=False)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aligo-6.0.6/src/aligo/types/BaseFile.py` & `aligo-6.1.0/src/aligo/types/BaseFile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """..."""
-from dataclasses import dataclass, field
+from dataclasses import dataclass
+from dataclasses import field
 from typing import Dict, List
 
-from .DataClass import DataClass
-from .Enum import *
+from .Type import DatClass
+from .Enum import BaseFileType, BaseFileCategory, BaseFileContentHashName
 from .FieldsInfo import FieldsInfo
 from .ImageMedia import ImageMedia
 from .VideoMedia import VideoMedia
 from .VideoPreview import VideoPreview
 
 
 @dataclass
-class BaseFile(DataClass):
+class BaseFile(DatClass):
     """..."""
     type: BaseFileType = None
     file_id: str = None
     name: str = None
     parent_file_id: str = field(default=None, repr=False)
     category: BaseFileCategory = field(default=None, repr=False)
     size: int = field(default=None, repr=False)
```

### Comparing `aligo-6.0.6/src/aligo/types/BaseShareFile.py` & `aligo-6.1.0/src/aligo/types/BaseShareFile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """基本分享文件"""
-from dataclasses import dataclass, field
+from dataclasses import dataclass
+from dataclasses import field
 from typing import List
 
-from .DataClass import DataClass
 from .Enum import BaseFileCategory, BaseFileType
 from .ImageMedia import ImageMedia
+from .Type import DatClass
 from .VideoMedia import VideoMedia
 from .VideoPreview import VideoPreview
 
 
 @dataclass
-class BaseShareFile(DataClass):
+class BaseShareFile(DatClass):
     """..."""
     share_id: str = None
     name: str = None
     size: int = None
     creator: str = None
     description: str = None
     category: BaseFileCategory = None
@@ -41,8 +42,8 @@
     drive_id: str = None
     domain_id: str = None
     revision_id: str = None
     # 2022年11月21日13时25分58秒
     starred: bool = False
     content_hash: str = None
     trashed_at: str = None
-    from_share_id : str = None
+    from_share_id: str = None
```

### Comparing `aligo-6.0.6/src/aligo/types/BaseUser.py` & `aligo-6.1.0/src/aligo/types/Token.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """..."""
-
 from dataclasses import dataclass, field
 
-from .DataClass import DataClass
-
-
-# 1. 只 REPR 能理解的数据
-# 2. 尽可能的少
-# 3. 不知道的不处理, 默认
+from .Type import DatClass
 
 
-@dataclass
-class BaseUser(DataClass):
+@dataclass(eq=False)
+class Token(DatClass):
     """..."""
     user_name: str = None
+    nick_name: str = None
     user_id: str = None
     default_drive_id: str = None
-    description: str = field(default=None, repr=False)
-    nick_name: str = field(default=None, repr=False)
-    email: str = field(default=None, repr=False)
-    phone: str = field(default=None, repr=False)
+    # noinspection SpellCheckingInspection
+    default_sbox_drive_id: str = None
     role: str = field(default=None, repr=False)
     status: str = field(default=None, repr=False)
-    created_at: int = field(default=None, repr=False)
-    domain_id: str = field(default=None, repr=False)
-    updated_at: int = field(default=None, repr=False)
+    access_token: str = field(default=None, repr=False)
+    refresh_token: str = field(default=None, repr=False)
+    expires_in: int = field(default=None, repr=False)
+    token_type: str = field(default=None, repr=False)
     avatar: str = field(default=None, repr=False)
+    expire_time: str = field(default=None, repr=False)
+    state: str = field(default=None, repr=False)
+    exist_link: list = field(default=None, repr=False)
+    need_link: bool = field(default=None, repr=False)
     user_data: dict = field(default=None, repr=False)
-    deny_change_password_by_self: bool = field(default=False, repr=False)
-    need_change_password_next_login: bool = field(default=False, repr=False)
-    permission: str = field(default=None, repr=False)
-    creator: str = None
-    expired_at: int = 0
-    default_location: str = ''
+    pin_setup: bool = field(default=None, repr=False)
+    is_first_login: bool = field(default=None, repr=False)
+    need_rp_verify: bool = field(default=None, repr=False)
+    device_id: str = field(default=None, repr=False)
+    domain_id: str = field(default=None, repr=False)
+    # noinspection SpellCheckingInspection
+    hlogin_url: str = field(default=None, repr=False)
+    # x-signature x-device-id x-nonce
+    x_device_id: str = field(default=None, repr=False)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aligo-6.0.6/src/aligo/types/Enum.py` & `aligo-6.1.0/src/aligo/types/Enum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.6/src/aligo/types/ImageMedia.py` & `aligo-6.1.0/src/aligo/types/ImageMedia.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """..."""
 from dataclasses import dataclass, field
 from typing import List
 
-from .FaceThumbnail import FaceThumbnail
 from .CroppingSuggestionItem import CroppingSuggestionItem
-from .DataClass import DataClass
+from .FaceThumbnail import FaceThumbnail
 from .ImageQuality import ImageQuality
 from .SystemTag import SystemTag
+from .Type import DatClass
 
 
 @dataclass
-class ImageMedia(DataClass):
+class ImageMedia(DatClass):
     """..."""
     time: str = None
     faces: str = None
     city: str = None
     country: str = None
     address_line: str = None
     exif: str = None
```

### Comparing `aligo-6.0.6/src/aligo/types/Null.py` & `aligo-6.1.0/src/aligo/types/Null.py`

 * *Files identical despite different names*

### Comparing `aligo-6.0.6/src/aligo/types/ShareLinkSchema.py` & `aligo-6.1.0/src/aligo/types/ShareLinkSchema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """..."""
-
 from dataclasses import dataclass, field
 from typing import List
 
-from .DataClass import DataClass
 from .Enum import *
 from .ShareLinkBaseFile import ShareLinkBaseFile
+from .Type import DatClass
 
 
 @dataclass
-class ShareLinkSchema(DataClass):
+class ShareLinkSchema(DatClass):
     """
     分享链接结构对象, 类似 BaseShareFile 的含义
     Attributes:
         created_at (str): 分享创建时间
         updated_at (str): 分享更新时间
         creator (str): 分享创建者
         description (str): 描述
```

### Comparing `aligo-6.0.6/src/aligo/types/Token.py` & `aligo-6.1.0/src/aligo/types/ShareLinkBaseFile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,72 @@
 """..."""
-from dataclasses import dataclass, field
+from dataclasses import dataclass
+from dataclasses import field
+from typing import Dict, List
 
-from .DataClass import DataClass
+from .Enum import BaseFileCategory, BaseFileContentHashName, BaseFileType
+from .FieldsInfo import FieldsInfo
+from .ImageMedia import ImageMedia
+from .Type import DatClass
+from .VideoMedia import VideoMedia
+from .VideoPreview import VideoPreview
 
 
-@dataclass(eq=False)
-class Token(DataClass):
+@dataclass
+class ShareLinkBaseFile(DatClass):
     """..."""
-    user_name: str = None
-    nick_name: str = None
-    user_id: str = None
-    default_drive_id: str = None
-    # noinspection SpellCheckingInspection
-    default_sbox_drive_id: str = None
-    role: str = field(default=None, repr=False)
-    status: str = field(default=None, repr=False)
-    access_token: str = field(default=None, repr=False)
-    refresh_token: str = field(default=None, repr=False)
-    expires_in: int = field(default=None, repr=False)
-    token_type: str = field(default=None, repr=False)
-    avatar: str = field(default=None, repr=False)
-    expire_time: str = field(default=None, repr=False)
-    state: str = field(default=None, repr=False)
-    exist_link: list = field(default=None, repr=False)
-    need_link: bool = field(default=None, repr=False)
-    user_data: dict = field(default=None, repr=False)
-    pin_setup: bool = field(default=None, repr=False)
-    is_first_login: bool = field(default=None, repr=False)
-    need_rp_verify: bool = field(default=None, repr=False)
-    device_id: str = field(default=None, repr=False)
+    type: BaseFileType = None
+    file_id: str = None
+    name: str = None
+    parent_file_id: str = field(default=None, repr=False)
+    category: BaseFileCategory = field(default=None, repr=False)
+    size: int = field(default=None, repr=False)
+    created_at: str = field(default=None, repr=False)
+    content_type: str = field(default=None, repr=False)
+    description: str = field(default=None, repr=False)
+    content_hash: str = field(default=None, repr=False)
+    content_hash_name: BaseFileContentHashName = field(default=None, repr=False)
+    crc64_hash: str = field(default=None, repr=False)
     domain_id: str = field(default=None, repr=False)
-    # noinspection SpellCheckingInspection
-    hlogin_url: str = field(default=None, repr=False)
-    # x-signature x-device-id x-nonce
-    x_device_id: str = field(default=None, repr=False)
+    download_url: str = field(default=None, repr=False)
+    drive_id: str = field(default=None, repr=False)
+    encrypt_mode: str = field(default=None, repr=False)
+    file_extension: str = field(default=None, repr=False)
+    hidden: bool = field(default=None, repr=False)
+    image_media_metadata: ImageMedia = field(default=None, repr=False)
+    labels: list = field(default=None, repr=False)
+    meta: str = field(default=None, repr=False)
+    mime_extension: str = field(default=None, repr=False)
+    mime_type: str = field(default=None, repr=False)
+    punish_flag: int = field(default=None, repr=False)
+    starred: bool = field(default=None, repr=False)
+    status: str = field(default=None, repr=False)
+    streams_url_info: Dict = field(default=None, repr=False)
+    streams_info: Dict = field(default=None, repr=False)
+    thumbnail: str = field(default=None, repr=False)
+    trashed: bool = field(default=None, repr=False)
+    trashed_at: str = field(default=None, repr=False)
+    updated_at: str = field(default=None, repr=False)
+    upload_id: str = field(default=None, repr=False)
+    url: str = field(default=None, repr=False)
+    user_meta: str = field(default=None, repr=False)
+    video_media_metadata: VideoMedia = field(default=None, repr=False)
+    video_preview_metadata: VideoPreview = field(default=None, repr=False)
+    location: str = field(default=None, repr=False)
+    action_list: List[str] = field(default_factory=list, repr=False)
+    user_tags: Dict = field(default=None, repr=False)
+    last_modifier_type: str = field(default=None, repr=False)
+    last_modifier_id: str = field(default=None, repr=False)
+    last_modifier_name: str = field(default=None, repr=False)
+    creator_type: str = field(default=None, repr=False)
+    creator_id: str = field(default=None, repr=False)
+    creator_name: str = field(default=None, repr=False)
+    revision_id: str = field(default=None, repr=False)
+    sync_flag: bool = field(default=None, repr=False)
+    sync_device_flag: bool = field(default=None, repr=False)
+    sync_meta: str = field(default=None, repr=False)
+    ex_fields_info: FieldsInfo = field(default=None, repr=False)
+    from_share_id: str = None
+    revision_version: int = None
+    channel: str = None
+    meta_name_punish_flag: int = None
+    meta_name_investigation_status: int = None
```

### Comparing `aligo-6.0.6/src/aligo/types/UserConfig.py` & `aligo-6.1.0/src/aligo/types/UserConfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """..."""
 from dataclasses import dataclass, field
 
-from .DataClass import DataClass
+from .Type import DatClass
 
 
 @dataclass
-class UserConfig(DataClass):
+class UserConfig(DatClass):
     """
     {
       "id": 601978,
       "face_ai_recognition_status": 1,
       "auto_generate_memory": 0,
       "is_sfiia_entry_hidden": false,
       "homepage_visibility": 1,
```

### Comparing `aligo-6.0.6/src/aligo/types/VideoMedia.py` & `aligo-6.1.0/src/aligo/types/VideoMedia.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """..."""
 from dataclasses import dataclass
 from typing import List
 
-from .DataClass import DataClass
 from .ImageTag import ImageTag
+from .Type import DatClass
 from .VideoMediaAudioStream import VideoMediaAudioStream
 from .VideoMediaVideoStream import VideoMediaVideoStream
 
 
 @dataclass
-class VideoMedia(DataClass):
+class VideoMedia(DatClass):
     """..."""
     time: str = None
     city: str = None
     country: str = None
     address_line: str = None
     district: str = None
     duration: str = None
```

### Comparing `aligo-6.0.6/src/aligo/types/VideoPreview.py` & `aligo-6.1.0/src/aligo/types/VideoPreview.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """..."""
 from dataclasses import dataclass
 from typing import List
 
 from .AudioMeta import AudioMeta
 from .AudioMusicMeta import AudioMusicMeta
 from .AudioTranscodeTemplate import AudioTranscodeTemplate
-from .DataClass import DataClass
+from .Type import DatClass
 from .VideoPreviewSprite import VideoPreviewSprite
 from .VideoTranscodeTemplate import VideoTranscodeTemplate
 
 
 @dataclass
-class VideoPreview(DataClass):
+class VideoPreview(DatClass):
     """..."""
     video_format: str = None
     audio_format: str = None
     duration: str = None
     audio_sample_rate: str = None
     audio_channels: int = None
     audio_template_list: List[AudioTranscodeTemplate] = None
```

### Comparing `aligo-6.0.6/src/aligo/types/__init__.py` & `aligo-6.1.0/src/aligo/types/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 """..."""
-# 必须在头部, 不能使用Pycharm的自动格式化
-# from .Enum import *
-
 from .AudioMeta import AudioMeta
 from .AudioMusicMeta import AudioMusicMeta
 from .AudioTranscodeTemplate import AudioTranscodeTemplate
 from .BaseAlbum import BaseAlbum
 from .BaseDrive import BaseDrive
 from .BaseFile import BaseFile
 from .BaseShareFile import BaseShareFile
 from .BaseUser import BaseUser
 from .CroppingBoundary import CroppingBoundary
 from .CroppingSuggestionItem import CroppingSuggestionItem
-from .DataClass import DataClass
+from .Type import DataType, DatClass
 from .DriveCapacityDetail import DriveCapacityDetail
 from .DriveFile import DriveFile
 from .EMailConfig import EMailConfig
 from .FaceThumbnail import FaceThumbnail
 from .FolderSizeInfo import FolderSizeInfo
 from .ImageMedia import ImageMedia
 from .ImageQuality import ImageQuality
 from .ImageTag import ImageTag
 from .ListAlbumItem import ListAlbumItem
 from .LoginDevice import LoginDevice
-from .LoginTimout import LoginTimeout
 from .MediaTransCodeTemplate import MediaTransCodeTemplate
 from .Null import Null
 from .PersonalRightsInfo import PersonalRightsInfo
 from .PersonalSpaceInfo import PersonalSpaceInfo
 from .Privilege import Privilege
 from .RateLimit import RateLimit
 from .ShareLinkBaseFile import ShareLinkBaseFile
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aligo-6.0.6/src/aligo.egg-info/PKG-INFO` & `aligo-6.1.0/src/aligo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.0.6
+Version: 6.1.0
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
@@ -115,14 +115,29 @@
 ```
 
 ## 如何彻底删除文件？
 > 无需先移动文件到回收站
 
 此功能太危险，**aligo** 未直接提供。不过 [这里](https://github.com/foyoux/aligo/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E5%8A%9F%E8%83%BD---%E5%BD%BB%E5%BA%95%E5%88%A0%E9%99%A4%E6%96%87%E4%BB%B6) 扩展了该功能，请小心使用！
 
+## 如何操作资源盘
+
+```python
+from aligo import Aligo
+
+if __name__ == '__main__':
+    ali = Aligo()
+    drives = ali.list_my_drives()
+    resource_drive_id = [drive.drive_id for drive in drives if drive.drive_name == 'resource'][0]
+    ll = ali.get_file_list(drive_id=resource_drive_id)
+    for i in ll:
+        print(i)
+
+```
+
 
 ## 关于扩展功能
 
 一般步骤：
 
     1. 使用浏览器或其他抓包工具，观察通信过程；
     2. 获取 url/path + 请求体；
```

### Comparing `aligo-6.0.6/src/aligo.egg-info/SOURCES.txt` & `aligo-6.1.0/src/aligo.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -162,41 +162,42 @@
 src/aligo/types/BaseAlbum.py
 src/aligo/types/BaseDrive.py
 src/aligo/types/BaseFile.py
 src/aligo/types/BaseShareFile.py
 src/aligo/types/BaseUser.py
 src/aligo/types/CroppingBoundary.py
 src/aligo/types/CroppingSuggestionItem.py
-src/aligo/types/DataClass.py
 src/aligo/types/DriveCapacityDetail.py
 src/aligo/types/DriveFile.py
 src/aligo/types/EMailConfig.py
 src/aligo/types/Enum.py
 src/aligo/types/FaceThumbnail.py
 src/aligo/types/FieldsInfo.py
 src/aligo/types/FolderSizeInfo.py
 src/aligo/types/ImageMedia.py
 src/aligo/types/ImageQuality.py
 src/aligo/types/ImageTag.py
 src/aligo/types/ListAlbumItem.py
 src/aligo/types/LoginDevice.py
-src/aligo/types/LoginTimout.py
 src/aligo/types/MediaTransCodeTemplate.py
 src/aligo/types/Null.py
 src/aligo/types/PersonalRightsInfo.py
 src/aligo/types/PersonalSpaceInfo.py
 src/aligo/types/Privilege.py
 src/aligo/types/RateLimit.py
 src/aligo/types/ShareLinkBaseFile.py
 src/aligo/types/ShareLinkSchema.py
 src/aligo/types/SystemTag.py
 src/aligo/types/Token.py
+src/aligo/types/Type.py
 src/aligo/types/UploadPartInfo.py
 src/aligo/types/UserConfig.py
 src/aligo/types/VideoMedia.py
 src/aligo/types/VideoMediaAudioStream.py
 src/aligo/types/VideoMediaVideoStream.py
 src/aligo/types/VideoPreview.py
 src/aligo/types/VideoPreviewPlayInfo.py
 src/aligo/types/VideoPreviewSprite.py
 src/aligo/types/VideoTranscodeTemplate.py
-src/aligo/types/__init__.py
+src/aligo/types/__init__.py
+src/aligo/utils/LoginTimout.py
+src/aligo/utils/__init__.py
```

