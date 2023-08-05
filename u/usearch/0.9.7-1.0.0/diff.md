# Comparing `tmp/usearch-0.9.7-cp39-cp39-manylinux_2_28_x86_64.whl.zip` & `tmp/usearch-1.0.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,15 @@
-Zip file size: 280689 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 22:22 usearch/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 22:22 usearch-0.9.7.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 22:22 usearch./
--rwxr-xr-x  2.0 unx   450521 b- defN 23-May-26 22:22 usearch/index.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     4207 b- defN 23-May-26 22:22 usearch/client.py
--rw-r--r--  2.0 unx     4075 b- defN 23-May-26 22:22 usearch/server.py
--rw-r--r--  2.0 unx     2231 b- defN 23-May-26 22:22 usearch/io.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-26 22:22 usearch/__init__.py
--rw-r--r--  2.0 unx        8 b- defN 23-May-26 22:22 usearch-0.9.7.dist-info/top_level.txt
--rw-r--r--  2.0 unx    11357 b- defN 23-May-26 22:22 usearch-0.9.7.dist-info/LICENSE
--rw-rw-r--  2.0 unx      886 b- defN 23-May-26 22:22 usearch-0.9.7.dist-info/RECORD
--rw-r--r--  2.0 unx    19393 b- defN 23-May-26 22:22 usearch-0.9.7.dist-info/METADATA
--rw-r--r--  2.0 unx      112 b- defN 23-May-26 22:22 usearch-0.9.7.dist-info/WHEEL
--rwxr-xr-x  2.0 unx   253289 b- defN 23-May-26 22:22 usearch./libgomp-2c51bfab.so.1.0.0
-14 files, 746079 bytes uncompressed, 278915 bytes compressed:  62.6%
+Zip file size: 211992 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-05 14:15 usearch/__init__.py
+-rw-rw-rw-  2.0 fat     4241 b- defN 23-Aug-05 14:15 usearch/client.py
+-rw-rw-rw-  2.0 fat   436736 b- defN 23-Aug-05 14:22 usearch/compiled.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    14953 b- defN 23-Aug-05 14:15 usearch/eval.py
+-rw-rw-rw-  2.0 fat    34478 b- defN 23-Aug-05 14:15 usearch/index.py
+-rw-rw-rw-  2.0 fat     3274 b- defN 23-Aug-05 14:15 usearch/io.py
+-rw-rw-rw-  2.0 fat     4100 b- defN 23-Aug-05 14:15 usearch/numba.py
+-rw-rw-rw-  2.0 fat     3858 b- defN 23-Aug-05 14:15 usearch/server.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Aug-05 14:22 usearch-1.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    16401 b- defN 23-Aug-05 14:22 usearch-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-05 14:22 usearch-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Aug-05 14:22 usearch-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      993 b- defN 23-Aug-05 14:22 usearch-1.0.0.dist-info/RECORD
+13 files, 530700 bytes uncompressed, 210368 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -1,43 +1,40 @@
-Filename: usearch/
-Comment: 
-
-Filename: usearch-0.9.7.dist-info/
+Filename: usearch/__init__.py
 Comment: 
 
-Filename: usearch./
+Filename: usearch/client.py
 Comment: 
 
-Filename: usearch/index.cpython-39-x86_64-linux-gnu.so
+Filename: usearch/compiled.cp39-win_amd64.pyd
 Comment: 
 
-Filename: usearch/client.py
+Filename: usearch/eval.py
 Comment: 
 
-Filename: usearch/server.py
+Filename: usearch/index.py
 Comment: 
 
 Filename: usearch/io.py
 Comment: 
 
-Filename: usearch/__init__.py
+Filename: usearch/numba.py
 Comment: 
 
-Filename: usearch-0.9.7.dist-info/top_level.txt
+Filename: usearch/server.py
 Comment: 
 
-Filename: usearch-0.9.7.dist-info/LICENSE
+Filename: usearch-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: usearch-0.9.7.dist-info/RECORD
+Filename: usearch-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: usearch-0.9.7.dist-info/METADATA
+Filename: usearch-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: usearch-0.9.7.dist-info/WHEEL
+Filename: usearch-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: usearch./libgomp-2c51bfab.so.1.0.0
+Filename: usearch-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## usearch/client.py

```diff
@@ -1,127 +1,124 @@
-from typing import Union, Optional
-
-import numpy as np
-from ucall.client import Client
-
-
-def _vector_to_ascii(vector: np.ndarray) -> Optional[str]:
-    if vector.dtype != np.int8 and vector.dtype != np.uint8 and vector.dtype != np.byte:
-        return None
-    if not np.all((vector >= 0) | (vector <= 100)):
-        return None
-
-    # Let's map [0, 100] to the range from [23, 123],
-    # poking 60 and replacing with the 124.
-    vector += 23
-    vector[vector == 60] = 124
-    ascii = str(vector)
-    return ascii
-
-
-Triplet = tuple[np.ndarray, np.ndarray, np.ndarray]
-
-
-class IndexClient:
-
-    def __init__(
-            self,
-            uri: str = '127.0.0.1',
-            port: int = 8545,
-            use_http: bool = True) -> None:
-        self.client = Client(uri=uri, port=port, use_http=use_http)
-
-    def add_one(self, label: int, vector: np.ndarray):
-        assert isinstance(label, int)
-        assert isinstance(vector, np.ndarray)
-        vector = vector.flatten()
-        ascii = _vector_to_ascii(vector)
-        if ascii:
-            self.client.add_ascii(label=label, string=ascii)
-        else:
-            self.client.add_one(label=label, vectors=vector)
-
-    def add_many(self, labels: np.ndarray, vectors: np.ndarray):
-        assert isinstance(labels, int)
-        assert isinstance(vectors, np.ndarray)
-        assert labels.ndim == 1 and vectors.ndim == 2
-        assert labels.shape[0] == vectors.shape[0]
-        self.client.add_many(labels=labels, vectors=vectors)
-
-    def add(self, labels: Union[np.ndarray, int], vectors: np.ndarray):
-        if isinstance(labels, int) or len(labels) == 1:
-            return self.add_one(labels, vectors)
-        else:
-            return self.add_many(labels, vectors)
-
-    def search_one(self, vector: np.ndarray, count: int) -> Triplet:
-        matches: list[dict] = []
-        vector = vector.flatten()
-        ascii = _vector_to_ascii(vector)
-        if ascii:
-            matches = self.client.search_ascii(string=ascii, count=count)
-        else:
-            matches = self.client.search_one(vector=vector, count=count)
-
-        print(matches.data)
-        matches = matches.json
-
-        labels = np.array((1, count), dtype=np.uint32)
-        distances = np.array((1, count), dtype=np.float32)
-        counts = np.array((1), dtype=np.uint32)
-        for col, result in enumerate(matches):
-            labels[0, col] = result['label']
-            distances[0, col] = result['distance']
-        counts[0] = len(matches)
-
-        return labels, distances, counts
-
-    def search_many(self, vectors: np.ndarray, count: int) -> Triplet:
-        batch_size: int = vectors.shape[0]
-        list_of_matches: list[list[dict]] = self.client.search_many(
-            vectors=vectors, count=count)
-
-        labels = np.array((batch_size, count), dtype=np.uint32)
-        distances = np.array((batch_size, count), dtype=np.float32)
-        counts = np.array((batch_size), dtype=np.uint32)
-        for row, matches in enumerate(list_of_matches):
-            for col, result in enumerate(matches):
-                labels[row, col] = result['label']
-                distances[row, col] = result['distance']
-            counts[row] = len(results)
-
-        return labels, distances, counts
-
-    def search(self, vectors: np.ndarray, count: int) -> Triplet:
-        if vectors.ndim == 1 or (vectors.ndim == 2 and vectors.shape[0] == 1):
-            return self.search_one(vectors, count)
-        else:
-            return self.search_many(vectors, count)
-
-    def __len__(self):
-        return self.client.size().json()
-
-    @property
-    def ndim(self):
-        return self.client.ndim().json()
-
-    def capacity(self):
-        return self.client.capacity().json()
-
-    def connectivity(self):
-        return self.client.connectivity().json()
-
-    def load(self, path: str):
-        raise NotImplementedError()
-
-    def view(self, path: str):
-        raise NotImplementedError()
-
-    def save(self, path: str):
-        raise NotImplementedError()
-
-
-if __name__ == '__main__':
-    index = IndexClient()
-    index.add(42, np.array([0.4] * 256, dtype=np.float32))
-    results = index.search(np.array([0.4] * 256, dtype=np.float32), 10)
-    print(results)
+from typing import Union, Optional, List
+
+import numpy as np
+from ucall.client import Client
+
+from usearch.index import Matches
+
+
+def _vector_to_ascii(vector: np.ndarray) -> Optional[str]:
+    if vector.dtype != np.int8 and vector.dtype != np.uint8 and vector.dtype != np.byte:
+        return None
+    if not np.all((vector >= 0) | (vector <= 100)):
+        return None
+
+    # Let's map [0, 100] to the range from [23, 123],
+    # poking 60 and replacing with the 124.
+    vector += 23
+    vector[vector == 60] = 124
+    ascii = str(vector)
+    return ascii
+
+
+class IndexClient:
+    def __init__(
+        self, uri: str = "127.0.0.1", port: int = 8545, use_http: bool = True
+    ) -> None:
+        self.client = Client(uri=uri, port=port, use_http=use_http)
+
+    def add_one(self, key: int, vector: np.ndarray):
+        assert isinstance(key, int)
+        assert isinstance(vector, np.ndarray)
+        vector = vector.flatten()
+        ascii = _vector_to_ascii(vector)
+        if ascii:
+            self.client.add_ascii(key=key, string=ascii)
+        else:
+            self.client.add_one(key=key, vectors=vector)
+
+    def add_many(self, keys: np.ndarray, vectors: np.ndarray):
+        assert isinstance(keys, int)
+        assert isinstance(vectors, np.ndarray)
+        assert keys.ndim == 1 and vectors.ndim == 2
+        assert keys.shape[0] == vectors.shape[0]
+        self.client.add_many(keys=keys, vectors=vectors)
+
+    def add(self, keys: Union[np.ndarray, int], vectors: np.ndarray):
+        if isinstance(keys, int) or len(keys) == 1:
+            return self.add_one(keys, vectors)
+        else:
+            return self.add_many(keys, vectors)
+
+    def search_one(self, vector: np.ndarray, count: int) -> Matches:
+        matches: List[dict] = []
+        vector = vector.flatten()
+        ascii = _vector_to_ascii(vector)
+        if ascii:
+            matches = self.client.search_ascii(string=ascii, count=count)
+        else:
+            matches = self.client.search_one(vector=vector, count=count)
+
+        print(matches.data)
+        matches = matches.json
+
+        keys = np.array((1, count), dtype=np.uint32)
+        distances = np.array((1, count), dtype=np.float32)
+        counts = np.array((1), dtype=np.uint32)
+        for col, result in enumerate(matches):
+            keys[0, col] = result["key"]
+            distances[0, col] = result["distance"]
+        counts[0] = len(matches)
+
+        return keys, distances, counts
+
+    def search_many(self, vectors: np.ndarray, count: int) -> Matches:
+        batch_size: int = vectors.shape[0]
+        list_of_matches: List[List[dict]] = self.client.search_many(
+            vectors=vectors, count=count
+        )
+
+        keys = np.array((batch_size, count), dtype=np.uint32)
+        distances = np.array((batch_size, count), dtype=np.float32)
+        counts = np.array((batch_size), dtype=np.uint32)
+        for row, matches in enumerate(list_of_matches):
+            for col, result in enumerate(matches):
+                keys[row, col] = result["key"]
+                distances[row, col] = result["distance"]
+            counts[row] = len(results)
+
+        return keys, distances, counts
+
+    def search(self, vectors: np.ndarray, count: int) -> Matches:
+        if vectors.ndim == 1 or (vectors.ndim == 2 and vectors.shape[0] == 1):
+            return self.search_one(vectors, count)
+        else:
+            return self.search_many(vectors, count)
+
+    def __len__(self):
+        return self.client.size().json()
+
+    @property
+    def ndim(self):
+        return self.client.ndim().json()
+
+    def capacity(self):
+        return self.client.capacity().json()
+
+    def connectivity(self):
+        return self.client.connectivity().json()
+
+    def load(self, path: str):
+        raise NotImplementedError()
+
+    def view(self, path: str):
+        raise NotImplementedError()
+
+    def save(self, path: str):
+        raise NotImplementedError()
+
+
+if __name__ == "__main__":
+    index = IndexClient()
+    index.add(42, np.array([0.4] * 256, dtype=np.float32))
+    results = index.search(np.array([0.4] * 256, dtype=np.float32), 10)
+    print(results)
```

## usearch/server.py

```diff
@@ -1,136 +1,137 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-import os
-import argparse
-import numpy as np
-
-from ucall.rich_posix import Server
-from usearch.index import Index
-
-Triplet = tuple[np.ndarray, np.ndarray, np.ndarray]
-
-
-def _results_to_json(results: Triplet, row: int) -> list[dict]:
-
-    count = results[2][row]
-    labels = results[0][row, :count]
-    distances = results[1][row, :count]
-    return [{'label': int(label), 'distance': float(distance)}
-            for label, distance in zip(labels, distances)]
-
-
-def _ascii_to_vector(string: str) -> np.ndarray:
-    """
-    WARNING: A dirty performance hack!
-    Assuming the `f8` vectors in our implementations are just integers,
-    and generally contain scalars in the [0, 100] range, we can transmit
-    them as JSON-embedded strings. The only symbols we must avoid are
-    the double-quote '"' (code 22) and backslash '\' (code 60).
-    Printable ASCII characters are in [20, 126].
-    """
-    vector = np.array(string, dtype=np.int8)
-    vector[vector == 124] = 60
-    vector -= 23
-    return vector
-
-
-def serve(
-        ndim_: int, metric: str = 'ip',
-        port: int = 8545, threads: int = 1,
-        path: str = 'index.usearch', immutable: bool = False):
-
-    server = Server(port=port)
-    index = Index(ndim=ndim_, metric=metric)
-
-    if os.path.exists(path):
-        if immutable:
-            index.view(path)
-        else:
-            index.load(path)
-
-    @server
-    def size() -> int:
-        return len(index)
-
-    @server
-    def ndim() -> int:
-        return index.ndim
-
-    @server
-    def capacity() -> int:
-        return index.capacity()
-
-    @server
-    def connectivity() -> int:
-        return index.connectivity()
-
-    @server
-    def add_one(label: int, vector: np.ndarray):
-        print('adding', label, vector)
-        labels = np.array([label], dtype=np.longlong)
-        vectors = vector.flatten().reshape(vector.shape[0], 1)
-        index.add(labels, vectors)
-
-    @server
-    def add_many(labels: np.ndarray, vectors: np.ndarray):
-        labels = labels.astype(np.longlong)
-        index.add(labels, vectors, threads=threads)
-
-    @server
-    def search_one(vector: np.ndarray, count: int) -> list[dict]:
-        print('search', vector, count)
-        vectors = vector.reshape(vector.shape[0], 1)
-        results = index.search(vectors, count)
-        return _results_to_json(results, 0)
-
-    @server
-    def search_many(vectors: np.ndarray, count: int) -> list[list[dict]]:
-        results = index.search(vectors, count)
-        return [_results_to_json(results, i) for i in range(vectors.shape[0])]
-
-    @server
-    def add_ascii(label: int, string: str):
-        return add_one(label, _ascii_to_vector(string))
-
-    @server
-    def search_ascii(string: str, count: int):
-        return search_one(_ascii_to_vector(string), count)
-
-    try:
-        server.run()
-    except KeyboardInterrupt:
-        if not immutable:
-            index.save(path)
-
-
-if __name__ == '__main__':
-
-    parser = argparse.ArgumentParser()
-    parser.add_argument('-v', '--verbose', help='log server activity')
-    parser.add_argument(
-        '--ndim', type=int,
-        help='dimensionality of the vectors')
-    parser.add_argument(
-        '--immutable', type=bool, default=False,
-        help='the index can not be updated')
-
-    parser.add_argument(
-        '--metric', type=str, default='ip', choices=['ip', 'cos', 'l2sq', 'haversine'],
-        help='distance function to compare vectors')
-    parser.add_argument(
-        '-p', '--port', type=int, default=8545,
-        help='port to open for client connections')
-    parser.add_argument(
-        '-j', '--threads', type=int, default=1,
-        help='number of CPU threads to use')
-    parser.add_argument(
-        '--path', type=str, default='index.usearch',
-        help='where to store the index')
-
-    args = parser.parse_args()
-    assert args.ndim is not None, 'Define the number of dimensions!'
-    serve(
-        ndim_=args.ndim, metric=args.metric,
-        threads=args.threads, port=args.port,
-        path=args.path, immutable=args.immutable)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+import os
+import argparse
+import numpy as np
+from typing import List
+
+from ucall.rich_posix import Server
+from usearch.index import Index, Matches, Key
+
+
+def _ascii_to_vector(string: str) -> np.ndarray:
+    """
+    WARNING: A dirty performance hack!
+    Assuming the `i8` vectors in our implementations are just integers,
+    and generally contain scalars in the [0, 100] range, we can transmit
+    them as JSON-embedded strings. The only symbols we must avoid are
+    the double-quote '"' (code 22) and backslash '\' (code 60).
+    Printable ASCII characters are in [20, 126].
+    """
+    vector = np.array(string, dtype=np.int8)
+    vector[vector == 124] = 60
+    vector -= 23
+    return vector
+
+
+def serve(
+    ndim_: int,
+    metric: str = "ip",
+    port: int = 8545,
+    threads: int = 1,
+    path: str = "index.usearch",
+    immutable: bool = False,
+):
+    server = Server(port=port)
+    index = Index(ndim=ndim_, metric=metric)
+
+    if os.path.exists(path):
+        if immutable:
+            index.view(path)
+        else:
+            index.load(path)
+
+    @server
+    def size() -> int:
+        return len(index)
+
+    @server
+    def ndim() -> int:
+        return index.ndim
+
+    @server
+    def capacity() -> int:
+        return index.capacity()
+
+    @server
+    def connectivity() -> int:
+        return index.connectivity()
+
+    @server
+    def add_one(key: int, vector: np.ndarray):
+        print("adding", key, vector)
+        keys = np.array([key], dtype=Key)
+        vectors = vector.flatten().reshape(vector.shape[0], 1)
+        index.add(keys, vectors)
+
+    @server
+    def add_many(keys: np.ndarray, vectors: np.ndarray):
+        index.add(keys, vectors, threads=threads)
+
+    @server
+    def search_one(vector: np.ndarray, count: int) -> List[dict]:
+        print("search", vector, count)
+        vectors = vector.reshape(vector.shape[0], 1)
+        results: Matches = index.search(vectors, count)
+        return results.to_list()
+
+    @server
+    def search_many(vectors: np.ndarray, count: int) -> List[List[dict]]:
+        results: Matches = index.search(vectors, count)
+        return results.to_list()
+
+    @server
+    def add_ascii(key: int, string: str):
+        return add_one(key, _ascii_to_vector(string))
+
+    @server
+    def search_ascii(string: str, count: int):
+        return search_one(_ascii_to_vector(string), count)
+
+    try:
+        server.run()
+    except KeyboardInterrupt:
+        if not immutable:
+            index.save(path)
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser()
+    parser.add_argument("-v", "--verbose", help="log server activity")
+    parser.add_argument("--ndim", type=int, help="dimensionality of the vectors")
+    parser.add_argument(
+        "--immutable", type=bool, default=False, help="the index can not be updated"
+    )
+
+    parser.add_argument(
+        "--metric",
+        type=str,
+        default="ip",
+        choices=["ip", "cos", "l2sq", "haversine"],
+        help="distance function to compare vectors",
+    )
+    parser.add_argument(
+        "-p",
+        "--port",
+        type=int,
+        default=8545,
+        help="port to open for client connections",
+    )
+    parser.add_argument(
+        "-j", "--threads", type=int, default=1, help="number of CPU threads to use"
+    )
+    parser.add_argument(
+        "--path", type=str, default="index.usearch", help="where to store the index"
+    )
+
+    args = parser.parse_args()
+    assert args.ndim is not None, "Define the number of dimensions!"
+    serve(
+        ndim_=args.ndim,
+        metric=args.metric,
+        threads=args.threads,
+        port=args.port,
+        path=args.path,
+        immutable=args.immutable,
+    )
```

## usearch/io.py

```diff
@@ -1,67 +1,113 @@
-import struct
-import numpy as np
-
-
-def load_matrix(filename: str, start_row: int = 0, count_rows: int = None, view: bool = False):
-    """
-    Read *.ibin, *.hbin, *.fbin, *.dbin files with matrixes.
-    Args:
-        :param filename (str): path to the matrix file
-        :param start_row (int): start reading vectors from this index
-        :param count_rows (int): number of vectors to read. If None, read all vectors
-    Returns:
-        Parsed matrix (numpy.ndarray)
-    """
-    dtype = np.float32
-    scalar_size = 4
-    if filename.endswith('.fbin'):
-        dtype = np.float32
-        scalar_size = 4
-    elif filename.endswith('.dbin'):
-        dtype = np.float64
-        scalar_size = 8
-    elif filename.endswith('.hbin'):
-        dtype = np.float16
-        scalar_size = 2
-    elif filename.endswith('.ibin'):
-        dtype = np.int32
-        scalar_size = 4
-    else:
-        raise Exception('Unknown file type')
-
-    with open(filename, 'rb') as f:
-        rows, cols = np.fromfile(f, count=2, dtype=np.int32)
-        rows = (rows - start_row) if count_rows is None else count_rows
-        row_offset = start_row * scalar_size * cols
-
-        if view:
-            return np.memmap(f, dtype=dtype, mode='r', offset=8+row_offset, shape=(rows, cols))
-        else:
-            return np.fromfile(f, count=rows * cols, dtype=dtype, offset=row_offset).reshape(rows, cols)
-
-
-def save_matrix(vecs: np.array, filename: str):
-    """
-    Write *.ibin, *.hbin, *.fbin, *.dbin files with matrixes.
-    Args:
-        :param vecs (numpy.array): the matrix to serialize
-        :param filename (str): path to the matrix file
-    """
-    dtype = np.float32
-    if filename.endswith('.fbin'):
-        dtype = np.float32
-    elif filename.endswith('.dbin'):
-        dtype = np.float64
-    elif filename.endswith('.hbin'):
-        dtype = np.float16
-    elif filename.endswith('.ibin'):
-        dtype = np.int32
-    else:
-        raise Exception('Unknown file type')
-
-    assert len(vecs.shape) == 2, 'Input array must have 2 dimensions'
-    with open(filename, 'wb') as f:
-        nvecs, dim = vecs.shape
-        f.write(struct.pack('<i', nvecs))
-        f.write(struct.pack('<i', dim))
-        vecs.astype(dtype).flatten().tofile(f)
+import os
+import struct
+import typing
+
+import numpy as np
+
+
+def numpy_scalar_size(dtype) -> int:
+    return {
+        np.float64: 8,
+        np.int64: 8,
+        np.uint64: 8,
+        np.float32: 4,
+        np.int32: 4,
+        np.uint32: 4,
+        np.float16: 2,
+        np.int16: 2,
+        np.uint16: 2,
+        np.int8: 1,
+        np.uint8: 1,
+    }[dtype]
+
+
+def guess_numpy_dtype_from_filename(filename) -> typing.Optional[type]:
+    if filename.endswith(".fbin"):
+        return np.float32
+    elif filename.endswith(".dbin"):
+        return np.float64
+    elif filename.endswith(".hbin"):
+        return np.float16
+    elif filename.endswith(".ibin"):
+        return np.int32
+    elif filename.endswith(".bbin"):
+        return np.uint8
+    else:
+        return None
+
+
+def load_matrix(
+    filename: str,
+    start_row: int = 0,
+    count_rows: int = None,
+    view: bool = False,
+    dtype: typing.Optional[type] = None,
+) -> typing.Optional[np.ndarray]:
+    """Read *.ibin, *.bbib, *.hbin, *.fbin, *.dbin files with matrices.
+
+    :param filename: path to the matrix file
+    :param start_row: start reading vectors from this index
+    :param count_rows: number of vectors to read. If None, read all vectors
+    :param view: set to `True` to memory-map the file instead of loading to RAM
+
+    :return: parsed matrix
+    :rtype: numpy.ndarray
+    """
+    if dtype is None:
+        dtype = guess_numpy_dtype_from_filename(filename)
+        if dtype is None:
+            raise Exception("Unknown file type")
+    scalar_size = numpy_scalar_size(dtype)
+
+    if not os.path.exists(filename):
+        return None
+
+    with open(filename, "rb") as f:
+        rows, cols = np.fromfile(f, count=2, dtype=np.int32)
+        rows = (rows - start_row) if count_rows is None else count_rows
+        row_offset = start_row * scalar_size * cols
+
+        if view:
+            return np.memmap(
+                f,
+                dtype=dtype,
+                mode="r",
+                offset=8 + row_offset,
+                shape=(rows, cols),
+            )
+        else:
+            return np.fromfile(
+                f,
+                count=rows * cols,
+                dtype=dtype,
+                offset=row_offset,
+            ).reshape(rows, cols)
+
+
+def save_matrix(vectors: np.ndarray, filename: str):
+    """Write *.ibin, *.bbib, *.hbin, *.fbin, *.dbin files with matrices.
+
+    :param vectors: the matrix to serialize
+    :type vectors: numpy.ndarray
+    :param filename: path to the matrix file
+    :type filename: str
+    """
+    if filename.endswith(".fbin"):
+        dtype = np.float32
+    elif filename.endswith(".dbin"):
+        dtype = np.float64
+    elif filename.endswith(".hbin"):
+        dtype = np.float16
+    elif filename.endswith(".ibin"):
+        dtype = np.int32
+    elif filename.endswith(".bbin"):
+        dtype = np.uint8
+    else:
+        dtype = vectors.dtype
+
+    assert len(vectors.shape) == 2, "Input array must have 2 dimensions"
+    with open(filename, "wb") as f:
+        count, dim = vectors.shape
+        f.write(struct.pack("<i", count))
+        f.write(struct.pack("<i", dim))
+        vectors.astype(dtype).flatten().tofile(f)
```

## Comparing `usearch-0.9.7.dist-info/LICENSE` & `usearch-1.0.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `usearch-0.9.7.dist-info/RECORD` & `usearch-1.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-usearch/index.cpython-39-x86_64-linux-gnu.so,sha256=TDvZkWg-sdlJyAJKRcInrL5yv_yurp0c_qArHtgmh6Y,450521
-usearch/client.py,sha256=zDhVmFQA99xi2X3h_JnhQ-mobx-51bJdcNFjbK7tDiA,4207
-usearch/server.py,sha256=nwOEstNJtEv4K9n-Blio9VGWkhVA7ZvHTh1ZUor8dno,4075
-usearch/io.py,sha256=RXeDDzH6Y2-7q7kIKv1fXQWgeYVyp3VpDns3M0aHYoI,2231
-usearch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-usearch-0.9.7.dist-info/top_level.txt,sha256=zFbid1SmQjk8RsbEgpqF7tTjgWdFvE2z0e1LQ2hKdPg,8
-usearch-0.9.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-usearch-0.9.7.dist-info/RECORD,,
-usearch-0.9.7.dist-info/METADATA,sha256=1izt4Fbuwv0iOTbiWo3POIS8wwOxh3NTGfOXMAzDNt0,19393
-usearch-0.9.7.dist-info/WHEEL,sha256=9XLhiVgNKmXDaCDhb12mWbAUBxzBeaB96RRFqZ-6gpw,112
-usearch./libgomp-2c51bfab.so.1.0.0,sha256=imIpWFhj6TDsKK3vSE1pMgyytX7howKopJy2HWrBk2U,253289
+usearch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+usearch/client.py,sha256=DcqPCZi15fMPd4Y9jXWSoRCp1fbjiOcnFmOO3lFe8f4,4241
+usearch/compiled.cp39-win_amd64.pyd,sha256=-arbDVEci7K5ane38a7PH-aNnIcwS38-lQ2uiE-L4-g,436736
+usearch/eval.py,sha256=rw4R7qPm_E85xSIijE8MsQElEZh-Xa7EoJBrdIx0TCY,14953
+usearch/index.py,sha256=PCPYYOCliBGv8rYB-Jx5neM042scwJ6fB0izCQCP5PI,34478
+usearch/io.py,sha256=dmx9xq04E691BDE8-kASLZ93iCi5rEdxhEk61BKm0gI,3274
+usearch/numba.py,sha256=qkdzziRfE1p7VPi7rxUcllli6iiyx2eR9krc3o3UTvY,4100
+usearch/server.py,sha256=RVl5pXZQXs80MzmYaTMU9Wg9pH0maWmh3tiF22pj4OI,3858
+usearch-1.0.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+usearch-1.0.0.dist-info/METADATA,sha256=GX6P9pl3rNpmlQnljmKSDoVmsO0QHmVxxydKCNYa2fc,16401
+usearch-1.0.0.dist-info/WHEEL,sha256=6LUvBh8thwnyqgVgCADtj3fTB0_JYWDpaYISzieo71U,100
+usearch-1.0.0.dist-info/top_level.txt,sha256=zFbid1SmQjk8RsbEgpqF7tTjgWdFvE2z0e1LQ2hKdPg,8
+usearch-1.0.0.dist-info/RECORD,,
```

