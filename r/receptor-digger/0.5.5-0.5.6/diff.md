# Comparing `tmp/receptor_digger-0.5.5.tar.gz` & `tmp/receptor_digger-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptor_digger-0.5.5.tar", last modified: Fri Jul 14 13:17:43 2023, max compression
+gzip compressed data, was "receptor_digger-0.5.6.tar", last modified: Sat Aug  5 14:03:38 2023, max compression
```

## Comparing `receptor_digger-0.5.5.tar` & `receptor_digger-0.5.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.307877 receptor_digger-0.5.5/
--rw-rw-rw-   0        0        0      582 2023-03-27 14:56:02.000000 receptor_digger-0.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1324 2023-07-14 13:17:43.307877 receptor_digger-0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0      745 2023-07-14 13:16:56.000000 receptor_digger-0.5.5/README.md
--rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_digger-0.5.5/pyproject.toml
--rw-rw-rw-   0        0        0     1218 2023-07-14 13:17:43.308879 receptor_digger-0.5.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.170339 receptor_digger-0.5.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.209103 receptor_digger-0.5.5/src/digger/
--rw-rw-rw-   0        0        0        0 2023-03-13 09:47:31.000000 receptor_digger-0.5.5/src/digger/__init__.py
--rw-rw-rw-   0        0        0     1364 2023-03-29 15:03:23.000000 receptor_digger-0.5.5/src/digger/blastresults_to_csv.py
--rw-rw-rw-   0        0        0     3812 2023-03-26 08:44:02.000000 receptor_digger-0.5.5/src/digger/calc_motifs.py
--rw-rw-rw-   0        0        0     2169 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/cirelli_contig_matches.py
--rw-rw-rw-   0        0        0      344 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/cirelli_to_fasta.py
--rw-rw-rw-   0        0        0    12754 2023-04-06 10:39:17.000000 receptor_digger-0.5.5/src/digger/compare_annotations.py
--rw-rw-rw-   0        0        0     9824 2023-06-29 17:40:47.000000 receptor_digger-0.5.5/src/digger/dig_sequence.py
--rw-rw-rw-   0        0        0    14954 2023-07-07 16:47:51.000000 receptor_digger-0.5.5/src/digger/dig_utils.py
--rw-rw-rw-   0        0        0     8440 2023-03-28 08:13:03.000000 receptor_digger-0.5.5/src/digger/digger.py
--rw-rw-rw-   0        0        0    18565 2023-07-14 13:12:14.000000 receptor_digger-0.5.5/src/digger/find_alignments.py
--rw-rw-rw-   0        0        0     3429 2023-03-26 08:44:02.000000 receptor_digger-0.5.5/src/digger/motif.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.169336 receptor_digger-0.5.5/src/digger/motifs/
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.169336 receptor_digger-0.5.5/src/digger/motifs/human/
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.226006 receptor_digger-0.5.5/src/digger/motifs/human/IGH/
--rw-rw-rw-   0        0        0      209 2023-03-20 09:36:55.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      267 2023-03-20 09:36:55.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      209 2023-03-20 09:36:54.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      269 2023-03-20 09:36:54.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      225 2023-03-20 09:36:53.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      280 2023-03-20 09:36:54.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1409 2023-03-20 09:36:57.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      334 2023-03-20 09:36:58.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      225 2023-03-20 09:36:58.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      281 2023-03-20 09:36:58.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-04-06 10:56:41.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGH/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.238005 receptor_digger-0.5.5/src/digger/motifs/human/IGK/
--rw-rw-rw-   0        0        0      225 2023-03-22 14:52:39.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGK/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-03-22 14:52:39.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGK/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1481 2023-03-22 14:52:40.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGK/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      341 2023-03-22 14:52:40.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGK/L-PART2_prob.csv
--rw-rw-rw-   0        0        0   152815 2023-03-22 14:52:37.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv
--rw-rw-rw-   0        0        0      194 2023-03-22 14:52:40.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGK/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      234 2023-03-22 14:52:40.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGK/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGK/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.248865 receptor_digger-0.5.5/src/digger/motifs/human/IGL/
--rw-rw-rw-   0        0        0      222 2023-03-23 17:10:50.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGL/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      280 2023-03-23 17:10:50.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGL/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1410 2023-03-23 10:57:55.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGL/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      339 2023-03-23 10:57:56.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGL/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      225 2023-03-23 10:57:56.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGL/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-03-23 10:57:56.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGL/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.5/src/digger/motifs/human/IGL/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.170339 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.263878 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/
--rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1288 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      320 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      165 2023-04-04 14:13:25.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/conserved_motifs.fasta
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.281876 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/
--rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      890 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv
--rw-rw-rw-   0        0        0     1463 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      319 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      210 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      271 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0       90 2023-04-04 10:42:00.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/conserved_motifs.fasta
--rw-rw-rw-   0        0        0     8433 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/features.csv
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.298877 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/
--rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/3'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/3'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/5'D-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/5'D-NONAMER_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/J-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/J-NONAMER_prob.csv
--rw-rw-rw-   0        0        0     1397 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv
--rw-rw-rw-   0        0        0      339 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/L-PART2_prob.csv
--rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/V-HEPTAMER_prob.csv
--rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/V-NONAMER_prob.csv
--rw-rw-rw-   0        0        0       90 2023-04-04 11:10:35.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/conserved_motifs.fasta
--rw-rw-rw-   0        0        0     7674 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/features.csv
--rw-rw-rw-   0        0        0    40654 2023-06-30 09:35:41.000000 receptor_digger-0.5.5/src/digger/parse_genes.py
--rw-rw-rw-   0        0        0    14499 2023-04-01 08:42:36.000000 receptor_digger-0.5.5/src/digger/parse_imgt_annotations.py
--rw-rw-rw-   0        0        0    12271 2023-06-29 17:40:47.000000 receptor_digger-0.5.5/src/digger/search_motifs.py
--rw-rw-rw-   0        0        0      856 2023-02-06 16:38:59.000000 receptor_digger-0.5.5/src/digger/slugify.py
-drwxrwxrwx   0        0        0        0 2023-07-14 13:17:43.306876 receptor_digger-0.5.5/src/receptor_digger.egg-info/
--rw-rw-rw-   0        0        0     1324 2023-07-14 13:17:43.000000 receptor_digger-0.5.5/src/receptor_digger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4011 2023-07-14 13:17:43.000000 receptor_digger-0.5.5/src/receptor_digger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 13:17:43.000000 receptor_digger-0.5.5/src/receptor_digger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      338 2023-07-14 13:17:43.000000 receptor_digger-0.5.5/src/receptor_digger.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-07-14 13:17:43.000000 receptor_digger-0.5.5/src/receptor_digger.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-14 13:17:43.000000 receptor_digger-0.5.5/src/receptor_digger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.417208 receptor_digger-0.5.6/
+-rw-rw-rw-   0        0        0      582 2023-03-27 14:56:02.000000 receptor_digger-0.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1460 2023-08-05 14:03:38.417208 receptor_digger-0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2023-08-05 14:02:47.000000 receptor_digger-0.5.6/README.md
+-rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_digger-0.5.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1218 2023-08-05 14:03:38.418208 receptor_digger-0.5.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.180512 receptor_digger-0.5.6/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.314296 receptor_digger-0.5.6/src/digger/
+-rw-rw-rw-   0        0        0        0 2023-03-13 09:47:31.000000 receptor_digger-0.5.6/src/digger/__init__.py
+-rw-rw-rw-   0        0        0     1364 2023-03-29 15:03:23.000000 receptor_digger-0.5.6/src/digger/blastresults_to_csv.py
+-rw-rw-rw-   0        0        0     3812 2023-03-26 08:44:02.000000 receptor_digger-0.5.6/src/digger/calc_motifs.py
+-rw-rw-rw-   0        0        0     2169 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/cirelli_contig_matches.py
+-rw-rw-rw-   0        0        0      344 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/cirelli_to_fasta.py
+-rw-rw-rw-   0        0        0    12754 2023-04-06 10:39:17.000000 receptor_digger-0.5.6/src/digger/compare_annotations.py
+-rw-rw-rw-   0        0        0     9824 2023-06-29 17:40:47.000000 receptor_digger-0.5.6/src/digger/dig_sequence.py
+-rw-rw-rw-   0        0        0    14954 2023-07-07 16:47:51.000000 receptor_digger-0.5.6/src/digger/dig_utils.py
+-rw-rw-rw-   0        0        0     8440 2023-08-05 10:14:50.000000 receptor_digger-0.5.6/src/digger/digger.py
+-rw-rw-rw-   0        0        0    18562 2023-08-05 10:16:06.000000 receptor_digger-0.5.6/src/digger/find_alignments.py
+-rw-rw-rw-   0        0        0     3429 2023-03-26 08:44:02.000000 receptor_digger-0.5.6/src/digger/motif.py
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.179511 receptor_digger-0.5.6/src/digger/motifs/
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.178512 receptor_digger-0.5.6/src/digger/motifs/human/
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.331298 receptor_digger-0.5.6/src/digger/motifs/human/IGH/
+-rw-rw-rw-   0        0        0      209 2023-03-20 09:36:55.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      267 2023-03-20 09:36:55.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      209 2023-03-20 09:36:54.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      269 2023-03-20 09:36:54.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      225 2023-03-20 09:36:53.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      280 2023-03-20 09:36:54.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1409 2023-03-20 09:36:57.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      334 2023-03-20 09:36:58.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      225 2023-03-20 09:36:58.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      281 2023-03-20 09:36:58.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-04-06 10:56:41.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGH/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.342303 receptor_digger-0.5.6/src/digger/motifs/human/IGK/
+-rw-rw-rw-   0        0        0      225 2023-03-22 14:52:39.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGK/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-03-22 14:52:39.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGK/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1481 2023-03-22 14:52:40.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGK/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      341 2023-03-22 14:52:40.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGK/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0   152815 2023-03-22 14:52:37.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv
+-rw-rw-rw-   0        0        0      194 2023-03-22 14:52:40.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGK/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      234 2023-03-22 14:52:40.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGK/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGK/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.352296 receptor_digger-0.5.6/src/digger/motifs/human/IGL/
+-rw-rw-rw-   0        0        0      222 2023-03-23 17:10:50.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGL/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      280 2023-03-23 17:10:50.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGL/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1410 2023-03-23 10:57:55.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGL/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      339 2023-03-23 10:57:56.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGL/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      225 2023-03-23 10:57:56.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGL/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-03-23 10:57:56.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGL/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      117 2023-03-26 18:09:48.000000 receptor_digger-0.5.6/src/digger/motifs/human/IGL/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.180512 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.368296 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/
+-rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1288 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      320 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      165 2023-04-04 14:13:25.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/conserved_motifs.fasta
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.388208 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/
+-rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      890 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv
+-rw-rw-rw-   0        0        0     1463 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      319 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      210 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      271 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0       90 2023-04-04 10:42:00.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0     8433 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/features.csv
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.405207 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/
+-rw-rw-rw-   0        0        0      220 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/3'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      277 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/3'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      221 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/5'D-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      283 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/5'D-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/J-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/J-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0     1397 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv
+-rw-rw-rw-   0        0        0      339 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/L-PART2_prob.csv
+-rw-rw-rw-   0        0        0      226 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/V-HEPTAMER_prob.csv
+-rw-rw-rw-   0        0        0      284 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/V-NONAMER_prob.csv
+-rw-rw-rw-   0        0        0       90 2023-04-04 11:10:35.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/conserved_motifs.fasta
+-rw-rw-rw-   0        0        0     7674 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/features.csv
+-rw-rw-rw-   0        0        0    40651 2023-08-05 10:16:15.000000 receptor_digger-0.5.6/src/digger/parse_genes.py
+-rw-rw-rw-   0        0        0    14499 2023-08-05 10:15:09.000000 receptor_digger-0.5.6/src/digger/parse_imgt_annotations.py
+-rw-rw-rw-   0        0        0    12271 2023-06-29 17:40:47.000000 receptor_digger-0.5.6/src/digger/search_motifs.py
+-rw-rw-rw-   0        0        0      856 2023-02-06 16:38:59.000000 receptor_digger-0.5.6/src/digger/slugify.py
+drwxrwxrwx   0        0        0        0 2023-08-05 14:03:38.415207 receptor_digger-0.5.6/src/receptor_digger.egg-info/
+-rw-rw-rw-   0        0        0     1460 2023-08-05 14:03:38.000000 receptor_digger-0.5.6/src/receptor_digger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4011 2023-08-05 14:03:38.000000 receptor_digger-0.5.6/src/receptor_digger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 14:03:38.000000 receptor_digger-0.5.6/src/receptor_digger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      338 2023-08-05 14:03:38.000000 receptor_digger-0.5.6/src/receptor_digger.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       41 2023-08-05 14:03:38.000000 receptor_digger-0.5.6/src/receptor_digger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-05 14:03:38.000000 receptor_digger-0.5.6/src/receptor_digger.egg-info/top_level.txt
```

### Comparing `receptor_digger-0.5.5/MANIFEST.in` & `receptor_digger-0.5.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/PKG-INFO` & `receptor_digger-0.5.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receptor_digger
-Version: 0.5.5
+Version: 0.5.6
 Summary: Tools for de novo discovery of genomic germline IG and TR receptor sequences
 Home-page: https://github.com/williamdlees/digger
 Author: William Lees
 Author-email: william@lees.org.uk
 Project-URL: Bug Tracker, https://github.com/williamdlees/digger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -13,14 +13,18 @@
 Description-Content-Type: text/markdown
 
 # Digger
 A toolkit for the automatic annotation of V,D and J genes and associated features in IG receptor genomic loci.
 
 For more details, please see the [documentation](https://williamdlees.github.io/digger/index.html).
 
+Changes in v 0.5.6:
+- compatibility update for receptor_utils 0.0.40
+- allow find_alignments to be called without a -ref parameter
+
 Changes in v 0.5.5:
 - speed optimisation for dig_sequence
 - allow find_alignments to be called without a -ref parameter
 
 Changes in V 0.5.4:
 - Minor fixes to handling of non-functional sequences
```

### Comparing `receptor_digger-0.5.5/README.md` & `receptor_digger-0.5.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Digger
 A toolkit for the automatic annotation of V,D and J genes and associated features in IG receptor genomic loci.
 
 For more details, please see the [documentation](https://williamdlees.github.io/digger/index.html).
 
+Changes in v 0.5.6:
+- compatibility update for receptor_utils 0.0.40
+- allow find_alignments to be called without a -ref parameter
+
 Changes in v 0.5.5:
 - speed optimisation for dig_sequence
 - allow find_alignments to be called without a -ref parameter
 
 Changes in V 0.5.4:
 - Minor fixes to handling of non-functional sequences
```

### Comparing `receptor_digger-0.5.5/setup.cfg` & `receptor_digger-0.5.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2072 6563 6570 746f 725f 6469 6767   = receptor_digg
 00000020: 6572 0d0a 7665 7273 696f 6e20 3d20 302e  er..version = 0.
-00000030: 352e 350d 0a61 7574 686f 7220 3d20 5769  5.5..author = Wi
+00000030: 352e 360d 0a61 7574 686f 7220 3d20 5769  5.6..author = Wi
 00000040: 6c6c 6961 6d20 4c65 6573 0d0a 6175 7468  lliam Lees..auth
 00000050: 6f72 5f65 6d61 696c 203d 2077 696c 6c69  or_email = willi
 00000060: 616d 406c 6565 732e 6f72 672e 756b 0d0a  am@lees.org.uk..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 546f  description = To
 00000080: 6f6c 7320 666f 7220 6465 206e 6f76 6f20  ols for de novo 
 00000090: 6469 7363 6f76 6572 7920 6f66 2067 656e  discovery of gen
 000000a0: 6f6d 6963 2067 6572 6d6c 696e 6520 4947  omic germline IG
```

### Comparing `receptor_digger-0.5.5/src/digger/blastresults_to_csv.py` & `receptor_digger-0.5.6/src/digger/blastresults_to_csv.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/calc_motifs.py` & `receptor_digger-0.5.6/src/digger/calc_motifs.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/cirelli_contig_matches.py` & `receptor_digger-0.5.6/src/digger/cirelli_contig_matches.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/compare_annotations.py` & `receptor_digger-0.5.6/src/digger/compare_annotations.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/dig_sequence.py` & `receptor_digger-0.5.6/src/digger/dig_sequence.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/dig_utils.py` & `receptor_digger-0.5.6/src/digger/dig_utils.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/digger.py` & `receptor_digger-0.5.6/src/digger/digger.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         if fn and not os.path.isfile(fn):
             print(f"{fn} - file not found")
             exit(1)
 
         if fn:
             full_germline_set |= simple.read_fasta(fn)
 
-    simple.write_fasta(full_germline_set, 'full_germline_set.fasta')
+    simple.write_fasta('full_germline_set.fasta', full_germline_set)
 
     if args.ref_comp:
         for ref_arg in args.ref_comp:
             ref_name, fn = ref_arg.split(',')
             if not os.path.isfile(fn):
                 print(f"{fn} - file not found")
                 exit(1)
@@ -105,15 +105,15 @@
 
     assembly_contents = simple.read_fasta(args.assembly_file)
 
     if len(assembly_contents) != 1:
         print('The assembly file must contain exactly one sequence.')
         exit(1)
 
-    simple.write_fasta({list(assembly_contents.keys())[0]: list(assembly_contents.values())[0]}, 'assembly.fasta')
+    simple.write_fasta('assembly.fasta', {list(assembly_contents.keys())[0]: list(assembly_contents.values())[0]})
     assembly_name = slugify(list(assembly_contents.keys())[0])
     assembly_length = len(list(assembly_contents.values())[0])
 
     locus = 'IGH'
 
     if args.locus:
         if args.locus not in ['IGH', 'IGK', 'IGL', 'TRA', 'TRB', 'TRD', 'TRG']:
```

### Comparing `receptor_digger-0.5.5/src/digger/find_alignments.py` & `receptor_digger-0.5.6/src/digger/find_alignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from operator import attrgetter, itemgetter
 
 from Bio import pairwise2
 import csv
 from collections import defaultdict
 from importlib.resources import files
 
-from receptor_utils.number_ighv import number_ighv, gap_nt_from_aa, nt_diff, gap_sequence
+from receptor_utils.number_v import number_ighv, gap_nt_from_aa, nt_diff, gap_sequence
 from math import ceil
 import glob
 import os.path
 import argparse
 from receptor_utils import simple_bio_seq as simple
 
 try:
```

### Comparing `receptor_digger-0.5.5/src/digger/motif.py` & `receptor_digger-0.5.6/src/digger/motif.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/motifs/human/IGH/L-PART1_prob.csv` & `receptor_digger-0.5.6/src/digger/motifs/human/IGH/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/motifs/human/IGK/L-PART1_prob.csv` & `receptor_digger-0.5.6/src/digger/motifs/human/IGK/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv` & `receptor_digger-0.5.6/src/digger/motifs/human/IGK/NC_000002.12_fw_rev.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/motifs/human/IGL/L-PART1_prob.csv` & `receptor_digger-0.5.6/src/digger/motifs/human/IGL/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv` & `receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGH/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv` & `receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/L-PART1_low_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv` & `receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGK/features.csv` & `receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGK/features.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv` & `receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/L-PART1_prob.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/motifs/rhesus_macaque/IGL/features.csv` & `receptor_digger-0.5.6/src/digger/motifs/rhesus_macaque/IGL/features.csv`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/parse_genes.py` & `receptor_digger-0.5.6/src/digger/parse_genes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 from math import ceil
 from operator import attrgetter
 
 from Bio import pairwise2
 from receptor_utils import simple_bio_seq as simple
-from receptor_utils.number_ighv import gap_sequence, number_ighv, gap_nt_from_aa
+from receptor_utils.number_v import gap_sequence, number_ighv, gap_nt_from_aa
 
 try:
     from motif import Motif
     from search_motifs import find_compound_motif, MotifResult, SingleMotifResult
 except:
     from digger.motif import Motif
     from digger.search_motifs import find_compound_motif, MotifResult, SingleMotifResult
```

### Comparing `receptor_digger-0.5.5/src/digger/parse_imgt_annotations.py` & `receptor_digger-0.5.6/src/digger/parse_imgt_annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,15 +344,15 @@
                 annotations = []
 
     if args.save_imgt_annots:
         with open(args.save_imgt_annots, 'w') as fo:
             fo.write('\n'.join(all_annotations))
 
     if args.save_sequence:
-        simple.write_fasta(sequences, args.save_sequence)
+        simple.write_fasta(args.save_sequence, sequences)
 
     if fieldnames:
         with open(args.outfile, 'w', newline='') as fo:
             writer = csv.DictWriter(fo, fieldnames=fieldnames, restval='')
             writer.writeheader()
             for parsed_gene in parsed_genes:
                 writer.writerow(parsed_gene)
```

### Comparing `receptor_digger-0.5.5/src/digger/search_motifs.py` & `receptor_digger-0.5.6/src/digger/search_motifs.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/digger/slugify.py` & `receptor_digger-0.5.6/src/digger/slugify.py`

 * *Files identical despite different names*

### Comparing `receptor_digger-0.5.5/src/receptor_digger.egg-info/PKG-INFO` & `receptor_digger-0.5.6/src/receptor_digger.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: receptor-digger
-Version: 0.5.5
+Version: 0.5.6
 Summary: Tools for de novo discovery of genomic germline IG and TR receptor sequences
 Home-page: https://github.com/williamdlees/digger
 Author: William Lees
 Author-email: william@lees.org.uk
 Project-URL: Bug Tracker, https://github.com/williamdlees/digger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
@@ -13,14 +13,18 @@
 Description-Content-Type: text/markdown
 
 # Digger
 A toolkit for the automatic annotation of V,D and J genes and associated features in IG receptor genomic loci.
 
 For more details, please see the [documentation](https://williamdlees.github.io/digger/index.html).
 
+Changes in v 0.5.6:
+- compatibility update for receptor_utils 0.0.40
+- allow find_alignments to be called without a -ref parameter
+
 Changes in v 0.5.5:
 - speed optimisation for dig_sequence
 - allow find_alignments to be called without a -ref parameter
 
 Changes in V 0.5.4:
 - Minor fixes to handling of non-functional sequences
```

### Comparing `receptor_digger-0.5.5/src/receptor_digger.egg-info/SOURCES.txt` & `receptor_digger-0.5.6/src/receptor_digger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

