# Comparing `tmp/algoritmo_gpt-0.0.1.tar.gz` & `tmp/algoritmo_gpt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algoritmo_gpt-0.0.1.tar", max compression
+gzip compressed data, was "algoritmo_gpt-0.1.0.tar", max compression
```

## Comparing `algoritmo_gpt-0.0.1.tar` & `algoritmo_gpt-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-08-04 22:09:14.944878 algoritmo_gpt-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-08-04 22:09:14.944878 algoritmo_gpt-0.0.1/algoritmo_gpt/__init__.py
--rw-r--r--   0        0        0      328 2023-08-04 22:09:45.264836 algoritmo_gpt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 algoritmo_gpt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-04 22:09:14.944878 algoritmo_gpt-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 22:09:14.944878 algoritmo_gpt-0.1.0/algoritmo_gpt/__init__.py
+-rw-r--r--   0        0        0      328 2023-08-04 22:09:30.288857 algoritmo_gpt-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      357 1970-01-01 00:00:00.000000 algoritmo_gpt-0.1.0/PKG-INFO
```

