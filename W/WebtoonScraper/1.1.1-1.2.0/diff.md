# Comparing `tmp/WebtoonScraper-1.1.1.tar.gz` & `tmp/WebtoonScraper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebtoonScraper-1.1.1.tar", last modified: Fri Jul 21 19:36:40 2023, max compression
+gzip compressed data, was "WebtoonScraper-1.2.0.tar", last modified: Thu Jul 27 13:38:03 2023, max compression
```

## Comparing `WebtoonScraper-1.1.1.tar` & `WebtoonScraper-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 19:36:40.375443 WebtoonScraper-1.1.1/
--rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-06-30 07:37:22.000000 WebtoonScraper-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0    10220 2023-07-21 19:36:40.374442 WebtoonScraper-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8801 2023-07-21 19:30:49.000000 WebtoonScraper-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 19:36:40.355785 WebtoonScraper-1.1.1/WebtoonScraper/
--rw-rw-rw-   0        0        0    10280 2023-07-20 14:17:03.000000 WebtoonScraper-1.1.1/WebtoonScraper/A_FolderManager.py
--rw-rw-rw-   0        0        0    11211 2023-07-21 19:17:57.000000 WebtoonScraper-1.1.1/WebtoonScraper/B_Webtoon.py
--rw-rw-rw-   0        0        0    24754 2023-07-21 19:04:45.000000 WebtoonScraper-1.1.1/WebtoonScraper/C_Scraper.py
--rw-rw-rw-   0        0        0     3942 2023-07-21 13:05:19.000000 WebtoonScraper-1.1.1/WebtoonScraper/D_NaverWebtoonScraper.py
--rw-rw-rw-   0        0        0      644 2023-07-21 11:20:47.000000 WebtoonScraper-1.1.1/WebtoonScraper/E_BestChallengeScraper.py
--rw-rw-rw-   0        0        0     4785 2023-07-21 13:08:33.000000 WebtoonScraper-1.1.1/WebtoonScraper/F_WebtoonOriginalsScraper.py
--rw-rw-rw-   0        0        0      640 2023-07-21 12:02:11.000000 WebtoonScraper-1.1.1/WebtoonScraper/G_WebtoonCanvasScraper.py
--rw-rw-rw-   0        0        0     3964 2023-07-21 19:05:52.000000 WebtoonScraper-1.1.1/WebtoonScraper/H_TelescopeScraper.py
--rw-rw-rw-   0        0        0     5689 2023-07-21 13:10:21.000000 WebtoonScraper-1.1.1/WebtoonScraper/I_BufftoonScraper.py
--rw-rw-rw-   0        0        0     6051 2023-07-21 13:19:51.000000 WebtoonScraper-1.1.1/WebtoonScraper/J_NaverPostScraper.py
--rw-rw-rw-   0        0        0     3451 2023-07-21 13:21:27.000000 WebtoonScraper-1.1.1/WebtoonScraper/K_NaverGameScraper.py
--rw-rw-rw-   0        0        0     1186 2023-07-21 13:34:50.000000 WebtoonScraper-1.1.1/WebtoonScraper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:36:40.369392 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/
--rw-rw-rw-   0        0        0    10220 2023-07-21 19:36:40.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      724 2023-07-21 19:36:40.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 19:36:40.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       37 2023-07-21 19:36:40.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-21 19:36:40.000000 WebtoonScraper-1.1.1/WebtoonScraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-21 19:36:40.375443 WebtoonScraper-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-07-21 14:03:11.000000 WebtoonScraper-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 19:36:40.373446 WebtoonScraper-1.1.1/test/
--rw-rw-rw-   0        0        0      217 2023-07-20 17:15:31.000000 WebtoonScraper-1.1.1/test/__init__.py
--rw-rw-rw-   0        0        0     1649 2023-07-20 16:42:26.000000 WebtoonScraper-1.1.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-07-27 13:38:03.263625 WebtoonScraper-1.2.0/
+-rw-rw-rw-   0        0        0     1089 2023-05-15 00:16:47.000000 WebtoonScraper-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-06-30 07:37:22.000000 WebtoonScraper-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12798 2023-07-27 13:38:03.262539 WebtoonScraper-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11379 2023-07-27 10:49:37.000000 WebtoonScraper-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 13:38:03.244732 WebtoonScraper-1.2.0/WebtoonScraper/
+-rw-rw-rw-   0        0        0    10280 2023-07-20 14:17:03.000000 WebtoonScraper-1.2.0/WebtoonScraper/A_FolderManager.py
+-rw-rw-rw-   0        0        0    12085 2023-07-27 10:18:06.000000 WebtoonScraper-1.2.0/WebtoonScraper/B_Webtoon.py
+-rw-rw-rw-   0        0        0    25977 2023-07-26 20:17:20.000000 WebtoonScraper-1.2.0/WebtoonScraper/C_Scraper.py
+-rw-rw-rw-   0        0        0     3944 2023-07-21 23:58:12.000000 WebtoonScraper-1.2.0/WebtoonScraper/D_NaverWebtoonScraper.py
+-rw-rw-rw-   0        0        0      644 2023-07-21 11:20:47.000000 WebtoonScraper-1.2.0/WebtoonScraper/E_BestChallengeScraper.py
+-rw-rw-rw-   0        0        0     4785 2023-07-21 13:08:33.000000 WebtoonScraper-1.2.0/WebtoonScraper/F_WebtoonOriginalsScraper.py
+-rw-rw-rw-   0        0        0      640 2023-07-21 12:02:11.000000 WebtoonScraper-1.2.0/WebtoonScraper/G_WebtoonCanvasScraper.py
+-rw-rw-rw-   0        0        0     3964 2023-07-21 19:05:52.000000 WebtoonScraper-1.2.0/WebtoonScraper/H_TelescopeScraper.py
+-rw-rw-rw-   0        0        0     5689 2023-07-21 13:10:21.000000 WebtoonScraper-1.2.0/WebtoonScraper/I_BufftoonScraper.py
+-rw-rw-rw-   0        0        0     6051 2023-07-21 13:19:51.000000 WebtoonScraper-1.2.0/WebtoonScraper/J_NaverPostScraper.py
+-rw-rw-rw-   0        0        0     3451 2023-07-21 13:21:27.000000 WebtoonScraper-1.2.0/WebtoonScraper/K_NaverGameScraper.py
+-rw-rw-rw-   0        0        0    16936 2023-07-27 13:19:15.000000 WebtoonScraper-1.2.0/WebtoonScraper/L_LezhinComicsScraper.py
+-rw-rw-rw-   0        0        0     1186 2023-07-21 13:34:50.000000 WebtoonScraper-1.2.0/WebtoonScraper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-27 13:38:03.258895 WebtoonScraper-1.2.0/WebtoonScraper.egg-info/
+-rw-rw-rw-   0        0        0    12798 2023-07-27 13:38:03.000000 WebtoonScraper-1.2.0/WebtoonScraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2023-07-27 13:38:03.000000 WebtoonScraper-1.2.0/WebtoonScraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 13:38:03.000000 WebtoonScraper-1.2.0/WebtoonScraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 14:16:38.000000 WebtoonScraper-1.2.0/WebtoonScraper.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-07-27 13:38:03.000000 WebtoonScraper-1.2.0/WebtoonScraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-27 13:38:03.000000 WebtoonScraper-1.2.0/WebtoonScraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 13:38:03.264633 WebtoonScraper-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-07-26 23:22:18.000000 WebtoonScraper-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 13:38:03.261420 WebtoonScraper-1.2.0/test/
+-rw-rw-rw-   0        0        0      217 2023-07-20 17:15:31.000000 WebtoonScraper-1.2.0/test/__init__.py
+-rw-rw-rw-   0        0        0     1649 2023-07-20 16:42:26.000000 WebtoonScraper-1.2.0/test/test.py
```

### Comparing `WebtoonScraper-1.1.1/LICENSE` & `WebtoonScraper-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.1.1/PKG-INFO` & `WebtoonScraper-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,37 @@
-Metadata-Version: 2.1
-Name: WebtoonScraper
-Version: 1.1.1
-Summary: Scraping webtoons and some utils for it
-Home-page: https://github.com/ilotoki0804/WebtoonScraper
-Author: ilotoki0804
-Author-email: ilotoki0804@gmail.com
-License: MIT
-Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다.
 
-네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임을 지원합니다.
+네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임, 레진 코믹스를 지원합니다.
 
 # 시작하기
 
 1. 파이썬을 설치합니다.
-2. cmd 창을 열어 pip 명령어를 실행합니다.
+2. 터미널에서 다음과 같은 명령어를 실행합니다.
    ```
    pip install -U WebtoonScraper
    ```
 
 # 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 네이버 게임 다운로드하기
 
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
 
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
    네이버 웹툰/베스트 도전(comic.naver.com):
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_webtoon.png)
+   ![img](images/naver_webtoon.png)
    웹툰 오리지널/캔버스(webtoons.com):
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/webtoons_original.png)
+   ![img](images/webtoons_original.png)
    만화경(manhwakyung.com)
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/manhwakyung.png)
+   ![img](images/manhwakyung.png)
    네이버 게임 오리지널 시리즈(game.naver.com/original_series):
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_game.png)
+   ![img](images/naver_game.png)
    버프툰과 네이버 포스트는 아래의 '버프툰 다운로드하기'섹션과 '네이버 포스트 다운로드하기' 섹션을 참고해 주세요.
+   레진코믹스는 따로 준비된 스크린샷은 없습니다만 방법은 네이버 게임 오리지널과 같습니다.
+   레진코믹스는 titleid가 문자열이라는 점에 참고하세요.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경, 네이버 게임 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
    wt.get_webtoon(76648, wt.N)  # titleid를 여기에다 붙여넣으세요.
@@ -62,26 +46,31 @@
    # 네이버 게임 오리지널 시리즈
    wt.get_webtoon(5, wt.G)  # titleid를 여기에다 붙여넣으세요.
    # 버프툰
    cookie = 'cookie here'  # cookie를 여기에다 붙여넣으세요. 자세한 설명은 아래의 '버프툰 다운로드하기'를 참고하세요.
    wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # titleid를 여기에다 붙여넣으세요.
    # 네이버 포스트
    wt.get_webtoon((597061, 19803452), wt.P)  # seriesNo와 memberNo를 각각 붙여넣으세요. 자세한 설명은 아래의 '네이버 포스트 다운받기'를 참고하세요.
+   # 레진코믹스
+   authorization = 'authorization here'  # authorization을 여기에다 붙여넣으세요. 자세한 설명은 아래의 '레진코믹스 다운로드하기'를 참고하세요.
+   wt.get_webtoon('some_webtoon', wt.L, authorization=authorization)  # titleid를 여기에다 붙여넣으세요.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
    cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 만약 몇몇 태그가 겹친다면 태그에 맞는 수를 입력하는 창에 알맞은 수를 입력하면 됩니다.
 
    episode_no_range 키워드를 이용하면 특정한 에피소드만 다운로드받을 수 있습니다.
+
    ```python
    wt.get_webtoon(5, wt.G, episode_no_range=(1,20))  # 1화부터 20화까지
    ```
 
    merge 키워드를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 원하는 개수 만큼 묶습니다.
+
    ```python
    wt.get_webtoon(5, wt.G, merge=5)
    ```
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
@@ -105,50 +94,74 @@
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 로그인한 상태에서 웹툰 다운로드하기
 
 이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
 
 1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다. 이 예시에서는 1007888입니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon1.png)
+   ![img](images/bufftoon1.png)
 2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon2.png)
+   ![img](images/bufftoon2.png)
 3. 새로고침을 한 뒤 '이름'에 있는 favicon.ico 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon3.png)
+   ![img](images/bufftoon3.png)
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon4.png)
+   ![img](images/bufftoon4.png)
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
    cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
    wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
 6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 주의사항
 
 * get_webtoon에서 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
+* favicon.ico가 요청에 뜨지 않는다면 ctrl+R을 해보고, 그래도 없다면 `필터`에서 `모두`로 설정되어 있는지 다시 확인하세요.
 
 # 네이버 포스트 다운로드하기
 
-1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
-   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_post.png)
+1. 웹툰이 있는 페이지로 가서 주소창에서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
+   ![img](images/naver_post.png)
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon((597061, 19803452), wt.P)
+   wt.get_webtoon((597061, 19803452), wt.P)  # 여기에 아까 복사한 seriesNo와 memberNo를 붙여넣으세요.
    ```
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
 * tuple를 입력하면 자동으로 포스트로 인식됩니다.
 
+# 레진코믹스 다운로드하기
+
+로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 에피소드의 개수가 제한된다는 점을 유의해 주십세요.
+로그인하지 않은 상태이더라도 웹툰을 다운로드받을 수는 있습니다.
+
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 문자열을 복사합니다.
+2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
+3. 새로고침을 한 뒤 '이름'에 있는 `balance?lezhinObjectId=...&lezhinObjectType=comic`(찾기 조금 어려울 수 있습니다.) 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
+4. 내려서 Authorization: 이라고 되어 있는 모든 내용을 복사합니다.
+5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+   authorization = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
+   wt.get_webtoon(1007888, wt.L, authorization=authorization)  # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
+   ```
+6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
+## 주의사항
+
+* 다른 웹툰 플렛폼과는 다르게 titleid가 문자열입니다.
+* 다른 웹툰 플랫폼들에 비해 다운로드 속도가 비교적 느린 편입니다.
+* 일부 웹툰은 셔플링이 되어 있습니다. 따라서 웹툰을 다 다운로드받은 후 언셔플링을 하는 과정이 필요하며, 이 과정에 다소 시간이 소요된다는 점 참고 바랍니다.
+
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import FolderManager
 
@@ -173,14 +186,16 @@
    fm= FolderManager()
    fm.restore_webtoons_in_directory()
    ```
 3. 'webtoon' 폴더에 있던 모든 웹툰이 웹툰을 처음 다운로드했던 상태로 되돌아갑니다.
 
 # Relese Note
 
+1.2.0: 레진코믹스 추가, 의존성 증가(pyjsparser, Pillow)
+
 1.1.1: 내부 모듈 이름 변경, merge option 추가, abstractmethod들의 일반 구현 추가
 
 1.0.2: 대형 리팩토링, get_webtoon_platform 비동기 방식으로 속도 개선, 상대경로로 변경, 테스트 추가
 
 1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경 (버그가 많기에 사용을 권장하지 않음)
 
 1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
```

### Comparing `WebtoonScraper-1.1.1/README.md` & `WebtoonScraper-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,55 @@
+Metadata-Version: 2.1
+Name: WebtoonScraper
+Version: 1.2.0
+Summary: Scraping webtoons and some utils for it
+Home-page: https://github.com/ilotoki0804/WebtoonScraper
+Author: ilotoki0804
+Author-email: ilotoki0804@gmail.com
+License: MIT
+Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다.
 
-네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임을 지원합니다.
+네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임, 레진 코믹스를 지원합니다.
 
 # 시작하기
 
 1. 파이썬을 설치합니다.
-2. cmd 창을 열어 pip 명령어를 실행합니다.
+2. 터미널에서 다음과 같은 명령어를 실행합니다.
    ```
    pip install -U WebtoonScraper
    ```
 
 # 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 네이버 게임 다운로드하기
 
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
 
 1. 원하는 웹툰으로 가서 titleid 또는 title_no를 복사하세요.
    네이버 웹툰/베스트 도전(comic.naver.com):
-   ![img](images/naver_webtoon.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_webtoon.png)
    웹툰 오리지널/캔버스(webtoons.com):
-   ![img](images/webtoons_original.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/webtoons_original.png)
    만화경(manhwakyung.com)
-   ![img](images/manhwakyung.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/manhwakyung.png)
    네이버 게임 오리지널 시리즈(game.naver.com/original_series):
-   ![img](images/naver_game.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_game.png)
    버프툰과 네이버 포스트는 아래의 '버프툰 다운로드하기'섹션과 '네이버 포스트 다운로드하기' 섹션을 참고해 주세요.
+   레진코믹스는 따로 준비된 스크린샷은 없습니다만 방법은 네이버 게임 오리지널과 같습니다.
+   레진코믹스는 titleid가 문자열이라는 점에 참고하세요.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경, 네이버 게임 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
    wt.get_webtoon(76648, wt.N)  # titleid를 여기에다 붙여넣으세요.
@@ -44,26 +64,31 @@
    # 네이버 게임 오리지널 시리즈
    wt.get_webtoon(5, wt.G)  # titleid를 여기에다 붙여넣으세요.
    # 버프툰
    cookie = 'cookie here'  # cookie를 여기에다 붙여넣으세요. 자세한 설명은 아래의 '버프툰 다운로드하기'를 참고하세요.
    wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # titleid를 여기에다 붙여넣으세요.
    # 네이버 포스트
    wt.get_webtoon((597061, 19803452), wt.P)  # seriesNo와 memberNo를 각각 붙여넣으세요. 자세한 설명은 아래의 '네이버 포스트 다운받기'를 참고하세요.
+   # 레진코믹스
+   authorization = 'authorization here'  # authorization을 여기에다 붙여넣으세요. 자세한 설명은 아래의 '레진코믹스 다운로드하기'를 참고하세요.
+   wt.get_webtoon('some_webtoon', wt.L, authorization=authorization)  # titleid를 여기에다 붙여넣으세요.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
    cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 만약 몇몇 태그가 겹친다면 태그에 맞는 수를 입력하는 창에 알맞은 수를 입력하면 됩니다.
 
    episode_no_range 키워드를 이용하면 특정한 에피소드만 다운로드받을 수 있습니다.
+
    ```python
    wt.get_webtoon(5, wt.G, episode_no_range=(1,20))  # 1화부터 20화까지
    ```
 
    merge 키워드를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 원하는 개수 만큼 묶습니다.
+
    ```python
    wt.get_webtoon(5, wt.G, merge=5)
    ```
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
@@ -87,50 +112,74 @@
 4. 로그인하지 않고 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 로그인한 상태에서 웹툰 다운로드하기
 
 이 과정은 PC를 기준으로 설명합니다. 만약 모바일이라면 Kiwi Browser 등을 통해 다음의 과정을 수행할 수 있습니다.
 
 1. 웹툰 페이지에 들어가 주소창의 맨 마지막 수를 복사합니다. 이 예시에서는 1007888입니다.
-   ![img](images/bufftoon1.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon1.png)
 2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
-   ![img](images/bufftoon2.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon2.png)
 3. 새로고침을 한 뒤 '이름'에 있는 favicon.ico 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
-   ![img](images/bufftoon3.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon3.png)
 4. 내려서 Cookie: 라고 되어 있는 모든 내용을 복사합니다.
-   ![img](images/bufftoon4.png)
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/bufftoon4.png)
 5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
    cookie = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
    wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
 6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 주의사항
 
 * get_webtoon에서 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
+* favicon.ico가 요청에 뜨지 않는다면 ctrl+R을 해보고, 그래도 없다면 `필터`에서 `모두`로 설정되어 있는지 다시 확인하세요.
 
 # 네이버 포스트 다운로드하기
 
-1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
-   ![img](images/naver_post.png)
+1. 웹툰이 있는 페이지로 가서 주소창에서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
+   ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_post.png)
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon((597061, 19803452), wt.P)
+   wt.get_webtoon((597061, 19803452), wt.P)  # 여기에 아까 복사한 seriesNo와 memberNo를 붙여넣으세요.
    ```
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
 * tuple를 입력하면 자동으로 포스트로 인식됩니다.
 
+# 레진코믹스 다운로드하기
+
+로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 에피소드의 개수가 제한된다는 점을 유의해 주십세요.
+로그인하지 않은 상태이더라도 웹툰을 다운로드받을 수는 있습니다.
+
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 문자열을 복사합니다.
+2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
+3. 새로고침을 한 뒤 '이름'에 있는 `balance?lezhinObjectId=...&lezhinObjectType=comic`(찾기 조금 어려울 수 있습니다.) 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
+4. 내려서 Authorization: 이라고 되어 있는 모든 내용을 복사합니다.
+5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+   authorization = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
+   wt.get_webtoon(1007888, wt.L, authorization=authorization)  # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
+   ```
+6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
+## 주의사항
+
+* 다른 웹툰 플렛폼과는 다르게 titleid가 문자열입니다.
+* 다른 웹툰 플랫폼들에 비해 다운로드 속도가 비교적 느린 편입니다.
+* 일부 웹툰은 셔플링이 되어 있습니다. 따라서 웹툰을 다 다운로드받은 후 언셔플링을 하는 과정이 필요하며, 이 과정에 다소 시간이 소요된다는 점 참고 바랍니다.
+
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import FolderManager
 
@@ -155,14 +204,16 @@
    fm= FolderManager()
    fm.restore_webtoons_in_directory()
    ```
 3. 'webtoon' 폴더에 있던 모든 웹툰이 웹툰을 처음 다운로드했던 상태로 되돌아갑니다.
 
 # Relese Note
 
+1.2.0: 레진코믹스 추가, 의존성 증가(pyjsparser, Pillow)
+
 1.1.1: 내부 모듈 이름 변경, merge option 추가, abstractmethod들의 일반 구현 추가
 
 1.0.2: 대형 리팩토링, get_webtoon_platform 비동기 방식으로 속도 개선, 상대경로로 변경, 테스트 추가
 
 1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경 (버그가 많기에 사용을 권장하지 않음)
 
 1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
```

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/A_FolderManager.py` & `WebtoonScraper-1.2.0/WebtoonScraper/A_FolderManager.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/B_Webtoon.py` & `WebtoonScraper-1.2.0/WebtoonScraper/B_Webtoon.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """Download webtoons automatiallly or easily"""
 
 import asyncio
 import contextlib
 from itertools import starmap
+import logging
 
 if __name__ in ("__main__", "B_Webtoon"):
     from A_FolderManager import FolderManager
     from D_NaverWebtoonScraper import NaverWebtoonScraper
     from E_BestChallengeScraper import BestChallengeScraper
     from F_WebtoonOriginalsScraper import WebtoonOriginalsScraper
     from G_WebtoonCanvasScraper import WebtoonCanvasScraper
     from H_TelescopeScraper import TelescopeScraper
     from I_BufftoonScraper import BufftoonScraper
     from J_NaverPostScraper import NaverPostScraper
     from K_NaverGameScraper import NaverGameScraper
+    from L_LezhinComicsScraper import LezhinComicsScraper
 else:
     from .A_FolderManager import FolderManager
     from .D_NaverWebtoonScraper import NaverWebtoonScraper
     from .E_BestChallengeScraper import BestChallengeScraper
     from .F_WebtoonOriginalsScraper import WebtoonOriginalsScraper
     from .G_WebtoonCanvasScraper import WebtoonCanvasScraper
     from .H_TelescopeScraper import TelescopeScraper
     from .I_BufftoonScraper import BufftoonScraper
     from .J_NaverPostScraper import NaverPostScraper
     from .K_NaverGameScraper import NaverGameScraper
+    from .L_LezhinComicsScraper import LezhinComicsScraper
 
 N = NAVER_WEBTOON = 'naver_webtoon'
 B = BEST_CHALLENGE = 'best_challenge'
 O = ORIGINALS = 'originals'  # noqa
 C = CANVAS = 'canvas'
 T = M = TELESCOPE = 'telescope'
 BF = BUFFTOON = 'bufftoon'
 P = POST = NAVER_POST = 'naver_post'
 G = NAVER_GAME = 'naver_game'
+L = LEZHIN = 'lezhin'
 
 
-async def get_webtoon_platform(webtoon_id: int, is_auto_select=False) -> str | None:  # noqa
+async def get_webtoon_platform(webtoon_id: int | str, is_auto_select=False) -> str | None:  # noqa
     # sourcery skip: low-code-quality
     """If webtoon is best challenge, this returns True. Otherwise, False."""
     loop = asyncio.get_running_loop()
 
     async def skip_when_errored(func, platform_name):
         try:
             # await func()
@@ -113,27 +117,51 @@
     async def canvas_fetch():
         title = await webtoonscraper.get_internet('soup_select_one', f'https://www.webtoons.com/en/challenge/meme-girls/list?title_no={webtoon_id}',
                                                   'meta[property="og:title"]')
         with contextlib.suppress(AttributeError):
             if title := title.get('content'):
                 available_webtoon.append((CANVAS, title))
 
+    # lezhin
+    async def lezhin_fetch():
+        # 불필요한 페칭 방지: int라면 어차피 lezhin일 수 없음. 이미 앞에서 걸리지긴 하지만 만약을 대비해 준비함.
+        if isinstance(webtoon_id, int):
+            return
+
+        title = await webtoonscraper.get_internet('soup_select_one', f'https://www.lezhin.com/ko/{webtoon_id}',
+                                                  'h2.comicInfo__title')
+
+        if title is None:
+            return
+
+        available_webtoon.append((LEZHIN, title.text))
+
     # 전체 동시 실행
-    webtoon_getters = starmap(
-        skip_when_errored,
-        (
-            (naver_webtoon_fetch, NAVER_WEBTOON),
-            (best_challenge_fetch, BEST_CHALLENGE),
-            (telescope_fetch, TELESCOPE),
-            (bufftoon_fetch, BUFFTOON),
-            (naver_game_fetch, NAVER_GAME),
-            (originals_fetch, ORIGINALS),
-            (canvas_fetch, CANVAS)
+    if isinstance(webtoon_id, int):
+        webtoon_getters = starmap(
+            skip_when_errored,
+            (
+                (naver_webtoon_fetch, NAVER_WEBTOON),
+                (best_challenge_fetch, BEST_CHALLENGE),
+                (telescope_fetch, TELESCOPE),
+                (bufftoon_fetch, BUFFTOON),
+                (naver_game_fetch, NAVER_GAME),
+                (originals_fetch, ORIGINALS),
+                (canvas_fetch, CANVAS),
+            )
         )
-    )
+    else:
+        logging.info('webtoon_id is string, so it checks if it is lezhin or not.')
+        webtoon_getters = starmap(
+            skip_when_errored,
+            (
+                (lezhin_fetch, LEZHIN),
+            )
+        )
+
     await asyncio.gather(*webtoon_getters)
 
     # 베스트 도전과 네이버 웹툰이 겹치고 둘의 제목이 같을 경우 베스트 도전을 배제함.
     nw_title, bc_title, bc_order = None, None, 0
     for i, (platform, title) in enumerate(available_webtoon):
         if platform == NAVER_WEBTOON:
             nw_title = title
@@ -180,77 +208,71 @@
         webtoonscraper = TelescopeScraper()
     elif webtoon_type.lower() == BUFFTOON:
         webtoonscraper = BufftoonScraper()
     elif webtoon_type.lower() == NAVER_POST:
         webtoonscraper = NaverPostScraper()
     elif webtoon_type.lower() == NAVER_GAME:
         webtoonscraper = NaverGameScraper()
+    elif webtoon_type.lower() == LEZHIN:
+        webtoonscraper = LezhinComicsScraper()
     else:
-        raise ValueError('webtoon_type should be among naver_webtoon, best_challenge, originals, canvas, bufftoon, telescope, naver_post, and naver_game.')
+        raise ValueError('webtoon_type should be among naver_webtoon, best_challenge, originals, canvas, bufftoon, telescope, naver_post, naver_game, and lezhin.')
     return webtoonscraper
 
 
 async def get_webtoon_async(
-        webtoon_id: int | tuple[int, int],
+        webtoon_id: int | tuple[int, int] | str,
         webtoon_type: None | str = None,
         *,
         merge: None | int = None,
         cookie: None | str = None,
         is_auto_select=False,
         episode_no_range: tuple[int, int] | int | None = None,
+        authorization: None | str = None
 ) -> None:
     def set_cookie(cookie):
         webtoonscraper = BufftoonScraper()
         if cookie:
             webtoonscraper.COOKIE = cookie
         else:
             webtoonscraper.COOKIE = input(f'Enter cookie of {webtoon_id} (Enter nothing to proceed without cookie): ')
         return webtoonscraper
 
-    if cookie is None:
+    if cookie is None and authorization is None:
         if isinstance(webtoon_id, tuple):
             webtoon_type = NAVER_POST
         elif webtoon_type is None:
             webtoon_type = await get_webtoon_platform(webtoon_id, is_auto_select)
             if webtoon_type is None:
                 raise ValueError('You must select item.')
 
         if webtoon_type.lower() == BUFFTOON:
             webtoonscraper = set_cookie(cookie)
         else:
             webtoonscraper = await get_scraper_instance(webtoon_type)
-    else:
+    elif cookie is not None:
         webtoonscraper = set_cookie(cookie)
-
-    # if webtoon_type is None and cookie is None:
-    #     if isinstance(webtoon_id, tuple):
-    #         webtoon_type = NAVER_POST
-    #     else:
-    #         webtoon_type = await get_webtoon_platform(webtoon_id, is_auto_select)
-    #         if webtoon_type is None:
-    #             raise ValueError('You must select item.')
-
-    # if cookie is not None or webtoon_type.lower() == BUFFTOON:
-    #     webtoonscraper = await get_scraper_instance(BUFFTOON)
-    #     if cookie:
-    #         webtoonscraper.COOKIE = cookie
-    #     else:
-    #         webtoonscraper.COOKIE = input(f'Enter cookie of {webtoon_id} (Enter nothing to proceed without cookie): ')
-    # else:
-    #     webtoonscraper = await get_scraper_instance(webtoon_type)
+    elif authorization is not None:
+        webtoonscraper = LezhinComicsScraper()
+        webtoonscraper.AUTHORIZATION = authorization
+    else:
+        raise ValueError('Placeholder for later new ones.')
 
     await webtoonscraper.download_one_webtoon_async(webtoon_id, episode_no_range, merge=merge)
 
+
 def get_webtoon(
-    webtoon_id: int,
-    webtoon_type: str | None = None,
-    *,
-    merge: None | int = None,
-    cookie: None | str = None,
-    episode_no_range: tuple[int, int] | int | None = None,
+        webtoon_id: int | tuple[int, int] | str,
+        webtoon_type: None | str = None,
+        *,
+        merge: None | int = None,
+        cookie: None | str = None,
+        is_auto_select=False,
+        episode_no_range: tuple[int, int] | int | None = None,
+        authorization: None | str = None
 ) -> None:
-    asyncio.run(get_webtoon_async(webtoon_id, webtoon_type, merge=merge, cookie=cookie, episode_no_range=episode_no_range))
+    asyncio.run(get_webtoon_async(webtoon_id, webtoon_type, merge=merge, cookie=cookie, is_auto_select=is_auto_select, episode_no_range=episode_no_range, authorization=authorization))
 
 
 if __name__ == '__main__':
     # asyncio.run(get_webtoon_platform(18))  # 네이버 게임
     asyncio.run(get_webtoon_platform(1022))  # 오리지널스
```

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/C_Scraper.py` & `WebtoonScraper-1.2.0/WebtoonScraper/C_Scraper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Abstract Class of all scrapers."""
-# solved: file_acceptable built-in으로 만들기
-# solved: titleid tuple도 허용해서 NPScraper에서 이용할 수 있도록 하기
-# SOLVED: get_data 시 list로 정보 받아오기
+# [x]: file_acceptable built-in으로 만들기
+# [x]: titleid tuple도 허용해서 NPScraper에서 이용할 수 있도록 하기
+# [x]: get_data 시 list로 정보 받아오기
 # TODO: None 대신 NoReturn 사용하기
 # TODO: download vs save : 용어 정리하기
-# TODO: 카카오 웹툰/카카오 페이지 웹툰, 레진 코믹스도 만들기 (HURRY!)
-# FIXME: episode_no와 episode_id를 구분해야 함!!!
+# TODO: 카카오 웹툰/카카오 페이지 웹툰, 네이버 블로그 만들기
 # TODO: short_connection 등 docs 추가하기
 # TODO: Webtoon get_webtoon_platform 조금 더 잘 만들 방법 강구하기
+# TODO: annotations 추가하고 필요 version낮추기
+# TODO: print문 모두 제거하고 logging으로 변경하기
+# TODO: get_webtoon_data에서 dataclass같은 걸 이용해서 self.webtoon_data.titleid같을 걸로 이용할 수 있도록 함.
 import re
 import os
 import asyncio
 import shutil
 import html
 from pathlib import Path
 # from typing import Iterable, Literal
-from typing import Literal
+from typing import Literal, NoReturn
 from abc import abstractmethod, ABCMeta
 # from collections import namedtuple
 # from contextlib import suppress
 from typing import overload
 # import logging
 
 import requests
@@ -30,15 +32,15 @@
 from async_lru import alru_cache
 
 if __name__ in ("__main__", "C_Scraper"):
     from A_FolderManager import FolderManager
 else:
     from .A_FolderManager import FolderManager
 
-TitleId = int | tuple[int, int]
+TitleId = int | tuple[int, int] | str
 
 
 class Scraper(metaclass=ABCMeta):
     """Abstract class of all scrapers.
 
     init, get_internet, 전반적인 로직 등은 모두 이 페이지에서 관리하고, 구체적인 다운로드 방법은 각각의 scraper들에게 맡깁니다.
     따라서 썸네일을 받아오거나 한 회차의 이미지 URL을 불러오는 등의 역할은 각자 scraper들에 구현되어 있습니다.
@@ -60,15 +62,15 @@
         self.BASE_DIR = 'webtoon'
         self.TIMEOUT = 120
         self.PBAR_INDEPENDENT = pbar_independent
         self.IS_STABLE_CONNECTION = None  # IS_STABLE_CONNECTION must be defined!
         self.short_connection = False
 
     @property
-    def short_connection(self):
+    def short_connection(self) -> bool:
         return self._short_connection
 
     @short_connection.setter
     def short_connection(self, short_connection: bool):
         """
         이 함수는 short_connection을 설정합니다.
         short_connection에는 특징이 있는데, True로 바꾸는 순간 그 전에 설정한 IS_STABLE_CONNECTION과
@@ -216,19 +218,19 @@
                     is_success = True
                     break
             if not is_success:
                 raise ConnectionError('Trying hard but failed. Maybe low attempt or timeout settizng is reason.'
                                       ' Trying increasing attempt time or timeout. Or sometimes it is caused by invaild titleid.')
 
         if get_type in ('soup', 'soup_select', 'soup_select_one'):
-            if selector is None:
-                raise ValueError('Selector can\'t be None.')
             soup = bs(response.text, "html.parser")
             if get_type == 'soup':
                 return soup
+            if selector is None:
+                raise ValueError('Selector can\'t be None.')
             if get_type == 'soup_select':
                 return soup.select(selector)
             if get_type == 'soup_select_one':
                 return soup.select_one(selector)
         elif get_type == 'requests':
             return response
         else:
@@ -262,15 +264,15 @@
 
         Args:
             filename_or_url: 파일 확장자가 궁금한 파일명이나 URL. 이때 URL 쿼리는 무시됩니다.
 
         Returns:
             파일 확장자를 반환합니다.
         """
-        serch_result: re.Match | None = re.search(r'(?<=[.])(jpg|png|jpeg|gif)(?=[?].+$|$)', filename_or_url, re.I)
+        serch_result: re.Match | None = re.search(r'(?<=[.])(jpg|png|jpeg|gif|webp)(?=[?].+$|$)', filename_or_url, re.I)
 
         return None if serch_result is None else serch_result[0]
         # return filename_or_url.split('.')[-1].lower()
 
     @staticmethod
     def get_safe_file_name(file_or_diretory_name: str) -> str:
         """Translate file or diretory name to accaptable name.
@@ -316,15 +318,16 @@
                                 int일 경우: 한 회차만 다운로드 받는다.
                                 None일 경우: 웹툰의 모든 회차를 다운로드 받는다.
         :merge: 웹툰을 모두 다운로드 받은 뒤 웹툰을 묶는다.
         """
         self.loop = asyncio.get_running_loop()
 
         title = self.get_safe_file_name(await self.get_title(titleid))
-        webtoon_dir = self.BASE_DIR / f'{title}({titleid})'
+        webtoon_dir_name = await self.get_webtoon_dir_name(titleid, title)
+        webtoon_dir = self.BASE_DIR / webtoon_dir_name
         self.webtoon_dir = webtoon_dir
 
         webtoon_dir.mkdir(parents=True, exist_ok=True)
 
         await self.save_webtoon_thumbnail(titleid, title, webtoon_dir)
 
         episode_no_list = await self.get_all_episode_no(titleid)
@@ -338,21 +341,30 @@
 
         # episode_nos_plus_1 starts with 1, but episode_no starts with 0, so it needs to be subtracted from 1
         self.pbar = tqdm([i - 1 for i in episode_no_list_plus_1])
         for episode_no in self.pbar:
             await self.download_one_episode(episode_no, titleid, webtoon_dir)
         print(f'A webtoon {title} download ended.')
 
+        webtoon_dir = await self.lezhin_unshuffle_process(titleid, webtoon_dir)
+
         if merge is not None:
             print('Merging webtoon has started...')
             fd = FolderManager()
-            print(webtoon_dir, fd)
+            # print(webtoon_dir, fd)
             fd.merge_webtoon_episodes(webtoon_dir, 5)
             print('Merging webtoon ended.')
 
+    async def get_webtoon_dir_name(self, titleid: TitleId, title: str) -> str:
+        return f'{title}({titleid})'
+
+    async def lezhin_unshuffle_process(self, titleid: TitleId, base_webtoon_dir: Path):
+        """For lezhin's shuffle process. This function changes webtoon_dir to unshuffled webtoon's directory."""
+        return base_webtoon_dir
+
     def _check_validate_of_files(self, episode_dir: Path, episode_no: int, image_urls: list, subtitle: str) -> None | bool:
         """episode_dir를 생성하고 이미 있다면 해당 폴더 내 내용물이 적합한지 조사한다.
 
         None를 return한다면 회차를 다운로드해야 한다는 의미이다.
         True를 return하면 해당 회차가 이미 완전히 다운로드되어 있으며, 따라서 다운로드를 지속할 이유가 없음을 의미한다.
         """
         try:
@@ -375,14 +387,19 @@
         if not subtitle:
             print(f'this episode is not free or not yet created. This episode won\'t be loaded. {episode_no=}')
             self._set_pbar('unknown episode')
             return
 
         episode_images_url = await self.get_episode_images_url(titleid, episode_no)
 
+        if episode_images_url is None:  # for lezhin
+            print(f'this episode is not free or not yet created. This episode won\'t be loaded. {episode_no=}')
+            self._set_pbar('unknown episode')
+            return
+
         episode_dir = webtoon_dir / f'{episode_no + 1:04d}. {subtitle}'
         if self._check_validate_of_files(episode_dir, episode_no, episode_images_url, subtitle):
             return
 
         self._set_pbar(f'downloading {subtitle}')
         get_image_coroutines = (self.download_single_image(episode_dir, element, i) for i, element in enumerate(episode_images_url))
         await asyncio.gather(*get_image_coroutines)
@@ -424,19 +441,23 @@
 
     @abstractmethod
     async def get_subtitle(self, titleid: TitleId, episode_no: int) -> str:
         """부제목, 즉 회차의 제목을 불러온다. 기본 구현을 사용할 시 super()를 이용하세요."""
         return (await self.get_webtoon_data(titleid))['subtitles'][episode_no]
 
     @abstractmethod
-    async def save_webtoon_thumbnail(self, titleid: TitleId, title: str, thumbnail_dir: Path) -> None:
+    async def save_webtoon_thumbnail(self, titleid: TitleId, title: str, thumbnail_dir: Path, default_file_extension: str | None = None) -> None:
         """웹툰의 썸네일을 불러오고 thumbnail_dir에 저장합니다. 기본 구현을 사용할 시 super()를 이용하세요."""
         thumbnail_data: str | tuple[bytes, str] = (await self.get_webtoon_data(titleid))['webtoon_thumbnail']
         if isinstance(thumbnail_data, str):  # It means thumnail_data is URL
             image_extension = self.get_file_extension(thumbnail_data)
+            if image_extension is None:
+                if default_file_extension is None:
+                    raise ValueError('File extension not detected.')
+                image_extension = default_file_extension
             image_raw = (await self.get_internet(get_type='requests', url=thumbnail_data)).content
         elif isinstance(thumbnail_data, tuple):  # It means thumnail_data is raw image data
             image_raw, image_extension = thumbnail_data
         else:
             raise ValueError('Thumbnail_data is invalid; It must be string or bytes.')
 
         image_path = thumbnail_dir / f'{title}.{image_extension}'
```

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/D_NaverWebtoonScraper.py` & `WebtoonScraper-1.2.0/WebtoonScraper/D_NaverWebtoonScraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 '''Download Webtoons from Naver Webtoon.'''
 from itertools import count
+
 from async_lru import alru_cache
 
 if __name__ in ("__main__", "D_NaverWebtoonScraper"):
     from C_Scraper import Scraper
 else:
     # from Scraper import Scraper
     from .C_Scraper import Scraper
```

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/E_BestChallengeScraper.py` & `WebtoonScraper-1.2.0/WebtoonScraper/E_BestChallengeScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/F_WebtoonOriginalsScraper.py` & `WebtoonScraper-1.2.0/WebtoonScraper/F_WebtoonOriginalsScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/G_WebtoonCanvasScraper.py` & `WebtoonScraper-1.2.0/WebtoonScraper/G_WebtoonCanvasScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/H_TelescopeScraper.py` & `WebtoonScraper-1.2.0/WebtoonScraper/H_TelescopeScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/I_BufftoonScraper.py` & `WebtoonScraper-1.2.0/WebtoonScraper/I_BufftoonScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/J_NaverPostScraper.py` & `WebtoonScraper-1.2.0/WebtoonScraper/J_NaverPostScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/K_NaverGameScraper.py` & `WebtoonScraper-1.2.0/WebtoonScraper/K_NaverGameScraper.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper/__init__.py` & `WebtoonScraper-1.2.0/WebtoonScraper/__init__.py`

 * *Files identical despite different names*

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper.egg-info/PKG-INFO` & `WebtoonScraper-1.2.0/WebtoonScraper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WebtoonScraper
-Version: 1.1.1
+Version: 1.2.0
 Summary: Scraping webtoons and some utils for it
 Home-page: https://github.com/ilotoki0804/WebtoonScraper
 Author: ilotoki0804
 Author-email: ilotoki0804@gmail.com
 License: MIT
 Keywords: Webtoon,Webtoon Scraper,Naver Webtoon,Webtoon Downloader,Download Webtoon
 Classifier: License :: OSI Approved :: MIT License
@@ -16,20 +16,20 @@
 License-File: LICENSE
 
 이 설명은 최신 버전이 아닐 수 있습니다. 만약 최신 버전을 확인하고 싶으시다면 [여기](https://github.com/ilotoki0804/WebtoonScraper)를 참고하세요.
 # WebtoonScraper
 
 웹툰을 다운로드하는 프로젝트입니다.
 
-네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임을 지원합니다.
+네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 버프툰, 네이버 포스트, 네이버 게임, 레진 코믹스를 지원합니다.
 
 # 시작하기
 
 1. 파이썬을 설치합니다.
-2. cmd 창을 열어 pip 명령어를 실행합니다.
+2. 터미널에서 다음과 같은 명령어를 실행합니다.
    ```
    pip install -U WebtoonScraper
    ```
 
 # 네이버 웹툰, 베스트 도전만화, 웹툰 오리지널, 웹툰 캔버스, 만화경, 네이버 게임 다운로드하기
 
 버프툰과 네이버 포스트는 아래로 가서 확인하세요.
@@ -40,14 +40,16 @@
    웹툰 오리지널/캔버스(webtoons.com):
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/webtoons_original.png)
    만화경(manhwakyung.com)
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/manhwakyung.png)
    네이버 게임 오리지널 시리즈(game.naver.com/original_series):
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_game.png)
    버프툰과 네이버 포스트는 아래의 '버프툰 다운로드하기'섹션과 '네이버 포스트 다운로드하기' 섹션을 참고해 주세요.
+   레진코믹스는 따로 준비된 스크린샷은 없습니다만 방법은 네이버 게임 오리지널과 같습니다.
+   레진코믹스는 titleid가 문자열이라는 점에 참고하세요.
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요. 웹툰은 정식 연재와 베스트 도전, Webtoons 오리지널과 캔버스, 만화경, 네이버 게임 모두 가능합니다.
 
    ```python
    from WebtoonScraper import Webtoon as wt
 
    # 네이버 웹툰
    wt.get_webtoon(76648, wt.N)  # titleid를 여기에다 붙여넣으세요.
@@ -62,26 +64,31 @@
    # 네이버 게임 오리지널 시리즈
    wt.get_webtoon(5, wt.G)  # titleid를 여기에다 붙여넣으세요.
    # 버프툰
    cookie = 'cookie here'  # cookie를 여기에다 붙여넣으세요. 자세한 설명은 아래의 '버프툰 다운로드하기'를 참고하세요.
    wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # titleid를 여기에다 붙여넣으세요.
    # 네이버 포스트
    wt.get_webtoon((597061, 19803452), wt.P)  # seriesNo와 memberNo를 각각 붙여넣으세요. 자세한 설명은 아래의 '네이버 포스트 다운받기'를 참고하세요.
+   # 레진코믹스
+   authorization = 'authorization here'  # authorization을 여기에다 붙여넣으세요. 자세한 설명은 아래의 '레진코믹스 다운로드하기'를 참고하세요.
+   wt.get_webtoon('some_webtoon', wt.L, authorization=authorization)  # titleid를 여기에다 붙여넣으세요.
    ```
 
    이제 웹툰이 webtoons 폴더에 다운로드됩니다.
 
    cf. 웹툰 태그를 생략하면 해당 웹툰이 어떤 사이트의 웹툰 id인지 자동으로 알아냅니다. 만약 몇몇 태그가 겹친다면 태그에 맞는 수를 입력하는 창에 알맞은 수를 입력하면 됩니다.
 
    episode_no_range 키워드를 이용하면 특정한 에피소드만 다운로드받을 수 있습니다.
+
    ```python
    wt.get_webtoon(5, wt.G, episode_no_range=(1,20))  # 1화부터 20화까지
    ```
 
    merge 키워드를 이용하면 webtoon 폴더 내에 있는 모든 웹툰을 원하는 개수 만큼 묶습니다.
+
    ```python
    wt.get_webtoon(5, wt.G, merge=5)
    ```
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
@@ -123,32 +130,56 @@
    wt.get_webtoon(1007888, wt.BF, cookie=cookie)  # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
    ```
 6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
 
 ## 주의사항
 
 * get_webtoon에서 cookie를 입력하면 자동으로 버프툰으로 인식합니다.
+* favicon.ico가 요청에 뜨지 않는다면 ctrl+R을 해보고, 그래도 없다면 `필터`에서 `모두`로 설정되어 있는지 다시 확인하세요.
 
 # 네이버 포스트 다운로드하기
 
-1. 웹툰이 있는 페이지로 가서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
+1. 웹툰이 있는 페이지로 가서 주소창에서 seriesNo와 memberNo를 복사하세요. 예시에서는 각각 597061과 19803452입니다.
    ![img](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/images/naver_post.png)
 2. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
    ```python
    from WebtoonScraper import Webtoon as wt
 
-   wt.get_webtoon((597061, 19803452), wt.P)
+   wt.get_webtoon((597061, 19803452), wt.P)  # 여기에 아까 복사한 seriesNo와 memberNo를 붙여넣으세요.
    ```
 3. 만화 뷰어 앱을 통해 다운로드한 웹툰을 시청할 수 있습니다.
 
 ## 주의사항
 
 * 가끔씩 이유 없는 오류가 발생할 수 있습니다. 그럴 때는 조금 시간이 지난 후에 다시 시도해 보세요.
 * tuple를 입력하면 자동으로 포스트로 인식됩니다.
 
+# 레진코믹스 다운로드하기
+
+로그인하지 않은 상태에서도 웹툰을 다운로드받을 수 있으나, 받을 수 있는 에피소드의 개수가 제한된다는 점을 유의해 주십세요.
+로그인하지 않은 상태이더라도 웹툰을 다운로드받을 수는 있습니다.
+
+1. 웹툰 페이지에 들어가 주소창의 맨 마지막 문자열을 복사합니다.
+2. 로그인을 하고 f12를 누르고 네트워크 창을 연 뒤 웹툰 페이지에 들어갑니다.
+3. 새로고침을 한 뒤 '이름'에 있는 `balance?lezhinObjectId=...&lezhinObjectType=comic`(찾기 조금 어려울 수 있습니다.) 요청을 클릭하고 나온 창에 '헤더' 탭을 엽니다.
+4. 내려서 Authorization: 이라고 되어 있는 모든 내용을 복사합니다.
+5. 다음의 파이썬 코드를 웹툰이 다운로드되길 원하는 폴더 내에서 실행해 주세요.
+   ```python
+   from WebtoonScraper import Webtoon as wt
+   authorization = '두 번째로 복사했던 문자를 여기에다 붙여넣으세요.'
+   wt.get_webtoon(1007888, wt.L, authorization=authorization)  # 첫 번째로 복사했던 수를 여기에다 붙여넣으세요.
+   ```
+6. 로그인하면 볼 수 있는 모든 에피소드가 다운로드됩니다.
+
+## 주의사항
+
+* 다른 웹툰 플렛폼과는 다르게 titleid가 문자열입니다.
+* 다른 웹툰 플랫폼들에 비해 다운로드 속도가 비교적 느린 편입니다.
+* 일부 웹툰은 셔플링이 되어 있습니다. 따라서 웹툰을 다 다운로드받은 후 언셔플링을 하는 과정이 필요하며, 이 과정에 다소 시간이 소요된다는 점 참고 바랍니다.
+
 # 여러 회차 하나로 묶기
 
 1. 웹툰을 상기한 대로 다운로드받습니다.
 2. 다음과 같이 코드를 짭니다.
    ```python
    from WebtoonScraper import FolderManager
 
@@ -173,14 +204,16 @@
    fm= FolderManager()
    fm.restore_webtoons_in_directory()
    ```
 3. 'webtoon' 폴더에 있던 모든 웹툰이 웹툰을 처음 다운로드했던 상태로 되돌아갑니다.
 
 # Relese Note
 
+1.2.0: 레진코믹스 추가, 의존성 증가(pyjsparser, Pillow)
+
 1.1.1: 내부 모듈 이름 변경, merge option 추가, abstractmethod들의 일반 구현 추가
 
 1.0.2: 대형 리팩토링, get_webtoon_platform 비동기 방식으로 속도 개선, 상대경로로 변경, 테스트 추가
 
 1.0.1: 코드 개선 및 리팩토링, api를 통한 로직으로 변경 (버그가 많기에 사용을 권장하지 않음)
 
 1.0.0: 네이버 게임 추가, FolderManager 리펙토링 및 개선, 정식 버전, docs 개선
```

### Comparing `WebtoonScraper-1.1.1/WebtoonScraper.egg-info/SOURCES.txt` & `WebtoonScraper-1.2.0/WebtoonScraper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 WebtoonScraper/E_BestChallengeScraper.py
 WebtoonScraper/F_WebtoonOriginalsScraper.py
 WebtoonScraper/G_WebtoonCanvasScraper.py
 WebtoonScraper/H_TelescopeScraper.py
 WebtoonScraper/I_BufftoonScraper.py
 WebtoonScraper/J_NaverPostScraper.py
 WebtoonScraper/K_NaverGameScraper.py
+WebtoonScraper/L_LezhinComicsScraper.py
 WebtoonScraper/__init__.py
 WebtoonScraper.egg-info/PKG-INFO
 WebtoonScraper.egg-info/SOURCES.txt
 WebtoonScraper.egg-info/dependency_links.txt
 WebtoonScraper.egg-info/not-zip-safe
 WebtoonScraper.egg-info/requires.txt
 WebtoonScraper.egg-info/top_level.txt
```

### Comparing `WebtoonScraper-1.1.1/setup.py` & `WebtoonScraper-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description += Path('README.md').read_text(encoding='utf-8')
 # 사진 대체
 repl = r'![\g<1>](https://raw.githubusercontent.com/ilotoki0804/WebtoonScraper/master/\g<2>)'
 long_description = re.sub(r'!\[(.+?)\]\((images\/.+?)\)', repl, long_description)
 
 setup(
     name='WebtoonScraper',
-    version='1.1.1',
+    version='1.2.0',
     description='Scraping webtoons and some utils for it',
     author='ilotoki0804',
     author_email='ilotoki0804@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/ilotoki0804/WebtoonScraper',
```

### Comparing `WebtoonScraper-1.1.1/test/test.py` & `WebtoonScraper-1.2.0/test/test.py`

 * *Files identical despite different names*

