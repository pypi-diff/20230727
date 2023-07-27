# Comparing `tmp/lazyinit-0.0.269.tar.gz` & `tmp/lazyinit-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyinit-0.0.269.tar", last modified: Thu Jul 27 11:16:33 2023, max compression
+gzip compressed data, was "lazyinit-0.0.27.tar", last modified: Thu Jul 27 11:55:42 2023, max compression
```

## Comparing `lazyinit-0.0.269.tar` & `lazyinit-0.0.27.tar`

### file list

```diff
@@ -1,347 +1,346 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.189023 lazyinit-0.0.269/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.125133 lazyinit-0.0.269/.git/
--rw-r--r--   0 dengyifan   (501) staff       (20)        3 2023-07-26 06:54:32.000000 lazyinit-0.0.269/.git/COMMIT_EDITMSG
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:11:53.000000 lazyinit-0.0.269/.git/FETCH_HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)       23 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 15:01:28.000000 lazyinit-0.0.269/.git/ORIG_HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)      345 2023-07-26 04:10:40.000000 lazyinit-0.0.269/.git/config
--rw-r--r--   0 dengyifan   (501) staff       (20)       73 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/description
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.127997 lazyinit-0.0.269/.git/hooks/
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      478 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      896 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4726 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      189 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/post-update.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      424 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1643 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      416 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1374 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/pre-push.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4898 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      544 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1492 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     2783 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     3650 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/hooks/update.sample
--rw-r--r--   0 dengyifan   (501) staff       (20)     4305 2023-07-26 15:01:28.000000 lazyinit-0.0.269/.git/index
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.128183 lazyinit-0.0.269/.git/info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      240 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/info/exclude
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.128354 lazyinit-0.0.269/.git/logs/
--rw-r--r--   0 dengyifan   (501) staff       (20)     1795 2023-07-26 15:01:28.000000 lazyinit-0.0.269/.git/logs/HEAD
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.105627 lazyinit-0.0.269/.git/logs/refs/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.128544 lazyinit-0.0.269/.git/logs/refs/heads/
--rw-r--r--   0 dengyifan   (501) staff       (20)     1795 2023-07-26 15:01:28.000000 lazyinit-0.0.269/.git/logs/refs/heads/master
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.105682 lazyinit-0.0.269/.git/logs/refs/remotes/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.129464 lazyinit-0.0.269/.git/logs/refs/remotes/origin/
--rw-r--r--   0 dengyifan   (501) staff       (20)     4396 2023-07-27 10:59:16.000000 lazyinit-0.0.269/.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)     1739 2023-07-26 08:16:23.000000 lazyinit-0.0.269/.git/logs/refs/remotes/origin/master
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.119873 lazyinit-0.0.269/.git/objects/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.129701 lazyinit-0.0.269/.git/objects/00/
--r--r--r--   0 dengyifan   (501) staff       (20)      147 2023-07-25 11:33:45.000000 lazyinit-0.0.269/.git/objects/00/41c04b20be6b4bbd75a815bebf7084805f8712
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.130018 lazyinit-0.0.269/.git/objects/01/
--r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 05:00:09.000000 lazyinit-0.0.269/.git/objects/01/cab3024759cc906cee0a6a3429918f5b63fabc
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.132203 lazyinit-0.0.269/.git/objects/04/
--r--r--r--   0 dengyifan   (501) staff       (20)      553 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063
--r--r--r--   0 dengyifan   (501) staff       (20)     1851 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.132598 lazyinit-0.0.269/.git/objects/05/
--r--r--r--   0 dengyifan   (501) staff       (20)      223 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/05/1acb58a6d6c6dbb4150bf9221569e1912eb5bc
--r--r--r--   0 dengyifan   (501) staff       (20)    42257 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.133333 lazyinit-0.0.269/.git/objects/0a/
--r--r--r--   0 dengyifan   (501) staff       (20)     2023 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.134824 lazyinit-0.0.269/.git/objects/0e/
--r--r--r--   0 dengyifan   (501) staff       (20)      261 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/0e/24281e6a23a799bba50234909a4eefc062407f
--r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 05:00:09.000000 lazyinit-0.0.269/.git/objects/0e/3fb35ffbadaf084a2915cfc29e9f63d8dc0b80
--r--r--r--   0 dengyifan   (501) staff       (20)     2330 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.135100 lazyinit-0.0.269/.git/objects/11/
--r--r--r--   0 dengyifan   (501) staff       (20)      119 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/11/f13a31edccde503893c6083b99d6243e26f111
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.135289 lazyinit-0.0.269/.git/objects/14/
--r--r--r--   0 dengyifan   (501) staff       (20)      146 2023-07-26 06:54:32.000000 lazyinit-0.0.269/.git/objects/14/2068ef3450523a0e5f073bd62eec3746405639
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.135588 lazyinit-0.0.269/.git/objects/1c/
--r--r--r--   0 dengyifan   (501) staff       (20)     1604 2023-07-26 08:16:23.000000 lazyinit-0.0.269/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.135892 lazyinit-0.0.269/.git/objects/1f/
--r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-25 11:16:46.000000 lazyinit-0.0.269/.git/objects/1f/bc66f0cf2ebf60d3c3d235e0e619a1f6622dbe
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.136434 lazyinit-0.0.269/.git/objects/22/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 14:00:51.000000 lazyinit-0.0.269/.git/objects/22/1b9304fb057784a1c767bdf222a4fd449db92f
--r--r--r--   0 dengyifan   (501) staff       (20)      283 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/22/28de42f4fd7fd7e337c26be6c47fa320f3555f
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.136617 lazyinit-0.0.269/.git/objects/24/
--r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-25 11:16:46.000000 lazyinit-0.0.269/.git/objects/24/0d08419d20e2d7cb6985f76926f93b83a8daa7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.136902 lazyinit-0.0.269/.git/objects/28/
--r--r--r--   0 dengyifan   (501) staff       (20)      358 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/28/5445a221c929c5f5f87e202f37320844e8f6d0
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.137967 lazyinit-0.0.269/.git/objects/2a/
--r--r--r--   0 dengyifan   (501) staff       (20)     1878 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.138919 lazyinit-0.0.269/.git/objects/2b/
--r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 05:00:09.000000 lazyinit-0.0.269/.git/objects/2b/c85ce5ce789ef99ce23645128dcbaad1ff3835
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.139284 lazyinit-0.0.269/.git/objects/2d/
--r--r--r--   0 dengyifan   (501) staff       (20)      372 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/2d/d1db85bd19ef19b8f7730625f1740902a4f846
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.139509 lazyinit-0.0.269/.git/objects/2e/
--r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.140044 lazyinit-0.0.269/.git/objects/32/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/32/025d715d168680f84c440a9eaa445bcfe82201
--r--r--r--   0 dengyifan   (501) staff       (20)     2217 2023-07-25 11:33:45.000000 lazyinit-0.0.269/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.140339 lazyinit-0.0.269/.git/objects/33/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 14:00:51.000000 lazyinit-0.0.269/.git/objects/33/1de14f34212468dbd7962fcd3aa2c27159be15
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.140623 lazyinit-0.0.269/.git/objects/38/
--r--r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/38/d0b85fd4bdd1685656cd6027825010486286ab
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.141271 lazyinit-0.0.269/.git/objects/39/
--r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/39/c27ee30de9577fb056d6adf1a75b5040624f1a
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:41:16.000000 lazyinit-0.0.269/.git/objects/39/df26c768c14049a07f62ddef6c9d8fe3635b43
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.141892 lazyinit-0.0.269/.git/objects/3d/
--r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-26 05:00:09.000000 lazyinit-0.0.269/.git/objects/3d/5d200d32889f9867e73ddd61f8de5d54006cca
--r--r--r--   0 dengyifan   (501) staff       (20)     1867 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.142113 lazyinit-0.0.269/.git/objects/40/
--r--r--r--   0 dengyifan   (501) staff       (20)      513 2023-07-25 11:41:16.000000 lazyinit-0.0.269/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.142402 lazyinit-0.0.269/.git/objects/41/
--r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 06:54:32.000000 lazyinit-0.0.269/.git/objects/41/483d9c24d49b463a3afea6c339c9444c92f01d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.142707 lazyinit-0.0.269/.git/objects/43/
--r--r--r--   0 dengyifan   (501) staff       (20)      291 2023-07-25 11:16:46.000000 lazyinit-0.0.269/.git/objects/43/3b5b7262dcbe0429a0a8e7ed7aee7ed4793ed4
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.144189 lazyinit-0.0.269/.git/objects/4d/
--r--r--r--   0 dengyifan   (501) staff       (20)     1995 2023-07-26 05:00:09.000000 lazyinit-0.0.269/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.144539 lazyinit-0.0.269/.git/objects/52/
--r--r--r--   0 dengyifan   (501) staff       (20)     2033 2023-07-25 11:41:16.000000 lazyinit-0.0.269/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.144819 lazyinit-0.0.269/.git/objects/55/
--r--r--r--   0 dengyifan   (501) staff       (20)      145 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/55/3ee9d39a64d1c55b084c4821a83d6574cee6da
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.147020 lazyinit-0.0.269/.git/objects/56/
--r--r--r--   0 dengyifan   (501) staff       (20)     3553 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.147494 lazyinit-0.0.269/.git/objects/5a/
--r--r--r--   0 dengyifan   (501) staff       (20)     1979 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.147886 lazyinit-0.0.269/.git/objects/5e/
--r--r--r--   0 dengyifan   (501) staff       (20)     1486 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.148369 lazyinit-0.0.269/.git/objects/5f/
--r--r--r--   0 dengyifan   (501) staff       (20)      125 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/5f/21b1e6c2be3514a4d5118cd8db61899648080a
--r--r--r--   0 dengyifan   (501) staff       (20)      549 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.148918 lazyinit-0.0.269/.git/objects/60/
--r--r--r--   0 dengyifan   (501) staff       (20)      514 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 06:54:32.000000 lazyinit-0.0.269/.git/objects/60/41ee332e98835ce7e3ed8b3ae41f91352bec33
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.149570 lazyinit-0.0.269/.git/objects/63/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/63/29d30bc981284e510de0c1938ade4c16e7bde9
--r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/63/3cf9d6946c15485dcb3cf3889f6b34de0c0bcd
--r--r--r--   0 dengyifan   (501) staff       (20)     2007 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.149825 lazyinit-0.0.269/.git/objects/64/
--r--r--r--   0 dengyifan   (501) staff       (20)     2420 2023-07-26 05:00:09.000000 lazyinit-0.0.269/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.150113 lazyinit-0.0.269/.git/objects/67/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/67/bf3997c2bc19d4034bd741ab9808c86b52376b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.150371 lazyinit-0.0.269/.git/objects/69/
--r--r--r--   0 dengyifan   (501) staff       (20)      930 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.150637 lazyinit-0.0.269/.git/objects/6a/
--r--r--r--   0 dengyifan   (501) staff       (20)     1554 2023-07-26 05:00:09.000000 lazyinit-0.0.269/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.150901 lazyinit-0.0.269/.git/objects/6b/
--r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.151435 lazyinit-0.0.269/.git/objects/6c/
--r--r--r--   0 dengyifan   (501) staff       (20)     1966 2023-07-25 11:16:46.000000 lazyinit-0.0.269/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66
--r--r--r--   0 dengyifan   (501) staff       (20)      233 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/6c/f23ede6f0221263856d80f2287298ce360df0d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.151661 lazyinit-0.0.269/.git/objects/6d/
--r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/6d/8911d55f9896b814e9db65f2edc1da1524c03b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.152133 lazyinit-0.0.269/.git/objects/6e/
--r--r--r--   0 dengyifan   (501) staff       (20)       37 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/6e/30ca1116ed7b5e804a19fc761a7a2d58c0e1dd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.152546 lazyinit-0.0.269/.git/objects/6f/
--r--r--r--   0 dengyifan   (501) staff       (20)      496 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/6f/9a4b893df9fff8b3995e4014388ba30f129cd2
--r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.269/.git/objects/6f/cdcf4e30a9697c1f5aceaf1dc7d39d98739f51
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.152855 lazyinit-0.0.269/.git/objects/73/
--r--r--r--   0 dengyifan   (501) staff       (20)       91 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/73/58417a5d41c0ae3f227f79be64cff1341921f3
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.159444 lazyinit-0.0.269/.git/objects/74/
--r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/74/453505ab7b002053a991e77614b41494aefd94
--r--r--r--   0 dengyifan   (501) staff       (20)      180 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/74/94617eb236a96a42041354b497fb373ff69e2a
--r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.269/.git/objects/74/e45b20bcfa13204500b46f9b3f794a2eedd610
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.159758 lazyinit-0.0.269/.git/objects/7e/
--r--r--r--   0 dengyifan   (501) staff       (20)      499 2023-07-25 11:33:45.000000 lazyinit-0.0.269/.git/objects/7e/cdeefbee966a2c48b1f3e93aef8772a83a927b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.160057 lazyinit-0.0.269/.git/objects/7f/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/7f/3aff99db09db5b9be0eb49dfbb83e5a2b2dfe6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.160290 lazyinit-0.0.269/.git/objects/80/
--r--r--r--   0 dengyifan   (501) staff       (20)      561 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.160775 lazyinit-0.0.269/.git/objects/83/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:41:16.000000 lazyinit-0.0.269/.git/objects/83/410ee7dbb23a43716f77560dfb52b6dbab167b
--r--r--r--   0 dengyifan   (501) staff       (20)     7437 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.161108 lazyinit-0.0.269/.git/objects/84/
--r--r--r--   0 dengyifan   (501) staff       (20)      281 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/84/32f5170b60379a5440d18af5c42da0c20bab36
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.161368 lazyinit-0.0.269/.git/objects/86/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 08:16:23.000000 lazyinit-0.0.269/.git/objects/86/305819935ba7c71d91c90bb164a58e855e7d1e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.161603 lazyinit-0.0.269/.git/objects/87/
--r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 08:16:23.000000 lazyinit-0.0.269/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.161873 lazyinit-0.0.269/.git/objects/88/
--r--r--r--   0 dengyifan   (501) staff       (20)     3155 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.162107 lazyinit-0.0.269/.git/objects/89/
--r--r--r--   0 dengyifan   (501) staff       (20)       34 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/89/fe87522f1d1d21fb72f29e4a3f3044b32cc64c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.162305 lazyinit-0.0.269/.git/objects/8b/
--r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 08:16:23.000000 lazyinit-0.0.269/.git/objects/8b/538f3380f85f22fc479f2298de08af638d91f6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.162522 lazyinit-0.0.269/.git/objects/8f/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/8f/821694556aac2a278c288de223659193dd2489
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.162718 lazyinit-0.0.269/.git/objects/91/
--r--r--r--   0 dengyifan   (501) staff       (20)     2328 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.163478 lazyinit-0.0.269/.git/objects/96/
--r--r--r--   0 dengyifan   (501) staff       (20)     3726 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/96/7c51d6a0690049febfd310c0257eb795caeaef
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.163703 lazyinit-0.0.269/.git/objects/99/
--r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/99/aee23747e74ecbb3e8ebdc64b65c85c55f51dd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.164220 lazyinit-0.0.269/.git/objects/9c/
--r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef
--r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/9c/fa0e1bf241048b8a143c7fef01067d5f9c3ac7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.164985 lazyinit-0.0.269/.git/objects/9d/
--r--r--r--   0 dengyifan   (501) staff       (20)      150 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/9d/1f61df1650e8ae0165c5d3e1f47e8384a76e25
--r--r--r--   0 dengyifan   (501) staff       (20)     2983 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.165795 lazyinit-0.0.269/.git/objects/a0/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/a0/2c8ecffe863e22a9a7510d5af5f8472da012c4
--r--r--r--   0 dengyifan   (501) staff       (20)      494 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/a0/8ceea5fa60b6a189bf2ca3e11a3e82d84375ea
--r--r--r--   0 dengyifan   (501) staff       (20)     1903 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.166415 lazyinit-0.0.269/.git/objects/a1/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:33:45.000000 lazyinit-0.0.269/.git/objects/a1/e2f9a9114e1b772f7fb22f7c2a26fc8fcf25ac
--r--r--r--   0 dengyifan   (501) staff       (20)     2165 2023-07-25 11:16:46.000000 lazyinit-0.0.269/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.166811 lazyinit-0.0.269/.git/objects/a3/
--r--r--r--   0 dengyifan   (501) staff       (20)      555 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.167380 lazyinit-0.0.269/.git/objects/a8/
--r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 05:00:09.000000 lazyinit-0.0.269/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:33:45.000000 lazyinit-0.0.269/.git/objects/a8/8453b2586a082782d165b46444353c6fda84f5
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.167691 lazyinit-0.0.269/.git/objects/a9/
--r--r--r--   0 dengyifan   (501) staff       (20)     1465 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.168371 lazyinit-0.0.269/.git/objects/aa/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 05:00:09.000000 lazyinit-0.0.269/.git/objects/aa/2f814ba87b54003ea2facaf8a8ac437b174212
--r--r--r--   0 dengyifan   (501) staff       (20)      920 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487
--r--r--r--   0 dengyifan   (501) staff       (20)     1811 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.168674 lazyinit-0.0.269/.git/objects/ad/
--r--r--r--   0 dengyifan   (501) staff       (20)     3750 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.169131 lazyinit-0.0.269/.git/objects/ae/
--r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/ae/99dcc87c6ca438bd127b06eee3ccc47f4ffd6c
--r--r--r--   0 dengyifan   (501) staff       (20)      215 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/ae/ca62bc1646058816f9a5bddd5681d0fb939b24
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.169747 lazyinit-0.0.269/.git/objects/af/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/af/272c05462dae29b6aadb455022bdbbf9f531e7
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/af/38c03c42f711bbfe4db00e49e92fb5761c80d7
--r--r--r--   0 dengyifan   (501) staff       (20)     1602 2023-07-26 06:54:32.000000 lazyinit-0.0.269/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.170400 lazyinit-0.0.269/.git/objects/b0/
--r--r--r--   0 dengyifan   (501) staff       (20)     4121 2023-07-26 05:00:09.000000 lazyinit-0.0.269/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:16:46.000000 lazyinit-0.0.269/.git/objects/b0/8c7ef81a8076086a4529e40583d52ff2e03d24
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.170687 lazyinit-0.0.269/.git/objects/b1/
--r--r--r--   0 dengyifan   (501) staff       (20)      729 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.170913 lazyinit-0.0.269/.git/objects/b4/
--r--r--r--   0 dengyifan   (501) staff       (20)      124 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/b4/31ec69865aa69f6bbac9893d5f3266ecd13273
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.171447 lazyinit-0.0.269/.git/objects/b6/
--r--r--r--   0 dengyifan   (501) staff       (20)      218 2023-07-25 11:16:46.000000 lazyinit-0.0.269/.git/objects/b6/9f632da541ff48fd18a636d74fca4d80935113
--r--r--r--   0 dengyifan   (501) staff       (20)       20 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/b6/fc4c620b67d95f953a5c1c1230aaab5db5a1b0
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.171701 lazyinit-0.0.269/.git/objects/b7/
--r--r--r--   0 dengyifan   (501) staff       (20)      500 2023-07-25 11:16:46.000000 lazyinit-0.0.269/.git/objects/b7/8ccba97db82f1ca4c6db7e0b5cd1bd8af07780
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.171913 lazyinit-0.0.269/.git/objects/bb/
--r--r--r--   0 dengyifan   (501) staff       (20)       31 2023-07-26 06:54:32.000000 lazyinit-0.0.269/.git/objects/bb/b84aa70c64fb0114dfa2f1df1cfffbc0123de9
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.173027 lazyinit-0.0.269/.git/objects/bc/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/bc/771507d6ab55b2ca55d1b567dc38064561aa6f
--r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01
--r--r--r--   0 dengyifan   (501) staff       (20)     2346 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385
--r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-25 11:41:16.000000 lazyinit-0.0.269/.git/objects/bc/e5df5b3fb9303de75d9ba662475c2e0940387e
--r--r--r--   0 dengyifan   (501) staff       (20)      200 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/bc/ed2eb0d31276a7b1ddfe5855190dc53fec2a91
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.173282 lazyinit-0.0.269/.git/objects/c1/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/c1/b6c43ce95f33b1c96bb259fd2c2facd4406ef8
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.173551 lazyinit-0.0.269/.git/objects/c4/
--r--r--r--   0 dengyifan   (501) staff       (20)     2032 2023-07-25 11:33:45.000000 lazyinit-0.0.269/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.174061 lazyinit-0.0.269/.git/objects/c5/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/c5/4ad76a5bccb99831a7a16f98637da3903c2cec
--r--r--r--   0 dengyifan   (501) staff       (20)      450 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/c5/f23c1c12745e22b14c79b57d397ae6685cf564
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.174242 lazyinit-0.0.269/.git/objects/c7/
--r--r--r--   0 dengyifan   (501) staff       (20)     1654 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.174433 lazyinit-0.0.269/.git/objects/c9/
--r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.174721 lazyinit-0.0.269/.git/objects/ca/
--r--r--r--   0 dengyifan   (501) staff       (20)     1263 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.175392 lazyinit-0.0.269/.git/objects/cc/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/cc/3a12d725fdd1884f2f104e1c11d8b87c1367cc
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/cc/46e850693cec9659b52d57dd78d6f60c242ebb
--r--r--r--   0 dengyifan   (501) staff       (20)      716 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.175998 lazyinit-0.0.269/.git/objects/cd/
--r--r--r--   0 dengyifan   (501) staff       (20)     5189 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591
--r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 06:54:32.000000 lazyinit-0.0.269/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.176278 lazyinit-0.0.269/.git/objects/ce/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/ce/3694e653f842cc70a8c5ef32cd9f75639bb14a
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.176515 lazyinit-0.0.269/.git/objects/d9/
--r--r--r--   0 dengyifan   (501) staff       (20)     5194 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.176805 lazyinit-0.0.269/.git/objects/da/
--r--r--r--   0 dengyifan   (501) staff       (20)      491 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/da/9fd18a499c0821bea6c2313d252a1d4bcf5846
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.177110 lazyinit-0.0.269/.git/objects/de/
--r--r--r--   0 dengyifan   (501) staff       (20)      100 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/de/8f446f94a50f937fed1c254a966f3ed6088e81
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.177372 lazyinit-0.0.269/.git/objects/df/
--r--r--r--   0 dengyifan   (501) staff       (20)     1977 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.177580 lazyinit-0.0.269/.git/objects/e4/
--r--r--r--   0 dengyifan   (501) staff       (20)      149 2023-07-25 14:00:51.000000 lazyinit-0.0.269/.git/objects/e4/632035cac16d026cc02de90ae31aef87867116
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.177884 lazyinit-0.0.269/.git/objects/e6/
--r--r--r--   0 dengyifan   (501) staff       (20)       15 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.178516 lazyinit-0.0.269/.git/objects/e8/
--r--r--r--   0 dengyifan   (501) staff       (20)      556 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b
--r--r--r--   0 dengyifan   (501) staff       (20)     1289 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.179025 lazyinit-0.0.269/.git/objects/eb/
--r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/eb/758cdc0fe911d913b208b48ee0ac14886927eb
--r--r--r--   0 dengyifan   (501) staff       (20)      566 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.179251 lazyinit-0.0.269/.git/objects/ec/
--r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/ec/47fd64ca8d46a3a1c345708cf6dd4b19e2d7a6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.179562 lazyinit-0.0.269/.git/objects/ef/
--r--r--r--   0 dengyifan   (501) staff       (20)      219 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/ef/0a2b00e7e0280dfe13a94d5abfeeba9aafabae
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.180033 lazyinit-0.0.269/.git/objects/f0/
--r--r--r--   0 dengyifan   (501) staff       (20)     8516 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c
--r--r--r--   0 dengyifan   (501) staff       (20)      433 2023-07-24 06:27:07.000000 lazyinit-0.0.269/.git/objects/f0/b6b75cf9a30d91dab0d80449c7c76a0191d8a7
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.180234 lazyinit-0.0.269/.git/objects/f1/
--r--r--r--   0 dengyifan   (501) staff       (20)      559 2023-07-26 04:07:28.000000 lazyinit-0.0.269/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.180458 lazyinit-0.0.269/.git/objects/f2/
--r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/f2/f3ccb260633b09276ccaaa358ce7df1a0025f6
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.180662 lazyinit-0.0.269/.git/objects/f5/
--r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 14:32:29.000000 lazyinit-0.0.269/.git/objects/f5/96444b272664dff576dc8ac874152f461a4f6e
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.180866 lazyinit-0.0.269/.git/objects/f6/
--r--r--r--   0 dengyifan   (501) staff       (20)     2002 2023-07-26 03:36:35.000000 lazyinit-0.0.269/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.120245 lazyinit-0.0.269/.git/refs/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.181076 lazyinit-0.0.269/.git/refs/heads/
--rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 15:01:28.000000 lazyinit-0.0.269/.git/refs/heads/master
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.120320 lazyinit-0.0.269/.git/refs/remotes/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.181650 lazyinit-0.0.269/.git/refs/remotes/origin/
--rw-r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-27 10:59:16.000000 lazyinit-0.0.269/.git/refs/remotes/origin/HEAD
--rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 08:16:23.000000 lazyinit-0.0.269/.git/refs/remotes/origin/master
--rw-r--r--   0 dengyifan   (501) staff       (20)       17 2023-07-26 05:01:41.000000 lazyinit-0.0.269/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-27 11:16:33.188830 lazyinit-0.0.269/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.269/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.182708 lazyinit-0.0.269/lazyinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.269/lazyinit/__init__.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.183893 lazyinit-0.0.269/lazyinit/__pycache__/
--rw-r--r--   0 dengyifan   (501) staff       (20)     8725 2023-07-26 04:15:42.000000 lazyinit-0.0.269/lazyinit/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 dengyifan   (501) staff       (20)     3763 2023-07-25 04:13:11.000000 lazyinit-0.0.269/lazyinit/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.269/lazyinit/bash_config.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     8515 2023-07-27 11:16:16.000000 lazyinit-0.0.269/lazyinit/init.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.184545 lazyinit-0.0.269/lazyinit/lazydl/
--rw-r--r--   0 dengyifan   (501) staff       (20)        5 2023-07-23 08:07:15.000000 lazyinit-0.0.269/lazyinit/lazydl/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.184657 lazyinit-0.0.269/lazyinit/lazydl/configs/
--rw-r--r--   0 dengyifan   (501) staff       (20)     1569 2023-07-25 13:48:22.000000 lazyinit-0.0.269/lazyinit/lazydl/configs/default_config.yaml
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.184793 lazyinit-0.0.269/lazyinit/lazydl/configs/exps/
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.185069 lazyinit-0.0.269/lazyinit/lazydl/configs/exps/focusl/
--rw-r--r--   0 dengyifan   (501) staff       (20)     3903 2023-07-25 13:51:05.000000 lazyinit-0.0.269/lazyinit/lazydl/configs/exps/focusl/baseline.yaml
--rw-r--r--   0 dengyifan   (501) staff       (20)    74072 2023-07-25 04:24:11.000000 lazyinit-0.0.269/lazyinit/lazydl/configs/exps/focusl/exp_plan.yaml
--rw-r--r--   0 dengyifan   (501) staff       (20)      644 2023-07-23 08:07:15.000000 lazyinit-0.0.269/lazyinit/lazydl/configs/exps/overfit_test.yaml
--rw-r--r--   0 dengyifan   (501) staff       (20)     1179 2023-07-23 08:16:18.000000 lazyinit-0.0.269/lazyinit/lazydl/minist.py
--rw-r--r--   0 dengyifan   (501) staff       (20)       16 2023-07-23 08:07:15.000000 lazyinit-0.0.269/lazyinit/lazydl/requirements.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     2727 2023-07-23 08:07:15.000000 lazyinit-0.0.269/lazyinit/lazydl/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-24 14:38:46.000000 lazyinit-0.0.269/lazyinit/lazydl/start.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.186212 lazyinit-0.0.269/lazyinit/ranger/
--rw-r--r--   0 dengyifan   (501) staff       (20)     6148 2023-07-24 04:18:46.000000 lazyinit-0.0.269/lazyinit/ranger/.DS_Store
--rwxr-xr-x   0 dengyifan   (501) staff       (20)       23 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.187393 lazyinit-0.0.269/lazyinit/ranger/colorschemes/
--rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/colorschemes/__init__.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      139 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/colorschemes/__init__.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     5769 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/colorschemes/default.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      696 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/colorschemes/jungle.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1171 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/colorschemes/snow.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1335 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/colorschemes/snow.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4929 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/colorschemes/zenburn.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     4758 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/commands.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.188583 lazyinit-0.0.269/lazyinit/ranger/plugins/
--rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/plugins/__init__.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      134 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/plugins/__init__.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    10718 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/plugins/devicons.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     6817 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/plugins/devicons.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)      479 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/plugins/devicons_linemode.py
--rwxr-xr-x   0 dengyifan   (501) staff       (20)     1271 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/plugins/devicons_linemode.pyo
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    23026 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/rc-sample.conf
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    18894 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/rc.conf
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    13012 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/rifle.conf
--rwxr-xr-x   0 dengyifan   (501) staff       (20)    10000 2023-07-23 10:15:36.000000 lazyinit-0.0.269/lazyinit/ranger/scope.sh
--rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.269/lazyinit/redis.conf
--rw-r--r--   0 dengyifan   (501) staff       (20)      142 2023-07-27 04:35:53.000000 lazyinit-0.0.269/lazyinit/redis.sh
--rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.269/lazyinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     6730 2023-07-27 11:05:08.000000 lazyinit-0.0.269/lazyinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:16:33.183607 lazyinit-0.0.269/lazyinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-27 11:16:33.000000 lazyinit-0.0.269/lazyinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)    10075 2023-07-27 11:16:33.000000 lazyinit-0.0.269/lazyinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-27 11:16:33.000000 lazyinit-0.0.269/lazyinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-27 11:16:33.000000 lazyinit-0.0.269/lazyinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-27 11:16:33.000000 lazyinit-0.0.269/lazyinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-27 11:16:33.000000 lazyinit-0.0.269/lazyinit.egg-info/top_level.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     1059 2023-07-23 12:54:16.000000 lazyinit-0.0.269/push.sh
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-27 11:16:33.189081 lazyinit-0.0.269/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      843 2023-07-27 11:05:13.000000 lazyinit-0.0.269/setup.py
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-27 10:58:57.000000 lazyinit-0.0.269/z.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.741329 lazyinit-0.0.27/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.657138 lazyinit-0.0.27/.git/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        3 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/COMMIT_EDITMSG
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:12.000000 lazyinit-0.0.27/.git/FETCH_HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       23 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 15:01:28.000000 lazyinit-0.0.27/.git/ORIG_HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)      345 2023-07-26 04:10:40.000000 lazyinit-0.0.27/.git/config
+-rw-r--r--   0 dengyifan   (501) staff       (20)       73 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/description
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.660115 lazyinit-0.0.27/.git/hooks/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      478 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      896 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4726 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      189 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/post-update.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      424 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1643 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      416 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1374 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4898 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      544 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1492 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     2783 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     3650 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/hooks/update.sample
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4305 2023-07-26 15:01:28.000000 lazyinit-0.0.27/.git/index
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.660328 lazyinit-0.0.27/.git/info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      240 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/info/exclude
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.660519 lazyinit-0.0.27/.git/logs/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1795 2023-07-26 15:01:28.000000 lazyinit-0.0.27/.git/logs/HEAD
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.644592 lazyinit-0.0.27/.git/logs/refs/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.660707 lazyinit-0.0.27/.git/logs/refs/heads/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1795 2023-07-26 15:01:28.000000 lazyinit-0.0.27/.git/logs/refs/heads/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.644643 lazyinit-0.0.27/.git/logs/refs/remotes/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.661167 lazyinit-0.0.27/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4396 2023-07-27 10:59:16.000000 lazyinit-0.0.27/.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1739 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/logs/refs/remotes/origin/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.653260 lazyinit-0.0.27/.git/objects/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.661354 lazyinit-0.0.27/.git/objects/00/
+-r--r--r--   0 dengyifan   (501) staff       (20)      147 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/00/41c04b20be6b4bbd75a815bebf7084805f8712
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.661618 lazyinit-0.0.27/.git/objects/01/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/01/cab3024759cc906cee0a6a3429918f5b63fabc
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.662081 lazyinit-0.0.27/.git/objects/04/
+-r--r--r--   0 dengyifan   (501) staff       (20)      553 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063
+-r--r--r--   0 dengyifan   (501) staff       (20)     1851 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.662468 lazyinit-0.0.27/.git/objects/05/
+-r--r--r--   0 dengyifan   (501) staff       (20)      223 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/05/1acb58a6d6c6dbb4150bf9221569e1912eb5bc
+-r--r--r--   0 dengyifan   (501) staff       (20)    42257 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.663379 lazyinit-0.0.27/.git/objects/0a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2023 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.664161 lazyinit-0.0.27/.git/objects/0e/
+-r--r--r--   0 dengyifan   (501) staff       (20)      261 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/0e/24281e6a23a799bba50234909a4eefc062407f
+-r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/0e/3fb35ffbadaf084a2915cfc29e9f63d8dc0b80
+-r--r--r--   0 dengyifan   (501) staff       (20)     2330 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.664457 lazyinit-0.0.27/.git/objects/11/
+-r--r--r--   0 dengyifan   (501) staff       (20)      119 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/11/f13a31edccde503893c6083b99d6243e26f111
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.664670 lazyinit-0.0.27/.git/objects/14/
+-r--r--r--   0 dengyifan   (501) staff       (20)      146 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/14/2068ef3450523a0e5f073bd62eec3746405639
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.665038 lazyinit-0.0.27/.git/objects/1c/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1604 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.665346 lazyinit-0.0.27/.git/objects/1f/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/1f/bc66f0cf2ebf60d3c3d235e0e619a1f6622dbe
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.665935 lazyinit-0.0.27/.git/objects/22/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 14:00:51.000000 lazyinit-0.0.27/.git/objects/22/1b9304fb057784a1c767bdf222a4fd449db92f
+-r--r--r--   0 dengyifan   (501) staff       (20)      283 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/22/28de42f4fd7fd7e337c26be6c47fa320f3555f
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.666155 lazyinit-0.0.27/.git/objects/24/
+-r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/24/0d08419d20e2d7cb6985f76926f93b83a8daa7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.666495 lazyinit-0.0.27/.git/objects/28/
+-r--r--r--   0 dengyifan   (501) staff       (20)      358 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/28/5445a221c929c5f5f87e202f37320844e8f6d0
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.667034 lazyinit-0.0.27/.git/objects/2a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1878 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.667374 lazyinit-0.0.27/.git/objects/2b/
+-r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/2b/c85ce5ce789ef99ce23645128dcbaad1ff3835
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.667729 lazyinit-0.0.27/.git/objects/2d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      372 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/2d/d1db85bd19ef19b8f7730625f1740902a4f846
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.668077 lazyinit-0.0.27/.git/objects/2e/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.668654 lazyinit-0.0.27/.git/objects/32/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/32/025d715d168680f84c440a9eaa445bcfe82201
+-r--r--r--   0 dengyifan   (501) staff       (20)     2217 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.668975 lazyinit-0.0.27/.git/objects/33/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 14:00:51.000000 lazyinit-0.0.27/.git/objects/33/1de14f34212468dbd7962fcd3aa2c27159be15
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.669298 lazyinit-0.0.27/.git/objects/38/
+-r--r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/38/d0b85fd4bdd1685656cd6027825010486286ab
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.671372 lazyinit-0.0.27/.git/objects/39/
+-r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/39/c27ee30de9577fb056d6adf1a75b5040624f1a
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:41:16.000000 lazyinit-0.0.27/.git/objects/39/df26c768c14049a07f62ddef6c9d8fe3635b43
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.671966 lazyinit-0.0.27/.git/objects/3d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/3d/5d200d32889f9867e73ddd61f8de5d54006cca
+-r--r--r--   0 dengyifan   (501) staff       (20)     1867 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.672204 lazyinit-0.0.27/.git/objects/40/
+-r--r--r--   0 dengyifan   (501) staff       (20)      513 2023-07-25 11:41:16.000000 lazyinit-0.0.27/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.674376 lazyinit-0.0.27/.git/objects/41/
+-r--r--r--   0 dengyifan   (501) staff       (20)      189 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/41/483d9c24d49b463a3afea6c339c9444c92f01d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.675423 lazyinit-0.0.27/.git/objects/43/
+-r--r--r--   0 dengyifan   (501) staff       (20)      291 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/43/3b5b7262dcbe0429a0a8e7ed7aee7ed4793ed4
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.679494 lazyinit-0.0.27/.git/objects/4d/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1995 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.679870 lazyinit-0.0.27/.git/objects/52/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2033 2023-07-25 11:41:16.000000 lazyinit-0.0.27/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.683917 lazyinit-0.0.27/.git/objects/55/
+-r--r--r--   0 dengyifan   (501) staff       (20)      145 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/55/3ee9d39a64d1c55b084c4821a83d6574cee6da
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.684280 lazyinit-0.0.27/.git/objects/56/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3553 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.684525 lazyinit-0.0.27/.git/objects/5a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1979 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.685339 lazyinit-0.0.27/.git/objects/5e/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1486 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.687164 lazyinit-0.0.27/.git/objects/5f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      125 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/5f/21b1e6c2be3514a4d5118cd8db61899648080a
+-r--r--r--   0 dengyifan   (501) staff       (20)      549 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.689767 lazyinit-0.0.27/.git/objects/60/
+-r--r--r--   0 dengyifan   (501) staff       (20)      514 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/60/41ee332e98835ce7e3ed8b3ae41f91352bec33
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.690559 lazyinit-0.0.27/.git/objects/63/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/63/29d30bc981284e510de0c1938ade4c16e7bde9
+-r--r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/63/3cf9d6946c15485dcb3cf3889f6b34de0c0bcd
+-r--r--r--   0 dengyifan   (501) staff       (20)     2007 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.695061 lazyinit-0.0.27/.git/objects/64/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2420 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.695832 lazyinit-0.0.27/.git/objects/67/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/67/bf3997c2bc19d4034bd741ab9808c86b52376b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.696122 lazyinit-0.0.27/.git/objects/69/
+-r--r--r--   0 dengyifan   (501) staff       (20)      930 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.696572 lazyinit-0.0.27/.git/objects/6a/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1554 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.696892 lazyinit-0.0.27/.git/objects/6b/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2003 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.697393 lazyinit-0.0.27/.git/objects/6c/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1966 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66
+-r--r--r--   0 dengyifan   (501) staff       (20)      233 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/6c/f23ede6f0221263856d80f2287298ce360df0d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.697594 lazyinit-0.0.27/.git/objects/6d/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/6d/8911d55f9896b814e9db65f2edc1da1524c03b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.697877 lazyinit-0.0.27/.git/objects/6e/
+-r--r--r--   0 dengyifan   (501) staff       (20)       37 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/6e/30ca1116ed7b5e804a19fc761a7a2d58c0e1dd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.698630 lazyinit-0.0.27/.git/objects/6f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      496 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/6f/9a4b893df9fff8b3995e4014388ba30f129cd2
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/6f/cdcf4e30a9697c1f5aceaf1dc7d39d98739f51
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.698908 lazyinit-0.0.27/.git/objects/73/
+-r--r--r--   0 dengyifan   (501) staff       (20)       91 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/73/58417a5d41c0ae3f227f79be64cff1341921f3
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.701500 lazyinit-0.0.27/.git/objects/74/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/74/453505ab7b002053a991e77614b41494aefd94
+-r--r--r--   0 dengyifan   (501) staff       (20)      180 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/74/94617eb236a96a42041354b497fb373ff69e2a
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/74/e45b20bcfa13204500b46f9b3f794a2eedd610
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.702074 lazyinit-0.0.27/.git/objects/7e/
+-r--r--r--   0 dengyifan   (501) staff       (20)      499 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/7e/cdeefbee966a2c48b1f3e93aef8772a83a927b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.705056 lazyinit-0.0.27/.git/objects/7f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/7f/3aff99db09db5b9be0eb49dfbb83e5a2b2dfe6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.705283 lazyinit-0.0.27/.git/objects/80/
+-r--r--r--   0 dengyifan   (501) staff       (20)      561 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.705799 lazyinit-0.0.27/.git/objects/83/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:41:16.000000 lazyinit-0.0.27/.git/objects/83/410ee7dbb23a43716f77560dfb52b6dbab167b
+-r--r--r--   0 dengyifan   (501) staff       (20)     7437 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.706085 lazyinit-0.0.27/.git/objects/84/
+-r--r--r--   0 dengyifan   (501) staff       (20)      281 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/84/32f5170b60379a5440d18af5c42da0c20bab36
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.706481 lazyinit-0.0.27/.git/objects/86/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/objects/86/305819935ba7c71d91c90bb164a58e855e7d1e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.706786 lazyinit-0.0.27/.git/objects/87/
+-r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.707142 lazyinit-0.0.27/.git/objects/88/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3155 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.707335 lazyinit-0.0.27/.git/objects/89/
+-r--r--r--   0 dengyifan   (501) staff       (20)       34 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/89/fe87522f1d1d21fb72f29e4a3f3044b32cc64c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.707536 lazyinit-0.0.27/.git/objects/8b/
+-r--r--r--   0 dengyifan   (501) staff       (20)      188 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/objects/8b/538f3380f85f22fc479f2298de08af638d91f6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.707731 lazyinit-0.0.27/.git/objects/8f/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/8f/821694556aac2a278c288de223659193dd2489
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.707919 lazyinit-0.0.27/.git/objects/91/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2328 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.708276 lazyinit-0.0.27/.git/objects/96/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3726 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/96/7c51d6a0690049febfd310c0257eb795caeaef
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.708449 lazyinit-0.0.27/.git/objects/99/
+-r--r--r--   0 dengyifan   (501) staff       (20)       95 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/99/aee23747e74ecbb3e8ebdc64b65c85c55f51dd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.709226 lazyinit-0.0.27/.git/objects/9c/
+-r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef
+-r--r--r--   0 dengyifan   (501) staff       (20)      186 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/9c/fa0e1bf241048b8a143c7fef01067d5f9c3ac7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.709688 lazyinit-0.0.27/.git/objects/9d/
+-r--r--r--   0 dengyifan   (501) staff       (20)      150 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/9d/1f61df1650e8ae0165c5d3e1f47e8384a76e25
+-r--r--r--   0 dengyifan   (501) staff       (20)     2983 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.710409 lazyinit-0.0.27/.git/objects/a0/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/a0/2c8ecffe863e22a9a7510d5af5f8472da012c4
+-r--r--r--   0 dengyifan   (501) staff       (20)      494 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/a0/8ceea5fa60b6a189bf2ca3e11a3e82d84375ea
+-r--r--r--   0 dengyifan   (501) staff       (20)     1903 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.710852 lazyinit-0.0.27/.git/objects/a1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/a1/e2f9a9114e1b772f7fb22f7c2a26fc8fcf25ac
+-r--r--r--   0 dengyifan   (501) staff       (20)     2165 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.711120 lazyinit-0.0.27/.git/objects/a3/
+-r--r--r--   0 dengyifan   (501) staff       (20)      555 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.711562 lazyinit-0.0.27/.git/objects/a8/
+-r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/a8/8453b2586a082782d165b46444353c6fda84f5
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.711838 lazyinit-0.0.27/.git/objects/a9/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1465 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.712541 lazyinit-0.0.27/.git/objects/aa/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/aa/2f814ba87b54003ea2facaf8a8ac437b174212
+-r--r--r--   0 dengyifan   (501) staff       (20)      920 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487
+-r--r--r--   0 dengyifan   (501) staff       (20)     1811 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.712822 lazyinit-0.0.27/.git/objects/ad/
+-r--r--r--   0 dengyifan   (501) staff       (20)     3750 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.713312 lazyinit-0.0.27/.git/objects/ae/
+-r--r--r--   0 dengyifan   (501) staff       (20)       92 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/ae/99dcc87c6ca438bd127b06eee3ccc47f4ffd6c
+-r--r--r--   0 dengyifan   (501) staff       (20)      215 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/ae/ca62bc1646058816f9a5bddd5681d0fb939b24
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.713889 lazyinit-0.0.27/.git/objects/af/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/af/272c05462dae29b6aadb455022bdbbf9f531e7
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/af/38c03c42f711bbfe4db00e49e92fb5761c80d7
+-r--r--r--   0 dengyifan   (501) staff       (20)     1602 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.714429 lazyinit-0.0.27/.git/objects/b0/
+-r--r--r--   0 dengyifan   (501) staff       (20)     4121 2023-07-26 05:00:09.000000 lazyinit-0.0.27/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/b0/8c7ef81a8076086a4529e40583d52ff2e03d24
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.714654 lazyinit-0.0.27/.git/objects/b1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      729 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.714852 lazyinit-0.0.27/.git/objects/b4/
+-r--r--r--   0 dengyifan   (501) staff       (20)      124 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/b4/31ec69865aa69f6bbac9893d5f3266ecd13273
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.715454 lazyinit-0.0.27/.git/objects/b6/
+-r--r--r--   0 dengyifan   (501) staff       (20)      218 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/b6/9f632da541ff48fd18a636d74fca4d80935113
+-r--r--r--   0 dengyifan   (501) staff       (20)       20 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/b6/fc4c620b67d95f953a5c1c1230aaab5db5a1b0
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.715703 lazyinit-0.0.27/.git/objects/b7/
+-r--r--r--   0 dengyifan   (501) staff       (20)      500 2023-07-25 11:16:46.000000 lazyinit-0.0.27/.git/objects/b7/8ccba97db82f1ca4c6db7e0b5cd1bd8af07780
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.715905 lazyinit-0.0.27/.git/objects/bb/
+-r--r--r--   0 dengyifan   (501) staff       (20)       31 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/bb/b84aa70c64fb0114dfa2f1df1cfffbc0123de9
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.717916 lazyinit-0.0.27/.git/objects/bc/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/bc/771507d6ab55b2ca55d1b567dc38064561aa6f
+-r--r--r--   0 dengyifan   (501) staff       (20)      552 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01
+-r--r--r--   0 dengyifan   (501) staff       (20)     2346 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385
+-r--r--r--   0 dengyifan   (501) staff       (20)      148 2023-07-25 11:41:16.000000 lazyinit-0.0.27/.git/objects/bc/e5df5b3fb9303de75d9ba662475c2e0940387e
+-r--r--r--   0 dengyifan   (501) staff       (20)      200 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/bc/ed2eb0d31276a7b1ddfe5855190dc53fec2a91
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.718304 lazyinit-0.0.27/.git/objects/c1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/c1/b6c43ce95f33b1c96bb259fd2c2facd4406ef8
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.718629 lazyinit-0.0.27/.git/objects/c4/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2032 2023-07-25 11:33:45.000000 lazyinit-0.0.27/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.719218 lazyinit-0.0.27/.git/objects/c5/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/c5/4ad76a5bccb99831a7a16f98637da3903c2cec
+-r--r--r--   0 dengyifan   (501) staff       (20)      450 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/c5/f23c1c12745e22b14c79b57d397ae6685cf564
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.719398 lazyinit-0.0.27/.git/objects/c7/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1654 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.719594 lazyinit-0.0.27/.git/objects/c9/
+-r--r--r--   0 dengyifan   (501) staff       (20)      547 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.719929 lazyinit-0.0.27/.git/objects/ca/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1263 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.720567 lazyinit-0.0.27/.git/objects/cc/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/cc/3a12d725fdd1884f2f104e1c11d8b87c1367cc
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/cc/46e850693cec9659b52d57dd78d6f60c242ebb
+-r--r--r--   0 dengyifan   (501) staff       (20)      716 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.721044 lazyinit-0.0.27/.git/objects/cd/
+-r--r--r--   0 dengyifan   (501) staff       (20)     5189 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591
+-r--r--r--   0 dengyifan   (501) staff       (20)      518 2023-07-26 06:54:32.000000 lazyinit-0.0.27/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.721183 lazyinit-0.0.27/.git/objects/ce/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/ce/3694e653f842cc70a8c5ef32cd9f75639bb14a
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.721362 lazyinit-0.0.27/.git/objects/d9/
+-r--r--r--   0 dengyifan   (501) staff       (20)     5194 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.721625 lazyinit-0.0.27/.git/objects/da/
+-r--r--r--   0 dengyifan   (501) staff       (20)      491 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/da/9fd18a499c0821bea6c2313d252a1d4bcf5846
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.721886 lazyinit-0.0.27/.git/objects/de/
+-r--r--r--   0 dengyifan   (501) staff       (20)      100 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/de/8f446f94a50f937fed1c254a966f3ed6088e81
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.722116 lazyinit-0.0.27/.git/objects/df/
+-r--r--r--   0 dengyifan   (501) staff       (20)     1977 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.722304 lazyinit-0.0.27/.git/objects/e4/
+-r--r--r--   0 dengyifan   (501) staff       (20)      149 2023-07-25 14:00:51.000000 lazyinit-0.0.27/.git/objects/e4/632035cac16d026cc02de90ae31aef87867116
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.722564 lazyinit-0.0.27/.git/objects/e6/
+-r--r--r--   0 dengyifan   (501) staff       (20)       15 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.722956 lazyinit-0.0.27/.git/objects/e8/
+-r--r--r--   0 dengyifan   (501) staff       (20)      556 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b
+-r--r--r--   0 dengyifan   (501) staff       (20)     1289 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.723417 lazyinit-0.0.27/.git/objects/eb/
+-r--r--r--   0 dengyifan   (501) staff       (20)       94 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/eb/758cdc0fe911d913b208b48ee0ac14886927eb
+-r--r--r--   0 dengyifan   (501) staff       (20)      566 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.723620 lazyinit-0.0.27/.git/objects/ec/
+-r--r--r--   0 dengyifan   (501) staff       (20)      290 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/ec/47fd64ca8d46a3a1c345708cf6dd4b19e2d7a6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.723884 lazyinit-0.0.27/.git/objects/ef/
+-r--r--r--   0 dengyifan   (501) staff       (20)      219 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/ef/0a2b00e7e0280dfe13a94d5abfeeba9aafabae
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.724354 lazyinit-0.0.27/.git/objects/f0/
+-r--r--r--   0 dengyifan   (501) staff       (20)     8516 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c
+-r--r--r--   0 dengyifan   (501) staff       (20)      433 2023-07-24 06:27:07.000000 lazyinit-0.0.27/.git/objects/f0/b6b75cf9a30d91dab0d80449c7c76a0191d8a7
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.724563 lazyinit-0.0.27/.git/objects/f1/
+-r--r--r--   0 dengyifan   (501) staff       (20)      559 2023-07-26 04:07:28.000000 lazyinit-0.0.27/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.724760 lazyinit-0.0.27/.git/objects/f2/
+-r--r--r--   0 dengyifan   (501) staff       (20)      321 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/f2/f3ccb260633b09276ccaaa358ce7df1a0025f6
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.724965 lazyinit-0.0.27/.git/objects/f5/
+-r--r--r--   0 dengyifan   (501) staff       (20)      187 2023-07-24 14:32:29.000000 lazyinit-0.0.27/.git/objects/f5/96444b272664dff576dc8ac874152f461a4f6e
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.725160 lazyinit-0.0.27/.git/objects/f6/
+-r--r--r--   0 dengyifan   (501) staff       (20)     2002 2023-07-26 03:36:35.000000 lazyinit-0.0.27/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.653492 lazyinit-0.0.27/.git/refs/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.725360 lazyinit-0.0.27/.git/refs/heads/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 15:01:28.000000 lazyinit-0.0.27/.git/refs/heads/master
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.653560 lazyinit-0.0.27/.git/refs/remotes/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.725997 lazyinit-0.0.27/.git/refs/remotes/origin/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       32 2023-07-27 10:59:16.000000 lazyinit-0.0.27/.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 dengyifan   (501) staff       (20)       41 2023-07-26 08:16:23.000000 lazyinit-0.0.27/.git/refs/remotes/origin/master
+-rw-r--r--   0 dengyifan   (501) staff       (20)       17 2023-07-26 05:01:41.000000 lazyinit-0.0.27/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-27 11:55:42.740970 lazyinit-0.0.27/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.27/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.727707 lazyinit-0.0.27/lazyinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.27/lazyinit/__init__.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.731268 lazyinit-0.0.27/lazyinit/__pycache__/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     8725 2023-07-26 04:15:42.000000 lazyinit-0.0.27/lazyinit/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3763 2023-07-25 04:13:11.000000 lazyinit-0.0.27/lazyinit/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.27/lazyinit/bash_config.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     8781 2023-07-27 11:55:34.000000 lazyinit-0.0.27/lazyinit/init.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.732083 lazyinit-0.0.27/lazyinit/lazydl/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        5 2023-07-23 08:07:15.000000 lazyinit-0.0.27/lazyinit/lazydl/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.732198 lazyinit-0.0.27/lazyinit/lazydl/configs/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1569 2023-07-25 13:48:22.000000 lazyinit-0.0.27/lazyinit/lazydl/configs/default_config.yaml
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.732335 lazyinit-0.0.27/lazyinit/lazydl/configs/exps/
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.732612 lazyinit-0.0.27/lazyinit/lazydl/configs/exps/focusl/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3903 2023-07-25 13:51:05.000000 lazyinit-0.0.27/lazyinit/lazydl/configs/exps/focusl/baseline.yaml
+-rw-r--r--   0 dengyifan   (501) staff       (20)    74072 2023-07-25 04:24:11.000000 lazyinit-0.0.27/lazyinit/lazydl/configs/exps/focusl/exp_plan.yaml
+-rw-r--r--   0 dengyifan   (501) staff       (20)      644 2023-07-23 08:07:15.000000 lazyinit-0.0.27/lazyinit/lazydl/configs/exps/overfit_test.yaml
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1179 2023-07-23 08:16:18.000000 lazyinit-0.0.27/lazyinit/lazydl/minist.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)       16 2023-07-23 08:07:15.000000 lazyinit-0.0.27/lazyinit/lazydl/requirements.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     2727 2023-07-23 08:07:15.000000 lazyinit-0.0.27/lazyinit/lazydl/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-24 14:38:46.000000 lazyinit-0.0.27/lazyinit/lazydl/start.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.734697 lazyinit-0.0.27/lazyinit/ranger/
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6148 2023-07-24 04:18:46.000000 lazyinit-0.0.27/lazyinit/ranger/.DS_Store
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)       23 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.737118 lazyinit-0.0.27/lazyinit/ranger/colorschemes/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/__init__.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      139 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/__init__.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     5769 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/default.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      696 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/jungle.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1171 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/snow.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1335 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/snow.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4929 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/colorschemes/zenburn.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     4758 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/commands.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.740667 lazyinit-0.0.27/lazyinit/ranger/plugins/
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/__init__.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      134 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/__init__.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    10718 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/devicons.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     6817 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/devicons.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)      479 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/devicons_linemode.py
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)     1271 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/plugins/devicons_linemode.pyo
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    23026 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/rc-sample.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    18894 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/rc.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    13012 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/rifle.conf
+-rwxr-xr-x   0 dengyifan   (501) staff       (20)    10000 2023-07-23 10:15:36.000000 lazyinit-0.0.27/lazyinit/ranger/scope.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.27/lazyinit/redis.conf
+-rw-r--r--   0 dengyifan   (501) staff       (20)      142 2023-07-27 04:35:53.000000 lazyinit-0.0.27/lazyinit/redis.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.27/lazyinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     6724 2023-07-27 11:48:11.000000 lazyinit-0.0.27/lazyinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-27 11:55:42.728692 lazyinit-0.0.27/lazyinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)    10070 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-27 11:55:42.000000 lazyinit-0.0.27/lazyinit.egg-info/top_level.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     1059 2023-07-23 12:54:16.000000 lazyinit-0.0.27/push.sh
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-27 11:55:42.741397 lazyinit-0.0.27/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      842 2023-07-27 11:55:39.000000 lazyinit-0.0.27/setup.py
```

### Comparing `lazyinit-0.0.269/.git/hooks/commit-msg.sample` & `lazyinit-0.0.27/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/hooks/fsmonitor-watchman.sample` & `lazyinit-0.0.27/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/hooks/pre-commit.sample` & `lazyinit-0.0.27/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/hooks/pre-push.sample` & `lazyinit-0.0.27/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/hooks/pre-rebase.sample` & `lazyinit-0.0.27/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/hooks/pre-receive.sample` & `lazyinit-0.0.27/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/hooks/prepare-commit-msg.sample` & `lazyinit-0.0.27/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/hooks/push-to-checkout.sample` & `lazyinit-0.0.27/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/hooks/update.sample` & `lazyinit-0.0.27/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/index` & `lazyinit-0.0.27/.git/index`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/logs/HEAD` & `lazyinit-0.0.27/.git/logs/HEAD`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/logs/refs/heads/master` & `lazyinit-0.0.27/.git/logs/refs/heads/master`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/logs/refs/remotes/origin/HEAD` & `lazyinit-0.0.27/.git/logs/refs/remotes/origin/HEAD`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/logs/refs/remotes/origin/master` & `lazyinit-0.0.27/.git/logs/refs/remotes/origin/master`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063` & `lazyinit-0.0.27/.git/objects/04/11b566ad4fa2d7dedd4026ac3a1aa81583f063`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9` & `lazyinit-0.0.27/.git/objects/04/8be6a509c9c6b3cd9d24bf7d2f04e8614144c9`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6` & `lazyinit-0.0.27/.git/objects/05/77692fdce48e2fd5c28dac0eacda2b48e87ca6`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead` & `lazyinit-0.0.27/.git/objects/0a/1bedc205741de440716866d33eb08b3e235ead`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d` & `lazyinit-0.0.27/.git/objects/0e/81dec5c311e0f1902b5a7476df00bf787b727d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae` & `lazyinit-0.0.27/.git/objects/1c/e230b6808423cf4b0db73fb340179061b087ae`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8` & `lazyinit-0.0.27/.git/objects/2a/96e537977cabee3e2b16068d4f9545000293b8`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34` & `lazyinit-0.0.27/.git/objects/2e/71bed4b04a4925d6e78012550fe22e26d08d34`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d` & `lazyinit-0.0.27/.git/objects/32/64c7079a7e0e39163475d2b4339003af04567d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3` & `lazyinit-0.0.27/.git/objects/3d/d722a456d2ec2295cbf0436b4b61c6c8c6b7c3`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7` & `lazyinit-0.0.27/.git/objects/40/59878eb4d85e7b6ef8fb04380bf6f9751584f7`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3` & `lazyinit-0.0.27/.git/objects/4d/2762b9e252de867acaf16b66114670aa11ecf3`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9` & `lazyinit-0.0.27/.git/objects/52/79a58bbcde1a77c583e479624d77ce6f2724b9`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd` & `lazyinit-0.0.27/.git/objects/56/e79ee804723417ab49741dd9472801b7299dcd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd` & `lazyinit-0.0.27/.git/objects/5a/2bc98288d465b99beaf4a0a140f0bdd41bc2cd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb` & `lazyinit-0.0.27/.git/objects/5e/8c24228a2bef23ae72b7be7ed156bf0042c8bb`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d` & `lazyinit-0.0.27/.git/objects/5f/9cbd2428e9c98934938c6677d49d4c9563df8d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1` & `lazyinit-0.0.27/.git/objects/60/34a9d5202ceac21a60ba1d870e3462bc3148a1`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b` & `lazyinit-0.0.27/.git/objects/63/ec73d50c150c85e2cb8244f2b2b63c8778481b`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f` & `lazyinit-0.0.27/.git/objects/64/df83d0de818da9d27056bdc81e11da87f9769f`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084` & `lazyinit-0.0.27/.git/objects/69/08d6e2eda83cfbe2af88aa30210d3d0dde0084`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4` & `lazyinit-0.0.27/.git/objects/6a/442e346cfff221cc741dbe80333a65d29c47d4`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04` & `lazyinit-0.0.27/.git/objects/6b/0999e44c09719dd1e38661844139175319fd04`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66` & `lazyinit-0.0.27/.git/objects/6c/acc4ed42148a0c6203f77156a07af4bf3f6d66`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86` & `lazyinit-0.0.27/.git/objects/80/08507a6ab8ee925f8ce6499f1abe2063803a86`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25` & `lazyinit-0.0.27/.git/objects/83/e83b22c2a56aa9dccd64d8601eec74aace5e25`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717` & `lazyinit-0.0.27/.git/objects/87/5e7c9d32e4d678ba2fbacb46a4a3de3402a717`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c` & `lazyinit-0.0.27/.git/objects/88/595b84b2702aa90f38deba1c57573443f4b50c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c` & `lazyinit-0.0.27/.git/objects/91/e8d51fd5b9847d77e1e5a8192490129210f85c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0` & `lazyinit-0.0.27/.git/objects/96/2bd45f2b76db40ecdcb6c8f41f964d9a8370e0`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef` & `lazyinit-0.0.27/.git/objects/9c/4a77711ab6e0689e536bcb5a7ef50a35e901ef`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e` & `lazyinit-0.0.27/.git/objects/9d/2c13ee0132c40f8315b78ecae1fd0edc5b427e`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd` & `lazyinit-0.0.27/.git/objects/a0/a81da425228ad48403f92935808a4ba6e05edd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083` & `lazyinit-0.0.27/.git/objects/a1/fccfb7ff71e181820dda3f82c497e8ef889083`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d` & `lazyinit-0.0.27/.git/objects/a3/bb4ffd7db4487e344ef1b2edd61ce07ff1167d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875` & `lazyinit-0.0.27/.git/objects/a8/257b5fea73a8211c7d6b82b7d491b8df413875`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b` & `lazyinit-0.0.27/.git/objects/a9/e01e0ccf1896b7d2cba4d39d6a7803f7b4ca1b`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487` & `lazyinit-0.0.27/.git/objects/aa/4841d8ba88abe35f8e8c996520aece061cd487`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477` & `lazyinit-0.0.27/.git/objects/aa/9285de3d559b18e802b30eec7e6455f777f477`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb` & `lazyinit-0.0.27/.git/objects/ad/54c4be70848f4939b1084f23f8669d9d08c3bb`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76` & `lazyinit-0.0.27/.git/objects/af/489d55fcb3625aab9e50f6488b4cdedb598a76`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45` & `lazyinit-0.0.27/.git/objects/b0/55fb21712baa4ca3586b392ae90537c6321d45`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c` & `lazyinit-0.0.27/.git/objects/b1/e1d5f1ef4985748c8bbbec46079c1d19b1b74c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01` & `lazyinit-0.0.27/.git/objects/bc/8af407bf0ffec0b136323ddfc4e0d51403ab01`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385` & `lazyinit-0.0.27/.git/objects/bc/aca677a552f0350772b01bf0633e91ff944385`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893` & `lazyinit-0.0.27/.git/objects/c4/a02b103bfb4e27b62f70ad0b70572491db9893`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586` & `lazyinit-0.0.27/.git/objects/c7/76bcdeba36a219858ebdaf5eedda8858abd586`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd` & `lazyinit-0.0.27/.git/objects/c9/4f017e905c920d805fe683c4069bb93a79e2fd`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d` & `lazyinit-0.0.27/.git/objects/ca/75f23da09a045e4eb7c3e1661fa44bd5edc17d`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c` & `lazyinit-0.0.27/.git/objects/cc/a0650a948c70a0a2c21edae5c06ef9c602ae6c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591` & `lazyinit-0.0.27/.git/objects/cd/0a5164bca945c0476011d2018a0070fb7c3591`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943` & `lazyinit-0.0.27/.git/objects/cd/bcc32e66dd83857d8aeb37b82b73da160d4943`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac` & `lazyinit-0.0.27/.git/objects/d9/c73c9b6f2db929dc33c91ff796eef14bf3eeac`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463` & `lazyinit-0.0.27/.git/objects/df/42758f2f033f69283d489c1fb5938e30a5d463`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b` & `lazyinit-0.0.27/.git/objects/e8/6d8a11ff224979d193280d3f9fe520bdde649b`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e` & `lazyinit-0.0.27/.git/objects/e8/bba2b5885562e3daa84849403890e1e0fb227e`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23` & `lazyinit-0.0.27/.git/objects/eb/ba6096a6751eea400adad09d35540db5f30c23`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c` & `lazyinit-0.0.27/.git/objects/f0/7ee5caab32d9cfa53fbfb771cafaf4a290400c`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb` & `lazyinit-0.0.27/.git/objects/f1/65c1685b6d3d791349a8114242da27efb4f7eb`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91` & `lazyinit-0.0.27/.git/objects/f6/058e560b217f1758b28ed292ec8e71419aff91`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/__pycache__/utils.cpython-311.pyc` & `lazyinit-0.0.27/lazyinit/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/__pycache__/utils.cpython-38.pyc` & `lazyinit-0.0.27/lazyinit/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/bash_config.txt` & `lazyinit-0.0.27/lazyinit/bash_config.txt`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/init.py` & `lazyinit-0.0.27/lazyinit/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             echo("请在 bash 环境下运行本工具！")
         echo("您可以通过以下命令查看所支持的 Shell 类型：\ncat /etc/shells", "red")
         echo("您可以通过以下命令切换 Shell 类型：\nchsh -s /bin/bash", "red")
         exit()
 
     pkg_current_path = os.path.dirname(os.path.abspath(__file__))
     python_version = "3.9"
-    env_name = "zhei"
+    env_name = "lazydl"
 
     # 读取 ~/.bashrc 文件内容
     if not os.path.exists("~/.bashrc"):
         run_cmd("touch ~/.bashrc", show_cmd=False)
     bashrc = run_cmd("cat ~/.bashrc", show_cmd=False)
-    if "zhei-init" not in bashrc:
-        print("未找到 zhei-init 配置，即将注入配置到 ~/.bashrc（完成后可能需要重启初始化工具）")
+    if "lazydl-init" not in bashrc:
+        print("未找到 lazydl-init 配置，即将注入配置到 ~/.bashrc（完成后可能需要重启初始化工具）")
         # ---------------------------------------------------------------------------- #
         #                         配置 Bash 环境变量                                     
         # ---------------------------------------------------------------------------- #
         bash = [
             "cd ~/",
             "cat {}/bash_config.txt >> ~/.bashrc".format(pkg_current_path),
         ]
@@ -43,15 +43,15 @@
     echo("     | |  | (_) \\ V  V /  __/ | | (_| |    | |_) | |_| |    | |__| |")
     echo("     |_|   \\___/ \\_/\\_/ \\___|_|  \\__,_|    |____/ \\__, |     \\____/")
     echo("                                                   __/ |")
     echo("                                                  |___/")
     echo("")
     echo("")
     echo("")
-    echo("             欢迎使用服务器环境初始化工具 zhei-init ！", "green")
+    echo("             欢迎使用服务器环境初始化工具 lazydl-init ！", "green")
     echo("")
     echo("   本工具将会帮助您初始化服务器环境，下面是功能菜单，可输入序号进行配置", "green")
 
     step = "-1"
     while step != "0":
         if step != "-1":
             echo("\n是否继续配置？（y/n）", "yellow")
@@ -61,15 +61,15 @@
         echo(" ", "blue")
         echo("1、设置 pip 源", "blue") 
         echo("2、安装 MiniConda", "blue")
         echo("3、安装 ranger 并自动配置", "blue")
         echo("4、创建 Conda  Pytorch 环境", "blue")
         echo("5、安装 Redis", "blue")
         echo("6、生成公钥", "blue")
-        echo("7、生成 zhei 项目模板", "blue")
+        echo("7、生成 lazydl 项目模板", "blue")
         echo("0、退出", "blue")
         echo(" ", "blue")
         echo("请在下方输入操作序号：", "yellow")
         step = input()
         if step == "1":
             # ---------------------------------------------------------------------------- #
             #                         设置 pip 源                                     
@@ -100,32 +100,34 @@
                 "python -m pip install ranger-fm",
                 "mv {}/ranger ~/.config/".format(pkg_current_path),
             ]
             run_cmd(ranger)
 
         elif step == "4":
             # ---------------------------------------------------------------------------- #
-            #                         创建 zhei 环境                                     
+            #                         创建 lazydl 环境                                     
             # ---------------------------------------------------------------------------- #
-            echo("即将创建 zhei 环境，请在下方输入 Python 版本号，默认为 3.9：", "yellow")
+            echo("即将创建 lazydl 环境，请在下方输入 Python 版本号，默认为 3.9：", "yellow")
             python_version = input()
             if python_version == "":
                 python_version = "3.9"
-            echo("即将创建 zhei 环境，请在下方输入环境名称，将会自动安装 zhei 包，默认名称为 zhei：", "yellow")
+            echo("即将创建 lazydl 环境，请在下方输入环境名称，将会自动安装 lazydl 包，默认名称为 lazydl：", "yellow")
             env_name = input()
             if env_name == "":
-                env_name = "zhei"
+                env_name = "lazydl"
             
             run_cmd_inactivate("conda create -n {} python={}".format(env_name, python_version))
             
-            zhei = [
+            echo("即将激活环境并安装依赖，如果是首次激活需要补充 “conda init” 指令哦！")
+            
+            lazydl = [
                 "conda activate {}".format(env_name),
-                "python -m pip install zhei --upgrade",
+                "python -m pip install lazydl --upgrade",
             ]
-            run_cmd(zhei)
+            run_cmd(lazydl)
 
             echo("即将安装 Pytorch，请选择 CUDA 版本号，默认为 11.8：", "yellow")
             cuda_version = input()
             torch_url, torchvision_url, torchaudio_url = show_available_version(cuda_version, python_version)
 
             echo("即将从以下链接安装 torch：\n {}".format(torch_url))
             torch_install = [
@@ -142,22 +144,23 @@
             echo("即将从以下链接安装 torchaudio：\n {}".format(torchaudio_url))
             torchaudio_install = [
                 "python -m pip install {}".format(torchaudio_url),
             ]   
             run_cmd(torchaudio_install)
 
         elif step == "5":
+            echo("安装 Redis 时间可能较长（大约五分钟），请耐心等待！")
             run_cmd([
                 "sh {}/redis.sh".format(pkg_current_path),
                 "cp {}/redis.conf ~/redis/bin/".format(pkg_current_path),
                 "~/redis/bin/redis-server ~/redis/bin/redis.conf",
             ])
             
         elif step == "6":
-            run_cmd([
+            run_cmd_inactivate([
                 "cd ~/.ssh",
                 "ssh-keygen -t rsa",
                 "cat id_rsa.pub"
             ])
             
         elif step == "7":
             echo("请在下方输入 “项目路径 项目文件夹名称”， 默认为 “./ lazydl” ：", "yellow")
```

### Comparing `lazyinit-0.0.269/lazyinit/lazydl/configs/default_config.yaml` & `lazyinit-0.0.27/lazyinit/lazydl/configs/default_config.yaml`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/lazydl/configs/exps/focusl/baseline.yaml` & `lazyinit-0.0.27/lazyinit/lazydl/configs/exps/focusl/baseline.yaml`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/lazydl/configs/exps/focusl/exp_plan.yaml` & `lazyinit-0.0.27/lazyinit/lazydl/configs/exps/focusl/exp_plan.yaml`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/lazydl/configs/exps/overfit_test.yaml` & `lazyinit-0.0.27/lazyinit/lazydl/configs/exps/overfit_test.yaml`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/lazydl/minist.py` & `lazyinit-0.0.27/lazyinit/lazydl/minist.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/lazydl/run.py` & `lazyinit-0.0.27/lazyinit/lazydl/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/.DS_Store` & `lazyinit-0.0.27/lazyinit/ranger/.DS_Store`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/colorschemes/default.py` & `lazyinit-0.0.27/lazyinit/ranger/colorschemes/default.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/colorschemes/jungle.py` & `lazyinit-0.0.27/lazyinit/ranger/colorschemes/jungle.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/colorschemes/snow.py` & `lazyinit-0.0.27/lazyinit/ranger/colorschemes/snow.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/colorschemes/snow.pyo` & `lazyinit-0.0.27/lazyinit/ranger/colorschemes/snow.pyo`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/colorschemes/zenburn.py` & `lazyinit-0.0.27/lazyinit/ranger/colorschemes/zenburn.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/commands.py` & `lazyinit-0.0.27/lazyinit/ranger/commands.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/plugins/devicons.py` & `lazyinit-0.0.27/lazyinit/ranger/plugins/devicons.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/plugins/devicons.pyo` & `lazyinit-0.0.27/lazyinit/ranger/plugins/devicons.pyo`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/plugins/devicons_linemode.pyo` & `lazyinit-0.0.27/lazyinit/ranger/plugins/devicons_linemode.pyo`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/rc-sample.conf` & `lazyinit-0.0.27/lazyinit/ranger/rc-sample.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/rc.conf` & `lazyinit-0.0.27/lazyinit/ranger/rc.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/rifle.conf` & `lazyinit-0.0.27/lazyinit/ranger/rifle.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/ranger/scope.sh` & `lazyinit-0.0.27/lazyinit/ranger/scope.sh`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/redis.conf` & `lazyinit-0.0.27/lazyinit/redis.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/run.py` & `lazyinit-0.0.27/lazyinit/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/lazyinit/utils.py` & `lazyinit-0.0.27/lazyinit/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,34 +22,34 @@
 def echo(msg, color="green"):
     console.print(msg, style=color)
     
 
 def run_cmd_inactivate(cmd_list):
     if isinstance(cmd_list, str):
         cmd = cmd_list
-        print("\n" + cmd, "blue")
+        print("\n" + cmd)
         while True:
             exitcode = os.system(cmd)
             if exitcode != 0:
                 echo("执行 {} 失败！".format(cmd), "#FF6AB3")
-                echo("可通过在下方修改命令继续执行，或者直接按下回车键忽略该错误：")
+                echo("可通过在下方修改命令继续执行，或者直接按下回车键结束操作：")
                 cmd = input()
                 if cmd == "":   
-                    break
+                    return exitcode
             else:
-                break
+                return exitcode
             
     outputs = []
-    for cmd in track(cmd_list, description="命令执行中...", transient=True):
+    for cmd in track(cmd_list, description="命令执行中", transient=True):
         print("\n" + cmd)
         while True:
             exitcode = os.system(cmd)
             if exitcode != 0:
                 echo("执行 {} 失败！".format(cmd), "#FF6AB3")
-                echo("可通过在下方修改命令继续执行，或者直接按下回车键忽略该错误：")
+                echo("可通过在下方修改命令继续执行，或者直接按下回车键结束操作：")
                 cmd = input()
                 if cmd == "":
                     break
             else:
                 break
 
     return outputs   
@@ -61,31 +61,31 @@
         if show_cmd:
             print("\n" + cmd)
         while True:
             exitcode, output = subprocess.getstatusoutput(cmd)
             if exitcode != 0:
                 echo("执行 {} 失败！".format(cmd), "#FF6AB3")
                 echo("错误信息：\n{}".format(output))
-                echo("可通过在下方修改命令继续执行，或者直接按下回车键忽略该错误：")
+                echo("可通过在下方修改命令继续执行，或者直接按下回车键结束操作：")
                 cmd = input()
                 if cmd == "":
                     return output
             else:
                 return output
             
     outputs = []
-    for cmd in track(cmd_list, description="命令执行中...", transient=True):
+    for cmd in track(cmd_list, description="命令执行中", transient=True):
         if show_cmd:
             print("\n" + cmd)
         while True:
             exitcode, output = subprocess.getstatusoutput(cmd)
             if exitcode != 0:
                 echo("执行 {} 失败！".format(cmd), "#FF6AB3")
                 echo("错误信息：\n{}".format(output))
-                echo("可通过在下方修改命令继续执行，或者直接按下回车键忽略该错误：")
+                echo("可通过在下方修改命令继续执行，或者直接按下回车键结束操作：")
                 cmd = input()
                 if cmd == "":
                     outputs.append(output)
                     break
             else:
                 outputs.append(output)
                 break
```

### Comparing `lazyinit-0.0.269/lazyinit.egg-info/SOURCES.txt` & `lazyinit-0.0.27/lazyinit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
 push.sh
 setup.py
-z.py
 .git/COMMIT_EDITMSG
 .git/FETCH_HEAD
 .git/HEAD
 .git/ORIG_HEAD
 .git/config
 .git/description
 .git/index
```

### Comparing `lazyinit-0.0.269/push.sh` & `lazyinit-0.0.27/push.sh`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.269/setup.py` & `lazyinit-0.0.27/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='lazyinit',
-    version='0.0.269',
+    version='0.0.27',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init zhei environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

