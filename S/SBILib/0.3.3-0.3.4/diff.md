# Comparing `tmp/SBILib-0.3.3.tar.gz` & `tmp/SBILib-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SBILib-0.3.3.tar", last modified: Sat Jul 22 21:19:59 2023, max compression
+gzip compressed data, was "SBILib-0.3.4.tar", last modified: Sat Aug  5 01:27:41 2023, max compression
```

## Comparing `SBILib-0.3.3.tar` & `SBILib-0.3.4.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.841251 SBILib-0.3.3/
--rw-r--r--   0 patrick    (501) staff       (20)      128 2023-07-21 15:34:16.000000 SBILib-0.3.3/MANIFEST.in
--rw-r--r--   0 patrick    (501) staff       (20)    37821 2023-07-22 21:19:59.844503 SBILib-0.3.3/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)    37560 2023-07-22 18:00:53.000000 SBILib-0.3.3/README.md
--rw-r--r--   0 patrick    (501) staff       (20)     6077 2023-07-21 20:09:42.000000 SBILib-0.3.3/Scenarios.md
--rw-r--r--   0 patrick    (501) staff       (20)      103 2023-07-22 21:19:59.846314 SBILib-0.3.3/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)      621 2023-07-22 21:19:29.000000 SBILib-0.3.3/setup.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.463632 SBILib-0.3.3/src/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.485565 SBILib-0.3.3/src/SBILib/
--rw-r--r--   0 patrick    (501) staff       (20)    12951 2023-07-22 21:19:07.000000 SBILib-0.3.3/src/SBILib/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.517659 SBILib-0.3.3/src/SBILib/beans/
--rw-r--r--   0 patrick    (501) staff       (20)     4500 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/beans/Executable.py
--rw-r--r--   0 patrick    (501) staff       (20)    11699 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/beans/File.py
--rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-07-19 22:56:14.000000 SBILib-0.3.3/src/SBILib/beans/IndexedNum.py
--rw-r--r--   0 patrick    (501) staff       (20)      349 2023-07-19 22:56:22.000000 SBILib-0.3.3/src/SBILib/beans/JSONer.py
--rw-r--r--   0 patrick    (501) staff       (20)    14930 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/beans/Path.py
--rw-r--r--   0 patrick    (501) staff       (20)     2926 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/beans/StorableObject.py
--rw-r--r--   0 patrick    (501) staff       (20)      187 2023-07-19 22:56:21.000000 SBILib-0.3.3/src/SBILib/beans/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-07-19 22:56:20.000000 SBILib-0.3.3/src/SBILib/beans/butler.py
--rw-r--r--   0 patrick    (501) staff       (20)      516 2023-07-19 22:56:23.000000 SBILib-0.3.3/src/SBILib/beans/singleton.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.537324 SBILib-0.3.3/src/SBILib/data/
--rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-07-19 22:55:56.000000 SBILib-0.3.3/src/SBILib/data/Alphabet.py
--rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-07-19 22:55:49.000000 SBILib-0.3.3/src/SBILib/data/AminoAcids.py
--rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-07-19 22:55:54.000000 SBILib-0.3.3/src/SBILib/data/AtomVariants.py
--rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-07-19 22:55:55.000000 SBILib-0.3.3/src/SBILib/data/Element.py
--rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-07-19 22:55:55.000000 SBILib-0.3.3/src/SBILib/data/Properties.py
--rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-07-19 22:55:57.000000 SBILib-0.3.3/src/SBILib/data/SetDict.py
--rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-07-19 22:55:53.000000 SBILib-0.3.3/src/SBILib/data/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.579454 SBILib-0.3.3/src/SBILib/databases/
--rw-r--r--   0 patrick    (501) staff       (20)      273 2023-07-19 22:56:12.000000 SBILib-0.3.3/src/SBILib/databases/AlphaFoldlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-07-19 22:56:12.000000 SBILib-0.3.3/src/SBILib/databases/CATHlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     8412 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/DrugBanklink.py
--rw-r--r--   0 patrick    (501) staff       (20)    13617 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/Enzymelink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5573 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/GOlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5355 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/PDBTMlink.py
--rw-r--r--   0 patrick    (501) staff       (20)      417 2023-07-19 22:56:01.000000 SBILib-0.3.3/src/SBILib/databases/PDBeChemConnect.py
--rw-r--r--   0 patrick    (501) staff       (20)     6713 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/PDBeChemlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     9123 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/PDBlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     1795 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/SCOPlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5733 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/TaxIDlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7098 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7063 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/__Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-07-19 22:56:07.000000 SBILib-0.3.3/src/SBILib/databases/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7149 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/dblink.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.586188 SBILib-0.3.3/src/SBILib/databases/uniprot/
--rw-r--r--   0 patrick    (501) staff       (20)       90 2023-07-19 22:56:09.000000 SBILib-0.3.3/src/SBILib/databases/uniprot/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     4777 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/uniprot/connect.py
--rw-r--r--   0 patrick    (501) staff       (20)     8169 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/uniprot/uniprot.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.596162 SBILib-0.3.3/src/SBILib/error/
--rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-07-19 22:55:48.000000 SBILib-0.3.3/src/SBILib/error/BlastError.py
--rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-07-19 22:55:43.000000 SBILib-0.3.3/src/SBILib/error/FileError.py
--rw-r--r--   0 patrick    (501) staff       (20)      896 2023-07-19 22:55:48.000000 SBILib-0.3.3/src/SBILib/error/SeqAliError.py
--rw-r--r--   0 patrick    (501) staff       (20)      108 2023-07-19 22:55:47.000000 SBILib-0.3.3/src/SBILib/error/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.602553 SBILib-0.3.3/src/SBILib/external/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.615765 SBILib-0.3.3/src/SBILib/external/CDhit/
--rw-r--r--   0 patrick    (501) staff       (20)      964 2023-07-19 22:57:25.000000 SBILib-0.3.3/src/SBILib/external/CDhit/CDhit.py
--rw-r--r--   0 patrick    (501) staff       (20)     2255 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/CDhit/CDhitExe.py
--rw-r--r--   0 patrick    (501) staff       (20)      802 2023-07-19 22:57:26.000000 SBILib-0.3.3/src/SBILib/external/CDhit/CDhitHomolog.py
--rw-r--r--   0 patrick    (501) staff       (20)     2223 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/CDhit/CDhitList.py
--rw-r--r--   0 patrick    (501) staff       (20)       64 2023-07-19 22:57:25.000000 SBILib-0.3.3/src/SBILib/external/CDhit/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.625783 SBILib-0.3.3/src/SBILib/external/DSSP/
--rw-r--r--   0 patrick    (501) staff       (20)     3324 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/DSSP/DSSP.py
--rw-r--r--   0 patrick    (501) staff       (20)     3606 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/DSSP/DSSPExe.py
--rw-r--r--   0 patrick    (501) staff       (20)       54 2023-07-19 22:57:32.000000 SBILib-0.3.3/src/SBILib/external/DSSP/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      338 2023-07-19 22:57:27.000000 SBILib-0.3.3/src/SBILib/external/README.md
--rw-r--r--   0 patrick    (501) staff       (20)       62 2023-07-19 22:57:28.000000 SBILib-0.3.3/src/SBILib/external/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.638283 SBILib-0.3.3/src/SBILib/external/blast/
--rw-r--r--   0 patrick    (501) staff       (20)     9107 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/blast/BlastExe.py
--rw-r--r--   0 patrick    (501) staff       (20)    12570 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/blast/BlastHit.py
--rw-r--r--   0 patrick    (501) staff       (20)    23488 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/blast/BlastResult.py
--rw-r--r--   0 patrick    (501) staff       (20)       83 2023-07-19 22:57:19.000000 SBILib-0.3.3/src/SBILib/external/blast/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     8072 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/blast/blast_parser.py
--rw-r--r--   0 patrick    (501) staff       (20)      312 2023-07-19 22:57:34.000000 SBILib-0.3.3/src/SBILib/external/configSBI.txt
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.642786 SBILib-0.3.3/src/SBILib/math/
--rw-r--r--   0 patrick    (501) staff       (20)       19 2023-07-19 22:57:36.000000 SBILib-0.3.3/src/SBILib/math/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-07-19 22:57:35.000000 SBILib-0.3.3/src/SBILib/math/stats.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.660878 SBILib-0.3.3/src/SBILib/sequence/
--rw-r--r--   0 patrick    (501) staff       (20)     6331 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/sequence/Fasta.py
--rw-r--r--   0 patrick    (501) staff       (20)     4871 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/sequence/IndexedSeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)    15045 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/sequence/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-07-19 22:57:13.000000 SBILib-0.3.3/src/SBILib/sequence/Sequence.py
--rw-r--r--   0 patrick    (501) staff       (20)      140 2023-07-19 22:57:10.000000 SBILib-0.3.3/src/SBILib/sequence/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.669878 SBILib-0.3.3/src/SBILib/sequence/alignment/
--rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-07-19 22:57:04.000000 SBILib-0.3.3/src/SBILib/sequence/alignment/Needleman_Wunsch.py
--rw-r--r--   0 patrick    (501) staff       (20)    43526 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/sequence/alignment/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-07-19 22:57:04.000000 SBILib-0.3.3/src/SBILib/sequence/alignment/SimilarityMatrix.py
--rw-r--r--   0 patrick    (501) staff       (20)       93 2023-07-19 22:57:05.000000 SBILib-0.3.3/src/SBILib/sequence/alignment/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.681214 SBILib-0.3.3/src/SBILib/structure/
--rw-r--r--   0 patrick    (501) staff       (20)    25560 2023-07-20 15:29:21.000000 SBILib-0.3.3/src/SBILib/structure/PDB.py
--rw-r--r--   0 patrick    (501) staff       (20)      460 2023-07-19 22:54:58.000000 SBILib-0.3.3/src/SBILib/structure/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.691647 SBILib-0.3.3/src/SBILib/structure/atom/
--rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-07-19 22:55:41.000000 SBILib-0.3.3/src/SBILib/structure/atom/Atom.py
--rw-r--r--   0 patrick    (501) staff       (20)      659 2023-07-19 22:55:42.000000 SBILib-0.3.3/src/SBILib/structure/atom/AtomOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)      803 2023-07-19 22:55:35.000000 SBILib-0.3.3/src/SBILib/structure/atom/AtomOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     3758 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/atom/AtomSeries.py
--rw-r--r--   0 patrick    (501) staff       (20)      127 2023-07-19 22:55:40.000000 SBILib-0.3.3/src/SBILib/structure/atom/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.707819 SBILib-0.3.3/src/SBILib/structure/chain/
--rw-r--r--   0 patrick    (501) staff       (20)    19964 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/chain/Chain.py
--rw-r--r--   0 patrick    (501) staff       (20)    13264 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/chain/ChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)     2763 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/chain/ChainOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     6877 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/chain/ChainOfProtein.py
--rw-r--r--   0 patrick    (501) staff       (20)     4988 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/chain/ProteinChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)      131 2023-07-19 22:54:38.000000 SBILib-0.3.3/src/SBILib/structure/chain/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.714779 SBILib-0.3.3/src/SBILib/structure/contacts/
--rw-r--r--   0 patrick    (501) staff       (20)     9010 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/Complex.py
--rw-r--r--   0 patrick    (501) staff       (20)     3408 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/InnerContacts.py
--rw-r--r--   0 patrick    (501) staff       (20)      277 2023-07-19 22:55:14.000000 SBILib-0.3.3/src/SBILib/structure/contacts/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.724895 SBILib-0.3.3/src/SBILib/structure/contacts/contact/
--rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-07-19 22:55:19.000000 SBILib-0.3.3/src/SBILib/structure/contacts/contact/Contact.py
--rw-r--r--   0 patrick    (501) staff       (20)     3806 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAA.py
--rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-07-19 22:55:19.000000 SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAH.py
--rw-r--r--   0 patrick    (501) staff       (20)     3275 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAN.py
--rw-r--r--   0 patrick    (501) staff       (20)      149 2023-07-19 22:55:18.000000 SBILib-0.3.3/src/SBILib/structure/contacts/contact/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.731119 SBILib-0.3.3/src/SBILib/structure/contacts/inner/
--rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-07-19 22:55:25.000000 SBILib-0.3.3/src/SBILib/structure/contacts/inner/PHInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-07-19 22:55:24.000000 SBILib-0.3.3/src/SBILib/structure/contacts/inner/PPInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)       85 2023-07-19 22:55:24.000000 SBILib-0.3.3/src/SBILib/structure/contacts/inner/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.744814 SBILib-0.3.3/src/SBILib/structure/contacts/interface/
--rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-07-19 22:55:11.000000 SBILib-0.3.3/src/SBILib/structure/contacts/interface/Interface.py
--rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-07-19 22:55:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/interface/PHInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    11115 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/interface/PNInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-07-19 22:55:11.000000 SBILib-0.3.3/src/SBILib/structure/contacts/interface/PPInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)      157 2023-07-19 22:55:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/interface/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.749065 SBILib-0.3.3/src/SBILib/structure/geometry/
--rw-r--r--   0 patrick    (501) staff       (20)    11737 2023-07-19 22:54:32.000000 SBILib-0.3.3/src/SBILib/structure/geometry/RMSD.py
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 22:54:33.000000 SBILib-0.3.3/src/SBILib/structure/geometry/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      662 2023-07-19 22:54:32.000000 SBILib-0.3.3/src/SBILib/structure/geometry/basics.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.777015 SBILib-0.3.3/src/SBILib/structure/header/
--rw-r--r--   0 patrick    (501) staff       (20)     2282 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/BioMolecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     3827 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/DBreference.py
--rw-r--r--   0 patrick    (501) staff       (20)     2011 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/Experiment.py
--rw-r--r--   0 patrick    (501) staff       (20)    14754 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/Header.py
--rw-r--r--   0 patrick    (501) staff       (20)     1199 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/HeteroAtom.py
--rw-r--r--   0 patrick    (501) staff       (20)      944 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/MiniRes.py
--rw-r--r--   0 patrick    (501) staff       (20)     7645 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/Molecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     8530 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     2421 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/Site.py
--rw-r--r--   0 patrick    (501) staff       (20)    18693 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    14368 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/parse_mmCIF.py
--rw-r--r--   0 patrick    (501) staff       (20)     8541 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/parse_pdb.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.792350 SBILib-0.3.3/src/SBILib/structure/protein/
--rw-r--r--   0 patrick    (501) staff       (20)    19068 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/protein/Arch.py
--rw-r--r--   0 patrick    (501) staff       (20)    19200 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/protein/SShelper.py
--rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-07-19 22:55:29.000000 SBILib-0.3.3/src/SBILib/structure/protein/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-07-19 22:55:34.000000 SBILib-0.3.3/src/SBILib/structure/protein/Sequencer.py
--rw-r--r--   0 patrick    (501) staff       (20)      134 2023-07-19 22:55:34.000000 SBILib-0.3.3/src/SBILib/structure/protein/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.802850 SBILib-0.3.3/src/SBILib/structure/residue/
--rw-r--r--   0 patrick    (501) staff       (20)    10771 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/residue/Residue.py
--rw-r--r--   0 patrick    (501) staff       (20)    10721 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/residue/ResidueOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)     5357 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/residue/ResidueOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)      146 2023-07-19 22:55:02.000000 SBILib-0.3.3/src/SBILib/structure/residue/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.836240 SBILib-0.3.3/src/SBILib/tests/
--rw-r--r--   0 patrick    (501) staff       (20)      426 2023-07-20 15:27:20.000000 SBILib-0.3.3/src/SBILib/tests/Test.py
--rw-r--r--   0 patrick    (501) staff       (20)   156217 2023-07-19 23:01:16.000000 SBILib-0.3.3/src/SBILib/tests/Test_1a3q.cif.gz
--rw-r--r--   0 patrick    (501) staff       (20)    47362 2023-07-19 23:01:16.000000 SBILib-0.3.3/src/SBILib/tests/Test_pdb1a2w.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:17.000000 SBILib-0.3.3/src/SBILib/tests/Test_pdb1a3q.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)   116164 2023-07-19 23:01:18.000000 SBILib-0.3.3/src/SBILib/tests/Test_pdb2ram.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 23:01:17.000000 SBILib-0.3.3/src/SBILib/tests/__ini__.py
--rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:21.000000 SBILib-0.3.3/src/SBILib/tests/pdb1a3q.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)     9923 2023-07-21 16:09:58.000000 SBILib-0.3.3/src/SBILib/tests/test_modules.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.492574 SBILib-0.3.3/src/SBILib.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)    37821 2023-07-22 21:19:59.000000 SBILib-0.3.3/src/SBILib.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     5049 2023-07-22 21:19:59.000000 SBILib-0.3.3/src/SBILib.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-07-22 21:19:59.000000 SBILib-0.3.3/src/SBILib.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)       39 2023-07-22 21:19:59.000000 SBILib-0.3.3/src/SBILib.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        7 2023-07-22 21:19:59.000000 SBILib-0.3.3/src/SBILib.egg-info/top_level.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.775630 SBILib-0.3.4/
+-rw-r--r--   0 patrick    (501) staff       (20)      128 2023-07-21 15:34:16.000000 SBILib-0.3.4/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)    37862 2023-08-05 01:27:41.776277 SBILib-0.3.4/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)    37564 2023-08-05 00:36:21.000000 SBILib-0.3.4/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)     6077 2023-07-21 20:09:42.000000 SBILib-0.3.4/Scenarios.md
+-rw-r--r--   0 patrick    (501) staff       (20)      103 2023-08-05 01:27:41.777737 SBILib-0.3.4/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)      621 2023-08-05 01:21:39.000000 SBILib-0.3.4/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.440747 SBILib-0.3.4/src/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.475896 SBILib-0.3.4/src/SBILib/
+-rw-r--r--   0 patrick    (501) staff       (20)    12951 2023-08-05 01:21:18.000000 SBILib-0.3.4/src/SBILib/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.501243 SBILib-0.3.4/src/SBILib/beans/
+-rw-r--r--   0 patrick    (501) staff       (20)     4500 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/beans/Executable.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11699 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/beans/File.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-07-19 22:56:14.000000 SBILib-0.3.4/src/SBILib/beans/IndexedNum.py
+-rw-r--r--   0 patrick    (501) staff       (20)      349 2023-07-19 22:56:22.000000 SBILib-0.3.4/src/SBILib/beans/JSONer.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14930 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/beans/Path.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2926 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/beans/StorableObject.py
+-rw-r--r--   0 patrick    (501) staff       (20)      187 2023-07-19 22:56:21.000000 SBILib-0.3.4/src/SBILib/beans/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-07-19 22:56:20.000000 SBILib-0.3.4/src/SBILib/beans/butler.py
+-rw-r--r--   0 patrick    (501) staff       (20)      516 2023-07-19 22:56:23.000000 SBILib-0.3.4/src/SBILib/beans/singleton.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.517671 SBILib-0.3.4/src/SBILib/data/
+-rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-07-19 22:55:56.000000 SBILib-0.3.4/src/SBILib/data/Alphabet.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-07-19 22:55:49.000000 SBILib-0.3.4/src/SBILib/data/AminoAcids.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-07-19 22:55:54.000000 SBILib-0.3.4/src/SBILib/data/AtomVariants.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-07-19 22:55:55.000000 SBILib-0.3.4/src/SBILib/data/Element.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-07-19 22:55:55.000000 SBILib-0.3.4/src/SBILib/data/Properties.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-07-19 22:55:57.000000 SBILib-0.3.4/src/SBILib/data/SetDict.py
+-rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-07-19 22:55:53.000000 SBILib-0.3.4/src/SBILib/data/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.551560 SBILib-0.3.4/src/SBILib/databases/
+-rw-r--r--   0 patrick    (501) staff       (20)      273 2023-07-19 22:56:12.000000 SBILib-0.3.4/src/SBILib/databases/AlphaFoldlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-07-19 22:56:12.000000 SBILib-0.3.4/src/SBILib/databases/CATHlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8412 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/DrugBanklink.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13617 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/Enzymelink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5573 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/GOlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5355 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/PDBTMlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)      417 2023-07-19 22:56:01.000000 SBILib-0.3.4/src/SBILib/databases/PDBeChemConnect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6713 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/PDBeChemlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9123 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/PDBlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1795 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/SCOPlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5733 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/TaxIDlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7098 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7063 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/__Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-07-19 22:56:07.000000 SBILib-0.3.4/src/SBILib/databases/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7149 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/dblink.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.557951 SBILib-0.3.4/src/SBILib/databases/uniprot/
+-rw-r--r--   0 patrick    (501) staff       (20)       90 2023-07-19 22:56:09.000000 SBILib-0.3.4/src/SBILib/databases/uniprot/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4777 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/uniprot/connect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8169 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/databases/uniprot/uniprot.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.568068 SBILib-0.3.4/src/SBILib/error/
+-rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-07-19 22:55:48.000000 SBILib-0.3.4/src/SBILib/error/BlastError.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-07-19 22:55:43.000000 SBILib-0.3.4/src/SBILib/error/FileError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      896 2023-07-19 22:55:48.000000 SBILib-0.3.4/src/SBILib/error/SeqAliError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      108 2023-07-19 22:55:47.000000 SBILib-0.3.4/src/SBILib/error/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.575034 SBILib-0.3.4/src/SBILib/external/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.586989 SBILib-0.3.4/src/SBILib/external/CDhit/
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-07-19 22:57:25.000000 SBILib-0.3.4/src/SBILib/external/CDhit/CDhit.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2255 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/external/CDhit/CDhitExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)      802 2023-07-19 22:57:26.000000 SBILib-0.3.4/src/SBILib/external/CDhit/CDhitHomolog.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2223 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/external/CDhit/CDhitList.py
+-rw-r--r--   0 patrick    (501) staff       (20)       64 2023-07-19 22:57:25.000000 SBILib-0.3.4/src/SBILib/external/CDhit/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.594949 SBILib-0.3.4/src/SBILib/external/DSSP/
+-rw-r--r--   0 patrick    (501) staff       (20)     3324 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/external/DSSP/DSSP.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3606 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/external/DSSP/DSSPExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)       54 2023-07-19 22:57:32.000000 SBILib-0.3.4/src/SBILib/external/DSSP/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      338 2023-07-19 22:57:27.000000 SBILib-0.3.4/src/SBILib/external/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)       62 2023-07-19 22:57:28.000000 SBILib-0.3.4/src/SBILib/external/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.606491 SBILib-0.3.4/src/SBILib/external/blast/
+-rw-r--r--   0 patrick    (501) staff       (20)     9107 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/external/blast/BlastExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12570 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/external/blast/BlastHit.py
+-rw-r--r--   0 patrick    (501) staff       (20)    23488 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/external/blast/BlastResult.py
+-rw-r--r--   0 patrick    (501) staff       (20)       83 2023-07-19 22:57:19.000000 SBILib-0.3.4/src/SBILib/external/blast/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8072 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/external/blast/blast_parser.py
+-rw-r--r--   0 patrick    (501) staff       (20)      312 2023-07-19 22:57:34.000000 SBILib-0.3.4/src/SBILib/external/configSBI.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.609975 SBILib-0.3.4/src/SBILib/math/
+-rw-r--r--   0 patrick    (501) staff       (20)       19 2023-07-19 22:57:36.000000 SBILib-0.3.4/src/SBILib/math/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-07-19 22:57:35.000000 SBILib-0.3.4/src/SBILib/math/stats.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.618746 SBILib-0.3.4/src/SBILib/sequence/
+-rw-r--r--   0 patrick    (501) staff       (20)     6331 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/sequence/Fasta.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4871 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/sequence/IndexedSeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)    15045 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/sequence/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-07-19 22:57:13.000000 SBILib-0.3.4/src/SBILib/sequence/Sequence.py
+-rw-r--r--   0 patrick    (501) staff       (20)      140 2023-07-19 22:57:10.000000 SBILib-0.3.4/src/SBILib/sequence/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.627436 SBILib-0.3.4/src/SBILib/sequence/alignment/
+-rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-07-19 22:57:04.000000 SBILib-0.3.4/src/SBILib/sequence/alignment/Needleman_Wunsch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    43526 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/sequence/alignment/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-07-19 22:57:04.000000 SBILib-0.3.4/src/SBILib/sequence/alignment/SimilarityMatrix.py
+-rw-r--r--   0 patrick    (501) staff       (20)       93 2023-07-19 22:57:05.000000 SBILib-0.3.4/src/SBILib/sequence/alignment/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.637885 SBILib-0.3.4/src/SBILib/structure/
+-rw-r--r--   0 patrick    (501) staff       (20)    26428 2023-08-05 01:19:49.000000 SBILib-0.3.4/src/SBILib/structure/PDB.py
+-rw-r--r--   0 patrick    (501) staff       (20)      460 2023-07-19 22:54:58.000000 SBILib-0.3.4/src/SBILib/structure/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.648106 SBILib-0.3.4/src/SBILib/structure/atom/
+-rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-07-19 22:55:41.000000 SBILib-0.3.4/src/SBILib/structure/atom/Atom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      659 2023-07-19 22:55:42.000000 SBILib-0.3.4/src/SBILib/structure/atom/AtomOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)      803 2023-07-19 22:55:35.000000 SBILib-0.3.4/src/SBILib/structure/atom/AtomOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3758 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/atom/AtomSeries.py
+-rw-r--r--   0 patrick    (501) staff       (20)      127 2023-07-19 22:55:40.000000 SBILib-0.3.4/src/SBILib/structure/atom/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.664922 SBILib-0.3.4/src/SBILib/structure/chain/
+-rw-r--r--   0 patrick    (501) staff       (20)    19964 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/chain/Chain.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13264 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/chain/ChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2763 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/chain/ChainOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6877 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/chain/ChainOfProtein.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4988 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/chain/ProteinChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)      131 2023-07-19 22:54:38.000000 SBILib-0.3.4/src/SBILib/structure/chain/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.671596 SBILib-0.3.4/src/SBILib/structure/contacts/
+-rw-r--r--   0 patrick    (501) staff       (20)     9010 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/contacts/Complex.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3408 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/contacts/InnerContacts.py
+-rw-r--r--   0 patrick    (501) staff       (20)      277 2023-07-19 22:55:14.000000 SBILib-0.3.4/src/SBILib/structure/contacts/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.681803 SBILib-0.3.4/src/SBILib/structure/contacts/contact/
+-rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-07-19 22:55:19.000000 SBILib-0.3.4/src/SBILib/structure/contacts/contact/Contact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3806 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/contacts/contact/ContactAA.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-07-19 22:55:19.000000 SBILib-0.3.4/src/SBILib/structure/contacts/contact/ContactAH.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3275 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/contacts/contact/ContactAN.py
+-rw-r--r--   0 patrick    (501) staff       (20)      149 2023-07-19 22:55:18.000000 SBILib-0.3.4/src/SBILib/structure/contacts/contact/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.690569 SBILib-0.3.4/src/SBILib/structure/contacts/inner/
+-rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-07-19 22:55:25.000000 SBILib-0.3.4/src/SBILib/structure/contacts/inner/PHInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-07-19 22:55:24.000000 SBILib-0.3.4/src/SBILib/structure/contacts/inner/PPInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)       85 2023-07-19 22:55:24.000000 SBILib-0.3.4/src/SBILib/structure/contacts/inner/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.701668 SBILib-0.3.4/src/SBILib/structure/contacts/interface/
+-rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-07-19 22:55:11.000000 SBILib-0.3.4/src/SBILib/structure/contacts/interface/Interface.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-07-19 22:55:10.000000 SBILib-0.3.4/src/SBILib/structure/contacts/interface/PHInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11115 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/contacts/interface/PNInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-07-19 22:55:11.000000 SBILib-0.3.4/src/SBILib/structure/contacts/interface/PPInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)      157 2023-07-19 22:55:10.000000 SBILib-0.3.4/src/SBILib/structure/contacts/interface/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.706655 SBILib-0.3.4/src/SBILib/structure/geometry/
+-rw-r--r--   0 patrick    (501) staff       (20)    11737 2023-07-19 22:54:32.000000 SBILib-0.3.4/src/SBILib/structure/geometry/RMSD.py
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 22:54:33.000000 SBILib-0.3.4/src/SBILib/structure/geometry/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      662 2023-07-19 22:54:32.000000 SBILib-0.3.4/src/SBILib/structure/geometry/basics.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.728023 SBILib-0.3.4/src/SBILib/structure/header/
+-rw-r--r--   0 patrick    (501) staff       (20)     2282 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/header/BioMolecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3827 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/header/DBreference.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2011 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/header/Experiment.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14754 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/header/Header.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1199 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/header/HeteroAtom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      944 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/header/MiniRes.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7645 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/header/Molecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8530 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/header/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2421 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/header/Site.py
+-rw-r--r--   0 patrick    (501) staff       (20)    18693 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/header/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14368 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/parse_mmCIF.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8541 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/parse_pdb.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.742596 SBILib-0.3.4/src/SBILib/structure/protein/
+-rw-r--r--   0 patrick    (501) staff       (20)    19068 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/protein/Arch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19200 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/protein/SShelper.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-07-19 22:55:29.000000 SBILib-0.3.4/src/SBILib/structure/protein/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-07-19 22:55:34.000000 SBILib-0.3.4/src/SBILib/structure/protein/Sequencer.py
+-rw-r--r--   0 patrick    (501) staff       (20)      134 2023-07-19 22:55:34.000000 SBILib-0.3.4/src/SBILib/structure/protein/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.749876 SBILib-0.3.4/src/SBILib/structure/residue/
+-rw-r--r--   0 patrick    (501) staff       (20)    10771 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/residue/Residue.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10721 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/residue/ResidueOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5357 2023-07-20 15:23:10.000000 SBILib-0.3.4/src/SBILib/structure/residue/ResidueOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)      146 2023-07-19 22:55:02.000000 SBILib-0.3.4/src/SBILib/structure/residue/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.774251 SBILib-0.3.4/src/SBILib/tests/
+-rw-r--r--   0 patrick    (501) staff       (20)      426 2023-07-20 15:27:20.000000 SBILib-0.3.4/src/SBILib/tests/Test.py
+-rw-r--r--   0 patrick    (501) staff       (20)   156217 2023-07-19 23:01:16.000000 SBILib-0.3.4/src/SBILib/tests/Test_1a3q.cif.gz
+-rw-r--r--   0 patrick    (501) staff       (20)    47362 2023-07-19 23:01:16.000000 SBILib-0.3.4/src/SBILib/tests/Test_pdb1a2w.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:17.000000 SBILib-0.3.4/src/SBILib/tests/Test_pdb1a3q.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)   116164 2023-07-19 23:01:18.000000 SBILib-0.3.4/src/SBILib/tests/Test_pdb2ram.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 23:01:17.000000 SBILib-0.3.4/src/SBILib/tests/__ini__.py
+-rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:21.000000 SBILib-0.3.4/src/SBILib/tests/pdb1a3q.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)     9923 2023-07-21 16:09:58.000000 SBILib-0.3.4/src/SBILib/tests/test_modules.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-05 01:27:41.482513 SBILib-0.3.4/src/SBILib.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)    37862 2023-08-05 01:27:41.000000 SBILib-0.3.4/src/SBILib.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     5049 2023-08-05 01:27:41.000000 SBILib-0.3.4/src/SBILib.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-08-05 01:27:41.000000 SBILib-0.3.4/src/SBILib.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       39 2023-08-05 01:27:41.000000 SBILib-0.3.4/src/SBILib.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        7 2023-08-05 01:27:41.000000 SBILib-0.3.4/src/SBILib.egg-info/top_level.txt
```

### Comparing `SBILib-0.3.3/PKG-INFO` & `SBILib-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: SBILib
-Version: 0.3.3
+Version: 0.3.4
+Summary: UNKNOWN
 Home-page: https://github.com/structuralbioinformatics/SBI
 Author: Patrick Gohl
 Author-email: patrick.gohl@upf.edu
 License: MIT
 Keywords: Structural Bioinformatics,Loops
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Welcome to the StructuralBioInformatics pylib
 
 The **SBILib** python library is a continuous work in progress that clusters functionalities to work with data derived from [PDB][1], from creating a local PDB repository to do _real_ Blast searches over PDB sequences (i.e. sequences of the really crystallized protein sections) to perform a simply split chains (separate the sections of a PDB file).
 
 
@@ -20,15 +22,15 @@
 [1]: http://www.pdb.org/
 
 
 # SBILib Library Manual 
 
 This manual contains a short turorial split into 6 common Tasks.<br/>
 Information on how to access more detailed help pages within python is provided at the end.<br/>
-We have made available a list of slightly more complex scenarios on which the SBILib library may be applied. In Scenarios.md (https://github.com/structuralbioinformatics/SBI)
+We have made available a list of slightly more complex scenarios on which the SBILib library may be applied. In Scenarios.md (https://github.com/structuralbioinformatics/SBILib)
 
 ### Dependencies
 python3 <br/>
 scipy <br/>
 numpy <br/>
 DSSP <br/>
 BLAST <br/>
@@ -44,18 +46,18 @@
 
 This command will install the package locally.<br/>
 
 
 It can also be directly cloned from our github repo:<br/>
 
 ```console
-git clone https://github.com/structuralbioinformatics/SBI
+git clone https://github.com/structuralbioinformatics/SBILib
 ```
 
-Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBI and copy the folder manually.<br/>
+Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBILib and copy the folder manually.<br/>
 
 
 ## Testing:
 We have implemented unit testing. After installation these scripts can be run to ensure that the package is functioning as it should.
 These scripts are located in the directory "tests". Due to size limits we werent able to provide the database file needed for BLAST through PyPi. This file, will be automatically downloaded from https://www.ebi.ac.uk/uniprot/download-center once the unit tests are conducted. Later users may define their own Blast database file as outlined in the BLAST section of this tutorial. IMPORTANT before running ensure that external dependencies are properly configured as per TASK 2.2. 
 ```console
 pip show SBILib | grep Location
@@ -148,15 +150,15 @@
 ChainA.renumerate_residues(1)
 ChainA.renumerate_atoms(1)
 
 ChainA.aminoacids
 
 ```
 
-This list all of the amino acids in the Chain and its atoms.<br/>
+This lists all of the amino acids in the Chain and its atoms.<br/>
 The selection can be more specific by selecting one amino acid from the list.<br/>
 We can access the number (the position of the amino acid on the chain)<br/>
 The type of amino acid (three letter code and single letter).<br/>
 The coordinates of the O, C, CA and CB (if present)<br/>
 The coordinates of the backbone atoms.<br/>
 
 
@@ -538,15 +540,15 @@
 
 ```
 
 ### 5) Find Results with matching secondary structure
 
 The secondary structure of a protein plays a vital role in its function.<br/>
 The SBILib package allows for the quick viewing of how secondary structure is represented in an alignment.<br/>
-Are vital secondary structure element located in a gap resulting in a homolog with unequal function?<br/>
+Are vital secondary structure elements located in a gap resulting in a homolog with unequal function?<br/>
 Here we demonstrate how this can be analyzed.<br/>
 
 ```{python}
 
 blastresults.str_PIR(result = 13)
 
 
@@ -563,15 +565,15 @@
 #KNEPYKPHPHDLVGKGCRD-GYYEAEFGPERQVLSFQNLGIQCVKKKDLKESISLRISK-
 #--KINPFNVPEEQLHNIDE--------YDLNVVRLCFQAFLPDEHGNYTLALPPLISNPI
 #YDNRAPNTAELRICRVNKNCGSVKGGDEIFLLCDKVQKDDIEVRFVLGN---WEAKGSFS
 #QADVHRQVAIVFRTPPFLG-DITEPITVKMQLRRPSDQAVSEPVDFRYLP*
 
 
 ```
-This wil output a PIR format alignment of the two proteins. Dashes in the target protein (second sequence of the PIR) indicate gaps in the alignment. We are interestsed in seeing what secondary structure elements (if any) may have gone missing as a result of these gaps.  
+This will output a PIR format alignment of the two proteins. Dashes in the target protein (second sequence of the PIR) indicate gaps in the alignment. We are interested in seeing what secondary structure elements (if any) may have gone missing as a result of these gaps.  
 ```{python}
 
 string = blastresults.str_PIR(result = 13)
 indices = [i for i, c in enumerate("".join(string.split(">")[2].split("\n")[2:]))if c == "-"]
 i = 0    
 string= ""
 for char in ChainA.gapped_protein_secondary_structure:
@@ -822,16 +824,16 @@
 #THETA: 98.69428 RHO: 74.28570 DELTA: 58.26752
 #**
 
 
 
 ```
 The output of the archs command is a list of the loop geometries calculated for the given chain (ChainA)<br/>
-We get the first secondary structure that flanks the loop. In parantheses the structure type (see Task2.3) it's start, length and end.<br/>
-An axis for flanking secondary structures 1 defined based on the shortest of the principal moments of inertia for that structures. <br/>
+We get the first secondary structure that flanks the loop. In parentheses the structure type (see Task2.3) it's start, length and end.<br/>
+An axis for flanking secondary structures 1 defined based on the shortest of the principal moments of inertia for that structure. <br/>
 The same information is printed out for the second flanking structure.<br/>
 The arch Type is printed:<br/>
 BK: beta-link<br/>
 BN: beta-hairpin<br/>
 EG: beta-helix310<br/>
 EH: beta-alpha helix<br/>
 GE: helix310-beta<br/>
@@ -860,22 +862,22 @@
 
 
 
 ## Task 6
 
 ### Loop Grafting
 
-We will show how SBILib may be used to graft the loop of one protein into the structure of another protein with similiar loop geometry. 
+We will show how SBILib may be used to graft the loop of one protein into the structure of another protein with similar loop geometry. 
 
 ```{python}
 
 new = PDBlink()
 path = new.get_PDB("2ram")
 protein2 = PDB(path)
-report = protein.compare_loops(self.protein2)
+report = protein.compare_loops(protein2)
 report[0]
 
 # 'QueryProt:A,176,182:TargetProt:A,160,166:VISQPIH,VLSHPIF'
 
 ```
 These Commands took the protein previously defined (1a3q here QueryProt) and for each loop within that protein searched for loops in the TargetProt (2ram) with matching geometries. These pairs are saved in a list (here defined by the variable report). Each element (loop matches) of that list is composed of a string with the format seen above. QueryProt:A refers to the first loop (from the query protein) being located on chain A. 176,182 the start and end positions of that loop respectively. TargetProt:A the second loop is found on chain A of the target protein. 160,166 our start and end positions. VISQPIH,VLSHPIF are the sequences for the Query protein and Target protein loops respectively. 
 We define loop geometries to be similar if all of the following conditions are met:<br/>
@@ -1032,9 +1034,11 @@
 
 
 
 
 
 
 
+
+
```

### Comparing `SBILib-0.3.3/README.md` & `SBILib-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [1]: http://www.pdb.org/
 
 
 # SBILib Library Manual 
 
 This manual contains a short turorial split into 6 common Tasks.<br/>
 Information on how to access more detailed help pages within python is provided at the end.<br/>
-We have made available a list of slightly more complex scenarios on which the SBILib library may be applied. In Scenarios.md (https://github.com/structuralbioinformatics/SBI)
+We have made available a list of slightly more complex scenarios on which the SBILib library may be applied. In Scenarios.md (https://github.com/structuralbioinformatics/SBILib)
 
 ### Dependencies
 python3 <br/>
 scipy <br/>
 numpy <br/>
 DSSP <br/>
 BLAST <br/>
@@ -34,18 +34,18 @@
 
 This command will install the package locally.<br/>
 
 
 It can also be directly cloned from our github repo:<br/>
 
 ```console
-git clone https://github.com/structuralbioinformatics/SBI
+git clone https://github.com/structuralbioinformatics/SBILib
 ```
 
-Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBI and copy the folder manually.<br/>
+Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBILib and copy the folder manually.<br/>
 
 
 ## Testing:
 We have implemented unit testing. After installation these scripts can be run to ensure that the package is functioning as it should.
 These scripts are located in the directory "tests". Due to size limits we werent able to provide the database file needed for BLAST through PyPi. This file, will be automatically downloaded from https://www.ebi.ac.uk/uniprot/download-center once the unit tests are conducted. Later users may define their own Blast database file as outlined in the BLAST section of this tutorial. IMPORTANT before running ensure that external dependencies are properly configured as per TASK 2.2. 
 ```console
 pip show SBILib | grep Location
@@ -138,15 +138,15 @@
 ChainA.renumerate_residues(1)
 ChainA.renumerate_atoms(1)
 
 ChainA.aminoacids
 
 ```
 
-This list all of the amino acids in the Chain and its atoms.<br/>
+This lists all of the amino acids in the Chain and its atoms.<br/>
 The selection can be more specific by selecting one amino acid from the list.<br/>
 We can access the number (the position of the amino acid on the chain)<br/>
 The type of amino acid (three letter code and single letter).<br/>
 The coordinates of the O, C, CA and CB (if present)<br/>
 The coordinates of the backbone atoms.<br/>
 
 
@@ -528,15 +528,15 @@
 
 ```
 
 ### 5) Find Results with matching secondary structure
 
 The secondary structure of a protein plays a vital role in its function.<br/>
 The SBILib package allows for the quick viewing of how secondary structure is represented in an alignment.<br/>
-Are vital secondary structure element located in a gap resulting in a homolog with unequal function?<br/>
+Are vital secondary structure elements located in a gap resulting in a homolog with unequal function?<br/>
 Here we demonstrate how this can be analyzed.<br/>
 
 ```{python}
 
 blastresults.str_PIR(result = 13)
 
 
@@ -553,15 +553,15 @@
 #KNEPYKPHPHDLVGKGCRD-GYYEAEFGPERQVLSFQNLGIQCVKKKDLKESISLRISK-
 #--KINPFNVPEEQLHNIDE--------YDLNVVRLCFQAFLPDEHGNYTLALPPLISNPI
 #YDNRAPNTAELRICRVNKNCGSVKGGDEIFLLCDKVQKDDIEVRFVLGN---WEAKGSFS
 #QADVHRQVAIVFRTPPFLG-DITEPITVKMQLRRPSDQAVSEPVDFRYLP*
 
 
 ```
-This wil output a PIR format alignment of the two proteins. Dashes in the target protein (second sequence of the PIR) indicate gaps in the alignment. We are interestsed in seeing what secondary structure elements (if any) may have gone missing as a result of these gaps.  
+This will output a PIR format alignment of the two proteins. Dashes in the target protein (second sequence of the PIR) indicate gaps in the alignment. We are interested in seeing what secondary structure elements (if any) may have gone missing as a result of these gaps.  
 ```{python}
 
 string = blastresults.str_PIR(result = 13)
 indices = [i for i, c in enumerate("".join(string.split(">")[2].split("\n")[2:]))if c == "-"]
 i = 0    
 string= ""
 for char in ChainA.gapped_protein_secondary_structure:
@@ -812,16 +812,16 @@
 #THETA: 98.69428 RHO: 74.28570 DELTA: 58.26752
 #**
 
 
 
 ```
 The output of the archs command is a list of the loop geometries calculated for the given chain (ChainA)<br/>
-We get the first secondary structure that flanks the loop. In parantheses the structure type (see Task2.3) it's start, length and end.<br/>
-An axis for flanking secondary structures 1 defined based on the shortest of the principal moments of inertia for that structures. <br/>
+We get the first secondary structure that flanks the loop. In parentheses the structure type (see Task2.3) it's start, length and end.<br/>
+An axis for flanking secondary structures 1 defined based on the shortest of the principal moments of inertia for that structure. <br/>
 The same information is printed out for the second flanking structure.<br/>
 The arch Type is printed:<br/>
 BK: beta-link<br/>
 BN: beta-hairpin<br/>
 EG: beta-helix310<br/>
 EH: beta-alpha helix<br/>
 GE: helix310-beta<br/>
@@ -850,22 +850,22 @@
 
 
 
 ## Task 6
 
 ### Loop Grafting
 
-We will show how SBILib may be used to graft the loop of one protein into the structure of another protein with similiar loop geometry. 
+We will show how SBILib may be used to graft the loop of one protein into the structure of another protein with similar loop geometry. 
 
 ```{python}
 
 new = PDBlink()
 path = new.get_PDB("2ram")
 protein2 = PDB(path)
-report = protein.compare_loops(self.protein2)
+report = protein.compare_loops(protein2)
 report[0]
 
 # 'QueryProt:A,176,182:TargetProt:A,160,166:VISQPIH,VLSHPIF'
 
 ```
 These Commands took the protein previously defined (1a3q here QueryProt) and for each loop within that protein searched for loops in the TargetProt (2ram) with matching geometries. These pairs are saved in a list (here defined by the variable report). Each element (loop matches) of that list is composed of a string with the format seen above. QueryProt:A refers to the first loop (from the query protein) being located on chain A. 176,182 the start and end positions of that loop respectively. TargetProt:A the second loop is found on chain A of the target protein. 160,166 our start and end positions. VISQPIH,VLSHPIF are the sequences for the Query protein and Target protein loops respectively. 
 We define loop geometries to be similar if all of the following conditions are met:<br/>
```

### Comparing `SBILib-0.3.3/Scenarios.md` & `SBILib-0.3.4/Scenarios.md`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/setup.py` & `SBILib-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md') as f:
     readme = f.read()
 
 
 setup(
     name='SBILib',
-    version='0.3.3',
+    version='0.3.4',
     license='MIT',
     author="Patrick Gohl",
     author_email='patrick.gohl@upf.edu',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     include_package_data=True,
     long_description=readme,
```

### Comparing `SBILib-0.3.3/src/SBILib/__init__.py` & `SBILib-0.3.4/src/SBILib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 import os
 import traceback
 import datetime
 import time
 import logging
 
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 
 
 class Parameters(object):
     '''
     Designed to work through all the {SBI} library.
     It contains several parameters that will control (a) the amount of data
     shown to the user during the execution of {SBI} subroutines and (b) the
```

### Comparing `SBILib-0.3.3/src/SBILib/beans/Executable.py` & `SBILib-0.3.4/src/SBILib/beans/Executable.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/beans/File.py` & `SBILib-0.3.4/src/SBILib/beans/File.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/beans/IndexedNum.py` & `SBILib-0.3.4/src/SBILib/beans/IndexedNum.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/beans/Path.py` & `SBILib-0.3.4/src/SBILib/beans/Path.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/beans/StorableObject.py` & `SBILib-0.3.4/src/SBILib/beans/StorableObject.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/beans/butler.py` & `SBILib-0.3.4/src/SBILib/beans/butler.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/beans/singleton.py` & `SBILib-0.3.4/src/SBILib/beans/singleton.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/data/Alphabet.py` & `SBILib-0.3.4/src/SBILib/data/Alphabet.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/data/AminoAcids.py` & `SBILib-0.3.4/src/SBILib/data/AminoAcids.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/data/AtomVariants.py` & `SBILib-0.3.4/src/SBILib/data/AtomVariants.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/data/Element.py` & `SBILib-0.3.4/src/SBILib/data/Element.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/data/Properties.py` & `SBILib-0.3.4/src/SBILib/data/Properties.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/data/SetDict.py` & `SBILib-0.3.4/src/SBILib/data/SetDict.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/data/__init__.py` & `SBILib-0.3.4/src/SBILib/data/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/CATHlink.py` & `SBILib-0.3.4/src/SBILib/databases/CATHlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/DrugBanklink.py` & `SBILib-0.3.4/src/SBILib/databases/DrugBanklink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/Enzymelink.py` & `SBILib-0.3.4/src/SBILib/databases/Enzymelink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/GOlink.py` & `SBILib-0.3.4/src/SBILib/databases/GOlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/PDBTMlink.py` & `SBILib-0.3.4/src/SBILib/databases/PDBTMlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/PDBeChemlink.py` & `SBILib-0.3.4/src/SBILib/databases/PDBeChemlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/PDBlink.py` & `SBILib-0.3.4/src/SBILib/databases/PDBlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/SCOPlink.py` & `SBILib-0.3.4/src/SBILib/databases/SCOPlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/TaxIDlink.py` & `SBILib-0.3.4/src/SBILib/databases/TaxIDlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/Uniprotlink.py` & `SBILib-0.3.4/src/SBILib/databases/Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/__Uniprotlink.py` & `SBILib-0.3.4/src/SBILib/databases/__Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/__init__.py` & `SBILib-0.3.4/src/SBILib/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/dblink.py` & `SBILib-0.3.4/src/SBILib/databases/dblink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/uniprot/connect.py` & `SBILib-0.3.4/src/SBILib/databases/uniprot/connect.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/databases/uniprot/uniprot.py` & `SBILib-0.3.4/src/SBILib/databases/uniprot/uniprot.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/error/BlastError.py` & `SBILib-0.3.4/src/SBILib/error/BlastError.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/error/FileError.py` & `SBILib-0.3.4/src/SBILib/error/FileError.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/error/SeqAliError.py` & `SBILib-0.3.4/src/SBILib/error/SeqAliError.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/external/CDhit/CDhit.py` & `SBILib-0.3.4/src/SBILib/external/CDhit/CDhit.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/external/CDhit/CDhitExe.py` & `SBILib-0.3.4/src/SBILib/external/CDhit/CDhitExe.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/external/CDhit/CDhitHomolog.py` & `SBILib-0.3.4/src/SBILib/external/CDhit/CDhitHomolog.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/external/CDhit/CDhitList.py` & `SBILib-0.3.4/src/SBILib/external/CDhit/CDhitList.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/external/DSSP/DSSP.py` & `SBILib-0.3.4/src/SBILib/external/DSSP/DSSP.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/external/DSSP/DSSPExe.py` & `SBILib-0.3.4/src/SBILib/external/DSSP/DSSPExe.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/external/blast/BlastExe.py` & `SBILib-0.3.4/src/SBILib/external/blast/BlastExe.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/external/blast/BlastHit.py` & `SBILib-0.3.4/src/SBILib/external/blast/BlastHit.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/external/blast/BlastResult.py` & `SBILib-0.3.4/src/SBILib/external/blast/BlastResult.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/external/blast/blast_parser.py` & `SBILib-0.3.4/src/SBILib/external/blast/blast_parser.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/math/stats.py` & `SBILib-0.3.4/src/SBILib/math/stats.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/sequence/Fasta.py` & `SBILib-0.3.4/src/SBILib/sequence/Fasta.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/sequence/IndexedSeqAli.py` & `SBILib-0.3.4/src/SBILib/sequence/IndexedSeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/sequence/SeqAli.py` & `SBILib-0.3.4/src/SBILib/sequence/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/sequence/Sequence.py` & `SBILib-0.3.4/src/SBILib/sequence/Sequence.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/sequence/alignment/Needleman_Wunsch.py` & `SBILib-0.3.4/src/SBILib/sequence/alignment/Needleman_Wunsch.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/sequence/alignment/SeqAli.py` & `SBILib-0.3.4/src/SBILib/sequence/alignment/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/sequence/alignment/SimilarityMatrix.py` & `SBILib-0.3.4/src/SBILib/sequence/alignment/SimilarityMatrix.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/PDB.py` & `SBILib-0.3.4/src/SBILib/structure/PDB.py`

 * *Files 4% similar despite different names*

```diff
@@ -685,36 +685,48 @@
 
     """ 
     Grafting a selected loop pair 
     """
     def graft(self, PDB2, selection):
         # gathering loop info from selection
         query_chain_id = selection.split(":")[1].split(",")[0]
-        query_start = selection.split(":")[1].split(",")[1]
-        query_end = selection.split(":")[1].split(",")[2]
+        query_start_1 = str(int(selection.split(":")[1].split(",")[1]) - 2)
+        query_end_1 = selection.split(":")[1].split(",")[1]
+        query_start_2 = selection.split(":")[1].split(",")[2]
+        query_end_2 = str(int(selection.split(":")[1].split(",")[2]) + 2) 
+        #query_start = selection.split(":")[1].split(",")[1]
+        #query_end = selection.split(":")[1].split(",")[2]
         target_chain_id = selection.split(":")[3].split(",")[0]
-        target_start = selection.split(":")[3].split(",")[1]
-        target_end = selection.split(":")[3].split(",")[2]
+        target_start_1 = str(int(selection.split(":")[3].split(",")[1]) -2)
+        target_end_1 = selection.split(":")[3].split(",")[1]
+        target_start_2 = selection.split(":")[3].split(",")[2]
+        target_end_2 = str(int(selection.split(":")[3].split(",")[2]) + 2)
+        #target_start = selection.split(":")[3].split(",")[1]
+        #target_end = selection.split(":")[3].split(",")[2]
 
         # grabbing the chains with selected loops
         query_chain = self.get_chain_by_id(query_chain_id)
         target_chain = PDB2.get_chain_by_id(target_chain_id)
 
         #grabbing the guiding loop 
-        nguide = query_chain.extract(int(query_start)-1 , int(query_end) - 1 , backbone=True)
+        nguide = query_chain.extract(int(query_start_1)-1 , int(query_end_1) - 1 , backbone=True)
+        addition = query_chain.extract(int(query_start_2)-1 , int(query_end_2) - 1 , backbone=True)
+        nguide._add_residues(addition._all_residues)
         # retriveing vector and center of guide
         nguide_vector = []
         for r in nguide.aminoacids:
             for a in r.atoms:
                 nguide_vector.append(numpy.copy(a.coordinates))
 
         nguide_center = numpy.mean(nguide_vector, axis = 0, dtype = numpy.float64)
 
         # Doing the same for the target loop
-        nquery = target_chain.extract(int(target_start) -1 , int(target_end)-1 , backbone=True)
+        nquery = target_chain.extract(int(target_start_1) -1 , int(target_end_1)-1 , backbone=True)
+        addition = target_chain.extract(int(target_start_2) -1 , int(target_end_2)-1 , backbone=True)
+        nquery._add_residues(addition._all_residues)
         nquery_vector = []
         for r in nquery.aminoacids:
             for a in r.atoms:
                 nquery_vector.append(numpy.copy(a.coordinates))
 
         nquery_center = numpy.mean(nquery_vector, axis = 0, dtype = numpy.float64)
```

### Comparing `SBILib-0.3.3/src/SBILib/structure/atom/Atom.py` & `SBILib-0.3.4/src/SBILib/structure/atom/Atom.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/atom/AtomOfAminoAcid.py` & `SBILib-0.3.4/src/SBILib/structure/atom/AtomOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/atom/AtomOfNucleotide.py` & `SBILib-0.3.4/src/SBILib/structure/atom/AtomOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/atom/AtomSeries.py` & `SBILib-0.3.4/src/SBILib/structure/atom/AtomSeries.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/chain/Chain.py` & `SBILib-0.3.4/src/SBILib/structure/chain/Chain.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/chain/ChainFrame.py` & `SBILib-0.3.4/src/SBILib/structure/chain/ChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/chain/ChainOfNucleotide.py` & `SBILib-0.3.4/src/SBILib/structure/chain/ChainOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/chain/ChainOfProtein.py` & `SBILib-0.3.4/src/SBILib/structure/chain/ChainOfProtein.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/chain/ProteinChainFrame.py` & `SBILib-0.3.4/src/SBILib/structure/chain/ProteinChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/Complex.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/Complex.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/InnerContacts.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/InnerContacts.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/contact/Contact.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/contact/Contact.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAA.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/contact/ContactAA.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAH.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/contact/ContactAH.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAN.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/contact/ContactAN.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/inner/PHInnerContact.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/inner/PHInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/inner/PPInnerContact.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/inner/PPInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/interface/Interface.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/interface/Interface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/interface/PHInterface.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/interface/PHInterface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/interface/PNInterface.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/interface/PNInterface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/contacts/interface/PPInterface.py` & `SBILib-0.3.4/src/SBILib/structure/contacts/interface/PPInterface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/geometry/RMSD.py` & `SBILib-0.3.4/src/SBILib/structure/geometry/RMSD.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/geometry/basics.py` & `SBILib-0.3.4/src/SBILib/structure/geometry/basics.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/header/BioMolecule.py` & `SBILib-0.3.4/src/SBILib/structure/header/BioMolecule.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/header/DBreference.py` & `SBILib-0.3.4/src/SBILib/structure/header/DBreference.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/header/Experiment.py` & `SBILib-0.3.4/src/SBILib/structure/header/Experiment.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/header/Header.py` & `SBILib-0.3.4/src/SBILib/structure/header/Header.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/header/HeteroAtom.py` & `SBILib-0.3.4/src/SBILib/structure/header/HeteroAtom.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/header/MiniRes.py` & `SBILib-0.3.4/src/SBILib/structure/header/MiniRes.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/header/Molecule.py` & `SBILib-0.3.4/src/SBILib/structure/header/Molecule.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/header/SecondaryStructure.py` & `SBILib-0.3.4/src/SBILib/structure/header/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/header/Site.py` & `SBILib-0.3.4/src/SBILib/structure/header/Site.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/header/__init__.py` & `SBILib-0.3.4/src/SBILib/structure/header/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/parse_mmCIF.py` & `SBILib-0.3.4/src/SBILib/structure/parse_mmCIF.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/parse_pdb.py` & `SBILib-0.3.4/src/SBILib/structure/parse_pdb.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/protein/Arch.py` & `SBILib-0.3.4/src/SBILib/structure/protein/Arch.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/protein/SShelper.py` & `SBILib-0.3.4/src/SBILib/structure/protein/SShelper.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/protein/SecondaryStructure.py` & `SBILib-0.3.4/src/SBILib/structure/protein/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/protein/Sequencer.py` & `SBILib-0.3.4/src/SBILib/structure/protein/Sequencer.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/residue/Residue.py` & `SBILib-0.3.4/src/SBILib/structure/residue/Residue.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/residue/ResidueOfAminoAcid.py` & `SBILib-0.3.4/src/SBILib/structure/residue/ResidueOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/structure/residue/ResidueOfNucleotide.py` & `SBILib-0.3.4/src/SBILib/structure/residue/ResidueOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/tests/Test_1a3q.cif.gz` & `SBILib-0.3.4/src/SBILib/tests/Test_1a3q.cif.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/tests/Test_pdb1a2w.ent.gz` & `SBILib-0.3.4/src/SBILib/tests/Test_pdb1a2w.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/tests/Test_pdb1a3q.ent.gz` & `SBILib-0.3.4/src/SBILib/tests/Test_pdb1a3q.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/tests/Test_pdb2ram.ent.gz` & `SBILib-0.3.4/src/SBILib/tests/Test_pdb2ram.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/tests/pdb1a3q.ent.gz` & `SBILib-0.3.4/src/SBILib/tests/pdb1a3q.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib/tests/test_modules.py` & `SBILib-0.3.4/src/SBILib/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.3/src/SBILib.egg-info/PKG-INFO` & `SBILib-0.3.4/src/SBILib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: SBILib
-Version: 0.3.3
+Version: 0.3.4
+Summary: UNKNOWN
 Home-page: https://github.com/structuralbioinformatics/SBI
 Author: Patrick Gohl
 Author-email: patrick.gohl@upf.edu
 License: MIT
 Keywords: Structural Bioinformatics,Loops
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Welcome to the StructuralBioInformatics pylib
 
 The **SBILib** python library is a continuous work in progress that clusters functionalities to work with data derived from [PDB][1], from creating a local PDB repository to do _real_ Blast searches over PDB sequences (i.e. sequences of the really crystallized protein sections) to perform a simply split chains (separate the sections of a PDB file).
 
 
@@ -20,15 +22,15 @@
 [1]: http://www.pdb.org/
 
 
 # SBILib Library Manual 
 
 This manual contains a short turorial split into 6 common Tasks.<br/>
 Information on how to access more detailed help pages within python is provided at the end.<br/>
-We have made available a list of slightly more complex scenarios on which the SBILib library may be applied. In Scenarios.md (https://github.com/structuralbioinformatics/SBI)
+We have made available a list of slightly more complex scenarios on which the SBILib library may be applied. In Scenarios.md (https://github.com/structuralbioinformatics/SBILib)
 
 ### Dependencies
 python3 <br/>
 scipy <br/>
 numpy <br/>
 DSSP <br/>
 BLAST <br/>
@@ -44,18 +46,18 @@
 
 This command will install the package locally.<br/>
 
 
 It can also be directly cloned from our github repo:<br/>
 
 ```console
-git clone https://github.com/structuralbioinformatics/SBI
+git clone https://github.com/structuralbioinformatics/SBILib
 ```
 
-Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBI and copy the folder manually.<br/>
+Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBILib and copy the folder manually.<br/>
 
 
 ## Testing:
 We have implemented unit testing. After installation these scripts can be run to ensure that the package is functioning as it should.
 These scripts are located in the directory "tests". Due to size limits we werent able to provide the database file needed for BLAST through PyPi. This file, will be automatically downloaded from https://www.ebi.ac.uk/uniprot/download-center once the unit tests are conducted. Later users may define their own Blast database file as outlined in the BLAST section of this tutorial. IMPORTANT before running ensure that external dependencies are properly configured as per TASK 2.2. 
 ```console
 pip show SBILib | grep Location
@@ -148,15 +150,15 @@
 ChainA.renumerate_residues(1)
 ChainA.renumerate_atoms(1)
 
 ChainA.aminoacids
 
 ```
 
-This list all of the amino acids in the Chain and its atoms.<br/>
+This lists all of the amino acids in the Chain and its atoms.<br/>
 The selection can be more specific by selecting one amino acid from the list.<br/>
 We can access the number (the position of the amino acid on the chain)<br/>
 The type of amino acid (three letter code and single letter).<br/>
 The coordinates of the O, C, CA and CB (if present)<br/>
 The coordinates of the backbone atoms.<br/>
 
 
@@ -538,15 +540,15 @@
 
 ```
 
 ### 5) Find Results with matching secondary structure
 
 The secondary structure of a protein plays a vital role in its function.<br/>
 The SBILib package allows for the quick viewing of how secondary structure is represented in an alignment.<br/>
-Are vital secondary structure element located in a gap resulting in a homolog with unequal function?<br/>
+Are vital secondary structure elements located in a gap resulting in a homolog with unequal function?<br/>
 Here we demonstrate how this can be analyzed.<br/>
 
 ```{python}
 
 blastresults.str_PIR(result = 13)
 
 
@@ -563,15 +565,15 @@
 #KNEPYKPHPHDLVGKGCRD-GYYEAEFGPERQVLSFQNLGIQCVKKKDLKESISLRISK-
 #--KINPFNVPEEQLHNIDE--------YDLNVVRLCFQAFLPDEHGNYTLALPPLISNPI
 #YDNRAPNTAELRICRVNKNCGSVKGGDEIFLLCDKVQKDDIEVRFVLGN---WEAKGSFS
 #QADVHRQVAIVFRTPPFLG-DITEPITVKMQLRRPSDQAVSEPVDFRYLP*
 
 
 ```
-This wil output a PIR format alignment of the two proteins. Dashes in the target protein (second sequence of the PIR) indicate gaps in the alignment. We are interestsed in seeing what secondary structure elements (if any) may have gone missing as a result of these gaps.  
+This will output a PIR format alignment of the two proteins. Dashes in the target protein (second sequence of the PIR) indicate gaps in the alignment. We are interested in seeing what secondary structure elements (if any) may have gone missing as a result of these gaps.  
 ```{python}
 
 string = blastresults.str_PIR(result = 13)
 indices = [i for i, c in enumerate("".join(string.split(">")[2].split("\n")[2:]))if c == "-"]
 i = 0    
 string= ""
 for char in ChainA.gapped_protein_secondary_structure:
@@ -822,16 +824,16 @@
 #THETA: 98.69428 RHO: 74.28570 DELTA: 58.26752
 #**
 
 
 
 ```
 The output of the archs command is a list of the loop geometries calculated for the given chain (ChainA)<br/>
-We get the first secondary structure that flanks the loop. In parantheses the structure type (see Task2.3) it's start, length and end.<br/>
-An axis for flanking secondary structures 1 defined based on the shortest of the principal moments of inertia for that structures. <br/>
+We get the first secondary structure that flanks the loop. In parentheses the structure type (see Task2.3) it's start, length and end.<br/>
+An axis for flanking secondary structures 1 defined based on the shortest of the principal moments of inertia for that structure. <br/>
 The same information is printed out for the second flanking structure.<br/>
 The arch Type is printed:<br/>
 BK: beta-link<br/>
 BN: beta-hairpin<br/>
 EG: beta-helix310<br/>
 EH: beta-alpha helix<br/>
 GE: helix310-beta<br/>
@@ -860,22 +862,22 @@
 
 
 
 ## Task 6
 
 ### Loop Grafting
 
-We will show how SBILib may be used to graft the loop of one protein into the structure of another protein with similiar loop geometry. 
+We will show how SBILib may be used to graft the loop of one protein into the structure of another protein with similar loop geometry. 
 
 ```{python}
 
 new = PDBlink()
 path = new.get_PDB("2ram")
 protein2 = PDB(path)
-report = protein.compare_loops(self.protein2)
+report = protein.compare_loops(protein2)
 report[0]
 
 # 'QueryProt:A,176,182:TargetProt:A,160,166:VISQPIH,VLSHPIF'
 
 ```
 These Commands took the protein previously defined (1a3q here QueryProt) and for each loop within that protein searched for loops in the TargetProt (2ram) with matching geometries. These pairs are saved in a list (here defined by the variable report). Each element (loop matches) of that list is composed of a string with the format seen above. QueryProt:A refers to the first loop (from the query protein) being located on chain A. 176,182 the start and end positions of that loop respectively. TargetProt:A the second loop is found on chain A of the target protein. 160,166 our start and end positions. VISQPIH,VLSHPIF are the sequences for the Query protein and Target protein loops respectively. 
 We define loop geometries to be similar if all of the following conditions are met:<br/>
@@ -1032,9 +1034,11 @@
 
 
 
 
 
 
 
+
+
```

### Comparing `SBILib-0.3.3/src/SBILib.egg-info/SOURCES.txt` & `SBILib-0.3.4/src/SBILib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

