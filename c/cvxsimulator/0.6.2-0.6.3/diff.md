# Comparing `tmp/cvxsimulator-0.6.2.tar.gz` & `tmp/cvxsimulator-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.6.2.tar", max compression
+gzip compressed data, was "cvxsimulator-0.6.3.tar", max compression
```

## Comparing `cvxsimulator-0.6.2.tar` & `cvxsimulator-0.6.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    10790 2023-07-14 22:59:44.301752 cvxsimulator-0.6.2/LICENSE
--rw-r--r--   0        0        0     5690 2023-07-14 22:59:44.301752 cvxsimulator-0.6.2/README.md
--rw-r--r--   0        0        0        0 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    17055 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1613 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1457 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/month.py
--rw-r--r--   0        0        0    23577 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      795 2023-07-14 22:59:44.389752 cvxsimulator-0.6.2/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      895 2023-07-14 23:00:18.521510 cvxsimulator-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     6308 1970-01-01 00:00:00.000000 cvxsimulator-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    10790 2023-07-27 03:11:23.671758 cvxsimulator-0.6.3/LICENSE
+-rw-r--r--   0        0        0     5741 2023-07-27 03:11:23.671758 cvxsimulator-0.6.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-27 03:11:23.747761 cvxsimulator-0.6.3/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    15121 2023-07-27 03:11:23.747761 cvxsimulator-0.6.3/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1613 2023-07-27 03:11:23.747761 cvxsimulator-0.6.3/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1559 2023-07-27 03:11:23.747761 cvxsimulator-0.6.3/cvx/simulator/month.py
+-rw-r--r--   0        0        0    23615 2023-07-27 03:11:23.751763 cvxsimulator-0.6.3/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      795 2023-07-27 03:11:23.751763 cvxsimulator-0.6.3/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0     1114 2023-07-27 03:11:59.242169 cvxsimulator-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 cvxsimulator-0.6.3/PKG-INFO
```

### Comparing `cvxsimulator-0.6.2/LICENSE` & `cvxsimulator-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.2/README.md` & `cvxsimulator-0.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,37 @@
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.png?branch=main)](https://coveralls.io/github/cvxgrp/simulator?branch=main)
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/cvxgrp/simulator)
 
-Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$,
-e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
-
-In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
-This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
+Given a universe of $m$ assets we are given prices for each of them at
+time $t_1, t_2, \ldots t_n$, e.g. we operate using an $n \times m$ matrix where
+each column corresponds to a particular asset.
+
+In a backtest we iterate in time (e.g. row by row) through the matrix and
+allocate positions to all or some of the assets. This tool shall help to
+simplify the accounting. It keeps track of the available cash,
+the profits achieved, etc.
 
 ## Creating portfolios
 
 The simulator shall be completely agnostic as to the trading policy/strategy.
 Our approach follows a rather common pattern:
 
 * [Create the builder object](#create-the-builder-object)
 * [Loop through time](#loop-through-time)
 * [Build the portfolio](#build-the-portfolio)
 
-We demonstrate those steps with somewhat silly policies. They are never good strategies, but are always valid ones.
+We demonstrate those steps with somewhat silly policies.
+They are never good strategies, but are always valid ones.
 
-Of course, some users may know prices and weights in advance. In that case, the building procedure can be bypassed.
+Of course, some users may know prices and weights in advance.
+In that case, the building procedure can be bypassed.
 We discuss this in
 
 * [Bypassing the builder](#bypassing-the-builder)
 
 ### Create the builder object
 
 The user defines a builder object by loading a frame of prices
@@ -36,27 +41,29 @@
 
 ```python
 from pathlib import Path
 
 import pandas as pd
 from cvx.simulator.builder import builder
 
-prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
+prices = pd.read_csv(Path("resources") / "price.csv",
+                     index_col=0, parse_dates=True, header=0).ffill()
 b = builder(prices=prices, initial_cash=1e6)
 ```
 
 It is also possible to specify a model for trading costs.
 The builder helps to fill up the frame of positions. Only once done
 we construct the actual portfolio.
 
 ### Loop through time
 
-We have overloaded the `__iter__` and `__setitem__` methods to create a custom loop.
-Let's start with a first strategy. Each day we choose two names from the universe at random.
-Buy one (say 0.1 of your portfolio wealth) and short one the same amount.
+We have overloaded the `__iter__` and `__setitem__` methods
+to create a custom loop. Let's start with a first strategy. Each day we choose
+two names from the universe at random. Buy one (say 0.1 of your
+portfolio wealth) and short one the same amount.
 
 ```python
 for t, state in b:
     # pick two assets at random
     pair = np.random.choice(b.assets, 2, replace=False)
     # compute the pair
     stocks = pd.Series(index=b.assets, data=0.0)
@@ -65,17 +72,19 @@
     b[t[-1]] = 0.1 * stocks
 ```
 
 Here t is the growing list of timestamps, e.g. in the first iteration
 t is $t1$, in the second iteration it will be $t1, t2$ etc.
 
 A lot of magic is hidden in the state variable.
-The state gives access to the currently available cash, the current prices and the current valuation of all holdings.
+The state gives access to the currently available cash, the current prices
+and the current valuation of all holdings.
 
-Here's a slightly more realistic loop. Given a set of $4$ assets we want to implmenent the popular $1/n$ strategy.
+Here's a slightly more realistic loop. Given a set of $4$ assets we want to
+implmenent the popular $1/n$ strategy.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b[t[-1]] = 0.25 * state.nav / state.prices
 ```
 
@@ -98,75 +107,76 @@
 ```
 
 ### Bypassing the builder
 
 Some may know the positions the portfolio shall enter for eternity.
 Running through a loop is rather non-pythonic waste of time in such a case.
 It is possible to completely bypass this step by submitting
-a frame of positions together with a frame of prices when creating the portfolio object.
+a frame of positions together with a frame of prices when creating the
+portfolio object.
 
 ```python
 from pathlib import Path
 
 import pandas as pd
 from cvx.simulator.portfolio import EquityPortfolio
 
-prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
-stocks = pd.read_csv(Path("resources") / "stock.csv", index_col=0, parse_dates=True, header=0)
+prices = pd.read_csv(Path("resources") / "price.csv",
+                     index_col=0, parse_dates=True, header=0).ffill()
+stocks = pd.read_csv(Path("resources") / "stock.csv",
+                     index_col=0, parse_dates=True, header=0)
 portfolio = EquityPortfolio(prices=prices, stocks=stocks, initial_cash=1e6)
 ```
 
-
 ## Analytics
 
 The portfolio object supports further analysis and exposes
 a number of properties, e.g.
 
 ```python
 portfolio.nav
 portfolio.cash
 portfolio.equity
 ```
 
-We have also integrated the [quantstats](https://github.com/ranaroussi/quantstats) package for further analysis.
-Hence it is possible to perform
+We have also integrated the [quantstats](https://github.com/ranaroussi/quantstats)
+package for further analysis. Hence it is possible to perform
 
 ```python
 portfolio.snapshot()
 portfolio.metrics()
 portfolio.plots()
 portfolio.html()
 ```
 
 We also added an enum
 
-
 ```python
 portfolio.plot(kind=Plot.DRAWDOWN)
 ```
 
 supporting all plots defined in quantstats.
 
 ![quantstats snapshot](portfolio.png)
 
-
-
-
 ## Poetry
 
-We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
+We assume you share already the love for [Poetry](https://python-poetry.org).
+Once you have installed poetry you can perform
 
 ```bash
 poetry install
 ```
 
 to replicate the virtual environment we have defined in pyproject.toml.
 
 ## Kernel
 
-We install [JupyterLab](https://jupyter.org) within your new virtual environment. Executing
+We install [JupyterLab](https://jupyter.org) within your new virtual
+environment. Executing
 
 ```bash
-./create_kernel.sh
+make kernel
 ```
 
-constructs a dedicated [Kernel](https://docs.jupyter.org/en/latest/projects/kernels.html) for the project.
+constructs a dedicated [Kernel](https://docs.jupyter.org/en/latest/projects/kernels.html)
+for the project.
```

### Comparing `cvxsimulator-0.6.2/cvx/simulator/builder.py` & `cvxsimulator-0.6.3/cvx/simulator/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,164 +1,139 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+from typing import Optional
 
 import pandas as pd
 
 from cvx.simulator.portfolio import EquityPortfolio
 from cvx.simulator.trading_costs import TradingCostModel
 
 
 @dataclass
 class _State:
-    """The _State class defines a state object used to keep track of the current state of the portfolio.
+    """The _State class defines a state object used to keep track of the current
+    state of the portfolio.
+
     Attributes:
 
-    prices: a pandas Series object containing the stock prices of the current portfolio state
+    prices: a pandas Series object containing the stock prices of the current
+    portfolio state
+
     position: a pandas Series object containing the current holdings of the portfolio
+
     cash: the amount of cash available in the portfolio.
 
     By default, prices and position are set to None, while cash is set to 1 million.
     These attributes can be updated and accessed through setter and getter methods
     """
 
     prices: pd.Series = None
     position: pd.Series = None
     cash: float = 1e6
 
     @property
     def value(self):
         """
-        The value method computes the value of the portfolio at the current time,
-        taking into account the current holdings and current stock prices.
-
-
-        Returns:
-
-        the value of the portfolio as a float. If the value cannot be computed due to missing position
+        The value property computes the value of the portfolio at the current
+        time taking into account the current holdings and current stock prices.
+        If the value cannot be computed due to missing positions
         (they might be still None), zero is returned instead.
-
-        The method is a decorator-based getter method, using the @property decorator to access
-        the value attribute as if it were a method. The value of the portfolio is computed as the
-        product of the current stock prices and the current holdings, summed together.
-        Note that if the current position is missing, the multiplication will raise a TypeError.
-        In this case, zero is returned as the value of the portfolio.
         """
-        # Note that the first position may not exist yet.
         try:
             return (self.prices * self.position).sum()
         except TypeError:
             return 0.0
 
     @property
     def nav(self):
         """
-        The nav method computes the net asset value (NAV) of the portfolio,
+        The nav property computes the net asset value (NAV) of the portfolio,
         which is the sum of the current value of the
-        portfolio as determined by the value method,
+        portfolio as determined by the value property,
         and the current amount of cash available in the portfolio.
-
-        Returns:
-
-        The net asset value of the portfolio as a float, computed as the sum of the current
-        value of the portfolio and the cash available in the portfolio.
-        The method is a decorator-based getter method using the @property decorator
-        to access the NAV attribute as if it were a method.
-        The NAV is computed as the sum of the current value (as computed by the value method)
-        and the amount of cash available.
         """
         return self.value + self.cash
 
     @property
     def weights(self):
         """
-        The weights method computes the weighting of each asset in the current portfolio
-        as a fraction of the total portfolio value.
+        The weights property computes the weighting of each asset in the current
+        portfolio as a fraction of the total portfolio value (nav).
 
         Returns:
 
-        a pandas series object containing the weighting of each asset as a fraction
-        of the total portfolio value. If the positions are still missing, then a series of zeroes is returned.
-        The method is a decorator-based getter method using the @property decorator to access
-        the weights attribute as if it were a method. The weighting for each asset is computed
-        as the product of the current position and the current stock prices,
-        divided by the net asset value of the portfolio (as computed by the nav method).
-        Note that this weighting represents the fraction of the portfolio value allocated to a particular asset.
-        If the portfolio weighting cannot be computed due to missing positions,
-        then a series of zeroes with the same size as the prices attribute is returned instead.
+        a pandas series object containing the weighting of each asset as a
+        fraction of the total portfolio value. If the positions are still
+        missing, then a series of zeroes is returned.
         """
         try:
             return (self.prices * self.position) / self.nav
         except TypeError:
             return 0 * self.prices
 
     @property
     def leverage(self):
         """
-        The `leverage` method computes the leverage of the portfolio,
+        The `leverage` property computes the leverage of the portfolio,
         which is the sum of the absolute values of the portfolio weights.
-
-        Returns:
-        - the portfolio leverage as a float, computed as the sum of the
-        absolute values of the portfolio weights.
-
-        The method is a decorator-based getter method using the
-        `@property` decorator to access the leverage attribute
-        as if it were a method. The portfolio leverage is computed as
-        the sum of the absolute values of the portfolio weights,
-        which represents the total exposure of the portfolio to multiple assets.
         """
         return self.weights.abs().sum()
 
     @property
     def position_robust(self):
+        """
+        The position_robust property returns the current position of the
+        portfolio or a series of zeroes if the position is still missing.
+        """
         if self.position is None:
             self.position = 0.0 * self.prices
 
         return self.position
 
     def update(self, position, model=None, **kwargs):
         """
-        The update method updates the current state of the portfolio with the new input position.
-        It calculates the trades made based on the new and the previous position,
-        updates the internal position and cash attributes,
-        and applies any applicable trading costs according to model parameter.
+        The update method updates the current state of the portfolio with the
+        new input position. It calculates the trades made based on the new
+        and the previous position, updates the internal position and
+        cash attributes, and applies any trading costs according to a model parameter.
 
         The method takes three input parameters:
 
-        position: a pandas series object representing the new position of the portfolio.
-        model: an optional trading cost model (e.g. slippage, fees) to be incorporated into the update.
-        If None, no trading costs will be applied.
-        **kwargs: additional keyword arguments to pass into the trading cost model.
+        position: a pandas series object representing the new position of the
+        portfolio.
+
+        model: an optional trading cost model (e.g. slippage, fees) to be
+        incorporated into the update. If None, no trading costs will be applied.
+
+        **kwargs: additional keyword arguments to pass into the trading cost
+        model.
 
         Returns:
         self: the _State instance with the updated position and cash.
 
         Updates:
 
         trades: the difference between positions in the old and new portfolio.
         position: the new position of the portfolio.
         cash: the new amount of cash in the portfolio after any trades and trading costs are applied.
 
         Note that the method does not return any value: instead,
         it updates the internal state of the _State instance.
         """
-        # if self.position is None:
-        #    self.position = 0.0 * position
-        # trades = position
-        # else:
         trades = position - self.position_robust
 
         self.position = position
         self.cash -= (trades * self.prices).sum()
 
         if model is not None:
             self.cash -= model.eval(self.prices, trades=trades, **kwargs).sum()
 
+        # builder is frozen, so we can't construct a new state
         return self
 
 
 def builder(
     prices,
     weights=None,
     market_cap=None,
@@ -216,18 +191,18 @@
     prices: pd.DataFrame
     stocks: pd.DataFrame
     trading_cost_model: TradingCostModel
     initial_cash: float = 1e6
     _state: _State = field(default_factory=_State)
     market_cap: pd.DataFrame = None
     trade_volume: pd.DataFrame = None
-    max_cap_fraction: float = None
-    min_cap_fraction: float = None
-    max_trade_fraction: float = None
-    min_trade_fraction: float = None
+    max_cap_fraction: Optional[float] = None
+    min_cap_fraction: Optional[float] = None
+    max_trade_fraction: Optional[float] = None
+    min_trade_fraction: Optional[float] = None
 
     def __post_init__(self):
         """
         The __post_init__ method is a special method of initialized instances
         of the _Builder class and is called after initialization.
         It sets the initial amount of cash in the portfolio to be equal to the input initial_cash parameter.
```

### Comparing `cvxsimulator-0.6.2/cvx/simulator/grid.py` & `cvxsimulator-0.6.3/cvx/simulator/grid.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.2/cvx/simulator/portfolio.py` & `cvxsimulator-0.6.3/cvx/simulator/portfolio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
+from typing import Optional
 
 import pandas as pd
 import quantstats as qs
 
 from cvx.simulator.grid import iron_frame
 from cvx.simulator.trading_costs import TradingCostModel
 
@@ -78,15 +79,15 @@
     If no trading cost model is provided, the trading_cost_model attribute
     will be set to None by default.
     If no initial cash value is provided, the initial_cash attribute
     will be set to a default value of 1,000,000."""
 
     prices: pd.DataFrame
     stocks: pd.DataFrame
-    trading_cost_model: TradingCostModel = None
+    trading_cost_model: Optional[TradingCostModel] = None
     initial_cash: float = 1e6
 
     def __post_init__(self):
         """A class method that performs input validation after object initialization.
         Notes: The post_init method is called after an instance of the EquityPortfolio class has been initialized,
         and performs a series of input validation checks to ensure that the prices
         and stocks dataframes are in the expected format
```

### Comparing `cvxsimulator-0.6.2/cvx/simulator/trading_costs.py` & `cvxsimulator-0.6.3/cvx/simulator/trading_costs.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.6.2/pyproject.toml` & `cvxsimulator-0.6.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.6.2"
+version = "v0.6.3"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.8,<3.12"
 numpy = "*"
 pandas = "*"
 quantstats = "*"
+pandas-stubs = "*"
 
 [tool.poetry.group.test.dependencies]
 pytest = "7.2.0"
 pytest-cov = "4.0.0"
 mock = "*"
 
 [tool.poetry.group.jupyter.dependencies]
 jupyterlab = "*"
 jupyter-book = "0.15.1"
+pyyaml = "6.0"
 
 [tool.peotry.group.linting.dependencies]
 pylint = "*"
 ruff = "0.0.277"
 pre-commit = "*"
 black = "23.3.0"
 
 
 [tool.poetry.group.dev.dependencies]
 yfinance = "*"
 plotly = "*"
 cvxpy = "*"
 loguru = "*"
 
+
+[tool.poetry.group.stubs.dependencies]
+mypy = "*"
+pandas-stubs = "*"
+#pandera = {version="*", extras = ["mypy"]}
+
+[tool.mypy]
+files = ["cvx/simulator"]
+explicit_package_bases = true
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = ["E", "F", "I"]
 line-length = 120
```

### Comparing `cvxsimulator-0.6.2/PKG-INFO` & `cvxsimulator-0.6.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.6.2
+Version: 0.6.3
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: pandas-stubs
 Requires-Dist: quantstats
 Project-URL: Repository, https://github.com/cvxgrp/simulator
 Description-Content-Type: text/markdown
 
 # [cvxsimulator](https://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
 [![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.png?branch=main)](https://coveralls.io/github/cvxgrp/simulator?branch=main)
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/cvxgrp/simulator)
 
-Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$,
-e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
-
-In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
-This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
+Given a universe of $m$ assets we are given prices for each of them at
+time $t_1, t_2, \ldots t_n$, e.g. we operate using an $n \times m$ matrix where
+each column corresponds to a particular asset.
+
+In a backtest we iterate in time (e.g. row by row) through the matrix and
+allocate positions to all or some of the assets. This tool shall help to
+simplify the accounting. It keeps track of the available cash,
+the profits achieved, etc.
 
 ## Creating portfolios
 
 The simulator shall be completely agnostic as to the trading policy/strategy.
 Our approach follows a rather common pattern:
 
 * [Create the builder object](#create-the-builder-object)
 * [Loop through time](#loop-through-time)
 * [Build the portfolio](#build-the-portfolio)
 
-We demonstrate those steps with somewhat silly policies. They are never good strategies, but are always valid ones.
+We demonstrate those steps with somewhat silly policies.
+They are never good strategies, but are always valid ones.
 
-Of course, some users may know prices and weights in advance. In that case, the building procedure can be bypassed.
+Of course, some users may know prices and weights in advance.
+In that case, the building procedure can be bypassed.
 We discuss this in
 
 * [Bypassing the builder](#bypassing-the-builder)
 
 ### Create the builder object
 
 The user defines a builder object by loading a frame of prices
@@ -54,27 +60,29 @@
 
 ```python
 from pathlib import Path
 
 import pandas as pd
 from cvx.simulator.builder import builder
 
-prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
+prices = pd.read_csv(Path("resources") / "price.csv",
+                     index_col=0, parse_dates=True, header=0).ffill()
 b = builder(prices=prices, initial_cash=1e6)
 ```
 
 It is also possible to specify a model for trading costs.
 The builder helps to fill up the frame of positions. Only once done
 we construct the actual portfolio.
 
 ### Loop through time
 
-We have overloaded the `__iter__` and `__setitem__` methods to create a custom loop.
-Let's start with a first strategy. Each day we choose two names from the universe at random.
-Buy one (say 0.1 of your portfolio wealth) and short one the same amount.
+We have overloaded the `__iter__` and `__setitem__` methods
+to create a custom loop. Let's start with a first strategy. Each day we choose
+two names from the universe at random. Buy one (say 0.1 of your
+portfolio wealth) and short one the same amount.
 
 ```python
 for t, state in b:
     # pick two assets at random
     pair = np.random.choice(b.assets, 2, replace=False)
     # compute the pair
     stocks = pd.Series(index=b.assets, data=0.0)
@@ -83,17 +91,19 @@
     b[t[-1]] = 0.1 * stocks
 ```
 
 Here t is the growing list of timestamps, e.g. in the first iteration
 t is $t1$, in the second iteration it will be $t1, t2$ etc.
 
 A lot of magic is hidden in the state variable.
-The state gives access to the currently available cash, the current prices and the current valuation of all holdings.
+The state gives access to the currently available cash, the current prices
+and the current valuation of all holdings.
 
-Here's a slightly more realistic loop. Given a set of $4$ assets we want to implmenent the popular $1/n$ strategy.
+Here's a slightly more realistic loop. Given a set of $4$ assets we want to
+implmenent the popular $1/n$ strategy.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b[t[-1]] = 0.25 * state.nav / state.prices
 ```
 
@@ -116,76 +126,77 @@
 ```
 
 ### Bypassing the builder
 
 Some may know the positions the portfolio shall enter for eternity.
 Running through a loop is rather non-pythonic waste of time in such a case.
 It is possible to completely bypass this step by submitting
-a frame of positions together with a frame of prices when creating the portfolio object.
+a frame of positions together with a frame of prices when creating the
+portfolio object.
 
 ```python
 from pathlib import Path
 
 import pandas as pd
 from cvx.simulator.portfolio import EquityPortfolio
 
-prices = pd.read_csv(Path("resources") / "price.csv", index_col=0, parse_dates=True, header=0).ffill()
-stocks = pd.read_csv(Path("resources") / "stock.csv", index_col=0, parse_dates=True, header=0)
+prices = pd.read_csv(Path("resources") / "price.csv",
+                     index_col=0, parse_dates=True, header=0).ffill()
+stocks = pd.read_csv(Path("resources") / "stock.csv",
+                     index_col=0, parse_dates=True, header=0)
 portfolio = EquityPortfolio(prices=prices, stocks=stocks, initial_cash=1e6)
 ```
 
-
 ## Analytics
 
 The portfolio object supports further analysis and exposes
 a number of properties, e.g.
 
 ```python
 portfolio.nav
 portfolio.cash
 portfolio.equity
 ```
 
-We have also integrated the [quantstats](https://github.com/ranaroussi/quantstats) package for further analysis.
-Hence it is possible to perform
+We have also integrated the [quantstats](https://github.com/ranaroussi/quantstats)
+package for further analysis. Hence it is possible to perform
 
 ```python
 portfolio.snapshot()
 portfolio.metrics()
 portfolio.plots()
 portfolio.html()
 ```
 
 We also added an enum
 
-
 ```python
 portfolio.plot(kind=Plot.DRAWDOWN)
 ```
 
 supporting all plots defined in quantstats.
 
 ![quantstats snapshot](portfolio.png)
 
-
-
-
 ## Poetry
 
-We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
+We assume you share already the love for [Poetry](https://python-poetry.org).
+Once you have installed poetry you can perform
 
 ```bash
 poetry install
 ```
 
 to replicate the virtual environment we have defined in pyproject.toml.
 
 ## Kernel
 
-We install [JupyterLab](https://jupyter.org) within your new virtual environment. Executing
+We install [JupyterLab](https://jupyter.org) within your new virtual
+environment. Executing
 
 ```bash
-./create_kernel.sh
+make kernel
 ```
 
-constructs a dedicated [Kernel](https://docs.jupyter.org/en/latest/projects/kernels.html) for the project.
+constructs a dedicated [Kernel](https://docs.jupyter.org/en/latest/projects/kernels.html)
+for the project.
```

