# Comparing `tmp/streamlit-text-annotator-0.1.3.tar.gz` & `tmp/streamlit-text-annotator-0.1.4.tar.gz`

```diff
@@ -1,219 +1,220 @@
-00000000: 1f8b 0808 7a95 3a64 02ff 7374 7265 616d  ....z.:d..stream
+00000000: 1f8b 0808 dc96 3a64 02ff 7374 7265 616d  ......:d..stream
 00000010: 6c69 742d 7465 7874 2d61 6e6e 6f74 6174  lit-text-annotat
-00000020: 6f72 2d30 2e31 2e33 2e74 6172 00ed 5d5b  or-0.1.3.tar..][
-00000030: 6fdb b812 ee33 7fc5 407d d8e4 c056 e47b  o....3..@}...V.{
-00000040: 6aac 8b75 13a7 31d6 b173 6c67 7b8a 22f0  j..u..1..slg{.".
-00000050: d232 6d6b 2b4b 5a51 4a6a 2cfa dfcf 0c25  .2mk+KZQJj,....%
-00000060: df93 26e9 c5bb db92 0860 8997 e10c 391c  ..&......`....9.
-00000070: 0e3f 8a8c 7964 1efd 72c9 3f9c 0b3e 12e1  .?..yd..r.?..>..
-00000080: b36f 12ac 24dc f76b 5985 e2ea 99e2 73b9  .o..$..kY.....s.
-00000090: 6229 ff0c 3e3c db43 8865 c443 acfe 6b0b  b)..><.C.e.C..k.
-000000a0: f92f 09f9 6398 45ce 4cd4 72e5 e35c a96c  ./..c.E.L.r..\.l
-000000b0: bd28 154d ebf8 f8b8 902b b267 3a7c f741  .(.M.....+.g:|.A
-000000c0: 46a1 e033 d789 b291 f810 65b9 e7f9 118f  F..3......e.....
-000000d0: fc30 6b99 39b3 70f4 d5c6 7fa5 544a 7ecb  .0k.9.p.....TJ~.
-000000e0: c9af 95df 1af3 1be3 bf5c 29e6 9e41 699f  .........\)..Ai.
-000000f0: e33f f487 8ef7 c986 e2e3 f1f7 37fe cd7f  .?..........7...
-00000100: 82fd cf97 77ed 7f41 dbff bdd8 fffc 9afd  ....w..A........
-00000110: 2fbe a858 b98a 6969 cbaf ed7f 62ff 5bcd  /..X..ii....b.[.
-00000120: 9346 bbd7 f8f2 a151 2e16 efb3 ff79 ab5c  .F.....Q.....y.\
-00000130: d81a ff95 4ab1 f20c ac7d 8eff 1fd4 fe5f  ....J....}....._
-00000140: 34fb d072 6ce1 49c1 d889 1fcc 4367 328d  4..rl.I.....Cg2.
-00000150: e0c0 3e84 bc95 3bce e6ad 7c0e bad4 3670  ..>...;...|...6p
-00000160: c1c3 3f63 1131 7629 c299 23a5 e37b e048  ..?c.1v)..#..{.H
-00000170: 988a 500c e730 09b9 1789 5106 c6a1 10e0  ..P..0....Q.....
-00000180: 8fc1 9ef2 7022 3210 f9c0 bd39 0422 9458  ....p"2....9.".X
-00000190: c01f 46dc f11c 6f02 1c6c ac8e 61ce 688a  ..F...o..l..a.h.
-000001a0: 64a4 3f8e 6e79 2830 f308 b894 beed 70a4  d.?.ny(0......p.
-000001b0: 0723 df8e 67c2 43a5 a4fa c68e 2b24 1c44  .#..g.C.....+$.D
-000001c0: 5301 462f 2d61 1caa 4a46 82bb 0cd9 a4b4  S.F/-a..JF......
-000001d0: 4512 dc3a d1d4 8f23 0805 2aba 6313 8d0c  E..:...#..*.c...
-000001e0: 389e edc6 23e2 6191 ec3a 3327 ad81 8aab  8...#.a..:3'....
-000001f0: 3690 0c89 c612 2520 3e33 30f3 47ce 987e  6.....% >30.G..~
-00000200: 8512 2b88 87ae 23a7 1918 3944 7a18 4718  ..+...#...9Dz.G.
-00000210: 2929 5235 6686 e438 f243 90c2 7519 5270  ))R5f..8.C..u.Rp
-00000220: 906f 25eb 8a3b 9587 580f a841 a3b4 8924  .o%..;..X..A...$
-00000230: c5dc 4efd d9a6 248e 64e3 38f4 b04a a1ca  ..N...$.d.8..J..
-00000240: 8c7c 6c32 55e3 1fc2 8e28 86b2 8f7d d7f5  .|l2U....(...}..
-00000250: 6f49 34db f746 0e49 24ab 8cf5 3189 0ffd  oI4..F.I$...1...
-00000260: 1ba1 6449 ba18 073a b29a b040 1d10 ac7a  ..dI...:...@...z
-00000270: 354d 9253 eeba 3014 6983 61bd d8bc 7c4d  5M.S..0.i.a...|M
-00000280: 9c90 aac7 81e1 450e 7721 f043 55df b698  ......E.w!.CU...
-00000290: 26d6 7fde 805e e7ac ffa6 de6d 40b3 0797  &....^.....m@...
-000002a0: ddce 6fcd d3c6 2918 f51e be1b 1978 d3ec  ..o...)......x..
-000002b0: 9f77 aefa 8039 baf5 76ff 2d74 cea0 de7e  .w...9..v.-t...~
-000002c0: 0bbf 36db a719 68fc efb2 dbe8 f5a0 d365  ..6...h........e
-000002d0: cd8b cb56 b381 71cd f649 ebea b4d9 7e0d  ...V..q..I....~.
-000002e0: afb0 5cbb 837a dc44 6d46 a2fd 0e50 8529  ..\..z.DmF...P.)
-000002f0: a966 a347 c42e 1add 9373 7cad bf6a b69a  .f.G.....s|..j..
-00000300: fdb7 1976 d6ec b789 e659 a70b 75b8 ac77  ...v.....Y..u..w
-00000310: fbcd 93ab 56bd 0b97 57dd cb4e af81 d59f  ....V...W..N....
-00000320: 22d9 76b3 7dd6 c55a 1a17 8d76 dfc4 5a31  ".v.}..Z...v..Z1
-00000330: 0e1a bfe1 0bf4 ceeb ad16 55c5 ea57 c87d  ..........U..W.}
-00000340: 97f8 8393 cee5 db6e f3f5 791f ce3b add3  .......n..y..;..
-00000350: 0646 be6a 2067 f557 ad46 5215 0a75 d2aa  .F.j g.W.FR..u..
-00000360: 372f 3270 5abf a8bf 6ea8 521d a4d2 6594  7/2pZ...n.R...e.
-00000370: 2de1 0ede 9c37 288a eaab e3df 49bf d969  -....7(.....I..i
-00000380: 9318 279d 76bf 8baf 1994 b2db 5f16 7dd3  ..'.v......._.}.
-00000390: ec35 3250 ef36 7bd4 2067 ddce 4586 5173  .52P.6{. g..E.Qs
-000003a0: 6289 8e22 82e5 da8d 840a 3535 6cf4 0866  b.."......55l..f
-000003b0: a1f7 ab5e 6349 104e 1bf5 16d2 ea51 6112  ...^cI.N.....Qa.
-000003c0: 7191 d9d4 cec1 f714 b4ff affd ff15 fe63  q..............c
-000003d0: 1dbf 28e5 b5ff affd ff85 ff7f 516f 37cf  ..(.........Qo7.
-000003e0: 1abd bef9 49df f8cb fc7f 4c2c 6d8e ffbc  ....I.....L,m...
-000003f0: 55c2 1fed ffef 2184 c28e 43e9 dc88 6cea  U.....!...C...l.
-00000400: e481 8c06 a40a 83a5 2a1c 8d43 1f5d 7b74  ........*..C.]{t
-00000410: 6787 b1e3 8ee0 3fda 3ce8 f9ff abce ff7a  g.....?.<......z
-00000420: ffe7 ef9b ffef deff c91f 97cb 7a98 ebf9  ............z...
-00000430: fff2 d7d7 595c 0077 be25 fe57 c0d1 be3d  ....Y\.w.%.W...=
-00000440: ff5b b4ff a3e7 ff3d e07f 22e2 231e f1ec  .[.....=..".#...
-00000450: 6f22 24ec a70a 7933 c7da 7c26 aa70 9f6e  o"$...y3..|&.p.n
-00000460: b065 5ea5 24ac 17cf 663c 9c57 e1c4 9f05  .e^.$...f<.W....
-00000470: be27 bc08 c67e 0869 7e02 a3a8 bc8a 6bb7  .'...~.i~.....k.
-00000480: 2e09 8bf3 dd98 a022 76ee cf44 36e0 13ac  ......."v..D6...
-00000490: 6c1a 4581 ac1e 1d4d 9c68 1a0f 4ddb 9f1d  l.E....M.h..M...
-000004a0: 85b3 0471 cce7 8e64 7437 27f5 389a fa61  ...q...dt7'.8..a
-000004b0: 750b a14c 62b3 62c6 1d77 2b0d 7e56 1d6d  u..Lb.b..w+.~V.m
-000004c0: a6a4 0bbf 4c28 1355 f792 5d86 3e61 69d9  ....L(.U..].>ai.
-000004d0: ab6e ab0a c41a 7196 7990 b37b 1a69 83da  .n....q.y..{.i..
-000004e0: ab78 02fd 90db ef45 f8b9 048f 1c29 6321  .x.....E.....)c!
-000004f0: d989 cba5 74c6 8e40 b1b1 8e49 c867 336a  ....t..@...I.g3j
-00000500: e316 f726 3132 0c55 8c9f 6303 78f4 54d8  ...&12.U..c.x.T.
-00000510: c89f 22bd 94d0 e935 a11e 04a1 7f23 46f4  .."....5.....#F.
-00000520: be0e 04af 17e9 0422 4c3a b137 c75e 9825  ......."L:.7.^.%
-00000530: 65a1 e98d 4480 3e21 7636 eb8a 3f63 077b  e...D.>!v6..?c.{
-00000540: 359b 545b 8597 b582 79cc 4e85 b443 27a0  5.T[....y.N..C'.
-00000550: 8ece 9e28 0f32 caf6 e701 f635 0976 8412  ...(.2.....5.v..
-00000560: bf1f f9b7 1e4b 6bcd 9e39 2ea6 a53b 0e8c  .....Kk..9...;..
-00000570: fd3c cdbd 5c53 c185 36a1 583f 1f61 1263  .<..\S..6.X?.a.c
-00000580: 5978 d7f4 7058 baee f5c1 7327 793a a4d8  Yx..pX....s'y:..
-00000590: ffc6 8efd 1eae a4c0 f83f e939 1b4b a152  .........?.9.K.R
-000005a0: 4ec5 8d70 fd80 f064 4c1b adde 0e19 c05d  N..p...dL......]
-000005b0: f4b2 b934 a51b 7b18 1bc6 9ea2 93b2 8c31  ...4..{........1
-000005c0: 29dc ab62 13b5 c348 ae1e 541c 09ae d061  )..b...H..T....a
-000005d0: 3f94 9862 afbd 1e32 c69e 435a 2563 bfff  ?..b...2..CZ%c..
-000005e0: fe3b 0b9c 00d2 9aef 145d 65c2 424b 0919  .;.......]e.BK..
-000005f0: 3bc1 5c11 c1b8 203e f059 e00a 3398 2b98  ;.\... >.Y..3.+.
-00000600: 5c51 0c54 8f30 f4e0 67bb 8e3d 3833 c26c  \Q.T.0..g..=83.l
-00000610: a117 f531 bebe d45c a686 6b0d 8c96 1f62  ...1...\..k....b
-00000620: 873b 818c 6730 f25d c27b 9d08 d036 4404  .;..g0.].{...6D.
-00000630: 8aa3 d876 24a2 1847 fac8 091c 6993 9208  ...v$..G....i...
-00000640: 64d8 84ba f004 7114 c114 7524 1421 16f3  d.....q...u$.!..
-00000650: 43db 3151 63b9 9064 2178 6c13 0b33 ee0a  C.1Qc..d!xl..3..
-00000660: 19a3 0902 d71f 1280 2c4d e8c5 9254 0bf5  ........,M...T..
-00000670: 1de5 b215 4918 3a43 8c8a 67aa e249 2c50  ....I.:C..g..I,P
-00000680: 875c 3796 803d 9841 d29e 82c8 8951 1347  .\7..=.A.....Q.G
-00000690: 7a1c 3a12 78b4 c843 9b02 7118 509c eb28  z.:.x..C..q.P..(
-000006a0: 2340 6b9e 589a 0663 5bb2 1f90 e887 4933  #@k.X..c[.....I3
-000006b0: 6397 5793 6e59 7605 a002 acb5 f3a2 3bd6  c.W.nYv.......;.
-000006c0: d40a 5fb7 fa14 4739 d82e 9a45 c0a7 5f56  .._...G9...E.._V
-000006d0: 63be fa88 316f 6276 668f eeb7 c4eb 0a93  c...1obvf.......
-000006e0: 1560 a61c 3d07 64fe 71bc 2f37 7fd0 00d0  .`..=.d.q./7....
-000006f0: 7ba2 c428 fde6 9ecf 7358 d764 35f8 3672  {..(....sX.d5.6r
-00000700: 5c1f dc67 5751 cdb5 9ba5 d77f 1aff fd17  \..gWQ..........
-00000710: e0bf b95c ae62 69fc 57af ff16 ebbf 6ea3  ...\.bi.W.....n.
-00000720: 7e7a d130 67a3 6fb8 fecb 5572 85ed f55f  ~z.0g.o...Ur..._
-00000730: 3e9f d7eb bf7d 04ed 656b 2f5b 7bd9 3fae  >....}..ek/[{.?.
-00000740: 97ad fd3f edff 6de0 fff9 b2f6 ffb4 ffb7  ...?..m.........
-00000750: f0ff 8279 90c0 9866 e4cf dc6f e4ff e573  ...y...f...o...s
-00000760: dbf8 7fae 5c2a 6aff 6f1f e15d dabf d7cc  ....\*j.o..]....
-00000770: 438f 83dc 91fb 34c2 6037 09ec 4f99 9476  C.....4.`7..O..v
-00000780: 182c 71c1 24c6 bc43 07ee 2f20 1a35 6363  .,q.$..C../ .5cc
-00000790: ca32 32a0 70f8 9a71 dfd4 65c0 c70c bb66  .22.p..q..e....f
-000007a0: a315 5c4c 353c 752f c160 c8f6 2811 61b9  ..\L5<u/.`..(.a.
-000007b0: 6aa1 c814 9b4e 7c34 4a55 e8b4 c1ec 25c8  j....N|4JU....%.
-000007c0: bde0 1fc0 7804 a06e 6492 ac8f c3d2 17b9  ....x..nd.......
-000007d0: 1f86 d10d 6a04 b6e8 0f33 0e5d 79cd 8cc5  ....j....3.]y...
-000007e0: 3684 419c 7fde c681 c18c b5ed 872f 2094  6.A........../ .
-000007f0: ee40 a03f f74e 7d09 9295 4a94 eb65 2353  .@.?.N}...J..e#S
-00000800: 3b1a 129d d520 f27d 57be ac95 73a6 655c  ;.... .}W...s.e\
-00000810: b324 f790 eaf7 464a c796 794c 9536 4067  .$....FJ..yL.6@g
-00000820: 971b 7ada f941 f1bf 4261 d7ff cb69 ff6f  ..z..A..Ba...i.o
-00000830: 2ffe 5fe5 aeef 3f5e 5805 7dfc 57fb 7f85  /._...?^X.}.W...
-00000840: 2365 a84d 7b3c f986 f89f 6515 cb3b df7f  #e.M{<....e..;..
-00000850: 9635 feb7 1fff 4f4c 2603 c71b fbd7 2ce2  .5....OL&.....,.
-00000860: 9341 f285 670d d4cb 8820 af1a 587a 034f  .A..g.... ..Xz.O
-00000870: cfff 1aff f931 f09f 4a49 9fff d6f3 ffd6  .....1..JI......
-00000880: fc1f ccbf 7868 7c0a ff29 e58a dbf3 7f51  ....xh|..).....Q
-00000890: e33f fb09 e9e6 d46a 41ce 181d 8a06 3f10  .?.....jA.....?.
-000008a0: dec1 1a90 9201 2324 28c7 b37d 3a39 5d33  ......#$(..}:9]3
-000008b0: e268 9c3d 360e 814b 184f ab0a e470 7d0f  .h.=6..K.O...p}.
-000008c0: 9d86 0d18 673c 3509 9639 3864 6c6d cdaf  ....g<5..98dlm..
-000008d0: 1e0f 5499 0431 923b 9845 029b a488 532d  ..T..1.;.E....S-
-000008e0: c59b 92c8 0474 da81 99d6 d206 0f21 4e49  .....t.......!NI
-000008f0: e635 566b 4fc7 9b32 77ca 5cdb 8eb8 3bdb  .5VkO..2w.\...;.
-00000900: c04e 3e88 1c44 f300 e5df f820 32a5 1c87  .N>..D..... 2...
-00000910: 28c1 677d 159b 1208 b8fd 9e4f c460 e484  (.g}.......O.`..
-00000920: d813 7f19 4615 0c19 dac6 c78d 6459 5beb  ....F.......dY[.
-00000930: 98b1 e38d 068b 8483 5b3a da5f 5365 0e93  ........[:._Se..
-00000940: 32e9 19a1 c192 348f 78ad 1fc6 2225 a950  2.....4.x..."%.P
-00000950: b2c1 020e aaa5 505b 92b8 86b7 d512 b4ed  ......P[........
-00000960: 8988 dbd3 51b7 c723 6f94 f37a 21a3 dae8  ....Q..#o..z!...
-00000970: 5b49 b1c6 ec6a 9bef 650d 72a6 655a abb2  [I...j..e.r.eZ..
-00000980: 87ff ca59 539f ffd1 e77f 76f1 1f9c 9e4b  ...YS.....v....K
-00000990: 79ed 056a ff0f 6dff d157 19ff 4fbb ffad  y..j..m..W..O...
-000009a0: 522a 58fa fe37 6dff b5fd ff7b ec7f a15c  R*X..7m....{...\
-000009b0: 2c15 b4fd d7f6 9fec ffee 8500 dfda fee7  ,...............
-000009c0: 0b05 aba2 edbf c67f b5fd df37 fe5b 2aeb  ...........7.[*.
-000009d0: fb7f b4fd 7fc0 fe0f 068e e744 83c1 2381  ...........D..#.
-000009e0: e187 ceff 972a dbf8 6fa9 58d0 e7ff f789  .....*..o.X.....
-000009f0: fffa 92a5 4f21 f746 fe8c 2d5e 97fa 41d8  ....O!.F..-^..A.
-00000a00: 6302 904a f326 47b0 ef2a 82b1 8087 8466  c..J.&G..*.....f
-00000a10: 2650 a32f cd80 4753 13df 08de 3d58 bcf3  &P./..GS....=X..
-00000a20: a1a4 df83 c180 4e4e 0c06 8787 c997 615b  ......NN......a[
-00000a30: c5fe f01d ef60 4530 03c6 e605 44c6 211b  .....`E0....D.!.
-00000a40: 2ceb 1e8c 63cf c6c2 6bdc 8d84 ed62 e955  ,...c...k....b.U
-00000a50: 9e03 63eb fc81 9101 aaa9 b6ac fd90 b191  ..c.............
-00000a60: 18c3 5dc7 1432 b03a 1822 0f13 a0db 308c  ..]..2.:."....0.
-00000a70: c581 10f0 c46d 0219 7ab6 baf6 74a7 2e93  .....m..z...t...
-00000a80: a932 973c a423 1d22 94ea 35bb 0cea 5581  .2.<.#."..5...U.
-00000a90: ccea c685 25d8 4877 76aa e8c8 a73b 3853  ....%.Hwv....;8S
-00000aa0: 2ec4 2821 b7c6 1496 731d 192d 0b36 93eb  ..(!....s..-.6..
-00000ab0: 3755 d929 a7e3 1804 c1cf 9188 f056 6432  7U.).........Vd2
-00000ac0: 2ad3 3a19 9b7b 5451 c0a5 4cae 18a5 0ccb  *.:..{TQ..L.....
-00000ad0: 4684 f46a d5b1 1fce 484e ae2a a5a7 5172  F..j....HN.*..Qr
-00000ae0: af2a 0fe9 4e50 b579 b079 1329 0a15 db51  .*..NP.y.y.)...Q
-00000af0: 1c8a ea92 c515 a4ba fb46 e1af 9d18 05a2  .........F......
-00000b00: f3a1 70ab 60a8 df35 8877 3dd0 688e aa60  ..p.`..5.w=.h..`
-00000b10: dd9d 8a3a 5485 9cb5 93f6 31f3 f7b3 b011  ...:T.....1.....
-00000b20: 739d f9a7 b5d0 267b 6cf7 493d 74e9 a492  s.....&{l.I=t...
-00000b30: b7a1 e2c9 560b ea08 dd17 db46 5dda d0f0  ....V......F]...
-00000b40: 7505 9ca1 0b0a c3b9 529f 588a 7057 e596  u.......R.X.pW..
-00000b50: aa36 ffb4 a201 bbbb 9d3e d53e 77b7 cb76  .6.......>.>w..v
-00000b60: 7b7c 640b 0bc0 9642 3f87 133a 1914 4d43  {|d....B?..:..MC
-00000b70: 3f9e 4c69 e4f8 7108 41e8 dc90 8958 8d20  ?.Li..q.A....X. 
-00000b80: 3255 c4be 09f5 70a2 2e35 c6f1 920c 3875  2U....p..5....8u
-00000b90: 8b72 4aec d649 6edd 5507 b816 f7fa a616  .rJ..In.U.......
-00000ba0: 3003 6a53 86e2 e63f 25d9 f80d 7750 1e57  0.jS...?%...wP.W
-00000bb0: a8db 793d 3078 3891 464a 6bd5 6066 1293  ..y=0x8.FJk.`f..
-00000bc0: c61b 68ee 78ec 4606 dde0 cc41 06c2 a62b  ..h.x.F....A...+
-00000bd0: 7c79 ca17 d2e7 5112 3ba6 514d 2cd0 944f  |y....Q.;.QM,..O
-00000be0: 7942 d5c5 299d 1bee c662 71e1 ef4a d2a1  yB..)....bq..J..
-00000bf0: c03e 13ab 8e24 33e4 a000 21b7 e94e 67d5  .>...$3...!..Ng.
-00000c00: 7738 a524 fb42 4b53 9e10 abc1 9675 5766  w8.$.BKS.....uWf
-00000c10: b8b6 638b 6beb 7699 a5fc bc21 2e62 7794  ..c.k.v....!.bw.
-00000c20: ded6 ac38 48c8 266c 63e5 ea94 de96 691b  ...8H.&lc.....i.
-00000c30: 533f dcaa 0bac d376 22e5 0cc5 4f12 3c1f  S?.....v"...O.<.
-00000c40: 4dfc f2ca 6575 5332 b633 75b0 74e8 90d7  M...euS2.3u.t...
-00000c50: e2b0 1764 6118 23a9 08cb 602f f86a 9b2f  ...da.#...`/.j./
-00000c60: 2196 54bd 2de8 3fe3 ab2a 8dff 69fc 6f17  !.T.-.?..*..i.o.
-00000c70: ffab 9472 96c6 fff4 fa2f 5dff a559 b696  ...r...../]..Y..
-00000c80: 81a6 984c b2f4 e9e8 d123 86c6 d3f0 bf32  ...L.....#.....2
-00000c90: ae09 35fe a7f1 3f6d fff7 8dff 29fb af2d  ..5...?m....)..-
-00000ca0: bfb6 ff4f b1ff 0fdc 12fa f4fb 3f2b c592  ...O........?+..
-00000cb0: feff 3f7b 09fa fe4f 7dff a7be ff53 df4c  ..?{...O}....S.L
-00000cc0: a46f 26d2 3713 e9fb 3f7f bca0 d77f 7afd  .o&.7...?.....z.
-00000cd0: a7d7 7f7a fdf7 45eb bf5e e7aa 7bd2 e899  ...z..E..^..{...
-00000ce0: d187 e833 d67f 56a9 90df 1cff 054c 2de8  ...3..V......L-.
-00000cf0: f5df 3ec2 c2dd 5efb 475f 6c79 ea8f 6d5e  ..>...^.G_ly..m^
-00000d00: ffc5 16a7 41d9 839f 05b1 a701 07ec c97a  ....A..........z
-00000d10: f6c8 128b 458a 3d1f b88e f75e 3ea1 e8e2  ....E.=....^>...
-00000d20: fcd7 138a 447e 3070 c917 bc6f 24e8 f95f  ....D~0p...o$.._
-00000d30: cfff 7afe d7e1 3b9b ffef b2b2 4f98 ff2d  ..z...;.....O..-
-00000d40: 2bb7 35ff e78b f992 9eff f711 f450 d7eb  +.5..........P..
-00000d50: 7f3d ffeb f95f cfff 7afe ffec f97f 7da9  .=..._..z.....}.
-00000d60: f419 eb7f 2bbf 3dff 5b95 92fe ffcf fbed  ....+.=.[.......
-00000d70: ff97 3575 9f89 1efa 7afe d7f3 bf9e ff75  ..5u....z......u
-00000d80: d0f3 ffa3 e7ff 0770 cf87 e7ff 6dfc 3f97  .......p....m.?.
-00000d90: b334 febf a7fe dfea 553d f675 d041 071d  .4......U=.u.A..
-00000da0: 7e88 f07f 31c6 c63a 00a0 0000            ~...1..:....
+00000020: 6f72 2d30 2e31 2e34 2e74 6172 00ed 5d5b  or-0.1.4.tar..][
+00000030: 6fdb b812 ee33 7fc5 407d d8e4 c056 24df  o....3..@}...V$.
+00000040: 921a eb62 ddc4 698c 75ec 1cdb d99e a208  ...b..i.u.......
+00000050: bcb4 4cdb daca 9256 9492 1a8b fef7 3343  ..L....V......3C
+00000060: c9d7 244d d28b 77b7 2511 c012 2fc3 195e  ..$M..w.%.../..^
+00000070: 86c3 8fe2 c43c 300f 7eb9 e01f ce04 1f89  .....<0.~.......
+00000080: e8d9 3709 561a eefb b5ac 6271 f54c f1b6  ..7.V.....bq.L..
+00000090: 5d2a dbcf e0c3 b31d 8444 c63c c2ea bfb6  ]*.......D.<....
+000000a0: 90ff 9250 3884 59ec ce44 cdae 1cd9 e58a  ...P8.Y..D......
+000000b0: 5db4 8ecc a255 7a71 5864 cf74 f8fe 838c  ]....UzqXd.t....
+000000c0: 23c1 679e 1be7 63f1 21ce 73df 0f62 1e07  #.g...c.!.s..b..
+000000d0: 51de 326d b374 f0d5 e6ff 61b9 9cfe 56d2  Q.2m.t....a...V.
+000000e0: 5fab 50da 9cf3 1bf3 bf72 582a 3c83 f22e  _.P......rX*<...
+000000f0: e77f 140c 5dff 930d c5c7 e3ef 6ffe 9bff  ....].......o...
+00000100: 04fd 5fa8 dcd6 ff45 adff 77a2 ff0b 6bfa  .._....E..w...k.
+00000110: 1fd5 be65 1f9a 9656 fd5a ffa7 fabf d53c  ...e...V.Z.....<
+00000120: 6eb4 7b8d 2f9f 1a95 52e9 3efd 5fb0 2adb  n.{./...R.>._.*.
+00000130: f6df e161 d97a 06d6 2ee7 ff0f aaff cf9b  ...a.z..........
+00000140: 7d68 b98e f0a5 60ec 3808 e791 3b99 c6b0  }h....`.8...;...
+00000150: e7ec 43c1 b28f f205 ab60 4397 da06 ce79  ..C......`C....y
+00000160: f467 2262 c62e 4434 73a5 7403 1f5c 0953  .g"b..D4s.t..\.S
+00000170: 1189 e11c 2611 f763 31ca c138 1202 8231  ....&..c1..8...1
+00000180: 3853 1e4d 440e e200 b83f 8750 4412 0b04  8S.MD....?.PD...
+00000190: c398 bbbe eb4f 8083 83d5 31cc 194f 918c  .....O....1..O..
+000001a0: 0cc6 f10d 8f04 661e 0197 3270 5c8e f460  ......f...2p\..`
+000001b0: 1438 c94c f838 28a9 beb1 eb09 097b f154  .8.L.8(......{.T
+000001c0: 80d1 cb4a 18fb aa92 91e0 1e43 3629 6d91  ...J.......C6)m.
+000001d0: 0437 6e3c 0d92 1822 8103 dd75 8846 0e5c  .7n<..."...u.F.\
+000001e0: dff1 9211 f1b0 48f6 dc99 9bd5 40c5 551b  ......H.....@.U.
+000001f0: 4886 4413 8912 109f 3998 0523 774c bf42  H.D.....9..#wL.B
+00000200: 8915 2643 cf95 d31c 8c5c 223d 4c62 8c94  ..&C.....\"=Lb..
+00000210: 14a9 1a33 4772 1c04 1148 e179 0c29 b8c8  ...3Gr...H.y.)..
+00000220: b792 75c5 9dca 43ac 87d4 a071 d644 9262  ..u...C....q.D.b
+00000230: 6ea6 c16c 5312 57b2 7112 f958 a550 6546  n..lS.W.q..X.PeF
+00000240: 0136 99aa f10f e1c4 1443 d9c7 81e7 0537  .6.......C.....7
+00000250: 249a 13f8 2397 2492 55c6 fa98 c487 c1b5  $...#.$.U.......
+00000260: 50b2 a45d 8c13 1d59 4d59 a00e 0857 bd9a  P..]...YMY...W..
+00000270: 25c9 29f7 3c18 8aac c1b0 5e6c 5ebe 264e  %.).<.....^l^.&N
+00000280: 44d5 e3c4 f063 977b 1006 91aa 6f5b 4c13  D....c.{....o[L.
+00000290: eb3f 6b40 af73 da7f 53ef 36a0 d983 8b6e  .?k@.s..S.6....n
+000002a0: e7b7 e649 e304 8c7a 0fdf 8d1c bc69 f6cf  ...I...z.....i..
+000002b0: 3a97 7dc0 1cdd 7abb ff16 3aa7 506f bf85  :.}...z...:.Po..
+000002c0: 5f9b ed93 1c34 fe77 d16d f47a d0e9 b2e6  _....4.w.m.z....
+000002d0: f945 abd9 c0b8 66fb b875 79d2 6cbf 8657  .E....f..uy.l..W
+000002e0: 58ae ddc1 71dc c4d1 8c44 fb1d a00a 3352  X...q....D....3R
+000002f0: cd46 8f88 9d37 bac7 67f8 5a7f d56c 35fb  .F...7..g.Z..l5.
+00000300: 6f73 ecb4 d96f 13cd d34e 17ea 7051 eff6  os...o...N..pQ..
+00000310: 9bc7 97ad 7a17 2e2e bb17 9d5e 03ab 3f41  ....z......^..?A
+00000320: b2ed 66fb b48b b534 ce1b edbe 89b5 621c  ..f....4......b.
+00000330: 347e c317 e89d d55b 2daa 8ad5 2f91 fb2e  4~.....[-.../...
+00000340: f107 c79d 8bb7 dde6 ebb3 3e9c 755a 270d  ..........>.uZ'.
+00000350: 8c7c d540 ceea af5a 8db4 2a14 eab8 556f  .|.@...Z..*...Uo
+00000360: 9ee7 e0a4 7e5e 7fdd 50a5 3a48 a5cb 285b  ....~^..P.:H..([
+00000370: ca1d bc39 6b50 14d5 57c7 bfe3 7eb3 d326  ...9kP..W...~..&
+00000380: 318e 3bed 7e17 5f73 2865 b7bf 2cfa a6d9  1.;.~._s(e..,...
+00000390: 6be4 a0de 6df6 a841 4ebb 9df3 1ca3 e6c4  k...m..AN.......
+000003a0: 121d 4504 cbb5 1b29 156a 6ad8 e811 cc42  ..E....).jj....B
+000003b0: ef97 bdc6 9220 9c34 ea2d a4d5 a3c2 24e2  ..... .4.-....$.
+000003c0: 22b3 a98d 83ef 2968 fb5f dbff 2bfc c73a  ".....)h._..+..:
+000003d0: 7a51 2e68 fb5f dbff 0bfb ffbc de6e 9e36  zQ.h._.......n.6
+000003e0: 7a7d f393 b6f1 97d9 ff98 58de 9cff 05ab  z}........X.....
+000003f0: 6cd9 dafe df45 8884 9344 d2bd 16f9 ccc8  l....E...D......
+00000400: 0319 0f68 280c 9643 e160 1c05 68da a339  ...h(..C.`..h..9
+00000410: 3b4c 5c6f 04ff d1ea 41af ff5f 75fd 2f96  ;L\o....A.._u./.
+00000420: 6eaf ff05 bdfe ef64 fd3f baf3 fca7 7458  n......d.?....tX
+00000430: 2ae9 69ae d7ff 8b5f 5fe7 7103 dcf9 96f8  *.i....__.q.....
+00000440: 5f11 67fb f6fa 6fd1 f98f 5eff 7780 ff89  _.g...o...^.w...
+00000450: 988f 78cc f3bf 8988 b09f 2a14 4c9b b5f9  ..x.......*.L...
+00000460: 4c54 e1be b1c1 9679 d520 61bd 6436 e3d1  LT.....y. a.d6..
+00000470: bc0a c7c1 2c0c 7ce1 c730 0e22 c8f2 1318  ....,.|..0."....
+00000480: 45e5 555c bb75 4158 5ce0 2504 15b1 b360  E.U\.uAX\.%....`
+00000490: 26f2 219f 6065 d338 0e65 f5e0 60e2 c6d3  &.!.`e.8.e..`...
+000004a0: 6468 3ac1 ec20 9aa5 8863 c13e 90f1 dd9c  dh:.. ...c.>....
+000004b0: d493 781a 44d5 2d84 328d cd8b 1977 bdad  ..x.D.-.2....w..
+000004c0: 34f8 5975 b499 912e fe32 a14c 54dd 4b76  4.Yu.....2.LT.Kv
+000004d0: 1105 84a5 e52f bbad 2a10 6bc4 59ee 41ce  ...../..*.k.Y.A.
+000004e0: ee69 a40d 6aaf 9209 f423 eebc 17d1 e712  .i..j....#......
+000004f0: 3c70 a54c 8464 c71e 97d2 1dbb 02c5 c63a  <p.L.d.........:
+00000500: 2611 9fcd a88d 5bdc 9f24 c830 5431 7e8e  &.....[..$.0T1~.
+00000510: 0de0 d353 7123 7f86 f452 42a7 d784 7a18  ...Sq#...RB...z.
+00000520: 46c1 b518 d1fb 3a10 bc5e a413 8a28 edc4  F.....:..^...(..
+00000530: de1c 7b61 9696 85a6 3f12 21da 84d8 d9ac  ..{a....?.!.....
+00000540: 2bfe 4c5c ecd5 7c5a 6d15 5ed6 8ae6 113b  +.L\..|Zm.^....;
+00000550: 11d2 89dc 903a 3a7f ac2c c838 df9f 87d8  .....::..,.8....
+00000560: d724 d801 4afc 7e14 dcf8 2cab 357f ea7a  .$..J.~...,.5..z
+00000570: 9896 9d38 30f6 f3d4 7eb9 3604 17a3 09c5  ...80...~.6.....
+00000580: faf9 0093 18cb c3bb a68f d3d2 f3ae f69e  ................
+00000590: bbe9 d33e c5fe 3771 9df7 7029 05c6 ff49  ...>..7q..p)...I
+000005a0: cff9 440a 9572 22ae 8517 8484 2763 da68  ..D..r".....'c.h
+000005b0: f5b6 cf00 eea2 97b7 b394 6ee2 636c 94f8  ..........n.cl..
+000005c0: 8a4e c632 c664 70af 8a4d 871d 4672 f5a0  .N.2.dp..M..Fr..
+000005d0: e248 7085 0e07 91c4 1467 ed75 9f31 f61c  .Hp......g.u.1..
+000005e0: b22a 19fb fdf7 df59 e886 90d5 7ca7 e82a  .*.....Y....|..*
+000005f0: 1316 5a4a c8d8 31e6 8a09 c605 f181 cf42  ..ZJ..1........B
+00000600: 4f98 e15c c1e4 8a62 a87a 84a1 053f bb6d  O..\...b.z...?.m
+00000610: d883 3b23 cc16 7a71 1fe3 ebcb 91cb d474  ..;#..zq.......t
+00000620: ad81 d10a 22ec 7037 94c9 0c46 8147 78af  ....".p7...F.Gx.
+00000630: 1b03 ea86 9840 7114 db89 459c e04c 1fb9  .....@q...E..L..
+00000640: a12b 1d1a 2402 1936 a12e 7c41 1cc5 30c5  .+..$..6..|A..0.
+00000650: 3112 8908 8b05 91e3 9a38 62b9 90a4 2178  1........8b...!x
+00000660: e210 0b33 ee09 99a0 0a02 2f18 1280 2c4d  ...3....../...,M
+00000670: e825 9286 168e 7794 cb51 2461 e80e 312a  .%....w..Q$a..1*
+00000680: 99a9 8a27 89c0 31e4 7989 04ec c11c 92f6  ...'..1.y.......
+00000690: 1544 4e8c 9a38 d393 c895 c0e3 451e 3a14  .DN..8......E.:.
+000006a0: 48a2 90e2 3c57 2901 daf3 24d2 3418 db92  H...<W)...$.4...
+000006b0: 7d8f 44df 4f9b 19bb bc9a 76cb b22b 0007  }.D.O.....v..+..
+000006c0: c05a 3b2f ba63 6d58 e1eb 569f e22c 07c7  .Z;/.cmX..V..,..
+000006d0: 43b5 08f8 f4cb 6ace 571f 31e7 4dcc ce9c  C.....j.W.1.M...
+000006e0: d1fd 9a78 7dc0 e405 9819 47cf 0199 7f1c  ...x}.....G.....
+000006f0: efcb c31f 5400 f49e 0e62 947e f3cc e739  ....T....b.~...9
+00000700: ac8f 6435 f936 725c eddd a757 7198 6b33  ..d5.6r\...Wq.k3
+00000710: 4bef ff34 fefb 2fc0 7f6d db3e b434 feab  K..4../..m.>.4..
+00000720: f77f 8bfd 5fb7 513f 396f 98b3 d137 dcff  ...._.Q?9o...7..
+00000730: d987 7671 7bff 5728 14f5 fe6f 1741 5bd9  ..vq{.W(...o.A[.
+00000740: daca d656 f68f 6b65 6bfb 4fdb 7feb f87f  ...V..kek.O.....
+00000750: e185 aded 3f6d ff2d ecbf 701e a630 a619  ....?m.-..p..0..
+00000760: 0733 ef1b d97f 057b 1bff b72b e5b2 b6ff  .3.....{...+....
+00000770: 7611 de65 fd7b c57c b438 c81c b96f 4418  v..e.{.|.8...oD.
+00000780: ec3a 85fd 2993 1a1d 064b 4d30 8931 efd0  .:..)....KM0.1..
+00000790: 80fb 0b88 46cd d858 b28c 1c28 1cbe 66dc  ....F..X...(..f.
+000007a0: b774 19f0 31c7 aed8 6805 1753 0d4f 3d4b  .t..1...h..S.O=K
+000007b0: 3018 b23d 4a45 58ee 5a28 32c3 a653 1b8d  0..=JEX.Z(2..S..
+000007c0: 5215 3a6d 3067 0972 2ff8 0730 1e01 a81b  R.:m0g.r/..0....
+000007d0: b934 ebe3 b0f4 45ee 8761 7483 1a81 2dfa  .4....E..at...-.
+000007e0: c34c 224f 5e31 6371 0c61 10e7 9f77 7060  .L"O^1cq.a...wp`
+000007f0: 3063 edf8 e10b 0865 2710 68cf bd53 5f82  0c.....e'.h..S_.
+00000800: e4a5 12e5 6ad9 c8d4 8e86 4463 358c 83c0  ....j.....Dc5...
+00000810: 932f 6b15 5c4c 8c2b 96e6 1e52 fdfe 488d  ./k.\L.+...R..H.
+00000820: b165 1e53 a50d d0d8 e586 5e76 7e50 fcaf  .e.S......^v~P..
+00000830: 58b8 6dff 59da fedb 89fd 57b9 ebfb 8fb2  X.m.Y.....W.....
+00000840: 75a4 27a3 b6ff 4a07 4a51 9bce 78f2 0df1  u.'...J.JQ..x...
+00000850: 3fcb 2a55 6e7d ff59 d1f8 df6e ec3f 3199  ?.*Un}.Y...n.?1.
+00000860: 0c5c 7f1c 5cb1 984f 06e9 179e 3550 2f23  .\..\..O....5P/#
+00000870: 82bc 6a60 e903 3cbd fe6b fce7 47c1 7f2a  ..j`..<..k..G..*
+00000880: 1aff d1eb ffe6 fa1f cebf 786a 7c0a ff29  ..........xj|..)
+00000890: dba5 edf5 bfa4 f19f dd84 ec70 6ab5 2167  ...........pj.!g
+000008a0: 8c2e 4543 100a 7f6f 0d48 c981 1111 94e3  ..EC...o.H......
+000008b0: 3b01 dd9c ae19 493c ce1f 19fb c025 8ca7  ;.....I<.....%..
+000008c0: 5505 7278 818f 46c3 068c 339e 9a04 cbec  U.rx..F...3.....
+000008d0: ed33 b6b6 e757 8f7b aa4c 8a18 c95b 9845  .3...W.{.L...[.E
+000008e0: 0a9b 6488 532d c39b d2c8 1474 ba05 33ad  ..d.S-.....t..3.
+000008f0: a50d 1e42 9cd2 cc6b acd6 9e8e 37e5 ee94  ...B...k....7...
+00000900: b9b6 1d71 77b6 8193 7e10 3988 e721 cabf  ...qw...~.9..!..
+00000910: f141 6446 3989 5082 cffa 2a36 2310 72e7  .AdF9.P...*6#.r.
+00000920: 3d9f 88c1 c88d b027 fe32 8c2a 1832 728c  =......'.2.*.2r.
+00000930: 8f1b c9b2 b6d6 3163 d71f 0d16 097b 3774  ......1c.....{7t
+00000940: b5bf a6ca eca7 65b2 3b42 8325 691e f35a  ......e.;B.%i..Z
+00000950: 3f4a 4446 52a1 6483 051c 54cb a0b6 3471  ?JDFR.d...T...4q
+00000960: 0d6f aba5 68db 1311 b7a7 a36e 8f47 de28  .o..h......n.G.(
+00000970: e7d5 4246 75d0 b792 628d d9d5 31df cb1a  ..BFu...b...1...
+00000980: d8a6 655a abb2 fbff ca55 53df ffd1 f77f  ..eZ.....US.....
+00000990: b6f1 9fc2 8bd2 51b9 f442 5b81 dafe 43dd  ......Q..B[...C.
+000009a0: 7ff0 55e6 ffd3 fcbf 1d96 8bb6 f6ff a6f5  ..U.............
+000009b0: bfd6 ff7f 87fe 2f5a b8ff b2cb 5aff 6bfd  ....../Z....Z.k.
+000009c0: 4ffa ffb6 4380 6fad ff0b c5a2 6d69 fdaf  O...C.o.....mi..
+000009d0: f15f adff 778c ff5a e58a f6ff a3f5 ff03  ._..w..Z........
+000009e0: fa7f 3070 7d37 1e0c 1e09 0c3f 74ff bf7c  ..0p}7.....?t..|
+000009f0: b88d ff96 4b45 7dff 7f97 f86f 2059 f614  ....KE}....o Y..
+00000a00: 717f 14cc d8e2 7539 3e08 7b4c 0152 695e  q.....u9>.{L.Ri^
+00000a10: db04 fbae 2218 0b79 4468 660a 3506 d20c  ...."..yDhf.5...
+00000a20: 793c 35f1 8de0 ddbd c53b 1f4a fadd 1b0c  y<5......;.J....
+00000a30: e8e6 c460 b0bf 9f7e 19b6 55ec 8fc0 f5f7  ...`...~..U.....
+00000a40: 5604 7360 6c3a 2032 f6d9 6059 f760 9cf8  V.s`l: 2..`Y.`..
+00000a50: 0e16 5ee3 6e24 1c0f 4baf f2ec 195b f70f  ..^.n$..K....[..
+00000a60: 8c1c 504d b565 edfb 8c8d c418 eeba a690  ..PM.e..........
+00000a70: 83d5 c510 b99f 02dd 8661 2c2e 8480 2f6e  .........a,.../n
+00000a80: 52c8 d077 94db d35b 7599 4c95 b9e0 115d  R..w...[u.L....]
+00000a90: e910 9154 aff9 6550 af0a 6456 1e17 9660  ...T..eP..dV...`
+00000aa0: 23f9 ec54 d171 403e 3833 2ec4 2825 b7c6  #..T.q@>83..(%..
+00000ab0: 1496 f35c 192f 0b36 53f7 9baa ec94 d375  ...\./.6S......u
+00000ac0: 0c82 e0e7 4844 f82b 3239 9569 9d8c c37d  ....HD.+29.i...}
+00000ad0: aa28 e452 a62e 4629 c3b2 1121 73ad 3a0e  .(.R..F)...!s.:.
+00000ae0: a219 c9c9 55a5 f434 4afd aaf2 887c 82aa  ....U..4J....|..
+00000af0: c383 4d4f a428 54e2 c449 24aa 4b16 5790  ..MO.(T..I$.K.W.
+00000b00: eaed 370a 7fdd 8a51 203a 1f0a af0a 86fa  ..7....Q :......
+00000b10: 5d83 78d7 03cd e6b8 0ad6 dda9 3886 aa60  ].x.........8..`
+00000b20: 5bb7 d23e e6fe 7e16 3662 ae72 ffb4 16da  [..>..~.6b.r....
+00000b30: 648f dd7e 520f 5dba a9e4 6f0c f1f4 a805  d..~R.]...o.....
+00000b40: c708 f98b 6de3 58da 18e1 eb03 7086 2628  ....m.X.....p.&(
+00000b50: 0ce7 6af8 2452 44b7 87dc 72a8 cd3f 3dd0  ..j.$RD...r..?=.
+00000b60: 80dd dd4e 9f6a 9fbb db65 bb3d 3eb2 8506  ...N.j...e.=>...
+00000b70: 604b a19f c331 dd0c 8aa7 5190 4ca6 3473  `K...1....Q.L.4s
+00000b80: 8224 8230 72af 4945 ac66 10a9 2a62 df84  .$.0r.IE.f..*b..
+00000b90: 7a34 514e 8d71 bea4 134e 7951 ce88 ddb8  z4QN.q...NyQ....
+00000ba0: a9d7 5d75 816b e1d7 37d3 8039 5087 3214  ..]u.k..7..9P.2.
+00000bb0: 37ff 29cd c6af b98b f278 4279 e7f5 c1e0  7.)......xBy....
+00000bc0: d144 1a19 ad55 8399 694c 166f a0ba e389  .D...U..iL.o....
+00000bd0: 171b e4c1 9983 0c85 432e 7c79 c617 d2e7  ........C.|y....
+00000be0: 711a 3ba6 594d 2cd0 924f 7922 d5c5 199d  q.;.YM,..Oy"....
+00000bf0: 6bee 2562 e1f0 7725 e950 609f 8955 4792  k.%b..w%.P`..UG.
+00000c00: 1a72 5180 883b e4d3 59f5 1d2e 29e9 b9d0  .rQ..;..Y...)...
+00000c10: 5295 a7c4 6ab0 a5dd 951a aedd d2c5 b575  R...j..........u
+00000c20: bdcc 327e de10 1789 37ca bc35 2b0e 52b2  ..2~....7..5+.R.
+00000c30: 29db 58b9 baa5 b7a5 dac6 d40f 37ca 8175  ).X.........7..u
+00000c40: d64e 3438 23f1 9304 3f40 15bf 74b9 ac3c  .N48#...?@..t..<
+00000c50: 2563 3b53 074b 972e 792d 2e7b 411e 8609  %c;S.K..y-.{A...
+00000c60: 928a b10c f642 a08e f952 6269 d5db 82fe  .....B...Rbi....
+00000c70: 33be aad2 f89f c6ff 6ee3 7fc5 ca91 55d0  3.......n.....U.
+00000c80: bb40 bdff 4bf7 7f59 96ad 6da0 2926 933c  .@..K..Y..m.)&.<
+00000c90: 7d3a 7af0 88a9 f134 fcaf 52ac 68fc 4fe3  }:z....4..R.h.O.
+00000ca0: 7f5a ffef 1aff 53fa 5fe3 7f5a ff3f 49ff  .Z....S._..Z.?I.
+00000cb0: 3fe0 25f4 e9fe 3f0f 4b15 fdff 7f76 12b4  ?.%...?.K....v..
+00000cc0: ff4f edff 53fb ffd4 9e89 b467 22ed 9948  .O..S......g"..H
+00000cd0: fbff fcf1 82de ffe9 fd9f deff e9fd df17  ................
+00000ce0: edff 7a9d cbee 71a3 67c6 1fe2 cfd8 ff59  ..z...q.g......Y
+00000cf0: e56d ff1f 454c 2de9 fddf 2ec2 c2dc 5efb  .m..EL-.......^.
+00000d00: 475f 6c79 eb8f 6dba ff62 8bdb a0ec c1cf  G_ly..m..b......
+00000d10: 82d8 d380 03f6 e471 f6c8 128b 4d8a 331f  .......q....M.3.
+00000d20: 78ae ff5e 3ea1 e8e2 fed7 138a c441 38f0  x..^>........A8.
+00000d30: c816 bc6f 26e8 f55f afff 7afd d7e1 3b5b  ...o&.._..z...;[
+00000d40: ffef d2b2 4f58 ff2d cbde 5aff 0b25 5409  ....OX.-..Z..%T.
+00000d50: 7afd df41 d053 5def fff5 faaf d77f bdfe  z..A.S].........
+00000d60: ebf5 ffb3 d7ff f5ad d267 ecff adc2 f6fa  .........g......
+00000d70: 6f1d 96f5 ff7f de6d ffbf ac29 7f26 7aea  o......m...).&z.
+00000d80: ebf5 5faf ff7a fdd7 41af ff8f 5eff 1fc0  .._..z..A...^...
+00000d90: 3d1f 5eff b7f1 7fdb b634 febf a3fe dfea  =.^......4......
+00000da0: 553d f775 d041 071d 7e88 f07f 5b61 f934  U=.u.A..~...[a.4
+00000db0: 00a0 0000                                ....
```

