# Comparing `tmp/phayes-0.0.0-py3-none-any.whl.zip` & `tmp/phayes-0.0.1.tar.gz`

 * *Command `'zipinfo {}'` failed with exit code 9. Standard output:*

 * *    Archive:  tmp/phayes-0.0.1.tar.gz*

 * *    […]*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

```diff
@@ -1,64 +1,53 @@
-00000000: 504b 0304 1400 0000 0800 ce50 be56 7c72  PK.........P.V|r
-00000010: 83bd 8900 0000 ad00 0000 1f00 0000 7068  ..............ph
-00000020: 6179 6573 2d30 2e30 2e30 2e64 6973 742d  ayes-0.0.0.dist-
-00000030: 696e 666f 2f4d 4554 4144 4154 413d ccb1  info/METADATA=..
-00000040: 0ec2 300c 04d0 dd5f e11f 4844 1933 81e8  ..0...._..HD.3..
-00000050: c002 42aa c46e 51b7 8d14 3ba5 7190 f87b  ..B..nQ...;.q..{
-00000060: 3254 e8b6 7ba7 bbb1 d148 46ee c95b 8959  2T..{....HF..[.Y
-00000070: 031e 7d07 7712 0eb8 2ef4 e502 7f39 f816  ..}.w........9..
-00000080: b866 61b7 d2dc 0670 aeb6 e42d e040 827d  .fa....p...-.@.}
-00000090: 9da6 c869 dc4b c742 3105 2c24 7edc e9f4  ...i.K.B1.,$~...
-000000a0: aea4 16b5 56f1 af2c 7049 544a 6cd4 2e7a  ....V..,pITJl..z
-000000b0: fe70 caab b01a 0e46 560b 8680 1d3a 7c24  .p.....FV....:|$
-000000c0: 528d 3a03 fc00 504b 0304 1400 0000 0800  R.:...PK........
-000000d0: ce50 be56 a1a5 31ee 5c00 0000 5c00 0000  .P.V..1.\...\...
-000000e0: 1c00 0000 7068 6179 6573 2d30 2e30 2e30  ....phayes-0.0.0
-000000f0: 2e64 6973 742d 696e 666f 2f57 4845 454c  .dist-info/WHEEL
-00000100: 0bcf 484d cdd1 0d4b 2d2a cecc cfb3 5230  ..HM...K-*....R0
-00000110: d433 e072 4fcd 4b2d 4a2c c92f b252 484a  .3.rO.K-J,./.RHJ
-00000120: c92c 2e89 2f07 a951 d030 d033 b6d0 33d1  .,../..Q.0.3..3.
-00000130: e40a cacf 2fd1 f52c d60d 282d 4acd c94c  ..../..,..(-J..L
-00000140: b252 2829 2a4d e50a 494c b752 28a8 34d6  .R()*M..IL.R(.4.
-00000150: cdcb cf4b d54d ccab e4e2 0200 504b 0304  ...K.M......PK..
-00000160: 1400 0000 0800 ce50 be56 9306 d732 0300  .......P.V...2..
-00000170: 0000 0100 0000 2400 0000 7068 6179 6573  ......$...phayes
-00000180: 2d30 2e30 2e30 2e64 6973 742d 696e 666f  -0.0.0.dist-info
-00000190: 2f74 6f70 5f6c 6576 656c 2e74 7874 e302  /top_level.txt..
-000001a0: 0050 4b03 0414 0000 0008 00ce 50be 5628  .PK.........P.V(
-000001b0: 873f 7acb 0000 0024 0100 001d 0000 0070  .?z....$.......p
-000001c0: 6861 7965 732d 302e 302e 302e 6469 7374  hayes-0.0.0.dist
-000001d0: 2d69 6e66 6f2f 5245 434f 5244 75cc 4157  -info/RECORDu.AW
-000001e0: 8230 0000 e0bb bf65 585b 1079 e830 dc1c  .0.....eX[.y.0..
-000001f0: 2f24 1249 1e5d f664 8ca0 090c b7d0 faf5  /$.I.].d........
-00000200: bd0e def4 7df7 4f37 fb1f 699c fbf9 bfaa  ....}.O7..i.....
-00000210: 35d6 69fb 7ab8 8b69 8609 ce30 30cd 1e79  5.i.z..i...00..y
-00000220: 8fcf bb00 25ad f7a4 2a16 7f6d 1691 a108  ....%...*..m....
-00000230: f3a8 cef9 2414 267c 2c09 1e3b a8e8 fb76  ....$.&|,..;...v
-00000240: 8a01 f41f 66fa 7a9b 8794 ae2f 273a 491d  ....f.z..../':I.
-00000250: c35e b964 ebca 952e 8e39 ccb2 f14d 0cec  .^.d.....9...M..
-00000260: b50e 9b26 e1ad d7b9 2269 bb72 000b 74ab  ...&...."i.r..t.
-00000270: b483 e607 39c9 c3dc 9eed a5c6 a50e 99f8  ....9...........
-00000280: 5c97 8e4a cd0b eb4f 2baa acf2 bf7f f547  \..J...O+......G
-00000290: b214 41e1 bb4e 1154 c768 c70c 80b7 e694  ..A..N.T.h......
-000002a0: 2e93 9400 30fb 0350 4b01 0214 0314 0000  ....0..PK.......
-000002b0: 0008 00ce 50be 567c 7283 bd89 0000 00ad  ....P.V|r.......
-000002c0: 0000 001f 0000 0000 0000 0000 0000 00a4  ................
-000002d0: 8100 0000 0070 6861 7965 732d 302e 302e  .....phayes-0.0.
-000002e0: 302e 6469 7374 2d69 6e66 6f2f 4d45 5441  0.dist-info/META
-000002f0: 4441 5441 504b 0102 1403 1400 0000 0800  DATAPK..........
-00000300: ce50 be56 a1a5 31ee 5c00 0000 5c00 0000  .P.V..1.\...\...
-00000310: 1c00 0000 0000 0000 0000 0000 a481 c600  ................
-00000320: 0000 7068 6179 6573 2d30 2e30 2e30 2e64  ..phayes-0.0.0.d
-00000330: 6973 742d 696e 666f 2f57 4845 454c 504b  ist-info/WHEELPK
-00000340: 0102 1403 1400 0000 0800 ce50 be56 9306  ...........P.V..
-00000350: d732 0300 0000 0100 0000 2400 0000 0000  .2........$.....
-00000360: 0000 0000 0000 a481 5c01 0000 7068 6179  ........\...phay
-00000370: 6573 2d30 2e30 2e30 2e64 6973 742d 696e  es-0.0.0.dist-in
-00000380: 666f 2f74 6f70 5f6c 6576 656c 2e74 7874  fo/top_level.txt
-00000390: 504b 0102 1403 1400 0000 0800 ce50 be56  PK...........P.V
-000003a0: 2887 3f7a cb00 0000 2401 0000 1d00 0000  (.?z....$.......
-000003b0: 0000 0000 0000 0000 b401 a101 0000 7068  ..............ph
-000003c0: 6179 6573 2d30 2e30 2e30 2e64 6973 742d  ayes-0.0.0.dist-
-000003d0: 696e 666f 2f52 4543 4f52 4450 4b05 0600  info/RECORDPK...
-000003e0: 0000 0004 0004 0034 0100 00a7 0200 0000  .......4........
-000003f0: 00                                       .
+00000000: 1f8b 0808 b5cb 7564 02ff 7068 6179 6573  ......ud..phayes
+00000010: 2d30 2e30 2e31 2e74 6172 00ed 9bdb 6e9b  -0.0.1.tar....n.
+00000020: 4010 867d cd53 ec1d ad54 c39e c0ae 254b  @..}.S...T....%K
+00000030: a99c b6a9 d226 69ad f626 8aac 8d59 6314  .....&i..&...Yc.
+00000040: 4e85 258a dfbe 6bb0 923a 3e54 5103 3930  N.%...k..:>TQ.90
+00000050: ff0d 30bb c692 d9f9 bf1d 34b6 6ccb 3e38  ..0.......4.l.>8
+00000060: 1337 4752 7832 ebd4 225c 69d7 1163 c6ee  .7GRx2.."\i..c..
+00000070: ce97 7182 2921 1d74 d369 4045 ae44 a6bf  ..q.)!.t.i@E.D..
+00000080: bed3 4ed1 1e8a 5410 c921 71fb 0ee7 84bb  ..N...T..!q.....
+00000090: c472 489f 5366 7440 af5f e95c 2c64 dec5  .rH.Sft@._.\,d..
+000000a0: 16b6 88dd a92f ff7b 8e53 1ddd ea88 295f  ...../.{.S....)_
+000000b0: cb79 c239 7318 775c d7d5 f94f a90e 21a7  .y.9s.w\...O..!.
+000000c0: c9fc cf45 e479 deee 797a da6c f6fa 9ebf  ...E.y..yz.l....
+000000d0: f52c fc9f 6ffa 3f05 ff6f c4ff fb5b fd9f  .,..o.?..o...[..
+000000e0: f6df 0300 5ae7 ff67 c79f bb5f 4e3e 9dd6  ....Z..g..._N>..
+000000f0: 90ff 2ee7 3bfd 9f61 76cf ff19 ede9 fd1f  ....;..av.......
+00000100: 6e32 ff5b eaff dfa4 129e 50a2 fb4b 6679  n2.[......P..Kfy
+00000110: 90c4 0344 2d62 9c88 480e 50b5 368c db91  ...D-b..H.P.6...
+00000120: 7291 1847 4924 bba9 f0f5 84b9 5269 3eb0  r..GI$......Ri>.
+00000130: 6d3f 50f3 e2d2 9a26 913d fa3e fa6a 7c28  m?P....&.=.>.j|(
+00000140: d43c c906 682c 2274 58cc 6681 0cbd 55b0  .<..h,"tX.f...U.
+00000150: 2b23 1184 03a4 7f6e cb5b 0d1d fc2e 44ac  +#.....n.[....D.
+00000160: 82b8 28a2 e53d 8c51 28f2 3cd0 43fa 1687  ..(..=.Q(.<.C...
+00000170: f25a 8649 1ac9 58a1 b112 aac8 d160 8008  .Z.I..X......`..
+00000180: eaa2 b350 c471 10fb 6053 2f9f ff50 ff3d  ...P.q..`S/..P.=
+00000190: b3fa 0f53 07f2 aa75 fcaf 2e2c e9fb dd20  ...S...u...,... 
+000001a0: 9e25 f623 e6ff c3ea 3f87 b80c eabf d6f8  .%.#....?.......
+000001b0: 3f75 37fd 9f81 ff37 e2ff 74d3 ff31 583f  ?u7....7..t..1X?
+000001c0: f8ff d2ff 1fa9 1e7c 58fd a7c7 894b 1d06  .......|X....K..
+000001d0: f51f d47f 50ff 01ff 81ff c07f d093 f07f  ....P...........
+000001e0: 7cfa f3c7 e8e3 d852 37aa 4efe d3b5 fa6f  |......R7.N....o
+000001f0: c9ff 1e66 2ef0 bf09 e552 15a9 952e 8c5d  ...f.....R.....]
+00000200: 7b3f 63cf a2d8 18f3 642a 634f c6d3 c524  {?c.....d*cO...$
+00000210: 0ce2 ab7c eb24 95a4 9370 89f5 ff5d 5720  ...|.$...p...]W 
+00000220: e03f f01f f80f aa89 ffdb ecbc 06fe 634c  .?............cL
+00000230: d6f9 4f09 6518 f8df 8420 d581 ffc0 7fe0  ..O.e.... ......
+00000240: 3ff0 1ff8 6fd7 54a9 3d98 ffa4 d7c3 f0fe  ?...o.T.=.......
+00000250: 1ff8 0f6a 07ff a1ff fbe9 f8bf bdff 9bf7  ...j............
+00000260: 3134 80b5 8eff d5cb e0e9 cc7f fcfc dfcb  14..............
+00000270: 7fee deeb ffe2 da00 80ff 4de8 5c6f f626  ..........M.\o.&
+00000280: cbcd de85 a184 3fb9 2c82 d043 4354 5e78  ......?.,..CCT^x
+00000290: 4249 7d8e 0d70 02e0 3fd4 ffad a8ff 29e3  BI}..p..?.....).
+000002a0: 50ff b79b ffe9 a286 fcdf c77f eede f5ff  P...............
+000002b0: 314a 97ff ffea 610a fc6f 42b3 2c89 50f9  1J....a..oB.,.P.
+000002c0: dc55 9284 390a a234 c954 1531 8cf2 f0c6  .U..9..4.T.1....
+000002d0: 405a b1d0 2661 56cb c57c 5786 aeab c6c0  @Z..&aV..|W.....
+000002e0: a159 ae9e 55d0 93f9 340b 5255 0eac 6261  .Y..U...4.RU..ba
+000002f0: 12eb ddc4 9681 220b 87e6 8e2e c2d5 1451  ......"........Q
+00000300: b60d 0ecd bf7b 09d7 8626 6547 e1d0 dcd3  .....{...&eG....
+00000310: 51b8 9a9f 8ae9 95f0 653e 3cbf a802 d3db  Q.......e><.....
+00000320: 4643 1d33 ffdd 6a68 eacf bd05 7304 8140  FC.3..jh....s..@
+00000330: 2010 0804 0281 402f 537f 000e 5ac1 8700   .....@/S...Z...
+00000340: 5000 00                                  P..
```

## Comparing `tmp/phayes-0.0.0-py3-none-any.whl.zip` & `tmp/phayes-0.0.1.tar.gz`

```diff
@@ -1,64 +1,53 @@
-00000000: 504b 0304 1400 0000 0800 ce50 be56 7c72  PK.........P.V|r
-00000010: 83bd 8900 0000 ad00 0000 1f00 0000 7068  ..............ph
-00000020: 6179 6573 2d30 2e30 2e30 2e64 6973 742d  ayes-0.0.0.dist-
-00000030: 696e 666f 2f4d 4554 4144 4154 413d ccb1  info/METADATA=..
-00000040: 0ec2 300c 04d0 dd5f e11f 4844 1933 81e8  ..0...._..HD.3..
-00000050: c002 42aa c46e 51b7 8d14 3ba5 7190 f87b  ..B..nQ...;.q..{
-00000060: 3254 e8b6 7ba7 bbb1 d148 46ee c95b 8959  2T..{....HF..[.Y
-00000070: 031e 7d07 7712 0eb8 2ef4 e502 7f39 f816  ..}.w........9..
-00000080: b866 61b7 d2dc 0670 aeb6 e42d e040 827d  .fa....p...-.@.}
-00000090: 9da6 c869 dc4b c742 3105 2c24 7edc e9f4  ...i.K.B1.,$~...
-000000a0: aea4 16b5 56f1 af2c 7049 544a 6cd4 2e7a  ....V..,pITJl..z
-000000b0: fe70 caab b01a 0e46 560b 8680 1d3a 7c24  .p.....FV....:|$
-000000c0: 528d 3a03 fc00 504b 0304 1400 0000 0800  R.:...PK........
-000000d0: ce50 be56 a1a5 31ee 5c00 0000 5c00 0000  .P.V..1.\...\...
-000000e0: 1c00 0000 7068 6179 6573 2d30 2e30 2e30  ....phayes-0.0.0
-000000f0: 2e64 6973 742d 696e 666f 2f57 4845 454c  .dist-info/WHEEL
-00000100: 0bcf 484d cdd1 0d4b 2d2a cecc cfb3 5230  ..HM...K-*....R0
-00000110: d433 e072 4fcd 4b2d 4a2c c92f b252 484a  .3.rO.K-J,./.RHJ
-00000120: c92c 2e89 2f07 a951 d030 d033 b6d0 33d1  .,../..Q.0.3..3.
-00000130: e40a cacf 2fd1 f52c d60d 282d 4acd c94c  ..../..,..(-J..L
-00000140: b252 2829 2a4d e50a 494c b752 28a8 34d6  .R()*M..IL.R(.4.
-00000150: cdcb cf4b d54d ccab e4e2 0200 504b 0304  ...K.M......PK..
-00000160: 1400 0000 0800 ce50 be56 9306 d732 0300  .......P.V...2..
-00000170: 0000 0100 0000 2400 0000 7068 6179 6573  ......$...phayes
-00000180: 2d30 2e30 2e30 2e64 6973 742d 696e 666f  -0.0.0.dist-info
-00000190: 2f74 6f70 5f6c 6576 656c 2e74 7874 e302  /top_level.txt..
-000001a0: 0050 4b03 0414 0000 0008 00ce 50be 5628  .PK.........P.V(
-000001b0: 873f 7acb 0000 0024 0100 001d 0000 0070  .?z....$.......p
-000001c0: 6861 7965 732d 302e 302e 302e 6469 7374  hayes-0.0.0.dist
-000001d0: 2d69 6e66 6f2f 5245 434f 5244 75cc 4157  -info/RECORDu.AW
-000001e0: 8230 0000 e0bb bf65 585b 1079 e830 dc1c  .0.....eX[.y.0..
-000001f0: 2f24 1249 1e5d f664 8ca0 090c b7d0 faf5  /$.I.].d........
-00000200: bd0e def4 7df7 4f37 fb1f 699c fbf9 bfaa  ....}.O7..i.....
-00000210: 35d6 69fb 7ab8 8b69 8609 ce30 30cd 1e79  5.i.z..i...00..y
-00000220: 8fcf bb00 25ad f7a4 2a16 7f6d 1691 a108  ....%...*..m....
-00000230: f3a8 cef9 2414 267c 2c09 1e3b a8e8 fb76  ....$.&|,..;...v
-00000240: 8a01 f41f 66fa 7a9b 8794 ae2f 273a 491d  ....f.z..../':I.
-00000250: c35e b964 ebca 952e 8e39 ccb2 f14d 0cec  .^.d.....9...M..
-00000260: b50e 9b26 e1ad d7b9 2269 bb72 000b 74ab  ...&...."i.r..t.
-00000270: b483 e607 39c9 c3dc 9eed a5c6 a50e 99f8  ....9...........
-00000280: 5c97 8e4a cd0b eb4f 2baa acf2 bf7f f547  \..J...O+......G
-00000290: b214 41e1 bb4e 1154 c768 c70c 80b7 e694  ..A..N.T.h......
-000002a0: 2e93 9400 30fb 0350 4b01 0214 0314 0000  ....0..PK.......
-000002b0: 0008 00ce 50be 567c 7283 bd89 0000 00ad  ....P.V|r.......
-000002c0: 0000 001f 0000 0000 0000 0000 0000 00a4  ................
-000002d0: 8100 0000 0070 6861 7965 732d 302e 302e  .....phayes-0.0.
-000002e0: 302e 6469 7374 2d69 6e66 6f2f 4d45 5441  0.dist-info/META
-000002f0: 4441 5441 504b 0102 1403 1400 0000 0800  DATAPK..........
-00000300: ce50 be56 a1a5 31ee 5c00 0000 5c00 0000  .P.V..1.\...\...
-00000310: 1c00 0000 0000 0000 0000 0000 a481 c600  ................
-00000320: 0000 7068 6179 6573 2d30 2e30 2e30 2e64  ..phayes-0.0.0.d
-00000330: 6973 742d 696e 666f 2f57 4845 454c 504b  ist-info/WHEELPK
-00000340: 0102 1403 1400 0000 0800 ce50 be56 9306  ...........P.V..
-00000350: d732 0300 0000 0100 0000 2400 0000 0000  .2........$.....
-00000360: 0000 0000 0000 a481 5c01 0000 7068 6179  ........\...phay
-00000370: 6573 2d30 2e30 2e30 2e64 6973 742d 696e  es-0.0.0.dist-in
-00000380: 666f 2f74 6f70 5f6c 6576 656c 2e74 7874  fo/top_level.txt
-00000390: 504b 0102 1403 1400 0000 0800 ce50 be56  PK...........P.V
-000003a0: 2887 3f7a cb00 0000 2401 0000 1d00 0000  (.?z....$.......
-000003b0: 0000 0000 0000 0000 b401 a101 0000 7068  ..............ph
-000003c0: 6179 6573 2d30 2e30 2e30 2e64 6973 742d  ayes-0.0.0.dist-
-000003d0: 696e 666f 2f52 4543 4f52 4450 4b05 0600  info/RECORDPK...
-000003e0: 0000 0004 0004 0034 0100 00a7 0200 0000  .......4........
-000003f0: 00                                       .
+00000000: 1f8b 0808 b5cb 7564 02ff 7068 6179 6573  ......ud..phayes
+00000010: 2d30 2e30 2e31 2e74 6172 00ed 9bdb 6e9b  -0.0.1.tar....n.
+00000020: 4010 867d cd53 ec1d ad54 c39e c0ae 254b  @..}.S...T....%K
+00000030: a99c b6a9 d226 69ad f626 8aac 8d59 6314  .....&i..&...Yc.
+00000040: 4e85 258a dfbe 6bb0 923a 3e54 5103 3930  N.%...k..:>TQ.90
+00000050: ff0d 30bb c692 d9f9 bf1d 34b6 6ccb 3e38  ..0.......4.l.>8
+00000060: 1337 4752 7832 ebd4 225c 69d7 1163 c6ee  .7GRx2.."\i..c..
+00000070: ce97 7182 2921 1d74 d369 4045 ae44 a6bf  ..q.)!.t.i@E.D..
+00000080: bed3 4ed1 1e8a 5410 c921 71fb 0ee7 84bb  ..N...T..!q.....
+00000090: c472 489f 5366 7440 af5f e95c 2c64 dec5  .rH.Sft@._.\,d..
+000000a0: 16b6 88dd a92f ff7b 8e53 1ddd ea88 295f  ...../.{.S....)_
+000000b0: cb79 c239 7318 775c d7d5 f94f a90e 21a7  .y.9s.w\...O..!.
+000000c0: c9fc cf45 e479 deee 797a da6c f6fa 9ebf  ...E.y..yz.l....
+000000d0: f52c fc9f 6ffa 3f05 ff6f c4ff fb5b fd9f  .,..o.?..o...[..
+000000e0: f6df 0300 5ae7 ff67 c79f bb5f 4e3e 9dd6  ....Z..g..._N>..
+000000f0: 90ff 2ee7 3bfd 9f61 76cf ff19 ede9 fd1f  ....;..av.......
+00000100: 6e32 ff5b eaff dfa4 129e 50a2 fb4b 6679  n2.[......P..Kfy
+00000110: 90c4 0344 2d62 9c88 480e 50b5 368c db91  ...D-b..H.P.6...
+00000120: 7291 1847 4924 bba9 f0f5 84b9 5269 3eb0  r..GI$......Ri>.
+00000130: 6d3f 50f3 e2d2 9a26 913d fa3e fa6a 7c28  m?P....&.=.>.j|(
+00000140: d43c c906 682c 2274 58cc 6681 0cbd 55b0  .<..h,"tX.f...U.
+00000150: 2b23 1184 03a4 7f6e cb5b 0d1d fc2e 44ac  +#.....n.[....D.
+00000160: 82b8 28a2 e53d 8c51 28f2 3cd0 43fa 1687  ..(..=.Q(.<.C...
+00000170: f25a 8649 1ac9 58a1 b112 aac8 d160 8008  .Z.I..X......`..
+00000180: eaa2 b350 c471 10fb 6053 2f9f ff50 ff3d  ...P.q..`S/..P.=
+00000190: b3fa 0f53 07f2 aa75 fcaf 2e2c e9fb dd20  ...S...u...,... 
+000001a0: 9e25 f623 e6ff c3ea 3f87 b80c eabf d6f8  .%.#....?.......
+000001b0: 3f75 37fd 9f81 ff37 e2ff 74d3 ff31 583f  ?u7....7..t..1X?
+000001c0: f8ff d2ff 1fa9 1e7c 58fd a7c7 894b 1d06  .......|X....K..
+000001d0: f51f d47f 50ff 01ff 81ff c07f d093 f07f  ....P...........
+000001e0: 7cfa f3c7 e8e3 d852 37aa 4efe d3b5 fa6f  |......R7.N....o
+000001f0: c9ff 1e66 2ef0 bf09 e552 15a9 952e 8c5d  ...f.....R.....]
+00000200: 7b3f 63cf a2d8 18f3 642a 634f c6d3 c524  {?c.....d*cO...$
+00000210: 0ce2 ab7c eb24 95a4 9370 89f5 ff5d 5720  ...|.$...p...]W 
+00000220: e03f f01f f80f aa89 ffdb ecbc 06fe 634c  .?............cL
+00000230: d6f9 4f09 6518 f8df 8420 d581 ffc0 7fe0  ..O.e.... ......
+00000240: 3ff0 1ff8 6fd7 54a9 3d98 ffa4 d7c3 f0fe  ?...o.T.=.......
+00000250: 1ff8 0f6a 07ff a1ff fbe9 f8bf bdff 9bf7  ...j............
+00000260: 3134 80b5 8eff d5cb e0e9 cc7f fcfc dfcb  14..............
+00000270: 7fee deeb ffe2 da00 80ff 4de8 5c6f f626  ..........M.\o.&
+00000280: cbcd de85 a184 3fb9 2c82 d043 4354 5e78  ......?.,..CCT^x
+00000290: 4249 7d8e 0d70 02e0 3fd4 ffad a8ff 29e3  BI}..p..?.....).
+000002a0: 50ff b79b ffe9 a286 fcdf c77f eede f5ff  P...............
+000002b0: 314a 97ff ffea 610a fc6f 42b3 2c89 50f9  1J....a..oB.,.P.
+000002c0: dc55 9284 390a a234 c954 1531 8cf2 f0c6  .U..9..4.T.1....
+000002d0: 405a b1d0 2661 56cb c57c 5786 aeab c6c0  @Z..&aV..|W.....
+000002e0: a159 ae9e 55d0 93f9 340b 5255 0eac 6261  .Y..U...4.RU..ba
+000002f0: 12eb ddc4 9681 220b 87e6 8e2e c2d5 1451  ......"........Q
+00000300: b60d 0ecd bf7b 09d7 8626 6547 e1d0 dcd3  .....{...&eG....
+00000310: 51b8 9a9f 8ae9 95f0 653e 3cbf a802 d3db  Q.......e><.....
+00000320: 4643 1d33 ffdd 6a68 eacf bd05 7304 8140  FC.3..jh....s..@
+00000330: 2010 0804 0281 402f 537f 000e 5ac1 8700   .....@/S...Z...
+00000340: 5000 00                                  P..
```
