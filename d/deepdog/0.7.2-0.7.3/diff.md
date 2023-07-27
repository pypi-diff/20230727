# Comparing `tmp/deepdog-0.7.2.tar.gz` & `tmp/deepdog-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepdog-0.7.2.tar", max compression
+gzip compressed data, was "deepdog-0.7.3.tar", max compression
```

## Comparing `deepdog-0.7.2.tar` & `deepdog-0.7.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      605 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/__init__.py
--rw-r--r--   0        0        0     8197 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/bayes_run.py
--rw-r--r--   0        0        0    11705 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/bayes_run_simulpairs.py
--rw-r--r--   0        0        0     6778 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/bayes_run_with_ss.py
--rw-r--r--   0        0        0       73 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/meta.py
--rw-r--r--   0        0        0     8471 2023-07-24 15:47:03.783448 deepdog-0.7.2/deepdog/real_spectrum_run.py
--rw-r--r--   0        0        0      110 2023-07-24 15:47:03.787449 deepdog-0.7.2/deepdog/subset_simulation/__init__.py
--rw-r--r--   0        0        0     8754 2023-07-24 15:47:03.787449 deepdog-0.7.2/deepdog/subset_simulation/subset_simulation_impl.py
--rw-r--r--   0        0        0     6794 2023-07-24 15:47:03.787449 deepdog-0.7.2/deepdog/temp_aware_real_spectrum_run.py
--rw-r--r--   0        0        0      898 2023-07-24 15:47:03.787449 deepdog-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      662 2023-07-24 15:48:06.191608 deepdog-0.7.2/setup.py
--rw-r--r--   0        0        0      361 2023-07-24 15:48:06.191916 deepdog-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      605 2023-07-27 01:28:09.712641 deepdog-0.7.3/deepdog/__init__.py
+-rw-r--r--   0        0        0     8197 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/bayes_run.py
+-rw-r--r--   0        0        0    11705 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/bayes_run_simulpairs.py
+-rw-r--r--   0        0        0     6973 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/bayes_run_with_ss.py
+-rw-r--r--   0        0        0       73 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/meta.py
+-rw-r--r--   0        0        0     8471 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/real_spectrum_run.py
+-rw-r--r--   0        0        0      110 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/subset_simulation/__init__.py
+-rw-r--r--   0        0        0     9657 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/subset_simulation/subset_simulation_impl.py
+-rw-r--r--   0        0        0     6794 2023-07-27 01:28:09.716642 deepdog-0.7.3/deepdog/temp_aware_real_spectrum_run.py
+-rw-r--r--   0        0        0      898 2023-07-27 01:28:09.716642 deepdog-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      662 2023-07-27 01:29:16.137585 deepdog-0.7.3/setup.py
+-rw-r--r--   0        0        0      361 2023-07-27 01:29:16.137938 deepdog-0.7.3/PKG-INFO
```

### Comparing `deepdog-0.7.2/deepdog/__init__.py` & `deepdog-0.7.3/deepdog/__init__.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.2/deepdog/bayes_run.py` & `deepdog-0.7.3/deepdog/bayes_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.2/deepdog/bayes_run_simulpairs.py` & `deepdog-0.7.3/deepdog/bayes_run_simulpairs.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.2/deepdog/bayes_run_with_ss.py` & `deepdog-0.7.3/deepdog/bayes_run_with_ss.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 		ss_mcmc_seed: int = 20,
 		ss_use_adaptive_steps=True,
 		ss_default_phi_step=0.01,
 		ss_default_theta_step=0.01,
 		ss_default_r_step=0.01,
 		ss_default_w_log_step=0.01,
 		ss_default_upper_w_log_step=4,
+		ss_dump_last_generation=False,
 	) -> None:
 		self.dot_inputs = pdme.inputs.inputs_with_frequency_range(
 			dot_positions, frequency_range
 		)
 		self.dot_inputs_array = pdme.measurement.input_types.dot_inputs_to_array(
 			self.dot_inputs
 		)
@@ -129,14 +130,15 @@
 		self.ss_mcmc_seed = ss_mcmc_seed
 		self.ss_use_adaptive_steps = ss_use_adaptive_steps
 		self.ss_default_phi_step = ss_default_phi_step
 		self.ss_default_theta_step = ss_default_theta_step
 		self.ss_default_r_step = ss_default_r_step
 		self.ss_default_w_log_step = ss_default_w_log_step
 		self.ss_default_upper_w_log_step = ss_default_upper_w_log_step
+		self.ss_dump_last_generation = ss_dump_last_generation
 
 		self.run_count = run_count
 
 	def go(self) -> None:
 		with open(self.filename, "a", newline="") as outfile:
 			writer = csv.DictWriter(outfile, fieldnames=self.csv_fields, dialect="unix")
 			writer.writeheader()
@@ -168,14 +170,16 @@
 					self.ss_mcmc_seed,
 					self.ss_use_adaptive_steps,
 					self.ss_default_phi_step,
 					self.ss_default_theta_step,
 					self.ss_default_r_step,
 					self.ss_default_w_log_step,
 					self.ss_default_upper_w_log_step,
+					keep_probs_list=False,
+					dump_last_generation_to_file=self.ss_dump_last_generation,
 				)
 				results.append(subset_run.execute())
 
 			_logger.debug("Done, constructing output now")
 			row = {
 				"dipole_moment_1": actual_dipoles.dipoles[0].p,
 				"dipole_location_1": actual_dipoles.dipoles[0].s,
@@ -192,15 +196,17 @@
 					break
 
 			likelihoods: List[float] = []
 
 			for (name, result) in zip(self.model_names, results):
 				if result.over_target_likelihood is None:
 					clamped_likelihood = result.probs_list[-1][0] / CLAMPING_FACTOR
-					_logger.warning(f"got a none result, clamping to {clamped_likelihood}")
+					_logger.warning(
+						f"got a none result, clamping to {clamped_likelihood}"
+					)
 				else:
 					clamped_likelihood = result.over_target_likelihood
 				likelihoods.append(clamped_likelihood)
 				row[f"{name}_likelihood"] = clamped_likelihood
 
 			success_weight = sum(
 				[
```

### Comparing `deepdog-0.7.2/deepdog/real_spectrum_run.py` & `deepdog-0.7.3/deepdog/real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.2/deepdog/subset_simulation/subset_simulation_impl.py` & `deepdog-0.7.3/deepdog/subset_simulation/subset_simulation_impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 @dataclass
 class SubsetSimulationResult:
 	probs_list: Sequence[Tuple]
 	over_target_cost: Optional[float]
 	over_target_likelihood: Optional[float]
 	under_target_cost: Optional[float]
 	under_target_likelihood: Optional[float]
+	lowest_likelihood: Optional[float]
 
 
 class SubsetSimulation:
 	def __init__(
 		self,
 		model_name_pair,
 		dot_inputs,
@@ -33,14 +34,16 @@
 		mcmc_seed: int = 20,
 		use_adaptive_steps=True,
 		default_phi_step=0.01,
 		default_theta_step=0.01,
 		default_r_step=0.01,
 		default_w_log_step=0.01,
 		default_upper_w_log_step=4,
+		keep_probs_list=True,
+		dump_last_generation_to_file=False,
 	):
 		name, model = model_name_pair
 		self.model_name = name
 		self.model = model
 		_logger.info(f"got model {self.model_name}")
 
 		self.dot_inputs_array = pdme.measurement.input_types.dot_inputs_to_array(
@@ -75,14 +78,17 @@
 		_logger.info(f"\tn_s: {self.n_s}")
 		_logger.info(f"\tm: {self.m_max}")
 		_logger.info("let's do level 0...")
 
 		self.target_cost = target_cost
 		_logger.info(f"will stop at target cost {target_cost}")
 
+		self.keep_probs_list = keep_probs_list
+		self.dump_last_generations = dump_last_generation_to_file
+
 	def execute(self) -> SubsetSimulationResult:
 
 		probs_list = []
 
 		sample_dipoles = self.model.get_monte_carlo_dipole_inputs(
 			self.n_c * self.n_s,
 			-1,
@@ -112,23 +118,35 @@
 		all_chains = list(zip(sorted_costs, all_dipoles))
 
 		mcmc_rng = numpy.random.default_rng(self.mcmc_seed)
 
 		for i in range(self.m_max):
 			next_seeds = all_chains[-self.n_c:]
 
-			for cost_index, cost_chain in enumerate(all_chains[: -self.n_c]):
-				probs_list.append(
-					(
-						((self.n_c * self.n_s - cost_index) / (self.n_c * self.n_s))
-						/ (self.n_s ** (i)),
-						cost_chain[0],
-						i + 1,
+			if self.dump_last_generations:
+				_logger.info("writing out csv file")
+				next_dipoles_seed_dipoles = numpy.array([n[1] for n in next_seeds])
+				for n in range(self.model.n):
+					_logger.info(f"{next_dipoles_seed_dipoles[:, n].shape}")
+					numpy.savetxt(
+						f"generation_{self.n_c}_{self.n_s}_{i}_dipole_{n}.csv",
+						next_dipoles_seed_dipoles[:, n],
+						delimiter=",",
+					)
+
+			if self.keep_probs_list:
+				for cost_index, cost_chain in enumerate(all_chains[: -self.n_c]):
+					probs_list.append(
+						(
+							((self.n_c * self.n_s - cost_index) / (self.n_c * self.n_s))
+							/ (self.n_s ** (i)),
+							cost_chain[0],
+							i + 1,
+						)
 					)
-				)
 
 			next_seeds_as_array = numpy.array([s for _, s in next_seeds])
 
 			stdevs = self.get_stdevs_from_arrays(next_seeds_as_array)
 			_logger.info(f"got stdevs: {stdevs.stdevs}")
 
 			all_chains = []
@@ -165,66 +183,76 @@
 				)
 
 				cost_list = [c[0] for c in all_chains]
 				over_index = reverse_bisect_right(cost_list, self.target_cost)
 
 				shorter_probs_list = []
 				for cost_index, cost_chain in enumerate(all_chains):
-					probs_list.append(
-						(
-							((self.n_c * self.n_s - cost_index) / (self.n_c * self.n_s))
-							/ (self.n_s ** (i)),
-							cost_chain[0],
-							i + 1,
+					if self.keep_probs_list:
+						probs_list.append(
+							(
+								(
+									(self.n_c * self.n_s - cost_index)
+									/ (self.n_c * self.n_s)
+								)
+								/ (self.n_s ** (i)),
+								cost_chain[0],
+								i + 1,
+							)
 						)
-					)
 					shorter_probs_list.append(
 						(
 							cost_chain[0],
 							((self.n_c * self.n_s - cost_index) / (self.n_c * self.n_s))
 							/ (self.n_s ** (i)),
 						)
 					)
 				# _logger.info(shorter_probs_list)
 				result = SubsetSimulationResult(
 					probs_list=probs_list,
 					over_target_cost=shorter_probs_list[over_index - 1][0],
 					over_target_likelihood=shorter_probs_list[over_index - 1][1],
 					under_target_cost=shorter_probs_list[over_index][0],
 					under_target_likelihood=shorter_probs_list[over_index][1],
+					lowest_likelihood=shorter_probs_list[-1][1],
 				)
 				return result
 
 			# _logger.debug([c[0] for c in all_chains[-n_c:]])
 			_logger.info(f"doing level {i + 1}")
 
-		for cost_index, cost_chain in enumerate(all_chains):
-			probs_list.append(
-				(
-					((self.n_c * self.n_s - cost_index) / (self.n_c * self.n_s))
-					/ (self.n_s ** (self.m_max)),
-					cost_chain[0],
-					self.m_max + 1,
+		if self.keep_probs_list:
+			for cost_index, cost_chain in enumerate(all_chains):
+				probs_list.append(
+					(
+						((self.n_c * self.n_s - cost_index) / (self.n_c * self.n_s))
+						/ (self.n_s ** (self.m_max)),
+						cost_chain[0],
+						self.m_max + 1,
+					)
 				)
-			)
 		threshold_cost = all_chains[-self.n_c][0]
 		_logger.info(
 			f"final threshold cost: {threshold_cost}, at P = (1 / {self.n_s})^{self.m_max + 1}"
 		)
 		for a in all_chains[-10:]:
 			_logger.info(a)
 		# for prob, prob_cost in probs_list:
 		# 	_logger.info(f"\t{prob}: {prob_cost}")
 		probs_list.sort(key=lambda c: c[0], reverse=True)
+
+		min_likelihood = ((1) / (self.n_c * self.n_s)) / (self.n_s ** (self.m_max + 1))
+
 		result = SubsetSimulationResult(
 			probs_list=probs_list,
 			over_target_cost=None,
 			over_target_likelihood=None,
 			under_target_cost=None,
 			under_target_likelihood=None,
+			lowest_likelihood=min_likelihood,
 		)
 		return result
 
 	def get_stdevs_from_arrays(
 		self, array
 	) -> pdme.subspace_simulation.MCMCStandardDeviation:
 		# stdevs = get_stdevs_from_arrays(next_seeds_as_array, model)
```

### Comparing `deepdog-0.7.2/deepdog/temp_aware_real_spectrum_run.py` & `deepdog-0.7.3/deepdog/temp_aware_real_spectrum_run.py`

 * *Files identical despite different names*

### Comparing `deepdog-0.7.2/pyproject.toml` & `deepdog-0.7.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "deepdog"
-version = "0.7.2"
+version = "0.7.3"
 description = ""
 authors = ["Deepak Mallubhotla <dmallubhotla+github@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 pdme = "^0.9.1"
 numpy = "1.22.3"
 scipy = "1.10"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6"
 flake8 = "^4.0.1"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.1.0"
 mypy = "^0.971"
 python-semantic-release = "^7.24.0"
 black = "^22.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `deepdog-0.7.2/setup.py` & `deepdog-0.7.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy==1.22.3', 'pdme>=0.9.1,<0.10.0', 'scipy==1.10']
 
 setup_kwargs = {
     'name': 'deepdog',
-    'version': '0.7.2',
+    'version': '0.7.3',
     'description': '',
     'long_description': None,
     'author': 'Deepak Mallubhotla',
     'author_email': 'dmallubhotla+github@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

