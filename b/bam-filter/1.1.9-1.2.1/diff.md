# Comparing `tmp/bam-filter-1.1.9.tar.gz` & `tmp/bam-filter-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-filter-1.1.9.tar", last modified: Mon Nov 14 22:04:19 2022, max compression
+gzip compressed data, was "bam-filter-1.2.1.tar", last modified: Sat Apr 15 20:03:47 2023, max compression
```

## Comparing `bam-filter-1.1.9.tar` & `bam-filter-1.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-14 22:04:19.500838 bam-filter-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (116)     1575 2022-11-14 22:04:15.000000 bam-filter-1.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       53 2022-11-14 22:04:15.000000 bam-filter-1.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      504 2022-11-14 22:04:19.500838 bam-filter-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    10887 2022-11-14 22:04:15.000000 bam-filter-1.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-14 22:04:19.500838 bam-filter-1.1.9/bam_filter/
--rw-r--r--   0 runner    (1001) docker     (116)       93 2022-11-14 22:04:15.000000 bam-filter-1.1.9/bam_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6508 2022-11-14 22:04:15.000000 bam-filter-1.1.9/bam_filter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2022-11-14 22:04:19.500838 bam-filter-1.1.9/bam_filter/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     6279 2022-11-14 22:04:15.000000 bam-filter-1.1.9/bam_filter/entropy.py
--rw-r--r--   0 runner    (1001) docker     (116)    31020 2022-11-14 22:04:15.000000 bam-filter-1.1.9/bam_filter/sam_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    15565 2022-11-14 22:04:15.000000 bam-filter-1.1.9/bam_filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-14 22:04:19.500838 bam-filter-1.1.9/bam_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      504 2022-11-14 22:04:19.000000 bam-filter-1.1.9/bam_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      403 2022-11-14 22:04:19.000000 bam-filter-1.1.9/bam_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-14 22:04:19.000000 bam-filter-1.1.9/bam_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       56 2022-11-14 22:04:19.000000 bam-filter-1.1.9/bam_filter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      170 2022-11-14 22:04:19.000000 bam-filter-1.1.9/bam_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2022-11-14 22:04:19.000000 bam-filter-1.1.9/bam_filter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      687 2022-11-14 22:04:19.500838 bam-filter-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1168 2022-11-14 22:04:15.000000 bam-filter-1.1.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)    70238 2022-11-14 22:04:15.000000 bam-filter-1.1.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:03:47.718148 bam-filter-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-15 20:03:42.000000 bam-filter-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-15 20:03:42.000000 bam-filter-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-15 20:03:47.718148 bam-filter-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-04-15 20:03:42.000000 bam-filter-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:03:47.718148 bam-filter-1.2.1/bam_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-15 20:03:42.000000 bam-filter-1.2.1/bam_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-04-15 20:03:42.000000 bam-filter-1.2.1/bam_filter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-15 20:03:47.718148 bam-filter-1.2.1/bam_filter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-04-15 20:03:42.000000 bam-filter-1.2.1/bam_filter/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43579 2023-04-15 20:03:42.000000 bam-filter-1.2.1/bam_filter/sam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23200 2023-04-15 20:03:42.000000 bam-filter-1.2.1/bam_filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 20:03:47.718148 bam-filter-1.2.1/bam_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-15 20:03:47.000000 bam-filter-1.2.1/bam_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-15 20:03:47.000000 bam-filter-1.2.1/bam_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 20:03:47.000000 bam-filter-1.2.1/bam_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-15 20:03:47.000000 bam-filter-1.2.1/bam_filter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-15 20:03:47.000000 bam-filter-1.2.1/bam_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 20:03:47.000000 bam-filter-1.2.1/bam_filter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-15 20:03:47.718148 bam-filter-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-15 20:03:42.000000 bam-filter-1.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70238 2023-04-15 20:03:42.000000 bam-filter-1.2.1/versioneer.py
```

### Comparing `bam-filter-1.1.9/LICENSE` & `bam-filter-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bam-filter-1.1.9/README.md` & `bam-filter-1.2.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -53,72 +53,108 @@
 
 # Usage
 
 filterBAM only needs a BAM file. For a complete list of options:
 
 ```
 $ filterBAM --help
-
-usage: filterBAM [-h] [-t THREADS] [-p PREFIX] [-A MIN_READ_ANI] [-l MIN_READ_LENGTH] [-n MIN_READ_COUNT] [-b MIN_EXPECTED_BREADTH_RATIO] [-e MIN_NORM_ENTROPY] [-g MIN_NORM_GINI] [-B MIN_BREADTH]
-                 [-a MIN_AVG_READ_ANI] [-c MIN_COVERAGE_EVENNESS] [-m SORT_MEMORY] [-N] [--scale SCALE] [-r REFERENCE_LENGTHS] [--read-length-freqs] [--only-stats] [--plot] [--only-stats-filtered]
-                 [--chunk-size CHUNK_SIZE] [--debug] [--version]
-                 bam
+usage: filterBAM [-h] --bam BAM [-t INT] [--reference-trim-length INT] [--trim-min INT]
+                 [--trim-max INT] [-p STR] [-A FLOAT] [-l INT] [-n INT] [-b FLOAT] [-e FLOAT]
+                 [-g FLOAT] [-B FLOAT] [-a FLOAT] [-c FLOAT] [-V FLOAT] [-C FLOAT]
+                 [--include-low-detection] [-m STR] [-N] [--disable-sort] [--scale STR] [-r FILE]
+                 --stats [FILE] [--stats-filtered [FILE]] [--bam-filtered [FILE]]
+                 [--read-length-freqs [FILE]] [--read-hits-count [FILE]] [--knee-plot [FILE]]
+                 [--coverage-plots [FILE]] [--chunk-size INT] [--tmp-dir DIR] [--low-memory] [--debug]
+                 [--version]
 
 A simple tool to calculate metrics from a BAM file and filter with uneven coverage.
 
-positional arguments:
-  bam                   BAM file containing aligned reads
-
 optional arguments:
   -h, --help            show this help message and exit
-  -t THREADS, --threads THREADS
+  --bam BAM             BAM file containing aligned reads (default: None)
+  -t INT, --threads INT
                         Number of threads to use (default: 1)
-  -p PREFIX, --prefix PREFIX
-                        Prefix used for the output files (default: None)
-  -A MIN_READ_ANI, --min-read-ani MIN_READ_ANI
+  -p STR, --prefix STR  Prefix used for the output files (default: None)
+  -m STR, --sort-memory STR
+                        Set maximum memory per thread for sorting; suffix K/M/G recognized (default:
+                        1G)
+  -N, --sort-by-name    Sort by read names (default: False)
+  --disable-sort        Disable sorting of the filtered BAM file (default: False)
+  --scale STR           Scale taxonomic abundance by this factor; suffix K/M recognized (default:
+                        1000000.0)
+  -r FILE, --reference-lengths FILE
+                        File with references lengths (default: None)
+  --chunk-size INT      Chunk size for parallel processing (default: None)
+  --tmp-dir DIR         Temporary directory (default: None)
+  --low-memory          Activate the low memory mode (default: False)
+  --debug               Print debug messages (default: False)
+  --version             Print program version
+
+filtering arguments:
+  -A FLOAT, --min-read-ani FLOAT
                         Minimum read ANI to keep a read (default: 90.0)
-  -l MIN_READ_LENGTH, --min-read-length MIN_READ_LENGTH
+  -l INT, --min-read-length INT
                         Minimum read length (default: 30)
-  -n MIN_READ_COUNT, --min-read-count MIN_READ_COUNT
-                        Minimum read count (default: 10)
-  -b MIN_EXPECTED_BREADTH_RATIO, --min-expected-breadth-ratio MIN_EXPECTED_BREADTH_RATIO
-                        Minimum expected breadth ratio (default: 0.5)
-  -e MIN_NORM_ENTROPY, --min-normalized-entropy MIN_NORM_ENTROPY
-                        Minimum normalized entropy (default: auto)
-  -g MIN_NORM_GINI, --min-normalized-gini MIN_NORM_GINI
-                        Minimum normalized Gini coefficient (default: auto)
-  -B MIN_BREADTH, --min-breadth MIN_BREADTH
+  -n INT, --min-read-count INT
+                        Minimum read count (default: 3)
+  -b FLOAT, --min-expected-breadth-ratio FLOAT
+                        Minimum expected breadth ratio (default: 0)
+  -e FLOAT, --min-normalized-entropy FLOAT
+                        Minimum normalized entropy (default: 0)
+  -g FLOAT, --min-normalized-gini FLOAT
+                        Minimum normalized Gini coefficient (default: 1.0)
+  -B FLOAT, --min-breadth FLOAT
                         Minimum breadth (default: 0)
-  -a MIN_AVG_READ_ANI, --min-avg-read-ani MIN_AVG_READ_ANI
+  -a FLOAT, --min-avg-read-ani FLOAT
                         Minimum average read ANI (default: 90.0)
-  -c MIN_COVERAGE_EVENNESS, --min-coverage-evenness MIN_COVERAGE_EVENNESS
+  -c FLOAT, --min-coverage-evenness FLOAT
                         Minimum coverage evenness (default: 0)
-  -m SORT_MEMORY, --sort-memory SORT_MEMORY
-                        Set maximum memory per thread for sorting; suffix K/M/G recognized (default: 1G)
-  -N, --sort-by-name    Sort by read names (default: False)
-  --scale SCALE         Scale taxonomic abundance by this factor; suffix K/M recognized (default: 1000000.0)
-  -r REFERENCE_LENGTHS, --reference-lengths REFERENCE_LENGTHS
-                        File with references lengths (default: None)
-  --read-length-freqs   Save a JSON file with the read length frequencies mapped to each reference (default: False)
-  --only-stats          Only produce statistics and skip filtering (default: False)
-  --plot                Plot genome coverage plots (default: False)
-  --only-stats-filtered
-                        Only filter statistics and skip BAM filtering (default: False)
-  --chunk-size CHUNK_SIZE
-                        Chunk size for parallel processing (default: None)
-  --debug               Print debug messages (default: False)
-  --version             Print program version
+  -V FLOAT, --min-coeff-var FLOAT
+                        Minimum coverage evenness calculated as SD/MEAN (default: inf)
+  -C FLOAT, --min-coverage-mean FLOAT
+                        Minimum coverage mean (default: 0)
+  --include-low-detection
+                        Include those references that fullfi all filtering criteria but the coverage
+                        evenness is 0 (default: False)
+
+miscellaneous arguments:
+  --reference-trim-length INT
+                        Exclude n bases at the ends of the reference sequences (default: 0)
+  --trim-min INT        Remove coverage that are below this percentile. Used for the Truncated Average
+                        Depth (TAD) calculation (default: 10)
+  --trim-max INT        Remove coverage that are above this percentile. Used for the Truncated Average
+                        Depth (TAD) calculation (default: 90)
+
+output arguments:
+  --stats [FILE]        Save a TSV file with the statistics for each reference (default: None)
+  --stats-filtered [FILE]
+                        Save a TSV file with the statistics for each reference after filtering
+                        (default: None)
+  --bam-filtered [FILE]
+                        Save a BAM file with the references that passed the filtering criteria
+                        (default: None)
+  --read-length-freqs [FILE]
+                        Save a JSON file with the read length frequencies mapped to each reference
+                        (default: None)
+  --read-hits-count [FILE]
+                        Save a TSV file with the read hits frequencies mapped to each reference
+                        (default: None)
+  --knee-plot [FILE]    Plot knee plot (default: None)
+  --coverage-plots [FILE]
+                        Folder where to save genome coverage plots (default: None)
 ```
 
 One would run filterBAM as:
 
 ```bash
-filterBAM --min-read-count 100 --min-expected-breadth-ratio 0.75 --min-read-ani 98 --sort-by-name --sort-memory 1G --reference-lengths gtdb-r202.len.map --threads 16  c55d4e2df1.dedup.bam 
+filterBAM --stats --min-read-count 100 --min-expected-breadth-ratio 0.75 --min-read-ani 98 --sort-by-name --sort-memory 1G --reference-lengths gtdb-r202.len.map --threads 16 --bam c55d4e2df1.dedup.bam 
 ```
 
+**--stats**: Save a TSV file with the statistics for each reference
+
 **--min-read-count**: Minimum number of reads mapped to a reference in the BAM file
 
 **--min-expected-breadth-ratio**: Minimum expected breadth ratio needed to keep a reference.
 
 **--min-read-ani**: Minimum average read ANI that a reference has
 
 **--sort-by-name**: Sort filtered BAM file by read name so it can be used in [metaDMG](https://metadmg-dev.github.io/metaDMG-core/)
@@ -150,14 +186,16 @@
     - **read_ani_mean**: Average ANI of the reads mapped to the reference
     - **read_ani_std**: Standard deviation of ANI of the reads mapped to the reference
     - **read_ani_median**: Median ANI of the reads mapped to the reference
     - **bases_covered**: Number of bases covered by the reference
     - **max_covered_bases**: Maximum number of bases covered in the reference
     - **mean_covered_bases**: Average number of bases covered in the reference
     - **coverage_mean**: Mean depth of the reference
+    - **coverage_mean_trunc**: Mean depth of the reference after removing the 10% and 90% of the coverage values (default: TAD80 as calculated [here](https://sfamjournals.onlinelibrary.wiley.com/doi/10.1111/1462-2920.15112))
+    - **coverage_mean_trunc_len**: Length of the reference after being truncated by the TAD(X) values
     - **coverage_covered_mean**: Mean depth of the reference only counting covered bases
     - **reference_length**: Real reference length
     - **bam_reference_length**: Length reported by the BAM file
     - **breadth**: Breadth of coverage 
     - **exp_breadth**: Expected breadth of coverage. Using the formula: _expected_breadth = 1 - e<sup>-coverage</sup>_
     - **breadth_exp_ratio**: Ration between the observed and the expected depth of coverage
     - **n_bins**: Number of bins used to calculate the read coverage distribution
@@ -167,14 +205,18 @@
     - **gini**: Gini coefficient of the read coverage distribution
     - **norm_gini**: Normalized Gini coefficient of the read coverage distribution
     - **c_v**: Coefficient of variation of the coverage
     - **d_i**: Dispersion index
     - **cov_evenness**: Eveness of coverage as calculated [here](https://www.nature.com/articles/jhg201621).
     - **tax_abund_read**: Counts estimated using the number of reads and normalized by the reference length.
     - **tax_abund_aln**: Counts estimated using the number of alignments and normalized by the reference length.
+    - **tax_abund_tad**: Counts estimated using the estimated number of reads in the TAD region and normalized by the length of the TAD region
+    - **n_reads_tad**: Number of reads estimated in the TAD region using the formula *C = LN / G*, where C stands for the TAD coverage, N for the length of the TAD region and L for the average read length mapped to the reference.
+
+> 
 
 ## Applications and recommendations
 
 One of the main applications of **bam-filter** is to reliably identify which potential organisms are present in a metagenomic ancient sample, and get relatively accurate taxonomic abundances, even when they are present in very low abundances. The resulting BAM file then can be used as input for [metaDMG](https://metadmg-dev.github.io/metaDMG-core/). We rely on several measures to discriminate between noise and a potential signal, analyzing the mapping results at two different levels:
 
 - Is the observed breadth aligned with the expected one?
 - Are the reads spread evenly across the reference or they are clumped in a few regions?
```

### Comparing `bam-filter-1.1.9/bam_filter/entropy.py` & `bam-filter-1.2.1/bam_filter/entropy.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 log = logging.getLogger("my_logger")
 
 plt_log = logging.getLogger("matplotlib")
 plt_log.setLevel(logging.ERROR)
 
 logging.getLogger("PIL").setLevel(logging.WARNING)
 
+
 # Code from: https://www.frontiersin.org/articles/10.3389/fmicb.2022.918015/full
 def entropy(counts):
     counts_vector = np.array(counts)
     frequencies = counts_vector / counts_vector.sum()
     H = 0
     for p in frequencies:
         if p != 0:
@@ -170,26 +171,30 @@
     y = df2_round["norm_entropy"].values
     kneedle = KneeLocator(
         x, y, S=1.0, curve="concave", direction="decreasing", online=True
     )
 
     if kneedle.knee is None:
         return None, None
-
     min_gini = round(kneedle.elbow, 3)
     min_entropy = round(kneedle.knee_y, 3)
     logging.info(f"Knee point found: gini={min_gini}, entropy={min_entropy}")
-    logging.info("Knee point figure saved at kneedle.png")
-    fig, ax = plt.subplots(nrows=1, ncols=1)
-    plt.suptitle("Knee Point")
-    plt.title(f"Knee point: gini={min_gini}, entropy={min_entropy}")
-    plt.plot(kneedle.x, kneedle.y, "c", label="data")
-    plt.vlines(
-        kneedle.knee, plt.ylim()[0], plt.ylim()[1], linestyles="--", label="knee/elbow"
-    )
-    plt.xlabel("Normalized Gini coefficient")
-    plt.ylabel("Normalized Entropy")
-    plt.legend(loc="best")  # create figure & 1 axis
-    fig.savefig(out_plot_name, dpi=300)
-    plt.close(fig)
+    if out_plot_name is not None:
+        logging.info("Knee point figure saved at kneedle.png")
+        fig, ax = plt.subplots(nrows=1, ncols=1)
+        plt.suptitle("Knee Point")
+        plt.title(f"Knee point: gini={min_gini}, entropy={min_entropy}")
+        plt.plot(kneedle.x, kneedle.y, "c", label="data")
+        plt.vlines(
+            kneedle.knee,
+            plt.ylim()[0],
+            plt.ylim()[1],
+            linestyles="--",
+            label="knee/elbow",
+        )
+        plt.xlabel("Normalized Gini coefficient")
+        plt.ylabel("Normalized Entropy")
+        plt.legend(loc="best")  # create figure & 1 axis
+        fig.savefig(out_plot_name, dpi=300)
+        plt.close(fig)
 
     return min_gini, min_entropy
```

### Comparing `bam-filter-1.1.9/bam_filter/sam_utils.py` & `bam-filter-1.2.1/bam_filter/sam_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,169 @@
 import pysam
 import numpy as np
-import os, sys
+import os
+import sys
 import pandas as pd
 from multiprocessing import Pool
 import functools
 from scipy import stats
-import pysam
 import tqdm
 import logging
 import warnings
-from bam_filter.utils import is_debug, calc_chunksize, initializer
+from bam_filter.utils import (
+    is_debug,
+    calc_chunksize,
+    initializer,
+    create_empty_output_files,
+    create_empty_bam,
+)
 from bam_filter.entropy import entropy, norm_entropy, gini_coeff, norm_gini_coeff
-
+from collections import defaultdict
 import pyranges as pr
+from pathlib import Path
 
 # import cProfile as profile
 # import pstats
 
+# import pstats
+
 import matplotlib.pyplot as plt
 
 log = logging.getLogger("my_logger")
 
 
 sys.setrecursionlimit(10**6)
 
 
+# def get_alns(params):
+#     bam, reference = params
+#     samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
+#     alns = []
+#     for aln in samfile.fetch(
+#         reference=reference, multiple_iterators=False, until_eof=True
+#     ):
+#         alns.append(aln.to_string())
+#     return alns
+
+
+def write_bam(bam, references, output_files, threads=1, sort_memory="1G"):
+    logging.info("::: Writing temporary filtered BAM file... (be patient)")
+    samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
+
+    if threads > 4:
+        threads = 4
+
+    # convert the dictionary to an array
+    refs_dict = dict(zip(samfile.references, samfile.lengths))
+    my_array = np.array(list(refs_dict.items()))
+
+    # get the indices of the keys to keep
+    keep_indices = np.isin(my_array[:, 0], references)
+
+    # use array indexing to get the key-value pairs to keep
+    filtered_array = my_array[keep_indices]
+
+    # convert the filtered array back to a dictionary
+    refs_dict = dict(filtered_array)
+
+    (ref_names, ref_lengths) = zip(*refs_dict.items())
+    ref_lengths = list(ref_lengths)
+    # convert reference lengths to integers
+    ref_lengths = [int(x) for x in ref_lengths]
+
+    refs_idx = {sys.intern(str(x)): i for i, x in enumerate(ref_names)}
+
+    if threads > 4:
+        write_threads = 4
+    else:
+        write_threads = threads
+
+    out_bam_file = pysam.AlignmentFile(
+        output_files["bam_tmp"],
+        "wb",
+        referencenames=list(ref_names),
+        referencelengths=ref_lengths,
+        threads=write_threads,
+    )
+
+    references = [x for x in samfile.references if x in refs_idx.keys()]
+
+    logging.info(f"::: ::: Filtering {len(references):,} references sequentially...")
+    for reference in tqdm.tqdm(
+        references,
+        total=len(references),
+        leave=False,
+        ncols=80,
+        desc="References processed",
+    ):
+        for aln in samfile.fetch(
+            reference=reference, multiple_iterators=False, until_eof=True
+        ):
+            aln.reference_id = refs_idx[aln.reference_name]
+            out_bam_file.write(aln)
+    out_bam_file.close()
+    samfile.close()
+    # prof.disable()
+    # # print profiling output
+    # stats = pstats.Stats(prof).strip_dirs().sort_stats("tottime")
+    # stats.print_stats(5)  # top 10 rows
+    logging.info("::: ::: Sorting BAM file...")
+    pysam.sort(
+        "-@",
+        str(threads),
+        "-m",
+        str(sort_memory),
+        "-o",
+        output_files["bam_tmp_sorted"],
+        output_files["bam_tmp"],
+    )
+
+    logging.info("::: ::: BAM index not found. Indexing...")
+    save = pysam.set_verbosity(0)
+    samfile = pysam.AlignmentFile(output_files["bam_tmp_sorted"], "rb", threads=threads)
+    chr_lengths = []
+    for chrom in samfile.references:
+        chr_lengths.append(samfile.get_reference_length(chrom))
+    max_chr_length = np.max(chr_lengths)
+    pysam.set_verbosity(save)
+    samfile.close()
+
+    if max_chr_length > 536870912:
+        logging.info("::: ::: A reference is longer than 2^29, indexing with csi")
+        pysam.index(
+            "-c",
+            "-@",
+            str(threads),
+            output_files["bam_tmp_sorted"],
+        )
+    else:
+        pysam.index(
+            "-@",
+            str(threads),
+            output_files["bam_tmp_sorted"],
+        )
+
+    os.remove(output_files["bam_tmp"])
+    return output_files["bam_tmp_sorted"]
+
+
+def get_tad(cov, trim_min=10, trim_max=90):
+    """
+    Get the TAD of a coverage
+    """
+    cov = cov[
+        (cov >= np.percentile(cov, trim_min)) & (cov <= np.percentile(cov, trim_max))
+    ]
+
+    if np.sum(cov) == 0:
+        return 0, 0
+    else:
+        return np.sum(cov) / len(cov), len(cov)
+
+
 # Function to calculate evenness of coverage
 def coverage_evenness(coverage):
     """
     Calculate the evenness of coverage
     """
     # get coverage evenness
     # covEvenness = (
@@ -45,15 +180,15 @@
     # D2 = [x for x in coverage if x <= C]
     # print(len(D2))
     # exit()
     if len(D2) == 0:  # pragma: no cover
         covEvenness = 1.0
     else:
         if C > 0:
-            covEvenness = 1.0 - (len(D2) - sum(D2) / C) / len(coverage)
+            covEvenness = 1.0 - (len(D2) - np.sum(D2) / C) / len(coverage)
         else:
             covEvenness = 0.0
 
     return covEvenness
 
 
 # function to calculate GC content
@@ -93,28 +228,34 @@
 
 
 def get_bam_stats(
     params,
     ref_lengths=None,
     min_read_ani=90.0,
     scale=1e6,
+    trim_ends=0,
+    trim_min=10,
+    trim_max=90,
     plot=False,
     plots_dir="coverage-plots",
+    read_length_freqs=False,
+    threads=1,
 ):
     """
     Worker function per chromosome
     loop over a bam file and create tuple with lists containing metrics:
     two definitions of the edit distances to the reference genome scaled by aligned read length
     """
     # prof = profile.Profile()
     # prof.enable()
     bam, references = params
     results = []
-    samfile = pysam.AlignmentFile(bam, "rb")
+    samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
 
+    read_hits = defaultdict(int)
     for reference in references:
         edit_distances = []
         # edit_distances_md = []
         ani_nm = []
         # ani_md = []
         read_length = []
         read_aligned_length = []
@@ -133,20 +274,22 @@
         log.debug(f"Processing reference {reference}")
         log.debug(f"Reference length: {reference_length:,}")
         log.debug(f"BAM reference length: {bam_reference_length:,}")
         starts = []
         ends = []
         strands = []
         cov_np = np.zeros(samfile.get_reference_length(reference), dtype=int)
+
         for aln in samfile.fetch(
-            contig=reference, multiple_iterators=False, until_eof=False
+            contig=reference, multiple_iterators=False, until_eof=True
         ):
             ani_read = (1 - ((aln.get_tag("NM") / aln.infer_query_length()))) * 100
             if ani_read >= min_read_ani:
                 n_alns += 1
+                read_hits[aln.query_name] += 1
                 if aln.has_tag("AS"):
                     read_aln_score.append(aln.get_tag("AS"))
                 else:
                     read_aln_score.append(np.nan)
 
                 if aln.has_tag("AS"):
                     edit_distances.append(aln.get_tag("NM"))
@@ -165,184 +308,240 @@
                     strand = "-"
                 else:
                     strand = "+"
                 starts.append(aln.reference_start)
                 ends.append(aln.reference_end)
                 strands.append(strand)
 
-            cov_np[aln.reference_start : aln.reference_end] += 1
+                cov_np[aln.reference_start : aln.reference_end] += 1
+        if n_alns > 0:
+            # get bases covered by reads pileup
+
+            # cov_pos_raw = [
+            #     (pileupcolumn.pos, pileupcolumn.n)
+            #     for pileupcolumn in samfile.pileup(
+            #         reference,
+            #         start=None,
+            #         stop=None,
+            #         region=None,
+            #         stepper="nofilter",
+            #         min_mapping_quality=0,
+            #         max_depth=100000000,
+            #     )
+            # ]
+            if trim_ends > len(cov_np) or trim_ends * 2 > len(cov_np):
+                log.warning(
+                    f"Trimming ends ({trim_ends}) is larger than reference length ({len(cov_np)}). Disabling trimming."
+                )
+                trim_ends = 0
 
-        # get bases covered by reads pileup
+            if trim_ends > 0:
+                cov_np = cov_np[trim_ends:-trim_ends]
 
-        # cov_pos_raw = [
-        #     (pileupcolumn.pos, pileupcolumn.n)
-        #     for pileupcolumn in samfile.pileup(
-        #         reference,
-        #         start=None,
-        #         stop=None,
-        #         region=None,
-        #         stepper="nofilter",
-        #         min_mapping_quality=0,
-        #         max_depth=100000000,
-        #     )
-        # ]
-        cov_pos = cov_np[cov_np > 0]
-        cov_positions = np.where(cov_np > 0)[0]
-        # convert datafrane to pyranges
-        ranges = create_pyranges(reference, starts, ends, strands)
-        if ranges.df.shape[0] == 0:
-            log.debug(f"No alignments found for {reference}")
-            return None
-        ranges_raw = ranges.merge(strand=False)
-        ranges = ranges_raw.lengths().to_list()
-
-        max_covered_bases = np.max(ranges)
-        mean_covered_bases = np.mean(ranges)
-        bases_covered = int(len(cov_pos))
-        # get SD from covered bases
-        cov_sd = np.std(cov_pos, ddof=1)
-        cov_var = np.var(cov_pos, ddof=1)
-        # get average coverage
-        mean_coverage = sum(cov_pos) / reference_length
-        mean_coverage_covered = sum(cov_pos) / bases_covered
-
-        breadth = bases_covered / reference_length
-        exp_breadth = 1 - np.exp(-mean_coverage)
-        breadth_exp_ratio = breadth / exp_breadth
-
-        if breadth_exp_ratio > 1:
-            breadth_exp_ratio = 1.0
-
-        # fill vector with zeros to match reference length
-        # cov_pos_zeroes = np.pad(
-        #     cov_pos, (0, reference_length - len(cov_pos)), "constant"
-        # )
-        cov_evenness = coverage_evenness(cov_np)
-        gc_content = (np.sum(read_gc_content) / np.sum(read_length)) * 100
-        c_v = cov_sd / mean_coverage
-        d_i = cov_var / mean_coverage
-
-        read_mapq = [np.nan if x == 255 else x for x in read_mapq]
-
-        tax_abund_aln = round((n_alns / reference_length) * scale)
-        tax_abund_read = round((len(set(read_names)) / reference_length) * scale)
-
-        # Analyse site distribution
-        n_sites = len(cov_pos)
-        genome_length = bam_reference_length
-        # Site density (sites per thousand bp)
-        site_density = 1000 * n_sites / genome_length
-
-        counts, bins = np.histogram(
-            cov_positions, bins="auto", range=(0, genome_length)
-        )
-
-        n_bins = len(bins)
-
-        entr = entropy(counts)  # Positional entropy
-        norm_entr = norm_entropy(counts)  # Normalized positional entropy
-        gini = gini_coeff(counts)  # Gini coefficient
-        norm_gini = norm_gini_coeff(counts)  # Normalized Gini coefficient
-
-        log.debug(f"Number of reads: {len(set(read_names)):,}")
-        log.debug(f"Number of alignments: {n_alns:,}")
-        log.debug(f"Bases covered: {bases_covered:,}")
-        log.debug(f"Mean coverage: {mean_coverage:.2f}")
-        log.debug(f"Mean coverage covered: {mean_coverage_covered:.2f}")
-        log.debug(f"Max covered bases: {max_covered_bases:,}")
-        log.debug(f"Mean covered bases: {mean_covered_bases:.2f}")
-        log.debug(f"SD: {cov_sd:.2f}")
-        log.debug(f"Breadth: {breadth:.2f}")
-        log.debug(f"Exp. breadth: {exp_breadth:.2f}")
-        log.debug(f"Breadth/exp. ratio: {breadth_exp_ratio:.2f}")
-        log.debug(f"Number of bins: {n_bins}")
-        log.debug(f"Site density: {site_density:.2f}")
-        log.debug(f"Entropy (H): {entr:.2f}")
-        log.debug(f"Normalized entropy (H*): {norm_entr:.2f}")
-        log.debug(f"Gini coefficient (G): {gini:.2f}")
-        log.debug(f"Normalized Gini coefficient (G*): {norm_gini:.2f}")
-        log.debug(f"Cov. evenness: {cov_evenness:.2f}")
-        log.debug(f"C_v: {c_v:.2f}")
-        log.debug(f"D_i: {d_i:.2f}")
-        log.debug(f"Mean mapq: {np.mean(read_mapq):.2f}")
-        log.debug(f"GC content: {gc_content:.2f}")
-        log.debug(f"Taxonomic abundance (alns): {tax_abund_aln:.2f}")
-        log.debug(f"Taxonomic abundance (reads): {tax_abund_read:.2f}")
-
-        if plot:
-            fig, ax = plt.subplots(nrows=1, ncols=1)  # create figure & 1 axis
-            # infer number of bins using Freedman-Diaconis rule
-            positions_cov_zeros = pd.DataFrame(
-                {"pos": range(1, bam_reference_length + 1)}
-            )
-            positions_cov = pd.DataFrame({"pos": cov_positions, "cov": cov_pos})
-            positions_cov = positions_cov_zeros.merge(
-                positions_cov, on="pos", how="left"
-            )
-            positions_cov["cov"] = positions_cov["cov"].fillna(0)
-            positions_cov["cov"] = positions_cov["cov"].astype(int)
-            positions_cov["cov_binary"] = positions_cov["cov"].apply(
-                lambda x: 1 if x > 0 else 0
-            )
-            plt.plot(
-                positions_cov["pos"],
-                positions_cov["cov"],
-                color="c",
-                ms=0.5,
-            )
-            plt.suptitle(f"{reference}")
-            plt.title(
-                f"cov:{mean_coverage:.4f} b/e:{breadth_exp_ratio:.2f} cov_e:{cov_evenness:.2f} entropy:{norm_entr:.2f} gini:{norm_gini:.2f}"
-            )
-            fig.savefig(f"{plots_dir}/{reference}_coverage.png", dpi=300)
-            plt.close(fig)
-
-        data = BamAlignment(
-            reference=reference,
-            n_alns=n_alns,
-            reference_length=reference_length,
-            bam_reference_length=bam_reference_length,
-            mean_coverage=mean_coverage,
-            mean_coverage_covered=mean_coverage_covered,
-            bases_covered=bases_covered,
-            max_covered_bases=max_covered_bases,
-            mean_covered_bases=mean_covered_bases,
-            cov_evenness=cov_evenness,
-            breadth=breadth,
-            exp_breadth=exp_breadth,
-            breadth_exp_ratio=breadth_exp_ratio,
-            n_bins=n_bins,
-            site_density=site_density,
-            entropy=entr,
-            norm_entropy=norm_entr,
-            gini=gini,
-            norm_gini=norm_gini,
-            c_v=c_v,
-            d_i=d_i,
-            edit_distances=edit_distances,
-            # edit_distances_md=edit_distances_md,
-            ani_nm=ani_nm,
-            # ani_md=ani_md,
-            read_length=read_length,
-            read_gc_content=read_gc_content,
-            read_aligned_length=read_aligned_length,
-            mapping_quality=read_mapq,
-            read_names=set(read_names),
-            read_aln_score=read_aln_score,
-            tax_abund_aln=tax_abund_aln,
-            tax_abund_read=tax_abund_read,
-        )
-        results.append(data)
+            mean_coverage_trunc, mean_coverage_trunc_len = get_tad(
+                cov_np,
+                trim_min=10,
+                trim_max=90,
+            )
+
+            cov_pos = cov_np[cov_np > 0]
+            cov_positions = np.where(cov_np > 0)[0]
+            # convert datafrane to pyranges
+            ranges = create_pyranges(reference, starts, ends, strands)
+            if ranges.df.shape[0] == 0:
+                log.debug(f"No alignments found for {reference}")
+                results.append(None)
+                continue
+            ranges_raw = ranges.merge(strand=False)
+            ranges = ranges_raw.lengths().to_list()
+
+            max_covered_bases = np.max(ranges)
+            mean_covered_bases = np.mean(ranges)
+            bases_covered = int(len(cov_pos))
+            # get SD from covered bases
+            cov_sd = np.std(cov_pos, ddof=1)
+            cov_var = np.var(cov_pos, ddof=1)
+            # get average coverage
+            mean_coverage = np.sum(cov_pos) / (reference_length - (2 * trim_ends))
+            mean_coverage_covered = np.sum(cov_pos) / bases_covered
+
+            breadth = bases_covered / (reference_length - (2 * trim_ends))
+            exp_breadth = 1 - np.exp(-mean_coverage)
+            breadth_exp_ratio = breadth / exp_breadth
+
+            if breadth_exp_ratio > 1:
+                breadth_exp_ratio = 1.0
+
+            # fill vector with zeros to match reference length
+            # cov_pos_zeroes = np.pad(
+            #     cov_pos, (0, reference_length - len(cov_pos)), "constant"
+            # )
+            cov_evenness = coverage_evenness(cov_np)
+            gc_content = (np.sum(read_gc_content) / np.sum(read_length)) * 100
+            c_v = cov_sd / mean_coverage
+            d_i = cov_var / mean_coverage
+
+            read_mapq = [np.nan if x == 255 else x for x in read_mapq]
+
+            tax_abund_aln = round((n_alns / reference_length) * scale)
+            tax_abund_read = round((len(set(read_names)) / reference_length) * scale)
+
+            # Using the trimmed mean to estimate number of reads that map to the reference
+            # This is to avoid the issue of having a very high coverage region that
+            # skews the mean coverage
+            # C = LN / G
+            # • C stands for coverage
+            # • G is the haploid genome length
+            # • L is the read length
+            # • N is the number of reads
+            #
+            if mean_coverage_trunc_len > 0 and mean_coverage_trunc > 0:
+                n_reads_tad = round(
+                    (reference_length * mean_coverage_trunc) / np.mean(read_length)
+                )
+                tax_abund_tad = round((n_reads_tad / mean_coverage_trunc_len) * scale)
+            else:
+                n_reads_tad = 0
+                tax_abund_tad = 0
+            # Analyse site distribution
+            n_sites = len(cov_pos)
+            genome_length = bam_reference_length
+            # Site density (sites per thousand bp)
+            site_density = 1000 * n_sites / genome_length
+
+            counts, bins = np.histogram(
+                cov_positions, bins="auto", range=(0, genome_length)
+            )
+
+            n_bins = len(bins)
+
+            entr = entropy(counts)  # Positional entropy
+            norm_entr = norm_entropy(counts)  # Normalized positional entropy
+            gini = gini_coeff(counts)  # Gini coefficient
+            norm_gini = norm_gini_coeff(counts)  # Normalized Gini coefficient
+
+            log.debug(f"Number of reads: {len(set(read_names)):,}")
+            log.debug(f"Number of alignments: {n_alns:,}")
+            log.debug(f"Bases covered: {bases_covered:,}")
+            log.debug(f"Mean coverage: {mean_coverage:.2f}")
+            log.debug(f"Mean coverage (truncated): {mean_coverage_trunc:.2f}")
+            log.debug(f"Reference length (truncated): {mean_coverage_trunc_len:.2f}")
+            log.debug(f"Mean coverage covered: {mean_coverage_covered:.2f}")
+            log.debug(f"Max covered bases: {max_covered_bases:,}")
+            log.debug(f"Mean covered bases: {mean_covered_bases:.2f}")
+            log.debug(f"SD: {cov_sd:.2f}")
+            log.debug(f"Breadth: {breadth:.2f}")
+            log.debug(f"Exp. breadth: {exp_breadth:.2f}")
+            log.debug(f"Breadth/exp. ratio: {breadth_exp_ratio:.2f}")
+            log.debug(f"Number of bins: {n_bins}")
+            log.debug(f"Site density: {site_density:.2f}")
+            log.debug(f"Entropy (H): {entr:.2f}")
+            log.debug(f"Normalized entropy (H*): {norm_entr:.2f}")
+            log.debug(f"Gini coefficient (G): {gini:.2f}")
+            log.debug(f"Normalized Gini coefficient (G*): {norm_gini:.2f}")
+            log.debug(f"Cov. evenness: {cov_evenness:.2f}")
+            log.debug(f"C_v: {c_v:.2f}")
+            log.debug(f"D_i: {d_i:.2f}")
+            log.debug(f"Mean mapq: {np.mean(read_mapq):.2f}")
+            log.debug(f"GC content: {gc_content:.2f}")
+            log.debug(f"Taxonomic abundance (alns): {tax_abund_aln:.2f}")
+            log.debug(f"Taxonomic abundance (reads): {tax_abund_read:.2f}")
+            log.debug(f"Taxonomic abundance (TAD): {tax_abund_tad:.2f}")
+            log.debug(f"Number of reads (TAD): {n_reads_tad:,}")
+            if plot:
+                fig, ax = plt.subplots(nrows=1, ncols=1)  # create figure & 1 axis
+                # infer number of bins using Freedman-Diaconis rule
+                positions_cov_zeros = pd.DataFrame(
+                    {"pos": range(1, bam_reference_length + 1)}
+                )
+                positions_cov = pd.DataFrame({"pos": cov_positions, "cov": cov_pos})
+                positions_cov = positions_cov_zeros.merge(
+                    positions_cov, on="pos", how="left"
+                )
+                positions_cov["cov"] = positions_cov["cov"].fillna(0)
+                positions_cov["cov"] = positions_cov["cov"].astype(int)
+                positions_cov["cov_binary"] = positions_cov["cov"].apply(
+                    lambda x: 1 if x > 0 else 0
+                )
+                plt.plot(
+                    positions_cov["pos"],
+                    positions_cov["cov"],
+                    color="c",
+                    ms=0.5,
+                )
+                plt.suptitle(f"{reference}")
+                plt.title(
+                    f"cov:{mean_coverage:.4f} b/e:{breadth_exp_ratio:.2f} cov_e:{cov_evenness:.2f} entropy:{norm_entr:.2f} gini:{norm_gini:.2f}"
+                )
+                fig.savefig(f"{plots_dir}/{reference}_coverage.png", dpi=300)
+                plt.close(fig)
+
+            data = BamAlignment(
+                reference=reference,
+                n_alns=n_alns,
+                reference_length=reference_length,
+                bam_reference_length=bam_reference_length,
+                mean_coverage=mean_coverage,
+                mean_coverage_trunc=mean_coverage_trunc,
+                mean_coverage_trunc_len=mean_coverage_trunc_len,
+                mean_coverage_covered=mean_coverage_covered,
+                bases_covered=bases_covered,
+                max_covered_bases=max_covered_bases,
+                mean_covered_bases=mean_covered_bases,
+                cov_evenness=cov_evenness,
+                breadth=breadth,
+                exp_breadth=exp_breadth,
+                breadth_exp_ratio=breadth_exp_ratio,
+                n_bins=n_bins,
+                site_density=site_density,
+                entropy=entr,
+                norm_entropy=norm_entr,
+                gini=gini,
+                norm_gini=norm_gini,
+                c_v=c_v,
+                d_i=d_i,
+                edit_distances=edit_distances,
+                # edit_distances_md=edit_distances_md,
+                ani_nm=ani_nm,
+                # ani_md=ani_md,
+                read_length=read_length,
+                read_gc_content=read_gc_content,
+                read_aligned_length=read_aligned_length,
+                mapping_quality=read_mapq,
+                read_names=set(read_names),
+                read_aln_score=read_aln_score,
+                tax_abund_aln=tax_abund_aln,
+                tax_abund_read=tax_abund_read,
+                tax_abund_tad=tax_abund_tad,
+                n_reads_tad=n_reads_tad,
+            )
+            results.append(data)
     samfile.close()
     # prof.disable()
     # # print profiling output
     # stats = pstats.Stats(prof).strip_dirs().sort_stats("tottime")
     # stats.print_stats(5)  # top 10 rows
-
-    return results
+    # exit()
+    # results = [x[0] for x in results if x[0] is not None]
+    results = list(filter(None, results))
+    data_df = pd.DataFrame([x.to_summary() for x in results])
+    # read_hits = (
+    #     pd.DataFrame.from_dict(read_hits, orient="index", columns=["count"])
+    #     .rename_axis("read_id")
+    #     .reset_index()
+    # )
+    if read_length_freqs:
+        read_lens = [x.get_read_length_freqs() for x in results]
+        return (data_df, read_lens, read_hits)
+    else:
+        return (
+            data_df,
+            None,
+            read_hits,
+        )
 
 
 class BamAlignment:
     """
     Class to store alignment information
     """
 
@@ -358,14 +557,16 @@
         # edit_distances_md,
         ani_nm,
         # ani_md,
         bases_covered,
         max_covered_bases,
         mean_covered_bases,
         mean_coverage,
+        mean_coverage_trunc,
+        mean_coverage_trunc_len,
         mean_coverage_covered,
         reference_length,
         bam_reference_length,
         breadth,
         exp_breadth,
         breadth_exp_ratio,
         n_bins,
@@ -377,14 +578,16 @@
         c_v,
         d_i,
         cov_evenness,
         read_names,
         read_aln_score,
         tax_abund_aln,
         tax_abund_read,
+        tax_abund_tad,
+        n_reads_tad,
     ):
         self.reference = reference
         self.n_alns = n_alns
         self.read_length = read_length
         self.read_gc_content = read_gc_content
         self.read_aligned_length = read_aligned_length
         self.read_aln_score = read_aln_score
@@ -393,14 +596,16 @@
         # self.edit_distances_md = edit_distances_md
         self.ani_nm = ani_nm
         # self.ani_md = ani_md
         self.bases_covered = bases_covered
         self.max_covered_bases = max_covered_bases
         self.mean_covered_bases = mean_covered_bases
         self.mean_coverage = mean_coverage
+        self.mean_coverage_trunc = mean_coverage_trunc
+        self.mean_coverage_trunc_len = mean_coverage_trunc_len
         self.mean_coverage_covered = mean_coverage_covered
         self.reference_length = reference_length
         self.bam_reference_length = bam_reference_length
         self.breadth = breadth
         self.exp_breadth = exp_breadth
         self.breadth_exp_ratio = breadth_exp_ratio
         self.n_bins = n_bins
@@ -411,14 +616,16 @@
         self.norm_gini = norm_gini
         self.c_v = c_v
         self.d_i = d_i
         self.cov_evenness = cov_evenness
         self.read_names = read_names
         self.tax_abund_aln = tax_abund_aln
         self.tax_abund_read = tax_abund_read
+        self.tax_abund_tad = tax_abund_tad
+        self.n_reads_tad = n_reads_tad
         # function to convert class to dict
 
     def as_dict(self):
         return {
             "reference": self.reference,
             "n_reads": self.read_names,
             "n_alns": self.n_alns,
@@ -431,14 +638,16 @@
             # "edit_distances_md": np.mean(self.edit_distances_md),
             "ani_nm": self.ani_nm,
             # "ani_md": np.mean(self.ani_md),
             "bases_covered": self.bases_covered,
             "max_covered_bases": self.max_covered_bases,
             "mean_covered_bases": self.mean_covered_bases,
             "mean_coverage": self.mean_coverage,
+            "mean_coverage_trunc": self.mean_coverage_trunc,
+            "mean_coverage_trunc_len": self.mean_coverage_trunc_len,
             "mean_coverage_covered": self.mean_coverage_covered,
             "reference_length": self.reference_length,
             "breadth": self.breadth,
             "exp_breadth": self.exp_breadth,
             "breadth_exp_ratio": self.breadth_exp_ratio,
             "n_bins": self.n_bins,
             "site_density": self.site_density,
@@ -447,14 +656,16 @@
             "gini": self.gini,
             "norm_gini": self.norm_gini,
             "c_v": self.c_v,
             "d_i": self.d_i,
             "cov_evenness": self.cov_evenness,
             "tax_abund_read": self.tax_abund_read,
             "tax_abund_aln": self.tax_abund_aln,
+            "tax_abund_tad": self.tax_abund_tad,
+            "n_reads_tad": self.n_reads_tad,
         }
 
     def to_summary(self):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", category=RuntimeWarning)
             read_length_mean = np.mean(self.read_length)
             read_length_median = np.median(self.read_length)
@@ -490,14 +701,16 @@
             "read_ani_std": read_ani_std,
             "read_ani_median": read_ani_median,
             # "ani_md": np.mean(self.ani_md),
             "bases_covered": self.bases_covered,
             "max_covered_bases": self.max_covered_bases,
             "mean_covered_bases": self.mean_covered_bases,
             "coverage_mean": self.mean_coverage,
+            "coverage_mean_trunc": self.mean_coverage_trunc,
+            "coverage_mean_trunc_len": self.mean_coverage_trunc_len,
             "coverage_covered_mean": self.mean_coverage_covered,
             "reference_length": self.reference_length,
             "bam_reference_length": self.bam_reference_length,
             "breadth": self.breadth,
             "exp_breadth": self.exp_breadth,
             "breadth_exp_ratio": self.breadth_exp_ratio,
             "n_bins": self.n_bins,
@@ -507,46 +720,36 @@
             "gini": self.gini,
             "norm_gini": self.norm_gini,
             "c_v": self.c_v,
             "d_i": self.d_i,
             "cov_evenness": self.cov_evenness,
             "tax_abund_read": self.tax_abund_read,
             "tax_abund_aln": self.tax_abund_aln,
+            "tax_abund_tad": self.tax_abund_tad,
+            "n_reads_tad": self.n_reads_tad,
         }
 
     def get_read_length_freqs(self):
         frags = {}
         lengths = pd.Series(self.read_length)
         lengths = lengths.value_counts().sort_index()
-        freqs = list(lengths / sum(lengths))
+        freqs = list(lengths / np.sum(lengths))
         frags[self.reference] = {"length": list(lengths.index), "freq": freqs}
         return frags
 
 
-# Inspired from https://gigabaseorgigabyte.wordpress.com/2017/04/14/getting-the-edit-distance-from-a-bam-alignment-a-journey/
-def process_bam(
+def check_bam_file(
     bam,
     threads=1,
     reference_lengths=None,
-    min_read_ani=90.0,
-    min_read_count=10,
-    scale=1e6,
     sort_memory="1G",
-    plot=False,
-    plots_dir="coverage-plots",
-    chunksize=None,
 ):
-    """
-    Processing function: calls pool of worker functions
-    to extract from a bam file two definitions of the edit distances to the reference genome scaled by read length
-    Returned in a pandas DataFrame
-    """
-    logging.info(f"Loading BAM file")
+    logging.info("Loading BAM file")
     save = pysam.set_verbosity(0)
-    samfile = pysam.AlignmentFile(bam, "rb")
+    samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
 
     references = samfile.references
 
     chr_lengths = []
     for chrom in samfile.references:
         chr_lengths.append(samfile.get_reference_length(chrom))
     max_chr_length = np.max(chr_lengths)
@@ -556,43 +759,91 @@
     if reference_lengths is not None:
         ref_lengths = pd.read_csv(
             reference_lengths, sep="\t", index_col=0, names=["reference", "length"]
         )
         # check if the dataframe contains all the References in the BAM file
         if not set(references).issubset(set(ref_lengths.index)):
             logging.error(
-                f"The BAM file contains references not found in the reference lengths file"
+                "The BAM file contains references not found in the reference lengths file"
             )
             sys.exit(1)
         max_chr_length = np.max(ref_lengths["length"].tolist())
 
     # Check if BAM files is not sorted by coordinates, sort it by coordinates
     if not samfile.header["HD"]["SO"] == "coordinate":
         log.info("BAM file is not sorted by coordinates, sorting it...")
         sorted_bam = bam.replace(".bam", ".bf-sorted.bam")
         pysam.sort("-@", str(threads), "-m", str(sort_memory), "-o", sorted_bam, bam)
         bam = sorted_bam
-        samfile = pysam.AlignmentFile(bam, "rb")
+        pysam.index("-c", "-@", str(threads), bam)
+        samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
 
     if not samfile.has_index():
         logging.info("BAM index not found. Indexing...")
         if max_chr_length > 536870912:
             logging.info("A reference is longer than 2^29, indexing with csi")
             pysam.index("-c", "-@", str(threads), bam)
         else:
             pysam.index(
                 "-@",
                 str(threads),
                 bam,
             )
+    logging.info("::: BAM file looks good.")
+
+    return bam  # Need to reload the samfile after creating index
+
+
+# Inspired from https://gigabaseorgigabyte.wordpress.com/2017/04/14/getting-the-edit-distance-from-a-bam-alignment-a-journey/
+def process_bam(
+    bam,
+    threads=1,
+    reference_lengths=None,
+    min_read_ani=90.0,
+    min_read_count=10,
+    trim_ends=0,
+    trim_min=10,
+    trim_max=90,
+    scale=1e6,
+    plot=False,
+    plots_dir="coverage-plots",
+    chunksize=None,
+    read_length_freqs=False,
+    output_files=None,
+    low_memory=False,
+    sort_memory="1G",
+):
+    """
+    Processing function: calls pool of worker functions
+    to extract from a bam file two definitions of the edit distances to the reference genome scaled by read length
+    Returned in a pandas DataFrame
+    """
+    logging.info("Loading BAM file")
+    save = pysam.set_verbosity(0)
+    samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
 
-        logging.info("Reloading BAM file")
-        samfile = pysam.AlignmentFile(
-            bam, "rb"
-        )  # Need to reload the samfile after creating index
+    references = samfile.references
+
+    # chr_lengths = []
+    # for chrom in samfile.references:
+    #     chr_lengths.append(samfile.get_reference_length(chrom))
+    pysam.set_verbosity(save)
+
+    ref_lengths = None
+    if reference_lengths is not None:
+        ref_lengths = pd.read_csv(
+            reference_lengths, sep="\t", index_col=0, names=["reference", "length"]
+        )
+        # check if the dataframe contains all the References in the BAM file
+        if not set(references).issubset(set(ref_lengths.index)):
+            logging.error(
+                "The BAM file contains references not found in the reference lengths file"
+            )
+            sys.exit(1)
+            sys.exit(1)
 
     total_refs = samfile.nreferences
     logging.info(f"Found {total_refs:,} reference sequences")
     # logging.info(f"Found {samfile.mapped:,} alignments")
     logging.info(
         f"Removing references without mappings or less than {min_read_count} reads..."
     )
@@ -602,245 +853,324 @@
     #     samfile.fetch(until_eof=True),
     #     total=samfile.mapped,
     #     leave=False,
     #     ncols=80,
     #     desc=f"Alignments processed",
     # ):
     #     alns_in_ref[aln.reference_name] += 1
-
     if plot:
         # Check if image folder exists
         if not os.path.exists(plots_dir):
             os.makedirs(plots_dir)
 
     references = [
         chrom.contig
         for chrom in samfile.get_index_statistics()
-        if chrom.mapped > min_read_count
+        if chrom.mapped >= min_read_count
     ]
 
     if len(references) == 0:
-        logging.error("No reference sequences with alignments found in the BAM file")
-        sys.exit(1)
+        logging.warning("No reference sequences with alignments found in the BAM file")
+        create_empty_output_files(output_files)
+        sys.exit(0)
 
     logging.info(f"Keeping {len(references):,} references")
 
+    if low_memory:
+        logging.info("Low memory mode enabled, writing filtered BAM file to disk")
+        samfile.close()
+        bam = write_bam(
+            bam=bam,
+            references=references,
+            output_files=output_files,
+            sort_memory=sort_memory,
+            threads=threads,
+        )
+        samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
+
     if (chunksize is not None) and ((len(references) // chunksize) > threads):
         c_size = chunksize
     else:
         c_size = calc_chunksize(
             n_workers=threads, len_iterable=len(references), factor=4
         )
-
     ref_chunks = [references[i : i + c_size] for i in range(0, len(references), c_size)]
     params = zip([bam] * len(ref_chunks), ref_chunks)
     try:
         logging.info(
             f"Processing {len(ref_chunks):,} chunks of {c_size:,} references each"
         )
         if is_debug():
             data = list(
                 map(
                     functools.partial(
                         get_bam_stats,
                         ref_lengths=ref_lengths,
                         min_read_ani=min_read_ani,
+                        trim_ends=0,
+                        trim_min=trim_min,
+                        trim_max=trim_max,
                         scale=scale,
                         plot=plot,
                         plots_dir=plots_dir,
+                        read_length_freqs=read_length_freqs,
+                        threads=threads,
                     ),
                     params,
                 )
             )
         else:
-
             p = Pool(
                 threads,
                 initializer=initializer,
                 initargs=([params, ref_lengths, scale],),
             )
 
             data = list(
                 tqdm.tqdm(
                     p.imap_unordered(
                         functools.partial(
                             get_bam_stats,
                             ref_lengths=ref_lengths,
                             min_read_ani=min_read_ani,
+                            trim_ends=0,
+                            trim_min=trim_min,
+                            trim_max=trim_max,
                             scale=scale,
                             plot=plot,
                             plots_dir=plots_dir,
+                            read_length_freqs=read_length_freqs,
+                            threads=threads,
                         ),
                         params,
                         chunksize=1,
                     ),
                     total=len(ref_chunks),
                     leave=False,
                     ncols=80,
-                    desc=f"References processed",
+                    desc="References processed",
                 )
             )
 
             p.close()
             p.join()
 
     except KeyboardInterrupt:
-        logging.info(f"User canceled the operation. Terminating jobs.")
+        logging.info("User canceled the operation. Terminating jobs.")
         p.terminate()
         p.join()
         sys.exit(0)
     return data
 
 
 def filter_reference_BAM(
     bam,
     df,
     filter_conditions,
     threads,
     out_files,
     sort_memory,
-    only_stats_filtered,
+    min_read_ani,
+    transform_cov_evenness=False,
     sort_by_name=False,
+    disable_sort=False,
 ):
     """Filter BAM based on certain conditions
 
     Args:
         bam (str): BAM file location
         data (pandas.DataFrame): Reference statistics
         filter_conditions (dict): A dictionary with the filter conditions to be used
         out_files (dict): Where to save the BAM files.
     """
     logging.info("Filtering stats...")
     if "min_norm_entropy" in filter_conditions and "min_norm_gini" in filter_conditions:
         logging.info(
-            f"min_read_count >= {filter_conditions['min_read_count']} & min_read_length >= {filter_conditions['min_read_length']} & min_avg_read_ani >= {filter_conditions['min_avg_read_ani']} & min_expected_breadth_ratio >= {filter_conditions['min_expected_breadth_ratio']} &  min_breadth >= {filter_conditions['min_breadth']} & min_coverage_evenness >= {filter_conditions['min_coverage_evenness']} & min_norm_entropy >= {filter_conditions['min_norm_entropy']} & min_norm_gini <= {filter_conditions['min_norm_gini']}"
+            f"::: min_read_count >= {filter_conditions['min_read_count']} "
+            f"& min_read_length >= {filter_conditions['min_read_length']} "
+            f"& min_avg_read_ani >= {filter_conditions['min_avg_read_ani']} "
+            f"& min_expected_breadth_ratio >= {filter_conditions['min_expected_breadth_ratio']} "
+            f"& min_breadth >= {filter_conditions['min_breadth']} "
+            f"& min_coverage_evenness >= {filter_conditions['min_coverage_evenness']} "
+            f"& min_coeff_var =< {filter_conditions['min_coeff_var']} "
+            f"& min_coverage_mean >= {filter_conditions['min_coverage_mean']} "
+            f"& min_norm_entropy >= {filter_conditions['min_norm_entropy']} "
+            f"& min_norm_gini <= {filter_conditions['min_norm_gini']}"
         )
+        # We transform the coverage_evenenness to 1.0 where the coverage is smaller than 1
+        if transform_cov_evenness is True:
+            df["cov_evenness_tmp"] = df["cov_evenness"]
+            df["cov_evenness_tmp"] = np.where(
+                np.rint(df.coverage_mean) < 1.0, 1.0, df.cov_evenness_tmp
+            )
+        else:
+            df["cov_evenness_tmp"] = df["cov_evenness"]
         df_filtered = df.loc[
             (df["n_reads"] >= filter_conditions["min_read_count"])
             & (df["read_length_mean"] >= filter_conditions["min_read_length"])
             & (df["read_ani_mean"] >= filter_conditions["min_avg_read_ani"])
             & (
                 df["breadth_exp_ratio"]
                 >= filter_conditions["min_expected_breadth_ratio"]
             )
             & (df["breadth"] >= filter_conditions["min_breadth"])
-            & (df["cov_evenness"] >= filter_conditions["min_coverage_evenness"])
+            & (df["cov_evenness_tmp"] >= filter_conditions["min_coverage_evenness"])
+            & (df["c_v"] <= filter_conditions["min_coeff_var"])
+            & (df["coverage_mean"] >= filter_conditions["min_coverage_mean"])
             & (df["norm_entropy"] >= filter_conditions["min_norm_entropy"])
             & (df["norm_gini"] <= filter_conditions["min_norm_gini"])
         ]
     else:
         logging.info(
-            f"min_read_count >= {filter_conditions['min_read_count']} & min_read_length >= {filter_conditions['min_read_length']} & min_avg_read_ani >= {filter_conditions['min_avg_read_ani']} & min_expected_breadth_ratio >= {filter_conditions['min_expected_breadth_ratio']} &  min_breadth >= {filter_conditions['min_breadth']} & min_coverage_evenness >= {filter_conditions['min_coverage_evenness']}"
+            f"::: min_read_count >= {filter_conditions['min_read_count']} "
+            f"& min_read_length >= {filter_conditions['min_read_length']} "
+            f"& min_avg_read_ani >= {filter_conditions['min_avg_read_ani']} "
+            f"& min_expected_breadth_ratio >= {filter_conditions['min_expected_breadth_ratio']} "
+            f"& min_breadth >= {filter_conditions['min_breadth']} "
+            f"& min_coverage_evenness >= {filter_conditions['min_coverage_evenness']} "
+            f"& min_coeff_var <= {filter_conditions['min_coeff_var']} "
+            f"& min_coverage_mean >= {filter_conditions['min_coverage_mean']}"
         )
+        if transform_cov_evenness is True:
+            df["cov_evenness_tmp"] = df["cov_evenness"]
+            df["cov_evenness_tmp"] = np.where(
+                np.rint(df.coverage_mean) < 1.0, 1.0, df.cov_evenness_tmp
+            )
+        else:
+            df["cov_evenness_tmp"] = df["cov_evenness"]
+
         df_filtered = df.loc[
             (df["n_reads"] >= filter_conditions["min_read_count"])
             & (df["read_length_mean"] >= filter_conditions["min_read_length"])
             & (df["read_ani_mean"] >= filter_conditions["min_avg_read_ani"])
             & (
                 df["breadth_exp_ratio"]
                 >= filter_conditions["min_expected_breadth_ratio"]
             )
             & (df["breadth"] >= filter_conditions["min_breadth"])
-            & (df["cov_evenness"] >= filter_conditions["min_coverage_evenness"])
+            & (df["cov_evenness_tmp"] >= filter_conditions["min_coverage_evenness"])
+            & (df["c_v"] <= filter_conditions["min_coeff_var"])
+            & (df["coverage_mean"] >= filter_conditions["min_coverage_mean"])
         ]
+
+    del df_filtered["cov_evenness_tmp"]
+    # prof = profile.Profile()
+    # prof.enable()
     if len(df_filtered.index) > 0:
-        logging.info(f"Saving filtered stats...")
+        # prof = profile.Profile()
+        # prof.enable()
+        logging.info("Saving filtered stats...")
         df_filtered.to_csv(
             out_files["stats_filtered"], sep="\t", index=False, compression="gzip"
         )
-        if only_stats_filtered:
-            logging.info("Skipping saving filtered BAM file.")
-        else:
+        if out_files["bam_filtered"] is not None:
             logging.info("Writing filtered BAM file... (be patient)")
             refs_dict = dict(
-                zip(df_filtered["reference"], df_filtered["reference_length"])
+                zip(df_filtered["reference"], df_filtered["bam_reference_length"])
             )
             (ref_names, ref_lengths) = zip(*refs_dict.items())
 
-            out_bam_file = pysam.Samfile(
+            refs_idx = {sys.intern(str(x)): i for i, x in enumerate(ref_names)}
+            if threads > 4:
+                write_threads = 4
+            else:
+                write_threads = threads
+
+            out_bam_file = pysam.AlignmentFile(
                 out_files["bam_filtered_tmp"],
                 "wb",
                 referencenames=list(ref_names),
                 referencelengths=list(ref_lengths),
-                threads=threads,
+                threads=write_threads,
             )
-            header = pysam.AlignmentHeader.from_references(
-                list(ref_names), list(ref_lengths)
-            )
-            references = df_filtered["reference"].values
 
-            logging.info("Filtering BAM file...")
-            samfile = pysam.AlignmentFile(bam, "rb")
+            samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
+            references = [x for x in samfile.references if x in refs_idx.keys()]
+
+            logging.info(
+                f"::: Filtering {len(references):,} references sequentially..."
+            )
             for reference in tqdm.tqdm(
                 references,
                 total=len(references),
                 leave=False,
                 ncols=80,
                 desc="References processed",
             ):
                 for aln in samfile.fetch(
                     reference=reference, multiple_iterators=False, until_eof=True
                 ):
-                    out_bam_file.write(
-                        pysam.AlignedSegment.fromstring(aln.to_string(), header=header)
-                    )
+                    ani_read = (
+                        1 - ((aln.get_tag("NM") / aln.infer_query_length()))
+                    ) * 100
+                    if ani_read >= min_read_ani:
+                        aln.reference_id = refs_idx[aln.reference_name]
+                        out_bam_file.write(aln)
             out_bam_file.close()
-            if sort_by_name:
-                logging.info("Sorting BAM file by read name...")
-                pysam.sort(
-                    "-n",
-                    "-@",
-                    str(threads),
-                    "-m",
-                    str(sort_memory),
-                    "-o",
-                    out_files["bam_filtered"],
-                    out_files["bam_filtered_tmp"],
-                )
-            else:
-                pysam.sort(
-                    "-@",
-                    str(threads),
-                    "-m",
-                    str(sort_memory),
-                    "-o",
-                    out_files["bam_filtered"],
-                    out_files["bam_filtered_tmp"],
-                )
-
-                save = pysam.set_verbosity(0)
-                samfile = pysam.AlignmentFile(out_files["bam_filtered"], "rb")
-                chr_lengths = []
-                for chrom in samfile.references:
-                    chr_lengths.append(samfile.get_reference_length(chrom))
-                max_chr_length = np.max(chr_lengths)
-                pysam.set_verbosity(save)
-                samfile.close()
-
-                logging.info("BAM index not found. Indexing...")
-                if max_chr_length > 536870912:
-                    logging.info("A reference is longer than 2^29, indexing with csi")
-                    pysam.index(
-                        out_files["bam_filtered"],
-                        "-c",
+            # prof.disable()
+            # # print profiling output
+            # stats = pstats.Stats(prof).strip_dirs().sort_stats("tottime")
+            # stats.print_stats(5)  # top 10 rows
+            if not disable_sort:
+                if sort_by_name:
+                    logging.info("Sorting BAM file by read name...")
+                    pysam.sort(
+                        "-n",
                         "-@",
                         str(threads),
+                        "-m",
+                        str(sort_memory),
+                        "-o",
+                        out_files["bam_filtered"],
+                        out_files["bam_filtered_tmp"],
                     )
                 else:
-                    pysam.index(
-                        out_files["bam_filtered"],
+                    pysam.sort(
                         "-@",
                         str(threads),
+                        "-m",
+                        str(sort_memory),
+                        "-o",
+                        out_files["bam_filtered"],
+                        out_files["bam_filtered_tmp"],
                     )
 
-            os.remove(out_files["bam_filtered_tmp"])
-    else:
-        logging.info("No references meet the filter conditions. Skipping...")
-
+                    logging.info("BAM index not found. Indexing...")
+                    save = pysam.set_verbosity(0)
+                    samfile = pysam.AlignmentFile(
+                        out_files["bam_filtered"], "rb", threads=threads
+                    )
+                    chr_lengths = []
+                    for chrom in samfile.references:
+                        chr_lengths.append(samfile.get_reference_length(chrom))
+                    max_chr_length = np.max(chr_lengths)
+                    pysam.set_verbosity(save)
+                    samfile.close()
+
+                    if max_chr_length > 536870912:
+                        logging.info(
+                            "A reference is longer than 2^29, indexing with csi"
+                        )
+                        pysam.index(
+                            "-c",
+                            "-@",
+                            str(threads),
+                            out_files["bam_filtered"],
+                        )
+                    else:
+                        pysam.index(
+                            "-@",
+                            str(threads),
+                            out_files["bam_filtered"],
+                        )
 
-def get_alns(params):
-    bam, reference = params
-    samfile = pysam.AlignmentFile(bam, "rb")
-    alns = []
-    for aln in samfile.fetch(reference=reference, multiple_iterators=False):
-        alns.append(aln.to_string())
-    return alns
+                os.remove(out_files["bam_filtered_tmp"])
+            else:
+                logging.info("Skipping BAM file sorting...")
+                os.rename(out_files["bam_filtered_tmp"], out_files["bam_filtered"])
+        else:
+            logging.info("Skipping filtering BAM file creation...")
+    else:
+        logging.info("No references meet the filter conditions.")
+        # Path(out_files["bam_filtered"]).touch()
+        create_empty_bam(out_files["bam_filtered"])
+        Path(out_files["stats_filtered"]).touch()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bam-filter-1.1.9/bam_filter/utils.py` & `bam-filter-1.2.1/bam_filter/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,26 +9,52 @@
 from functools import partial
 from contextlib import contextmanager, redirect_stderr, redirect_stdout
 from os import devnull
 import tqdm
 from bam_filter import __version__
 import time
 from itertools import chain
+import numpy as np
+from pathlib import Path
+import pysam
 
 log = logging.getLogger("my_logger")
 log.setLevel(logging.INFO)
 timestr = time.strftime("%Y%m%d-%H%M%S")
 
 
 def is_debug():
     return logging.getLogger("my_logger").getEffectiveLevel() == logging.DEBUG
 
 
-def check_values(val, minval, maxval, parser, var):
+def create_empty_output_files(out_files):
+    for key, value in out_files.items():
+        if value is not None:
+            if key == "bam_filtered":
+                create_empty_bam(value)
+            elif (
+                key == "bam_filtered_tmp" or key == "bam_tmp" or key == "bam_tmp_sorted"
+            ):
+                continue
+            else:
+                Path(value).touch()
+
+
+# function that creates an empty bam file
+def create_empty_bam(output):
+    """
+    Create an empty bam file
+    """
+    header = {"HD": {"VN": "1.0", "SO": "unsorted"}}
+    # Create an empty BAM file with the specified header
+    with pysam.AlignmentFile(output, "wb", header=header) as outfile:
+        pass
+
 
+def check_values(val, minval, maxval, parser, var):
     try:
         value = float(val)
     except ValueError:
         parser.error(
             f"argument {var}: Invalid value {val}. Value has to be a 'float' between {minval} and {maxval}!"
         )
     value = float(val)
@@ -134,251 +160,424 @@
         parser.error("argument %s: The file %s does not exist!" % (var, arg))
     else:
         return arg
 
 
 defaults = {
     "min_read_length": 30,
-    "min_read_count": 10,
-    "min_expected_breadth_ratio": 0.5,
-    "min_norm_entropy": "auto",
-    "min_norm_gini": None,
+    "min_read_count": 3,
+    "min_expected_breadth_ratio": 0,
+    "min_norm_entropy": 0,
+    "min_norm_gini": 1.0,
     "min_avg_read_ani": 90.0,
     "min_read_ani": 90.0,
     "min_breadth": 0,
     "min_coverage_evenness": 0,
+    "min_coeff_var": np.Inf,
+    "min_coverage_mean": 0,
     "prefix": None,
     "sort_memory": "1G",
     "reference_lengths": None,
     "scale": 1e6,
     "chunk_size": None,
-    "plot": False,
+    "coverage_plots": None,
+    "stats": None,
+    "stats_filtered": None,
+    "bam_filtered": None,
+    "knee_plot": None,
+    "read_length_freqs": None,
+    "read_hits_count": None,
+    "tmp_dir": None,
 }
 
 help_msg = {
     "bam": "BAM file containing aligned reads",
     "threads": "Number of threads to use",
     "prefix": "Prefix used for the output files",
     "min_read_length": "Minimum read length",
     "min_read_count": "Minimum read count",
+    "trim_ends": "Exclude n bases at the ends of the reference sequences",
+    "trim_min": "Remove coverage that are below this percentile. Used for the Truncated Average Depth (TAD) calculation",
+    "trim_max": "Remove coverage that are above this percentile. Used for the Truncated Average Depth (TAD) calculation",
     "min_breadth": "Minimum breadth",
     "min_expected_breadth_ratio": "Minimum expected breadth ratio",
     "min_norm_entropy": "Minimum normalized entropy",
     "min_norm_gini": "Minimum normalized Gini coefficient",
     "min_read_ani": "Minimum read ANI to keep a read",
     "min_avg_read_ani": "Minimum average read ANI",
     "min_coverage_evenness": "Minimum coverage evenness",
+    "min_coeff_var": "Minimum coverage evenness calculated as SD/MEAN",
+    "min_coverage_mean": "Minimum coverage mean",
+    "transform_cov_evenness": "Include those references that fullfi all filtering criteria but the coverage evenness is 0",
     "sort_memory": "Set maximum memory per thread for sorting; suffix K/M/G recognized",
     "scale": "Scale taxonomic abundance by this factor; suffix K/M recognized",
     "read_length_freqs": "Save a JSON file with the read length frequencies mapped to each reference",
-    "only_stats": "Only produce statistics and skip filtering",
-    "only_stats_filtered": "Only filter statistics and skip BAM filtering",
-    "plot": "Plot genome coverage plots",
+    "read_hits_count": "Save a TSV file with the read hits frequencies mapped to each reference",
+    "stats": "Save a TSV file with the statistics for each reference",
+    "stats_filtered": "Save a TSV file with the statistics for each reference after filtering",
+    "bam_filtered": "Save a BAM file with the references that passed the filtering criteria",
+    "coverage_plots": "Folder where to save genome coverage plots",
+    "knee_plot": "Plot knee plot",
     "sort_by_name": "Sort by read names",
+    "disable_sort": "Disable sorting of the filtered BAM file",
     "chunk_size": "Chunk size for parallel processing",
+    "tmp_dir": "Temporary directory",
     "help": "Help message",
     "debug": "Print debug messages",
     "reference_lengths": "File with references lengths",
+    "low_memory": "Activate the low memory mode",
     "version": "Print program version",
 }
 
 
 def get_arguments(argv=None):
     parser = argparse.ArgumentParser(
         description="A simple tool to calculate metrics from a BAM file and filter with uneven coverage.",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument(
-        "bam",
+    # add subparser for filtering options:
+    filter_args = parser.add_argument_group("filtering arguments")
+    misc_args = parser.add_argument_group("miscellaneous arguments")
+    out_args = parser.add_argument_group("output arguments")
+    parser.add_argument(
+        "--bam",
+        required=True,
+        dest="bam",
         type=lambda x: is_valid_file(parser, x, "bam"),
         help=help_msg["bam"],
     )
     parser.add_argument(
         "-t",
         "--threads",
         type=lambda x: int(
             check_values(x, minval=1, maxval=1000, parser=parser, var="--threads")
         ),
         dest="threads",
+        metavar="INT",
         default=1,
         help=help_msg["threads"],
     )
+    misc_args.add_argument(
+        "--reference-trim-length",
+        type=lambda x: int(
+            check_values(
+                x, minval=0, maxval=10000, parser=parser, var="---reference-trim-length"
+            )
+        ),
+        dest="trim_ends",
+        metavar="INT",
+        default=0,
+        help=help_msg["trim_ends"],
+    )
+    misc_args.add_argument(
+        "--trim-min",
+        type=lambda x: int(
+            check_values(x, minval=0, maxval=100, parser=parser, var="--trim-min")
+        ),
+        dest="trim_min",
+        metavar="INT",
+        default=10,
+        help=help_msg["trim_min"],
+    )
+    misc_args.add_argument(
+        "--trim-max",
+        type=lambda x: int(
+            check_values(x, minval=0, maxval=100, parser=parser, var="--trim-max")
+        ),
+        dest="trim_max",
+        metavar="INT",
+        default=90,
+        help=help_msg["trim_max"],
+    )
     parser.add_argument(
         "-p",
         "--prefix",
         type=str,
         default=defaults["prefix"],
+        metavar="STR",
         dest="prefix",
         help=help_msg["prefix"],
     )
-    parser.add_argument(
+    filter_args.add_argument(
         "-A",
         "--min-read-ani",
         type=lambda x: float(
             check_values(x, minval=0, maxval=100, parser=parser, var="--min-read-ani")
         ),
+        metavar="FLOAT",
         default=defaults["min_read_ani"],
         dest="min_read_ani",
         help=help_msg["min_read_ani"],
     )
-    parser.add_argument(
+    filter_args.add_argument(
         "-l",
         "--min-read-length",
         type=lambda x: int(
             check_values(
                 x, minval=1, maxval=100000, parser=parser, var="--min-read-length"
             )
         ),
         default=defaults["min_read_length"],
+        metavar="INT",
         dest="min_read_length",
         help=help_msg["min_read_length"],
     )
-    parser.add_argument(
+    filter_args.add_argument(
         "-n",
         "--min-read-count",
         type=lambda x: int(
             check_values(
-                x, minval=1, maxval=100000, parser=parser, var="--min-read-count"
+                x, minval=1, maxval=np.Inf, parser=parser, var="--min-read-count"
             )
         ),
         default=defaults["min_read_count"],
+        metavar="INT",
         dest="min_read_count",
         help=help_msg["min_read_count"],
     )
-    parser.add_argument(
+    filter_args.add_argument(
         "-b",
         "--min-expected-breadth-ratio",
         type=lambda x: float(
             check_values(
                 x, minval=0, maxval=1, parser=parser, var="--min-expected-breadth-ratio"
             )
         ),
+        metavar="FLOAT",
         default=defaults["min_expected_breadth_ratio"],
         dest="min_expected_breadth_ratio",
         help=help_msg["min_expected_breadth_ratio"],
     )
-    parser.add_argument(
+    filter_args.add_argument(
         "-e",
         "--min-normalized-entropy",
         type=lambda x: check_values_auto(
             x, minval=0, maxval=1, parser=parser, var="--min-normalized-entropy"
         ),
         default=defaults["min_norm_entropy"],
+        metavar="FLOAT",
         dest="min_norm_entropy",
         help=help_msg["min_norm_entropy"],
     )
-    parser.add_argument(
+    filter_args.add_argument(
         "-g",
         "--min-normalized-gini",
         type=lambda x: check_values_auto(
             x, minval=0, maxval=1, parser=parser, var="--min-normalized-gini"
         ),
         default=defaults["min_norm_gini"],
+        metavar="FLOAT",
         dest="min_norm_gini",
         help=help_msg["min_norm_gini"],
     )
-    parser.add_argument(
+    filter_args.add_argument(
         "-B",
         "--min-breadth",
         type=lambda x: float(
             check_values(x, minval=0, maxval=1, parser=parser, var="--min-breadth")
         ),
         default=defaults["min_breadth"],
+        metavar="FLOAT",
         dest="min_breadth",
         help=help_msg["min_breadth"],
     )
-    parser.add_argument(
+    filter_args.add_argument(
         "-a",
         "--min-avg-read-ani",
         type=lambda x: float(
             check_values(
                 x, minval=0, maxval=100, parser=parser, var="--min-avg-read-ani"
             )
         ),
+        metavar="FLOAT",
         default=defaults["min_avg_read_ani"],
         dest="min_avg_read_ani",
         help=help_msg["min_avg_read_ani"],
     )
-    parser.add_argument(
+    filter_args.add_argument(
         "-c",
         "--min-coverage-evenness",
         type=lambda x: float(
             check_values(
                 x, minval=0, maxval=1, parser=parser, var="--min-coverage-evenness"
             )
         ),
+        metavar="FLOAT",
         default=defaults["min_coverage_evenness"],
         dest="min_coverage_evenness",
         help=help_msg["min_coverage_evenness"],
     )
+    filter_args.add_argument(
+        "-V",
+        "--min-coeff-var",
+        type=lambda x: float(
+            check_values(
+                x, minval=0, maxval=np.Inf, parser=parser, var="--min-evenness"
+            )
+        ),
+        default=defaults["min_coeff_var"],
+        metavar="FLOAT",
+        dest="min_coeff_var",
+        help=help_msg["min_coeff_var"],
+    )
+    filter_args.add_argument(
+        "-C",
+        "--min-coverage-mean",
+        type=lambda x: float(
+            check_values(
+                x, minval=0, maxval=1000000, parser=parser, var="--min-coverage-mean"
+            )
+        ),
+        default=defaults["min_coverage_mean"],
+        metavar="FLOAT",
+        dest="min_coverage_mean",
+        help=help_msg["min_coverage_mean"],
+    )
+    filter_args.add_argument(
+        "--include-low-detection",
+        dest="transform_cov_evenness",
+        action="store_true",
+        help=help_msg["transform_cov_evenness"],
+    )
     parser.add_argument(
         "-m",
         "--sort-memory",
         type=lambda x: check_suffix(x, parser=parser, var="--sort-memory"),
         default=defaults["sort_memory"],
+        metavar="STR",
         dest="sort_memory",
         help=help_msg["sort_memory"],
     )
     parser.add_argument(
         "-N",
         "--sort-by-name",
         dest="sort_by_name",
         action="store_true",
         help=help_msg["sort_by_name"],
     )
     parser.add_argument(
+        "--disable-sort",
+        dest="disable_sort",
+        action="store_true",
+        help=help_msg["disable_sort"],
+    )
+    parser.add_argument(
         "--scale",
         type=lambda x: check_suffix(x, parser=parser, var="--scale"),
         default=defaults["scale"],
         dest="scale",
+        metavar="STR",
         help=help_msg["scale"],
     )
     # reference_lengths
     parser.add_argument(
         "-r",
         "--reference-lengths",
         type=lambda x: is_valid_file(parser, x, "reference_lengths"),
+        metavar="FILE",
         default=defaults["reference_lengths"],
         dest="reference_lengths",
         help=help_msg["reference_lengths"],
     )
-    parser.add_argument(
+    out_args.add_argument(
+        "--stats",
+        dest="stats",
+        default=defaults["stats"],
+        type=str,
+        metavar="FILE",
+        nargs="?",
+        const="",
+        required=True,
+        help=help_msg["stats"],
+    )
+    out_args.add_argument(
+        "--stats-filtered",
+        dest="stats_filtered",
+        default=defaults["stats_filtered"],
+        type=str,
+        metavar="FILE",
+        nargs="?",
+        const="",
+        help=help_msg["stats_filtered"],
+    )
+    out_args.add_argument(
+        "--bam-filtered",
+        dest="bam_filtered",
+        default=defaults["bam_filtered"],
+        metavar="FILE",
+        type=str,
+        nargs="?",
+        const="",
+        help=help_msg["bam_filtered"],
+    )
+    out_args.add_argument(
         "--read-length-freqs",
         dest="read_length_freqs",
-        action="store_true",
+        default=defaults["read_length_freqs"],
+        metavar="FILE",
+        type=str,
+        nargs="?",
+        const="",
         help=help_msg["read_length_freqs"],
     )
-    parser.add_argument(
-        "--only-stats",
-        dest="only_stats",
-        action="store_true",
-        help=help_msg["only_stats"],
-    )
-    parser.add_argument(
-        "--plot",
-        dest="plot",
-        action="store_true",
-        help=help_msg["plot"],
-    )
-    parser.add_argument(
-        "--only-stats-filtered",
-        dest="only_stats_filtered",
-        action="store_true",
-        help=help_msg["only_stats_filtered"],
+    out_args.add_argument(
+        "--read-hits-count",
+        dest="read_hits_count",
+        default=defaults["read_hits_count"],
+        metavar="FILE",
+        type=str,
+        nargs="?",
+        const="",
+        help=help_msg["read_hits_count"],
+    )
+    out_args.add_argument(
+        "--knee-plot",
+        dest="knee_plot",
+        default=defaults["knee_plot"],
+        metavar="FILE",
+        type=str,
+        nargs="?",
+        const="",
+        help=help_msg["knee_plot"],
+    )
+    out_args.add_argument(
+        "--coverage-plots",
+        dest="coverage_plots",
+        metavar="FILE",
+        default=defaults["coverage_plots"],
+        type=str,
+        nargs="?",
+        const="",
+        help=help_msg["coverage_plots"],
     )
     parser.add_argument(
         "--chunk-size",
         type=lambda x: int(
             check_values(x, minval=1, maxval=100000, parser=parser, var="--chunk-size")
         ),
         default=defaults["chunk_size"],
+        metavar="INT",
         dest="chunk_size",
         help=help_msg["chunk_size"],
     )
     parser.add_argument(
+        "--tmp-dir",
+        type=str,
+        default=defaults["tmp_dir"],
+        metavar="DIR",
+        dest="tmp_dir",
+        help=help_msg["tmp_dir"],
+    )
+    parser.add_argument(
+        "--low-memory",
+        dest="low_memory",
+        action="store_true",
+        help=help_msg["low_memory"],
+    )
+    parser.add_argument(
         "--debug", dest="debug", action="store_true", help=help_msg["debug"]
     )
     parser.add_argument(
         "--version",
         action="version",
         version="%(prog)s " + __version__,
         help=help_msg["version"],
@@ -423,77 +622,17 @@
 
 
 def initializer(init_data):
     global parms
     parms = init_data
 
 
-def do_parallel(parms, lst, func, threads):
-    if is_debug():
-        dfs = list(map(partial(func, parms=parms), lst))
-    else:
-        p = Pool(threads, initializer=initializer, initargs=(parms,))
-        c_size = calc_chunksize(threads, len(lst))
-        dfs = list(
-            tqdm.tqdm(
-                p.imap_unordered(
-                    partial(func, parms=parms),
-                    lst,
-                    chunksize=c_size,
-                ),
-                total=len(lst),
-                leave=False,
-                ncols=80,
-                desc=f"Components processed",
-            )
-        )
-        p.close()
-        p.join()
-    return concat_df(dfs)
-
-
-def do_parallel_lst(parms, lst, func, threads):
-    if is_debug():
-        lst = list(map(partial(func, parms=parms), lst))
-    else:
-        p = Pool(threads, initializer=initializer, initargs=(parms,))
-        c_size = calc_chunksize(threads, len(lst))
-        lst = list(
-            tqdm.tqdm(
-                p.imap_unordered(
-                    partial(func, parms=parms),
-                    lst,
-                    chunksize=c_size,
-                ),
-                total=len(lst),
-                leave=False,
-                ncols=80,
-                desc=f"Components processed",
-            )
-        )
-
-    return lst
-
-
-def get_components_large(parms, components, func, threads):
-    dfs = list(
-        tqdm.tqdm(
-            map(partial(func, parms=parms), components),
-            total=len(components),
-            leave=False,
-            ncols=80,
-            desc=f"Components processed",
-        )
-    )
-    return concat_df(dfs)
-
-
 def clean_up(keep, temp_dir):
     if keep:
-        logging.info(f"Cleaning up temporary files")
+        logging.info("Cleaning up temporary files")
         logging.shutdown()
         shutil.rmtree(temp_dir, ignore_errors=True)
 
 
 # from https://stackoverflow.com/questions/53751050/python-multiprocessing-understanding-logic-behind-chunksize/54032744#54032744
 def calc_chunksize(n_workers, len_iterable, factor=4):
     """Calculate chunksize argument for Pool-methods.
@@ -502,21 +641,116 @@
     """
     chunksize, extra = divmod(len_iterable, n_workers * factor)
     if extra:
         chunksize += 1
     return chunksize
 
 
-def create_output_files(prefix, bam):
+# def create_output_files(
+#     prefix,
+#     bam,
+#     stats,
+#     stats_filtered,
+#     bam_filtered,
+#     read_length_freqs,
+#     read_hits_count,
+#     knee_plot,
+#     coverage_plots,
+# ):
+#     if prefix is None:
+#         prefix = bam.replace(".bam", "")
+
+#     out_files = {}
+#     if stats is not None:
+#         if stats == "":
+#             out_files["stats"] = f"{prefix}_stats.tsv.gz"
+#         else:
+#             out_files["stats"] = stats
+#     if stats_filtered is not None:
+#         if stats_filtered == "":
+#             out_files["stats_filtered"] = f"{prefix}_stats-filtered.tsv.gz"
+#         else:
+#             out_files["stats_filtered"] = stats_filtered
+#     if bam_filtered is not None:
+#         if bam_filtered == "":
+#             out_files["bam_filtered"] = f"{prefix}.filtered.bam"
+#         else:
+#             out_files["bam_filtered"] = bam_filtered
+#     if read_length_freqs is not None:
+#         if read_length_freqs == "":
+#             out_files["read_length_freqs"] = f"{prefix}_read-length-freqs.json"
+#         else:
+#             out_files["read_length_freqs"] = read_length_freqs
+#     if read_hits_count is not None:
+#         if read_hits_count == "":
+#             out_files["read_hits_count"] = f"{prefix}_read-hits-count.tsv.gz"
+#         else:
+#             out_files["read_hits_count"] = read_hits_count
+#     if knee_plot is not None:
+#         if knee_plot == "":
+#             out_files["knee_plot"] = f"{prefix}_knee-plot.png"
+#         else:
+#             out_files["knee_plot"] = knee_plot
+#     if coverage_plots is not None:
+#         if coverage_plots == "":
+#             out_files["coverage_plot_dir"] = f"{prefix}_coverage-plots"
+#         else:
+#             out_files["coverage_plot_dir"] = coverage_plots
+#     out_files["bam_filtered_tmp"] = (f"{prefix}.filtered.tmp.bam",)
+
+
+#     # create output files
+#     out_files = {
+#         "stats": stats,
+#         "stats_filtered": stats_filtered,
+#         "bam_filtered_tmp": f"{prefix}.filtered.tmp.bam",
+#         "bam_filtered": bam_filtered,
+#         "read_length_freqs": read_length_freqs,
+#         "read_hits_count": read_hits_count,
+#         "knee_plot": knee_plot,
+#         "coverage_plot_dir": coverage_plots,
+#     }
+#     return out_files
+def create_output_files(
+    prefix,
+    bam,
+    stats,
+    stats_filtered,
+    bam_filtered,
+    read_length_freqs,
+    read_hits_count,
+    knee_plot,
+    coverage_plots,
+    tmp_dir,
+):
     if prefix is None:
-        prefix = bam.replace(".bam", "")
+        prefix = Path(bam).with_suffix("").name
+
+    if stats == "":
+        stats = f"{prefix}_stats.tsv.gz"
+    if stats_filtered == "":
+        stats_filtered = f"{prefix}_stats-filtered.tsv.gz"
+    if bam_filtered == "":
+        bam_filtered = f"{prefix}.filtered.bam"
+    if read_length_freqs == "":
+        read_length_freqs = f"{prefix}_read-length-freqs.json"
+    if read_hits_count == "":
+        read_hits_count = f"{prefix}_read-hits-count.tsv.gz"
+    if knee_plot == "":
+        knee_plot = f"{prefix}_knee-plot.png"
+    if coverage_plots == "":
+        coverage_plots = f"{prefix}_coverage-plots"
+
     # create output files
     out_files = {
-        "stats": f"{prefix}_stats.tsv.gz",
-        "stats_filtered": f"{prefix}_stats-filtered.tsv.gz",
-        "bam_filtered_tmp": f"{prefix}.filtered.tmp.bam",
-        "bam_filtered": f"{prefix}.filtered.bam",
-        "read_length_freqs": f"{prefix}_read-length-freqs.json",
-        "knee_plot": f"{prefix}_knee-plot.png",
-        "coverage_plot_dir": f"{prefix}_coverage-plots",
+        "stats": stats,
+        "stats_filtered": stats_filtered,
+        "bam_filtered_tmp": f"{tmp_dir.name}/{prefix}.filtered.tmp.bam",
+        "bam_tmp": f"{tmp_dir.name}/{prefix}.tmp.bam",
+        "bam_tmp_sorted": f"{tmp_dir.name}/{prefix}.tmp.sorted.bam",
+        "bam_filtered": bam_filtered,
+        "read_length_freqs": read_length_freqs,
+        "read_hits_count": read_hits_count,
+        "knee_plot": knee_plot,
+        "coverage_plot_dir": coverage_plots,
     }
     return out_files
```

### Comparing `bam-filter-1.1.9/setup.cfg` & `bam-filter-1.2.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [flake8]
-max-line-length = 100
-ignore = E122,E123,E126,E127,E128,E731,E722
+max-line-length = 1000
+ignore = E122,E123,E126,E127,E128,E731,E722,E203,W503
 exclude = build,bam_filter/_version.py,tests,conda.recipe,.git,versioneer.py,benchmarks,.asv
 
 [tool:pytest]
 norecursedirs = .* *.egg* build dist conda.recipe
 addopts = 
 	--junitxml=junit.xml
 	--ignore setup.py
```

### Comparing `bam-filter-1.1.9/setup.py` & `bam-filter-1.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 requirements = [
     "Cython>=0.29.24",
     "pandas>=1.3.3",
     "scipy>=1.9.0",
     "tqdm>=4.64.1",
     "pysam>=0.17.0",
-    "numpy>=1.21.2",
+    "numpy>1.24",
     "pyrle>=0.0.31",
-    "sorted-nearest<=0.0.33",
-    "pyranges>=0.0.112",
+    "sorted-nearest>=0.0.38",
+    "pyranges>=0.0.118",
     "kneed>=0.8.1",
     "matplotlib>=3.6.0",
 ]
 
 setup(
     setup_requires=[
         # Setuptools 18.0 properly handles Cython extensions.
```

### Comparing `bam-filter-1.1.9/versioneer.py` & `bam-filter-1.2.1/versioneer.py`

 * *Files identical despite different names*

