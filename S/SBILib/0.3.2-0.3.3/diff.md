# Comparing `tmp/SBILib-0.3.2.tar.gz` & `tmp/SBILib-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SBILib-0.3.2.tar", last modified: Fri Jul 21 16:14:42 2023, max compression
+gzip compressed data, was "SBILib-0.3.3.tar", last modified: Sat Jul 22 21:19:59 2023, max compression
```

## Comparing `SBILib-0.3.2.tar` & `SBILib-0.3.3.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.807696 SBILib-0.3.2/
--rw-r--r--   0 patrick    (501) staff       (20)      128 2023-07-21 15:34:16.000000 SBILib-0.3.2/MANIFEST.in
--rw-r--r--   0 patrick    (501) staff       (20)    25858 2023-07-21 16:14:42.808001 SBILib-0.3.2/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)    25597 2023-07-20 16:37:41.000000 SBILib-0.3.2/README.md
--rw-r--r--   0 patrick    (501) staff       (20)     6077 2023-07-19 23:01:24.000000 SBILib-0.3.2/Scenarios.md
--rw-r--r--   0 patrick    (501) staff       (20)      103 2023-07-21 16:14:42.809348 SBILib-0.3.2/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)      621 2023-07-21 16:12:19.000000 SBILib-0.3.2/setup.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.490268 SBILib-0.3.2/src/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.507323 SBILib-0.3.2/src/SBILib/
--rw-r--r--   0 patrick    (501) staff       (20)    12951 2023-07-21 15:36:22.000000 SBILib-0.3.2/src/SBILib/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.532662 SBILib-0.3.2/src/SBILib/beans/
--rw-r--r--   0 patrick    (501) staff       (20)     4500 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/beans/Executable.py
--rw-r--r--   0 patrick    (501) staff       (20)    11699 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/beans/File.py
--rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-07-19 22:56:14.000000 SBILib-0.3.2/src/SBILib/beans/IndexedNum.py
--rw-r--r--   0 patrick    (501) staff       (20)      349 2023-07-19 22:56:22.000000 SBILib-0.3.2/src/SBILib/beans/JSONer.py
--rw-r--r--   0 patrick    (501) staff       (20)    14930 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/beans/Path.py
--rw-r--r--   0 patrick    (501) staff       (20)     2926 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/beans/StorableObject.py
--rw-r--r--   0 patrick    (501) staff       (20)      187 2023-07-19 22:56:21.000000 SBILib-0.3.2/src/SBILib/beans/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-07-19 22:56:20.000000 SBILib-0.3.2/src/SBILib/beans/butler.py
--rw-r--r--   0 patrick    (501) staff       (20)      516 2023-07-19 22:56:23.000000 SBILib-0.3.2/src/SBILib/beans/singleton.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.551570 SBILib-0.3.2/src/SBILib/data/
--rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-07-19 22:55:56.000000 SBILib-0.3.2/src/SBILib/data/Alphabet.py
--rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-07-19 22:55:49.000000 SBILib-0.3.2/src/SBILib/data/AminoAcids.py
--rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-07-19 22:55:54.000000 SBILib-0.3.2/src/SBILib/data/AtomVariants.py
--rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-07-19 22:55:55.000000 SBILib-0.3.2/src/SBILib/data/Element.py
--rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-07-19 22:55:55.000000 SBILib-0.3.2/src/SBILib/data/Properties.py
--rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-07-19 22:55:57.000000 SBILib-0.3.2/src/SBILib/data/SetDict.py
--rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-07-19 22:55:53.000000 SBILib-0.3.2/src/SBILib/data/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.586132 SBILib-0.3.2/src/SBILib/databases/
--rw-r--r--   0 patrick    (501) staff       (20)      273 2023-07-19 22:56:12.000000 SBILib-0.3.2/src/SBILib/databases/AlphaFoldlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-07-19 22:56:12.000000 SBILib-0.3.2/src/SBILib/databases/CATHlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     8412 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/DrugBanklink.py
--rw-r--r--   0 patrick    (501) staff       (20)    13617 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/Enzymelink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5573 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/GOlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5355 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/PDBTMlink.py
--rw-r--r--   0 patrick    (501) staff       (20)      417 2023-07-19 22:56:01.000000 SBILib-0.3.2/src/SBILib/databases/PDBeChemConnect.py
--rw-r--r--   0 patrick    (501) staff       (20)     6713 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/PDBeChemlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     9123 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/PDBlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     1795 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/SCOPlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     5733 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/TaxIDlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7098 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     7063 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/__Uniprotlink.py
--rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-07-19 22:56:07.000000 SBILib-0.3.2/src/SBILib/databases/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7149 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/dblink.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.592414 SBILib-0.3.2/src/SBILib/databases/uniprot/
--rw-r--r--   0 patrick    (501) staff       (20)       90 2023-07-19 22:56:09.000000 SBILib-0.3.2/src/SBILib/databases/uniprot/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     4777 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/uniprot/connect.py
--rw-r--r--   0 patrick    (501) staff       (20)     8169 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/databases/uniprot/uniprot.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.602206 SBILib-0.3.2/src/SBILib/error/
--rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-07-19 22:55:48.000000 SBILib-0.3.2/src/SBILib/error/BlastError.py
--rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-07-19 22:55:43.000000 SBILib-0.3.2/src/SBILib/error/FileError.py
--rw-r--r--   0 patrick    (501) staff       (20)      896 2023-07-19 22:55:48.000000 SBILib-0.3.2/src/SBILib/error/SeqAliError.py
--rw-r--r--   0 patrick    (501) staff       (20)      108 2023-07-19 22:55:47.000000 SBILib-0.3.2/src/SBILib/error/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.608223 SBILib-0.3.2/src/SBILib/external/
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.620227 SBILib-0.3.2/src/SBILib/external/CDhit/
--rw-r--r--   0 patrick    (501) staff       (20)      964 2023-07-19 22:57:25.000000 SBILib-0.3.2/src/SBILib/external/CDhit/CDhit.py
--rw-r--r--   0 patrick    (501) staff       (20)     2255 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/CDhit/CDhitExe.py
--rw-r--r--   0 patrick    (501) staff       (20)      802 2023-07-19 22:57:26.000000 SBILib-0.3.2/src/SBILib/external/CDhit/CDhitHomolog.py
--rw-r--r--   0 patrick    (501) staff       (20)     2223 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/CDhit/CDhitList.py
--rw-r--r--   0 patrick    (501) staff       (20)       64 2023-07-19 22:57:25.000000 SBILib-0.3.2/src/SBILib/external/CDhit/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.626122 SBILib-0.3.2/src/SBILib/external/DSSP/
--rw-r--r--   0 patrick    (501) staff       (20)     3324 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/DSSP/DSSP.py
--rw-r--r--   0 patrick    (501) staff       (20)     3606 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/DSSP/DSSPExe.py
--rw-r--r--   0 patrick    (501) staff       (20)       54 2023-07-19 22:57:32.000000 SBILib-0.3.2/src/SBILib/external/DSSP/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      338 2023-07-19 22:57:27.000000 SBILib-0.3.2/src/SBILib/external/README.md
--rw-r--r--   0 patrick    (501) staff       (20)       62 2023-07-19 22:57:28.000000 SBILib-0.3.2/src/SBILib/external/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.638485 SBILib-0.3.2/src/SBILib/external/blast/
--rw-r--r--   0 patrick    (501) staff       (20)     9107 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/blast/BlastExe.py
--rw-r--r--   0 patrick    (501) staff       (20)    12570 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/blast/BlastHit.py
--rw-r--r--   0 patrick    (501) staff       (20)    23488 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/blast/BlastResult.py
--rw-r--r--   0 patrick    (501) staff       (20)       83 2023-07-19 22:57:19.000000 SBILib-0.3.2/src/SBILib/external/blast/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     8072 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/external/blast/blast_parser.py
--rw-r--r--   0 patrick    (501) staff       (20)      312 2023-07-19 22:57:34.000000 SBILib-0.3.2/src/SBILib/external/configSBI.txt
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.642582 SBILib-0.3.2/src/SBILib/math/
--rw-r--r--   0 patrick    (501) staff       (20)       19 2023-07-19 22:57:36.000000 SBILib-0.3.2/src/SBILib/math/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-07-19 22:57:35.000000 SBILib-0.3.2/src/SBILib/math/stats.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.653894 SBILib-0.3.2/src/SBILib/sequence/
--rw-r--r--   0 patrick    (501) staff       (20)     6331 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/sequence/Fasta.py
--rw-r--r--   0 patrick    (501) staff       (20)     4871 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/sequence/IndexedSeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)    15045 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/sequence/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-07-19 22:57:13.000000 SBILib-0.3.2/src/SBILib/sequence/Sequence.py
--rw-r--r--   0 patrick    (501) staff       (20)      140 2023-07-19 22:57:10.000000 SBILib-0.3.2/src/SBILib/sequence/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.663100 SBILib-0.3.2/src/SBILib/sequence/alignment/
--rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-07-19 22:57:04.000000 SBILib-0.3.2/src/SBILib/sequence/alignment/Needleman_Wunsch.py
--rw-r--r--   0 patrick    (501) staff       (20)    43526 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/sequence/alignment/SeqAli.py
--rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-07-19 22:57:04.000000 SBILib-0.3.2/src/SBILib/sequence/alignment/SimilarityMatrix.py
--rw-r--r--   0 patrick    (501) staff       (20)       93 2023-07-19 22:57:05.000000 SBILib-0.3.2/src/SBILib/sequence/alignment/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.673499 SBILib-0.3.2/src/SBILib/structure/
--rw-r--r--   0 patrick    (501) staff       (20)    25560 2023-07-20 15:29:21.000000 SBILib-0.3.2/src/SBILib/structure/PDB.py
--rw-r--r--   0 patrick    (501) staff       (20)      460 2023-07-19 22:54:58.000000 SBILib-0.3.2/src/SBILib/structure/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.686040 SBILib-0.3.2/src/SBILib/structure/atom/
--rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-07-19 22:55:41.000000 SBILib-0.3.2/src/SBILib/structure/atom/Atom.py
--rw-r--r--   0 patrick    (501) staff       (20)      659 2023-07-19 22:55:42.000000 SBILib-0.3.2/src/SBILib/structure/atom/AtomOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)      803 2023-07-19 22:55:35.000000 SBILib-0.3.2/src/SBILib/structure/atom/AtomOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     3758 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/atom/AtomSeries.py
--rw-r--r--   0 patrick    (501) staff       (20)      127 2023-07-19 22:55:40.000000 SBILib-0.3.2/src/SBILib/structure/atom/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.699052 SBILib-0.3.2/src/SBILib/structure/chain/
--rw-r--r--   0 patrick    (501) staff       (20)    19964 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/chain/Chain.py
--rw-r--r--   0 patrick    (501) staff       (20)    13264 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/chain/ChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)     2763 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/chain/ChainOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)     6877 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/chain/ChainOfProtein.py
--rw-r--r--   0 patrick    (501) staff       (20)     4988 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/chain/ProteinChainFrame.py
--rw-r--r--   0 patrick    (501) staff       (20)      131 2023-07-19 22:54:38.000000 SBILib-0.3.2/src/SBILib/structure/chain/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.707094 SBILib-0.3.2/src/SBILib/structure/contacts/
--rw-r--r--   0 patrick    (501) staff       (20)     9010 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/Complex.py
--rw-r--r--   0 patrick    (501) staff       (20)     3408 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/InnerContacts.py
--rw-r--r--   0 patrick    (501) staff       (20)      277 2023-07-19 22:55:14.000000 SBILib-0.3.2/src/SBILib/structure/contacts/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.719137 SBILib-0.3.2/src/SBILib/structure/contacts/contact/
--rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-07-19 22:55:19.000000 SBILib-0.3.2/src/SBILib/structure/contacts/contact/Contact.py
--rw-r--r--   0 patrick    (501) staff       (20)     3806 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAA.py
--rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-07-19 22:55:19.000000 SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAH.py
--rw-r--r--   0 patrick    (501) staff       (20)     3275 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAN.py
--rw-r--r--   0 patrick    (501) staff       (20)      149 2023-07-19 22:55:18.000000 SBILib-0.3.2/src/SBILib/structure/contacts/contact/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.724194 SBILib-0.3.2/src/SBILib/structure/contacts/inner/
--rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-07-19 22:55:25.000000 SBILib-0.3.2/src/SBILib/structure/contacts/inner/PHInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-07-19 22:55:24.000000 SBILib-0.3.2/src/SBILib/structure/contacts/inner/PPInnerContact.py
--rw-r--r--   0 patrick    (501) staff       (20)       85 2023-07-19 22:55:24.000000 SBILib-0.3.2/src/SBILib/structure/contacts/inner/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.734256 SBILib-0.3.2/src/SBILib/structure/contacts/interface/
--rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-07-19 22:55:11.000000 SBILib-0.3.2/src/SBILib/structure/contacts/interface/Interface.py
--rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-07-19 22:55:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/interface/PHInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    11115 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/interface/PNInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-07-19 22:55:11.000000 SBILib-0.3.2/src/SBILib/structure/contacts/interface/PPInterface.py
--rw-r--r--   0 patrick    (501) staff       (20)      157 2023-07-19 22:55:10.000000 SBILib-0.3.2/src/SBILib/structure/contacts/interface/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.738805 SBILib-0.3.2/src/SBILib/structure/geometry/
--rw-r--r--   0 patrick    (501) staff       (20)    11737 2023-07-19 22:54:32.000000 SBILib-0.3.2/src/SBILib/structure/geometry/RMSD.py
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 22:54:33.000000 SBILib-0.3.2/src/SBILib/structure/geometry/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      662 2023-07-19 22:54:32.000000 SBILib-0.3.2/src/SBILib/structure/geometry/basics.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.762081 SBILib-0.3.2/src/SBILib/structure/header/
--rw-r--r--   0 patrick    (501) staff       (20)     2282 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/BioMolecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     3827 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/DBreference.py
--rw-r--r--   0 patrick    (501) staff       (20)     2011 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/Experiment.py
--rw-r--r--   0 patrick    (501) staff       (20)    14754 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/Header.py
--rw-r--r--   0 patrick    (501) staff       (20)     1199 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/HeteroAtom.py
--rw-r--r--   0 patrick    (501) staff       (20)      944 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/MiniRes.py
--rw-r--r--   0 patrick    (501) staff       (20)     7645 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/Molecule.py
--rw-r--r--   0 patrick    (501) staff       (20)     8530 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     2421 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/Site.py
--rw-r--r--   0 patrick    (501) staff       (20)    18693 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/header/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)    14368 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/parse_mmCIF.py
--rw-r--r--   0 patrick    (501) staff       (20)     8541 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/parse_pdb.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.775417 SBILib-0.3.2/src/SBILib/structure/protein/
--rw-r--r--   0 patrick    (501) staff       (20)    19068 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/protein/Arch.py
--rw-r--r--   0 patrick    (501) staff       (20)    19200 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/protein/SShelper.py
--rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-07-19 22:55:29.000000 SBILib-0.3.2/src/SBILib/structure/protein/SecondaryStructure.py
--rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-07-19 22:55:34.000000 SBILib-0.3.2/src/SBILib/structure/protein/Sequencer.py
--rw-r--r--   0 patrick    (501) staff       (20)      134 2023-07-19 22:55:34.000000 SBILib-0.3.2/src/SBILib/structure/protein/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.784215 SBILib-0.3.2/src/SBILib/structure/residue/
--rw-r--r--   0 patrick    (501) staff       (20)    10771 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/residue/Residue.py
--rw-r--r--   0 patrick    (501) staff       (20)    10721 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/residue/ResidueOfAminoAcid.py
--rw-r--r--   0 patrick    (501) staff       (20)     5357 2023-07-20 15:23:10.000000 SBILib-0.3.2/src/SBILib/structure/residue/ResidueOfNucleotide.py
--rw-r--r--   0 patrick    (501) staff       (20)      146 2023-07-19 22:55:02.000000 SBILib-0.3.2/src/SBILib/structure/residue/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.806880 SBILib-0.3.2/src/SBILib/tests/
--rw-r--r--   0 patrick    (501) staff       (20)      426 2023-07-20 15:27:20.000000 SBILib-0.3.2/src/SBILib/tests/Test.py
--rw-r--r--   0 patrick    (501) staff       (20)   156217 2023-07-19 23:01:16.000000 SBILib-0.3.2/src/SBILib/tests/Test_1a3q.cif.gz
--rw-r--r--   0 patrick    (501) staff       (20)    47362 2023-07-19 23:01:16.000000 SBILib-0.3.2/src/SBILib/tests/Test_pdb1a2w.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:17.000000 SBILib-0.3.2/src/SBILib/tests/Test_pdb1a3q.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)   116164 2023-07-19 23:01:18.000000 SBILib-0.3.2/src/SBILib/tests/Test_pdb2ram.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 23:01:17.000000 SBILib-0.3.2/src/SBILib/tests/__ini__.py
--rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:21.000000 SBILib-0.3.2/src/SBILib/tests/pdb1a3q.ent.gz
--rw-r--r--   0 patrick    (501) staff       (20)     9923 2023-07-21 16:09:58.000000 SBILib-0.3.2/src/SBILib/tests/test_modules.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-21 16:14:42.515944 SBILib-0.3.2/src/SBILib.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)    25858 2023-07-21 16:14:42.000000 SBILib-0.3.2/src/SBILib.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     5049 2023-07-21 16:14:42.000000 SBILib-0.3.2/src/SBILib.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-07-21 16:14:42.000000 SBILib-0.3.2/src/SBILib.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)       39 2023-07-21 16:14:42.000000 SBILib-0.3.2/src/SBILib.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        7 2023-07-21 16:14:42.000000 SBILib-0.3.2/src/SBILib.egg-info/top_level.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.841251 SBILib-0.3.3/
+-rw-r--r--   0 patrick    (501) staff       (20)      128 2023-07-21 15:34:16.000000 SBILib-0.3.3/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)    37821 2023-07-22 21:19:59.844503 SBILib-0.3.3/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)    37560 2023-07-22 18:00:53.000000 SBILib-0.3.3/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)     6077 2023-07-21 20:09:42.000000 SBILib-0.3.3/Scenarios.md
+-rw-r--r--   0 patrick    (501) staff       (20)      103 2023-07-22 21:19:59.846314 SBILib-0.3.3/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)      621 2023-07-22 21:19:29.000000 SBILib-0.3.3/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.463632 SBILib-0.3.3/src/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.485565 SBILib-0.3.3/src/SBILib/
+-rw-r--r--   0 patrick    (501) staff       (20)    12951 2023-07-22 21:19:07.000000 SBILib-0.3.3/src/SBILib/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.517659 SBILib-0.3.3/src/SBILib/beans/
+-rw-r--r--   0 patrick    (501) staff       (20)     4500 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/beans/Executable.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11699 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/beans/File.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4779 2023-07-19 22:56:14.000000 SBILib-0.3.3/src/SBILib/beans/IndexedNum.py
+-rw-r--r--   0 patrick    (501) staff       (20)      349 2023-07-19 22:56:22.000000 SBILib-0.3.3/src/SBILib/beans/JSONer.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14930 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/beans/Path.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2926 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/beans/StorableObject.py
+-rw-r--r--   0 patrick    (501) staff       (20)      187 2023-07-19 22:56:21.000000 SBILib-0.3.3/src/SBILib/beans/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12746 2023-07-19 22:56:20.000000 SBILib-0.3.3/src/SBILib/beans/butler.py
+-rw-r--r--   0 patrick    (501) staff       (20)      516 2023-07-19 22:56:23.000000 SBILib-0.3.3/src/SBILib/beans/singleton.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.537324 SBILib-0.3.3/src/SBILib/data/
+-rw-r--r--   0 patrick    (501) staff       (20)     6426 2023-07-19 22:55:56.000000 SBILib-0.3.3/src/SBILib/data/Alphabet.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8845 2023-07-19 22:55:49.000000 SBILib-0.3.3/src/SBILib/data/AminoAcids.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4566 2023-07-19 22:55:54.000000 SBILib-0.3.3/src/SBILib/data/AtomVariants.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4411 2023-07-19 22:55:55.000000 SBILib-0.3.3/src/SBILib/data/Element.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3413 2023-07-19 22:55:55.000000 SBILib-0.3.3/src/SBILib/data/Properties.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2863 2023-07-19 22:55:57.000000 SBILib-0.3.3/src/SBILib/data/SetDict.py
+-rw-r--r--   0 patrick    (501) staff       (20)    29056 2023-07-19 22:55:53.000000 SBILib-0.3.3/src/SBILib/data/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.579454 SBILib-0.3.3/src/SBILib/databases/
+-rw-r--r--   0 patrick    (501) staff       (20)      273 2023-07-19 22:56:12.000000 SBILib-0.3.3/src/SBILib/databases/AlphaFoldlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5290 2023-07-19 22:56:12.000000 SBILib-0.3.3/src/SBILib/databases/CATHlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8412 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/DrugBanklink.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13617 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/Enzymelink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5573 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/GOlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5355 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/PDBTMlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)      417 2023-07-19 22:56:01.000000 SBILib-0.3.3/src/SBILib/databases/PDBeChemConnect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6713 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/PDBeChemlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9123 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/PDBlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1795 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/SCOPlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5733 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/TaxIDlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7098 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7063 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/__Uniprotlink.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2772 2023-07-19 22:56:07.000000 SBILib-0.3.3/src/SBILib/databases/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7149 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/dblink.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.586188 SBILib-0.3.3/src/SBILib/databases/uniprot/
+-rw-r--r--   0 patrick    (501) staff       (20)       90 2023-07-19 22:56:09.000000 SBILib-0.3.3/src/SBILib/databases/uniprot/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4777 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/uniprot/connect.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8169 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/databases/uniprot/uniprot.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.596162 SBILib-0.3.3/src/SBILib/error/
+-rw-r--r--   0 patrick    (501) staff       (20)     3400 2023-07-19 22:55:48.000000 SBILib-0.3.3/src/SBILib/error/BlastError.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2000 2023-07-19 22:55:43.000000 SBILib-0.3.3/src/SBILib/error/FileError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      896 2023-07-19 22:55:48.000000 SBILib-0.3.3/src/SBILib/error/SeqAliError.py
+-rw-r--r--   0 patrick    (501) staff       (20)      108 2023-07-19 22:55:47.000000 SBILib-0.3.3/src/SBILib/error/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.602553 SBILib-0.3.3/src/SBILib/external/
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.615765 SBILib-0.3.3/src/SBILib/external/CDhit/
+-rw-r--r--   0 patrick    (501) staff       (20)      964 2023-07-19 22:57:25.000000 SBILib-0.3.3/src/SBILib/external/CDhit/CDhit.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2255 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/CDhit/CDhitExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)      802 2023-07-19 22:57:26.000000 SBILib-0.3.3/src/SBILib/external/CDhit/CDhitHomolog.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2223 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/CDhit/CDhitList.py
+-rw-r--r--   0 patrick    (501) staff       (20)       64 2023-07-19 22:57:25.000000 SBILib-0.3.3/src/SBILib/external/CDhit/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.625783 SBILib-0.3.3/src/SBILib/external/DSSP/
+-rw-r--r--   0 patrick    (501) staff       (20)     3324 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/DSSP/DSSP.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3606 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/DSSP/DSSPExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)       54 2023-07-19 22:57:32.000000 SBILib-0.3.3/src/SBILib/external/DSSP/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      338 2023-07-19 22:57:27.000000 SBILib-0.3.3/src/SBILib/external/README.md
+-rw-r--r--   0 patrick    (501) staff       (20)       62 2023-07-19 22:57:28.000000 SBILib-0.3.3/src/SBILib/external/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.638283 SBILib-0.3.3/src/SBILib/external/blast/
+-rw-r--r--   0 patrick    (501) staff       (20)     9107 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/blast/BlastExe.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12570 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/blast/BlastHit.py
+-rw-r--r--   0 patrick    (501) staff       (20)    23488 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/blast/BlastResult.py
+-rw-r--r--   0 patrick    (501) staff       (20)       83 2023-07-19 22:57:19.000000 SBILib-0.3.3/src/SBILib/external/blast/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8072 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/external/blast/blast_parser.py
+-rw-r--r--   0 patrick    (501) staff       (20)      312 2023-07-19 22:57:34.000000 SBILib-0.3.3/src/SBILib/external/configSBI.txt
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.642786 SBILib-0.3.3/src/SBILib/math/
+-rw-r--r--   0 patrick    (501) staff       (20)       19 2023-07-19 22:57:36.000000 SBILib-0.3.3/src/SBILib/math/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1003 2023-07-19 22:57:35.000000 SBILib-0.3.3/src/SBILib/math/stats.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.660878 SBILib-0.3.3/src/SBILib/sequence/
+-rw-r--r--   0 patrick    (501) staff       (20)     6331 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/sequence/Fasta.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4871 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/sequence/IndexedSeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)    15045 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/sequence/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3930 2023-07-19 22:57:13.000000 SBILib-0.3.3/src/SBILib/sequence/Sequence.py
+-rw-r--r--   0 patrick    (501) staff       (20)      140 2023-07-19 22:57:10.000000 SBILib-0.3.3/src/SBILib/sequence/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.669878 SBILib-0.3.3/src/SBILib/sequence/alignment/
+-rw-r--r--   0 patrick    (501) staff       (20)     3338 2023-07-19 22:57:04.000000 SBILib-0.3.3/src/SBILib/sequence/alignment/Needleman_Wunsch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    43526 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/sequence/alignment/SeqAli.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1129 2023-07-19 22:57:04.000000 SBILib-0.3.3/src/SBILib/sequence/alignment/SimilarityMatrix.py
+-rw-r--r--   0 patrick    (501) staff       (20)       93 2023-07-19 22:57:05.000000 SBILib-0.3.3/src/SBILib/sequence/alignment/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.681214 SBILib-0.3.3/src/SBILib/structure/
+-rw-r--r--   0 patrick    (501) staff       (20)    25560 2023-07-20 15:29:21.000000 SBILib-0.3.3/src/SBILib/structure/PDB.py
+-rw-r--r--   0 patrick    (501) staff       (20)      460 2023-07-19 22:54:58.000000 SBILib-0.3.3/src/SBILib/structure/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.691647 SBILib-0.3.3/src/SBILib/structure/atom/
+-rw-r--r--   0 patrick    (501) staff       (20)     4446 2023-07-19 22:55:41.000000 SBILib-0.3.3/src/SBILib/structure/atom/Atom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      659 2023-07-19 22:55:42.000000 SBILib-0.3.3/src/SBILib/structure/atom/AtomOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)      803 2023-07-19 22:55:35.000000 SBILib-0.3.3/src/SBILib/structure/atom/AtomOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3758 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/atom/AtomSeries.py
+-rw-r--r--   0 patrick    (501) staff       (20)      127 2023-07-19 22:55:40.000000 SBILib-0.3.3/src/SBILib/structure/atom/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.707819 SBILib-0.3.3/src/SBILib/structure/chain/
+-rw-r--r--   0 patrick    (501) staff       (20)    19964 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/chain/Chain.py
+-rw-r--r--   0 patrick    (501) staff       (20)    13264 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/chain/ChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2763 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/chain/ChainOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6877 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/chain/ChainOfProtein.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4988 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/chain/ProteinChainFrame.py
+-rw-r--r--   0 patrick    (501) staff       (20)      131 2023-07-19 22:54:38.000000 SBILib-0.3.3/src/SBILib/structure/chain/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.714779 SBILib-0.3.3/src/SBILib/structure/contacts/
+-rw-r--r--   0 patrick    (501) staff       (20)     9010 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/Complex.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3408 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/InnerContacts.py
+-rw-r--r--   0 patrick    (501) staff       (20)      277 2023-07-19 22:55:14.000000 SBILib-0.3.3/src/SBILib/structure/contacts/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.724895 SBILib-0.3.3/src/SBILib/structure/contacts/contact/
+-rw-r--r--   0 patrick    (501) staff       (20)     4649 2023-07-19 22:55:19.000000 SBILib-0.3.3/src/SBILib/structure/contacts/contact/Contact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3806 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAA.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2525 2023-07-19 22:55:19.000000 SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAH.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3275 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAN.py
+-rw-r--r--   0 patrick    (501) staff       (20)      149 2023-07-19 22:55:18.000000 SBILib-0.3.3/src/SBILib/structure/contacts/contact/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.731119 SBILib-0.3.3/src/SBILib/structure/contacts/inner/
+-rw-r--r--   0 patrick    (501) staff       (20)     2912 2023-07-19 22:55:25.000000 SBILib-0.3.3/src/SBILib/structure/contacts/inner/PHInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2905 2023-07-19 22:55:24.000000 SBILib-0.3.3/src/SBILib/structure/contacts/inner/PPInnerContact.py
+-rw-r--r--   0 patrick    (501) staff       (20)       85 2023-07-19 22:55:24.000000 SBILib-0.3.3/src/SBILib/structure/contacts/inner/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.744814 SBILib-0.3.3/src/SBILib/structure/contacts/interface/
+-rw-r--r--   0 patrick    (501) staff       (20)     4328 2023-07-19 22:55:11.000000 SBILib-0.3.3/src/SBILib/structure/contacts/interface/Interface.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3298 2023-07-19 22:55:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/interface/PHInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    11115 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/interface/PNInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)    12530 2023-07-19 22:55:11.000000 SBILib-0.3.3/src/SBILib/structure/contacts/interface/PPInterface.py
+-rw-r--r--   0 patrick    (501) staff       (20)      157 2023-07-19 22:55:10.000000 SBILib-0.3.3/src/SBILib/structure/contacts/interface/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.749065 SBILib-0.3.3/src/SBILib/structure/geometry/
+-rw-r--r--   0 patrick    (501) staff       (20)    11737 2023-07-19 22:54:32.000000 SBILib-0.3.3/src/SBILib/structure/geometry/RMSD.py
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 22:54:33.000000 SBILib-0.3.3/src/SBILib/structure/geometry/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)      662 2023-07-19 22:54:32.000000 SBILib-0.3.3/src/SBILib/structure/geometry/basics.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.777015 SBILib-0.3.3/src/SBILib/structure/header/
+-rw-r--r--   0 patrick    (501) staff       (20)     2282 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/BioMolecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     3827 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/DBreference.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2011 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/Experiment.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14754 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/Header.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1199 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/HeteroAtom.py
+-rw-r--r--   0 patrick    (501) staff       (20)      944 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/MiniRes.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7645 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/Molecule.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8530 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2421 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/Site.py
+-rw-r--r--   0 patrick    (501) staff       (20)    18693 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/header/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)    14368 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/parse_mmCIF.py
+-rw-r--r--   0 patrick    (501) staff       (20)     8541 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/parse_pdb.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.792350 SBILib-0.3.3/src/SBILib/structure/protein/
+-rw-r--r--   0 patrick    (501) staff       (20)    19068 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/protein/Arch.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19200 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/protein/SShelper.py
+-rw-r--r--   0 patrick    (501) staff       (20)     9282 2023-07-19 22:55:29.000000 SBILib-0.3.3/src/SBILib/structure/protein/SecondaryStructure.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1691 2023-07-19 22:55:34.000000 SBILib-0.3.3/src/SBILib/structure/protein/Sequencer.py
+-rw-r--r--   0 patrick    (501) staff       (20)      134 2023-07-19 22:55:34.000000 SBILib-0.3.3/src/SBILib/structure/protein/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.802850 SBILib-0.3.3/src/SBILib/structure/residue/
+-rw-r--r--   0 patrick    (501) staff       (20)    10771 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/residue/Residue.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10721 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/residue/ResidueOfAminoAcid.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5357 2023-07-20 15:23:10.000000 SBILib-0.3.3/src/SBILib/structure/residue/ResidueOfNucleotide.py
+-rw-r--r--   0 patrick    (501) staff       (20)      146 2023-07-19 22:55:02.000000 SBILib-0.3.3/src/SBILib/structure/residue/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.836240 SBILib-0.3.3/src/SBILib/tests/
+-rw-r--r--   0 patrick    (501) staff       (20)      426 2023-07-20 15:27:20.000000 SBILib-0.3.3/src/SBILib/tests/Test.py
+-rw-r--r--   0 patrick    (501) staff       (20)   156217 2023-07-19 23:01:16.000000 SBILib-0.3.3/src/SBILib/tests/Test_1a3q.cif.gz
+-rw-r--r--   0 patrick    (501) staff       (20)    47362 2023-07-19 23:01:16.000000 SBILib-0.3.3/src/SBILib/tests/Test_pdb1a2w.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:17.000000 SBILib-0.3.3/src/SBILib/tests/Test_pdb1a3q.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)   116164 2023-07-19 23:01:18.000000 SBILib-0.3.3/src/SBILib/tests/Test_pdb2ram.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-07-19 23:01:17.000000 SBILib-0.3.3/src/SBILib/tests/__ini__.py
+-rw-r--r--   0 patrick    (501) staff       (20)   125951 2023-07-19 23:01:21.000000 SBILib-0.3.3/src/SBILib/tests/pdb1a3q.ent.gz
+-rw-r--r--   0 patrick    (501) staff       (20)     9923 2023-07-21 16:09:58.000000 SBILib-0.3.3/src/SBILib/tests/test_modules.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-07-22 21:19:59.492574 SBILib-0.3.3/src/SBILib.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)    37821 2023-07-22 21:19:59.000000 SBILib-0.3.3/src/SBILib.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     5049 2023-07-22 21:19:59.000000 SBILib-0.3.3/src/SBILib.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-07-22 21:19:59.000000 SBILib-0.3.3/src/SBILib.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       39 2023-07-22 21:19:59.000000 SBILib-0.3.3/src/SBILib.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        7 2023-07-22 21:19:59.000000 SBILib-0.3.3/src/SBILib.egg-info/top_level.txt
```

### Comparing `SBILib-0.3.2/PKG-INFO` & `SBILib-0.3.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,63 @@
-Metadata-Version: 2.1
-Name: SBILib
-Version: 0.3.2
-Home-page: https://github.com/structuralbioinformatics/SBI
-Author: Patrick Gohl
-Author-email: patrick.gohl@upf.edu
-License: MIT
-Keywords: Structural Bioinformatics,Loops
-Description-Content-Type: text/markdown
-
 # Welcome to the StructuralBioInformatics pylib
 
 The **SBILib** python library is a continuous work in progress that clusters functionalities to work with data derived from [PDB][1], from creating a local PDB repository to do _real_ Blast searches over PDB sequences (i.e. sequences of the really crystallized protein sections) to perform a simply split chains (separate the sections of a PDB file).
 
 
+## Requirements:
+
+The library **is not exempt of bugs** (probably), and can not be considered a final version. This means that one must use it at its own risk. And, while new functionalities are bound to appear, others might disappear at any given moment. Any comments, complains or bug reports can be addressed in the corresponding sections.
+
+[1]: http://www.pdb.org/
+
+
+# SBILib Library Manual 
+
+This manual contains a short turorial split into 6 common Tasks.<br/>
+Information on how to access more detailed help pages within python is provided at the end.<br/>
+We have made available a list of slightly more complex scenarios on which the SBILib library may be applied. In Scenarios.md (https://github.com/structuralbioinformatics/SBI)
+
+### Dependencies
+python3 <br/>
+scipy <br/>
+numpy <br/>
+DSSP <br/>
+BLAST <br/>
+CD-Hit <br/>
+
+
 ## Installation:
-SBILib has been distributed on PyPi and can be installed with pip. However due to size limits we werent able to provide the BLAST database file through PyPi. This file, which will be needed for running BLAST and passing the unit tests, is available on our github repository. The full pip installation is outlined below. Alternatively you can define your own Blast database file as outlined in the BLAST section of this tutorial. 
+SBILib has been distributed on PyPi and can be installed with pip. <br/>
 
 ```console
 pip install SBILib
-
-
 ```
 
+This command will install the package locally.<br/>
 
 
-
-It can also be directly cloned from our github repo:
+It can also be directly cloned from our github repo:<br/>
 
 ```console
 git clone https://github.com/structuralbioinformatics/SBI
 ```
 
-Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBI and copy the folder manually.
+Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBI and copy the folder manually.<br/>
 
 
 ## Testing:
-We have implemented unit testing. After installation these scripts can be run to ensure that the package is functioning as it should
-These scripts are located in the directory "tests". REMEMBER the BLAST database file must be installed if installation occured with pip
+We have implemented unit testing. After installation these scripts can be run to ensure that the package is functioning as it should.
+These scripts are located in the directory "tests". Due to size limits we werent able to provide the database file needed for BLAST through PyPi. This file, will be automatically downloaded from https://www.ebi.ac.uk/uniprot/download-center once the unit tests are conducted. Later users may define their own Blast database file as outlined in the BLAST section of this tutorial. IMPORTANT before running ensure that external dependencies are properly configured as per TASK 2.2. 
 ```console
+pip show SBILib | grep Location
+
+# Location: /location/of/SBILib/locally
+
+cd /location/of/SBILib/locally/SBILib/tests
+
 python Test.py
 
 #........('TEST_PDB1A3Q_A.66.pdb', 'TEST_PDB1A3Q_A.66.dssp')
 #truncated chain!TEST_PDB1A3Q_A.66.dssp
 #.('TEST_PDB2RAM_A.38.pdb', 'TEST_PDB2RAM_A.38.dssp')
 #('TEST_PDB2RAM_B.26.pdb', 'TEST_PDB2RAM_B.26.dssp')
 #('TEST_PDB1A3Q_A.30.pdb', 'TEST_PDB1A3Q_A.30.dssp')
@@ -52,61 +68,21 @@
 #----------------------------------------------------------------------
 #Ran 11 tests in 67.249s
 #
 #OK
 ```
 
 
-## Requirements:
-
-
-You can start to play by reading a PDB using the following command:
-
-```python
-from SBILib.structure import PDB
-newPDBobject = PDB('pdbfilename')
-```
-
-The library **is not exempt of bugs** (probably), and can not be considered a final version. This means that one must use it at its own risk. And, while new functionalities are bound to appear, others might disappear at any given moment. Any comments, complains or bug reports can be addressed in the corresponding sections.
-
-[1]: http://www.pdb.org/
-
-
-
-
-# SBILib Library Manual 
-
-This manual contains a short turorial split into 5 common Tasks.
-Information on how to access more detailed help pages within python is provided at the end.
-We have made available a list of slightly more complex scenarios on which the SBILib library may be applied. In Scenarios.md
-
-### Dependencies
-python3 <br/>
-scipy <br/>
-numpy <br/>
-DSSP <br/>
-BLAST <br/>
-CD-Hit <br/>
-
-
-## Installation
-
-Download the SBILib library <br/>
-Navigate to SBILib/external/configSBI.txt <br/>
-Alter the path variable for each external dependency to point to the location the executable is stored in on you system. <br/>
-Once done the SBILib library is ready to use either interactivly or through a script. <br/>
-
-
 ## TASK 1
 
 ### 1) loading in the appropriate modules
 
 The following code demonstrates how a PDB file can be loaded: <br/>
 
-The first step is to load in the modules necessary. <br/>
+The first step is to load in the necessary modules. <br/>
 PDB link will allow us to grab a protein from the protein data bank. While the PDB module will allow us to do some basic tasks on the protein. <br/>
 ```{python}
 
 from SBILib.databases import PDBlink
 from SBILib.structure import PDB
 
 ```
@@ -120,29 +96,119 @@
 ```{python}
 
 new = PDBlink()
 path = new.get_PDB("1a3q")
 protein1 = PDB(path)
 
 ```
+
+Additionally predicted PDBs can also be fetched from the AlphaFold2 model database.
+
+```{python}
+
+from SBILib.databases import AlphaFoldlink
+
+alphaPath = AlphaFoldlink.download_pdb("P31946")
+
+AlphModel = PDB(alphaPath)
+
+```
+
 ### 3) Reading out chains in a protein
 
 First I will load in a second protein this time providing the address directly, and then have a look at the chains contained within the protein. <br/>
 We can look at exacty what chains are contained within the protein. <br/>
 Here our protein contains 2 chains identified as A and B <br/>
 
 ```{python}
 
 protein2 = PDB(path/to/pdbfile.pdb)
 protein2.chain_identifiers
 # set(['A', 'B'])
 
 ```
 
-### 4) Duplicating protein and fusing chains
+### 4) Selecting other elements of PDB 
+
+Now that we have seen how to select Chains of a protein we can also select the amino acids.<br/>
+We will renumerate the atoms and residues so that they start at 1.<br/>
+```{python}
+
+ChainA = protein.get_chain_by_id("A")
+
+ChainA.renumerate_residues(1)
+ChainA.renumerate_atoms(1)
+
+ChainA.aminoacids
+
+```
+
+This list all of the amino acids in the Chain and its atoms.<br/>
+The selection can be more specific by selecting one amino acid from the list.<br/>
+We can access the number (the position of the amino acid on the chain)<br/>
+The type of amino acid (three letter code and single letter).<br/>
+The coordinates of the O, C, CA and CB (if present)<br/>
+The coordinates of the backbone atoms.<br/>
+
+
+```{python}
+
+ChainA.aminoacids[0].number
+#1
+ChainA.aminoacids[0].type
+#'GLY'
+ChainA.aminoacids[0].single_letter
+#G
+ChainA.aminoacids[0].n 
+#<AtomOfAminoAcid: [N, 1]:(-5.833, 72.589, 45.643)>
+ChainA.aminoacids[0].o 
+#<AtomOfAminoAcid: [O, 4]:(-5.436, 72.093, 42.983)>
+ChainA.aminoacids[0].c
+#<AtomOfAminoAcid: [C, 3]:(-5.850, 73.226, 43.203)>
+ChainA.aminoacids[0].ca
+#<AtomOfAminoAcid: [CA, 2]:(-5.902, 73.707, 44.647)>
+ChainA.aminoacids[0].cb
+#
+ChainA.aminoacids[0].backbone_atoms
+#[<AtomOfAminoAcid: [N, 1]:(-5.833, 72.589, 45.643)>, <AtomOfAminoAcid: [CA, 2]:(-5.902, 73.707, 44.647)>, <AtomOfAminoAcid: [C, 3]:(-5.850, 73.226, 43.203)>]
+
+
+
+```
+There are other features such as secondary structure and accessibility information which is only available once the dssp of the chain has been calculated (see Task 2).<br/>
+
+Alternatively we can also accesss the atoms of the amino acid by their index.<br/>
+We see that the first amino acid has 4 atoms<br/>
+We see the name and number of the atom<br/>
+We can then access the x,y,and z coordinate of the atom<br/>
+We can also see the occupancy <br/>
+
+```{python}
+
+len( ChainA.aminoacids[0].atoms)
+#4
+ChainA.aminoacids[0].atoms[0].name
+#N
+ChainA.aminoacids[0].atoms[0].number
+#1
+ChainA.aminoacids[0].atoms[0].x
+#-5.833
+ChainA.aminoacids[0].atoms[0].y
+#72.589
+ChainA.aminoacids[0].atoms[0].z
+#45.643
+
+
+```
+
+
+
+
+
+### 5) Duplicating protein and fusing chains
 
 We can duplicate the protein as a new object with the duplicate command. <br/>
 Then if we want to we could fuse chains "A" and "B" into a new chain "A" <br/>
 Note that you will not be able to fuse two different kinds of structural chains. <br/>
 
 ```{python}
 
@@ -150,15 +216,15 @@
 protein3 = protein3.fuse_chains(["A","B"])
 protein3.chain_identifiers
 # set(["A"])
 
 ```
 
 
-### 5) Adding a chain to a protein
+### 6) Adding a chain to a protein
 
 Now let us imagine a scenario where we wanted to take chain A from protein2 and add it to protein1. <br/>
 First we have to pull out the chain that we want (A) from protein2. <br/>
 Then by checking the chain Identifiers in protein1 we can see that it already has a chain "A". <br/>
 This means that we will have to change the identifier of the chain we wish to add. Lets make it "E". <br/>
 First we will have to duplicate the chain, creating a new object (ChainE), so that we dont alter the chain Ids of protein2. <br/>
 Now we can add the chain to protein1 <br/>
@@ -174,15 +240,15 @@
 ChainE.chain = "E"
 protein1.add_chain(ChainE)
 protein1.chain_identifiers
 # set(['A', 'C', 'B', 'D', 'E'])
 
 ```
 
-### 6) Removing chain(s) from a protein
+### 7) Removing chain(s) from a protein
 
 Now we would like to delete this chain again: <br/>
 First we set up a temporary empty PDB object and call it protein3. <br/>
 Then we will define a list of the chain identifiers we wish to remove (in this case only "E") <br/>
 First we loop through all of the chains ids in protein1. <br/>
 If that protein is not in the deletion list we provided... <br/>
 We add it to the newly created protein3. <br/>
@@ -200,15 +266,15 @@
              elif (protein1.get_chain_by_id(chain).chaintype == "N"):
              	protein3._has_nucl = "TRUE"
 
 protein1 = protein3
 
 ```
 
-### 7) Adding multiple chains to a protein
+### 8) Adding multiple chains to a protein
 
 Addition of multiple chains can also be accomplished. <br/>
 First we have to grab the second chain from protein2 and change its id like we did to ChainA. <br/>
 Then we change the identifiers of both chains as we have done previously <br/>
 Then we create a list of the chains that we wish to add <br/>
 We then add this list of chains to protein1 <br/>
 
@@ -222,15 +288,15 @@
 protein1.chain_identifiers
 # set(['A','B','C','D','E','F'])
 
 ```
 
 You can revert back to the original protein by repeating step 6 and adding "F" to the deletion list. <br/>
 
-### 8) Reading out protein sequence (gapped and exact)
+### 9) Reading out protein sequence (gapped and exact)
 
 We can now have a look at the protein sequence <br/>
 First we can have a look at the exact sequence of the protein without gaps indicated (not containing gaps of non-crystalized positions).  <br/>
 Then we look at the gapped version (default). Xs will be placed where the crystal sequence contains gaps. <br/>
 We can also read out the sequence of each chain individually as a gapped sequence (as shown with ChainA) <br/>
 We can also read out the non gapped sequence of each chain as shown <br/>
 
@@ -244,33 +310,32 @@
 ChainA.gapped_protein_sequence
 # "gapped protein sequence for Chain A only"
 ChainA.protein_sequence
 # "The exact sequence in the crysal without non crystalized positions indicated"
 
 ```
 
-### 9) Getting DNA sequence
+### 10) Getting DNA sequence
 
 In addition to protein sequences the PDB may contain DNA <br/>
 We can check if this is the case for protein1 <br/>
 In the case where this is true we can read out the sequences in Fasta format <br/>
 
 
 ```{python}
 protein1.has_nucleotide
 # True
 for chain in protein1.nucleotides:
 	print(">" + chain.globalID + "\n" + chain.nucleotide_sequence())
 # >"globalID"
 # "Nucleotide Sequence"
-...
 
 ``` 
 
-### 10) Cleaning protein and writing PDBfile
+### 11) Cleaning protein and writing PDBfile
 
 We can clean the protein with the following command <br/>
 We can then write the PDB of the protein out to a file name that we provide <br/>
 
 ```{python}
 
 protein1.clean()
@@ -321,38 +386,55 @@
 protein = PDB("pdb1a3q.ent.gz")
 ChainA = protein.get_chain_by_id("A")
 ChainA.calculate_dssp()
 ChainA.gapped_protein_secondary_structure
 # "gapped secondary structure"
 
 ```
+
+The secondary structure annotation follows the DSSP classification:<br/>
+
+G = 3-turn helix (310 helix). Min length 3 residues.<br/>
+H = 4-turn helix (α helix). Minimum length 4 residues.<br/>
+I = 5-turn helix (π helix). Minimum length 5 residues.<br/>
+T = hydrogen bonded turn (3, 4 or 5 turn)<br/>
+E = extended strand in parallel and/or anti-parallel β-sheet conformation. Min length 2 residues.<br/>
+B = residue in isolated β-bridge (single pair β-sheet hydrogen bond formation)<br/>
+S = bend (the only non-hydrogen-bond based assignment).<br/>
+C = coil (residues which are not in any of the above conformations).<br/>
+
+
+
 ### 4) printing out the entire proteins amino acid sequence and secondary structure
 
 ```{python}
 
 for chain in protein.proteins:
 	chain.calculate_dssp()
 	print(">" + chain.globalID + "\n" + chain.gapped_protein_sequence + "\n" + chain.gapped_protein_secondary_structure)
 
 # >"globalID"
 # "gapped amino acid sequence"
 # "gapped secondary structure"
 
 
 ```
+This Gives us an overview of the protein. We see the Amino Acid sequence and the DSSP predicted Secondary structure all together.
+
 
 ## TASK 3
 
 ### 1) Set up a blast  
 
 
 In order to blast you must have a database <br/>
 This is a multifasta file containing protein or DNA sequences depending on the blast type. <br/>
 Reformating of the multifasta file will be done automatically once it is provided. <br/>
 The blast object will now know that the blast is to be conducted on this database. <br/>
+If the unittest was run after installation a database file will be located in the tests folder (see Testing section)<br/>
 
 ```{python}
 
 from SBILib.external.blast import BlastExe
 blast = BlastExe(database = "path/to/database/file.fa")
 
 ```
@@ -384,17 +466,35 @@
 blastresults.print_compacted_blast()
 # query and target info, e-value, coverage etc. 
 
 for hit in blastresults.get_hits():
 	print(hit.sequenceID, " ", hit.e_value)
 # list of all hits and their associated e-values.
 
-
 ```
 
+The compacted blast output is divided into the following collumns:<br/>
+Query ID, Query length, Target ID, Accession length, Identities, Positives, Gaps, e_value , Query sequence, Target sequence, Format Positions<br/>
+The varying outputs here have the following meaning:<br/>
+
+Query ID = ID of provided sequence<br/>
+Query length = length of provided sequence<br/>
+Target ID = id of the hit sequence<br/>
+Accession length = length of the hit sequence<br/>
+Identities = number of identical amino acids between the query and target<br/>
+Positives = The number of amino acids that are either identical between the query and the subject sequence or have similar chemical properties<br/>
+Gaps = number of gaps in the alignment<br/>
+e_value = the expected number of hits expected to be seen by chance given the size of the blast database.<br/>
+Query sequence = provided sequence<br/>
+Target sequence = hit sequence<br/>
+Format Positions = a single string in which fragment definitions will be represented as follows: <br/>
+Query segment 1 start : Hit segment 1start, Query segment 1 end : Hit segment 1 end,Query segment 2 start : Hit segment 2 start, Query segment 2 end : Hit segment 2 end  etc.<br/>
+
+
+
 ### 4) Filter results
 If we want to evaluate whether the proteins fall within the Rost Curve twilight zone, <br/>
 we can parse through the list and print it off similarly to how it was done above. <br/>
 If we want to only consider hits passing the rost evaluation we can pass that as an argument to the "get_hits" command <br/>
 
 
 
@@ -407,14 +507,15 @@
 for hit in blastresults.get_hits(tz_type = "ID"):
 	print(hit.sequenceID, " ", hit.evaluate_Rost_twilight_zone())
 # only hits that pass the test will be shown
 
 
 ```
 
+
 ### 4) PIR 
 
 PIR formatted alignments are available for every hit. <br/>
 We can select hit number 13 with the result parameter <br/>
 We could add in the filters to grab the PIR of alll of the best results <br/>
 
 ```{python}
@@ -423,35 +524,151 @@
 # PIR alignment
 for hit in  blastresults.get_hits( evalue = 0, tz_type = "ID"):
 	blastresults.str_PIR(result = hit._num_seq)
 # All PIRs with hits that match the criteria given 
 
 ```
 
+### 5) Find Results with matching secondary structure
+
+The secondary structure of a protein plays a vital role in its function.<br/>
+The SBILib package allows for the quick viewing of how secondary structure is represented in an alignment.<br/>
+Are vital secondary structure element located in a gap resulting in a homolog with unequal function?<br/>
+Here we demonstrate how this can be analyzed.<br/>
+
+```{python}
+
+blastresults.str_PIR(result = 13)
+
+
+#>P1;1A3Q_A
+#sequence:1A3Q_A:2:.:285:.:.:.:.:.
+#PYLVIVEQPKQRGFRFRYGCEGPSHGGLPGASSEKGRKTYPTVKICNYEGPAKIEVDLVT
+#HSDPPRAHAHSLVGKQCSELGICAVSVGPKDMTAQFNNLGVLHVTKKNMMGTMIQKLQRQ
+#RLRSRPQGLTEAEQRELEQEAKELKKVMDLSIVRLRFSAFL------RSLPLKPVISQPI
+#HDSKSPGASNLKISRMDKTAGSVRGGDEVYLLCDKVQKDDIEVRFYEDDENGWQAFGDFS
+#PTDVHKQYAIVFRTPPYHKMKIERPVTVFLQLKRKRGGDVSDSKQFTYYP*
+#>P1;REL
+#structureX:REL:16:AVIRE:289:AVIRE:.:.:.:.
+#PYIEIFEQPRQRGTRFRYKCEGRSAGSIPGEHSTDNNKTFPSIQILNYFGKVKIRTTLVT
+#KNEPYKPHPHDLVGKGCRD-GYYEAEFGPERQVLSFQNLGIQCVKKKDLKESISLRISK-
+#--KINPFNVPEEQLHNIDE--------YDLNVVRLCFQAFLPDEHGNYTLALPPLISNPI
+#YDNRAPNTAELRICRVNKNCGSVKGGDEIFLLCDKVQKDDIEVRFVLGN---WEAKGSFS
+#QADVHRQVAIVFRTPPFLG-DITEPITVKMQLRRPSDQAVSEPVDFRYLP*
+
+
+```
+This wil output a PIR format alignment of the two proteins. Dashes in the target protein (second sequence of the PIR) indicate gaps in the alignment. We are interestsed in seeing what secondary structure elements (if any) may have gone missing as a result of these gaps.  
+```{python}
+
+string = blastresults.str_PIR(result = 13)
+indices = [i for i, c in enumerate("".join(string.split(">")[2].split("\n")[2:]))if c == "-"]
+i = 0    
+string= ""
+for char in ChainA.gapped_protein_secondary_structure:
+	if i in indices:
+		string = string + char
+	else:
+		string = string + "-"
+	i+=1
+
+
+lines = textwrap.wrap(string,60)
+print("\n".join(lines))
+
+#------------------------------------------------------------
+#-------------------T---------------------------------------
+#HHH-----------------HHHHHHHT--------------------------------
+#--------------------------------------------------SSS-------
+#----------------------------------------------------
+
+```
+
+Here we can see what secondary structures go missing as a result of the alignment.<br/>
+To remind ourselves of the query proteins secondary structure lets look at it again:
+
+```{python}
+lines = textwrap.wrap(ChainA.gapped_protein_secondary_structure, 60)
+print("\n".join(lines))
+
+
+#--EEEEEE-B-SSSB--EETTT-S-S----BS---TT-----EEEEET--
+#SSEEEEEEEE-SSSS--B-SSEEEETTB-TTS-EEEEE-SS--EEE---EEEEE--
+#TTTHHHHHHHHHHHHHTTTS-S---HHHHHHHHHHHHHHHTT--TTEEEEEEEEEE-
+#xxxxxx-EE---EE---EEBTTSTTTS---EEEES-SEEETT---EEEEEESS--
+#TTTEEEEEEE-SSS-EEEE-B--GGGEETTTEEEEE----S-TT-SS-EEEEEEEEETTT
+#--B---EEEEEE-
+
+
+
+```
+We can see that for this Homolog according to our alignment half of a 4-turn helix is missing in our target protein.<br/> 
+Should this element be of functional significance we would have to continue our search for a more suitable homolog.<br/> 
+
 
 ## Task 4
 
 ### 1) Complex
 For this exercise we will use the protein DNA complex that we used in the previous tasks. <br/>
 In order to extract the interfaces from a protein complex we will first have to create an object of the complex class. <br/> 
 In createing a new complex class we need to provide the protein complex. <br/>
-Optional arguments are PPI,PNI,PHI threshold distances (in Angstrom). At default these are 12, 8 and 6 respectively. <br/>
 We can grab the individual chains of the complex straight from this class using the .pdb method if we wanted. <br/>
 
 ```{python}
 
 from SBILib.structure import Complex
 from SBILib.structure import PDB
 protein = PDB("pdb1a3q.ent.gz")
 complex = Complex(protein)
 complex.pdb
 # PDB object
 
 
 ```
+Here we have used the default definitions for contacts within the complex which are as follows.
+
+```{python}
+Complex(pdb, biomolecule=False, PPI=True, PPI_type='cb', PPI_distance=12, PNI=True, PNI_type='min', PNI_distance=8, PHI=True, PHI_type='min', PHI_distance=6)
+```
+Protein Protein interaction:<br/>
+	type: beta carbons<br/>
+	distance: 12 Angstrom<br/>
+	
+Protein Nucleotide interaction:<br/>
+	type: minimum<br/>
+	distance: 8 Angstrom<br/>
+
+Protein Heteroatom interaction:<br/>
+	type: minimum<br/>
+	distance: 6 Angstrom<br/>
+
+
+However these can be altered:
+```{python}
+
+complex = Complex(protein, PPI_type='ca', PPI_distance=14)
+
+```
+
+The available contact types are:<br/>
+Protein Protein interaction:<br/>
+	minimum (the distance between the closest pairs of atoms of each residue)<br/>
+	alpha carbons (distance between the alpha carbons of the two residues)<br/>
+	beta carbons (distance between the beta carbons of the two residues)<br/>
+	geometric (distance between the geometric centers of the two residues)<br/>
+	backbone (distance between the center of the backbone atoms between the two residues)<br/>
+Protein Nucleotide interaction:<br/>
+	minimum<br/>
+	geometric<br/>
+	backbone<br/>
+Protein Heteroatom interaction:<br/>
+	minimum<br/>
+	geometric<br/>
+
+
 
 ### 2) PPI
 The interfaces are already calculated and present within the Complex object. <br/>
 The results of the Protein Protein Interfaces are stored in a list and accessible with the PPInterfaces method <br/>
 We can count the number of interfaces produced by looking at the length of the list (here just 1) <br/>
 To access the interfaces we can simply index the list <br/>
 The results can quickly be summarized by converting to a string. <br/>
@@ -476,14 +693,16 @@
 	print(contact.aminoacid1.identifier, contact.aminoacid1.single_letter, contact.aminoacid1.ca.coordinates)
 	print(contact.aminoacid2.identifier, contact.aminoacid2.single_letter, contact.aminoacid2.ca.coordinates)
 	print(contact.geometric_distance)
 # complete list of the contacts, coordinates and distances in this interface
 
 ```
 
+
+
 ### 2) PNI
 
 We can calculate Protein Nucleotide interfaces as well. <br/>
 The interfaces are accessible with the PNInterfaces method. <br/> 
 When we take a look at the interface list we see that this time we have multiple results. <br/>
 These can be accessed by indexing or iterated through. <br/>
 We can then gather the position and identifiers for the amino acid and nucleotides. As well as the alpha carbon coordinate in the case of the amino acid and the phosphate coordinate in the case of the nucleotide. <br/>
@@ -577,18 +796,105 @@
 In the SBILib library loops are refered to as archs. <br/>
 
 ```{python}
 
 ChainA.calculate_dssp()
 ChainA.calculate_archs()
 ChainA.archs
+
+#[**Secondary Structure Relation:
+#STR1:	( E )  39  <--  6 -->  44 
+#	f11:  43  cmf11:              [-3.84483333 62.7425     28.42483333] eigf11:              [ 0.34916202 -0.59272239 -0.72578651]
+#STR2:	( E )  54  <--  2 -->  55 
+#	f44:  55  cmf44:              [ 7.85366667 71.586       7.988     ] eigf44:              [ 0.04348626  0.87377397 -0.48438414]
+#ARCH TYPE: BK
+#INTERNAL SS: 0
+#DISTANCE: 22.978424484459143
+#THETA: 98.69428 RHO: 74.28570 DELTA: 58.26752
+#**
+
+
+
+```
+The output of the archs command is a list of the loop geometries calculated for the given chain (ChainA)<br/>
+We get the first secondary structure that flanks the loop. In parantheses the structure type (see Task2.3) it's start, length and end.<br/>
+An axis for flanking secondary structures 1 defined based on the shortest of the principal moments of inertia for that structures. <br/>
+The same information is printed out for the second flanking structure.<br/>
+The arch Type is printed:<br/>
+BK: beta-link<br/>
+BN: beta-hairpin<br/>
+EG: beta-helix310<br/>
+EH: beta-alpha helix<br/>
+GE: helix310-beta<br/>
+GG: helix310-helix310<br/>
+GH: helix310-alpha helix<br/>
+HE: alpha helix-beta<br/>
+HG: alpha helix-helix310<br/>
+HH: alpha helix-alpha helix<br/>
+
+INTERNAL SS = the number of secondary structures contained in the loop.<br/>
+Distance = The euclidean distance between the beginning and end of the loop.<br/>
+Theta: the angle between the axes of secondary structure 1 and 2.<br/>
+Delta: the angle between the axis of secondary structure 1 and the vector of distance between beginning and end of loop.<br/>
+Rho: the angle between the secondary structure 2 axis and the plane that contains the axis of secondary structure 1.<br/>
+
+
+To get larger loops which may contain secondary structures:
+
+```{python}
+
 ChainA.superarchs
 
 ```
 
+The output follows the same format as the previous.
+
+
+
+## Task 6
+
+### Loop Grafting
+
+We will show how SBILib may be used to graft the loop of one protein into the structure of another protein with similiar loop geometry. 
+
+```{python}
+
+new = PDBlink()
+path = new.get_PDB("2ram")
+protein2 = PDB(path)
+report = protein.compare_loops(self.protein2)
+report[0]
+
+# 'QueryProt:A,176,182:TargetProt:A,160,166:VISQPIH,VLSHPIF'
+
+```
+These Commands took the protein previously defined (1a3q here QueryProt) and for each loop within that protein searched for loops in the TargetProt (2ram) with matching geometries. These pairs are saved in a list (here defined by the variable report). Each element (loop matches) of that list is composed of a string with the format seen above. QueryProt:A refers to the first loop (from the query protein) being located on chain A. 176,182 the start and end positions of that loop respectively. TargetProt:A the second loop is found on chain A of the target protein. 160,166 our start and end positions. VISQPIH,VLSHPIF are the sequences for the Query protein and Target protein loops respectively. 
+We define loop geometries to be similar if all of the following conditions are met:<br/>
+
+```{python}
+Rho = math.sqrt((loop1.rho - loop2.rho)**2) <= 10 
+Delta = math.sqrt((loop1.delta - loop2.delta)**2) <= 5
+Theta = math.sqrt((loop1.theta - loop2.theta)**2) <= 5
+Distance = math.sqrt((loop1.cartesian_distance - loop2.cartesian_distance)**2) <= 0.5 
+
+```
+That is to say if the difference between each type of angle and distance is less than the thresholds of (10 Rho angle, 5 Delta angle, 5 Theta angle, 0.5 Cartesian distance)<br/>
+
+
+
+Now we tell the protein to graft the target protein loop into the query protein using the first match found in the previous output list. Note that if the loops are of unequal length this will not work. 
+```{python}
+
+graft = self.protein.graft(self.protein2, report[0])
+
+```
+
+
+
+
 ## Details on classes
 If you wish to check the functions available for any class, they are available with pytons dir method. <br/>
 first create an instance of the class you wish to inspect. <br/>
 then call the dir method on that instance. What follows is a list of all of the functions of the PDB class <br/>
 to get more detailed information call the help methdod. <br/>
 
 ```{python}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `SBILib-0.3.2/Scenarios.md` & `SBILib-0.3.3/Scenarios.md`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/setup.py` & `SBILib-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md') as f:
     readme = f.read()
 
 
 setup(
     name='SBILib',
-    version='0.3.2',
+    version='0.3.3',
     license='MIT',
     author="Patrick Gohl",
     author_email='patrick.gohl@upf.edu',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     include_package_data=True,
     long_description=readme,
```

### Comparing `SBILib-0.3.2/src/SBILib/__init__.py` & `SBILib-0.3.3/src/SBILib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 import os
 import traceback
 import datetime
 import time
 import logging
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 
 
 class Parameters(object):
     '''
     Designed to work through all the {SBI} library.
     It contains several parameters that will control (a) the amount of data
     shown to the user during the execution of {SBI} subroutines and (b) the
```

### Comparing `SBILib-0.3.2/src/SBILib/beans/Executable.py` & `SBILib-0.3.3/src/SBILib/beans/Executable.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/beans/File.py` & `SBILib-0.3.3/src/SBILib/beans/File.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/beans/IndexedNum.py` & `SBILib-0.3.3/src/SBILib/beans/IndexedNum.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/beans/Path.py` & `SBILib-0.3.3/src/SBILib/beans/Path.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/beans/StorableObject.py` & `SBILib-0.3.3/src/SBILib/beans/StorableObject.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/beans/butler.py` & `SBILib-0.3.3/src/SBILib/beans/butler.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/beans/singleton.py` & `SBILib-0.3.3/src/SBILib/beans/singleton.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/data/Alphabet.py` & `SBILib-0.3.3/src/SBILib/data/Alphabet.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/data/AminoAcids.py` & `SBILib-0.3.3/src/SBILib/data/AminoAcids.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/data/AtomVariants.py` & `SBILib-0.3.3/src/SBILib/data/AtomVariants.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/data/Element.py` & `SBILib-0.3.3/src/SBILib/data/Element.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/data/Properties.py` & `SBILib-0.3.3/src/SBILib/data/Properties.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/data/SetDict.py` & `SBILib-0.3.3/src/SBILib/data/SetDict.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/data/__init__.py` & `SBILib-0.3.3/src/SBILib/data/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/CATHlink.py` & `SBILib-0.3.3/src/SBILib/databases/CATHlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/DrugBanklink.py` & `SBILib-0.3.3/src/SBILib/databases/DrugBanklink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/Enzymelink.py` & `SBILib-0.3.3/src/SBILib/databases/Enzymelink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/GOlink.py` & `SBILib-0.3.3/src/SBILib/databases/GOlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/PDBTMlink.py` & `SBILib-0.3.3/src/SBILib/databases/PDBTMlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/PDBeChemlink.py` & `SBILib-0.3.3/src/SBILib/databases/PDBeChemlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/PDBlink.py` & `SBILib-0.3.3/src/SBILib/databases/PDBlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/SCOPlink.py` & `SBILib-0.3.3/src/SBILib/databases/SCOPlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/TaxIDlink.py` & `SBILib-0.3.3/src/SBILib/databases/TaxIDlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/Uniprotlink.py` & `SBILib-0.3.3/src/SBILib/databases/Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/__Uniprotlink.py` & `SBILib-0.3.3/src/SBILib/databases/__Uniprotlink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/__init__.py` & `SBILib-0.3.3/src/SBILib/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/dblink.py` & `SBILib-0.3.3/src/SBILib/databases/dblink.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/uniprot/connect.py` & `SBILib-0.3.3/src/SBILib/databases/uniprot/connect.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/databases/uniprot/uniprot.py` & `SBILib-0.3.3/src/SBILib/databases/uniprot/uniprot.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/error/BlastError.py` & `SBILib-0.3.3/src/SBILib/error/BlastError.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/error/FileError.py` & `SBILib-0.3.3/src/SBILib/error/FileError.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/error/SeqAliError.py` & `SBILib-0.3.3/src/SBILib/error/SeqAliError.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/external/CDhit/CDhit.py` & `SBILib-0.3.3/src/SBILib/external/CDhit/CDhit.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/external/CDhit/CDhitExe.py` & `SBILib-0.3.3/src/SBILib/external/CDhit/CDhitExe.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/external/CDhit/CDhitHomolog.py` & `SBILib-0.3.3/src/SBILib/external/CDhit/CDhitHomolog.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/external/CDhit/CDhitList.py` & `SBILib-0.3.3/src/SBILib/external/CDhit/CDhitList.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/external/DSSP/DSSP.py` & `SBILib-0.3.3/src/SBILib/external/DSSP/DSSP.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/external/DSSP/DSSPExe.py` & `SBILib-0.3.3/src/SBILib/external/DSSP/DSSPExe.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/external/blast/BlastExe.py` & `SBILib-0.3.3/src/SBILib/external/blast/BlastExe.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/external/blast/BlastHit.py` & `SBILib-0.3.3/src/SBILib/external/blast/BlastHit.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/external/blast/BlastResult.py` & `SBILib-0.3.3/src/SBILib/external/blast/BlastResult.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/external/blast/blast_parser.py` & `SBILib-0.3.3/src/SBILib/external/blast/blast_parser.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/math/stats.py` & `SBILib-0.3.3/src/SBILib/math/stats.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/sequence/Fasta.py` & `SBILib-0.3.3/src/SBILib/sequence/Fasta.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/sequence/IndexedSeqAli.py` & `SBILib-0.3.3/src/SBILib/sequence/IndexedSeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/sequence/SeqAli.py` & `SBILib-0.3.3/src/SBILib/sequence/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/sequence/Sequence.py` & `SBILib-0.3.3/src/SBILib/sequence/Sequence.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/sequence/alignment/Needleman_Wunsch.py` & `SBILib-0.3.3/src/SBILib/sequence/alignment/Needleman_Wunsch.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/sequence/alignment/SeqAli.py` & `SBILib-0.3.3/src/SBILib/sequence/alignment/SeqAli.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/sequence/alignment/SimilarityMatrix.py` & `SBILib-0.3.3/src/SBILib/sequence/alignment/SimilarityMatrix.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/PDB.py` & `SBILib-0.3.3/src/SBILib/structure/PDB.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/atom/Atom.py` & `SBILib-0.3.3/src/SBILib/structure/atom/Atom.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/atom/AtomOfAminoAcid.py` & `SBILib-0.3.3/src/SBILib/structure/atom/AtomOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/atom/AtomOfNucleotide.py` & `SBILib-0.3.3/src/SBILib/structure/atom/AtomOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/atom/AtomSeries.py` & `SBILib-0.3.3/src/SBILib/structure/atom/AtomSeries.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/chain/Chain.py` & `SBILib-0.3.3/src/SBILib/structure/chain/Chain.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/chain/ChainFrame.py` & `SBILib-0.3.3/src/SBILib/structure/chain/ChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/chain/ChainOfNucleotide.py` & `SBILib-0.3.3/src/SBILib/structure/chain/ChainOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/chain/ChainOfProtein.py` & `SBILib-0.3.3/src/SBILib/structure/chain/ChainOfProtein.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/chain/ProteinChainFrame.py` & `SBILib-0.3.3/src/SBILib/structure/chain/ProteinChainFrame.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/Complex.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/Complex.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/InnerContacts.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/InnerContacts.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/contact/Contact.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/contact/Contact.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAA.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAA.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAH.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAH.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/contact/ContactAN.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/contact/ContactAN.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/inner/PHInnerContact.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/inner/PHInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/inner/PPInnerContact.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/inner/PPInnerContact.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/interface/Interface.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/interface/Interface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/interface/PHInterface.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/interface/PHInterface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/interface/PNInterface.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/interface/PNInterface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/contacts/interface/PPInterface.py` & `SBILib-0.3.3/src/SBILib/structure/contacts/interface/PPInterface.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/geometry/RMSD.py` & `SBILib-0.3.3/src/SBILib/structure/geometry/RMSD.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/geometry/basics.py` & `SBILib-0.3.3/src/SBILib/structure/geometry/basics.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/header/BioMolecule.py` & `SBILib-0.3.3/src/SBILib/structure/header/BioMolecule.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/header/DBreference.py` & `SBILib-0.3.3/src/SBILib/structure/header/DBreference.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/header/Experiment.py` & `SBILib-0.3.3/src/SBILib/structure/header/Experiment.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/header/Header.py` & `SBILib-0.3.3/src/SBILib/structure/header/Header.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/header/HeteroAtom.py` & `SBILib-0.3.3/src/SBILib/structure/header/HeteroAtom.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/header/MiniRes.py` & `SBILib-0.3.3/src/SBILib/structure/header/MiniRes.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/header/Molecule.py` & `SBILib-0.3.3/src/SBILib/structure/header/Molecule.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/header/SecondaryStructure.py` & `SBILib-0.3.3/src/SBILib/structure/header/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/header/Site.py` & `SBILib-0.3.3/src/SBILib/structure/header/Site.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/header/__init__.py` & `SBILib-0.3.3/src/SBILib/structure/header/__init__.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/parse_mmCIF.py` & `SBILib-0.3.3/src/SBILib/structure/parse_mmCIF.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/parse_pdb.py` & `SBILib-0.3.3/src/SBILib/structure/parse_pdb.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/protein/Arch.py` & `SBILib-0.3.3/src/SBILib/structure/protein/Arch.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/protein/SShelper.py` & `SBILib-0.3.3/src/SBILib/structure/protein/SShelper.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/protein/SecondaryStructure.py` & `SBILib-0.3.3/src/SBILib/structure/protein/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/protein/Sequencer.py` & `SBILib-0.3.3/src/SBILib/structure/protein/Sequencer.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/residue/Residue.py` & `SBILib-0.3.3/src/SBILib/structure/residue/Residue.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/residue/ResidueOfAminoAcid.py` & `SBILib-0.3.3/src/SBILib/structure/residue/ResidueOfAminoAcid.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/structure/residue/ResidueOfNucleotide.py` & `SBILib-0.3.3/src/SBILib/structure/residue/ResidueOfNucleotide.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/tests/Test_1a3q.cif.gz` & `SBILib-0.3.3/src/SBILib/tests/Test_1a3q.cif.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/tests/Test_pdb1a2w.ent.gz` & `SBILib-0.3.3/src/SBILib/tests/Test_pdb1a2w.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/tests/Test_pdb1a3q.ent.gz` & `SBILib-0.3.3/src/SBILib/tests/Test_pdb1a3q.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/tests/Test_pdb2ram.ent.gz` & `SBILib-0.3.3/src/SBILib/tests/Test_pdb2ram.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/tests/pdb1a3q.ent.gz` & `SBILib-0.3.3/src/SBILib/tests/pdb1a3q.ent.gz`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib/tests/test_modules.py` & `SBILib-0.3.3/src/SBILib/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `SBILib-0.3.2/src/SBILib.egg-info/PKG-INFO` & `SBILib-0.3.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,73 @@
 Metadata-Version: 2.1
 Name: SBILib
-Version: 0.3.2
+Version: 0.3.3
 Home-page: https://github.com/structuralbioinformatics/SBI
 Author: Patrick Gohl
 Author-email: patrick.gohl@upf.edu
 License: MIT
 Keywords: Structural Bioinformatics,Loops
 Description-Content-Type: text/markdown
 
 # Welcome to the StructuralBioInformatics pylib
 
 The **SBILib** python library is a continuous work in progress that clusters functionalities to work with data derived from [PDB][1], from creating a local PDB repository to do _real_ Blast searches over PDB sequences (i.e. sequences of the really crystallized protein sections) to perform a simply split chains (separate the sections of a PDB file).
 
 
+## Requirements:
+
+The library **is not exempt of bugs** (probably), and can not be considered a final version. This means that one must use it at its own risk. And, while new functionalities are bound to appear, others might disappear at any given moment. Any comments, complains or bug reports can be addressed in the corresponding sections.
+
+[1]: http://www.pdb.org/
+
+
+# SBILib Library Manual 
+
+This manual contains a short turorial split into 6 common Tasks.<br/>
+Information on how to access more detailed help pages within python is provided at the end.<br/>
+We have made available a list of slightly more complex scenarios on which the SBILib library may be applied. In Scenarios.md (https://github.com/structuralbioinformatics/SBI)
+
+### Dependencies
+python3 <br/>
+scipy <br/>
+numpy <br/>
+DSSP <br/>
+BLAST <br/>
+CD-Hit <br/>
+
+
 ## Installation:
-SBILib has been distributed on PyPi and can be installed with pip. However due to size limits we werent able to provide the BLAST database file through PyPi. This file, which will be needed for running BLAST and passing the unit tests, is available on our github repository. The full pip installation is outlined below. Alternatively you can define your own Blast database file as outlined in the BLAST section of this tutorial. 
+SBILib has been distributed on PyPi and can be installed with pip. <br/>
 
 ```console
 pip install SBILib
-
-
 ```
 
+This command will install the package locally.<br/>
 
 
-
-It can also be directly cloned from our github repo:
+It can also be directly cloned from our github repo:<br/>
 
 ```console
 git clone https://github.com/structuralbioinformatics/SBI
 ```
 
-Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBI and copy the folder manually.
+Alternatively it is also possible to navigate directly to the repository https://github.com/structuralbioinformatics/SBI and copy the folder manually.<br/>
 
 
 ## Testing:
-We have implemented unit testing. After installation these scripts can be run to ensure that the package is functioning as it should
-These scripts are located in the directory "tests". REMEMBER the BLAST database file must be installed if installation occured with pip
+We have implemented unit testing. After installation these scripts can be run to ensure that the package is functioning as it should.
+These scripts are located in the directory "tests". Due to size limits we werent able to provide the database file needed for BLAST through PyPi. This file, will be automatically downloaded from https://www.ebi.ac.uk/uniprot/download-center once the unit tests are conducted. Later users may define their own Blast database file as outlined in the BLAST section of this tutorial. IMPORTANT before running ensure that external dependencies are properly configured as per TASK 2.2. 
 ```console
+pip show SBILib | grep Location
+
+# Location: /location/of/SBILib/locally
+
+cd /location/of/SBILib/locally/SBILib/tests
+
 python Test.py
 
 #........('TEST_PDB1A3Q_A.66.pdb', 'TEST_PDB1A3Q_A.66.dssp')
 #truncated chain!TEST_PDB1A3Q_A.66.dssp
 #.('TEST_PDB2RAM_A.38.pdb', 'TEST_PDB2RAM_A.38.dssp')
 #('TEST_PDB2RAM_B.26.pdb', 'TEST_PDB2RAM_B.26.dssp')
 #('TEST_PDB1A3Q_A.30.pdb', 'TEST_PDB1A3Q_A.30.dssp')
@@ -52,61 +78,21 @@
 #----------------------------------------------------------------------
 #Ran 11 tests in 67.249s
 #
 #OK
 ```
 
 
-## Requirements:
-
-
-You can start to play by reading a PDB using the following command:
-
-```python
-from SBILib.structure import PDB
-newPDBobject = PDB('pdbfilename')
-```
-
-The library **is not exempt of bugs** (probably), and can not be considered a final version. This means that one must use it at its own risk. And, while new functionalities are bound to appear, others might disappear at any given moment. Any comments, complains or bug reports can be addressed in the corresponding sections.
-
-[1]: http://www.pdb.org/
-
-
-
-
-# SBILib Library Manual 
-
-This manual contains a short turorial split into 5 common Tasks.
-Information on how to access more detailed help pages within python is provided at the end.
-We have made available a list of slightly more complex scenarios on which the SBILib library may be applied. In Scenarios.md
-
-### Dependencies
-python3 <br/>
-scipy <br/>
-numpy <br/>
-DSSP <br/>
-BLAST <br/>
-CD-Hit <br/>
-
-
-## Installation
-
-Download the SBILib library <br/>
-Navigate to SBILib/external/configSBI.txt <br/>
-Alter the path variable for each external dependency to point to the location the executable is stored in on you system. <br/>
-Once done the SBILib library is ready to use either interactivly or through a script. <br/>
-
-
 ## TASK 1
 
 ### 1) loading in the appropriate modules
 
 The following code demonstrates how a PDB file can be loaded: <br/>
 
-The first step is to load in the modules necessary. <br/>
+The first step is to load in the necessary modules. <br/>
 PDB link will allow us to grab a protein from the protein data bank. While the PDB module will allow us to do some basic tasks on the protein. <br/>
 ```{python}
 
 from SBILib.databases import PDBlink
 from SBILib.structure import PDB
 
 ```
@@ -120,29 +106,119 @@
 ```{python}
 
 new = PDBlink()
 path = new.get_PDB("1a3q")
 protein1 = PDB(path)
 
 ```
+
+Additionally predicted PDBs can also be fetched from the AlphaFold2 model database.
+
+```{python}
+
+from SBILib.databases import AlphaFoldlink
+
+alphaPath = AlphaFoldlink.download_pdb("P31946")
+
+AlphModel = PDB(alphaPath)
+
+```
+
 ### 3) Reading out chains in a protein
 
 First I will load in a second protein this time providing the address directly, and then have a look at the chains contained within the protein. <br/>
 We can look at exacty what chains are contained within the protein. <br/>
 Here our protein contains 2 chains identified as A and B <br/>
 
 ```{python}
 
 protein2 = PDB(path/to/pdbfile.pdb)
 protein2.chain_identifiers
 # set(['A', 'B'])
 
 ```
 
-### 4) Duplicating protein and fusing chains
+### 4) Selecting other elements of PDB 
+
+Now that we have seen how to select Chains of a protein we can also select the amino acids.<br/>
+We will renumerate the atoms and residues so that they start at 1.<br/>
+```{python}
+
+ChainA = protein.get_chain_by_id("A")
+
+ChainA.renumerate_residues(1)
+ChainA.renumerate_atoms(1)
+
+ChainA.aminoacids
+
+```
+
+This list all of the amino acids in the Chain and its atoms.<br/>
+The selection can be more specific by selecting one amino acid from the list.<br/>
+We can access the number (the position of the amino acid on the chain)<br/>
+The type of amino acid (three letter code and single letter).<br/>
+The coordinates of the O, C, CA and CB (if present)<br/>
+The coordinates of the backbone atoms.<br/>
+
+
+```{python}
+
+ChainA.aminoacids[0].number
+#1
+ChainA.aminoacids[0].type
+#'GLY'
+ChainA.aminoacids[0].single_letter
+#G
+ChainA.aminoacids[0].n 
+#<AtomOfAminoAcid: [N, 1]:(-5.833, 72.589, 45.643)>
+ChainA.aminoacids[0].o 
+#<AtomOfAminoAcid: [O, 4]:(-5.436, 72.093, 42.983)>
+ChainA.aminoacids[0].c
+#<AtomOfAminoAcid: [C, 3]:(-5.850, 73.226, 43.203)>
+ChainA.aminoacids[0].ca
+#<AtomOfAminoAcid: [CA, 2]:(-5.902, 73.707, 44.647)>
+ChainA.aminoacids[0].cb
+#
+ChainA.aminoacids[0].backbone_atoms
+#[<AtomOfAminoAcid: [N, 1]:(-5.833, 72.589, 45.643)>, <AtomOfAminoAcid: [CA, 2]:(-5.902, 73.707, 44.647)>, <AtomOfAminoAcid: [C, 3]:(-5.850, 73.226, 43.203)>]
+
+
+
+```
+There are other features such as secondary structure and accessibility information which is only available once the dssp of the chain has been calculated (see Task 2).<br/>
+
+Alternatively we can also accesss the atoms of the amino acid by their index.<br/>
+We see that the first amino acid has 4 atoms<br/>
+We see the name and number of the atom<br/>
+We can then access the x,y,and z coordinate of the atom<br/>
+We can also see the occupancy <br/>
+
+```{python}
+
+len( ChainA.aminoacids[0].atoms)
+#4
+ChainA.aminoacids[0].atoms[0].name
+#N
+ChainA.aminoacids[0].atoms[0].number
+#1
+ChainA.aminoacids[0].atoms[0].x
+#-5.833
+ChainA.aminoacids[0].atoms[0].y
+#72.589
+ChainA.aminoacids[0].atoms[0].z
+#45.643
+
+
+```
+
+
+
+
+
+### 5) Duplicating protein and fusing chains
 
 We can duplicate the protein as a new object with the duplicate command. <br/>
 Then if we want to we could fuse chains "A" and "B" into a new chain "A" <br/>
 Note that you will not be able to fuse two different kinds of structural chains. <br/>
 
 ```{python}
 
@@ -150,15 +226,15 @@
 protein3 = protein3.fuse_chains(["A","B"])
 protein3.chain_identifiers
 # set(["A"])
 
 ```
 
 
-### 5) Adding a chain to a protein
+### 6) Adding a chain to a protein
 
 Now let us imagine a scenario where we wanted to take chain A from protein2 and add it to protein1. <br/>
 First we have to pull out the chain that we want (A) from protein2. <br/>
 Then by checking the chain Identifiers in protein1 we can see that it already has a chain "A". <br/>
 This means that we will have to change the identifier of the chain we wish to add. Lets make it "E". <br/>
 First we will have to duplicate the chain, creating a new object (ChainE), so that we dont alter the chain Ids of protein2. <br/>
 Now we can add the chain to protein1 <br/>
@@ -174,15 +250,15 @@
 ChainE.chain = "E"
 protein1.add_chain(ChainE)
 protein1.chain_identifiers
 # set(['A', 'C', 'B', 'D', 'E'])
 
 ```
 
-### 6) Removing chain(s) from a protein
+### 7) Removing chain(s) from a protein
 
 Now we would like to delete this chain again: <br/>
 First we set up a temporary empty PDB object and call it protein3. <br/>
 Then we will define a list of the chain identifiers we wish to remove (in this case only "E") <br/>
 First we loop through all of the chains ids in protein1. <br/>
 If that protein is not in the deletion list we provided... <br/>
 We add it to the newly created protein3. <br/>
@@ -200,15 +276,15 @@
              elif (protein1.get_chain_by_id(chain).chaintype == "N"):
              	protein3._has_nucl = "TRUE"
 
 protein1 = protein3
 
 ```
 
-### 7) Adding multiple chains to a protein
+### 8) Adding multiple chains to a protein
 
 Addition of multiple chains can also be accomplished. <br/>
 First we have to grab the second chain from protein2 and change its id like we did to ChainA. <br/>
 Then we change the identifiers of both chains as we have done previously <br/>
 Then we create a list of the chains that we wish to add <br/>
 We then add this list of chains to protein1 <br/>
 
@@ -222,15 +298,15 @@
 protein1.chain_identifiers
 # set(['A','B','C','D','E','F'])
 
 ```
 
 You can revert back to the original protein by repeating step 6 and adding "F" to the deletion list. <br/>
 
-### 8) Reading out protein sequence (gapped and exact)
+### 9) Reading out protein sequence (gapped and exact)
 
 We can now have a look at the protein sequence <br/>
 First we can have a look at the exact sequence of the protein without gaps indicated (not containing gaps of non-crystalized positions).  <br/>
 Then we look at the gapped version (default). Xs will be placed where the crystal sequence contains gaps. <br/>
 We can also read out the sequence of each chain individually as a gapped sequence (as shown with ChainA) <br/>
 We can also read out the non gapped sequence of each chain as shown <br/>
 
@@ -244,33 +320,32 @@
 ChainA.gapped_protein_sequence
 # "gapped protein sequence for Chain A only"
 ChainA.protein_sequence
 # "The exact sequence in the crysal without non crystalized positions indicated"
 
 ```
 
-### 9) Getting DNA sequence
+### 10) Getting DNA sequence
 
 In addition to protein sequences the PDB may contain DNA <br/>
 We can check if this is the case for protein1 <br/>
 In the case where this is true we can read out the sequences in Fasta format <br/>
 
 
 ```{python}
 protein1.has_nucleotide
 # True
 for chain in protein1.nucleotides:
 	print(">" + chain.globalID + "\n" + chain.nucleotide_sequence())
 # >"globalID"
 # "Nucleotide Sequence"
-...
 
 ``` 
 
-### 10) Cleaning protein and writing PDBfile
+### 11) Cleaning protein and writing PDBfile
 
 We can clean the protein with the following command <br/>
 We can then write the PDB of the protein out to a file name that we provide <br/>
 
 ```{python}
 
 protein1.clean()
@@ -321,38 +396,55 @@
 protein = PDB("pdb1a3q.ent.gz")
 ChainA = protein.get_chain_by_id("A")
 ChainA.calculate_dssp()
 ChainA.gapped_protein_secondary_structure
 # "gapped secondary structure"
 
 ```
+
+The secondary structure annotation follows the DSSP classification:<br/>
+
+G = 3-turn helix (310 helix). Min length 3 residues.<br/>
+H = 4-turn helix (α helix). Minimum length 4 residues.<br/>
+I = 5-turn helix (π helix). Minimum length 5 residues.<br/>
+T = hydrogen bonded turn (3, 4 or 5 turn)<br/>
+E = extended strand in parallel and/or anti-parallel β-sheet conformation. Min length 2 residues.<br/>
+B = residue in isolated β-bridge (single pair β-sheet hydrogen bond formation)<br/>
+S = bend (the only non-hydrogen-bond based assignment).<br/>
+C = coil (residues which are not in any of the above conformations).<br/>
+
+
+
 ### 4) printing out the entire proteins amino acid sequence and secondary structure
 
 ```{python}
 
 for chain in protein.proteins:
 	chain.calculate_dssp()
 	print(">" + chain.globalID + "\n" + chain.gapped_protein_sequence + "\n" + chain.gapped_protein_secondary_structure)
 
 # >"globalID"
 # "gapped amino acid sequence"
 # "gapped secondary structure"
 
 
 ```
+This Gives us an overview of the protein. We see the Amino Acid sequence and the DSSP predicted Secondary structure all together.
+
 
 ## TASK 3
 
 ### 1) Set up a blast  
 
 
 In order to blast you must have a database <br/>
 This is a multifasta file containing protein or DNA sequences depending on the blast type. <br/>
 Reformating of the multifasta file will be done automatically once it is provided. <br/>
 The blast object will now know that the blast is to be conducted on this database. <br/>
+If the unittest was run after installation a database file will be located in the tests folder (see Testing section)<br/>
 
 ```{python}
 
 from SBILib.external.blast import BlastExe
 blast = BlastExe(database = "path/to/database/file.fa")
 
 ```
@@ -384,17 +476,35 @@
 blastresults.print_compacted_blast()
 # query and target info, e-value, coverage etc. 
 
 for hit in blastresults.get_hits():
 	print(hit.sequenceID, " ", hit.e_value)
 # list of all hits and their associated e-values.
 
-
 ```
 
+The compacted blast output is divided into the following collumns:<br/>
+Query ID, Query length, Target ID, Accession length, Identities, Positives, Gaps, e_value , Query sequence, Target sequence, Format Positions<br/>
+The varying outputs here have the following meaning:<br/>
+
+Query ID = ID of provided sequence<br/>
+Query length = length of provided sequence<br/>
+Target ID = id of the hit sequence<br/>
+Accession length = length of the hit sequence<br/>
+Identities = number of identical amino acids between the query and target<br/>
+Positives = The number of amino acids that are either identical between the query and the subject sequence or have similar chemical properties<br/>
+Gaps = number of gaps in the alignment<br/>
+e_value = the expected number of hits expected to be seen by chance given the size of the blast database.<br/>
+Query sequence = provided sequence<br/>
+Target sequence = hit sequence<br/>
+Format Positions = a single string in which fragment definitions will be represented as follows: <br/>
+Query segment 1 start : Hit segment 1start, Query segment 1 end : Hit segment 1 end,Query segment 2 start : Hit segment 2 start, Query segment 2 end : Hit segment 2 end  etc.<br/>
+
+
+
 ### 4) Filter results
 If we want to evaluate whether the proteins fall within the Rost Curve twilight zone, <br/>
 we can parse through the list and print it off similarly to how it was done above. <br/>
 If we want to only consider hits passing the rost evaluation we can pass that as an argument to the "get_hits" command <br/>
 
 
 
@@ -407,14 +517,15 @@
 for hit in blastresults.get_hits(tz_type = "ID"):
 	print(hit.sequenceID, " ", hit.evaluate_Rost_twilight_zone())
 # only hits that pass the test will be shown
 
 
 ```
 
+
 ### 4) PIR 
 
 PIR formatted alignments are available for every hit. <br/>
 We can select hit number 13 with the result parameter <br/>
 We could add in the filters to grab the PIR of alll of the best results <br/>
 
 ```{python}
@@ -423,35 +534,151 @@
 # PIR alignment
 for hit in  blastresults.get_hits( evalue = 0, tz_type = "ID"):
 	blastresults.str_PIR(result = hit._num_seq)
 # All PIRs with hits that match the criteria given 
 
 ```
 
+### 5) Find Results with matching secondary structure
+
+The secondary structure of a protein plays a vital role in its function.<br/>
+The SBILib package allows for the quick viewing of how secondary structure is represented in an alignment.<br/>
+Are vital secondary structure element located in a gap resulting in a homolog with unequal function?<br/>
+Here we demonstrate how this can be analyzed.<br/>
+
+```{python}
+
+blastresults.str_PIR(result = 13)
+
+
+#>P1;1A3Q_A
+#sequence:1A3Q_A:2:.:285:.:.:.:.:.
+#PYLVIVEQPKQRGFRFRYGCEGPSHGGLPGASSEKGRKTYPTVKICNYEGPAKIEVDLVT
+#HSDPPRAHAHSLVGKQCSELGICAVSVGPKDMTAQFNNLGVLHVTKKNMMGTMIQKLQRQ
+#RLRSRPQGLTEAEQRELEQEAKELKKVMDLSIVRLRFSAFL------RSLPLKPVISQPI
+#HDSKSPGASNLKISRMDKTAGSVRGGDEVYLLCDKVQKDDIEVRFYEDDENGWQAFGDFS
+#PTDVHKQYAIVFRTPPYHKMKIERPVTVFLQLKRKRGGDVSDSKQFTYYP*
+#>P1;REL
+#structureX:REL:16:AVIRE:289:AVIRE:.:.:.:.
+#PYIEIFEQPRQRGTRFRYKCEGRSAGSIPGEHSTDNNKTFPSIQILNYFGKVKIRTTLVT
+#KNEPYKPHPHDLVGKGCRD-GYYEAEFGPERQVLSFQNLGIQCVKKKDLKESISLRISK-
+#--KINPFNVPEEQLHNIDE--------YDLNVVRLCFQAFLPDEHGNYTLALPPLISNPI
+#YDNRAPNTAELRICRVNKNCGSVKGGDEIFLLCDKVQKDDIEVRFVLGN---WEAKGSFS
+#QADVHRQVAIVFRTPPFLG-DITEPITVKMQLRRPSDQAVSEPVDFRYLP*
+
+
+```
+This wil output a PIR format alignment of the two proteins. Dashes in the target protein (second sequence of the PIR) indicate gaps in the alignment. We are interestsed in seeing what secondary structure elements (if any) may have gone missing as a result of these gaps.  
+```{python}
+
+string = blastresults.str_PIR(result = 13)
+indices = [i for i, c in enumerate("".join(string.split(">")[2].split("\n")[2:]))if c == "-"]
+i = 0    
+string= ""
+for char in ChainA.gapped_protein_secondary_structure:
+	if i in indices:
+		string = string + char
+	else:
+		string = string + "-"
+	i+=1
+
+
+lines = textwrap.wrap(string,60)
+print("\n".join(lines))
+
+#------------------------------------------------------------
+#-------------------T---------------------------------------
+#HHH-----------------HHHHHHHT--------------------------------
+#--------------------------------------------------SSS-------
+#----------------------------------------------------
+
+```
+
+Here we can see what secondary structures go missing as a result of the alignment.<br/>
+To remind ourselves of the query proteins secondary structure lets look at it again:
+
+```{python}
+lines = textwrap.wrap(ChainA.gapped_protein_secondary_structure, 60)
+print("\n".join(lines))
+
+
+#--EEEEEE-B-SSSB--EETTT-S-S----BS---TT-----EEEEET--
+#SSEEEEEEEE-SSSS--B-SSEEEETTB-TTS-EEEEE-SS--EEE---EEEEE--
+#TTTHHHHHHHHHHHHHTTTS-S---HHHHHHHHHHHHHHHTT--TTEEEEEEEEEE-
+#xxxxxx-EE---EE---EEBTTSTTTS---EEEES-SEEETT---EEEEEESS--
+#TTTEEEEEEE-SSS-EEEE-B--GGGEETTTEEEEE----S-TT-SS-EEEEEEEEETTT
+#--B---EEEEEE-
+
+
+
+```
+We can see that for this Homolog according to our alignment half of a 4-turn helix is missing in our target protein.<br/> 
+Should this element be of functional significance we would have to continue our search for a more suitable homolog.<br/> 
+
 
 ## Task 4
 
 ### 1) Complex
 For this exercise we will use the protein DNA complex that we used in the previous tasks. <br/>
 In order to extract the interfaces from a protein complex we will first have to create an object of the complex class. <br/> 
 In createing a new complex class we need to provide the protein complex. <br/>
-Optional arguments are PPI,PNI,PHI threshold distances (in Angstrom). At default these are 12, 8 and 6 respectively. <br/>
 We can grab the individual chains of the complex straight from this class using the .pdb method if we wanted. <br/>
 
 ```{python}
 
 from SBILib.structure import Complex
 from SBILib.structure import PDB
 protein = PDB("pdb1a3q.ent.gz")
 complex = Complex(protein)
 complex.pdb
 # PDB object
 
 
 ```
+Here we have used the default definitions for contacts within the complex which are as follows.
+
+```{python}
+Complex(pdb, biomolecule=False, PPI=True, PPI_type='cb', PPI_distance=12, PNI=True, PNI_type='min', PNI_distance=8, PHI=True, PHI_type='min', PHI_distance=6)
+```
+Protein Protein interaction:<br/>
+	type: beta carbons<br/>
+	distance: 12 Angstrom<br/>
+	
+Protein Nucleotide interaction:<br/>
+	type: minimum<br/>
+	distance: 8 Angstrom<br/>
+
+Protein Heteroatom interaction:<br/>
+	type: minimum<br/>
+	distance: 6 Angstrom<br/>
+
+
+However these can be altered:
+```{python}
+
+complex = Complex(protein, PPI_type='ca', PPI_distance=14)
+
+```
+
+The available contact types are:<br/>
+Protein Protein interaction:<br/>
+	minimum (the distance between the closest pairs of atoms of each residue)<br/>
+	alpha carbons (distance between the alpha carbons of the two residues)<br/>
+	beta carbons (distance between the beta carbons of the two residues)<br/>
+	geometric (distance between the geometric centers of the two residues)<br/>
+	backbone (distance between the center of the backbone atoms between the two residues)<br/>
+Protein Nucleotide interaction:<br/>
+	minimum<br/>
+	geometric<br/>
+	backbone<br/>
+Protein Heteroatom interaction:<br/>
+	minimum<br/>
+	geometric<br/>
+
+
 
 ### 2) PPI
 The interfaces are already calculated and present within the Complex object. <br/>
 The results of the Protein Protein Interfaces are stored in a list and accessible with the PPInterfaces method <br/>
 We can count the number of interfaces produced by looking at the length of the list (here just 1) <br/>
 To access the interfaces we can simply index the list <br/>
 The results can quickly be summarized by converting to a string. <br/>
@@ -476,14 +703,16 @@
 	print(contact.aminoacid1.identifier, contact.aminoacid1.single_letter, contact.aminoacid1.ca.coordinates)
 	print(contact.aminoacid2.identifier, contact.aminoacid2.single_letter, contact.aminoacid2.ca.coordinates)
 	print(contact.geometric_distance)
 # complete list of the contacts, coordinates and distances in this interface
 
 ```
 
+
+
 ### 2) PNI
 
 We can calculate Protein Nucleotide interfaces as well. <br/>
 The interfaces are accessible with the PNInterfaces method. <br/> 
 When we take a look at the interface list we see that this time we have multiple results. <br/>
 These can be accessed by indexing or iterated through. <br/>
 We can then gather the position and identifiers for the amino acid and nucleotides. As well as the alpha carbon coordinate in the case of the amino acid and the phosphate coordinate in the case of the nucleotide. <br/>
@@ -577,18 +806,105 @@
 In the SBILib library loops are refered to as archs. <br/>
 
 ```{python}
 
 ChainA.calculate_dssp()
 ChainA.calculate_archs()
 ChainA.archs
+
+#[**Secondary Structure Relation:
+#STR1:	( E )  39  <--  6 -->  44 
+#	f11:  43  cmf11:              [-3.84483333 62.7425     28.42483333] eigf11:              [ 0.34916202 -0.59272239 -0.72578651]
+#STR2:	( E )  54  <--  2 -->  55 
+#	f44:  55  cmf44:              [ 7.85366667 71.586       7.988     ] eigf44:              [ 0.04348626  0.87377397 -0.48438414]
+#ARCH TYPE: BK
+#INTERNAL SS: 0
+#DISTANCE: 22.978424484459143
+#THETA: 98.69428 RHO: 74.28570 DELTA: 58.26752
+#**
+
+
+
+```
+The output of the archs command is a list of the loop geometries calculated for the given chain (ChainA)<br/>
+We get the first secondary structure that flanks the loop. In parantheses the structure type (see Task2.3) it's start, length and end.<br/>
+An axis for flanking secondary structures 1 defined based on the shortest of the principal moments of inertia for that structures. <br/>
+The same information is printed out for the second flanking structure.<br/>
+The arch Type is printed:<br/>
+BK: beta-link<br/>
+BN: beta-hairpin<br/>
+EG: beta-helix310<br/>
+EH: beta-alpha helix<br/>
+GE: helix310-beta<br/>
+GG: helix310-helix310<br/>
+GH: helix310-alpha helix<br/>
+HE: alpha helix-beta<br/>
+HG: alpha helix-helix310<br/>
+HH: alpha helix-alpha helix<br/>
+
+INTERNAL SS = the number of secondary structures contained in the loop.<br/>
+Distance = The euclidean distance between the beginning and end of the loop.<br/>
+Theta: the angle between the axes of secondary structure 1 and 2.<br/>
+Delta: the angle between the axis of secondary structure 1 and the vector of distance between beginning and end of loop.<br/>
+Rho: the angle between the secondary structure 2 axis and the plane that contains the axis of secondary structure 1.<br/>
+
+
+To get larger loops which may contain secondary structures:
+
+```{python}
+
 ChainA.superarchs
 
 ```
 
+The output follows the same format as the previous.
+
+
+
+## Task 6
+
+### Loop Grafting
+
+We will show how SBILib may be used to graft the loop of one protein into the structure of another protein with similiar loop geometry. 
+
+```{python}
+
+new = PDBlink()
+path = new.get_PDB("2ram")
+protein2 = PDB(path)
+report = protein.compare_loops(self.protein2)
+report[0]
+
+# 'QueryProt:A,176,182:TargetProt:A,160,166:VISQPIH,VLSHPIF'
+
+```
+These Commands took the protein previously defined (1a3q here QueryProt) and for each loop within that protein searched for loops in the TargetProt (2ram) with matching geometries. These pairs are saved in a list (here defined by the variable report). Each element (loop matches) of that list is composed of a string with the format seen above. QueryProt:A refers to the first loop (from the query protein) being located on chain A. 176,182 the start and end positions of that loop respectively. TargetProt:A the second loop is found on chain A of the target protein. 160,166 our start and end positions. VISQPIH,VLSHPIF are the sequences for the Query protein and Target protein loops respectively. 
+We define loop geometries to be similar if all of the following conditions are met:<br/>
+
+```{python}
+Rho = math.sqrt((loop1.rho - loop2.rho)**2) <= 10 
+Delta = math.sqrt((loop1.delta - loop2.delta)**2) <= 5
+Theta = math.sqrt((loop1.theta - loop2.theta)**2) <= 5
+Distance = math.sqrt((loop1.cartesian_distance - loop2.cartesian_distance)**2) <= 0.5 
+
+```
+That is to say if the difference between each type of angle and distance is less than the thresholds of (10 Rho angle, 5 Delta angle, 5 Theta angle, 0.5 Cartesian distance)<br/>
+
+
+
+Now we tell the protein to graft the target protein loop into the query protein using the first match found in the previous output list. Note that if the loops are of unequal length this will not work. 
+```{python}
+
+graft = self.protein.graft(self.protein2, report[0])
+
+```
+
+
+
+
 ## Details on classes
 If you wish to check the functions available for any class, they are available with pytons dir method. <br/>
 first create an instance of the class you wish to inspect. <br/>
 then call the dir method on that instance. What follows is a list of all of the functions of the PDB class <br/>
 to get more detailed information call the help methdod. <br/>
 
 ```{python}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `SBILib-0.3.2/src/SBILib.egg-info/SOURCES.txt` & `SBILib-0.3.3/src/SBILib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

