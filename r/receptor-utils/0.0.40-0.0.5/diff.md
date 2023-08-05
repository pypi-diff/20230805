# Comparing `tmp/receptor_utils-0.0.40.tar.gz` & `tmp/receptor_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptor_utils-0.0.40.tar", last modified: Sat Aug  5 10:30:59 2023, max compression
+gzip compressed data, was "receptor_utils-0.0.5.tar", last modified: Thu Jan 20 10:22:49 2022, max compression
```

## Comparing `receptor_utils-0.0.40.tar` & `receptor_utils-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 10:30:59.676435 receptor_utils-0.0.40/
--rw-rw-rw-   0        0        0      240 2021-12-29 13:38:03.000000 receptor_utils-0.0.40/LICENSE
--rw-rw-rw-   0        0        0     1736 2023-08-05 10:30:59.677435 receptor_utils-0.0.40/PKG-INFO
--rw-rw-rw-   0        0        0     1131 2023-08-05 10:30:02.000000 receptor_utils-0.0.40/README.md
--rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_utils-0.0.40/pyproject.toml
--rw-rw-rw-   0        0        0     1229 2023-08-05 10:30:59.678437 receptor_utils-0.0.40/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-05 10:30:59.536097 receptor_utils-0.0.40/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 10:30:59.546099 receptor_utils-0.0.40/src/receptor_utils/
--rw-rw-rw-   0        0        0      300 2023-08-05 09:14:08.000000 receptor_utils-0.0.40/src/receptor_utils/__init__.py
--rw-rw-rw-   0        0        0    10883 2023-08-05 09:09:09.000000 receptor_utils-0.0.40/src/receptor_utils/novel_allele_name.py
--rw-rw-rw-   0        0        0    13093 2023-08-05 09:13:25.000000 receptor_utils-0.0.40/src/receptor_utils/number_v.py
--rw-rw-rw-   0        0        0    13272 2023-08-05 09:27:00.000000 receptor_utils-0.0.40/src/receptor_utils/simple_bio_seq.py
-drwxrwxrwx   0        0        0        0 2023-08-05 10:30:59.553097 receptor_utils-0.0.40/src/receptor_utils.egg-info/
--rw-rw-rw-   0        0        0     1736 2023-08-05 10:30:59.000000 receptor_utils-0.0.40/src/receptor_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      742 2023-08-05 10:30:59.000000 receptor_utils-0.0.40/src/receptor_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 10:30:59.000000 receptor_utils-0.0.40/src/receptor_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      437 2023-08-05 10:30:59.000000 receptor_utils-0.0.40/src/receptor_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2023-08-05 10:30:59.000000 receptor_utils-0.0.40/src/receptor_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-05 10:30:59.674433 receptor_utils-0.0.40/src/scripts/
--rw-rw-rw-   0        0        0        0 2022-11-21 17:22:07.000000 receptor_utils-0.0.40/src/scripts/__init__.py
--rw-rw-rw-   0        0        0     3694 2023-07-18 10:35:37.000000 receptor_utils-0.0.40/src/scripts/annotate_j.py
--rw-rw-rw-   0        0        0     1234 2022-11-21 09:52:05.000000 receptor_utils-0.0.40/src/scripts/at_coords.py
--rw-rw-rw-   0        0        0     2720 2023-08-05 09:31:48.000000 receptor_utils-0.0.40/src/scripts/extract_refs.py
--rw-rw-rw-   0        0        0     1501 2023-08-05 09:32:14.000000 receptor_utils-0.0.40/src/scripts/fix_macaque_gaps.py
--rw-rw-rw-   0        0        0     2546 2023-08-05 09:32:33.000000 receptor_utils-0.0.40/src/scripts/gap_inferred.py
--rw-rw-rw-   0        0        0     1291 2022-11-21 10:21:52.000000 receptor_utils-0.0.40/src/scripts/identical_seqs.py
--rw-rw-rw-   0        0        0     5777 2023-07-18 10:13:35.000000 receptor_utils-0.0.40/src/scripts/make_igblast_ndm.py
--rw-rw-rw-   0        0        0     1036 2023-08-05 09:33:10.000000 receptor_utils-0.0.40/src/scripts/merge_fasta.py
--rw-rw-rw-   0        0        0     2467 2022-12-13 10:59:05.000000 receptor_utils-0.0.40/src/scripts/name_allele.py
--rw-rw-rw-   0        0        0      653 2022-11-21 10:42:26.000000 receptor_utils-0.0.40/src/scripts/reverse_complement.py
-drwxrwxrwx   0        0        0        0 2023-08-05 10:30:59.675435 receptor_utils-0.0.40/tests/
--rw-rw-rw-   0        0        0      248 2022-07-25 12:41:04.000000 receptor_utils-0.0.40/tests/test_scored_gap_consensus.py
+drwxrwxrwx   0        0        0        0 2022-01-20 10:22:49.330403 receptor_utils-0.0.5/
+-rw-rw-rw-   0        0        0      240 2021-12-29 13:38:03.000000 receptor_utils-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3218 2022-01-20 10:22:49.330403 receptor_utils-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2573 2022-01-20 10:18:59.000000 receptor_utils-0.0.5/README.md
+-rw-rw-rw-   0        0        0      110 2021-12-29 13:39:50.000000 receptor_utils-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      943 2022-01-20 10:22:49.332403 receptor_utils-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-01-20 10:22:49.176113 receptor_utils-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2022-01-20 10:22:49.314403 receptor_utils-0.0.5/src/receptor_utils/
+-rw-rw-rw-   0        0        0        0 2021-12-30 16:26:06.000000 receptor_utils-0.0.5/src/receptor_utils/__init__.py
+-rw-rw-rw-   0        0        0     1218 2022-01-19 12:24:36.000000 receptor_utils-0.0.5/src/receptor_utils/extract_refs.py
+-rw-rw-rw-   0        0        0     1749 2022-01-20 09:38:18.000000 receptor_utils-0.0.5/src/receptor_utils/gap_inferred.py
+-rw-rw-rw-   0        0        0      993 2022-01-19 12:07:22.000000 receptor_utils-0.0.5/src/receptor_utils/identical_seqs.py
+-rw-rw-rw-   0        0        0     6174 2022-01-11 09:48:59.000000 receptor_utils-0.0.5/src/receptor_utils/novel_allele_name.py
+-rw-rw-rw-   0        0        0    12364 2022-01-20 09:23:34.000000 receptor_utils-0.0.5/src/receptor_utils/number_ighv.py
+-rw-rw-rw-   0        0        0     3878 2021-12-12 16:10:58.000000 receptor_utils-0.0.5/src/receptor_utils/simple_bio_seq.py
+drwxrwxrwx   0        0        0        0 2022-01-20 10:22:49.329403 receptor_utils-0.0.5/src/receptor_utils.egg-info/
+-rw-rw-rw-   0        0        0     3218 2022-01-20 10:22:49.000000 receptor_utils-0.0.5/src/receptor_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2022-01-20 10:22:49.000000 receptor_utils-0.0.5/src/receptor_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-20 10:22:49.000000 receptor_utils-0.0.5/src/receptor_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2022-01-20 10:22:49.000000 receptor_utils-0.0.5/src/receptor_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2022-01-20 10:22:49.000000 receptor_utils-0.0.5/src/receptor_utils.egg-info/top_level.txt
```

### Comparing `receptor_utils-0.0.40/src/receptor_utils/number_v.py` & `receptor_utils-0.0.5/src/receptor_utils/number_ighv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-
-# Copyright (c) 2021 William Lees
-
-# This source code, and any executable file compiled or derived from it, is governed by the European Union Public License v. 1.2,
-# the English version of which is available here: https://perma.cc/DK5U-NDVE
+# De novo IMGT-gapping of macaque IGHV germline genes, using guidance from http://www.bioinf.org.uk/abs/info.html#cdrid to confirm CDR1 and 2
 
 import re
 from receptor_utils import simple_bio_seq as simple
 
 def nt_diff(s1, s2):
     diffs = 0
     row = list(zip(s1.upper(), s2.upper()))
@@ -15,17 +11,15 @@
         if row[p][0] != row[p][1] and (row[p][0] not in ['X', 'N'] and row[p][1] not in ['X', 'N']):
             diffs += 1
 
     diffs += abs(len(s1) - len(s2))
     return diffs
 
 
-# De novo IMGT-gapping of IGHV germline genes, using guidance from http://www.bioinf.org.uk/abs/info.html#cdrid to confirm CDR1 and 2
-# This is experimental. Not used in the examples and specific to IGHV. Maybe a recourse if there is no suitable gapped reference template
-# to rely on
+# Number the protein translation of an entire IGHV V-gene
 def number_ighv(seq):
     gapped = ''
     # find the conserved Cys at 23
     if 'C' not in seq[21:23]:
         return None, 'First conserved cysteine not found'
 
     if seq[21] == 'C':
@@ -144,18 +138,26 @@
     seq = insert_space(seq, 55)
     seq = insert_space(seq, 38)
     seq = insert_space(seq, 26)
 
     print(pretty_header)
     print(seq)
 
+def chunks(l, n):
+    """ Yield successive n-sized chunks from l."""
+    for i in range(0, len(l), n):
+        yield l[i:i+n]
 
 # Given a gapped AA sequence and an ungapped nt sequence, produce a gapped nt sequence
 def gap_nt_from_aa(nucleotide_seq, peptide_seq):
-    codons = [codon for codon in simple.chunks(nucleotide_seq, 3)]  #splits nucleotides into codons (triplets)
+    """ Transfers gaps from aligned peptide seq into codon partitioned nucleotide seq (codon alignment)
+          - peptide_seq is an aligned peptide sequence with gaps that need to be transferred to nucleotide seq
+          - nucleotide_seq is an un-aligned dna sequence whose codons translate to peptide seq"""
+
+    codons = [codon for codon in chunks(nucleotide_seq, 3)]  #splits nucleotides into codons (triplets)
     remains = nucleotide_seq[3*len(codons):] if 3*len(codons) != len(nucleotide_seq) else ''
     gapped_codons = []
     codon_count = 0
 
     for aa in peptide_seq:  #adds '---' gaps to nucleotide seq corresponding to peptide
         if aa not in ('-', '.'):
             gapped_codons.append(codons[codon_count])
@@ -168,103 +170,77 @@
         codon_count += 1
 
     return ''.join(gapped_codons) + remains
 
 
 def gap_align(seq, ref):
     seq_i = iter(seq)
+    ref_i = iter(ref)
 
     res = ''
-    started = False
 
     for r in ref:
         if r != '.':
-            started = True
             try:
                 res += next(seq_i)
             except StopIteration:
                 res += '.'
         else:
-            if started:
-                res += '.'
-            else:
-                try:
-                    res += next(seq_i)
-                except StopIteration:
-                    res += '.'
+            res += '.'
 
     while True:
         try:
             res += next(seq_i)
         except StopIteration:
             break
 
     # remove trailing gaps
 
     i = len(res) - 1
 
-    while i and res[i] == '.':
+    while res[i] == '.':
         i -= 1
 
     res = res[:i+1]
 
 
     return res
 
 
 def gap_align_aa(seq, ref):
     seq_i = iter(seq)
+    ref_i = iter(ref)
 
     res = ''
-    started = False
 
     for r in ref:
         if r != '.':
-            started = True
             try:
                 res += next(seq_i)
             except StopIteration:
                 break
         else:
-            if started:
-                res += '.'
-            else:
-                try:
-                    res += next(seq_i)
-                except StopIteration:
-                    break
+            res += '.'
 
     while True:
         try:
             res += next(seq_i)
         except StopIteration:
             break
 
     return res
 
 
 def gap_align_aa_from_nt(aa_seq, nt_gapped):
     aa_i = iter(aa_seq)
     gapped_aa = ''
-
-    started = False
-
-    for codon in simple.chunks(nt_gapped, 3):
+    for codon in chunks(nt_gapped, 3):
         if '.' in codon:
-            if started:
-                gapped_aa += '.'
-            else:
-                try:
-                    gapped_aa += next(aa_i)
-                except StopIteration:
-                    break
-
+            gapped_aa += '.'
         else:
-            started = True
-
             try:
                 gapped_aa += next(aa_i)
             except StopIteration:
                 break
 
     return gapped_aa
 
@@ -275,49 +251,38 @@
     closest = ''
     for name, ref in ungapped_ref.items():
         d = nt_diff(seq, ref)
         if d < diffs:
             closest = name
             diffs = d
 
-    # print(f'gapping with {closest}')
     res = gap_align(seq, gapped_ref[closest])
     aa = simple.translate(seq)
     aa = gap_align_aa_from_nt(aa, res)
 
-    notes = ''
     # checks
-    if 'V' in closest:
-        notes = check_conserved_residues(aa)
+    notes = check_conserved_residues(aa)
 
     return (res, aa, notes)
 
 
 def check_conserved_residues(aa):
-    notes = []
-
-    if len(aa) < 104:
-        return 'Sequence truncated before second cysteine'
-
+    notes = ''
     # allow stop codon in final nucleotides without warning
-    if '*' in aa:
-        pos = aa.index('*')
-        if pos <= 103:
-            notes.append('Stop codon in V-REGION before 2nd cysteine')
-
-    if aa[22] != 'C':
-        notes.append('First cysteine not found')
-
-    if aa[40] != 'W':
-        notes.append('Conserved Trp not found')
-
-    if aa[103] != 'C':
-        notes.append('Second cysteine not found')
-
-    return ', '.join(notes)
+    if 'X' in aa[:-1] or '*' in aa[:-1]:
+        notes = 'Stop codon in V-REGION'
+    elif aa[22] != 'C':
+        notes = 'First cysteine not found'
+    elif aa[40] != 'W':
+        notes = 'Conserved Trp not found'
+    elif len(aa) < 104:
+        notes = 'Sequence truncated before second cysteine'
+    elif aa[103] != 'C':
+        notes = 'Second cysteine not found'
+    return notes
 
 
 def run_tests():
     failed = 0
 
     print('1-64')
     query = 'EMQLVQSEAEVKKPGASVKISCKASGYTFTYRYLHWLRQTPGQGLEWMGWITPYNGNTNYAQKFQDRATITRDRSMSTAYMELSSLRSEDTAVYYCAR'
```

### Comparing `receptor_utils-0.0.40/src/scripts/fix_macaque_gaps.py` & `receptor_utils-0.0.5/src/receptor_utils/gap_inferred.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,54 @@
-# Remove unwanted inserted codons in IMGT alignment of macaque IG sequences
+#!python
+# Gap sequences inferred by IgDiscover
 
-from receptor_utils import simple_bio_seq as simple
+from receptor_utils import number_ighv
 import argparse
-
-def get_parser():
-    parser = argparse.ArgumentParser(description='Remove unwanted inserted codons in IMGT alignment of rhesus macaque IG sequences')
-    parser.add_argument('infile', help='gapped file from IMGT')
-    parser.add_argument('outfile', help='gapped file confirming to the customary alignment (without inserted codons)')
-    parser.add_argument('chain', help='IGH, IGK or IGL')
-    return parser
-
-
-unwanted_codons = {
-    'IGL': [21, 52, 53],
-    'IGK': [21],
-    'IGH': [16, 28],
-}
+from receptor_utils import simple_bio_seq as simple
+import Bio.Data.CodonTable
 
 
 def main():
-    parser = get_parser()
+    parser = argparse.ArgumentParser(description='Gap inferred sequences')
+    parser.add_argument('inferred_file', help='ungapped inferred sequences (fasta)')
+    parser.add_argument('ref_file', help='gapped reference set (fasta)')
+    parser.add_argument('out_file', help='output file containing gapped inferred sequences')
     args = parser.parse_args()
 
-    if args.chain not in ['IGH', 'IGK', 'IGL']:
-        print("'chain' must be one of IGH, IGK, IGL")
-        exit(0)
-
-    seqs = simple.read_fasta(args.infile)
-    unwanted_seqs = []
-
-    for name, seq in seqs.items():
-        for unw in sorted(unwanted_codons[args.chain], reverse=True):
-            if seq[(unw-1)*3] == '.':
-                seq = seq[:(unw-1)*3] + seq[3 + (unw-1)*3:]
-            else:
-                print(f"Unwanted codon at {unw} in sequence {name} is non-blank: dropping sequence")
-                unwanted_seqs.append(name)
-                break
-            seqs[name] = seq
+    inferred = simple.read_fasta(args.inferred_file)
+    refs = simple.read_fasta(args.ref_file)
+    
+    # Check that reference sequences have conserved residues - remove any that don't
+    
+    for ref, seq in list(refs.items()):
+        try:
+            aa = simple.translate(seq.replace('.', '-'))
+            notes = number_ighv.check_conserved_residues(aa)
+
+            if notes:
+                print(f'Removing {ref} from reference: {notes}\n{aa}')
+                del refs[ref]
+        except Bio.Data.CodonTable.TranslationError as e:
+            print(f'Removing {ref} from reference: {e}\n{aa}')
+            del refs[ref]
+
+    ungapped_refs = {}
+
+    for id, seq in refs.items():
+        ungapped_refs[id] = seq.replace('.', '')
+
+    gapped = {}
+
+    for id, seq in inferred.items():
+        if '.' not in seq:
+            gapped[id], aa, notes = number_ighv.gap_sequence(seq, refs, ungapped_refs)
+            if notes is not None and len(notes) > 0:
+                print('%s: %s' % (id, notes))
+        else:
+            gapped[id] = seq
 
-    for unw in unwanted_seqs:
-        del seqs[unw]
+    simple.write_fasta(gapped, args.out_file)
 
-    simple.write_fasta(args.outfile, seqs)
 
 
 if __name__ == "__main__":
     main()
```

