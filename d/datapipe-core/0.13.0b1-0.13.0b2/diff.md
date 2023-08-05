# Comparing `tmp/datapipe_core-0.13.0b1.tar.gz` & `tmp/datapipe_core-0.13.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapipe_core-0.13.0b1.tar", max compression
+gzip compressed data, was "datapipe_core-0.13.0b2.tar", max compression
```

## Comparing `datapipe_core-0.13.0b1.tar` & `datapipe_core-0.13.0b2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.0b1/LICENSE
--rw-r--r--   0        0        0      779 2023-07-30 16:02:08.285417 datapipe_core-0.13.0b1/README.md
--rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.0b1/datapipe/__init__.py
--rw-r--r--   0        0        0    16171 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/cli.py
--rw-r--r--   0        0        0     9435 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/compute.py
--rw-r--r--   0        0        0    23521 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/datatable.py
--rw-r--r--   0        0        0     4649 2023-07-31 17:04:18.495884 datapipe_core-0.13.0b1/datapipe/event_logger.py
--rw-r--r--   0        0        0     1628 2023-07-30 17:16:08.720825 datapipe_core-0.13.0b1/datapipe/executor/__init__.py
--rw-r--r--   0        0        0     2183 2023-07-30 17:16:08.720825 datapipe_core-0.13.0b1/datapipe/executor/ray.py
--rw-r--r--   0        0        0     4236 2023-07-30 17:16:08.720825 datapipe_core-0.13.0b1/datapipe/lints.py
--rw-r--r--   0        0        0        0 2023-07-31 17:04:18.495884 datapipe_core-0.13.0b1/datapipe/migrations/__init__.py
--rw-r--r--   0        0        0     3081 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/migrations/v013.py
--rw-r--r--   0        0        0      969 2023-08-01 20:24:08.421185 datapipe_core-0.13.0b1/datapipe/run_config.py
--rw-r--r--   0        0        0        0 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/step/__init__.py
--rw-r--r--   0        0        0     3667 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/step/batch_generate.py
--rw-r--r--   0        0        0    34123 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/step/batch_transform.py
--rw-r--r--   0        0        0     3680 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/step/datatable_transform.py
--rw-r--r--   0        0        0     2532 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/step/update_external_table.py
--rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.0b1/datapipe/store/__init__.py
--rw-r--r--   0        0        0     8435 2023-07-30 16:02:08.295417 datapipe_core-0.13.0b1/datapipe/store/database.py
--rw-r--r--   0        0        0    18254 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/store/filedir.py
--rw-r--r--   0        0        0     3595 2023-07-30 16:02:08.295417 datapipe_core-0.13.0b1/datapipe/store/milvus.py
--rw-r--r--   0        0        0     1337 2023-07-30 16:02:08.295417 datapipe_core-0.13.0b1/datapipe/store/pandas.py
--rw-r--r--   0        0        0     8674 2023-07-30 16:02:08.295417 datapipe_core-0.13.0b1/datapipe/store/qdrant.py
--rw-r--r--   0        0        0     3209 2023-07-30 16:02:08.295417 datapipe_core-0.13.0b1/datapipe/store/redis.py
--rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.13.0b1/datapipe/store/table_store.py
--rw-r--r--   0        0        0    10104 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/datapipe/types.py
--rw-r--r--   0        0        0     2144 2023-08-02 18:09:28.809171 datapipe_core-0.13.0b1/pyproject.toml
--rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 datapipe_core-0.13.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.0b2/LICENSE
+-rw-r--r--   0        0        0      779 2023-07-30 16:02:08.285417 datapipe_core-0.13.0b2/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.0b2/datapipe/__init__.py
+-rw-r--r--   0        0        0    16171 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/cli.py
+-rw-r--r--   0        0        0     9435 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/compute.py
+-rw-r--r--   0        0        0    21593 2023-08-05 17:33:50.789530 datapipe_core-0.13.0b2/datapipe/datatable.py
+-rw-r--r--   0        0        0     4649 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/event_logger.py
+-rw-r--r--   0        0        0     1628 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/executor/__init__.py
+-rw-r--r--   0        0        0     2183 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/executor/ray.py
+-rw-r--r--   0        0        0     4236 2023-08-02 18:50:17.831640 datapipe_core-0.13.0b2/datapipe/lints.py
+-rw-r--r--   0        0        0        0 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/migrations/__init__.py
+-rw-r--r--   0        0        0     2985 2023-08-05 17:20:15.969334 datapipe_core-0.13.0b2/datapipe/migrations/v013.py
+-rw-r--r--   0        0        0      969 2023-08-01 20:24:08.421185 datapipe_core-0.13.0b2/datapipe/run_config.py
+-rw-r--r--   0        0        0     2113 2023-08-02 21:03:28.623421 datapipe_core-0.13.0b2/datapipe/sql_util.py
+-rw-r--r--   0        0        0        0 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/step/__init__.py
+-rw-r--r--   0        0        0     3667 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/step/batch_generate.py
+-rw-r--r--   0        0        0    32217 2023-08-05 17:20:15.969334 datapipe_core-0.13.0b2/datapipe/step/batch_transform.py
+-rw-r--r--   0        0        0     3680 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/step/datatable_transform.py
+-rw-r--r--   0        0        0     2548 2023-08-02 19:38:54.821220 datapipe_core-0.13.0b2/datapipe/step/update_external_table.py
+-rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.0b2/datapipe/store/__init__.py
+-rw-r--r--   0        0        0     7328 2023-08-05 17:20:15.969334 datapipe_core-0.13.0b2/datapipe/store/database.py
+-rw-r--r--   0        0        0    18254 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/store/filedir.py
+-rw-r--r--   0        0        0     3595 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/store/milvus.py
+-rw-r--r--   0        0        0     1331 2023-08-02 20:46:55.147139 datapipe_core-0.13.0b2/datapipe/store/pandas.py
+-rw-r--r--   0        0        0     8877 2023-08-05 17:17:45.446459 datapipe_core-0.13.0b2/datapipe/store/qdrant.py
+-rw-r--r--   0        0        0     3209 2023-08-02 18:17:25.319165 datapipe_core-0.13.0b2/datapipe/store/redis.py
+-rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.13.0b2/datapipe/store/table_store.py
+-rw-r--r--   0        0        0     7292 2023-08-05 17:17:45.446459 datapipe_core-0.13.0b2/datapipe/types.py
+-rw-r--r--   0        0        0     2144 2023-08-02 19:38:54.821220 datapipe_core-0.13.0b2/pyproject.toml
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 datapipe_core-0.13.0b2/PKG-INFO
```

### Comparing `datapipe_core-0.13.0b1/LICENSE` & `datapipe_core-0.13.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/README.md` & `datapipe_core-0.13.0b2/README.md`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/cli.py` & `datapipe_core-0.13.0b2/datapipe/cli.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/compute.py` & `datapipe_core-0.13.0b2/datapipe/compute.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/datatable.py` & `datapipe_core-0.13.0b2/datapipe/datatable.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 import time
 from dataclasses import dataclass
 from typing import Any, Dict, Iterator, List, Optional, Tuple, cast
 
 import pandas as pd
 from cityhash import CityHash32
 from opentelemetry import trace
-from sqlalchemy import Column, Float, Integer, Table
-from sqlalchemy.sql.expression import and_, delete, func, or_, select, text, tuple_
+from sqlalchemy import Column, Float, Integer, Table, column
+from sqlalchemy.sql.expression import and_, func, or_, select
 
 from datapipe.event_logger import EventLogger
 from datapipe.run_config import RunConfig
-from datapipe.store.database import (
-    DBConn,
-    MetaKey,
-    sql_apply_idx_filter,
+from datapipe.sql_util import (
+    sql_apply_filters_idx_to_subquery,
+    sql_apply_idx_filter_to_table,
     sql_apply_runconfig_filter,
-    sql_schema_to_sqltype,
 )
+from datapipe.store.database import DBConn, MetaKey
 from datapipe.store.table_store import TableStore
 from datapipe.types import (
     DataDF,
     DataSchema,
     IndexDF,
     MetadataDF,
     MetaSchema,
@@ -120,15 +119,17 @@
     ):
         if idx is not None:
             if len(self.primary_keys) == 0:
                 # Когда ключей нет - не делаем ничего
                 pass
 
             else:
-                sql = sql_apply_idx_filter(sql, self.sql_table, self.primary_keys, idx)
+                sql = sql_apply_idx_filter_to_table(
+                    sql, self.sql_table, self.primary_keys, idx
+                )
 
         if not include_deleted:
             sql = sql.where(self.sql_table.c.delete_ts.is_(None))
 
         return sql
 
     def get_metadata(
@@ -332,126 +333,34 @@
         return (
             cast(DataDF, new_df),
             cast(DataDF, changed_df),
             cast(MetadataDF, new_meta_df),
             cast(MetadataDF, changed_meta_df[meta_cols]),
         )
 
-    def _insert_rows(self, df: MetadataDF) -> None:
-        if len(df) > 0:
-            logger.debug(f"Inserting {len(df)} rows into {self.name} data")
-
-            with self.dbconn.con.begin() as con:
-                df.to_sql(
-                    name=self.sql_table.name,
-                    con=con,
-                    schema=self.dbconn.schema,
-                    if_exists="append",
-                    index=False,
-                    chunksize=1000,
-                    method="multi",
-                    dtype=sql_schema_to_sqltype(self.sql_schema),  # type: ignore
-                )
-
-    def _delete_rows(self, df: MetadataDF) -> None:
-        if len(df) == 0:
+    def update_rows(self, df: MetadataDF) -> None:
+        if df.empty:
             return
 
-        idx = df[self.primary_keys]
-        sql = delete(self.sql_table)
-
-        for chunk_idx in self._chunk_idx_df(idx):
-            if len(self.primary_keys) == 1:
-                # Когда ключ один - сравниваем напрямую
-                key = self.primary_keys[0]
-                chunk_sql = sql.where(
-                    self.sql_table.c[key].in_(chunk_idx[key].to_list())
-                )
-
-            else:
-                # Когда ключей много - сравниваем через tuple
-                keys: Any = tuple_(
-                    *[self.sql_table.c[key] for key in self.primary_keys]
-                )
-
-                chunk_sql = sql.where(
-                    keys.in_(
-                        [
-                            tuple([r[key] for key in self.primary_keys])  # type: ignore
-                            for r in chunk_idx.to_dict(orient="records")
-                        ]
-                    )
-                )
-
-            with self.dbconn.con.begin() as con:
-                con.execute(chunk_sql)
-
-    def _update_existing_metadata_rows(self, df: MetadataDF) -> None:
-        if len(df) == 0:
-            return
-
-        table = (
-            f"{self.dbconn.schema}.{self.sql_table.name}"
-            if self.dbconn.schema
-            else self.sql_table.name
-        )
-        values_table = f"{self.sql_table.name}_values"
-        columns = [column.name for column in self.sql_schema]  # type: ignore
-        update_columns = set(columns) - set(self.primary_keys)
-
-        update_expression = ", ".join(
-            [f"{column}={values_table}.{column}" for column in update_columns]
+        insert_sql = self.dbconn.insert(self.sql_table).values(
+            df.to_dict(orient="records")
         )
 
-        where_expressiom = " AND ".join(
-            [f"{table}.{key} = {values_table}.{key}" for key in self.primary_keys]
+        sql = insert_sql.on_conflict_do_update(
+            index_elements=self.primary_keys,
+            set_={
+                "hash": insert_sql.excluded.hash,
+                "update_ts": insert_sql.excluded.update_ts,
+                "process_ts": insert_sql.excluded.process_ts,
+                "delete_ts": insert_sql.excluded.delete_ts,
+            },
         )
 
-        for chunk_df in self._chunk_idx_df(df):
-            params_df = chunk_df.reset_index()[columns]
-            values_params = []
-            params = {}
-
-            for index, row in params_df.iterrows():
-                row_values = [
-                    f"CAST(:{column.name}_{index} AS {column.type})"  # type: ignore
-                    for column in self.sql_schema
-                ]
-                row_params = {f"{key}_{index}": row[key] for key in row.keys()}
-
-                values_params.append(f'({", ".join(row_values)})')
-                params.update(row_params)
-
-            # TODO сделать через sqlalchemy
-            stmt = text(
-                f"""
-                UPDATE {table}
-                SET {update_expression}
-                FROM (
-                    VALUES {", ".join(values_params)}
-                ) AS {values_table} ({', '.join(columns)})
-                WHERE {where_expressiom}
-            """
-            )
-
-            with self.dbconn.con.execution_options(compiled_cache=None).begin() as con:
-                con.execute(stmt, params)
-
-    # TODO объединить
-    def insert_meta_for_store_chunk(self, new_meta_df: MetadataDF) -> None:
-        if len(new_meta_df) > 0:
-            self._insert_rows(new_meta_df)
-
-    def update_meta_for_store_chunk(self, changed_meta_df: MetadataDF) -> None:
-        if len(changed_meta_df) > 0:
-            if self.dbconn.supports_update_from:
-                self._update_existing_metadata_rows(changed_meta_df)
-            else:
-                self._delete_rows(changed_meta_df)
-                self._insert_rows(changed_meta_df)
+        with self.dbconn.con.begin() as con:
+            con.execute(sql)
 
     def mark_rows_deleted(
         self,
         deleted_idx: IndexDF,
         now: Optional[float] = None,
     ) -> None:
         if len(deleted_idx) > 0:
@@ -461,15 +370,15 @@
             meta_df = self.get_metadata(deleted_idx)
 
             meta_df["hash"] = 0
             meta_df["delete_ts"] = now
             meta_df["update_ts"] = now
             meta_df["process_ts"] = now
 
-            self.update_meta_for_store_chunk(meta_df)
+            self.update_rows(meta_df)
 
     def get_stale_idx(
         self,
         process_ts: float,
         run_config: Optional[RunConfig] = None,
     ) -> Iterator[IndexDF]:
         idx_cols = [self.sql_table.c[key] for key in self.primary_keys]
@@ -486,14 +395,31 @@
 
         with self.dbconn.con.begin() as con:
             return cast(
                 Iterator[IndexDF],
                 list(pd.read_sql_query(sql, con=con, chunksize=1000)),
             )
 
+    def get_changed_rows_count_after_timestamp(
+        self,
+        ts: float,
+    ) -> int:
+        sql = select(func.count()).where(
+            and_(
+                self.sql_table.c.process_ts > ts,
+                self.sql_table.c.delete_ts.is_(None),
+            )
+        )
+
+        with self.dbconn.con.begin() as con:
+            res = con.execute(sql).fetchone()
+            assert res is not None and len(res) == 1
+
+            return res[0]
+
 
 class DataTable:
     def __init__(
         self,
         name: str,
         meta_dbconn: DBConn,
         meta_table: MetaTable,
@@ -570,16 +496,17 @@
 
                 # TODO implement transaction meckanism
                 with tracer.start_as_current_span("store data"):
                     self.table_store.insert_rows(new_df)
                     self.table_store.update_rows(changed_df)
 
                 with tracer.start_as_current_span("store metadata"):
-                    self.meta_table.insert_meta_for_store_chunk(new_meta_df)
-                    self.meta_table.update_meta_for_store_chunk(changed_meta_df)
+                    self.meta_table.update_rows(
+                        cast(MetadataDF, pd.concat([new_meta_df, changed_meta_df]))
+                    )
 
                     changes.append(data_to_index(new_df, self.primary_keys))
                     changes.append(data_to_index(changed_df, self.primary_keys))
             else:
                 data_df = pd.DataFrame(columns=self.primary_keys)
 
             with tracer.start_as_current_span("cleanup deleted rows"):
@@ -616,14 +543,48 @@
         for deleted_df in self.meta_table.get_stale_idx(
             process_ts, run_config=run_config
         ):
             deleted_idx = data_to_index(deleted_df, self.primary_keys)
 
             self.delete_by_idx(deleted_idx, now=now, run_config=run_config)
 
+    def get_agg_cte(
+        self,
+        transform_keys: List[str],
+        filters_idx: Optional[IndexDF] = None,
+        run_config: Optional[RunConfig] = None,
+    ) -> Tuple[List[str], Any]:
+        """
+        Create a CTE that aggregates the table by transform keys and returns the
+        maximum update_ts for each group.
+
+        CTE has the following columns:
+
+        * transform keys which are present in primary keys
+        * update_ts
+
+        Returns a tuple of (keys, CTE).
+        """
+
+        tbl = self.meta_table.sql_table
+
+        keys = [k for k in transform_keys if k in self.primary_keys]
+        key_cols = [column(k) for k in keys]
+
+        sql: Any = (
+            select(*key_cols + [func.max(tbl.c["update_ts"]).label("update_ts")])
+            .select_from(tbl)
+            .group_by(*key_cols)
+        )
+
+        sql = sql_apply_filters_idx_to_subquery(sql, keys, filters_idx)
+        sql = sql_apply_runconfig_filter(sql, tbl, self.primary_keys, run_config)
+
+        return (keys, sql.cte(name=f"{tbl.name}__update"))
+
 
 class DataStore:
     def __init__(
         self,
         meta_dbconn: DBConn,
         create_meta_table: bool = False,
     ) -> None:
```

### Comparing `datapipe_core-0.13.0b1/datapipe/event_logger.py` & `datapipe_core-0.13.0b2/datapipe/event_logger.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/executor/__init__.py` & `datapipe_core-0.13.0b2/datapipe/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/executor/ray.py` & `datapipe_core-0.13.0b2/datapipe/executor/ray.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/lints.py` & `datapipe_core-0.13.0b2/datapipe/lints.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/migrations/v013.py` & `datapipe_core-0.13.0b2/datapipe/migrations/v013.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,14 @@
             continue
 
         rprint(f"Migrate '{batch_transform.get_name()}': ")
         size = batch_transform.meta_table.get_metadata_size()
         if size > 0:
             print(f"Skipping -- size of metadata is greater 0: {size=}")
             continue
-        if app.ds.meta_dbconn.con.driver in ("sqlite", "pysqlite"):
-            greatest_func = func.max
-        else:
-            greatest_func = func.greatest
         output_tbls = [
             output_dt.meta_table.sql_table for output_dt in batch_transform.output_dts
         ]
 
         def make_ids_cte():
             ids_cte = (
                 select(
@@ -53,15 +49,17 @@
 
         ids_cte = make_ids_cte()
 
         sql = (
             select(
                 *[ids_cte.c[k] for k in batch_transform.transform_keys],
                 func.max(
-                    greatest_func(*[tbl.c["process_ts"] for tbl in output_tbls])
+                    app.ds.meta_dbconn.func_greatest(
+                        *[tbl.c["process_ts"] for tbl in output_tbls]
+                    )
                 ).label("process_ts"),
             )
             .select_from(ids_cte)
             .where(and_(*[tbl.c.delete_ts.is_(None) for tbl in output_tbls]))
         )
 
         for tbl in output_tbls:
```

### Comparing `datapipe_core-0.13.0b1/datapipe/run_config.py` & `datapipe_core-0.13.0b2/datapipe/run_config.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/step/batch_generate.py` & `datapipe_core-0.13.0b2/datapipe/step/batch_generate.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/step/batch_transform.py` & `datapipe_core-0.13.0b2/datapipe/step/batch_transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,35 +33,37 @@
     asc,
     column,
     desc,
     func,
     literal,
     or_,
     select,
-    tuple_,
     update,
 )
 from sqlalchemy.sql.expression import select
 from tqdm_loggable.auto import tqdm
 
 from datapipe.compute import Catalog, ComputeStep, PipelineStep
 from datapipe.datatable import DataStore, DataTable, MetaTable
 from datapipe.executor import Executor, ExecutorConfig, SingleThreadExecutor
 from datapipe.run_config import LabelDict, RunConfig
-from datapipe.store.database import DBConn, sql_apply_runconfig_filter
+from datapipe.sql_util import (
+    sql_apply_filters_idx_to_subquery,
+    sql_apply_runconfig_filter,
+)
+from datapipe.store.database import DBConn
 from datapipe.types import (
     ChangeList,
     DataDF,
     DataSchema,
     IndexDF,
     Labels,
     MetaSchema,
     TransformResult,
     data_to_index,
-    get_tables_that_have_different_intersections,
 )
 
 logger = logging.getLogger("datapipe.step.batch_transform")
 tracer = trace.get_tracer("datapipe.step.batch_transform")
 
 
 # TODO подумать, может быть мы хотим дать возможность возвращать итератор TransformResult
@@ -293,28 +295,14 @@
             primary_schema=self.transform_schema,
             create_table=ds.create_meta_table,
         )
         self.filters = filters
         self.order_by = order_by
         self.order = order
 
-        # Check that all keys are either in one input table or in all input tables
-        # Currently we do not support partial primary keys
-        tables_that_have_different_intersections = (
-            get_tables_that_have_different_intersections(
-                [dt.primary_schema for dt in self.input_dts],
-                [dt.name for dt in self.input_dts],
-            )
-        )
-        if len(tables_that_have_different_intersections) > 0:
-            raise NotImplementedError(
-                f"{self.get_name()}: Different pairwise intersection of columns in inputs tables is not supported yet."
-                f"{tables_that_have_different_intersections}"
-            )
-
     @classmethod
     def compute_transform_schema(
         cls,
         input_mts: List[MetaTable],
         output_mts: List[MetaTable],
         transform_keys: Optional[List[str]],
     ) -> Tuple[List[str], MetaSchema]:
@@ -367,57 +355,14 @@
 
         common_keys = [
             k for k, v in all_input_keys_counts.items() if v == len(self.input_dts)
         ]
 
         common_transform_keys = [k for k in self.transform_keys if k in common_keys]
 
-        # TODO move to DBConn compatiblity layer
-        if ds.meta_dbconn.con.driver in ("sqlite", "pysqlite"):
-            greatest_func = func.max
-        else:
-            greatest_func = func.greatest
-
-        def _apply_filters_idx(sql, keys, filters_idx):
-            if filters_idx is None:
-                return sql
-
-            applicable_filter_keys = [i for i in filters_idx.columns if i in keys]
-            if len(applicable_filter_keys) > 0:
-                sql = sql.where(
-                    tuple_(*[column(i) for i in applicable_filter_keys]).in_(
-                        [
-                            tuple_(*[r[k] for k in applicable_filter_keys])
-                            for r in filters_idx.to_dict(orient="records")
-                        ]
-                    )
-                )
-
-            return sql
-
-        def _make_agg_cte(
-            dt: DataTable, agg_fun, agg_col: str
-        ) -> Tuple[List[str], Any]:
-            tbl = dt.meta_table.sql_table
-
-            keys = [k for k in self.transform_keys if k in dt.primary_keys]
-            key_cols = [column(k) for k in keys]
-
-            sql: Any = (
-                select(*key_cols + [agg_fun(tbl.c[agg_col]).label(agg_col)])
-                .select_from(tbl)
-                .group_by(*key_cols)
-            )
-
-            sql = _apply_filters_idx(sql, keys, filters_idx)
-
-            sql = sql_apply_runconfig_filter(sql, tbl, dt.primary_keys, run_config)
-
-            return (keys, sql.cte(name=f"{tbl.name}__{agg_col}"))
-
         def _make_agg_of_agg(ctes, agg_col):
             assert len(ctes) > 0
 
             if len(ctes) == 1:
                 return ctes[0][1]
 
             coalesce_keys = []
@@ -431,21 +376,21 @@
                 if len(ctes_with_key) == 1:
                     coalesce_keys.append(ctes_with_key[0].c[key])
                 else:
                     coalesce_keys.append(
                         func.coalesce(*[cte.c[key] for cte in ctes_with_key]).label(key)
                     )
 
-            agg = greatest_func(*[subq.c[agg_col] for (subq_keys, subq) in ctes]).label(
-                agg_col
-            )
+            agg = ds.meta_dbconn.func_greatest(
+                *[subq.c[agg_col] for (_, subq) in ctes]
+            ).label(agg_col)
 
             _, first_cte = ctes[0]
 
-            sql = select(*coalesce_keys + [agg]).select_from(first_cte)
+            sql = select(*coalesce_keys + [agg]).distinct().select_from(first_cte)
 
             for _, cte in ctes[1:]:
                 if len(common_transform_keys) > 0:
                     sql = sql.join(
                         cte,
                         onclause=and_(
                             *[
@@ -459,38 +404,45 @@
                     sql = sql.join(
                         cte,
                         onclause=literal(True),
                     )
 
             return sql.cte(name=f"all__{agg_col}")
 
-        inp_ctes = [_make_agg_cte(tbl, func.max, "update_ts") for tbl in self.input_dts]
+        inp_ctes = [
+            tbl.get_agg_cte(
+                transform_keys=self.transform_keys,
+                filters_idx=filters_idx,
+                run_config=run_config,
+            )
+            for tbl in self.input_dts
+        ]
 
         inp = _make_agg_of_agg(inp_ctes, "update_ts")
 
         tr_tbl = self.meta_table.sql_table
         out: Any = (
             select(
                 *[column(k) for k in self.transform_keys]
                 + [tr_tbl.c.process_ts, tr_tbl.c.priority, tr_tbl.c.is_success]
             )
             .select_from(tr_tbl)
             .group_by(*[column(k) for k in self.transform_keys])
         )
 
-        out = _apply_filters_idx(out, self.transform_keys, filters_idx)
+        out = sql_apply_filters_idx_to_subquery(out, self.transform_keys, filters_idx)
 
         out = out.cte(name="transform")
 
         sql = (
             select(
                 *[
                     func.coalesce(inp.c[key], out.c[key]).label(key)
                     for key in self.transform_keys
-                ]
+                ],
             )
             .select_from(inp)
             .outerjoin(
                 out,
                 onclause=and_(
                     *[inp.c[key] == out.c[key] for key in self.transform_keys]
                 ),
@@ -886,14 +838,15 @@
 
 @dataclass
 class DatatableBatchTransform(PipelineStep):
     func: DatatableBatchTransformFunc
     inputs: List[str]
     outputs: List[str]
     chunk_size: int = 1000
+    transform_keys: Optional[List[str]] = None
     kwargs: Optional[Dict] = None
     labels: Optional[Labels] = None
 
     def build_compute(self, ds: DataStore, catalog: Catalog) -> List[ComputeStep]:
         input_dts = [catalog.get_datatable(ds, name) for name in self.inputs]
         output_dts = [catalog.get_datatable(ds, name) for name in self.outputs]
 
@@ -901,14 +854,15 @@
             DatatableBatchTransformStep(
                 ds=ds,
                 name=f"{self.func.__name__}",
                 func=self.func,
                 input_dts=input_dts,
                 output_dts=output_dts,
                 kwargs=self.kwargs,
+                transform_keys=self.transform_keys,
                 chunk_size=self.chunk_size,
                 labels=self.labels,
             )
         ]
 
 
 class DatatableBatchTransformStep(BaseBatchTransformStep):
```

### Comparing `datapipe_core-0.13.0b1/datapipe/step/datatable_transform.py` & `datapipe_core-0.13.0b2/datapipe/step/datatable_transform.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/step/update_external_table.py` & `datapipe_core-0.13.0b2/datapipe/step/update_external_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 import time
 from typing import List, Optional
 
+import pandas as pd
 from tqdm_loggable.auto import tqdm
 
 from datapipe.compute import Catalog, ComputeStep, PipelineStep
 from datapipe.datatable import DataStore, DataTable
 from datapipe.run_config import RunConfig
 from datapipe.step.datatable_transform import (
     DatatableTransformFunc,
     DatatableTransformStep,
 )
-from datapipe.types import Labels, cast
+from datapipe.types import Labels, MetadataDF, cast
 
 logger = logging.getLogger("datapipe.step.update_external_table")
 
 
 def update_external_table(
     ds: DataStore, table: DataTable, run_config: Optional[RunConfig] = None
 ) -> None:
@@ -29,16 +30,17 @@
             changed_df,
             new_meta_df,
             changed_meta_df,
         ) = table.meta_table.get_changes_for_store_chunk(ps_df, now=now)
 
         # TODO switch to iterative store_chunk and table.sync_meta_by_process_ts
 
-        table.meta_table.insert_meta_for_store_chunk(new_meta_df)
-        table.meta_table.update_meta_for_store_chunk(changed_meta_df)
+        table.meta_table.update_rows(
+            cast(MetadataDF, pd.concat([new_meta_df, changed_meta_df]))
+        )
 
     for stale_idx in table.meta_table.get_stale_idx(now, run_config=run_config):
         logger.debug(f"Deleting {len(stale_idx.index)} rows from {table.name} data")
         table.event_logger.log_state(
             table.name,
             added_count=0,
             updated_count=0,
```

### Comparing `datapipe_core-0.13.0b1/datapipe/store/database.py` & `datapipe_core-0.13.0b2/datapipe/store/database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,57 @@
 import copy
 import logging
 import math
-from typing import Any, Dict, Iterator, List, Optional, Union, cast
+from typing import Any, Iterator, List, Optional, Union, cast
 
 import pandas as pd
 from opentelemetry import trace
-from sqlalchemy import Column, Integer, MetaData, String, Table, create_engine
+from sqlalchemy import Column, MetaData, Table, create_engine, func
 from sqlalchemy.pool import QueuePool, SingletonThreadPool
 from sqlalchemy.schema import SchemaItem
-from sqlalchemy.sql.base import Executable, SchemaEventTarget
-from sqlalchemy.sql.expression import delete, select, tuple_
+from sqlalchemy.sql.base import SchemaEventTarget
+from sqlalchemy.sql.expression import delete, select
 
 from datapipe.run_config import RunConfig
+from datapipe.sql_util import sql_apply_idx_filter_to_table, sql_apply_runconfig_filter
 from datapipe.store.table_store import TableStore
-from datapipe.types import (
-    DataDF,
-    DataSchema,
-    IndexDF,
-    MetaSchema,
-    TAnyDF,
-    data_to_index,
-)
+from datapipe.types import DataDF, DataSchema, IndexDF, MetaSchema, TAnyDF
 
 logger = logging.getLogger("datapipe.store.database")
 tracer = trace.get_tracer("datapipe.store.database")
 
 
-SCHEMA_TO_DTYPE_LOOKUP = {
-    String: str,
-    Integer: int,
-}
-
-
-def sql_schema_to_dtype(schema: List[Column]) -> Dict[str, Any]:
-    return {i.name: SCHEMA_TO_DTYPE_LOOKUP[i.type.__class__] for i in schema}
-
-
-def sql_schema_to_sqltype(schema: List[Column]) -> Dict[str, Any]:
-    return {i.name: i.type for i in schema}
-
-
 class DBConn:
     def __init__(self, connstr: str, schema: Optional[str] = None):
         self._init(connstr, schema)
 
     def _init(self, connstr: str, schema: Optional[str]) -> None:
         self.connstr = connstr
         self.schema = schema
 
-        if connstr.startswith("sqlite"):
+        if connstr.startswith("sqlite") or connstr.startswith("pysqlite"):
             self.supports_update_from = False
 
             from sqlalchemy.dialects.sqlite import insert
 
             self.insert = insert
+            self.func_greatest = func.max
 
             self.con = create_engine(
                 connstr,
                 poolclass=SingletonThreadPool,
             )
         else:
             # Assume relatively new Postgres
             self.supports_update_from = True
 
             from sqlalchemy.dialects.postgresql import insert
 
             self.insert = insert
+            self.func_greatest = func.greatest
 
             self.con = create_engine(
                 connstr,
                 poolclass=QueuePool,
                 # pool_size=25,
             )
 
@@ -81,55 +63,14 @@
             "schema": self.schema,
         }
 
     def __setstate__(self, state):
         self._init(state["connstr"], state["schema"])
 
 
-def sql_apply_runconfig_filter(
-    sql: Any,
-    table: Table,
-    primary_keys: List[str],
-    run_config: Optional[RunConfig] = None,
-) -> Any:
-    if run_config is not None:
-        for k, v in run_config.filters.items():
-            if k in primary_keys:
-                sql = sql.where(table.c[k] == v)
-
-    return sql
-
-
-def sql_apply_idx_filter(
-    sql: Any,
-    table: Table,
-    primary_keys: List[str],
-    idx: IndexDF,
-) -> Any:
-    if len(primary_keys) == 1:
-        # Когда ключ один - сравниваем напрямую
-        key = primary_keys[0]
-        sql = sql.where(table.c[key].in_(idx[key].to_list()))
-
-    else:
-        # Когда ключей много - сравниваем по кортежу
-        keys = tuple_(*[table.c[key] for key in primary_keys])  # type: ignore
-
-        sql = sql.where(
-            keys.in_(
-                [
-                    tuple([r[key] for key in primary_keys])  # type: ignore
-                    for r in idx.to_dict(orient="records")
-                ]
-            )
-        )
-
-    return sql
-
-
 class MetaKey(SchemaItem):
     def __init__(self, target_name: Optional[str] = None) -> None:
         self.target_name = target_name
 
     def _set_parent(self, parent: SchemaEventTarget, **kw: Any) -> None:
         self.parent = parent
         self.parent.meta_key = self  # type: ignore
@@ -154,14 +95,18 @@
             self.dbconn = DBConn(dbconn)
         else:
             self.dbconn = dbconn
         self.name = name
 
         self.data_sql_schema = data_sql_schema
 
+        self.data_keys = [
+            column.name for column in self.data_sql_schema if not column.primary_key
+        ]
+
         self.data_table = Table(
             self.name,
             self.dbconn.sqla_metadata,
             *[copy.copy(i) for i in self.data_sql_schema],
             extend_existing=True,
         )
 
@@ -203,42 +148,45 @@
     def delete_rows(self, idx: IndexDF) -> None:
         if idx is None or len(idx.index) == 0:
             return
 
         logger.debug(f"Deleting {len(idx.index)} rows from {self.name} data")
 
         for chunk_idx in self._chunk_idx_df(idx):
-            sql = sql_apply_idx_filter(
+            sql = sql_apply_idx_filter_to_table(
                 delete(self.data_table), self.data_table, self.primary_keys, chunk_idx
             )
             with self.dbconn.con.begin() as con:
                 con.execute(sql)
 
     def insert_rows(self, df: DataDF) -> None:
+        self.update_rows(df)
+
+    def update_rows(self, df: DataDF) -> None:
         if df.empty:
             return
 
-        self.delete_rows(data_to_index(df, self.primary_keys))
-        logger.debug(f"Inserting {len(df)} rows into {self.name} data")
+        insert_sql = self.dbconn.insert(self.data_table).values(
+            df.to_dict(orient="records")
+        )
 
-        with self.dbconn.con.begin() as con:
-            for chunk_df in self._chunk_idx_df(df):
-                chunk_df.to_sql(
-                    name=self.name,
-                    con=con,
-                    schema=self.dbconn.schema,
-                    if_exists="append",
-                    index=False,
-                    chunksize=1000,
-                    method="multi",
-                    dtype=sql_schema_to_sqltype(self.data_sql_schema),
-                )
+        if len(self.data_keys) > 0:
+            sql = insert_sql.on_conflict_do_update(
+                index_elements=self.primary_keys,
+                set_={
+                    col.name: insert_sql.excluded[col.name]
+                    for col in self.data_sql_schema
+                    if not col.primary_key
+                },
+            )
+        else:
+            sql = insert_sql.on_conflict_do_nothing(index_elements=self.primary_keys)
 
-    def update_rows(self, df: DataDF) -> None:
-        self.insert_rows(df)
+        with self.dbconn.con.begin() as con:
+            con.execute(sql)
 
     # Fix numpy types in IndexDF
     def _get_sql_param(self, param):
         return param.item() if hasattr(param, "item") else param
 
     def read_rows(self, idx: Optional[IndexDF] = None) -> pd.DataFrame:
         sql = select(self.data_table.c)
@@ -250,15 +198,15 @@
                     columns=[column.name for column in self.data_sql_schema]
                 )
 
             res = []
 
             with self.dbconn.con.begin() as con:
                 for chunk_idx in self._chunk_idx_df(idx):
-                    chunk_sql = sql_apply_idx_filter(
+                    chunk_sql = sql_apply_idx_filter_to_table(
                         sql, self.data_table, self.primary_keys, chunk_idx
                     )
                     chunk_df = pd.read_sql_query(chunk_sql, con=con)
 
                     res.append(chunk_df)
 
             return pd.concat(res, ignore_index=True)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `datapipe_core-0.13.0b1/datapipe/store/filedir.py` & `datapipe_core-0.13.0b2/datapipe/store/filedir.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/store/milvus.py` & `datapipe_core-0.13.0b2/datapipe/store/milvus.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/store/pandas.py` & `datapipe_core-0.13.0b2/datapipe/store/pandas.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC
 from typing import Optional
 
 import fsspec
 import pandas as pd
 
-from datapipe.store.database import sql_schema_to_dtype
+from datapipe.sql_util import sql_schema_to_dtype
 from datapipe.store.table_store import TableDataSingleFileStore
 from datapipe.types import DataDF
 
 
 class TableStoreExcel(TableDataSingleFileStore, ABC):
     def load_file(self) -> Optional[pd.DataFrame]:
         of = fsspec.open(self.filename)
```

### Comparing `datapipe_core-0.13.0b1/datapipe/store/qdrant.py` & `datapipe_core-0.13.0b2/datapipe/store/qdrant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import hashlib
 import re
 import uuid
 from collections.abc import Iterable
-from typing import Any, Optional
+from typing import Any, Dict, List, Optional, cast
 
 import pandas as pd
 from qdrant_client import QdrantClient
 from qdrant_client.http import models as rest
 from qdrant_client.http.exceptions import UnexpectedResponse
 
 from datapipe.store.table_store import TableStore
@@ -86,15 +86,18 @@
 
         assert self.client is not None
         self.client.upsert(
             self.name,
             rest.Batch(
                 ids=self.__get_ids(df),
                 vectors=df[self.embedding_field].apply(list).to_list(),
-                payloads=df[self.paylods_filelds].to_dict(orient="records"),
+                payloads=cast(
+                    List[Dict[str, Any]],
+                    df[self.paylods_filelds].to_dict(orient="records"),
+                ),
             ),
             wait=True,
         )
 
     def update_rows(self, df: DataDF) -> None:
         self.insert_rows(df)
 
@@ -226,15 +229,18 @@
 
             assert self.client is not None
             self.client.upsert(
                 name,
                 rest.Batch(
                     ids=self.__get_ids(gdf),
                     vectors=gdf[self.embedding_field].apply(list).to_list(),
-                    payloads=gdf[self.paylods_filelds].to_dict(orient="records"),
+                    payloads=cast(
+                        List[Dict[str, Any]],
+                        df[self.paylods_filelds].to_dict(orient="records"),
+                    ),
                 ),
                 wait=True,
             )
 
     def update_rows(self, df: DataDF) -> None:
         self.insert_rows(df)
```

### Comparing `datapipe_core-0.13.0b1/datapipe/store/redis.py` & `datapipe_core-0.13.0b2/datapipe/store/redis.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/datapipe/store/table_store.py` & `datapipe_core-0.13.0b2/datapipe/store/table_store.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0b1/pyproject.toml` & `datapipe_core-0.13.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datapipe-core"
-version = "0.13.0-beta.1"
+version = "0.13.0-beta.2"
 description = "`datapipe` is a realtime incremental ETL library for Python application"
 readme = "README.md"
 repository = "https://github.com/epoch8/datapipe"
 authors = ["Andrey Tatarinov <a@tatarinov.co>"]
 packages = [
     { include = "datapipe" }
 ]
```

### Comparing `datapipe_core-0.13.0b1/PKG-INFO` & `datapipe_core-0.13.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapipe-core
-Version: 0.13.0b1
+Version: 0.13.0b2
 Summary: `datapipe` is a realtime incremental ETL library for Python application
 Home-page: https://github.com/epoch8/datapipe
 Author: Andrey Tatarinov
 Author-email: a@tatarinov.co
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

