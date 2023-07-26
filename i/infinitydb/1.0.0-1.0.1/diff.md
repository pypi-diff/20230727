# Comparing `tmp/infinitydb-1.0.0.tar.gz` & `tmp/infinitydb-1.0.1.tar.gz`

## Comparing `infinitydb-1.0.0.tar` & `infinitydb-1.0.1.tar`

### file list

```diff
@@ -1,2034 +1,11 @@
--rw-r--r--   0        0        0   145903 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/0/4/1/8/c/0418c83b80f7f7bfaec2738bfbbee53d2c1562196c0781702f6eddc8
--rw-r--r--   0        0        0    76875 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/0/6/2/4/7/062478cdc6c508c348d625c54e1c27266b7c2545b1a05567a038b5cf
--rw-r--r--   0        0        0    35965 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/1/f/d/9/a/1fd9ade2b751542e96db097082f121ecac23098b3cd95c8a877f0716
--rw-r--r--   0        0        0   805170 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/3/1/0/a/4/310a48cdaab5cf1631d625b4eb978cba70beab76027b6ec70636fd63
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/3/3/9/7/4/33974f84394d9a943f68359da08431dab4af9f86c33962982ea21b5f
--rw-r--r--   0        0        0    14404 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/4/2/2/2/1/4222164d43b51edeaab5262b2a9b3e43c548671c440d00d67b94796e
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/4/4/e/5/b/44e5b11a6caa92636d8ccfe658d420ba4ed8f67f7f4e835b214255aa
--rw-r--r--   0        0        0    18859 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/5/d/e/d/8/5ded8d61275a0ea81ed54f01958b5ab6f6909b3970b755d118b3b517
--rw-r--r--   0        0        0    11576 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/6/2/e/2/c/62e2caaadb9fd2d0a88b65a7d2043b2c343936491ef44dc753aa91e0
--rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/6/4/9/8/a/6498a97ba33d5bdd385aa8f5ea5d4d15aa22b0d23b6bd2e36e941896
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/7/7/c/2/7/77c274bfa9e9411e23c1852c72be58a71b4675a133b6e0afb63d0178
--rw-r--r--   0        0        0    50030 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/7/8/4/9/7/784975fc571b5b09b0278cb4a652d0647a56c0e1219ed29ad50ba28a
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/9/e/d/3/7/9ed377a761861346a483546ee4ebbe92a83f2d3a40e917849c2eb140
--rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/a/1/9/5/3/a19537d3cf37c122db841d6fe4cd322bc10d1a558bb00d146b85cb9a
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/a/b/a/9/e/aba9e729cd995ae60ba611539054f97c57ab58fe38387b2391cc5545
--rw-r--r--   0        0        0    30413 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/c/6/5/0/6/c650606ff8337102e85ade34bf42ce6292563652faa6ec533c984362
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/c/8/4/6/0/c84608549463ae90303a0f39c4b1e01a1717f15e0529931eee51391c
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/e/7/e/1/1/e7e11bf4fc1ff29feff55b10f7dee3ce79cfb8c866c278585bcbadb1
--rw-r--r--   0        0        0    14382 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/f/3/6/d/5/f36d58c71164036f2cff3c9d0bb0c2b4d1d94bd0814c26b9cbe036b2
--rw-r--r--   0        0        0    13132 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/http/f/9/6/5/9/f9659e50df363f8369e6abe4c4008418f9de6a660e264dbba624109f
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 infinitydb-1.0.0/c:/Users/roger/Documents/.cache/pip/selfcheck/241e69162522ccf5846a2f42ebc24b17464915a155679666b89a9f31
--rwxr-xr-x   0        0        0    30342 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/LICENSE.txt
--rwxr-xr-x   0        0        0    22911 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/Python-ast.h
--rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/Python.h
--rwxr-xr-x   0        0        0    48828 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/abstract.h
--rwxr-xr-x   0        0        0     1053 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/accu.h
--rwxr-xr-x   0        0        0     1259 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/asdl.h
--rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/ast.h
--rwxr-xr-x   0        0        0      824 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/bitset.h
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/bltinmodule.h
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/boolobject.h
--rwxr-xr-x   0        0        0     2176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/bytearrayobject.h
--rwxr-xr-x   0        0        0     3258 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/bytes_methods.h
--rwxr-xr-x   0        0        0     8587 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/bytesobject.h
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/cellobject.h
--rwxr-xr-x   0        0        0     8762 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/ceval.h
--rwxr-xr-x   0        0        0     1724 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/classobject.h
--rwxr-xr-x   0        0        0     6102 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/code.h
--rwxr-xr-x   0        0        0     7033 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/codecs.h
--rwxr-xr-x   0        0        0     2237 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/compile.h
--rwxr-xr-x   0        0        0     1876 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/complexobject.h
--rwxr-xr-x   0        0        0     9674 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/datetime.h
--rwxr-xr-x   0        0        0     3071 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/descrobject.h
--rwxr-xr-x   0        0        0     7355 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/dictobject.h
--rwxr-xr-x   0        0        0      477 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/dtoa.h
--rwxr-xr-x   0        0        0    22968 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/dynamic_annotations.h
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/enumobject.h
--rwxr-xr-x   0        0        0     1535 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/errcode.h
--rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/eval.h
--rwxr-xr-x   0        0        0     1701 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/fileobject.h
--rwxr-xr-x   0        0        0     3683 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/fileutils.h
--rwxr-xr-x   0        0        0     4924 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/floatobject.h
--rwxr-xr-x   0        0        0     3625 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/frameobject.h
--rwxr-xr-x   0        0        0     4182 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/funcobject.h
--rwxr-xr-x   0        0        0     3687 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/genobject.h
--rwxr-xr-x   0        0        0     2054 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/graminit.h
--rwxr-xr-x   0        0        0     2168 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/grammar.h
--rwxr-xr-x   0        0        0     4373 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/import.h
--rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/intrcheck.h
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/iterobject.h
--rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/listobject.h
--rwxr-xr-x   0        0        0     3860 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/longintrepr.h
--rwxr-xr-x   0        0        0     8686 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/longobject.h
--rwxr-xr-x   0        0        0      831 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/marshal.h
--rwxr-xr-x   0        0        0     2837 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/memoryobject.h
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/metagrammar.h
--rwxr-xr-x   0        0        0     3957 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/methodobject.h
--rwxr-xr-x   0        0        0     7500 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/modsupport.h
--rwxr-xr-x   0        0        0     2374 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/moduleobject.h
--rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/namespaceobject.h
--rwxr-xr-x   0        0        0     1051 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/node.h
--rwxr-xr-x   0        0        0    41451 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/object.h
--rwxr-xr-x   0        0        0    14614 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/objimpl.h
--rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/odictobject.h
--rwxr-xr-x   0        0        0     5219 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/opcode.h
--rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/osdefs.h
--rwxr-xr-x   0        0        0      308 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/osmodule.h
--rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/parsetok.h
--rwxr-xr-x   0        0        0     1163 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/patchlevel.h
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pgen.h
--rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pgenheaders.h
--rwxr-xr-x   0        0        0     4485 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/py_curses.h
--rwxr-xr-x   0        0        0     2808 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pyarena.h
--rwxr-xr-x   0        0        0     8378 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pyatomic.h
--rwxr-xr-x   0        0        0     1785 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pycapsule.h
--rwxr-xr-x   0        0        0    20430 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pyconfig.h
--rwxr-xr-x   0        0        0     1353 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pyctype.h
--rwxr-xr-x   0        0        0     1249 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pydebug.h
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pydtrace.h
--rwxr-xr-x   0        0        0    17722 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pyerrors.h
--rwxr-xr-x   0        0        0     2505 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pyexpat.h
--rwxr-xr-x   0        0        0     8647 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pyfpe.h
--rwxr-xr-x   0        0        0      431 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pygetopt.h
--rwxr-xr-x   0        0        0     4284 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pyhash.h
--rwxr-xr-x   0        0        0     4209 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pylifecycle.h
--rwxr-xr-x   0        0        0     3091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pymacconfig.h
--rwxr-xr-x   0        0        0     3598 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pymacro.h
--rwxr-xr-x   0        0        0     8542 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pymath.h
--rwxr-xr-x   0        0        0     8792 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pymem.h
--rwxr-xr-x   0        0        0    28340 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pyport.h
--rwxr-xr-x   0        0        0    11470 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pystate.h
--rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pystrcmp.h
--rwxr-xr-x   0        0        0      514 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pystrhex.h
--rwxr-xr-x   0        0        0     1528 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pystrtod.h
--rwxr-xr-x   0        0        0     6979 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pythonrun.h
--rwxr-xr-x   0        0        0     3082 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pythread.h
--rwxr-xr-x   0        0        0     7820 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/pytime.h
--rwxr-xr-x   0        0        0      656 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/rangeobject.h
--rwxr-xr-x   0        0        0     3441 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/setobject.h
--rwxr-xr-x   0        0        0     2550 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/sliceobject.h
--rwxr-xr-x   0        0        0     2092 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/structmember.h
--rwxr-xr-x   0        0        0     1402 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/structseq.h
--rwxr-xr-x   0        0        0     5113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/symtable.h
--rwxr-xr-x   0        0        0     1398 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/sysmodule.h
--rwxr-xr-x   0        0        0     2033 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/token.h
--rwxr-xr-x   0        0        0     3763 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/traceback.h
--rwxr-xr-x   0        0        0     2517 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/tupleobject.h
--rwxr-xr-x   0        0        0     2338 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/typeslots.h
--rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/ucnhash.h
--rwxr-xr-x   0        0        0    84121 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/unicodeobject.h
--rwxr-xr-x   0        0        0     1756 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/warnings.h
--rwxr-xr-x   0        0        0     2952 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Include/weakrefobject.h
--rwxr-xr-x   0        0        0     4981 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/__future__.py
--rwxr-xr-x   0        0        0     1335 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/_bootlocale.py
--rwxr-xr-x   0        0        0    27403 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/_collections_abc.py
--rwxr-xr-x   0        0        0     5281 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/_dummy_thread.py
--rwxr-xr-x   0        0        0     5901 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/_weakrefset.py
--rwxr-xr-x   0        0        0     8977 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/abc.py
--rwxr-xr-x   0        0        0    20975 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/base64.py
--rwxr-xr-x   0        0        0     2687 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/bisect.py
--rwxr-xr-x   0        0        0    37389 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/codecs.py
--rwxr-xr-x   0        0        0     9128 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/copy.py
--rwxr-xr-x   0        0        0     7213 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/copyreg.py
--rwxr-xr-x   0        0        0    34483 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/enum.py
--rwxr-xr-x   0        0        0     3275 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/fnmatch.py
--rwxr-xr-x   0        0        0    32162 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/functools.py
--rwxr-xr-x   0        0        0     4907 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/genericpath.py
--rwxr-xr-x   0        0        0     9785 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/hashlib.py
--rwxr-xr-x   0        0        0    23536 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/heapq.py
--rwxr-xr-x   0        0        0     5201 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/hmac.py
--rwxr-xr-x   0        0        0    11015 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/imp.py
--rwxr-xr-x   0        0        0     3616 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/io.py
--rwxr-xr-x   0        0        0     2305 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/keyword.py
--rwxr-xr-x   0        0        0     5489 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/linecache.py
--rwxr-xr-x   0        0        0    79031 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/locale.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/no-global-site-packages.txt
--rwxr-xr-x   0        0        0    23785 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/ntpath.py
--rwxr-xr-x   0        0        0    11327 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/operator.py
--rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/orig-prefix.txt
--rwxr-xr-x   0        0        0    38595 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/os.py
--rwxr-xr-x   0        0        0    16301 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/posixpath.py
--rwxr-xr-x   0        0        0    28214 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/random.py
--rwxr-xr-x   0        0        0    15933 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/re.py
--rwxr-xr-x   0        0        0     5500 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/reprlib.py
--rwxr-xr-x   0        0        0     7302 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/rlcompleter.py
--rwxr-xr-x   0        0        0    41699 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/shutil.py
--rwxr-xr-x   0        0        0    28770 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site.py
--rwxr-xr-x   0        0        0    19918 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/sre_compile.py
--rwxr-xr-x   0        0        0     7054 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/sre_constants.py
--rwxr-xr-x   0        0        0    37509 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/sre_parse.py
--rwxr-xr-x   0        0        0     5216 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/stat.py
--rwxr-xr-x   0        0        0      272 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/struct.py
--rwxr-xr-x   0        0        0    95767 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/tarfile.py
--rwxr-xr-x   0        0        0    27589 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/tempfile.py
--rwxr-xr-x   0        0        0     3218 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/token.py
--rwxr-xr-x   0        0        0    30299 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/tokenize.py
--rwxr-xr-x   0        0        0     9136 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/types.py
--rwxr-xr-x   0        0        0    19014 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/warnings.py
--rwxr-xr-x   0        0        0    21098 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/weakref.py
--rwxr-xr-x   0        0        0    47056 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/collections/__init__.py
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/collections/abc.py
--rwxr-xr-x   0        0        0     4374 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/distutils/__init__.py
--rwxr-xr-x   0        0        0      228 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/distutils/distutils.cfg
--rwxr-xr-x   0        0        0     5811 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/__init__.py
--rwxr-xr-x   0        0        0    16127 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/aliases.py
--rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/ascii.py
--rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/base64_codec.py
--rwxr-xr-x   0        0        0     1058 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/big5.py
--rwxr-xr-x   0        0        0     1078 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/big5hkscs.py
--rwxr-xr-x   0        0        0     2327 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/bz2_codec.py
--rwxr-xr-x   0        0        0     2153 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/charmap.py
--rwxr-xr-x   0        0        0    13428 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp037.py
--rwxr-xr-x   0        0        0    13875 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1006.py
--rwxr-xr-x   0        0        0    13420 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1026.py
--rwxr-xr-x   0        0        0    35295 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1125.py
--rwxr-xr-x   0        0        0    13412 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1140.py
--rwxr-xr-x   0        0        0    13993 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1250.py
--rwxr-xr-x   0        0        0    13668 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1251.py
--rwxr-xr-x   0        0        0    13818 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1252.py
--rwxr-xr-x   0        0        0    13401 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1253.py
--rwxr-xr-x   0        0        0    13809 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1254.py
--rwxr-xr-x   0        0        0    12773 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1255.py
--rwxr-xr-x   0        0        0    13121 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1256.py
--rwxr-xr-x   0        0        0    13681 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1257.py
--rwxr-xr-x   0        0        0    13671 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp1258.py
--rwxr-xr-x   0        0        0    14439 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp273.py
--rwxr-xr-x   0        0        0    12362 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp424.py
--rwxr-xr-x   0        0        0    35262 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp437.py
--rwxr-xr-x   0        0        0    13428 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp500.py
--rwxr-xr-x   0        0        0     1149 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp65001.py
--rwxr-xr-x   0        0        0    13995 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp720.py
--rwxr-xr-x   0        0        0    35379 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp737.py
--rwxr-xr-x   0        0        0    35173 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp775.py
--rwxr-xr-x   0        0        0    34803 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp850.py
--rwxr-xr-x   0        0        0    35700 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp852.py
--rwxr-xr-x   0        0        0    34548 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp855.py
--rwxr-xr-x   0        0        0    12730 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp856.py
--rwxr-xr-x   0        0        0    34602 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp857.py
--rwxr-xr-x   0        0        0    34713 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp858.py
--rwxr-xr-x   0        0        0    35379 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp860.py
--rwxr-xr-x   0        0        0    35331 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp861.py
--rwxr-xr-x   0        0        0    34068 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp862.py
--rwxr-xr-x   0        0        0    34950 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp863.py
--rwxr-xr-x   0        0        0    34353 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp864.py
--rwxr-xr-x   0        0        0    35316 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp865.py
--rwxr-xr-x   0        0        0    35094 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp866.py
--rwxr-xr-x   0        0        0    33654 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp869.py
--rwxr-xr-x   0        0        0    12902 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp874.py
--rwxr-xr-x   0        0        0    13161 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp875.py
--rwxr-xr-x   0        0        0     1062 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp932.py
--rwxr-xr-x   0        0        0     1062 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp949.py
--rwxr-xr-x   0        0        0     1062 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/cp950.py
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/euc_jis_2004.py
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/euc_jisx0213.py
--rwxr-xr-x   0        0        0     1066 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/euc_jp.py
--rwxr-xr-x   0        0        0     1066 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/euc_kr.py
--rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/gb18030.py
--rwxr-xr-x   0        0        0     1066 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/gb2312.py
--rwxr-xr-x   0        0        0     1054 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/gbk.py
--rwxr-xr-x   0        0        0     1563 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/hex_codec.py
--rwxr-xr-x   0        0        0    13789 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/hp_roman8.py
--rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/hz.py
--rwxr-xr-x   0        0        0     9479 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/idna.py
--rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso2022_jp.py
--rwxr-xr-x   0        0        0     1100 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso2022_jp_1.py
--rwxr-xr-x   0        0        0     1100 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso2022_jp_2.py
--rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso2022_jp_2004.py
--rwxr-xr-x   0        0        0     1100 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso2022_jp_3.py
--rwxr-xr-x   0        0        0     1108 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso2022_jp_ext.py
--rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso2022_kr.py
--rwxr-xr-x   0        0        0    13483 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_1.py
--rwxr-xr-x   0        0        0    13896 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_10.py
--rwxr-xr-x   0        0        0    12642 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_11.py
--rwxr-xr-x   0        0        0    13578 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_13.py
--rwxr-xr-x   0        0        0    13959 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_14.py
--rwxr-xr-x   0        0        0    13519 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_15.py
--rwxr-xr-x   0        0        0    13864 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_16.py
--rwxr-xr-x   0        0        0    13711 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_2.py
--rwxr-xr-x   0        0        0    13396 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_3.py
--rwxr-xr-x   0        0        0    13683 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_4.py
--rwxr-xr-x   0        0        0    13322 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_5.py
--rwxr-xr-x   0        0        0    11140 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_6.py
--rwxr-xr-x   0        0        0    13151 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_7.py
--rwxr-xr-x   0        0        0    11343 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_8.py
--rwxr-xr-x   0        0        0    13463 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/iso8859_9.py
--rwxr-xr-x   0        0        0     1062 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/johab.py
--rwxr-xr-x   0        0        0    14086 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/koi8_r.py
--rwxr-xr-x   0        0        0    13501 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/koi8_t.py
--rwxr-xr-x   0        0        0    14069 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/koi8_u.py
--rwxr-xr-x   0        0        0    14030 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/kz1048.py
--rwxr-xr-x   0        0        0     1314 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/latin_1.py
--rwxr-xr-x   0        0        0    37165 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_arabic.py
--rwxr-xr-x   0        0        0    14409 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_centeuro.py
--rwxr-xr-x   0        0        0    13940 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_croatian.py
--rwxr-xr-x   0        0        0    13761 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_cyrillic.py
--rwxr-xr-x   0        0        0    15477 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_farsi.py
--rwxr-xr-x   0        0        0    14028 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_greek.py
--rwxr-xr-x   0        0        0    13805 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_iceland.py
--rwxr-xr-x   0        0        0    14430 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_latin2.py
--rwxr-xr-x   0        0        0    13787 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_roman.py
--rwxr-xr-x   0        0        0    13968 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_romanian.py
--rwxr-xr-x   0        0        0    13820 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mac_turkish.py
--rwxr-xr-x   0        0        0     1258 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/mbcs.py
--rwxr-xr-x   0        0        0     1060 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/oem.py
--rwxr-xr-x   0        0        0    13827 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/palmos.py
--rwxr-xr-x   0        0        0    14327 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/ptcp154.py
--rwxr-xr-x   0        0        0     7118 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/punycode.py
--rwxr-xr-x   0        0        0     1581 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/quopri_codec.py
--rwxr-xr-x   0        0        0     1253 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/raw_unicode_escape.py
--rwxr-xr-x   0        0        0     2541 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/rot_13.py
--rwxr-xr-x   0        0        0     1078 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/shift_jis.py
--rwxr-xr-x   0        0        0     1098 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/shift_jis_2004.py
--rwxr-xr-x   0        0        0     1098 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/shift_jisx0213.py
--rwxr-xr-x   0        0        0    12607 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/tis_620.py
--rwxr-xr-x   0        0        0     1348 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/undefined.py
--rwxr-xr-x   0        0        0     1229 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/unicode_escape.py
--rwxr-xr-x   0        0        0     1241 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/unicode_internal.py
--rwxr-xr-x   0        0        0     5391 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/utf_16.py
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/utf_16_be.py
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/utf_16_le.py
--rwxr-xr-x   0        0        0     5279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/utf_32.py
--rwxr-xr-x   0        0        0      967 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/utf_32_be.py
--rwxr-xr-x   0        0        0      967 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/utf_32_le.py
--rwxr-xr-x   0        0        0      984 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/utf_7.py
--rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/utf_8.py
--rwxr-xr-x   0        0        0     4263 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/utf_8_sig.py
--rwxr-xr-x   0        0        0     2820 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/uu_codec.py
--rwxr-xr-x   0        0        0     2281 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/encodings/zlib_codec.py
--rwxr-xr-x   0        0        0     6043 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/importlib/__init__.py
--rwxr-xr-x   0        0        0    40004 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/importlib/_bootstrap.py
--rwxr-xr-x   0        0        0    55930 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/importlib/_bootstrap_external.py
--rwxr-xr-x   0        0        0    11111 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/importlib/abc.py
--rwxr-xr-x   0        0        0      865 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/importlib/machinery.py
--rwxr-xr-x   0        0        0    11171 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/importlib/util.py
--rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/distutils-precedence.pth
--rwxr-xr-x   0        0        0   107685 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/typing_extensions.py
--rwxr-xr-x   0        0        0     8425 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/zipp.py
--rwxr-xr-x   0        0        0     3759 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/_distutils_hack/__init__.py
--rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/_distutils_hack/override.py
--rwxr-xr-x   0        0        0    19573 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build/__init__.py
--rwxr-xr-x   0        0        0    12204 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build/__main__.py
--rwxr-xr-x   0        0        0    12631 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build/env.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build/py.typed
--rwxr-xr-x   0        0        0     1672 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build/util.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build-0.9.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build-0.9.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     4054 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build-0.9.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     1274 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build-0.9.0.dist-info/RECORD
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build-0.9.0.dist-info/REQUESTED
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build-0.9.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0      108 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build-0.9.0.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/build-0.9.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama/__init__.py
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama/ansi.py
--rwxr-xr-x   0        0        0    10830 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama/ansitowin32.py
--rwxr-xr-x   0        0        0     1915 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama/initialise.py
--rwxr-xr-x   0        0        0     5404 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama/win32.py
--rwxr-xr-x   0        0        0     6438 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama/winterm.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama-0.4.5.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1491 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama-0.4.5.dist-info/LICENSE.txt
--rwxr-xr-x   0        0        0    15128 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama-0.4.5.dist-info/METADATA
--rwxr-xr-x   0        0        0     1240 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama-0.4.5.dist-info/RECORD
--rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama-0.4.5.dist-info/WHEEL
--rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/colorama-0.4.5.dist-info/top_level.txt
--rwxr-xr-x   0        0        0    30503 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata/__init__.py
--rwxr-xr-x   0        0        0     1862 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata/_adapters.py
--rwxr-xr-x   0        0        0      743 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata/_collections.py
--rwxr-xr-x   0        0        0     1826 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata/_compat.py
--rwxr-xr-x   0        0        0     2895 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata/_functools.py
--rwxr-xr-x   0        0        0     2068 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata/_itertools.py
--rwxr-xr-x   0        0        0     1154 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata/_meta.py
--rwxr-xr-x   0        0        0     2166 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata/_text.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata/py.typed
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata-4.8.3.dist-info/INSTALLER
--rwxr-xr-x   0        0        0      571 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata-4.8.3.dist-info/LICENSE
--rwxr-xr-x   0        0        0     4008 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata-4.8.3.dist-info/METADATA
--rwxr-xr-x   0        0        0     1798 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata-4.8.3.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata-4.8.3.dist-info/WHEEL
--rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/importlib_metadata-4.8.3.dist-info/top_level.txt
--rwxr-xr-x   0        0        0      661 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/__about__.py
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/__init__.py
--rwxr-xr-x   0        0        0    11488 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/_manylinux.py
--rwxr-xr-x   0        0        0     4378 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/_musllinux.py
--rwxr-xr-x   0        0        0     1431 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/_structures.py
--rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/markers.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/py.typed
--rwxr-xr-x   0        0        0     4664 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/requirements.py
--rwxr-xr-x   0        0        0    30110 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/specifiers.py
--rwxr-xr-x   0        0        0    15699 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/tags.py
--rwxr-xr-x   0        0        0     4200 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/utils.py
--rwxr-xr-x   0        0        0    14665 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging/version.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging-21.3.dist-info/INSTALLER
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging-21.3.dist-info/LICENSE
--rwxr-xr-x   0        0        0    10174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging-21.3.dist-info/LICENSE.APACHE
--rwxr-xr-x   0        0        0     1344 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging-21.3.dist-info/LICENSE.BSD
--rwxr-xr-x   0        0        0    15147 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging-21.3.dist-info/METADATA
--rwxr-xr-x   0        0        0     2170 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging-21.3.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging-21.3.dist-info/WHEEL
--rwxr-xr-x   0        0        0       10 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/packaging-21.3.dist-info/top_level.txt
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/__init__.py
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/_compat.py
--rwxr-xr-x   0        0        0     3443 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/build.py
--rwxr-xr-x   0        0        0     6083 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/check.py
--rwxr-xr-x   0        0        0     3994 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/colorlog.py
--rwxr-xr-x   0        0        0      607 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/dirtools.py
--rwxr-xr-x   0        0        0     6081 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/envbuild.py
--rwxr-xr-x   0        0        0     2520 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/meta.py
--rwxr-xr-x   0        0        0    12721 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/wrappers.py
--rwxr-xr-x   0        0        0      872 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/in_process/__init__.py
--rwxr-xr-x   0        0        0    10801 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517/in_process/_in_process.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517-0.13.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1081 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517-0.13.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     3802 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517-0.13.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     1754 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517-0.13.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pep517-0.13.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/__init__.py
--rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/__main__.py
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/py.typed
--rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/__init__.py
--rwxr-xr-x   0        0        0     9950 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/build_env.py
--rwxr-xr-x   0        0        0     9441 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cache.py
--rwxr-xr-x   0        0        0    13153 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/configuration.py
--rwxr-xr-x   0        0        0    12762 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/exceptions.py
--rwxr-xr-x   0        0        0      340 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/main.py
--rwxr-xr-x   0        0        0     7215 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/pyproject.py
--rwxr-xr-x   0        0        0     6393 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/self_outdated_check.py
--rwxr-xr-x   0        0        0    12247 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/wheel_builder.py
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/__init__.py
--rwxr-xr-x   0        0        0     6399 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rwxr-xr-x   0        0        0     7790 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/base_command.py
--rwxr-xr-x   0        0        0    28391 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rwxr-xr-x   0        0        0      760 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/command_context.py
--rwxr-xr-x   0        0        0     2472 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/main.py
--rwxr-xr-x   0        0        0     2614 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/main_parser.py
--rwxr-xr-x   0        0        0    10788 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/parser.py
--rwxr-xr-x   0        0        0     8300 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rwxr-xr-x   0        0        0    17097 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/req_command.py
--rwxr-xr-x   0        0        0     5076 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/spinners.py
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/cli/status_codes.py
--rwxr-xr-x   0        0        0     3736 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/__init__.py
--rwxr-xr-x   0        0        0     7524 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/cache.py
--rwxr-xr-x   0        0        0     1685 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/check.py
--rwxr-xr-x   0        0        0     2958 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/completion.py
--rwxr-xr-x   0        0        0     8944 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/configuration.py
--rwxr-xr-x   0        0        0     6629 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/debug.py
--rwxr-xr-x   0        0        0     4904 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/download.py
--rwxr-xr-x   0        0        0     2951 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/freeze.py
--rwxr-xr-x   0        0        0     1703 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/hash.py
--rwxr-xr-x   0        0        0     1132 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/help.py
--rwxr-xr-x   0        0        0     4762 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/index.py
--rwxr-xr-x   0        0        0    27851 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/install.py
--rwxr-xr-x   0        0        0    12203 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/list.py
--rwxr-xr-x   0        0        0     5697 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/search.py
--rwxr-xr-x   0        0        0     8064 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/show.py
--rwxr-xr-x   0        0        0     3526 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/uninstall.py
--rwxr-xr-x   0        0        0     6168 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/commands/wheel.py
--rwxr-xr-x   0        0        0      858 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/distributions/__init__.py
--rwxr-xr-x   0        0        0     1172 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/distributions/base.py
--rwxr-xr-x   0        0        0      767 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/distributions/installed.py
--rwxr-xr-x   0        0        0     5598 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/distributions/sdist.py
--rwxr-xr-x   0        0        0     1115 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/distributions/wheel.py
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/index/__init__.py
--rwxr-xr-x   0        0        0    17534 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/index/collector.py
--rwxr-xr-x   0        0        0    36344 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/index/package_finder.py
--rwxr-xr-x   0        0        0     6557 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/index/sources.py
--rwxr-xr-x   0        0        0    14444 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/locations/__init__.py
--rwxr-xr-x   0        0        0     5871 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/locations/_distutils.py
--rwxr-xr-x   0        0        0     7918 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rwxr-xr-x   0        0        0     1579 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/locations/base.py
--rwxr-xr-x   0        0        0     1660 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/metadata/__init__.py
--rwxr-xr-x   0        0        0    11103 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/metadata/base.py
--rwxr-xr-x   0        0        0     5089 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/__init__.py
--rwxr-xr-x   0        0        0      990 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/candidate.py
--rwxr-xr-x   0        0        0     6350 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/direct_url.py
--rwxr-xr-x   0        0        0     2520 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/format_control.py
--rwxr-xr-x   0        0        0     1030 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/index.py
--rwxr-xr-x   0        0        0     9817 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/link.py
--rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/scheme.py
--rwxr-xr-x   0        0        0     4520 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/search_scope.py
--rwxr-xr-x   0        0        0     1907 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rwxr-xr-x   0        0        0     3858 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/target_python.py
--rwxr-xr-x   0        0        0     3500 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/models/wheel.py
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/network/__init__.py
--rwxr-xr-x   0        0        0    12190 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/network/auth.py
--rwxr-xr-x   0        0        0     2100 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/network/cache.py
--rwxr-xr-x   0        0        0     6016 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/network/download.py
--rwxr-xr-x   0        0        0     7627 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rwxr-xr-x   0        0        0    16729 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/network/session.py
--rwxr-xr-x   0        0        0     4059 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/network/utils.py
--rwxr-xr-x   0        0        0     1791 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/network/xmlrpc.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/__init__.py
--rwxr-xr-x   0        0        0     5109 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/check.py
--rwxr-xr-x   0        0        0     9770 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/freeze.py
--rwxr-xr-x   0        0        0    23838 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/prepare.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rwxr-xr-x   0        0        0     1119 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rwxr-xr-x   0        0        0     1177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rwxr-xr-x   0        0        0     1945 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rwxr-xr-x   0        0        0     1063 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rwxr-xr-x   0        0        0     1405 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rwxr-xr-x   0        0        0     3047 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/install/legacy.py
--rwxr-xr-x   0        0        0    27412 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rwxr-xr-x   0        0        0     2793 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/req/__init__.py
--rwxr-xr-x   0        0        0    15285 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/req/constructors.py
--rwxr-xr-x   0        0        0    17421 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/req/req_file.py
--rwxr-xr-x   0        0        0    33804 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/req/req_install.py
--rwxr-xr-x   0        0        0     7584 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/req/req_set.py
--rwxr-xr-x   0        0        0     4117 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/req/req_tracker.py
--rwxr-xr-x   0        0        0    23748 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/req/req_uninstall.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/__init__.py
--rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/base.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rwxr-xr-x   0        0        0    18312 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rwxr-xr-x   0        0        0     5220 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rwxr-xr-x   0        0        0    18210 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rwxr-xr-x   0        0        0    26806 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rwxr-xr-x   0        0        0     5705 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rwxr-xr-x   0        0        0     9205 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rwxr-xr-x   0        0        0     2526 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rwxr-xr-x   0        0        0     5455 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rwxr-xr-x   0        0        0     9580 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/__init__.py
--rwxr-xr-x   0        0        0     1015 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/_log.py
--rwxr-xr-x   0        0        0     1665 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/appdirs.py
--rwxr-xr-x   0        0        0     1884 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/compat.py
--rwxr-xr-x   0        0        0     5377 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/datetime.py
--rwxr-xr-x   0        0        0     3627 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/deprecation.py
--rwxr-xr-x   0        0        0     3206 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rwxr-xr-x   0        0        0     1249 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/distutils_args.py
--rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/egg_link.py
--rwxr-xr-x   0        0        0     1169 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/encoding.py
--rwxr-xr-x   0        0        0     1055 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/filesystem.py
--rwxr-xr-x   0        0        0      716 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/filetypes.py
--rwxr-xr-x   0        0        0     3110 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/glibc.py
--rwxr-xr-x   0        0        0     4811 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/hashes.py
--rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rwxr-xr-x   0        0        0    11532 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/logging.py
--rwxr-xr-x   0        0        0    20432 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/misc.py
--rwxr-xr-x   0        0        0     1193 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/models.py
--rwxr-xr-x   0        0        0     2952 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/packaging.py
--rwxr-xr-x   0        0        0     3196 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/parallel.py
--rwxr-xr-x   0        0        0      987 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/pkg_resources.py
--rwxr-xr-x   0        0        0     4697 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rwxr-xr-x   0        0        0    10058 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/subprocess.py
--rwxr-xr-x   0        0        0     7662 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rwxr-xr-x   0        0        0     8906 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/unpacking.py
--rwxr-xr-x   0        0        0     1759 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/urls.py
--rwxr-xr-x   0        0        0     3459 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rwxr-xr-x   0        0        0     6163 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/utils/wheel.py
--rwxr-xr-x   0        0        0      596 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/vcs/__init__.py
--rwxr-xr-x   0        0        0     2857 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rwxr-xr-x   0        0        0    17804 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/vcs/git.py
--rwxr-xr-x   0        0        0     4945 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rwxr-xr-x   0        0        0    11596 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/vcs/subversion.py
--rwxr-xr-x   0        0        0    22414 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rwxr-xr-x   0        0        0     4708 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/__init__.py
--rwxr-xr-x   0        0        0    48414 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distro.py
--rwxr-xr-x   0        0        0   273394 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pyparsing.py
--rwxr-xr-x   0        0        0    34549 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/six.py
--rwxr-xr-x   0        0        0      432 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/vendor.txt
--rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rwxr-xr-x   0        0        0     1295 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rwxr-xr-x   0        0        0     4882 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rwxr-xr-x   0        0        0      805 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rwxr-xr-x   0        0        0      695 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rwxr-xr-x   0        0        0    14149 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rwxr-xr-x   0        0        0     2533 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rwxr-xr-x   0        0        0     4070 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rwxr-xr-x   0        0        0     7091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rwxr-xr-x   0        0        0      690 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rwxr-xr-x   0        0        0     4153 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rwxr-xr-x   0        0        0   259465 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/certifi/cacert.pem
--rwxr-xr-x   0        0        0     2840 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/certifi/core.py
--rwxr-xr-x   0        0        0     3271 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rwxr-xr-x   0        0        0    31254 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rwxr-xr-x   0        0        0     1757 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rwxr-xr-x   0        0        0     9411 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rwxr-xr-x   0        0        0     3839 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rwxr-xr-x   0        0        0     5110 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rwxr-xr-x   0        0        0     3590 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rwxr-xr-x   0        0        0     1200 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/compat.py
--rwxr-xr-x   0        0        0     1855 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rwxr-xr-x   0        0        0     1661 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/enums.py
--rwxr-xr-x   0        0        0     3950 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rwxr-xr-x   0        0        0    10510 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rwxr-xr-x   0        0        0     3749 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rwxr-xr-x   0        0        0    13546 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rwxr-xr-x   0        0        0     1748 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rwxr-xr-x   0        0        0    31621 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rwxr-xr-x   0        0        0     1747 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rwxr-xr-x   0        0        0    20715 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rwxr-xr-x   0        0        0     1754 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rwxr-xr-x   0        0        0    13838 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rwxr-xr-x   0        0        0    25777 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rwxr-xr-x   0        0        0    19643 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rwxr-xr-x   0        0        0   105697 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rwxr-xr-x   0        0        0    99571 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rwxr-xr-x   0        0        0    98776 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rwxr-xr-x   0        0        0   102498 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rwxr-xr-x   0        0        0   131180 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rwxr-xr-x   0        0        0   103312 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rwxr-xr-x   0        0        0    95946 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rwxr-xr-x   0        0        0     5370 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rwxr-xr-x   0        0        0     3413 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rwxr-xr-x   0        0        0     2012 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rwxr-xr-x   0        0        0    25481 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rwxr-xr-x   0        0        0     6136 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rwxr-xr-x   0        0        0     4309 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rwxr-xr-x   0        0        0     3774 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rwxr-xr-x   0        0        0    12503 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rwxr-xr-x   0        0        0     2766 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/version.py
--rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rwxr-xr-x   0        0        0    19474 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rwxr-xr-x   0        0        0    10517 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rwxr-xr-x   0        0        0     1915 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rwxr-xr-x   0        0        0     5404 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/colorama/win32.py
--rwxr-xr-x   0        0        0     6438 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/colorama/winterm.py
--rwxr-xr-x   0        0        0      581 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rwxr-xr-x   0        0        0    41495 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/compat.py
--rwxr-xr-x   0        0        0    51059 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/database.py
--rwxr-xr-x   0        0        0    20739 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/index.py
--rwxr-xr-x   0        0        0    51965 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/locators.py
--rwxr-xr-x   0        0        0    14811 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rwxr-xr-x   0        0        0     4989 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/markers.py
--rwxr-xr-x   0        0        0    39109 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rwxr-xr-x   0        0        0    10820 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/resources.py
--rwxr-xr-x   0        0        0    17720 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    96768 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   180736 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   105984 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/t64.exe
--rwxr-xr-x   0        0        0    67766 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/util.py
--rwxr-xr-x   0        0        0    23513 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    90112 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   166400 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0    99840 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/w64.exe
--rwxr-xr-x   0        0        0    42943 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/_backport/__init__.py
--rwxr-xr-x   0        0        0      971 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py
--rwxr-xr-x   0        0        0    25707 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py
--rwxr-xr-x   0        0        0     2617 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.cfg
--rwxr-xr-x   0        0        0    26854 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
--rwxr-xr-x   0        0        0    92628 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py
--rwxr-xr-x   0        0        0     1160 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/__init__.py
--rwxr-xr-x   0        0        0    16728 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py
--rwxr-xr-x   0        0        0    32353 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py
--rwxr-xr-x   0        0        0    77040 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py
--rwxr-xr-x   0        0        0     4931 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/_utils.py
--rwxr-xr-x   0        0        0    83464 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/constants.py
--rwxr-xr-x   0        0        0   117186 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/html5parser.py
--rwxr-xr-x   0        0        0    15759 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/serializer.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/_trie/__init__.py
--rwxr-xr-x   0        0        0     1013 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py
--rwxr-xr-x   0        0        0     1775 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/filters/__init__.py
--rwxr-xr-x   0        0        0      919 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/filters/base.py
--rwxr-xr-x   0        0        0     2945 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rwxr-xr-x   0        0        0     3643 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py
--rwxr-xr-x   0        0        0    10588 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
--rwxr-xr-x   0        0        0    26897 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
--rwxr-xr-x   0        0        0     1214 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py
--rwxr-xr-x   0        0        0      679 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
--rwxr-xr-x   0        0        0     1715 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
--rwxr-xr-x   0        0        0     1776 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
--rwxr-xr-x   0        0        0     3592 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
--rwxr-xr-x   0        0        0    14565 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py
--rwxr-xr-x   0        0        0     8925 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
--rwxr-xr-x   0        0        0    12836 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
--rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
--rwxr-xr-x   0        0        0     5719 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
--rwxr-xr-x   0        0        0     7476 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py
--rwxr-xr-x   0        0        0     1413 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
--rwxr-xr-x   0        0        0     4551 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
--rwxr-xr-x   0        0        0     6357 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rwxr-xr-x   0        0        0     2309 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
--rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/idna/__init__.py
--rwxr-xr-x   0        0        0     3453 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/idna/codec.py
--rwxr-xr-x   0        0        0      360 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/idna/compat.py
--rwxr-xr-x   0        0        0    12826 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/idna/core.py
--rwxr-xr-x   0        0        0    42350 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rwxr-xr-x   0        0        0     1933 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/idna/intranges.py
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/idna/package_data.py
--rwxr-xr-x   0        0        0   201849 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/idna/uts46data.py
--rwxr-xr-x   0        0        0     1118 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/msgpack/_version.py
--rwxr-xr-x   0        0        0     1081 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rwxr-xr-x   0        0        0     6088 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rwxr-xr-x   0        0        0    38026 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/msgpack/fallback.py
--rwxr-xr-x   0        0        0      661 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rwxr-xr-x   0        0        0    11488 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rwxr-xr-x   0        0        0     4378 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rwxr-xr-x   0        0        0     1629 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rwxr-xr-x   0        0        0     8487 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/markers.py
--rwxr-xr-x   0        0        0     4676 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rwxr-xr-x   0        0        0    30964 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rwxr-xr-x   0        0        0    15714 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/tags.py
--rwxr-xr-x   0        0        0     4200 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/utils.py
--rwxr-xr-x   0        0        0    14665 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/packaging/version.py
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/__init__.py
--rwxr-xr-x   0        0        0     3457 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/build.py
--rwxr-xr-x   0        0        0     6084 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/check.py
--rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/colorlog.py
--rwxr-xr-x   0        0        0     1253 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/compat.py
--rwxr-xr-x   0        0        0     1129 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/dirtools.py
--rwxr-xr-x   0        0        0     6100 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/envbuild.py
--rwxr-xr-x   0        0        0     2463 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/meta.py
--rwxr-xr-x   0        0        0    13429 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/wrappers.py
--rwxr-xr-x   0        0        0      563 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rwxr-xr-x   0        0        0    11201 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rwxr-xr-x   0        0        0   108287 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rwxr-xr-x   0        0        0    12859 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rwxr-xr-x   0        0        0     1140 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rwxr-xr-x   0        0        0     3994 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rwxr-xr-x   0        0        0     4922 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rwxr-xr-x   0        0        0     2619 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rwxr-xr-x   0        0        0     6905 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rwxr-xr-x   0        0        0     6416 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/platformdirs/windows.py
--rwxr-xr-x   0        0        0     5294 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/progress/__init__.py
--rwxr-xr-x   0        0        0     2942 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/progress/bar.py
--rwxr-xr-x   0        0        0     2655 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/progress/colors.py
--rwxr-xr-x   0        0        0     1613 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/progress/counter.py
--rwxr-xr-x   0        0        0     1461 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/progress/spinner.py
--rwxr-xr-x   0        0        0     5113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/__init__.py
--rwxr-xr-x   0        0        0      441 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/__version__.py
--rwxr-xr-x   0        0        0     1096 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rwxr-xr-x   0        0        0    21548 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/adapters.py
--rwxr-xr-x   0        0        0     6402 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/api.py
--rwxr-xr-x   0        0        0    10207 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/auth.py
--rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/certs.py
--rwxr-xr-x   0        0        0     2045 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/compat.py
--rwxr-xr-x   0        0        0    18430 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/cookies.py
--rwxr-xr-x   0        0        0     3250 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rwxr-xr-x   0        0        0     3972 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/help.py
--rwxr-xr-x   0        0        0      757 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/hooks.py
--rwxr-xr-x   0        0        0    34924 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/models.py
--rwxr-xr-x   0        0        0      695 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/packages.py
--rwxr-xr-x   0        0        0    30168 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/sessions.py
--rwxr-xr-x   0        0        0     4188 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rwxr-xr-x   0        0        0     3005 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/structures.py
--rwxr-xr-x   0        0        0    31394 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/requests/utils.py
--rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
--rwxr-xr-x   0        0        0     5872 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rwxr-xr-x   0        0        0     1364 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rwxr-xr-x   0        0        0    17540 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rwxr-xr-x   0        0        0     4794 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/resolvelib/structs.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rwxr-xr-x   0        0        0    18257 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rwxr-xr-x   0        0        0     3314 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rwxr-xr-x   0        0        0     1944 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rwxr-xr-x   0        0        0     1496 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/after.py
--rwxr-xr-x   0        0        0     1376 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/before.py
--rwxr-xr-x   0        0        0     1908 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rwxr-xr-x   0        0        0     1383 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rwxr-xr-x   0        0        0     6645 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rwxr-xr-x   0        0        0     2790 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rwxr-xr-x   0        0        0     2145 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rwxr-xr-x   0        0        0     6691 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tenacity/wait.py
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rwxr-xr-x   0        0        0    22415 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rwxr-xr-x   0        0        0     2681 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/tomli/_re.py
--rwxr-xr-x   0        0        0     2763 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rwxr-xr-x   0        0        0    10811 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rwxr-xr-x   0        0        0    20080 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rwxr-xr-x   0        0        0    37587 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rwxr-xr-x   0        0        0     8217 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rwxr-xr-x   0        0        0     8579 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rwxr-xr-x   0        0        0     2440 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/filepost.py
--rwxr-xr-x   0        0        0    19763 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rwxr-xr-x   0        0        0     5985 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/request.py
--rwxr-xr-x   0        0        0    28203 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/response.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rwxr-xr-x   0        0        0    11034 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rwxr-xr-x   0        0        0     4538 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rwxr-xr-x   0        0        0    16900 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rwxr-xr-x   0        0        0    34449 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rwxr-xr-x   0        0        0     7097 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rwxr-xr-x   0        0        0    17649 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rwxr-xr-x   0        0        0    13922 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rwxr-xr-x   0        0        0      108 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rwxr-xr-x   0        0        0    34666 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rwxr-xr-x   0        0        0     1417 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rwxr-xr-x   0        0        0      927 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
--rwxr-xr-x   0        0        0     5679 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
--rwxr-xr-x   0        0        0     1155 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rwxr-xr-x   0        0        0     4920 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rwxr-xr-x   0        0        0     1605 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rwxr-xr-x   0        0        0      498 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rwxr-xr-x   0        0        0     4123 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rwxr-xr-x   0        0        0     3510 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rwxr-xr-x   0        0        0    21391 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rwxr-xr-x   0        0        0    17177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rwxr-xr-x   0        0        0     6931 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rwxr-xr-x   0        0        0    10003 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rwxr-xr-x   0        0        0    14047 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rwxr-xr-x   0        0        0     5404 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rwxr-xr-x   0        0        0    10579 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rwxr-xr-x   0        0        0     8979 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rwxr-xr-x   0        0        0     1305 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rwxr-xr-x   0        0        0     6563 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rwxr-xr-x   0        0        0     4307 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip-21.3.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip-21.3.1.dist-info/LICENSE.txt
--rwxr-xr-x   0        0        0     4216 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip-21.3.1.dist-info/METADATA
--rwxr-xr-x   0        0        0    63513 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip-21.3.1.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip-21.3.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip-21.3.1.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pip-21.3.1.dist-info/top_level.txt
--rwxr-xr-x   0        0        0   108573 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rwxr-xr-x   0        0        0    24701 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/appdirs.py
--rwxr-xr-x   0        0        0   232055 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/pyparsing.py
--rwxr-xr-x   0        0        0      661 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rwxr-xr-x   0        0        0    11488 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rwxr-xr-x   0        0        0     4378 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rwxr-xr-x   0        0        0     1629 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rwxr-xr-x   0        0        0     8496 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rwxr-xr-x   0        0        0     4706 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rwxr-xr-x   0        0        0    30964 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rwxr-xr-x   0        0        0    15710 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rwxr-xr-x   0        0        0     4200 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rwxr-xr-x   0        0        0    14665 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
--rwxr-xr-x   0        0        0     2362 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/extern/__init__.py
--rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
--rwxr-xr-x   0        0        0     9104 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/__init__.py
--rwxr-xr-x   0        0        0     6567 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/actions.py
--rwxr-xr-x   0        0        0    13387 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/common.py
--rwxr-xr-x   0        0        0   224411 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/core.py
--rwxr-xr-x   0        0        0     9523 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/exceptions.py
--rwxr-xr-x   0        0        0    38646 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/helpers.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/py.typed
--rwxr-xr-x   0        0        0    26692 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/results.py
--rwxr-xr-x   0        0        0    13488 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/testing.py
--rwxr-xr-x   0        0        0    10634 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/unicode.py
--rwxr-xr-x   0        0        0     8670 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/util.py
--rwxr-xr-x   0        0        0    24198 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing/diagram/__init__.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing-3.1.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1023 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing-3.1.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     4927 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing-3.1.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     1875 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing-3.1.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/pyparsing-3.1.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0     7448 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/__init__.py
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_deprecation_warning.py
--rwxr-xr-x   0        0        0     2392 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_imp.py
--rwxr-xr-x   0        0        0     7077 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/archive_util.py
--rwxr-xr-x   0        0        0    10536 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/build_meta.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/cli-32.exe
--rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/cli-64.exe
--rwxr-xr-x   0        0        0   137216 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/cli-arm64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/cli.exe
--rwxr-xr-x   0        0        0    23153 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/config.py
--rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/dep_util.py
--rwxr-xr-x   0        0        0     5499 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/depends.py
--rwxr-xr-x   0        0        0    43154 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/dist.py
--rwxr-xr-x   0        0        0     1555 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/errors.py
--rwxr-xr-x   0        0        0     1684 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/extension.py
--rwxr-xr-x   0        0        0     4873 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/glob.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/gui-32.exe
--rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/gui-64.exe
--rwxr-xr-x   0        0        0   137728 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/gui-arm64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/gui.exe
--rwxr-xr-x   0        0        0     3824 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/installer.py
--rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/launch.py
--rwxr-xr-x   0        0        0     5217 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/monkey.py
--rwxr-xr-x   0        0        0    50561 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/msvc.py
--rwxr-xr-x   0        0        0     3093 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/namespaces.py
--rwxr-xr-x   0        0        0    40092 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/package_index.py
--rwxr-xr-x   0        0        0      245 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/py34compat.py
--rwxr-xr-x   0        0        0    14348 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/sandbox.py
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/script (dev).tmpl
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/script.tmpl
--rwxr-xr-x   0        0        0      941 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/unicode_utils.py
--rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/version.py
--rwxr-xr-x   0        0        0     8288 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/wheel.py
--rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/windows_support.py
--rwxr-xr-x   0        0        0      536 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/__init__.py
--rwxr-xr-x   0        0        0    20813 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rwxr-xr-x   0        0        0     8572 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/archive_util.py
--rwxr-xr-x   0        0        0    14894 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rwxr-xr-x   0        0        0    47644 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rwxr-xr-x   0        0        0    18079 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/cmd.py
--rwxr-xr-x   0        0        0     4827 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/config.py
--rwxr-xr-x   0        0        0     9282 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/core.py
--rwxr-xr-x   0        0        0    17330 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/debug.py
--rwxr-xr-x   0        0        0     3491 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/dep_util.py
--rwxr-xr-x   0        0        0     7778 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/dir_util.py
--rwxr-xr-x   0        0        0    50421 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/dist.py
--rwxr-xr-x   0        0        0     3577 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/errors.py
--rwxr-xr-x   0        0        0    10515 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/extension.py
--rwxr-xr-x   0        0        0    17784 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rwxr-xr-x   0        0        0     8148 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/file_util.py
--rwxr-xr-x   0        0        0    13407 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/filelist.py
--rwxr-xr-x   0        0        0     1969 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/log.py
--rwxr-xr-x   0        0        0    30453 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rwxr-xr-x   0        0        0    23540 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rwxr-xr-x   0        0        0      455 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/py35compat.py
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/py38compat.py
--rwxr-xr-x   0        0        0     3498 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/spawn.py
--rwxr-xr-x   0        0        0    22151 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rwxr-xr-x   0        0        0    12483 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/text_file.py
--rwxr-xr-x   0        0        0    14538 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rwxr-xr-x   0        0        0    20655 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/util.py
--rwxr-xr-x   0        0        0    13015 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/version.py
--rwxr-xr-x   0        0        0     5277 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rwxr-xr-x   0        0        0      799 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rwxr-xr-x   0        0        0     5562 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rwxr-xr-x   0        0        0     4913 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rwxr-xr-x   0        0        0    35579 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/bdist_msi.py
--rwxr-xr-x   0        0        0    21537 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rwxr-xr-x   0        0        0    16030 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/bdist_wininst.py
--rwxr-xr-x   0        0        0     5773 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/build.py
--rwxr-xr-x   0        0        0     8022 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rwxr-xr-x   0        0        0    31612 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rwxr-xr-x   0        0        0    16495 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rwxr-xr-x   0        0        0     5963 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rwxr-xr-x   0        0        0     5637 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/check.py
--rwxr-xr-x   0        0        0     2776 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/clean.py
--rwxr-xr-x   0        0        0    13117 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/config.py
--rwxr-xr-x   0        0        0    28970 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/install.py
--rwxr-xr-x   0        0        0     2822 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rwxr-xr-x   0        0        0     2753 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rwxr-xr-x   0        0        0     8397 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rwxr-xr-x   0        0        0     2017 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rwxr-xr-x   0        0        0      671 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rwxr-xr-x   0        0        0    11712 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/register.py
--rwxr-xr-x   0        0        0    19005 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rwxr-xr-x   0        0        0     7597 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_distutils/command/upload.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/__init__.py
--rwxr-xr-x   0        0        0    15130 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/ordered_set.py
--rwxr-xr-x   0        0        0   232055 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/pyparsing.py
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rwxr-xr-x   0        0        0   117968 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rwxr-xr-x   0        0        0    16256 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rwxr-xr-x   0        0        0      661 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rwxr-xr-x   0        0        0    11488 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rwxr-xr-x   0        0        0     4378 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rwxr-xr-x   0        0        0     1629 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rwxr-xr-x   0        0        0     8493 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rwxr-xr-x   0        0        0     4700 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rwxr-xr-x   0        0        0    30964 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rwxr-xr-x   0        0        0    15710 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rwxr-xr-x   0        0        0     4200 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rwxr-xr-x   0        0        0    14665 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/_vendor/packaging/version.py
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/__init__.py
--rwxr-xr-x   0        0        0     2381 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/alias.py
--rwxr-xr-x   0        0        0    16604 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/bdist_egg.py
--rwxr-xr-x   0        0        0     1182 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/bdist_rpm.py
--rwxr-xr-x   0        0        0     4415 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/build_clib.py
--rwxr-xr-x   0        0        0    13212 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/build_ext.py
--rwxr-xr-x   0        0        0     8751 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/build_py.py
--rwxr-xr-x   0        0        0     7012 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/develop.py
--rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/dist_info.py
--rwxr-xr-x   0        0        0    85639 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/easy_install.py
--rwxr-xr-x   0        0        0    26126 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/egg_info.py
--rwxr-xr-x   0        0        0     4906 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/install.py
--rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/install_egg_info.py
--rwxr-xr-x   0        0        0     3875 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/install_lib.py
--rwxr-xr-x   0        0        0     2593 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/install_scripts.py
--rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/launcher manifest.xml
--rwxr-xr-x   0        0        0     4946 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/py36compat.py
--rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/register.py
--rwxr-xr-x   0        0        0     2128 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/rotate.py
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/saveopts.py
--rwxr-xr-x   0        0        0     6413 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/sdist.py
--rwxr-xr-x   0        0        0     5086 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/setopt.py
--rwxr-xr-x   0        0        0     8088 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/test.py
--rwxr-xr-x   0        0        0      462 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/upload.py
--rwxr-xr-x   0        0        0     7218 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/command/upload_docs.py
--rwxr-xr-x   0        0        0     2407 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools/extern/__init__.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools-59.6.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools-59.6.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     4963 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools-59.6.0.dist-info/METADATA
--rwxr-xr-x   0        0        0    23044 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools-59.6.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools-59.6.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0     2636 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools-59.6.0.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/setuptools-59.6.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0      299 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/tomli/__init__.py
--rwxr-xr-x   0        0        0    21659 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/tomli/_parser.py
--rwxr-xr-x   0        0        0     2818 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/tomli/_re.py
--rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/tomli/_types.py
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/tomli/py.typed
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/tomli-1.2.3.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/tomli-1.2.3.dist-info/LICENSE
--rwxr-xr-x   0        0        0     9089 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/tomli-1.2.3.dist-info/METADATA
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/tomli-1.2.3.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/tomli-1.2.3.dist-info/WHEEL
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/typing_extensions-4.1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0    12755 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/typing_extensions-4.1.1.dist-info/LICENSE
--rwxr-xr-x   0        0        0     1736 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/typing_extensions-4.1.1.dist-info/METADATA
--rwxr-xr-x   0        0        0      565 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/typing_extensions-4.1.1.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/typing_extensions-4.1.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/__init__.py
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/__main__.py
--rwxr-xr-x   0        0        0    19075 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/bdist_wheel.py
--rwxr-xr-x   0        0        0    15930 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/macosx_libfile.py
--rwxr-xr-x   0        0        0     4344 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/metadata.py
--rwxr-xr-x   0        0        0     1257 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/pkginfo.py
--rwxr-xr-x   0        0        0      938 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/util.py
--rwxr-xr-x   0        0        0     7574 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/wheelfile.py
--rwxr-xr-x   0        0        0     2572 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/cli/__init__.py
--rwxr-xr-x   0        0        0     9498 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/cli/convert.py
--rwxr-xr-x   0        0        0     3364 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/cli/pack.py
--rwxr-xr-x   0        0        0      673 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/cli/unpack.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/vendored/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/vendored/packaging/__init__.py
--rwxr-xr-x   0        0        0     1812 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/vendored/packaging/_typing.py
--rwxr-xr-x   0        0        0    29560 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel/vendored/packaging/tags.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel-0.37.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1125 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel-0.37.1.dist-info/LICENSE.txt
--rwxr-xr-x   0        0        0     2328 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel-0.37.1.dist-info/METADATA
--rwxr-xr-x   0        0        0     2718 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel-0.37.1.dist-info/RECORD
--rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel-0.37.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0      108 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel-0.37.1.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/wheel-0.37.1.dist-info/top_level.txt
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/zipp-3.6.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/zipp-3.6.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     2263 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/zipp-3.6.0.dist-info/METADATA
--rwxr-xr-x   0        0        0      560 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/zipp-3.6.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/zipp-3.6.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0        5 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Lib/site-packages/zipp-3.6.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     2355 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/activate
--rwxr-xr-x   0        0        0      894 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/activate.bat
--rwxr-xr-x   0        0        0     1755 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/activate.ps1
--rwxr-xr-x   0        0        0     1179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/activate.xsh
--rwxr-xr-x   0        0        0     1517 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/activate_this.py
--rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0   102794 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/pip.exe
--rwxr-xr-x   0        0        0   102794 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/pip3.6.exe
--rwxr-xr-x   0        0        0   102794 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/pip3.exe
--rwxr-xr-x   0        0        0   106379 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/pyproject-build.exe
--rwxr-xr-x   0        0        0    99856 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/python.exe
--rwxr-xr-x   0        0        0    58384 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/python3.dll
--rwxr-xr-x   0        0        0  3619856 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/python36.dll
--rwxr-xr-x   0        0        0    98320 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/pythonw.exe
--rwxr-xr-x   0        0        0   102781 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/Scripts/wheel.exe
--rwxr-xr-x   0        0        0    21317 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/auto.tcl
--rwxr-xr-x   0        0        0   128934 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/clock.tcl
--rwxr-xr-x   0        0        0     7328 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/history.tcl
--rwxr-xr-x   0        0        0    24289 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/init.tcl
--rwxr-xr-x   0        0        0    22959 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/package.tcl
--rwxr-xr-x   0        0        0      816 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/parray.tcl
--rwxr-xr-x   0        0        0    33439 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/safe.tcl
--rwxr-xr-x   0        0        0     5415 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tclIndex
--rwxr-xr-x   0        0        0    11633 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tm.tcl
--rwxr-xr-x   0        0        0     4860 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/word.tcl
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/ascii.enc
--rwxr-xr-x   0        0        0    92873 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/big5.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp1250.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp1251.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp1252.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp1253.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp1254.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp1255.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp1256.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp1257.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp1258.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp437.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp737.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp775.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp850.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp852.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp855.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp857.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp860.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp861.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp862.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp863.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp864.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp865.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp866.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp869.enc
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp874.enc
--rwxr-xr-x   0        0        0    48207 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp932.enc
--rwxr-xr-x   0        0        0   132509 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp936.enc
--rwxr-xr-x   0        0        0   130423 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp949.enc
--rwxr-xr-x   0        0        0    91831 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/cp950.enc
--rwxr-xr-x   0        0        0     1093 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/dingbats.enc
--rwxr-xr-x   0        0        0     1054 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/ebcdic.enc
--rwxr-xr-x   0        0        0    85574 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/euc-cn.enc
--rwxr-xr-x   0        0        0    82537 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/euc-jp.enc
--rwxr-xr-x   0        0        0    93918 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/euc-kr.enc
--rwxr-xr-x   0        0        0    86619 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/gb12345.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/gb1988.enc
--rwxr-xr-x   0        0        0    84532 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/gb2312-raw.enc
--rwxr-xr-x   0        0        0    85574 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/gb2312.enc
--rwxr-xr-x   0        0        0      192 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso2022-jp.enc
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso2022-kr.enc
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso2022.enc
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-1.enc
--rwxr-xr-x   0        0        0     1095 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-10.enc
--rwxr-xr-x   0        0        0     1095 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-13.enc
--rwxr-xr-x   0        0        0     1095 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-14.enc
--rwxr-xr-x   0        0        0     1095 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-15.enc
--rwxr-xr-x   0        0        0     1095 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-16.enc
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-2.enc
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-3.enc
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-4.enc
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-5.enc
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-6.enc
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-7.enc
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-8.enc
--rwxr-xr-x   0        0        0     1094 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/iso8859-9.enc
--rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/jis0201.enc
--rwxr-xr-x   0        0        0    80453 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/jis0208.enc
--rwxr-xr-x   0        0        0    70974 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/jis0212.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/koi8-r.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/koi8-u.enc
--rwxr-xr-x   0        0        0    92877 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/ksc5601.enc
--rwxr-xr-x   0        0        0     1096 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macCentEuro.enc
--rwxr-xr-x   0        0        0     1096 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macCroatian.enc
--rwxr-xr-x   0        0        0     1096 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macCyrillic.enc
--rwxr-xr-x   0        0        0     1096 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macDingbats.enc
--rwxr-xr-x   0        0        0     1093 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macGreek.enc
--rwxr-xr-x   0        0        0     1095 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macIceland.enc
--rwxr-xr-x   0        0        0    48028 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macJapan.enc
--rwxr-xr-x   0        0        0     1093 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macRoman.enc
--rwxr-xr-x   0        0        0     1095 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macRomania.enc
--rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macThai.enc
--rwxr-xr-x   0        0        0     1095 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macTurkish.enc
--rwxr-xr-x   0        0        0     1095 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/macUkraine.enc
--rwxr-xr-x   0        0        0    41862 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/shiftjis.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/symbol.enc
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/encoding/tis-620.enc
--rwxr-xr-x   0        0        0     9689 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/http1.0/http.tcl
--rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/http1.0/pkgIndex.tcl
--rwxr-xr-x   0        0        0      989 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/af.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/af_za.msg
--rwxr-xr-x   0        0        0     1964 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ar.msg
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ar_in.msg
--rwxr-xr-x   0        0        0     1812 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ar_jo.msg
--rwxr-xr-x   0        0        0     1812 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ar_lb.msg
--rwxr-xr-x   0        0        0     1812 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ar_sy.msg
--rwxr-xr-x   0        0        0     2105 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/be.msg
--rwxr-xr-x   0        0        0     1819 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/bg.msg
--rwxr-xr-x   0        0        0     2286 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/bn.msg
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/bn_in.msg
--rwxr-xr-x   0        0        0     1102 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ca.msg
--rwxr-xr-x   0        0        0     1300 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/cs.msg
--rwxr-xr-x   0        0        0     1156 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/da.msg
--rwxr-xr-x   0        0        0     1222 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/de.msg
--rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/de_at.msg
--rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/de_be.msg
--rwxr-xr-x   0        0        0     2252 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/el.msg
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_au.msg
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_be.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_bw.msg
--rwxr-xr-x   0        0        0      288 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_ca.msg
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_gb.msg
--rwxr-xr-x   0        0        0      321 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_hk.msg
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_ie.msg
--rwxr-xr-x   0        0        0      310 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_in.msg
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_nz.msg
--rwxr-xr-x   0        0        0      321 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_ph.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_sg.msg
--rwxr-xr-x   0        0        0      245 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_za.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/en_zw.msg
--rwxr-xr-x   0        0        0     1231 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/eo.msg
--rwxr-xr-x   0        0        0     1180 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es.msg
--rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_ar.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_bo.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_cl.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_co.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_cr.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_do.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_ec.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_gt.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_hn.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_mx.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_ni.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_pa.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_pe.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_pr.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_py.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_sv.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_uy.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/es_ve.msg
--rwxr-xr-x   0        0        0     1206 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/et.msg
--rwxr-xr-x   0        0        0      985 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/eu.msg
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/eu_es.msg
--rwxr-xr-x   0        0        0     1664 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/fa.msg
--rwxr-xr-x   0        0        0     1957 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/fa_in.msg
--rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/fa_ir.msg
--rwxr-xr-x   0        0        0     1145 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/fi.msg
--rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/fo.msg
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/fo_fo.msg
--rwxr-xr-x   0        0        0     1205 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/fr.msg
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/fr_be.msg
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/fr_ca.msg
--rwxr-xr-x   0        0        0      281 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/fr_ch.msg
--rwxr-xr-x   0        0        0     1141 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ga.msg
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ga_ie.msg
--rwxr-xr-x   0        0        0      950 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/gl.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/gl_es.msg
--rwxr-xr-x   0        0        0     1037 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/gv.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/gv_gb.msg
--rwxr-xr-x   0        0        0     1938 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/he.msg
--rwxr-xr-x   0        0        0     1738 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/hi.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/hi_in.msg
--rwxr-xr-x   0        0        0     1121 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/hr.msg
--rwxr-xr-x   0        0        0     1327 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/hu.msg
--rwxr-xr-x   0        0        0      914 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/id.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/id_id.msg
--rwxr-xr-x   0        0        0     1255 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/is.msg
--rwxr-xr-x   0        0        0     1240 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/it.msg
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/it_ch.msg
--rwxr-xr-x   0        0        0     1664 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ja.msg
--rwxr-xr-x   0        0        0      978 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/kl.msg
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/kl_gl.msg
--rwxr-xr-x   0        0        0     1566 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ko.msg
--rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ko_kr.msg
--rwxr-xr-x   0        0        0     1958 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/kok.msg
--rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/kok_in.msg
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/kw.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/kw_gb.msg
--rwxr-xr-x   0        0        0     1255 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/lt.msg
--rwxr-xr-x   0        0        0     1219 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/lv.msg
--rwxr-xr-x   0        0        0     2105 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/mk.msg
--rwxr-xr-x   0        0        0     1807 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/mr.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/mr_in.msg
--rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ms.msg
--rwxr-xr-x   0        0        0      259 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ms_my.msg
--rwxr-xr-x   0        0        0      690 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/mt.msg
--rwxr-xr-x   0        0        0     1157 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/nb.msg
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/nl.msg
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/nl_be.msg
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/nn.msg
--rwxr-xr-x   0        0        0     1211 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/pl.msg
--rwxr-xr-x   0        0        0     1127 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/pt.msg
--rwxr-xr-x   0        0        0      279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/pt_br.msg
--rwxr-xr-x   0        0        0     1172 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ro.msg
--rwxr-xr-x   0        0        0     2039 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ru.msg
--rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ru_ua.msg
--rwxr-xr-x   0        0        0     1160 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/sh.msg
--rwxr-xr-x   0        0        0     1203 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/sk.msg
--rwxr-xr-x   0        0        0     1164 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/sl.msg
--rwxr-xr-x   0        0        0     1267 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/sq.msg
--rwxr-xr-x   0        0        0     2035 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/sr.msg
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/sv.msg
--rwxr-xr-x   0        0        0      991 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/sw.msg
--rwxr-xr-x   0        0        0     1835 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ta.msg
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/ta_in.msg
--rwxr-xr-x   0        0        0     2102 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/te.msg
--rwxr-xr-x   0        0        0      411 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/te_in.msg
--rwxr-xr-x   0        0        0     2305 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/th.msg
--rwxr-xr-x   0        0        0     1133 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/tr.msg
--rwxr-xr-x   0        0        0     2113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/uk.msg
--rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/vi.msg
--rwxr-xr-x   0        0        0     3330 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/zh.msg
--rwxr-xr-x   0        0        0      312 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/zh_cn.msg
--rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/zh_hk.msg
--rwxr-xr-x   0        0        0      339 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/zh_sg.msg
--rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/msgs/zh_tw.msg
--rwxr-xr-x   0        0        0    32718 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/opt0.4/optparse.tcl
--rwxr-xr-x   0        0        0      607 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/opt0.4/pkgIndex.tcl
--rwxr-xr-x   0        0        0     7471 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/CET
--rwxr-xr-x   0        0        0     8227 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/CST6CDT
--rwxr-xr-x   0        0        0      170 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Cuba
--rwxr-xr-x   0        0        0     7189 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/EET
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/EST
--rwxr-xr-x   0        0        0     8227 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/EST5EDT
--rwxr-xr-x   0        0        0      165 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Egypt
--rwxr-xr-x   0        0        0      167 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Eire
--rwxr-xr-x   0        0        0      165 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/GB
--rwxr-xr-x   0        0        0      170 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/GB-Eire
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/GMT
--rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/GMT+0
--rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/GMT-0
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/GMT0
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Greenwich
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/HST
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Hongkong
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Iceland
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Iran
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Israel
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Jamaica
--rwxr-xr-x   0        0        0      159 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Japan
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Kwajalein
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Libya
--rwxr-xr-x   0        0        0     7471 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/MET
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/MST
--rwxr-xr-x   0        0        0     8227 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/MST7MDT
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/NZ
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/NZ-CHAT
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Navajo
--rwxr-xr-x   0        0        0      166 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/PRC
--rwxr-xr-x   0        0        0     8227 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/PST8PDT
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Poland
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Portugal
--rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/ROC
--rwxr-xr-x   0        0        0      157 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/ROK
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Singapore
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Turkey
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/UCT
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/UTC
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Universal
--rwxr-xr-x   0        0        0      167 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/W-SU
--rwxr-xr-x   0        0        0     6694 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/WET
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Zulu
--rwxr-xr-x   0        0        0      141 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Abidjan
--rwxr-xr-x   0        0        0     1416 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Accra
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Addis_Ababa
--rwxr-xr-x   0        0        0     1041 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Algiers
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Asmara
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Asmera
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Bamako
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Bangui
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Banjul
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Bissau
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Blantyre
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Brazzaville
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Bujumbura
--rwxr-xr-x   0        0        0     3720 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Cairo
--rwxr-xr-x   0        0        0     6176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Casablanca
--rwxr-xr-x   0        0        0     7253 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Ceuta
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Conakry
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Dakar
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Dar_es_Salaam
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Djibouti
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Douala
--rwxr-xr-x   0        0        0     5885 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/El_Aaiun
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Freetown
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Gaborone
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Harare
--rwxr-xr-x   0        0        0      298 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Johannesburg
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Juba
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Kampala
--rwxr-xr-x   0        0        0     1063 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Khartoum
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Kigali
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Kinshasa
--rwxr-xr-x   0        0        0      141 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Lagos
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Libreville
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Lome
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Luanda
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Lubumbashi
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Lusaka
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Malabo
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Maputo
--rwxr-xr-x   0        0        0      194 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Maseru
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Mbabane
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Mogadishu
--rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Monrovia
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Nairobi
--rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Ndjamena
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Niamey
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Nouakchott
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Ouagadougou
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Porto-Novo
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Sao_Tome
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Timbuktu
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Tripoli
--rwxr-xr-x   0        0        0     1072 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Tunis
--rwxr-xr-x   0        0        0     6288 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Africa/Windhoek
--rwxr-xr-x   0        0        0     8171 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Adak
--rwxr-xr-x   0        0        0     8444 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Anchorage
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Anguilla
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Antigua
--rwxr-xr-x   0        0        0     1747 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Araguaina
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Aruba
--rwxr-xr-x   0        0        0     7810 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Asuncion
--rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Atikokan
--rwxr-xr-x   0        0        0      172 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Atka
--rwxr-xr-x   0        0        0     1974 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Bahia
--rwxr-xr-x   0        0        0     6625 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Bahia_Banderas
--rwxr-xr-x   0        0        0      413 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Barbados
--rwxr-xr-x   0        0        0     1010 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Belem
--rwxr-xr-x   0        0        0     1829 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Belize
--rwxr-xr-x   0        0        0      331 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Blanc-Sablon
--rwxr-xr-x   0        0        0     1175 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Boa_Vista
--rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Bogota
--rwxr-xr-x   0        0        0     8324 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Boise
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Buenos_Aires
--rwxr-xr-x   0        0        0     7487 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Cambridge_Bay
--rwxr-xr-x   0        0        0     7778 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Campo_Grande
--rwxr-xr-x   0        0        0     1365 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Cancun
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Caracas
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Catamarca
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Cayenne
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Cayman
--rwxr-xr-x   0        0        0    11003 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Chicago
--rwxr-xr-x   0        0        0     6593 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Chihuahua
--rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Coral_Harbour
--rwxr-xr-x   0        0        0      214 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Cordoba
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Costa_Rica
--rwxr-xr-x   0        0        0      211 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Creston
--rwxr-xr-x   0        0        0     7771 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Cuiaba
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Curacao
--rwxr-xr-x   0        0        0     1105 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Danmarkshavn
--rwxr-xr-x   0        0        0     7609 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Dawson
--rwxr-xr-x   0        0        0     1876 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Dawson_Creek
--rwxr-xr-x   0        0        0     8629 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Denver
--rwxr-xr-x   0        0        0     8068 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Detroit
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Dominica
--rwxr-xr-x   0        0        0     8435 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Edmonton
--rwxr-xr-x   0        0        0     1204 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Eirunepe
--rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/El_Salvador
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Ensenada
--rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Fort_Nelson
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Fort_Wayne
--rwxr-xr-x   0        0        0     1394 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Fortaleza
--rwxr-xr-x   0        0        0     8099 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Glace_Bay
--rwxr-xr-x   0        0        0     7306 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Godthab
--rwxr-xr-x   0        0        0    10015 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Goose_Bay
--rwxr-xr-x   0        0        0     2387 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Grand_Turk
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Grenada
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Guadeloupe
--rwxr-xr-x   0        0        0      385 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Guatemala
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Guayaquil
--rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Guyana
--rwxr-xr-x   0        0        0    10763 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Halifax
--rwxr-xr-x   0        0        0     8444 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Havana
--rwxr-xr-x   0        0        0      595 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Hermosillo
--rwxr-xr-x   0        0        0      228 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Indianapolis
--rwxr-xr-x   0        0        0     7389 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Inuvik
--rwxr-xr-x   0        0        0     7421 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Iqaluit
--rwxr-xr-x   0        0        0      818 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Jamaica
--rwxr-xr-x   0        0        0      206 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Jujuy
--rwxr-xr-x   0        0        0     8406 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Juneau
--rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Knox_IN
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Kralendijk
--rwxr-xr-x   0        0        0      211 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/La_Paz
--rwxr-xr-x   0        0        0      447 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Lima
--rwxr-xr-x   0        0        0     9409 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Los_Angeles
--rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Louisville
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Lower_Princes
--rwxr-xr-x   0        0        0     1507 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Maceio
--rwxr-xr-x   0        0        0      590 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Managua
--rwxr-xr-x   0        0        0     1142 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Manaus
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Marigot
--rwxr-xr-x   0        0        0      242 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Martinique
--rwxr-xr-x   0        0        0     6526 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Matamoros
--rwxr-xr-x   0        0        0     6619 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Mazatlan
--rwxr-xr-x   0        0        0      214 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Mendoza
--rwxr-xr-x   0        0        0     8136 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Menominee
--rwxr-xr-x   0        0        0     6435 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Merida
--rwxr-xr-x   0        0        0     6462 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Metlakatla
--rwxr-xr-x   0        0        0     6807 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Mexico_City
--rwxr-xr-x   0        0        0     7074 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Miquelon
--rwxr-xr-x   0        0        0    10165 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Moncton
--rwxr-xr-x   0        0        0     6496 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Monterrey
--rwxr-xr-x   0        0        0     2743 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Montevideo
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Montreal
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Montserrat
--rwxr-xr-x   0        0        0     8260 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Nassau
--rwxr-xr-x   0        0        0    11004 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/New_York
--rwxr-xr-x   0        0        0     7836 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Nipigon
--rwxr-xr-x   0        0        0     8404 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Nome
--rwxr-xr-x   0        0        0     1368 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Noronha
--rwxr-xr-x   0        0        0     6621 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Ojinaga
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Panama
--rwxr-xr-x   0        0        0     7484 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Pangnirtung
--rwxr-xr-x   0        0        0      272 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Paramaribo
--rwxr-xr-x   0        0        0      479 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Phoenix
--rwxr-xr-x   0        0        0     1418 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Port-au-Prince
--rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Port_of_Spain
--rwxr-xr-x   0        0        0      196 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Porto_Acre
--rwxr-xr-x   0        0        0     1030 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Porto_Velho
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Puerto_Rico
--rwxr-xr-x   0        0        0     7840 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Rainy_River
--rwxr-xr-x   0        0        0     7366 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Rankin_Inlet
--rwxr-xr-x   0        0        0     1391 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Recife
--rwxr-xr-x   0        0        0     1723 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Regina
--rwxr-xr-x   0        0        0     7362 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Resolute
--rwxr-xr-x   0        0        0     1089 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Rio_Branco
--rwxr-xr-x   0        0        0      214 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Rosario
--rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Santa_Isabel
--rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Santarem
--rwxr-xr-x   0        0        0     8719 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Santiago
--rwxr-xr-x   0        0        0      590 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Santo_Domingo
--rwxr-xr-x   0        0        0     7678 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Sao_Paulo
--rwxr-xr-x   0        0        0     6713 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Scoresbysund
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Shiprock
--rwxr-xr-x   0        0        0     8376 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Sitka
--rwxr-xr-x   0        0        0      208 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/St_Barthelemy
--rwxr-xr-x   0        0        0    10917 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/St_Johns
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/St_Kitts
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/St_Lucia
--rwxr-xr-x   0        0        0      204 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/St_Thomas
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/St_Vincent
--rwxr-xr-x   0        0        0      845 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Swift_Current
--rwxr-xr-x   0        0        0      329 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Tegucigalpa
--rwxr-xr-x   0        0        0     6666 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Thule
--rwxr-xr-x   0        0        0     8058 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Thunder_Bay
--rwxr-xr-x   0        0        0     8470 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Tijuana
--rwxr-xr-x   0        0        0    10883 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Toronto
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Tortola
--rwxr-xr-x   0        0        0     9495 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Vancouver
--rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Virgin
--rwxr-xr-x   0        0        0     7613 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Whitehorse
--rwxr-xr-x   0        0        0     9379 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Winnipeg
--rwxr-xr-x   0        0        0     8407 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Yakutat
--rwxr-xr-x   0        0        0     7485 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Yellowknife
--rwxr-xr-x   0        0        0     2010 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/Buenos_Aires
--rwxr-xr-x   0        0        0     2039 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/Catamarca
--rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/ComodRivadavia
--rwxr-xr-x   0        0        0     2006 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/Cordoba
--rwxr-xr-x   0        0        0     2005 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/Jujuy
--rwxr-xr-x   0        0        0     2067 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/La_Rioja
--rwxr-xr-x   0        0        0     2043 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/Mendoza
--rwxr-xr-x   0        0        0     2041 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/Rio_Gallegos
--rwxr-xr-x   0        0        0     1974 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/Salta
--rwxr-xr-x   0        0        0     2067 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/San_Juan
--rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/San_Luis
--rwxr-xr-x   0        0        0     2067 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/Tucuman
--rwxr-xr-x   0        0        0     2036 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Argentina/Ushuaia
--rwxr-xr-x   0        0        0     6996 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Indiana/Indianapolis
--rwxr-xr-x   0        0        0     8470 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Indiana/Knox
--rwxr-xr-x   0        0        0     7037 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Indiana/Marengo
--rwxr-xr-x   0        0        0     7364 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Indiana/Petersburg
--rwxr-xr-x   0        0        0     6992 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Indiana/Tell_City
--rwxr-xr-x   0        0        0     6350 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Indiana/Vevay
--rwxr-xr-x   0        0        0     6992 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Indiana/Vincennes
--rwxr-xr-x   0        0        0     7170 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Indiana/Winamac
--rwxr-xr-x   0        0        0     9332 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Kentucky/Louisville
--rwxr-xr-x   0        0        0     8279 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/Kentucky/Monticello
--rwxr-xr-x   0        0        0     8278 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/North_Dakota/Beulah
--rwxr-xr-x   0        0        0     8278 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/North_Dakota/Center
--rwxr-xr-x   0        0        0     8281 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/America/North_Dakota/New_Salem
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/Casey
--rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/Davis
--rwxr-xr-x   0        0        0      207 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/DumontDUrville
--rwxr-xr-x   0        0        0     2801 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/Macquarie
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/Mawson
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/McMurdo
--rwxr-xr-x   0        0        0     7598 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/Palmer
--rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/Rothera
--rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/South_Pole
--rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/Syowa
--rwxr-xr-x   0        0        0     5269 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/Troll
--rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Antarctica/Vostok
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Arctic/Longyearbyen
--rwxr-xr-x   0        0        0      166 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Aden
--rwxr-xr-x   0        0        0     1580 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Almaty
--rwxr-xr-x   0        0        0     7055 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Amman
--rwxr-xr-x   0        0        0     2126 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Anadyr
--rwxr-xr-x   0        0        0     1636 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Aqtau
--rwxr-xr-x   0        0        0     1608 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Aqtobe
--rwxr-xr-x   0        0        0      883 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Ashgabat
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Ashkhabad
--rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Baghdad
--rwxr-xr-x   0        0        0      166 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Bahrain
--rwxr-xr-x   0        0        0     2131 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Baku
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Bangkok
--rwxr-xr-x   0        0        0     2044 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Barnaul
--rwxr-xr-x   0        0        0     7754 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Beirut
--rwxr-xr-x   0        0        0     1631 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Bishkek
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Brunei
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Calcutta
--rwxr-xr-x   0        0        0     2120 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Chita
--rwxr-xr-x   0        0        0     6701 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Choibalsan
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Chongqing
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Chungking
--rwxr-xr-x   0        0        0      347 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Colombo
--rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Dacca
--rwxr-xr-x   0        0        0     8031 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Damascus
--rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Dhaka
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Dili
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Dubai
--rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Dushanbe
--rwxr-xr-x   0        0        0     7963 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Gaza
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Harbin
--rwxr-xr-x   0        0        0     7939 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Hebron
--rwxr-xr-x   0        0        0      381 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Ho_Chi_Minh
--rwxr-xr-x   0        0        0     2150 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Hong_Kong
--rwxr-xr-x   0        0        0     6665 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Hovd
--rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Irkutsk
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Istanbul
--rwxr-xr-x   0        0        0      350 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Jakarta
--rwxr-xr-x   0        0        0      204 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Jayapura
--rwxr-xr-x   0        0        0     7690 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Jerusalem
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Kabul
--rwxr-xr-x   0        0        0     2097 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Kamchatka
--rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Karachi
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Kashgar
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Kathmandu
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Katmandu
--rwxr-xr-x   0        0        0     2156 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Khandyga
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Kolkata
--rwxr-xr-x   0        0        0     2096 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Krasnoyarsk
--rwxr-xr-x   0        0        0      360 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Kuala_Lumpur
--rwxr-xr-x   0        0        0      703 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Kuching
--rwxr-xr-x   0        0        0      168 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Kuwait
--rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Macao
--rwxr-xr-x   0        0        0     1286 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Macau
--rwxr-xr-x   0        0        0     2122 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Magadan
--rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Makassar
--rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Manila
--rwxr-xr-x   0        0        0      165 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Muscat
--rwxr-xr-x   0        0        0     7368 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Nicosia
--rwxr-xr-x   0        0        0     1992 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Novokuznetsk
--rwxr-xr-x   0        0        0     2048 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Novosibirsk
--rwxr-xr-x   0        0        0     2089 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Omsk
--rwxr-xr-x   0        0        0     1606 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Oral
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Phnom_Penh
--rwxr-xr-x   0        0        0      350 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Pontianak
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Pyongyang
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Qatar
--rwxr-xr-x   0        0        0     1583 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Qyzylorda
--rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Rangoon
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Riyadh
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Saigon
--rwxr-xr-x   0        0        0     2184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Sakhalin
--rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Samarkand
--rwxr-xr-x   0        0        0      750 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Seoul
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Shanghai
--rwxr-xr-x   0        0        0      386 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Singapore
--rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Srednekolymsk
--rwxr-xr-x   0        0        0     1299 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Taipei
--rwxr-xr-x   0        0        0      911 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Tashkent
--rwxr-xr-x   0        0        0     1719 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Tbilisi
--rwxr-xr-x   0        0        0     6804 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Tehran
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Tel_Aviv
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Thimbu
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Thimphu
--rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Tokyo
--rwxr-xr-x   0        0        0     2043 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Tomsk
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Ujung_Pandang
--rwxr-xr-x   0        0        0     6672 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Ulaanbaatar
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Ulan_Bator
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Urumqi
--rwxr-xr-x   0        0        0     2089 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Ust-Nera
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Vientiane
--rwxr-xr-x   0        0        0     2096 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Vladivostok
--rwxr-xr-x   0        0        0     2092 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Yakutsk
--rwxr-xr-x   0        0        0     2128 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Yekaterinburg
--rwxr-xr-x   0        0        0     2013 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Asia/Yerevan
--rwxr-xr-x   0        0        0    10092 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/Azores
--rwxr-xr-x   0        0        0     7684 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/Bermuda
--rwxr-xr-x   0        0        0     6610 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/Canary
--rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/Cape_Verde
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/Faeroe
--rwxr-xr-x   0        0        0     6551 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/Faroe
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/Jan_Mayen
--rwxr-xr-x   0        0        0     9568 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/Madeira
--rwxr-xr-x   0        0        0     1995 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/Reykjavik
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/South_Georgia
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/St_Helena
--rwxr-xr-x   0        0        0     2215 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Atlantic/Stanley
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/ACT
--rwxr-xr-x   0        0        0     8099 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Adelaide
--rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Brisbane
--rwxr-xr-x   0        0        0     8162 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Broken_Hill
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Canberra
--rwxr-xr-x   0        0        0     8097 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Currie
--rwxr-xr-x   0        0        0      422 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Darwin
--rwxr-xr-x   0        0        0      734 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Eucla
--rwxr-xr-x   0        0        0     8325 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Hobart
--rwxr-xr-x   0        0        0      194 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/LHI
--rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Lindeman
--rwxr-xr-x   0        0        0     7251 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Lord_Howe
--rwxr-xr-x   0        0        0     8069 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Melbourne
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/NSW
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/North
--rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Perth
--rwxr-xr-x   0        0        0      198 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Queensland
--rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/South
--rwxr-xr-x   0        0        0     8066 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Sydney
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Tasmania
--rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Victoria
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/West
--rwxr-xr-x   0        0        0      207 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Australia/Yancowinna
--rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Brazil/Acre
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Brazil/DeNoronha
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Brazil/East
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Brazil/West
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Canada/Atlantic
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Canada/Central
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Canada/East-Saskatchewan
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Canada/Eastern
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Canada/Mountain
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Canada/Newfoundland
--rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Canada/Pacific
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Canada/Saskatchewan
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Canada/Yukon
--rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Chile/Continental
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Chile/EasterIsland
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+0
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+1
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+10
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+11
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+12
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+2
--rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+3
--rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+4
--rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+5
--rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+6
--rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+7
--rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+8
--rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT+9
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-0
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-1
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-10
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-11
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-12
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-13
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-14
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-2
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-3
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-4
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-5
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-6
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-7
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-8
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT-9
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/GMT0
--rwxr-xr-x   0        0        0      158 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/Greenwich
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/UCT
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/UTC
--rwxr-xr-x   0        0        0      158 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/Universal
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Etc/Zulu
--rwxr-xr-x   0        0        0     8783 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Amsterdam
--rwxr-xr-x   0        0        0     6690 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Andorra
--rwxr-xr-x   0        0        0     1992 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Astrakhan
--rwxr-xr-x   0        0        0     7686 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Athens
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Belfast
--rwxr-xr-x   0        0        0     7059 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Belgrade
--rwxr-xr-x   0        0        0     7746 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Berlin
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Bratislava
--rwxr-xr-x   0        0        0     8907 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Brussels
--rwxr-xr-x   0        0        0     7706 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Bucharest
--rwxr-xr-x   0        0        0     7975 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Budapest
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Busingen
--rwxr-xr-x   0        0        0     7824 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Chisinau
--rwxr-xr-x   0        0        0     7458 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Copenhagen
--rwxr-xr-x   0        0        0     9476 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Dublin
--rwxr-xr-x   0        0        0     9181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Gibraltar
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Guernsey
--rwxr-xr-x   0        0        0     7120 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Helsinki
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Isle_of_Man
--rwxr-xr-x   0        0        0     8793 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Istanbul
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Jersey
--rwxr-xr-x   0        0        0     2397 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Kaliningrad
--rwxr-xr-x   0        0        0     7202 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Kiev
--rwxr-xr-x   0        0        0     1959 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Kirov
--rwxr-xr-x   0        0        0     9471 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Lisbon
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Ljubljana
--rwxr-xr-x   0        0        0     9839 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/London
--rwxr-xr-x   0        0        0     8826 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Luxembourg
--rwxr-xr-x   0        0        0     8282 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Madrid
--rwxr-xr-x   0        0        0     8425 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Malta
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Mariehamn
--rwxr-xr-x   0        0        0     2131 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Minsk
--rwxr-xr-x   0        0        0     8871 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Monaco
--rwxr-xr-x   0        0        0     2347 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Moscow
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Nicosia
--rwxr-xr-x   0        0        0     7651 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Oslo
--rwxr-xr-x   0        0        0     8838 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Paris
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Podgorica
--rwxr-xr-x   0        0        0     7684 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Prague
--rwxr-xr-x   0        0        0     7400 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Riga
--rwxr-xr-x   0        0        0     8481 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Rome
--rwxr-xr-x   0        0        0     2143 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Samara
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/San_Marino
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Sarajevo
--rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Simferopol
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Skopje
--rwxr-xr-x   0        0        0     7396 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Sofia
--rwxr-xr-x   0        0        0     7058 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Stockholm
--rwxr-xr-x   0        0        0     7295 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Tallinn
--rwxr-xr-x   0        0        0     7412 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Tirane
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Tiraspol
--rwxr-xr-x   0        0        0     2046 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Ulyanovsk
--rwxr-xr-x   0        0        0     7287 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Uzhgorod
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Vaduz
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Vatican
--rwxr-xr-x   0        0        0     7659 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Vienna
--rwxr-xr-x   0        0        0     7233 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Vilnius
--rwxr-xr-x   0        0        0     2064 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Volgograd
--rwxr-xr-x   0        0        0     8366 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Warsaw
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Zagreb
--rwxr-xr-x   0        0        0     7236 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Zaporozhye
--rwxr-xr-x   0        0        0     7055 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Europe/Zurich
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Antananarivo
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Chagos
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Christmas
--rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Cocos
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Comoro
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Kerguelen
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Mahe
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Maldives
--rwxr-xr-x   0        0        0      264 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Mauritius
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Mayotte
--rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Indian/Reunion
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Mexico/BajaNorte
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Mexico/BajaSur
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Mexico/General
--rwxr-xr-x   0        0        0     5607 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Apia
--rwxr-xr-x   0        0        0     8487 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Auckland
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Bougainville
--rwxr-xr-x   0        0        0     7907 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Chatham
--rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Chuuk
--rwxr-xr-x   0        0        0     8328 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Easter
--rwxr-xr-x   0        0        0      715 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Efate
--rwxr-xr-x   0        0        0      211 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Enderbury
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Fakaofo
--rwxr-xr-x   0        0        0     5598 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Fiji
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Funafuti
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Galapagos
--rwxr-xr-x   0        0        0      150 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Gambier
--rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Guadalcanal
--rwxr-xr-x   0        0        0      204 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Guam
--rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Honolulu
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Johnston
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Kiritimati
--rwxr-xr-x   0        0        0      204 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Kosrae
--rwxr-xr-x   0        0        0      206 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Kwajalein
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Majuro
--rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Marquesas
--rwxr-xr-x   0        0        0      189 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Midway
--rwxr-xr-x   0        0        0      231 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Nauru
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Niue
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Norfolk
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Noumea
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Pago_Pago
--rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Palau
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Pitcairn
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Pohnpei
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Ponape
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Port_Moresby
--rwxr-xr-x   0        0        0      931 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Rarotonga
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Saipan
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Samoa
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Tahiti
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Tarawa
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Tongatapu
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Truk
--rwxr-xr-x   0        0        0      145 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Wake
--rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Wallis
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/Pacific/Yap
--rwxr-xr-x   0        0        0      196 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/AST4
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/AST4ADT
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/CST6
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/CST6CDT
--rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/EST5
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/EST5EDT
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/HST10
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/MST7
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/MST7MDT
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/PST8
--rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/PST8PDT
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/YST9
--rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/SystemV/YST9YDT
--rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Alaska
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Aleutian
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Arizona
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Central
--rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/East-Indiana
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Eastern
--rwxr-xr-x   0        0        0      181 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Hawaii
--rwxr-xr-x   0        0        0      201 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Indiana-Starke
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Michigan
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Mountain
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Pacific
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Pacific-New
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tcl8.6/tzdata/US/Samoa
--rwxr-xr-x   0        0        0     8246 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/bgerror.tcl
--rwxr-xr-x   0        0        0    20642 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/button.tcl
--rwxr-xr-x   0        0        0     9652 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/choosedir.tcl
--rwxr-xr-x   0        0        0    21432 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/clrpick.tcl
--rwxr-xr-x   0        0        0     8229 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/comdlg.tcl
--rwxr-xr-x   0        0        0    32740 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/console.tcl
--rwxr-xr-x   0        0        0     6025 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/dialog.tcl
--rwxr-xr-x   0        0        0    16950 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/entry.tcl
--rwxr-xr-x   0        0        0     4857 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/focus.tcl
--rwxr-xr-x   0        0        0    15685 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/fontchooser.tcl
--rwxr-xr-x   0        0        0    15978 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/iconlist.tcl
--rwxr-xr-x   0        0        0    10883 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/icons.tcl
--rwxr-xr-x   0        0        0     2267 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/license.terms
--rwxr-xr-x   0        0        0    14603 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/listbox.tcl
--rwxr-xr-x   0        0        0     9569 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/megawidget.tcl
--rwxr-xr-x   0        0        0    37914 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/menu.tcl
--rwxr-xr-x   0        0        0    29352 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/mkpsenc.tcl
--rwxr-xr-x   0        0        0    16471 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgbox.tcl
--rwxr-xr-x   0        0        0     5594 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/obsolete.tcl
--rwxr-xr-x   0        0        0     1586 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/optMenu.tcl
--rwxr-xr-x   0        0        0     7923 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/palette.tcl
--rwxr-xr-x   0        0        0     5176 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/panedwindow.tcl
--rwxr-xr-x   0        0        0      371 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/pkgIndex.tcl
--rwxr-xr-x   0        0        0     7381 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/safetk.tcl
--rwxr-xr-x   0        0        0     7766 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/scale.tcl
--rwxr-xr-x   0        0        0    12748 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/scrlbar.tcl
--rwxr-xr-x   0        0        0    15640 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/spinbox.tcl
--rwxr-xr-x   0        0        0    20270 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/tclIndex
--rwxr-xr-x   0        0        0     5142 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/tearoff.tcl
--rwxr-xr-x   0        0        0    32996 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/text.tcl
--rwxr-xr-x   0        0        0    23066 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/tk.tcl
--rwxr-xr-x   0        0        0    38255 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/tkfbox.tcl
--rwxr-xr-x   0        0        0    10252 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/unsupported.tcl
--rwxr-xr-x   0        0        0    26031 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/xmfbox.tcl
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/README
--rwxr-xr-x   0        0        0     6670 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/anilabel.tcl
--rwxr-xr-x   0        0        0     3494 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/aniwave.tcl
--rwxr-xr-x   0        0        0     7984 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/arrow.tcl
--rwxr-xr-x   0        0        0     2948 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/bind.tcl
--rwxr-xr-x   0        0        0     1411 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/bitmap.tcl
--rwxr-xr-x   0        0        0     1755 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/browse
--rwxr-xr-x   0        0        0     1504 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/button.tcl
--rwxr-xr-x   0        0        0     2278 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/check.tcl
--rwxr-xr-x   0        0        0     1431 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/clrpick.tcl
--rwxr-xr-x   0        0        0     4995 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/colors.tcl
--rwxr-xr-x   0        0        0     1963 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/combo.tcl
--rwxr-xr-x   0        0        0     3389 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/cscroll.tcl
--rwxr-xr-x   0        0        0     6019 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/ctext.tcl
--rwxr-xr-x   0        0        0      660 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/dialog1.tcl
--rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/dialog2.tcl
--rwxr-xr-x   0        0        0     3871 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/en.msg
--rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/entry1.tcl
--rwxr-xr-x   0        0        0     2081 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/entry2.tcl
--rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/entry3.tcl
--rwxr-xr-x   0        0        0     2351 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/filebox.tcl
--rwxr-xr-x   0        0        0    79108 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/floor.tcl
--rwxr-xr-x   0        0        0     1752 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/fontchoose.tcl
--rwxr-xr-x   0        0        0     1046 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/form.tcl
--rwxr-xr-x   0        0        0    56556 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/goldberg.tcl
--rwxr-xr-x   0        0        0      509 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/hello
--rwxr-xr-x   0        0        0     1497 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/hscale.tcl
--rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/icon.tcl
--rwxr-xr-x   0        0        0     1002 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/image1.tcl
--rwxr-xr-x   0        0        0     3352 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/image2.tcl
--rwxr-xr-x   0        0        0    10133 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/items.tcl
--rwxr-xr-x   0        0        0     8065 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/ixset
--rwxr-xr-x   0        0        0     9140 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/knightstour.tcl
--rwxr-xr-x   0        0        0     1379 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/label.tcl
--rwxr-xr-x   0        0        0     1847 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/labelframe.tcl
--rwxr-xr-x   0        0        0     2267 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/license.terms
--rwxr-xr-x   0        0        0     4357 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/mclist.tcl
--rwxr-xr-x   0        0        0     6729 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/menu.tcl
--rwxr-xr-x   0        0        0     4476 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/menubu.tcl
--rwxr-xr-x   0        0        0     1998 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/msgbox.tcl
--rwxr-xr-x   0        0        0     6753 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/nl.msg
--rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/paned1.tcl
--rwxr-xr-x   0        0        0     2244 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/paned2.tcl
--rwxr-xr-x   0        0        0     7596 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/pendulum.tcl
--rwxr-xr-x   0        0        0     2758 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/plot.tcl
--rwxr-xr-x   0        0        0     2596 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/puzzle.tcl
--rwxr-xr-x   0        0        0     2752 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/radio.tcl
--rwxr-xr-x   0        0        0     5316 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/rmt
--rwxr-xr-x   0        0        0     8297 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/rolodex
--rwxr-xr-x   0        0        0     5211 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/ruler.tcl
--rwxr-xr-x   0        0        0     2273 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/sayings.tcl
--rwxr-xr-x   0        0        0     4403 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/search.tcl
--rwxr-xr-x   0        0        0     1820 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/spin.tcl
--rwxr-xr-x   0        0        0     1314 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/square
--rwxr-xr-x   0        0        0     2048 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/states.tcl
--rwxr-xr-x   0        0        0     6943 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/style.tcl
--rwxr-xr-x   0        0        0     4354 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/tclIndex
--rwxr-xr-x   0        0        0    11247 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/tcolor
--rwxr-xr-x   0        0        0     4267 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/text.tcl
--rwxr-xr-x   0        0        0     2188 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/textpeer.tcl
--rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/timer
--rwxr-xr-x   0        0        0     3264 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/toolbar.tcl
--rwxr-xr-x   0        0        0     3162 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/tree.tcl
--rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/ttkbut.tcl
--rwxr-xr-x   0        0        0     2391 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/ttkmenu.tcl
--rwxr-xr-x   0        0        0     2317 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/ttknote.tcl
--rwxr-xr-x   0        0        0     4172 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/ttkpane.tcl
--rwxr-xr-x   0        0        0     1536 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/ttkprogress.tcl
--rwxr-xr-x   0        0        0     1420 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/ttkscale.tcl
--rwxr-xr-x   0        0        0    10836 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/twind.tcl
--rwxr-xr-x   0        0        0     4399 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/unicodeout.tcl
--rwxr-xr-x   0        0        0     1477 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/vscale.tcl
--rwxr-xr-x   0        0        0    23264 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/widget
--rwxr-xr-x   0        0        0    51712 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/earth.gif
--rwxr-xr-x   0        0        0     6343 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/earthris.gif
--rwxr-xr-x   0        0        0     1886 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/flagdown.xbm
--rwxr-xr-x   0        0        0     1880 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/flagup.xbm
--rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/gray25.xbm
--rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/letters.xbm
--rwxr-xr-x   0        0        0     1889 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/noletter.xbm
--rwxr-xr-x   0        0        0    54257 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/ouster.png
--rwxr-xr-x   0        0        0      272 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/pattern.xbm
--rwxr-xr-x   0        0        0     2341 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/tcllogo.gif
--rwxr-xr-x   0        0        0   196623 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/demos/images/teapot.ppm
--rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/README
--rwxr-xr-x   0        0        0    32900 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/logo.eps
--rwxr-xr-x   0        0        0     2341 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/logo100.gif
--rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/logo64.gif
--rwxr-xr-x   0        0        0    11000 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/logoLarge.gif
--rwxr-xr-x   0        0        0     3889 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/logoMed.gif
--rwxr-xr-x   0        0        0    27809 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/pwrdLogo.eps
--rwxr-xr-x   0        0        0     1615 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/pwrdLogo100.gif
--rwxr-xr-x   0        0        0     2489 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/pwrdLogo150.gif
--rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/pwrdLogo175.gif
--rwxr-xr-x   0        0        0     3491 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/pwrdLogo200.gif
--rwxr-xr-x   0        0        0     1171 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/pwrdLogo75.gif
--rwxr-xr-x   0        0        0     5473 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/images/tai-ku.gif
--rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/cs.msg
--rwxr-xr-x   0        0        0     3909 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/da.msg
--rwxr-xr-x   0        0        0     4823 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/de.msg
--rwxr-xr-x   0        0        0     8698 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/el.msg
--rwxr-xr-x   0        0        0     3286 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/en.msg
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/en_gb.msg
--rwxr-xr-x   0        0        0     3916 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/eo.msg
--rwxr-xr-x   0        0        0     3948 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/es.msg
--rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/fr.msg
--rwxr-xr-x   0        0        0     4600 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/hu.msg
--rwxr-xr-x   0        0        0     3692 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/it.msg
--rwxr-xr-x   0        0        0     4466 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/nl.msg
--rwxr-xr-x   0        0        0     4841 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/pl.msg
--rwxr-xr-x   0        0        0     3913 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/pt.msg
--rwxr-xr-x   0        0        0     7214 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/ru.msg
--rwxr-xr-x   0        0        0     3832 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/msgs/sv.msg
--rwxr-xr-x   0        0        0     3342 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/altTheme.tcl
--rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/aquaTheme.tcl
--rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/button.tcl
--rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/clamTheme.tcl
--rwxr-xr-x   0        0        0     3520 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/classicTheme.tcl
--rwxr-xr-x   0        0        0    12394 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/combobox.tcl
--rwxr-xr-x   0        0        0     4007 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/cursors.tcl
--rwxr-xr-x   0        0        0     3684 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/defaults.tcl
--rwxr-xr-x   0        0        0    16396 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/entry.tcl
--rwxr-xr-x   0        0        0     5576 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/fonts.tcl
--rwxr-xr-x   0        0        0     4913 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/menubutton.tcl
--rwxr-xr-x   0        0        0     5619 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/notebook.tcl
--rwxr-xr-x   0        0        0     1920 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/panedwindow.tcl
--rwxr-xr-x   0        0        0     1089 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/progress.tcl
--rwxr-xr-x   0        0        0     2698 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/scale.tcl
--rwxr-xr-x   0        0        0     3097 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/scrollbar.tcl
--rwxr-xr-x   0        0        0     2392 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/sizegrip.tcl
--rwxr-xr-x   0        0        0     4255 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/spinbox.tcl
--rwxr-xr-x   0        0        0     8859 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/treeview.tcl
--rwxr-xr-x   0        0        0     4546 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/ttk.tcl
--rwxr-xr-x   0        0        0     8562 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/utils.tcl
--rwxr-xr-x   0        0        0     9349 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/vistaTheme.tcl
--rwxr-xr-x   0        0        0     2643 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/winTheme.tcl
--rwxr-xr-x   0        0        0     1920 2020-02-02 00:00:00.000000 infinitydb-1.0.0/env/tcl/tk8.6/ttk/xpTheme.tcl
--rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 infinitydb-1.0.0/src/infinitydb/__init__.py
--rwxr-xr-x   0        0        0    66136 2020-02-02 00:00:00.000000 infinitydb-1.0.0/src/infinitydb/access.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 infinitydb-1.0.0/src/infinitydb.egg-info/PKG-INFO
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 infinitydb-1.0.0/src/infinitydb.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 infinitydb-1.0.0/src/infinitydb.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 infinitydb-1.0.0/src/infinitydb.egg-info/top_level.txt
--rwxr-xr-x   0        0        0      167 2020-02-02 00:00:00.000000 infinitydb-1.0.0/.gitignore
--rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.0/LICENSE
--rwxr-xr-x   0        0        0      961 2020-02-02 00:00:00.000000 infinitydb-1.0.0/README.md
--rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 infinitydb-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 infinitydb-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 infinitydb-1.0.1/src/infinitydb/__init__.py
+-rwxr-xr-x   0        0        0    66268 2020-02-02 00:00:00.000000 infinitydb-1.0.1/src/infinitydb/access.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 infinitydb-1.0.1/src/infinitydb.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 infinitydb-1.0.1/src/infinitydb.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 infinitydb-1.0.1/src/infinitydb.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 infinitydb-1.0.1/src/infinitydb.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0      167 2020-02-02 00:00:00.000000 infinitydb-1.0.1/.gitignore
+-rwxr-xr-x   0        0        0     1091 2020-02-02 00:00:00.000000 infinitydb-1.0.1/LICENSE
+-rwxr-xr-x   0        0        0      969 2020-02-02 00:00:00.000000 infinitydb-1.0.1/README.md
+-rwxr-xr-x   0        0        0      586 2020-02-02 00:00:00.000000 infinitydb-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 infinitydb-1.0.1/PKG-INFO
```

### Comparing `infinitydb-1.0.0/env/Lib/importlib/_bootstrap_external.py` & `infinitydb-1.0.1/src/infinitydb/access.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1443 +1,1712 @@
-"""Core implementation of path-based import.
-
-This module is NOT meant to be directly imported! It has been designed such
-that it can be bootstrapped into Python as the implementation of import. As
-such it requires the injection of specific modules and attributes in order to
-work. One should use importlib as the public-facing version of this module.
-
-"""
+# MIT License
 #
-# IMPORTANT: Whenever making changes to this module, be sure to run
-# a top-level make in order to get the frozen version of the module
-# updated. Not doing so will result in the Makefile to fail for
-# all others who don't have a ./python around to freeze the module
-# in the early stages of compilation.
+# Copyright (c) 2023 Roger L Deran
 #
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
 
-# See importlib._setup() for what is injected into the global namespace.
-
-# When editing this code be aware that code executed at import time CANNOT
-# reference any injected objects! This includes not only global code but also
-# anything specified at the class level.
-
-# Bootstrap-related code ######################################################
-_CASE_INSENSITIVE_PLATFORMS_STR_KEY = 'win',
-_CASE_INSENSITIVE_PLATFORMS_BYTES_KEY = 'cygwin', 'darwin'
-_CASE_INSENSITIVE_PLATFORMS =  (_CASE_INSENSITIVE_PLATFORMS_BYTES_KEY
-                                + _CASE_INSENSITIVE_PLATFORMS_STR_KEY)
-
-
-def _make_relax_case():
-    if sys.platform.startswith(_CASE_INSENSITIVE_PLATFORMS):
-        if sys.platform.startswith(_CASE_INSENSITIVE_PLATFORMS_STR_KEY):
-            key = 'PYTHONCASEOK'
-        else:
-            key = b'PYTHONCASEOK'
-
-        def _relax_case():
-            """True if filenames must be checked case-insensitively."""
-            return key in _os.environ
-    else:
-        def _relax_case():
-            """True if filenames must be checked case-insensitively."""
-            return False
-    return _relax_case
-
-
-def _w_long(x):
-    """Convert a 32-bit integer to little-endian."""
-    return (int(x) & 0xFFFFFFFF).to_bytes(4, 'little')
-
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""InfinityDB database access utilities
 
-def _r_long(int_bytes):
-    """Convert 4 bytes in little-endian to an integer."""
-    return int.from_bytes(int_bytes, 'little')
+Allow access to an InfinityDB database server via http(s) 
+REST requests and JSON encoded data or blobs. See boilerbay.com. 
 
+The rest of the InfinityDB software is not free or open source. That
+includes mostly the server itself, while client access code is open source.
 
-def _path_join(*path_parts):
-    """Replacement for os.path.join()."""
-    return path_sep.join([part.rstrip(path_separators)
-                          for part in path_parts if part])
+Requires Python 3. 
+"""
 
+import base64
+import datetime
+import json
+import re
+import ssl
+from urllib.parse import urlparse
+import urllib.request
+
+import dateutil.parser
+from requests import Request, Session
+from requests.exceptions import ConnectionError
+
+
+__author__ = 'Roger L Deran'
+__version__ = '1.2'
+__all__ = ['InfinityDBAccessor',
+           'InfinityDBError',
+           'escape_uri_components',
+           'underscore_quote',
+           'underscore_quote_key',
+           'underscore_unquote',
+           'parse_primitive',
+           'to_json_extended',
+           'Attribute',
+           'EntityClass',
+           'Index',
+           'flatten_to_tuples',
+           'unflatten_from_tuples',
+           'flatten_lists_to_indexes',
+           'unflatten_lists_from_indexes',
+           'compact_tree_tips',
+           'uncompact_tree_tips',
+           'is_legal_entity_class_name',
+           'is_legal_attribute_name',
+           'parse_token_string_into_components',
+           'item_to_tuples',
+           'json_quote_primitives',
+           'json_quote_primitive'
+           ]
 
-def _path_split(path):
-    """Replacement for os.path.split()."""
-    if len(path_separators) == 1:
-        front, _, tail = path.rpartition(path_sep)
-        return front, tail
-    for x in reversed(path):
-        if x in path_separators:
-            front, tail = path.rsplit(x, maxsplit=1)
-            return front, tail
-    return '', path
+"""
+'first_item',
+'first_component',
+'first_tuple',
+'next_item',
+'next_component',
+'next_tuple',
+'last_item',
+'last_component',
+'last_tuple',
+'previous_item',
+'previous_component',
+'previous_tuple',
+'get_items',
+'get_items_batch',
+'execute_query',
+"""
 
 
-def _path_stat(path):
-    """Stat the path.
+def is_legal_entity_class_name(s):
+    return (_entity_class_attribute_regex.match(s)
+            and s[0] >= 'A' and s[0] <= 'Z')
+
+
+def is_legal_attribute_name(s):
+    return (_entity_class_attribute_regex.match(s)
+             and s[0] >= 'a' and s[0] <= 'z')
+
+""" The special InfinityDB components that can appear in an Item.
+
+Their names match [a-zA-Z][a-zA-Z0-9_.-]* or are numeric ids.
+An EntityClass component is normally first and can be thought of as
+a 'table name'.  It can occur later frequently.
+An Attribute component is like a 'column name'.  For an 
+EntityClass 'E' and a primitive or composite called 'entity', 
+and an Attribute 'a', and a primitive  or composite 'v', 
+one often sees: [E, e, a, v] as a 'quad', sometimes with 
+an 'inversion' [EInverse, v, aInverse, e]. EntityClasses 
+start with an uppercase letter, Attributes with lowercase.
+"""
 
-    Made a separate function to make it easier to override in experiments
-    (e.g. cache stat results).
 
+# TODO it would be good to be able to compare magnitudes of different
+# component types, including EntityClass, Attribute, and Index,
+# as well as the primitive component types since that is possible
+# in InfinityDB as components of Items. In fact all component types
+# can be compared, and there is a fixed order of the types,
+# with Index last.
+#
+# Also, EC and Att identified using ids should sort differently
+# from the named ones, but we just use the string in any case,
+# and that comparison will be slower, but the
+# id-based ones are rare now.
+class EntityClass:
+    """ EntityClass corresponds to the InfinityDB EntityClass 
+    component type.
+    
+    When a JSON-encoded access to the InfinityDB server occurs, 
+    any EntityClass components in the Items transferred use 
+    EntityClass instances as the keys in corresponding dict. 
+    
+    An EntityClass is identified solely by its string 
+    value, or if that is not given, then it is 
+    identified by its integer id.
     """
-    return _os.stat(path)
 
+    def __init__(self, value):
+        if isinstance(value, str):
+            self.s = value
+            self.id = -1
+            if not is_legal_entity_class_name(value):
+                raise ValueError(
+                    "InfinityDB EntityClass name "
+                    "must match [A-Z][A-Za-z0-9._-]*: " + value
+                    )
+        elif isinstance(value, int):
+            self.s = 'EntityClass(' + str(value) + ')'
+            self.id = int(value)
+        else:
+            raise ValueError("An EntityClass "
+                             "requires a string or int")
 
-def _path_is_mode_type(path, mode):
-    """Test whether the path is the specified mode type."""
-    try:
-        stat_info = _path_stat(path)
-    except OSError:
-        return False
-    return (stat_info.st_mode & 0o170000) == mode
+    def __str__(self):
+        return self.s
 
+    def __repr__(self):
+        return self.s
 
-def _path_isfile(path):
-    """Replacement for os.path.isfile."""
-    return _path_is_mode_type(path, 0o100000)
-
-
-def _path_isdir(path):
-    """Replacement for os.path.isdir."""
-    if not path:
-        path = _os.getcwd()
-    return _path_is_mode_type(path, 0o040000)
-
-
-def _write_atomic(path, data, mode=0o666):
-    """Best-effort function to write data to a path atomically.
-    Be prepared to handle a FileExistsError if concurrent writing of the
-    temporary file is attempted."""
-    # id() is used to generate a pseudo-random filename.
-    path_tmp = '{}.{}'.format(path, id(path))
-    fd = _os.open(path_tmp,
-                  _os.O_EXCL | _os.O_CREAT | _os.O_WRONLY, mode & 0o666)
-    try:
-        # We first write data to a temporary file, and then use os.replace() to
-        # perform an atomic rename.
-        with _io.FileIO(fd, 'wb') as file:
-            file.write(data)
-        _os.replace(path_tmp, path)
-    except OSError:
-        try:
-            _os.unlink(path_tmp)
-        except OSError:
-            pass
-        raise
+    def __hash__(self):
+        return hash(self.id) if self.id != -1 else hash(self.s)
 
+    def __eq__(self, other):
+        return isinstance(other, EntityClass) and self.s == other.s
 
-_code_type = type(_write_atomic.__code__)
+    def __ne__(self, other):
+        return not isinstance(other, EntityClass) or self.s != other.s
 
+    def __lt__(self, other):
+        if not isinstance(other, EntityClass):
+            raise TypeError("Unorderable types:"
+                            "not both InfinityDB EntityClasses")
+        return self.s < other.s
+
+    def __gt__(self, other):
+        if not isinstance(other, EntityClass):
+            raise TypeError("Unorderable types: "
+                            "not both InfinityDB EntityClasses")
+        return self.s > other.s
+
+    def __le__(self, other):
+        if not isinstance(other, EntityClass):
+            raise TypeError("Unorderable types: "
+                            "not both InfinityDB EntityClasses")
+        return self.s <= other.s
+
+    def __ge__(self, other):
+        if not isinstance(other, EntityClass):
+            raise TypeError("Unorderable types: "
+                            "not both InfinityDB EntityClasses")
+        return self.s >= other.s
+
+
+class Attribute:
+    """ Attribute corresponds to the InfinityDB 
+    Attribute component type.
+    
+    When a JSON-encoded access to the InfinityDB 
+    server occurs, any Attribute components in the Items 
+    transferred use Attribute instances as the keys
+    in corresponding dict.
+    
+    An Attribute is identified solely by its string 
+    value, or if that is not given, then it is 
+    identified by its integer id.
+    """
 
-# Finder/loader utility code ###############################################
+    def __init__(self, value):
+        if isinstance(value, str):
+            self.s = value
+            self.id = -1
+            if not is_legal_attribute_name(value):
+                raise ValueError(
+                    "InfinityDB Attribute name must "
+                    "match [a-z][A-Za-z0-9._-]*: " + value)
+        elif isinstance(value, int):
+            self.s = 'Attribute(' + str(value) + ')'
+            self.id = int(value)
+        else:
+            raise ValueError(
+                    "An InfinityDB Attribute requires "
+                    "a string or int id")
 
-# Magic word to reject .pyc files generated by other Python versions.
-# It should change for each incompatible change to the bytecode.
-#
-# The value of CR and LF is incorporated so if you ever read or write
-# a .pyc file in text mode the magic number will be wrong; also, the
-# Apple MPW compiler swaps their values, botching string constants.
-#
-# There were a variety of old schemes for setting the magic number.
-# The current working scheme is to increment the previous value by
-# 10.
-#
-# Starting with the adoption of PEP 3147 in Python 3.2, every bump in magic
-# number also includes a new "magic tag", i.e. a human readable string used
-# to represent the magic number in __pycache__ directories.  When you change
-# the magic number, you must also set a new unique magic tag.  Generally this
-# can be named after the Python major version of the magic number bump, but
-# it can really be anything, as long as it's different than anything else
-# that's come before.  The tags are included in the following table, starting
-# with Python 3.2a0.
-#
-# Known values:
-#  Python 1.5:   20121
-#  Python 1.5.1: 20121
-#     Python 1.5.2: 20121
-#     Python 1.6:   50428
-#     Python 2.0:   50823
-#     Python 2.0.1: 50823
-#     Python 2.1:   60202
-#     Python 2.1.1: 60202
-#     Python 2.1.2: 60202
-#     Python 2.2:   60717
-#     Python 2.3a0: 62011
-#     Python 2.3a0: 62021
-#     Python 2.3a0: 62011 (!)
-#     Python 2.4a0: 62041
-#     Python 2.4a3: 62051
-#     Python 2.4b1: 62061
-#     Python 2.5a0: 62071
-#     Python 2.5a0: 62081 (ast-branch)
-#     Python 2.5a0: 62091 (with)
-#     Python 2.5a0: 62092 (changed WITH_CLEANUP opcode)
-#     Python 2.5b3: 62101 (fix wrong code: for x, in ...)
-#     Python 2.5b3: 62111 (fix wrong code: x += yield)
-#     Python 2.5c1: 62121 (fix wrong lnotab with for loops and
-#                          storing constants that should have been removed)
-#     Python 2.5c2: 62131 (fix wrong code: for x, in ... in listcomp/genexp)
-#     Python 2.6a0: 62151 (peephole optimizations and STORE_MAP opcode)
-#     Python 2.6a1: 62161 (WITH_CLEANUP optimization)
-#     Python 2.7a0: 62171 (optimize list comprehensions/change LIST_APPEND)
-#     Python 2.7a0: 62181 (optimize conditional branches:
-#                          introduce POP_JUMP_IF_FALSE and POP_JUMP_IF_TRUE)
-#     Python 2.7a0  62191 (introduce SETUP_WITH)
-#     Python 2.7a0  62201 (introduce BUILD_SET)
-#     Python 2.7a0  62211 (introduce MAP_ADD and SET_ADD)
-#     Python 3000:   3000
-#                    3010 (removed UNARY_CONVERT)
-#                    3020 (added BUILD_SET)
-#                    3030 (added keyword-only parameters)
-#                    3040 (added signature annotations)
-#                    3050 (print becomes a function)
-#                    3060 (PEP 3115 metaclass syntax)
-#                    3061 (string literals become unicode)
-#                    3071 (PEP 3109 raise changes)
-#                    3081 (PEP 3137 make __file__ and __name__ unicode)
-#                    3091 (kill str8 interning)
-#                    3101 (merge from 2.6a0, see 62151)
-#                    3103 (__file__ points to source file)
-#     Python 3.0a4: 3111 (WITH_CLEANUP optimization).
-#     Python 3.0a5: 3131 (lexical exception stacking, including POP_EXCEPT)
-#     Python 3.1a0: 3141 (optimize list, set and dict comprehensions:
-#             change LIST_APPEND and SET_ADD, add MAP_ADD)
-#     Python 3.1a0: 3151 (optimize conditional branches:
-#             introduce POP_JUMP_IF_FALSE and POP_JUMP_IF_TRUE)
-#     Python 3.2a0: 3160 (add SETUP_WITH)
-#                   tag: cpython-32
-#     Python 3.2a1: 3170 (add DUP_TOP_TWO, remove DUP_TOPX and ROT_FOUR)
-#                   tag: cpython-32
-#     Python 3.2a2  3180 (add DELETE_DEREF)
-#     Python 3.3a0  3190 __class__ super closure changed
-#     Python 3.3a0  3200 (__qualname__ added)
-#                      3210 (added size modulo 2**32 to the pyc header)
-#     Python 3.3a1  3220 (changed PEP 380 implementation)
-#     Python 3.3a4  3230 (revert changes to implicit __class__ closure)
-#     Python 3.4a1  3250 (evaluate positional default arguments before
-#                        keyword-only defaults)
-#     Python 3.4a1  3260 (add LOAD_CLASSDEREF; allow locals of class to override
-#                        free vars)
-#     Python 3.4a1  3270 (various tweaks to the __class__ closure)
-#     Python 3.4a1  3280 (remove implicit class argument)
-#     Python 3.4a4  3290 (changes to __qualname__ computation)
-#     Python 3.4a4  3300 (more changes to __qualname__ computation)
-#     Python 3.4rc2 3310 (alter __qualname__ computation)
-#     Python 3.5a0  3320 (matrix multiplication operator)
-#     Python 3.5b1  3330 (PEP 448: Additional Unpacking Generalizations)
-#     Python 3.5b2  3340 (fix dictionary display evaluation order #11205)
-#     Python 3.5b2  3350 (add GET_YIELD_FROM_ITER opcode #24400)
-#     Python 3.5.2  3351 (fix BUILD_MAP_UNPACK_WITH_CALL opcode #27286)
-#     Python 3.6a0  3360 (add FORMAT_VALUE opcode #25483
-#     Python 3.6a0  3361 (lineno delta of code.co_lnotab becomes signed)
-#     Python 3.6a1  3370 (16 bit wordcode)
-#     Python 3.6a1  3371 (add BUILD_CONST_KEY_MAP opcode #27140)
-#     Python 3.6a1  3372 (MAKE_FUNCTION simplification, remove MAKE_CLOSURE
-#                         #27095)
-#     Python 3.6b1  3373 (add BUILD_STRING opcode #27078)
-#     Python 3.6b1  3375 (add SETUP_ANNOTATIONS and STORE_ANNOTATION opcodes
-#                         #27985)
-#     Python 3.6b1  3376 (simplify CALL_FUNCTIONs & BUILD_MAP_UNPACK_WITH_CALL)
-#     Python 3.6b1  3377 (set __class__ cell from type.__new__ #23722)
-#     Python 3.6b2  3378 (add BUILD_TUPLE_UNPACK_WITH_CALL #28257)
-#     Python 3.6rc1 3379 (more thorough __class__ validation #23722)
-#
-# MAGIC must change whenever the bytecode emitted by the compiler may no
-# longer be understood by older implementations of the eval loop (usually
-# due to the addition of new opcodes).
-#
-# Whenever MAGIC_NUMBER is changed, the ranges in the magic_values array
-# in PC/launcher.c must also be updated.
+    def __str__(self):
+        return self.s
 
-MAGIC_NUMBER = (3379).to_bytes(2, 'little') + b'\r\n'
-_RAW_MAGIC_NUMBER = int.from_bytes(MAGIC_NUMBER, 'little')  # For import.c
+    def __repr__(self):
+        return self.s
 
-_PYCACHE = '__pycache__'
-_OPT = 'opt-'
+    def __hash__(self):
+        return hash(self.id) if self.id != -1 else hash(self.s)
+
+    def __eq__(self, other):
+        return isinstance(other, Attribute) and self.s == other.s
 
-SOURCE_SUFFIXES = ['.py']  # _setup() adds .pyw as needed.
+    def __ne__(self, other):
+        return not isinstance(other, Attribute) or self.s != other.s
 
-BYTECODE_SUFFIXES = ['.pyc']
-# Deprecated.
-DEBUG_BYTECODE_SUFFIXES = OPTIMIZED_BYTECODE_SUFFIXES = BYTECODE_SUFFIXES
+    def __lt__(self, other):
+        if not isinstance(other, Attribute):
+            raise TypeError("Unorderable types: not "
+            "both InfinityDB Attributes")
+        return self.s < other.s
+
+    def __gt__(self, other):
+        if not isinstance(other, Attribute):
+            raise TypeError("Unorderable types: "
+            "not both InfinityDB Attributes")
+        return self.s > other.s
+
+    def __le__(self, other):
+        if not isinstance(other, Attribute):
+            raise TypeError("Unorderable types: "
+            "not both InfinityDB Attributes")
+        return self.s <= other.s
+
+    def __ge__(self, other):
+        if not isinstance(other, Attribute):
+            raise TypeError(
+                "Unorderable types: not "
+                "both InfinityDB Attributes")
+        return self.s >= other.s
+
+
+class Index:
+    """ Index corresponds to the InfinityDB Index component type.
+    
+    Transferring data as JSON to and from the InfinityDB REST
+    access encodes the lists as JSON lists. However, internally
+    InfinityDB stores lists as Items having Index components.
+    
+    It is possible to flatten a list to a pure dict in which the
+    keys are Indexes. This allows dicts and lists to be
+    flattened to dict trees in which the keys are tuples that
+    represent paths, and which can contain Indexes in the tuples.
+    Such a representation is more convenient in some situations,
+    and it corresponds more directly to the encoding of data
+    in InfinityDB as sets of Items.
+    
+    An Index is identified solely buy its index integer attribute.
+    The dicts containing Index component keys will automatically be
+    encoded as Python lists, however, transparently.
+    """
 
-def cache_from_source(path, debug_override=None, *, optimization=None):
-    """Given the path to a .py file, return the path to its .pyc file.
+    def __init__(self, index):
+        if isinstance(index, int):
+            self.index = index
+        else:
+            raise ValueError("An InfinityDB Index "
+                             "component requires an int")
 
-    The .py file does not need to exist; this simply returns the path to the
-    .pyc file calculated as if the .py file were imported.
+    def __str__(self):
+        return '[' + str(self.index) + ']'
 
-    The 'optimization' parameter controls the presumed optimization level of
-    the bytecode file. If 'optimization' is not None, the string representation
-    of the argument is taken and verified to be alphanumeric (else ValueError
-    is raised).
+    def __repr__(self):
+        return '[' + str(self.index) + ']'
 
-    The debug_override parameter is deprecated. If debug_override is not None,
-    a True value is the same as setting 'optimization' to the empty string
-    while a False value is equivalent to setting 'optimization' to '1'.
+    def __hash__(self):
+        return hash(self.index)
 
-    If sys.implementation.cache_tag is None then NotImplementedError is raised.
+    def __eq__(self, other):
+        return isinstance(other, Index) and self.index == other.index
 
+    def __ne__(self, other):
+        return (not isinstance(other, Index) or
+                self.index != other.index)
+
+    def __lt__(self, other):
+        if not isinstance(other, Index):
+            raise TypeError("Unorderable types: not "
+                "both InfinityDB Indexes")
+        return self.index < other.index
+
+    def __gt__(self, other):
+        if not isinstance(other, Index):
+            raise TypeError("Unorderable types: not "
+                "both InfinityDB Indexes")
+        return self.index > other.index
+
+    def __le__(self, other):
+        if not isinstance(other, Index):
+            raise TypeError("Unorderable types: not "
+            "both InfinityDB Indexes")
+        return self.index <= other.index
+
+    def __ge__(self, other):
+        if not isinstance(other, Index):
+            raise TypeError("Unorderable types: not "
+            "both InfinityDB Indexes")
+        return self.index > other.index
+
+    def get_index(self):
+        return self.index
+
+
+def escape_uri_components(*k):
+    """ This is for accessing the InfinityDB via a URL 
+    that ends with a path down into the database, which 
+    can be considered to be a key prefix to traverse 
+    the logical JSON.
+     
+    The escaped path has '/' separators but the components 
+    do not. For example, to access the 10'th element of the
+    outer array, and the "temp" key of the object at that 
+    position, do escape_uri_components([10],'temp'). The 
+    keys do not have to be strings, because we store 
+    'extended' json. Keys can be dates as well.
     """
-    if debug_override is not None:
-        _warnings.warn('the debug_override parameter is deprecated; use '
-                       "'optimization' instead", DeprecationWarning)
-        if optimization is not None:
-            message = 'debug_override or optimization must be set to None'
-            raise TypeError(message)
-        optimization = '' if debug_override else 1
-    path = _os.fspath(path)
-    head, tail = _path_split(path)
-    base, sep, rest = tail.rpartition('.')
-    tag = sys.implementation.cache_tag
-    if tag is None:
-        raise NotImplementedError('sys.implementation.cache_tag is None')
-    almost_filename = ''.join([(base if base else rest), sep, tag])
-    if optimization is None:
-        if sys.flags.optimize == 0:
-            optimization = ''
-        else:
-            optimization = sys.flags.optimize
-    optimization = str(optimization)
-    if optimization != '':
-        if not optimization.isalnum():
-            raise ValueError('{!r} is not alphanumeric'.format(optimization))
-        almost_filename = '{}.{}{}'.format(almost_filename, _OPT, optimization)
-    return _path_join(head, _PYCACHE, almost_filename + BYTECODE_SUFFIXES[0])
-
-
-def source_from_cache(path):
-    """Given the path to a .pyc. file, return the path to its .py file.
-
-    The .pyc file does not need to exist; this simply returns the path to
-    the .py file calculated to correspond to the .pyc file.  If path does
-    not conform to PEP 3147/488 format, ValueError will be raised. If
-    sys.implementation.cache_tag is None then NotImplementedError is raised.
 
+    k_flattened = flatten_to_list(k)
+    p = []
+    for s in k_flattened:
+        if s == None:
+            p.append('null')
+        elif s is True:
+            p.append('true')
+        elif s is False:
+            p.append('false')
+        elif isinstance(s, str):
+            p.append(json_quote_string(s))
+        elif isinstance(s, datetime.datetime):
+            p.append(s.isoformat())
+        elif isinstance(s, list):
+            # A one-element list is just used to represent
+            # an index into a JSON array
+            if len(s) != 1 or not isinstance(s[0], int):
+                raise TypeError(
+                    "an array index must be a single int")
+            p.append('[' + str(s[0]) + ']')
+        elif isinstance(s, (float, int)):
+            p.append(str(s))
+        elif isinstance(s, (EntityClass, Attribute)):
+            p.append(str(s))
+        elif isinstance(s, Index):
+            p.append('[' + s.get_index() + ']')
+        else: raise TypeError("a primitive, index, "
+            "or date is expected")
+    return '/'.join([urllib.request.quote(s, safe='') for s in p])
+
+# Assume  dict has only one key! They are not in a particular order
+def flatten_to_list(x):
+    flattened = []
+    if isinstance(x, dict):
+        for e in x:
+            flattened += flatten_to_list(e) + flatten_to_list(x[e]) 
+            break
+    elif isinstance(x, (tuple,list)):
+        for e in x:
+            flattened += flatten_to_list(e)
+    elif x is not None:
+        flattened += [x]
+    return flattened
+    
+# Convert {x:None} to (x,), or {(x,y):None} to (x,y) or [x,y] to (x,y)
+# or {(x,y):(m,n)} to (x,y,m,n) or {(x,(y,),z):{m:None}} to (x,y,z,m)
+# recursively.
+# Assume  dict has only one key! They are not in a particular order
+def flatten_to_tuple(x):
+    flattened = ()
+    if isinstance(x, dict):
+        for e in x:
+            flattened += flatten_to_tuple(e) + flatten_to_tuple(x[e]) 
+            break
+    elif isinstance(x, (tuple,list)):
+        for e in x:
+            flattened += flatten_to_tuple(e)
+    elif x is not None:
+        flattened += (x,)
+    return flattened
+
+def to_json_extended(o, depth=0, *, is_indented=True):
+    """ Return a string encoded in the infinitydb 
+    extended JSON format for a structure o, including 
+    dates and non-string keys. Tuples become lists.
     """
-    if sys.implementation.cache_tag is None:
-        raise NotImplementedError('sys.implementation.cache_tag is None')
-    path = _os.fspath(path)
-    head, pycache_filename = _path_split(path)
-    head, pycache = _path_split(head)
-    if pycache != _PYCACHE:
-        raise ValueError('{} not bottom-level directory in '
-                         '{!r}'.format(_PYCACHE, path))
-    dot_count = pycache_filename.count('.')
-    if dot_count not in {2, 3}:
-        raise ValueError('expected only 2 or 3 dots in '
-                         '{!r}'.format(pycache_filename))
-    elif dot_count == 3:
-        optimization = pycache_filename.rsplit('.', 2)[-2]
-        if not optimization.startswith(_OPT):
-            raise ValueError("optimization portion of filename does not start "
-                             "with {!r}".format(_OPT))
-        opt_level = optimization[len(_OPT):]
-        if not opt_level.isalnum():
-            raise ValueError("optimization level {!r} is not an alphanumeric "
-                             "value".format(optimization))
-    base_filename = pycache_filename.partition('.')[0]
-    return _path_join(head, base_filename + SOURCE_SUFFIXES[0])
+    is_first = True
+    s = ''
+    ind = '    ' * depth
+    if o == None:
+        return 'null'
+    elif o is True:
+        return 'true'
+    elif o is False:
+        return 'false'
+    elif isinstance(o, dict):
+        s = '{'
+        for k in o:
+            if not is_first:
+                s += ','
+            if is_indented:
+                s += '\r\n   ' + ind
+            s += to_json_extended(k, depth + 1, is_indented=is_indented) + ':'
+            if is_indented:
+                s += ' '
+            s += to_json_extended(o[k], depth + 1, is_indented=is_indented)
+            is_first = False
+        if not is_first and is_indented:
+            s += '\r\n' + ind
+        s += '}'
+    elif isinstance(o, (list, tuple)):
+        s = '['
+        for v in o:
+            if not is_first: 
+                s += ','
+            if is_indented:
+                s += '\r\n   ' + ind
+            s += to_json_extended(v, depth + 1, is_indented=is_indented)
+            is_first = False
+        if not is_first and is_indented: 
+            s += '\r\n' + ind
+        s += ']'
+    elif isinstance(o, str):
+        s = json_quote_string(o)
+    elif isinstance(o, datetime.datetime):
+        s = o.isoformat()
+    else:
+        s = str(o)
+    return s
 
 
-def _get_sourcefile(bytecode_path):
-    """Convert a bytecode file path to a source path (if possible).
+# experimental
+def json_quote_string(s):
+    if isinstance(s, bytes):
+        s = s.decode('utf-8')
+    quoted = '"'
+    # duplicate any backslashes
+    for c in s:
+        quoted += '\\\\' if c == '\\' else '\"' if c == '"' else c
+    return quoted + '"'
+
+
+# start is offset in s. Return parsed_string, True if found, offset after string
+# Using json.loads(s) has no start, after_string, or found boolean result.
+# experimental
+def json_parse_string(s, *, start=0):
+    if len(s) <= start or  s[start] != '"':
+        return '', False, start
+    content = ''
+    i = start + 1
+    while i < len(s):
+        c = s[i]
+        if c == '"':
+            return content, True, i + 1
+        elif c == '\\':
+            i += 1
+            if i >= len(s):
+                raise TypeError("end of string after backslash in: '" + s + "'")
+            content += s[i]
+        else:
+            content += c
+        i += 1
+    raise TypeError("ending quote not found in: '" + s + "'")
+
+
+# Only for differentiating ints and floats
+# Regexes may have ReDOS characteristics for some input data,
+# which cannot easily be proved, so it should be done differently.
+_float_regex = re.compile('[+-]?[0-9]+[.]')
+# only for differentiating numbers and dates
+_date_regex = re.compile('[0-9]+[-]')
+_entity_class_attribute_regex = re.compile('[a-zA-Z][a-zA-Z0-9_.-]*')
+
+
+def underscore_quote(o):
+    """ Pre-process a general structure o by changing its 
+    keys and dates to strings using prefixed underscores 
+    as a quote.
+    
+    The result is suitable for JSON encoding.
+    TODO: byte[], char[], ByteString
+    """
+    if isinstance(o, dict):
+        return {underscore_quote_key(k) : underscore_quote(v)
+                for k, v in o.items()}
+    elif isinstance(o, list):
+        return [underscore_quote(v) for v in o]
+    elif isinstance(o, tuple):
+        return tuple(underscore_quote(v) for v in o)
+    elif isinstance(o, bytes):
+        o = o.decode('utf-8')
+        return o if o[0] != '_' else '_' + o
+    elif isinstance(o, str):
+            # stuff an extra underscore
+            return o if o == '' or o[0] != '_' else '_' + o
+    elif isinstance(o, datetime.datetime):
+        return '_' + o.isoformat()
+    elif isinstance(o, EntityClass) or isinstance(o, Attribute):
+        return '_' + str(o)
+    else: return o
+
+
+def underscore_quote_key(k):
+    """ Make any primitive or date into an 'underscore-quoted' 
+     string for use as a JSON key when serializing into JSON"""
+    if k == None:
+        return '_null'
+    elif isinstance(k, bool):
+        return '_true' if k else '_false'
+    elif isinstance(k, int) or isinstance(k, float):
+        return '_' + str(k)
+    elif isinstance(k, bytes):
+        k = k.decode('utf-8')
+        # stuff an extra underscore if necessary
+        return k if k[:1] != '_' else '_' + k
+    elif isinstance(k, str):
+        # stuff an extra underscore if necessary
+        return k if k[:1] != '_' else '_' + k
+    elif isinstance(k, datetime.datetime):
+        return '_' + k.isoformat()
+    elif isinstance(k, EntityClass) or isinstance(k, Attribute):
+        return '_' + str(k)
+    else:
+        raise TypeError('keys must be primitive or date')
 
-    This function exists purely for backwards-compatibility for
-    PyImport_ExecCodeModuleWithFilenames() in the C API.
 
+def underscore_unquote(o):
+    """ Take a limited structure that was read in as
+    JSON and convert to a more general Python structure 
+    having non-string keys as well as key or value dates.
+    
+    The non-string keys and dates are encoded as strings 
+    with an initial '_', while strings originally starting 
+    with '_' have another '_' stuffed at the front. Keys 
+    must be primitives, however. e.g.: 
+    o = underscore_unquote(json.loads(s))
     """
-    if len(bytecode_path) == 0:
+    # TODO bug: index primitives break in parse_primitive(),
+    # but should turn into lists.
+    if isinstance(o, dict):
+        return {underscore_unquote(k) :
+                 underscore_unquote(v) for k, v in o.items()}
+    elif isinstance(o, list):
+        return [underscore_unquote(v) for v in o]
+    elif isinstance(o, tuple):
+        return tuple(underscore_unquote(v) for v in o)
+    elif isinstance(o, str):
+        if len(o) == 0:
+            return o
+        elif o[0:2] == '__':
+            # Undo the 'underscore stuffing' for
+            # strings containing an initial '_'
+            return o[1:]
+        elif o[0] == '_':
+            # an underscore-quoted primitive
+            return parse_primitive(o[1:])
+        else: return o
+    else: return o
+
+
+# TODO: byte string, byte array, char array
+def parse_primitive(s):
+    if len(s) == 0:
+        raise TypeError("InfinityDB primitive "
+                        "value expected, but is empty")
+    elif s == 'true':
+        return True
+    elif s == 'false':
+        return False
+    elif s == 'null':
         return None
-    rest, _, extension = bytecode_path.rpartition('.')
-    if not rest or extension.lower()[-3:-1] != 'py':
-        return bytecode_path
-    try:
-        source_path = source_from_cache(bytecode_path)
-    except (NotImplementedError, ValueError):
-        source_path = bytecode_path[:-1]
-    return source_path if _path_isfile(source_path) else bytecode_path
-
-
-def _get_cached(filename):
-    if filename.endswith(tuple(SOURCE_SUFFIXES)):
+    elif s[0].isdigit() or s[0] == '+' or s[0] == '-':
+        if _date_regex.match(s):
+            return dateutil.parser.parse(s)
+#        elif match(_float_regex, s):
+        elif '.' in s:
+            # BUG
+            # we lose the distinction between float and double
+            # provided by InfinityDB
+            return float(s if s[-1:] != 'f' else s[:-1])
+        else: return int(s)
+    elif s[0] == '[':
+        if s.find(']') != len(s) - 1:
+            raise TypeError(
+                "InfinityDB primitive index component "
+                "does not end with ']': " + s)
         try:
-            return cache_from_source(filename)
-        except NotImplementedError:
-            pass
-    elif filename.endswith(tuple(BYTECODE_SUFFIXES)):
-        return filename
-    else:
-        return None
-
-
-def _calc_mode(path):
-    """Calculate the mode permissions for a bytecode file."""
-    try:
-        mode = _path_stat(path).st_mode
-    except OSError:
-        mode = 0o666
-    # We always ensure write access so we can update cached files
-    # later even when the source files are read-only on Windows (#6074)
-    mode |= 0o200
-    return mode
-
-
-def _check_name(method):
-    """Decorator to verify that the module being requested matches the one the
-    loader can handle.
+            index = int(s[1:-1])
+        except TypeError:
+            raise TypeError("InfinityDB primitive index "
+                "component must contain an int: '" + s + "'")
+        return Index(index)
+    elif _entity_class_attribute_regex.match(s):
+        c = s[0]
+        if 'A' <= c <= 'Z':
+            return EntityClass(s)
+        elif 'a' <= c <= 'z':
+            return Attribute(s)
+    elif s[0] == '"':
+        parsed_string, found, offset_after_string = json_parse_string(s);
+        if found:
+            if offset_after_string != len(s):
+                raise TypeError("InfinityDB string "
+                                "does not end at component end: '" + s + "'")
+            return parsed_string
+    raise TypeError('InfinityDB primitive value expected: ' + s)
+
+
+# Note \r and \n are considered white space between tokens
+def parse_token_string_into_components(s):
+    """ Convert a string into a list of components as tokens """
+    components = []
+    component = ''
+    i = 0;
+#    while i < len(s) and s[i] not in '\r\n\t\v\f':
+    while True:
+        # handle embedded white
+        parsed_string, found, offset_after_string = json_parse_string(s, start=i)
+        if  found:
+            i = offset_after_string
+            component = parsed_string
+        else:
+            # Skip non-white. Only strings contain white.
+            j = i
+            while j < len(s) and s[j] not in ' \r\n\t\v\f':
+                j += 1
+            component = parse_primitive(s[i:j])
+            i = j
+        components.append(component)
+        # skip white between components
+        while i < len(s) and s[i] in ' \r\n\t\v\f':
+            i += 1
+        if i == len(s):
+            break
+    return components
 
-    The first argument (self) must define _name which the second argument is
-    compared against. If the comparison fails then ImportError is raised.
 
+def json_quote_primitives(o):
+    """ Pre-process recursively a structure of dicts, lists and tuples 
+    by changing dates to quoted ISO strings, strings to JSON quoted 
+    strings, everything else to a quoted string. However None, 
+    numbers and booleans are left alone except as keys as they 
+    are left alone by json.dumps().
+    
+    The result is suitable for JSON encoding by json.dumps().
     """
-    def _check_name_wrapper(self, name=None, *args, **kwargs):
-        if name is None:
-            name = self.name
-        elif self.name != name:
-            raise ImportError('loader for %s cannot handle %s' %
-                                (self.name, name), name=name)
-        return method(self, name, *args, **kwargs)
-    try:
-        _wrap = _bootstrap._wrap
-    except NameError:
-        # XXX yuck
-        def _wrap(new, old):
-            for replace in ['__module__', '__name__', '__qualname__', '__doc__']:
-                if hasattr(old, replace):
-                    setattr(new, replace, getattr(old, replace))
-            new.__dict__.update(old.__dict__)
-    _wrap(_check_name_wrapper, method)
-    return _check_name_wrapper
-
-
-def _find_module_shim(self, fullname):
-    """Try to find a loader for the specified module by delegating to
-    self.find_loader().
+    if o == None or isinstance(o, float) or isinstance(o, int) or isinstance(o, bool):
+        return o
+    elif isinstance(o, dict):
+        return {json_quote_primitive(k) : json_quote_primitives(v)
+                for k, v in o.items()}
+    elif isinstance(o, list):
+        return [json_quote_primitives(v) for v in o]
+    elif isinstance(o, tuple):
+        return tuple(json_quote_primitives(v) for v in o)
+    else:
+        return json_quote_primitive(o)
 
-    This method is deprecated in favor of finder.find_spec().
 
+def json_quote_primitive(o):
+    """ TODO InfinityDB CharArray, ByteArray, and ByteString 
+    component types, which need
+    their own classes like EntityClass and Attribute.
+    However, we use those only in the db itself, because
+    we access them as blobs except ByteString, which is not 
+    used much.
     """
-    # Call find_loader(). If it returns a string (indicating this
-    # is a namespace package portion), generate a warning and
-    # return None.
-    loader, portions = self.find_loader(fullname)
-    if loader is None and len(portions):
-        msg = 'Not importing directory {}: missing __init__'
-        _warnings.warn(msg.format(portions[0]), ImportWarning)
-    return loader
-
-
-def _validate_bytecode_header(data, source_stats=None, name=None, path=None):
-    """Validate the header of the passed-in bytecode against source_stats (if
-    given) and returning the bytecode that can be compiled by compile().
-
-    All other arguments are used to enhance error reporting.
-
-    ImportError is raised when the magic number is incorrect or the bytecode is
-    found to be stale. EOFError is raised when the data is found to be
-    truncated.
-
+    if isinstance(o, bytes):
+        o = o.decode('utf-8')
+    if isinstance(o, str):
+        # doubly-quoted
+        return '"' + json_quote_string(o) + '"'
+    elif isinstance(o, datetime.datetime):
+        return '"' + o.isoformat() + '"'
+    return '"' + str(o) + '"'
+
+
+def flatten_to_tuples(o, *, flattened_lists, compact_tips):
+    """Convert a nested dict tree into one with tuple keys 
+    that represent paths within the original tree. 
+     
+    This is very  convenient for working with trees that 
+    represent sets of Items to  be logically interchanged with 
+    InfinityDB, as the models are similar. The tuple keys may 
+    have zero or more elements, with mixed lengths. A tuple that
+    is a prefix of another cannot, however, be represented
+    in the normal non-tuple tree form of nested dicts and will 
+    disappear after converted back.
+    
+    Any EntityClass or Attribute keys found delimit the tuples, 
+    so they never occur within the tuple elements. The resulting 
+    tree is then an alternation depth-wise between keys that are 
+    simple EntityClass and Attribute instances, and tuple keys 
+    between them. This allows a high degree of forwards and 
+    backwards compatibility, as the tuples can be various 
+    lengths and can be extended in future databases without 
+    causing incompatibilities with old code. InfinityDB can deal 
+    with its Items in the same way.
+    
+    The InfinityDB accessor does no conversion, and the client code
+    must do it, so that there are no tuple keys given to or 
+    returned by the accessor. The accessor works logically 
+    on JSON, i.e. nested Python lists and dicts with non-tuple
+    keys. Also, the accessor assumes the terminals have been 
+    compacted with compact_tree_tips(), because a terminal {} 
+    will cause the Item to disappear.
+    
+    Note that the flattening functions sometimes try to share
+    references to components and subtrees rather than 
+    copying them.
+    
+    Args:
+    flattened_lists: if not, make the resulting tree have lists, or else
+        put Indexes in the tuples to represent them. The Index class
+        is a simple integer key that represents the position of 
+        the child tree within the list. So, for flattened_lists true,
+        {x,[{y:0}]} becomes {(x,Index(0),y,0):None}
+    compact_tips: if a tip can be represented without 
+        nesting, do so. So {k:{}} becomes k, and {(k):None} becomes
+        k. The result is some compact {k:v} terminals where k is 
+        a non-tuple and v is not a dict or list. For multi-key dicts, 
+        {k1:{},k2:{}} becomes {k1:None,k2:None}
+        If None, do nothing to the tips.
+        
+    Returns:
+        flattened  tree
     """
-    exc_details = {}
-    if name is not None:
-        exc_details['name'] = name
+    if flattened_lists:
+        # lists become dicts with keys that are
+        # Indexes having increasing ids
+        rslt = flatten_lists_to_indexes(o)
     else:
-        # To prevent having to make all messages have a conditional name.
-        name = '<bytecode>'
-    if path is not None:
-        exc_details['path'] = path
-    magic = data[:4]
-    raw_timestamp = data[4:8]
-    raw_size = data[8:12]
-    if magic != MAGIC_NUMBER:
-        message = 'bad magic number in {!r}: {!r}'.format(name, magic)
-        _bootstrap._verbose_message('{}', message)
-        raise ImportError(message, **exc_details)
-    elif len(raw_timestamp) != 4:
-        message = 'reached EOF while reading timestamp in {!r}'.format(name)
-        _bootstrap._verbose_message('{}', message)
-        raise EOFError(message)
-    elif len(raw_size) != 4:
-        message = 'reached EOF while reading size of source in {!r}'.format(name)
-        _bootstrap._verbose_message('{}', message)
-        raise EOFError(message)
-    if source_stats is not None:
-        try:
-            source_mtime = int(source_stats['mtime'])
-        except KeyError:
-            pass
-        else:
-            if _r_long(raw_timestamp) != source_mtime:
-                message = 'bytecode is stale for {!r}'.format(name)
-                _bootstrap._verbose_message('{}', message)
-                raise ImportError(message, **exc_details)
-        try:
-            source_size = source_stats['size'] & 0xFFFFFFFF
-        except KeyError:
-            pass
-        else:
-            if _r_long(raw_size) != source_size:
-                raise ImportError('bytecode is stale for {!r}'.format(name),
-                                  **exc_details)
-    return data[12:]
-
-
-def _compile_bytecode(data, name=None, bytecode_path=None, source_path=None):
-    """Compile bytecode as returned by _validate_bytecode_header()."""
-    code = marshal.loads(data)
-    if isinstance(code, _code_type):
-        _bootstrap._verbose_message('code object from {!r}', bytecode_path)
-        if source_path is not None:
-            _imp._fix_co_filename(code, source_path)
-        return code
+        rslt = unflatten_lists_from_indexes(o, strict=False)
+    rslt = flatten_to_tuples_preserving_lists(rslt)
+    if compact_tips == None:
+        return rslt
+    elif compact_tips:
+        return compact_tree_tips(rslt)
     else:
-        raise ImportError('Non-code object in {!r}'.format(bytecode_path),
-                          name=name, path=bytecode_path)
-
-def _code_to_bytecode(code, mtime=0, source_size=0):
-    """Compile a code object into bytecode for writing out to a byte-compiled
-    file."""
-    data = bytearray(MAGIC_NUMBER)
-    data.extend(_w_long(mtime))
-    data.extend(_w_long(source_size))
-    data.extend(marshal.dumps(code))
-    return data
+        return uncompact_tree_tips(rslt)
 
+""" Flatten, preserving lists.
 
-def decode_source(source_bytes):
-    """Decode bytes representing source code and return the string.
+Any Index keys i.e. components already there 
+become part of the tuples.
+"""
 
-    Universal newline support is used in the decoding.
-    """
-    import tokenize  # To avoid bootstrap issues.
-    source_bytes_readline = _io.BytesIO(source_bytes).readline
-    encoding = tokenize.detect_encoding(source_bytes_readline)
-    newline_decoder = _io.IncrementalNewlineDecoder(None, True)
-    return newline_decoder.decode(source_bytes.decode(encoding[0]))
 
+def flatten_to_tuples_preserving_lists(o):
+    if not o:
+        return None
+    if isinstance(o, dict):
+        rslt = {}
+        for k, v in o.items():
+            if k == None:
+                continue
+            nested = flatten_to_tuples_preserving_lists(v)
+            if nested == {}:
+                return {(k,):None}
+            elif isinstance(nested, dict):
+                for k2, v2 in nested.items():
+                    if k2 == None:
+                        continue
+                    if isinstance(k, (EntityClass, Attribute)):
+                        if isinstance(k2, (EntityClass, Attribute)):
+                            rslt[k] = {():{k2:v2}}
+                        else:
+                            if not k in rslt:
+                                rslt[k] = {}
+                            rslt[k][k2] = v2
+                    else:
+                        if isinstance(k2, (EntityClass, Attribute)):
+                            rslt[(k,)] = {k2:v2}
+                        elif isinstance(k2, tuple):
+                            rslt[(k, *k2)] = v2
+                        else:
+                            rslt[(k, k2)] = v2
+            elif isinstance(nested, (EntityClass, Attribute, list)):
+                if isinstance(k, (EntityClass, Attribute)):
+                    rslt[k] = nested
+                else:
+                    rslt[(k,)] = nested
+            elif v == None:
+                rslt[(k)] = None
+            else:
+                rslt[(k, v)] = None
+        return rslt
+    elif isinstance(o, list):
+        return [flatten_to_tuples_preserving_lists(e) for e in o]
+    return {(o,):None}
 
-# Module specifications #######################################################
+""" Convert lists in the dict tree to lists.
 
-_POPULATE = object()
+This prepares for flattening_to_tuples().
+"""
 
 
-def spec_from_file_location(name, location=None, *, loader=None,
-                            submodule_search_locations=_POPULATE):
-    """Return a module spec based on a file location.
+def flatten_lists_to_indexes(o):
+    if isinstance(o, dict):
+        return {k:flatten_lists_to_indexes(v) for k, v in o.items()}
+    elif isinstance(o, list):
+        return {Index(i):flatten_lists_to_indexes(e)
+                for i, e in enumerate(o)}
+    else:
+        return o
 
-    To indicate that the module is a package, set
-    submodule_search_locations to a list of directory paths.  An
-    empty list is sufficient, though its not otherwise useful to the
-    import system.
+""" 
+Undo the effects of flatten_to_tuples() except for 
+the conversion of Index components back into lists.
+Also see unflatten_lists_from_indexes().So for {(x,y):z}
+you get {x :{y: {z: None}}}. Use compact_tree_tips() if
+you want, so that {..{x: {y: None}}} becomes {..{x:y}}.
+A simple {x:y} is unchanged.
+The form {x : {y : {}}} is not used, because it 
+can be interpreted as non-existent even though it
+is more appealing and might sometimes be easier to work with.
+Also, x or [y,z] is unchanged but [(x,y),(z)] becomes
+[{x: {y: None}},{z: None}]. A bare (x,y) becomes {x: {y: Nnne}}
+Generally, the server regards x and {x : None} as the same, 
+both representing a singleton x.
+
+This makes everything convertible into JSON and from JSON
+into Items, for the REST interface to InfinityDB v6 server.
+However, the reverse conversion does not produce the same
+tuple keys, and tuple keys are only created when nested
+inside or outside of metas. The reverse conversion also
+normalizes by combining immediately nested tuple keys 
+into a single tuple key. 
 
-    The loader must take a spec as its only __init__() arg.
+"""
 
-    """
-    if location is None:
-        # The caller may simply want a partially populated location-
-        # oriented spec.  So we set the location to a bogus value and
-        # fill in as much as we can.
-        location = '<unknown>'
-        if hasattr(loader, 'get_filename'):
-            # ExecutionLoader
-            try:
-                location = loader.get_filename(name)
-            except ImportError:
-                pass
+def unflatten_from_tuples(o):
+    result = {}
+    _unflatten_from_tuples_1(o, (), result)
+    return result
+
+    # a placeholder that signals a list is present
+INDEX = Index(0)
+    
+def _unflatten_from_tuples_1(o, item, result):
+    if o == None:
+        _unflatten_from_tuples_insert(result, item)
+    if isinstance(o, tuple):
+        _unflatten_from_tuples_insert(result, item + o)
+    elif isinstance(o, list):
+        # Unnecessary, just for nicer looking JSON. Sending an empty list is the same as nothing
+        # This gets you item + [{}], but {} is 'lack of an Item'. On parsing the
+        # JSON at the server, it is removed and there is no Item for it presented
+        # to the PatternQuery in the  request content.
+    #    if o == []:
+    #        _unflatten_from_tuples_insert(result, item + (INDEX,))
+    #        return
+        for e in o:
+            if isinstance(e, tuple):
+                _unflatten_from_tuples_insert(result, item + (INDEX,) + e)
+            elif isinstance(e, (list, dict)):
+                _unflatten_from_tuples_1(e, item + INDEX, result)
+            else:
+                _unflatten_from_tuples_insert(result, item + (INDEX,) + (e,))
+    elif isinstance(o, dict):
+        for k in o:
+            if isinstance(k, tuple):
+                _unflatten_from_tuples_1(o[k], item + k, result)
+            elif isinstance(k, (list, dict)):
+                # impossible
+                raise TypeError
+            else:
+                _unflatten_from_tuples_1(o[k], item + (k,), result)
     else:
-        location = _os.fspath(location)
-
-    # If the location is on the filesystem, but doesn't actually exist,
-    # we could return None here, indicating that the location is not
-    # valid.  However, we don't have a good way of testing since an
-    # indirect location (e.g. a zip file or URL) will look like a
-    # non-existent file relative to the filesystem.
-
-    spec = _bootstrap.ModuleSpec(name, loader, origin=location)
-    spec._set_fileattr = True
-
-    # Pick a loader if one wasn't provided.
-    if loader is None:
-        for loader_class, suffixes in _get_supported_file_loaders():
-            if location.endswith(tuple(suffixes)):
-                loader = loader_class(name, location)
-                spec.loader = loader
-                break
-        else:
-            return None
+        _unflatten_from_tuples_insert(result, item + (o,))
 
-    # Set submodule_search_paths appropriately.
-    if submodule_search_locations is _POPULATE:
-        # Check the loader.
-        if hasattr(loader, 'is_package'):
-            try:
-                is_package = loader.is_package(name)
-            except ImportError:
-                pass
+# insert the item into the result dict
+def _unflatten_from_tuples_insert(result, item):
+    if result == None or item == ():
+        return
+    if not isinstance(item, tuple):
+        raise TypeError
+    elif isinstance(result, list):
+        if item[0] != INDEX:
+            raise TypeError
+        result.append(unflatten_from_tuples(item[1:]))
+    elif isinstance(result, dict):
+        if not item[0] in result:
+            if item[0] == INDEX:
+                raise TypeError
+            elif len(item) > 1 and item[1] == INDEX:
+                result[item[0]] = []
+            elif len(item) == 1:
+                result[item[0]] = None
             else:
-                if is_package:
-                    spec.submodule_search_locations = []
+                result[item[0]] = {}
+        _unflatten_from_tuples_insert(result[item[0]], item[1:])
     else:
-        spec.submodule_search_locations = submodule_search_locations
-    if spec.submodule_search_locations == []:
-        if location:
-            dirname = _path_split(location)[0]
-            spec.submodule_search_locations.append(dirname)
+        raise TypeError
 
-    return spec
+def remove_empty_tuples(o):
+    if isinstance(o, dict):
+        if () in o:
+            return remove_empty_tuples(o[()])
+    return remove_empty_tuples(o)
+
+
+def compact_tree_tips(o):
+    """ Translate from terminals like {k:{}} to k and from {(k):None} 
+    to k, possibly at the ends of the branches of a tree. This means
+    that {k1:{k2:{}} becomes {k1:k2}.
+    
+    But note that, {(k):{}} becomes (k).
+    We do not combine {(k):{(k2):{}}} to become {(k,k2):None} though.
+    To do that, convert and re-establish the tuples with 
+    unflatten_from_tuples() and then flatten_to_tuples().
+    Also, multi-key dicts like {k:{},k2:{}} are left intact, 
+    but those with tuples like {(k1):None,k2:{}} become {k1:{},k2:{}}
+    """
+    if isinstance(o, dict):
+        if len(o) == 1:
+            for k, v in o.items():
+                if v == {}:
+                    return k
+                elif isinstance(k, tuple) and len(k) == 1:
+                    if v == None:
+                        return k[0]
+                    else:
+                        return {k:compact_tree_tips(v)}
+                elif isinstance(k, (dict, list)):
+                    raise TypeError("impossible dict: "
+                                    "keys are dicts or lists")
+                break
+        return {k:compact_tree_tips(v) for k, v in o.items()}
+    elif isinstance(o, list):
+        return [compact_tree_tips(e) for e in o]
+    else:
+        return o
 
 
-# Loaders #####################################################################
+def uncompact_tree_tips(o):
+    """ Normalize the tree so {k: v} becomes {k:{v: None}}.
+    For every k, there is a value that is a dictionary or None.
+    
+    This undoes compact_tree_tips(). Note {(k1,k2): None} is 
+    not affected. For that, if you want to undo the
+    tupleness of the keys, use unflatten_from_tuples()
+    """
+    if isinstance(o, dict):
+        rslt = {}
+        for k, v in o.items():
+            if isinstance(k, tuple) and v == None:
+                if len(k) == 1:
+                    rslt[k[0]] = None
+                else:
+                    # Can't get rid of a long tuple here.
+                    # Use unflatten().
+                    rslt[k] = None
+            elif (not isinstance(k, (tuple, dict, list))
+                  and v != None and not isinstance(v, (tuple, dict, list))):
+                rslt[k] = {v: None}
+            else:
+                rslt[k] = uncompact_tree_tips(v)
+        return rslt
+    elif isinstance(o, list):
+        return [uncompact_tree_tips(e) for e in o]
+    elif o == None:
+        return None
+    else:
+        return {o: None}
 
-class WindowsRegistryFinder:
 
-    """Meta path finder for modules declared in the Windows registry."""
+def unflatten_lists_from_indexes(o, *, strict=True,
+                             collapse_sparseness=False):
+    """ Change a dict that has Index keys into an actual 
+    list recursively.
+    
+    Keys must not be tuples, so first use an 
+    unflatten_from_tuples() if necessary. A dict that is to be 
+    converted to a list must have only Index keys.
+    
+    An Index component is an instance of the Index class, and 
+    it contains an int that represents the position in a list 
+    when it is a dict key. So, dicts may be used in place of 
+    lists, by using Index keys. InfinityDB has a corresponding 
+    Index component type that can be mixed with any other component 
+    type, such as primitive components, in any Item at any position.
+    
+    InfinityDB can compare components of any of its 12 
+    component types according to a strict inter-type ordering 
+    that puts Index components last. So, InfinityDB never 
+    causes errors in constructing Items or comparing Items, 
+    while Python cannot compare, say strings and numbers.
+    
+    strict: 
+        the conversion raises ValueError if a mixture of Index and 
+        others are present as keys in a given dict. No mixtures will be 
+        present if the tuple keys were created using 
+        flatten_to_tuples() when
+        it works on actual lists, but if there are Index components 
+        already there as as bare keys in a dict, they can end up 
+        mixed with non-Index components. InfinityDB can represent 
+        any mixture.
+    collapse_sparseness: 
+        if a dict contains Index component keys alone, it can 
+        be converted to  a list, but the Index components do 
+        not necessarily ascend monotonically, and if not, we can 
+        remove the logical None's between them. 
+        flatten_to_tuples() always creates monotonic Indexes,
+        but InfinityDB can represent sparse arrays without Nones.
+    """
+    if isinstance(o, list):
+        return [
+            unflatten_lists_from_indexes(e,
+                strict=strict,
+                collapse_sparseness=collapse_sparseness) for e in o]
+    if not isinstance(o, dict) or len(o) == 0:
+        return o
+    # Tf any element is not an index, we can't convert to a
+    # real list, so we have to leave the Index components in there.
+    # InfinityDB can mix Index components with others.
+    contains_index = False
+    contains_non_index = False
+    for k in o:
+        if isinstance(k, Index):
+            contains_index = True
+        else:
+            contains_non_index = True
+        if contains_index and contains_non_index and strict:
+            raise ValueError
+        if contains_non_index:
+            break
+    if contains_index and contains_non_index and strict:
+        raise ValueError
+    if contains_index and not contains_non_index:
+        # all keys are Index components, so we can convert it to a list
+        rslt = []
+        i = 0
+        # The sort never raises a TypeError because there
+        # are no non-Index keys
+        for index in sorted(o):
+            # handle sparseness if present
+            if not collapse_sparseness:
+                while i < index.get_index():
+                    rslt.append(None)
+                    i += 1
+            rslt.append(unflatten_lists_from_indexes(
+                o[index], strict=strict,
+                collapse_sparseness=collapse_sparseness
+                ))
+            i += 1
+        return rslt
+    else:
+        # Actually InfinityDB can represent mixtures of
+        # any type, under any given prefix, so after this,
+        # there may still be some Indexes there as keys.
+        return {
+            k: unflatten_lists_from_indexes(
+                v,
+                strict=strict,
+                collapse_sparseness=collapse_sparseness
+                )
+             for k, v in o.items()
+             }
+
+
+def item_to_tuples(item):
+    """ Change an Item, which is a list of components, into a list
+    of tuples, EnitityClasses, and Attributes, 
+    like [(),MyEC,('some entity',9),my_att,('some value',42)]. 
+    There is always at least one tuple, but it may be empty. Tuples are
+    delimited by the start and end, and by any intervening
+    EntityClasses and Attribute components. Each EntityClass or
+    Attribute comes between tuples, so there are n + 1 tuples,
+    where n is the number of EntityClasses plus Attributes.
+    Because there is almost always an initial EntityCLass,
+    there is almost always an initial empty tuple.
+    """
+    tuple = ()
+    tuples = []
+    for i in range(len(item)):
+        if isinstance(item[i], (EntityClass, Attribute)):
+            tuples.append(tuple)
+            tuple = ()
+            tuples.append(item[i])
+        else:
+            tuple += (item[i],)
+    tuples.append(tuple)
+    return tuples
+
+class InfinityDBError(IOError):
+
+    def __init__(self, *, code, reason=None):
+        super().__init__(code, reason)
+
+
+class InfinityDBAccessor:
+    """ The essential accessor class.
+    
+    infdb=InfinityDBAccessor('https://infinitydb.com:37411',
+    user='testUser', password='db')
+    
+    In order to read the the documentation out of the 
+    read-only demo database go to: https://infinitydb.com:37411/
+    infinitydb/data/demo/readonly/Documentation?action=edit
 
-    REGISTRY_KEY = (
-        'Software\\Python\\PythonCore\\{sys_version}'
-        '\\Modules\\{fullname}')
-    REGISTRY_KEY_DEBUG = (
-        'Software\\Python\\PythonCore\\{sys_version}'
-        '\\Modules\\{fullname}\\Debug')
-    DEBUG_BUILD = False  # Changed in _setup()
+    Or, read the doc by using access.py itself:
+    success, content, content_type = db.get_json('demo/readonly','Documentation')
+    """
 
-    @classmethod
-    def _open_registry(cls, key):
+    def __init__(self, server_url, *, db=None, user=None, password=None,
+                 default_parameters={}):
+        self.server_url = server_url
+        # default if not provided in client call
+        self.db = db
+        self.user = user
+        self.password = password
+        self.context = None
+        self.next_buf = None
+        self.default_parameters = default_parameters.copy()
+        print(ssl.get_default_verify_paths())
+        self.session = Session()
+        self.is_verification_enabled = self.check_verification_required(self.server_url) 
+
+    # Return False for special domains that are not to be verified
+    # Eventually some kind of configurability might be nice.
+    # Disabling verification allows https for encryption, but disables
+    # server authentication, which is fine for AWS EC2 instances and azure
+    # instances. 
+    # The server always has some kind of cert, self-signed or otherwise.
+    # We do not expect it to be possible to spoof
+    # a domain name ending with .amazonaws.com, but to be more specific
+    # like compute.amazonaws.com would possibly miss 
+    # some like compute-X.amazonaws.com. Not sure if this is right for
+    # azure, but google cloud has no default public domain names at all.
+    # Without this disabling, you cannot launch an instance and be able to use
+    # it immediately via its default temporary public ip.
+    def check_verification_required(self, url):
+        hostname = urlparse(url).hostname
+        # leave the initial dot there.
+        return not hostname.endswith('.amazonaws.com') and not hostname.endswith('.azure.com') 
+        
+    def _make_headers(self, content_type=None):
+        headers = {}
+        if self.user is not None:
+            b = '%s:%s' % (self.user, self.password)
+            b = b.encode()
+            b = base64.encodebytes(b)[:-1]
+            b = b.decode()
+            headers['Authorization'] = 'Basic %s' % b
+        if content_type is not None:
+            headers['Content-Type'] = content_type
+        return headers
+
+    def head(self):
+        full_url = self.server_url + '/' + self.db
+        headers = self._make_headers()
+        """ To be used to verify connectivity."""
+#         request = Request('HEAD', self.server_url, headers=headers)
+#         prepped_request = self.session.prepare_request(request)
+#        response = self.session.send(prepped_request)
         try:
-            return _winreg.OpenKey(_winreg.HKEY_CURRENT_USER, key)
-        except OSError:
-            return _winreg.OpenKey(_winreg.HKEY_LOCAL_MACHINE, key)
-
-    @classmethod
-    def _search_registry(cls, fullname):
-        if cls.DEBUG_BUILD:
-            registry_key = cls.REGISTRY_KEY_DEBUG
-        else:
-            registry_key = cls.REGISTRY_KEY
-        key = registry_key.format(fullname=fullname,
-                                  sys_version='%d.%d' % sys.version_info[:2])
-        try:
-            with cls._open_registry(key) as hkey:
-                filepath = _winreg.QueryValue(hkey, '')
-        except OSError:
-            return None
-        return filepath
+            response = self.session.request('HEAD', full_url,
+                                        headers=headers, verify=self.is_verification_enabled)
+        except ConnectionError as ce:
+            raise InfinityDBError(code=400, reason='cannot connect to ' + full_url)
+        if (response.status_code == 204):
+            response.status_code = 200
+        return response.status_code, response.reason
+
+    def create_params(self, **kwargs):
+        params = ''
+        kwargs2 = self.default_parameters.copy()
+        kwargs2.update(kwargs)
+        for kw, value in kwargs2.items():
+            params += '&' if params else '?'
+            if value is None:
+                # this leaves an extra '&'
+                pass
+            elif value is True:
+                params += kw + '=true'
+            elif value is False:
+                params += kw + '=false'
+            elif isinstance(value, str):
+                # TODO XXX must escape & somehow,
+                # we don't want to force all strings to be surrounded with
+                # quotes.
+                params += kw + '=' + value
+            elif isinstance(value, int):
+                params += kw + '=' + str(value)
+            elif isinstance(value, dict):
+                value_unflattened = unflatten_from_tuples(value)
+                value_json = to_json_extended(value_unflattened, is_indented=False)
+                value_uri = urllib.request.quote(value_json, safe='')
+                params += kw + '=' + value_uri
+            else:
+                raise ValueError
+        return params
 
-    @classmethod
-    def find_spec(cls, fullname, path=None, target=None):
-        filepath = cls._search_registry(fullname)
-        if filepath is None:
-            return None
+    def _do_command(self, prefix, *, db, 
+                    action=None,
+                    content_type=None, 
+                    method='GET',
+                    data=None, 
+                    no_content=False, 
+                    always_return_none=False,
+                    **kwargs):
+        prefix = underscore_unquote(prefix)
+        if action:
+            kwargs['action'] = action
+        if self.db is None and db is None:
+            raise ValueError('Missing self.db or db')
+        full_url = (self.server_url + '/' + (db if db else self.db)
+                    + '/' + escape_uri_components(*prefix)
+                    + self.create_params(**kwargs))
+        headers = self._make_headers(content_type=content_type)
+        # requests is in python 3
         try:
-            _path_stat(filepath)
-        except OSError:
-            return None
-        for loader, suffixes in _get_supported_file_loaders():
-            if filepath.endswith(tuple(suffixes)):
-                spec = _bootstrap.spec_from_loader(fullname,
-                                                   loader(fullname, filepath),
-                                                   origin=filepath)
-                return spec
-
-    @classmethod
-    def find_module(cls, fullname, path=None):
-        """Find module named in the registry.
-
-        This method is deprecated.  Use exec_module() instead.
-
-        """
-        spec = cls.find_spec(fullname, path)
-        if spec is not None:
-            return spec.loader
-        else:
+            response = self.session.request(method, full_url,
+                                        headers=headers,
+                                        data=data, verify=self.is_verification_enabled)
+        except ConnectionError as ce:
+            raise InfinityDBError(code=400, reason='cannot connect to ' + full_url)
+        # touching this finishes the operation
+        content = response.content
+        if content == None:
+            raise InfinityDBError(code=400, reason="Null content")
+        if not response.status_code in (200, 204):
+            raise InfinityDBError(code=response.status_code, reason=response.reason + " " + str(prefix))
+        if always_return_none:
             return None
-
-
-class _LoaderBasics:
-
-    """Base class of common code needed by both SourceLoader and
-    SourcelessFileLoader."""
-
-    def is_package(self, fullname):
-        """Concrete implementation of InspectLoader.is_package by checking if
-        the path returned by get_filename has a filename of '__init__.py'."""
-        filename = _path_split(self.get_filename(fullname))[1]
-        filename_base = filename.rsplit('.', 1)[0]
-        tail_name = fullname.rpartition('.')[2]
-        return filename_base == '__init__' and tail_name != '__init__'
-
-    def create_module(self, spec):
-        """Use default semantics for module creation."""
-
-    def exec_module(self, module):
-        """Execute the module."""
-        code = self.get_code(module.__name__)
-        if code is None:
-            raise ImportError('cannot load module {!r} when get_code() '
-                              'returns None'.format(module.__name__))
-        _bootstrap._call_with_frames_removed(exec, code, module.__dict__)
-
-    def load_module(self, fullname):
-        """This module is deprecated."""
-        return _bootstrap._load_module_shim(self, fullname)
-
-
-class SourceLoader(_LoaderBasics):
-
-    def path_mtime(self, path):
-        """Optional method that returns the modification time (an int) for the
-        specified path, where path is a str.
-
-        Raises IOError when the path cannot be handled.
+        if no_content:
+            return response.status_code == 200
+        response_content_type = response.headers['Content-Type']
+        return response.status_code == 200, content, response_content_type
+
+    def get_blob(self, prefix, *, db=None, **kwargs):
+        return self._do_command(prefix, db=db,
+                                action='get-blob', **kwargs)
+
+    def get_json(self, prefix, *, db=None, **kwargs):
+        """ get Items from an infinitydb db as a
+        dict decoded from the json.
         """
-        raise IOError
-
-    def path_stats(self, path):
-        """Optional method returning a metadata dict for the specified path
-        to by the path (str).
-        Possible keys:
-        - 'mtime' (mandatory) is the numeric timestamp of last source
-          code modification;
-        - 'size' (optional) is the size in bytes of the source code.
-
-        Implementing this method allows the loader to read bytecode files.
-        Raises IOError when the path cannot be handled.
+        success, content, response_content_type = self._do_command(prefix, db=db,
+                                         action='as-json', **kwargs)
+        if not success:
+            return False, None, None
+        data_quoted = json.loads(content)
+        content = underscore_unquote(data_quoted)
+        return True, content, response_content_type
+
+    def get_items(self, prefix, db=None, **kwargs):
+        """ get Items from an infinitydb db encoded as components
+        under a given key prefix, up to a limit.
+        Param limit is the max item count.
         """
-        return {'mtime': self.path_mtime(path)}
-
-    def _cache_bytecode(self, source_path, cache_path, data):
-        """Optional method which writes data (bytes) to a file path (a str).
+        return self._do_command(prefix, action='as-items', db=db, **kwargs)
 
-        Implementing this method allows for the writing of bytecode files.
-
-        The source path is needed in order to correctly transfer permissions
+    def get_items_batch(self, prefix, db=None, **kwargs):
+        """ get Items from an infinitydb db encoded as components
+        starting at the key prefix, up to a limit.
+        Param limit is the max item count
         """
-        # For backwards compatibility, we delegate to set_data()
-        return self.set_data(cache_path, data)
-
-    def set_data(self, path, data):
-        """Optional method which writes data (bytes) to a file path (a str).
+        return self._do_command(prefix, action='as-items-batch', db=db, **kwargs)
 
-        Implementing this method allows for the writing of bytecode files.
-        """
-
-
-    def get_source(self, fullname):
-        """Concrete implementation of InspectLoader.get_source."""
-        path = self.get_filename(fullname)
-        try:
-            source_bytes = self.get_data(path)
-        except OSError as exc:
-            raise ImportError('source not available through get_data()',
-                              name=fullname) from exc
-        return decode_source(source_bytes)
-
-    def source_to_code(self, data, path, *, _optimize=-1):
-        """Return the code object compiled from source.
-
-        The 'data' argument can be any object type that compile() supports.
-        """
-        return _bootstrap._call_with_frames_removed(compile, data, path, 'exec',
-                                        dont_inherit=True, optimize=_optimize)
-
-    def get_code(self, fullname):
-        """Concrete implementation of InspectLoader.get_code.
-
-        Reading of bytecode requires path_stats to be implemented. To write
-        bytecode, set_data must also be implemented.
-
-        """
-        source_path = self.get_filename(fullname)
-        source_mtime = None
-        try:
-            bytecode_path = cache_from_source(source_path)
-        except NotImplementedError:
-            bytecode_path = None
+    def put_blob(self, prefix, data, content_type, db=None, **kwargs):
+        return self._do_command(prefix,
+                                db=db,
+                                content_type=content_type,
+                                action='put',
+                                method='put',
+                                data=data, always_return_none=True, **kwargs)
+
+    def put_json(self, prefix, data, *, db=None, **kwargs):
+        # Convert non-string keys and dates to
+        # 'underscored quoted' string form
+        data_quoted = underscore_quote(data)
+        # convert the structure to a byte array
+        json_data = json.dumps(data_quoted).encode()
+        return self._do_command(prefix,
+                                db=db,
+                                content_type='application/json',
+                                method='put',
+                                data=json_data, always_return_none=True, **kwargs)
+
+    def post_json(self, prefix, data, *, db=None, **kwargs):
+        # Convert non-string keys and dates to
+        # 'underscored quoted' string form
+        data_quoted = underscore_quote(data)
+        # convert the structure to a byte array
+        json_data = json.dumps(data_quoted).encode()
+        success, content, response_content_type = self._do_command(prefix,
+                                db=db,
+                                content_type='application/json',
+                                method='post',
+                                data=json_data,
+                                **kwargs)
+        if not success:
+            return False, None, None
+        components = parse_token_string_into_components(content.decode())
+        return True, components, response_content_type
+
+    def delete(self, prefix, *, db=None, **kwargs):
+        return self._do_command(prefix,
+                                db=db,
+                                content_type='application/json',
+                                method='delete',
+                                always_return_none=True,
+                                **kwargs)
+
+    def execute_query(self, prefix, *, 
+                      data=None, 
+                      db=None,
+                      unflatten=True,
+                      flatten=True, 
+                      is_get_blob=False,
+                      is_put_blob=False,
+                      params_url_parameter=None,
+                      compact_tips=False,
+                      content_type='application/json',
+                      **kwargs):
+        # Must compact the tips, or it is interpreted as empty
+        if not is_put_blob:
+            if unflatten:
+                data = unflatten_from_tuples(data)
+            #TODO remove prints
+            print('unflattened input data to execute_query():', data)
+            data_quoted = underscore_quote(data)
+            data = json.dumps(data_quoted).encode()
+        if params_url_parameter:
+            # this goes in the URL's query string as the 'params' parameter
+            kwargs["params"] = params_url_parameter
+        action = 'execute-get-blob-query' if is_get_blob else 'execute-put-blob-query' if is_put_blob else 'execute-query'
+        success, content, response_content_type = self._do_command(prefix,
+                            db=db,
+                            content_type=content_type,
+                            method='get' if is_get_blob else 'post',
+                            data=data,
+                            action=action,
+                             **kwargs)
+        if not success:
+            return False, None, None
+        if content == None:
+            raise InfinityDBError(code=400, reason="Null content")
+        if is_get_blob:
+            return True, content, response_content_type
+        if content == b'':
+            data_quoted = {}
         else:
-            try:
-                st = self.path_stats(source_path)
-            except IOError:
-                pass
-            else:
-                source_mtime = int(st['mtime'])
-                try:
-                    data = self.get_data(bytecode_path)
-                except OSError:
-                    pass
-                else:
-                    try:
-                        bytes_data = _validate_bytecode_header(data,
-                                source_stats=st, name=fullname,
-                                path=bytecode_path)
-                    except (ImportError, EOFError):
-                        pass
-                    else:
-                        _bootstrap._verbose_message('{} matches {}', bytecode_path,
-                                                    source_path)
-                        return _compile_bytecode(bytes_data, name=fullname,
-                                                 bytecode_path=bytecode_path,
-                                                 source_path=source_path)
-        source_bytes = self.get_data(source_path)
-        code_object = self.source_to_code(source_bytes, source_path)
-        _bootstrap._verbose_message('code object from {}', source_path)
-        if (not sys.dont_write_bytecode and bytecode_path is not None and
-                source_mtime is not None):
-            data = _code_to_bytecode(code_object, source_mtime,
-                    len(source_bytes))
-            try:
-                self._cache_bytecode(source_path, bytecode_path, data)
-                _bootstrap._verbose_message('wrote {!r}', bytecode_path)
-            except NotImplementedError:
-                pass
-        return code_object
-
-
-class FileLoader:
-
-    """Base file loader class which implements the loader protocol methods that
-    require file system usage."""
-
-    def __init__(self, fullname, path):
-        """Cache the module name and the path to the file found by the
-        finder."""
-        self.name = fullname
-        self.path = path
-
-    def __eq__(self, other):
-        return (self.__class__ == other.__class__ and
-                self.__dict__ == other.__dict__)
-
-    def __hash__(self):
-        return hash(self.name) ^ hash(self.path)
-
-    @_check_name
-    def load_module(self, fullname):
-        """Load a module from a file.
-
-        This method is deprecated.  Use exec_module() instead.
-
-        """
-        # The only reason for this method is for the name check.
-        # Issue #14857: Avoid the zero-argument form of super so the implementation
-        # of that form can be updated without breaking the frozen module
-        return super(FileLoader, self).load_module(fullname)
-
-    @_check_name
-    def get_filename(self, fullname):
-        """Return the path to the source file as found by the finder."""
-        return self.path
-
-    def get_data(self, path):
-        """Return the data from path as raw bytes."""
-        with _io.FileIO(path, 'r') as file:
-            return file.read()
-
-
-class SourceFileLoader(FileLoader, SourceLoader):
-
-    """Concrete implementation of SourceLoader using the file system."""
-
-    def path_stats(self, path):
-        """Return the metadata for the path."""
-        st = _path_stat(path)
-        return {'mtime': st.st_mtime, 'size': st.st_size}
-
-    def _cache_bytecode(self, source_path, bytecode_path, data):
-        # Adapt between the two APIs
-        mode = _calc_mode(source_path)
-        return self.set_data(bytecode_path, data, _mode=mode)
-
-    def set_data(self, path, data, *, _mode=0o666):
-        """Write bytes data to a file."""
-        parent, filename = _path_split(path)
-        path_parts = []
-        # Figure out what directories are missing.
-        while parent and not _path_isdir(parent):
-            parent, part = _path_split(parent)
-            path_parts.append(part)
-        # Create needed directories.
-        for part in reversed(path_parts):
-            parent = _path_join(parent, part)
-            try:
-                _os.mkdir(parent)
-            except FileExistsError:
-                # Probably another Python process already created the dir.
-                continue
-            except OSError as exc:
-                # Could be a permission error, read-only filesystem: just forget
-                # about writing the data.
-                _bootstrap._verbose_message('could not create {!r}: {!r}',
-                                            parent, exc)
-                return
-        try:
-            _write_atomic(path, data, _mode)
-            _bootstrap._verbose_message('created {!r}', path)
-        except OSError as exc:
-            # Same as above: just don't write the bytecode.
-            _bootstrap._verbose_message('could not create {!r}: {!r}', path,
-                                        exc)
-
-
-class SourcelessFileLoader(FileLoader, _LoaderBasics):
-
-    """Loader which handles sourceless file imports."""
-
-    def get_code(self, fullname):
-        path = self.get_filename(fullname)
-        data = self.get_data(path)
-        bytes_data = _validate_bytecode_header(data, name=fullname, path=path)
-        return _compile_bytecode(bytes_data, name=fullname, bytecode_path=path)
-
-    def get_source(self, fullname):
-        """Return None as there is no source code."""
-        return None
-
-
-# Filled in by _setup().
-EXTENSION_SUFFIXES = []
-
-
-class ExtensionFileLoader(FileLoader, _LoaderBasics):
-
-    """Loader for extension modules.
-
-    The constructor is designed to work with FileFinder.
+            data_quoted = json.loads(content)
+        content = underscore_unquote(data_quoted)
+        if flatten:
+            content = flatten_to_tuples(content, flattened_lists=False, compact_tips=compact_tips)
+        elif compact_tips==True:
+            content = compact_tips(content)
+        elif compact_tips==False:
+            content = uncompact_tree_tips(content)
+        return True, content, response_content_type
+
+    def execute_get_blob_query(self, prefix, **kwargs):
+        return self.execute_query(prefix, 
+                                  is_get_blob=True,
+                                  content_type='application/json', 
+                                  **kwargs)
+
+    def execute_put_blob_query(self, prefix, *,
+                               content_type, 
+                               **kwargs):
+        return self.execute_query(prefix, 
+                                  is_put_blob=True,
+                                  content_type=content_type, 
+                                  **kwargs)
+        
+    def move(self, action, prefix, *, db, **kwargs):
+        success, content, response_content_type = self._do_command(prefix,
+                                db=db,
+                                content_type='application/json',
+                                action=action,
+                                **kwargs)
+        if not success:
+            return False, None, None
+        data = content.decode()
+        components = parse_token_string_into_components(data)
+        return True, components
+
+    def first_item(self, prefix, *, db=None, **kwargs):
+        """ Move to the nearest greater than or equal Item,
+        with the prefix length set to 0. Because the prefix
+        length is 0, the entire database can be iterated. """
+        return self.move('first-item', prefix, db=db, **kwargs)
+
+    def first_component(self, prefix, *, db=None, **kwargs):
+        """ Move to the nearest greater than or equal component, 
+        with the prefix length set to the beginning of the 
+        last component in the key"""
+        return self.move('first-component', prefix, db=db, **kwargs)
+
+    def first_tuple(self, prefix, *, db=None, **kwargs):
+        """ Move to the nearest greater than or equal tuple, 
+        with the prefix length set to the beginning of the 
+        last tuple in the key"""
+        return self.move('first-tuple', prefix, db=db, **kwargs)
 
+    """ For next speed, keep a single buffer in memory that is a list
+    of Items, each being a list.
     """
 
-    def __init__(self, name, path):
-        self.name = name
-        self.path = path
-
-    def __eq__(self, other):
-        return (self.__class__ == other.__class__ and
-                self.__dict__ == other.__dict__)
-
-    def __hash__(self):
-        return hash(self.name) ^ hash(self.path)
-
-    def create_module(self, spec):
-        """Create an unitialized extension module"""
-        module = _bootstrap._call_with_frames_removed(
-            _imp.create_dynamic, spec)
-        _bootstrap._verbose_message('extension module {!r} loaded from {!r}',
-                         spec.name, self.path)
-        return module
-
-    def exec_module(self, module):
-        """Initialize an extension module"""
-        _bootstrap._call_with_frames_removed(_imp.exec_dynamic, module)
-        _bootstrap._verbose_message('extension module {!r} executed from {!r}',
-                         self.name, self.path)
-
-    def is_package(self, fullname):
-        """Return True if the extension module is a package."""
-        file_name = _path_split(self.path)[1]
-        return any(file_name == '__init__' + suffix
-                   for suffix in EXTENSION_SUFFIXES)
-
-    def get_code(self, fullname):
-        """Return None as an extension module cannot create a code object."""
-        return None
-
-    def get_source(self, fullname):
-        """Return None as extension modules have no source code."""
-        return None
-
-    @_check_name
-    def get_filename(self, fullname):
-        """Return the path to the source file as found by the finder."""
-        return self.path
-
-
-class _NamespacePath:
-    """Represents a namespace package's path.  It uses the module name
-    to find its parent module, and from there it looks up the parent's
-    __path__.  When this changes, the module's own path is recomputed,
-    using path_finder.  For top-level modules, the parent module's path
-    is sys.path."""
-
-    def __init__(self, name, path, path_finder):
-        self._name = name
-        self._path = path
-        self._last_parent_path = tuple(self._get_parent_path())
-        self._path_finder = path_finder
-
-    def _find_parent_path_names(self):
-        """Returns a tuple of (parent-module-name, parent-path-attr-name)"""
-        parent, dot, me = self._name.rpartition('.')
-        if dot == '':
-            # This is a top-level module. sys.path contains the parent path.
-            return 'sys', 'path'
-        # Not a top-level module. parent-module.__path__ contains the
-        #  parent path.
-        return parent, '__path__'
-
-    def _get_parent_path(self):
-        parent_module_name, path_attr_name = self._find_parent_path_names()
-        return getattr(sys.modules[parent_module_name], path_attr_name)
-
-    def _recalculate(self):
-        # If the parent's path has changed, recalculate _path
-        parent_path = tuple(self._get_parent_path()) # Make a copy
-        if parent_path != self._last_parent_path:
-            spec = self._path_finder(self._name, parent_path)
-            # Note that no changes are made if a loader is returned, but we
-            #  do remember the new parent path
-            if spec is not None and spec.loader is None:
-                if spec.submodule_search_locations:
-                    self._path = spec.submodule_search_locations
-            self._last_parent_path = parent_path     # Save the copy
-        return self._path
-
-    def __iter__(self):
-        return iter(self._recalculate())
-
-    def __setitem__(self, index, path):
-        self._path[index] = path
-
-    def __len__(self):
-        return len(self._recalculate())
-
-    def __repr__(self):
-        return '_NamespacePath({!r})'.format(self._path)
-
-    def __contains__(self, item):
-        return item in self._recalculate()
-
-    def append(self, item):
-        self._path.append(item)
-
-
-# We use this exclusively in module_from_spec() for backward-compatibility.
-class _NamespaceLoader:
-    def __init__(self, name, path, path_finder):
-        self._path = _NamespacePath(name, path, path_finder)
-
-    @classmethod
-    def module_repr(cls, module):
-        """Return repr for the module.
-
-        The method is deprecated.  The import machinery does the job itself.
-
-        """
-        return '<module {!r} (namespace)>'.format(module.__name__)
-
-    def is_package(self, fullname):
-        return True
-
-    def get_source(self, fullname):
-        return ''
-
-    def get_code(self, fullname):
-        return compile('', '<string>', 'exec', dont_inherit=True)
-
-    def create_module(self, spec):
-        """Use default semantics for module creation."""
-
-    def exec_module(self, module):
-        pass
-
-    def load_module(self, fullname):
-        """Load a namespace module.
-
-        This method is deprecated.  Use exec_module() instead.
-
-        """
-        # The import system never calls this method.
-        _bootstrap._verbose_message('namespace module loaded with path {!r}',
-                                    self._path)
-        return _bootstrap._load_module_shim(self, fullname)
-
-
-# Finders #####################################################################
-
-class PathFinder:
-
-    """Meta path finder for sys.path and package __path__ attributes."""
-
-    @classmethod
-    def invalidate_caches(cls):
-        """Call the invalidate_caches() method on all path entry finders
-        stored in sys.path_importer_caches (where implemented)."""
-        for finder in sys.path_importer_cache.values():
-            if hasattr(finder, 'invalidate_caches'):
-                finder.invalidate_caches()
-
-    @classmethod
-    def _path_hooks(cls, path):
-        """Search sys.path_hooks for a finder for 'path'."""
-        if sys.path_hooks is not None and not sys.path_hooks:
-            _warnings.warn('sys.path_hooks is empty', ImportWarning)
-        for hook in sys.path_hooks:
-            try:
-                return hook(path)
-            except ImportError:
-                continue
+    # get more Items into the next_buf starting at prefix
+    def _fill_next_buf(self, prefix, bound_type, *, db, **kwargs):
+        success, next_item = self.next_bounded(prefix,
+                                            bound_type, db=db, **kwargs)
+        if not success:
+            return False, []
+        success, content, content_type = self.get_items_batch(
+            next_item,
+            limit=self.next_buf.size, db=db, **kwargs)
+        if not success:
+            return False, None
+        lines = content.decode().splitlines()
+        items = [parse_token_string_into_components(line) for line in lines]
+        return True, items
+
+    def _buffered_next(self, prefix, bound, *, db, **kwargs):
+        # lazy construction
+        if not self.next_buf:
+            self.next_buf = NextBuf(self._fill_next_buf)
+        return self.next_buf.next(prefix, bound, db=db, **kwargs)
+
+    def set_next_buffer(self, *, flush=True, size=None):
+        if not self.next_buf:
+            self.next_buf = NextBuf(self._fill_next_buf)
+        if  flush:
+            self.next_buf.flush()
+        if size:
+            self.next_buf.set_size(size)
+
+    def next_bounded(self, prefix, bound_type, *, db=None, **kwargs):
+        if bound_type == Bound.ITEM:
+            return self.move('next-item', prefix, db=db, **kwargs)
+        elif bound_type == Bound.TUPLE:
+            return self.move('next-tuple', prefix, db=db, **kwargs)
+        elif bound_type == Bound.COMPONENT:
+            return self.move('next-component', prefix, db=db, **kwargs)
         else:
-            return None
+            raise ValueError
 
-    @classmethod
-    def _path_importer_cache(cls, path):
-        """Get the finder for the path entry from sys.path_importer_cache.
-
-        If the path entry is not in the cache, find the appropriate finder
-        and cache it. If no finder is available, store None.
-
-        """
-        if path == '':
-            try:
-                path = _os.getcwd()
-            except FileNotFoundError:
-                # Don't cache the failure as the cwd can easily change to
-                # a valid directory later on.
-                return None
-        try:
-            finder = sys.path_importer_cache[path]
-        except KeyError:
-            finder = cls._path_hooks(path)
-            sys.path_importer_cache[path] = finder
-        return finder
-
-    @classmethod
-    def _legacy_get_spec(cls, fullname, finder):
-        # This would be a good place for a DeprecationWarning if
-        # we ended up going that route.
-        if hasattr(finder, 'find_loader'):
-            loader, portions = finder.find_loader(fullname)
+    def next_item(self, prefix, *, db=None, buffered=False, flush=False, **kwargs):
+        if flush:
+            self.next_buf.flush()
+        if buffered:
+            return self._buffered_next(prefix, Bound.ITEM, db=db if db else self.db, **kwargs)
         else:
-            loader = finder.find_module(fullname)
-            portions = []
-        if loader is not None:
-            return _bootstrap.spec_from_loader(fullname, loader)
-        spec = _bootstrap.ModuleSpec(fullname, None)
-        spec.submodule_search_locations = portions
-        return spec
-
-    @classmethod
-    def _get_spec(cls, fullname, path, target=None):
-        """Find the loader or namespace_path for this module/package name."""
-        # If this ends up being a namespace package, namespace_path is
-        #  the list of paths that will become its __path__
-        namespace_path = []
-        for entry in path:
-            if not isinstance(entry, (str, bytes)):
-                continue
-            finder = cls._path_importer_cache(entry)
-            if finder is not None:
-                if hasattr(finder, 'find_spec'):
-                    spec = finder.find_spec(fullname, target)
-                else:
-                    spec = cls._legacy_get_spec(fullname, finder)
-                if spec is None:
-                    continue
-                if spec.loader is not None:
-                    return spec
-                portions = spec.submodule_search_locations
-                if portions is None:
-                    raise ImportError('spec missing loader')
-                # This is possibly part of a namespace package.
-                #  Remember these path entries (if any) for when we
-                #  create a namespace package, and continue iterating
-                #  on path.
-                namespace_path.extend(portions)
+            return self.move('next-item', prefix, db=db, **kwargs)
+
+    def next_component(self, prefix, *, db=None, buffered=False, flush=False, **kwargs):
+        if flush:
+            self.next_buf.flush()
+        if buffered:
+            return self._buffered_next(prefix, Bound.COMPONENT, db=db if db else self.db, **kwargs)
         else:
-            spec = _bootstrap.ModuleSpec(fullname, None)
-            spec.submodule_search_locations = namespace_path
-            return spec
-
-    @classmethod
-    def find_spec(cls, fullname, path=None, target=None):
-        """Try to find a spec for 'fullname' on sys.path or 'path'.
+            return self.move('next-component', prefix, db=db, **kwargs)
 
-        The search is based on sys.path_hooks and sys.path_importer_cache.
-        """
-        if path is None:
-            path = sys.path
-        spec = cls._get_spec(fullname, path, target)
-        if spec is None:
-            return None
-        elif spec.loader is None:
-            namespace_path = spec.submodule_search_locations
-            if namespace_path:
-                # We found at least one namespace path.  Return a
-                #  spec which can create the namespace package.
-                spec.origin = 'namespace'
-                spec.submodule_search_locations = _NamespacePath(fullname, namespace_path, cls._get_spec)
-                return spec
-            else:
-                return None
+    def next_tuple(self, prefix, *, db=None, buffered=False, flush=False, **kwargs):
+        if flush:
+            self.next_buf.flush()
+        if buffered:
+            return self._buffered_next(prefix, Bound.TUPLE, db=db if db else self.db, **kwargs)
         else:
-            return spec
+            return self.move('next-tuple', prefix, db=db, **kwargs)
 
-    @classmethod
-    def find_module(cls, fullname, path=None):
-        """find the module on sys.path or 'path' based on sys.path_hooks and
-        sys.path_importer_cache.
+    def last_item(self, prefix, *, db=None, **kwargs):
+        return self.move('last-item', prefix, db=db, **kwargs)
 
-        This method is deprecated.  Use find_spec() instead.
+    def last_component(self, prefix, *, db=None, **kwargs):
+        return self.move('last-component', prefix, db=db, **kwargs)
 
+    def last_tuple(self, prefix, *, db=None, **kwargs):
+        return self.move('last-tuple', prefix, db=db, **kwargs)
+
+    def previous_item(self, prefix, *, db=None, **kwargs):
+        return self.move('previous-item', prefix, db=db, **kwargs)
+
+    def previous_component(self, prefix, *, db=None, **kwargs):
+        return self.move('previous-component', prefix, db=db, **kwargs)
+
+    def previous_tuple(self, prefix, *, db=None, **kwargs):
+        return self.move('previous-tuple', prefix, db=db, **kwargs)
+
+    def exists(self, item, *, db=None, **kwargs):
+        return self._do_command(item,
+                                db=db,
+                                content_type='application/json',
+                                no_content=True,
+                                action='exists', **kwargs)
+
+    def _simple_item_output_command(self, item, action, *, db, **kwargs):
+        return self._do_command(item,
+                                db=db,
+                                content_type='application/json',
+                                always_return_none=True,
+                                action=action, **kwargs)
+
+    def insert_item(self, item, *, db=None, **kwargs):
+        self._simple_item_output_command(item, 'insert-item', db=db, **kwargs)
+
+    def delete_item(self, item, *, db=None, **kwargs):
+        self._simple_item_output_command(item, 'delete-item', db=db, **kwargs)
+
+    def delete_subspace(self, item, *, db=None, **kwargs):
+        self._simple_item_output_command(item, 'delete-subspace', db=db, **kwargs)
+
+    def commit(self, *, db=None, **kwargs):
+        """ The global commit, not the optimistic commit 
+            You can use wait_for_durable and retry_time_out, in
+            milliseconds.
+            
+            Uses not application/json, but application/infinitydb
         """
-        spec = cls.find_spec(fullname, path)
-        if spec is None:
-            return None
-        return spec.loader
-
-
-class FileFinder:
-
-    """File-based finder.
-
-    Interactions with the file system are cached for performance, being
-    refreshed when the directory the finder is handling has been modified.
-
-    """
-
-    def __init__(self, path, *loader_details):
-        """Initialize with the path to search on and a variable number of
-        2-tuples containing the loader and the file suffixes the loader
-        recognizes."""
-        loaders = []
-        for loader, suffixes in loader_details:
-            loaders.extend((suffix, loader) for suffix in suffixes)
-        self._loaders = loaders
-        # Base (directory) path
-        self.path = path or '.'
-        self._path_mtime = -1
-        self._path_cache = set()
-        self._relaxed_path_cache = set()
-
-    def invalidate_caches(self):
-        """Invalidate the directory mtime."""
-        self._path_mtime = -1
-
-    find_module = _find_module_shim
-
-    def find_loader(self, fullname):
-        """Try to find a loader for the specified module, or the namespace
-        package portions. Returns (loader, list-of-portions).
-
-        This method is deprecated.  Use find_spec() instead.
-
+        # TODO untested
+        self._do_command(None,
+                        db=db,
+                        content_type='application/infinitydb',
+                        action='commit',
+                        always_return_none=True,
+                        wait_for_durable=True, **kwargs)
+
+    def roll_back(self, *, db=None, **kwargs):
+        """ The global rollback, not the optimistic rollback 
+            Uses not application/json, but application/infinitydb
         """
-        spec = self.find_spec(fullname)
-        if spec is None:
-            return None, []
-        return spec.loader, spec.submodule_search_locations or []
-
-    def _get_spec(self, loader_class, fullname, path, smsl, target):
-        loader = loader_class(fullname, path)
-        return spec_from_file_location(fullname, path, loader=loader,
-                                       submodule_search_locations=smsl)
+        # TODO untested
+        self._do_command(None, db=db,
+                        content_type='application/infinitydb',
+                        always_return_none=True,
+                        action='commit', **kwargs)
+
+    # TODO incomplete
+    # data is the dict for the query definition and source/dest prefixes,
+    # plus operation type: clear_results, merge_with_results, subtract_from_results.
+    # Also, a prefix referring to a stored query can be handled,
+    # but then we need to be able to override parts of it, especially
+    # the constants in the Where.
+#    def pattern_query(self, *, db=None, **kwargs):
+#        return self._do_command(None,
+#                                db=db,
+#                                content_type='application/infinitydb',
+#                                action='pattern-query',
+#                                  data=query_data,
+#                                  **kwargs)
+
+
+class Bound:
+    """ For NextBuf. How to find the prefix length. 
+    We go backwards from the end of the Item. The result 
+    is the start, the last tuple, or the last component.
+    Also, for tuples, truncate before the next EC/Att, and
+    for components, truncate after the final component.
+     """
+    ITEM = 0
+    TUPLE = 1
+    COMPONENT = 2
 
-    def find_spec(self, fullname, target=None):
-        """Try to find a spec for the specified module.
 
-        Returns the matching spec, or None if not found.
-        """
-        is_namespace = False
-        tail_module = fullname.rpartition('.')[2]
-        try:
-            mtime = _path_stat(self.path or _os.getcwd()).st_mtime
-        except OSError:
-            mtime = -1
-        if mtime != self._path_mtime:
-            self._fill_cache()
-            self._path_mtime = mtime
-        # tail_module keeps the original casing, for __file__ and friends
-        if _relax_case():
-            cache = self._relaxed_path_cache
-            cache_module = tail_module.lower()
-        else:
-            cache = self._path_cache
-            cache_module = tail_module
-        # Check if the module is the name of a directory (and thus a package).
-        if cache_module in cache:
-            base_path = _path_join(self.path, tail_module)
-            for suffix, loader_class in self._loaders:
-                init_filename = '__init__' + suffix
-                full_path = _path_join(base_path, init_filename)
-                if _path_isfile(full_path):
-                    return self._get_spec(loader_class, fullname, full_path, [base_path], target)
-            else:
-                # If a namespace package, return the path if we don't
-                #  find a module in the next section.
-                is_namespace = _path_isdir(base_path)
-        # Check for a file w/ a proper suffix exists.
-        for suffix, loader_class in self._loaders:
-            full_path = _path_join(self.path, tail_module + suffix)
-            _bootstrap._verbose_message('trying {}', full_path, verbosity=2)
-            if cache_module + suffix in cache:
-                if _path_isfile(full_path):
-                    return self._get_spec(loader_class, fullname, full_path,
-                                          None, target)
-        if is_namespace:
-            _bootstrap._verbose_message('possible namespace for {}', base_path)
-            spec = _bootstrap.ModuleSpec(fullname, None)
-            spec.submodule_search_locations = [base_path]
-            return spec
-        return None
+class NextBuf:
+    """ For reading batches of Items, which can be searched 
+    """
+    DEFAULT_SIZE = 1000
 
-    def _fill_cache(self):
-        """Fill the cache of potential modules and packages for this directory."""
-        path = self.path
-        try:
-            contents = _os.listdir(path or _os.getcwd())
-        except (FileNotFoundError, PermissionError, NotADirectoryError):
-            # Directory has either been removed, turned into a file, or made
-            # unreadable.
-            contents = []
-        # We store two cached versions, to handle runtime changes of the
-        # PYTHONCASEOK environment variable.
-        if not sys.platform.startswith('win'):
-            self._path_cache = set(contents)
+    def __init__(self, buf_filler):
+        # a list of items following the last fill
+        self.buf = []
+        self.db = None
+        # This function returns the next buf after a given item
+        self.buf_filler = buf_filler
+        self.size = NextBuf.DEFAULT_SIZE
+
+    def flush(self):
+        self.buf = []
+        self.db = None
+
+    def set_size(self, size):
+        self.size = size
+
+    def _get_last_tuple_off(self, item):
+        off = 0
+        for i in range(len(item)):
+            if isinstance(item[i], (EntityClass, Attribute)):
+                off = i + 1
+        return off
+
+    def _skip_tuple(self, item, off):
+        for i in range(off, len(item)):
+            if isinstance(item[i], (EntityClass, Attribute)):
+                return i
+        return len(item)
+
+    def _locate_prefix_in_buf(self, prefix):
+        for i in range(len(self.buf)):
+            if prefix == self.buf[i][:len(prefix)]:
+                return i
+        return -1
+
+    def _get_off_of_bound(self, item, bound_type):
+        if bound_type == Bound.ITEM:
+            return 0
+        elif bound_type == Bound.COMPONENT:
+            return len(item) - 1 if len(item) > 0 else 0
+        elif bound_type == Bound.TUPLE:
+            return self._get_last_tuple_off(item)
         else:
-            # Windows users can import modules with case-insensitive file
-            # suffixes (for legacy reasons). Make the suffix lowercase here
-            # so it's done once instead of for every import. This is safe as
-            # the specified suffixes to check against are always specified in a
-            # case-sensitive manner.
-            lower_suffix_contents = set()
-            for item in contents:
-                name, dot, suffix = item.partition('.')
-                if dot:
-                    new_name = '{}.{}'.format(name, suffix.lower())
-                else:
-                    new_name = name
-                lower_suffix_contents.add(new_name)
-            self._path_cache = lower_suffix_contents
-        if sys.platform.startswith(_CASE_INSENSITIVE_PLATFORMS):
-            self._relaxed_path_cache = {fn.lower() for fn in contents}
-
-    @classmethod
-    def path_hook(cls, *loader_details):
-        """A class method which returns a closure to use on sys.path_hook
-        which will return an instance using the specified loaders and the path
-        called on the closure.
-
-        If the path called on the closure is not a directory, ImportError is
-        raised.
-
-        """
-        def path_hook_for_FileFinder(path):
-            """Path hook for importlib.machinery.FileFinder."""
-            if not _path_isdir(path):
-                raise ImportError('only directories are supported', path=path)
-            return cls(path, *loader_details)
-
-        return path_hook_for_FileFinder
-
-    def __repr__(self):
-        return 'FileFinder({!r})'.format(self.path)
-
+            raise ValueError
 
-# Import setup ###############################################################
-
-def _fix_up_module(ns, name, pathname, cpathname=None):
-    # This function is used by PyImport_ExecCodeModuleObject().
-    loader = ns.get('__loader__')
-    spec = ns.get('__spec__')
-    if not loader:
-        if spec:
-            loader = spec.loader
-        elif pathname == cpathname:
-            loader = SourcelessFileLoader(name, pathname)
+    def _skip_bound(self, item, bound_type, off):
+        if bound_type == Bound.ITEM:
+            return len(item)
+        elif bound_type == Bound.COMPONENT:
+            return off + 1 if off < len(item) else len(item)
+        elif bound_type == Bound.TUPLE:
+            return self._skip_tuple(item, off)
         else:
-            loader = SourceFileLoader(name, pathname)
-    if not spec:
-        spec = spec_from_file_location(name, pathname, loader=loader)
-    try:
-        ns['__spec__'] = spec
-        ns['__loader__'] = loader
-        ns['__file__'] = pathname
-        ns['__cached__'] = cpathname
-    except Exception:
-        # Not important enough to report.
-        pass
-
+            raise ValueError
 
-def _get_supported_file_loaders():
-    """Returns a list of file-based module loaders.
-
-    Each item is a tuple (loader, suffixes).
+    """ We can't compare Items for magnitude as we can
+    in InfinityDB, so everything must use equality,
+    possibly over prefixes. This is not as good,
+    being linear in the buffer size, instead of log.
+
+     We have to match the previously found Item up
+     to after the last bound (such as the last tuple) or 
+     else read a buf starting at the next Item.
     """
-    extensions = ExtensionFileLoader, _imp.extension_suffixes()
-    source = SourceFileLoader, SOURCE_SUFFIXES
-    bytecode = SourcelessFileLoader, BYTECODE_SUFFIXES
-    return [extensions, source, bytecode]
-
+    ITEM_NOT_IN_BUF = -1
+    FINAL_ITEM = -2
 
-def _setup(_bootstrap_module):
-    """Setup the path-based importers for importlib by importing needed
-    built-in modules and injecting them into the global namespace.
+    def _get_next_from_buf(self, item, bound_type):
+        if not self.buf:
+            return NextBuf.ITEM_NOT_IN_BUF
+        # The given Item must be already there for quick success
+        pos = self._locate_prefix_in_buf(item)
+        if pos == -1:
+            # Must do it the hard way, by re-reading the buf.
+            return NextBuf.ITEM_NOT_IN_BUF
+        # item or its extension is found in buf at pos.
+        # find the last component or last tuple, or end of item
+        # according to the bound type
+        prefix_len = self._get_off_of_bound(item, bound_type)
+        # prefix_len is 0, or at last tuple or component
+        prefix = item[:prefix_len]
+        for i in range(pos, len(self.buf)):
+            found_item = self.buf[i]
+            if found_item[:prefix_len] != prefix:
+                # end of Items in this prefix
+                return NextBuf.FINAL_ITEM
+            after_bound = self._skip_bound(found_item,
+                                           bound_type, prefix_len)
+            truncated_found_item = found_item[:after_bound]
+            if truncated_found_item != item:
+                return truncated_found_item
+            # loop over extensions of item
+        return NextBuf.ITEM_NOT_IN_BUF
+
+    def next(self, item, bound_type, *, db, **kwargs):
+        if db != self.db:
+            self.db = db
+            self.buf = []
+        next_item = self._get_next_from_buf(item, bound_type)
+        if next_item == NextBuf.FINAL_ITEM:
+            # NO_CONTENT
+            return False, None
+        elif next_item != NextBuf.ITEM_NOT_IN_BUF:
+            return True, next_item
+        success, self.buf = self.buf_filler(item, bound_type, db=self.db, **kwargs)
+        if not success:
+            return False, None
+        # First Item in buf is nearest >= given item.
+        prefix_length = self._get_off_of_bound(item, bound_type)
+        next_item = self.buf[0]
+        if next_item == item:
+            # shouldn't happen
+            next_item = self.buf[1]
+        if next_item[:prefix_length] == item[:prefix_length]:
+            after_bound = self._skip_bound(next_item, bound_type, prefix_length)
+            return True, next_item[:after_bound]
+        return False, None
 
-    Other components are extracted from the core bootstrap module.
-
-    """
-    global sys, _imp, _bootstrap
-    _bootstrap = _bootstrap_module
-    sys = _bootstrap.sys
-    _imp = _bootstrap._imp
-
-    # Directly load built-in modules needed during bootstrap.
-    self_module = sys.modules[__name__]
-    for builtin_name in ('_io', '_warnings', 'builtins', 'marshal'):
-        if builtin_name not in sys.modules:
-            builtin_module = _bootstrap._builtin_from_name(builtin_name)
-        else:
-            builtin_module = sys.modules[builtin_name]
-        setattr(self_module, builtin_name, builtin_module)
-
-    # Directly load the os module (needed during bootstrap).
-    os_details = ('posix', ['/']), ('nt', ['\\', '/'])
-    for builtin_os, path_separators in os_details:
-        # Assumption made in _path_join()
-        assert all(len(sep) == 1 for sep in path_separators)
-        path_sep = path_separators[0]
-        if builtin_os in sys.modules:
-            os_module = sys.modules[builtin_os]
-            break
-        else:
-            try:
-                os_module = _bootstrap._builtin_from_name(builtin_os)
-                break
-            except ImportError:
-                continue
-    else:
-        raise ImportError('importlib requires posix or nt')
-    setattr(self_module, '_os', os_module)
-    setattr(self_module, 'path_sep', path_sep)
-    setattr(self_module, 'path_separators', ''.join(path_separators))
-
-    # Directly load the _thread module (needed during bootstrap).
-    try:
-        thread_module = _bootstrap._builtin_from_name('_thread')
-    except ImportError:
-        # Python was built without threads
-        thread_module = None
-    setattr(self_module, '_thread', thread_module)
-
-    # Directly load the _weakref module (needed during bootstrap).
-    weakref_module = _bootstrap._builtin_from_name('_weakref')
-    setattr(self_module, '_weakref', weakref_module)
-
-    # Directly load the winreg module (needed during bootstrap).
-    if builtin_os == 'nt':
-        winreg_module = _bootstrap._builtin_from_name('winreg')
-        setattr(self_module, '_winreg', winreg_module)
-
-    # Constants
-    setattr(self_module, '_relax_case', _make_relax_case())
-    EXTENSION_SUFFIXES.extend(_imp.extension_suffixes())
-    if builtin_os == 'nt':
-        SOURCE_SUFFIXES.append('.pyw')
-        if '_d.pyd' in EXTENSION_SUFFIXES:
-            WindowsRegistryFinder.DEBUG_BUILD = True
-
-
-def _install(_bootstrap_module):
-    """Install the path-based import components."""
-    _setup(_bootstrap_module)
-    supported_loaders = _get_supported_file_loaders()
-    sys.path_hooks.extend([FileFinder.path_hook(*supported_loaders)])
-    sys.meta_path.append(PathFinder)
```

### Comparing `infinitydb-1.0.0/env/Lib/site-packages/pep517-0.13.0.dist-info/LICENSE` & `infinitydb-1.0.1/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2017 Thomas Kluyver
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Roger L Deran
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `infinitydb-1.0.0/src/infinitydb.egg-info/PKG-INFO` & `infinitydb-1.0.1/src/infinitydb.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `infinitydb-1.0.0/README.md` & `infinitydb-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,9 +18,9 @@
  
  The actual access is done through the module's convenience
  functions. Also, the data representation of 'Items' is
  more general than JSON, so there are functions to
  convert from JSON to Python dicts and deal with
  tuples.
  
- See [boilerbay.com](boilerbay.com) for more.
+ See [boilerbay.com](https://boilerbay.com) for more.
```

### Comparing `infinitydb-1.0.0/pyproject.toml` & `infinitydb-1.0.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "infinitydb"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Roger Deran", email="roger.deran@gmail.com" },
 ]
 description = "Access to the InfinityDB server via REST"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-
+dependencies = [
+  'python-dateutil >= 2.8.2',
+  'requests',
+]
 [project.urls]
 Homepage = "https://boilerbay.com"
```

### Comparing `infinitydb-1.0.0/PKG-INFO` & `infinitydb-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: infinitydb
-Version: 1.0.0
+Version: 1.0.1
 Summary: Access to the InfinityDB server via REST
 Project-URL: Homepage, https://boilerbay.com
 Author-email: Roger Deran <roger.deran@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 
 # InfinityDB NoSQL DBMS REST Access
 
 The infinitydb.access module provides a REST interface to the APIs
 defined in the server by means of PatternQueries.
@@ -31,9 +33,9 @@
  
  The actual access is done through the module's convenience
  functions. Also, the data representation of 'Items' is
  more general than JSON, so there are functions to
  convert from JSON to Python dicts and deal with
  tuples.
  
- See [boilerbay.com](boilerbay.com) for more.
+ See [boilerbay.com](https://boilerbay.com) for more.
```

