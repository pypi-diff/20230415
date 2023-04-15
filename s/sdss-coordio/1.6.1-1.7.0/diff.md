# Comparing `tmp/sdss-coordio-1.6.1.tar.gz` & `tmp/sdss-coordio-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-coordio-1.6.1.tar", last modified: Sun Jan 15 17:28:16 2023, max compression
+gzip compressed data, was "sdss-coordio-1.7.0.tar", last modified: Sat Apr 15 21:06:00 2023, max compression
```

## Comparing `sdss-coordio-1.6.1.tar` & `sdss-coordio-1.7.0.tar`

### file list

```diff
@@ -1,311 +1,330 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-15 17:28:16.727399 sdss-coordio-1.6.1/
--rw-r--r--   0 runner     (501) staff       (20)     1504 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)       62 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     1737 2023-01-15 17:28:16.727598 sdss-coordio-1.6.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      796 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-15 17:28:16.571880 sdss-coordio-1.6.1/cextern/
--rw-r--r--   0 runner     (501) staff       (20)      343 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/README.md
--rw-r--r--   0 runner     (501) staff       (20)    12507 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/conv.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-15 17:28:16.578956 sdss-coordio-1.6.1/cextern/dimage/
--rw-r--r--   0 runner     (501) staff       (20)     3150 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dallpeaks.c
--rw-r--r--   0 runner     (501) staff       (20)     1295 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dcen3x3.c
--rw-r--r--   0 runner     (501) staff       (20)     3239 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dfind.c
--rw-r--r--   0 runner     (501) staff       (20)     2553 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dfloodfill.c
--rw-r--r--   0 runner     (501) staff       (20)     1407 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dimage.h
--rw-r--r--   0 runner     (501) staff       (20)     6057 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dmedsmooth.c
--rw-r--r--   0 runner     (501) staff       (20)     1351 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dobjects.c
--rw-r--r--   0 runner     (501) staff       (20)     3798 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dpeaks.c
--rw-r--r--   0 runner     (501) staff       (20)     2856 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/drefine.c
--rw-r--r--   0 runner     (501) staff       (20)     1872 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dselip.c
--rw-r--r--   0 runner     (501) staff       (20)     1252 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dsigma.c
--rw-r--r--   0 runner     (501) staff       (20)     3854 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/dsmooth.c
--rw-r--r--   0 runner     (501) staff       (20)       58 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/readme.txt
--rw-r--r--   0 runner     (501) staff       (20)     1984 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/dimage/simplexy.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-15 17:28:16.709681 sdss-coordio-1.6.1/cextern/sofa/
--rw-r--r--   0 runner     (501) staff       (20)     6468 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/a2af.c
--rw-r--r--   0 runner     (501) staff       (20)     6374 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/a2tf.c
--rw-r--r--   0 runner     (501) staff       (20)     6611 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/ab.c
--rw-r--r--   0 runner     (501) staff       (20)     7187 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/ae2hd.c
--rw-r--r--   0 runner     (501) staff       (20)     6087 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/af2a.c
--rw-r--r--   0 runner     (501) staff       (20)     4955 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/anp.c
--rw-r--r--   0 runner     (501) staff       (20)     4983 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/anpm.c
--rw-r--r--   0 runner     (501) staff       (20)     9173 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/apcg.c
--rw-r--r--   0 runner     (501) staff       (20)     9278 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/apcg13.c
--rw-r--r--   0 runner     (501) staff       (20)     9669 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/apci.c
--rw-r--r--   0 runner     (501) staff       (20)     9954 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/apci13.c
--rw-r--r--   0 runner     (501) staff       (20)    12864 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/apco.c
--rw-r--r--   0 runner     (501) staff       (20)    14172 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/apco13.c
--rw-r--r--   0 runner     (501) staff       (20)    11004 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/apcs.c
--rw-r--r--   0 runner     (501) staff       (20)     9686 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/apcs13.c
--rw-r--r--   0 runner     (501) staff       (20)     8285 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/aper.c
--rw-r--r--   0 runner     (501) staff       (20)     9207 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/aper13.c
--rw-r--r--   0 runner     (501) staff       (20)    10588 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/apio.c
--rw-r--r--   0 runner     (501) staff       (20)    12842 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/apio13.c
--rw-r--r--   0 runner     (501) staff       (20)     8257 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atci13.c
--rw-r--r--   0 runner     (501) staff       (20)     7978 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atciq.c
--rw-r--r--   0 runner     (501) staff       (20)     9826 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atciqn.c
--rw-r--r--   0 runner     (501) staff       (20)     7729 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atciqz.c
--rw-r--r--   0 runner     (501) staff       (20)    12474 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atco13.c
--rw-r--r--   0 runner     (501) staff       (20)     7919 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atic13.c
--rw-r--r--   0 runner     (501) staff       (20)     8735 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/aticq.c
--rw-r--r--   0 runner     (501) staff       (20)    10634 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/aticqn.c
--rw-r--r--   0 runner     (501) staff       (20)    11485 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atio13.c
--rw-r--r--   0 runner     (501) staff       (20)    11389 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atioq.c
--rw-r--r--   0 runner     (501) staff       (20)    12003 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atoc13.c
--rw-r--r--   0 runner     (501) staff       (20)    11902 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atoi13.c
--rw-r--r--   0 runner     (501) staff       (20)    11115 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/atoiq.c
--rw-r--r--   0 runner     (501) staff       (20)     6640 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/bi00.c
--rw-r--r--   0 runner     (501) staff       (20)     8454 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/bp00.c
--rw-r--r--   0 runner     (501) staff       (20)     7280 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/bp06.c
--rw-r--r--   0 runner     (501) staff       (20)     5822 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/bpn2xy.c
--rw-r--r--   0 runner     (501) staff       (20)     7375 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2i00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7362 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2i00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7165 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2i06a.c
--rw-r--r--   0 runner     (501) staff       (20)     7592 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2ibpn.c
--rw-r--r--   0 runner     (501) staff       (20)     7162 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2ixy.c
--rw-r--r--   0 runner     (501) staff       (20)     6391 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2ixys.c
--rw-r--r--   0 runner     (501) staff       (20)     5320 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2s.c
--rw-r--r--   0 runner     (501) staff       (20)     8083 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2t00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7985 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2t00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7970 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2t06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6652 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2tcio.c
--rw-r--r--   0 runner     (501) staff       (20)     6679 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2teqx.c
--rw-r--r--   0 runner     (501) staff       (20)     8786 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2tpe.c
--rw-r--r--   0 runner     (501) staff       (20)     8249 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/c2txy.c
--rw-r--r--   0 runner     (501) staff       (20)     6962 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/cal2jd.c
--rw-r--r--   0 runner     (501) staff       (20)     4897 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/cp.c
--rw-r--r--   0 runner     (501) staff       (20)     4990 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/cpv.c
--rw-r--r--   0 runner     (501) staff       (20)     4974 2023-01-15 17:27:00.000000 sdss-coordio-1.6.1/cextern/sofa/cr.c
--rw-r--r--   0 runner     (501) staff       (20)     9794 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/d2dtf.c
--rw-r--r--   0 runner     (501) staff       (20)     7240 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/d2tf.c
--rw-r--r--   0 runner     (501) staff       (20)    13394 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/dat.c
--rw-r--r--   0 runner     (501) staff       (20)    63548 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/dtdb.c
--rw-r--r--   0 runner     (501) staff       (20)     9375 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/dtf2d.c
--rw-r--r--   0 runner     (501) staff       (20)     7237 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/eceq06.c
--rw-r--r--   0 runner     (501) staff       (20)     7251 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ecm06.c
--rw-r--r--   0 runner     (501) staff       (20)     6929 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ee00.c
--rw-r--r--   0 runner     (501) staff       (20)     7105 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ee00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7436 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ee00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6632 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ee06a.c
--rw-r--r--   0 runner     (501) staff       (20)    12358 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/eect00.c
--rw-r--r--   0 runner     (501) staff       (20)     6688 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/eform.c
--rw-r--r--   0 runner     (501) staff       (20)     7000 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/eo06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6082 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/eors.c
--rw-r--r--   0 runner     (501) staff       (20)     5398 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/epb.c
--rw-r--r--   0 runner     (501) staff       (20)     5342 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/epb2jd.c
--rw-r--r--   0 runner     (501) staff       (20)     5327 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/epj.c
--rw-r--r--   0 runner     (501) staff       (20)     5330 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/epj2jd.c
--rw-r--r--   0 runner     (501) staff       (20)   152024 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/epv00.c
--rw-r--r--   0 runner     (501) staff       (20)     7238 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/eqec06.c
--rw-r--r--   0 runner     (501) staff       (20)     6953 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/eqeq94.c
--rw-r--r--   0 runner     (501) staff       (20)     6978 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/era00.c
--rw-r--r--   0 runner     (501) staff       (20)     5789 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fad03.c
--rw-r--r--   0 runner     (501) staff       (20)     5756 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fae03.c
--rw-r--r--   0 runner     (501) staff       (20)     5883 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/faf03.c
--rw-r--r--   0 runner     (501) staff       (20)     5768 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/faju03.c
--rw-r--r--   0 runner     (501) staff       (20)     5758 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fal03.c
--rw-r--r--   0 runner     (501) staff       (20)     5758 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/falp03.c
--rw-r--r--   0 runner     (501) staff       (20)     5760 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fama03.c
--rw-r--r--   0 runner     (501) staff       (20)     5770 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fame03.c
--rw-r--r--   0 runner     (501) staff       (20)     5631 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fane03.c
--rw-r--r--   0 runner     (501) staff       (20)     5826 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/faom03.c
--rw-r--r--   0 runner     (501) staff       (20)     5754 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fapa03.c
--rw-r--r--   0 runner     (501) staff       (20)     5765 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fasa03.c
--rw-r--r--   0 runner     (501) staff       (20)     5629 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/faur03.c
--rw-r--r--   0 runner     (501) staff       (20)     5764 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fave03.c
--rw-r--r--   0 runner     (501) staff       (20)    12333 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fk425.c
--rw-r--r--   0 runner     (501) staff       (20)     9855 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fk45z.c
--rw-r--r--   0 runner     (501) staff       (20)    12391 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fk524.c
--rw-r--r--   0 runner     (501) staff       (20)     7422 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fk52h.c
--rw-r--r--   0 runner     (501) staff       (20)     7286 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fk54z.c
--rw-r--r--   0 runner     (501) staff       (20)     6198 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fk5hip.c
--rw-r--r--   0 runner     (501) staff       (20)     8093 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fk5hz.c
--rw-r--r--   0 runner     (501) staff       (20)     7061 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fw2m.c
--rw-r--r--   0 runner     (501) staff       (20)     6147 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/fw2xy.c
--rw-r--r--   0 runner     (501) staff       (20)     8396 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/g2icrs.c
--rw-r--r--   0 runner     (501) staff       (20)     6710 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gc2gd.c
--rw-r--r--   0 runner     (501) staff       (20)     8338 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gc2gde.c
--rw-r--r--   0 runner     (501) staff       (20)     6783 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gd2gc.c
--rw-r--r--   0 runner     (501) staff       (20)     6968 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gd2gce.c
--rw-r--r--   0 runner     (501) staff       (20)     7699 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gmst00.c
--rw-r--r--   0 runner     (501) staff       (20)     7337 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gmst06.c
--rw-r--r--   0 runner     (501) staff       (20)     7688 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gmst82.c
--rw-r--r--   0 runner     (501) staff       (20)     7470 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gst00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7770 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gst00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7536 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gst06.c
--rw-r--r--   0 runner     (501) staff       (20)     7174 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gst06a.c
--rw-r--r--   0 runner     (501) staff       (20)     7099 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/gst94.c
--rw-r--r--   0 runner     (501) staff       (20)     7614 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/h2fk5.c
--rw-r--r--   0 runner     (501) staff       (20)     7382 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/hd2ae.c
--rw-r--r--   0 runner     (501) staff       (20)     6333 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/hd2pa.c
--rw-r--r--   0 runner     (501) staff       (20)     8684 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/hfk5z.c
--rw-r--r--   0 runner     (501) staff       (20)     8382 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/icrs2g.c
--rw-r--r--   0 runner     (501) staff       (20)     4970 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ir.c
--rw-r--r--   0 runner     (501) staff       (20)     8269 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/jd2cal.c
--rw-r--r--   0 runner     (501) staff       (20)     7559 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/jdcalf.c
--rw-r--r--   0 runner     (501) staff       (20)     7662 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ld.c
--rw-r--r--   0 runner     (501) staff       (20)     8829 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ldn.c
--rw-r--r--   0 runner     (501) staff       (20)     5982 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ldsun.c
--rw-r--r--   0 runner     (501) staff       (20)     7014 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/lteceq.c
--rw-r--r--   0 runner     (501) staff       (20)     7567 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ltecm.c
--rw-r--r--   0 runner     (501) staff       (20)     7019 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/lteqec.c
--rw-r--r--   0 runner     (501) staff       (20)     6500 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ltp.c
--rw-r--r--   0 runner     (501) staff       (20)     6581 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ltpb.c
--rw-r--r--   0 runner     (501) staff       (20)     7601 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ltpecl.c
--rw-r--r--   0 runner     (501) staff       (20)     7880 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ltpequ.c
--rw-r--r--   0 runner     (501) staff       (20)    27755 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/makefile
--rw-r--r--   0 runner     (501) staff       (20)     6728 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/num00a.c
--rw-r--r--   0 runner     (501) staff       (20)     6713 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/num00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6660 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/num06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6057 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/numat.c
--rw-r--r--   0 runner     (501) staff       (20)   119801 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/nut00a.c
--rw-r--r--   0 runner     (501) staff       (20)    19020 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/nut00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7823 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/nut06a.c
--rw-r--r--   0 runner     (501) staff       (20)    16295 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/nut80.c
--rw-r--r--   0 runner     (501) staff       (20)     6473 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/nutm80.c
--rw-r--r--   0 runner     (501) staff       (20)     6414 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/obl06.c
--rw-r--r--   0 runner     (501) staff       (20)     6459 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/obl80.c
--rw-r--r--   0 runner     (501) staff       (20)    13793 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/p06e.c
--rw-r--r--   0 runner     (501) staff       (20)     5029 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/p2pv.c
--rw-r--r--   0 runner     (501) staff       (20)     5276 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/p2s.c
--rw-r--r--   0 runner     (501) staff       (20)     6768 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pap.c
--rw-r--r--   0 runner     (501) staff       (20)     5638 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pas.c
--rw-r--r--   0 runner     (501) staff       (20)     7817 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pb06.c
--rw-r--r--   0 runner     (501) staff       (20)     5008 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pdp.c
--rw-r--r--   0 runner     (501) staff       (20)     7964 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pfw06.c
--rw-r--r--   0 runner     (501) staff       (20)    23180 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/plan94.c
--rw-r--r--   0 runner     (501) staff       (20)     4887 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pm.c
--rw-r--r--   0 runner     (501) staff       (20)     6579 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pmat00.c
--rw-r--r--   0 runner     (501) staff       (20)     6683 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pmat06.c
--rw-r--r--   0 runner     (501) staff       (20)     7548 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pmat76.c
--rw-r--r--   0 runner     (501) staff       (20)     5090 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pmp.c
--rw-r--r--   0 runner     (501) staff       (20)     7054 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pmpx.c
--rw-r--r--   0 runner     (501) staff       (20)    10220 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pmsafe.c
--rw-r--r--   0 runner     (501) staff       (20)     5495 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pn.c
--rw-r--r--   0 runner     (501) staff       (20)     9146 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pn00.c
--rw-r--r--   0 runner     (501) staff       (20)     8833 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pn00a.c
--rw-r--r--   0 runner     (501) staff       (20)     8825 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pn00b.c
--rw-r--r--   0 runner     (501) staff       (20)     9253 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pn06.c
--rw-r--r--   0 runner     (501) staff       (20)     8282 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pn06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6802 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pnm00a.c
--rw-r--r--   0 runner     (501) staff       (20)     6797 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pnm00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6835 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pnm06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6778 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pnm80.c
--rw-r--r--   0 runner     (501) staff       (20)     6453 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pom00.c
--rw-r--r--   0 runner     (501) staff       (20)     5087 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ppp.c
--rw-r--r--   0 runner     (501) staff       (20)     5275 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ppsp.c
--rw-r--r--   0 runner     (501) staff       (20)     7813 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pr00.c
--rw-r--r--   0 runner     (501) staff       (20)     8023 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/prec76.c
--rw-r--r--   0 runner     (501) staff       (20)     4958 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pv2p.c
--rw-r--r--   0 runner     (501) staff       (20)     6861 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pv2s.c
--rw-r--r--   0 runner     (501) staff       (20)     5587 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pvdpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5073 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pvm.c
--rw-r--r--   0 runner     (501) staff       (20)     5182 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pvmpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5177 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pvppv.c
--rw-r--r--   0 runner     (501) staff       (20)    10128 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pvstar.c
--rw-r--r--   0 runner     (501) staff       (20)     7712 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pvtob.c
--rw-r--r--   0 runner     (501) staff       (20)     5373 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pvu.c
--rw-r--r--   0 runner     (501) staff       (20)     5280 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pvup.c
--rw-r--r--   0 runner     (501) staff       (20)     5842 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pvxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5234 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/pxp.c
--rw-r--r--   0 runner     (501) staff       (20)    11663 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/refco.c
--rw-r--r--   0 runner     (501) staff       (20)     5989 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/rm2v.c
--rw-r--r--   0 runner     (501) staff       (20)     5996 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/rv2m.c
--rw-r--r--   0 runner     (501) staff       (20)     5807 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/rx.c
--rw-r--r--   0 runner     (501) staff       (20)     5298 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/rxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5144 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/rxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5337 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/rxr.c
--rw-r--r--   0 runner     (501) staff       (20)     5848 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ry.c
--rw-r--r--   0 runner     (501) staff       (20)     5817 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/rz.c
--rw-r--r--   0 runner     (501) staff       (20)    15540 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/s00.c
--rw-r--r--   0 runner     (501) staff       (20)     7781 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/s00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7772 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/s00b.c
--rw-r--r--   0 runner     (501) staff       (20)    15442 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/s06.c
--rw-r--r--   0 runner     (501) staff       (20)     7799 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/s06a.c
--rw-r--r--   0 runner     (501) staff       (20)     5073 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/s2c.c
--rw-r--r--   0 runner     (501) staff       (20)     5209 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/s2p.c
--rw-r--r--   0 runner     (501) staff       (20)     5636 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/s2pv.c
--rw-r--r--   0 runner     (501) staff       (20)     5282 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/s2xpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5877 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/sepp.c
--rw-r--r--   0 runner     (501) staff       (20)     5424 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/seps.c
--rw-r--r--   0 runner     (501) staff       (20)    26863 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/sofa.h
--rw-r--r--   0 runner     (501) staff       (20)     8772 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/sofam.h
--rw-r--r--   0 runner     (501) staff       (20)     6557 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/sp00.c
--rw-r--r--   0 runner     (501) staff       (20)    10677 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/starpm.c
--rw-r--r--   0 runner     (501) staff       (20)    11959 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/starpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5038 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/sxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5101 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/sxpv.c
--rw-r--r--   0 runner     (501) staff       (20)   241327 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/t_sofa_c.c
--rw-r--r--   0 runner     (501) staff       (20)     5845 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/taitt.c
--rw-r--r--   0 runner     (501) staff       (20)     5901 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/taiut1.c
--rw-r--r--   0 runner     (501) staff       (20)     7493 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/taiutc.c
--rw-r--r--   0 runner     (501) staff       (20)     6987 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tcbtdb.c
--rw-r--r--   0 runner     (501) staff       (20)     5845 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tcgtt.c
--rw-r--r--   0 runner     (501) staff       (20)     7109 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tdbtcb.c
--rw-r--r--   0 runner     (501) staff       (20)     6353 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tdbtt.c
--rw-r--r--   0 runner     (501) staff       (20)     6062 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tf2a.c
--rw-r--r--   0 runner     (501) staff       (20)     6066 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tf2d.c
--rw-r--r--   0 runner     (501) staff       (20)     8685 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tpors.c
--rw-r--r--   0 runner     (501) staff       (20)     8649 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tporv.c
--rw-r--r--   0 runner     (501) staff       (20)     6534 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tpsts.c
--rw-r--r--   0 runner     (501) staff       (20)     7337 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tpstv.c
--rw-r--r--   0 runner     (501) staff       (20)     7253 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tpxes.c
--rw-r--r--   0 runner     (501) staff       (20)     7927 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tpxev.c
--rw-r--r--   0 runner     (501) staff       (20)     5136 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tr.c
--rw-r--r--   0 runner     (501) staff       (20)     5263 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/trxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5291 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/trxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5841 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tttai.c
--rw-r--r--   0 runner     (501) staff       (20)     5913 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tttcg.c
--rw-r--r--   0 runner     (501) staff       (20)     6345 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/tttdb.c
--rw-r--r--   0 runner     (501) staff       (20)     5794 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ttut1.c
--rw-r--r--   0 runner     (501) staff       (20)     5898 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ut1tai.c
--rw-r--r--   0 runner     (501) staff       (20)     5798 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ut1tt.c
--rw-r--r--   0 runner     (501) staff       (20)     8782 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/ut1utc.c
--rw-r--r--   0 runner     (501) staff       (20)     8283 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/utctai.c
--rw-r--r--   0 runner     (501) staff       (20)     7458 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/utcut1.c
--rw-r--r--   0 runner     (501) staff       (20)   133674 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/xy06.c
--rw-r--r--   0 runner     (501) staff       (20)     7028 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/xys00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7010 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/xys00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7056 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/xys06a.c
--rw-r--r--   0 runner     (501) staff       (20)     4820 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/zp.c
--rw-r--r--   0 runner     (501) staff       (20)     4874 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/zpv.c
--rw-r--r--   0 runner     (501) staff       (20)     4967 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/cextern/sofa/zr.c
--rw-r--r--   0 runner     (501) staff       (20)     2341 2023-01-15 17:28:16.728957 sdss-coordio-1.6.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2697 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-15 17:28:16.568405 sdss-coordio-1.6.1/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-15 17:28:16.722154 sdss-coordio-1.6.1/src/coordio/
--rw-r--r--   0 runner     (501) staff       (20)     1178 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12342 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/astrometry.py
--rw-r--r--   0 runner     (501) staff       (20)     5635 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/calibration.py
--rw-r--r--   0 runner     (501) staff       (20)    51063 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/conv.py
--rw-r--r--   0 runner     (501) staff       (20)     9926 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/coordinate.py
--rw-r--r--   0 runner     (501) staff       (20)     7570 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/defaults.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-15 17:28:16.723272 sdss-coordio-1.6.1/src/coordio/etc/
--rw-r--r--   0 runner     (501) staff       (20)       73 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/etc/astrometrynet.cfg
--rw-r--r--   0 runner     (501) staff       (20)      366 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/etc/coordio.yml
--rw-r--r--   0 runner     (501) staff       (20)      722 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    12748 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/extraction.py
--rwxr-xr-x   0 runner     (501) staff       (20)    13362 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/fitData.py
--rw-r--r--   0 runner     (501) staff       (20)    24723 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/guide.py
--rw-r--r--   0 runner     (501) staff       (20)     5870 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/iers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-15 17:28:16.723760 sdss-coordio-1.6.1/src/coordio/include/
--rw-r--r--   0 runner     (501) staff       (20)     1992 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/include/coordio.h
--rw-r--r--   0 runner     (501) staff       (20)     4013 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/positioner.py
--rw-r--r--   0 runner     (501) staff       (20)     4146 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/site.py
--rw-r--r--   0 runner     (501) staff       (20)    14255 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/sky.py
--rw-r--r--   0 runner     (501) staff       (20)     6133 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/sofa_bindings.py
--rw-r--r--   0 runner     (501) staff       (20)    10661 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/tangent.py
--rw-r--r--   0 runner     (501) staff       (20)    12382 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/telescope.py
--rw-r--r--   0 runner     (501) staff       (20)     6451 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/time.py
--rw-r--r--   0 runner     (501) staff       (20)    51552 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/transforms.py
--rw-r--r--   0 runner     (501) staff       (20)    33510 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     3734 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/wok.py
--rw-r--r--   0 runner     (501) staff       (20)    14872 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/zernike.py
--rw-r--r--   0 runner     (501) staff       (20)    12907 2023-01-15 17:27:01.000000 sdss-coordio-1.6.1/src/coordio/zhaoburge.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-01-15 17:28:16.727010 sdss-coordio-1.6.1/src/sdss_coordio.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1737 2023-01-15 17:28:16.000000 sdss-coordio-1.6.1/src/sdss_coordio.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6477 2023-01-15 17:28:16.000000 sdss-coordio-1.6.1/src/sdss_coordio.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-01-15 17:28:16.000000 sdss-coordio-1.6.1/src/sdss_coordio.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-01-15 17:27:24.000000 sdss-coordio-1.6.1/src/sdss_coordio.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      483 2023-01-15 17:28:16.000000 sdss-coordio-1.6.1/src/sdss_coordio.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        8 2023-01-15 17:28:16.000000 sdss-coordio-1.6.1/src/sdss_coordio.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.504047 sdss-coordio-1.7.0/
+-rw-r--r--   0 runner     (501) staff       (20)     1504 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)       62 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     1737 2023-04-15 21:06:00.504233 sdss-coordio-1.7.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      796 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.338636 sdss-coordio-1.7.0/cextern/
+-rw-r--r--   0 runner     (501) staff       (20)      343 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/README.md
+-rw-r--r--   0 runner     (501) staff       (20)    12507 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/conv.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.345707 sdss-coordio-1.7.0/cextern/dimage/
+-rw-r--r--   0 runner     (501) staff       (20)     3150 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dallpeaks.c
+-rw-r--r--   0 runner     (501) staff       (20)     1295 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dcen3x3.c
+-rw-r--r--   0 runner     (501) staff       (20)     3239 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dfind.c
+-rw-r--r--   0 runner     (501) staff       (20)     2553 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dfloodfill.c
+-rw-r--r--   0 runner     (501) staff       (20)     1407 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dimage.h
+-rw-r--r--   0 runner     (501) staff       (20)     6057 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dmedsmooth.c
+-rw-r--r--   0 runner     (501) staff       (20)     1351 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dobjects.c
+-rw-r--r--   0 runner     (501) staff       (20)     3798 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dpeaks.c
+-rw-r--r--   0 runner     (501) staff       (20)     2856 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/drefine.c
+-rw-r--r--   0 runner     (501) staff       (20)     1872 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dselip.c
+-rw-r--r--   0 runner     (501) staff       (20)     1252 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dsigma.c
+-rw-r--r--   0 runner     (501) staff       (20)     3854 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dsmooth.c
+-rw-r--r--   0 runner     (501) staff       (20)       58 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/readme.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1984 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/simplexy.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.477114 sdss-coordio-1.7.0/cextern/sofa/
+-rw-r--r--   0 runner     (501) staff       (20)     6468 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/a2af.c
+-rw-r--r--   0 runner     (501) staff       (20)     6374 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/a2tf.c
+-rw-r--r--   0 runner     (501) staff       (20)     6611 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ab.c
+-rw-r--r--   0 runner     (501) staff       (20)     7187 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ae2hd.c
+-rw-r--r--   0 runner     (501) staff       (20)     6087 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/af2a.c
+-rw-r--r--   0 runner     (501) staff       (20)     4955 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/anp.c
+-rw-r--r--   0 runner     (501) staff       (20)     4983 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/anpm.c
+-rw-r--r--   0 runner     (501) staff       (20)     9173 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apcg.c
+-rw-r--r--   0 runner     (501) staff       (20)     9278 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apcg13.c
+-rw-r--r--   0 runner     (501) staff       (20)     9669 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apci.c
+-rw-r--r--   0 runner     (501) staff       (20)     9954 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apci13.c
+-rw-r--r--   0 runner     (501) staff       (20)    12864 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apco.c
+-rw-r--r--   0 runner     (501) staff       (20)    14172 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apco13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11004 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apcs.c
+-rw-r--r--   0 runner     (501) staff       (20)     9686 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apcs13.c
+-rw-r--r--   0 runner     (501) staff       (20)     8285 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/aper.c
+-rw-r--r--   0 runner     (501) staff       (20)     9207 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/aper13.c
+-rw-r--r--   0 runner     (501) staff       (20)    10588 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apio.c
+-rw-r--r--   0 runner     (501) staff       (20)    12842 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apio13.c
+-rw-r--r--   0 runner     (501) staff       (20)     8257 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atci13.c
+-rw-r--r--   0 runner     (501) staff       (20)     7978 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atciq.c
+-rw-r--r--   0 runner     (501) staff       (20)     9826 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atciqn.c
+-rw-r--r--   0 runner     (501) staff       (20)     7729 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atciqz.c
+-rw-r--r--   0 runner     (501) staff       (20)    12474 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atco13.c
+-rw-r--r--   0 runner     (501) staff       (20)     7919 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atic13.c
+-rw-r--r--   0 runner     (501) staff       (20)     8735 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/aticq.c
+-rw-r--r--   0 runner     (501) staff       (20)    10634 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/aticqn.c
+-rw-r--r--   0 runner     (501) staff       (20)    11485 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atio13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11389 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atioq.c
+-rw-r--r--   0 runner     (501) staff       (20)    12003 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atoc13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11902 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atoi13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11115 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atoiq.c
+-rw-r--r--   0 runner     (501) staff       (20)     6640 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/bi00.c
+-rw-r--r--   0 runner     (501) staff       (20)     8454 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/bp00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7280 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/bp06.c
+-rw-r--r--   0 runner     (501) staff       (20)     5822 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/bpn2xy.c
+-rw-r--r--   0 runner     (501) staff       (20)     7375 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2i00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7362 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2i00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7165 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2i06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7592 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2ibpn.c
+-rw-r--r--   0 runner     (501) staff       (20)     7162 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2ixy.c
+-rw-r--r--   0 runner     (501) staff       (20)     6391 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2ixys.c
+-rw-r--r--   0 runner     (501) staff       (20)     5320 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2s.c
+-rw-r--r--   0 runner     (501) staff       (20)     8083 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2t00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7985 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2t00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7970 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2t06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6652 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2tcio.c
+-rw-r--r--   0 runner     (501) staff       (20)     6679 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2teqx.c
+-rw-r--r--   0 runner     (501) staff       (20)     8786 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2tpe.c
+-rw-r--r--   0 runner     (501) staff       (20)     8249 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2txy.c
+-rw-r--r--   0 runner     (501) staff       (20)     6962 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/cal2jd.c
+-rw-r--r--   0 runner     (501) staff       (20)     4897 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/cp.c
+-rw-r--r--   0 runner     (501) staff       (20)     4990 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/cpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     4974 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/cr.c
+-rw-r--r--   0 runner     (501) staff       (20)     9794 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/d2dtf.c
+-rw-r--r--   0 runner     (501) staff       (20)     7240 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/d2tf.c
+-rw-r--r--   0 runner     (501) staff       (20)    13394 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/dat.c
+-rw-r--r--   0 runner     (501) staff       (20)    63548 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/dtdb.c
+-rw-r--r--   0 runner     (501) staff       (20)     9375 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/dtf2d.c
+-rw-r--r--   0 runner     (501) staff       (20)     7237 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eceq06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7251 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ecm06.c
+-rw-r--r--   0 runner     (501) staff       (20)     6929 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ee00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7105 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ee00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7436 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ee00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     6632 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ee06a.c
+-rw-r--r--   0 runner     (501) staff       (20)    12358 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eect00.c
+-rw-r--r--   0 runner     (501) staff       (20)     6688 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eform.c
+-rw-r--r--   0 runner     (501) staff       (20)     7000 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eo06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6082 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eors.c
+-rw-r--r--   0 runner     (501) staff       (20)     5398 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/epb.c
+-rw-r--r--   0 runner     (501) staff       (20)     5342 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/epb2jd.c
+-rw-r--r--   0 runner     (501) staff       (20)     5327 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/epj.c
+-rw-r--r--   0 runner     (501) staff       (20)     5330 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/epj2jd.c
+-rw-r--r--   0 runner     (501) staff       (20)   152024 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/epv00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7238 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eqec06.c
+-rw-r--r--   0 runner     (501) staff       (20)     6953 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eqeq94.c
+-rw-r--r--   0 runner     (501) staff       (20)     6978 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/era00.c
+-rw-r--r--   0 runner     (501) staff       (20)     5789 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fad03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5756 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fae03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5883 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/faf03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5768 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/faju03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5758 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fal03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5758 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/falp03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5760 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fama03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5770 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fame03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5631 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fane03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5826 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/faom03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5754 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fapa03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5765 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fasa03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5629 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/faur03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5764 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fave03.c
+-rw-r--r--   0 runner     (501) staff       (20)    12333 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk425.c
+-rw-r--r--   0 runner     (501) staff       (20)     9855 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk45z.c
+-rw-r--r--   0 runner     (501) staff       (20)    12391 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk524.c
+-rw-r--r--   0 runner     (501) staff       (20)     7422 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk52h.c
+-rw-r--r--   0 runner     (501) staff       (20)     7286 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk54z.c
+-rw-r--r--   0 runner     (501) staff       (20)     6198 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk5hip.c
+-rw-r--r--   0 runner     (501) staff       (20)     8093 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk5hz.c
+-rw-r--r--   0 runner     (501) staff       (20)     7061 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fw2m.c
+-rw-r--r--   0 runner     (501) staff       (20)     6147 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fw2xy.c
+-rw-r--r--   0 runner     (501) staff       (20)     8396 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/g2icrs.c
+-rw-r--r--   0 runner     (501) staff       (20)     6710 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gc2gd.c
+-rw-r--r--   0 runner     (501) staff       (20)     8338 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gc2gde.c
+-rw-r--r--   0 runner     (501) staff       (20)     6783 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gd2gc.c
+-rw-r--r--   0 runner     (501) staff       (20)     6968 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gd2gce.c
+-rw-r--r--   0 runner     (501) staff       (20)     7699 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gmst00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7337 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gmst06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7688 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gmst82.c
+-rw-r--r--   0 runner     (501) staff       (20)     7470 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gst00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7770 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gst00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7536 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gst06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7174 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gst06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7099 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gst94.c
+-rw-r--r--   0 runner     (501) staff       (20)     7614 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/h2fk5.c
+-rw-r--r--   0 runner     (501) staff       (20)     7382 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/hd2ae.c
+-rw-r--r--   0 runner     (501) staff       (20)     6333 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/hd2pa.c
+-rw-r--r--   0 runner     (501) staff       (20)     8684 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/hfk5z.c
+-rw-r--r--   0 runner     (501) staff       (20)     8382 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/icrs2g.c
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ir.c
+-rw-r--r--   0 runner     (501) staff       (20)     8269 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/jd2cal.c
+-rw-r--r--   0 runner     (501) staff       (20)     7559 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/jdcalf.c
+-rw-r--r--   0 runner     (501) staff       (20)     7662 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ld.c
+-rw-r--r--   0 runner     (501) staff       (20)     8829 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ldn.c
+-rw-r--r--   0 runner     (501) staff       (20)     5982 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ldsun.c
+-rw-r--r--   0 runner     (501) staff       (20)     7014 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/lteceq.c
+-rw-r--r--   0 runner     (501) staff       (20)     7567 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ltecm.c
+-rw-r--r--   0 runner     (501) staff       (20)     7019 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/lteqec.c
+-rw-r--r--   0 runner     (501) staff       (20)     6500 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ltp.c
+-rw-r--r--   0 runner     (501) staff       (20)     6581 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ltpb.c
+-rw-r--r--   0 runner     (501) staff       (20)     7601 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ltpecl.c
+-rw-r--r--   0 runner     (501) staff       (20)     7880 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ltpequ.c
+-rw-r--r--   0 runner     (501) staff       (20)    27755 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/makefile
+-rw-r--r--   0 runner     (501) staff       (20)     6728 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/num00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6713 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/num00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     6660 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/num06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6057 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/numat.c
+-rw-r--r--   0 runner     (501) staff       (20)   119801 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/nut00a.c
+-rw-r--r--   0 runner     (501) staff       (20)    19020 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/nut00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7823 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/nut06a.c
+-rw-r--r--   0 runner     (501) staff       (20)    16295 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/nut80.c
+-rw-r--r--   0 runner     (501) staff       (20)     6473 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/nutm80.c
+-rw-r--r--   0 runner     (501) staff       (20)     6414 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/obl06.c
+-rw-r--r--   0 runner     (501) staff       (20)     6459 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/obl80.c
+-rw-r--r--   0 runner     (501) staff       (20)    13793 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/p06e.c
+-rw-r--r--   0 runner     (501) staff       (20)     5029 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/p2pv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5276 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/p2s.c
+-rw-r--r--   0 runner     (501) staff       (20)     6768 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pap.c
+-rw-r--r--   0 runner     (501) staff       (20)     5638 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pas.c
+-rw-r--r--   0 runner     (501) staff       (20)     7817 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pb06.c
+-rw-r--r--   0 runner     (501) staff       (20)     5008 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pdp.c
+-rw-r--r--   0 runner     (501) staff       (20)     7964 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pfw06.c
+-rw-r--r--   0 runner     (501) staff       (20)    23180 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/plan94.c
+-rw-r--r--   0 runner     (501) staff       (20)     4887 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pm.c
+-rw-r--r--   0 runner     (501) staff       (20)     6579 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmat00.c
+-rw-r--r--   0 runner     (501) staff       (20)     6683 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmat06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7548 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmat76.c
+-rw-r--r--   0 runner     (501) staff       (20)     5090 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmp.c
+-rw-r--r--   0 runner     (501) staff       (20)     7054 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmpx.c
+-rw-r--r--   0 runner     (501) staff       (20)    10220 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmsafe.c
+-rw-r--r--   0 runner     (501) staff       (20)     5495 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn.c
+-rw-r--r--   0 runner     (501) staff       (20)     9146 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn00.c
+-rw-r--r--   0 runner     (501) staff       (20)     8833 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     8825 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     9253 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn06.c
+-rw-r--r--   0 runner     (501) staff       (20)     8282 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6802 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pnm00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6797 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pnm00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     6835 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pnm06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6778 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pnm80.c
+-rw-r--r--   0 runner     (501) staff       (20)     6453 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pom00.c
+-rw-r--r--   0 runner     (501) staff       (20)     5087 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ppp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5275 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ppsp.c
+-rw-r--r--   0 runner     (501) staff       (20)     7813 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pr00.c
+-rw-r--r--   0 runner     (501) staff       (20)     8023 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/prec76.c
+-rw-r--r--   0 runner     (501) staff       (20)     4958 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pv2p.c
+-rw-r--r--   0 runner     (501) staff       (20)     6861 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pv2s.c
+-rw-r--r--   0 runner     (501) staff       (20)     5587 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvdpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5073 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvm.c
+-rw-r--r--   0 runner     (501) staff       (20)     5182 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvmpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5177 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvppv.c
+-rw-r--r--   0 runner     (501) staff       (20)    10128 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvstar.c
+-rw-r--r--   0 runner     (501) staff       (20)     7712 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvtob.c
+-rw-r--r--   0 runner     (501) staff       (20)     5373 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvu.c
+-rw-r--r--   0 runner     (501) staff       (20)     5280 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvup.c
+-rw-r--r--   0 runner     (501) staff       (20)     5842 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5234 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pxp.c
+-rw-r--r--   0 runner     (501) staff       (20)    11663 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/refco.c
+-rw-r--r--   0 runner     (501) staff       (20)     5989 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rm2v.c
+-rw-r--r--   0 runner     (501) staff       (20)     5996 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rv2m.c
+-rw-r--r--   0 runner     (501) staff       (20)     5807 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rx.c
+-rw-r--r--   0 runner     (501) staff       (20)     5298 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rxp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5144 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5337 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rxr.c
+-rw-r--r--   0 runner     (501) staff       (20)     5848 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ry.c
+-rw-r--r--   0 runner     (501) staff       (20)     5817 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rz.c
+-rw-r--r--   0 runner     (501) staff       (20)    15540 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7781 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7772 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s00b.c
+-rw-r--r--   0 runner     (501) staff       (20)    15442 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7799 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     5073 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s2c.c
+-rw-r--r--   0 runner     (501) staff       (20)     5209 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s2p.c
+-rw-r--r--   0 runner     (501) staff       (20)     5636 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s2pv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5282 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s2xpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5877 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sepp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5424 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/seps.c
+-rw-r--r--   0 runner     (501) staff       (20)    26863 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sofa.h
+-rw-r--r--   0 runner     (501) staff       (20)     8772 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sofam.h
+-rw-r--r--   0 runner     (501) staff       (20)     6557 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sp00.c
+-rw-r--r--   0 runner     (501) staff       (20)    10677 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/starpm.c
+-rw-r--r--   0 runner     (501) staff       (20)    11959 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/starpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5038 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sxp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5101 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)   241327 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/t_sofa_c.c
+-rw-r--r--   0 runner     (501) staff       (20)     5845 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/taitt.c
+-rw-r--r--   0 runner     (501) staff       (20)     5901 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/taiut1.c
+-rw-r--r--   0 runner     (501) staff       (20)     7493 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/taiutc.c
+-rw-r--r--   0 runner     (501) staff       (20)     6987 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tcbtdb.c
+-rw-r--r--   0 runner     (501) staff       (20)     5845 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tcgtt.c
+-rw-r--r--   0 runner     (501) staff       (20)     7109 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tdbtcb.c
+-rw-r--r--   0 runner     (501) staff       (20)     6353 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tdbtt.c
+-rw-r--r--   0 runner     (501) staff       (20)     6062 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tf2a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6066 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tf2d.c
+-rw-r--r--   0 runner     (501) staff       (20)     8685 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tpors.c
+-rw-r--r--   0 runner     (501) staff       (20)     8649 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tporv.c
+-rw-r--r--   0 runner     (501) staff       (20)     6534 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tpsts.c
+-rw-r--r--   0 runner     (501) staff       (20)     7337 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tpstv.c
+-rw-r--r--   0 runner     (501) staff       (20)     7253 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tpxes.c
+-rw-r--r--   0 runner     (501) staff       (20)     7927 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tpxev.c
+-rw-r--r--   0 runner     (501) staff       (20)     5136 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tr.c
+-rw-r--r--   0 runner     (501) staff       (20)     5263 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/trxp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5291 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/trxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5841 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tttai.c
+-rw-r--r--   0 runner     (501) staff       (20)     5913 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tttcg.c
+-rw-r--r--   0 runner     (501) staff       (20)     6345 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tttdb.c
+-rw-r--r--   0 runner     (501) staff       (20)     5794 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ttut1.c
+-rw-r--r--   0 runner     (501) staff       (20)     5898 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ut1tai.c
+-rw-r--r--   0 runner     (501) staff       (20)     5798 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ut1tt.c
+-rw-r--r--   0 runner     (501) staff       (20)     8782 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ut1utc.c
+-rw-r--r--   0 runner     (501) staff       (20)     8283 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/utctai.c
+-rw-r--r--   0 runner     (501) staff       (20)     7458 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/utcut1.c
+-rw-r--r--   0 runner     (501) staff       (20)   133674 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/xy06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7028 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/xys00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7010 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/xys00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7056 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/xys06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     4820 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/zp.c
+-rw-r--r--   0 runner     (501) staff       (20)     4874 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/zpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     4967 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/zr.c
+-rw-r--r--   0 runner     (501) staff       (20)     2386 2023-04-15 21:06:00.505559 sdss-coordio-1.7.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2697 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.334758 sdss-coordio-1.7.0/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.489105 sdss-coordio-1.7.0/src/coordio/
+-rw-r--r--   0 runner     (501) staff       (20)     1178 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12342 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/astrometry.py
+-rw-r--r--   0 runner     (501) staff       (20)     5635 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/calibration.py
+-rw-r--r--   0 runner     (501) staff       (20)    51063 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/conv.py
+-rw-r--r--   0 runner     (501) staff       (20)     9926 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/coordinate.py
+-rw-r--r--   0 runner     (501) staff       (20)     7570 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/defaults.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.490147 sdss-coordio-1.7.0/src/coordio/etc/
+-rw-r--r--   0 runner     (501) staff       (20)       73 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/etc/astrometrynet.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      366 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/etc/coordio.yml
+-rw-r--r--   0 runner     (501) staff       (20)      722 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    12748 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/extraction.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    13362 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/fitData.py
+-rw-r--r--   0 runner     (501) staff       (20)    24723 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/guide.py
+-rw-r--r--   0 runner     (501) staff       (20)     5870 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/iers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.490642 sdss-coordio-1.7.0/src/coordio/include/
+-rw-r--r--   0 runner     (501) staff       (20)     1992 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/include/coordio.h
+-rw-r--r--   0 runner     (501) staff       (20)     4013 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/positioner.py
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/site.py
+-rw-r--r--   0 runner     (501) staff       (20)    14255 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/sky.py
+-rw-r--r--   0 runner     (501) staff       (20)     6440 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/sofa_bindings.py
+-rw-r--r--   0 runner     (501) staff       (20)    10661 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/tangent.py
+-rw-r--r--   0 runner     (501) staff       (20)    13390 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/telescope.py
+-rw-r--r--   0 runner     (501) staff       (20)     6451 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/time.py
+-rw-r--r--   0 runner     (501) staff       (20)    51462 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/transforms.py
+-rw-r--r--   0 runner     (501) staff       (20)    33540 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     3734 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/wok.py
+-rw-r--r--   0 runner     (501) staff       (20)    14872 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/zernike.py
+-rw-r--r--   0 runner     (501) staff       (20)    12907 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/zhaoburge.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.494410 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1737 2023-04-15 21:06:00.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6867 2023-04-15 21:06:00.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-15 21:06:00.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-15 21:02:48.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      483 2023-04-15 21:06:00.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        8 2023-04-15 21:06:00.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.503631 sdss-coordio-1.7.0/tests/
+-rw-r--r--   0 runner     (501) staff       (20)    13006 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_conv.py
+-rw-r--r--   0 runner     (501) staff       (20)     7006 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_coordinate.py
+-rw-r--r--   0 runner     (501) staff       (20)     1386 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_fpScale.py
+-rw-r--r--   0 runner     (501) staff       (20)     4290 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_guide.py
+-rw-r--r--   0 runner     (501) staff       (20)     1418 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_iers.py
+-rw-r--r--   0 runner     (501) staff       (20)    11447 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_libcoordio.py
+-rw-r--r--   0 runner     (501) staff       (20)     5271 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_offset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8074 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_plPlug.py
+-rw-r--r--   0 runner     (501) staff       (20)     5525 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_positioner.py
+-rw-r--r--   0 runner     (501) staff       (20)     1105 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_site.py
+-rw-r--r--   0 runner     (501) staff       (20)     5302 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_sky.py
+-rw-r--r--   0 runner     (501) staff       (20)     1171 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_sofa.py
+-rw-r--r--   0 runner     (501) staff       (20)     3340 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_tangent.py
+-rw-r--r--   0 runner     (501) staff       (20)     2738 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_tangentToPositioner2.py
+-rw-r--r--   0 runner     (501) staff       (20)    13872 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_telescope.py
+-rw-r--r--   0 runner     (501) staff       (20)     1407 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_time.py
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_wok.py
+-rw-r--r--   0 runner     (501) staff       (20)     1363 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_zern.py
```

### Comparing `sdss-coordio-1.6.1/LICENSE.md` & `sdss-coordio-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/PKG-INFO` & `sdss-coordio-1.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-coordio
-Version: 1.6.1
+Version: 1.7.0
 Summary: Coordinate conversion for SDSS-V
 Home-page: https://github.com/sdss/coordio
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/coordio
 Project-URL: Documentation, https://sdss-coordio.readthedocs.org
```

### Comparing `sdss-coordio-1.6.1/README.md` & `sdss-coordio-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/conv.cpp` & `sdss-coordio-1.7.0/cextern/conv.cpp`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dallpeaks.c` & `sdss-coordio-1.7.0/cextern/dimage/dallpeaks.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dcen3x3.c` & `sdss-coordio-1.7.0/cextern/dimage/dcen3x3.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dfind.c` & `sdss-coordio-1.7.0/cextern/dimage/dfind.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dfloodfill.c` & `sdss-coordio-1.7.0/cextern/dimage/dfloodfill.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dimage.h` & `sdss-coordio-1.7.0/cextern/dimage/dimage.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dmedsmooth.c` & `sdss-coordio-1.7.0/cextern/dimage/dmedsmooth.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dobjects.c` & `sdss-coordio-1.7.0/cextern/dimage/dobjects.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dpeaks.c` & `sdss-coordio-1.7.0/cextern/dimage/dpeaks.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/drefine.c` & `sdss-coordio-1.7.0/cextern/dimage/drefine.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dselip.c` & `sdss-coordio-1.7.0/cextern/dimage/dselip.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dsigma.c` & `sdss-coordio-1.7.0/cextern/dimage/dsigma.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/dsmooth.c` & `sdss-coordio-1.7.0/cextern/dimage/dsmooth.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/dimage/simplexy.c` & `sdss-coordio-1.7.0/cextern/dimage/simplexy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/a2af.c` & `sdss-coordio-1.7.0/cextern/sofa/a2af.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/a2tf.c` & `sdss-coordio-1.7.0/cextern/sofa/a2tf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ab.c` & `sdss-coordio-1.7.0/cextern/sofa/ab.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ae2hd.c` & `sdss-coordio-1.7.0/cextern/sofa/ae2hd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/af2a.c` & `sdss-coordio-1.7.0/cextern/sofa/af2a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/anp.c` & `sdss-coordio-1.7.0/cextern/sofa/anp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/anpm.c` & `sdss-coordio-1.7.0/cextern/sofa/anpm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/apcg.c` & `sdss-coordio-1.7.0/cextern/sofa/apcg.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/apcg13.c` & `sdss-coordio-1.7.0/cextern/sofa/apcg13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/apci.c` & `sdss-coordio-1.7.0/cextern/sofa/apci.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/apci13.c` & `sdss-coordio-1.7.0/cextern/sofa/apci13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/apco.c` & `sdss-coordio-1.7.0/cextern/sofa/apco.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/apco13.c` & `sdss-coordio-1.7.0/cextern/sofa/apco13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/apcs.c` & `sdss-coordio-1.7.0/cextern/sofa/apcs.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/apcs13.c` & `sdss-coordio-1.7.0/cextern/sofa/apcs13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/aper.c` & `sdss-coordio-1.7.0/cextern/sofa/aper.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/aper13.c` & `sdss-coordio-1.7.0/cextern/sofa/aper13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/apio.c` & `sdss-coordio-1.7.0/cextern/sofa/apio.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/apio13.c` & `sdss-coordio-1.7.0/cextern/sofa/apio13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atci13.c` & `sdss-coordio-1.7.0/cextern/sofa/atci13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atciq.c` & `sdss-coordio-1.7.0/cextern/sofa/atciq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atciqn.c` & `sdss-coordio-1.7.0/cextern/sofa/atciqn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atciqz.c` & `sdss-coordio-1.7.0/cextern/sofa/atciqz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atco13.c` & `sdss-coordio-1.7.0/cextern/sofa/atco13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atic13.c` & `sdss-coordio-1.7.0/cextern/sofa/atic13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/aticq.c` & `sdss-coordio-1.7.0/cextern/sofa/aticq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/aticqn.c` & `sdss-coordio-1.7.0/cextern/sofa/aticqn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atio13.c` & `sdss-coordio-1.7.0/cextern/sofa/atio13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atioq.c` & `sdss-coordio-1.7.0/cextern/sofa/atioq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atoc13.c` & `sdss-coordio-1.7.0/cextern/sofa/atoc13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atoi13.c` & `sdss-coordio-1.7.0/cextern/sofa/atoi13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/atoiq.c` & `sdss-coordio-1.7.0/cextern/sofa/atoiq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/bi00.c` & `sdss-coordio-1.7.0/cextern/sofa/bi00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/bp00.c` & `sdss-coordio-1.7.0/cextern/sofa/bp00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/bp06.c` & `sdss-coordio-1.7.0/cextern/sofa/bp06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/bpn2xy.c` & `sdss-coordio-1.7.0/cextern/sofa/bpn2xy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2i00a.c` & `sdss-coordio-1.7.0/cextern/sofa/c2i00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2i00b.c` & `sdss-coordio-1.7.0/cextern/sofa/c2i00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2i06a.c` & `sdss-coordio-1.7.0/cextern/sofa/c2i06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2ibpn.c` & `sdss-coordio-1.7.0/cextern/sofa/c2ibpn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2ixy.c` & `sdss-coordio-1.7.0/cextern/sofa/c2ixy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2ixys.c` & `sdss-coordio-1.7.0/cextern/sofa/c2ixys.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2s.c` & `sdss-coordio-1.7.0/cextern/sofa/c2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2t00a.c` & `sdss-coordio-1.7.0/cextern/sofa/c2t00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2t00b.c` & `sdss-coordio-1.7.0/cextern/sofa/c2t00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2t06a.c` & `sdss-coordio-1.7.0/cextern/sofa/c2t06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2tcio.c` & `sdss-coordio-1.7.0/cextern/sofa/c2tcio.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2teqx.c` & `sdss-coordio-1.7.0/cextern/sofa/c2teqx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2tpe.c` & `sdss-coordio-1.7.0/cextern/sofa/c2tpe.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/c2txy.c` & `sdss-coordio-1.7.0/cextern/sofa/c2txy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/cal2jd.c` & `sdss-coordio-1.7.0/cextern/sofa/cal2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/cp.c` & `sdss-coordio-1.7.0/cextern/sofa/cp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/cpv.c` & `sdss-coordio-1.7.0/cextern/sofa/cpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/cr.c` & `sdss-coordio-1.7.0/cextern/sofa/cr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/d2dtf.c` & `sdss-coordio-1.7.0/cextern/sofa/d2dtf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/d2tf.c` & `sdss-coordio-1.7.0/cextern/sofa/d2tf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/dat.c` & `sdss-coordio-1.7.0/cextern/sofa/dat.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/dtdb.c` & `sdss-coordio-1.7.0/cextern/sofa/dtdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/dtf2d.c` & `sdss-coordio-1.7.0/cextern/sofa/dtf2d.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/eceq06.c` & `sdss-coordio-1.7.0/cextern/sofa/eceq06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ecm06.c` & `sdss-coordio-1.7.0/cextern/sofa/ecm06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ee00.c` & `sdss-coordio-1.7.0/cextern/sofa/ee00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ee00a.c` & `sdss-coordio-1.7.0/cextern/sofa/ee00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ee00b.c` & `sdss-coordio-1.7.0/cextern/sofa/ee00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ee06a.c` & `sdss-coordio-1.7.0/cextern/sofa/ee06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/eect00.c` & `sdss-coordio-1.7.0/cextern/sofa/eect00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/eform.c` & `sdss-coordio-1.7.0/cextern/sofa/eform.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/eo06a.c` & `sdss-coordio-1.7.0/cextern/sofa/eo06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/eors.c` & `sdss-coordio-1.7.0/cextern/sofa/eors.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/epb.c` & `sdss-coordio-1.7.0/cextern/sofa/epb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/epb2jd.c` & `sdss-coordio-1.7.0/cextern/sofa/epb2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/epj.c` & `sdss-coordio-1.7.0/cextern/sofa/epj.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/epj2jd.c` & `sdss-coordio-1.7.0/cextern/sofa/epj2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/epv00.c` & `sdss-coordio-1.7.0/cextern/sofa/epv00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/eqec06.c` & `sdss-coordio-1.7.0/cextern/sofa/eqec06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/eqeq94.c` & `sdss-coordio-1.7.0/cextern/sofa/eqeq94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/era00.c` & `sdss-coordio-1.7.0/cextern/sofa/era00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fad03.c` & `sdss-coordio-1.7.0/cextern/sofa/fad03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fae03.c` & `sdss-coordio-1.7.0/cextern/sofa/fae03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/faf03.c` & `sdss-coordio-1.7.0/cextern/sofa/faf03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/faju03.c` & `sdss-coordio-1.7.0/cextern/sofa/faju03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fal03.c` & `sdss-coordio-1.7.0/cextern/sofa/fal03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/falp03.c` & `sdss-coordio-1.7.0/cextern/sofa/falp03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fama03.c` & `sdss-coordio-1.7.0/cextern/sofa/fama03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fame03.c` & `sdss-coordio-1.7.0/cextern/sofa/fame03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fane03.c` & `sdss-coordio-1.7.0/cextern/sofa/fane03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/faom03.c` & `sdss-coordio-1.7.0/cextern/sofa/faom03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fapa03.c` & `sdss-coordio-1.7.0/cextern/sofa/fapa03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fasa03.c` & `sdss-coordio-1.7.0/cextern/sofa/fasa03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/faur03.c` & `sdss-coordio-1.7.0/cextern/sofa/faur03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fave03.c` & `sdss-coordio-1.7.0/cextern/sofa/fave03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fk425.c` & `sdss-coordio-1.7.0/cextern/sofa/fk425.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fk45z.c` & `sdss-coordio-1.7.0/cextern/sofa/fk45z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fk524.c` & `sdss-coordio-1.7.0/cextern/sofa/fk524.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fk52h.c` & `sdss-coordio-1.7.0/cextern/sofa/fk52h.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fk54z.c` & `sdss-coordio-1.7.0/cextern/sofa/fk54z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fk5hip.c` & `sdss-coordio-1.7.0/cextern/sofa/fk5hip.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fk5hz.c` & `sdss-coordio-1.7.0/cextern/sofa/fk5hz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fw2m.c` & `sdss-coordio-1.7.0/cextern/sofa/fw2m.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/fw2xy.c` & `sdss-coordio-1.7.0/cextern/sofa/fw2xy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/g2icrs.c` & `sdss-coordio-1.7.0/cextern/sofa/g2icrs.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gc2gd.c` & `sdss-coordio-1.7.0/cextern/sofa/gc2gd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gc2gde.c` & `sdss-coordio-1.7.0/cextern/sofa/gc2gde.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gd2gc.c` & `sdss-coordio-1.7.0/cextern/sofa/gd2gc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gd2gce.c` & `sdss-coordio-1.7.0/cextern/sofa/gd2gce.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gmst00.c` & `sdss-coordio-1.7.0/cextern/sofa/gmst00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gmst06.c` & `sdss-coordio-1.7.0/cextern/sofa/gmst06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gmst82.c` & `sdss-coordio-1.7.0/cextern/sofa/gmst82.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gst00a.c` & `sdss-coordio-1.7.0/cextern/sofa/gst00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gst00b.c` & `sdss-coordio-1.7.0/cextern/sofa/gst00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gst06.c` & `sdss-coordio-1.7.0/cextern/sofa/gst06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gst06a.c` & `sdss-coordio-1.7.0/cextern/sofa/gst06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/gst94.c` & `sdss-coordio-1.7.0/cextern/sofa/gst94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/h2fk5.c` & `sdss-coordio-1.7.0/cextern/sofa/h2fk5.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/hd2ae.c` & `sdss-coordio-1.7.0/cextern/sofa/hd2ae.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/hd2pa.c` & `sdss-coordio-1.7.0/cextern/sofa/hd2pa.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/hfk5z.c` & `sdss-coordio-1.7.0/cextern/sofa/hfk5z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/icrs2g.c` & `sdss-coordio-1.7.0/cextern/sofa/icrs2g.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ir.c` & `sdss-coordio-1.7.0/cextern/sofa/ir.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/jd2cal.c` & `sdss-coordio-1.7.0/cextern/sofa/jd2cal.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/jdcalf.c` & `sdss-coordio-1.7.0/cextern/sofa/jdcalf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ld.c` & `sdss-coordio-1.7.0/cextern/sofa/ld.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ldn.c` & `sdss-coordio-1.7.0/cextern/sofa/ldn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ldsun.c` & `sdss-coordio-1.7.0/cextern/sofa/ldsun.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/lteceq.c` & `sdss-coordio-1.7.0/cextern/sofa/lteceq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ltecm.c` & `sdss-coordio-1.7.0/cextern/sofa/ltecm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/lteqec.c` & `sdss-coordio-1.7.0/cextern/sofa/lteqec.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ltp.c` & `sdss-coordio-1.7.0/cextern/sofa/ltp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ltpb.c` & `sdss-coordio-1.7.0/cextern/sofa/ltpb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ltpecl.c` & `sdss-coordio-1.7.0/cextern/sofa/ltpecl.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ltpequ.c` & `sdss-coordio-1.7.0/cextern/sofa/ltpequ.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/makefile` & `sdss-coordio-1.7.0/cextern/sofa/makefile`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/num00a.c` & `sdss-coordio-1.7.0/cextern/sofa/num00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/num00b.c` & `sdss-coordio-1.7.0/cextern/sofa/num00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/num06a.c` & `sdss-coordio-1.7.0/cextern/sofa/num06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/numat.c` & `sdss-coordio-1.7.0/cextern/sofa/numat.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/nut00a.c` & `sdss-coordio-1.7.0/cextern/sofa/nut00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/nut00b.c` & `sdss-coordio-1.7.0/cextern/sofa/nut00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/nut06a.c` & `sdss-coordio-1.7.0/cextern/sofa/nut06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/nut80.c` & `sdss-coordio-1.7.0/cextern/sofa/nut80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/nutm80.c` & `sdss-coordio-1.7.0/cextern/sofa/nutm80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/obl06.c` & `sdss-coordio-1.7.0/cextern/sofa/obl06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/obl80.c` & `sdss-coordio-1.7.0/cextern/sofa/obl80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/p06e.c` & `sdss-coordio-1.7.0/cextern/sofa/p06e.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/p2pv.c` & `sdss-coordio-1.7.0/cextern/sofa/p2pv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/p2s.c` & `sdss-coordio-1.7.0/cextern/sofa/p2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pap.c` & `sdss-coordio-1.7.0/cextern/sofa/pap.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pas.c` & `sdss-coordio-1.7.0/cextern/sofa/pas.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pb06.c` & `sdss-coordio-1.7.0/cextern/sofa/pb06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pdp.c` & `sdss-coordio-1.7.0/cextern/sofa/pdp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pfw06.c` & `sdss-coordio-1.7.0/cextern/sofa/pfw06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/plan94.c` & `sdss-coordio-1.7.0/cextern/sofa/plan94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pm.c` & `sdss-coordio-1.7.0/cextern/sofa/pm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pmat00.c` & `sdss-coordio-1.7.0/cextern/sofa/pmat00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pmat06.c` & `sdss-coordio-1.7.0/cextern/sofa/pmat06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pmat76.c` & `sdss-coordio-1.7.0/cextern/sofa/pmat76.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pmp.c` & `sdss-coordio-1.7.0/cextern/sofa/pmp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pmpx.c` & `sdss-coordio-1.7.0/cextern/sofa/pmpx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pmsafe.c` & `sdss-coordio-1.7.0/cextern/sofa/pmsafe.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pn.c` & `sdss-coordio-1.7.0/cextern/sofa/pn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pn00.c` & `sdss-coordio-1.7.0/cextern/sofa/pn00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pn00a.c` & `sdss-coordio-1.7.0/cextern/sofa/pn00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pn00b.c` & `sdss-coordio-1.7.0/cextern/sofa/pn00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pn06.c` & `sdss-coordio-1.7.0/cextern/sofa/pn06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pn06a.c` & `sdss-coordio-1.7.0/cextern/sofa/pn06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pnm00a.c` & `sdss-coordio-1.7.0/cextern/sofa/pnm00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pnm00b.c` & `sdss-coordio-1.7.0/cextern/sofa/pnm00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pnm06a.c` & `sdss-coordio-1.7.0/cextern/sofa/pnm06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pnm80.c` & `sdss-coordio-1.7.0/cextern/sofa/pnm80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pom00.c` & `sdss-coordio-1.7.0/cextern/sofa/pom00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ppp.c` & `sdss-coordio-1.7.0/cextern/sofa/ppp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ppsp.c` & `sdss-coordio-1.7.0/cextern/sofa/ppsp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pr00.c` & `sdss-coordio-1.7.0/cextern/sofa/pr00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/prec76.c` & `sdss-coordio-1.7.0/cextern/sofa/prec76.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pv2p.c` & `sdss-coordio-1.7.0/cextern/sofa/pv2p.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pv2s.c` & `sdss-coordio-1.7.0/cextern/sofa/pv2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pvdpv.c` & `sdss-coordio-1.7.0/cextern/sofa/pvdpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pvm.c` & `sdss-coordio-1.7.0/cextern/sofa/pvm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pvmpv.c` & `sdss-coordio-1.7.0/cextern/sofa/pvmpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pvppv.c` & `sdss-coordio-1.7.0/cextern/sofa/pvppv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pvstar.c` & `sdss-coordio-1.7.0/cextern/sofa/pvstar.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pvtob.c` & `sdss-coordio-1.7.0/cextern/sofa/pvtob.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pvu.c` & `sdss-coordio-1.7.0/cextern/sofa/pvu.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pvup.c` & `sdss-coordio-1.7.0/cextern/sofa/pvup.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pvxpv.c` & `sdss-coordio-1.7.0/cextern/sofa/pvxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/pxp.c` & `sdss-coordio-1.7.0/cextern/sofa/pxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/refco.c` & `sdss-coordio-1.7.0/cextern/sofa/refco.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/rm2v.c` & `sdss-coordio-1.7.0/cextern/sofa/rm2v.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/rv2m.c` & `sdss-coordio-1.7.0/cextern/sofa/rv2m.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/rx.c` & `sdss-coordio-1.7.0/cextern/sofa/rx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/rxp.c` & `sdss-coordio-1.7.0/cextern/sofa/rxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/rxpv.c` & `sdss-coordio-1.7.0/cextern/sofa/rxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/rxr.c` & `sdss-coordio-1.7.0/cextern/sofa/rxr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ry.c` & `sdss-coordio-1.7.0/cextern/sofa/ry.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/rz.c` & `sdss-coordio-1.7.0/cextern/sofa/rz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/s00.c` & `sdss-coordio-1.7.0/cextern/sofa/s00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/s00a.c` & `sdss-coordio-1.7.0/cextern/sofa/s00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/s00b.c` & `sdss-coordio-1.7.0/cextern/sofa/s00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/s06.c` & `sdss-coordio-1.7.0/cextern/sofa/s06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/s06a.c` & `sdss-coordio-1.7.0/cextern/sofa/s06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/s2c.c` & `sdss-coordio-1.7.0/cextern/sofa/s2c.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/s2p.c` & `sdss-coordio-1.7.0/cextern/sofa/s2p.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/s2pv.c` & `sdss-coordio-1.7.0/cextern/sofa/s2pv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/s2xpv.c` & `sdss-coordio-1.7.0/cextern/sofa/s2xpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/sepp.c` & `sdss-coordio-1.7.0/cextern/sofa/sepp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/seps.c` & `sdss-coordio-1.7.0/cextern/sofa/seps.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/sofa.h` & `sdss-coordio-1.7.0/cextern/sofa/sofa.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/sofam.h` & `sdss-coordio-1.7.0/cextern/sofa/sofam.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/sp00.c` & `sdss-coordio-1.7.0/cextern/sofa/sp00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/starpm.c` & `sdss-coordio-1.7.0/cextern/sofa/starpm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/starpv.c` & `sdss-coordio-1.7.0/cextern/sofa/starpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/sxp.c` & `sdss-coordio-1.7.0/cextern/sofa/sxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/sxpv.c` & `sdss-coordio-1.7.0/cextern/sofa/sxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/t_sofa_c.c` & `sdss-coordio-1.7.0/cextern/sofa/t_sofa_c.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/taitt.c` & `sdss-coordio-1.7.0/cextern/sofa/taitt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/taiut1.c` & `sdss-coordio-1.7.0/cextern/sofa/taiut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/taiutc.c` & `sdss-coordio-1.7.0/cextern/sofa/taiutc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tcbtdb.c` & `sdss-coordio-1.7.0/cextern/sofa/tcbtdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tcgtt.c` & `sdss-coordio-1.7.0/cextern/sofa/tcgtt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tdbtcb.c` & `sdss-coordio-1.7.0/cextern/sofa/tdbtcb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tdbtt.c` & `sdss-coordio-1.7.0/cextern/sofa/tdbtt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tf2a.c` & `sdss-coordio-1.7.0/cextern/sofa/tf2a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tf2d.c` & `sdss-coordio-1.7.0/cextern/sofa/tf2d.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tpors.c` & `sdss-coordio-1.7.0/cextern/sofa/tpors.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tporv.c` & `sdss-coordio-1.7.0/cextern/sofa/tporv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tpsts.c` & `sdss-coordio-1.7.0/cextern/sofa/tpsts.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tpstv.c` & `sdss-coordio-1.7.0/cextern/sofa/tpstv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tpxes.c` & `sdss-coordio-1.7.0/cextern/sofa/tpxes.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tpxev.c` & `sdss-coordio-1.7.0/cextern/sofa/tpxev.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tr.c` & `sdss-coordio-1.7.0/cextern/sofa/tr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/trxp.c` & `sdss-coordio-1.7.0/cextern/sofa/trxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/trxpv.c` & `sdss-coordio-1.7.0/cextern/sofa/trxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tttai.c` & `sdss-coordio-1.7.0/cextern/sofa/tttai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tttcg.c` & `sdss-coordio-1.7.0/cextern/sofa/tttcg.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/tttdb.c` & `sdss-coordio-1.7.0/cextern/sofa/tttdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ttut1.c` & `sdss-coordio-1.7.0/cextern/sofa/ttut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ut1tai.c` & `sdss-coordio-1.7.0/cextern/sofa/ut1tai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ut1tt.c` & `sdss-coordio-1.7.0/cextern/sofa/ut1tt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/ut1utc.c` & `sdss-coordio-1.7.0/cextern/sofa/ut1utc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/utctai.c` & `sdss-coordio-1.7.0/cextern/sofa/utctai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/utcut1.c` & `sdss-coordio-1.7.0/cextern/sofa/utcut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/xy06.c` & `sdss-coordio-1.7.0/cextern/sofa/xy06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/xys00a.c` & `sdss-coordio-1.7.0/cextern/sofa/xys00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/xys00b.c` & `sdss-coordio-1.7.0/cextern/sofa/xys00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/xys06a.c` & `sdss-coordio-1.7.0/cextern/sofa/xys06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/zp.c` & `sdss-coordio-1.7.0/cextern/sofa/zp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/zpv.c` & `sdss-coordio-1.7.0/cextern/sofa/zpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/cextern/sofa/zr.c` & `sdss-coordio-1.7.0/cextern/sofa/zr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/setup.cfg` & `sdss-coordio-1.7.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-coordio
-version = 1.6.1
+version = 1.7.0
 author = Conor Sayres
 author_email = csayres@uw.edu
 description = Coordinate conversion for SDSS-V
 url = https://github.com/sdss/coordio
 project_urls = 
 	Repository = https://github.com/sdss/coordio
 	Documentation = https://sdss-coordio.readthedocs.org
@@ -30,15 +30,16 @@
 python_requires = >=3.7
 packages = find:
 package_dir = 
 	= src
 setup_requires = 
 	pybind11>=2.6.2
 install_requires = 
-	sdsstools>=1.0.0
+	sdsstools>=1.0.0; python_version>'3.7'
+	sdsstools<1.0.0; python_version<='3.7'
 	numpy<1.23.0; python_version<='3.7'
 	numpy>=1.23.0; python_version>'3.7'
 	pandas>=1.2.1
 	matplotlib>=3.1.1
 	scipy>=1.2.1
 	pybind11>=2.6.2
 	scikit-image>=0.17.2
@@ -64,15 +65,14 @@
 	doc8>=0.8.0
 	pytest>=5.2.2
 	pytest-asyncio>=0.10.0
 	pytest-cov>=2.8.1
 	pytest-mock>=1.13.0
 	pytest-sugar>=0.9.2
 	isort>=4.3.21
-	codecov>=2.0.15
 	coverage[toml]>=5.0
 	ipdb>=0.12.3
 	rstcheck>=3.3.1
 	twine>=3.4.2
 	wheel>=0.36.2
 	sphinx>=4.0
```

### Comparing `sdss-coordio-1.6.1/setup.py` & `sdss-coordio-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/__init__.py` & `sdss-coordio-1.7.0/src/coordio/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/astrometry.py` & `sdss-coordio-1.7.0/src/coordio/astrometry.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/calibration.py` & `sdss-coordio-1.7.0/src/coordio/calibration.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/conv.py` & `sdss-coordio-1.7.0/src/coordio/conv.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/coordinate.py` & `sdss-coordio-1.7.0/src/coordio/coordinate.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/defaults.py` & `sdss-coordio-1.7.0/src/coordio/defaults.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/exceptions.py` & `sdss-coordio-1.7.0/src/coordio/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/extraction.py` & `sdss-coordio-1.7.0/src/coordio/extraction.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/fitData.py` & `sdss-coordio-1.7.0/src/coordio/fitData.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/guide.py` & `sdss-coordio-1.7.0/src/coordio/guide.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/iers.py` & `sdss-coordio-1.7.0/src/coordio/iers.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/include/coordio.h` & `sdss-coordio-1.7.0/src/coordio/include/coordio.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/positioner.py` & `sdss-coordio-1.7.0/src/coordio/positioner.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/site.py` & `sdss-coordio-1.7.0/src/coordio/site.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/sky.py` & `sdss-coordio-1.7.0/src/coordio/sky.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/sofa_bindings.py` & `sdss-coordio-1.7.0/src/coordio/sofa_bindings.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,16 +80,21 @@
     # args: double az, double alt, double latitude, double *ha, double *dec
     ('iauAe2hd', (c_double, c_double, c_double,
                   POINTER(c_double), POINTER(c_double))),
 
     # Earth rotation angle
     # sum of the arguments should be jd in the UT1 scale
     # args: double jd, double 0
-    ('iauEra00', (c_double, c_double))
+    ('iauEra00', (c_double, c_double)),
 
+    # Determine the constants A and B in the atmospheric refraction model
+    # dZ = A tan Z + B tan^3 Z.
+    # args: double phpa, double tc, double rh, double wl, double *refa, double *refb
+    ('iauRefco', (c_double, c_double, c_double, c_double,
+                  POINTER(c_double), POINTER(c_double)))
 ]
 
 
 class SOFA(ctypes.CDLL):
     """Load the SOFA C extension.
 
     Parameters
```

### Comparing `sdss-coordio-1.6.1/src/coordio/tangent.py` & `sdss-coordio-1.7.0/src/coordio/tangent.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/telescope.py` & `sdss-coordio-1.7.0/src/coordio/telescope.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 
 from typing import TYPE_CHECKING
 
 import numpy
 
 from . import conv, defaults
 from .conv import cart2FieldAngle, sph2Cart
-from .coordinate import (Coordinate, Coordinate2D, Coordinate3D,
-                         verifySite, verifyWavelength)
+from .coordinate import (
+    Coordinate,
+    Coordinate2D,
+    Coordinate3D,
+    verifySite,
+    verifyWavelength
+)
 from .exceptions import CoordIOError
 
 
 if TYPE_CHECKING:
     from .site import Site
     from .sky import Observed
 
@@ -208,45 +213,68 @@
         to BOSS, Apogee, and sdss-r band (GFA).  Defaults to GFA wavelength.
     site : `.Site`
         Used to pick the focal plane model to use which is telescope dependent
     fpScale : float
         Multiplicative scale factor to apply between wok and focal
         coords.  An adjustment to the focal plane model.  Defaults to
         coordio.defaults.FOCAL_SCALE.
+    use_closest_wavelength : bool
+        If `True`, uses the ZEMAX model with the closes wavelength to the
+        input wavelength.
 
     Attributes
     -----------
     b : numpy.ndarray
         A 1D array containing the location of the spherical fit's center
         (origin of rays) along the optical axis in mm.  Varies with wavelength.
     R : numpy.ndarray
         1D array containing the radius of curvature for the spherical fit in
         mm.  Varies with wavelength.
     field_warn: numpy.ndarray
         boolean array indicating suspect conversions from large field angles
     """
 
-    __extra_params__ = ["site", "fpScale"]
+    __extra_params__ = ["site", "fpScale", "use_closest_wavelength"]
     __extra_arrays__ = ["wavelength"]
     __computed_arrays__ = ["b", "R"]
     __warn_arrays__ = ["field_warn"]
 
     b: numpy.ndarray
     R: numpy.ndarray
     field_warn: numpy.ndarray
     wavelength: numpy.ndarray
     site: Site
     fpScale: float
+    use_closest_wavelength: bool
 
     def __new__(cls, value, **kwargs):
 
         verifySite(kwargs)
 
+        use_closest_wavelength = kwargs.get('use_closest_wavelength', False)
+
+        # If using the closes wavelength, override the wavelength entry in kwargs
+        # with an array with the closest valid wavelength for each input wavelength.
+        wls = kwargs.get('wavelength', None)
+        if wls is not None and use_closest_wavelength:
+            if hasattr(wls, "__len__"):
+                # array passed
+                wls = numpy.array(wls, dtype=numpy.float64)
+            else:
+                # single value passed
+                wls = numpy.zeros(len(value)) + float(wls)
+
+            valid_wls = numpy.array(list(defaults.VALID_WAVELENGTHS))
+            nearest = valid_wls[abs(wls[None, :] - valid_wls[:, None]).argmin(axis=0)]
+            kwargs['wavelength'] = nearest
+
         verifyWavelength(
-            kwargs, len(value), strict=True
+            kwargs,
+            len(value),
+            strict=True,
         )
 
         fpScale = kwargs.get("fpScale", None)
         if fpScale is None:
             if kwargs["site"].name == "APO":
                 kwargs["fpScale"] = defaults.SITE_TO_SCALE["APO"]
             elif kwargs["site"].name == "LCO":
```

### Comparing `sdss-coordio-1.6.1/src/coordio/time.py` & `sdss-coordio-1.7.0/src/coordio/time.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/transforms.py` & `sdss-coordio-1.7.0/src/coordio/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -744,20 +744,31 @@
 # hogg fourier basis fit stuff
 
 IMAX = 32 # maximum integer wave number
 DELTAK = 2. * numpy.pi / 10000.0 # wave number spacing in inverse pixels
 _wcd = os.environ.get('WOKCALIB_DIR')
 ### BIG WARNING ### if two wok calib dirs are present just take the first one
 ### should eventually move this to calibrations for better handling
-if ":" in _wcd:
-    _wcd = _wcd.split(":")[0]
-with open(os.path.join(_wcd, "beta_x.npy"), "rb") as f:
-    beta_x = numpy.load(f)
-with open(os.path.join(_wcd, "beta_y.npy"), "rb") as f:
-    beta_y = numpy.load(f)
+beta_x_apo = None
+beta_y_apo = None
+beta_x_lco = None
+beta_y_lco = None
+for _path in _wcd.split(":"):
+    with open(os.path.join(_path, "beta_x.npy"), "rb") as f:
+        beta_x = numpy.load(f)
+    with open(os.path.join(_path, "beta_y.npy"), "rb") as f:
+        beta_y = numpy.load(f)
+    if "/lco/" in _path:
+        beta_x_lco = beta_x.copy()
+        beta_y_lco = beta_y.copy()
+    else:
+        beta_x_apo = beta_x.copy()
+        beta_y_apo = beta_y.copy()
+beta_x = None
+beta_y = None
 
 
 # functions to set up design matrices
 
 
 def fourier_functions(xs, ys):
     n = len(xs)
@@ -779,18 +790,22 @@
     fxs, fys, iis = fourier_functions(xs, ys)
     n, p = fxs.shape
     Xbig = (fxs[:, :, None] * fys[:, None, :]).reshape((n, p * p))
     i2plusj2 = (iis[:, None] ** 2 + iis[None, :] ** 2).reshape(p * p)
     return Xbig[:, i2plusj2 <= IMAX ** 2]
 
 
-def updateCCDMeas(x,y, dxythresh=0.75):
+def updateCCDMeas(x,y,dxythresh=0.75,site="APO"):
     X = design_matrix(x,y)
-    dx = X @ beta_x
-    dy = X @ beta_y
+    if site == "APO":
+        dx = X @ beta_x_apo
+        dy = X @ beta_y_apo
+    else:
+        dx = X @ beta_x_lco
+        dy = X @ beta_y_lco
 
     rejectInds = (numpy.abs(dx) > dxythresh) | (numpy.abs(dy) > dxythresh)
 
     newX = x - dx
     newY = y - dy
 
     newX[rejectInds] = x[rejectInds]
@@ -824,26 +839,29 @@
        1.01954593e-06,  -2.25406706e-06,   2.50511002e-08,  -9.82154214e-09,
       -4.41479884e-09
     ])
     telRotAngRef = 135.4
     rotAngDir = 1
     centType = "zbplus2"
     telescopePlateScale = 0.060 # mm/arcsec
+    nudgeOffX = 1000 # fix nudge model after FVC resize
+    site = "APO"
 
     def __init__(
         self,
         fvcImgData,
         positionerCoords,
         telRotAng,
         plotPathPrefix=None,
         positionerTable=calibration.positionerTable,
         wokCoords=calibration.wokCoords,
         fiducialCoords=calibration.fiducialCoords,
         telRotAngRef=None,
-        polids=None
+        polids=None,
+        nudgeAdjust=True
     ):
         """
         Parameters
         -------------
         fvcImgData : numpy.ndarray
             raw image data from the fvc
         positionerCoords : pandas.DataFrame
@@ -870,14 +888,15 @@
             telescope rotator angle in mount coordinate degrees at
             which xyCCD ~= xyWok directions.
             Default is 135.4 (for APO)
         polids : 1D array or None
             list of integers for selecting zhaoburge basis polynomials.
             Default is supplied by class attribute polids
         """
+        self.nudgeAdjust = nudgeAdjust
 
         self.fvcImgData = numpy.array(fvcImgData, dtype=numpy.float32)
         # apply rough bias/background subtraction
         # rough bias/bg subtract
         imbias = numpy.median(self.fvcImgData, axis=0)
         imbias = numpy.outer(
             numpy.ones(self.fvcImgData.shape[0], dtype=numpy.float32),
@@ -1050,110 +1069,88 @@
             err=self.bkg.globalrms,
         )
 
         # get rid of obvious bogus detections
         objects = objects[objects["npix"] > centroidMinNpix]
         # remove detections near edges of chip
         # (causes issues for unlucky winpos detections)
-        objects = objects[objects["x"] > 500]
-        objects = objects[objects["x"] < 7500]
-        objects = objects[objects["y"] > 30]
-        objects = objects[objects["y"] < 5970]
+        # objects = objects[objects["x"] > 500]
+        # objects = objects[objects["x"] < 7500]
+        # objects = objects[objects["y"] > 30]
+        # objects = objects[objects["y"] < 5970]
 
         # update based on CCD distortion model the "true location"
         # of the fibers
-        xNudge, yNudge = updateCCDMeas(objects["x"], objects["y"])
+        if self.data_sub.shape[1] < 8000 and self.nudgeAdjust:
+            # ccd was trimmed
+            xNudge, yNudge = updateCCDMeas(objects["x"]+self.nudgeOffX, objects["y"], site=self.site)
+            xNudge = xNudge - self.nudgeOffX
+        else:
+            xNudge, yNudge = updateCCDMeas(objects["x"], objects["y"], site=self.site)
+
 
         # don't fit anything with an absolute correction > 0.75 pixels
         # rejectInds = (numpy.abs(xNudge) > 0.75) | (numpy.abs(yNudge) > 0.75)
 
 
         # create mask and re-extract using winpos algorithm
-        maskArr = numpy.ones(self.data_sub.shape, dtype=bool)
-        boxRad = numpy.floor(winposBoxSize/2)
-        boxSteps = numpy.arange(-boxRad, boxRad+1, dtype=int)
-
-        for ii in range(len(objects)):
-            _xm = objects["xcpeak"][ii]
-            _ym = objects["ycpeak"][ii]
-            for xstep in boxSteps:
-                for ystep in boxSteps:
-                    maskArr[_ym + ystep, _xm + xstep] = False
-
-        xNew, yNew, flags = sep.winpos(
-            self.data_sub,
-            objects["xcpeak"],
-            objects["ycpeak"],
-            sig=winposSigma,
-            mask=maskArr
-        )
+        # maskArr = numpy.ones(self.data_sub.shape, dtype=bool)
+        # boxRad = numpy.floor(winposBoxSize/2)
+        # boxSteps = numpy.arange(-boxRad, boxRad+1, dtype=int)
+
+        # for ii in range(len(objects)):
+        #     _xm = objects["xcpeak"][ii]
+        #     _ym = objects["ycpeak"][ii]
+        #     for xstep in boxSteps:
+        #         for ystep in boxSteps:
+        #             maskArr[_ym + ystep, _xm + xstep] = False
+
+        # xNew, yNew, flags = sep.winpos(
+        #     self.data_sub,
+        #     objects["xcpeak"],
+        #     objects["ycpeak"],
+        #     sig=winposSigma,
+        #     mask=maskArr
+        # )
+
+
+        # off = 1022  # trim the LR edges refinexy needs square
+        # im = self.data_sub[:, off:-off].copy()
+
+        # xSimple, ySimple = refinexy(
+        #     im, xNew-off, yNew,
+        #     psf_sigma=self.simpleSigma, cutout=self.simpleBoxSize
+        # )
 
 
-        off = 1022  # trim the LR edges refinexy needs square
-        im = self.data_sub[:, off:-off].copy()
-
-        xSimple, ySimple = refinexy(
-            im, xNew-off, yNew,
-            psf_sigma=self.simpleSigma, cutout=self.simpleBoxSize
-        )
-
-
-        xSimple = xSimple + off
+        # xSimple = xSimple + off
 
         objects = pandas.DataFrame(objects)
 
-        objects["xWinpos"] = xNew
-        objects["yWinpos"] = yNew
-        objects["xSimple"] = xSimple
-        objects["ySimple"] = ySimple
+        # objects["xWinpos"] = xNew
+        # objects["yWinpos"] = yNew
+        # objects["xSimple"] = xSimple
+        # objects["ySimple"] = ySimple
         objects["xNudge"] = xNudge
         objects["yNudge"] = yNudge
 
         # rotate raw centroids by rotator angle
         _centTypes = [
             ["x", "y"],
-            ["xWinpos", "yWinpos"],
-            ["xSimple", "ySimple"],
+            # ["xWinpos", "yWinpos"],
+            # ["xSimple", "ySimple"],
             ["xNudge", "yNudge"]
         ]
 
         for _centType in _centTypes:
             xy = objects[_centType].to_numpy()
             xyRot = (self.rotMat @ (xy - ccdRotCenXY).T).T + ccdRotCenXY
             objects[_centType[0]+"Rot"] = xyRot[:,0]
             objects[_centType[1]+"Rot"] = xyRot[:,1]
 
-        # xy = objects[["x", "y"]].to_numpy()
-        # xyRot = (self.rotMat @ (xy - ccdRotCenXY).T).T + ccdRotCenXY
-
-        # objects["xRot"] = xyRot[:, 0]
-        # objects["yRot"] = xyRot[:, 1]
-
-        # # rotate winpos centroids by rotator angle
-        # xy = objects[["xWinpos", "yWinpos"]].to_numpy()
-        # xyRot = (self.rotMat @ (xy - ccdRotCenXY).T).T + ccdRotCenXY
-
-        # objects["xWinposRot"] = xyRot[:, 0]
-        # objects["yWinposRot"] = xyRot[:, 1]
-
-        # # rotate simple centroids by rotator angle
-        # xy = objects[["xSimple", "ySimple"]].to_numpy()
-        # xyRot = (self.rotMat @ (xy - ccdRotCenXY).T).T + ccdRotCenXY
-
-        # objects["xSimpleRot"] = xyRot[:, 0]
-        # objects["ySimpleRot"] = xyRot[:, 1]
-
-        # # rotate nudged centroids by rotator angle
-        # xy = objects[["xNudge", "yNudge"]].to_numpy()
-        # xyRot = (self.rotMat @ (xy - ccdRotCenXY).T).T + ccdRotCenXY
-
-        # objects["xNudgeRot"] = xyRot[:, 0]
-        # objects["yNudgeRot"] = xyRot[:, 1]
-
-
         objects["centroidID"] = list(range(len(objects)))
 
         self.centroids = objects
         self.nCentroids = len(objects)
 
         return self.centroids
 
@@ -1168,15 +1165,15 @@
         """
         Calculate xy wok positions of centroids.  Store results
         in self.fullTable (a pandas.DataFrame)
 
         Parameters
         -----------
         centType : str
-            one of "zbplus2", zbplus", "zbminus", sep", "winpos", "nudge" or "simple", default is "nudge"
+            one of "zbplus2", zbplus", "zbminus", "sep", or "nudge", default is "nudge"
         maxRoughDist : float
             Max distance for an outer fiducial match (rough mm)
         maxMidDist : float
             Max distance for all fiducial matches after similarity
             transform based on outer fiducials (~ mm)
         maxFinalDist : float
             Max distance for positioner and fiducial matches
@@ -1190,32 +1187,32 @@
         self.maxRoughDist = maxRoughDist
         self.maxMidDist = maxMidDist
         self.maxFinalDist = maxFinalDist
         self.newInvKin = newInvKin
 
         if self.centroids is None:
             raise CoordIOError("Must run extractCentroids before fit")
-        if self.centType not in ["zbplus2", "zbplus", "zbminus", "sep", "winpos", "nudge", "simple"]:
+        if self.centType not in ["zbplus2", "zbplus", "zbminus", "sep", "nudge"]:
             raise CoordIOError("unknown centType: %s"%str(self.centType))
 
         xyMetFiber = self._fullTable[
             ["xWokReportMetrology", "yWokReportMetrology"]
         ].to_numpy()
 
         xyWokFIF = self.fiducialCoords[["xWok", "yWok"]].to_numpy()
 
-        if self.centType == "winpos":
-            xyCCDRot = self.centroids[["xWinposRot", "yWinposRot"]].to_numpy()
-            xyCCD = self.centroids[["xWinpos", "yWinpos"]].to_numpy()
-        elif self.centType == "sep":
+        # if self.centType == "winpos":
+        #     xyCCDRot = self.centroids[["xWinposRot", "yWinposRot"]].to_numpy()
+        #     xyCCD = self.centroids[["xWinpos", "yWinpos"]].to_numpy()
+        if self.centType == "sep":
             xyCCDRot = self.centroids[["xRot", "yRot"]].to_numpy()
             xyCCD = self.centroids[["x", "y"]].to_numpy()
-        elif self.centType == "simple":
-            xyCCDRot = self.centroids[["xSimpleRot", "ySimpleRot"]].to_numpy()
-            xyCCD = self.centroids[["xSimple", "ySimple"]].to_numpy()
+        # elif self.centType == "simple":
+        #     xyCCDRot = self.centroids[["xSimpleRot", "ySimpleRot"]].to_numpy()
+        #     xyCCD = self.centroids[["xSimple", "ySimple"]].to_numpy()
         elif self.centType in ["nudge", "zbplus", "zbminus", "zbplus2"]:
             xyCCDRot = self.centroids[["xNudgeRot", "yNudgeRot"]].to_numpy()
             xyCCD = self.centroids[["xNudge", "yNudge"]].to_numpy()
         else:
             raise CoordIOError("unknown centroid type passed to fit")
 
         # first do a rough transform
@@ -1456,36 +1453,37 @@
         )
 
         if self.centType in ["nudge", "zbplus", "zbminus", "zbplus2"]:
             self.positionerTableMeas["xFVC"] = self.positionerTableMeas["xNudge"]
             self.positionerTableMeas["yFVC"] = self.positionerTableMeas["yNudge"]
             self.fiducialCoordsMeas["xFVC"] = self.fiducialCoordsMeas["xNudge"]
             self.fiducialCoordsMeas["yFVC"] = self.fiducialCoordsMeas["yNudge"]
-        elif self.centType == "winpos":
-            self.positionerTableMeas["xFVC"] = self.positionerTableMeas["xWinpos"]
-            self.positionerTableMeas["yFVC"] = self.positionerTableMeas["yWinpos"]
-            self.fiducialCoordsMeas["xFVC"] = self.fiducialCoordsMeas["xWinpos"]
-            self.fiducialCoordsMeas["yFVC"] = self.fiducialCoordsMeas["yWinpos"]
-        elif self.centType == "simple":
-            self.positionerTableMeas["xFVC"] = self.positionerTableMeas["xSimple"]
-            self.positionerTableMeas["yFVC"] = self.positionerTableMeas["ySimple"]
-            self.fiducialCoordsMeas["xFVC"] = self.fiducialCoordsMeas["xSimple"]
-            self.fiducialCoordsMeas["yFVC"] = self.fiducialCoordsMeas["ySimple"]
+        # elif self.centType == "winpos":
+        #     self.positionerTableMeas["xFVC"] = self.positionerTableMeas["xWinpos"]
+        #     self.positionerTableMeas["yFVC"] = self.positionerTableMeas["yWinpos"]
+        #     self.fiducialCoordsMeas["xFVC"] = self.fiducialCoordsMeas["xWinpos"]
+        #     self.fiducialCoordsMeas["yFVC"] = self.fiducialCoordsMeas["yWinpos"]
+        # elif self.centType == "simple":
+        #     self.positionerTableMeas["xFVC"] = self.positionerTableMeas["xSimple"]
+        #     self.positionerTableMeas["yFVC"] = self.positionerTableMeas["ySimple"]
+        #     self.fiducialCoordsMeas["xFVC"] = self.fiducialCoordsMeas["xSimple"]
+        #     self.fiducialCoordsMeas["yFVC"] = self.fiducialCoordsMeas["ySimple"]
         elif self.centType == "sep":
             self.positionerTableMeas["xFVC"] = self.positionerTableMeas["x"]
             self.positionerTableMeas["yFVC"] = self.positionerTableMeas["y"]
             self.fiducialCoordsMeas["xFVC"] = self.fiducialCoordsMeas["x"]
             self.fiducialCoordsMeas["yFVC"] = self.fiducialCoordsMeas["y"]
 
 
 class FVCTransformLCO(FVCTransformAPO):
-    polids = [0, 1, 2, 3, 4, 5, 6, 9, 20, 28, 29]  # Zhao-Burge basis defaults, best so far
+    # polids = [0, 1, 2, 3, 4, 5, 6, 9, 20, 28, 29]  # Zhao-Burge basis defaults, best so far
 
-    # polids = numpy.arange(33)
+    polids = numpy.arange(33)
     zbCoeffs = None
     zbCoeffsFieldCenter = None
     telRotAngRef = 89 # rotator angle that puts xyWok aligned with xyCCD on FVC image
     rotAngDir = -1
     centType = "nudge"
     telescopePlateScale = 0.092 # mm/arcsec
-
+    nudgeOffX = 1250 # fix nudge model after FVC resize
+    site = "LCO"
```

### Comparing `sdss-coordio-1.6.1/src/coordio/utils.py` & `sdss-coordio-1.7.0/src/coordio/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,15 +188,19 @@
     # propogate propermotions, etc
     icrs = icrs.to_epoch(obsTime, site=site)
     if focalScale is None:
         focalScale = defaults.SITE_TO_SCALE[obsSite]
 
     obs = Observed(icrs, site=site, wavelength=wavelength)
     field = Field(obs, field_center=obsCen)
-    focal = FocalPlane(field, wavelength=wavelength, site=site, fpScale=focalScale)
+    focal = FocalPlane(field,
+                       wavelength=wavelength,
+                       site=site,
+                       fpScale=focalScale,
+                       use_closest_wavelength=True)
     wok = Wok(focal, site=site, obsAngle=obsAngle)
 
     output = (
         wok[:, 0], wok[:, 1], focal.field_warn,
         float(obsCen.ha), float(obsCen.pa)
     )
     return output
@@ -304,15 +308,19 @@
     xyzWok[:, 0] = xWok
     xyzWok[:, 1] = yWok
     xyzWok[:, 2] = zWok
 
     wok = Wok(xyzWok, site=site, obsAngle=obsAngle)
     if focalScale is None:
         focalScale = defaults.SITE_TO_SCALE[obsSite]
-    focal = FocalPlane(wok, wavelength=wavelength, site=site, fpScale=focalScale)
+    focal = FocalPlane(wok,
+                       wavelength=wavelength,
+                       site=site,
+                       fpScale=focalScale,
+                       use_closest_wavelength=True)
     field = Field(focal, field_center=obsCen)
     obs = Observed(field, site=site, wavelength=wavelength)
     icrs = ICRS(obs, epoch=obsTime)
 
     return icrs[:, 0], icrs[:, 1], field.field_warn
 
 
@@ -721,23 +729,21 @@
         offset_flag = 0
         if mag <= mag_limit and mag not in cases and can_offset and mag > offset_bright_limit:
             # linear portion in the wings
             r_wings = ((mag_limit + safety_factor) - mag - 8.2) / 0.05
             # linear portion in transition area
             r_trans = ((mag_limit + safety_factor) - mag - 4.5) / 0.25
             # core area
-            # do dark core for apogee or dark
-            if lunation == 'bright' or waveName == 'Apogee':
-                if beta != fmagloss.beta_interp2d or FWHM not in fmagloss.FWHM_interp2d:
-                    fmagloss = Moffat2dInterp(beta=beta, FWHM=[FWHM])
-                    r_core = fmagloss((mag_limit + safety_factor) - mag, FWHM)
-                else:
-                    r_core = fmagloss((mag_limit + safety_factor) - mag, FWHM)
+            if beta != fmagloss.beta_interp2d or FWHM not in fmagloss.FWHM_interp2d:
+                fmagloss = Moffat2dInterp(beta=beta, FWHM=[FWHM])
+                r_core = fmagloss((mag_limit + safety_factor) - mag, FWHM)
             else:
-                r_core = 1.5 * ((mag_limit + safety_factor) - mag) ** 0.8
+                r_core = fmagloss((mag_limit + safety_factor) - mag, FWHM)
+            # tom's old conservative core function
+            # r_core = 1.5 * ((mag_limit + safety_factor) - mag) ** 0.8
             # exlusion radius is the max of each section
             r = numpy.nanmax([r_wings, r_trans, r_core])
         else:
             r = 0.
             if mag > mag_limit:
                 offset_flag += 1
             elif mag in cases:
@@ -769,40 +775,37 @@
         offset_flag[~can_offset] += 16
         offset_flag[(mag <= offset_bright_limit) & ~((numpy.isin(mag, cases)) | (numpy.isnan(mag)))] += 32
         # linear portion in the wings
         r_wings[mag_valid] = ((mag_limit + safety_factor) - mag[mag_valid] - 8.2) / 0.05
         # linear portion in transition area
         r_trans[mag_valid] = ((mag_limit + safety_factor) - mag[mag_valid] - 4.5) / 0.25
         # core area
-        # core area
-        # do dark core for apogee or dark
-        if lunation == 'bright' or waveName == 'Apogee':
-            if beta != fmagloss.beta_interp2d or FWHM not in fmagloss.FWHM_interp2d:
-                fmagloss = Moffat2dInterp(beta=beta, FWHM=[FWHM])
-                r_core[mag_valid] = fmagloss((mag_limit + safety_factor) - mag[mag_valid],
-                                             FWHM)
-            else:
-                r_core[mag_valid] = fmagloss((mag_limit + safety_factor) - mag[mag_valid],
-                                             FWHM)
+        if beta != fmagloss.beta_interp2d or FWHM not in fmagloss.FWHM_interp2d:
+            fmagloss = Moffat2dInterp(beta=beta, FWHM=[FWHM])
+            r_core[mag_valid] = fmagloss((mag_limit + safety_factor) - mag[mag_valid],
+                                         FWHM)
         else:
-            r_core[mag_valid] = 1.5 * ((mag_limit + safety_factor) - mag[mag_valid]) ** 0.8
+            r_core[mag_valid] = fmagloss((mag_limit + safety_factor) - mag[mag_valid],
+                                         FWHM)
+        # tom's old conservative core function
+        # r_core[mag_valid] = 1.5 * ((mag_limit + safety_factor) - mag[mag_valid]) ** 0.8
         # exlusion radius is the max of each section
         r = numpy.nanmax(numpy.column_stack((r_wings,
                                              r_trans,
                                              r_core)),
                          axis=1)
         if skybrightness is not None and offset_min_skybrightness is not None:
             if skybrightness <= offset_min_skybrightness:
                 offset_flag[:] += 8
                 r[:] = 0.
     return r, offset_flag
 
 
 def object_offset(mag, mag_limits, lunation, waveName, fmagloss=None,
-                  safety_factor=0.1, beta=5, FWHM=1.7, skybrightness=None,
+                  safety_factor=0.5, beta=5, FWHM=1.7, skybrightness=None,
                   offset_min_skybrightness=None, can_offset=None):
     """
     Returns the offset needed for object with mag to be
     observed at mag_limit. Currently assumption is all offsets
     are set in positive RA direction.
 
     Parameters
```

### Comparing `sdss-coordio-1.6.1/src/coordio/wok.py` & `sdss-coordio-1.7.0/src/coordio/wok.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/zernike.py` & `sdss-coordio-1.7.0/src/coordio/zernike.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/coordio/zhaoburge.py` & `sdss-coordio-1.7.0/src/coordio/zhaoburge.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.6.1/src/sdss_coordio.egg-info/PKG-INFO` & `sdss-coordio-1.7.0/src/sdss_coordio.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-coordio
-Version: 1.6.1
+Version: 1.7.0
 Summary: Coordinate conversion for SDSS-V
 Home-page: https://github.com/sdss/coordio
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/coordio
 Project-URL: Documentation, https://sdss-coordio.readthedocs.org
```

### Comparing `sdss-coordio-1.6.1/src/sdss_coordio.egg-info/SOURCES.txt` & `sdss-coordio-1.7.0/src/sdss_coordio.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -294,8 +294,26 @@
 src/coordio/etc/coordio.yml
 src/coordio/include/coordio.h
 src/sdss_coordio.egg-info/PKG-INFO
 src/sdss_coordio.egg-info/SOURCES.txt
 src/sdss_coordio.egg-info/dependency_links.txt
 src/sdss_coordio.egg-info/not-zip-safe
 src/sdss_coordio.egg-info/requires.txt
-src/sdss_coordio.egg-info/top_level.txt
+src/sdss_coordio.egg-info/top_level.txt
+tests/test_conv.py
+tests/test_coordinate.py
+tests/test_fpScale.py
+tests/test_guide.py
+tests/test_iers.py
+tests/test_libcoordio.py
+tests/test_offset.py
+tests/test_plPlug.py
+tests/test_positioner.py
+tests/test_site.py
+tests/test_sky.py
+tests/test_sofa.py
+tests/test_tangent.py
+tests/test_tangentToPositioner2.py
+tests/test_telescope.py
+tests/test_time.py
+tests/test_wok.py
+tests/test_zern.py
```

