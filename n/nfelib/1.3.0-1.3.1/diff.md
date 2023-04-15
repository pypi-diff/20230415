# Comparing `tmp/nfelib-1.3.0.zip` & `tmp/nfelib-1.3.1.zip`

## zipinfo {}

```diff
@@ -1,125 +1,121 @@
-Zip file size: 779569 bytes, number of entries: 123
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/schemas/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/nfelib.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/nfelib/
--rw-rw-r--  2.0 unx    11761 b- defN 22-Jul-31 16:47 nfelib-1.3.0/README.md
--rw-rw-r--  2.0 unx    12963 b- defN 22-Jul-31 16:55 nfelib-1.3.0/PKG-INFO
--rw-rw-r--  2.0 unx     1399 b- defN 22-Jul-31 16:55 nfelib-1.3.0/setup.cfg
--rw-rw-r--  2.0 unx       64 b- defN 22-Jul-31 10:33 nfelib-1.3.0/MANIFEST.in
--rw-rw-r--  2.0 unx       38 b- defN 22-Jul-31 10:33 nfelib-1.3.0/setup.py
--rw-rw-r--  2.0 unx     1074 b- defN 22-Jul-31 10:33 nfelib-1.3.0/MIT-LICENSE
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/schemas/nfe/
--rw-rw-r--  2.0 unx      107 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/README.txt
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/schemas/nfe/v4_00/
--rw-rw-r--  2.0 unx      581 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/procEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx    15624 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/leiauteConfRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx      589 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/retEnvEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     1755 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/e210240_v1.00.xsd
--rw-rw-r--  2.0 unx      569 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/retEnvEvento_v1.00.xsd
--rw-rw-r--  2.0 unx      612 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/envConfRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx      598 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/procConfRecebtoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      630 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/envCCe_v1.00.xsd
--rw-rw-r--  2.0 unx      579 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/procInutNFe_v4.00.xsd
--rw-rw-r--  2.0 unx    21488 b- defN 21-Jun-28 11:21 nfelib-1.3.0/schemas/nfe/v4_00/tiposBasico_v4.00.xsd
--rw-rw-r--  2.0 unx      572 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/eventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx     4933 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/resNFe_v1.01.xsd
--rw-rw-r--  2.0 unx      568 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/consSitNFe_v4.00.xsd
--rw-rw-r--  2.0 unx    14282 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/leiauteEvento_v1.00.xsd
--rw-rw-r--  2.0 unx     3340 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/e110110_v1.00.xsd
--rw-rw-r--  2.0 unx      628 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/retConsReciNFe_v4.00.xsd
--rw-rw-r--  2.0 unx     7801 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/leiauteInutNFe_v4.00.xsd
--rw-rw-r--  2.0 unx   310082 b- defN 22-Jul-31 16:47 nfelib-1.3.0/schemas/nfe/v4_00/leiauteNFe_v4.00.xsd
--rw-rw-r--  2.0 unx     4407 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/retDistDFeInt_v1.01.xsd
--rw-rw-r--  2.0 unx     1253 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/e210210_v1.00.xsd
--rw-rw-r--  2.0 unx     1767 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/e210220_v1.00.xsd
--rw-rw-r--  2.0 unx     3902 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/leiauteConsStatServ_v4.00.xsd
--rw-rw-r--  2.0 unx      522 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/nfe_v4.00.xsd
--rw-rw-r--  2.0 unx      600 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/enviNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      595 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/consStatServ_v4.00.xsd
--rw-rw-r--  2.0 unx      602 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/retConsSitNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      606 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/retConsCad_v2.00.xsd
--rw-rw-r--  2.0 unx    13952 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/leiauteEventoCancNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      586 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/confRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx    29554 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/tiposBasico_v1.03.xsd
--rw-rw-r--  2.0 unx     8230 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/tiposDistDFe_v1.01.xsd
--rw-rw-r--  2.0 unx      627 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/procCCeNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      522 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/procNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      604 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/retConsStatServ_v4.00.xsd
--rw-rw-r--  2.0 unx      623 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/retInutNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      627 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/retEnvCCe_v1.00.xsd
--rw-rw-r--  2.0 unx      657 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/CCe_v1.00.xsd
--rw-rw-r--  2.0 unx      607 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/retEnvConfRecebto_v1.00.xsd
--rw-rw-r--  2.0 unx      600 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/consCad_v2.00.xsd
--rw-rw-r--  2.0 unx      572 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/procEventoNFe_v1.00.xsd
--rw-rw-r--  2.0 unx      610 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/consReciNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      617 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/retEnviNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      606 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/inutNFe_v4.00.xsd
--rw-rw-r--  2.0 unx     4034 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/distDFeInt_v1.01.xsd
--rw-rw-r--  2.0 unx     3747 b- defN 22-Jul-31 16:47 nfelib-1.3.0/schemas/nfe/v4_00/xmldsig-core-schema_v1.01.xsd
--rw-rw-r--  2.0 unx     4495 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/resEvento_v1.01.xsd
--rw-rw-r--  2.0 unx    15469 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/leiauteConsultaCadastro_v2.00.xsd
--rw-rw-r--  2.0 unx    17276 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/leiauteCCe_v1.00.xsd
--rw-rw-r--  2.0 unx     1269 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/e210200_v1.00.xsd
--rw-rw-r--  2.0 unx    20047 b- defN 21-Jun-01 11:38 nfelib-1.3.0/schemas/nfe/v4_00/leiauteConsSitNFe_v4.00.xsd
--rw-rw-r--  2.0 unx      575 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/envEvento_v1.00.xsd
--rw-rw-r--  2.0 unx     1770 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/e110111_v1.00.xsd
--rw-rw-r--  2.0 unx      595 b- defN 22-Jul-31 10:33 nfelib-1.3.0/schemas/nfe/v4_00/envEventoCancNFe_v1.00.xsd
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/tests/nfe/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/tests/cce/
--rw-rw-r--  2.0 unx        0 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/__init__.py
--rw-rw-r--  2.0 unx    11544 b- defN 22-Jul-31 16:51 nfelib-1.3.0/tests/input.xml
--rw-rw-r--  2.0 unx     1230 b- defN 22-Jul-31 16:51 nfelib-1.3.0/tests/output.xml
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/tests/nfe/v4_00/
--rw-rw-r--  2.0 unx       26 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/__init__.py
--rw-rw-r--  2.0 unx     4567 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/test_nfelib.py
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/tests/nfe/v4_00/leiauteInutNFe/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/
--rw-rw-r--  2.0 unx      484 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
--rw-rw-r--  2.0 unx    32177 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
--rw-rw-r--  2.0 unx     9767 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
--rw-rw-r--  2.0 unx    11802 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
--rw-rw-r--  2.0 unx    10848 b- defN 22-Jul-31 10:52 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
--rw-rw-r--  2.0 unx    68825 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
--rw-rw-r--  2.0 unx     9301 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
--rw-rw-r--  2.0 unx     9218 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
--rw-rw-r--  2.0 unx    14549 b- defN 22-Jul-31 10:52 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
--rw-rw-r--  2.0 unx    46216 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
--rw-rw-r--  2.0 unx    10647 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
--rw-rw-r--  2.0 unx    46079 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
--rw-rw-r--  2.0 unx    14538 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
--rw-rw-r--  2.0 unx    37663 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
--rw-rw-r--  2.0 unx    19259 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
--rw-rw-r--  2.0 unx     5471 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
--rw-rw-r--  2.0 unx    15749 b- defN 22-Jul-31 10:44 nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/tests/cce/v1_00/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/tests/cce/v1_00/leiauteCCe/
--rw-rw-r--  2.0 unx     1128 b- defN 22-Jul-31 10:33 nfelib-1.3.0/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
--rw-rw-r--  2.0 unx       46 b- defN 22-Jul-31 16:55 nfelib-1.3.0/nfelib.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 22-Jul-31 16:55 nfelib-1.3.0/nfelib.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx    12963 b- defN 22-Jul-31 16:55 nfelib-1.3.0/nfelib.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx     4472 b- defN 22-Jul-31 16:55 nfelib-1.3.0/nfelib.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx       21 b- defN 22-Jul-31 16:55 nfelib-1.3.0/nfelib.egg-info/top_level.txt
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/nfelib/docs/
-drwxrwxr-x  2.0 unx        0 b- stor 22-Jul-31 16:55 nfelib-1.3.0/nfelib/v4_00/
--rw-rw-r--  2.0 unx        0 b- defN 22-Jul-31 16:49 nfelib-1.3.0/nfelib/__init__.py
--rw-rw-r--  2.0 unx     2860 b- defN 22-Jul-31 10:33 nfelib-1.3.0/nfelib/leiauteNFe_sub.py
--rw-rw-r--  2.0 unx      467 b- defN 22-Jul-31 16:53 nfelib-1.3.0/nfelib/docs/module_contents.txt
--rw-rw-r--  2.0 unx       51 b- defN 22-Jul-31 16:49 nfelib-1.3.0/nfelib/docs/conf.py
--rw-rw-r--  2.0 unx  1859544 b- defN 22-Jul-31 16:53 nfelib-1.3.0/nfelib/v4_00/retConsReciNFe.py
--rw-rw-r--  2.0 unx    88685 b- defN 22-Jul-31 16:53 nfelib-1.3.0/nfelib/v4_00/retConsStatServ.py
--rw-rw-r--  2.0 unx   231041 b- defN 22-Jul-31 10:43 nfelib-1.3.0/nfelib/v4_00/retEnvEvento.py
--rw-rw-r--  2.0 unx        0 b- defN 22-Jul-31 16:49 nfelib-1.3.0/nfelib/v4_00/__init__.py
--rw-rw-r--  2.0 unx    80047 b- defN 22-Jul-31 10:43 nfelib-1.3.0/nfelib/v4_00/distDFeInt.py
--rw-rw-r--  2.0 unx   237200 b- defN 22-Jul-31 10:43 nfelib-1.3.0/nfelib/v4_00/retEnvEventoCancNFe.py
--rw-rw-r--  2.0 unx  1859480 b- defN 22-Jul-31 16:53 nfelib-1.3.0/nfelib/v4_00/retEnviNFe.py
--rw-rw-r--  2.0 unx  1859480 b- defN 22-Jul-31 16:49 nfelib-1.3.0/nfelib/v4_00/retEnviNFe.py.orig
--rw-rw-r--  2.0 unx   159793 b- defN 22-Jul-31 10:43 nfelib-1.3.0/nfelib/v4_00/retConsCad.py
--rw-rw-r--  2.0 unx    79013 b- defN 22-Jul-31 10:43 nfelib-1.3.0/nfelib/v4_00/retDistDFeInt.py
--rw-rw-r--  2.0 unx   289846 b- defN 22-Jul-31 16:53 nfelib-1.3.0/nfelib/v4_00/retConsSitNFe.py
--rw-rw-r--  2.0 unx   239970 b- defN 22-Jul-31 10:43 nfelib-1.3.0/nfelib/v4_00/retEnvCCe.py
--rw-rw-r--  2.0 unx   235328 b- defN 22-Jul-31 10:43 nfelib-1.3.0/nfelib/v4_00/retEnvConfRecebto.py
--rw-rw-r--  2.0 unx   188157 b- defN 22-Jul-31 16:53 nfelib-1.3.0/nfelib/v4_00/retInutNFe.py
--rw-rw-r--  2.0 unx     2863 b- defN 22-Jul-31 10:43 nfelib-1.3.0/nfelib/v4_00/leiauteNFe_sub.py
-123 files, 8368178 bytes uncompressed, 757793 bytes compressed:  90.9%
+Zip file size: 646757 bytes, number of entries: 119
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/schemas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/nfelib.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/nfelib/
+-rw-rw-r--  2.0 unx    11761 b- defN 23-Apr-14 22:53 nfelib-1.3.1/README.md
+-rw-rw-r--  2.0 unx    12963 b- defN 23-Apr-14 22:54 nfelib-1.3.1/PKG-INFO
+-rw-rw-r--  2.0 unx     1399 b- defN 23-Apr-14 22:54 nfelib-1.3.1/setup.cfg
+-rw-rw-r--  2.0 unx       64 b- defN 23-Apr-14 22:53 nfelib-1.3.1/MANIFEST.in
+-rw-rw-r--  2.0 unx       38 b- defN 23-Apr-14 22:53 nfelib-1.3.1/setup.py
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Apr-14 22:53 nfelib-1.3.1/MIT-LICENSE
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/schemas/nfe/
+-rw-rw-r--  2.0 unx      107 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/README.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/schemas/nfe/v4_00/
+-rw-rw-r--  2.0 unx      581 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/procEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx    15624 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/leiauteConfRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx      589 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retEnvEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1755 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/e210240_v1.00.xsd
+-rw-rw-r--  2.0 unx      569 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retEnvEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx      612 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/envConfRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx      598 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/procConfRecebtoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      630 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/envCCe_v1.00.xsd
+-rw-rw-r--  2.0 unx      579 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/procInutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx    21488 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/tiposBasico_v4.00.xsd
+-rw-rw-r--  2.0 unx      572 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/eventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx     4933 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/resNFe_v1.01.xsd
+-rw-rw-r--  2.0 unx      568 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/consSitNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx    14282 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/leiauteEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx     3340 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/e110110_v1.00.xsd
+-rw-rw-r--  2.0 unx      628 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retConsReciNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx     7801 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/leiauteInutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx   310082 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/leiauteNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx     4407 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retDistDFeInt_v1.01.xsd
+-rw-rw-r--  2.0 unx     1253 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/e210210_v1.00.xsd
+-rw-rw-r--  2.0 unx     1767 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/e210220_v1.00.xsd
+-rw-rw-r--  2.0 unx     3902 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/leiauteConsStatServ_v4.00.xsd
+-rw-rw-r--  2.0 unx      522 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/nfe_v4.00.xsd
+-rw-rw-r--  2.0 unx      600 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/enviNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      595 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/consStatServ_v4.00.xsd
+-rw-rw-r--  2.0 unx      602 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retConsSitNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      606 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retConsCad_v2.00.xsd
+-rw-rw-r--  2.0 unx    13952 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/leiauteEventoCancNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      586 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/confRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx    29554 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/tiposBasico_v1.03.xsd
+-rw-rw-r--  2.0 unx     8230 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/tiposDistDFe_v1.01.xsd
+-rw-rw-r--  2.0 unx      627 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/procCCeNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      522 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/procNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      604 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retConsStatServ_v4.00.xsd
+-rw-rw-r--  2.0 unx      623 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retInutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      627 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retEnvCCe_v1.00.xsd
+-rw-rw-r--  2.0 unx      657 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/CCe_v1.00.xsd
+-rw-rw-r--  2.0 unx      607 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retEnvConfRecebto_v1.00.xsd
+-rw-rw-r--  2.0 unx      600 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/consCad_v2.00.xsd
+-rw-rw-r--  2.0 unx      572 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/procEventoNFe_v1.00.xsd
+-rw-rw-r--  2.0 unx      610 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/consReciNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      617 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/retEnviNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      606 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/inutNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx     4034 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/distDFeInt_v1.01.xsd
+-rw-rw-r--  2.0 unx     3747 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/xmldsig-core-schema_v1.01.xsd
+-rw-rw-r--  2.0 unx     4495 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/resEvento_v1.01.xsd
+-rw-rw-r--  2.0 unx    15469 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/leiauteConsultaCadastro_v2.00.xsd
+-rw-rw-r--  2.0 unx    17276 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/leiauteCCe_v1.00.xsd
+-rw-rw-r--  2.0 unx     1269 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/e210200_v1.00.xsd
+-rw-rw-r--  2.0 unx    20047 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/leiauteConsSitNFe_v4.00.xsd
+-rw-rw-r--  2.0 unx      575 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/envEvento_v1.00.xsd
+-rw-rw-r--  2.0 unx     1770 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/e110111_v1.00.xsd
+-rw-rw-r--  2.0 unx      595 b- defN 23-Apr-14 22:53 nfelib-1.3.1/schemas/nfe/v4_00/envEventoCancNFe_v1.00.xsd
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/tests/nfe/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/tests/cce/
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/tests/nfe/v4_00/
+-rw-rw-r--  2.0 unx       26 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/__init__.py
+-rw-rw-r--  2.0 unx     4567 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/test_nfelib.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/tests/nfe/v4_00/leiauteInutNFe/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/
+-rw-rw-r--  2.0 unx      484 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
+-rw-rw-r--  2.0 unx    32177 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
+-rw-rw-r--  2.0 unx     9767 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
+-rw-rw-r--  2.0 unx    11802 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
+-rw-rw-r--  2.0 unx    10848 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
+-rw-rw-r--  2.0 unx    68825 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
+-rw-rw-r--  2.0 unx     9301 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
+-rw-rw-r--  2.0 unx     9218 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
+-rw-rw-r--  2.0 unx    14549 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
+-rw-rw-r--  2.0 unx    46216 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
+-rw-rw-r--  2.0 unx    10647 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
+-rw-rw-r--  2.0 unx    46079 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
+-rw-rw-r--  2.0 unx    14538 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
+-rw-rw-r--  2.0 unx    37663 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
+-rw-rw-r--  2.0 unx    19259 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
+-rw-rw-r--  2.0 unx     5471 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
+-rw-rw-r--  2.0 unx    15749 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/tests/cce/v1_00/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/tests/cce/v1_00/leiauteCCe/
+-rw-rw-r--  2.0 unx     1128 b- defN 23-Apr-14 22:53 nfelib-1.3.1/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
+-rw-rw-r--  2.0 unx       46 b- defN 23-Apr-14 22:54 nfelib-1.3.1/nfelib.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-14 22:54 nfelib-1.3.1/nfelib.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx    12963 b- defN 23-Apr-14 22:54 nfelib-1.3.1/nfelib.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     4382 b- defN 23-Apr-14 22:54 nfelib-1.3.1/nfelib.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx       21 b- defN 23-Apr-14 22:54 nfelib-1.3.1/nfelib.egg-info/top_level.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/nfelib/docs/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-14 22:54 nfelib-1.3.1/nfelib/v4_00/
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/__init__.py
+-rw-rw-r--  2.0 unx      467 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/docs/module_contents.txt
+-rw-rw-r--  2.0 unx       51 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/docs/conf.py
+-rw-rw-r--  2.0 unx  1859541 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retConsReciNFe.py
+-rw-rw-r--  2.0 unx    88685 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retConsStatServ.py
+-rw-rw-r--  2.0 unx   231041 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retEnvEvento.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/__init__.py
+-rw-rw-r--  2.0 unx    80047 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/distDFeInt.py
+-rw-rw-r--  2.0 unx   237200 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retEnvEventoCancNFe.py
+-rw-rw-r--  2.0 unx  1859480 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retEnviNFe.py
+-rw-rw-r--  2.0 unx   159793 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retConsCad.py
+-rw-rw-r--  2.0 unx    79013 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retDistDFeInt.py
+-rw-rw-r--  2.0 unx   289846 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retConsSitNFe.py
+-rw-rw-r--  2.0 unx   239970 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retEnvCCe.py
+-rw-rw-r--  2.0 unx   235328 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retEnvConfRecebto.py
+-rw-rw-r--  2.0 unx   188157 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/retInutNFe.py
+-rw-rw-r--  2.0 unx     2863 b- defN 23-Apr-14 22:53 nfelib-1.3.1/nfelib/v4_00/leiauteNFe_sub.py
+119 files, 6492971 bytes uncompressed, 625561 bytes compressed:  90.4%
```

## zipnote {}

```diff
@@ -1,370 +1,358 @@
-Filename: nfelib-1.3.0/
+Filename: nfelib-1.3.1/
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/
+Filename: nfelib-1.3.1/schemas/
 Comment: 
 
-Filename: nfelib-1.3.0/tests/
+Filename: nfelib-1.3.1/tests/
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib.egg-info/
+Filename: nfelib-1.3.1/nfelib.egg-info/
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/
+Filename: nfelib-1.3.1/nfelib/
 Comment: 
 
-Filename: nfelib-1.3.0/README.md
+Filename: nfelib-1.3.1/README.md
 Comment: 
 
-Filename: nfelib-1.3.0/PKG-INFO
+Filename: nfelib-1.3.1/PKG-INFO
 Comment: 
 
-Filename: nfelib-1.3.0/setup.cfg
+Filename: nfelib-1.3.1/setup.cfg
 Comment: 
 
-Filename: nfelib-1.3.0/MANIFEST.in
+Filename: nfelib-1.3.1/MANIFEST.in
 Comment: 
 
-Filename: nfelib-1.3.0/setup.py
+Filename: nfelib-1.3.1/setup.py
 Comment: 
 
-Filename: nfelib-1.3.0/MIT-LICENSE
+Filename: nfelib-1.3.1/MIT-LICENSE
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/
+Filename: nfelib-1.3.1/schemas/nfe/
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/README.txt
+Filename: nfelib-1.3.1/schemas/README.txt
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/procEventoCancNFe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/procEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/leiauteConfRecebto_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/leiauteConfRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retEnvEventoCancNFe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retEnvEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/e210240_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/e210240_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retEnvEvento_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retEnvEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/envConfRecebto_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/envConfRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/procConfRecebtoNFe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/procConfRecebtoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/envCCe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/envCCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/procInutNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/procInutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/tiposBasico_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/tiposBasico_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/eventoCancNFe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/eventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/resNFe_v1.01.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/resNFe_v1.01.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/consSitNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/consSitNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/leiauteEvento_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/leiauteEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/e110110_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/e110110_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retConsReciNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retConsReciNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/leiauteInutNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/leiauteInutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/leiauteNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/leiauteNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retDistDFeInt_v1.01.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retDistDFeInt_v1.01.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/e210210_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/e210210_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/e210220_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/e210220_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/leiauteConsStatServ_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/leiauteConsStatServ_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/nfe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/nfe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/enviNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/enviNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/consStatServ_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/consStatServ_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retConsSitNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retConsSitNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retConsCad_v2.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retConsCad_v2.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/leiauteEventoCancNFe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/leiauteEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/confRecebto_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/confRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/tiposBasico_v1.03.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/tiposBasico_v1.03.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/tiposDistDFe_v1.01.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/tiposDistDFe_v1.01.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/procCCeNFe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/procCCeNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/procNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/procNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retConsStatServ_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retConsStatServ_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retInutNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retInutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retEnvCCe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retEnvCCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/CCe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/CCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retEnvConfRecebto_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retEnvConfRecebto_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/consCad_v2.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/consCad_v2.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/procEventoNFe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/procEventoNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/consReciNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/consReciNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/retEnviNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/retEnviNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/inutNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/inutNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/distDFeInt_v1.01.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/distDFeInt_v1.01.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/xmldsig-core-schema_v1.01.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/xmldsig-core-schema_v1.01.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/resEvento_v1.01.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/resEvento_v1.01.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/leiauteConsultaCadastro_v2.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/leiauteConsultaCadastro_v2.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/leiauteCCe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/leiauteCCe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/e210200_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/e210200_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/leiauteConsSitNFe_v4.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/leiauteConsSitNFe_v4.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/envEvento_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/envEvento_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/e110111_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/e110111_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/schemas/nfe/v4_00/envEventoCancNFe_v1.00.xsd
+Filename: nfelib-1.3.1/schemas/nfe/v4_00/envEventoCancNFe_v1.00.xsd
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/
+Filename: nfelib-1.3.1/tests/nfe/
 Comment: 
 
-Filename: nfelib-1.3.0/tests/cce/
+Filename: nfelib-1.3.1/tests/cce/
 Comment: 
 
-Filename: nfelib-1.3.0/tests/__init__.py
+Filename: nfelib-1.3.1/tests/__init__.py
 Comment: 
 
-Filename: nfelib-1.3.0/tests/input.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/
 Comment: 
 
-Filename: nfelib-1.3.0/tests/output.xml
+Filename: nfelib-1.3.1/tests/nfe/__init__.py
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/
+Filename: nfelib-1.3.1/tests/nfe/test_nfelib.py
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/__init__.py
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteInutNFe/
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/test_nfelib.py
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteInutNFe/
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
+Filename: nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml
+Filename: nfelib-1.3.1/tests/cce/v1_00/
 Comment: 
 
-Filename: nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml
+Filename: nfelib-1.3.1/tests/cce/v1_00/leiauteCCe/
 Comment: 
 
-Filename: nfelib-1.3.0/tests/cce/v1_00/
+Filename: nfelib-1.3.1/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
 Comment: 
 
-Filename: nfelib-1.3.0/tests/cce/v1_00/leiauteCCe/
+Filename: nfelib-1.3.1/nfelib.egg-info/requires.txt
 Comment: 
 
-Filename: nfelib-1.3.0/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
+Filename: nfelib-1.3.1/nfelib.egg-info/dependency_links.txt
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib.egg-info/requires.txt
+Filename: nfelib-1.3.1/nfelib.egg-info/PKG-INFO
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib.egg-info/dependency_links.txt
+Filename: nfelib-1.3.1/nfelib.egg-info/SOURCES.txt
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib.egg-info/PKG-INFO
+Filename: nfelib-1.3.1/nfelib.egg-info/top_level.txt
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib.egg-info/SOURCES.txt
+Filename: nfelib-1.3.1/nfelib/docs/
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib.egg-info/top_level.txt
+Filename: nfelib-1.3.1/nfelib/v4_00/
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/docs/
+Filename: nfelib-1.3.1/nfelib/__init__.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/
+Filename: nfelib-1.3.1/nfelib/docs/module_contents.txt
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/__init__.py
+Filename: nfelib-1.3.1/nfelib/docs/conf.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/leiauteNFe_sub.py
+Filename: nfelib-1.3.1/nfelib/v4_00/retConsReciNFe.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/docs/module_contents.txt
+Filename: nfelib-1.3.1/nfelib/v4_00/retConsStatServ.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/docs/conf.py
+Filename: nfelib-1.3.1/nfelib/v4_00/retEnvEvento.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/retConsReciNFe.py
+Filename: nfelib-1.3.1/nfelib/v4_00/__init__.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/retConsStatServ.py
+Filename: nfelib-1.3.1/nfelib/v4_00/distDFeInt.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/retEnvEvento.py
+Filename: nfelib-1.3.1/nfelib/v4_00/retEnvEventoCancNFe.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/__init__.py
+Filename: nfelib-1.3.1/nfelib/v4_00/retEnviNFe.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/distDFeInt.py
+Filename: nfelib-1.3.1/nfelib/v4_00/retConsCad.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/retEnvEventoCancNFe.py
+Filename: nfelib-1.3.1/nfelib/v4_00/retDistDFeInt.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/retEnviNFe.py
+Filename: nfelib-1.3.1/nfelib/v4_00/retConsSitNFe.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/retEnviNFe.py.orig
+Filename: nfelib-1.3.1/nfelib/v4_00/retEnvCCe.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/retConsCad.py
+Filename: nfelib-1.3.1/nfelib/v4_00/retEnvConfRecebto.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/retDistDFeInt.py
+Filename: nfelib-1.3.1/nfelib/v4_00/retInutNFe.py
 Comment: 
 
-Filename: nfelib-1.3.0/nfelib/v4_00/retConsSitNFe.py
-Comment: 
-
-Filename: nfelib-1.3.0/nfelib/v4_00/retEnvCCe.py
-Comment: 
-
-Filename: nfelib-1.3.0/nfelib/v4_00/retEnvConfRecebto.py
-Comment: 
-
-Filename: nfelib-1.3.0/nfelib/v4_00/retInutNFe.py
-Comment: 
-
-Filename: nfelib-1.3.0/nfelib/v4_00/leiauteNFe_sub.py
+Filename: nfelib-1.3.1/nfelib/v4_00/leiauteNFe_sub.py
 Comment: 
 
 Zip file comment:
```

## Comparing `nfelib-1.3.0/README.md` & `nfelib-1.3.1/README.md`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/PKG-INFO` & `nfelib-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfelib
-Version: 1.3.0
+Version: 1.3.1
 Summary: nfelib: electronic invoicing library for Brazil
 Home-page: https://github.com/akretion/nfelib
 Author: Raphaël Valyi
 Author-email: "raphael.valyi@akretion.com.br"
 License: MIT
 Project-URL: Source, https://github.com/akretion/nfelib
 Keywords: e-invoicing,NFe,ERP,Odoo
```

## Comparing `nfelib-1.3.0/setup.cfg` & `nfelib-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nfelib
-version = 1.3.0
+version = 1.3.1
 description = nfelib: electronic invoicing library for Brazil
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/akretion/nfelib
 author = Raphaël Valyi
 author_email = "raphael.valyi@akretion.com.br"
 license = MIT
```

## Comparing `nfelib-1.3.0/MIT-LICENSE` & `nfelib-1.3.1/MIT-LICENSE`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/procEventoCancNFe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/procEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/leiauteConfRecebto_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/leiauteConfRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retEnvEventoCancNFe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retEnvEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/e210240_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/e210240_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retEnvEvento_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retEnvEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/envConfRecebto_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/envConfRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/procConfRecebtoNFe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/procConfRecebtoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/envCCe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/envCCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/procInutNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/procInutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/tiposBasico_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/tiposBasico_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/eventoCancNFe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/eventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/resNFe_v1.01.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/resNFe_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/consSitNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/consSitNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/leiauteEvento_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/leiauteEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/e110110_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/e110110_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retConsReciNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retConsReciNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/leiauteInutNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/leiauteInutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/leiauteNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/leiauteNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retDistDFeInt_v1.01.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retDistDFeInt_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/e210210_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/e210210_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/e210220_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/e210220_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/leiauteConsStatServ_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/leiauteConsStatServ_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/nfe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/nfe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/enviNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/enviNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/consStatServ_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/consStatServ_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retConsSitNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retConsSitNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retConsCad_v2.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retConsCad_v2.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/leiauteEventoCancNFe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/leiauteEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/confRecebto_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/confRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/tiposBasico_v1.03.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/tiposBasico_v1.03.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/tiposDistDFe_v1.01.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/tiposDistDFe_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/procCCeNFe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/procCCeNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/procNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/procNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retConsStatServ_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retConsStatServ_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retInutNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retInutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retEnvCCe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retEnvCCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/CCe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/CCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retEnvConfRecebto_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retEnvConfRecebto_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/consCad_v2.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/consCad_v2.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/procEventoNFe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/procEventoNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/consReciNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/consReciNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/retEnviNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/retEnviNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/inutNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/inutNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/distDFeInt_v1.01.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/distDFeInt_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/xmldsig-core-schema_v1.01.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/xmldsig-core-schema_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/resEvento_v1.01.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/resEvento_v1.01.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/leiauteConsultaCadastro_v2.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/leiauteConsultaCadastro_v2.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/leiauteCCe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/leiauteCCe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/e210200_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/e210200_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/leiauteConsSitNFe_v4.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/leiauteConsSitNFe_v4.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/envEvento_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/envEvento_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/e110111_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/e110111_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/schemas/nfe/v4_00/envEventoCancNFe_v1.00.xsd` & `nfelib-1.3.1/schemas/nfe/v4_00/envEventoCancNFe_v1.00.xsd`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/test_nfelib.py` & `nfelib-1.3.1/tests/nfe/test_nfelib.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476491552806942-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476121675985748-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/42220575277525000178550030000292481295366801-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476861118934859-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476781421693968-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/41170706117473000150550010000463202612756525-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/42210775277525000178550030000266631762885493-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474641681223493-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476711079516696-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474501597356342-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000476051695511860-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/NFe35200159594315000157550010000000012062777161.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/nfe/v4_00/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml` & `nfelib-1.3.1/tests/nfe/v4_00/leiauteNFe/42211275277525000178550030000276771368212013-procNFe.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml` & `nfelib-1.3.1/tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib.egg-info/PKG-INFO` & `nfelib-1.3.1/nfelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nfelib
-Version: 1.3.0
+Version: 1.3.1
 Summary: nfelib: electronic invoicing library for Brazil
 Home-page: https://github.com/akretion/nfelib
 Author: Raphaël Valyi
 Author-email: "raphael.valyi@akretion.com.br"
 License: MIT
 Project-URL: Source, https://github.com/akretion/nfelib
 Keywords: e-invoicing,NFe,ERP,Odoo
```

## Comparing `nfelib-1.3.0/nfelib.egg-info/SOURCES.txt` & `nfelib-1.3.1/nfelib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 MANIFEST.in
 MIT-LICENSE
 README.md
 setup.cfg
 setup.py
 nfelib/__init__.py
-nfelib/leiauteNFe_sub.py
 nfelib.egg-info/PKG-INFO
 nfelib.egg-info/SOURCES.txt
 nfelib.egg-info/dependency_links.txt
 nfelib.egg-info/requires.txt
 nfelib.egg-info/top_level.txt
 nfelib/docs/conf.py
 nfelib/docs/module_contents.txt
@@ -21,15 +20,14 @@
 nfelib/v4_00/retConsStatServ.py
 nfelib/v4_00/retDistDFeInt.py
 nfelib/v4_00/retEnvCCe.py
 nfelib/v4_00/retEnvConfRecebto.py
 nfelib/v4_00/retEnvEvento.py
 nfelib/v4_00/retEnvEventoCancNFe.py
 nfelib/v4_00/retEnviNFe.py
-nfelib/v4_00/retEnviNFe.py.orig
 nfelib/v4_00/retInutNFe.py
 schemas/README.txt
 schemas/nfe/v4_00/CCe_v1.00.xsd
 schemas/nfe/v4_00/confRecebto_v1.00.xsd
 schemas/nfe/v4_00/consCad_v2.00.xsd
 schemas/nfe/v4_00/consReciNFe_v4.00.xsd
 schemas/nfe/v4_00/consSitNFe_v4.00.xsd
@@ -78,16 +76,14 @@
 schemas/nfe/v4_00/retEnviNFe_v4.00.xsd
 schemas/nfe/v4_00/retInutNFe_v4.00.xsd
 schemas/nfe/v4_00/tiposBasico_v1.03.xsd
 schemas/nfe/v4_00/tiposBasico_v4.00.xsd
 schemas/nfe/v4_00/tiposDistDFe_v1.01.xsd
 schemas/nfe/v4_00/xmldsig-core-schema_v1.01.xsd
 tests/__init__.py
-tests/input.xml
-tests/output.xml
 tests/cce/v1_00/leiauteCCe/35180803102452000172550010000476051695511860-01-cce.xml
 tests/nfe/__init__.py
 tests/nfe/test_nfelib.py
 tests/nfe/v4_00/leiauteInutNFe/41080676472349000430550010000001041671821888-ped-inu.xml
 tests/nfe/v4_00/leiauteNFe/26180875335849000115550010000016871192213331-nfe.xml
 tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474281920007498-nfe.xml
 tests/nfe/v4_00/leiauteNFe/35180834128745000152550010000474491454651420-nfe.xml
```

## Comparing `nfelib-1.3.0/nfelib/leiauteNFe_sub.py` & `nfelib-1.3.1/nfelib/v4_00/leiauteNFe_sub.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     if not parser:
         # Use the lxml ElementTree compatible parser so that, e.g.,
         # we ignore comments.
         parser = etree_.ETCompatXMLParser()
 
     doc = etree_.parse(infile, parser=parser, **kwargs)
+
     if doc.getroot().tag == '{http://www.portalfiscal.inf.br/nfe}nfeProc':
         root = doc.getroot()[0]
     else:
         root = doc.getroot()
     # remove Signature element before XML comparison
     if not keep_signature:
         for child in root:
@@ -54,15 +55,15 @@
 
     if not parser.validate(doc):
         for e in parser.error_log:
             validation_messages.append(e.message)
     return validation_messages
 
 
-def parse(inFilename, parser=None, silence=False):
+def parse(inFilename, parser = None, silence=False):
     doc = parsexml_(inFilename, parser)
     rootNode = doc.getroot()
     rootTag, rootClass = supermod.get_root_tag(rootNode)
     if rootClass is None:
         rootClass = supermod.TNFe
     rootObj = rootClass.factory()
     rootObj.build(rootNode)
```

## Comparing `nfelib-1.3.0/nfelib/v4_00/retConsReciNFe.py` & `nfelib-1.3.1/nfelib/v4_00/retConsReciNFe.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 # Calls to the methods in these classes are generated by generateDS.py.
 # You can replace these methods by re-implementing the following class
 #   in a module named generatedssuper.py.
 
 try:
     from generatedssuper import GeneratedsSuper
 except ModulenotfoundExp_ as exp:
-    
+
     class GeneratedsSuper(object):
         __hash__ = object.__hash__
         tzoff_pattern = re_.compile(r'(\+|-)((0\d|1[0-3]):[0-5]\d|14:00)$')
         class _FixedOffsetTZ(datetime_.tzinfo):
             def __init__(self, offset, name):
                 self.__offset = datetime_.timedelta(minutes=offset)
                 self.__name = name
@@ -656,16 +656,16 @@
         def gds_get_node_lineno_(self):
             if (hasattr(self, "gds_elementtree_node_") and
                     self.gds_elementtree_node_ is not None):
                 return ' near line {}'.format(
                     self.gds_elementtree_node_.sourceline)
             else:
                 return ""
-    
-    
+
+
     def getSubclassFromModule_(module, class_):
         '''Get the subclass of a class from a specific module.'''
         name = class_.__name__ + 'Sub'
         if hasattr(module, name):
             return getattr(module, name)
         else:
             return None
@@ -31996,15 +31996,15 @@
         if self.nProt is not None:
             namespaceprefix_ = self.nProt_nsprefix_ + ':' if (UseCapturedNS_ and self.nProt_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%snProt>%s</%snProt>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.nProt), input_name='nProt')), namespaceprefix_ , eol_))
         if self.digVal is not None:
             namespaceprefix_ = self.digVal_nsprefix_ + ':' if (UseCapturedNS_ and self.digVal_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
-            outfile.write('<%sdigVal>%s</%sdigVal>%s' % (namespaceprefix_ , self.gds_format_base64(self.digVal, input_name='digVal'), namespaceprefix_ , eol_))
+            outfile.write('<%sdigVal>%s</%sdigVal>%s' % (namespaceprefix_ , self.gds_format_base64(self.digVal, input_name='digVal').decode(), namespaceprefix_ , eol_))
         if self.cStat is not None:
             namespaceprefix_ = self.cStat_nsprefix_ + ':' if (UseCapturedNS_ and self.cStat_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%scStat>%s</%scStat>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.cStat), input_name='cStat')), namespaceprefix_ , eol_))
         if self.xMotivo is not None:
             namespaceprefix_ = self.xMotivo_nsprefix_ + ':' if (UseCapturedNS_ and self.xMotivo_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
```

## Comparing `nfelib-1.3.0/nfelib/v4_00/retConsStatServ.py` & `nfelib-1.3.1/nfelib/v4_00/retConsStatServ.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib/v4_00/retEnvEvento.py` & `nfelib-1.3.1/nfelib/v4_00/retEnvEvento.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib/v4_00/distDFeInt.py` & `nfelib-1.3.1/nfelib/v4_00/distDFeInt.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib/v4_00/retEnvEventoCancNFe.py` & `nfelib-1.3.1/nfelib/v4_00/retEnvEventoCancNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib/v4_00/retEnviNFe.py` & `nfelib-1.3.1/nfelib/v4_00/retEnviNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib/v4_00/retConsCad.py` & `nfelib-1.3.1/nfelib/v4_00/retConsCad.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib/v4_00/retDistDFeInt.py` & `nfelib-1.3.1/nfelib/v4_00/retDistDFeInt.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib/v4_00/retConsSitNFe.py` & `nfelib-1.3.1/nfelib/v4_00/retConsSitNFe.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib/v4_00/retEnvCCe.py` & `nfelib-1.3.1/nfelib/v4_00/retEnvCCe.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib/v4_00/retEnvConfRecebto.py` & `nfelib-1.3.1/nfelib/v4_00/retEnvConfRecebto.py`

 * *Files identical despite different names*

## Comparing `nfelib-1.3.0/nfelib/v4_00/retInutNFe.py` & `nfelib-1.3.1/nfelib/v4_00/retInutNFe.py`

 * *Files identical despite different names*

