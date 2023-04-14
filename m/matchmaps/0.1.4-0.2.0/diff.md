# Comparing `tmp/matchmaps-0.1.4.tar.gz` & `tmp/matchmaps-0.2.0.tar.gz`

## Comparing `matchmaps-0.1.4.tar` & `matchmaps-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github_changelog_generator
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.1.4/setup.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.1.4/tox.ini
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/workflows/cron.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/Makefile
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/cli.rst
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/conf.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/index.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/make.bat
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/_static/custom.css
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.1.4/src/matchmaps/__init__.py
--rwxr-xr-x   0        0        0    11679 2020-02-02 00:00:00.000000 matchmaps-0.1.4/src/matchmaps/_compute_realspace_diff.py
--rw-r--r--   0        0        0    17638 2020-02-02 00:00:00.000000 matchmaps-0.1.4/src/matchmaps/_utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.1.4/tests/test_matchmaps.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.1.4/LICENSE
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.1.4/README.md
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 matchmaps-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 matchmaps-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github_changelog_generator
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.2.0/setup.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.2.0/tox.ini
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/about.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/cli.md
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/index.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.2.0/docs/_static/custom.css
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.2.0/src/matchmaps/__init__.py
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 matchmaps-0.2.0/src/matchmaps/_compute_ncs_diff.py
+-rwxr-xr-x   0        0        0    11908 2020-02-02 00:00:00.000000 matchmaps-0.2.0/src/matchmaps/_compute_realspace_diff.py
+-rw-r--r--   0        0        0    20103 2020-02-02 00:00:00.000000 matchmaps-0.2.0/src/matchmaps/_utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.2.0/tests/test_matchmaps.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 matchmaps-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.2.0/LICENSE
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.2.0/README.md
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 matchmaps-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 matchmaps-0.2.0/PKG-INFO
```

### Comparing `matchmaps-0.1.4/.pre-commit-config.yaml` & `matchmaps-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/setup.py` & `matchmaps-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/tox.ini` & `matchmaps-0.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/.github/workflows/build_docs.yml` & `matchmaps-0.2.0/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/.github/workflows/ci.yml` & `matchmaps-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/.github/workflows/cron.yml` & `matchmaps-0.2.0/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/docs/Makefile` & `matchmaps-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/docs/conf.py` & `matchmaps-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/docs/index.md` & `matchmaps-0.2.0/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 /path/to/ccp4/start
 ```
 
 At this point, you should be good to go! Please [file an issue on github](https://github.com/dennisbrookner/matchmaps/issues) is this is not working.
 
 ## Using matchmaps
 
-Read about [using `matchmaps` in the command-line](cli.rst)
+Read about [using `matchmaps` in the command-line](cli.md)
 
 ```{eval-rst}
 .. toctree::
    :maxdepth: 1
    :hidden:
 
    Command-line usage <cli>
+   About the algorithm <about>
 ```
```

### Comparing `matchmaps-0.1.4/docs/make.bat` & `matchmaps-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/src/matchmaps/_compute_realspace_diff.py` & `matchmaps-0.2.0/src/matchmaps/_compute_realspace_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,16 @@
         description=(
             "Compute a real-space difference map. "
             "You will need two MTZ files, which will be referred to throughout as 'on' and 'off', "
             "though they could also be light/dark, bound/apo, mutant/WT, hot/cold, etc. "
             "Each mtz will need to contain structure factor amplitudes and uncertainties; you will not need any phases. "
             "You will, however, need an input model (assumed to correspond with the 'off' state) which will be used to determine phases. "
             "Please note that both ccp4 and phenix must be installed and active in your environment for this function to run. "
+            ""
+            "If you'd like to make an internal difference map instead, see matchmaps.ncs "
         )
     )
 
     parser.add_argument(
         "--mtzoff",
         "-f",
         nargs=3,
@@ -339,14 +341,17 @@
 def main():
     parser = parse_arguments()
     args = parser.parse_args()
 
     if not os.path.exists(args.output_dir):
         os.makedirs(args.output_dir)
 
+    if not os.path.exists(args.input_dir):
+        raise ValueError(f"Input directory '{args.input_dir}' does not exist")
+
     compute_realspace_difference_map(
         pdboff=args.pdboff,
         ligands=args.ligands,
         mtzoff=args.mtzoff[0],
         mtzon=args.mtzon[0],
         Foff=args.mtzoff[1],
         SigFoff=args.mtzoff[2],
```

### Comparing `matchmaps-0.1.4/src/matchmaps/_utils.py` & `matchmaps-0.2.0/src/matchmaps/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,17 +92,17 @@
     Parameters
     ----------
     mtz : rs.DataSet
         mtz data to be transformed into real space
     spacing : float
         Approximate voxel size desired (will be rounded as necessary to create integer grid dimensions)
     F : str, optional
-        Column in mtz containing structure factor amplitudes to use for calculation, by default "2FOFCWT"
+        Column in mtz containing structure factor amplitudes to use for calculation
     Phi : str, optional
-        Column in mtz containing phases to be used for calculation, by default "PH2FOFCWT"
+        Column in mtz containing phases to be used for calculation
     spacegroup : str, optional
         Spacegroup for the output FloatGrid. Defaults to P1.
     dmin: float, optional
         Highest resolution reflections to include in Fourier transform. Defaults to None, no cutoff.
 
     Returns
     -------
@@ -463,32 +463,15 @@
 
     masker.put_mask_on_float_grid(fg_mask_only, pdb_for_mask)
     masked_difference_array = np.logical_not(fg_mask_only.array) * difference_array
 
     # and finally, write stuff out
 
     # coot refuses to render periodic boundaries for P1 maps with alpha=beta=gamma=90, sooooo
-    if all(
-        [
-            angle == 90
-            for angle in (
-                fg_fixed.unit_cell.alpha,
-                fg_fixed.unit_cell.beta,
-                fg_fixed.unit_cell.gamma,
-            )
-        ]
-    ):
-        fg_fixed.unit_cell = gemmi.UnitCell(
-            fg_fixed.unit_cell.a,
-            fg_fixed.unit_cell.b,
-            fg_fixed.unit_cell.c,
-            90.006,
-            fg_fixed.unit_cell.beta,
-            fg_fixed.unit_cell.gamma,
-        )
+    fg_fixed.unit_cell = _unit_cell_hack(fg_fixed.unit_cell)
 
     # use partial function to guarantee I'm always using the same and correct cell
     write_maps = partial(
         rs.io.write_ccp4_map, cell=fg_fixed.unit_cell, spacegroup=fg_fixed.spacegroup
     )
 
     write_maps(fg_on.array, f"{output_dir}/{on_name}.map")
@@ -499,14 +482,53 @@
     write_maps(
         difference_array, f"{output_dir}/{on_name}_minus_{off_name}_unmasked.map"
     )
 
     return
 
 
+def _unit_cell_hack(cell):
+    """
+    Helper function to check if alpha, beta and gamma are all 90, and if so,
+    set alpha to 90.006. Otherwise, do nothing. a, b, c, beta, and gamma are never changed.
+
+    This is necessary because coot assumes that maps in P1 with alpha, beta, gamma all = 90 are
+    EM maps, and do not have periodic boundaries. Setting alpha=90.006 is sufficient to convince
+    coot to render periodic boundaries.
+
+    Parameters
+    ----------
+    cell : gemmi.UnitCell
+
+    Returns
+    -------
+    cell_with_hack : gemmi.UnitCell
+    """
+    if all(
+        [
+            angle == 90
+            for angle in (
+                cell.alpha,
+                cell.beta,
+                cell.gamma,
+            )
+        ]
+    ):
+        return gemmi.UnitCell(
+            cell.a,
+            cell.b,
+            cell.c,
+            90.006,
+            cell.beta,
+            cell.gamma,
+        )
+    else:
+        return cell
+
+
 def align_grids_from_model_transform(grid1, grid2, structure1, structure2, selection):
     """
     This function is basically just a wrapper around `gemmi.interpolate_grid_of_aligned_model2`, which is an amazing thing that exists!!.
 
     Parameters
     ----------
     grid1 : gemmi.FloatGrid
@@ -568,7 +590,82 @@
     # selection can be either a string or a list of strings
 
     sel = gemmi.Selection(selection)
 
     pdb_selection = sel.copy_model_selection(pdb)
 
     return pdb_selection
+
+
+def _ncs_align_and_subtract(
+    fg,
+    pdb,
+    ncs_chains,
+    name,
+    output_dir,
+):
+    # here, ncs_chains would be ["B", "C"] for example
+    # first element is 'fixed', second is 'moving'
+
+    fg.unit_cell = _unit_cell_hack(fg.unit_cell)
+
+    sup = gemmi.calculate_superposition(
+        pdb[0][ncs_chains[0]].get_polymer(),
+        pdb[0][ncs_chains[1]].get_polymer(),
+        gemmi.PolymerType.PeptideL,
+        gemmi.SupSelect.CaP,
+    )
+
+    fg2 = fg.clone()
+    fg2.fill(0)
+
+    gemmi.interpolate_grid_of_aligned_model2(
+        dest=fg2,
+        src=fg,
+        tr=sup.transform.inverse(),
+        dest_model=pdb[0],
+        radius=8,
+        order=2,
+    )
+
+    model = gemmi.Model("dummy model")
+    model.add_chain(pdb[0][ncs_chains[0]])
+
+    fg_mask_only = fg.clone()
+    fg_mask_only.fill(0)
+
+    masker = gemmi.SolventMasker(gemmi.AtomicRadiiSet.Cctbx)
+    masker.rprobe = 4  # generous mask to be sure to leave no islands
+    masker.put_mask_on_float_grid(fg_mask_only, model)
+
+    masked_arr1 = np.logical_not(fg_mask_only.array) * fg.array
+    masked_arr2 = np.logical_not(fg_mask_only.array) * fg2.array
+
+    mask = np.logical_not(fg_mask_only.array.astype(bool))
+
+    masked_arr1[mask] = _quicknorm(masked_arr1[mask])
+    masked_arr2[mask] = _quicknorm(masked_arr2[mask])
+
+    fg.set_subarray(arr=masked_arr1, start=(0, 0, 0))
+    fg2.set_subarray(arr=masked_arr2, start=(0, 0, 0))
+
+    print(f"{time.strftime('%H:%M:%S')}: Writing files...")
+
+    write_maps = partial(
+        rs.io.write_ccp4_map, cell=fg.unit_cell, spacegroup=fg.spacegroup
+    )
+
+    write_maps(fg.array, f"{output_dir}/{name}_{ncs_chains[0]}.map")
+    write_maps(fg2.array, f"{output_dir}/{name}_{ncs_chains[1]}.map")
+
+    write_maps(
+        fg2.array - fg.array,
+        f"{output_dir}/{name}_{ncs_chains[1]}_minus_{ncs_chains[0]}.map",
+    )
+
+    print(f"{time.strftime('%H:%M:%S')}: Done!")
+
+    return
+
+
+def _quicknorm(array):
+    return (array - array.mean()) / array.std()
```

### Comparing `matchmaps-0.1.4/.gitignore` & `matchmaps-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/LICENSE` & `matchmaps-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/README.md` & `matchmaps-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.4/pyproject.toml` & `matchmaps-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 [project.urls]
 homepage = "https://dennisbrookner.github.io/matchmaps/"
 repository = "https://github.com/dennisbrookner/matchmaps"
 
 # same as console_scripts entry point
 [project.scripts]
 matchmaps = "matchmaps._compute_realspace_diff:main"
+"matchmaps.ncs" = "matchmaps._compute_ncs_diff:main"
 
 # Entry points
 # https://peps.python.org/pep-0621/#entry-points
 # [project.entry-points."spam.magical"]
 # tomatoes = "spam:main_tomatoes"
 
 # https://hatch.pypa.io/latest/config/metadata/
```

### Comparing `matchmaps-0.1.4/PKG-INFO` & `matchmaps-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmaps
-Version: 0.1.4
+Version: 0.2.0
 Summary: Make unbiased difference maps even for non-isomorphous inputs
 Project-URL: homepage, https://dennisbrookner.github.io/matchmaps/
 Project-URL: repository, https://github.com/dennisbrookner/matchmaps
 Author-email: Dennis Brookner <debrookner@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

