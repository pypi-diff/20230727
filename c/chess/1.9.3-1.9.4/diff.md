# Comparing `tmp/chess-1.9.3.tar.gz` & `tmp/chess-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess-1.9.3.tar", last modified: Fri Sep 16 12:34:11 2022, max compression
+gzip compressed data, was "chess-1.9.4.tar", last modified: Thu Dec 22 11:32:51 2022, max compression
```

## Comparing `chess-1.9.3.tar` & `chess-1.9.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 niklas    (1000) niklas    (1000)        0 2022-09-16 12:34:11.008938 chess-1.9.3/
--rw-r--r--   0 niklas    (1000) niklas    (1000)     8965 2022-09-16 12:27:44.000000 chess-1.9.3/CHANGELOG.rst
--rw-r--r--   0 niklas    (1000) niklas    (1000)    35147 2017-10-30 20:11:39.000000 chess-1.9.3/LICENSE.txt
--rw-r--r--   0 niklas    (1000) niklas    (1000)       42 2022-05-26 10:51:13.000000 chess-1.9.3/MANIFEST.in
--rw-r--r--   0 niklas    (1000) niklas    (1000)    18363 2022-09-16 12:34:11.008938 chess-1.9.3/PKG-INFO
--rw-r--r--   0 niklas    (1000) niklas    (1000)    17053 2022-09-16 12:07:38.000000 chess-1.9.3/README.rst
-drwxr-xr-x   0 niklas    (1000) niklas    (1000)        0 2022-09-16 12:34:11.008938 chess-1.9.3/chess/
--rw-r--r--   0 niklas    (1000) niklas    (1000)   145065 2022-09-16 12:23:10.000000 chess-1.9.3/chess/__init__.py
--rw-r--r--   0 niklas    (1000) niklas    (1000)     5843 2022-05-26 10:51:13.000000 chess-1.9.3/chess/_interactive.py
--rw-r--r--   0 niklas    (1000) niklas    (1000)   118248 2022-07-22 08:58:27.000000 chess-1.9.3/chess/engine.py
--rw-r--r--   0 niklas    (1000) niklas    (1000)    63004 2022-05-26 10:51:13.000000 chess-1.9.3/chess/gaviota.py
--rw-r--r--   0 niklas    (1000) niklas    (1000)    57846 2022-07-29 06:57:28.000000 chess-1.9.3/chess/pgn.py
--rw-r--r--   0 niklas    (1000) niklas    (1000)    28194 2022-05-26 10:51:13.000000 chess-1.9.3/chess/polyglot.py
--rw-r--r--   0 niklas    (1000) niklas    (1000)        0 2020-10-29 17:30:41.000000 chess-1.9.3/chess/py.typed
--rw-r--r--   0 niklas    (1000) niklas    (1000)    31838 2022-06-16 18:52:38.000000 chess-1.9.3/chess/svg.py
--rw-r--r--   0 niklas    (1000) niklas    (1000)    69661 2022-05-26 10:51:13.000000 chess-1.9.3/chess/syzygy.py
--rw-r--r--   0 niklas    (1000) niklas    (1000)    46056 2022-07-22 09:08:54.000000 chess-1.9.3/chess/variant.py
-drwxr-xr-x   0 niklas    (1000) niklas    (1000)        0 2022-09-16 12:34:11.008938 chess-1.9.3/chess.egg-info/
--rw-r--r--   0 niklas    (1000) niklas    (1000)    18363 2022-09-16 12:34:10.000000 chess-1.9.3/chess.egg-info/PKG-INFO
--rw-r--r--   0 niklas    (1000) niklas    (1000)      366 2022-09-16 12:34:10.000000 chess-1.9.3/chess.egg-info/SOURCES.txt
--rw-r--r--   0 niklas    (1000) niklas    (1000)        1 2022-09-16 12:34:10.000000 chess-1.9.3/chess.egg-info/dependency_links.txt
--rw-r--r--   0 niklas    (1000) niklas    (1000)        1 2020-10-26 07:36:05.000000 chess-1.9.3/chess.egg-info/not-zip-safe
--rw-r--r--   0 niklas    (1000) niklas    (1000)        6 2022-09-16 12:34:10.000000 chess-1.9.3/chess.egg-info/top_level.txt
--rw-r--r--   0 niklas    (1000) niklas    (1000)       38 2022-09-16 12:34:11.008938 chess-1.9.3/setup.cfg
--rwxr-xr-x   0 niklas    (1000) niklas    (1000)     3686 2022-05-26 10:51:13.000000 chess-1.9.3/setup.py
+drwxr-xr-x   0 niklas    (1000) niklas    (1000)        0 2022-12-22 11:32:51.358749 chess-1.9.4/
+-rw-r--r--   0 niklas    (1000) niklas    (1000)     9998 2022-12-22 11:24:07.000000 chess-1.9.4/CHANGELOG.rst
+-rw-r--r--   0 niklas    (1000) niklas    (1000)    35147 2017-07-09 08:11:55.000000 chess-1.9.4/LICENSE.txt
+-rw-r--r--   0 niklas    (1000) niklas    (1000)       42 2021-06-01 14:37:48.000000 chess-1.9.4/MANIFEST.in
+-rw-r--r--   0 niklas    (1000) niklas    (1000)    18724 2022-12-22 11:32:51.358749 chess-1.9.4/PKG-INFO
+-rw-r--r--   0 niklas    (1000) niklas    (1000)    17363 2022-11-27 08:57:46.000000 chess-1.9.4/README.rst
+drwxr-xr-x   0 niklas    (1000) niklas    (1000)        0 2022-12-22 11:32:51.358749 chess-1.9.4/chess/
+-rw-r--r--   0 niklas    (1000) niklas    (1000)   146728 2022-12-22 11:27:15.000000 chess-1.9.4/chess/__init__.py
+-rw-r--r--   0 niklas    (1000) niklas    (1000)     5843 2021-06-01 14:37:48.000000 chess-1.9.4/chess/_interactive.py
+-rw-r--r--   0 niklas    (1000) niklas    (1000)   119042 2022-12-18 16:40:16.000000 chess-1.9.4/chess/engine.py
+-rw-r--r--   0 niklas    (1000) niklas    (1000)    63004 2021-11-07 13:36:40.000000 chess-1.9.4/chess/gaviota.py
+-rw-r--r--   0 niklas    (1000) niklas    (1000)    57846 2022-08-21 09:05:45.000000 chess-1.9.4/chess/pgn.py
+-rw-r--r--   0 niklas    (1000) niklas    (1000)    28194 2021-06-01 14:37:48.000000 chess-1.9.4/chess/polyglot.py
+-rw-r--r--   0 niklas    (1000) niklas    (1000)        0 2021-06-01 14:37:48.000000 chess-1.9.4/chess/py.typed
+-rw-r--r--   0 niklas    (1000) niklas    (1000)    31812 2022-11-27 08:57:46.000000 chess-1.9.4/chess/svg.py
+-rw-r--r--   0 niklas    (1000) niklas    (1000)    69830 2022-11-27 08:57:46.000000 chess-1.9.4/chess/syzygy.py
+-rw-r--r--   0 niklas    (1000) niklas    (1000)    46048 2022-11-27 08:57:46.000000 chess-1.9.4/chess/variant.py
+drwxr-xr-x   0 niklas    (1000) niklas    (1000)        0 2022-12-22 11:32:51.358749 chess-1.9.4/chess.egg-info/
+-rw-r--r--   0 niklas    (1000) niklas    (1000)    18724 2022-12-22 11:32:51.000000 chess-1.9.4/chess.egg-info/PKG-INFO
+-rw-r--r--   0 niklas    (1000) niklas    (1000)      366 2022-12-22 11:32:51.000000 chess-1.9.4/chess.egg-info/SOURCES.txt
+-rw-r--r--   0 niklas    (1000) niklas    (1000)        1 2022-12-22 11:32:51.000000 chess-1.9.4/chess.egg-info/dependency_links.txt
+-rw-r--r--   0 niklas    (1000) niklas    (1000)        1 2020-10-26 10:58:03.000000 chess-1.9.4/chess.egg-info/not-zip-safe
+-rw-r--r--   0 niklas    (1000) niklas    (1000)        6 2022-12-22 11:32:51.000000 chess-1.9.4/chess.egg-info/top_level.txt
+-rw-r--r--   0 niklas    (1000) niklas    (1000)       38 2022-12-22 11:32:51.358749 chess-1.9.4/setup.cfg
+-rwxr-xr-x   0 niklas    (1000) niklas    (1000)     3736 2022-11-27 08:57:46.000000 chess-1.9.4/setup.py
```

### Comparing `chess-1.9.3/CHANGELOG.rst` & `chess-1.9.4/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 Changelog for python-chess
 ==========================
 
-New in v1.9.3
--------------
+New in v1.9.4 (22nd Dec 2022)
+-----------------------------
+
+Bugfixes:
+
+* Fix ``PovScore.wdl()`` ignored ``model`` and ``ply`` parameters.
+* ``chess.syzygy``: Check that board matches tablebase variant.
+
+New features:
+
+* Add model ``sf15.1`` for ``chess.engine.Score.wdl()``.
+* Raise more specific exceptions: ``chess.IllegalMoveError``,
+  ``chess.AmbiguousMoveError``, and ``chess.InvalidMoveError``.
+
+New in v1.9.3 (16th Sep 2022)
+-----------------------------
 
 Bugfixes:
 
 * Fix some valid characters were not accepted in PGN tag names.
 
 Changes:
 
 * Skip over syntactically invalid PGN tags.
 * Detect Antichess insufficient material with two opposing knights.
 
 New features:
 
 * Add ``chess.Board.unicode(..., orientation=chess.WHITE)``.
 
-New in v1.9.2
--------------
+New in v1.9.2 (17th Jun 2022)
+-----------------------------
 
 Bugfixes:
 
 * Fix recursive Crazyhouse move generation sometimes failing with
   with ``RuntimeError``.
 * Fix rendering of black pawn SVG on dark background.
 
 New features:
 
 * Add ``chess.engine.AnalysisResult.would_block()``.
 
-New in v1.9.1
--------------
+New in v1.9.1 (28th May 2022)
+-----------------------------
 
 Bugfixes:
 
 * Reject pawn capture SAN if the original file is not specified, e.g.,
   ``d5`` will no longer match ``cxd5``.
 
 Changes:
@@ -46,64 +60,64 @@
   newline character. When removing annotations from comments, leftover
   whitespace is avoided.
 
 New features:
 
 * Add model ``sf15`` for ``chess.engine.Score.wdl()``.
 
-New in v1.9.0
--------------
+New in v1.9.0 (18th Mar 2022)
+-----------------------------
 
 Bugfixes:
 
 * Expand position validation to detect check conflicting with en passant
   square.
 
 New features:
 
 * Add ``chess.svg.board(..., fill=...)``.
 * Let ``chess.svg.board()`` add ASCII board as description of SVG.
 * Add hint when engine process dies due to illegal instruction.
 
-New in v1.8.0
--------------
+New in v1.8.0 (23rd Dec 2021)
+-----------------------------
 
 Bugfixes:
 
 * Fix ``SquareSet.issuperset()`` and ``SquareSet.issubset()`` by swapping
   their respective implementations.
 
 New features:
 
 * Read and write PGN comments like ``[%emt 0:05:21]``.
 
-New in v1.7.0
--------------
+New in v1.7.0 (7th Oct 2021)
+----------------------------
 
 New features:
 
 * Add new models for ``chess.engine.Score.wdl()``: ``sf`` (the new default)
   and ``sf14``.
 * Add ``chess.Board.piece_map()``.
 
 Bugfixes:
 
 * ``chess.pgn``: Fix skipping with nested variations.
 * ``chess.svg``: Make check gradient compatible with QtSvg.
 
-New in v1.6.1
--------------
+New in v1.6.1 (12th Jun 2021)
+-----------------------------
 
 Bugfixes:
 
 * Make ``chess.engine.SimpleEngine.play(..., draw_offered=True)`` available.
   Previously only added for ``chess.engine.Protocol``.
 
-New in v1.6.0
--------------
+New in v1.6.0 (11th Jun 2021)
+-----------------------------
 
 New features:
 
 * Allow offering a draw to XBoard engines using
   ``chess.engine.Protocol.play(..., draw_offered=True)``.
 * Now detects insufficient material in Horde. Thanks @stevepapazis!
 
@@ -117,16 +131,16 @@
   compatibility.
 
 Bugfixes:
 
 * Fix slightly off-center pawns in ``chess.svg``.
 * Fix typing error in Python 3.10 (due to added ``int.bit_count``).
 
-New in v1.5.0
--------------
+New in v1.5.0 (7th Apr 2021)
+----------------------------
 
 Bugfixes:
 
 * Fixed typing of ``chess.pgn.Mainline.__reversed__()``. It is now a generator,
   and ``chess.pgn.ReverseMainline`` has been **removed**.
   This is a breaking change but a required bugfix.
 * Implement UCI **ponderhit** for consecutive calls to
@@ -144,16 +158,16 @@
 
 * Added ``chess.Board.outcome()``.
 * Implement and accept usermove feature for XBoard engines.
 
 Special thanks to @MarkZH for many of the engine related changes in this
 release!
 
-New in v1.4.0
--------------
+New in v1.4.0 (25th Jan 2021)
+-----------------------------
 
 New features:
 
 * Let ``chess.pgn.GameNode.eval()`` accept PGN comments like
   ``[%eval 2.5,11]``, meaning 250 centipawns at depth 11.
   Use ``chess.pgn.GameNode.eval_depth()`` and
   ``chess.pgn.GameNode.set_eval(..., depth)`` to get and set the depth.
@@ -161,16 +175,16 @@
   ``[%clk 1:23:45.678]``.
 
 Changes:
 
 * Recover from invalid UTF-8 sent by an UCI engine, by ignoring that
   (and only that) line.
 
-New in v1.3.3
--------------
+New in v1.3.3 (27th Dec 2020)
+-----------------------------
 
 Bugfixes:
 
 * Fixed unintended collisions and optimized ``chess.Piece.__hash__()``.
 * Fixed false-positive ``chess.STATUS_IMPOSSIBLE_CHECK`` if checkers are
   aligned with other king.
 
@@ -180,36 +194,36 @@
   en passant square and king.
 
 New features:
 
 * Implemented Lichess winning chance model for ``chess.engine.Score``:
   ``score.wdl(model="lichess")``.
 
-New in v1.3.2
--------------
+New in v1.3.2 (12th Dec 2020)
+-----------------------------
 
 Bugfixes:
 
 * Added a new reason for ``board.status()`` to be invalid:
   ``chess.STATUS_IMPOSSIBLE_CHECK``. This detects positions where two sliding
   pieces are giving check while also being aligned with the king
   on the same rank, file, or diagonal. Such positions are impossible to reach,
   break Stockfish, and maybe other engines.
 
-New in v1.3.1
--------------
+New in v1.3.1 (6th Dec 2020)
+----------------------------
 
 Bugfixes:
 
 * ``chess.pgn.read_game()`` now properly detects variant games with Chess960
   castling rights (as well as mislabeled Standard Chess960 games). Previously,
   all castling moves in such games were rejected.
 
-New in v1.3.0
--------------
+New in v1.3.0 (6th Nov 2020)
+----------------------------
 
 Changes:
 
 * Introduced ``chess.pgn.ChildNode``, a subclass of ``chess.pgn.GameNode``
   for all nodes other than the root node, and converted ``chess.pgn.GameNode``
   to an abstract base class. This improves ergonomics in typed code.
 
@@ -224,24 +238,24 @@
 
 * Removed broken ``weakref``-based caching in ``chess.pgn.GameNode.board()``.
 
 New features:
 
 * Added ``chess.pgn.GameNode.next()``.
 
-New in v1.2.2
--------------
+New in v1.2.2 (29th Oct 2020)
+-----------------------------
 
 Bugfixes:
 
 * Fixed regression where releases were uploaded without the ``py.typed``
   marker.
 
-New in v1.2.1
--------------
+New in v1.2.1 (26th Oct 2020)
+-----------------------------
 
 Changes:
 
 * The primary location for the published package is now
   https://pypi.org/project/chess/. Thanks to
   `Kristian Glass <https://github.com/doismellburning>`_ for transferring the
   namespace.
@@ -250,16 +264,16 @@
   installs the package from the new location as a dependency (as recommended by
   `PEP423 <https://www.python.org/dev/peps/pep-0423/#how-to-rename-a-project>`_).
 
   ``ModuleNotFoundError: No module named 'chess'`` after upgrading from
   previous versions? Run ``pip install --force-reinstall chess``
   (due to https://github.com/niklasf/python-chess/issues/680).
 
-New in v1.2.0
--------------
+New in v1.2.0 (22nd Oct 2020)
+-----------------------------
 
 New features:
 
 * Added ``chess.Board.ply()``.
 * Added ``chess.pgn.GameNode.ply()`` and ``chess.pgn.GameNode.turn()``.
 * Added ``chess.engine.PovWdl``, ``chess.engine.Wdl``, and conversions from
   scores: ``chess.engine.PovScore.wdl()``, ``chess.engine.Score.wdl()``.
@@ -278,34 +292,34 @@
   but it is recommended to use its documented fields and methods instead.
 * Removed ``chess.engine.PovScore.__str__()``. String representation falls back
   to ``__repr__``.
 * The ``en_passant`` parameter of ``chess.Board.fen()`` and
   ``chess.Board.epd()`` is now typed as ``Literal["legal", "fen", "xfen"]``
   rather than ``str``.
 
-New in v1.1.0
--------------
+New in v1.1.0 (4th Oct 2020)
+----------------------------
 
 New features:
 
 * Added ``chess.svg.board(..., orientation)``. This is a more idiomatic way to
   set the board orientation than ``flipped``.
 * Added ``chess.svg.Arrow.pgn()`` and ``chess.svg.Arrow.from_pgn()``.
 
 Changes:
 
 * Further relaxed ``chess.Board.parse_san()``. Now accepts fully specified moves
   like ``e2e4``, even if that is not a pawn move, castling notation with zeros,
   null moves in UCI notation, and null moves in XBoard notation.
 
-New in v1.0.1
--------------
+New in v1.0.1 (24th Sep 2020)
+-----------------------------
 
 Bugfixes:
 
 * ``chess.svg``: Restored SVG Tiny compatibility by splitting colors like
   ``#rrggbbaa`` into a solid color and opacity.
 
-New in v1.0.0
--------------
+New in v1.0.0 (24th Sep 2020)
+-----------------------------
 
 See ``CHANGELOG-OLD.rst`` for changes up to v1.0.0.
```

### Comparing `chess-1.9.3/LICENSE.txt` & `chess-1.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chess-1.9.3/PKG-INFO` & `chess-1.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess
-Version: 1.9.3
+Version: 1.9.4
 Summary: A chess library with move generation and validation, Polyglot opening book probing, PGN reading and writing, Gaviota tablebase probing, Syzygy tablebase probing, and XBoard/UCI engine communication.
 Home-page: https://github.com/niklasf/python-chess
 Author: Niklas Fiekas
 Author-email: niklas.fiekas@backscattering.de
 License: GPL-3.0+
 Project-URL: Documentation, https://python-chess.readthedocs.io
 Keywords: chess fen epd pgn polyglot syzygy gaviota uci xboard
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Obsoletes: python_chess
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -34,16 +35,16 @@
     :target: https://github.com/niklasf/python-chess/actions
     :alt: Test status
 
 .. image:: https://badge.fury.io/py/chess.svg
     :target: https://pypi.python.org/pypi/chess
     :alt: PyPI package
 
-.. image:: https://readthedocs.org/projects/python-chess/badge/?version=v1.9.3
-    :target: https://python-chess.readthedocs.io/en/v1.9.3/
+.. image:: https://readthedocs.org/projects/python-chess/badge/?version=v1.9.4
+    :target: https://python-chess.readthedocs.io/en/v1.9.4/
     :alt: Docs
 
 .. image:: https://badges.gitter.im/python-chess/community.svg
     :target: https://gitter.im/python-chess/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
     :alt: Chat on Gitter
 
 Introduction
@@ -91,44 +92,44 @@
 Requires Python 3.7+. Download and install the latest release:
 
 ::
 
     pip install chess
 
 
-`Documentation <https://python-chess.readthedocs.io/en/v1.9.3/>`__
+`Documentation <https://python-chess.readthedocs.io/en/v1.9.4/>`__
 --------------------------------------------------------------------
 
-* `Core <https://python-chess.readthedocs.io/en/v1.9.3/core.html>`_
-* `PGN parsing and writing <https://python-chess.readthedocs.io/en/v1.9.3/pgn.html>`_
-* `Polyglot opening book reading <https://python-chess.readthedocs.io/en/v1.9.3/polyglot.html>`_
-* `Gaviota endgame tablebase probing <https://python-chess.readthedocs.io/en/v1.9.3/gaviota.html>`_
-* `Syzygy endgame tablebase probing <https://python-chess.readthedocs.io/en/v1.9.3/syzygy.html>`_
-* `UCI/XBoard engine communication <https://python-chess.readthedocs.io/en/v1.9.3/engine.html>`_
-* `Variants <https://python-chess.readthedocs.io/en/v1.9.3/variant.html>`_
-* `Changelog <https://python-chess.readthedocs.io/en/v1.9.3/changelog.html>`_
+* `Core <https://python-chess.readthedocs.io/en/v1.9.4/core.html>`_
+* `PGN parsing and writing <https://python-chess.readthedocs.io/en/v1.9.4/pgn.html>`_
+* `Polyglot opening book reading <https://python-chess.readthedocs.io/en/v1.9.4/polyglot.html>`_
+* `Gaviota endgame tablebase probing <https://python-chess.readthedocs.io/en/v1.9.4/gaviota.html>`_
+* `Syzygy endgame tablebase probing <https://python-chess.readthedocs.io/en/v1.9.4/syzygy.html>`_
+* `UCI/XBoard engine communication <https://python-chess.readthedocs.io/en/v1.9.4/engine.html>`_
+* `Variants <https://python-chess.readthedocs.io/en/v1.9.4/variant.html>`_
+* `Changelog <https://python-chess.readthedocs.io/en/v1.9.4/changelog.html>`_
 
 Features
 --------
 
 * Includes mypy typings.
 
 * IPython/Jupyter Notebook integration.
-  `SVG rendering docs <https://python-chess.readthedocs.io/en/v1.9.3/svg.html>`_.
+  `SVG rendering docs <https://python-chess.readthedocs.io/en/v1.9.4/svg.html>`_.
 
   .. code:: python
 
       >>> board
 
   .. image:: https://backscattering.de/web-boardimage/board.png?fen=r1bqkb1r/pppp1Qpp/2n2n2/4p3/2B1P3/8/PPPP1PPP/RNB1K1NR&lastmove=h5f7&check=e8
       :alt: r1bqkb1r/pppp1Qpp/2n2n2/4p3/2B1P3/8/PPPP1PPP/RNB1K1NR
 
 * Chess variants: Standard, Chess960, Suicide, Giveaway, Atomic,
   King of the Hill, Racing Kings, Horde, Three-check, Crazyhouse.
-  `Variant docs <https://python-chess.readthedocs.io/en/v1.9.3/variant.html>`_.
+  `Variant docs <https://python-chess.readthedocs.io/en/v1.9.4/variant.html>`_.
 
 * Make and unmake moves.
 
   .. code:: python
 
       >>> Nf3 = chess.Move.from_uci("g1f3")
       >>> board.push(Nf3)  # Make the move
@@ -242,18 +243,18 @@
       >>> board.epd(bm=board.parse_uci("d2d4"))
       'rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR w KQkq - bm d4;'
 
       >>> ops = board.set_epd("1k1r4/pp1b1R2/3q2pp/4p3/2B5/4Q3/PPP2B2/2K5 b - - bm Qd1+; id \"BK.01\";")
       >>> ops == {'bm': [chess.Move.from_uci('d6d1')], 'id': 'BK.01'}
       True
 
-* Detects `absolute pins and their directions <https://python-chess.readthedocs.io/en/v1.9.3/core.html#chess.Board.pin>`_.
+* Detects `absolute pins and their directions <https://python-chess.readthedocs.io/en/v1.9.4/core.html#chess.Board.pin>`_.
 
 * Reads Polyglot opening books.
-  `Docs <https://python-chess.readthedocs.io/en/v1.9.3/polyglot.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v1.9.4/polyglot.html>`__.
 
   .. code:: python
 
       >>> import chess.polyglot
 
       >>> book = chess.polyglot.open_reader("data/polyglot/performance.bin")
 
@@ -264,15 +265,15 @@
       >>> main_entry.weight
       1
 
       >>> book.close()
 
 * Reads and writes PGNs. Supports headers, comments, NAGs and a tree of
   variations.
-  `Docs <https://python-chess.readthedocs.io/en/v1.9.3/pgn.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v1.9.4/pgn.html>`__.
 
   .. code:: python
 
       >>> import chess.pgn
 
       >>> with open("data/pgn/molinari-bordais-1979.pgn") as pgn:
       ...     first_game = chess.pgn.read_game(pgn)
@@ -285,18 +286,18 @@
       >>> first_game.mainline()
       <Mainline at ... (1. e4 c5 2. c4 Nc6 3. Ne2 Nf6 4. Nbc3 Nb4 5. g3 Nd3#)>
 
       >>> first_game.headers["Result"]
       '0-1'
 
 * Probe Gaviota endgame tablebases (DTM, WDL).
-  `Docs <https://python-chess.readthedocs.io/en/v1.9.3/gaviota.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v1.9.4/gaviota.html>`__.
 
 * Probe Syzygy endgame tablebases (DTZ, WDL).
-  `Docs <https://python-chess.readthedocs.io/en/v1.9.3/syzygy.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v1.9.4/syzygy.html>`__.
 
   .. code:: python
 
       >>> import chess.syzygy
 
       >>> tablebase = chess.syzygy.open_tablebase("data/syzygy/regular")
 
@@ -305,15 +306,15 @@
       >>> board = chess.Board("8/2K5/4B3/3N4/8/8/4k3/8 b - - 0 1")
       >>> tablebase.probe_dtz(board)
       -53
 
       >>> tablebase.close()
 
 * Communicate with UCI/XBoard engines. Based on ``asyncio``.
-  `Docs <https://python-chess.readthedocs.io/en/v1.9.3/engine.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v1.9.4/engine.html>`__.
 
   .. code:: python
 
       >>> import chess.engine
 
       >>> engine = chess.engine.SimpleEngine.popen_uci("stockfish")
 
@@ -325,58 +326,60 @@
       >>> engine.quit()
 
 Selected projects
 -----------------
 
 If you like, share interesting things you are using python-chess for, for example:
 
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/syzygy.png?raw=true       | https://syzygy-tables.info/                                                             |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://syzygy-tables.info/                                                             | A website to probe Syzygy endgame tablebases                                            |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/maia.png?raw=true         | https://maiachess.com/                                                                  |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://maiachess.com/                                                                  | A human-like neural network chess engine                                                |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/clente-chess.png?raw=true | `clente/chess <https://github.com/clente/chess>`_                                       |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://github.com/clente/chess                                                         | Oppinionated wrapper to use python-chess from the R programming language                |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/crazyara.png?raw=true     | https://crazyara.org/                                                                   |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://crazyara.org/                                                                   | Deep learning for Crazyhouse                                                            |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/jcchess.png?raw=true      | `http://johncheetham.com <http://johncheetham.com/projects/jcchess/>`_                  |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: http://johncheetham.com/projects/jcchess/                                               | A GUI to play against UCI chess engines                                                 |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/pettingzoo.png?raw=true   | `https://www.pettingzoo.ml <https://www.pettingzoo.ml/classic/chess>`_                  |
-|     :width: 64                                                                                       |                                                                                         |
-|     :height: 64                                                                                      |                                                                                         |
-|     :target: https://www.pettingzoo.ml/classic/chess                                                 | A multi-agent reinforcement learning environment                                        |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/syzygy.png?raw=true       | https://syzygy-tables.info/                                                                  |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://syzygy-tables.info/                                                             | A website to probe Syzygy endgame tablebases                                                 |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/maia.png?raw=true         | https://maiachess.com/                                                                       |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://maiachess.com/                                                                  | A human-like neural network chess engine                                                     |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/clente-chess.png?raw=true | `clente/chess <https://github.com/clente/chess>`_                                            |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://github.com/clente/chess                                                         | Oppinionated wrapper to use python-chess from the R programming language                     |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/crazyara.png?raw=true     | https://crazyara.org/                                                                        |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://crazyara.org/                                                                   | Deep learning for Crazyhouse                                                                 |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/jcchess.png?raw=true      | `http://johncheetham.com <http://johncheetham.com/projects/jcchess/>`_                       |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: http://johncheetham.com/projects/jcchess/                                               | A GUI to play against UCI chess engines                                                      |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/pettingzoo.png?raw=true   | `https://pettingzoo.farama.org <https://pettingzoo.farama.org/environments/classic/chess/>`_ |
+|     :width: 64                                                                                       |                                                                                              |
+|     :height: 64                                                                                      |                                                                                              |
+|     :target: https://pettingzoo.farama.org/environments/classic/chess/                               | A multi-agent reinforcement learning environment                                             |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
 
 * extensions to build engines (search and evaluation) – https://github.com/Mk-Chan/python-chess-engine-extensions
 * a stand-alone chess computer based on DGT board – http://www.picochess.org/
 * a bridge between Lichess API and chess engines – https://github.com/careless25/lichess-bot
 * a command-line PGN annotator – https://github.com/rpdelaney/python-chess-annotator
 * an HTTP microservice to render board images – https://github.com/niklasf/web-boardimage
 * building a toy chess engine with alpha-beta pruning, piece-square tables, and move ordering – https://healeycodes.com/building-my-own-chess-engine/
 * a JIT compiled chess engine – https://github.com/SamRagusa/Batch-First
 * teaching Cognitive Science – `https://jupyter.brynmawr.edu <https://jupyter.brynmawr.edu/services/public/dblank/CS371%20Cognitive%20Science/2016-Fall/Programming%20a%20Chess%20Player.ipynb>`_
 * an `Alexa skill to play blindfold chess <https://www.amazon.com/Laynr-blindfold-chess/dp/B0859QF8YL>`_ – https://github.com/laynr/blindfold-chess
 * a chessboard widget for PySide2 – https://github.com/H-a-y-k/hichesslib
 * Django Rest Framework API for multiplayer chess – https://github.com/WorkShoft/capablanca-api
 * a `browser based PGN viewer <https://about.nmstoker.com/chess2.html>`_ written in PyScript – https://github.com/nmstoker/ChessMatchViewer
+* an accessible chessboard that allows blind and visually impaired  players  to play chess against Stockfish – https://github.com/blindpandas/chessmart
+
 
 Acknowledgements
 ----------------
 
 Thanks to the Stockfish authors and thanks to Sam Tannous for publishing his
 approach to `avoid rotated bitboards with direct lookup (PDF) <http://arxiv.org/pdf/0704.3773.pdf>`_
 alongside his GPL2+ engine `Shatranj <https://github.com/stannous/shatranj>`_.
```

### Comparing `chess-1.9.3/README.rst` & `chess-1.9.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -296,58 +296,60 @@
       >>> engine.quit()
 
 Selected projects
 -----------------
 
 If you like, share interesting things you are using python-chess for, for example:
 
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/syzygy.png?raw=true       | https://syzygy-tables.info/                                                             |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://syzygy-tables.info/                                                             | A website to probe Syzygy endgame tablebases                                            |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/maia.png?raw=true         | https://maiachess.com/                                                                  |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://maiachess.com/                                                                  | A human-like neural network chess engine                                                |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/clente-chess.png?raw=true | `clente/chess <https://github.com/clente/chess>`_                                       |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://github.com/clente/chess                                                         | Oppinionated wrapper to use python-chess from the R programming language                |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/crazyara.png?raw=true     | https://crazyara.org/                                                                   |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://crazyara.org/                                                                   | Deep learning for Crazyhouse                                                            |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/jcchess.png?raw=true      | `http://johncheetham.com <http://johncheetham.com/projects/jcchess/>`_                  |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: http://johncheetham.com/projects/jcchess/                                               | A GUI to play against UCI chess engines                                                 |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/pettingzoo.png?raw=true   | `https://www.pettingzoo.ml <https://www.pettingzoo.ml/classic/chess>`_                  |
-|     :width: 64                                                                                       |                                                                                         |
-|     :height: 64                                                                                      |                                                                                         |
-|     :target: https://www.pettingzoo.ml/classic/chess                                                 | A multi-agent reinforcement learning environment                                        |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/syzygy.png?raw=true       | https://syzygy-tables.info/                                                                  |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://syzygy-tables.info/                                                             | A website to probe Syzygy endgame tablebases                                                 |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/maia.png?raw=true         | https://maiachess.com/                                                                       |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://maiachess.com/                                                                  | A human-like neural network chess engine                                                     |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/clente-chess.png?raw=true | `clente/chess <https://github.com/clente/chess>`_                                            |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://github.com/clente/chess                                                         | Oppinionated wrapper to use python-chess from the R programming language                     |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/crazyara.png?raw=true     | https://crazyara.org/                                                                        |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://crazyara.org/                                                                   | Deep learning for Crazyhouse                                                                 |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/jcchess.png?raw=true      | `http://johncheetham.com <http://johncheetham.com/projects/jcchess/>`_                       |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: http://johncheetham.com/projects/jcchess/                                               | A GUI to play against UCI chess engines                                                      |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/pettingzoo.png?raw=true   | `https://pettingzoo.farama.org <https://pettingzoo.farama.org/environments/classic/chess/>`_ |
+|     :width: 64                                                                                       |                                                                                              |
+|     :height: 64                                                                                      |                                                                                              |
+|     :target: https://pettingzoo.farama.org/environments/classic/chess/                               | A multi-agent reinforcement learning environment                                             |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
 
 * extensions to build engines (search and evaluation) – https://github.com/Mk-Chan/python-chess-engine-extensions
 * a stand-alone chess computer based on DGT board – http://www.picochess.org/
 * a bridge between Lichess API and chess engines – https://github.com/careless25/lichess-bot
 * a command-line PGN annotator – https://github.com/rpdelaney/python-chess-annotator
 * an HTTP microservice to render board images – https://github.com/niklasf/web-boardimage
 * building a toy chess engine with alpha-beta pruning, piece-square tables, and move ordering – https://healeycodes.com/building-my-own-chess-engine/
 * a JIT compiled chess engine – https://github.com/SamRagusa/Batch-First
 * teaching Cognitive Science – `https://jupyter.brynmawr.edu <https://jupyter.brynmawr.edu/services/public/dblank/CS371%20Cognitive%20Science/2016-Fall/Programming%20a%20Chess%20Player.ipynb>`_
 * an `Alexa skill to play blindfold chess <https://www.amazon.com/Laynr-blindfold-chess/dp/B0859QF8YL>`_ – https://github.com/laynr/blindfold-chess
 * a chessboard widget for PySide2 – https://github.com/H-a-y-k/hichesslib
 * Django Rest Framework API for multiplayer chess – https://github.com/WorkShoft/capablanca-api
 * a `browser based PGN viewer <https://about.nmstoker.com/chess2.html>`_ written in PyScript – https://github.com/nmstoker/ChessMatchViewer
+* an accessible chessboard that allows blind and visually impaired  players  to play chess against Stockfish – https://github.com/blindpandas/chessmart
+
 
 Acknowledgements
 ----------------
 
 Thanks to the Stockfish authors and thanks to Sam Tannous for publishing his
 approach to `avoid rotated bitboards with direct lookup (PDF) <http://arxiv.org/pdf/0704.3773.pdf>`_
 alongside his GPL2+ engine `Shatranj <https://github.com/stannous/shatranj>`_.
```

### Comparing `chess-1.9.3/chess/__init__.py` & `chess-1.9.4/chess/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 from __future__ import annotations
 
 __author__ = "Niklas Fiekas"
 
 __email__ = "niklas.fiekas@backscattering.de"
 
-__version__ = "1.9.3"
+__version__ = "1.9.4"
 
 import collections
 import copy
 import dataclasses
 import enum
 import math
 import re
@@ -161,14 +161,26 @@
     """The winning color or ``None`` if drawn."""
 
     def result(self) -> str:
         """Returns ``1-0``, ``0-1`` or ``1/2-1/2``."""
         return "1/2-1/2" if self.winner is None else ("1-0" if self.winner else "0-1")
 
 
+class InvalidMoveError(ValueError):
+    """Raised when move notation is not syntactically valid"""
+
+
+class IllegalMoveError(ValueError):
+    """Raised when the attempted move is illegal in the current position"""
+
+
+class AmbiguousMoveError(ValueError):
+    """Raised when the attempted move is ambiguous in the current position"""
+
+
 Square = int
 SQUARES = [
     A1, B1, C1, D1, E1, F1, G1, H1,
     A2, B2, C2, D2, E2, F2, G2, H2,
     A3, B3, C3, D3, E3, F3, G3, H3,
     A4, B4, C4, D4, E4, F4, G4, H4,
     A5, B5, C5, D5, E5, F5, G5, H5,
@@ -547,31 +559,37 @@
         return self.uci()
 
     @classmethod
     def from_uci(cls, uci: str) -> Move:
         """
         Parses a UCI string.
 
-        :raises: :exc:`ValueError` if the UCI string is invalid.
+        :raises: :exc:`InvalidMoveError` if the UCI string is invalid.
         """
         if uci == "0000":
             return cls.null()
         elif len(uci) == 4 and "@" == uci[1]:
-            drop = PIECE_SYMBOLS.index(uci[0].lower())
-            square = SQUARE_NAMES.index(uci[2:])
+            try:
+                drop = PIECE_SYMBOLS.index(uci[0].lower())
+                square = SQUARE_NAMES.index(uci[2:])
+            except ValueError:
+                raise InvalidMoveError(f"invalid uci: {uci!r}")
             return cls(square, square, drop=drop)
         elif 4 <= len(uci) <= 5:
-            from_square = SQUARE_NAMES.index(uci[0:2])
-            to_square = SQUARE_NAMES.index(uci[2:4])
-            promotion = PIECE_SYMBOLS.index(uci[4]) if len(uci) == 5 else None
+            try:
+                from_square = SQUARE_NAMES.index(uci[0:2])
+                to_square = SQUARE_NAMES.index(uci[2:4])
+                promotion = PIECE_SYMBOLS.index(uci[4]) if len(uci) == 5 else None
+            except ValueError:
+                raise InvalidMoveError(f"invalid uci: {uci!r}")
             if from_square == to_square:
-                raise ValueError(f"invalid uci (use 0000 for null moves): {uci!r}")
+                raise InvalidMoveError(f"invalid uci (use 0000 for null moves): {uci!r}")
             return cls(from_square, to_square, promotion=promotion)
         else:
-            raise ValueError(f"expected uci string to be of length 4 or 5: {uci!r}")
+            raise InvalidMoveError(f"expected uci string to be of length 4 or 5: {uci!r}")
 
     @classmethod
     def null(cls) -> Move:
         """
         Gets a null move.
 
         A null move just passes the turn to the other side (and possibly
@@ -2301,22 +2319,22 @@
 
         For pawn moves to the backrank, the promotion piece type defaults to
         :data:`chess.QUEEN`, unless otherwise specified.
 
         Castling moves are normalized to king moves by two steps, except in
         Chess960.
 
-        :raises: :exc:`ValueError` if no matching legal move is found.
+        :raises: :exc:`IllegalMoveError` if no matching legal move is found.
         """
         if promotion is None and self.pawns & BB_SQUARES[from_square] and BB_SQUARES[to_square] & BB_BACKRANKS:
             promotion = QUEEN
 
         move = self._from_chess960(self.chess960, from_square, to_square, promotion)
         if not self.is_legal(move):
-            raise ValueError(f"no matching legal move for {move.uci()} ({SQUARE_NAMES[from_square]} -> {SQUARE_NAMES[to_square]}) in {self.fen()}")
+            raise IllegalMoveError(f"no matching legal move for {move.uci()} ({SQUARE_NAMES[from_square]} -> {SQUARE_NAMES[to_square]}) in {self.fen()}")
 
         return move
 
     def castling_shredder_fen(self) -> str:
         castling_rights = self.clean_castling_rights()
         if not castling_rights:
             return "-"
@@ -2934,22 +2952,22 @@
         """
         Given a sequence of moves, returns a string representing the sequence
         in standard algebraic notation (e.g., ``1. e4 e5 2. Nf3 Nc6`` or
         ``37...Bg6 38. fxg6``).
 
         The board will not be modified as a result of calling this.
 
-        :raises: :exc:`ValueError` if any moves in the sequence are illegal.
+        :raises: :exc:`IllegalMoveError` if any moves in the sequence are illegal.
         """
         board = self.copy(stack=False)
         san = []
 
         for move in variation:
             if not board.is_legal(move):
-                raise ValueError(f"illegal move {move} in position {board.fen()}")
+                raise IllegalMoveError(f"illegal move {move} in position {board.fen()}")
 
             if board.turn == WHITE:
                 san.append(f"{board.fullmove_number}. {board.san_and_push(move)}")
             elif not san:
                 san.append(f"{board.fullmove_number}...{board.san_and_push(move)}")
             else:
                 san.append(board.san_and_push(move))
@@ -2958,39 +2976,44 @@
 
     def parse_san(self, san: str) -> Move:
         """
         Uses the current position as the context to parse a move in standard
         algebraic notation and returns the corresponding move object.
 
         Ambiguous moves are rejected. Overspecified moves (including long
-        algebraic notation) are accepted.
+        algebraic notation) are accepted. Some common syntactical deviations
+        are also accepted.
 
         The returned move is guaranteed to be either legal or a null move.
 
-        :raises: :exc:`ValueError` if the SAN is invalid, illegal or ambiguous.
+        :raises:
+            :exc:`ValueError` (specifically an exception specified below) if the SAN is invalid, illegal or ambiguous.
+                - :exc:`InvalidMoveError` if the SAN is syntactically invalid.
+                - :exc:`IllegalMoveError` if the SAN is illegal.
+                - :exc:`AmbiguousMoveError` if the SAN is ambiguous.
         """
         # Castling.
         try:
             if san in ["O-O", "O-O+", "O-O#", "0-0", "0-0+", "0-0#"]:
                 return next(move for move in self.generate_castling_moves() if self.is_kingside_castling(move))
             elif san in ["O-O-O", "O-O-O+", "O-O-O#", "0-0-0", "0-0-0+", "0-0-0#"]:
                 return next(move for move in self.generate_castling_moves() if self.is_queenside_castling(move))
         except StopIteration:
-            raise ValueError(f"illegal san: {san!r} in {self.fen()}")
+            raise IllegalMoveError(f"illegal san: {san!r} in {self.fen()}")
 
         # Match normal moves.
         match = SAN_REGEX.match(san)
         if not match:
             # Null moves.
             if san in ["--", "Z0", "0000", "@@@@"]:
                 return Move.null()
             elif "," in san:
-                raise ValueError(f"unsupported multi-leg move: {san!r}")
+                raise InvalidMoveError(f"unsupported multi-leg move: {san!r}")
             else:
-                raise ValueError(f"invalid san: {san!r}")
+                raise InvalidMoveError(f"invalid san: {san!r}")
 
         # Get target square. Mask our own pieces to exclude castling moves.
         to_square = SQUARE_NAMES.index(match.group(4))
         to_mask = BB_SQUARES[to_square] & ~self.occupied_co[self.turn]
 
         # Get the promotion piece type.
         p = match.group(5)
@@ -3012,46 +3035,50 @@
         elif match.group(2) and match.group(3):
             # Allow fully specified moves, even if they are not pawn moves,
             # including castling moves.
             move = self.find_move(square(from_file, from_rank), to_square, promotion)
             if move.promotion == promotion:
                 return move
             else:
-                raise ValueError(f"missing promotion piece type: {san!r} in {self.fen()}")
+                raise IllegalMoveError(f"missing promotion piece type: {san!r} in {self.fen()}")
         else:
             from_mask &= self.pawns
 
             # Do not allow pawn captures if file is not specified.
             if not match.group(2):
                 from_mask &= BB_FILES[square_file(to_square)]
 
         # Match legal moves.
         matched_move = None
         for move in self.generate_legal_moves(from_mask, to_mask):
             if move.promotion != promotion:
                 continue
 
             if matched_move:
-                raise ValueError(f"ambiguous san: {san!r} in {self.fen()}")
+                raise AmbiguousMoveError(f"ambiguous san: {san!r} in {self.fen()}")
 
             matched_move = move
 
         if not matched_move:
-            raise ValueError(f"illegal san: {san!r} in {self.fen()}")
+            raise IllegalMoveError(f"illegal san: {san!r} in {self.fen()}")
 
         return matched_move
 
     def push_san(self, san: str) -> Move:
         """
         Parses a move in standard algebraic notation, makes the move and puts
         it onto the move stack.
 
         Returns the move.
 
-        :raises: :exc:`ValueError` if neither legal nor a null move.
+        :raises:
+            :exc:`ValueError` (specifically an exception specified below) if neither legal nor a null move.
+                - :exc:`InvalidMoveError` if the SAN is syntactically invalid.
+                - :exc:`IllegalMoveError` if the SAN is illegal.
+                - :exc:`AmbiguousMoveError` if the SAN is ambiguous.
         """
         move = self.parse_san(san)
         self.push(move)
         return move
 
     def uci(self, move: Move, *, chess960: Optional[bool] = None) -> str:
         """
@@ -3071,38 +3098,44 @@
         """
         Parses the given move in UCI notation.
 
         Supports both Chess960 and standard UCI notation.
 
         The returned move is guaranteed to be either legal or a null move.
 
-        :raises: :exc:`ValueError` if the move is invalid or illegal in the
+        :raises:
+            :exc:`ValueError` (specifically an exception specified below) if the move is invalid or illegal in the
             current position (but not a null move).
+                - :exc:`InvalidMoveError` if the UCI is syntactically invalid.
+                - :exc:`IllegalMoveError` if the UCI is illegal.
         """
         move = Move.from_uci(uci)
 
         if not move:
             return move
 
         move = self._to_chess960(move)
         move = self._from_chess960(self.chess960, move.from_square, move.to_square, move.promotion, move.drop)
 
         if not self.is_legal(move):
-            raise ValueError(f"illegal uci: {uci!r} in {self.fen()}")
+            raise IllegalMoveError(f"illegal uci: {uci!r} in {self.fen()}")
 
         return move
 
     def push_uci(self, uci: str) -> Move:
         """
         Parses a move in UCI notation and puts it on the move stack.
 
         Returns the move.
 
-        :raises: :exc:`ValueError` if the move is invalid or illegal in the
+        :raises:
+            :exc:`ValueError` (specifically an exception specified below) if the move is invalid or illegal in the
             current position (but not a null move).
+                - :exc:`InvalidMoveError` if the UCI is syntactically invalid.
+                - :exc:`IllegalMoveError` if the UCI is illegal.
         """
         move = self.parse_uci(uci)
         self.push(move)
         return move
 
     def xboard(self, move: Move, chess960: Optional[bool] = None) -> str:
         if chess960 is None:
```

### Comparing `chess-1.9.3/chess/_interactive.py` & `chess-1.9.4/chess/_interactive.py`

 * *Files identical despite different names*

### Comparing `chess-1.9.3/chess/engine.py` & `chess-1.9.4/chess/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 from chess import Color
 from types import TracebackType
 from typing import Any, Callable, Coroutine, Deque, Dict, Generator, Generic, Iterable, Iterator, List, Mapping, MutableMapping, Optional, Tuple, Type, TypeVar, Union
 
 try:
     from typing import Literal
-    _WdlModel = Literal["sf", "sf15", "sf14", "sf12", "lichess"]
+    _WdlModel = Literal["sf", "sf15.1", "sf15", "sf14", "sf12", "lichess"]
 except ImportError:
     # Before Python 3.8.
     _WdlModel = str  # type: ignore
 
 
 T = TypeVar("T")
 ProtocolT = TypeVar("ProtocolT", bound="Protocol")
@@ -465,15 +465,15 @@
 
     def is_mate(self) -> bool:
         """Tests if this is a mate score."""
         return self.relative.is_mate()
 
     def wdl(self, *, model: _WdlModel = "sf", ply: int = 30) -> PovWdl:
         """See :func:`~chess.engine.Score.wdl()`."""
-        return PovWdl(self.relative.wdl(), self.turn)
+        return PovWdl(self.relative.wdl(model=model, ply=ply), self.turn)
 
     def __repr__(self) -> str:
         return "PovScore({!r}, {})".format(self.relative, "WHITE" if self.turn else "BLACK")
 
     def __eq__(self, other: object) -> bool:
         if isinstance(other, PovScore):
             return self.white() == other.white()
@@ -560,15 +560,16 @@
         0.379...
 
         >>> Cp(500).wdl().expectation() - Cp(300).wdl().expectation()  # doctest: +ELLIPSIS
         0.015...
 
         :param model:
             * ``sf``, the WDL model used by the latest Stockfish
-              (currently ``sf15``).
+              (currently ``sf15.1``).
+            * ``sf15.1``, the WDL model used by Stockfish 15.1.
             * ``sf15``, the WDL model used by Stockfish 15.
             * ``sf14``, the WDL model used by Stockfish 14.
             * ``sf12``, the WDL model used by Stockfish 12.
             * ``lichess``, the win rate model used by Lichess.
               Does not use *ply*, and does not consider drawing chances.
         :param ply: The number of half-moves played since the starting
             position. Models may scale scores slightly differently based on
@@ -624,14 +625,24 @@
     def __ge__(self, other: object) -> bool:
         if isinstance(other, Score):
             return self._score_tuple() >= other._score_tuple()
         else:
             return NotImplemented
 
 
+def _sf15_1_wins(cp: int, *, ply: int) -> int:
+    # https://github.com/official-stockfish/Stockfish/blob/sf_15.1/src/uci.cpp#L200-L224
+    # https://github.com/official-stockfish/Stockfish/blob/sf_15.1/src/uci.h#L38
+    NormalizeToPawnValue = 361
+    m = min(240, max(ply, 0)) / 64
+    a = (((-0.58270499 * m + 2.68512549) * m + 15.24638015) * m) + 344.49745382
+    b = (((-2.65734562 * m + 15.96509799) * m + -20.69040836) * m) + 73.61029937
+    x = min(4000, max(cp * NormalizeToPawnValue / 100, -4000))
+    return int(0.5 + 1000 / (1 + math.exp((a - x) / b)))
+
 def _sf15_wins(cp: int, *, ply: int) -> int:
     # https://github.com/official-stockfish/Stockfish/blob/sf_15/src/uci.cpp#L200-L220
     m = min(240, max(ply, 0)) / 64
     a = (((-1.17202460e-1 * m + 5.94729104e-1) * m + 1.12065546e+1) * m) + 1.22606222e+2
     b = (((-1.79066759 * m + 11.30759193) * m + -17.43677612) * m) + 36.47147479
     x = min(2000, max(cp, -2000))
     return int(0.5 + 1000 / (1 + math.exp((a - x) / b)))
@@ -674,17 +685,20 @@
             losses = 1000 - wins
         elif model == "sf12":
             wins = _sf12_wins(self.cp, ply=ply)
             losses = _sf12_wins(-self.cp, ply=ply)
         elif model == "sf14":
             wins = _sf14_wins(self.cp, ply=ply)
             losses = _sf14_wins(-self.cp, ply=ply)
-        else:
+        elif model == "sf15":
             wins = _sf15_wins(self.cp, ply=ply)
             losses = _sf15_wins(-self.cp, ply=ply)
+        else:
+            wins = _sf15_1_wins(self.cp, ply=ply)
+            losses = _sf15_1_wins(-self.cp, ply=ply)
         draws = 1000 - wins - losses
         return Wdl(wins, draws, losses)
 
     def __str__(self) -> str:
         return f"+{self.cp:d}" if self.cp > 0 else str(self.cp)
 
     def __repr__(self) -> str:
```

### Comparing `chess-1.9.3/chess/gaviota.py` & `chess-1.9.4/chess/gaviota.py`

 * *Files identical despite different names*

### Comparing `chess-1.9.3/chess/pgn.py` & `chess-1.9.4/chess/pgn.py`

 * *Files identical despite different names*

### Comparing `chess-1.9.3/chess/polyglot.py` & `chess-1.9.4/chess/polyglot.py`

 * *Files identical despite different names*

### Comparing `chess-1.9.3/chess/svg.py` & `chess-1.9.4/chess/svg.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
     >>> import chess
     >>> import chess.svg
     >>>
     >>> board = chess.Board("8/8/8/8/4N3/8/8/8 w - - 0 1")
     >>>
     >>> chess.svg.board(
     ...     board,
-    ...     fill=dict.fromkeys(board.attacks(chess.E4), "#cc0000cc") | {chess.E4: "#00cc00cc"},
+    ...     fill=dict.fromkeys(board.attacks(chess.E4), "#cc0000cc"),
     ...     arrows=[chess.svg.Arrow(chess.E4, chess.F6, color="#0000cccc")],
     ...     squares=chess.SquareSet(chess.BB_DARK_SQUARES & chess.BB_FILE_B),
     ...     size=350,
     ... )  # doctest: +SKIP
 
     .. image:: ../docs/Ne4.svg
         :alt: 8/8/8/8/4N3/8/8/8
```

### Comparing `chess-1.9.3/chess/syzygy.py` & `chess-1.9.4/chess/syzygy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1581,14 +1581,23 @@
             raise MissingTableError(f"did not find wdl table {key}")
 
         self._bump_lru(table)
 
         return table.probe_wdl_table(board)
 
     def probe_ab(self, board: chess.Board, alpha: int, beta: int, threats: bool = False) -> Tuple[int, int]:
+        # Check preconditions.
+        if board.uci_variant != self.variant.uci_variant:
+            raise KeyError(f"tablebase has been opened for {self.variant.uci_variant}, probed with: {board.uci_variant}")
+        if board.castling_rights:
+            raise KeyError(f"syzygy tables do not contain positions with castling rights: {board.fen()}")
+        if chess.popcount(board.occupied) > TBPIECES:
+            raise KeyError(f"syzygy tables support up to {TBPIECES} pieces, not {chess.popcount(board.occupied)}: {board.fen()}")
+
+        # Special case: Variant with compulsory captures.
         if self.variant.captures_compulsory:
             if board.is_variant_win():
                 return 2, 2
             elif board.is_variant_loss():
                 return -2, 2
             elif board.is_variant_draw():
                 return 0, 2
@@ -1697,22 +1706,14 @@
             :exc:`chess.syzygy.MissingTableError`) if the position could not
             be found in the tablebase. Use
             :func:`~chess.syzygy.Tablebase.get_wdl()` if you prefer to get
             ``None`` instead of an exception.
 
             Note that probing corrupted table files is undefined behavior.
         """
-        # Positions with castling rights are not in the tablebase.
-        if board.castling_rights:
-            raise KeyError(f"syzygy tables do not contain positions with castling rights: {board.fen()}")
-
-        # Validate piece count.
-        if chess.popcount(board.occupied) > TBPIECES:
-            raise KeyError(f"syzygy tables support up to {TBPIECES} pieces, not {chess.popcount(board.occupied)}: {board.fen()}")
-
         # Probe.
         v, _ = self.probe_ab(board, -2, 2)
 
         # If en passant is not possible, we are done.
         if not board.ep_square or self.variant.captures_compulsory:
             return v
```

### Comparing `chess-1.9.3/chess/variant.py` & `chess-1.9.4/chess/variant.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,14 @@
     xboard_variant = "atomic"
 
     tbw_suffix = ".atbw"
     tbz_suffix = ".atbz"
     tbw_magic = b"\x55\x8d\xa4\x49"
     tbz_magic = b"\x91\xa9\x5e\xeb"
     connected_kings = True
-    one_king = True
 
     def is_variant_end(self) -> bool:
         return not all(self.kings & side for side in self.occupied_co)
 
     def is_variant_win(self) -> bool:
         return bool(self.kings and not self.kings & self.occupied_co[not self.turn])
 
@@ -985,15 +984,15 @@
     def parse_san(self, san: str) -> chess.Move:
         if "@" in san:
             uci = san.rstrip("+#")
             if uci[0] == "@":
                 uci = "P" + uci
             move = chess.Move.from_uci(uci)
             if not self.is_legal(move):
-                raise ValueError(f"illegal drop san: {san!r} in {self.fen()}")
+                raise chess.IllegalMoveError(f"illegal drop san: {san!r} in {self.fen()}")
             return move
         else:
             return super().parse_san(san)
 
     def has_insufficient_material(self, color: chess.Color) -> bool:
         # In practice, no material can leave the game, but this is easy to
         # implement, anyway. Note that bishops can be captured and put onto
```

### Comparing `chess-1.9.3/chess.egg-info/PKG-INFO` & `chess-1.9.4/chess.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess
-Version: 1.9.3
+Version: 1.9.4
 Summary: A chess library with move generation and validation, Polyglot opening book probing, PGN reading and writing, Gaviota tablebase probing, Syzygy tablebase probing, and XBoard/UCI engine communication.
 Home-page: https://github.com/niklasf/python-chess
 Author: Niklas Fiekas
 Author-email: niklas.fiekas@backscattering.de
 License: GPL-3.0+
 Project-URL: Documentation, https://python-chess.readthedocs.io
 Keywords: chess fen epd pgn polyglot syzygy gaviota uci xboard
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Obsoletes: python_chess
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -34,16 +35,16 @@
     :target: https://github.com/niklasf/python-chess/actions
     :alt: Test status
 
 .. image:: https://badge.fury.io/py/chess.svg
     :target: https://pypi.python.org/pypi/chess
     :alt: PyPI package
 
-.. image:: https://readthedocs.org/projects/python-chess/badge/?version=v1.9.3
-    :target: https://python-chess.readthedocs.io/en/v1.9.3/
+.. image:: https://readthedocs.org/projects/python-chess/badge/?version=v1.9.4
+    :target: https://python-chess.readthedocs.io/en/v1.9.4/
     :alt: Docs
 
 .. image:: https://badges.gitter.im/python-chess/community.svg
     :target: https://gitter.im/python-chess/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
     :alt: Chat on Gitter
 
 Introduction
@@ -91,44 +92,44 @@
 Requires Python 3.7+. Download and install the latest release:
 
 ::
 
     pip install chess
 
 
-`Documentation <https://python-chess.readthedocs.io/en/v1.9.3/>`__
+`Documentation <https://python-chess.readthedocs.io/en/v1.9.4/>`__
 --------------------------------------------------------------------
 
-* `Core <https://python-chess.readthedocs.io/en/v1.9.3/core.html>`_
-* `PGN parsing and writing <https://python-chess.readthedocs.io/en/v1.9.3/pgn.html>`_
-* `Polyglot opening book reading <https://python-chess.readthedocs.io/en/v1.9.3/polyglot.html>`_
-* `Gaviota endgame tablebase probing <https://python-chess.readthedocs.io/en/v1.9.3/gaviota.html>`_
-* `Syzygy endgame tablebase probing <https://python-chess.readthedocs.io/en/v1.9.3/syzygy.html>`_
-* `UCI/XBoard engine communication <https://python-chess.readthedocs.io/en/v1.9.3/engine.html>`_
-* `Variants <https://python-chess.readthedocs.io/en/v1.9.3/variant.html>`_
-* `Changelog <https://python-chess.readthedocs.io/en/v1.9.3/changelog.html>`_
+* `Core <https://python-chess.readthedocs.io/en/v1.9.4/core.html>`_
+* `PGN parsing and writing <https://python-chess.readthedocs.io/en/v1.9.4/pgn.html>`_
+* `Polyglot opening book reading <https://python-chess.readthedocs.io/en/v1.9.4/polyglot.html>`_
+* `Gaviota endgame tablebase probing <https://python-chess.readthedocs.io/en/v1.9.4/gaviota.html>`_
+* `Syzygy endgame tablebase probing <https://python-chess.readthedocs.io/en/v1.9.4/syzygy.html>`_
+* `UCI/XBoard engine communication <https://python-chess.readthedocs.io/en/v1.9.4/engine.html>`_
+* `Variants <https://python-chess.readthedocs.io/en/v1.9.4/variant.html>`_
+* `Changelog <https://python-chess.readthedocs.io/en/v1.9.4/changelog.html>`_
 
 Features
 --------
 
 * Includes mypy typings.
 
 * IPython/Jupyter Notebook integration.
-  `SVG rendering docs <https://python-chess.readthedocs.io/en/v1.9.3/svg.html>`_.
+  `SVG rendering docs <https://python-chess.readthedocs.io/en/v1.9.4/svg.html>`_.
 
   .. code:: python
 
       >>> board
 
   .. image:: https://backscattering.de/web-boardimage/board.png?fen=r1bqkb1r/pppp1Qpp/2n2n2/4p3/2B1P3/8/PPPP1PPP/RNB1K1NR&lastmove=h5f7&check=e8
       :alt: r1bqkb1r/pppp1Qpp/2n2n2/4p3/2B1P3/8/PPPP1PPP/RNB1K1NR
 
 * Chess variants: Standard, Chess960, Suicide, Giveaway, Atomic,
   King of the Hill, Racing Kings, Horde, Three-check, Crazyhouse.
-  `Variant docs <https://python-chess.readthedocs.io/en/v1.9.3/variant.html>`_.
+  `Variant docs <https://python-chess.readthedocs.io/en/v1.9.4/variant.html>`_.
 
 * Make and unmake moves.
 
   .. code:: python
 
       >>> Nf3 = chess.Move.from_uci("g1f3")
       >>> board.push(Nf3)  # Make the move
@@ -242,18 +243,18 @@
       >>> board.epd(bm=board.parse_uci("d2d4"))
       'rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR w KQkq - bm d4;'
 
       >>> ops = board.set_epd("1k1r4/pp1b1R2/3q2pp/4p3/2B5/4Q3/PPP2B2/2K5 b - - bm Qd1+; id \"BK.01\";")
       >>> ops == {'bm': [chess.Move.from_uci('d6d1')], 'id': 'BK.01'}
       True
 
-* Detects `absolute pins and their directions <https://python-chess.readthedocs.io/en/v1.9.3/core.html#chess.Board.pin>`_.
+* Detects `absolute pins and their directions <https://python-chess.readthedocs.io/en/v1.9.4/core.html#chess.Board.pin>`_.
 
 * Reads Polyglot opening books.
-  `Docs <https://python-chess.readthedocs.io/en/v1.9.3/polyglot.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v1.9.4/polyglot.html>`__.
 
   .. code:: python
 
       >>> import chess.polyglot
 
       >>> book = chess.polyglot.open_reader("data/polyglot/performance.bin")
 
@@ -264,15 +265,15 @@
       >>> main_entry.weight
       1
 
       >>> book.close()
 
 * Reads and writes PGNs. Supports headers, comments, NAGs and a tree of
   variations.
-  `Docs <https://python-chess.readthedocs.io/en/v1.9.3/pgn.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v1.9.4/pgn.html>`__.
 
   .. code:: python
 
       >>> import chess.pgn
 
       >>> with open("data/pgn/molinari-bordais-1979.pgn") as pgn:
       ...     first_game = chess.pgn.read_game(pgn)
@@ -285,18 +286,18 @@
       >>> first_game.mainline()
       <Mainline at ... (1. e4 c5 2. c4 Nc6 3. Ne2 Nf6 4. Nbc3 Nb4 5. g3 Nd3#)>
 
       >>> first_game.headers["Result"]
       '0-1'
 
 * Probe Gaviota endgame tablebases (DTM, WDL).
-  `Docs <https://python-chess.readthedocs.io/en/v1.9.3/gaviota.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v1.9.4/gaviota.html>`__.
 
 * Probe Syzygy endgame tablebases (DTZ, WDL).
-  `Docs <https://python-chess.readthedocs.io/en/v1.9.3/syzygy.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v1.9.4/syzygy.html>`__.
 
   .. code:: python
 
       >>> import chess.syzygy
 
       >>> tablebase = chess.syzygy.open_tablebase("data/syzygy/regular")
 
@@ -305,15 +306,15 @@
       >>> board = chess.Board("8/2K5/4B3/3N4/8/8/4k3/8 b - - 0 1")
       >>> tablebase.probe_dtz(board)
       -53
 
       >>> tablebase.close()
 
 * Communicate with UCI/XBoard engines. Based on ``asyncio``.
-  `Docs <https://python-chess.readthedocs.io/en/v1.9.3/engine.html>`__.
+  `Docs <https://python-chess.readthedocs.io/en/v1.9.4/engine.html>`__.
 
   .. code:: python
 
       >>> import chess.engine
 
       >>> engine = chess.engine.SimpleEngine.popen_uci("stockfish")
 
@@ -325,58 +326,60 @@
       >>> engine.quit()
 
 Selected projects
 -----------------
 
 If you like, share interesting things you are using python-chess for, for example:
 
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/syzygy.png?raw=true       | https://syzygy-tables.info/                                                             |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://syzygy-tables.info/                                                             | A website to probe Syzygy endgame tablebases                                            |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/maia.png?raw=true         | https://maiachess.com/                                                                  |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://maiachess.com/                                                                  | A human-like neural network chess engine                                                |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/clente-chess.png?raw=true | `clente/chess <https://github.com/clente/chess>`_                                       |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://github.com/clente/chess                                                         | Oppinionated wrapper to use python-chess from the R programming language                |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/crazyara.png?raw=true     | https://crazyara.org/                                                                   |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: https://crazyara.org/                                                                   | Deep learning for Crazyhouse                                                            |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/jcchess.png?raw=true      | `http://johncheetham.com <http://johncheetham.com/projects/jcchess/>`_                  |
-|     :height: 64                                                                                      |                                                                                         |
-|     :width: 64                                                                                       |                                                                                         |
-|     :target: http://johncheetham.com/projects/jcchess/                                               | A GUI to play against UCI chess engines                                                 |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
-| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/pettingzoo.png?raw=true   | `https://www.pettingzoo.ml <https://www.pettingzoo.ml/classic/chess>`_                  |
-|     :width: 64                                                                                       |                                                                                         |
-|     :height: 64                                                                                      |                                                                                         |
-|     :target: https://www.pettingzoo.ml/classic/chess                                                 | A multi-agent reinforcement learning environment                                        |
-+------------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------+
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/syzygy.png?raw=true       | https://syzygy-tables.info/                                                                  |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://syzygy-tables.info/                                                             | A website to probe Syzygy endgame tablebases                                                 |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/maia.png?raw=true         | https://maiachess.com/                                                                       |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://maiachess.com/                                                                  | A human-like neural network chess engine                                                     |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/clente-chess.png?raw=true | `clente/chess <https://github.com/clente/chess>`_                                            |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://github.com/clente/chess                                                         | Oppinionated wrapper to use python-chess from the R programming language                     |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/crazyara.png?raw=true     | https://crazyara.org/                                                                        |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: https://crazyara.org/                                                                   | Deep learning for Crazyhouse                                                                 |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/jcchess.png?raw=true      | `http://johncheetham.com <http://johncheetham.com/projects/jcchess/>`_                       |
+|     :height: 64                                                                                      |                                                                                              |
+|     :width: 64                                                                                       |                                                                                              |
+|     :target: http://johncheetham.com/projects/jcchess/                                               | A GUI to play against UCI chess engines                                                      |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
+| .. image:: https://github.com/niklasf/python-chess/blob/master/docs/images/pettingzoo.png?raw=true   | `https://pettingzoo.farama.org <https://pettingzoo.farama.org/environments/classic/chess/>`_ |
+|     :width: 64                                                                                       |                                                                                              |
+|     :height: 64                                                                                      |                                                                                              |
+|     :target: https://pettingzoo.farama.org/environments/classic/chess/                               | A multi-agent reinforcement learning environment                                             |
++------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------+
 
 * extensions to build engines (search and evaluation) – https://github.com/Mk-Chan/python-chess-engine-extensions
 * a stand-alone chess computer based on DGT board – http://www.picochess.org/
 * a bridge between Lichess API and chess engines – https://github.com/careless25/lichess-bot
 * a command-line PGN annotator – https://github.com/rpdelaney/python-chess-annotator
 * an HTTP microservice to render board images – https://github.com/niklasf/web-boardimage
 * building a toy chess engine with alpha-beta pruning, piece-square tables, and move ordering – https://healeycodes.com/building-my-own-chess-engine/
 * a JIT compiled chess engine – https://github.com/SamRagusa/Batch-First
 * teaching Cognitive Science – `https://jupyter.brynmawr.edu <https://jupyter.brynmawr.edu/services/public/dblank/CS371%20Cognitive%20Science/2016-Fall/Programming%20a%20Chess%20Player.ipynb>`_
 * an `Alexa skill to play blindfold chess <https://www.amazon.com/Laynr-blindfold-chess/dp/B0859QF8YL>`_ – https://github.com/laynr/blindfold-chess
 * a chessboard widget for PySide2 – https://github.com/H-a-y-k/hichesslib
 * Django Rest Framework API for multiplayer chess – https://github.com/WorkShoft/capablanca-api
 * a `browser based PGN viewer <https://about.nmstoker.com/chess2.html>`_ written in PyScript – https://github.com/nmstoker/ChessMatchViewer
+* an accessible chessboard that allows blind and visually impaired  players  to play chess against Stockfish – https://github.com/blindpandas/chessmart
+
 
 Acknowledgements
 ----------------
 
 Thanks to the Stockfish authors and thanks to Sam Tannous for publishing his
 approach to `avoid rotated bitboards with direct lookup (PDF) <http://arxiv.org/pdf/0704.3773.pdf>`_
 alongside his GPL2+ engine `Shatranj <https://github.com/stannous/shatranj>`_.
```

### Comparing `chess-1.9.3/setup.py` & `chess-1.9.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Games/Entertainment :: Board Games",
         "Topic :: Games/Entertainment :: Turn Based Strategy",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Typing :: Typed",
     ],
     project_urls={
         "Documentation": "https://python-chess.readthedocs.io",
```

