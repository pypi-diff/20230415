# Comparing `tmp/felupe-7.0.0.tar.gz` & `tmp/felupe-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felupe-7.0.0.tar", last modified: Fri Apr  7 11:58:36 2023, max compression
+gzip compressed data, was "felupe-7.1.0.tar", last modified: Fri Apr 14 22:57:35 2023, max compression
```

## Comparing `felupe-7.0.0.tar` & `felupe-7.1.0.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.311094 felupe-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-04-07 11:58:26.000000 felupe-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    47965 2023-04-07 11:58:36.311094 felupe-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-07 11:58:26.000000 felupe-7.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-07 11:58:26.000000 felupe-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 11:58:36.311094 felupe-7.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.291093 felupe-7.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.295093 felupe-7.0.0/src/felupe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.295093 felupe-7.0.0/src/felupe/_assembly/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_assembly/_axi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_assembly/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_assembly/_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_assembly/_mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.295093 felupe-7.0.0/src/felupe/_basis/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_basis/_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.299093 felupe-7.0.0/src/felupe/_field/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_field/_axi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_field/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_field/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_field/_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_field/_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/_field/_planestrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.299093 felupe-7.0.0/src/felupe/constitution/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/constitution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/constitution/_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17288 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/constitution/_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/constitution/_models_hyperelasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/constitution/_models_hyperelasticity_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/constitution/_models_linear_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/constitution/_models_pseudo_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/constitution/_user_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/constitution/_user_materials_hyperelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/constitution/_user_materials_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.299093 felupe-7.0.0/src/felupe/dof/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/dof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/dof/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/dof/_loadcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/dof/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.299093 felupe-7.0.0/src/felupe/element/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/element/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13838 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/element/_hexahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/element/_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/element/_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/element/_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/element/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/element/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.303094 felupe-7.0.0/src/felupe/math/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/math/_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/math/_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/math/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/math/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.303094 felupe-7.0.0/src/felupe/mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/_pointload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/_solidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/_solidbody_gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/_solidbody_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/_solidbody_pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mechanics/_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.303094 felupe-7.0.0/src/felupe/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mesh/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mesh/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mesh/_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mesh/_discrete_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mesh/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mesh/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mesh/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mesh/_read.py
--rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/mesh/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.307094 felupe-7.0.0/src/felupe/quadrature/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/quadrature/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/quadrature/_gausslegendre.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/quadrature/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/quadrature/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.307094 felupe-7.0.0/src/felupe/region/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/region/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/region/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/region/_region.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/region/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.307094 felupe-7.0.0/src/felupe/solve/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/solve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/solve/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.307094 felupe-7.0.0/src/felupe/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/tools/_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/tools/_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/tools/_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/tools/_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-07 11:58:26.000000 felupe-7.0.0/src/felupe/tools/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.295093 felupe-7.0.0/src/felupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47965 2023-04-07 11:58:36.000000 felupe-7.0.0/src/felupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-07 11:58:36.000000 felupe-7.0.0/src/felupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 11:58:36.000000 felupe-7.0.0/src/felupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-07 11:58:36.000000 felupe-7.0.0/src/felupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-07 11:58:36.000000 felupe-7.0.0/src/felupe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:58:36.311094 felupe-7.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_bilinearform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_constitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_dof.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_planestrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-07 11:58:26.000000 felupe-7.0.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.686366 felupe-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-04-14 22:57:27.000000 felupe-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    48189 2023-04-14 22:57:35.682366 felupe-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-04-14 22:57:27.000000 felupe-7.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 22:57:27.000000 felupe-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 22:57:35.686366 felupe-7.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.670365 felupe-7.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.670365 felupe-7.1.0/src/felupe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.674366 felupe-7.1.0/src/felupe/_assembly/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_assembly/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_assembly/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_assembly/_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_assembly/_mixed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.674366 felupe-7.1.0/src/felupe/_basis/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_basis/_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.674366 felupe-7.1.0/src/felupe/_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_planestrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.674366 felupe-7.1.0/src/felupe/constitution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17288 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_models_hyperelasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_models_hyperelasticity_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_models_linear_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_models_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_user_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_user_materials_hyperelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_user_materials_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.674366 felupe-7.1.0/src/felupe/dof/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/dof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/dof/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/dof/_loadcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/dof/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.678366 felupe-7.1.0/src/felupe/element/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13838 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_hexahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.678366 felupe-7.1.0/src/felupe/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/math/_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/math/_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/math/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/math/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.678366 felupe-7.1.0/src/felupe/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_pointload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_solidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_solidbody_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_solidbody_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_solidbody_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.678366 felupe-7.1.0/src/felupe/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_discrete_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15966 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.678366 felupe-7.1.0/src/felupe/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/quadrature/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/quadrature/_gausslegendre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/quadrature/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/quadrature/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.682366 felupe-7.1.0/src/felupe/region/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/region/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/region/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/region/_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/region/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.682366 felupe-7.1.0/src/felupe/solve/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/solve/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.682366 felupe-7.1.0/src/felupe/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.670365 felupe-7.1.0/src/felupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48189 2023-04-14 22:57:35.000000 felupe-7.1.0/src/felupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-14 22:57:35.000000 felupe-7.1.0/src/felupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:57:35.000000 felupe-7.1.0/src/felupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 22:57:35.000000 felupe-7.1.0/src/felupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 22:57:35.000000 felupe-7.1.0/src/felupe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.682366 felupe-7.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_bilinearform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_constitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_dof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_planestrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_tools.py
```

### Comparing `felupe-7.0.0/LICENSE` & `felupe-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/PKG-INFO` & `felupe-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 7.0.0
+Version: 7.1.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -696,33 +696,36 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 # 🔍 FElupe - Finite Element Analysis
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe)
 
-<img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/logo_light.svg" height="120px"/> <img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="120px"/> <img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="120px"/>
+<p align="center">
+  <img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/logo_light.svg" height="120px"/> <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="120px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="120px"/></a>
+</p>
 
 FElupe is a Python 3.7+ finite element analysis package focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics of solid bodies. Its name is a combination of FE (finite element) and the german word *Lupe* (magnifying glass) as a synonym for getting an insight how a finite element analysis code looks like under the hood.
 
 # Installation
 Install Python, fire up a terminal and run
 
 ```shell
 pip install felupe[all]
 ```
 
-where `[all]` installs all optional dependencies. By default, FElupe depends on `numpy`, `scipy` and `einsumt`. In order to make use of all features of FElupe, it is suggested to install all optional dependencies (`h5py`, `meshio` and `tensortrax`).
+where `[all]` installs all optional dependencies. By default, FElupe depends on `numpy` and `scipy`. In order to make use of all features of FElupe, it is suggested to install all optional dependencies (`einsumt`, `h5py`, `matplotlib`, `meshio` and `tensortrax`).
 
 # Getting Started
 A quarter model of a solid cube with hyperelastic material behaviour is subjected to a uniaxial elongation applied at a clamped end-face. This involves the creation of a mesh, a region as well as a displacement field (encapsulated in a field container). Furthermore, the boundary conditions are created by a template for a uniaxial loadcase. An isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model formulation in combination with an isotropic hyperelastic Neo-Hookean material formulation is applied on a nearly-incompressible solid body. A step generates the consecutive substep-movements of a given boundary condition. The step is further added to a list of steps of a job (here, a characteristic-curve job is used). During evaluation, each substep of each step is solved by an iterative Newton-Rhapson procedure. The solution is exported after each completed substep as a time-series XDMF file. For more details beside this high-level code snippet, please have a look at the [documentation](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 ```python
 import felupe as fem
```

### Comparing `felupe-7.0.0/README.md` & `felupe-7.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,334 +55,347 @@
 00000360: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
 00000370: 6974 6875 622f 7374 6172 732f 6164 747a  ithub/stars/adtz
 00000380: 6c72 2f66 656c 7570 653f 6c6f 676f 3d67  lr/felupe?logo=g
 00000390: 6974 6875 6229 2021 5b50 7950 4920 2d20  ithub) ![PyPI - 
 000003a0: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
 000003b0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
 000003c0: 6f2f 7079 7069 2f64 6d2f 6665 6c75 7065  o/pypi/dm/felupe
-000003d0: 290a 0a3c 696d 6720 7372 633d 2268 7474  )..<img src="htt
-000003e0: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
-000003f0: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f61  sercontent.com/a
-00000400: 6474 7a6c 722f 6665 6c75 7065 2f6d 6169  dtzlr/felupe/mai
-00000410: 6e2f 646f 6373 2f5f 7374 6174 6963 2f6c  n/docs/_static/l
-00000420: 6f67 6f5f 6c69 6768 742e 7376 6722 2068  ogo_light.svg" h
-00000430: 6569 6768 743d 2231 3230 7078 222f 3e20  eight="120px"/> 
-00000440: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000450: 2f2f 7573 6572 2d69 6d61 6765 732e 6769  //user-images.gi
-00000460: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
-00000470: 636f 6d2f 3537 3933 3135 332f 3233 3036  com/5793153/2306
-00000480: 3034 3234 362d 3561 3431 3630 3831 2d36  04246-5a416081-6
-00000490: 3737 372d 3466 3333 2d61 6664 662d 6566  777-4f33-afdf-ef
-000004a0: 6462 3531 3333 3837 3232 2e70 6e67 2220  db51338722.png" 
-000004b0: 6865 6967 6874 3d22 3132 3070 7822 2f3e  height="120px"/>
-000004c0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-000004d0: 3a2f 2f75 7365 722d 696d 6167 6573 2e67  ://user-images.g
-000004e0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
-000004f0: 2e63 6f6d 2f35 3739 3331 3533 2f32 3330  .com/5793153/230
-00000500: 3630 3435 3837 2d34 3265 3365 3333 392d  604587-42e3e339-
-00000510: 6530 3863 2d34 6363 382d 3830 3030 2d66  e08c-4cc8-8000-f
-00000520: 3730 3436 6138 6439 3564 662e 706e 6722  7046a8d95df.png"
-00000530: 2068 6569 6768 743d 2231 3230 7078 222f   height="120px"/
-00000540: 3e0a 0a46 456c 7570 6520 6973 2061 2050  >..FElupe is a P
-00000550: 7974 686f 6e20 332e 372b 2066 696e 6974  ython 3.7+ finit
-00000560: 6520 656c 656d 656e 7420 616e 616c 7973  e element analys
-00000570: 6973 2070 6163 6b61 6765 2066 6f63 7573  is package focus
-00000580: 7369 6e67 206f 6e20 7468 6520 666f 726d  sing on the form
-00000590: 756c 6174 696f 6e20 616e 6420 6e75 6d65  ulation and nume
-000005a0: 7269 6361 6c20 736f 6c75 7469 6f6e 206f  rical solution o
-000005b0: 6620 6e6f 6e6c 696e 6561 7220 7072 6f62  f nonlinear prob
-000005c0: 6c65 6d73 2069 6e20 636f 6e74 696e 7575  lems in continuu
-000005d0: 6d20 6d65 6368 616e 6963 7320 6f66 2073  m mechanics of s
-000005e0: 6f6c 6964 2062 6f64 6965 732e 2049 7473  olid bodies. Its
-000005f0: 206e 616d 6520 6973 2061 2063 6f6d 6269   name is a combi
-00000600: 6e61 7469 6f6e 206f 6620 4645 2028 6669  nation of FE (fi
-00000610: 6e69 7465 2065 6c65 6d65 6e74 2920 616e  nite element) an
-00000620: 6420 7468 6520 6765 726d 616e 2077 6f72  d the german wor
-00000630: 6420 2a4c 7570 652a 2028 6d61 676e 6966  d *Lupe* (magnif
-00000640: 7969 6e67 2067 6c61 7373 2920 6173 2061  ying glass) as a
-00000650: 2073 796e 6f6e 796d 2066 6f72 2067 6574   synonym for get
-00000660: 7469 6e67 2061 6e20 696e 7369 6768 7420  ting an insight 
-00000670: 686f 7720 6120 6669 6e69 7465 2065 6c65  how a finite ele
-00000680: 6d65 6e74 2061 6e61 6c79 7369 7320 636f  ment analysis co
-00000690: 6465 206c 6f6f 6b73 206c 696b 6520 756e  de looks like un
-000006a0: 6465 7220 7468 6520 686f 6f64 2e0a 0a23  der the hood...#
-000006b0: 2049 6e73 7461 6c6c 6174 696f 6e0a 496e   Installation.In
-000006c0: 7374 616c 6c20 5079 7468 6f6e 2c20 6669  stall Python, fi
-000006d0: 7265 2075 7020 6120 7465 726d 696e 616c  re up a terminal
-000006e0: 2061 6e64 2072 756e 0a0a 6060 6073 6865   and run..```she
-000006f0: 6c6c 0a70 6970 2069 6e73 7461 6c6c 2066  ll.pip install f
-00000700: 656c 7570 655b 616c 6c5d 0a60 6060 0a0a  elupe[all].```..
-00000710: 7768 6572 6520 605b 616c 6c5d 6020 696e  where `[all]` in
-00000720: 7374 616c 6c73 2061 6c6c 206f 7074 696f  stalls all optio
-00000730: 6e61 6c20 6465 7065 6e64 656e 6369 6573  nal dependencies
-00000740: 2e20 4279 2064 6566 6175 6c74 2c20 4645  . By default, FE
-00000750: 6c75 7065 2064 6570 656e 6473 206f 6e20  lupe depends on 
-00000760: 606e 756d 7079 602c 2060 7363 6970 7960  `numpy`, `scipy`
-00000770: 2061 6e64 2060 6569 6e73 756d 7460 2e20   and `einsumt`. 
-00000780: 496e 206f 7264 6572 2074 6f20 6d61 6b65  In order to make
-00000790: 2075 7365 206f 6620 616c 6c20 6665 6174   use of all feat
-000007a0: 7572 6573 206f 6620 4645 6c75 7065 2c20  ures of FElupe, 
-000007b0: 6974 2069 7320 7375 6767 6573 7465 6420  it is suggested 
-000007c0: 746f 2069 6e73 7461 6c6c 2061 6c6c 206f  to install all o
-000007d0: 7074 696f 6e61 6c20 6465 7065 6e64 656e  ptional dependen
-000007e0: 6369 6573 2028 6068 3570 7960 2c20 606d  cies (`h5py`, `m
-000007f0: 6573 6869 6f60 2061 6e64 2060 7465 6e73  eshio` and `tens
-00000800: 6f72 7472 6178 6029 2e0a 0a23 2047 6574  ortrax`)...# Get
-00000810: 7469 6e67 2053 7461 7274 6564 0a41 2071  ting Started.A q
-00000820: 7561 7274 6572 206d 6f64 656c 206f 6620  uarter model of 
-00000830: 6120 736f 6c69 6420 6375 6265 2077 6974  a solid cube wit
-00000840: 6820 6879 7065 7265 6c61 7374 6963 206d  h hyperelastic m
-00000850: 6174 6572 6961 6c20 6265 6861 7669 6f75  aterial behaviou
-00000860: 7220 6973 2073 7562 6a65 6374 6564 2074  r is subjected t
-00000870: 6f20 6120 756e 6961 7869 616c 2065 6c6f  o a uniaxial elo
-00000880: 6e67 6174 696f 6e20 6170 706c 6965 6420  ngation applied 
-00000890: 6174 2061 2063 6c61 6d70 6564 2065 6e64  at a clamped end
-000008a0: 2d66 6163 652e 2054 6869 7320 696e 766f  -face. This invo
-000008b0: 6c76 6573 2074 6865 2063 7265 6174 696f  lves the creatio
-000008c0: 6e20 6f66 2061 206d 6573 682c 2061 2072  n of a mesh, a r
-000008d0: 6567 696f 6e20 6173 2077 656c 6c20 6173  egion as well as
-000008e0: 2061 2064 6973 706c 6163 656d 656e 7420   a displacement 
-000008f0: 6669 656c 6420 2865 6e63 6170 7375 6c61  field (encapsula
-00000900: 7465 6420 696e 2061 2066 6965 6c64 2063  ted in a field c
-00000910: 6f6e 7461 696e 6572 292e 2046 7572 7468  ontainer). Furth
-00000920: 6572 6d6f 7265 2c20 7468 6520 626f 756e  ermore, the boun
-00000930: 6461 7279 2063 6f6e 6469 7469 6f6e 7320  dary conditions 
-00000940: 6172 6520 6372 6561 7465 6420 6279 2061  are created by a
-00000950: 2074 656d 706c 6174 6520 666f 7220 6120   template for a 
-00000960: 756e 6961 7869 616c 206c 6f61 6463 6173  uniaxial loadcas
-00000970: 652e 2041 6e20 6973 6f74 726f 7069 6320  e. An isotropic 
-00000980: 7073 6575 646f 2d65 6c61 7374 6963 204f  pseudo-elastic O
-00000990: 6764 656e 2d52 6f78 6275 7267 6820 4d75  gden-Roxburgh Mu
-000009a0: 6c6c 696e 732d 736f 6674 656e 696e 6720  llins-softening 
-000009b0: 6d6f 6465 6c20 666f 726d 756c 6174 696f  model formulatio
-000009c0: 6e20 696e 2063 6f6d 6269 6e61 7469 6f6e  n in combination
-000009d0: 2077 6974 6820 616e 2069 736f 7472 6f70   with an isotrop
-000009e0: 6963 2068 7970 6572 656c 6173 7469 6320  ic hyperelastic 
-000009f0: 4e65 6f2d 486f 6f6b 6561 6e20 6d61 7465  Neo-Hookean mate
-00000a00: 7269 616c 2066 6f72 6d75 6c61 7469 6f6e  rial formulation
-00000a10: 2069 7320 6170 706c 6965 6420 6f6e 2061   is applied on a
-00000a20: 206e 6561 726c 792d 696e 636f 6d70 7265   nearly-incompre
-00000a30: 7373 6962 6c65 2073 6f6c 6964 2062 6f64  ssible solid bod
-00000a40: 792e 2041 2073 7465 7020 6765 6e65 7261  y. A step genera
-00000a50: 7465 7320 7468 6520 636f 6e73 6563 7574  tes the consecut
-00000a60: 6976 6520 7375 6273 7465 702d 6d6f 7665  ive substep-move
-00000a70: 6d65 6e74 7320 6f66 2061 2067 6976 656e  ments of a given
-00000a80: 2062 6f75 6e64 6172 7920 636f 6e64 6974   boundary condit
-00000a90: 696f 6e2e 2054 6865 2073 7465 7020 6973  ion. The step is
-00000aa0: 2066 7572 7468 6572 2061 6464 6564 2074   further added t
-00000ab0: 6f20 6120 6c69 7374 206f 6620 7374 6570  o a list of step
-00000ac0: 7320 6f66 2061 206a 6f62 2028 6865 7265  s of a job (here
-00000ad0: 2c20 6120 6368 6172 6163 7465 7269 7374  , a characterist
-00000ae0: 6963 2d63 7572 7665 206a 6f62 2069 7320  ic-curve job is 
-00000af0: 7573 6564 292e 2044 7572 696e 6720 6576  used). During ev
-00000b00: 616c 7561 7469 6f6e 2c20 6561 6368 2073  aluation, each s
-00000b10: 7562 7374 6570 206f 6620 6561 6368 2073  ubstep of each s
-00000b20: 7465 7020 6973 2073 6f6c 7665 6420 6279  tep is solved by
-00000b30: 2061 6e20 6974 6572 6174 6976 6520 4e65   an iterative Ne
-00000b40: 7774 6f6e 2d52 6861 7073 6f6e 2070 726f  wton-Rhapson pro
-00000b50: 6365 6475 7265 2e20 5468 6520 736f 6c75  cedure. The solu
-00000b60: 7469 6f6e 2069 7320 6578 706f 7274 6564  tion is exported
-00000b70: 2061 6674 6572 2065 6163 6820 636f 6d70   after each comp
-00000b80: 6c65 7465 6420 7375 6273 7465 7020 6173  leted substep as
-00000b90: 2061 2074 696d 652d 7365 7269 6573 2058   a time-series X
-00000ba0: 444d 4620 6669 6c65 2e20 466f 7220 6d6f  DMF file. For mo
-00000bb0: 7265 2064 6574 6169 6c73 2062 6573 6964  re details besid
-00000bc0: 6520 7468 6973 2068 6967 682d 6c65 7665  e this high-leve
-00000bd0: 6c20 636f 6465 2073 6e69 7070 6574 2c20  l code snippet, 
-00000be0: 706c 6561 7365 2068 6176 6520 6120 6c6f  please have a lo
-00000bf0: 6f6b 2061 7420 7468 6520 5b64 6f63 756d  ok at the [docum
-00000c00: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-00000c10: 2f2f 6665 6c75 7065 2e72 6561 6474 6865  //felupe.readthe
-00000c20: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-00000c30: 742f 3f62 6164 6765 3d6c 6174 6573 7429  t/?badge=latest)
-00000c40: 2e0a 0a60 6060 7079 7468 6f6e 0a69 6d70  ...```python.imp
-00000c50: 6f72 7420 6665 6c75 7065 2061 7320 6665  ort felupe as fe
-00000c60: 6d0a 0a23 2063 7265 6174 6520 6120 6865  m..# create a he
-00000c70: 7861 6865 6472 6f6e 2d72 6567 696f 6e20  xahedron-region 
-00000c80: 6f6e 2061 2063 7562 650a 6d65 7368 203d  on a cube.mesh =
-00000c90: 2066 656d 2e43 7562 6528 6e3d 3131 290a   fem.Cube(n=11).
-00000ca0: 7265 6769 6f6e 203d 2066 656d 2e52 6567  region = fem.Reg
-00000cb0: 696f 6e48 6578 6168 6564 726f 6e28 6d65  ionHexahedron(me
-00000cc0: 7368 290a 0a23 2061 6464 2061 2066 6965  sh)..# add a fie
-00000cd0: 6c64 2063 6f6e 7461 696e 6572 2028 7769  ld container (wi
-00000ce0: 7468 2061 2076 6563 746f 722d 7661 6c75  th a vector-valu
-00000cf0: 6564 2064 6973 706c 6163 656d 656e 7420  ed displacement 
-00000d00: 6669 656c 6429 0a66 6965 6c64 203d 2066  field).field = f
-00000d10: 656d 2e46 6965 6c64 436f 6e74 6169 6e65  em.FieldContaine
-00000d20: 7228 5b66 656d 2e46 6965 6c64 2872 6567  r([fem.Field(reg
-00000d30: 696f 6e2c 2064 696d 3d33 295d 290a 0a23  ion, dim=3)])..#
-00000d40: 2061 7070 6c79 2061 2075 6e69 6178 6961   apply a uniaxia
-00000d50: 6c20 656c 6f6e 6761 7469 6f6e 206f 6e20  l elongation on 
-00000d60: 7468 6520 6375 6265 0a62 6f75 6e64 6172  the cube.boundar
-00000d70: 6965 7320 3d20 6665 6d2e 646f 662e 756e  ies = fem.dof.un
-00000d80: 6961 7869 616c 2866 6965 6c64 2c20 636c  iaxial(field, cl
-00000d90: 616d 7065 643d 5472 7565 295b 305d 0a0a  amped=True)[0]..
-00000da0: 2320 6465 6669 6e65 2074 6865 2063 6f6e  # define the con
-00000db0: 7374 6974 7574 6976 6520 6d61 7465 7269  stitutive materi
-00000dc0: 616c 2062 6568 6176 696f 7572 0a23 2061  al behaviour.# a
-00000dd0: 6e64 2063 7265 6174 6520 6120 6e65 6172  nd create a near
-00000de0: 6c79 2d69 6e63 6f6d 7072 6573 7369 626c  ly-incompressibl
-00000df0: 6520 2875 2c70 2c4a 202d 2066 6f72 6d75  e (u,p,J - formu
-00000e00: 6c61 7469 6f6e 2920 736f 6c69 6420 626f  lation) solid bo
-00000e10: 6479 0a75 6d61 7420 3d20 6665 6d2e 4f67  dy.umat = fem.Og
-00000e20: 6465 6e52 6f78 6275 7267 6828 6d61 7465  denRoxburgh(mate
-00000e30: 7269 616c 3d66 656d 2e4e 656f 486f 6f6b  rial=fem.NeoHook
-00000e40: 6528 6d75 3d31 292c 2072 3d33 2c20 6d3d  e(mu=1), r=3, m=
-00000e50: 312c 2062 6574 613d 3029 0a73 6f6c 6964  1, beta=0).solid
-00000e60: 203d 2066 656d 2e53 6f6c 6964 426f 6479   = fem.SolidBody
-00000e70: 4e65 6172 6c79 496e 636f 6d70 7265 7373  NearlyIncompress
-00000e80: 6962 6c65 2875 6d61 742c 2066 6965 6c64  ible(umat, field
-00000e90: 2c20 6275 6c6b 3d35 3030 3029 0a0a 2320  , bulk=5000)..# 
-00000ea0: 7072 6570 6172 6520 6120 7374 6570 2077  prepare a step w
-00000eb0: 6974 6820 7375 6273 7465 7073 0a6d 6f76  ith substeps.mov
-00000ec0: 6520 3d20 6665 6d2e 6d61 7468 2e6c 696e  e = fem.math.lin
-00000ed0: 7374 6570 7328 5b30 2c20 322c 2030 5d2c  steps([0, 2, 0],
-00000ee0: 206e 756d 3d31 3029 0a73 7465 7020 3d20   num=10).step = 
-00000ef0: 6665 6d2e 5374 6570 2869 7465 6d73 3d5b  fem.Step(items=[
-00000f00: 736f 6c69 645d 2c20 7261 6d70 3d7b 626f  solid], ramp={bo
-00000f10: 756e 6461 7269 6573 5b22 6d6f 7665 225d  undaries["move"]
-00000f20: 3a20 6d6f 7665 7d2c 2062 6f75 6e64 6172  : move}, boundar
-00000f30: 6965 733d 626f 756e 6461 7269 6573 290a  ies=boundaries).
-00000f40: 0a23 2061 6464 2074 6865 2073 7465 7020  .# add the step 
-00000f50: 746f 2061 206a 6f62 2c20 6576 616c 7561  to a job, evalua
-00000f60: 7465 2061 6c6c 2073 7562 7374 6570 7320  te all substeps 
-00000f70: 616e 6420 6372 6561 7465 2061 2070 6c6f  and create a plo
-00000f80: 740a 6a6f 6220 3d20 6665 6d2e 4368 6172  t.job = fem.Char
-00000f90: 6163 7465 7269 7374 6963 4375 7276 6528  acteristicCurve(
-00000fa0: 7374 6570 733d 5b73 7465 705d 2c20 626f  steps=[step], bo
-00000fb0: 756e 6461 7279 3d62 6f75 6e64 6172 6965  undary=boundarie
-00000fc0: 735b 226d 6f76 6522 5d29 0a6a 6f62 2e65  s["move"]).job.e
-00000fd0: 7661 6c75 6174 6528 6669 6c65 6e61 6d65  valuate(filename
-00000fe0: 3d22 7265 7375 6c74 2e78 646d 6622 290a  ="result.xdmf").
-00000ff0: 6669 672c 2061 7820 3d20 6a6f 622e 706c  fig, ax = job.pl
-00001000: 6f74 280a 2020 2020 786c 6162 656c 3d22  ot(.    xlabel="
-00001010: 4469 7370 6c61 6365 6d65 6e74 2024 7524  Displacement $u$
-00001020: 2069 6e20 6d6d 2024 5c6c 6f6e 6772 6967   in mm $\longrig
-00001030: 6874 6172 726f 7724 222c 0a20 2020 2079  htarrow$",.    y
-00001040: 6c61 6265 6c3d 224e 6f72 6d61 6c20 466f  label="Normal Fo
-00001050: 7263 6520 2446 2420 696e 204e 2024 5c6c  rce $F$ in N $\l
-00001060: 6f6e 6772 6967 6874 6172 726f 7724 222c  ongrightarrow$",
-00001070: 0a29 0a60 6060 0a0a 6874 7470 733a 2f2f  .).```..https://
-00001080: 7573 6572 2d69 6d61 6765 732e 6769 7468  user-images.gith
-00001090: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
-000010a0: 6d2f 3537 3933 3135 332f 3230 3039 3531  m/5793153/200951
-000010b0: 3338 312d 6561 3331 3065 3534 2d37 3632  381-ea310e54-762
-000010c0: 332d 3464 6431 2d61 3535 662d 6132 3866  3-4dd1-a55f-a28f
-000010d0: 3930 3535 3036 3366 2e6d 7034 0a0a 3c69  9055063f.mp4..<i
-000010e0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000010f0: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00001100: 6e74 656e 742e 636f 6d2f 6164 747a 6c72  ntent.com/adtzlr
-00001110: 2f66 656c 7570 652f 6d61 696e 2f64 6f63  /felupe/main/doc
-00001120: 732f 5f73 7461 7469 632f 7265 6164 6d65  s/_static/readme
-00001130: 5f63 6861 7261 6374 6572 6973 7469 635f  _characteristic_
-00001140: 6375 7276 652e 7376 6722 2077 6964 7468  curve.svg" width
-00001150: 3d22 3630 3070 7822 2f3e 0a0a 2320 446f  ="600px"/>..# Do
-00001160: 6375 6d65 6e74 6174 696f 6e0a 5468 6520  cumentation.The 
-00001170: 646f 6375 6d65 6e74 6174 696f 6e20 6973  documentation is
-00001180: 206c 6f63 6174 6564 205b 6865 7265 5d28   located [here](
-00001190: 6874 7470 733a 2f2f 6665 6c75 7065 2e72  https://felupe.r
-000011a0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-000011b0: 2f6c 6174 6573 742f 3f62 6164 6765 3d6c  /latest/?badge=l
-000011c0: 6174 6573 7429 2e0a 0a23 2045 7874 656e  atest)...# Exten
-000011d0: 7369 6f6e 2050 6163 6b61 6765 730a 5468  sion Packages.Th
-000011e0: 6520 6361 7061 6269 6c69 7469 6573 206f  e capabilities o
-000011f0: 6620 4645 6c75 7065 206d 6179 2062 6520  f FElupe may be 
-00001200: 656e 6861 6e63 6564 2077 6974 6820 6578  enhanced with ex
-00001210: 7465 6e73 696f 6e20 7061 636b 6167 6573  tension packages
-00001220: 2063 7265 6174 6564 2062 7920 7468 6520   created by the 
-00001230: 636f 6d6d 756e 6974 792e 0a0a 7c20 2a2a  community...| **
-00001240: 5061 636b 6167 652a 2a20 7c20 2020 2020  Package** |     
-00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 2a2a 4465 7363 7269 7074 696f 6e2a 2a20  **Description** 
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00001290: 2020 2020 202a 2a4c 696e 6b2a 2a20 2020       **Link**   
-000012a0: 2020 2020 2020 2020 2020 2020 7c0a 7c3a              |.|:
-000012b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d  -----------:|:--
-000012c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000012d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000012e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000012f0: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-00001300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a  -------------:|.
-00001320: 7c20 2074 656e 736f 7274 7261 7820 7c20  |  tensortrax | 
-00001330: 2020 2020 4d61 7468 206f 6e20 2848 7970      Math on (Hyp
-00001340: 6572 2d44 7561 6c29 2054 656e 736f 7273  er-Dual) Tensors
-00001350: 2077 6974 6820 5472 6169 6c69 6e67 2041   with Trailing A
-00001360: 7865 7320 2020 2020 7c20 2068 7474 7073  xes     |  https
-00001370: 3a2f 2f67 6974 6875 622e 636f 6d2f 6164  ://github.com/ad
-00001380: 747a 6c72 2f74 656e 736f 7274 7261 7820  tzlr/tensortrax 
-00001390: 7c0a 7c20 2020 206d 6174 4144 6920 2020  |.|    matADi   
-000013a0: 7c20 4d61 7465 7269 616c 2044 6566 696e  | Material Defin
-000013b0: 6974 696f 6e20 7769 7468 2041 7574 6f6d  ition with Autom
-000013c0: 6174 6963 2044 6966 6665 7265 6e74 6961  atic Differentia
-000013d0: 7469 6f6e 2028 4144 2920 7c20 2020 2068  tion (AD) |    h
-000013e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000013f0: 6d2f 6164 747a 6c72 2f6d 6174 6164 6920  m/adtzlr/matadi 
-00001400: 2020 7c0a 7c20 2020 2046 4570 6c6f 7420    |.|    FEplot 
-00001410: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00001420: 4120 7669 7375 616c 697a 6174 696f 6e20  A visualization 
-00001430: 746f 6f6c 2066 6f72 2046 456c 7570 6520  tool for FElupe 
-00001440: 2020 2020 2020 2020 2020 2020 7c20 6874              | ht
-00001450: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001460: 2f5a 4141 5241 4f55 4939 3939 2f66 6570  /ZAARAOUI999/fep
-00001470: 6c6f 7420 7c0a 0a23 2043 6861 6e67 656c  lot |..# Changel
-00001480: 6f67 0a41 6c6c 206e 6f74 6162 6c65 2063  og.All notable c
-00001490: 6861 6e67 6573 2074 6f20 7468 6973 2070  hanges to this p
-000014a0: 726f 6a65 6374 2077 696c 6c20 6265 2064  roject will be d
-000014b0: 6f63 756d 656e 7465 6420 696e 205b 7468  ocumented in [th
-000014c0: 6973 2066 696c 655d 2843 4841 4e47 454c  is file](CHANGEL
-000014d0: 4f47 2e6d 6429 2e20 5468 6520 666f 726d  OG.md). The form
-000014e0: 6174 2069 7320 6261 7365 6420 6f6e 205b  at is based on [
-000014f0: 4b65 6570 2061 2043 6861 6e67 656c 6f67  Keep a Changelog
-00001500: 5d28 6874 7470 733a 2f2f 6b65 6570 6163  ](https://keepac
-00001510: 6861 6e67 656c 6f67 2e63 6f6d 2f65 6e2f  hangelog.com/en/
-00001520: 312e 302e 302f 292c 2061 6e64 2074 6869  1.0.0/), and thi
-00001530: 7320 7072 6f6a 6563 7420 6164 6865 7265  s project adhere
-00001540: 7320 746f 205b 5365 6d61 6e74 6963 2056  s to [Semantic V
-00001550: 6572 7369 6f6e 696e 675d 2868 7474 7073  ersioning](https
-00001560: 3a2f 2f73 656d 7665 722e 6f72 672f 7370  ://semver.org/sp
-00001570: 6563 2f76 322e 302e 302e 6874 6d6c 292e  ec/v2.0.0.html).
-00001580: 0a0a 2320 4c69 6365 6e73 650a 4645 6c75  ..# License.FElu
-00001590: 7065 202d 2066 696e 6974 6520 656c 656d  pe - finite elem
-000015a0: 656e 7420 616e 616c 7973 6973 2028 4329  ent analysis (C)
-000015b0: 2032 3032 3320 416e 6472 6561 7320 4475   2023 Andreas Du
-000015c0: 747a 6c65 722c 2047 7261 7a20 2841 7573  tzler, Graz (Aus
-000015d0: 7472 6961 292e 0a0a 5468 6973 2070 726f  tria)...This pro
-000015e0: 6772 616d 2069 7320 6672 6565 2073 6f66  gram is free sof
-000015f0: 7477 6172 653a 2079 6f75 2063 616e 2072  tware: you can r
-00001600: 6564 6973 7472 6962 7574 6520 6974 2061  edistribute it a
-00001610: 6e64 2f6f 7220 6d6f 6469 6679 2069 7420  nd/or modify it 
-00001620: 756e 6465 7220 7468 6520 7465 726d 7320  under the terms 
-00001630: 6f66 2074 6865 2047 4e55 2047 656e 6572  of the GNU Gener
-00001640: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-00001650: 6520 6173 2070 7562 6c69 7368 6564 2062  e as published b
-00001660: 7920 7468 6520 4672 6565 2053 6f66 7477  y the Free Softw
-00001670: 6172 6520 466f 756e 6461 7469 6f6e 2c20  are Foundation, 
-00001680: 6569 7468 6572 2076 6572 7369 6f6e 2033  either version 3
-00001690: 206f 6620 7468 6520 4c69 6365 6e73 652c   of the License,
-000016a0: 206f 7220 2861 7420 796f 7572 206f 7074   or (at your opt
-000016b0: 696f 6e29 2061 6e79 206c 6174 6572 2076  ion) any later v
-000016c0: 6572 7369 6f6e 2e0a 0a54 6869 7320 7072  ersion...This pr
-000016d0: 6f67 7261 6d20 6973 2064 6973 7472 6962  ogram is distrib
-000016e0: 7574 6564 2069 6e20 7468 6520 686f 7065  uted in the hope
-000016f0: 2074 6861 7420 6974 2077 696c 6c20 6265   that it will be
-00001700: 2075 7365 6675 6c2c 2062 7574 2057 4954   useful, but WIT
-00001710: 484f 5554 2041 4e59 2057 4152 5241 4e54  HOUT ANY WARRANT
-00001720: 593b 2077 6974 686f 7574 2065 7665 6e20  Y; without even 
-00001730: 7468 6520 696d 706c 6965 6420 7761 7272  the implied warr
-00001740: 616e 7479 206f 6620 4d45 5243 4841 4e54  anty of MERCHANT
-00001750: 4142 494c 4954 5920 6f72 2046 4954 4e45  ABILITY or FITNE
-00001760: 5353 2046 4f52 2041 2050 4152 5449 4355  SS FOR A PARTICU
-00001770: 4c41 5220 5055 5250 4f53 452e 2053 6565  LAR PURPOSE. See
-00001780: 2074 6865 2047 4e55 2047 656e 6572 616c   the GNU General
-00001790: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
-000017a0: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
-000017b0: 2e0a 0a59 6f75 2073 686f 756c 6420 6861  ...You should ha
-000017c0: 7665 2072 6563 6569 7665 6420 6120 636f  ve received a co
-000017d0: 7079 206f 6620 7468 6520 474e 5520 4765  py of the GNU Ge
-000017e0: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
-000017f0: 656e 7365 2061 6c6f 6e67 2077 6974 6820  ense along with 
-00001800: 7468 6973 2070 726f 6772 616d 2e20 4966  this program. If
-00001810: 206e 6f74 2c20 7365 6520 3c68 7474 7073   not, see <https
-00001820: 3a2f 2f77 7777 2e67 6e75 2e6f 7267 2f6c  ://www.gnu.org/l
-00001830: 6963 656e 7365 732f 3e2e 0a              icenses/>..
+000003d0: 290a 0a3c 7020 616c 6967 6e3d 2263 656e  )..<p align="cen
+000003e0: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
+000003f0: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00000400: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000410: 636f 6d2f 6164 747a 6c72 2f66 656c 7570  com/adtzlr/felup
+00000420: 652f 6d61 696e 2f64 6f63 732f 5f73 7461  e/main/docs/_sta
+00000430: 7469 632f 6c6f 676f 5f6c 6967 6874 2e73  tic/logo_light.s
+00000440: 7667 2220 6865 6967 6874 3d22 3132 3070  vg" height="120p
+00000450: 7822 2f3e 203c 6120 6872 6566 3d22 6874  x"/> <a href="ht
+00000460: 7470 733a 2f2f 6665 6c75 7065 2e72 6561  tps://felupe.rea
+00000470: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000480: 6174 6573 742f 6578 616d 706c 6573 2f72  atest/examples/r
+00000490: 7562 6265 7273 7072 696e 672e 6874 6d6c  ubberspring.html
+000004a0: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+000004b0: 733a 2f2f 7573 6572 2d69 6d61 6765 732e  s://user-images.
+000004c0: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+000004d0: 742e 636f 6d2f 3537 3933 3135 332f 3233  t.com/5793153/23
+000004e0: 3036 3034 3234 362d 3561 3431 3630 3831  0604246-5a416081
+000004f0: 2d36 3737 372d 3466 3333 2d61 6664 662d  -6777-4f33-afdf-
+00000500: 6566 6462 3531 3333 3837 3232 2e70 6e67  efdb51338722.png
+00000510: 2220 6865 6967 6874 3d22 3132 3070 7822  " height="120px"
+00000520: 2f3e 3c2f 613e 203c 6120 6872 6566 3d22  /></a> <a href="
+00000530: 6874 7470 733a 2f2f 6665 6c75 7065 2e72  https://felupe.r
+00000540: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00000550: 2f6c 6174 6573 742f 6578 616d 706c 6573  /latest/examples
+00000560: 2f70 6c61 7465 7769 7468 686f 6c65 2e68  /platewithhole.h
+00000570: 746d 6c22 3e3c 696d 6720 7372 633d 2268  tml"><img src="h
+00000580: 7474 7073 3a2f 2f75 7365 722d 696d 6167  ttps://user-imag
+00000590: 6573 2e67 6974 6875 6275 7365 7263 6f6e  es.githubusercon
+000005a0: 7465 6e74 2e63 6f6d 2f35 3739 3331 3533  tent.com/5793153
+000005b0: 2f32 3330 3630 3435 3837 2d34 3265 3365  /230604587-42e3e
+000005c0: 3333 392d 6530 3863 2d34 6363 382d 3830  339-e08c-4cc8-80
+000005d0: 3030 2d66 3730 3436 6138 6439 3564 662e  00-f7046a8d95df.
+000005e0: 706e 6722 2068 6569 6768 743d 2231 3230  png" height="120
+000005f0: 7078 222f 3e3c 2f61 3e0a 3c2f 703e 0a0a  px"/></a>.</p>..
+00000600: 4645 6c75 7065 2069 7320 6120 5079 7468  FElupe is a Pyth
+00000610: 6f6e 2033 2e37 2b20 6669 6e69 7465 2065  on 3.7+ finite e
+00000620: 6c65 6d65 6e74 2061 6e61 6c79 7369 7320  lement analysis 
+00000630: 7061 636b 6167 6520 666f 6375 7373 696e  package focussin
+00000640: 6720 6f6e 2074 6865 2066 6f72 6d75 6c61  g on the formula
+00000650: 7469 6f6e 2061 6e64 206e 756d 6572 6963  tion and numeric
+00000660: 616c 2073 6f6c 7574 696f 6e20 6f66 206e  al solution of n
+00000670: 6f6e 6c69 6e65 6172 2070 726f 626c 656d  onlinear problem
+00000680: 7320 696e 2063 6f6e 7469 6e75 756d 206d  s in continuum m
+00000690: 6563 6861 6e69 6373 206f 6620 736f 6c69  echanics of soli
+000006a0: 6420 626f 6469 6573 2e20 4974 7320 6e61  d bodies. Its na
+000006b0: 6d65 2069 7320 6120 636f 6d62 696e 6174  me is a combinat
+000006c0: 696f 6e20 6f66 2046 4520 2866 696e 6974  ion of FE (finit
+000006d0: 6520 656c 656d 656e 7429 2061 6e64 2074  e element) and t
+000006e0: 6865 2067 6572 6d61 6e20 776f 7264 202a  he german word *
+000006f0: 4c75 7065 2a20 286d 6167 6e69 6679 696e  Lupe* (magnifyin
+00000700: 6720 676c 6173 7329 2061 7320 6120 7379  g glass) as a sy
+00000710: 6e6f 6e79 6d20 666f 7220 6765 7474 696e  nonym for gettin
+00000720: 6720 616e 2069 6e73 6967 6874 2068 6f77  g an insight how
+00000730: 2061 2066 696e 6974 6520 656c 656d 656e   a finite elemen
+00000740: 7420 616e 616c 7973 6973 2063 6f64 6520  t analysis code 
+00000750: 6c6f 6f6b 7320 6c69 6b65 2075 6e64 6572  looks like under
+00000760: 2074 6865 2068 6f6f 642e 0a0a 2320 496e   the hood...# In
+00000770: 7374 616c 6c61 7469 6f6e 0a49 6e73 7461  stallation.Insta
+00000780: 6c6c 2050 7974 686f 6e2c 2066 6972 6520  ll Python, fire 
+00000790: 7570 2061 2074 6572 6d69 6e61 6c20 616e  up a terminal an
+000007a0: 6420 7275 6e0a 0a60 6060 7368 656c 6c0a  d run..```shell.
+000007b0: 7069 7020 696e 7374 616c 6c20 6665 6c75  pip install felu
+000007c0: 7065 5b61 6c6c 5d0a 6060 600a 0a77 6865  pe[all].```..whe
+000007d0: 7265 2060 5b61 6c6c 5d60 2069 6e73 7461  re `[all]` insta
+000007e0: 6c6c 7320 616c 6c20 6f70 7469 6f6e 616c  lls all optional
+000007f0: 2064 6570 656e 6465 6e63 6965 732e 2042   dependencies. B
+00000800: 7920 6465 6661 756c 742c 2046 456c 7570  y default, FElup
+00000810: 6520 6465 7065 6e64 7320 6f6e 2060 6e75  e depends on `nu
+00000820: 6d70 7960 2061 6e64 2060 7363 6970 7960  mpy` and `scipy`
+00000830: 2e20 496e 206f 7264 6572 2074 6f20 6d61  . In order to ma
+00000840: 6b65 2075 7365 206f 6620 616c 6c20 6665  ke use of all fe
+00000850: 6174 7572 6573 206f 6620 4645 6c75 7065  atures of FElupe
+00000860: 2c20 6974 2069 7320 7375 6767 6573 7465  , it is suggeste
+00000870: 6420 746f 2069 6e73 7461 6c6c 2061 6c6c  d to install all
+00000880: 206f 7074 696f 6e61 6c20 6465 7065 6e64   optional depend
+00000890: 656e 6369 6573 2028 6065 696e 7375 6d74  encies (`einsumt
+000008a0: 602c 2060 6835 7079 602c 2060 6d61 7470  `, `h5py`, `matp
+000008b0: 6c6f 746c 6962 602c 2060 6d65 7368 696f  lotlib`, `meshio
+000008c0: 6020 616e 6420 6074 656e 736f 7274 7261  ` and `tensortra
+000008d0: 7860 292e 0a0a 2320 4765 7474 696e 6720  x`)...# Getting 
+000008e0: 5374 6172 7465 640a 4120 7175 6172 7465  Started.A quarte
+000008f0: 7220 6d6f 6465 6c20 6f66 2061 2073 6f6c  r model of a sol
+00000900: 6964 2063 7562 6520 7769 7468 2068 7970  id cube with hyp
+00000910: 6572 656c 6173 7469 6320 6d61 7465 7269  erelastic materi
+00000920: 616c 2062 6568 6176 696f 7572 2069 7320  al behaviour is 
+00000930: 7375 626a 6563 7465 6420 746f 2061 2075  subjected to a u
+00000940: 6e69 6178 6961 6c20 656c 6f6e 6761 7469  niaxial elongati
+00000950: 6f6e 2061 7070 6c69 6564 2061 7420 6120  on applied at a 
+00000960: 636c 616d 7065 6420 656e 642d 6661 6365  clamped end-face
+00000970: 2e20 5468 6973 2069 6e76 6f6c 7665 7320  . This involves 
+00000980: 7468 6520 6372 6561 7469 6f6e 206f 6620  the creation of 
+00000990: 6120 6d65 7368 2c20 6120 7265 6769 6f6e  a mesh, a region
+000009a0: 2061 7320 7765 6c6c 2061 7320 6120 6469   as well as a di
+000009b0: 7370 6c61 6365 6d65 6e74 2066 6965 6c64  splacement field
+000009c0: 2028 656e 6361 7073 756c 6174 6564 2069   (encapsulated i
+000009d0: 6e20 6120 6669 656c 6420 636f 6e74 6169  n a field contai
+000009e0: 6e65 7229 2e20 4675 7274 6865 726d 6f72  ner). Furthermor
+000009f0: 652c 2074 6865 2062 6f75 6e64 6172 7920  e, the boundary 
+00000a00: 636f 6e64 6974 696f 6e73 2061 7265 2063  conditions are c
+00000a10: 7265 6174 6564 2062 7920 6120 7465 6d70  reated by a temp
+00000a20: 6c61 7465 2066 6f72 2061 2075 6e69 6178  late for a uniax
+00000a30: 6961 6c20 6c6f 6164 6361 7365 2e20 416e  ial loadcase. An
+00000a40: 2069 736f 7472 6f70 6963 2070 7365 7564   isotropic pseud
+00000a50: 6f2d 656c 6173 7469 6320 4f67 6465 6e2d  o-elastic Ogden-
+00000a60: 526f 7862 7572 6768 204d 756c 6c69 6e73  Roxburgh Mullins
+00000a70: 2d73 6f66 7465 6e69 6e67 206d 6f64 656c  -softening model
+00000a80: 2066 6f72 6d75 6c61 7469 6f6e 2069 6e20   formulation in 
+00000a90: 636f 6d62 696e 6174 696f 6e20 7769 7468  combination with
+00000aa0: 2061 6e20 6973 6f74 726f 7069 6320 6879   an isotropic hy
+00000ab0: 7065 7265 6c61 7374 6963 204e 656f 2d48  perelastic Neo-H
+00000ac0: 6f6f 6b65 616e 206d 6174 6572 6961 6c20  ookean material 
+00000ad0: 666f 726d 756c 6174 696f 6e20 6973 2061  formulation is a
+00000ae0: 7070 6c69 6564 206f 6e20 6120 6e65 6172  pplied on a near
+00000af0: 6c79 2d69 6e63 6f6d 7072 6573 7369 626c  ly-incompressibl
+00000b00: 6520 736f 6c69 6420 626f 6479 2e20 4120  e solid body. A 
+00000b10: 7374 6570 2067 656e 6572 6174 6573 2074  step generates t
+00000b20: 6865 2063 6f6e 7365 6375 7469 7665 2073  he consecutive s
+00000b30: 7562 7374 6570 2d6d 6f76 656d 656e 7473  ubstep-movements
+00000b40: 206f 6620 6120 6769 7665 6e20 626f 756e   of a given boun
+00000b50: 6461 7279 2063 6f6e 6469 7469 6f6e 2e20  dary condition. 
+00000b60: 5468 6520 7374 6570 2069 7320 6675 7274  The step is furt
+00000b70: 6865 7220 6164 6465 6420 746f 2061 206c  her added to a l
+00000b80: 6973 7420 6f66 2073 7465 7073 206f 6620  ist of steps of 
+00000b90: 6120 6a6f 6220 2868 6572 652c 2061 2063  a job (here, a c
+00000ba0: 6861 7261 6374 6572 6973 7469 632d 6375  haracteristic-cu
+00000bb0: 7276 6520 6a6f 6220 6973 2075 7365 6429  rve job is used)
+00000bc0: 2e20 4475 7269 6e67 2065 7661 6c75 6174  . During evaluat
+00000bd0: 696f 6e2c 2065 6163 6820 7375 6273 7465  ion, each subste
+00000be0: 7020 6f66 2065 6163 6820 7374 6570 2069  p of each step i
+00000bf0: 7320 736f 6c76 6564 2062 7920 616e 2069  s solved by an i
+00000c00: 7465 7261 7469 7665 204e 6577 746f 6e2d  terative Newton-
+00000c10: 5268 6170 736f 6e20 7072 6f63 6564 7572  Rhapson procedur
+00000c20: 652e 2054 6865 2073 6f6c 7574 696f 6e20  e. The solution 
+00000c30: 6973 2065 7870 6f72 7465 6420 6166 7465  is exported afte
+00000c40: 7220 6561 6368 2063 6f6d 706c 6574 6564  r each completed
+00000c50: 2073 7562 7374 6570 2061 7320 6120 7469   substep as a ti
+00000c60: 6d65 2d73 6572 6965 7320 5844 4d46 2066  me-series XDMF f
+00000c70: 696c 652e 2046 6f72 206d 6f72 6520 6465  ile. For more de
+00000c80: 7461 696c 7320 6265 7369 6465 2074 6869  tails beside thi
+00000c90: 7320 6869 6768 2d6c 6576 656c 2063 6f64  s high-level cod
+00000ca0: 6520 736e 6970 7065 742c 2070 6c65 6173  e snippet, pleas
+00000cb0: 6520 6861 7665 2061 206c 6f6f 6b20 6174  e have a look at
+00000cc0: 2074 6865 205b 646f 6375 6d65 6e74 6174   the [documentat
+00000cd0: 696f 6e5d 2868 7474 7073 3a2f 2f66 656c  ion](https://fel
+00000ce0: 7570 652e 7265 6164 7468 6564 6f63 732e  upe.readthedocs.
+00000cf0: 696f 2f65 6e2f 6c61 7465 7374 2f3f 6261  io/en/latest/?ba
+00000d00: 6467 653d 6c61 7465 7374 292e 0a0a 6060  dge=latest)...``
+00000d10: 6070 7974 686f 6e0a 696d 706f 7274 2066  `python.import f
+00000d20: 656c 7570 6520 6173 2066 656d 0a0a 2320  elupe as fem..# 
+00000d30: 6372 6561 7465 2061 2068 6578 6168 6564  create a hexahed
+00000d40: 726f 6e2d 7265 6769 6f6e 206f 6e20 6120  ron-region on a 
+00000d50: 6375 6265 0a6d 6573 6820 3d20 6665 6d2e  cube.mesh = fem.
+00000d60: 4375 6265 286e 3d31 3129 0a72 6567 696f  Cube(n=11).regio
+00000d70: 6e20 3d20 6665 6d2e 5265 6769 6f6e 4865  n = fem.RegionHe
+00000d80: 7861 6865 6472 6f6e 286d 6573 6829 0a0a  xahedron(mesh)..
+00000d90: 2320 6164 6420 6120 6669 656c 6420 636f  # add a field co
+00000da0: 6e74 6169 6e65 7220 2877 6974 6820 6120  ntainer (with a 
+00000db0: 7665 6374 6f72 2d76 616c 7565 6420 6469  vector-valued di
+00000dc0: 7370 6c61 6365 6d65 6e74 2066 6965 6c64  splacement field
+00000dd0: 290a 6669 656c 6420 3d20 6665 6d2e 4669  ).field = fem.Fi
+00000de0: 656c 6443 6f6e 7461 696e 6572 285b 6665  eldContainer([fe
+00000df0: 6d2e 4669 656c 6428 7265 6769 6f6e 2c20  m.Field(region, 
+00000e00: 6469 6d3d 3329 5d29 0a0a 2320 6170 706c  dim=3)])..# appl
+00000e10: 7920 6120 756e 6961 7869 616c 2065 6c6f  y a uniaxial elo
+00000e20: 6e67 6174 696f 6e20 6f6e 2074 6865 2063  ngation on the c
+00000e30: 7562 650a 626f 756e 6461 7269 6573 203d  ube.boundaries =
+00000e40: 2066 656d 2e64 6f66 2e75 6e69 6178 6961   fem.dof.uniaxia
+00000e50: 6c28 6669 656c 642c 2063 6c61 6d70 6564  l(field, clamped
+00000e60: 3d54 7275 6529 5b30 5d0a 0a23 2064 6566  =True)[0]..# def
+00000e70: 696e 6520 7468 6520 636f 6e73 7469 7475  ine the constitu
+00000e80: 7469 7665 206d 6174 6572 6961 6c20 6265  tive material be
+00000e90: 6861 7669 6f75 720a 2320 616e 6420 6372  haviour.# and cr
+00000ea0: 6561 7465 2061 206e 6561 726c 792d 696e  eate a nearly-in
+00000eb0: 636f 6d70 7265 7373 6962 6c65 2028 752c  compressible (u,
+00000ec0: 702c 4a20 2d20 666f 726d 756c 6174 696f  p,J - formulatio
+00000ed0: 6e29 2073 6f6c 6964 2062 6f64 790a 756d  n) solid body.um
+00000ee0: 6174 203d 2066 656d 2e4f 6764 656e 526f  at = fem.OgdenRo
+00000ef0: 7862 7572 6768 286d 6174 6572 6961 6c3d  xburgh(material=
+00000f00: 6665 6d2e 4e65 6f48 6f6f 6b65 286d 753d  fem.NeoHooke(mu=
+00000f10: 3129 2c20 723d 332c 206d 3d31 2c20 6265  1), r=3, m=1, be
+00000f20: 7461 3d30 290a 736f 6c69 6420 3d20 6665  ta=0).solid = fe
+00000f30: 6d2e 536f 6c69 6442 6f64 794e 6561 726c  m.SolidBodyNearl
+00000f40: 7949 6e63 6f6d 7072 6573 7369 626c 6528  yIncompressible(
+00000f50: 756d 6174 2c20 6669 656c 642c 2062 756c  umat, field, bul
+00000f60: 6b3d 3530 3030 290a 0a23 2070 7265 7061  k=5000)..# prepa
+00000f70: 7265 2061 2073 7465 7020 7769 7468 2073  re a step with s
+00000f80: 7562 7374 6570 730a 6d6f 7665 203d 2066  ubsteps.move = f
+00000f90: 656d 2e6d 6174 682e 6c69 6e73 7465 7073  em.math.linsteps
+00000fa0: 285b 302c 2032 2c20 305d 2c20 6e75 6d3d  ([0, 2, 0], num=
+00000fb0: 3130 290a 7374 6570 203d 2066 656d 2e53  10).step = fem.S
+00000fc0: 7465 7028 6974 656d 733d 5b73 6f6c 6964  tep(items=[solid
+00000fd0: 5d2c 2072 616d 703d 7b62 6f75 6e64 6172  ], ramp={boundar
+00000fe0: 6965 735b 226d 6f76 6522 5d3a 206d 6f76  ies["move"]: mov
+00000ff0: 657d 2c20 626f 756e 6461 7269 6573 3d62  e}, boundaries=b
+00001000: 6f75 6e64 6172 6965 7329 0a0a 2320 6164  oundaries)..# ad
+00001010: 6420 7468 6520 7374 6570 2074 6f20 6120  d the step to a 
+00001020: 6a6f 622c 2065 7661 6c75 6174 6520 616c  job, evaluate al
+00001030: 6c20 7375 6273 7465 7073 2061 6e64 2063  l substeps and c
+00001040: 7265 6174 6520 6120 706c 6f74 0a6a 6f62  reate a plot.job
+00001050: 203d 2066 656d 2e43 6861 7261 6374 6572   = fem.Character
+00001060: 6973 7469 6343 7572 7665 2873 7465 7073  isticCurve(steps
+00001070: 3d5b 7374 6570 5d2c 2062 6f75 6e64 6172  =[step], boundar
+00001080: 793d 626f 756e 6461 7269 6573 5b22 6d6f  y=boundaries["mo
+00001090: 7665 225d 290a 6a6f 622e 6576 616c 7561  ve"]).job.evalua
+000010a0: 7465 2866 696c 656e 616d 653d 2272 6573  te(filename="res
+000010b0: 756c 742e 7864 6d66 2229 0a66 6967 2c20  ult.xdmf").fig, 
+000010c0: 6178 203d 206a 6f62 2e70 6c6f 7428 0a20  ax = job.plot(. 
+000010d0: 2020 2078 6c61 6265 6c3d 2244 6973 706c     xlabel="Displ
+000010e0: 6163 656d 656e 7420 2475 2420 696e 206d  acement $u$ in m
+000010f0: 6d20 245c 6c6f 6e67 7269 6768 7461 7272  m $\longrightarr
+00001100: 6f77 2422 2c0a 2020 2020 796c 6162 656c  ow$",.    ylabel
+00001110: 3d22 4e6f 726d 616c 2046 6f72 6365 2024  ="Normal Force $
+00001120: 4624 2069 6e20 4e20 245c 6c6f 6e67 7269  F$ in N $\longri
+00001130: 6768 7461 7272 6f77 2422 2c0a 290a 6060  ghtarrow$",.).``
+00001140: 600a 0a68 7474 7073 3a2f 2f75 7365 722d  `..https://user-
+00001150: 696d 6167 6573 2e67 6974 6875 6275 7365  images.githubuse
+00001160: 7263 6f6e 7465 6e74 2e63 6f6d 2f35 3739  rcontent.com/579
+00001170: 3331 3533 2f32 3030 3935 3133 3831 2d65  3153/200951381-e
+00001180: 6133 3130 6535 342d 3736 3233 2d34 6464  a310e54-7623-4dd
+00001190: 312d 6135 3566 2d61 3238 6639 3035 3530  1-a55f-a28f90550
+000011a0: 3633 662e 6d70 340a 0a3c 696d 6720 7372  63f.mp4..<img sr
+000011b0: 633d 2268 7474 7073 3a2f 2f72 6177 2e67  c="https://raw.g
+000011c0: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+000011d0: 2e63 6f6d 2f61 6474 7a6c 722f 6665 6c75  .com/adtzlr/felu
+000011e0: 7065 2f6d 6169 6e2f 646f 6373 2f5f 7374  pe/main/docs/_st
+000011f0: 6174 6963 2f72 6561 646d 655f 6368 6172  atic/readme_char
+00001200: 6163 7465 7269 7374 6963 5f63 7572 7665  acteristic_curve
+00001210: 2e73 7667 2220 7769 6474 683d 2236 3030  .svg" width="600
+00001220: 7078 222f 3e0a 0a23 2044 6f63 756d 656e  px"/>..# Documen
+00001230: 7461 7469 6f6e 0a54 6865 2064 6f63 756d  tation.The docum
+00001240: 656e 7461 7469 6f6e 2069 7320 6c6f 6361  entation is loca
+00001250: 7465 6420 5b68 6572 655d 2868 7474 7073  ted [here](https
+00001260: 3a2f 2f66 656c 7570 652e 7265 6164 7468  ://felupe.readth
+00001270: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00001280: 7374 2f3f 6261 6467 653d 6c61 7465 7374  st/?badge=latest
+00001290: 292e 0a0a 2320 4578 7465 6e73 696f 6e20  )...# Extension 
+000012a0: 5061 636b 6167 6573 0a54 6865 2063 6170  Packages.The cap
+000012b0: 6162 696c 6974 6965 7320 6f66 2046 456c  abilities of FEl
+000012c0: 7570 6520 6d61 7920 6265 2065 6e68 616e  upe may be enhan
+000012d0: 6365 6420 7769 7468 2065 7874 656e 7369  ced with extensi
+000012e0: 6f6e 2070 6163 6b61 6765 7320 6372 6561  on packages crea
+000012f0: 7465 6420 6279 2074 6865 2063 6f6d 6d75  ted by the commu
+00001300: 6e69 7479 2e0a 0a7c 202a 2a50 6163 6b61  nity...| **Packa
+00001310: 6765 2a2a 207c 2020 2020 2020 2020 2020  ge** |          
+00001320: 2020 2020 2020 2020 2020 202a 2a44 6573             **Des
+00001330: 6372 6970 7469 6f6e 2a2a 2020 2020 2020  cription**      
+00001340: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001360: 2a2a 4c69 6e6b 2a2a 2020 2020 2020 2020  **Link**        
+00001370: 2020 2020 2020 207c 0a7c 3a2d 2d2d 2d2d         |.|:-----
+00001380: 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d  ------:|:-------
+00001390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013c0: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|:-------------
+000013d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013e0: 2d2d 2d2d 2d2d 2d2d 3a7c 0a7c 2020 7465  --------:|.|  te
+000013f0: 6e73 6f72 7472 6178 207c 2020 2020 204d  nsortrax |     M
+00001400: 6174 6820 6f6e 2028 4879 7065 722d 4475  ath on (Hyper-Du
+00001410: 616c 2920 5465 6e73 6f72 7320 7769 7468  al) Tensors with
+00001420: 2054 7261 696c 696e 6720 4178 6573 2020   Trailing Axes  
+00001430: 2020 207c 2020 6874 7470 733a 2f2f 6769     |  https://gi
+00001440: 7468 7562 2e63 6f6d 2f61 6474 7a6c 722f  thub.com/adtzlr/
+00001450: 7465 6e73 6f72 7472 6178 207c 0a7c 2020  tensortrax |.|  
+00001460: 2020 6d61 7441 4469 2020 207c 204d 6174    matADi   | Mat
+00001470: 6572 6961 6c20 4465 6669 6e69 7469 6f6e  erial Definition
+00001480: 2077 6974 6820 4175 746f 6d61 7469 6320   with Automatic 
+00001490: 4469 6666 6572 656e 7469 6174 696f 6e20  Differentiation 
+000014a0: 2841 4429 207c 2020 2020 6874 7470 733a  (AD) |    https:
+000014b0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 6474  //github.com/adt
+000014c0: 7a6c 722f 6d61 7461 6469 2020 207c 0a7c  zlr/matadi   |.|
+000014d0: 2020 2020 4645 706c 6f74 2020 207c 2020      FEplot   |  
+000014e0: 2020 2020 2020 2020 2020 2041 2076 6973             A vis
+000014f0: 7561 6c69 7a61 7469 6f6e 2074 6f6f 6c20  ualization tool 
+00001500: 666f 7220 4645 6c75 7065 2020 2020 2020  for FElupe      
+00001510: 2020 2020 2020 207c 2068 7474 7073 3a2f         | https:/
+00001520: 2f67 6974 6875 622e 636f 6d2f 5a41 4152  /github.com/ZAAR
+00001530: 414f 5549 3939 392f 6665 706c 6f74 207c  AOUI999/feplot |
+00001540: 0a0a 2320 4368 616e 6765 6c6f 670a 416c  ..# Changelog.Al
+00001550: 6c20 6e6f 7461 626c 6520 6368 616e 6765  l notable change
+00001560: 7320 746f 2074 6869 7320 7072 6f6a 6563  s to this projec
+00001570: 7420 7769 6c6c 2062 6520 646f 6375 6d65  t will be docume
+00001580: 6e74 6564 2069 6e20 5b74 6869 7320 6669  nted in [this fi
+00001590: 6c65 5d28 4348 414e 4745 4c4f 472e 6d64  le](CHANGELOG.md
+000015a0: 292e 2054 6865 2066 6f72 6d61 7420 6973  ). The format is
+000015b0: 2062 6173 6564 206f 6e20 5b4b 6565 7020   based on [Keep 
+000015c0: 6120 4368 616e 6765 6c6f 675d 2868 7474  a Changelog](htt
+000015d0: 7073 3a2f 2f6b 6565 7061 6368 616e 6765  ps://keepachange
+000015e0: 6c6f 672e 636f 6d2f 656e 2f31 2e30 2e30  log.com/en/1.0.0
+000015f0: 2f29 2c20 616e 6420 7468 6973 2070 726f  /), and this pro
+00001600: 6a65 6374 2061 6468 6572 6573 2074 6f20  ject adheres to 
+00001610: 5b53 656d 616e 7469 6320 5665 7273 696f  [Semantic Versio
+00001620: 6e69 6e67 5d28 6874 7470 733a 2f2f 7365  ning](https://se
+00001630: 6d76 6572 2e6f 7267 2f73 7065 632f 7632  mver.org/spec/v2
+00001640: 2e30 2e30 2e68 746d 6c29 2e0a 0a23 204c  .0.0.html)...# L
+00001650: 6963 656e 7365 0a46 456c 7570 6520 2d20  icense.FElupe - 
+00001660: 6669 6e69 7465 2065 6c65 6d65 6e74 2061  finite element a
+00001670: 6e61 6c79 7369 7320 2843 2920 3230 3233  nalysis (C) 2023
+00001680: 2041 6e64 7265 6173 2044 7574 7a6c 6572   Andreas Dutzler
+00001690: 2c20 4772 617a 2028 4175 7374 7269 6129  , Graz (Austria)
+000016a0: 2e0a 0a54 6869 7320 7072 6f67 7261 6d20  ...This program 
+000016b0: 6973 2066 7265 6520 736f 6674 7761 7265  is free software
+000016c0: 3a20 796f 7520 6361 6e20 7265 6469 7374  : you can redist
+000016d0: 7269 6275 7465 2069 7420 616e 642f 6f72  ribute it and/or
+000016e0: 206d 6f64 6966 7920 6974 2075 6e64 6572   modify it under
+000016f0: 2074 6865 2074 6572 6d73 206f 6620 7468   the terms of th
+00001700: 6520 474e 5520 4765 6e65 7261 6c20 5075  e GNU General Pu
+00001710: 626c 6963 204c 6963 656e 7365 2061 7320  blic License as 
+00001720: 7075 626c 6973 6865 6420 6279 2074 6865  published by the
+00001730: 2046 7265 6520 536f 6674 7761 7265 2046   Free Software F
+00001740: 6f75 6e64 6174 696f 6e2c 2065 6974 6865  oundation, eithe
+00001750: 7220 7665 7273 696f 6e20 3320 6f66 2074  r version 3 of t
+00001760: 6865 204c 6963 656e 7365 2c20 6f72 2028  he License, or (
+00001770: 6174 2079 6f75 7220 6f70 7469 6f6e 2920  at your option) 
+00001780: 616e 7920 6c61 7465 7220 7665 7273 696f  any later versio
+00001790: 6e2e 0a0a 5468 6973 2070 726f 6772 616d  n...This program
+000017a0: 2069 7320 6469 7374 7269 6275 7465 6420   is distributed 
+000017b0: 696e 2074 6865 2068 6f70 6520 7468 6174  in the hope that
+000017c0: 2069 7420 7769 6c6c 2062 6520 7573 6566   it will be usef
+000017d0: 756c 2c20 6275 7420 5749 5448 4f55 5420  ul, but WITHOUT 
+000017e0: 414e 5920 5741 5252 414e 5459 3b20 7769  ANY WARRANTY; wi
+000017f0: 7468 6f75 7420 6576 656e 2074 6865 2069  thout even the i
+00001800: 6d70 6c69 6564 2077 6172 7261 6e74 7920  mplied warranty 
+00001810: 6f66 204d 4552 4348 414e 5441 4249 4c49  of MERCHANTABILI
+00001820: 5459 206f 7220 4649 544e 4553 5320 464f  TY or FITNESS FO
+00001830: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
+00001840: 5552 504f 5345 2e20 5365 6520 7468 6520  URPOSE. See the 
+00001850: 474e 5520 4765 6e65 7261 6c20 5075 626c  GNU General Publ
+00001860: 6963 204c 6963 656e 7365 2066 6f72 206d  ic License for m
+00001870: 6f72 6520 6465 7461 696c 732e 0a0a 596f  ore details...Yo
+00001880: 7520 7368 6f75 6c64 2068 6176 6520 7265  u should have re
+00001890: 6365 6976 6564 2061 2063 6f70 7920 6f66  ceived a copy of
+000018a0: 2074 6865 2047 4e55 2047 656e 6572 616c   the GNU General
+000018b0: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+000018c0: 616c 6f6e 6720 7769 7468 2074 6869 7320  along with this 
+000018d0: 7072 6f67 7261 6d2e 2049 6620 6e6f 742c  program. If not,
+000018e0: 2073 6565 203c 6874 7470 733a 2f2f 7777   see <https://ww
+000018f0: 772e 676e 752e 6f72 672f 6c69 6365 6e73  w.gnu.org/licens
+00001900: 6573 2f3e 2e0a                           es/>..
```

### Comparing `felupe-7.0.0/pyproject.toml` & `felupe-7.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,21 +40,28 @@
   "Topic :: Utilities"
 ]
 dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
   "numpy",
   "scipy",
-  "einsumt",
 ]
 
 [project.optional-dependencies]
-all = [
+test = [
+    "h5py",
+    "matplotlib",
     "meshio",
+    "tensortrax",
+]
+all = [
+    "einsumt",
     "h5py",
+    "matplotlib",
+    "meshio",
     "tensortrax",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "felupe.__about__.__version__"}
 
 [project.urls]
```

### Comparing `felupe-7.0.0/src/felupe/__init__.py` & `felupe-7.1.0/src/felupe/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/_assembly/_axi.py` & `felupe-7.1.0/src/felupe/_assembly/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/_assembly/_base.py` & `felupe-7.1.0/src/felupe/_assembly/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,20 @@
 
 You should have received a copy of the GNU General Public License
 along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
 import numpy as np
-from einsumt import einsumt
+
+try:
+    from einsumt import einsumt
+except ModuleNotFoundError:
+    from numpy import einsum as einsumt
+
 from scipy.sparse import csr_matrix as sparsematrix
 
 
 class IntegralForm:
     r"""Integral Form constructed by a function result ``fun``,
     a virtual field ``v``, differential volumes ``dV`` and optionally a
     field ``u``. For both fields ``v`` and ``u`` gradients may be passed by
```

### Comparing `felupe-7.0.0/src/felupe/_assembly/_form.py` & `felupe-7.1.0/src/felupe/_assembly/_form.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/_assembly/_mixed.py` & `felupe-7.1.0/src/felupe/_assembly/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/_basis/_basis.py` & `felupe-7.1.0/src/felupe/_basis/_basis.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 
 You should have received a copy of the GNU General Public License
 along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
 import numpy as np
-from einsumt import einsumt
+
+try:
+    from einsumt import einsumt
+except ModuleNotFoundError:
+    from numpy import einsum as einsumt
 
 
 class Basis:
     r"""A basis and its gradient built on top of a scalar- or vector-valued
     field. *Basis* refers to the trial and test field, either values or
     gradients evaluated at quadrature points. The first two indices of a basis
     are used for looping over the element shape functions ``a`` and its
```

### Comparing `felupe-7.0.0/src/felupe/_field/_axi.py` & `felupe-7.1.0/src/felupe/_field/_axi.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/_field/_base.py` & `felupe-7.1.0/src/felupe/_field/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/_field/_container.py` & `felupe-7.1.0/src/felupe/_field/_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,25 @@
         self.fields = fields
         self.region = fields[0].region
 
         # get sizes of fields and calculate offsets
         self.fieldsizes = [f.indices.dof.size for f in self.fields]
         self.offsets = np.cumsum(self.fieldsizes)[:-1]
 
+    def __repr__(self):
+        header = "<felupe FieldContainer object>"
+        size = f"  Number of fields: {len(self.fields)}"
+        fields_header = "  Dimension of fields:"
+        fields = [
+            f"    {type(field).__name__}: {field.dim}"
+            for a, field in enumerate(self.fields)
+        ]
+
+        return "\n".join([header, size, fields_header, *fields])
+
     def extract(self, grad=True, sym=False, add_identity=True):
         """Generalized extraction method which evaluates either the gradient
         or the field values at the integration points of all cells
         in the region. Optionally, the symmetric part of the gradient is
         evaluated and/or the identity matrix is added to the gradient.
 
         Arguments
```

### Comparing `felupe-7.0.0/src/felupe/_field/_fields.py` & `felupe-7.1.0/src/felupe/_field/_fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -98,30 +98,41 @@
             RegionTriQuadraticHexahedron: RegionHexahedron,
             RegionQuadraticTetra: RegionTetra,
             RegionQuadraticTriangle: RegionTriangle,
             RegionTetraMINI: RegionTetra,
             RegionTriangleMINI: RegionTriangle,
             RegionLagrange: RegionLagrange,
         }
+        points_per_cell = {
+            RegionConstantHexahedron: 1,
+            RegionConstantQuad: 1,
+            RegionQuad: 4,
+            RegionHexahedron: 8,
+            RegionTriangle: 3,
+            RegionTetra: 4,
+            RegionLagrange: None,
+        }
 
         kwargs0 = {}
 
-        if offset > 0:
-            kwargs0["offset"] = offset
-        if npoints is not None:
-            kwargs0["npoints"] = npoints
-
         if isinstance(region, RegionLagrange):
             kwargs0["order"] = region.order - 1
             kwargs0["dim"] = region.mesh.dim
+            points_per_cell[RegionLagrange] = region.order**region.element.dim
+
+        RegionDual = regions[type(region)]
 
-        if mesh is None:
-            mesh = region.mesh
+        if mesh is None and points_per_cell[RegionDual] is not None:
+            mesh = region.mesh.dual(
+                points_per_cell=points_per_cell[RegionDual],
+                offset=offset,
+                npoints=npoints,
+            )
 
-        region_dual = regions[type(region)](
+        region_dual = RegionDual(
             mesh,
             quadrature=region.quadrature,
             grad=False,
             **{**kwargs0, **kwargs},
         )
 
         if axisymmetric is False and planestrain is False:
```

### Comparing `felupe-7.0.0/src/felupe/_field/_indices.py` & `felupe-7.1.0/src/felupe/_field/_indices.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/_field/_planestrain.py` & `felupe-7.1.0/src/felupe/_field/_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/constitution/__init__.py` & `felupe-7.1.0/src/felupe/constitution/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/constitution/_kinematics.py` & `felupe-7.1.0/src/felupe/constitution/_kinematics.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 
 You should have received a copy of the GNU General Public License
 along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
 import numpy as np
-from einsumt import einsumt
+
+try:
+    from einsumt import einsumt
+except ModuleNotFoundError:
+    from numpy import einsum as einsumt
 
 from ..math import cdya_ik, cdya_il, det, dot, dya, identity, inv, transpose
 
 
 class LineChange:
     r"""Line Change.
```

### Comparing `felupe-7.0.0/src/felupe/constitution/_mixed.py` & `felupe-7.1.0/src/felupe/constitution/_mixed.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/constitution/_models_hyperelasticity.py` & `felupe-7.1.0/src/felupe/constitution/_models_hyperelasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/constitution/_models_hyperelasticity_ad.py` & `felupe-7.1.0/src/felupe/constitution/_models_hyperelasticity_ad.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/constitution/_models_linear_elasticity.py` & `felupe-7.1.0/src/felupe/constitution/_models_linear_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/constitution/_models_pseudo_elasticity.py` & `felupe-7.1.0/src/felupe/constitution/_models_pseudo_elasticity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/constitution/_user_materials.py` & `felupe-7.1.0/src/felupe/constitution/_user_materials.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/constitution/_user_materials_hyperelastic.py` & `felupe-7.1.0/src/felupe/constitution/_user_materials_hyperelastic.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/constitution/_user_materials_models.py` & `felupe-7.1.0/src/felupe/constitution/_user_materials_models.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/dof/_boundary.py` & `felupe-7.1.0/src/felupe/dof/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/dof/_loadcase.py` & `felupe-7.1.0/src/felupe/dof/_loadcase.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/dof/_tools.py` & `felupe-7.1.0/src/felupe/dof/_tools.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/element/_base.py` & `felupe-7.1.0/src/felupe/element/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/element/_hexahedron.py` & `felupe-7.1.0/src/felupe/element/_hexahedron.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/element/_lagrange.py` & `felupe-7.1.0/src/felupe/element/_lagrange.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/element/_line.py` & `felupe-7.1.0/src/felupe/element/_line.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/element/_quad.py` & `felupe-7.1.0/src/felupe/element/_quad.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/element/_tetra.py` & `felupe-7.1.0/src/felupe/element/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/element/_triangle.py` & `felupe-7.1.0/src/felupe/element/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/math/_field.py` & `felupe-7.1.0/src/felupe/math/_field.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/math/_math.py` & `felupe-7.1.0/src/felupe/math/_math.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
 import numpy as np
 
 
-def linsteps(points, num=10):
+def linsteps(points, num=10, endpoint=True):
 
     points = np.array(points).ravel()
     start = points[:-1]
     end = points[1:]
     num = np.array([num]).ravel()
 
     if len(num) == 1:
@@ -45,10 +45,12 @@
     ]
     if len(steplist) > 0:
         steps = np.concatenate(
             [np.linspace(a, b, n, endpoint=False) for a, b, n in zip(start, end, num)]
         )
     else:
         steps = np.array([])
-    steps_with_endpoint = np.append(steps, points[-1])
 
-    return steps_with_endpoint
+    if endpoint:
+        steps = np.append(steps, points[-1])
+
+    return steps
```

### Comparing `felupe-7.0.0/src/felupe/math/_spatial.py` & `felupe-7.1.0/src/felupe/math/_spatial.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/math/_tensor.py` & `felupe-7.1.0/src/felupe/math/_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 
 You should have received a copy of the GNU General Public License
 along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
 import numpy as np
-from einsumt import einsumt
+
+try:
+    from einsumt import einsumt
+except ModuleNotFoundError:
+    from numpy import einsum as einsumt
 
 
 def identity(A=None, dim=None, shape=None):
     "Identity according to matrix A with optional specified dim."
     if A is not None:
         dimA, g, e = A.shape[-3:]
         if dim is None:
```

### Comparing `felupe-7.0.0/src/felupe/mechanics/_curve.py` & `felupe-7.1.0/src/felupe/mechanics/_curve.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,24 +72,24 @@
         xlabel="x",
         ylabel="y",
         xscale=1,
         yscale=1,
         gradient=False,
         fig=None,
         ax=None,
-        linestyle=".-",
         items=None,
         **kwargs
     ):
+        if self.res is None:
+            raise ValueError(
+                "Job results are empty. Run `job.evaluate()` and call `job.plot()` again."
+            )
 
         import matplotlib.pyplot as plt
 
-        if self.res is None:
-            self.evaluate(**kwargs)
-
         if x is None:
             x = self.x
         if y is None:
             y = self.y
 
         if items is None:
             items = slice(None)
@@ -102,12 +102,12 @@
             z = np.gradient(y, x[:, xaxis], edge_order=2, axis=0)
             cuttoff = np.mean(abs(z[:, yaxis])) + 2 * np.std(abs(z[:, yaxis]))
             y[abs(z) > cuttoff] = np.nan
 
         if fig is None or ax is None:
             fig, ax = plt.subplots()
 
-        ax.plot(x[:, xaxis] * xscale, y[:, yaxis] * yscale, linestyle)
+        ax.plot(x[:, xaxis] * xscale, y[:, yaxis] * yscale, **kwargs)
         ax.set_xlabel(xlabel)
         ax.set_ylabel(ylabel)
 
         return fig, ax
```

### Comparing `felupe-7.0.0/src/felupe/mechanics/_helpers.py` & `felupe-7.1.0/src/felupe/mechanics/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mechanics/_job.py` & `felupe-7.1.0/src/felupe/mechanics/_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         filename=None,
         mesh=None,
         point_data=None,
         cell_data=None,
         point_data_default=True,
         cell_data_default=True,
         verbose=True,
+        parallel=False,
         **kwargs,
     ):
 
         if verbose:
             print(
                 f"""
  _______  _______  ___      __   __  _______  _______ 
@@ -110,14 +111,19 @@
 
 """
             )
 
             print("Run Job")
             print("=======\n")
 
+        if parallel:
+            if not "kwargs" in kwargs.keys():
+                kwargs["kwargs"] = {}
+            kwargs["kwargs"]["parallel"] = True
+
         if filename is not None:
             from meshio.xdmf import TimeSeriesWriter
 
             if mesh is None:
                 if "x0" in kwargs.keys():
                     mesh = kwargs["x0"].region.mesh.as_meshio()
                 else:
```

### Comparing `felupe-7.0.0/src/felupe/mechanics/_multipoint.py` & `felupe-7.1.0/src/felupe/mechanics/_multipoint.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mechanics/_pointload.py` & `felupe-7.1.0/src/felupe/mechanics/_pointload.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mechanics/_solidbody.py` & `felupe-7.1.0/src/felupe/mechanics/_solidbody.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mechanics/_solidbody_gravity.py` & `felupe-7.1.0/src/felupe/mechanics/_solidbody_gravity.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mechanics/_solidbody_incompressible.py` & `felupe-7.1.0/src/felupe/mechanics/_solidbody_incompressible.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mechanics/_solidbody_pressure.py` & `felupe-7.1.0/src/felupe/mechanics/_solidbody_pressure.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mechanics/_step.py` & `felupe-7.1.0/src/felupe/mechanics/_step.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mesh/__init__.py` & `felupe-7.1.0/src/felupe/mesh/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     add_midpoints_faces,
     add_midpoints_volumes,
     collect_edges,
     collect_faces,
     collect_volumes,
     convert,
 )
+from ._dual import dual
 from ._geometry import (
     Cube,
     CubeArbitraryOrderHexahedron,
     Grid,
     Line,
     Rectangle,
     RectangleArbitraryOrderQuad,
@@ -25,10 +26,12 @@
     concatenate,
     expand,
     flip,
     mirror,
     revolve,
     rotate,
     runouts,
+    stack,
     sweep,
+    translate,
     triangulate,
 )
```

### Comparing `felupe-7.0.0/src/felupe/mesh/_base.py` & `felupe-7.1.0/src/felupe/mesh/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mesh/_container.py` & `felupe-7.1.0/src/felupe/mesh/_container.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mesh/_convert.py` & `felupe-7.1.0/src/felupe/mesh/_convert.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mesh/_discrete_geometry.py` & `felupe-7.1.0/src/felupe/mesh/_discrete_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mesh/_geometry.py` & `felupe-7.1.0/src/felupe/mesh/_geometry.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mesh/_helpers.py` & `felupe-7.1.0/src/felupe/mesh/_helpers.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mesh/_mesh.py` & `felupe-7.1.0/src/felupe/mesh/_mesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,26 @@
     add_midpoints_volumes,
     collect_edges,
     collect_faces,
     collect_volumes,
     convert,
 )
 from ._discrete_geometry import DiscreteGeometry
-from ._tools import expand, flip, mirror, revolve, rotate, runouts, sweep, triangulate
+from ._dual import dual
+from ._tools import (
+    expand,
+    flip,
+    mirror,
+    revolve,
+    rotate,
+    runouts,
+    sweep,
+    translate,
+    triangulate,
+)
 
 
 def as_mesh(obj):
     "Convert a ``DiscreteGeometry`` object to a ``Mesh`` object."
     return Mesh(points=obj.points, cells=obj.cells, cell_type=obj.cell_type)
 
 
@@ -77,15 +88,15 @@
         self.cell_type = cell_type
 
         super().__init__(points=points, cells=cells, cell_type=cell_type)
 
         self.__mesh__ = Mesh
 
     def __repr__(self):
-        header = "<felupe mesh object>"
+        header = "<felupe Mesh object>"
         points = f"  Number of points: {len(self.points)}"
         cells_header = "  Number of cells:"
         cells = [f"    {self.cell_type}: {self.ncells}"]
 
         return "\n".join([header, points, cells_header, *cells])
 
     def __str__(self):
@@ -93,31 +104,21 @@
 
     def disconnect(self, points_per_cell=None, calc_points=True):
         """Return a new instance of a Mesh with disconnected cells. Optionally, the
         points-per-cell may be specified (must be lower or equal the number of points-
         per-cell of the original Mesh). If the Mesh is to be used as a *dual* Mesh, then
         the point-coordinates do not have to be re-created because they are not used."""
 
-        cells_trimmed = self.cells
-        cell_type = self.cell_type
-
-        if points_per_cell is not None:
-            cell_type = None
-            cells_trimmed = cells_trimmed[:, :points_per_cell]
-
-        if calc_points:
-            points = self.points[cells_trimmed].reshape(-1, self.dim)
-        else:
-            points = np.zeros(
-                (self.ncells * cells_trimmed.shape[1], self.dim), dtype=int
-            )
-
-        cells = np.arange(cells_trimmed.size).reshape(*cells_trimmed.shape)
-
-        return Mesh(points, cells, cell_type=cell_type)
+        return self.dual(
+            points_per_cell=points_per_cell,
+            disconnect=True,
+            calc_points=calc_points,
+            offset=0,
+            npoints=None,
+        )
 
     def as_meshio(self, **kwargs):
         "Export the mesh as ``meshio.Mesh``."
 
         import meshio
 
         cells = {self.cell_type: self.cells}
@@ -144,14 +145,34 @@
         Mesh
             A deepcopy of the mesh.
 
         """
 
         return deepcopy(self)
 
+    @wraps(dual)
+    def dual(
+        self,
+        points_per_cell=None,
+        disconnect=True,
+        calc_points=False,
+        offset=0,
+        npoints=None,
+    ):
+        return as_mesh(
+            dual(
+                self,
+                points_per_cell=points_per_cell,
+                disconnect=disconnect,
+                calc_points=calc_points,
+                offset=offset,
+                npoints=npoints,
+            )
+        )
+
     @wraps(expand)
     def expand(self, n=11, z=1):
         return as_mesh(expand(self, n=n, z=z))
 
     @wraps(rotate)
     def rotate(self, angle_deg, axis, center=None):
         return as_mesh(rotate(self, angle_deg=angle_deg, axis=axis, center=center))
@@ -168,14 +189,18 @@
     def flip(self, mask=None):
         return as_mesh(flip(self, mask=mask))
 
     @wraps(mirror)
     def mirror(self, normal=[1, 0, 0], centerpoint=[0, 0, 0], axis=None):
         return as_mesh(mirror(self, normal=normal, centerpoint=centerpoint, axis=axis))
 
+    @wraps(translate)
+    def translate(self, move, axis):
+        return as_mesh(translate(self, move=move, axis=axis))
+
     @wraps(triangulate)
     def triangulate(self, mode=3):
         return as_mesh(triangulate(self, mode=mode))
 
     @wraps(runouts)
     def add_runouts(
         self,
```

### Comparing `felupe-7.0.0/src/felupe/mesh/_read.py` & `felupe-7.1.0/src/felupe/mesh/_read.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/mesh/_tools.py` & `felupe-7.1.0/src/felupe/mesh/_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -255,14 +255,47 @@
     for i, j in zip(find, replace):
         cells_new[cells == i] = j
 
     return points_new, cells_new, cell_type
 
 
 @mesh_or_data
+def translate(points, cells, cell_type, move, axis):
+    """Translate (move) a Mesh.
+
+    Parameters
+    ----------
+    points : list or ndarray
+        Original point coordinates.
+    cells : list or ndarray
+        Original point-connectivity of cells.
+    cell_type : str
+        A string in VTK-convention that specifies the cell type.
+    move : float
+        Translation along given axis.
+    axis : int
+        Translation axis.
+
+    Returns
+    -------
+    points : ndarray
+        Modified point coordinates.
+    cells : list or ndarray
+        Original point-connectivity of cells.
+    cell_type : str or None
+        A string in VTK-convention that specifies the cell type.
+    """
+
+    points_new = np.array(points)
+    points_new[:, axis] += move
+
+    return points_new, cells, cell_type
+
+
+@mesh_or_data
 def flip(points, cells, cell_type, mask=None):
     """Ensure positive cell volumes for `tria`, `tetra`, `quad` and
     `hexahedron` cell types.
 
     Parameters
     ----------
     points : list or ndarray
@@ -372,14 +405,26 @@
     offsets = np.cumsum(np.insert([mesh.npoints for mesh in meshes][:-1], 0, 0))
     cells = np.vstack([offset + mesh.cells for offset, mesh in zip(offsets, meshes)])
     mesh = Mesh(points=points, cells=cells, cell_type=meshes[0].cell_type)
 
     return mesh
 
 
+def stack(meshes):
+    "Stack cell-blocks from meshes with identical points-array and cell-types."
+
+    Mesh = meshes[0].__mesh__
+
+    points = meshes[0].points
+    cells = np.vstack([mesh.cells for mesh in meshes])
+    mesh = Mesh(points=points, cells=cells, cell_type=meshes[0].cell_type)
+
+    return mesh
+
+
 @mesh_or_data
 def triangulate(points, cells, cell_type, mode=3):
     """Triangulate a quad or a hex mesh.
 
     Parameters
     ----------
     points : list or ndarray
```

### Comparing `felupe-7.0.0/src/felupe/quadrature/_base.py` & `felupe-7.1.0/src/felupe/quadrature/_base.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/quadrature/_gausslegendre.py` & `felupe-7.1.0/src/felupe/quadrature/_gausslegendre.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/quadrature/_tetra.py` & `felupe-7.1.0/src/felupe/quadrature/_tetra.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/quadrature/_triangle.py` & `felupe-7.1.0/src/felupe/quadrature/_triangle.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/region/__init__.py` & `felupe-7.1.0/src/felupe/region/__init__.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/region/_boundary.py` & `felupe-7.1.0/src/felupe/region/_boundary.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/region/_region.py` & `felupe-7.1.0/src/felupe/region/_region.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,7 +118,15 @@
                 warnings.warn(
                     f"Negative volumes in Region for cells \n {cells_negative_volume}\n Try ``mesh.flip(np.any(region.dV < 0, axis=0))`` and re-create the region."
                 )
 
             # Partial derivative of element shape function
             # w.r.t. undeformed coordinates
             self.dhdX = np.einsum("aIpc,IJpc->aJpc", self.dhdr, self.drdX)
+
+    def __repr__(self):
+        header = "<felupe Region object>"
+        element = f"  Element formulation: {type(self.element).__name__}"
+        quadrature = f"  Quadrature rule: {type(self.quadrature).__name__}"
+        grad = f"  Gradient evaluated: {hasattr(self, 'dV')}"
+
+        return "\n".join([header, element, quadrature, grad])
```

### Comparing `felupe-7.0.0/src/felupe/region/_templates.py` & `felupe-7.1.0/src/felupe/region/_templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,62 +56,53 @@
     "A region with a constant quad element."
 
     def __init__(
         self,
         mesh,
         quadrature=GaussLegendre(order=1, dim=2),
         grad=False,
-        offset=0,
-        npoints=None,
     ):
 
         element = ConstantQuad()
-
-        if npoints is not None:
-            npts = npoints
-        else:
-            npts = offset + mesh.ncells
-
-        points = np.zeros((npts, mesh.dim), dtype=int)
-        cells = offset + np.arange(mesh.ncells).reshape(-1, 1)
-        m = Mesh(points, cells, mesh.cell_type)
-
-        super().__init__(m, element, quadrature, grad=grad)
+        super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionQuad(Region):
     "A region with a quad element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=1, dim=2), grad=True):
 
         element = Quad()
 
         if len(mesh.cells.T) > 4:
-            m = Mesh(mesh.points, mesh.cells[:, :4], "quad")
-        else:
-            m = mesh
+            mesh = Mesh(mesh.points, mesh.cells[:, :4], "quad")
 
-        super().__init__(m, element, quadrature, grad=grad)
+        super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionQuadraticQuad(Region):
     "A region with a (serendipity) quadratic quad element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=2, dim=2), grad=True):
 
         element = QuadraticQuad()
+
+        if len(mesh.cells.T) > 8:
+            mesh = Mesh(mesh.points, mesh.cells[:, :8], "quad8")
+
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionBiQuadraticQuad(Region):
     "A region with a bi-quadratic (lagrange) quad element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=2, dim=2), grad=True):
 
         element = BiQuadraticQuad()
+
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionQuadBoundary(RegionBoundary):
     "A region with a quad element."
 
     def __init__(
@@ -193,47 +184,31 @@
     "A region with a constant hexahedron element."
 
     def __init__(
         self,
         mesh,
         quadrature=GaussLegendre(order=1, dim=3),
         grad=False,
-        offset=0,
-        npoints=None,
     ):
 
         element = ConstantHexahedron()
-
-        if npoints is not None:
-            npts = npoints
-            ncells = min(npoints, mesh.ncells)
-        else:
-            npts = offset + mesh.ncells
-            ncells = mesh.ncells
-
-        points = np.zeros((npts, mesh.dim), dtype=int)
-        cells = offset + np.arange(ncells).reshape(-1, 1)
-        m = Mesh(points, cells, mesh.cell_type)
-
-        super().__init__(m, element, quadrature, grad=grad)
+        super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionHexahedron(Region):
     "A region with a hexahedron element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=1, dim=3), grad=True):
 
         element = Hexahedron()
 
         if len(mesh.cells.T) > 8:
-            m = Mesh(mesh.points, mesh.cells[:, :8], "hexahedron")
-        else:
-            m = mesh
+            mesh = Mesh(mesh.points, mesh.cells[:, :8], "hexahedron")
 
-        super().__init__(m, element, quadrature, grad=grad)
+        super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionHexahedronBoundary(RegionBoundary):
     "A region with a hexahedron element."
 
     def __init__(
         self,
@@ -252,14 +227,18 @@
 
 class RegionQuadraticHexahedron(Region):
     "A region with a (serendipity) quadratic hexahedron element."
 
     def __init__(self, mesh, quadrature=GaussLegendre(order=2, dim=3), grad=True):
 
         element = QuadraticHexahedron()
+
+        if len(mesh.cells.T) > 20:
+            mesh = Mesh(mesh.points, mesh.cells[:, :20], "hexahedron20")
+
         super().__init__(mesh, element, quadrature, grad=grad)
 
 
 class RegionQuadraticHexahedronBoundary(RegionBoundary):
     "A boundary region with a (serendipity) quadratic hexahedron element."
 
     def __init__(
```

### Comparing `felupe-7.0.0/src/felupe/solve/_solve.py` & `felupe-7.1.0/src/felupe/solve/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/tools/_newton.py` & `felupe-7.1.0/src/felupe/tools/_newton.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/tools/_post.py` & `felupe-7.1.0/src/felupe/tools/_post.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/tools/_project.py` & `felupe-7.1.0/src/felupe/tools/_project.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/tools/_save.py` & `felupe-7.1.0/src/felupe/tools/_save.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe/tools/_solve.py` & `felupe-7.1.0/src/felupe/tools/_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/src/felupe.egg-info/PKG-INFO` & `felupe-7.1.0/src/felupe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 7.0.0
+Version: 7.1.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -696,33 +696,36 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
 # 🔍 FElupe - Finite Element Analysis
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe)
 
-<img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/logo_light.svg" height="120px"/> <img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="120px"/> <img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="120px"/>
+<p align="center">
+  <img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/logo_light.svg" height="120px"/> <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="120px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="120px"/></a>
+</p>
 
 FElupe is a Python 3.7+ finite element analysis package focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics of solid bodies. Its name is a combination of FE (finite element) and the german word *Lupe* (magnifying glass) as a synonym for getting an insight how a finite element analysis code looks like under the hood.
 
 # Installation
 Install Python, fire up a terminal and run
 
 ```shell
 pip install felupe[all]
 ```
 
-where `[all]` installs all optional dependencies. By default, FElupe depends on `numpy`, `scipy` and `einsumt`. In order to make use of all features of FElupe, it is suggested to install all optional dependencies (`h5py`, `meshio` and `tensortrax`).
+where `[all]` installs all optional dependencies. By default, FElupe depends on `numpy` and `scipy`. In order to make use of all features of FElupe, it is suggested to install all optional dependencies (`einsumt`, `h5py`, `matplotlib`, `meshio` and `tensortrax`).
 
 # Getting Started
 A quarter model of a solid cube with hyperelastic material behaviour is subjected to a uniaxial elongation applied at a clamped end-face. This involves the creation of a mesh, a region as well as a displacement field (encapsulated in a field container). Furthermore, the boundary conditions are created by a template for a uniaxial loadcase. An isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model formulation in combination with an isotropic hyperelastic Neo-Hookean material formulation is applied on a nearly-incompressible solid body. A step generates the consecutive substep-movements of a given boundary condition. The step is further added to a list of steps of a job (here, a characteristic-curve job is used). During evaluation, each substep of each step is solved by an iterative Newton-Rhapson procedure. The solution is exported after each completed substep as a time-series XDMF file. For more details beside this high-level code snippet, please have a look at the [documentation](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 ```python
 import felupe as fem
```

### Comparing `felupe-7.0.0/src/felupe.egg-info/SOURCES.txt` & `felupe-7.1.0/src/felupe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 src/felupe/mechanics/_solidbody_pressure.py
 src/felupe/mechanics/_step.py
 src/felupe/mesh/__init__.py
 src/felupe/mesh/_base.py
 src/felupe/mesh/_container.py
 src/felupe/mesh/_convert.py
 src/felupe/mesh/_discrete_geometry.py
+src/felupe/mesh/_dual.py
 src/felupe/mesh/_geometry.py
 src/felupe/mesh/_helpers.py
 src/felupe/mesh/_mesh.py
 src/felupe/mesh/_read.py
 src/felupe/mesh/_tools.py
 src/felupe/quadrature/__init__.py
 src/felupe/quadrature/_base.py
```

### Comparing `felupe-7.0.0/tests/test_basis.py` & `felupe-7.1.0/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_bilinearform.py` & `felupe-7.1.0/tests/test_bilinearform.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     return dot(p, q) * dot(r, p)
 
 
 def pre(dim):
 
     mesh = fe.Cube(n=3)
     region = fe.RegionHexahedron(mesh)
-    region0 = fe.RegionConstantHexahedron(mesh)
+    region0 = fe.RegionConstantHexahedron(mesh.dual(points_per_cell=1))
     u = fe.Field(region, dim=3)
     p = fe.Field(region0)
     up = fe.FieldContainer([u, p])
 
     return up
```

### Comparing `felupe-7.0.0/tests/test_composite.py` & `felupe-7.1.0/tests/test_composite.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 
 import felupe as fe
 
 
 def test_composite():
 
-    n = 10
+    n = 5
     mesh = fe.Cube(n=n)
     region = fe.RegionHexahedron(mesh)
 
     points = np.arange(mesh.npoints)[
         np.logical_or.reduce(
             (
                 mesh.points[:, 0] == 0,
@@ -65,9 +65,74 @@
     reinforced = fe.SolidBody(nh2, field_reinforced)
 
     res = fe.newtonrhapson(field, items=[rubber, reinforced], **loadcase)
 
     fe.save(region, res.x)
 
 
+def test_composite_planestrain():
+
+    n = 5
+    mesh = fe.Rectangle(n=n)
+    region = fe.RegionQuad(mesh)
+
+    points = np.arange(mesh.npoints)[
+        np.logical_or.reduce(
+            (
+                mesh.points[:, 0] == 0,
+                mesh.points[:, 0] == 0 + 1 / (n - 1),
+                mesh.points[:, 0] == 0.5 - 1 / (n - 1) / 2,
+                mesh.points[:, 0] == 0.5 + 1 / (n - 1) / 2,
+                mesh.points[:, 0] == 1 - 1 / (n - 1),
+                mesh.points[:, 0] == 1,
+            )
+        )
+    ]
+    cells = np.isin(mesh.cells, points).sum(1) == mesh.cells.shape[1]
+
+    mesh_rubber = mesh.copy()
+    mesh_rubber.update(mesh_rubber.cells[~cells])
+
+    mesh_reinforced = mesh.copy()
+    mesh_reinforced.update(mesh_reinforced.cells[cells])
+
+    region_rubber = fe.RegionQuad(mesh_rubber)
+    field_rubber = fe.FieldsMixed(
+        region_rubber,
+        n=3,
+        offset=0,
+        planestrain=True,
+        npoints=mesh_rubber.ncells + mesh_reinforced.ncells,
+    )
+
+    region_reinforced = fe.RegionQuad(mesh_reinforced)
+    field_reinforced = fe.FieldsMixed(
+        region_reinforced,
+        n=3,
+        offset=mesh_rubber.ncells,
+        planestrain=True,
+        npoints=mesh_rubber.ncells + mesh_reinforced.ncells,
+    )
+
+    field = fe.FieldsMixed(
+        region,
+        n=3,
+        planestrain=True,
+        npoints=mesh_rubber.ncells + mesh_reinforced.ncells,
+    )
+
+    boundaries, loadcase = fe.dof.uniaxial(field, move=-0.1)
+
+    nh1 = fe.ThreeFieldVariation(fe.NeoHooke(mu=1, bulk=5000))
+    nh2 = fe.ThreeFieldVariation(fe.NeoHooke(mu=5000, bulk=5000))
+
+    rubber = fe.SolidBody(nh1, field_rubber)
+    reinforced = fe.SolidBody(nh2, field_reinforced)
+
+    res = fe.newtonrhapson(field, items=[rubber, reinforced], **loadcase)
+
+    fe.save(region, res.x)
+
+
 if __name__ == "__main__":
     test_composite()
+    test_composite_planestrain()
```

### Comparing `felupe-7.0.0/tests/test_constitution.py` & `felupe-7.1.0/tests/test_constitution.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_dof.py` & `felupe-7.1.0/tests/test_dof.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_element.py` & `felupe-7.1.0/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_field.py` & `felupe-7.1.0/tests/test_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,27 +35,30 @@
 
     m = fe.Cube(n=3)
     e = fe.Hexahedron()
     q = fe.GaussLegendre(1, 3)
     r = fe.Region(m, e, q)
     u = fe.Field(r, dim=3, values=values)
     v = fe.FieldContainer([u])
+
     return r, v
 
 
 def pre_axi():
 
     m = fe.Rectangle(n=3)
     e = fe.Quad()
     q = fe.GaussLegendre(1, 2)
     r = fe.Region(m, e, q)
 
     u = fe.FieldAxisymmetric(r)
     v = fe.FieldContainer([u])
 
+    print(m), print(r), print(v)
+
     return r, v
 
 
 def pre_mixed():
 
     m = fe.Cube(n=3)
     e = fe.Hexahedron()
@@ -65,14 +68,16 @@
     u = fe.Field(r, dim=3)
     p = fe.Field(r)
     J = fe.Field(r, values=1)
 
     f = fe.FieldContainer((u, p, J))
     g = fe.FieldsMixed(fe.RegionHexahedron(m), n=3)
 
+    print(m), print(r), print(f)
+
     u.values[0] = np.ones(3)
     assert np.all(f.values()[0][0] == 1)
     assert len(g.fields) == 3
 
     fe.Field(r, dim=9, values=np.eye(3))
 
     return r, f, u, p, J
```

### Comparing `felupe-7.0.0/tests/test_form.py` & `felupe-7.1.0/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_job.py` & `felupe-7.1.0/tests/test_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 Created on Sun Aug 21 00:27:38 2022
 
 @author: z0039mte
 """
 
 import numpy as np
+import pytest
 
 import felupe as fem
 
 
 def pre():
 
     mesh = fem.Rectangle(n=2)
@@ -46,26 +47,26 @@
 
     field, step = pre()
     job = fem.Job(steps=[step])
     job.evaluate()
 
     field, step = pre()
     job = fem.Job(steps=[step])
-    job.evaluate()
+    job.evaluate(parallel=True, kwargs={"parallel": False})
 
 
 def test_job_xdmf():
 
     field, step = pre()
     job = fem.Job(steps=[step])
     job.evaluate()
 
     field, step = pre()
     job = fem.Job(steps=[step])
-    job.evaluate(filename="result.xdmf")
+    job.evaluate(filename="result.xdmf", parallel=True)
 
 
 def test_job_xdmf_global_field():
 
     field, step = pre()
     job = fem.Job(steps=[step])
     job.evaluate()
@@ -76,14 +77,19 @@
 
 
 def test_curve():
 
     field, step = pre()
 
     curve = fem.CharacteristicCurve(steps=[step], boundary=step.boundaries["move"])
+
+    with pytest.raises(ValueError):
+        curve.plot()
+
+    curve.evaluate()
     curve.plot(xaxis=0, yaxis=0)
     curve.plot(x=np.zeros((10, 2)), y=np.ones((10, 2)), xaxis=0, yaxis=0)
 
     stretch = 1 + np.array(curve.x)[:, 0]
     area = 1**2 * np.pi
     force = (stretch - 1 / stretch**2) * area
 
@@ -108,14 +114,15 @@
 def test_curve_custom_items():
 
     field, step = pre()
 
     curve = fem.CharacteristicCurve(
         steps=[step], items=step.items, boundary=step.boundaries["move"]
     )
+    curve.evaluate()
     curve.plot(xaxis=0, yaxis=0, gradient=True)
     curve.plot(x=np.zeros((10, 2)), y=np.ones((10, 2)), xaxis=0, yaxis=0)
 
     stretch = 1 + np.array(curve.x)[:, 0]
     area = 1**2 * np.pi
     force = (stretch - 1 / stretch**2) * area
```

### Comparing `felupe-7.0.0/tests/test_math.py` & `felupe-7.1.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_mechanics.py` & `felupe-7.1.0/tests/test_mechanics.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_mesh.py` & `felupe-7.1.0/tests/test_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,18 @@
 
     m = fe.Mesh(
         points=np.array([[0, 0, 0], [1, 0, 0], [0, 1, 0], [0, 0, 1]]),
         cells=np.array([[0, 1, 2, 3]]),
         cell_type="tetra",
     )
 
+    m.dual()
+    fe.mesh.dual(m, disconnect=False)
+    fe.mesh.dual(m, calc_points=True)
+
     fe.mesh.convert(m, order=0)
     fe.mesh.convert(m, order=0, calc_points=True)
     fe.mesh.convert(m, order=2)
     fe.mesh.convert(m, order=2, calc_midfaces=True)
 
     m = fe.mesh.Line(n=5)
     assert m.points.shape == (5, 1)
@@ -134,14 +138,19 @@
     fe.mesh.convert(m, order=2, calc_midfaces=True, calc_midvolumes=True)
 
     fe.mesh.rotate(m, angle_deg=10, axis=0, center=None)
     fe.mesh.rotate(m.points, m.cells, m.cell_type, angle_deg=10, axis=0, center=None)
     fe.mesh.rotate(m, angle_deg=10, axis=1, center=[0, 0, 0])
     m.rotate(angle_deg=10, axis=0, center=None)
 
+    fe.mesh.translate(m, move=1, axis=1)
+    fe.mesh.translate(m.points, m.cells, m.cell_type, move=1, axis=1)
+    fe.mesh.translate(m, move=1, axis=1)
+    m.translate(move=1, axis=1)
+
     fe.mesh.CubeArbitraryOrderHexahedron()
     fe.mesh.RectangleArbitraryOrderQuad()
 
     m = fe.Rectangle(n=5)
     m.points = np.vstack((m.points, [10, 10]))
     assert m.points.shape == (26, 2)
     assert m.cells.shape == (16, 4)
@@ -267,22 +276,27 @@
 
     x = [0.5, 0.5]
     n = fe.mesh.runouts(m, values=[0.1], axis=0, centerpoint=x)
     assert (n.points - x)[:, 1].min() == (m.points - x)[:, 1].min() * 1.1
     assert (n.points - x)[:, 1].max() == (m.points - x)[:, 1].max() * 1.1
 
 
-def test_concatenate():
+def test_concatenate_stack():
     m = fe.Rectangle(n=3)
 
     n = fe.mesh.concatenate([m, m, m])
 
     assert n.npoints == 3 * m.npoints
     assert n.ncells == 3 * m.ncells
 
+    p = fe.mesh.stack([m, m, m])
+
+    assert m.npoints == p.npoints
+    assert n.ncells == p.ncells
+
 
 def test_grid():
     m = fe.Rectangle(b=(10, 3), n=(4, 5))
 
     x = np.linspace(0, 10, 4)
     y = np.linspace(0, 3, 5)
     n = fe.mesh.Grid(x, y)
@@ -380,14 +394,14 @@
 
 
 if __name__ == "__main__":
     test_meshes()
     test_mirror()
     test_triangulate()
     test_runouts()
-    test_concatenate()
+    test_concatenate_stack()
     test_grid()
     test_grid_1d()
     test_container()
     test_read(filename="mesh.bdf")
     test_mesh_methods()
     test_read_nocells(filename="mesh_no-cells.bdf")
```

### Comparing `felupe-7.0.0/tests/test_mpc.py` & `felupe-7.1.0/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_planestrain.py` & `felupe-7.1.0/tests/test_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_quadrature.py` & `felupe-7.1.0/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_readme.py` & `felupe-7.1.0/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_region.py` & `felupe-7.1.0/tests/test_region.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     mesh2 = fe.mesh.convert(mesh, 2, True, False, False)
     r = fe.RegionQuadraticQuad(mesh2)
     f = fe.FieldsMixed(r)
 
     r = fe.RegionQuadraticQuadBoundary(mesh2, ensure_3d=True)
 
     mesh3 = fe.mesh.convert(mesh, 2, True, True, False)
+    r = fe.RegionQuad(mesh3)
+    r = fe.RegionQuadraticQuad(mesh3)
     r = fe.RegionBiQuadraticQuad(mesh3)
     f = fe.FieldsMixed(r)
 
     r = fe.RegionBiQuadraticQuadBoundary(mesh3)
 
     mesh.cell_type = "some_fancy_cell_type"
     with pytest.raises(NotImplementedError):
@@ -71,36 +73,40 @@
     mesh2 = fe.mesh.convert(mesh, 2, True, False, False)
     r = fe.RegionQuadraticHexahedron(mesh2)
     f = fe.FieldsMixed(r)
 
     r = fe.RegionQuadraticHexahedronBoundary(mesh2)
 
     mesh3 = fe.mesh.convert(mesh, 2, True, True, True)
+    r = fe.RegionHexahedron(mesh3)
+    r = fe.RegionQuadraticHexahedron(mesh3)
     r = fe.RegionTriQuadraticHexahedron(mesh3)
     f = fe.FieldsMixed(r)
 
     r = fe.RegionTriQuadraticHexahedronBoundary(mesh3)
 
     triangle = fe.Triangle()
     points = triangle.points
     cells = np.arange(3).reshape(1, -1)
     mesh = fe.Mesh(points, cells, "triangle")
     r = fe.RegionTriangle(mesh)
 
     mesh2 = fe.mesh.convert(mesh, 2, True, False, False)
+    r = fe.RegionTriangle(mesh2)
     r = fe.RegionQuadraticTriangle(mesh2)
     f = fe.FieldsMixed(r)
 
     tetra = fe.Tetra()
     points = tetra.points
     cells = np.arange(4).reshape(1, -1)
     mesh = fe.Mesh(points, cells, "tetra")
     r = fe.RegionTetra(mesh)
 
     mesh2 = fe.mesh.convert(mesh, 2, True, False, False)
+    r = fe.RegionTetra(mesh2)
     r = fe.RegionQuadraticTetra(mesh2)
     f = fe.FieldsMixed(r)
 
     triangle = fe.TriangleMINI()
     points = triangle.points
     cells = np.arange(4).reshape(1, -1)
     mesh = fe.Mesh(points, cells, "triangle-mini")
```

### Comparing `felupe-7.0.0/tests/test_solve.py` & `felupe-7.1.0/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `felupe-7.0.0/tests/test_tools.py` & `felupe-7.1.0/tests/test_tools.py`

 * *Files identical despite different names*

