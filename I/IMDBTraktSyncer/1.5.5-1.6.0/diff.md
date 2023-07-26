# Comparing `tmp/IMDBTraktSyncer-1.5.5.tar.gz` & `tmp/IMDBTraktSyncer-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.5.5.tar", last modified: Sat Jul  1 00:58:12 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.6.0.tar", last modified: Wed Jul 26 21:56:53 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.5.5.tar` & `IMDBTraktSyncer-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 00:58:12.187823 IMDBTraktSyncer-1.5.5/
-drwxrwxrwx   0        0        0        0 2023-07-01 00:58:12.155671 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    35244 2023-06-27 07:18:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     6946 2023-06-27 06:49:08.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    10884 2023-06-28 04:22:19.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-07-01 00:58:12.185669 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12155 2023-07-01 00:58:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-07-01 00:58:12.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 00:58:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-07-01 00:58:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-07-01 00:58:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-01 00:58:11.000000 IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.5.5/LICENSE
--rw-rw-rw-   0        0        0    12155 2023-07-01 00:58:12.187823 IMDBTraktSyncer-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0    11409 2023-07-01 00:57:17.000000 IMDBTraktSyncer-1.5.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-01 00:58:12.188825 IMDBTraktSyncer-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-07-01 00:57:43.000000 IMDBTraktSyncer-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 21:56:53.150218 IMDBTraktSyncer-1.6.0/
+drwxrwxrwx   0        0        0        0 2023-07-26 21:56:53.119219 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    39380 2023-07-26 21:50:56.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     6946 2023-06-27 06:49:08.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    10884 2023-06-28 04:22:19.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-07-26 21:56:53.148218 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12569 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-26 21:56:52.000000 IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0    12569 2023-07-26 21:56:53.150218 IMDBTraktSyncer-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11822 2023-07-26 21:55:34.000000 IMDBTraktSyncer-1.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 21:56:53.151209 IMDBTraktSyncer-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-07-26 21:56:19.000000 IMDBTraktSyncer-1.6.0/setup.py
```

### Comparing `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,16 @@
             print("Error: Not signed in to IMDB")
             print("\nPossible IMDB captcha check or IMDB login incorrect.")
             print("\nIf your login is correct then an IMDB captcha check likely the cause of this error. To fix this, simply login to the IMDB website in your browser, preferably Chrome, and from the same computer. If logged in, log out and log back in. It may ask you to fill in a captcha; complete it and finish logging in. After logging in successfully on your browser, run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues.")
             print("\nIf your IMDB login is incorrect, simply edit the credentials.txt file with the correct login or delete the credentials file and run the script again.")
             print("\nSee this GitHub link for more details: https://github.com/RileyXX/IMDB-Trakt-Syncer/issues/2")
             print("\nStopping script...")
             EL.logger.error("Error: Not signed in to IMDB")
+            driver.quit()
+            service.stop()
             raise SystemExit
         
         trakt_watchlist, trakt_ratings, trakt_reviews, watched_content = traktData.getTraktData()
         imdb_watchlist, imdb_ratings, imdb_reviews, errors_found_getting_imdb_reviews = imdbData.getImdbData(imdb_username, imdb_password, driver, directory, wait)
 
         # Get trakt and imdb data and filter out items with missing imdb id
         trakt_ratings = [rating for rating in trakt_ratings if rating.get('IMDB_ID') is not None]
@@ -227,39 +229,53 @@
                         
                         # Load page
                         success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver, wait)
                         if not success:
                             # Page failed to load, raise an exception
                             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
                         
-                        # Wait until the loader has disappeared, indicating the watchlist button has loaded
-                        wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="tm-box-wl-loader"]')))
+                        current_url = driver.current_url
                         
-                        # Scroll the page to bring the element into view
-                        watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
-                        driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
-                        
-                        # Wait for the element to be clickable
-                        watchlist_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
-                        
-                        # Check if item is already in watchlist otherwise skip it
-                        if 'ipc-icon--done' not in watchlist_button.get_attribute('innerHTML'):
-                            retry_count = 0
-                            while retry_count < 2:
+                        # Check if the URL doesn't contain "/reference"
+                        if "/reference" not in current_url:
+                            # Wait until the loader has disappeared, indicating the watchlist button has loaded
+                            wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="tm-box-wl-loader"]')))
+                            
+                            # Scroll the page to bring the element into view
+                            watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
+                            driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
+                            
+                            # Wait for the element to be clickable
+                            watchlist_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
+                            
+                            # Check if item is already in watchlist otherwise skip it
+                            if 'ipc-icon--done' not in watchlist_button.get_attribute('innerHTML'):
+                                retry_count = 0
+                                while retry_count < 2:
+                                    driver.execute_script("arguments[0].click();", watchlist_button)
+                                    try:
+                                        WebDriverWait(driver, 3).until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"] .ipc-icon--done')))
+                                        break  # Break the loop if successful
+                                    except TimeoutException:
+                                        retry_count += 1
+
+                                if retry_count == 2:
+                                    error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['IMDB_ID']})"
+                                    print(f"   - {error_message}")
+                                    EL.logger.error(error_message)
+                        else:
+                            # Handle the case when the URL contains "/reference"
+                            
+                            # Scroll the page to bring the element into view
+                            watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '.titlereference-watch-ribbon > .wl-ribbon')))
+                            driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
+                            
+                            # Check if watchlist_button has class .not-inWL before clicking
+                            if 'not-inWL' in watchlist_button.get_attribute('class'):
                                 driver.execute_script("arguments[0].click();", watchlist_button)
-                                try:
-                                    WebDriverWait(driver, 3).until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"] .ipc-icon--done')))
-                                    break  # Break the loop if successful
-                                except TimeoutException:
-                                    retry_count += 1
-
-                            if retry_count == 2:
-                                error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['IMDB_ID']})"
-                                print(f"   - {error_message}")
-                                EL.logger.error(error_message)
                         
                     except (NoSuchElementException, TimeoutException, PageLoadException):
                         error_message = f"Failed to add item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist ({item['IMDB_ID']})"
                         print(f"   - {error_message}")
                         EL.logger.error(error_message, exc_info=True)
                         pass
 
@@ -344,31 +360,52 @@
                     try:
                         # Load page
                         success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver, wait)
                         if not success:
                             # Page failed to load, raise an exception
                             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
                         
-                        # Wait until the rating bar has loaded
-                        wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__loading"]')))
+                        current_url = driver.current_url
                         
-                        # Wait until rate button is located and scroll to it
-                        button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
-                        driver.execute_script("arguments[0].scrollIntoView(true);", button)
-
-                        # click on "Rate" button and select rating option, then submit rating
-                        button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
-                        element_rating_bar = button.find_element(By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating__unrated"]')
-                        if element_rating_bar:
+                        # Check if the URL doesn't contain "/reference"
+                        if "/reference" not in current_url:
+                            # Wait until the rating bar has loaded
+                            wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__loading"]')))
+                            
+                            # Wait until rate button is located and scroll to it
+                            button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
+                            driver.execute_script("arguments[0].scrollIntoView(true);", button)
+
+                            # click on "Rate" button and select rating option, then submit rating
+                            button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating"] button.ipc-btn')))
+                            element_rating_bar = button.find_element(By.CSS_SELECTOR, '[data-testid="hero-rating-bar__user-rating__unrated"]')
+                            if element_rating_bar:
+                                driver.execute_script("arguments[0].click();", button)
+                                rating_option_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
+                                driver.execute_script("arguments[0].click();", rating_option_element)
+                                submit_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
+                                submit_element.click()
+                                time.sleep(1)
+                        else:
+                            # Handle the case when the URL contains "/reference"
+                            
+                            # Wait until rate button is located and scroll to it
+                            button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '.ipl-rating-interactive__star-container')))
+                            driver.execute_script("arguments[0].scrollIntoView(true);", button)
+
+                            # click on "Rate" button and select rating option, then submit rating
+                            button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, '.ipl-rating-interactive__star-container')))
                             driver.execute_script("arguments[0].click();", button)
-                            rating_option_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'button[aria-label="Rate {item["Rating"]}"]')))
+                            
+                            # Find the rating option element based on the data-value attribute
+                            rating_option_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, f'.ipl-rating-selector__star-link[data-value="{item["Rating"]}"]')))
                             driver.execute_script("arguments[0].click();", rating_option_element)
-                            submit_element = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button.ipc-rating-prompt__rate-button')))
-                            submit_element.click()
+                            
                             time.sleep(1)
+                            
                     except (NoSuchElementException, TimeoutException, PageLoadException):
                         error_message = f'Failed to rate {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB ({item["IMDB_ID"]})'
                         print(f"   - {error_message}")
                         EL.logger.error(error_message, exc_info=True)
                         pass
 
                 print('Setting IMDB Ratings Complete')
@@ -562,39 +599,54 @@
                         
                         # Load page
                         success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver, wait)
                         if not success:
                             # Page failed to load, raise an exception
                             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
                         
-                        # Wait until the loader has disappeared, indicating the watchlist button has loaded
-                        wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="tm-box-wl-loader"]')))
+                        current_url = driver.current_url
                         
-                        # Scroll the page to bring the element into view
-                        watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
-                        driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
-                        
-                        # Wait for the element to be clickable
-                        watchlist_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
-                        
-                        # Check if item is not in watchlist otherwise skip it
-                        if 'ipc-icon--add' not in watchlist_button.get_attribute('innerHTML'):
-                            retry_count = 0
-                            while retry_count < 2:
+                        # Check if the URL doesn't contain "/reference"
+                        if "/reference" not in current_url:
+                            # Wait until the loader has disappeared, indicating the watchlist button has loaded
+                            wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="tm-box-wl-loader"]')))
+                            
+                            # Scroll the page to bring the element into view
+                            watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
+                            driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
+                            
+                            # Wait for the element to be clickable
+                            watchlist_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"]')))
+                            
+                            # Check if item is not in watchlist otherwise skip it
+                            if 'ipc-icon--add' not in watchlist_button.get_attribute('innerHTML'):
+                                retry_count = 0
+                                while retry_count < 2:
+                                    driver.execute_script("arguments[0].click();", watchlist_button)
+                                    try:
+                                        WebDriverWait(driver, 3).until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"] .ipc-icon--add')))
+                                        break  # Break the loop if successful
+                                    except TimeoutException:
+                                        retry_count += 1
+
+                                if retry_count == 2:
+                                    error_message = f"Failed to remove item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist ({item['IMDB_ID']})"
+                                    print(f"   - {error_message}")
+                                    EL.logger.error(error_message)
+                    
+                        else:
+                            # Handle the case when the URL contains "/reference"
+                            
+                            # Scroll the page to bring the element into view
+                            watchlist_button = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, '.titlereference-watch-ribbon > .wl-ribbon')))
+                            driver.execute_script("arguments[0].scrollIntoView(true);", watchlist_button)
+                            
+                            # Check if watchlist_button doesn't have the class .not-inWL before clicking
+                            if 'not-inWL' not in watchlist_button.get_attribute('class'):
                                 driver.execute_script("arguments[0].click();", watchlist_button)
-                                try:
-                                    WebDriverWait(driver, 3).until(EC.presence_of_element_located((By.CSS_SELECTOR, 'button[data-testid="tm-box-wl-button"] .ipc-icon--add')))
-                                    break  # Break the loop if successful
-                                except TimeoutException:
-                                    retry_count += 1
-
-                            if retry_count == 2:
-                                error_message = f"Failed to remove item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist ({item['IMDB_ID']})"
-                                print(f"   - {error_message}")
-                                EL.logger.error(error_message)
 
                     except (NoSuchElementException, TimeoutException, PageLoadException):
                         error_message = f"Failed to remove item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist ({item['IMDB_ID']})"
                         print(f"   - {error_message}")
                         EL.logger.error(error_message, exc_info=True)
                         pass
 
@@ -608,10 +660,16 @@
         driver.quit()
         service.stop()
     
     except Exception as e:
         error_message = "An error occurred while running the script."
         EH.report_error(error_message)
         EL.logger.error(error_message, exc_info=True)
+        
+        # Close the driver and stop the service if they were initialized
+        if 'driver' in locals() and driver is not None:
+            driver.quit()
+        if 'service' in locals() and service is not None:
+            service.stop()
 
 if __name__ == '__main__':
     main()
```

### Comparing `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/errorHandling.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/errorLogger.py` & `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/errorLogger.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/imdbData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.5.5
+Version: 1.6.0
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
-6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
 ```
 python -m pip install IMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
 ## Running the Script:
@@ -56,15 +56,15 @@
 
 ## Alternative Manual Installation Method (without pip install)
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
-6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
@@ -97,26 +97,27 @@
 
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
 | [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / AudioSubChanger](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/audio_sub_changer.py) | A script with advanced options for changing audio & subtitle tracks in Plex. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
 | [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
 | [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
 | [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
 | [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
 | [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
 | [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
 | [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
 | [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
 | [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
 | [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
 | [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
-| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [AirVPN](https://airvpn.org/) | A VPN client with port forwarding support. Great VPN for torrents. |
 | [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
 | [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
 | [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `IMDBTraktSyncer-1.5.5/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.6.0/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.5/LICENSE` & `IMDBTraktSyncer-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.5/PKG-INFO` & `IMDBTraktSyncer-1.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.5.5
+Version: 1.6.0
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
-6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
 ```
 python -m pip install IMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
 ## Running the Script:
@@ -56,15 +56,15 @@
 
 ## Alternative Manual Installation Method (without pip install)
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
-6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
@@ -97,26 +97,27 @@
 
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
 | [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / AudioSubChanger](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/audio_sub_changer.py) | A script with advanced options for changing audio & subtitle tracks in Plex. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
 | [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
 | [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
 | [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
 | [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
 | [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
 | [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
 | [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
 | [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
 | [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
 | [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
 | [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
-| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [AirVPN](https://airvpn.org/) | A VPN client with port forwarding support. Great VPN for torrents. |
 | [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
 | [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
 | [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `IMDBTraktSyncer-1.5.5/README.md` & `IMDBTraktSyncer-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 ## Installation Instructions
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Install the script by executing `python -m pip install IMDBTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run the script by executing `IMDBTraktSyncer` in the command line.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
-6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## Installing the Script:
 ```
 python -m pip install IMDBTraktSyncer
 ```
 _Run in your operating system's native command line._
 ## Running the Script:
@@ -40,15 +40,15 @@
 
 ## Alternative Manual Installation Method (without pip install)
 1. Install [Python](https://www.python.org/downloads/) (v3.6 or later) and [Google Chrome](https://www.google.com/chrome/).  _If these are already installed, you can skip this step. Please note this script does not affect Chrome in anyway, it is simply required in order for chromedriver to work._
 2. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDB-Trakt-Syncer/releases) and extract it to the desired directory.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application named `IMDBTraktSyncer`. In the "Redirect uri" field, enter `urn:ietf:wg:oauth:2.0:oob`, then save the application.
 4. Run `IMDBTraktSyncer.py` or open the terminal and navigate to the folder where `IMDBTraktSyncer.py` is located. Run `IMDBTraktSyncer.py` in the terminal.
 5. Follow the prompts during the first run. You will need to enter your Trakt `client ID` and `client secret` from step 3, as well as your IMDB `username` and `password`. Please note that these details are saved insecurely as `credentials.txt` in the same folder as the script. It is recommended to change your IMDB password to something unique beforehand.
-6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line.
+6. Setup is complete. The script will continue running and syncing your ratings. You can monitor its progress in the command line. See below for [setting up automation](https://github.com/RileyXX/IMDB-Trakt-Syncer#for-setting-up-automation-see-the-following-wiki-pages).
 
 ## For Setting Up Automation See the Following Wiki Pages:
 - Setup Automation for:
    - [Windows](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Windows)
    - [Linux](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-Linux)
    - [macOS](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Setting-Up-Automation-on-macOS)
 - Python Script to Update all Packages with Pip (Windows, Linux, Mac, ChromeOS, etc.) [Link #1](https://github.com/RileyXX/IMDB-Trakt-Syncer/wiki/Python-Script-to-Update-all-Packages-with-Pip-\(Windows,-Linux,-Mac,-ChromeOS,-etc\))
@@ -81,26 +81,27 @@
 
 | Project Name | Description |
 |--------------|-------------|
 | [PlexTraktSync](https://github.com/Taxel/PlexTraktSync) | A script that syncs user watch history and ratings between Trakt and Plex (without needing a PlexPass or Trakt VIP subscription). |
 | [IMDB-Trakt-Syncer](https://github.com/RileyXX/IMDB-Trakt-Syncer) | A script that syncs user watchlist, ratings, and comments both ways between Trakt and IMDB. |
 | [TMDB-Trakt-Syncer](https://github.com/RileyXX/TMDB-Trakt-Syncer) | A script that syncs user watchlist and ratings both ways between Trakt and TMDB. |
 | [PlexPreferNonForcedSubs](https://github.com/RileyXX/PlexPreferNonForcedSubs) | A script that sets all movies and shows in your local Plex library to English non-forced subtitles by default. |
+| [Casvt / AudioSubChanger](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/audio_sub_changer.py) | A script with advanced options for changing audio & subtitle tracks in Plex. |
 | [Casvt / PlexAutoDelete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py) | A script for automatically deleting watched content from Plex. |
 | [universal-trakt-scrobbler](https://github.com/trakt-tools/universal-trakt-scrobbler) | An extension that automatically scrobbles TV shows and Movies from several streaming services to Trakt. |
 | [Netflix-to-Trakt-Import](https://github.com/jensb89/Netflix-to-Trakt-Import) | A tool to import your Netflix viewing history into Trakt. |
 | [trakt-tv-backup](https://darekkay.com/blog/trakt-tv-backup/) | A command-line tool for backing up your Trakt.tv data. |
 | [blacktwin / JBOPS](https://github.com/blacktwin/JBOPS) | A collection of scripts and tools for enhancing and automating tasks in Plex. |
 | [Casvt / Plex-scripts](https://github.com/Casvt/Plex-scripts) | A collection of useful scripts for Plex automation and management. |
 | [trakt---letterboxd-import](https://github.com/jensb89/trakt---letterboxd-import) | A tool to import your Letterboxd ratings and watchlist into Trakt. |
 | [TraktRater](https://github.com/damienhaynes/TraktRater/) | A tool to help users transfer user episode, show, and movie user ratings and watchlists from multiple media database sites around the web. |
 | [TvTimeToTrakt](https://github.com/lukearran/TvTimeToTrakt) | A tool to sync your TV Time watch history with Trakt.tv. |
 | [Plex Media Server](https://www.plex.tv/media-server-downloads/#plex-app) | A media server software to organize and stream your personal media collection. |
 | [Radarr](https://github.com/Radarr/Radarr) | A movie collection manager and downloader for various platforms. |
 | [Sonarr](https://github.com/Sonarr/Sonarr) | A TV show collection manager and downloader for various platforms. |
 | [Jackett](https://github.com/Jackett/Jackett) | A proxy server that provides API support for various torrent trackers commonly used with Radarr and Sonarr. |
 | [qBittorrent](https://github.com/qbittorrent/qBittorrent) | A free and open-source BitTorrent client. |
-| [Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) | An open-source VPN client for Mullvad VPN service with port forwarding support. Great VPN for torrents. |
+| [AirVPN](https://airvpn.org/) | A VPN client with port forwarding support. Great VPN for torrents. |
 | [Overseerr](https://github.com/sct/overseerr) | A request management and media discovery tool for your home media server. |
 | [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | A reverse proxy solution to bypass Cloudflare protection and access websites commonly used with Jackett. |
 | [youtube-dl](https://github.com/ytdl-org/youtube-dl) | A command-line program to download videos from YouTube and other sites. |
```

### Comparing `IMDBTraktSyncer-1.5.5/setup.py` & `IMDBTraktSyncer-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.5.5'
+VERSION = '1.6.0'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

