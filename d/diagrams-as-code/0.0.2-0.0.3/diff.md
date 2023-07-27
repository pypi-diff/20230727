# Comparing `tmp/diagrams-as-code-0.0.2.tar.gz` & `tmp/diagrams-as-code-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagrams-as-code-0.0.2.tar", last modified: Thu Jul 27 18:02:11 2023, max compression
+gzip compressed data, was "diagrams-as-code-0.0.3.tar", last modified: Thu Jul 27 18:11:55 2023, max compression
```

## Comparing `diagrams-as-code-0.0.2.tar` & `diagrams-as-code-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:02:11.391606 diagrams-as-code-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/.project-version
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-07-27 18:02:11.391606 diagrams-as-code-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20791 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:02:11.387606 diagrams-as-code-0.0.2/diagrams_as_code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/diagrams_as_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/diagrams_as_code/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/diagrams_as_code/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/diagrams_as_code/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/diagrams_as_code/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:02:11.391606 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 18:02:11.000000 diagrams-as-code-0.0.2/diagrams_as_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:02:11.391606 diagrams-as-code-0.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/requirements/project.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 18:02:11.391606 diagrams-as-code-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-27 18:01:47.000000 diagrams-as-code-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:11:55.912076 diagrams-as-code-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/.project-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21703 2023-07-27 18:11:55.912076 diagrams-as-code-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20812 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:11:55.912076 diagrams-as-code-0.0.3/diagrams_as_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/diagrams_as_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/diagrams_as_code/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/diagrams_as_code/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/diagrams_as_code/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/diagrams_as_code/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:11:55.912076 diagrams-as-code-0.0.3/diagrams_as_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21703 2023-07-27 18:11:55.000000 diagrams-as-code-0.0.3/diagrams_as_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-27 18:11:55.000000 diagrams-as-code-0.0.3/diagrams_as_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:11:55.000000 diagrams-as-code-0.0.3/diagrams_as_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-27 18:11:55.000000 diagrams-as-code-0.0.3/diagrams_as_code.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 18:11:55.000000 diagrams-as-code-0.0.3/diagrams_as_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 18:11:55.000000 diagrams-as-code-0.0.3/diagrams_as_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:11:55.912076 diagrams-as-code-0.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/requirements/project.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-27 18:11:55.912076 diagrams-as-code-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-27 18:11:31.000000 diagrams-as-code-0.0.3/setup.py
```

### Comparing `diagrams-as-code-0.0.2/LICENSE` & `diagrams-as-code-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `diagrams-as-code-0.0.2/PKG-INFO` & `diagrams-as-code-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagrams-as-code
-Version: 0.0.2
+Version: 0.0.3
 Summary: Diagrams as code: declarative configurations using YAML for drawing cloud system architectures.
 Home-page: https://github.com/dmytrostriletskyi/diagrams-as-code
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dmytrostriletskyi/diagrams-as-code/issues
 Project-URL: Source Code, https://github.com/dmytrostriletskyi/diagrams-as-code
@@ -50,19 +50,19 @@
 on specific web services such as [draw.io](https://app.diagrams.net). It lets you generate the cloud system architecture
 in a **declarative** way with widely used `YAML` syntax (which is de facto a standard for infrastructure and 
 configurations).
 
 Declarative method of describing things means that a user simply describes the solution they need, how it should look, 
 and everything that would be in the state of the final solution, leaving the process for the software to decide.
 
-`Diagrams as code` brings you the following benefits comparing to drawing architecture on your own, it:
+`Diagrams as code` brings you the following benefits compared to drawing architecture on your own, it:
 
 * Does not require any knowledge about how to properly draw an architecture diagram. Basically, you just define a set of 
   resources, compose them into groups and set relationships, the rest is done for you.
-* Allows you to track an architecture diagram changes with a version control systems such as `Git`.
+* Allows you to track architecture diagram changes with a version control systems such as `Git`.
 * Moves collaboration to the next level: updating an architecture diagram through a pull request with a code review 
   instead of a video session and/or screen sharing.
 * Reduces costs on further updating of an initial architecture diagram. Basically, when you create an image on a web 
   service you have to eventually store two files: `PNG`-like to put into your documentation and `XML` to be able to 
   adjust your image in the future. So, there is no need to care about `XML` anymore.
 * Backups you in case of losing `XML` files as `YAML` files are always stored in a repository.
 * Improves consistency as now a diagram is stored along the code in a repository, the place you visit and work on
@@ -116,15 +116,15 @@
 
 When you will be writing your own `YAML` files, you likely need a syntax highlighting. Currently, there is no mapping
 of the `YAML` files to a specific schema to enable the syntax highlighting automatically. So, there is a need for
 manual operation here.
 
 #### PyCharm
 
-For `PyCharm`, open the settings and proceed to `Languages & Framworks`, then to `Scheams and DTDs`, then to
+For `PyCharm`, open the settings and proceed to `Languages & Frameworks, then to `Scheams and DTDs`, then to
 `JSON Schema Mappings`. After, create a new schema, name it `Diagrams as code`, choose
 `JSON Schema version 7`, paste `https://raw.githubusercontent.com/dmytrostriletskyi/diagrams-as-code/main/json-schemas/0.0.1.json`
 to the `Schema file or URL` field and click `Apply`:
 
 <details>
   <summary>Open Illustration</summary>
 
@@ -135,23 +135,23 @@
 
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/down-panel-json-schema.png)
 </details>
 
-It will open a panel where you can choose the newly created schema with name `Diagrams as code`:
+It will open a panel where you can choose the newly created schema with the name `Diagrams as code`:
 
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/panel-json-schema.png)
 </details>
 
-As the result, you will experience the syntax highlighting when typing:
+As a result, you will experience syntax highlighting when typing:
 
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/syntax-highlight.png)
 </details>
 
@@ -165,17 +165,17 @@
 ```bash
 $ diagrams-as-code examples/web-services-aws.yaml
 ```
 
 ### Guide
 
 Please, check [all-fields.yaml](./examples/all-fields.yaml) as the example to see all possible configurations
-before diving into detailed explanation about them (and [this](./assets/all-fields.jpg) is the result image).
+before diving into a detailed explanation about them (and [this](./assets/all-fields.jpg) is the result image).
 
-A `YAML` file conceptually contains two configurations: generic information such as name of a diagram, format of an 
+A `YAML` file conceptually contains two configurations: generic information such as a name of a diagram, a format of an 
 image to be generated, style and resources themselves such as `AWS` and `Kubernetes` resources, `Nginx`, `ElasticSearch`
 and all other things you actually want to draw, and relationships among them.
 
 ```yaml
 diagram:
   name: Web Services Architecture on AWS
   file_name: web-services-architecture-aws
@@ -190,15 +190,15 @@
       color: '#000000'
   label_resources: false
   open: true
   resource:
     ...
 ```
 
-Generic information schema looks like:
+Generic information schema looks like this:
 
 | Field             | Type    | Required | Restrictions                                                        | Default         | Description                                                            |
 |-------------------|---------|----------|---------------------------------------------------------------------|-----------------|------------------------------------------------------------------------|
 | `name`            | String  | Yes      | -                                                                   | `PNG`           | A name of the diagram which is shown in the image.                     |
 | `file_name`       | String  | No       | -                                                                   | -               | A file name of the image that would be created.                        |
 | `format`          | String  | No       | `png`, `jpg`, `svg`, `pdf`, `dot`                                   | `png`           | A format of the image that would be created.                           |
 | `direction`       | String  | No       | `left-to-right`, `right-to-left`, `top-to-bottom`, `bottom-to-top`  | `left-to-right` | A direction of the diagram's resource.                                 |
@@ -254,15 +254,15 @@
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/guide-resource-relationship.png)
 </details>
 
 There is also a type named `group`. It is not a specific resource, it is rather a group **of** resources. It is needed
-for other resource to be able to have a relationship to all group's resources at once. Each group's resource can can
+for other resources to be able to have a relationship with all group's resources at once. Each group's resource can have
 separate relationships as well:
 
 ```yaml
 diagram:
   resources:
     - id: elb
       name: ELB
@@ -292,15 +292,15 @@
 </details>
 
 There is also a type named `cluster`. It is needed to separate multiple resources or groups logically: for instance,
 there might be a cluster of different APIs composed as groups, a cluster of databases and a cluster of caches.
 
 > Pay attention that to refer a cluster resource, there are the following identifiers `web-services.graphql-api` and 
 > `web-services.rest-api` what means that you need to chain identifiers of nested resources through a dot to identify a 
-> resource you build a relationship to.
+> resource you build a relationship with.
 
 ```yaml
 diagram:
   resources:
     - id: elb
       name: ELB
       type: aws.network.ELB
@@ -363,15 +363,15 @@
 Basically, to recap and also clarify:
 
 * There are resources, groups (of resources or other groups) and clusters (of resources, groups or other clusters).
 * You can build a relationship between resource to resource and resource to group (and vice versa), it is impossible to
   relate to a cluster.
 * You should chain identifiers of nested resources through a dot to identify a resource you build a relationship to.
 
-`resources` schema looks like:
+`resources` schema looks like this:
 
 | Field     | Type   | Required | Restrictions                                                                                        | Default | Description                              |
 |-----------|--------|----------|-----------------------------------------------------------------------------------------------------|---------|------------------------------------------|
 | `id`      | String | Yes      | -                                                                                                   | -       | A unique identifier of the resource.     |
 | `name`    | String | Yes      | -                                                                                                   | -       | A name of the resource.                  |
 | `type`    | String | Yes      | One of the [those](https://github.com/dmytrostriletskyi/diagrams-as-code/tree/main/docs/resources). | -       | A type of the resource.                  |
 | `relates` | Object | No       | -                                                                                                   | -       | A relationship to a resource or a group. |
@@ -406,15 +406,15 @@
 | `direction` | String | Yes      | `incoming`, `outgoing`, `bidirectional`, `undirected` | -         | A direction of a relationship.                            |
 | `label`     | String | No       | -                                                     | -         | A label of a relationship.                                |
 | `color`     | String | No       | `Hexadecimal color` with the `#` symbol.              | `#2D3436` | A color of a relationship.                                |
 | `style`     | String | No       | -                                                     | -         | A style of a relationship.                                |
 
 ## Disclaimer
 
-`diagrams-as-code` is a wrapper around original [diagrams](https://github.com/mingrammer/diagrams). The original `diagrams` 
+`diagrams-as-code` is a wrapper around the original [diagrams](https://github.com/mingrammer/diagrams). The original `diagrams` 
 lets you draw the cloud system architecture in `Python` code. It was born for prototyping a new system architecture 
-design without any design tools. Under the hood, `diagrams-as-code` parse a `YAML` file and map to specific set of 
-`diagrams`'s functions and classes, and executes them in proper order.
+design without any design tools. Under the hood, `diagrams-as-code` parse a `YAML` file and map to a specific set of 
+`diagrams`'s functions and classes, and execute them in proper order.
 
 But you don't have to worry about `diagrams` because `diagrams-as-code` is self-contained and encapsulates it well.
```

### Comparing `diagrams-as-code-0.0.2/README.md` & `diagrams-as-code-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 on specific web services such as [draw.io](https://app.diagrams.net). It lets you generate the cloud system architecture
 in a **declarative** way with widely used `YAML` syntax (which is de facto a standard for infrastructure and 
 configurations).
 
 Declarative method of describing things means that a user simply describes the solution they need, how it should look, 
 and everything that would be in the state of the final solution, leaving the process for the software to decide.
 
-`Diagrams as code` brings you the following benefits comparing to drawing architecture on your own, it:
+`Diagrams as code` brings you the following benefits compared to drawing architecture on your own, it:
 
 * Does not require any knowledge about how to properly draw an architecture diagram. Basically, you just define a set of 
   resources, compose them into groups and set relationships, the rest is done for you.
-* Allows you to track an architecture diagram changes with a version control systems such as `Git`.
+* Allows you to track architecture diagram changes with a version control systems such as `Git`.
 * Moves collaboration to the next level: updating an architecture diagram through a pull request with a code review 
   instead of a video session and/or screen sharing.
 * Reduces costs on further updating of an initial architecture diagram. Basically, when you create an image on a web 
   service you have to eventually store two files: `PNG`-like to put into your documentation and `XML` to be able to 
   adjust your image in the future. So, there is no need to care about `XML` anymore.
 * Backups you in case of losing `XML` files as `YAML` files are always stored in a repository.
 * Improves consistency as now a diagram is stored along the code in a repository, the place you visit and work on
@@ -96,15 +96,15 @@
 
 When you will be writing your own `YAML` files, you likely need a syntax highlighting. Currently, there is no mapping
 of the `YAML` files to a specific schema to enable the syntax highlighting automatically. So, there is a need for
 manual operation here.
 
 #### PyCharm
 
-For `PyCharm`, open the settings and proceed to `Languages & Framworks`, then to `Scheams and DTDs`, then to
+For `PyCharm`, open the settings and proceed to `Languages & Frameworks, then to `Scheams and DTDs`, then to
 `JSON Schema Mappings`. After, create a new schema, name it `Diagrams as code`, choose
 `JSON Schema version 7`, paste `https://raw.githubusercontent.com/dmytrostriletskyi/diagrams-as-code/main/json-schemas/0.0.1.json`
 to the `Schema file or URL` field and click `Apply`:
 
 <details>
   <summary>Open Illustration</summary>
 
@@ -115,23 +115,23 @@
 
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/down-panel-json-schema.png)
 </details>
 
-It will open a panel where you can choose the newly created schema with name `Diagrams as code`:
+It will open a panel where you can choose the newly created schema with the name `Diagrams as code`:
 
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/panel-json-schema.png)
 </details>
 
-As the result, you will experience the syntax highlighting when typing:
+As a result, you will experience syntax highlighting when typing:
 
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/syntax-highlight.png)
 </details>
 
@@ -145,17 +145,17 @@
 ```bash
 $ diagrams-as-code examples/web-services-aws.yaml
 ```
 
 ### Guide
 
 Please, check [all-fields.yaml](./examples/all-fields.yaml) as the example to see all possible configurations
-before diving into detailed explanation about them (and [this](./assets/all-fields.jpg) is the result image).
+before diving into a detailed explanation about them (and [this](./assets/all-fields.jpg) is the result image).
 
-A `YAML` file conceptually contains two configurations: generic information such as name of a diagram, format of an 
+A `YAML` file conceptually contains two configurations: generic information such as a name of a diagram, a format of an 
 image to be generated, style and resources themselves such as `AWS` and `Kubernetes` resources, `Nginx`, `ElasticSearch`
 and all other things you actually want to draw, and relationships among them.
 
 ```yaml
 diagram:
   name: Web Services Architecture on AWS
   file_name: web-services-architecture-aws
@@ -170,15 +170,15 @@
       color: '#000000'
   label_resources: false
   open: true
   resource:
     ...
 ```
 
-Generic information schema looks like:
+Generic information schema looks like this:
 
 | Field             | Type    | Required | Restrictions                                                        | Default         | Description                                                            |
 |-------------------|---------|----------|---------------------------------------------------------------------|-----------------|------------------------------------------------------------------------|
 | `name`            | String  | Yes      | -                                                                   | `PNG`           | A name of the diagram which is shown in the image.                     |
 | `file_name`       | String  | No       | -                                                                   | -               | A file name of the image that would be created.                        |
 | `format`          | String  | No       | `png`, `jpg`, `svg`, `pdf`, `dot`                                   | `png`           | A format of the image that would be created.                           |
 | `direction`       | String  | No       | `left-to-right`, `right-to-left`, `top-to-bottom`, `bottom-to-top`  | `left-to-right` | A direction of the diagram's resource.                                 |
@@ -234,15 +234,15 @@
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/guide-resource-relationship.png)
 </details>
 
 There is also a type named `group`. It is not a specific resource, it is rather a group **of** resources. It is needed
-for other resource to be able to have a relationship to all group's resources at once. Each group's resource can can
+for other resources to be able to have a relationship with all group's resources at once. Each group's resource can have
 separate relationships as well:
 
 ```yaml
 diagram:
   resources:
     - id: elb
       name: ELB
@@ -272,15 +272,15 @@
 </details>
 
 There is also a type named `cluster`. It is needed to separate multiple resources or groups logically: for instance,
 there might be a cluster of different APIs composed as groups, a cluster of databases and a cluster of caches.
 
 > Pay attention that to refer a cluster resource, there are the following identifiers `web-services.graphql-api` and 
 > `web-services.rest-api` what means that you need to chain identifiers of nested resources through a dot to identify a 
-> resource you build a relationship to.
+> resource you build a relationship with.
 
 ```yaml
 diagram:
   resources:
     - id: elb
       name: ELB
       type: aws.network.ELB
@@ -343,15 +343,15 @@
 Basically, to recap and also clarify:
 
 * There are resources, groups (of resources or other groups) and clusters (of resources, groups or other clusters).
 * You can build a relationship between resource to resource and resource to group (and vice versa), it is impossible to
   relate to a cluster.
 * You should chain identifiers of nested resources through a dot to identify a resource you build a relationship to.
 
-`resources` schema looks like:
+`resources` schema looks like this:
 
 | Field     | Type   | Required | Restrictions                                                                                        | Default | Description                              |
 |-----------|--------|----------|-----------------------------------------------------------------------------------------------------|---------|------------------------------------------|
 | `id`      | String | Yes      | -                                                                                                   | -       | A unique identifier of the resource.     |
 | `name`    | String | Yes      | -                                                                                                   | -       | A name of the resource.                  |
 | `type`    | String | Yes      | One of the [those](https://github.com/dmytrostriletskyi/diagrams-as-code/tree/main/docs/resources). | -       | A type of the resource.                  |
 | `relates` | Object | No       | -                                                                                                   | -       | A relationship to a resource or a group. |
@@ -386,13 +386,13 @@
 | `direction` | String | Yes      | `incoming`, `outgoing`, `bidirectional`, `undirected` | -         | A direction of a relationship.                            |
 | `label`     | String | No       | -                                                     | -         | A label of a relationship.                                |
 | `color`     | String | No       | `Hexadecimal color` with the `#` symbol.              | `#2D3436` | A color of a relationship.                                |
 | `style`     | String | No       | -                                                     | -         | A style of a relationship.                                |
 
 ## Disclaimer
 
-`diagrams-as-code` is a wrapper around original [diagrams](https://github.com/mingrammer/diagrams). The original `diagrams` 
+`diagrams-as-code` is a wrapper around the original [diagrams](https://github.com/mingrammer/diagrams). The original `diagrams` 
 lets you draw the cloud system architecture in `Python` code. It was born for prototyping a new system architecture 
-design without any design tools. Under the hood, `diagrams-as-code` parse a `YAML` file and map to specific set of 
-`diagrams`'s functions and classes, and executes them in proper order.
+design without any design tools. Under the hood, `diagrams-as-code` parse a `YAML` file and map to a specific set of 
+`diagrams`'s functions and classes, and execute them in proper order.
 
 But you don't have to worry about `diagrams` because `diagrams-as-code` is self-contained and encapsulates it well.
```

### Comparing `diagrams-as-code-0.0.2/diagrams_as_code/entrypoint.py` & `diagrams-as-code-0.0.3/diagrams_as_code/entrypoint.py`

 * *Files identical despite different names*

### Comparing `diagrams-as-code-0.0.2/diagrams_as_code/enums.py` & `diagrams-as-code-0.0.3/diagrams_as_code/enums.py`

 * *Files identical despite different names*

### Comparing `diagrams-as-code-0.0.2/diagrams_as_code/resources.py` & `diagrams-as-code-0.0.3/diagrams_as_code/resources.py`

 * *Files identical despite different names*

### Comparing `diagrams-as-code-0.0.2/diagrams_as_code/schema.py` & `diagrams-as-code-0.0.3/diagrams_as_code/schema.py`

 * *Files identical despite different names*

### Comparing `diagrams-as-code-0.0.2/diagrams_as_code.egg-info/PKG-INFO` & `diagrams-as-code-0.0.3/diagrams_as_code.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagrams-as-code
-Version: 0.0.2
+Version: 0.0.3
 Summary: Diagrams as code: declarative configurations using YAML for drawing cloud system architectures.
 Home-page: https://github.com/dmytrostriletskyi/diagrams-as-code
 Author: Dmytro Striletskyi
 Author-email: dmytro.striletskyi@gmail.com
 License: MIT
 Project-URL: Issue Tracker, https://github.com/dmytrostriletskyi/diagrams-as-code/issues
 Project-URL: Source Code, https://github.com/dmytrostriletskyi/diagrams-as-code
@@ -50,19 +50,19 @@
 on specific web services such as [draw.io](https://app.diagrams.net). It lets you generate the cloud system architecture
 in a **declarative** way with widely used `YAML` syntax (which is de facto a standard for infrastructure and 
 configurations).
 
 Declarative method of describing things means that a user simply describes the solution they need, how it should look, 
 and everything that would be in the state of the final solution, leaving the process for the software to decide.
 
-`Diagrams as code` brings you the following benefits comparing to drawing architecture on your own, it:
+`Diagrams as code` brings you the following benefits compared to drawing architecture on your own, it:
 
 * Does not require any knowledge about how to properly draw an architecture diagram. Basically, you just define a set of 
   resources, compose them into groups and set relationships, the rest is done for you.
-* Allows you to track an architecture diagram changes with a version control systems such as `Git`.
+* Allows you to track architecture diagram changes with a version control systems such as `Git`.
 * Moves collaboration to the next level: updating an architecture diagram through a pull request with a code review 
   instead of a video session and/or screen sharing.
 * Reduces costs on further updating of an initial architecture diagram. Basically, when you create an image on a web 
   service you have to eventually store two files: `PNG`-like to put into your documentation and `XML` to be able to 
   adjust your image in the future. So, there is no need to care about `XML` anymore.
 * Backups you in case of losing `XML` files as `YAML` files are always stored in a repository.
 * Improves consistency as now a diagram is stored along the code in a repository, the place you visit and work on
@@ -116,15 +116,15 @@
 
 When you will be writing your own `YAML` files, you likely need a syntax highlighting. Currently, there is no mapping
 of the `YAML` files to a specific schema to enable the syntax highlighting automatically. So, there is a need for
 manual operation here.
 
 #### PyCharm
 
-For `PyCharm`, open the settings and proceed to `Languages & Framworks`, then to `Scheams and DTDs`, then to
+For `PyCharm`, open the settings and proceed to `Languages & Frameworks, then to `Scheams and DTDs`, then to
 `JSON Schema Mappings`. After, create a new schema, name it `Diagrams as code`, choose
 `JSON Schema version 7`, paste `https://raw.githubusercontent.com/dmytrostriletskyi/diagrams-as-code/main/json-schemas/0.0.1.json`
 to the `Schema file or URL` field and click `Apply`:
 
 <details>
   <summary>Open Illustration</summary>
 
@@ -135,23 +135,23 @@
 
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/down-panel-json-schema.png)
 </details>
 
-It will open a panel where you can choose the newly created schema with name `Diagrams as code`:
+It will open a panel where you can choose the newly created schema with the name `Diagrams as code`:
 
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/panel-json-schema.png)
 </details>
 
-As the result, you will experience the syntax highlighting when typing:
+As a result, you will experience syntax highlighting when typing:
 
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/syntax-highlight.png)
 </details>
 
@@ -165,17 +165,17 @@
 ```bash
 $ diagrams-as-code examples/web-services-aws.yaml
 ```
 
 ### Guide
 
 Please, check [all-fields.yaml](./examples/all-fields.yaml) as the example to see all possible configurations
-before diving into detailed explanation about them (and [this](./assets/all-fields.jpg) is the result image).
+before diving into a detailed explanation about them (and [this](./assets/all-fields.jpg) is the result image).
 
-A `YAML` file conceptually contains two configurations: generic information such as name of a diagram, format of an 
+A `YAML` file conceptually contains two configurations: generic information such as a name of a diagram, a format of an 
 image to be generated, style and resources themselves such as `AWS` and `Kubernetes` resources, `Nginx`, `ElasticSearch`
 and all other things you actually want to draw, and relationships among them.
 
 ```yaml
 diagram:
   name: Web Services Architecture on AWS
   file_name: web-services-architecture-aws
@@ -190,15 +190,15 @@
       color: '#000000'
   label_resources: false
   open: true
   resource:
     ...
 ```
 
-Generic information schema looks like:
+Generic information schema looks like this:
 
 | Field             | Type    | Required | Restrictions                                                        | Default         | Description                                                            |
 |-------------------|---------|----------|---------------------------------------------------------------------|-----------------|------------------------------------------------------------------------|
 | `name`            | String  | Yes      | -                                                                   | `PNG`           | A name of the diagram which is shown in the image.                     |
 | `file_name`       | String  | No       | -                                                                   | -               | A file name of the image that would be created.                        |
 | `format`          | String  | No       | `png`, `jpg`, `svg`, `pdf`, `dot`                                   | `png`           | A format of the image that would be created.                           |
 | `direction`       | String  | No       | `left-to-right`, `right-to-left`, `top-to-bottom`, `bottom-to-top`  | `left-to-right` | A direction of the diagram's resource.                                 |
@@ -254,15 +254,15 @@
 <details>
   <summary>Open Illustration</summary>
 
   ![](./assets/guide-resource-relationship.png)
 </details>
 
 There is also a type named `group`. It is not a specific resource, it is rather a group **of** resources. It is needed
-for other resource to be able to have a relationship to all group's resources at once. Each group's resource can can
+for other resources to be able to have a relationship with all group's resources at once. Each group's resource can have
 separate relationships as well:
 
 ```yaml
 diagram:
   resources:
     - id: elb
       name: ELB
@@ -292,15 +292,15 @@
 </details>
 
 There is also a type named `cluster`. It is needed to separate multiple resources or groups logically: for instance,
 there might be a cluster of different APIs composed as groups, a cluster of databases and a cluster of caches.
 
 > Pay attention that to refer a cluster resource, there are the following identifiers `web-services.graphql-api` and 
 > `web-services.rest-api` what means that you need to chain identifiers of nested resources through a dot to identify a 
-> resource you build a relationship to.
+> resource you build a relationship with.
 
 ```yaml
 diagram:
   resources:
     - id: elb
       name: ELB
       type: aws.network.ELB
@@ -363,15 +363,15 @@
 Basically, to recap and also clarify:
 
 * There are resources, groups (of resources or other groups) and clusters (of resources, groups or other clusters).
 * You can build a relationship between resource to resource and resource to group (and vice versa), it is impossible to
   relate to a cluster.
 * You should chain identifiers of nested resources through a dot to identify a resource you build a relationship to.
 
-`resources` schema looks like:
+`resources` schema looks like this:
 
 | Field     | Type   | Required | Restrictions                                                                                        | Default | Description                              |
 |-----------|--------|----------|-----------------------------------------------------------------------------------------------------|---------|------------------------------------------|
 | `id`      | String | Yes      | -                                                                                                   | -       | A unique identifier of the resource.     |
 | `name`    | String | Yes      | -                                                                                                   | -       | A name of the resource.                  |
 | `type`    | String | Yes      | One of the [those](https://github.com/dmytrostriletskyi/diagrams-as-code/tree/main/docs/resources). | -       | A type of the resource.                  |
 | `relates` | Object | No       | -                                                                                                   | -       | A relationship to a resource or a group. |
@@ -406,15 +406,15 @@
 | `direction` | String | Yes      | `incoming`, `outgoing`, `bidirectional`, `undirected` | -         | A direction of a relationship.                            |
 | `label`     | String | No       | -                                                     | -         | A label of a relationship.                                |
 | `color`     | String | No       | `Hexadecimal color` with the `#` symbol.              | `#2D3436` | A color of a relationship.                                |
 | `style`     | String | No       | -                                                     | -         | A style of a relationship.                                |
 
 ## Disclaimer
 
-`diagrams-as-code` is a wrapper around original [diagrams](https://github.com/mingrammer/diagrams). The original `diagrams` 
+`diagrams-as-code` is a wrapper around the original [diagrams](https://github.com/mingrammer/diagrams). The original `diagrams` 
 lets you draw the cloud system architecture in `Python` code. It was born for prototyping a new system architecture 
-design without any design tools. Under the hood, `diagrams-as-code` parse a `YAML` file and map to specific set of 
-`diagrams`'s functions and classes, and executes them in proper order.
+design without any design tools. Under the hood, `diagrams-as-code` parse a `YAML` file and map to a specific set of 
+`diagrams`'s functions and classes, and execute them in proper order.
 
 But you don't have to worry about `diagrams` because `diagrams-as-code` is self-contained and encapsulates it well.
```

### Comparing `diagrams-as-code-0.0.2/setup.py` & `diagrams-as-code-0.0.3/setup.py`

 * *Files identical despite different names*

