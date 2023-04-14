# Comparing `tmp/datamol-0.9.4.tar.gz` & `tmp/datamol-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamol-0.9.4.tar", last modified: Fri Apr 14 14:57:34 2023, max compression
+gzip compressed data, was "datamol-0.9.6.tar", last modified: Fri Apr 14 22:54:02 2023, max compression
```

## Comparing `datamol-0.9.4.tar` & `datamol-0.9.6.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.922034 datamol-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-14 14:56:08.000000 datamol-0.9.4/.authors.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 14:56:08.000000 datamol-0.9.4/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-14 14:56:08.000000 datamol-0.9.4/.devcontainer/bashrc
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-14 14:56:08.000000 datamol-0.9.4/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-14 14:56:08.000000 datamol-0.9.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 14:56:08.000000 datamol-0.9.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-14 14:56:08.000000 datamol-0.9.4/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-14 14:56:08.000000 datamol-0.9.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-04-14 14:56:08.000000 datamol-0.9.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-04-14 14:56:08.000000 datamol-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 14:57:34.922034 datamol-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-14 14:56:08.000000 datamol-0.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 14:56:08.000000 datamol-0.9.4/binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 14:56:08.000000 datamol-0.9.4/binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 14:56:08.000000 datamol-0.9.4/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/datamol/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/_sanifix4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.902033 datamol-0.9.4/datamol/conformers/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/conformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/conformers/_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/conformers/_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.902033 datamol-0.9.4/datamol/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   160134 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/cdk2.sdf
--rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/freesolv.csv
--rw-r--r--   0 runner    (1001) docker     (123)   124841 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/reactions.json
--rw-r--r--   0 runner    (1001) docker     (123)   245735 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/solubility.test.sdf
--rw-r--r--   0 runner    (1001) docker     (123)  1376487 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/data/solubility.train.sdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.902033 datamol-0.9.4/datamol/descriptors/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/descriptors/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/descriptors/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/fp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.902033 datamol-0.9.4/datamol/fragment/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/fragment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/fragment/_assemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/fragment/_fragment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.902033 datamol-0.9.4/datamol/isomers/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/isomers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/isomers/_enumerate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/isomers/_structural.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/mcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43876 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/molar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/datamol/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/predictors/esol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/datamol/reactions/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/reactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/reactions/_attachments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/reactions/_reactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/datamol/scaffold/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/scaffold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/scaffold/_fuzzy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/datamol/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/datamol/viz/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/_circle_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19046 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/_lasso_highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/_substructure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 14:56:08.000000 datamol-0.9.4/datamol/viz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.898033 datamol-0.9.4/datamol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 14:57:34.000000 datamol-0.9.4/datamol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-14 14:57:34.000000 datamol-0.9.4/datamol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:57:34.000000 datamol-0.9.4/datamol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-14 14:57:34.000000 datamol-0.9.4/datamol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 14:57:34.000000 datamol-0.9.4/datamol.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.906033 datamol-0.9.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.910033 datamol-0.9.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.align.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.cluster.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.conformers.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.convert.md
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.data.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.descriptors.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.fp.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.fragment.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.graph.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.io.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.isomers.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.log.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.mol.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.molar.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.reactions.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.scaffold.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.similarity.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/api/datamol.viz.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.894033 datamol-0.9.4/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.910033 datamol-0.9.4/docs/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/assets/css/custom-datamol.css
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/assets/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/assets/css/tweak-width.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.910033 datamol-0.9.4/docs/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/assets/js/google-analytics.js
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/contribute.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.910033 datamol-0.9.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/images/logo-black.png
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/images/logo-black.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/images/logo-title.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.914034 datamol-0.9.4/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)   298565 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Aligning.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   174933 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Clustering.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    94833 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Conformers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   180458 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Descriptors.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Filesystem.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   297941 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Fragment.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   210862 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Fuzzy_Scaffolds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    42846 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Preprocessing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    89360 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Reactions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   151601 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Scaffolds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   521054 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/The_Basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   181122 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/Visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.914034 datamol-0.9.4/docs/tutorials/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1345316 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/data/ReactionBlock.rxn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.918034 datamol-0.9.4/docs/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (123)   141008 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Aligning_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    76455 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Aligning_2.png
--rw-r--r--   0 runner    (1001) docker     (123)   310889 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Conformers_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Descriptors_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   422734 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Fragment_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    67840 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Fragment_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    34879 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Fragment_3.png
--rw-r--r--   0 runner    (1001) docker     (123)   333241 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Preprocess_1.png
--rw-r--r--   0 runner    (1001) docker     (123)   102167 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/tutorials/images/Scaffolds_1.png
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 14:56:08.000000 datamol-0.9.4/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-14 14:56:08.000000 datamol-0.9.4/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-14 14:56:08.000000 datamol-0.9.4/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.918034 datamol-0.9.4/news/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 14:56:08.000000 datamol-0.9.4/news/TEMPLATE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-14 14:56:08.000000 datamol-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 14:56:08.000000 datamol-0.9.4/rever.xsh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:57:34.922034 datamol-0.9.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.922034 datamol-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:57:34.922034 datamol-0.9.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/TUBB3-observations-last-broken.sdf
--rw-r--r--   0 runner    (1001) docker     (123)    30331 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/TUBB3-observations.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/TUBB3-observations.sdf.gz
--rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/freesolv.csv
--rw-r--r--   0 runner    (1001) docker     (123)    28227 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/freesolv.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/data/test.mol2
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_datamol_import_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_fp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_fragment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_isomers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_mcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_mol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_molar.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_utils_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_utils_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_utils_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_viz_lasso_highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 14:56:08.000000 datamol-0.9.4/tests/test_viz_substrcture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.898833 datamol-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-14 22:53:52.000000 datamol-0.9.6/.authors.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.874833 datamol-0.9.6/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-14 22:52:32.000000 datamol-0.9.6/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-14 22:52:32.000000 datamol-0.9.6/.devcontainer/bashrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-14 22:52:32.000000 datamol-0.9.6/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.874833 datamol-0.9.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 22:52:32.000000 datamol-0.9.6/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-14 22:52:32.000000 datamol-0.9.6/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-14 22:52:32.000000 datamol-0.9.6/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-14 22:52:32.000000 datamol-0.9.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 22:52:32.000000 datamol-0.9.6/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.874833 datamol-0.9.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-14 22:52:32.000000 datamol-0.9.6/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-14 22:52:32.000000 datamol-0.9.6/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-14 22:52:32.000000 datamol-0.9.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-14 22:52:32.000000 datamol-0.9.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 22:52:32.000000 datamol-0.9.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-14 22:53:52.000000 datamol-0.9.6/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-14 22:53:52.000000 datamol-0.9.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26231 2023-04-14 22:53:52.000000 datamol-0.9.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-04-14 22:52:32.000000 datamol-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 22:54:02.898833 datamol-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-04-14 22:52:32.000000 datamol-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.874833 datamol-0.9.6/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 22:52:32.000000 datamol-0.9.6/binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 22:52:32.000000 datamol-0.9.6/binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 22:52:32.000000 datamol-0.9.6/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.878833 datamol-0.9.6/datamol/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/_sanifix4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.878833 datamol-0.9.6/datamol/conformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/conformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/conformers/_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/conformers/_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.878833 datamol-0.9.6/datamol/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   160134 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/data/cdk2.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/data/freesolv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   124841 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/data/reactions.json
+-rw-r--r--   0 runner    (1001) docker     (123)   245735 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/data/solubility.test.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)  1376487 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/data/solubility.train.sdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.878833 datamol-0.9.6/datamol/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/descriptors/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/descriptors/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/fp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.882833 datamol-0.9.6/datamol/fragment/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/fragment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/fragment/_assemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/fragment/_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.882833 datamol-0.9.6/datamol/isomers/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/isomers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/isomers/_enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/isomers/_structural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/mcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43876 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/molar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.882833 datamol-0.9.6/datamol/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/predictors/esol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.882833 datamol-0.9.6/datamol/reactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/reactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/reactions/_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/reactions/_reactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.882833 datamol-0.9.6/datamol/scaffold/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/scaffold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/scaffold/_fuzzy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.882833 datamol-0.9.6/datamol/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/utils/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/utils/perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.882833 datamol-0.9.6/datamol/viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/viz/_circle_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/viz/_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19046 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/viz/_lasso_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/viz/_substructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/viz/_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 22:52:32.000000 datamol-0.9.6/datamol/viz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.878833 datamol-0.9.6/datamol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-14 22:54:02.000000 datamol-0.9.6/datamol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-14 22:54:02.000000 datamol-0.9.6/datamol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:54:02.000000 datamol-0.9.6/datamol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-14 22:54:02.000000 datamol-0.9.6/datamol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 22:54:02.000000 datamol-0.9.6/datamol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.882833 datamol-0.9.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.886833 datamol-0.9.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.align.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.cluster.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.conformers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.convert.md
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.data.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.descriptors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.fp.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.fragment.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.graph.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.io.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.isomers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.log.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.mol.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.molar.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.reactions.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.scaffold.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.similarity.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/api/datamol.viz.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.874833 datamol-0.9.6/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.886833 datamol-0.9.6/docs/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/assets/css/custom-datamol.css
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/assets/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/assets/css/tweak-width.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.886833 datamol-0.9.6/docs/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/assets/js/google-analytics.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/contribute.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.886833 datamol-0.9.6/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/images/logo-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/images/logo-black.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/images/logo-title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.890833 datamol-0.9.6/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)   298565 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Aligning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   174933 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Clustering.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    94833 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Conformers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   180458 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Descriptors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Filesystem.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   297941 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Fragment.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   210862 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Fuzzy_Scaffolds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    42846 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Preprocessing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    89360 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Reactions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   151601 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Scaffolds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   521054 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/The_Basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   181122 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/Visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.890833 datamol-0.9.6/docs/tutorials/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1345316 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/data/ReactionBlock.rxn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.894833 datamol-0.9.6/docs/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   141008 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/images/Aligning_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76455 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/images/Aligning_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   310889 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/images/Conformers_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/images/Descriptors_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   422734 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/images/Fragment_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67840 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/images/Fragment_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34879 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/images/Fragment_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)   333241 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/images/Preprocess_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102167 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/tutorials/images/Scaffolds_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-14 22:52:32.000000 datamol-0.9.6/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 22:52:32.000000 datamol-0.9.6/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-14 22:52:32.000000 datamol-0.9.6/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.894833 datamol-0.9.6/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 22:52:32.000000 datamol-0.9.6/news/TEMPLATE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-14 22:52:32.000000 datamol-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 22:52:32.000000 datamol-0.9.6/rever.xsh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 22:54:02.898833 datamol-0.9.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.894833 datamol-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:54:02.898833 datamol-0.9.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    30130 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/data/TUBB3-observations-last-broken.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)    30331 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/data/TUBB3-observations.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/data/TUBB3-observations.sdf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    32060 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/data/freesolv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28227 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/data/freesolv.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/data/test.mol2
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10464 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_datamol_import_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_fragment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12272 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_isomers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_mcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28542 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_mol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_molar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_utils_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_utils_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_utils_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_viz_lasso_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 22:52:32.000000 datamol-0.9.6/tests/test_viz_substrcture.py
```

### Comparing `datamol-0.9.4/.authors.yml` & `datamol-0.9.6/.authors.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 - name: Emmanuel Noutahi
   email: emmanuel.noutahi@hotmail.ca
   aliases:
   - maclandrol
-  num_commits: 34
+  num_commits: 0
   first_commit: 2020-10-25 10:15:22
   github: DomInvivo
 - name: Hadrien Mary
   email: hadrien.mary@gmail.com
   aliases:
   - hadim
   alternate_emails:
   - hadim@users.noreply.github.com
-  num_commits: 39
+  num_commits: 0
   first_commit: 2020-10-24 11:46:22
   github: matudor
 - name: michelml
   email: michmoreau.l@gmail.com
-  num_commits: 26
+  num_commits: 0
   first_commit: 2021-02-25 15:48:52
 - name: Honoré Hounwanou
   email: mercuryseries@gmail.com
-  num_commits: 3
+  num_commits: 0
   first_commit: 2021-02-12 17:01:32
 - name: Therence1
   email: 38595485+Therence1@users.noreply.github.com
-  num_commits: 13
+  num_commits: 0
   first_commit: 2021-04-03 17:31:09
 - name: mike
   email: michael@invivoai.com
-  num_commits: 3
+  num_commits: 0
   first_commit: 2021-03-30 16:03:51
 - name: Ishan Kumar
   email: ishankumar216@gmail.com
-  num_commits: 5
+  num_commits: 0
   first_commit: 2021-05-10 11:45:15
 - name: deepsource-autofix[bot]
   email: 62050782+deepsource-autofix[bot]@users.noreply.github.com
-  num_commits: 1
+  num_commits: 0
   first_commit: 2021-07-19 17:58:37
 - name: DeepSource Bot
   email: bot@deepsource.io
-  num_commits: 1
+  num_commits: 0
   first_commit: 2021-07-14 17:41:40
 - name: Julien Horwood
   email: julien@invivoai.com
-  num_commits: 7
+  num_commits: 0
   first_commit: 2022-01-26 17:14:26
 - name: Cas
   email: caswognum@hotmail.com
-  num_commits: 7
+  num_commits: 0
   first_commit: 2022-06-02 16:20:56
   aliases:
   - cwognum
   alternate_emails:
   - caswognum@outlook.com
   github: cwognum
 - name: DomInvivo
   email: dominique@invivoai.com
-  num_commits: 31
+  num_commits: 0
   first_commit: 2022-06-14 09:40:04
   github: DomInvivo
 - name: Matt
   email: mtudor@proteovant.com
-  num_commits: 12
+  num_commits: 0
   first_commit: 2022-08-09 16:54:28
   github: matudor
 - name: Valence-JonnyHsu
   email: 104230580+Valence-JonnyHsu@users.noreply.github.com
-  num_commits: 12
+  num_commits: 0
   first_commit: 2022-09-08 10:46:44
 - name: Lu Zhu
   email: lu@valencediscovery.com
-  num_commits: 14
+  num_commits: 0
   first_commit: 2022-09-07 13:45:44
 - name: Saurav Maheshkar
   email: sauravvmaheshkar@gmail.com
-  num_commits: 5
+  num_commits: 0
   first_commit: 2023-03-07 16:59:47
   github: SauravMaheshkar
 - name: Pakman450
   email: steven.pak10@gmail.com
-  num_commits: 10
+  num_commits: 0
   first_commit: 2023-03-30 00:37:39
   github: Pakman450
 - name: dessygil
   email: desmondgilmour@gmail.com
-  num_commits: 6
+  num_commits: 0
   first_commit: 2023-04-05 17:40:19
```

### Comparing `datamol-0.9.4/.devcontainer/Dockerfile` & `datamol-0.9.6/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/.devcontainer/devcontainer.json` & `datamol-0.9.6/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/.github/CODE_OF_CONDUCT.md` & `datamol-0.9.6/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/.github/workflows/code-check.yml` & `datamol-0.9.6/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/.github/workflows/doc.yml` & `datamol-0.9.6/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/.github/workflows/test.yml` & `datamol-0.9.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/.gitignore` & `datamol-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/.mailmap` & `datamol-0.9.6/.mailmap`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/CHANGELOG.rst` & `datamol-0.9.6/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 ==================
 Datamol Changelogs
 ==================
 
 .. current developments
 
+v0.9.6
+====================
+
+**Authors:**
+
+* Hadrien Mary
+
+
+
 v0.9.4
 ====================
 
 **Fixed:**
 
 * Fix wrong image output for lasso viz function. Make it consistent with `dm.to_image()` and rdkit.
 * Avoid global `IPython` import so it's not an hard datamol dependency.
```

### Comparing `datamol-0.9.4/LICENSE` & `datamol-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/PKG-INFO` & `datamol-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamol
-Version: 0.9.4
+Version: 0.9.6
 Summary: A python library to work with molecules. Built on top of RDKit.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol
 Project-URL: Bug Tracker, https://github.com/datamol-io/datamol/issues
 Project-URL: Documentation, https://docs.datamol.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datamol Version: 0.9.4 Summary: A python library to
+Metadata-Version: 2.1 Name: datamol Version: 0.9.6 Summary: A python library to
 work with molecules. Built on top of RDKit. Author-email: Hadrien Mary
 valencediscovery.com> License: Apache Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol Project-URL:
 Bug Tracker, https://github.com/datamol-io/datamol/issues Project-URL:
 Documentation, https://docs.datamol.io Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
```

### Comparing `datamol-0.9.4/README.md` & `datamol-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/binder/environment.yml` & `datamol-0.9.6/binder/environment.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/__init__.py` & `datamol-0.9.6/datamol/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/_sanifix4.py` & `datamol-0.9.6/datamol/_sanifix4.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/_version.py` & `datamol-0.9.6/datamol/_version.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/align.py` & `datamol-0.9.6/datamol/align.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/cluster.py` & `datamol-0.9.6/datamol/cluster.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/conformers/_conformers.py` & `datamol-0.9.6/datamol/conformers/_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/conformers/_features.py` & `datamol-0.9.6/datamol/conformers/_features.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/convert.py` & `datamol-0.9.6/datamol/convert.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/data/__init__.py` & `datamol-0.9.6/datamol/data/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/data/cdk2.sdf` & `datamol-0.9.6/datamol/data/cdk2.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/data/freesolv.csv` & `datamol-0.9.6/datamol/data/freesolv.csv`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/data/reactions.json` & `datamol-0.9.6/datamol/data/reactions.json`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/data/solubility.test.sdf` & `datamol-0.9.6/datamol/data/solubility.test.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/data/solubility.train.sdf` & `datamol-0.9.6/datamol/data/solubility.train.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/descriptors/__init__.py` & `datamol-0.9.6/datamol/descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/descriptors/compute.py` & `datamol-0.9.6/datamol/descriptors/compute.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/descriptors/descriptors.py` & `datamol-0.9.6/datamol/descriptors/descriptors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/fp.py` & `datamol-0.9.6/datamol/fp.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/fragment/_assemble.py` & `datamol-0.9.6/datamol/fragment/_assemble.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/fragment/_fragment.py` & `datamol-0.9.6/datamol/fragment/_fragment.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/graph.py` & `datamol-0.9.6/datamol/graph.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/io.py` & `datamol-0.9.6/datamol/io.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/isomers/_enumerate.py` & `datamol-0.9.6/datamol/isomers/_enumerate.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/isomers/_structural.py` & `datamol-0.9.6/datamol/isomers/_structural.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/log.py` & `datamol-0.9.6/datamol/log.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/mcs.py` & `datamol-0.9.6/datamol/mcs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/mol.py` & `datamol-0.9.6/datamol/mol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/molar.py` & `datamol-0.9.6/datamol/molar.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/predictors/esol.py` & `datamol-0.9.6/datamol/predictors/esol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/reactions/__init__.py` & `datamol-0.9.6/datamol/reactions/__init__.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/reactions/_attachments.py` & `datamol-0.9.6/datamol/reactions/_attachments.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/reactions/_reactions.py` & `datamol-0.9.6/datamol/reactions/_reactions.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/scaffold/_fuzzy.py` & `datamol-0.9.6/datamol/scaffold/_fuzzy.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/similarity.py` & `datamol-0.9.6/datamol/similarity.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/utils/decorators.py` & `datamol-0.9.6/datamol/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/utils/fs.py` & `datamol-0.9.6/datamol/utils/fs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/utils/jobs.py` & `datamol-0.9.6/datamol/utils/jobs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/utils/perf.py` & `datamol-0.9.6/datamol/utils/perf.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/utils/testing.py` & `datamol-0.9.6/datamol/utils/testing.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/viz/_circle_grid.py` & `datamol-0.9.6/datamol/viz/_circle_grid.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/viz/_conformers.py` & `datamol-0.9.6/datamol/viz/_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/viz/_lasso_highlight.py` & `datamol-0.9.6/datamol/viz/_lasso_highlight.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/viz/_substructure.py` & `datamol-0.9.6/datamol/viz/_substructure.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/viz/_viz.py` & `datamol-0.9.6/datamol/viz/_viz.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol/viz/utils.py` & `datamol-0.9.6/datamol/viz/utils.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/datamol.egg-info/PKG-INFO` & `datamol-0.9.6/datamol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamol
-Version: 0.9.4
+Version: 0.9.6
 Summary: A python library to work with molecules. Built on top of RDKit.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol
 Project-URL: Bug Tracker, https://github.com/datamol-io/datamol/issues
 Project-URL: Documentation, https://docs.datamol.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datamol Version: 0.9.4 Summary: A python library to
+Metadata-Version: 2.1 Name: datamol Version: 0.9.6 Summary: A python library to
 work with molecules. Built on top of RDKit. Author-email: Hadrien Mary
 valencediscovery.com> License: Apache Project-URL: Website, https://datamol.io
 Project-URL: Source Code, https://github.com/datamol-io/datamol Project-URL:
 Bug Tracker, https://github.com/datamol-io/datamol/issues Project-URL:
 Documentation, https://docs.datamol.io Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
```

### Comparing `datamol-0.9.4/datamol.egg-info/SOURCES.txt` & `datamol-0.9.6/datamol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/assets/css/custom-datamol.css` & `datamol-0.9.6/docs/assets/css/custom-datamol.css`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/assets/css/custom.css` & `datamol-0.9.6/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/contribute.md` & `datamol-0.9.6/docs/contribute.md`

 * *Files 17% similar despite different names*

```diff
@@ -44,16 +44,8 @@
 
 ### Multi-versionning
 
 The doc is built for eash push on `main` and every git tags using [mike](https://github.com/jimporter/mike). Everything is automated using Github Actions. Please refer to the official mike's documentation for the details.
 
 ## Release a new version
 
-- Run check: `rever check`.
-- Bump and release new version: `rever VERSION_NUMBER`.
-- Releasing a new version will do the following things in that order:
-  - Update `AUTHORS.rst`.
-  - Update `CHANGELOG.rst`.
-  - Bump the version number in `setup.py` and `_version.py`.
-  - Add a git tag.
-  - Push the git tag.
-  - Then a GH Action will upload a new release on the GH repo associated with the git tag and push the package to PyPi.
+The process is fully automated by executing the [`release` GH Action](https://github.com/datamol-io/datamol/actions/workflows/release.yml).
```

### Comparing `datamol-0.9.4/docs/images/logo-black.png` & `datamol-0.9.6/docs/images/logo-black.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/images/logo-black.svg` & `datamol-0.9.6/docs/images/logo-black.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/images/logo-title.svg` & `datamol-0.9.6/docs/images/logo-title.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/images/logo.png` & `datamol-0.9.6/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/images/logo.svg` & `datamol-0.9.6/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/index.md` & `datamol-0.9.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Aligning.ipynb` & `datamol-0.9.6/docs/tutorials/Aligning.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Clustering.ipynb` & `datamol-0.9.6/docs/tutorials/Clustering.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Conformers.ipynb` & `datamol-0.9.6/docs/tutorials/Conformers.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Descriptors.ipynb` & `datamol-0.9.6/docs/tutorials/Descriptors.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Filesystem.ipynb` & `datamol-0.9.6/docs/tutorials/Filesystem.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Fragment.ipynb` & `datamol-0.9.6/docs/tutorials/Fragment.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Fuzzy_Scaffolds.ipynb` & `datamol-0.9.6/docs/tutorials/Fuzzy_Scaffolds.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Preprocessing.ipynb` & `datamol-0.9.6/docs/tutorials/Preprocessing.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Reactions.ipynb` & `datamol-0.9.6/docs/tutorials/Reactions.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Scaffolds.ipynb` & `datamol-0.9.6/docs/tutorials/Scaffolds.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/The_Basics.ipynb` & `datamol-0.9.6/docs/tutorials/The_Basics.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/Visualization.ipynb` & `datamol-0.9.6/docs/tutorials/Visualization.ipynb`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf` & `datamol-0.9.6/docs/tutorials/data/Enamine_DNA_Libary_5530cmpds_20200831_SMALL.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/data/ReactionBlock.rxn` & `datamol-0.9.6/docs/tutorials/data/ReactionBlock.rxn`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/images/Aligning_1.png` & `datamol-0.9.6/docs/tutorials/images/Aligning_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/images/Aligning_2.png` & `datamol-0.9.6/docs/tutorials/images/Aligning_2.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/images/Conformers_1.png` & `datamol-0.9.6/docs/tutorials/images/Conformers_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/images/Descriptors_1.png` & `datamol-0.9.6/docs/tutorials/images/Descriptors_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/images/Fragment_1.png` & `datamol-0.9.6/docs/tutorials/images/Fragment_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/images/Fragment_2.png` & `datamol-0.9.6/docs/tutorials/images/Fragment_2.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/images/Fragment_3.png` & `datamol-0.9.6/docs/tutorials/images/Fragment_3.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/images/Preprocess_1.png` & `datamol-0.9.6/docs/tutorials/images/Preprocess_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/tutorials/images/Scaffolds_1.png` & `datamol-0.9.6/docs/tutorials/images/Scaffolds_1.png`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/docs/usage.md` & `datamol-0.9.6/docs/usage.md`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/env.yml` & `datamol-0.9.6/env.yml`

 * *Files 10% similar despite different names*

```diff
@@ -51,14 +51,7 @@
   - mkdocstrings
   - mkdocstrings-python
   - mkdocs-jupyter
   - markdown-include
   - mdx_truly_sane_lists
   - mike >=1.0.0
   - seaborn
-
-  # Releasing tools
-  - rever >=0.4.5
-  - conda-smithy
-  - twine
-  - build
-  - setuptools-scm
```

### Comparing `datamol-0.9.4/mkdocs.yml` & `datamol-0.9.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/pyproject.toml` & `datamol-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/conftest.py` & `datamol-0.9.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/data/TUBB3-observations-last-broken.sdf` & `datamol-0.9.6/tests/data/TUBB3-observations-last-broken.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/data/TUBB3-observations.sdf` & `datamol-0.9.6/tests/data/TUBB3-observations.sdf`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/data/TUBB3-observations.sdf.gz` & `datamol-0.9.6/tests/data/TUBB3-observations.sdf.gz`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/data/freesolv.csv` & `datamol-0.9.6/tests/data/freesolv.csv`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/data/freesolv.xlsx` & `datamol-0.9.6/tests/data/freesolv.xlsx`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/data/test.mol2` & `datamol-0.9.6/tests/data/test.mol2`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_align.py` & `datamol-0.9.6/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_cluster.py` & `datamol-0.9.6/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_conformers.py` & `datamol-0.9.6/tests/test_conformers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_convert.py` & `datamol-0.9.6/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_data.py` & `datamol-0.9.6/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_datamol_import_time.py` & `datamol-0.9.6/tests/test_datamol_import_time.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_descriptors.py` & `datamol-0.9.6/tests/test_descriptors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_fp.py` & `datamol-0.9.6/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_fragment.py` & `datamol-0.9.6/tests/test_fragment.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_graph.py` & `datamol-0.9.6/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_io.py` & `datamol-0.9.6/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_isomers.py` & `datamol-0.9.6/tests/test_isomers.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_log.py` & `datamol-0.9.6/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_mcs.py` & `datamol-0.9.6/tests/test_mcs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_mol.py` & `datamol-0.9.6/tests/test_mol.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_molar.py` & `datamol-0.9.6/tests/test_molar.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_notebooks.py` & `datamol-0.9.6/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_predictors.py` & `datamol-0.9.6/tests/test_predictors.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_reactions.py` & `datamol-0.9.6/tests/test_reactions.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_scaffold.py` & `datamol-0.9.6/tests/test_scaffold.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_similarity.py` & `datamol-0.9.6/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_utils_fs.py` & `datamol-0.9.6/tests/test_utils_fs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_utils_jobs.py` & `datamol-0.9.6/tests/test_utils_jobs.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_viz.py` & `datamol-0.9.6/tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_viz_lasso_highlight.py` & `datamol-0.9.6/tests/test_viz_lasso_highlight.py`

 * *Files identical despite different names*

### Comparing `datamol-0.9.4/tests/test_viz_substrcture.py` & `datamol-0.9.6/tests/test_viz_substrcture.py`

 * *Files identical despite different names*

