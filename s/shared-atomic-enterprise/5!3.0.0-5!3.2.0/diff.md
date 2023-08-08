# Comparing `tmp/shared_atomic_enterprise-5!3.0.0-py39-none-win_amd64.whl.zip` & `tmp/shared_atomic_enterprise-5!3.2.0-pp39-none-win_amd64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,22 +1,22 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   2746532 (000000000029E8A4h)
-  Actual end-cent-dir record offset:       2746510 (000000000029E88Eh)
-  Expected end-cent-dir record offset:     2746510 (000000000029E88Eh)
+  Zip archive file size:                   6251997 (00000000005F65DDh)
+  Actual end-cent-dir record offset:       6251975 (00000000005F65C7h)
+  Expected end-cent-dir record offset:     6251975 (00000000005F65C7h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 37 entries.
-  The central directory is 3804 (0000000000000EDCh) bytes long,
+  central directory contains 47 entries.
+  The central directory is 4875 (000000000000130Bh) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 2742706 (000000000029D9B2h).
+  is 6247100 (00000000005F52BCh).
 
 
 Central directory entry #1:
 ---------------------------
 
   shared_atomic/
 
@@ -25,58 +25,58 @@
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             14 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (10 hex):                dir 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 164 bytes of NT security descriptor data.
+    The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  shared_atomic/atomic_activation.cp39-win_amd64.pyd
+  shared_atomic/atomic_activation.pypy39-pp73-win_amd64.pyd
 
   offset of local header from start of archive:   158
                                                   (000000000000009Eh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:01:06
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:01:06 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:01:06 UTC
-  32-bit CRC value (hex):                         4d7d7ab4
-  compressed size:                                456237 bytes
-  uncompressed size:                              1125376 bytes
-  length of filename:                             50 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:17:42
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:17:42 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:17:42 UTC
+  32-bit CRC value (hex):                         2d4b67c3
+  compressed size:                                163984 bytes
+  uncompressed size:                              412672 bytes
+  length of filename:                             57 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -87,33 +87,33 @@
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  shared_atomic/atomic_async_activation_check.cp39-win_amd64.pyd
+  shared_atomic/atomic_activation_cpython.cp39-win_amd64.pyd
 
-  offset of local header from start of archive:   456589
-                                                  (000000000006F78Dh) bytes
+  offset of local header from start of archive:   164343
+                                                  (00000000000281F7h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:01:34
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:01:33 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:01:33 UTC
-  32-bit CRC value (hex):                         1399bbfa
-  compressed size:                                222265 bytes
-  uncompressed size:                              548864 bytes
-  length of filename:                             62 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:16:14
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:16:13 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:16:13 UTC
+  32-bit CRC value (hex):                         32d75c34
+  compressed size:                                271365 bytes
+  uncompressed size:                              677376 bytes
+  length of filename:                             58 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -124,33 +124,33 @@
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  shared_atomic/atomic_boolfloat.cp39-win_amd64.pyd
+  shared_atomic/atomic_activation_cpython_wrapper.exe
 
-  offset of local header from start of archive:   679060
-                                                  (00000000000A5C94h) bytes
+  offset of local header from start of archive:   435910
+                                                  (000000000006A6C6h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:02:08
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:08 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:08 UTC
-  32-bit CRC value (hex):                         e698fbf3
-  compressed size:                                34828 bytes
-  uncompressed size:                              76800 bytes
-  length of filename:                             49 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:16:16
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:16:15 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:16:15 UTC
+  32-bit CRC value (hex):                         d28192d3
+  compressed size:                                7200 bytes
+  uncompressed size:                              15872 bytes
+  length of filename:                             51 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -161,29 +161,66 @@
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
+  shared_atomic/atomic_async_activation_check.pypy39-pp73-win_amd64.pyd
+
+  offset of local header from start of archive:   443305
+                                                  (000000000006C3A9h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Aug 7 20:18:34
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:18:33 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:18:33 UTC
+  32-bit CRC value (hex):                         e98b061d
+  compressed size:                                168878 bytes
+  uncompressed size:                              425984 bytes
+  length of filename:                             69 characters
+  length of extra field:                          17 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
+    The local extra field has 152 bytes of NT security descriptor data.
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access/creation times.
+
+  There is no file comment.
+
+Central directory entry #6:
+---------------------------
+
   shared_atomic/atomic_boolfloat.pxd
 
-  offset of local header from start of archive:   714081
-                                                  (00000000000AE561h) bytes
+  offset of local header from start of archive:   612396
+                                                  (000000000009582Ch) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 21 15:11:28
-  file last modified on (UT extra field modtime): 2023 May 21 07:11:27 local
-  file last modified on (UT extra field modtime): 2023 May 21 07:11:27 UTC
+  file last modified on (DOS date/time):          2023 Jul 17 16:41:40
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 local
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 UTC
   32-bit CRC value (hex):                         062e805b
   compressed size:                                202 bytes
   uncompressed size:                              696 bytes
   length of filename:                             34 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -195,36 +232,36 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #6:
+Central directory entry #7:
 ---------------------------
 
-  shared_atomic/atomic_bytearray.cp39-win_amd64.pyd
+  shared_atomic/atomic_boolfloat.pypy39-pp73-win_amd64.pyd
 
-  offset of local header from start of archive:   714461
-                                                  (00000000000AE6DDh) bytes
+  offset of local header from start of archive:   612776
+                                                  (00000000000959A8h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:02:22
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:21 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:21 UTC
-  32-bit CRC value (hex):                         584dd5b1
-  compressed size:                                63311 bytes
-  uncompressed size:                              171520 bytes
-  length of filename:                             49 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:19:44
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:19:43 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:19:43 UTC
+  32-bit CRC value (hex):                         470897fd
+  compressed size:                                27048 bytes
+  uncompressed size:                              61952 bytes
+  length of filename:                             56 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -232,32 +269,32 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #8:
 ---------------------------
 
   shared_atomic/atomic_bytearray.pxd
 
-  offset of local header from start of archive:   777965
-                                                  (00000000000BDEEDh) bytes
+  offset of local header from start of archive:   640024
+                                                  (000000000009C418h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jun 1 11:02:56
-  file last modified on (UT extra field modtime): 2023 Jun 1 03:02:56 local
-  file last modified on (UT extra field modtime): 2023 Jun 1 03:02:56 UTC
+  file last modified on (DOS date/time):          2023 Jul 17 16:41:38
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:38 local
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:38 UTC
   32-bit CRC value (hex):                         e7f8dc6e
   compressed size:                                421 bytes
   uncompressed size:                              2659 bytes
   length of filename:                             34 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -269,35 +306,72 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #8:
+Central directory entry #9:
+---------------------------
+
+  shared_atomic/atomic_bytearray.pypy39-pp73-win_amd64.pyd
+
+  offset of local header from start of archive:   640623
+                                                  (000000000009C66Fh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Aug 7 20:20:12
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:20:12 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:20:12 UTC
+  32-bit CRC value (hex):                         c4ea3a19
+  compressed size:                                51733 bytes
+  uncompressed size:                              139776 bytes
+  length of filename:                             56 characters
+  length of extra field:                          17 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
+    The local extra field has 152 bytes of NT security descriptor data.
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access/creation times.
+
+  There is no file comment.
+
+Central directory entry #10:
 ---------------------------
 
   shared_atomic/atomic_decryption_.cp39-win_amd64.pyd
 
-  offset of local header from start of archive:   778564
-                                                  (00000000000BE144h) bytes
+  offset of local header from start of archive:   692556
+                                                  (00000000000A914Ch) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:00:30
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:00:30 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:00:30 UTC
-  32-bit CRC value (hex):                         bde6fdb6
-  compressed size:                                13471 bytes
-  uncompressed size:                              34816 bytes
+  file last modified on (DOS date/time):          2023 Aug 7 20:15:52
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:15:52 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:15:52 UTC
+  32-bit CRC value (hex):                         6c1037c3
+  compressed size:                                13700 bytes
+  uncompressed size:                              35328 bytes
   length of filename:                             51 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -306,36 +380,36 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #9:
+Central directory entry #11:
 ---------------------------
 
-  shared_atomic/atomic_int.cp39-win_amd64.pyd
+  shared_atomic/atomic_decryption_.pypy39-pp73-win_amd64.pyd
 
-  offset of local header from start of archive:   792230
-                                                  (00000000000C16A6h) bytes
+  offset of local header from start of archive:   706451
+                                                  (00000000000AC793h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:02:30
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:30 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:30 UTC
-  32-bit CRC value (hex):                         63944e4a
-  compressed size:                                41641 bytes
-  uncompressed size:                              103424 bytes
-  length of filename:                             43 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:15:44
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:15:44 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:15:44 UTC
+  32-bit CRC value (hex):                         d7ad5409
+  compressed size:                                6783 bytes
+  uncompressed size:                              15872 bytes
+  length of filename:                             58 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -343,32 +417,32 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #10:
+Central directory entry #12:
 ---------------------------
 
   shared_atomic/atomic_int.pxd
 
-  offset of local header from start of archive:   834058
-                                                  (00000000000CBA0Ah) bytes
+  offset of local header from start of archive:   713436
+                                                  (00000000000AE2DCh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 18 13:56:40
-  file last modified on (UT extra field modtime): 2023 May 18 05:56:39 local
-  file last modified on (UT extra field modtime): 2023 May 18 05:56:39 UTC
+  file last modified on (DOS date/time):          2023 Jul 17 16:41:38
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:38 local
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:38 UTC
   32-bit CRC value (hex):                         21630272
   compressed size:                                351 bytes
   uncompressed size:                              2402 bytes
   length of filename:                             28 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -380,36 +454,36 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #11:
+Central directory entry #13:
 ---------------------------
 
-  shared_atomic/atomic_list.cp39-win_amd64.pyd
+  shared_atomic/atomic_int.pypy39-pp73-win_amd64.pyd
 
-  offset of local header from start of archive:   834581
-                                                  (00000000000CBC15h) bytes
+  offset of local header from start of archive:   713959
+                                                  (00000000000AE4E7h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:02:38
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:37 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:37 UTC
-  32-bit CRC value (hex):                         35dfefe3
-  compressed size:                                51815 bytes
-  uncompressed size:                              117760 bytes
-  length of filename:                             44 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:20:32
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:20:31 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:20:31 UTC
+  32-bit CRC value (hex):                         7b5e066c
+  compressed size:                                33358 bytes
+  uncompressed size:                              86016 bytes
+  length of filename:                             50 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -417,32 +491,32 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #12:
+Central directory entry #14:
 ---------------------------
 
   shared_atomic/atomic_list.pxd
 
-  offset of local header from start of archive:   886584
-                                                  (00000000000D8738h) bytes
+  offset of local header from start of archive:   747511
+                                                  (00000000000B67F7h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 29 10:01:02
-  file last modified on (UT extra field modtime): 2023 May 29 02:01:01 local
-  file last modified on (UT extra field modtime): 2023 May 29 02:01:01 UTC
+  file last modified on (DOS date/time):          2023 Jul 17 16:41:40
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 local
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 UTC
   32-bit CRC value (hex):                         28c11051
   compressed size:                                397 bytes
   uncompressed size:                              1408 bytes
   length of filename:                             29 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -454,36 +528,36 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #13:
+Central directory entry #15:
 ---------------------------
 
-  shared_atomic/atomic_object.cp39-win_amd64.pyd
+  shared_atomic/atomic_list.pypy39-pp73-win_amd64.pyd
 
-  offset of local header from start of archive:   887154
-                                                  (00000000000D8972h) bytes
+  offset of local header from start of archive:   748081
+                                                  (00000000000B6A31h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:01:58
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:01:57 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:01:57 UTC
-  32-bit CRC value (hex):                         4d731f32
-  compressed size:                                15125 bytes
-  uncompressed size:                              36352 bytes
-  length of filename:                             46 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:21:14
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:21:13 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:21:13 UTC
+  32-bit CRC value (hex):                         d0e2d49b
+  compressed size:                                39919 bytes
+  uncompressed size:                              94208 bytes
+  length of filename:                             51 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -491,32 +565,32 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #14:
+Central directory entry #16:
 ---------------------------
 
   shared_atomic/atomic_object.pxd
 
-  offset of local header from start of archive:   902469
-                                                  (00000000000DC545h) bytes
+  offset of local header from start of archive:   788195
+                                                  (00000000000C06E3h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 23 15:36:10
-  file last modified on (UT extra field modtime): 2023 May 23 07:36:10 local
-  file last modified on (UT extra field modtime): 2023 May 23 07:36:10 UTC
+  file last modified on (DOS date/time):          2023 Jul 17 16:41:40
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 local
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 UTC
   32-bit CRC value (hex):                         c01014fd
   compressed size:                                411 bytes
   uncompressed size:                              4093 bytes
   length of filename:                             31 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -528,36 +602,36 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #15:
+Central directory entry #17:
 ---------------------------
 
-  shared_atomic/atomic_object_backend.cp39-win_amd64.pyd
+  shared_atomic/atomic_object.pypy39-pp73-win_amd64.pyd
 
-  offset of local header from start of archive:   903055
-                                                  (00000000000DC78Fh) bytes
+  offset of local header from start of archive:   788781
+                                                  (00000000000C092Dh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:01:50
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:01:50 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:01:50 UTC
-  32-bit CRC value (hex):                         8ed93748
-  compressed size:                                91039 bytes
-  uncompressed size:                              244224 bytes
-  length of filename:                             54 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:19:26
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:19:26 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:19:26 UTC
+  32-bit CRC value (hex):                         e0a088e4
+  compressed size:                                14223 bytes
+  uncompressed size:                              34816 bytes
+  length of filename:                             53 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -565,32 +639,32 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #16:
+Central directory entry #18:
 ---------------------------
 
   shared_atomic/atomic_object_backend.pxd
 
-  offset of local header from start of archive:   994292
-                                                  (00000000000F2BF4h) bytes
+  offset of local header from start of archive:   803201
+                                                  (00000000000C4181h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jun 5 16:24:00
-  file last modified on (UT extra field modtime): 2023 Jun 5 08:24:00 local
-  file last modified on (UT extra field modtime): 2023 Jun 5 08:24:00 UTC
+  file last modified on (DOS date/time):          2023 Jul 17 16:41:40
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 local
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 UTC
   32-bit CRC value (hex):                         dceb602d
   compressed size:                                261 bytes
   uncompressed size:                              714 bytes
   length of filename:                             39 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -602,36 +676,36 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #17:
+Central directory entry #19:
 ---------------------------
 
-  shared_atomic/atomic_set.cp39-win_amd64.pyd
+  shared_atomic/atomic_object_backend.pypy39-pp73-win_amd64.pyd
 
-  offset of local header from start of archive:   994736
-                                                  (00000000000F2DB0h) bytes
+  offset of local header from start of archive:   803645
+                                                  (00000000000C433Dh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:02:46
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:45 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:45 UTC
-  32-bit CRC value (hex):                         72f8b80e
-  compressed size:                                51909 bytes
-  uncompressed size:                              117248 bytes
-  length of filename:                             43 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:19:14
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:19:14 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:19:14 UTC
+  32-bit CRC value (hex):                         a3336996
+  compressed size:                                75991 bytes
+  uncompressed size:                              209408 bytes
+  length of filename:                             61 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -639,32 +713,32 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #18:
+Central directory entry #20:
 ---------------------------
 
   shared_atomic/atomic_set.pxd
 
-  offset of local header from start of archive:   1046832
-                                                  (00000000000FF930h) bytes
+  offset of local header from start of archive:   879841
+                                                  (00000000000D6CE1h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 23 21:53:56
-  file last modified on (UT extra field modtime): 2023 May 23 13:53:55 local
-  file last modified on (UT extra field modtime): 2023 May 23 13:53:55 UTC
+  file last modified on (DOS date/time):          2023 Jul 17 16:41:40
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 local
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 UTC
   32-bit CRC value (hex):                         08589092
   compressed size:                                298 bytes
   uncompressed size:                              1108 bytes
   length of filename:                             28 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -676,36 +750,36 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #19:
+Central directory entry #21:
 ---------------------------
 
-  shared_atomic/atomic_shared_memory.cp39-win_amd64.pyd
+  shared_atomic/atomic_set.pypy39-pp73-win_amd64.pyd
 
-  offset of local header from start of archive:   1047302
-                                                  (00000000000FFB06h) bytes
+  offset of local header from start of archive:   880311
+                                                  (00000000000D6EB7h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:12
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:12 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:12 UTC
-  32-bit CRC value (hex):                         972e5b4f
-  compressed size:                                162191 bytes
-  uncompressed size:                              450048 bytes
-  length of filename:                             53 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:21:36
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:21:35 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:21:35 UTC
+  32-bit CRC value (hex):                         ec36d0f6
+  compressed size:                                39972 bytes
+  uncompressed size:                              93696 bytes
+  length of filename:                             50 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -713,32 +787,32 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #20:
+Central directory entry #22:
 ---------------------------
 
   shared_atomic/atomic_shared_memory.pxd
 
-  offset of local header from start of archive:   1209690
-                                                  (000000000012755Ah) bytes
+  offset of local header from start of archive:   920477
+                                                  (00000000000E0B9Dh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 29 10:17:58
-  file last modified on (UT extra field modtime): 2023 May 29 02:17:58 local
-  file last modified on (UT extra field modtime): 2023 May 29 02:17:58 UTC
+  file last modified on (DOS date/time):          2023 Jul 17 16:41:40
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 local
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 UTC
   32-bit CRC value (hex):                         eebeb83f
   compressed size:                                719 bytes
   uncompressed size:                              5193 bytes
   length of filename:                             38 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -750,36 +824,36 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #21:
+Central directory entry #23:
 ---------------------------
 
-  shared_atomic/atomic_string.cp39-win_amd64.pyd
+  shared_atomic/atomic_shared_memory.pypy39-pp73-win_amd64.pyd
 
-  offset of local header from start of archive:   1210591
-                                                  (00000000001278DFh) bytes
+  offset of local header from start of archive:   921378
+                                                  (00000000000E0F22h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:02:54
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:54 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:02:54 UTC
-  32-bit CRC value (hex):                         32b76678
-  compressed size:                                50413 bytes
-  uncompressed size:                              113152 bytes
-  length of filename:                             46 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:38
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:38 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:38 UTC
+  32-bit CRC value (hex):                         3de62c95
+  compressed size:                                144474 bytes
+  uncompressed size:                              411648 bytes
+  length of filename:                             60 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -787,32 +861,32 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #22:
+Central directory entry #24:
 ---------------------------
 
   shared_atomic/atomic_string.pxd
 
-  offset of local header from start of archive:   1261194
-                                                  (0000000000133E8Ah) bytes
+  offset of local header from start of archive:   1066056
+                                                  (0000000000104448h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jun 2 09:30:58
-  file last modified on (UT extra field modtime): 2023 Jun 2 01:30:58 local
-  file last modified on (UT extra field modtime): 2023 Jun 2 01:30:58 UTC
+  file last modified on (DOS date/time):          2023 Jul 17 16:41:40
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 local
+  file last modified on (UT extra field modtime): 2023 Jul 17 08:41:39 UTC
   32-bit CRC value (hex):                         74581693
   compressed size:                                296 bytes
   uncompressed size:                              1037 bytes
   length of filename:                             31 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -824,73 +898,109 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #23:
+Central directory entry #25:
 ---------------------------
 
-  shared_atomic/atomic_tools.py
+  shared_atomic/atomic_string.pypy39-pp73-win_amd64.pyd
 
-  offset of local header from start of archive:   1261665
-                                                  (0000000000134061h) bytes
+  offset of local header from start of archive:   1066527
+                                                  (000000000010461Fh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
-  32-bit CRC value (hex):                         446ec06d
-  compressed size:                                427 bytes
-  uncompressed size:                              893 bytes
-  length of filename:                             29 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:22:16
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:22:16 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:22:16 UTC
+  32-bit CRC value (hex):                         f4886d97
+  compressed size:                                39335 bytes
+  uncompressed size:                              90624 bytes
+  length of filename:                             53 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 164 bytes of NT security descriptor data.
+    The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #24:
+Central directory entry #26:
 ---------------------------
 
-  shared_atomic/atomic_uint.cp39-win_amd64.pyd
+  shared_atomic/atomic_tools.py
 
-  offset of local header from start of archive:   1262265
-                                                  (00000000001342B9h) bytes
+  offset of local header from start of archive:   1106059
+                                                  (000000000010E08Bh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 May 30 19:54:36
-  file last modified on (UT extra field modtime): 2023 May 30 11:54:35 local
-  file last modified on (UT extra field modtime): 2023 May 30 11:54:35 UTC
-  32-bit CRC value (hex):                         09e47146
-  compressed size:                                45587 bytes
-  uncompressed size:                              118272 bytes
-  length of filename:                             44 characters
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
+  32-bit CRC value (hex):                         8d990fa9
+  compressed size:                                408 bytes
+  uncompressed size:                              807 bytes
+  length of filename:                             29 characters
+  length of extra field:                          17 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
+    The local extra field has 152 bytes of NT security descriptor data.
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access/creation times.
+
+  There is no file comment.
+
+Central directory entry #27:
+---------------------------
+
+  shared_atomic/cpython_libs.zip
+
+  offset of local header from start of archive:   1106640
+                                                  (000000000010E2D0h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Aug 1 15:50:58
+  file last modified on (UT extra field modtime): 2023 Aug 1 07:50:57 local
+  file last modified on (UT extra field modtime): 2023 Aug 1 07:50:57 UTC
+  32-bit CRC value (hex):                         9b818705
+  compressed size:                                1117653 bytes
+  uncompressed size:                              1117653 bytes
+  length of filename:                             30 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
@@ -898,71 +1008,107 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #25:
+Central directory entry #28:
 ---------------------------
 
   shared_atomic/end_user_license_agreement.txt
 
-  offset of local header from start of archive:   1308040
-                                                  (000000000013F588h) bytes
+  offset of local header from start of archive:   2224467
+                                                  (000000000021F153h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
-  32-bit CRC value (hex):                         1e4b4415
-  compressed size:                                4959 bytes
-  uncompressed size:                              15099 bytes
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
+  32-bit CRC value (hex):                         1a5ee3e0
+  compressed size:                                15630 bytes
+  uncompressed size:                              49645 bytes
   length of filename:                             44 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 164 bytes of NT security descriptor data.
+    The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #26:
+Central directory entry #29:
+---------------------------
+
+  shared_atomic/lib/
+
+  offset of local header from start of archive:   2240285
+                                                  (0000000000222F1Dh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 Apr 4 12:29:26
+  file last modified on (UT extra field modtime): 2023 Apr 4 04:29:26 local
+  file last modified on (UT extra field modtime): 2023 Apr 4 04:29:26 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             18 characters
+  length of extra field:                          17 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
+    The local extra field has 152 bytes of NT security descriptor data.
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access/creation times.
+
+  There is no file comment.
+
+Central directory entry #30:
 ---------------------------
 
   shared_atomic/libdecryption.dll
 
-  offset of local header from start of archive:   1313187
-                                                  (00000000001409A3h) bytes
+  offset of local header from start of archive:   2240447
+                                                  (0000000000222FBFh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:00:26
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:00:25 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:00:25 UTC
-  32-bit CRC value (hex):                         79f91363
-  compressed size:                                1335872 bytes
+  file last modified on (DOS date/time):          2023 Aug 7 20:15:36
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:15:36 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:15:36 UTC
+  32-bit CRC value (hex):                         4d217c38
+  compressed size:                                1335871 bytes
   uncompressed size:                              3496448 bytes
   length of filename:                             31 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
@@ -972,34 +1118,34 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #27:
+Central directory entry #31:
 ---------------------------
 
   shared_atomic/libdecryption11.dll
 
-  offset of local header from start of archive:   2649234
-                                                  (0000000000286C92h) bytes
+  offset of local header from start of archive:   3576493
+                                                  (00000000003692ADh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:00:26
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:00:26 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:00:26 UTC
-  32-bit CRC value (hex):                         180fc3e7
-  compressed size:                                4012 bytes
+  file last modified on (DOS date/time):          2023 Aug 7 20:15:36
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:15:36 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:15:36 UTC
+  32-bit CRC value (hex):                         46ace242
+  compressed size:                                4011 bytes
   uncompressed size:                              9728 bytes
   length of filename:                             33 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
@@ -1009,215 +1155,437 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #28:
+Central directory entry #32:
+---------------------------
+
+  shared_atomic/python3.dll
+
+  offset of local header from start of archive:   3580681
+                                                  (000000000036A309h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2022 May 17 16:46:04
+  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 local
+  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 UTC
+  32-bit CRC value (hex):                         ae4f95ee
+  compressed size:                                20281 bytes
+  uncompressed size:                              61432 bytes
+  length of filename:                             25 characters
+  length of extra field:                          17 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
+    The local extra field has 152 bytes of NT security descriptor data.
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access/creation times.
+
+  There is no file comment.
+
+Central directory entry #33:
+---------------------------
+
+  shared_atomic/python39.dll
+
+  offset of local header from start of archive:   3601131
+                                                  (000000000036F2EBh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2022 May 17 16:46:04
+  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 local
+  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 UTC
+  32-bit CRC value (hex):                         85fa642a
+  compressed size:                                2008848 bytes
+  uncompressed size:                              4527096 bytes
+  length of filename:                             26 characters
+  length of extra field:                          17 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
+    The local extra field has 152 bytes of NT security descriptor data.
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access/creation times.
+
+  There is no file comment.
+
+Central directory entry #34:
 ---------------------------
 
   shared_atomic/readme.txt
 
-  offset of local header from start of archive:   2653423
-                                                  (0000000000287CEFh) bytes
+  offset of local header from start of archive:   5610149
+                                                  (0000000000559AA5h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
   32-bit CRC value (hex):                         ba5f87e5
   compressed size:                                370 bytes
   uncompressed size:                              622 bytes
   length of filename:                             24 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 164 bytes of NT security descriptor data.
+    The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #29:
+Central directory entry #35:
 ---------------------------
 
-  shared_atomic/setup.py
+  shared_atomic/select.pyd
 
-  offset of local header from start of archive:   2653961
-                                                  (0000000000287F09h) bytes
+  offset of local header from start of archive:   5610687
+                                                  (0000000000559CBFh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
-  32-bit CRC value (hex):                         d05a746c
-  compressed size:                                928 bytes
-  uncompressed size:                              2755 bytes
-  length of filename:                             22 characters
+  file last modified on (DOS date/time):          2022 May 17 16:46:02
+  file last modified on (UT extra field modtime): 2022 May 17 08:46:02 local
+  file last modified on (UT extra field modtime): 2022 May 17 08:46:02 UTC
+  32-bit CRC value (hex):                         dd7e6338
+  compressed size:                                17169 bytes
+  uncompressed size:                              30712 bytes
+  length of filename:                             24 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             text
+  apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 164 bytes of NT security descriptor data.
+    The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #30:
+Central directory entry #36:
+---------------------------
+
+  shared_atomic/unicodedata.pyd
+
+  offset of local header from start of archive:   5628024
+                                                  (000000000055E078h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2022 May 17 16:46:04
+  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 local
+  file last modified on (UT extra field modtime): 2022 May 17 08:46:04 UTC
+  32-bit CRC value (hex):                         bd6c26a1
+  compressed size:                                409871 bytes
+  uncompressed size:                              1123832 bytes
+  length of filename:                             29 characters
+  length of extra field:                          17 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
+    The local extra field has 152 bytes of NT security descriptor data.
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access/creation times.
+
+  There is no file comment.
+
+Central directory entry #37:
 ---------------------------
 
   shared_atomic/urwid_win_patch.py
 
-  offset of local header from start of archive:   2655055
-                                                  (000000000028834Fh) bytes
+  offset of local header from start of archive:   6038068
+                                                  (00000000005C2234h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
-  32-bit CRC value (hex):                         ecc3f14e
-  compressed size:                                1469 bytes
-  uncompressed size:                              4070 bytes
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
+  32-bit CRC value (hex):                         86741696
+  compressed size:                                1224 bytes
+  uncompressed size:                              3423 bytes
   length of filename:                             32 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 164 bytes of NT security descriptor data.
+    The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #31:
+Central directory entry #38:
 ---------------------------
 
   shared_atomic/_cffi_backend.cp39-win_amd64.pyd
 
-  offset of local header from start of archive:   2656700
-                                                  (00000000002889BCh) bytes
+  offset of local header from start of archive:   6039468
+                                                  (00000000005C27ACh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2022 Oct 24 17:28:50
-  file last modified on (UT extra field modtime): 2022 Oct 24 09:28:50 local
-  file last modified on (UT extra field modtime): 2022 Oct 24 09:28:50 UTC
+  file last modified on (DOS date/time):          2022 Oct 24 17:24:38
+  file last modified on (UT extra field modtime): 2022 Oct 24 09:24:38 local
+  file last modified on (UT extra field modtime): 2022 Oct 24 09:24:38 UTC
   32-bit CRC value (hex):                         8a34aa66
   compressed size:                                82369 bytes
   uncompressed size:                              183296 bytes
   length of filename:                             46 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 164 bytes of NT security descriptor data.
+    The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #32:
+Central directory entry #39:
+---------------------------
+
+  shared_atomic/_curses.cp39-win_amd64.pyd
+
+  offset of local header from start of archive:   6122027
+                                                  (00000000005D6A2Bh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2022 Nov 18 15:48:24
+  file last modified on (UT extra field modtime): 2022 Nov 18 07:48:23 local
+  file last modified on (UT extra field modtime): 2022 Nov 18 07:48:23 UTC
+  32-bit CRC value (hex):                         13bd25c0
+  compressed size:                                70392 bytes
+  uncompressed size:                              171008 bytes
+  length of filename:                             40 characters
+  length of extra field:                          17 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
+    The local extra field has 152 bytes of NT security descriptor data.
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access/creation times.
+
+  There is no file comment.
+
+Central directory entry #40:
+---------------------------
+
+  shared_atomic/_curses_panel.cp39-win_amd64.pyd
+
+  offset of local header from start of archive:   6192603
+                                                  (00000000005E7DDBh) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2022 Nov 18 15:48:24
+  file last modified on (UT extra field modtime): 2022 Nov 18 07:48:23 local
+  file last modified on (UT extra field modtime): 2022 Nov 18 07:48:23 UTC
+  32-bit CRC value (hex):                         9ae10466
+  compressed size:                                11882 bytes
+  uncompressed size:                              27648 bytes
+  length of filename:                             46 characters
+  length of extra field:                          17 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
+    The local extra field has 152 bytes of NT security descriptor data.
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access/creation times.
+
+  There is no file comment.
+
+Central directory entry #41:
+---------------------------
+
+  shared_atomic/_socket.pyd
+
+  offset of local header from start of archive:   6204675
+                                                  (00000000005EAD03h) bytes
+  file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   2.0
+  compression method:                             deflated
+  compression sub-type (deflation):               normal
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2022 May 17 16:46:02
+  file last modified on (UT extra field modtime): 2022 May 17 08:46:02 local
+  file last modified on (UT extra field modtime): 2022 May 17 08:46:02 UTC
+  32-bit CRC value (hex):                         56944ef3
+  compressed size:                                38791 bytes
+  uncompressed size:                              81912 bytes
+  length of filename:                             25 characters
+  length of extra field:                          17 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  non-MSDOS external file attributes:             000000 hex
+  MS-DOS file attributes (20 hex):                arc 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
+    The local extra field has 152 bytes of NT security descriptor data.
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access/creation times.
+
+  There is no file comment.
+
+Central directory entry #42:
 ---------------------------
 
   shared_atomic/__init__.py
 
-  offset of local header from start of archive:   2739259
-                                                  (000000000029CC3Bh) bytes
+  offset of local header from start of archive:   6243635
+                                                  (00000000005F4533h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             25 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
 
   The central-directory extra field contains:
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
-    The local extra field has 164 bytes of NT security descriptor data.
+    The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #33:
+Central directory entry #43:
 ---------------------------
 
-  shared_atomic_enterprise-5!3.0.0.dist-info/
+  shared_atomic_enterprise-5!3.2.0.dist-info/
 
-  offset of local header from start of archive:   2739428
-                                                  (000000000029CCE4h) bytes
+  offset of local header from start of archive:   6243804
+                                                  (00000000005F45DCh) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
   32-bit CRC value (hex):                         00000000
   compressed size:                                0 bytes
   uncompressed size:                              0 bytes
   length of filename:                             43 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -1229,35 +1597,35 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #34:
+Central directory entry #44:
 ---------------------------
 
-  shared_atomic_enterprise-5!3.0.0.dist-info/METADATA
+  shared_atomic_enterprise-5!3.2.0.dist-info/METADATA
 
-  offset of local header from start of archive:   2739615
-                                                  (000000000029CD9Fh) bytes
+  offset of local header from start of archive:   6243991
+                                                  (00000000005F4697h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
-  32-bit CRC value (hex):                         d7069c53
-  compressed size:                                1146 bytes
-  uncompressed size:                              2866 bytes
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
+  32-bit CRC value (hex):                         c0cd8c0a
+  compressed size:                                1158 bytes
+  uncompressed size:                              2981 bytes
   length of filename:                             51 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -1266,35 +1634,35 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #35:
+Central directory entry #45:
 ---------------------------
 
-  shared_atomic_enterprise-5!3.0.0.dist-info/RECORD
+  shared_atomic_enterprise-5!3.2.0.dist-info/RECORD
 
-  offset of local header from start of archive:   2740956
-                                                  (000000000029D2DCh) bytes
+  offset of local header from start of archive:   6245344
+                                                  (00000000005F4BE0h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
-  32-bit CRC value (hex):                         5ffc1c99
-  compressed size:                                1052 bytes
-  uncompressed size:                              1925 bytes
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
+  32-bit CRC value (hex):                         9a4dee88
+  compressed size:                                1058 bytes
+  uncompressed size:                              1982 bytes
   length of filename:                             49 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
   non-MSDOS external file attributes:             000000 hex
   MS-DOS file attributes (20 hex):                arc 
@@ -1303,31 +1671,31 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #36:
+Central directory entry #46:
 ---------------------------
 
-  shared_atomic_enterprise-5!3.0.0.dist-info/top_level.txt
+  shared_atomic_enterprise-5!3.2.0.dist-info/top_level.txt
 
-  offset of local header from start of archive:   2742201
-                                                  (000000000029D7B9h) bytes
+  offset of local header from start of archive:   6246595
+                                                  (00000000005F50C3h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
   32-bit CRC value (hex):                         3ae435d8
   compressed size:                                14 bytes
   uncompressed size:                              14 bytes
   length of filename:                             56 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
@@ -1339,32 +1707,32 @@
   - A subfield with ID 0x4453 (Security Descriptor) and 4 data bytes.
     The local extra field has 152 bytes of NT security descriptor data.
   - A subfield with ID 0x5455 (universal time) and 5 data bytes.
     The local extra field has UTC/GMT modification/access/creation times.
 
   There is no file comment.
 
-Central directory entry #37:
+Central directory entry #47:
 ---------------------------
 
-  shared_atomic_enterprise-5!3.0.0.dist-info/WHEEL
+  shared_atomic_enterprise-5!3.2.0.dist-info/WHEEL
 
-  offset of local header from start of archive:   2742415
-                                                  (000000000029D88Fh) bytes
+  offset of local header from start of archive:   6246809
+                                                  (00000000005F5199h) bytes
   file system or operating system of origin:      MS-DOS, OS/2 or NT FAT
   version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   1.0
   compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Jul 6 17:03:14
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 local
-  file last modified on (UT extra field modtime): 2023 Jul 6 09:03:13 UTC
-  32-bit CRC value (hex):                         7e3cc389
+  file last modified on (DOS date/time):          2023 Aug 7 20:23:40
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 local
+  file last modified on (UT extra field modtime): 2023 Aug 7 12:23:39 UTC
+  32-bit CRC value (hex):                         31fa862c
   compressed size:                                99 bytes
   uncompressed size:                              99 bytes
   length of filename:                             48 characters
   length of extra field:                          17 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             text
```

## zipnote {}

```diff
@@ -1,112 +1,142 @@
 Filename: shared_atomic/
 Comment: 
 
-Filename: shared_atomic/atomic_activation.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_activation.pypy39-pp73-win_amd64.pyd
 Comment: 
 
-Filename: shared_atomic/atomic_async_activation_check.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_activation_cpython.cp39-win_amd64.pyd
 Comment: 
 
-Filename: shared_atomic/atomic_boolfloat.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_activation_cpython_wrapper.exe
+Comment: 
+
+Filename: shared_atomic/atomic_async_activation_check.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_boolfloat.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_bytearray.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_boolfloat.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_bytearray.pxd
 Comment: 
 
+Filename: shared_atomic/atomic_bytearray.pypy39-pp73-win_amd64.pyd
+Comment: 
+
 Filename: shared_atomic/atomic_decryption_.cp39-win_amd64.pyd
 Comment: 
 
-Filename: shared_atomic/atomic_int.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_decryption_.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_int.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_list.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_int.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_list.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_object.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_list.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_object.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_object_backend.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_object.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_object_backend.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_set.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_object_backend.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_set.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_shared_memory.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_set.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_shared_memory.pxd
 Comment: 
 
-Filename: shared_atomic/atomic_string.cp39-win_amd64.pyd
+Filename: shared_atomic/atomic_shared_memory.pypy39-pp73-win_amd64.pyd
 Comment: 
 
 Filename: shared_atomic/atomic_string.pxd
 Comment: 
 
+Filename: shared_atomic/atomic_string.pypy39-pp73-win_amd64.pyd
+Comment: 
+
 Filename: shared_atomic/atomic_tools.py
 Comment: 
 
-Filename: shared_atomic/atomic_uint.cp39-win_amd64.pyd
+Filename: shared_atomic/cpython_libs.zip
 Comment: 
 
 Filename: shared_atomic/end_user_license_agreement.txt
 Comment: 
 
+Filename: shared_atomic/lib/
+Comment: 
+
 Filename: shared_atomic/libdecryption.dll
 Comment: 
 
 Filename: shared_atomic/libdecryption11.dll
 Comment: 
 
+Filename: shared_atomic/python3.dll
+Comment: 
+
+Filename: shared_atomic/python39.dll
+Comment: 
+
 Filename: shared_atomic/readme.txt
 Comment: 
 
-Filename: shared_atomic/setup.py
+Filename: shared_atomic/select.pyd
+Comment: 
+
+Filename: shared_atomic/unicodedata.pyd
 Comment: 
 
 Filename: shared_atomic/urwid_win_patch.py
 Comment: 
 
 Filename: shared_atomic/_cffi_backend.cp39-win_amd64.pyd
 Comment: 
 
+Filename: shared_atomic/_curses.cp39-win_amd64.pyd
+Comment: 
+
+Filename: shared_atomic/_curses_panel.cp39-win_amd64.pyd
+Comment: 
+
+Filename: shared_atomic/_socket.pyd
+Comment: 
+
 Filename: shared_atomic/__init__.py
 Comment: 
 
-Filename: shared_atomic_enterprise-5!3.0.0.dist-info/
+Filename: shared_atomic_enterprise-5!3.2.0.dist-info/
 Comment: 
 
-Filename: shared_atomic_enterprise-5!3.0.0.dist-info/METADATA
+Filename: shared_atomic_enterprise-5!3.2.0.dist-info/METADATA
 Comment: 
 
-Filename: shared_atomic_enterprise-5!3.0.0.dist-info/RECORD
+Filename: shared_atomic_enterprise-5!3.2.0.dist-info/RECORD
 Comment: 
 
-Filename: shared_atomic_enterprise-5!3.0.0.dist-info/top_level.txt
+Filename: shared_atomic_enterprise-5!3.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: shared_atomic_enterprise-5!3.0.0.dist-info/WHEEL
+Filename: shared_atomic_enterprise-5!3.2.0.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## shared_atomic/atomic_tools.py

```diff
@@ -1,32 +1,30 @@
 import sys
 from pathlib import Path
 importpath = str(Path(__file__).parent.parent)
 sys.path[0] = importpath
 import argparse
-from shared_atomic.atomic_activation import activation, modify_proxy
+from shared_atomic.atomic_activation import modify_proxy
 
 if sys.platform not in ('darwin', 'linux','win32'):
     raise NotImplementedError('Unsupported platform!')
 
 def test_activation():
     activation()
 
 
 if __name__ == "__main__":
 
     parser = argparse.ArgumentParser(description="user tools for Shared Atomic Enterprise")
     parser.add_argument('-a','--action',
-                        choices=['a','p'],
-                        help="a for activation, p for proxy setting",
+                        choices=['p'],
+                        help="p for proxy setting",
                         required=True,
                         dest='action')
     parsed = parser.parse_args()
-    if parsed.action == 'a':
-        activation()
 
-    elif parsed.action == 'p':
+    if parsed.action == 'p':
         modify_proxy()
     else:
         print("Invalid action!")
         exit()
```

## shared_atomic/end_user_license_agreement.txt

```diff
@@ -87,14 +87,519 @@
 The service agreement could be found at https://sharedatomic.top/enterprise_service.html
 
 20) Complete term:
 This EULA includs supplement terms and terms in the external links, because they are all components of this EULA.
 After installation and activation, licensee could still read it by restart the activation process, and click "Read End User Licence Agreement" Button
 
 21) Other authors:
+The embedded urwid_win_patch.py and code under urwid in cpython_libs.zip is under following GNU LESSER GENERAL PUBLIC LICENSE.
+
+              GNU LESSER GENERAL PUBLIC LICENSE
+                   Version 2.1, February 1999
+
+     Copyright (C) 1991, 1999 Free Software Foundation, Inc.
+     51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
+     Everyone is permitted to copy and distribute verbatim copies
+     of this license document, but changing it is not allowed.
+
+    [This is the first released version of the Lesser GPL.  It also counts
+     as the successor of the GNU Library Public License, version 2, hence
+     the version number 2.1.]
+
+                    Preamble
+
+      The licenses for most software are designed to take away your
+    freedom to share and change it.  By contrast, the GNU General Public
+    Licenses are intended to guarantee your freedom to share and change
+    free software--to make sure the software is free for all its users.
+
+      This license, the Lesser General Public License, applies to some
+    specially designated software packages--typically libraries--of the
+    Free Software Foundation and other authors who decide to use it.  You
+    can use it too, but we suggest you first think carefully about whether
+    this license or the ordinary General Public License is the better
+    strategy to use in any particular case, based on the explanations below.
+
+      When we speak of free software, we are referring to freedom of use,
+    not price.  Our General Public Licenses are designed to make sure that
+    you have the freedom to distribute copies of free software (and charge
+    for this service if you wish); that you receive source code or can get
+    it if you want it; that you can change the software and use pieces of
+    it in new free programs; and that you are informed that you can do
+    these things.
+
+      To protect your rights, we need to make restrictions that forbid
+    distributors to deny you these rights or to ask you to surrender these
+    rights.  These restrictions translate to certain responsibilities for
+    you if you distribute copies of the library or if you modify it.
+
+      For example, if you distribute copies of the library, whether gratis
+    or for a fee, you must give the recipients all the rights that we gave
+    you.  You must make sure that they, too, receive or can get the source
+    code.  If you link other code with the library, you must provide
+    complete object files to the recipients, so that they can relink them
+    with the library after making changes to the library and recompiling
+    it.  And you must show them these terms so they know their rights.
+
+      We protect your rights with a two-step method: (1) we copyright the
+    library, and (2) we offer you this license, which gives you legal
+    permission to copy, distribute and/or modify the library.
+
+      To protect each distributor, we want to make it very clear that
+    there is no warranty for the free library.  Also, if the library is
+    modified by someone else and passed on, the recipients should know
+    that what they have is not the original version, so that the original
+    author's reputation will not be affected by problems that might be
+    introduced by others.
+
+      Finally, software patents pose a constant threat to the existence of
+    any free program.  We wish to make sure that a company cannot
+    effectively restrict the users of a free program by obtaining a
+    restrictive license from a patent holder.  Therefore, we insist that
+    any patent license obtained for a version of the library must be
+    consistent with the full freedom of use specified in this license.
+
+      Most GNU software, including some libraries, is covered by the
+    ordinary GNU General Public License.  This license, the GNU Lesser
+    General Public License, applies to certain designated libraries, and
+    is quite different from the ordinary General Public License.  We use
+    this license for certain libraries in order to permit linking those
+    libraries into non-free programs.
+
+      When a program is linked with a library, whether statically or using
+    a shared library, the combination of the two is legally speaking a
+    combined work, a derivative of the original library.  The ordinary
+    General Public License therefore permits such linking only if the
+    entire combination fits its criteria of freedom.  The Lesser General
+    Public License permits more lax criteria for linking other code with
+    the library.
+
+      We call this license the "Lesser" General Public License because it
+    does Less to protect the user's freedom than the ordinary General
+    Public License.  It also provides other free software developers Less
+    of an advantage over competing non-free programs.  These disadvantages
+    are the reason we use the ordinary General Public License for many
+    libraries.  However, the Lesser license provides advantages in certain
+    special circumstances.
+
+      For example, on rare occasions, there may be a special need to
+    encourage the widest possible use of a certain library, so that it becomes
+    a de-facto standard.  To achieve this, non-free programs must be
+    allowed to use the library.  A more frequent case is that a free
+    library does the same job as widely used non-free libraries.  In this
+    case, there is little to gain by limiting the free library to free
+    software only, so we use the Lesser General Public License.
+
+      In other cases, permission to use a particular library in non-free
+    programs enables a greater number of people to use a large body of
+    free software.  For example, permission to use the GNU C Library in
+    non-free programs enables many more people to use the whole GNU
+    operating system, as well as its variant, the GNU/Linux operating
+    system.
+
+      Although the Lesser General Public License is Less protective of the
+    users' freedom, it does ensure that the user of a program that is
+    linked with the Library has the freedom and the wherewithal to run
+    that program using a modified version of the Library.
+
+      The precise terms and conditions for copying, distribution and
+    modification follow.  Pay close attention to the difference between a
+    "work based on the library" and a "work that uses the library".  The
+    former contains code derived from the library, whereas the latter must
+    be combined with the library in order to run.
+
+              GNU LESSER GENERAL PUBLIC LICENSE
+       TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+      0. This License Agreement applies to any software library or other
+    program which contains a notice placed by the copyright holder or
+    other authorized party saying it may be distributed under the terms of
+    this Lesser General Public License (also called "this License").
+    Each licensee is addressed as "you".
+
+      A "library" means a collection of software functions and/or data
+    prepared so as to be conveniently linked with application programs
+    (which use some of those functions and data) to form executables.
+
+      The "Library", below, refers to any such software library or work
+    which has been distributed under these terms.  A "work based on the
+    Library" means either the Library or any derivative work under
+    copyright law: that is to say, a work containing the Library or a
+    portion of it, either verbatim or with modifications and/or translated
+    straightforwardly into another language.  (Hereinafter, translation is
+    included without limitation in the term "modification".)
+
+      "Source code" for a work means the preferred form of the work for
+    making modifications to it.  For a library, complete source code means
+    all the source code for all modules it contains, plus any associated
+    interface definition files, plus the scripts used to control compilation
+    and installation of the library.
+
+      Activities other than copying, distribution and modification are not
+    covered by this License; they are outside its scope.  The act of
+    running a program using the Library is not restricted, and output from
+    such a program is covered only if its contents constitute a work based
+    on the Library (independent of the use of the Library in a tool for
+    writing it).  Whether that is true depends on what the Library does
+    and what the program that uses the Library does.
+
+      1. You may copy and distribute verbatim copies of the Library's
+    complete source code as you receive it, in any medium, provided that
+    you conspicuously and appropriately publish on each copy an
+    appropriate copyright notice and disclaimer of warranty; keep intact
+    all the notices that refer to this License and to the absence of any
+    warranty; and distribute a copy of this License along with the
+    Library.
+
+      You may charge a fee for the physical act of transferring a copy,
+    and you may at your option offer warranty protection in exchange for a
+    fee.
+
+      2. You may modify your copy or copies of the Library or any portion
+    of it, thus forming a work based on the Library, and copy and
+    distribute such modifications or work under the terms of Section 1
+    above, provided that you also meet all of these conditions:
+
+        a) The modified work must itself be a software library.
+
+        b) You must cause the files modified to carry prominent notices
+        stating that you changed the files and the date of any change.
+
+        c) You must cause the whole of the work to be licensed at no
+        charge to all third parties under the terms of this License.
+
+        d) If a facility in the modified Library refers to a function or a
+        table of data to be supplied by an application program that uses
+        the facility, other than as an argument passed when the facility
+        is invoked, then you must make a good faith effort to ensure that,
+        in the event an application does not supply such function or
+        table, the facility still operates, and performs whatever part of
+        its purpose remains meaningful.
+
+        (For example, a function in a library to compute square roots has
+        a purpose that is entirely well-defined independent of the
+        application.  Therefore, Subsection 2d requires that any
+        application-supplied function or table used by this function must
+        be optional: if the application does not supply it, the square
+        root function must still compute square roots.)
+
+    These requirements apply to the modified work as a whole.  If
+    identifiable sections of that work are not derived from the Library,
+    and can be reasonably considered independent and separate works in
+    themselves, then this License, and its terms, do not apply to those
+    sections when you distribute them as separate works.  But when you
+    distribute the same sections as part of a whole which is a work based
+    on the Library, the distribution of the whole must be on the terms of
+    this License, whose permissions for other licensees extend to the
+    entire whole, and thus to each and every part regardless of who wrote
+    it.
+
+    Thus, it is not the intent of this section to claim rights or contest
+    your rights to work written entirely by you; rather, the intent is to
+    exercise the right to control the distribution of derivative or
+    collective works based on the Library.
+
+    In addition, mere aggregation of another work not based on the Library
+    with the Library (or with a work based on the Library) on a volume of
+    a storage or distribution medium does not bring the other work under
+    the scope of this License.
+
+      3. You may opt to apply the terms of the ordinary GNU General Public
+    License instead of this License to a given copy of the Library.  To do
+    this, you must alter all the notices that refer to this License, so
+    that they refer to the ordinary GNU General Public License, version 2,
+    instead of to this License.  (If a newer version than version 2 of the
+    ordinary GNU General Public License has appeared, then you can specify
+    that version instead if you wish.)  Do not make any other change in
+    these notices.
+
+      Once this change is made in a given copy, it is irreversible for
+    that copy, so the ordinary GNU General Public License applies to all
+    subsequent copies and derivative works made from that copy.
+
+      This option is useful when you wish to copy part of the code of
+    the Library into a program that is not a library.
+
+      4. You may copy and distribute the Library (or a portion or
+    derivative of it, under Section 2) in object code or executable form
+    under the terms of Sections 1 and 2 above provided that you accompany
+    it with the complete corresponding machine-readable source code, which
+    must be distributed under the terms of Sections 1 and 2 above on a
+    medium customarily used for software interchange.
+
+      If distribution of object code is made by offering access to copy
+    from a designated place, then offering equivalent access to copy the
+    source code from the same place satisfies the requirement to
+    distribute the source code, even though third parties are not
+    compelled to copy the source along with the object code.
+
+      5. A program that contains no derivative of any portion of the
+    Library, but is designed to work with the Library by being compiled or
+    linked with it, is called a "work that uses the Library".  Such a
+    work, in isolation, is not a derivative work of the Library, and
+    therefore falls outside the scope of this License.
+
+      However, linking a "work that uses the Library" with the Library
+    creates an executable that is a derivative of the Library (because it
+    contains portions of the Library), rather than a "work that uses the
+    library".  The executable is therefore covered by this License.
+    Section 6 states terms for distribution of such executables.
+
+      When a "work that uses the Library" uses material from a header file
+    that is part of the Library, the object code for the work may be a
+    derivative work of the Library even though the source code is not.
+    Whether this is true is especially significant if the work can be
+    linked without the Library, or if the work is itself a library.  The
+    threshold for this to be true is not precisely defined by law.
+
+      If such an object file uses only numerical parameters, data
+    structure layouts and accessors, and small macros and small inline
+    functions (ten lines or less in length), then the use of the object
+    file is unrestricted, regardless of whether it is legally a derivative
+    work.  (Executables containing this object code plus portions of the
+    Library will still fall under Section 6.)
+
+      Otherwise, if the work is a derivative of the Library, you may
+    distribute the object code for the work under the terms of Section 6.
+    Any executables containing that work also fall under Section 6,
+    whether or not they are linked directly with the Library itself.
+
+      6. As an exception to the Sections above, you may also combine or
+    link a "work that uses the Library" with the Library to produce a
+    work containing portions of the Library, and distribute that work
+    under terms of your choice, provided that the terms permit
+    modification of the work for the customer's own use and reverse
+    engineering for debugging such modifications.
+
+      You must give prominent notice with each copy of the work that the
+    Library is used in it and that the Library and its use are covered by
+    this License.  You must supply a copy of this License.  If the work
+    during execution displays copyright notices, you must include the
+    copyright notice for the Library among them, as well as a reference
+    directing the user to the copy of this License.  Also, you must do one
+    of these things:
+
+        a) Accompany the work with the complete corresponding
+        machine-readable source code for the Library including whatever
+        changes were used in the work (which must be distributed under
+        Sections 1 and 2 above); and, if the work is an executable linked
+        with the Library, with the complete machine-readable "work that
+        uses the Library", as object code and/or source code, so that the
+        user can modify the Library and then relink to produce a modified
+        executable containing the modified Library.  (It is understood
+        that the user who changes the contents of definitions files in the
+        Library will not necessarily be able to recompile the application
+        to use the modified definitions.)
+
+        b) Use a suitable shared library mechanism for linking with the
+        Library.  A suitable mechanism is one that (1) uses at run time a
+        copy of the library already present on the user's computer system,
+        rather than copying library functions into the executable, and (2)
+        will operate properly with a modified version of the library, if
+        the user installs one, as long as the modified version is
+        interface-compatible with the version that the work was made with.
+
+        c) Accompany the work with a written offer, valid for at
+        least three years, to give the same user the materials
+        specified in Subsection 6a, above, for a charge no more
+        than the cost of performing this distribution.
+
+        d) If distribution of the work is made by offering access to copy
+        from a designated place, offer equivalent access to copy the above
+        specified materials from the same place.
+
+        e) Verify that the user has already received a copy of these
+        materials or that you have already sent this user a copy.
+
+      For an executable, the required form of the "work that uses the
+    Library" must include any data and utility programs needed for
+    reproducing the executable from it.  However, as a special exception,
+    the materials to be distributed need not include anything that is
+    normally distributed (in either source or binary form) with the major
+    components (compiler, kernel, and so on) of the operating system on
+    which the executable runs, unless that component itself accompanies
+    the executable.
+
+      It may happen that this requirement contradicts the license
+    restrictions of other proprietary libraries that do not normally
+    accompany the operating system.  Such a contradiction means you cannot
+    use both them and the Library together in an executable that you
+    distribute.
+
+      7. You may place library facilities that are a work based on the
+    Library side-by-side in a single library together with other library
+    facilities not covered by this License, and distribute such a combined
+    library, provided that the separate distribution of the work based on
+    the Library and of the other library facilities is otherwise
+    permitted, and provided that you do these two things:
+
+        a) Accompany the combined library with a copy of the same work
+        based on the Library, uncombined with any other library
+        facilities.  This must be distributed under the terms of the
+        Sections above.
+
+        b) Give prominent notice with the combined library of the fact
+        that part of it is a work based on the Library, and explaining
+        where to find the accompanying uncombined form of the same work.
+
+      8. You may not copy, modify, sublicense, link with, or distribute
+    the Library except as expressly provided under this License.  Any
+    attempt otherwise to copy, modify, sublicense, link with, or
+    distribute the Library is void, and will automatically terminate your
+    rights under this License.  However, parties who have received copies,
+    or rights, from you under this License will not have their licenses
+    terminated so long as such parties remain in full compliance.
+
+      9. You are not required to accept this License, since you have not
+    signed it.  However, nothing else grants you permission to modify or
+    distribute the Library or its derivative works.  These actions are
+    prohibited by law if you do not accept this License.  Therefore, by
+    modifying or distributing the Library (or any work based on the
+    Library), you indicate your acceptance of this License to do so, and
+    all its terms and conditions for copying, distributing or modifying
+    the Library or works based on it.
+
+      10. Each time you redistribute the Library (or any work based on the
+    Library), the recipient automatically receives a license from the
+    original licensor to copy, distribute, link with or modify the Library
+    subject to these terms and conditions.  You may not impose any further
+    restrictions on the recipients' exercise of the rights granted herein.
+    You are not responsible for enforcing compliance by third parties with
+    this License.
+
+      11. If, as a consequence of a court judgment or allegation of patent
+    infringement or for any other reason (not limited to patent issues),
+    conditions are imposed on you (whether by court order, agreement or
+    otherwise) that contradict the conditions of this License, they do not
+    excuse you from the conditions of this License.  If you cannot
+    distribute so as to satisfy simultaneously your obligations under this
+    License and any other pertinent obligations, then as a consequence you
+    may not distribute the Library at all.  For example, if a patent
+    license would not permit royalty-free redistribution of the Library by
+    all those who receive copies directly or indirectly through you, then
+    the only way you could satisfy both it and this License would be to
+    refrain entirely from distribution of the Library.
+
+    If any portion of this section is held invalid or unenforceable under any
+    particular circumstance, the balance of the section is intended to apply,
+    and the section as a whole is intended to apply in other circumstances.
+
+    It is not the purpose of this section to induce you to infringe any
+    patents or other property right claims or to contest validity of any
+    such claims; this section has the sole purpose of protecting the
+    integrity of the free software distribution system which is
+    implemented by public license practices.  Many people have made
+    generous contributions to the wide range of software distributed
+    through that system in reliance on consistent application of that
+    system; it is up to the author/donor to decide if he or she is willing
+    to distribute software through any other system and a licensee cannot
+    impose that choice.
+
+    This section is intended to make thoroughly clear what is believed to
+    be a consequence of the rest of this License.
+
+      12. If the distribution and/or use of the Library is restricted in
+    certain countries either by patents or by copyrighted interfaces, the
+    original copyright holder who places the Library under this License may add
+    an explicit geographical distribution limitation excluding those countries,
+    so that distribution is permitted only in or among countries not thus
+    excluded.  In such case, this License incorporates the limitation as if
+    written in the body of this License.
+
+      13. The Free Software Foundation may publish revised and/or new
+    versions of the Lesser General Public License from time to time.
+    Such new versions will be similar in spirit to the present version,
+    but may differ in detail to address new problems or concerns.
+
+    Each version is given a distinguishing version number.  If the Library
+    specifies a version number of this License which applies to it and
+    "any later version", you have the option of following the terms and
+    conditions either of that version or of any later version published by
+    the Free Software Foundation.  If the Library does not specify a
+    license version number, you may choose any version ever published by
+    the Free Software Foundation.
+
+      14. If you wish to incorporate parts of the Library into other free
+    programs whose distribution conditions are incompatible with these,
+    write to the author to ask for permission.  For software which is
+    copyrighted by the Free Software Foundation, write to the Free
+    Software Foundation; we sometimes make exceptions for this.  Our
+    decision will be guided by the two goals of preserving the free status
+    of all derivatives of our free software and of promoting the sharing
+    and reuse of software generally.
+
+                    NO WARRANTY
+
+      15. BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
+    WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
+    EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
+    OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
+    KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
+    IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+    PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
+    LIBRARY IS WITH YOU.  SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
+    THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+      16. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
+    WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
+    AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
+    FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
+    CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
+    LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
+    RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
+    FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
+    SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
+    DAMAGES.
+
+                 END OF TERMS AND CONDITIONS
+
+               How to Apply These Terms to Your New Libraries
+
+      If you develop a new library, and you want it to be of the greatest
+    possible use to the public, we recommend making it free software that
+    everyone can redistribute and change.  You can do so by permitting
+    redistribution under these terms (or, alternatively, under the terms of the
+    ordinary General Public License).
+
+      To apply these terms, attach the following notices to the library.  It is
+    safest to attach them to the start of each source file to most effectively
+    convey the exclusion of warranty; and each file should have at least the
+    "copyright" line and a pointer to where the full notice is found.
+
+        <one line to give the library's name and a brief idea of what it does.>
+        Copyright (C) <year>  <name of author>
+
+        This library is free software; you can redistribute it and/or
+        modify it under the terms of the GNU Lesser General Public
+        License as published by the Free Software Foundation; either
+        version 2.1 of the License, or (at your option) any later version.
+
+        This library is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+        Lesser General Public License for more details.
+
+        You should have received a copy of the GNU Lesser General Public
+        License along with this library; if not, write to the Free Software
+        Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
+
+    Also add information on how to contact you by electronic and paper mail.
+
+    You should also get your employer (if you work as a programmer) or your
+    school, if any, to sign a "copyright disclaimer" for the library, if
+    necessary.  Here is a sample; alter the names:
+
+      Yoyodyne, Inc., hereby disclaims all copyright interest in the
+      library `Frob' (a library for tweaking knobs) written by James Random Hacker.
+
+      <signature of Ty Coon>, 1 April 1990
+      Ty Coon, President of Vice
+
+    That's all there is to it!
+
 The embedded cffi, whose author is Armin Rigo and Maciej Fijalkowski, as a dependency named _cffi_backend.cp39-win_amd64.pyd, is under following MIT licence.
 
     The MIT License
 
     Permission is hereby granted, free of charge, to any person
     obtaining a copy of this software and associated documentation
     files (the "Software"), to deal in the Software without
@@ -118,15 +623,120 @@
     distribute, sublicense, and/or sell copies of the Software, and to
     permit persons to whom the Software is furnished to do so, subject to
     the following conditions:
 
     The above copyright notice and this permission notice shall be
     included in all copies or substantial portions of the Software.
 
-
+The embedded python, which are named as python3.dll, python39.dll,
+_socket.pyd, select.pyd, unicodedata.pyd and zipped in cpython_libs.zip except urwid
+and urwid_win_patch.py as well as the embedded windows_curses dependencies as
+_curses_panel.cp39-win_amd64.pyd and _curses.cp39-win_amd64.pyd are under PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2.
+the posix module in the dependency uses the OpenSSL library for added performance. The OpenSSL library is under the Openssl Licence
+and Original SSLeay License which has been stated bellow.
+
+    PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2
+    --------------------------------------------
+
+    1. This LICENSE AGREEMENT is between the Python Software Foundation
+    ("PSF"), and the Individual or Organization ("Licensee") accessing and
+    otherwise using this software ("Python") in source or binary form and
+    its associated documentation.
+
+    2. Subject to the terms and conditions of this License Agreement, PSF hereby
+    grants Licensee a nonexclusive, royalty-free, world-wide license to reproduce,
+    analyze, test, perform and/or display publicly, prepare derivative works,
+    distribute, and otherwise use Python alone or in any derivative version,
+    provided, however, that PSF's License Agreement and PSF's notice of copyright,
+    i.e., "Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010,
+    2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020 Python Software Foundation;
+    All Rights Reserved" are retained in Python alone or in any derivative version
+    prepared by Licensee.
+
+    3. In the event Licensee prepares a derivative work that is based on
+    or incorporates Python or any part thereof, and wants to make
+    the derivative work available to others as provided herein, then
+    Licensee hereby agrees to include in any such work a brief summary of
+    the changes made to Python.
+
+    4. PSF is making Python available to Licensee on an "AS IS"
+    basis.  PSF MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
+    IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, PSF MAKES NO AND
+    DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
+    FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF PYTHON WILL NOT
+    INFRINGE ANY THIRD PARTY RIGHTS.
+
+    5. PSF SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF PYTHON
+    FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS
+    A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING PYTHON,
+    OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
+
+    6. This License Agreement will automatically terminate upon a material
+    breach of its terms and conditions.
+
+    7. Nothing in this License Agreement shall be deemed to create any
+    relationship of agency, partnership, or joint venture between PSF and
+    Licensee.  This License Agreement does not grant permission to use PSF
+    trademarks or trade name in a trademark sense to endorse or promote
+    products or services of Licensee, or any third party.
+
+    8. By copying, installing or otherwise using Python, Licensee
+    agrees to be bound by the terms and conditions of this License
+    Agreement.
+
+    SipHash24
+    Files mentioned above, contains
+    Marek Majkowski's implementation of Dan Bernstein's SipHash24 algorithm. It contains the following note:
+    <MIT License>
+    Copyright (c) 2013  Marek Majkowski <marek@popcount.org>
+
+    Permission is hereby granted, free of charge, to any person obtaining a copy
+    of this software and associated documentation files (the "Software"), to deal
+    in the Software without restriction, including without limitation the rights
+    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+    copies of the Software, and to permit persons to whom the Software is
+    furnished to do so, subject to the following conditions:
+
+    The above copyright notice and this permission notice shall be included in
+    all copies or substantial portions of the Software.
+    </MIT License>
+
+    Original location:
+       https://github.com/majek/csiphash/
+
+    Solution inspired by code from:
+       Samuel Neves (supercop/crypto_auth/siphash24/little)
+       djb (supercop/crypto_auth/siphash24/little2)
+       Jean-Philippe Aumasson (https://131002.net/siphash/siphash24.c)
+
+    strtod and dtoa
+    Files mentioned above, contains C functions dtoa and strtod for conversion of C
+    doubles to and from strings,
+    is derived from the file of the same name by David M. Gay, currently available
+    from https://web.archive.org/web/20220517033456/http://www.netlib.org/fp/dtoa.c.
+    The original file, as retrieved on March 16, 2009, contains the following copyright
+    and licensing notice:
+    /****************************************************************
+     *
+     * The author of this software is David M. Gay.
+     *
+     * Copyright (c) 1991, 2000, 2001 by Lucent Technologies.
+     *
+     * Permission to use, copy, modify, and distribute this software for any
+     * purpose without fee is hereby granted, provided that this entire notice
+     * is included in all copies of any software which is or includes a copy
+     * or modification of this software and in all copies of the supporting
+     * documentation for such software.
+     *
+     * THIS SOFTWARE IS BEING PROVIDED "AS IS", WITHOUT ANY EXPRESS OR IMPLIED
+     * WARRANTY.  IN PARTICULAR, NEITHER THE AUTHOR NOR LUCENT MAKES ANY
+     * REPRESENTATION OR WARRANTY OF ANY KIND CONCERNING THE MERCHANTABILITY
+     * OF THIS SOFTWARE OR ITS FITNESS FOR ANY PARTICULAR PURPOSE.
+     *
+     ***************************************************************/
 
 The embedded openssl, embedded in libdecryption11.dll and libdecryption.dll, is under following double licences.
 
       OpenSSL License
       ---------------
     /* ====================================================================
      * Copyright (c) 1998-2019 The OpenSSL Project.  All rights reserved.
```

## shared_atomic/libdecryption.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180283860
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Jul  6 09:00:25 2023
+Time/Date		Mon Aug  7 12:15:36 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000285000
 SizeOfInitializedData	00000000000d2e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000283860
@@ -950038,15 +950038,15 @@
 	...
    18031f188:	and    %bl,0x180(%rbx,%rsi,1)
    18031f18f:	add    %al,%al
    18031f191:	pushf
    18031f192:	xor    0x1(%rax),%eax
    18031f198:	add    %al,(%rax)
    18031f19a:	add    %al,(%rax)
-   18031f19c:	test   $0x64a682,%eax
+   18031f19c:	push   $0x64d0e0
    18031f1a1:	add    %al,(%rax)
    18031f1a3:	add    %cl,0x7c000000(%rip)        # 0x1fc31f1a9
    18031f1a9:	add    (%rax),%al
    18031f1ab:	add    %cl,%al
    18031f1ad:	clc
    18031f1ae:	xor    %eax,(%rax)
    18031f1b0:	enter  $0x31ec,$0x0
```

## shared_atomic/libdecryption11.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001320
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Jul  6 09:00:26 2023
+Time/Date		Mon Aug  7 12:15:36 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000000e00
 SizeOfInitializedData	0000000000001400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001320
@@ -1464,17 +1464,18 @@
    18000215a:	(bad)
    18000215b:	(bad)
    18000215c:	(bad)
    18000215d:	(bad)
    18000215e:	(bad)
    18000215f:	incl   (%rax)
    180002161:	add    %al,(%rax)
-   180002163:	add    %ch,0x64a682(%rdx)
-   180002169:	add    %al,(%rax)
-   18000216b:	add    %cl,0x58000000(%rip)        # 0x1d8002171
+   180002163:	add    %ch,-0x20(%rax)
+   180002166:	shlb   0x0(%rax,%rax,1)
+   18000216a:	add    %al,(%rax)
+   18000216c:	or     $0x58000000,%eax
    180002171:	add    (%rax),%al
    180002173:	add    %bl,(%rax)
    180002175:	and    (%rax),%eax
    180002177:	add    %bl,(%rax)
    180002179:	adc    $0x0,%eax
    18000217e:	add    %al,(%rax)
    180002180:	cmp    %al,(%rcx)
```

## shared_atomic/urwid_win_patch.py

```diff
@@ -1,34 +1,20 @@
 """
 Patch urwid on Windows and WSL.
 
 On Windows, install the package "windows-curses".
 """
 import curses
-import platform
-import re
 
 import urwid
 import urwid.curses_display
 import urwid.raw_display
 
-IS_WSL = ("Linux" in platform.platform()) and ("Microsoft" in platform.platform())
-IS_WINDOWS = ("Windows" in platform.platform()) and ("Linux" not in platform.platform())
-
-if IS_WSL:
-    # Filter out SI/SO under WSL. See:
-    # https://github.com/mitmproxy/mitmproxy/blob/8dfb8a9a7471e00b0f723de66d3b63bd089e9802/mitmproxy/tools/console/window.py#L316-L323
-    wsl_patch_orig_write = urwid.raw_display.Screen.write
-    wsl_patch_write_re = re.compile("[\x0e\x0f]")
-
-    def wsl_patch_write(self, data):
-        data = wsl_patch_write_re.sub("", data)
-        return wsl_patch_orig_write(self, data)
-
-    urwid.raw_display.Screen.write = wsl_patch_write
+IS_WSL = False
+IS_WINDOWS = True
 
 if IS_WINDOWS:
     def win_patch_tty_signal_keys(self, intr=None, quit=None, start=None, stop=None, susp=None, fileno=None):
         pass  # no signals on Windows; not needed for resize
     urwid.display_common.RealTerminal.tty_signal_keys = win_patch_tty_signal_keys
 
     win_patch_orig__start = urwid.curses_display.Screen._start
```

