# Comparing `tmp/pxblat-0.2.0.tar.gz` & `tmp/pxblat-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxblat-0.2.0.tar", max compression
+gzip compressed data, was "pxblat-0.3.0.tar", max compression
```

## Comparing `pxblat-0.2.0.tar` & `pxblat-0.3.0.tar`

### file list

```diff
@@ -1,199 +1,198 @@
--rw-r--r--   0        0        0     1067 2023-06-13 04:56:47.859163 pxblat-0.2.0/LICENSE
--rw-r--r--   0        0        0     7841 2023-06-13 04:56:47.859163 pxblat-0.2.0/README.md
--rw-r--r--   0        0        0     8835 2023-06-13 04:56:48.311165 pxblat-0.2.0/build.py
--rw-r--r--   0        0        0     2671 2023-06-13 04:57:21.947353 pxblat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1356 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/__init__.py
--rw-r--r--   0        0        0       40 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/__init__.py
--rw-r--r--   0        0        0      632 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/cli.py
--rw-r--r--   0        0        0     5944 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/client.py
--rw-r--r--   0        0        0     2316 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/fa2twobit.py
--rw-r--r--   0        0        0      214 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/log.py
--rw-r--r--   0        0        0     7914 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/server.py
--rw-r--r--   0        0        0     3587 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/cli/twobit2fa.py
--rw-r--r--   0        0        0      560 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/__init__.py
--rw-r--r--   0        0        0    27659 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/__init__.pyi
--rw-r--r--   0        0        0       40 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/.clang-format
--rw-r--r--   0        0        0     2083 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/_extc.cpp
--rw-r--r--   0        0        0       11 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/_extc.modules
--rw-r--r--   0        0        0       81 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/_extc.sources
--rw-r--r--   0        0        0     2163 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/faToTwoBit.cpp
--rw-r--r--   0        0        0    10670 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfClient.cpp
--rw-r--r--   0        0        0    20188 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfServer.cpp
--rw-r--r--   0        0        0     2715 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfServer_1.cpp
--rw-r--r--   0        0        0     4632 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/pygfServer.cpp
--rw-r--r--   0        0        0     5912 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/binder/twoBitToFa.cpp
--rw-r--r--   0        0        0    33509 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/bs_thread_pool.hpp
--rw-r--r--   0        0        0    28417 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/dbg.h
--rw-r--r--   0        0        0     2116 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/faToTwoBit.cpp
--rw-r--r--   0        0        0     1243 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/faToTwoBit.hpp
--rw-r--r--   0        0        0    13652 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/gfClient.cpp
--rw-r--r--   0        0        0     4820 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/gfClient.hpp
--rw-r--r--   0        0        0    60809 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/gfServer.cpp
--rw-r--r--   0        0        0    11554 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/gfServer.hpp
--rw-r--r--   0        0        0    11325 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/pygfServer.cpp
--rw-r--r--   0        0        0      973 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/pygfServer.hpp
--rw-r--r--   0        0        0     8728 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/twoBitToFa.cpp
--rw-r--r--   0        0        0     3521 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/bindings/twoBitToFa.hpp
--rw-r--r--   0        0        0    24597 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/blat.c
--rw-r--r--   0        0        0     3485 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/faToTwoBit.c
--rw-r--r--   0        0        0     9944 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/gfClient.c
--rw-r--r--   0        0        0    53782 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/gfServer.c
--rw-r--r--   0        0        0       40 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/.clang-format
--rw-r--r--   0        0        0     2088 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/bandExt.h
--rw-r--r--   0        0        0     1073 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/base64.h
--rw-r--r--   0        0        0    27036 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/cheapcgi.h
--rw-r--r--   0        0        0     2097 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/filePath.h
--rw-r--r--   0        0        0      871 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/gfxPoly.h
--rw-r--r--   0        0        0     1034 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/hex.h
--rw-r--r--   0        0        0    10111 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/htmlPage.h
--rw-r--r--   0        0        0     9985 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/htmshell.h
--rw-r--r--   0        0        0      332 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/https.h
--rw-r--r--   0        0        0     4404 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/internet.h
--rw-r--r--   0        0        0     1990 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/kxTok.h
--rw-r--r--   0        0        0    16767 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/memgfx.h
--rw-r--r--   0        0        0     2997 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/mime.h
--rw-r--r--   0        0        0     1166 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/portimpl.h
--rw-r--r--   0        0        0     4401 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/rbTree.h
--rw-r--r--   0        0        0      164 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/aux/srcVersion.h
--rw-r--r--   0        0        0      916 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/core/aliType.h
--rw-r--r--   0        0        0     6547 2023-06-13 04:56:48.343165 pxblat-0.2.0/src/pxblat/extc/include/core/asParse.h
--rw-r--r--   0        0        0    10193 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/axt.h
--rw-r--r--   0        0        0     6470 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/bPlusTree.h
--rw-r--r--   0        0        0    14293 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/basicBed.h
--rw-r--r--   0        0        0     4355 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/binRange.h
--rw-r--r--   0        0        0     3456 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/bits.h
--rw-r--r--   0        0        0     5877 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/chain.h
--rw-r--r--   0        0        0     1839 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/chainBlock.h
--rw-r--r--   0        0        0    56916 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/common.h
--rw-r--r--   0        0        0     4198 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/dlist.h
--rw-r--r--   0        0        0     2681 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/dnaseq.h
--rw-r--r--   0        0        0    10058 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/dnautil.h
--rw-r--r--   0        0        0     3658 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/dystring.h
--rw-r--r--   0        0        0     2795 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/errAbort.h
--rw-r--r--   0        0        0     2128 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/errCatch.h
--rw-r--r--   0        0        0     5228 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/fa.h
--rw-r--r--   0        0        0    10590 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/fuzzyFind.h
--rw-r--r--   0        0        0    19945 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/genoFind.h
--rw-r--r--   0        0        0     1115 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/gfClientLib.h
--rw-r--r--   0        0        0     2884 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/gfInternal.h
--rw-r--r--   0        0        0    12187 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/hash.h
--rw-r--r--   0        0        0     1111 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/htmlColor.h
--rw-r--r--   0        0        0    14055 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/linefile.h
--rw-r--r--   0        0        0     3618 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/localmem.h
--rw-r--r--   0        0        0    10130 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/maf.h
--rw-r--r--   0        0        0     1786 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/memalloc.h
--rw-r--r--   0        0        0    12155 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/net.h
--rw-r--r--   0        0        0    12162 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/netlib.h
--rw-r--r--   0        0        0     4114 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/nib.h
--rw-r--r--   0        0        0     8773 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/obscure.h
--rw-r--r--   0        0        0      605 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/ooc.h
--rw-r--r--   0        0        0     3981 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/options.h
--rw-r--r--   0        0        0     1910 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/patSpace.h
--rw-r--r--   0        0        0     7300 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/pipeline.h
--rw-r--r--   0        0        0     6256 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/portable.h
--rw-r--r--   0        0        0    14633 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/psl.h
--rw-r--r--   0        0        0     4818 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/rangeTree.h
--rw-r--r--   0        0        0     2459 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/repMask.h
--rw-r--r--   0        0        0     3070 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/sig.h
--rw-r--r--   0        0        0     6814 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/sqlList.h
--rw-r--r--   0        0        0     3444 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/sqlNum.h
--rw-r--r--   0        0        0     2492 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/supStitch.h
--rw-r--r--   0        0        0     2499 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/tokenizer.h
--rw-r--r--   0        0        0     2086 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/trans3.h
--rw-r--r--   0        0        0     8657 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/twoBit.h
--rw-r--r--   0        0        0     9058 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/udc.h
--rw-r--r--   0        0        0     1821 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/core/verbose.h
--rw-r--r--   0        0        0        0 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/net/gfNet.h
--rw-r--r--   0        0        0     2278 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/include/net/log.h
--rw-r--r--   0        0        0       40 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/.clang-format
--rw-r--r--   0        0        0    31426 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/axt.c
--rw-r--r--   0        0        0    14386 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/bandExt.c
--rw-r--r--   0        0        0     2996 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/base64.c
--rw-r--r--   0        0        0    11289 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/binRange.c
--rw-r--r--   0        0        0    25709 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/blastOut.c
--rw-r--r--   0        0        0    80472 2023-06-13 04:56:48.347165 pxblat-0.2.0/src/pxblat/extc/src/aux/cheapcgi.c
--rw-r--r--   0        0        0    32618 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/ffSeedExtend.c
--rw-r--r--   0        0        0     6436 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/filePath.c
--rw-r--r--   0        0        0     2363 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/hex.c
--rw-r--r--   0        0        0    53011 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/htmlPage.c
--rw-r--r--   0        0        0    46630 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/htmshell.c
--rw-r--r--   0        0        0    27672 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/https.c
--rw-r--r--   0        0        0     2489 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/intExp.c
--rw-r--r--   0        0        0    16703 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/internet.c
--rw-r--r--   0        0        0    24031 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/maf.c
--rw-r--r--   0        0        0     2306 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/mafFromAxt.c
--rw-r--r--   0        0        0    16690 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/mime.c
--rw-r--r--   0        0        0    62706 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/net.c
--rw-r--r--   0        0        0    62778 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/netlib.c
--rw-r--r--   0        0        0     1742 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/ooc.c
--rw-r--r--   0        0        0    11962 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/patSpace.c
--rw-r--r--   0        0        0     3896 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/portimpl.c
--rw-r--r--   0        0        0    13003 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/rangeTree.c
--rw-r--r--   0        0        0    18572 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/rbTree.c
--rw-r--r--   0        0        0     5678 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/repMask.c
--rw-r--r--   0        0        0      848 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/servBrcMcw.c
--rw-r--r--   0        0        0     1033 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/servCrunx.c
--rw-r--r--   0        0        0      864 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/servcis.c
--rw-r--r--   0        0        0      906 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/servmsII.c
--rw-r--r--   0        0        0      921 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/servpws.c
--rw-r--r--   0        0        0    27041 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/sqlList.c
--rw-r--r--   0        0        0     7239 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/sqlNum.c
--rw-r--r--   0        0        0     3898 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/aux/wildcmp.c
--rw-r--r--   0        0        0      930 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/aliType.c
--rw-r--r--   0        0        0    21737 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/asParse.c
--rw-r--r--   0        0        0    19732 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/bPlusTree.c
--rw-r--r--   0        0        0    54752 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/basicBed.c
--rw-r--r--   0        0        0     9051 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/bits.c
--rw-r--r--   0        0        0    17259 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/chain.c
--rw-r--r--   0        0        0    17077 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/chainBlock.c
--rw-r--r--   0        0        0    90522 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/common.c
--rw-r--r--   0        0        0     9450 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/dlist.c
--rw-r--r--   0        0        0     4604 2023-06-13 04:56:48.351165 pxblat-0.2.0/src/pxblat/extc/src/core/dnaseq.c
--rw-r--r--   0        0        0    29952 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/dnautil.c
--rw-r--r--   0        0        0     7156 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/dystring.c
--rw-r--r--   0        0        0    12046 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/errAbort.c
--rw-r--r--   0        0        0     3932 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/errCatch.c
--rw-r--r--   0        0        0    15611 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/fa.c
--rw-r--r--   0        0        0     3714 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/ffAli.c
--rw-r--r--   0        0        0    10802 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/ffAliHelp.c
--rw-r--r--   0        0        0     4868 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/ffScore.c
--rw-r--r--   0        0        0    40189 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/fuzzyFind.c
--rw-r--r--   0        0        0    70461 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/genoFind.c
--rw-r--r--   0        0        0    52425 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/gfBlatLib.c
--rw-r--r--   0        0        0     6363 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/gfClientLib.c
--rw-r--r--   0        0        0     3845 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/gfInternal.c
--rw-r--r--   0        0        0    18190 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/gfOut.c
--rw-r--r--   0        0        0    22265 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/hash.c
--rw-r--r--   0        0        0     2919 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/htmlColor.c
--rw-r--r--   0        0        0     5273 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/kxTok.c
--rw-r--r--   0        0        0    40326 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/linefile.c
--rw-r--r--   0        0        0     7256 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/localmem.c
--rw-r--r--   0        0        0    15074 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/memalloc.c
--rw-r--r--   0        0        0    12778 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/nib.c
--rw-r--r--   0        0        0    24969 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/obscure.c
--rw-r--r--   0        0        0    13012 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/options.c
--rw-r--r--   0        0        0    20522 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/osunix.c
--rw-r--r--   0        0        0    23419 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/pipeline.c
--rw-r--r--   0        0        0    63467 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/psl.c
--rw-r--r--   0        0        0     1203 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/servcl.c
--rw-r--r--   0        0        0    26961 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/supStitch.c
--rw-r--r--   0        0        0     5025 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/tokenizer.c
--rw-r--r--   0        0        0     3216 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/trans3.c
--rw-r--r--   0        0        0    33527 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/twoBit.c
--rw-r--r--   0        0        0    71967 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/udc.c
--rw-r--r--   0        0        0     4255 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/core/verbose.c
--rw-r--r--   0        0        0     2571 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/net/gfNet.c
--rw-r--r--   0        0        0     8795 2023-06-13 04:56:48.355165 pxblat-0.2.0/src/pxblat/extc/src/net/log.c
--rw-r--r--   0        0        0     7666 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/extc/twoBitToFa.c
--rw-r--r--   0        0        0     3052 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/parser.py
--rw-r--r--   0        0        0        0 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/py.typed
--rw-r--r--   0        0        0      988 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/__init__.py
--rw-r--r--   0        0        0    15567 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/basic.py
--rw-r--r--   0        0        0     4665 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/client.py
--rw-r--r--   0        0        0    10366 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/server.py
--rw-r--r--   0        0        0     1041 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/status.py
--rw-r--r--   0        0        0      115 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/server/utils.py
--rw-r--r--   0        0        0     1796 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/toolkit/__init__.py
--rw-r--r--   0        0        0     3431 2023-06-13 04:56:48.359166 pxblat-0.2.0/src/pxblat/utils.py
--rw-r--r--   0        0        0     9495 1970-01-01 00:00:00.000000 pxblat-0.2.0/setup.py
--rw-r--r--   0        0        0     8742 1970-01-01 00:00:00.000000 pxblat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-27 03:36:11.031192 pxblat-0.3.0/LICENSE
+-rw-r--r--   0        0        0    12251 2023-07-27 03:36:11.031192 pxblat-0.3.0/README.md
+-rw-r--r--   0        0        0     8835 2023-07-27 03:36:11.567234 pxblat-0.3.0/build.py
+-rw-r--r--   0        0        0     4104 2023-07-27 03:36:49.822201 pxblat-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1484 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/__init__.py
+-rw-r--r--   0        0        0       80 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/cli/__init__.py
+-rw-r--r--   0        0        0      721 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/cli/cli.py
+-rw-r--r--   0        0        0     5997 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/cli/client.py
+-rw-r--r--   0        0        0     2373 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/cli/fa2twobit.py
+-rw-r--r--   0        0        0      227 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/cli/log.py
+-rw-r--r--   0        0        0     7933 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/cli/server.py
+-rw-r--r--   0        0        0     3559 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/cli/twobit2fa.py
+-rw-r--r--   0        0        0      560 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/__init__.py
+-rw-r--r--   0        0        0    27386 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/__init__.pyi
+-rw-r--r--   0        0        0       40 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/binder/.clang-format
+-rw-r--r--   0        0        0     2083 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/binder/_extc.cpp
+-rw-r--r--   0        0        0       11 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/binder/_extc.modules
+-rw-r--r--   0        0        0       81 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/binder/_extc.sources
+-rw-r--r--   0        0        0     2163 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/binder/faToTwoBit.cpp
+-rw-r--r--   0        0        0    10825 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/binder/gfClient.cpp
+-rw-r--r--   0        0        0    20049 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/binder/gfServer.cpp
+-rw-r--r--   0        0        0     2715 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/binder/gfServer_1.cpp
+-rw-r--r--   0        0        0     4632 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/binder/pygfServer.cpp
+-rw-r--r--   0        0        0     5912 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/binder/twoBitToFa.cpp
+-rw-r--r--   0        0        0    33509 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/bs_thread_pool.hpp
+-rw-r--r--   0        0        0    28417 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/dbg.h
+-rw-r--r--   0        0        0     2116 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/faToTwoBit.cpp
+-rw-r--r--   0        0        0     1243 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/faToTwoBit.hpp
+-rw-r--r--   0        0        0    13652 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/gfClient.cpp
+-rw-r--r--   0        0        0     4820 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/gfClient.hpp
+-rw-r--r--   0        0        0    60623 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/gfServer.cpp
+-rw-r--r--   0        0        0    11419 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/gfServer.hpp
+-rw-r--r--   0        0        0    11325 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/pygfServer.cpp
+-rw-r--r--   0        0        0      973 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/pygfServer.hpp
+-rw-r--r--   0        0        0     8728 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/twoBitToFa.cpp
+-rw-r--r--   0        0        0     3521 2023-07-27 03:36:11.603237 pxblat-0.3.0/src/pxblat/extc/bindings/twoBitToFa.hpp
+-rw-r--r--   0        0        0    24597 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/blat.c
+-rw-r--r--   0        0        0     3485 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/faToTwoBit.c
+-rw-r--r--   0        0        0     9944 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/gfClient.c
+-rw-r--r--   0        0        0    53782 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/gfServer.c
+-rw-r--r--   0        0        0       40 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/.clang-format
+-rw-r--r--   0        0        0     2088 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/bandExt.h
+-rw-r--r--   0        0        0     1073 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/base64.h
+-rw-r--r--   0        0        0    27036 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/cheapcgi.h
+-rw-r--r--   0        0        0     2097 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/filePath.h
+-rw-r--r--   0        0        0      871 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/gfxPoly.h
+-rw-r--r--   0        0        0     1034 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/hex.h
+-rw-r--r--   0        0        0    10111 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/htmlPage.h
+-rw-r--r--   0        0        0     9985 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/htmshell.h
+-rw-r--r--   0        0        0      332 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/https.h
+-rw-r--r--   0        0        0     4404 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/internet.h
+-rw-r--r--   0        0        0     1990 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/kxTok.h
+-rw-r--r--   0        0        0    16767 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/memgfx.h
+-rw-r--r--   0        0        0     2997 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/mime.h
+-rw-r--r--   0        0        0     1166 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/portimpl.h
+-rw-r--r--   0        0        0     4401 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/rbTree.h
+-rw-r--r--   0        0        0      164 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/aux/srcVersion.h
+-rw-r--r--   0        0        0      916 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/aliType.h
+-rw-r--r--   0        0        0     6547 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/asParse.h
+-rw-r--r--   0        0        0    10193 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/axt.h
+-rw-r--r--   0        0        0     6470 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/bPlusTree.h
+-rw-r--r--   0        0        0    14293 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/basicBed.h
+-rw-r--r--   0        0        0     4355 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/binRange.h
+-rw-r--r--   0        0        0     3456 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/bits.h
+-rw-r--r--   0        0        0     5877 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/chain.h
+-rw-r--r--   0        0        0     1839 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/chainBlock.h
+-rw-r--r--   0        0        0    56916 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/common.h
+-rw-r--r--   0        0        0     4198 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/dlist.h
+-rw-r--r--   0        0        0     2681 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/dnaseq.h
+-rw-r--r--   0        0        0    10058 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/dnautil.h
+-rw-r--r--   0        0        0     3658 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/dystring.h
+-rw-r--r--   0        0        0     2795 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/errAbort.h
+-rw-r--r--   0        0        0     2128 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/errCatch.h
+-rw-r--r--   0        0        0     5228 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/fa.h
+-rw-r--r--   0        0        0    10590 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/fuzzyFind.h
+-rw-r--r--   0        0        0    19945 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/genoFind.h
+-rw-r--r--   0        0        0     1115 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/gfClientLib.h
+-rw-r--r--   0        0        0     2884 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/gfInternal.h
+-rw-r--r--   0        0        0    12187 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/hash.h
+-rw-r--r--   0        0        0     1111 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/htmlColor.h
+-rw-r--r--   0        0        0    14055 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/linefile.h
+-rw-r--r--   0        0        0     3618 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/localmem.h
+-rw-r--r--   0        0        0    10130 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/maf.h
+-rw-r--r--   0        0        0     1786 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/memalloc.h
+-rw-r--r--   0        0        0    12155 2023-07-27 03:36:11.607237 pxblat-0.3.0/src/pxblat/extc/include/core/net.h
+-rw-r--r--   0        0        0    12162 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/netlib.h
+-rw-r--r--   0        0        0     4114 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/nib.h
+-rw-r--r--   0        0        0     8773 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/obscure.h
+-rw-r--r--   0        0        0      605 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/ooc.h
+-rw-r--r--   0        0        0     3981 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/options.h
+-rw-r--r--   0        0        0     1910 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/patSpace.h
+-rw-r--r--   0        0        0     7300 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/pipeline.h
+-rw-r--r--   0        0        0     6256 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/portable.h
+-rw-r--r--   0        0        0    14633 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/psl.h
+-rw-r--r--   0        0        0     4818 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/rangeTree.h
+-rw-r--r--   0        0        0     2459 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/repMask.h
+-rw-r--r--   0        0        0     3070 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/sig.h
+-rw-r--r--   0        0        0     6814 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/sqlList.h
+-rw-r--r--   0        0        0     3444 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/sqlNum.h
+-rw-r--r--   0        0        0     2492 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/supStitch.h
+-rw-r--r--   0        0        0     2499 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/tokenizer.h
+-rw-r--r--   0        0        0     2086 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/trans3.h
+-rw-r--r--   0        0        0     8657 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/twoBit.h
+-rw-r--r--   0        0        0     9058 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/udc.h
+-rw-r--r--   0        0        0     1821 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/core/verbose.h
+-rw-r--r--   0        0        0        0 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/net/gfNet.h
+-rw-r--r--   0        0        0     2278 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/include/net/log.h
+-rw-r--r--   0        0        0       40 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/.clang-format
+-rw-r--r--   0        0        0    31426 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/axt.c
+-rw-r--r--   0        0        0    14386 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/bandExt.c
+-rw-r--r--   0        0        0     2996 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/base64.c
+-rw-r--r--   0        0        0    11289 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/binRange.c
+-rw-r--r--   0        0        0    25709 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/blastOut.c
+-rw-r--r--   0        0        0    80472 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/cheapcgi.c
+-rw-r--r--   0        0        0    32618 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/ffSeedExtend.c
+-rw-r--r--   0        0        0     6436 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/filePath.c
+-rw-r--r--   0        0        0     2363 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/hex.c
+-rw-r--r--   0        0        0    53011 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/htmlPage.c
+-rw-r--r--   0        0        0    46630 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/htmshell.c
+-rw-r--r--   0        0        0    27672 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/https.c
+-rw-r--r--   0        0        0     2489 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/intExp.c
+-rw-r--r--   0        0        0    16703 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/internet.c
+-rw-r--r--   0        0        0    24031 2023-07-27 03:36:11.611237 pxblat-0.3.0/src/pxblat/extc/src/aux/maf.c
+-rw-r--r--   0        0        0     2306 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/mafFromAxt.c
+-rw-r--r--   0        0        0    16690 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/mime.c
+-rw-r--r--   0        0        0    62706 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/net.c
+-rw-r--r--   0        0        0    62778 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/netlib.c
+-rw-r--r--   0        0        0     1742 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/ooc.c
+-rw-r--r--   0        0        0    11962 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/patSpace.c
+-rw-r--r--   0        0        0     3896 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/portimpl.c
+-rw-r--r--   0        0        0    13003 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/rangeTree.c
+-rw-r--r--   0        0        0    18572 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/rbTree.c
+-rw-r--r--   0        0        0     5678 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/repMask.c
+-rw-r--r--   0        0        0      848 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/servBrcMcw.c
+-rw-r--r--   0        0        0     1033 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/servCrunx.c
+-rw-r--r--   0        0        0      864 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/servcis.c
+-rw-r--r--   0        0        0      906 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/servmsII.c
+-rw-r--r--   0        0        0      921 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/servpws.c
+-rw-r--r--   0        0        0    27041 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/sqlList.c
+-rw-r--r--   0        0        0     7239 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/sqlNum.c
+-rw-r--r--   0        0        0     3898 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/aux/wildcmp.c
+-rw-r--r--   0        0        0      930 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/aliType.c
+-rw-r--r--   0        0        0    21737 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/asParse.c
+-rw-r--r--   0        0        0    19732 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/bPlusTree.c
+-rw-r--r--   0        0        0    54752 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/basicBed.c
+-rw-r--r--   0        0        0     9051 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/bits.c
+-rw-r--r--   0        0        0    17259 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/chain.c
+-rw-r--r--   0        0        0    17077 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/chainBlock.c
+-rw-r--r--   0        0        0    90522 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/common.c
+-rw-r--r--   0        0        0     9450 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/dlist.c
+-rw-r--r--   0        0        0     4604 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/dnaseq.c
+-rw-r--r--   0        0        0    29952 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/dnautil.c
+-rw-r--r--   0        0        0     7156 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/dystring.c
+-rw-r--r--   0        0        0    12046 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/errAbort.c
+-rw-r--r--   0        0        0     3932 2023-07-27 03:36:11.615238 pxblat-0.3.0/src/pxblat/extc/src/core/errCatch.c
+-rw-r--r--   0        0        0    15611 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/fa.c
+-rw-r--r--   0        0        0     3714 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/ffAli.c
+-rw-r--r--   0        0        0    10802 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/ffAliHelp.c
+-rw-r--r--   0        0        0     4868 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/ffScore.c
+-rw-r--r--   0        0        0    40189 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/fuzzyFind.c
+-rw-r--r--   0        0        0    70461 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/genoFind.c
+-rw-r--r--   0        0        0    52425 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/gfBlatLib.c
+-rw-r--r--   0        0        0     6363 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/gfClientLib.c
+-rw-r--r--   0        0        0     3845 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/gfInternal.c
+-rw-r--r--   0        0        0    18190 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/gfOut.c
+-rw-r--r--   0        0        0    22265 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/hash.c
+-rw-r--r--   0        0        0     2919 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/htmlColor.c
+-rw-r--r--   0        0        0     5273 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/kxTok.c
+-rw-r--r--   0        0        0    40326 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/linefile.c
+-rw-r--r--   0        0        0     7256 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/localmem.c
+-rw-r--r--   0        0        0    15074 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/memalloc.c
+-rw-r--r--   0        0        0    12778 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/nib.c
+-rw-r--r--   0        0        0    24969 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/obscure.c
+-rw-r--r--   0        0        0    13012 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/options.c
+-rw-r--r--   0        0        0    20522 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/osunix.c
+-rw-r--r--   0        0        0    23419 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/pipeline.c
+-rw-r--r--   0        0        0    63467 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/psl.c
+-rw-r--r--   0        0        0     1203 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/servcl.c
+-rw-r--r--   0        0        0    26961 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/supStitch.c
+-rw-r--r--   0        0        0     5025 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/tokenizer.c
+-rw-r--r--   0        0        0     3216 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/trans3.c
+-rw-r--r--   0        0        0    33527 2023-07-27 03:36:11.619238 pxblat-0.3.0/src/pxblat/extc/src/core/twoBit.c
+-rw-r--r--   0        0        0    71967 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/extc/src/core/udc.c
+-rw-r--r--   0        0        0     4255 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/extc/src/core/verbose.c
+-rw-r--r--   0        0        0     2571 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/extc/src/net/gfNet.c
+-rw-r--r--   0        0        0     8795 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/extc/src/net/log.c
+-rw-r--r--   0        0        0     7666 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/extc/twoBitToFa.c
+-rw-r--r--   0        0        0     6472 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/parser.py
+-rw-r--r--   0        0        0        0 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/py.typed
+-rw-r--r--   0        0        0      873 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/server/__init__.py
+-rw-r--r--   0        0        0    16205 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/server/basic.py
+-rw-r--r--   0        0        0    16214 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/server/client.py
+-rw-r--r--   0        0        0    11837 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/server/server.py
+-rw-r--r--   0        0        0     1812 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/server/status.py
+-rw-r--r--   0        0        0      114 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/server/utils.py
+-rw-r--r--   0        0        0     2930 2023-07-27 03:36:11.623238 pxblat-0.3.0/src/pxblat/toolkit/__init__.py
+-rw-r--r--   0        0        0    13997 1970-01-01 00:00:00.000000 pxblat-0.3.0/setup.py
+-rw-r--r--   0        0        0    13227 1970-01-01 00:00:00.000000 pxblat-0.3.0/PKG-INFO
```

### Comparing `pxblat-0.2.0/LICENSE` & `pxblat-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/build.py` & `pxblat-0.3.0/build.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/__init__.py` & `pxblat-0.3.0/src/pxblat/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,34 +2,40 @@
 from .extc import ServerOption
 from .extc import TwoBitToFaOption
 from .extc import UsageStats
 from .parser import read
 from .server import check_port_in_use
 from .server import check_port_open
 from .server import Client
+from .server import ClientThread
 from .server import create_client_option
 from .server import create_server_option
-from .server import DEFAULT_PORT
+from .server import copy_client_option
 from .server import files
 from .server import find_free_port
 from .server import query_server
 from .server import Server
 from .server import server_query
 from .server import start_server
 from .server import start_server_mt
 from .server import start_server_mt_nb
 from .server import Status
 from .server import status_server
 from .server import stop_server
 from .server import wait_server_ready
 from .toolkit import fa_to_two_bit
 from .toolkit import two_bit_to_fa
+from rich.traceback import install
+
+install(show_locals=True)
+
 
 __all__ = [
     "Server",
+    "ClientThread",
     "Client",
     "files",
     "server_query",
     "start_server_mt",
     "start_server",
     "status_server",
     "stop_server",
@@ -39,15 +45,15 @@
     "two_bit_to_fa",
     "create_server_option",
     "check_port_open",
     "start_server_mt_nb",
     "wait_server_ready",
     "find_free_port",
     "check_port_in_use",
-    "DEFAULT_PORT",
+    "copy_client_option",
     "Status",
     "read",
     "TwoBitToFaOption",
     "ClientOption",
     "ServerOption",
     "UsageStats",
 ]
```

### Comparing `pxblat-0.2.0/src/pxblat/cli/cli.py` & `pxblat-0.3.0/src/pxblat/cli/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+"""Command line interface for pxblat."""
 import sys
+from datetime import datetime
 
 import typer
 
 from .client import client
 from .fa2twobit import faToTwoBit
 from .server import server_app
 from .twobit2fa import twoBitToFa
 
 app = typer.Typer(
-    epilog="YangyangLi 2023 yangyang.li@northwstern.edu",
+    epilog=f"YangyangLi {datetime.now().year} yangyang.li@northwstern.edu",
     context_settings={"help_option_names": ["-h", "--help"]},
 )
 
 app.command()(faToTwoBit)
 app.command()(client)
 app.command()(twoBitToFa)
```

### Comparing `pxblat-0.2.0/src/pxblat/cli/client.py` & `pxblat-0.3.0/src/pxblat/cli/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 import typer
+
 from pxblat.extc import pygfClient
 from pxblat.server import create_client_option
 
-
 # gfClient v. 37x1 - A client for the genomic finding program that produces a .psl file
 # usage:
 #    gfClient host port seqDir in.fa out.psl
 # where
 #    host is the name of the machine running the gfServer
 #    port is the same port that you started the gfServer with
 #    seqDir is the path of the .2bit or .nib files relative to the current dir
@@ -45,36 +45,38 @@
 #                    blast - similar to NCBI blast format
 #                    blast8- NCBI blast tabular format
 #                    blast9 - NCBI blast tabular format with comments
 #    -maxIntron=N   Sets maximum intron size. Default is 750000.
 #    -genome=name  When using a dynamic gfServer, The genome name is used to
 #                  find the data files relative to the dynamic gfServer root, named
 #                  in the form $genome.2bit, $genome.untrans.gfidx, and $genome.trans.gfidx
-#    -genomeDataDir=path
 #                  When using a dynamic gfServer, this is the dynamic gfServer root directory
 #                  that contained the genome data files.  Defaults to being the root directory.
 
 
 default_option = create_client_option()
 
 
 def client(
     host: str = typer.Argument(
-        ..., help="The name of the machine running the gfServer"
+        ...,
+        help="The name of the machine running the gfServer",
     ),
     port: int = typer.Argument(
-        ..., help="The same port that you started the gfServer with"
+        ...,
+        help="The same port that you started the gfServer with",
     ),
     seqdir: Path = typer.Argument(
         ...,
         dir_okay=True,
         help="The path of the .2bit or .nib files relative to the current dir",
     ),
     infasta: Path = typer.Argument(
-        ..., help="Fasta format file.  May contain multiple records"
+        ...,
+        help="Fasta format file.  May contain multiple records",
     ),
     outpsl: Path = typer.Argument(..., help="where to put the output"),
     tType: str = typer.Option(
         default_option.tType,
         "--type",
         "-t",
         help="Database type. Type is one of: dna, prot, dnax",
@@ -83,18 +85,22 @@
         default_option.qType,
         "--qtype",
         "-q",
         help="Query type. Type is one of: dna, rna, prot, dnax, rnax",
     ),
     prot: bool = typer.Option(False, "--prot", help="Synonymous with -t=prot -q=prot."),
     dots: int = typer.Option(
-        default_option.dots, "--dots", help="Output a dot every N query sequences."
+        default_option.dots,
+        "--dots",
+        help="Output a dot every N query sequences.",
     ),
     nohead: bool = typer.Option(
-        default_option.nohead, "--nohead", help="Suppresses 5-line psl header."
+        default_option.nohead,
+        "--nohead",
+        help="Suppresses 5-line psl header.",
     ),
     minnScore: int = typer.Option(
         default_option.minScore,
         "--minScore",
         help="Sets minimum score.  This is twice the matches minus the mismatches minus some sort of gap penalty.  Default is 30.",
     ),
     minIdentity: int = typer.Option(
@@ -110,19 +116,20 @@
     maxIntron: int = typer.Option(
         default_option.maxIntron,
         "--maxIntron",
         help="Sets maximum intron size. Default is 750000.",
     ),
     genome: str = typer.Option(default_option.genome, "--genome", help="dynamic"),
     genomeDataDir: str = typer.Option(
-        default_option.genomeDataDir, "--genomeDataDir", help="dynamic"
+        default_option.genomeDataDir,
+        "--genomeDataDir",
+        help="dynamic",
     ),
 ):
-    """A client for the genomic finding program that produces a .psl file"""
-
+    """A client for the genomic finding program that produces a .psl file."""
     if prot:
         tType = "prot"
         qType = "prot"
 
     client_option = (
         create_client_option()
         .withHost(host)
```

### Comparing `pxblat-0.2.0/src/pxblat/cli/fa2twobit.py` & `pxblat-0.3.0/src/pxblat/cli/fa2twobit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 
 import typer
+
 from pxblat import fa_to_two_bit
 
 from .log import logger
 
 # faToTwoBit - Convert DNA from fasta to 2bit format
 # usage:
 #    faToTwoBit in.fa [in2.fa in3.fa ...] out.2bit
@@ -37,40 +38,42 @@
     ),
     long: bool = typer.Option(
         False,
         "--long",
         help="Use 64-bit offsets for index. Allow for twoBit to contain more than 4Gb of sequence.",
     ),
     noMask: bool = typer.Option(
-        False, "--nomask", help="Ignore lower-case masking in fa file."
+        False,
+        "--nomask",
+        help="Ignore lower-case masking in fa file.",
     ),
     stripVersion: bool = typer.Option(
         False,
         "--stripVersion",
         help="Strip off version number after '.' for GenBank accessions.",
     ),
     ignoreDups: bool = typer.Option(
         False,
         "--ignoreDups",
         help="Convert first sequence only if there are duplicate sequence names. Use 'twoBitDup' to find duplicate sequences.",
     ),
 ):
-    """Convert DNA from fasta to 2bit format"""
+    """Convert DNA from fasta to 2bit format."""
     for file in infa:
         if not file.exists():
             logger.error(f"{file} not exists")
             raise typer.Abort()
-        elif not file.is_file():
+        if not file.is_file():
             logger.error(f"{file} is not a file")
             raise typer.Abort()
 
     if out2bit.exists():
-        logger.warning(f"{out2bit} exist will be overide")
+        logger.warning(f"{out2bit} exist will be override")
 
     fa_to_two_bit(
         [f.as_posix() for f in infa],
         out2bit.as_posix(),
-        noMask,
-        stripVersion,
-        ignoreDups,
-        long,
+        noMask=noMask,
+        stripVersion=stripVersion,
+        ignoreDups=ignoreDups,
+        useLong=long,
     )
```

### Comparing `pxblat-0.2.0/src/pxblat/cli/server.py` & `pxblat-0.3.0/src/pxblat/cli/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from pathlib import Path
 
 import typer
+from rich import print
+
 from pxblat.extc import UsageStats
-from pxblat.server import create_server_option
+from pxblat.server import (
+    create_server_option,
+    start_server_mt,
+    status_server,
+    stop_server,
+)
 from pxblat.server import files as server_files
-from pxblat.server import start_server_mt
-from pxblat.server import status_server
-from pxblat.server import stop_server
-from rich import print
 
 # gfServer v 37x1 - Make a server to quickly find where DNA occurs in genome
 
 #    To set up a server:
 #       gfServer start host port file(s)
 #       where the files are .2bit or .nib format files specified relative to the current directory
 
@@ -72,15 +75,15 @@
 #      The -perSeqMax functionality can be implemented by creating a file
 #          $rootdir/$genomeDataDir/$genome.perseqmax
 
 
 default_option = create_server_option()
 
 server_app = typer.Typer(
-    help="Make a server to quickly find where DNA occurs in genome"
+    help="Make a server to quickly find where DNA occurs in genome",
 )
 
 
 tileSize: int = typer.Option(
     default_option.tileSize,
     "--tile-size",
     help="Size of n-mers to index.  Default is 11 for nucleotides, 4 for proteins (or translated nucleotides).",
@@ -95,27 +98,31 @@
 minMatch: int = typer.Option(
     default_option.minMatch,
     "--min-match",
     help="Number of n-mer matches that trigger detailed alignment. Default is 2 for nucleotides, 3 for proteins.",
 )
 
 trans: bool = typer.Option(
-    default_option.trans, "--trans", help="Translate database to protein in 6 frames."
+    default_option.trans,
+    "--trans",
+    help="Translate database to protein in 6 frames.",
 )
 
 log: str = typer.Option(
     None,
     "--log",
     exists=True,
     dir_okay=False,
     help="Keep a log file that records server requests.",
 )
 
 mask: bool = typer.Option(
-    default_option.mask, "--mask", help="Use masking from .2bit file."
+    default_option.mask,
+    "--mask",
+    help="Use masking from .2bit file.",
 )
 
 repMatch: int = typer.Option(
     default_option.repMatch,
     "--repMatch",
     help="Number of occurrences of a tile (n-mer) that triggers repeat masking the tile. Default is 1024.",
 )
@@ -162,15 +169,17 @@
     None,
     "--indexFile",
     exists=True,
     dir_okay=False,
     help="Index file create by `gfServer index'.",
 )
 timeout: int = typer.Option(
-    default_option.timeout, "--timeout", help="Timeout in seconds."
+    default_option.timeout,
+    "--timeout",
+    help="Timeout in seconds.",
 )
 
 
 two_bit: Path = typer.Argument(
     ...,
     exists=True,
     dir_okay=False,
@@ -198,21 +207,20 @@
     maxNtSize: int = maxNtSize,
     perSeqMax: Path = perSeqMax,
     canStop: bool = canStop,
     indexFile: Path = indexFile,
     timeout: int = timeout,
     _threads: int = threads,
 ):
-    """To set up a server
+    """To set up a server.
 
     gfServer start host port file(s)
 
     where the files are .2bit or .nib format files specified relative to the current directory
     """
-
     server_option = (
         create_server_option()
         .withTileSize(tileSize)
         .withStepSize(stepSize)
         .withMinMatch(minMatch)
         .withTrans(trans)
         .withMask(mask)
@@ -235,35 +243,40 @@
         server_option.withIndexFile(indexFile.as_posix())
 
     server_option.build()
 
     stat = UsageStats()
 
     start_server_mt(
-        host, port, two_bit.as_posix(), server_option, stat, try_new_port=False
+        host,
+        port,
+        two_bit.as_posix(),
+        server_option,
+        stat,
+        try_new_port=False,
     )
 
 
 @server_app.command()
 def stop(host: str, port: int):
-    """To remove a server"""
+    """To remove a server."""
     stop_server(host, port)
 
 
 @server_app.command()
 def status(
     host: str,
     port: int,
     trans: bool = trans,
 ):
-    """To figure out if server is alive, on static instances get usage statics"""
+    """To figure out if server is alive, on static instances get usage statics."""
     server_option = create_server_option().withTrans(trans)
     server_option.build()
     ret = status_server(host, port, server_option)
     print(ret)
 
 
 @server_app.command()
 def files(host: str, port: int):
-    """To get input file list"""
+    """To get input file list."""
     ret = server_files(host, port)
     print(ret)
```

### Comparing `pxblat-0.2.0/src/pxblat/cli/twobit2fa.py` & `pxblat-0.3.0/src/pxblat/cli/twobit2fa.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 import typer
-from pxblat import two_bit_to_fa
-from pxblat import TwoBitToFaOption
+
+from pxblat import TwoBitToFaOption, two_bit_to_fa
 
 # twoBitToFa - Convert all or part of .2bit file to fasta
 # usage:
 #    twoBitToFa input.2bit output.fa
 # options:
 #    -seq=name       Restrict this to just one sequence.
 #    -start=X        Start at given position in sequence (zero-based).
@@ -25,15 +25,14 @@
 #    or
 #       /path/input.2bit:name:start-end
 
 
 # out: str = typer.Option(
 #        default_option.outputFormat,
 #        "--out",
-#        help="Controls output file format.  Type is one of: psl, pslx, axt, maf, sim4, wublast, blast, blast8, blast9",
 #    ),
 
 
 def twoBitToFa(
     input2bit: Path = typer.Argument(
         ...,
         exists=True,
@@ -48,53 +47,62 @@
         writable=True,
         show_default=False,
         metavar="out.fa",
         help="The output fasta file",
     ),
     seq: str = typer.Option("", "--seq", help="Restrict this to just one sequence."),
     start: int = typer.Option(
-        0, "--start", help="Start at given position in sequence (zero-based)."
+        0,
+        "--start",
+        help="Start at given position in sequence (zero-based).",
     ),
     end: int = typer.Option(
-        0, "--end", help="End at given position in sequence (non-inclusive)."
+        0,
+        "--end",
+        help="End at given position in sequence (non-inclusive).",
     ),
     seqList: str = typer.Option(
-        "", "--seqList", help="File containing list of the desired sequence names"
+        "",
+        "--seqList",
+        help="File containing list of the desired sequence names",
     ),
     noMask: bool = typer.Option(
-        False, "--noMask", help="Convert sequence to all upper case."
+        False,
+        "--noMask",
+        help="Convert sequence to all upper case.",
     ),
     bpt: str = typer.Option("", "--bpt", help="Use bpt index instead of built-in one."),
     bed: str = typer.Option("", "--bed", help="Grab sequences specified by input.bed."),
     bedPos: bool = typer.Option(
         False,
         "--bedPos",
         help="With -bed, use chrom:start-end as the fasta ID in output.fa.",
     ),
     udcDir: str = typer.Option(
-        "", "--udcDir", help="Place to put cache for remote bigBed/bigWigs."
+        "",
+        "--udcDir",
+        help="Place to put cache for remote bigBed/bigWigs.",
     ),
 ):
-    """Convert all or part of .2bit file to fasta"""
-
-    if seqList:
-        if not Path(seqList).exists():
-            raise typer.BadParameter(f"{seqList} does not exist")
-
-    if bpt:
-        if not Path(bpt).exists():
-            raise typer.BadParameter(f"{bpt} does not exist")
-
-    if bed:
-        if not Path(bed).exists():
-            raise typer.BadParameter(f"{bed} does not exist")
-
-    if udcDir:
-        if not Path(udcDir).exists():
-            raise typer.BadParameter(f"{udcDir} does not exist")
+    """Convert all or part of .2bit file to fasta."""
+    if seqList and not Path(seqList).exists():
+        msg = f"{seqList} does not exist"
+        raise typer.BadParameter(msg)
+
+    if bpt and not Path(bpt).exists():
+        msg = f"{bpt} does not exist"
+        raise typer.BadParameter(msg)
+
+    if bed and not Path(bed).exists():
+        msg = f"{bed} does not exist"
+        raise typer.BadParameter(msg)
+
+    if udcDir and not Path(udcDir).exists():
+        msg = f"{udcDir} does not exist"
+        raise typer.BadParameter(msg)
 
     option = TwoBitToFaOption()
     option.withSeq(seq).withStart(start).withEnd(end).withSeqList(seqList).withNoMask(
-        noMask
+        noMask,
     ).withBpt(bpt).withBed(bed).withBedPos(bedPos).withUdcDir(udcDir).build()
 
     two_bit_to_fa(input2bit, outputfa, option=option)
```

### Comparing `pxblat-0.2.0/src/pxblat/extc/__init__.py` & `pxblat-0.3.0/src/pxblat/extc/__init__.py`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/__init__.pyi` & `pxblat-0.3.0/src/pxblat/extc/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Bindings for ::cppbinding namespace"""
 from __future__ import annotations
 import pxblat._extc.cppbinding
 import typing
 
 __all__ = [
     "IntStruct",
-    "Signal",
     "TwoBitToFaOption",
     "UsageStats",
     "buildIndex",
     "faToTwoBit",
     "genoFindDirect",
     "genoPcrDirect",
     "getFileList",
@@ -40,27 +39,14 @@
     "twoBitToFa",
 ]
 
 class IntStruct:
     def __init__(self, arg0: int) -> None: ...
     pass
 
-class Signal:
-    def __init__(self) -> None: ...
-    def __str__(self) -> str: ...
-    @property
-    def isReady(self) -> bool:
-        """
-        :type: bool
-        """
-    @isReady.setter
-    def isReady(self, arg0: bool) -> None:
-        pass
-    pass
-
 class TwoBitToFaOption:
     def __getstate__(self) -> tuple: ...
     @typing.overload
     def __init__(self) -> None: ...
     @typing.overload
     def __init__(self, arg0: TwoBitToFaOption) -> None: ...
     def __setstate__(self, arg0: tuple) -> None: ...
```

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/binder/_extc.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/binder/_extc.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/binder/faToTwoBit.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/binder/faToTwoBit.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfClient.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/binder/gfClient.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 		cl.def("withSeqDir", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withSeqDir, "C++: cppbinding::ClientOption::withSeqDir(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("SeqDir_"));
 		cl.def("withInName", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withInName, "C++: cppbinding::ClientOption::withInName(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("inName_"));
 		cl.def("withOutName", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withOutName, "C++: cppbinding::ClientOption::withOutName(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("outName_"));
 		cl.def("withInSeq", (struct cppbinding::ClientOption & (cppbinding::ClientOption::*)(const std::string &)) &cppbinding::ClientOption::withInSeq, "C++: cppbinding::ClientOption::withInSeq(const std::string &) --> struct cppbinding::ClientOption &", pybind11::return_value_policy::automatic, pybind11::arg("inseq_"));
 		cl.def("to_string", (std::string (cppbinding::ClientOption::*)() const) &cppbinding::ClientOption::to_string, "C++: cppbinding::ClientOption::to_string() const --> std::string");
 
 		cl.def("__str__", [](cppbinding::ClientOption const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
+		cl.def("__repr__", [](cppbinding::ClientOption const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
 
         cl.def(pybind11::pickle([](const cppbinding::ClientOption& p){
                return pybind11::make_tuple(p.hostName, p.portName,p.tType, p.qType, p.dots,
                                            p.nohead, p.minScore, p.minIdentity,
                                            p.outputFormat, p.maxIntron, p.genome,
                                            p.genomeDataDir, p.isDynamic, p.SeqDir,
                                            p.inName, p.outName, p.inSeq); },
```

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfServer.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/binder/gfServer.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -20,34 +20,28 @@
 	PYBIND11_DECLARE_HOLDER_TYPE(T, std::shared_ptr<T>)
 	PYBIND11_DECLARE_HOLDER_TYPE(T, T*)
 	PYBIND11_MAKE_OPAQUE(std::shared_ptr<void>)
 #endif
 
 void bind_gfServer(std::function< pybind11::module &(std::string const &namespace_) > &M)
 {
-	{ // cppbinding::Signal file:gfServer.hpp line:39
-		pybind11::class_<cppbinding::Signal, std::shared_ptr<cppbinding::Signal>> cl(M("cppbinding"), "Signal", "");
-		cl.def( pybind11::init( [](){ return new cppbinding::Signal(); } ) );
-		cl.def_readwrite("isReady", &cppbinding::Signal::isReady);
-
-		cl.def("__str__", [](cppbinding::Signal const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
-	}
 	{ // cppbinding::UsageStats file:gfServer.hpp line:45
 		pybind11::class_<cppbinding::UsageStats, std::shared_ptr<cppbinding::UsageStats>> cl(M("cppbinding"), "UsageStats", "");
 		cl.def( pybind11::init( [](){ return new cppbinding::UsageStats(); } ) );
 		cl.def_readwrite("baseCount", &cppbinding::UsageStats::baseCount);
 		cl.def_readwrite("blatCount", &cppbinding::UsageStats::blatCount);
 		cl.def_readwrite("aaCount", &cppbinding::UsageStats::aaCount);
 		cl.def_readwrite("pcrCount", &cppbinding::UsageStats::pcrCount);
 		cl.def_readwrite("warnCount", &cppbinding::UsageStats::warnCount);
 		cl.def_readwrite("noSigCount", &cppbinding::UsageStats::noSigCount);
 		cl.def_readwrite("missCount", &cppbinding::UsageStats::missCount);
 		cl.def_readwrite("trimCount", &cppbinding::UsageStats::trimCount);
 
 		cl.def("__str__", [](cppbinding::UsageStats const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
+		cl.def("__repr__", [](cppbinding::UsageStats const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
 
         cl.def(pybind11::pickle([](const cppbinding::UsageStats &p) { // __getstate__
             return pybind11::make_tuple(p.baseCount, p.blatCount, p.aaCount, p.pcrCount, p.warnCount
                                                             , p.noSigCount, p.missCount, p.trimCount);
 
              },
             [](pybind11::tuple t) { // __setstate__
@@ -119,14 +113,15 @@
 		cl.def("withPerSeqMax", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(std::string)) &cppbinding::ServerOption::withPerSeqMax, "C++: cppbinding::ServerOption::withPerSeqMax(std::string) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("perSeqMax_"));
 		cl.def("withNoSimpRepMask", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(bool)) &cppbinding::ServerOption::withNoSimpRepMask, "C++: cppbinding::ServerOption::withNoSimpRepMask(bool) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("noSimpRepMask_"));
 		cl.def("withIndexFile", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(std::string)) &cppbinding::ServerOption::withIndexFile, "C++: cppbinding::ServerOption::withIndexFile(std::string) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("indexFile_"));
 		cl.def("withTimeout", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withTimeout, "C++: cppbinding::ServerOption::withTimeout(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("timeout_"));
 		cl.def("withThreads", (struct cppbinding::ServerOption & (cppbinding::ServerOption::*)(int)) &cppbinding::ServerOption::withThreads, "C++: cppbinding::ServerOption::withThreads(int) --> struct cppbinding::ServerOption &", pybind11::return_value_policy::automatic, pybind11::arg("threads_"));
 
 		cl.def("__str__", [](cppbinding::ServerOption const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
+		cl.def("__repr__", [](cppbinding::ServerOption const &o) -> std::string { std::ostringstream s; using namespace cppbinding; s << o; return s.str(); } );
 
         cl.def(pybind11::pickle(
             [](const cppbinding::ServerOption &p) { // __getstate__
 
                 return pybind11::make_tuple(p.canStop,p.log,p.logFacility, p.mask, p.maxAaSize, p.maxDnaHits,
                                             p.maxGap, p.maxNtSize, p.maxTransHits, p.minMatch, p.repMatch,
                                             p.seqLog, p.ipLog, p.debugLog, p.tileSize, p.stepSize,p.trans,
```

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/binder/gfServer_1.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/binder/gfServer_1.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/binder/pygfServer.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/binder/pygfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/binder/twoBitToFa.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/binder/twoBitToFa.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/bs_thread_pool.hpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/bs_thread_pool.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/dbg.h` & `pxblat-0.3.0/src/pxblat/extc/bindings/dbg.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/faToTwoBit.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/faToTwoBit.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/faToTwoBit.hpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/faToTwoBit.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/gfClient.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/gfClient.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/gfClient.hpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/gfClient.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/gfServer.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/gfServer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1034,15 +1034,14 @@
   }
   logGenoFindIndex(gfIdx);
 
   /* Set up socket.  Get ready to listen to it. */
   socketHandle = netAcceptingSocket(port, 100);
   if (socketHandle < 0) errAbort("Fatal Error: Unable to open listening socket on port %d.", port);
 
-  // signal.isReady = true;
   logInfo("Server ready for queries!");
   printf("Server ready for queries!\n");
 
   int connectFailCount = 0;
   for (;;) {
     ZeroVar(&fromAddr);
     fromLen = sizeof(fromAddr);
@@ -1729,20 +1728,14 @@
   os << ", noSigCount: " << stats.noSigCount;
   os << ", missCount: " << stats.missCount;
   os << ", trimCount: " << stats.trimCount;
   os << ")";
   return os;
 }
 
-std::ostream &operator<<(std::ostream &os, const Signal &signal) {
-  os << "Signal(";
-  os << "signal: " << std::boolalpha << signal.isReady;
-  return os;
-}
-
 int globalint = 1;
 
 void test_stdout() {
   printf("stdout\n");
   globalint += 1;
   printf("globalint is %d\n", globalint);
 }
```

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/gfServer.hpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/gfServer.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -35,20 +35,14 @@
 #include "nib.h"
 #include "portable.h"
 #include "trans3.h"
 #include "twoBit.h"
 
 namespace cppbinding {
 
-struct Signal {
-  bool isReady{};
-  Signal() = default;
-  friend std::ostream &operator<<(std::ostream &os, const Signal &signal);
-};
-
 struct UsageStats {
   long baseCount{0}, blatCount{0}, aaCount{0}, pcrCount{0};
   int warnCount{0};
   int noSigCount{0};
   int missCount{0};
   int trimCount{0};
   UsageStats() = default;
```

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/pygfServer.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/pygfServer.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/pygfServer.hpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/pygfServer.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/twoBitToFa.cpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/twoBitToFa.cpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/bindings/twoBitToFa.hpp` & `pxblat-0.3.0/src/pxblat/extc/bindings/twoBitToFa.hpp`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/blat.c` & `pxblat-0.3.0/src/pxblat/extc/blat.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/faToTwoBit.c` & `pxblat-0.3.0/src/pxblat/extc/faToTwoBit.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/gfClient.c` & `pxblat-0.3.0/src/pxblat/extc/gfClient.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/gfServer.c` & `pxblat-0.3.0/src/pxblat/extc/gfServer.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/bandExt.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/bandExt.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/base64.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/base64.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/cheapcgi.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/cheapcgi.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/filePath.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/filePath.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/gfxPoly.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/gfxPoly.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/hex.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/hex.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/htmlPage.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/htmlPage.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/htmshell.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/htmshell.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/internet.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/internet.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/kxTok.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/kxTok.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/memgfx.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/memgfx.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/mime.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/mime.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/portimpl.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/portimpl.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/aux/rbTree.h` & `pxblat-0.3.0/src/pxblat/extc/include/aux/rbTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/aliType.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/aliType.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/asParse.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/asParse.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/axt.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/axt.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/bPlusTree.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/bPlusTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/basicBed.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/basicBed.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/binRange.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/binRange.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/bits.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/bits.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/chain.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/chain.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/chainBlock.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/chainBlock.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/common.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/common.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/dlist.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/dlist.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/dnaseq.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/dnaseq.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/dnautil.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/dnautil.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/dystring.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/dystring.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/errAbort.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/errAbort.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/errCatch.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/errCatch.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/fa.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/fa.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/fuzzyFind.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/fuzzyFind.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/genoFind.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/genoFind.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/gfClientLib.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/gfClientLib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/gfInternal.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/gfInternal.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/hash.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/hash.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/htmlColor.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/htmlColor.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/linefile.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/linefile.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/localmem.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/localmem.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/maf.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/maf.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/memalloc.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/memalloc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/net.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/net.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/netlib.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/netlib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/nib.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/nib.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/obscure.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/obscure.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/ooc.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/ooc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/options.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/options.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/patSpace.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/patSpace.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/pipeline.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/pipeline.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/portable.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/portable.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/psl.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/psl.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/rangeTree.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/rangeTree.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/repMask.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/repMask.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/sig.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/sig.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/sqlList.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/sqlList.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/sqlNum.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/sqlNum.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/supStitch.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/supStitch.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/tokenizer.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/tokenizer.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/trans3.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/trans3.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/twoBit.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/twoBit.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/udc.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/udc.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/core/verbose.h` & `pxblat-0.3.0/src/pxblat/extc/include/core/verbose.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/include/net/log.h` & `pxblat-0.3.0/src/pxblat/extc/include/net/log.h`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/axt.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/axt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/bandExt.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/bandExt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/base64.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/base64.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/binRange.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/binRange.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/blastOut.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/blastOut.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/cheapcgi.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/cheapcgi.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/ffSeedExtend.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/ffSeedExtend.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/filePath.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/filePath.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/hex.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/hex.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/htmlPage.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/htmlPage.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/htmshell.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/htmshell.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/https.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/https.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/intExp.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/intExp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/internet.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/internet.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/maf.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/maf.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/mafFromAxt.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/mafFromAxt.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/mime.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/mime.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/net.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/net.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/netlib.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/netlib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/ooc.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/ooc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/patSpace.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/patSpace.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/portimpl.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/portimpl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/rangeTree.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/rangeTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/rbTree.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/rbTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/repMask.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/repMask.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/servBrcMcw.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/servBrcMcw.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/servCrunx.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/servCrunx.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/servcis.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/servcis.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/servmsII.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/servmsII.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/servpws.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/servpws.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/sqlList.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/sqlList.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/sqlNum.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/sqlNum.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/aux/wildcmp.c` & `pxblat-0.3.0/src/pxblat/extc/src/aux/wildcmp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/aliType.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/aliType.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/asParse.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/asParse.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/bPlusTree.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/bPlusTree.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/basicBed.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/basicBed.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/bits.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/bits.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/chain.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/chain.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/chainBlock.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/chainBlock.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/common.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/common.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/dlist.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/dlist.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/dnaseq.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/dnaseq.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/dnautil.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/dnautil.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/dystring.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/dystring.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/errAbort.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/errAbort.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/errCatch.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/errCatch.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/fa.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/fa.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/ffAli.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/ffAli.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/ffAliHelp.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/ffAliHelp.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/ffScore.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/ffScore.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/fuzzyFind.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/fuzzyFind.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/genoFind.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/genoFind.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/gfBlatLib.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/gfBlatLib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/gfClientLib.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/gfClientLib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/gfInternal.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/gfInternal.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/gfOut.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/gfOut.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/hash.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/hash.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/htmlColor.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/htmlColor.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/kxTok.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/kxTok.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/linefile.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/linefile.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/localmem.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/localmem.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/memalloc.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/memalloc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/nib.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/nib.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/obscure.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/obscure.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/options.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/options.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/osunix.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/osunix.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/pipeline.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/pipeline.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/psl.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/psl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/servcl.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/servcl.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/supStitch.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/supStitch.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/tokenizer.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/tokenizer.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/trans3.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/trans3.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/twoBit.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/twoBit.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/udc.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/udc.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/core/verbose.c` & `pxblat-0.3.0/src/pxblat/extc/src/core/verbose.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/net/gfNet.c` & `pxblat-0.3.0/src/pxblat/extc/src/net/gfNet.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/src/net/log.c` & `pxblat-0.3.0/src/pxblat/extc/src/net/log.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/extc/twoBitToFa.c` & `pxblat-0.3.0/src/pxblat/extc/twoBitToFa.c`

 * *Files identical despite different names*

### Comparing `pxblat-0.2.0/src/pxblat/server/basic.py` & `pxblat-0.3.0/src/pxblat/server/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,33 @@
+from __future__ import annotations
+
 import errno
 import socket
 import time
-import typing as t
 import warnings
 from collections import Counter
 from multiprocessing import Process
 
 from deprecated import deprecated  # type: ignore
-from pxblat.extc import pygetFileList
-from pxblat.extc import pyqueryServer
-from pxblat.extc import pystartServer
-from pxblat.extc import ServerOption
-from pxblat.extc import startServer
-from pxblat.extc import UsageStats
-
-from .status import Status
-from .utils import logger
-
-DEFAULT_PORT = 65000
-
-
-def check_host_port(host: str, port: int) -> None:
-    """Check if the given host and port are valid.
-
-    Args:
-        host (str): The host to check.
-        port (int): The port to check.
-
-    Returns:
-        None
 
-    Raises:
-        RuntimeError: If the host is not a string or the port is not an integer.
-
-    This function checks if the given host and port are valid. The host must be a string and the port must be an integer.
-    If either of these conditions are not met, a RuntimeError is raised with an appropriate error message.
+from pxblat.extc import (
+    ServerOption,
+    UsageStats,
+    pygetFileList,
+    pyqueryServer,
+    pystartServer,
+    startServer,
+)
 
-    Example:
-        >>> check_host_port("localhost", 8080)
-        None
-    """
-    if not isinstance(host, str):
-        raise RuntimeError("host must be str")
+from .status import Status
 
-    if not isinstance(port, int):
-        raise RuntimeError("port must be number")
+MAX_PORT = 65535
 
 
-def check_port_in_use(host: str, port: int = DEFAULT_PORT, tries: int = 3) -> bool:
+def check_port_in_use(host: str, port: int, tries: int = 3) -> bool:
     """Check if a given port on a host is in use.
 
     Args:
         host (str): The hostname or IP address of the host to check.
         port (int, optional): The port number to check. Defaults to DEFAULT_PORT.
         tries (int, optional): The number of times to attempt the check. Defaults to 3.
 
@@ -65,154 +41,159 @@
     This function attempts to connect to the specified host and port using the socket library. It will attempt the connection
     a number of times specified by the tries argument. If the connection is successful, it will return True, indicating that
     the port is in use. If the connection fails, it will return False.
 
     If the host argument is not a string, a TypeError will be raised. If the port argument is not a valid port number, a
     ValueError will be raised.
 
-    Example usage:
-    >>> check_port_in_use('localhost', 8080)
-    True
+    Example:
+        >>> check_port_in_use('localhost', 8080)
+        True
     """
     res = [_check_port_in_use_by_connect(host, port) for _ in range(tries)]
     counter = Counter(res)
-    logger.debug(f"{res}")
     return counter[True] > counter[False]
 
 
 def _check_port_in_use_by_status(
-    host: str, port: int, gfserver_option: ServerOption
+    host: str,
+    port: int,
+    server_option: ServerOption,
 ) -> bool:
-    """Check the port is in use by status_server
+    """Check the port is in use by status_server.
 
     Args:
         host: host name
         port: port number
-        gfserver_option: server option for the opening server
+        server_option: server option for the opening server
 
     Returns:
         True if the port is in use
 
-    note:
+    Note:
         The server option can be default value and will not influence result
         Also, it can detect if the port is opened by gfServer as well
     """
-    logger.debug(f"check port {host}:{port}")
-    return check_server_status(host, port, gfserver_option)
+    return check_server_status(host, port, server_option)
 
 
 def _check_port_in_use_by_connect(host: str, port: int):
-    """Check the port is in use by connect to the port
+    """Check the port is in use by connect to the port.
 
     Args:
         host: host name
         port: port number
 
     Returns:
         True if the port is in use
 
-    note:
+    Note:
         The function has same feature as `_check_port_in_use_by_status`
         It check the port if it is in use by connect to the port.
         But it cannot detect if the port is opened by gfServer
     """
     return check_port_open(host, port)
 
 
 @deprecated(
-    reason="The func will generate false alarm. Please use `_check_port_in_use_by_status` or  `_check_port_in_use_by_connect` instead"
+    reason="The func will generate false alarm. Please use `_check_port_in_use_by_status` or  `_check_port_in_use_by_connect` instead",
 )
-def _check_port_in_use_by_bind(host: str, port: int = DEFAULT_PORT):
-    """Check the port is in use by bind to the port
+def _check_port_in_use_by_bind(host: str, port: int):
+    """Check the port is in use by bind to the port.
 
     Args:
         host: host name
         port: port number
 
     Returns:
         True if the port is in use
 
-    note:
+    Note:
         The function check the port if it is in use by bind to the port.
-        It is not reliable as `_check_port_in_use_by_connect` or `_check_port_in_use_by_status`
+        It is not reliable as ``_check_port_in_use_by_connect`` or
+        ``_check_port_in_use_by_status``
+
     """
-    logger.debug(f"check port {host}:{port}")
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     try:
         s.bind((host, port))
-    except socket.error as e:
-        logger.debug(f"port {host}:{port} is in use {e}")
+    except OSError as e:
         if e.errno == errno.EADDRINUSE:
             return True
 
         raise e
 
     s.close()
     return False
 
 
 def wait_server_ready(
-    host: str, port: int, timeout: int = 60, gfserver_option=None
+    host: str,
+    port: int,
+    timeout: int = 60,
+    server_option=None,
 ) -> None:
     """Wait for a server to become ready by checking if a given port is open or if a specific server status is reached.
 
     Args:
         host (str): The hostname or IP address of the server to check.
         port (int): The port number to check for open status.
         timeout (int, optional): The maximum number of seconds to wait for the server to become ready. Defaults to 60.
-        gfserver_option (str, optional): The specific server status to check for. If None, the function will check for an open port. Defaults to None.
+        server_option (str, optional): The specific server status to check for. If None, the function will check for an open port. Defaults to None.
 
     Raises:
         RuntimeError: If the server does not become ready within the specified timeout.
 
     Returns:
         None
     """
     start = time.perf_counter()
 
-    if gfserver_option is None:
+    if server_option is None:
         warnings.warn(
             "Use `check_server_status` instead of `check_port_open` when wait for ready",
             stacklevel=1,
         )
         while not check_port_open(host, port):
             time.sleep(1)
             if time.perf_counter() - start > timeout:
-                raise RuntimeError("wait for server ready timeout")
+                msg = "wait for server ready timeout"
+                raise RuntimeError(msg)
     else:
-        while not check_server_status(host, port, gfserver_option):
+        while not check_server_status(host, port, server_option):
             time.sleep(1)
             if time.perf_counter() - start > timeout:
-                raise RuntimeError("wait for server ready timeout")
+                msg = "wait for server ready timeout"
+                raise RuntimeError(msg)
 
 
 def check_server_status(
     host: str,
     port: int,
-    gfserver_option: ServerOption,
+    server_option: ServerOption,
 ) -> bool:
     """Check the status of a server by attempting to connect to it using the specified host, port, and gfserver_option.
 
     Args:
         host (str): The hostname or IP address of the server to check.
         port (int): The port number to use when attempting to connect to the server.
-        gfserver_option (ServerOption): The gfserver option to use when attempting to connect to the server.
+        server_option (ServerOption): The gfserver option to use when attempting to connect to the server.
 
     Returns:
         bool: True if the server is running and accepting connections, False otherwise.
 
     Raises:
         ConnectionRefusedError: If the server is not running or is not accepting connections.
 
     Example:
         >>> check_server_status('localhost', 8080, ServerOption)
         True
     """
     try:
-        status_server(host, port, gfserver_option)
+        status_server(host, port, server_option)
     except ConnectionRefusedError:
         return False
     else:
         return True
 
 
 def check_port_open(host: str, port: int) -> bool:
@@ -225,43 +206,46 @@
     Returns:
         True if the port is open and can accept message, otherwise False.
     """
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         return s.connect_ex((host, port)) == 0
 
 
-def gfSignature() -> str:
+def _gfSignature() -> str:
+    """Get the gfSignature."""
     return "0ddf270562684f29"
 
 
 def status_server(
-    host: str, port: int, options: ServerOption, instance=False
-) -> t.Union[Status, t.Dict[str, str]]:
+    host: str,
+    port: int,
+    server_option: ServerOption,
+    *,
+    instance=False,
+) -> Status | dict[str, str]:
     """Get the status of a running server.
 
     Args:
         host (str): The hostname or IP address of the server to check.
         port (int): The port number to use when attempting to connect to the server.
-        options (ServerOption): The gfserver option to use when attempting to connect to the server.
+        server_option (ServerOption): The gfserver option to use when attempting to connect to the server.
         instance (bool, optional): If True, return a Status object instead of a dictionary. Defaults to False.
 
     Returns:
         Union[Status, Dict[str, str]]: A dictionary or Status object containing the status information for the server.
 
     Example:
         >>> status_server('localhost', 8080, ServerOption, instance=True)
         Status(uptime='0', queries='0', sequences='0', bytes='0', memory='0', threads='0', connections='0')
     """
-    if not options.genome:
-        message = f"{gfSignature()}status".encode()
+    if not server_option.genome:
+        message = f"{_gfSignature()}status".encode()
     else:
-        temp = "transInfo" if options.trans else "untransInfo"
-        message = (
-            f"{gfSignature()}{temp} {options.genome} {options.genomeDataDir}".encode()
-        )
+        temp = "transInfo" if server_option.trans else "untransInfo"
+        message = f"{_gfSignature()}{temp} {server_option.genome} {server_option.genomeDataDir}".encode()
 
     data = b""
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.connect((host, port))
         s.sendall(message)
         while True:
             data += s.recv(1024)
@@ -310,16 +294,15 @@
 
     This function stops a running server by sending a "quit" message to the server. The function takes the hostname and port number
     of the server as arguments. The function returns None.
 
     Example:
         >>> stop_server('localhost', 8080)
     """
-
-    message = f"{gfSignature()}quit".encode()
+    message = f"{_gfSignature()}quit".encode()
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         s.connect((host, port))
         s.sendall(message)
 
 
 def files(host: str, port: int) -> list[str]:
     """Get a list of files available on the server.
@@ -334,22 +317,28 @@
     This function retrieves a list of files available on the server by sending a "files" message to the server. The function takes
     the hostname and port number of the server as arguments. The function returns a list of file names available on the server.
 
     Example:
         >>> files('localhost', 8080)
         ['file1', 'file2', 'file3']
     """
-
     ret_str = pygetFileList(host, str(port))
-    assert ret_str, "ret_str cannot be empty"
+    if ret_str == "":
+        raise ValueError
     return [file for file in ret_str.split("\n") if file]
 
 
 def server_query(
-    intype: str, host: str, port: int, faName: str, isComplex: bool, isProt: bool
+    intype: str,
+    host: str,
+    port: int,
+    faName: str,
+    *,
+    isComplex: bool,
+    isProt: bool,
 ):
     """Query a running server with a sequence.
 
     Args:
         intype (str): The type of input sequence. Must be one of 'dna', 'rna', or 'protein'.
         host (str): The hostname or IP address of the server to query.
         port (int): The port number to use when attempting to connect to the server.
@@ -364,132 +353,148 @@
     type of input sequence, hostname, port number, sequence name, and whether the sequence is complex or a protein sequence as
     arguments. The function returns the result of the query as a string.
 
     Example:
         >>> server_query('dna', 'localhost', 8080, 'sequence1', False, False)
         'result1'
     """
-    re_str = pyqueryServer(intype, host, str(port), faName, isComplex, isProt)
-    return re_str
+    return pyqueryServer(intype, host, str(port), faName, isComplex, isProt)
 
 
 def start_server(
     host: str,
     port: int,
     two_bit_file: str,
-    option: ServerOption,
+    server_option: ServerOption,
     stat: UsageStats,
 ):
     """Start a server in blocking mode.
 
     Args:
         host (str): The hostname or IP address to bind the server to.
         port (int): The port number to bind the server to.
         two_bit_file (str): The path to the 2bit file to use for the server.
-        option (ServerOption): The options to use for the server.
+        server_option (ServerOption): The options to use for the server.
         stat (UsageStats): The usage statistics for the server.
 
     Returns:
         None
 
     This function starts a server in blocking mode by calling the pystartServer function with the given arguments. The function
     takes the hostname, port number, 2bit file path, server options, and usage statistics as arguments. The function returns None.
 
     Example:
         >>> start_server('localhost', 8080, '/path/to/2bit/file', ServerOption, UsageStats())
     """
-    return startServer(host, str(port), 1, [two_bit_file], option, stat)
+    return startServer(host, str(port), 1, [two_bit_file], server_option, stat)
 
 
 def start_server_mt(
     host: str,
     port: int,
     two_bit_file: str,
-    option: ServerOption,
+    server_option: ServerOption,
     stat: UsageStats,
+    *,
     use_others: bool = False,
-    timeout: int = 60,
     try_new_port: bool = True,
 ):
-    """Start server in blocking mode.
+    """Starts a server on a new thread.
+
+    This function attempts to start a server on the given host and port, using the provided .2bit file, options, and usage stats.
+    If the port is in use, it either waits for the server to be ready, tries a new port, or raises an error, depending on the options.
 
     Args:
-        host: host name
-        port: port number
-        two_bit_file: two bit file path
-        option: gfServeoption
-        stat: statastic for server
+        host (str): The hostname or IP address to start the server on.
+        port (int): The initial port number to try to start the server on.
+        two_bit_file (str): The .2bit file to use for the server.
+        server_option (ServerOption): The options to use when starting the server.
+        stat (UsageStats): The usage stats to use for the server.
+        use_others (bool, optional): Whether to use the port even if it is already in use. Defaults to False.
+        try_new_port (bool, optional): Whether to try a new port if the initial port is in use. Defaults to True.
+
+    Raises:
+        ValueError: If the port is in use and neither 'use_others' nor 'try_new_port' is True.
+        Exception: If there is any other error in starting the server.
     """
     try:
         if check_port_in_use(host, port):
             if use_others:
                 pass
-                # wait_server_ready(host, port, timeout)
-                # status_server(host, port, option)
             elif try_new_port:
                 port = find_free_port(host, start=port + 1)
-                pystartServer(host, str(port), 1, [two_bit_file], option, stat)
+                pystartServer(host, str(port), 1, [two_bit_file], server_option, stat)
             else:
-                raise ValueError(f"The port {port} is used")
+                msg = f"The port {port} is used"
+                raise ValueError(msg)
         else:
-            pystartServer(host, str(port), 1, [two_bit_file], option, stat)
+            pystartServer(host, str(port), 1, [two_bit_file], server_option, stat)
     except Exception as e:
         raise e
 
 
 def start_server_mt_nb(
     host: str,
     port: int,
     two_bit_file: str,
-    option: ServerOption,
+    server_option: ServerOption,
     stat: UsageStats,
+    *,
     use_others: bool = False,
-    timeout: int = 60,
     try_new_port: bool = True,
 ) -> Process:
-    """Start server in non-blocking mode.
+    """Starts a server on a new thread and immediately returns a Process object.
+
+    This function calls `start_server_mt` to start a server on the given host and port, using the provided .2bit file, options, and usage stats,
+    in a new thread, and immediately returns a Process object for the new thread.
 
     Args:
-        host: host name
-        port: port number
-        two_bit_file: two bit file path
-        option: gfServeoption
-        stat: statastic for server
+        host (str): The hostname or IP address to start the server on.
+        port (int): The initial port number to try to start the server on.
+        two_bit_file (str): The .2bit file to use for the server.
+        server_option (ServerOption): The options to use when starting the server.
+        stat (UsageStats): The usage stats to use for the server.
+        use_others (bool, optional): Whether to use the port even if it is already in use. Defaults to False.
+        try_new_port (bool, optional): Whether to try a new port if the initial port is in use. Defaults to True.
 
     Returns:
-        Process: a process object
+        Process: A Process object for the newly started thread.
     """
     process = Process(
         target=start_server_mt,
         args=(
             host,
             port,
             two_bit_file,
-            option,
+            server_option,
             stat,
-            use_others,
-            timeout,
-            try_new_port,
         ),
+        kwargs={
+            "use_others": use_others,
+            "try_new_port": try_new_port,
+        },
         daemon=True,
     )
 
     process.start()
     return process
 
 
-def find_free_port(host: str, start: int = DEFAULT_PORT, end: int = 65535) -> int:
-    """Find an available port in the range of [start, end].
+def find_free_port(host: str, start: int, end: int = MAX_PORT) -> int:
+    """Find an available port in the range of [start, end).
+
     Args:
         host: Hostname
         start: Start port number
-        end: End port number
+        end: End port number.
     """
-    assert start < end
+    if start > end:
+        raise ValueError
 
     for port in range(start, end):
         try:
             if not check_port_in_use(host, port):
                 return port
-        except socket.error as e:
+        except OSError as e:
             raise e
-    raise RuntimeError(f"Cannot find available port in range [{start}, {end}]")
+    msg = f"Cannot find available port in range [{start}, {end}]"
+    raise RuntimeError(msg)
```

### Comparing `pxblat-0.2.0/src/pxblat/server/server.py` & `pxblat-0.3.0/src/pxblat/server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,86 @@
+from __future__ import annotations
+
 import typing as t
 from contextlib import ContextDecorator
 from multiprocessing import Process
-from pathlib import Path
-from typing import Union
 
-from pxblat.extc import pystartServer
-from pxblat.extc import ServerOption
-from pxblat.extc import UsageStats
-
-from .basic import check_port_in_use
-from .basic import files
-from .basic import find_free_port
-from .basic import logger
-from .basic import server_query
-from .basic import status_server
-from .basic import stop_server
-from .basic import wait_server_ready
-from .status import Status
+from pxblat.extc import ServerOption, UsageStats, pystartServer
+
+from .basic import (
+    check_port_in_use,
+    files,
+    find_free_port,
+    server_query,
+    status_server,
+    stop_server,
+    wait_server_ready,
+)
+
+if t.TYPE_CHECKING:
+    from pathlib import Path
+
+    from .status import Status
 
 
 def _pystartServer(
     hostName: str,
     portName: str,
-    seqFiles: t.List[str],
+    seqFiles: list[str],
     options: ServerOption,
     stats: UsageStats,
 ):
     pystartServer(hostName, portName, len(seqFiles), seqFiles, options, stats)
 
 
 def create_server_option() -> ServerOption:
-    """
-    Creates a new ServerOption object with default values.
+    """Creates a new ServerOption object with default values.
 
     Returns:
         ServerOption: A new ServerOption object with default values.
     """
     return ServerOption()
 
 
 class Server(ContextDecorator):
+    """A context manager and decorator for managing a server process.
+
+    This class can be used as a context manager or decorator to manage a server process. It starts the server with the given
+    options, and can run it as a daemon process or block until it is ready.
+
+    Attributes:
+        host (str): The hostname or IP address to bind the server to.
+        port (int): The port number to bind the server to.
+        two_bit (Union[Path, str]): The path to the 2bit file or the URL of the 2bit file.
+        option (ServerOption): The options to use when starting the server.
+        daemon (bool, optional): Whether to run the server as a daemon process. Defaults to True.
+        use_others (bool, optional): Whether to allow other users to access the server. Defaults to False.
+        timeout (int, optional): The number of seconds to wait for the server to start. Defaults to 60.
+        block (bool, optional): Whether to block until the server is ready. Defaults to False.
+
+    Raises:
+        ValueError: If the given two_bit file or URL is invalid.
+        OSError: If there is an error starting the server process.
+
+    Order:
+        -10
+    """
+
     def __init__(
         self,
         host: str,
         port: int,
-        two_bit: Union[Path, str],
+        two_bit: Path | str,
         option: ServerOption,
+        *,
         daemon=True,
         use_others: bool = False,
         timeout: int = 60,
         block: bool = False,
-    ):
+    ) -> None:
         """Initializes a gfServer object with the given parameters.
 
         Args:
             host (str): The hostname or IP address to bind the server to.
             port (int): The port number to bind the server to.
             two_bit (Union[Path, str]): The path to the 2bit file or the URL of the 2bit file.
             option (ServerOption): The options to use when starting the server.
@@ -85,70 +111,76 @@
         self._block = block
         self._is_ready = False
         self._is_open = True
         self._process = None
 
     @property
     def host(self):
+        """The hostname or IP address to bind the server to."""
         return self._host
 
     @host.setter
     def host(self, value: str):
+        """Sets the hostname or IP address to bind the server to."""
         self._host = value
 
     @property
     def port(self) -> int:
+        """The port number to bind the server to."""
         return self._port
 
     @port.setter
     def port(self, value: int):
+        """Sets the port number to bind the server to."""
         self._port = value
 
     def _start_b(self):
         """Start server in blocking mode."""
         two_bit_file = (
             self.two_bit if isinstance(self.two_bit, str) else self.two_bit.as_posix()
         )
         try:
             if check_port_in_use(self.host, self.port):
                 if self.use_others:
                     self._is_open = False
                     # WARN: Use server that is already open. However, the server may be not opened by gfServer <05-16-23>
                     # Hence, the `wait_server_ready` may be timeout.
 
-                    # wait_server_ready(host, port, timeout)
                 else:
                     self._is_open = True
                     new_port = find_free_port(self.host, start=self.port + 1)
                     self.port = new_port
                     pystartServer(
                         self.host,
                         str(self.port),
                         1,
                         [two_bit_file],
                         self.option,
                         self.stat,
                     )
             else:
                 pystartServer(
-                    self.host, str(self.port), 1, [two_bit_file], self.option, self.stat
+                    self.host,
+                    str(self.port),
+                    1,
+                    [two_bit_file],
+                    self.option,
+                    self.stat,
                 )
         except Exception as e:
             raise e
 
     def _start_nb(self):
         two_bit_file = (
             self.two_bit if isinstance(self.two_bit, str) else self.two_bit.as_posix()
         )
         try:
             if check_port_in_use(self.host, self.port):
-                logger.debug(f"{self.port} port in use")
                 if self.use_others:
                     self._is_open = False
-                    # wait_server_ready(host, port, timeout)
                 else:
                     self._is_open = True
                     new_port = find_free_port(self._host, start=self.port + 1)
                     self.port = new_port
                     host = self.host
                     port = self.port
 
@@ -162,15 +194,14 @@
                             self.stat,
                         ),
                         daemon=self.daemon,
                     )
 
             else:
                 self._is_open = True
-                logger.debug(f"{self.port} port not in use")
                 self._process = Process(
                     target=_pystartServer,
                     args=(
                         self.host,
                         str(self.port),
                         [two_bit_file],
                         self.option,
@@ -182,92 +213,95 @@
             raise e
 
         else:
             if self._process is not None:
                 self._process.start()
 
     def start(self):
-        """
-        Starts the gfServer instance in either blocking or non-blocking mode.
+        """Starts the gfServer instance in either blocking or non-blocking mode.
 
         If the server is set to non-blocking mode, it will start the server in a separate process.
         If the server is set to blocking mode, it will start the server in the current process.
         """
         if not self._block:
             self._start_nb()
         else:
             self._start_b()
 
     def stop(self):
-        """
-        Stops the gfServer instance if it is running.
+        """Stops the gfServer instance if it is running.
 
         This method sends a stop signal to the server process, causing it to terminate gracefully.
         """
         if self._is_open:
             stop_server(self.host, self.port)
 
         if self._process is not None:
             self._process.terminate()
 
-    def status(self, instance=False) -> t.Union[t.Dict[str, str], Status]:
-        """
-        Retrieves the status of the gfServer instance.
+    def status(self, *, instance=False) -> dict[str, str] | Status:
+        """Retrieves the status of the gfServer instance.
 
         Args:
             instance (bool, optional): If True, returns a Status object. If False, returns a dictionary with status information. Defaults to False.
 
         Returns:
             t.Union[t.Dict[str, str], Status]: The status of the gfServer instance, either as a dictionary or a Status object.
         """
         return status_server(self.host, self.port, self.option, instance=instance)
 
     def files(self) -> list[str]:
-        """
-        Retrieves the list of files served by the gfServer instance.
+        """Retrieves the list of files served by the gfServer instance.
 
         Returns:
             list[str]: A list of file names served by the gfServer instance.
+
+        See Also:
+            :func:`files` is a free function to query file status for server.
         """
         return files(self.host, self.port)
 
-    def query(self, intype: str, faName: str, isComplex: bool, isProt: bool) -> str:
-        """
-        Queries the gfServer instance with the given parameters.
+    def query(self, intype: str, faName: str, *, isComplex: bool, isProt: bool) -> str:
+        """Queries the gfServer instance with the given parameters.
 
         Args:
             intype (str): The type of input sequence. Must be one of "dna", "rna", or "protein".
             faName (str): The name of the input sequence.
             isComplex (bool): Whether the input sequence is complex.
             isProt (bool): Whether the input sequence is a protein sequence.
 
         Returns:
             str: The result of the query as a string.
         """
-        return server_query(intype, self.host, self.port, faName, isComplex, isProt)
+        return server_query(
+            intype,
+            self.host,
+            self.port,
+            faName,
+            isComplex=isComplex,
+            isProt=isProt,
+        )
 
     def is_ready(self) -> bool:
-        """
-        Returns True if the server is ready to accept queries, False otherwise.
+        """Returns True if the server is ready to accept queries, False otherwise.
 
         Returns:
             bool: True if the server is ready to accept queries, False otherwise.
         """
         return self._is_ready
 
     def is_open(self) -> bool:
-        """
-        Returns True if the server is open, False otherwise.
+        """Returns True if the server is open, False otherwise.
 
         Returns:
             bool: True if the server is open, False otherwise.
         """
         return self._is_open
 
-    def wait_ready(self, timeout: int = 60, restart: bool = False):
+    def wait_ready(self, timeout: int = 60, *, restart: bool = False):
         """Wait server ready in block mode.
 
         Args:
             timeout: Timeout for wait server ready.
             restart: If timeout, restart server and wait again.
 
         Raises:
@@ -277,36 +311,37 @@
         if not self._is_ready:
             try:
                 wait_server_ready(self.host, self.port, timeout, self.option)
             except RuntimeError as e:
                 if restart and self.use_others:
                     self.use_others = False
                     self.start()
-                    self.wait_ready(timeout * 2, restart)
+                    self.wait_ready(timeout * 2, restart=restart)
                 else:
+                    msg = f"Timeout for Waiting for {self.host} {self.port} server ready due to server is not opened by gfServer or need longer time to wait"
                     raise RuntimeError(
-                        f"Timeout for Waitting for {self.host} {self.port} server ready due to server is not opened by gfServer or need longer time to wait"
+                        msg,
                     ) from e
             else:
                 self._is_ready = True
 
-    @classmethod
-    def create_option(cls):
-        """
-        Creates a dictionary of options for the gfServer instance.
+    @staticmethod
+    def create_option() -> ServerOption:
+        """Creates a ServerOption for the gfServer instance.
 
         Returns:
-            dict: A dictionary of options for the gfServer instance.
+            ServerOption: A class that hold options for the gfServer instance.
         """
         return create_server_option()
 
-    def __str__(self):
+    def __str__(self) -> str:
+        """Return server option as a string."""
         return f"Server({self.host}, {self.port}, ready: {self.is_ready()} open: {self.is_open()} {self.option})"
 
     def __enter__(self):
-        print("start server")
+        """Starts the gfServer instance in blocking mode when used as a context manager."""
         self.start()
         return self
 
     def __exit__(self, *exc):
-        print("stop server")
+        """Stops the gfServer."""
         self.stop()
```

### Comparing `pxblat-0.2.0/src/pxblat/toolkit/__init__.py` & `pxblat-0.3.0/src/pxblat/toolkit/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,50 @@
-import typing as t
+"""Toolkit functions for working with BLAT."""
+from __future__ import annotations
+
 from pathlib import Path
 
-from pxblat.extc import faToTwoBit
-from pxblat.extc import twoBitToFa
-from pxblat.extc import TwoBitToFaOption
+from pxblat.extc import TwoBitToFaOption, faToTwoBit, twoBitToFa
+
+#     "Args",
+#     "Arguments",
+#     "Attention",
+#     "Attributes",
+#     "Caution",
+#     "Danger",
+#     "Error",
+#     "Example",
+#     "Examples",
+#     "Hint",
+#     "Important",
+#     "Keyword Args",
+#     "Keyword Arguments",
+#     "Methods",
+#     "Note",
+#     "Notes",
+#     "Return",
+#     "Returns",
+#     "Raises",
+#     "References",
+#     "See Also",
+#     "Tip",
+#     "Todo",
+#     "Warning",
+#     "Warnings",
+#     "Warns",
+#     "Yield",
+#     "Yields",
+
+__all__ = ["fa_to_two_bit", "two_bit_to_fa"]
 
 
 def fa_to_two_bit(
-    inFiles: t.List[str],
+    inFiles: list[str],
     outFile: str,
+    *,
     noMask: bool = False,
     stripVersion: bool = False,
     ignoreDups: bool = False,
     useLong: bool = False,
 ):
     """Convert one or more FASTA files to two-bit format.
 
@@ -34,16 +66,31 @@
     Example:
         >>> fa_to_two_bit(['input.fasta'], 'output.2bit')
     """
     return faToTwoBit(inFiles, outFile, noMask, stripVersion, ignoreDups, useLong)
 
 
 def two_bit_to_fa(
-    inName: t.Union[str, Path], outName: t.Union[str, Path], option: TwoBitToFaOption
+    inName: str | Path,
+    outName: str | Path,
+    option: TwoBitToFaOption,
 ):
+    """Converts a .2bit file to a .fa file.
+
+    This function takes the name of an input .2bit file and an output .fa file, and an option object,
+    converts the .2bit file to .fa format using the `twoBitToFa` function, and saves the result to the output file.
+
+    Args:
+        inName (Union[str, Path]): The name or Path of the input .2bit file.
+        outName (Union[str, Path]): The name or Path of the output .fa file.
+        option (TwoBitToFaOption): The options to use when converting the .2bit file.
+
+    Returns:
+        The return value from the `twoBitToFa` function.
+    """
     if isinstance(inName, Path):
         inName = str(inName)
 
     if isinstance(outName, Path):
         outName = str(outName)
 
     return twoBitToFa(inName, outName, option)
```

