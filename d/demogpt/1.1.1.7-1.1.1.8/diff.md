# Comparing `tmp/demogpt-1.1.1.7.tar.gz` & `tmp/demogpt-1.1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demogpt-1.1.1.7.tar", last modified: Sat Jul 22 20:49:08 2023, max compression
+gzip compressed data, was "demogpt-1.1.1.8.tar", max compression
```

## Comparing `demogpt-1.1.1.7.tar` & `demogpt-1.1.1.8.tar`

### file list

```diff
@@ -1,50 +1,10 @@
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:08.000589 demogpt-1.1.1.7/
--rw-rw-r--   0 melih     (1000) melih     (1000)     1069 2023-06-07 10:58:37.000000 demogpt-1.1.1.7/LICENSE
--rw-rw-r--   0 melih     (1000) melih     (1000)      409 2023-07-22 20:49:08.000589 demogpt-1.1.1.7/PKG-INFO
--rw-rw-r--   0 melih     (1000) melih     (1000)     6530 2023-07-19 15:30:18.000000 demogpt-1.1.1.7/README.md
--rw-rw-r--   0 melih     (1000) melih     (1000)       38 2023-07-22 20:49:08.000589 demogpt-1.1.1.7/setup.cfg
--rw-rw-r--   0 melih     (1000) melih     (1000)      832 2023-07-22 20:49:01.000000 demogpt-1.1.1.7/setup.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:07.992589 demogpt-1.1.1.7/src/
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:07.996589 demogpt-1.1.1.7/src/alpha/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4995 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/agent_prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     3868 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/app.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:07.996589 demogpt-1.1.1.7/src/alpha/chains/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/chains/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     2444 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/chains/chains.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     7505 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/chains/prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4277 2023-07-22 17:12:22.000000 demogpt-1.1.1.7/src/alpha/code.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1820 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/example_generation.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8510 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/langchain_agent.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8899 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/langchain_coder.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4368 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/langchain_expert.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     5537 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/model.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1963 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/alpha/utils.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:07.996589 demogpt-1.1.1.7/src/beta/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 08:30:31.000000 demogpt-1.1.1.7/src/beta/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4995 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/agent_prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     3868 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/app.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:07.996589 demogpt-1.1.1.7/src/beta/chains/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-21 08:30:31.000000 demogpt-1.1.1.7/src/beta/chains/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     2444 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/chains/chains.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     7505 2023-07-21 08:30:31.000000 demogpt-1.1.1.7/src/beta/chains/prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1820 2023-07-21 08:30:31.000000 demogpt-1.1.1.7/src/beta/example_generation.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8510 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/langchain_agent.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     8898 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/langchain_coder.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4368 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/langchain_expert.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     5537 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/beta/model.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     1963 2023-07-21 08:30:31.000000 demogpt-1.1.1.7/src/beta/utils.py
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:08.000589 demogpt-1.1.1.7/src/demogpt.egg-info/
--rw-rw-r--   0 melih     (1000) melih     (1000)      409 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/PKG-INFO
--rw-rw-r--   0 melih     (1000) melih     (1000)     1020 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/SOURCES.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)        1 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/dependency_links.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)       50 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/entry_points.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)       41 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/requires.txt
--rw-rw-r--   0 melih     (1000) melih     (1000)       24 2023-07-22 20:49:07.000000 demogpt-1.1.1.7/src/demogpt.egg-info/top_level.txt
-drwxrwxr-x   0 melih     (1000) melih     (1000)        0 2023-07-22 20:49:08.000589 demogpt-1.1.1.7/src/prompt_based/
--rw-rw-r--   0 melih     (1000) melih     (1000)        0 2023-07-22 20:22:29.000000 demogpt-1.1.1.7/src/prompt_based/__init__.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     4158 2023-07-22 20:22:27.000000 demogpt-1.1.1.7/src/prompt_based/app.py
--rw-rw-r--   0 melih     (1000) melih     (1000)      230 2023-07-22 20:32:48.000000 demogpt-1.1.1.7/src/prompt_based/cli.py
--rw-rw-r--   0 melih     (1000) melih     (1000)    10642 2023-07-22 20:48:24.000000 demogpt-1.1.1.7/src/prompt_based/model.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     6115 2023-07-21 17:19:00.000000 demogpt-1.1.1.7/src/prompt_based/prompts.py
--rw-rw-r--   0 melih     (1000) melih     (1000)     6169 2023-07-09 11:27:25.000000 demogpt-1.1.1.7/src/prompt_based/prompts.txt
+-rw-r--r--   0        0        0     1069 2023-06-07 10:58:37.634100 demogpt-1.1.1.8/LICENSE
+-rw-r--r--   0        0        0     7796 2023-07-26 19:08:40.283549 demogpt-1.1.1.8/README.md
+-rw-r--r--   0        0        0      736 2023-07-26 23:32:18.300869 demogpt-1.1.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-22 20:22:29.809285 demogpt-1.1.1.8/src/prompt_based/__init__.py
+-rw-r--r--   0        0        0     4175 2023-07-26 18:39:20.445611 demogpt-1.1.1.8/src/prompt_based/app.py
+-rw-r--r--   0        0        0      232 2023-07-26 16:32:26.414466 demogpt-1.1.1.8/src/prompt_based/cli.py
+-rw-r--r--   0        0        0    11248 2023-07-26 20:43:27.076622 demogpt-1.1.1.8/src/prompt_based/model.py
+-rw-r--r--   0        0        0     6115 2023-07-26 16:32:26.414466 demogpt-1.1.1.8/src/prompt_based/prompts.py
+-rw-r--r--   0        0        0     6169 2023-07-09 11:27:25.126475 demogpt-1.1.1.8/src/prompt_based/prompts.txt
+-rw-r--r--   0        0        0     8573 1970-01-01 00:00:00.000000 demogpt-1.1.1.8/PKG-INFO
```

### Comparing `demogpt-1.1.1.7/LICENSE` & `demogpt-1.1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.7/README.md` & `demogpt-1.1.1.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 <p align="center">
 <a href=""><img src="assets/banner_small.png" alt="DemoGPT logo: Generate automatic LangChain pipelines" width="450px"></a>
 </p>
 
 <p align="center">
 <b>⚡ With just a prompt, you can create interactive Streamlit apps via 🦜️🔗 LangChain's transformative capabilities & Llama 2.⚡</b>
 </p>
-
 <p align="center">
+<a href="https://pepy.tech/project/demogpt"><img src="https://static.pepy.tech/badge/demogpt/month" alt="Downloads"></a>
 <a href="https://github.com/melih-unsal/DemoGPT/releases"><img src="https://img.shields.io/github/release/melih-unsal/DemoGPT" alt="Releases"></a>
 <a href="https://demogpt.io"><img src="https://img.shields.io/badge/Official%20Website-demogpt.io-blue?style=flat&logo=world&logoColor=white" alt="Official Website"></a>
 <a href="https://melih-unsal.github.io/DemoGPT-Docs/"><img src="https://img.shields.io/badge/Documentation-📘-blueviolet" alt="DemoGPT Documentation"></a>
 </p>
 
 <p align="center">
 <a href="docs/README_CN.md"><img src="https://img.shields.io/badge/文档-中文版-blue.svg" alt="CN doc"></a>
@@ -34,14 +34,19 @@
 </p>
 
 <p align="center">
 <a href="https://demogpt.streamlit.app"><img src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg" alt="Streamlit application"></a>
 <a href="https://huggingface.co/spaces/melihunsal/demogpt"><img src="https://img.shields.io/badge/%F0%9F%A4%97-Spaces-yellow"></a>
 </p>
 
+<p align="center">
+<a href="https://www.producthunt.com/posts/demogpt"><img src="https://img.shields.io/static/v1?style=for-the-badge&message=Product+Hunt&color=DA552F&logo=Product+Hunt&logoColor=FFFFFF&label=" alt="Product Hunt" height="25"/></a>
+<a href="https://demogpt.medium.com/"><img src="https://img.shields.io/static/v1?style=for-the-badge&message=Medium&color=000000&logo=Medium&logoColor=FFFFFF&label=" alt="DemoGPT Medium" height="25"/></a>
+</p>
+
 ## ⭐ Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=melih-unsal/DemoGPT&type=Timeline)](https://star-history.com/#melih-unsal/DemoGPT&Timeline)
 
 ⭐ Consider starring us if you're using DemoGPT so more people hear about us!
 
 ## 🔥 Demo
@@ -54,14 +59,28 @@
 
 ## 📚 Documentation
 
 See our documentation site [here](https://melih-unsal.github.io/DemoGPT-Docs/) for full how-to docs and guidelines
 
 ⚡ The new release with the power of **Llama 2** is within a week. ⚡
 
+## 📦 Using DemoGPT Package
+
+The DemoGPT package is now available and can be installed using pip. Run the following command to install the package:
+
+```sh
+pip install demogpt
+```
+
+To use the DemoGPT application, simply type "demogpt" into your terminal:
+
+```sh
+demogpt
+```
+
 
 ## 📑 Table of Contents
 
 - [Introduction](#-introduction)
 - [Pipeline](#%EF%B8%8F-pipeline)
 - [Installation](#-installation)
 - [Usage](#-usage)
@@ -86,14 +105,25 @@
 
 ## ⚙️ Architecture
 ### DemoGPT Architecture
 ![DemoGPT Architecture](assets/demogpt_new_pipeline1.jpeg?raw=true "DemoGPT Architecture")
 
 ## 🔧 Installation
 
+### For the Package Version
+
+You can install the DemoGPT package by running the following command:
+
+```sh
+pip install demogpt
+```
+
+### For the Source Code Version
+
+
 1. Clone the repository:
     ```sh
     git clone https://github.com/melih-unsal/DemoGPT.git
     ```
 2. Navigate into the project directory:
     ```sh
     cd DemoGPT
@@ -101,15 +131,25 @@
 3. Install the necessary dependencies: 
     ```sh
     pip install -r requirements.txt
     ```
 
 ## 🎮 Usage
 
-Once installed, you can use DemoGPT by running the following command:
+### For the Package Version
+
+Once the DemoGPT package is installed, you can use it by running the following command in your terminal:
+
+```sh
+demogpt
+```
+
+### For the Source Code Version
+
+If you have cloned the repository and wish to run the source code version, you can use DemoGPT by running the following command:
 
 ```sh
 streamlit run src/prompt_based/app.py
 ```
 
 ## 🤝 Contribute
```

#### html2text {}

```diff
@@ -1,61 +1,71 @@
 # ![favicon](assets/puzzle.png) DemoGPT: Auto Gen-AI App Generator with the
 Power of Llama 2
             [DemoGPT logo: Generate automatic LangChain pipelines]
      â¡ With just a prompt, you can create interactive Streamlit apps via
        ð¦ï¸ð LangChain's transformative capabilities & Llama 2.â¡
-             [Releases] [Official_Website] [DemoGPT_Documentation]
+       [Downloads] [Releases] [Official_Website] [DemoGPT_Documentation]
              [CN_doc] [EN_doc] [roadmap] [roadmap] [License:_MIT]
                [Open_an_issue] [Closed_issues] [DemoGPT__Stars]
                            [WeChat] [Twitter_Follow]
   [Streamlit_application] [https://img.shields.io/badge/%F0%9F%A4%97-Spaces-
                                     yellow]
+                        [Product_Hunt] [DemoGPT_Medium]
 ## â­ Star History [![Star History Chart](https://api.star-history.com/
 svg?repos=melih-unsal/DemoGPT&type=Timeline)](https://star-history.com/#melih-
 unsal/DemoGPT&Timeline) â­ Consider starring us if you're using DemoGPT so
 more people hear about us! ## ð¥ Demo For quick demo, you can visit [our
 website](https://demogpt.io) ![Humor Machine](assets/humor_machine.gif) https:/
 /github.com/melih-unsal/DemoGPT/assets/34304254/8991e296-b6fe-4817-bd08-
 4dab6d13020d ## ð Documentation See our documentation site [here](https://
 melih-unsal.github.io/DemoGPT-Docs/) for full how-to docs and guidelines â¡
-The new release with the power of **Llama 2** is within a week. â¡ ## ð
-Table of Contents - [Introduction](#-introduction) - [Pipeline](#%EF%B8%8F-
-pipeline) - [Installation](#-installation) - [Usage](#-usage) - [Contribute](#-
-contribute) - [License](#-license) ## ð Introduction Welcome to DemoGPT, a
-ground-breaking open-source initiative aimed at optimizing and democratizing
-the development of Large Language Model (LLM) based applications. At the heart
-of DemoGPT lies the potent GPT-3.5-turbo, which enables the auto-generation of
-LangChain code. This process is fueled by a unique self-refining strategy that
-seamlessly blends document understanding from the LangChain documentation tree
-with user prompts. The outcome is a piece of code that doesn't just work, but
-is inherently robust, adhering to best coding practices while maintaining a
-deep-rooted alignment with the LangChain library. The LangChain code, once
-generated, is not a final product but an intermediate stage. The code is
-further transformed into a user-friendly Streamlit application, adding an
-interactive layer to the logic produced. Alongside this, DemoGPT embraces an
-iterative development process, wherein each code segment is individually
-tested. This approach, coupled with the self-refining strategy, enables an
-efficient and error-minimized workflow, pushing the envelope in traditional
-code development. By making software development accessible through simple
-prompts, DemoGPT is laying the groundwork for a paradigm shift in how we
-create, refine, and customize LLM-based applications. The end goal is a
-broader, more inclusive ecosystem where users, regardless of their coding
-proficiency, can contribute to the continuous evolution of products. In
-summary, DemoGPT isn't just a project; it is a forward-thinking approach,
-redefining the boundaries of LLM-based application development. In the next
-release, we are gonna add **Llama 2** inside of DemoGPT to make the whole
-system runnable completely locally. ## âï¸ Architecture ### DemoGPT
-Architecture ![DemoGPT Architecture](assets/demogpt_new_pipeline1.jpeg?raw=true
-"DemoGPT Architecture") ## ð§ Installation 1. Clone the repository: ```sh git
-clone https://github.com/melih-unsal/DemoGPT.git ``` 2. Navigate into the
-project directory: ```sh cd DemoGPT ``` 3. Install the necessary dependencies:
-```sh pip install -r requirements.txt ``` ## ð® Usage Once installed, you can
-use DemoGPT by running the following command: ```sh streamlit run src/
-prompt_based/app.py ``` ## ð¤ Contribute Contributions to the DemoGPT project
-are welcomed! Whether you're fixing bugs, improving the documentation, or
-proposing new features, your efforts are highly appreciated. Please check the
-open issues before starting any work. > Please read [`CONTRIBUTING`]
-(CONTRIBUTING.md) for details on our [`CODE OF CONDUCT`](CODE_OF_CONDUCT.md),
-and the process for submitting pull requests to us. ## ð License DemoGPT is
-an open-source project licensed under [MIT License](LICENSE). --- For any
-issues, questions, or comments, please feel free to contact us or open an
-issue. We appreciate your feedback to make DemoGPT better.
+The new release with the power of **Llama 2** is within a week. â¡ ## ð¦
+Using DemoGPT Package The DemoGPT package is now available and can be installed
+using pip. Run the following command to install the package: ```sh pip install
+demogpt ``` To use the DemoGPT application, simply type "demogpt" into your
+terminal: ```sh demogpt ``` ## ð Table of Contents - [Introduction](#-
+introduction) - [Pipeline](#%EF%B8%8F-pipeline) - [Installation](#-
+installation) - [Usage](#-usage) - [Contribute](#-contribute) - [License](#-
+license) ## ð Introduction Welcome to DemoGPT, a ground-breaking open-source
+initiative aimed at optimizing and democratizing the development of Large
+Language Model (LLM) based applications. At the heart of DemoGPT lies the
+potent GPT-3.5-turbo, which enables the auto-generation of LangChain code. This
+process is fueled by a unique self-refining strategy that seamlessly blends
+document understanding from the LangChain documentation tree with user prompts.
+The outcome is a piece of code that doesn't just work, but is inherently
+robust, adhering to best coding practices while maintaining a deep-rooted
+alignment with the LangChain library. The LangChain code, once generated, is
+not a final product but an intermediate stage. The code is further transformed
+into a user-friendly Streamlit application, adding an interactive layer to the
+logic produced. Alongside this, DemoGPT embraces an iterative development
+process, wherein each code segment is individually tested. This approach,
+coupled with the self-refining strategy, enables an efficient and error-
+minimized workflow, pushing the envelope in traditional code development. By
+making software development accessible through simple prompts, DemoGPT is
+laying the groundwork for a paradigm shift in how we create, refine, and
+customize LLM-based applications. The end goal is a broader, more inclusive
+ecosystem where users, regardless of their coding proficiency, can contribute
+to the continuous evolution of products. In summary, DemoGPT isn't just a
+project; it is a forward-thinking approach, redefining the boundaries of LLM-
+based application development. In the next release, we are gonna add **Llama
+2** inside of DemoGPT to make the whole system runnable completely locally. ##
+âï¸ Architecture ### DemoGPT Architecture ![DemoGPT Architecture](assets/
+demogpt_new_pipeline1.jpeg?raw=true "DemoGPT Architecture") ## ð§
+Installation ### For the Package Version You can install the DemoGPT package by
+running the following command: ```sh pip install demogpt ``` ### For the Source
+Code Version 1. Clone the repository: ```sh git clone https://github.com/melih-
+unsal/DemoGPT.git ``` 2. Navigate into the project directory: ```sh cd DemoGPT
+``` 3. Install the necessary dependencies: ```sh pip install -
+r requirements.txt ``` ## ð® Usage ### For the Package Version Once the
+DemoGPT package is installed, you can use it by running the following command
+in your terminal: ```sh demogpt ``` ### For the Source Code Version If you have
+cloned the repository and wish to run the source code version, you can use
+DemoGPT by running the following command: ```sh streamlit run src/prompt_based/
+app.py ``` ## ð¤ Contribute Contributions to the DemoGPT project are
+welcomed! Whether you're fixing bugs, improving the documentation, or proposing
+new features, your efforts are highly appreciated. Please check the open issues
+before starting any work. > Please read [`CONTRIBUTING`](CONTRIBUTING.md) for
+details on our [`CODE OF CONDUCT`](CODE_OF_CONDUCT.md), and the process for
+submitting pull requests to us. ## ð License DemoGPT is an open-source
+project licensed under [MIT License](LICENSE). --- For any issues, questions,
+or comments, please feel free to contact us or open an issue. We appreciate
+your feedback to make DemoGPT better.
```

### Comparing `demogpt-1.1.1.7/src/alpha/app.py` & `demogpt-1.1.1.8/src/prompt_based/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,134 +2,140 @@
 import os
 import signal
 import webbrowser
 from time import sleep
 
 import streamlit as st
 
-import utils
-from langchain_coder import LangChainCoder
-
-# logging.basicConfig(level = logging.DEBUG,format='%(levelname)s-%(message)s')
+from model import LogicModel, StreamlitModel
 
 try:
     from dotenv import load_dotenv
 
     load_dotenv()
 except Exception as e:
     logging.error("dotenv import error but no needed")
 
-num_of_iterations = 10
 
+def main():
 
-def generate_response(txt, title):
-    """
-    Generate response using the LangChainCoder.
-
-    Args:
-        txt (str): The input text.
-
-    Yields:
-        dict: A dictionary containing response information.
-    """
-    for data in agent(txt, title, num_of_iterations):
-        yield data
-
-
-# Page title
-title = "🧩 DemoGPT"
-
-st.set_page_config(page_title=title)
-st.title(title)
-# Text input
-
-openai_api_key = st.sidebar.text_input(
-    "OpenAI API Key",
-    placeholder="sk-...",
-    value=os.getenv("OPENAI_API_KEY", ""),
-    type="password",
-)
-demo_title = st.text_input("Enter your demo title", placeholder="Type your demo title")
-empty_idea = st.empty()
-demo_idea = empty_idea.text_area(
-    "Enter your LLM-based demo idea", placeholder="Type your demo idea here", height=100
-)
-
-st.write("Examples")
-
-cols = st.columns([1, 1, 1.2])
-
-PROGRESS_BAR_INFO = {
-    "start": {"text": "Generating Code...", "percentage": 25},
-    "langchain": {"text": "Transforming to streamlit code", "percentage": 35},
-    "refining": {"text": "Refining Code...", "percentage": 50},
-    "streamlit": {"text": "Creating App...", "percentage": 75},
-    "failed": {"text": "Failed", "percentage": 100},
-}
-
-
-def progressBar(key, bar=None):
-    info = PROGRESS_BAR_INFO[key]
-    if bar:
-        bar.progress(info["percentage"], text=info["text"])
-    else:
-        return st.progress(info["percentage"], text=info["text"])
-
-
-examples = [
-    "Language Translator 📝",
-    "Grammer Corrector 🛠",
-    "Blog post generator from title 📔",
-]
-
-if "pid" not in st.session_state:
-    st.session_state["pid"] = -1
-
-example_submitted = False
-
-with st.form("a", clear_on_submit=True):
-    submitted = st.form_submit_button("Submit")
-    for col, example in zip(cols, examples):
-        if col.button(example):
-            example_submitted = True
-            demo_idea = empty_idea.text_area(
-                "Enter your LLM-based demo idea", example, height=100
-            )
-            logging.info(f"Demo Idea:{demo_idea}")
-
-    if submitted or example_submitted:
-
-        if not openai_api_key.startswith("sk-"):
-            st.warning("Please enter your OpenAI API Key!", icon="⚠️")
-        else:
-            bar = progressBar("start")
-
-            agent = LangChainCoder(openai_api_key=openai_api_key)
-
-            if st.session_state["pid"] != -1:
-                logging.info(f"Terminating the previous applicaton ...")
-                os.kill(st.session_state["pid"], signal.SIGTERM)
-                st.session_state["pid"] = -1
-
-            code_empty = st.empty()
-            for data in generate_response(demo_idea, demo_title):
-                code = data["code"]
-                success = data["success"]
-                task_id = data["task_id"]
-                stage = data["stage"]
-
-                if success:
-                    progressBar(stage, bar)
-                    if stage == "streamlit" and task_id == "final":
-                        with st.expander("Code"):
-                            st.code(code)
+    num_of_iterations = 10
+
+    def generate_response(txt):
+        """
+        Generate response using the LogicModel.
+
+        Args:
+            txt (str): The input text.
+
+        Yields:
+            dict: A dictionary containing response information.
+        """
+        for data in agent(txt, num_of_iterations):
+            yield data
+
+    # Page title
+    title = "🧩 DemoGPT"
+
+    st.set_page_config(page_title=title)
+    st.title(title)
+    # Text input
+
+    openai_api_key = st.sidebar.text_input(
+        "OpenAI API Key",
+        placeholder="sk-...",
+        value=os.getenv("OPENAI_API_KEY", ""),
+        type="password",
+    )
+    demo_title = st.text_input(
+        "Enter your demo title", placeholder="Type your demo title"
+    )
+    empty_idea = st.empty()
+    demo_idea = empty_idea.text_area(
+        "Enter your LLM-based demo idea",
+        placeholder="Type your demo idea here",
+        height=100,
+    )
+
+    st.write("Examples")
+
+    cols = st.columns([1, 1, 1.2])
+
+    PROGRESS_BAR_TEXTS = {
+        "start": "Generating Code...",
+        "creating": "Creating App...",
+        "refining": "Refining Code...",
+        "failed": "Failed",
+    }
+
+    examples = [
+        "Language Translator 📝",
+        "Grammer Corrector 🛠",
+        "Blog post generator from title 📔",
+    ]
+
+    if "pid" not in st.session_state:
+        st.session_state["pid"] = -1
+
+    example_submitted = False
+
+    final_code_empty = st.empty()
+
+    with st.form("a", clear_on_submit=True):
+        submitted = st.form_submit_button("Submit")
+        for col, example in zip(cols, examples):
+            if col.button(example):
+                example_submitted = True
+                demo_idea = empty_idea.text_area(
+                    "Enter your LLM-based demo idea", example, height=100
+                )
+                logging.info(f"Demo Idea:{demo_idea}")
+
+        if submitted or example_submitted:
+
+            if not openai_api_key.startswith("sk-"):
+                st.warning("Please enter your OpenAI API Key!", icon="⚠️")
+            else:
+                agent = LogicModel(openai_api_key=openai_api_key)
+                streamlit_agent = StreamlitModel(openai_api_key=openai_api_key)
+
+                if st.session_state["pid"] != -1:
+                    logging.info(f"Terminating the previous applicaton ...")
+                    os.kill(st.session_state["pid"], signal.SIGTERM)
+                    st.session_state["pid"] = -1
+
+                bar = st.progress(25, PROGRESS_BAR_TEXTS["start"])
+                for data in generate_response(demo_idea):
+                    response = data["out"]
+                    error = data["error"]
+                    code = data["code"]
+                    test_code = data["test_code"]
+                    success = data["success"]
+                    percentage = data["percentage"]
+
+                    if success:
+                        bar.progress(75, text=PROGRESS_BAR_TEXTS["creating"])
                         example_submitted = False
-                        st.session_state["pid"] = utils.runStreamlit(
-                            code, openai_api_key
+                        st.session_state["pid"], streamlit_code = streamlit_agent(
+                            demo_idea,
+                            demo_title,
+                            code,
+                            test_code,
+                            bar.progress,
+                            st.balloons,
                         )
+                        with st.expander("Code"):
+                            st.code(streamlit_code)
                         sleep(5)
                         webbrowser.open("http://localhost:8502")
+
+                    else:
+                        bar.progress(50, text=PROGRESS_BAR_TEXTS["refining"])
+
+                    if success:
                         break
                 else:
-                    progressBar("refining")
-            else:
-                progressBar("failed")
+                    bar.progress(100, text=PROGRESS_BAR_TEXTS["failed"])
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `demogpt-1.1.1.7/src/prompt_based/model.py` & `demogpt-1.1.1.8/src/prompt_based/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 import os
 import platform
 import shutil
 import subprocess
 import sys
 import tempfile
 import threading
+import unicodedata
 from subprocess import PIPE
 from threading import Timer
 
+from prompts import *
+
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
 
-from prompt_based.prompts import *
 from pkg_resources import resource_stream
 
 
 class BaseModel:
     """
     Base class for the LogicModel and StreamlitModel classes.
 
@@ -50,14 +52,29 @@
         """
         if "```" in code:
             code = code.split("```")[1]
             if code.startswith("python"):
                 code = code[len("python") :].strip()
         return code
 
+    def normalize(self, code):
+        """Fix Unicode related problems
+
+        Args:
+            code (str): The code to be refined.
+
+        Returns:
+            str: refined version of the code
+        """
+        return (
+            unicodedata.normalize("NFKD", code)
+            .encode("ascii", "ignore")
+            .decode("utf-8")
+        )
+
 
 class LogicModel(BaseModel):
     """
     Represents the logic model for generating Python code.
 
     Methods:
         - __init__(self, openai_api_key: str):
@@ -93,16 +110,20 @@
 
     def addDocuments(self):
         """
         Adds documents to the logic model for generating Python code.
         """
         self.document = ""
         for path in ["prompts.txt"]:
-            with resource_stream('prompt_based', path) as f:
-                self.document += f.read().decode('utf-8')
+            try:
+                with resource_stream("prompt_based", path) as f:
+                    self.document += f.read().decode("utf-8")
+            except ImportError:
+                with open(f"src/prompt_based/{path}", "r") as f:
+                    self.document += f.read()
 
     def decode_results(self, results):
         """
         Decodes the results returned by the executed python code
 
         Args:
             results: The results to be decoded.
@@ -118,16 +139,19 @@
 
         Args:
             code (str): The Python code to be executed.
 
         Returns:
             Tuple[str, str, bool]: The output, error, and success status of the execution.
         """
-        tmp = tempfile.NamedTemporaryFile("w", suffix=".py", delete=False, encoding='utf-8')
-        tmp.write(code)
+
+        tmp = tempfile.NamedTemporaryFile(
+            "w", suffix=".py", delete=False, encoding="utf-8"
+        )
+        tmp.write(self.normalize(code))
         tmp.flush()
         environmental_variables = {"OPENAI_API_KEY": self.openai_api_key}
         python_path = shutil.which("python")
         if platform.system() == "Windows":
             env = os.environ.copy()
             env["PYTHONPATH"] = ""
             env["OPENAI_API_KEY"] = self.openai_api_key
@@ -254,16 +278,18 @@
 
         Args:
             code (str): The code of the Streamlit application.
 
         Returns:
             int: The process ID of the Streamlit application.
         """
-        tmp = tempfile.NamedTemporaryFile("w", suffix=".py", delete=False,encoding='utf-8')
-        tmp.write(code)
+        tmp = tempfile.NamedTemporaryFile(
+            "w", suffix=".py", delete=False, encoding="utf-8"
+        )
+        tmp.write(self.normalize(code))
         tmp.flush()
         environmental_variables = {
             "OPENAI_API_KEY": self.openai_api_key,
             "STREAMLIT_SERVER_PORT": "8502",
         }
         streamlit_path = shutil.which("streamlit")
         if platform.system() == "Windows":
```

### Comparing `demogpt-1.1.1.7/src/prompt_based/prompts.py` & `demogpt-1.1.1.8/src/prompt_based/prompts.py`

 * *Files identical despite different names*

### Comparing `demogpt-1.1.1.7/src/prompt_based/prompts.txt` & `demogpt-1.1.1.8/src/prompt_based/prompts.txt`

 * *Files identical despite different names*

