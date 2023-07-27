# Comparing `tmp/collective.easyform-4.1.3.tar.gz` & `tmp/collective.easyform-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.easyform-4.1.3.tar", last modified: Tue May 16 07:21:17 2023, max compression
+gzip compressed data, was "collective.easyform-4.1.4.tar", last modified: Thu Jul 27 15:28:53 2023, max compression
```

## Comparing `collective.easyform-4.1.3.tar` & `collective.easyform-4.1.4.tar`

### file list

```diff
@@ -1,271 +1,291 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.609701 collective.easyform-4.1.3/
--rw-r--r--   0 maurits    (501) staff       (20)    16725 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)      781 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/CONTRIBUTORS.rst
--rw-r--r--   0 maurits    (501) staff       (20)      197 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    26881 2023-05-16 07:21:17.609854 collective.easyform-4.1.3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     9067 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.542689 collective.easyform-4.1.3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)      433 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/INSTALL.txt
--rw-r--r--   0 maurits    (501) staff       (20)    18032 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      736 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2755 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/actions.rst
--rw-r--r--   0 maurits    (501) staff       (20)      677 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/adding.rst
--rw-r--r--   0 maurits    (501) staff       (20)      851 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/collective.easyform.browser.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1784 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/collective.easyform.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8426 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)     1855 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/fields.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.554359 collective.easyform-4.1.3/docs/images/
--rw-r--r--   0 maurits    (501) staff       (20)    41696 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/add-new-action-overlay.png
--rw-r--r--   0 maurits    (501) staff       (20)    41507 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/add-new-field-overlay.png
--rw-r--r--   0 maurits    (501) staff       (20)    20434 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/add-new-fieldset-overlay.png
--rw-r--r--   0 maurits    (501) staff       (20)    20189 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/add-new-menu.png
--rw-r--r--   0 maurits    (501) staff       (20)     5577 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/added-new-action.png
--rw-r--r--   0 maurits    (501) staff       (20)     4427 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/added-new-field.png
--rw-r--r--   0 maurits    (501) staff       (20)     2220 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/added-new-fieldset.png
--rw-r--r--   0 maurits    (501) staff       (20)     8436 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/click-actions-contentview.png
--rw-r--r--   0 maurits    (501) staff       (20)     6638 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/click-add-new-action.png
--rw-r--r--   0 maurits    (501) staff       (20)     6571 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/click-add-new-field.png
--rw-r--r--   0 maurits    (501) staff       (20)     7140 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/click-add-new-fieldset.png
--rw-r--r--   0 maurits    (501) staff       (20)     8513 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/click-fields-contentview.png
--rw-r--r--   0 maurits    (501) staff       (20)   212025 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/conditional_fields_and_field_css.png
--rw-r--r--   0 maurits    (501) staff       (20)    13050 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/created-easyform-actions.png
--rw-r--r--   0 maurits    (501) staff       (20)    22083 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/created-easyform-fields.png
--rw-r--r--   0 maurits    (501) staff       (20)    14271 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/created-easyform.png
--rw-r--r--   0 maurits    (501) staff       (20)    85234 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/default-actions-mailer.png
--rw-r--r--   0 maurits    (501) staff       (20)   139577 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/define-actions-menu-choice.png
--rw-r--r--   0 maurits    (501) staff       (20)    78436 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/easyform-youtube.png
--rw-r--r--   0 maurits    (501) staff       (20)     9762 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/edit-xml-actions-model-button.png
--rw-r--r--   0 maurits    (501) staff       (20)    38328 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/edit-xml-actions-model-page.png
--rw-r--r--   0 maurits    (501) staff       (20)     9283 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/edit-xml-fields-model-button.png
--rw-r--r--   0 maurits    (501) staff       (20)    50439 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/edit-xml-fields-model-page.png
--rw-r--r--   0 maurits    (501) staff       (20)   143076 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/form_multicolumns.png
--rw-r--r--   0 maurits    (501) staff       (20)   124476 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/mailer-adapter-message-settings.png
--rw-r--r--   0 maurits    (501) staff       (20)    75303 2023-05-16 07:21:16.000000 collective.easyform-4.1.3/docs/images/new-easyform-default-contributor.png
--rw-r--r--   0 maurits    (501) staff       (20)    82997 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/images/new-easyform-default.png
--rw-r--r--   0 maurits    (501) staff       (20)   100335 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/images/new-easyform-overrides.png
--rw-r--r--   0 maurits    (501) staff       (20)    62231 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/images/new-easyform-thankspage-contributor.png
--rw-r--r--   0 maurits    (501) staff       (20)    59760 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/images/new-easyform-thankspage.png
--rw-r--r--   0 maurits    (501) staff       (20)     2298 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6453 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/rtd-requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)      405 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/docs/tests.rst
--rw-r--r--   0 maurits    (501) staff       (20)      278 2023-05-16 07:21:17.610330 collective.easyform-4.1.3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2648 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.528786 collective.easyform-4.1.3/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.554748 collective.easyform-4.1.3/src/collective/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.563642 collective.easyform-4.1.3/src/collective/easyform/
--rw-r--r--   0 maurits    (501) staff       (20)      104 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/Form.gif
--rw-r--r--   0 maurits    (501) staff       (20)      135 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    32069 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      748 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/actions.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    10365 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/api.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.573463 collective.easyform-4.1.3/src/collective/easyform/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3084 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/action_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)    12722 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)     3053 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/actions.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4360 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/actions_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3037 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1549 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/controlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)      972 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/easyform.css
--rw-r--r--   0 maurits    (501) staff       (20)      851 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/easyform_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1032 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/easyform_form_embedded.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/easyform_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)      128 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/empty.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2331 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)     7766 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     3398 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/fields.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5233 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/fields_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1243 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/label.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2212 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/likert.py
--rw-r--r--   0 maurits    (501) staff       (20)      958 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/likert.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      973 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/likert_display.pt
--rw-r--r--   0 maurits    (501) staff       (20)      492 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/likert_hidden.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1558 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/likert_input.pt
--rw-r--r--   0 maurits    (501) staff       (20)      777 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/model_listing.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2149 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/modeleditor.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1251 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/rich_label.pt
--rw-r--r--   0 maurits    (501) staff       (20)      956 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/saveddata.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2211 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/saveddata_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1456 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/thank_you.pt
--rw-r--r--   0 maurits    (501) staff       (20)    19775 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/view.py
--rw-r--r--   0 maurits    (501) staff       (20)     2059 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/widget.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3233 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/widgets.py
--rw-r--r--   0 maurits    (501) staff       (20)     4886 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/browser/widgets.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2142 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/config.py
--rw-r--r--   0 maurits    (501) staff       (20)     2181 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      241 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/content.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.574707 collective.easyform-4.1.3/src/collective/easyform/default_schemata/
--rw-r--r--   0 maurits    (501) staff       (20)      494 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/default_schemata/actions_default.xml
--rw-r--r--   0 maurits    (501) staff       (20)      903 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/default_schemata/fields_default.xml
--rw-r--r--   0 maurits    (501) staff       (20)      528 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/default_schemata/mail_body_default.pt
--rw-r--r--   0 maurits    (501) staff       (20)       94 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/default_schemata/model_default.xml
--rw-r--r--   0 maurits    (501) staff       (20)     5668 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)      980 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/exportimport.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9505 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     2309 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/fields.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.577499 collective.easyform-4.1.3/src/collective/easyform/interfaces/
--rw-r--r--   0 maurits    (501) staff       (20)     1694 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3762 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)     1244 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/customscript.py
--rw-r--r--   0 maurits    (501) staff       (20)    17139 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/easyform.py
--rw-r--r--   0 maurits    (501) staff       (20)     8953 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)      177 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)    19973 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/mailer.py
--rw-r--r--   0 maurits    (501) staff       (20)     2910 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/savedata.py
--rw-r--r--   0 maurits    (501) staff       (20)      889 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/interfaces/validators.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.578169 collective.easyform-4.1.3/src/collective/easyform/locales/
--rw-r--r--   0 maurits    (501) staff       (20)    32629 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/collective.easyform.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.530400 collective.easyform-4.1.3/src/collective/easyform/locales/de/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.578837 collective.easyform-4.1.3/src/collective/easyform/locales/de/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    37093 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      679 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/de/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.530801 collective.easyform-4.1.3/src/collective/easyform/locales/en/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.579498 collective.easyform-4.1.3/src/collective/easyform/locales/en/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    32468 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      654 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.531195 collective.easyform-4.1.3/src/collective/easyform/locales/es/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.580165 collective.easyform-4.1.3/src/collective/easyform/locales/es/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    46845 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      718 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.531603 collective.easyform-4.1.3/src/collective/easyform/locales/eu/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.580816 collective.easyform-4.1.3/src/collective/easyform/locales/eu/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    43331 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      656 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/eu/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.532009 collective.easyform-4.1.3/src/collective/easyform/locales/fr/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.581452 collective.easyform-4.1.3/src/collective/easyform/locales/fr/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    47080 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      667 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.532455 collective.easyform-4.1.3/src/collective/easyform/locales/it/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.582084 collective.easyform-4.1.3/src/collective/easyform/locales/it/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    37804 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      654 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/it/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.532872 collective.easyform-4.1.3/src/collective/easyform/locales/ja/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.582707 collective.easyform-4.1.3/src/collective/easyform/locales/ja/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    63446 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      647 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/ja/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.533278 collective.easyform-4.1.3/src/collective/easyform/locales/nl/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.583325 collective.easyform-4.1.3/src/collective/easyform/locales/nl/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    44857 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      689 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/nl/LC_MESSAGES/plone.po
--rw-r--r--   0 maurits    (501) staff       (20)      653 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/plone.pot
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.533681 collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.583963 collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    44331 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      653 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.534081 collective.easyform-4.1.3/src/collective/easyform/locales/uk/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.584575 collective.easyform-4.1.3/src/collective/easyform/locales/uk/LC_MESSAGES/
--rw-r--r--   0 maurits    (501) staff       (20)    52193 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.po
--rw-r--r--   0 maurits    (501) staff       (20)      682 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/locales/uk/LC_MESSAGES/plone.po
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.586083 collective.easyform-4.1.3/src/collective/easyform/migration/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5058 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      393 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2278 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/data.py
--rw-r--r--   0 maurits    (501) staff       (20)    10128 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/fields.py
--rw-r--r--   0 maurits    (501) staff       (20)     4012 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/migration/pfg.py
--rw-r--r--   0 maurits    (501) staff       (20)     1429 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.535118 collective.easyform-4.1.3/src/collective/easyform/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.587972 collective.easyform-4.1.3/src/collective/easyform/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)     4710 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      427 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)       71 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     3345 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2186 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/rolemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.588254 collective.easyform-4.1.3/src/collective/easyform/profiles/default/types/
--rw-r--r--   0 maurits    (501) staff       (20)     2408 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/types/EasyForm.xml
--rw-r--r--   0 maurits    (501) staff       (20)      166 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/default/types.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.589787 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/
--rw-r--r--   0 maurits    (501) staff       (20)      732 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 maurits    (501) staff       (20)      272 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)      190 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/types.xml
--rw-r--r--   0 maurits    (501) staff       (20)     5236 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/serializer.py
--rw-r--r--   0 maurits    (501) staff       (20)      805 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)      269 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/subscribers.py
--rw-r--r--   0 maurits    (501) staff       (20)      453 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/subscribers.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.596881 collective.easyform-4.1.3/src/collective/easyform/tests/
--rw-r--r--   0 maurits    (501) staff       (20)     4339 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/PloneLogo.png
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4813 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/action_errors.rst
--rw-r--r--   0 maurits    (501) staff       (20)    10119 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/attachment.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4498 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     2924 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/basic.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7732 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/browser.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.601199 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/
--rw-r--r--   0 maurits    (501) staff       (20)     1077 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_file.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1492 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_form.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_multiple_choice.xml
--rw-r--r--   0 maurits    (501) staff       (20)      921 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_recaptcha.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_with_single_field.xml
--rw-r--r--   0 maurits    (501) staff       (20)      826 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/hcaptcha.xml
--rw-r--r--   0 maurits    (501) staff       (20)      799 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/hidden_form.xml
--rw-r--r--   0 maurits    (501) staff       (20)      879 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/radio_form.xml
--rw-r--r--   0 maurits    (501) staff       (20)      827 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/recaptcha.xml
--rw-r--r--   0 maurits    (501) staff       (20)      921 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/single_field.xml
--rw-r--r--   0 maurits    (501) staff       (20)      263 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/tests.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      883 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/wrapper_template.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.603948 collective.easyform-4.1.3/src/collective/easyform/tests/robot/
--rw-r--r--   0 maurits    (501) staff       (20)     2005 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/keywords.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3099 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_addform.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1517 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_editxmlmodel.robot
--rw-r--r--   0 maurits    (501) staff       (20)      619 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_headerinjection.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2201 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addaction.robot
--rw-r--r--   0 maurits    (501) staff       (20)     2564 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addfield.robot
--rw-r--r--   0 maurits    (501) staff       (20)     1447 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addfieldset.robot
--rw-r--r--   0 maurits    (501) staff       (20)      542 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_submit.robot
--rw-r--r--   0 maurits    (501) staff       (20)     3431 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/serverside_field.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1966 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/ssl.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8436 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testApi.py
--rw-r--r--   0 maurits    (501) staff       (20)     4656 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testControlpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)    10802 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testCustomScript.py
--rw-r--r--   0 maurits    (501) staff       (20)     2061 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testDocTests.py
--rw-r--r--   0 maurits    (501) staff       (20)     5394 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testEmbedding.py
--rw-r--r--   0 maurits    (501) staff       (20)     1113 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testEvents.py
--rw-r--r--   0 maurits    (501) staff       (20)     5957 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testLikert.py
--rw-r--r--   0 maurits    (501) staff       (20)    29357 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testMailer.py
--rw-r--r--   0 maurits    (501) staff       (20)     3830 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testMisc.py
--rw-r--r--   0 maurits    (501) staff       (20)     8312 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testSavedDataSerializer.py
--rw-r--r--   0 maurits    (501) staff       (20)    27302 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testSaver.py
--rw-r--r--   0 maurits    (501) staff       (20)     4039 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testSetup.py
--rw-r--r--   0 maurits    (501) staff       (20)     6799 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testThanksPage.py
--rw-r--r--   0 maurits    (501) staff       (20)    18564 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/testValidators.py
--rw-r--r--   0 maurits    (501) staff       (20)      780 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/tests/test_robot.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.608931 collective.easyform-4.1.3/src/collective/easyform/upgrades/
--rw-r--r--   0 maurits    (501) staff       (20)      508 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1001.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      582 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1002.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      449 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1003.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      466 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1004.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      495 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1005.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      442 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1006.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      518 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1007.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1008.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1009.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      400 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1010.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      398 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1011.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      410 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1012.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      414 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1013.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      400 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1014.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      395 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1015.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      654 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/1016.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3231 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      562 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.536378 collective.easyform-4.1.3/src/collective/easyform/upgrades/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.609458 collective.easyform-4.1.3/src/collective/easyform/upgrades/profiles/1016/
--rw-r--r--   0 maurits    (501) staff       (20)     1480 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/profiles/1016/actions.xml
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/upgrades/profiles/1016/registry.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2532 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/validators.py
--rw-r--r--   0 maurits    (501) staff       (20)      749 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/validators.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4317 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/vocabularies.py
--rw-r--r--   0 maurits    (501) staff       (20)     1347 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective/easyform/vocabularies.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-05-16 07:21:17.557205 collective.easyform-4.1.3/src/collective.easyform.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    26881 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)    10353 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      636 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2023-05-16 07:21:17.000000 collective.easyform-4.1.3/src/collective.easyform.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.779812 collective.easyform-4.1.4/
+-rw-r--r--   0 maurits    (501) staff       (20)    16916 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      781 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/CONTRIBUTORS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      197 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    27093 2023-07-27 15:28:53.779976 collective.easyform-4.1.4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     9088 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.720124 collective.easyform-4.1.4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)      433 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/INSTALL.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    18032 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      736 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2755 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/actions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/adding.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      851 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/collective.easyform.browser.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1784 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/collective.easyform.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8426 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1855 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/fields.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.728979 collective.easyform-4.1.4/docs/images/
+-rw-r--r--   0 maurits    (501) staff       (20)    41696 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/add-new-action-overlay.png
+-rw-r--r--   0 maurits    (501) staff       (20)    41507 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/add-new-field-overlay.png
+-rw-r--r--   0 maurits    (501) staff       (20)    20434 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/add-new-fieldset-overlay.png
+-rw-r--r--   0 maurits    (501) staff       (20)    20189 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/add-new-menu.png
+-rw-r--r--   0 maurits    (501) staff       (20)     5577 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/added-new-action.png
+-rw-r--r--   0 maurits    (501) staff       (20)     4427 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/added-new-field.png
+-rw-r--r--   0 maurits    (501) staff       (20)     2220 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/added-new-fieldset.png
+-rw-r--r--   0 maurits    (501) staff       (20)     8436 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/click-actions-contentview.png
+-rw-r--r--   0 maurits    (501) staff       (20)     6638 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/click-add-new-action.png
+-rw-r--r--   0 maurits    (501) staff       (20)     6571 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/click-add-new-field.png
+-rw-r--r--   0 maurits    (501) staff       (20)     7140 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/click-add-new-fieldset.png
+-rw-r--r--   0 maurits    (501) staff       (20)     8513 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/click-fields-contentview.png
+-rw-r--r--   0 maurits    (501) staff       (20)   212025 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/conditional_fields_and_field_css.png
+-rw-r--r--   0 maurits    (501) staff       (20)    13050 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/created-easyform-actions.png
+-rw-r--r--   0 maurits    (501) staff       (20)    22083 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/created-easyform-fields.png
+-rw-r--r--   0 maurits    (501) staff       (20)    14271 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/created-easyform.png
+-rw-r--r--   0 maurits    (501) staff       (20)    85234 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/default-actions-mailer.png
+-rw-r--r--   0 maurits    (501) staff       (20)   139577 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/define-actions-menu-choice.png
+-rw-r--r--   0 maurits    (501) staff       (20)    78436 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/easyform-youtube.png
+-rw-r--r--   0 maurits    (501) staff       (20)     9762 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/edit-xml-actions-model-button.png
+-rw-r--r--   0 maurits    (501) staff       (20)    38328 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/edit-xml-actions-model-page.png
+-rw-r--r--   0 maurits    (501) staff       (20)     9283 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/edit-xml-fields-model-button.png
+-rw-r--r--   0 maurits    (501) staff       (20)    50439 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/edit-xml-fields-model-page.png
+-rw-r--r--   0 maurits    (501) staff       (20)   143076 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/form_multicolumns.png
+-rw-r--r--   0 maurits    (501) staff       (20)   124476 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/mailer-adapter-message-settings.png
+-rw-r--r--   0 maurits    (501) staff       (20)    75303 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/new-easyform-default-contributor.png
+-rw-r--r--   0 maurits    (501) staff       (20)    82997 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/new-easyform-default.png
+-rw-r--r--   0 maurits    (501) staff       (20)   100335 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/new-easyform-overrides.png
+-rw-r--r--   0 maurits    (501) staff       (20)    62231 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/new-easyform-thankspage-contributor.png
+-rw-r--r--   0 maurits    (501) staff       (20)    59760 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/images/new-easyform-thankspage.png
+-rw-r--r--   0 maurits    (501) staff       (20)     2298 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6453 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/rtd-requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      405 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/docs/tests.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      278 2023-07-27 15:28:53.780486 collective.easyform-4.1.4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2648 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.711618 collective.easyform-4.1.4/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.729275 collective.easyform-4.1.4/src/collective/
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.736479 collective.easyform-4.1.4/src/collective/easyform/
+-rw-r--r--   0 maurits    (501) staff       (20)      104 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/Form.gif
+-rw-r--r--   0 maurits    (501) staff       (20)      135 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    32069 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      748 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/actions.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    10365 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/api.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.744094 collective.easyform-4.1.4/src/collective/easyform/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3084 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/action_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    12722 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3053 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/actions.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4360 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/actions_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3228 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1549 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/controlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)      972 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/easyform.css
+-rw-r--r--   0 maurits    (501) staff       (20)      851 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/easyform_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1032 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/easyform_form_embedded.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/easyform_layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      128 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/empty.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2331 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7766 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3398 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/fields.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5233 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/fields_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1243 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/label.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2212 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/likert.py
+-rw-r--r--   0 maurits    (501) staff       (20)      958 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/likert.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      973 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/likert_display.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      492 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/likert_hidden.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1558 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/likert_input.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      777 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/model_listing.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2149 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/modeleditor.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1251 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/rich_label.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      956 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/saveddata.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2211 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/saveddata_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1456 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/thank_you.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    19775 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2059 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/widget.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3233 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/widgets.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4886 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/browser/widgets.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2142 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/config.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2181 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      241 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/content.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.745209 collective.easyform-4.1.4/src/collective/easyform/default_schemata/
+-rw-r--r--   0 maurits    (501) staff       (20)      494 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/default_schemata/actions_default.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      903 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/default_schemata/fields_default.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      528 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/default_schemata/mail_body_default.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       94 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/default_schemata/model_default.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     5668 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)      980 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/exportimport.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9505 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2309 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/fields.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.747390 collective.easyform-4.1.4/src/collective/easyform/interfaces/
+-rw-r--r--   0 maurits    (501) staff       (20)     1694 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/interfaces/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3762 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/interfaces/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1244 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/interfaces/customscript.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17139 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/interfaces/easyform.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8953 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/interfaces/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)      177 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/interfaces/layer.py
+-rw-r--r--   0 maurits    (501) staff       (20)    19973 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/interfaces/mailer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2910 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/interfaces/savedata.py
+-rw-r--r--   0 maurits    (501) staff       (20)      889 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/interfaces/validators.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.747962 collective.easyform-4.1.4/src/collective/easyform/locales/
+-rw-r--r--   0 maurits    (501) staff       (20)    32629 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/collective.easyform.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.712380 collective.easyform-4.1.4/src/collective/easyform/locales/de/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.749044 collective.easyform-4.1.4/src/collective/easyform/locales/de/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    10818 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.mo
+-rw-r--r--   0 maurits    (501) staff       (20)    37093 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      532 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/de/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      679 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/de/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.712638 collective.easyform-4.1.4/src/collective/easyform/locales/en/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.750005 collective.easyform-4.1.4/src/collective/easyform/locales/en/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)      458 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.mo
+-rw-r--r--   0 maurits    (501) staff       (20)    32468 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      458 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      654 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.712830 collective.easyform-4.1.4/src/collective/easyform/locales/es/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.751146 collective.easyform-4.1.4/src/collective/easyform/locales/es/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    22175 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.mo
+-rw-r--r--   0 maurits    (501) staff       (20)    46845 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      563 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/es/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      718 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.713024 collective.easyform-4.1.4/src/collective/easyform/locales/eu/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.752312 collective.easyform-4.1.4/src/collective/easyform/locales/eu/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    17463 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.mo
+-rw-r--r--   0 maurits    (501) staff       (20)    43331 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      501 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/eu/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      656 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.713214 collective.easyform-4.1.4/src/collective/easyform/locales/fr/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.753386 collective.easyform-4.1.4/src/collective/easyform/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    22405 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.mo
+-rw-r--r--   0 maurits    (501) staff       (20)    47080 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      520 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      667 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.713406 collective.easyform-4.1.4/src/collective/easyform/locales/it/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.754455 collective.easyform-4.1.4/src/collective/easyform/locales/it/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    10596 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.mo
+-rw-r--r--   0 maurits    (501) staff       (20)    37804 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      458 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      654 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/it/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.713604 collective.easyform-4.1.4/src/collective/easyform/locales/ja/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.755524 collective.easyform-4.1.4/src/collective/easyform/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    22354 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.mo
+-rw-r--r--   0 maurits    (501) staff       (20)    63446 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      451 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/ja/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      647 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/ja/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.713796 collective.easyform-4.1.4/src/collective/easyform/locales/nl/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.756562 collective.easyform-4.1.4/src/collective/easyform/locales/nl/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    18660 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.mo
+-rw-r--r--   0 maurits    (501) staff       (20)    44857 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      538 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      689 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/nl/LC_MESSAGES/plone.po
+-rw-r--r--   0 maurits    (501) staff       (20)      653 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/plone.pot
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.713988 collective.easyform-4.1.4/src/collective/easyform/locales/pt_BR/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.757699 collective.easyform-4.1.4/src/collective/easyform/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    18432 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.mo
+-rw-r--r--   0 maurits    (501) staff       (20)    44331 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      506 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      653 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.714179 collective.easyform-4.1.4/src/collective/easyform/locales/uk/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.758772 collective.easyform-4.1.4/src/collective/easyform/locales/uk/LC_MESSAGES/
+-rw-r--r--   0 maurits    (501) staff       (20)    22068 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.mo
+-rw-r--r--   0 maurits    (501) staff       (20)    52193 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.po
+-rw-r--r--   0 maurits    (501) staff       (20)      535 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/uk/LC_MESSAGES/plone.mo
+-rw-r--r--   0 maurits    (501) staff       (20)      682 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/locales/uk/LC_MESSAGES/plone.po
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.760110 collective.easyform-4.1.4/src/collective/easyform/migration/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/migration/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5058 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/migration/actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      393 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/migration/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2278 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/migration/data.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10134 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/migration/fields.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4012 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/migration/pfg.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1429 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.714766 collective.easyform-4.1.4/src/collective/easyform/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.762016 collective.easyform-4.1.4/src/collective/easyform/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)     4710 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/default/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/default/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      427 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/default/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       71 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     3345 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/default/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2186 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/default/rolemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.762257 collective.easyform-4.1.4/src/collective/easyform/profiles/default/types/
+-rw-r--r--   0 maurits    (501) staff       (20)     2408 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/default/types/EasyForm.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      166 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/default/types.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.763501 collective.easyform-4.1.4/src/collective/easyform/profiles/uninstall/
+-rw-r--r--   0 maurits    (501) staff       (20)      732 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/uninstall/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      272 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/uninstall/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      190 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/profiles/uninstall/types.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     5236 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/serializer.py
+-rw-r--r--   0 maurits    (501) staff       (20)      805 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      269 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/subscribers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      453 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/subscribers.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.769762 collective.easyform-4.1.4/src/collective/easyform/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)     4339 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/PloneLogo.png
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4813 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/action_errors.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    10119 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/attachment.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4498 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2924 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/basic.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7732 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/browser.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.772616 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/
+-rw-r--r--   0 maurits    (501) staff       (20)     1077 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/fieldset_file.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1492 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/fieldset_form.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/fieldset_multiple_choice.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      921 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/fieldset_recaptcha.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1019 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/fieldset_with_single_field.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      826 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/hcaptcha.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      799 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/hidden_form.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      879 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/radio_form.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      827 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/recaptcha.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      921 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/single_field.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      263 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/tests.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      883 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/wrapper_template.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.774648 collective.easyform-4.1.4/src/collective/easyform/tests/robot/
+-rw-r--r--   0 maurits    (501) staff       (20)     2005 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/robot/keywords.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3099 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/robot/test_addform.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1517 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/robot/test_editxmlmodel.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      619 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/robot/test_headerinjection.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2201 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/robot/todo_test_addaction.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     2564 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/robot/todo_test_addfield.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     1447 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/robot/todo_test_addfieldset.robot
+-rw-r--r--   0 maurits    (501) staff       (20)      542 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/robot/todo_test_submit.robot
+-rw-r--r--   0 maurits    (501) staff       (20)     3431 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/serverside_field.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1966 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/ssl.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8436 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testApi.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4656 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testControlpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10802 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testCustomScript.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2061 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testDocTests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5394 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testEmbedding.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1113 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testEvents.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5957 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testLikert.py
+-rw-r--r--   0 maurits    (501) staff       (20)    29357 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testMailer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3830 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testMisc.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8312 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testSavedDataSerializer.py
+-rw-r--r--   0 maurits    (501) staff       (20)    27302 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testSaver.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4039 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testSetup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6799 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testThanksPage.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18552 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/testValidators.py
+-rw-r--r--   0 maurits    (501) staff       (20)      780 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/tests/test_robot.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.779000 collective.easyform-4.1.4/src/collective/easyform/upgrades/
+-rw-r--r--   0 maurits    (501) staff       (20)      508 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1001.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      582 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1002.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      449 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1003.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      466 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1004.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      495 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1005.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      442 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1006.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      518 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1007.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1008.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      397 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1009.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      400 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1010.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      398 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1011.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      410 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1012.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      414 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1013.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      400 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1014.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      395 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1015.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      654 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/1016.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3231 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      562 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.715408 collective.easyform-4.1.4/src/collective/easyform/upgrades/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.779498 collective.easyform-4.1.4/src/collective/easyform/upgrades/profiles/1016/
+-rw-r--r--   0 maurits    (501) staff       (20)     1480 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/profiles/1016/actions.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/upgrades/profiles/1016/registry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2532 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/validators.py
+-rw-r--r--   0 maurits    (501) staff       (20)      749 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/validators.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4317 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/vocabularies.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1347 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective/easyform/vocabularies.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-27 15:28:53.731336 collective.easyform-4.1.4/src/collective.easyform.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    27093 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective.easyform.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)    11619 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective.easyform.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective.easyform.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective.easyform.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective.easyform.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective.easyform.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      636 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective.easyform.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-07-27 15:28:53.000000 collective.easyform-4.1.4/src/collective.easyform.egg-info/top_level.txt
```

### Comparing `collective.easyform-4.1.3/CHANGES.rst` & `collective.easyform-4.1.4/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 Changelog
 =========
 
 
+4.1.4 (2023-07-27)
+------------------
+
+- fix folder_contents accessibility from @@saveddata. [ThibautBorn]
+
+- make ReCaptcha fields not required during PloneFormGen migration [ThibautBorn]
+
+
 4.1.3 (2023-05-16)
 ------------------
 
 
 Bug fixes:
 
 - Add upgrade step and profile to update contenttype icon in registry.
```

### Comparing `collective.easyform-4.1.3/CONTRIBUTORS.rst` & `collective.easyform-4.1.4/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/PKG-INFO` & `collective.easyform-4.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.easyform
-Version: 4.1.3
+Version: 4.1.4
 Summary: Forms for Plone
 Home-page: https://github.com/collective/collective.easyform
 Author: Roman Kozlovskyi
 Author-email: krzroman@gmail.com
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -33,16 +33,16 @@
 EasyForm - Form Builder for Plone
 =================================
 
 .. image:: https://badge.fury.io/py/collective.easyform.svg
     :target: https://badge.fury.io/py/collective.easyform
     :alt: latest release version badge by Badge Fury
 
-.. image:: https://travis-ci.org/collective/collective.easyform.png?branch=master
-    :target: https://travis-ci.org/collective/collective.easyform
+.. image:: https://github.com/collective/collective.easyform/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/collective/collective.easyform/actions
     :alt: Travis CI status
 
 .. image:: https://coveralls.io/repos/github/collective/collective.easyform/badge.svg?branch=master
     :target: https://coveralls.io/github/collective/collective.easyform?branch=master
     :alt: Coveralls status
 
 
@@ -342,14 +342,22 @@
 - 3.x targets Plone 5.2
 - 4.x targets Plone 6, on Python 3
 
 Changelog
 =========
 
 
+4.1.4 (2023-07-27)
+------------------
+
+- fix folder_contents accessibility from @@saveddata. [ThibautBorn]
+
+- make ReCaptcha fields not required during PloneFormGen migration [ThibautBorn]
+
+
 4.1.3 (2023-05-16)
 ------------------
 
 
 Bug fixes:
 
 - Add upgrade step and profile to update contenttype icon in registry.
```

### Comparing `collective.easyform-4.1.3/README.rst` & `collective.easyform-4.1.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 EasyForm - Form Builder for Plone
 =================================
 
 .. image:: https://badge.fury.io/py/collective.easyform.svg
     :target: https://badge.fury.io/py/collective.easyform
     :alt: latest release version badge by Badge Fury
 
-.. image:: https://travis-ci.org/collective/collective.easyform.png?branch=master
-    :target: https://travis-ci.org/collective/collective.easyform
+.. image:: https://github.com/collective/collective.easyform/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/collective/collective.easyform/actions
     :alt: Travis CI status
 
 .. image:: https://coveralls.io/repos/github/collective/collective.easyform/badge.svg?branch=master
     :target: https://coveralls.io/github/collective/collective.easyform?branch=master
     :alt: Coveralls status
```

### Comparing `collective.easyform-4.1.3/docs/LICENSE.GPL` & `collective.easyform-4.1.4/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/LICENSE.txt` & `collective.easyform-4.1.4/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/actions.rst` & `collective.easyform-4.1.4/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/adding.rst` & `collective.easyform-4.1.4/docs/adding.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/collective.easyform.browser.rst` & `collective.easyform-4.1.4/docs/collective.easyform.browser.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/collective.easyform.rst` & `collective.easyform-4.1.4/docs/collective.easyform.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/conf.py` & `collective.easyform-4.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/fields.rst` & `collective.easyform-4.1.4/docs/fields.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/add-new-action-overlay.png` & `collective.easyform-4.1.4/docs/images/add-new-action-overlay.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/add-new-field-overlay.png` & `collective.easyform-4.1.4/docs/images/add-new-field-overlay.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/add-new-fieldset-overlay.png` & `collective.easyform-4.1.4/docs/images/add-new-fieldset-overlay.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/add-new-menu.png` & `collective.easyform-4.1.4/docs/images/add-new-menu.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/added-new-action.png` & `collective.easyform-4.1.4/docs/images/added-new-action.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/added-new-field.png` & `collective.easyform-4.1.4/docs/images/added-new-field.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/added-new-fieldset.png` & `collective.easyform-4.1.4/docs/images/added-new-fieldset.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/click-actions-contentview.png` & `collective.easyform-4.1.4/docs/images/click-actions-contentview.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/click-add-new-action.png` & `collective.easyform-4.1.4/docs/images/click-add-new-action.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/click-add-new-field.png` & `collective.easyform-4.1.4/docs/images/click-add-new-field.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/click-add-new-fieldset.png` & `collective.easyform-4.1.4/docs/images/click-add-new-fieldset.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/click-fields-contentview.png` & `collective.easyform-4.1.4/docs/images/click-fields-contentview.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/conditional_fields_and_field_css.png` & `collective.easyform-4.1.4/docs/images/conditional_fields_and_field_css.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/created-easyform-actions.png` & `collective.easyform-4.1.4/docs/images/created-easyform-actions.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/created-easyform-fields.png` & `collective.easyform-4.1.4/docs/images/created-easyform-fields.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/created-easyform.png` & `collective.easyform-4.1.4/docs/images/created-easyform.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/default-actions-mailer.png` & `collective.easyform-4.1.4/docs/images/default-actions-mailer.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/define-actions-menu-choice.png` & `collective.easyform-4.1.4/docs/images/define-actions-menu-choice.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/easyform-youtube.png` & `collective.easyform-4.1.4/docs/images/easyform-youtube.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/edit-xml-actions-model-button.png` & `collective.easyform-4.1.4/docs/images/edit-xml-actions-model-button.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/edit-xml-actions-model-page.png` & `collective.easyform-4.1.4/docs/images/edit-xml-actions-model-page.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/edit-xml-fields-model-button.png` & `collective.easyform-4.1.4/docs/images/edit-xml-fields-model-button.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/edit-xml-fields-model-page.png` & `collective.easyform-4.1.4/docs/images/edit-xml-fields-model-page.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/form_multicolumns.png` & `collective.easyform-4.1.4/docs/images/form_multicolumns.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/mailer-adapter-message-settings.png` & `collective.easyform-4.1.4/docs/images/mailer-adapter-message-settings.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/new-easyform-default-contributor.png` & `collective.easyform-4.1.4/docs/images/new-easyform-default-contributor.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/new-easyform-default.png` & `collective.easyform-4.1.4/docs/images/new-easyform-default.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/new-easyform-overrides.png` & `collective.easyform-4.1.4/docs/images/new-easyform-overrides.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/new-easyform-thankspage-contributor.png` & `collective.easyform-4.1.4/docs/images/new-easyform-thankspage-contributor.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/images/new-easyform-thankspage.png` & `collective.easyform-4.1.4/docs/images/new-easyform-thankspage.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/index.rst` & `collective.easyform-4.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/docs/rtd-requirements.txt` & `collective.easyform-4.1.4/docs/rtd-requirements.txt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/setup.py` & `collective.easyform-4.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.1.3"
+version = "4.1.4"
 
 setup(
     name="collective.easyform",
     version=version,
     description="Forms for Plone",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     # Get more strings from https://pypi.org/classifiers/
```

### Comparing `collective.easyform-4.1.3/src/collective/easyform/actions.py` & `collective.easyform-4.1.4/src/collective/easyform/actions.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/actions.zcml` & `collective.easyform-4.1.4/src/collective/easyform/actions.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/api.py` & `collective.easyform-4.1.4/src/collective/easyform/api.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/action_input.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/action_input.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/actions.py` & `collective.easyform-4.1.4/src/collective/easyform/browser/actions.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/actions.zcml` & `collective.easyform-4.1.4/src/collective/easyform/browser/actions.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/actions_listing.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/actions_listing.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/configure.zcml` & `collective.easyform-4.1.4/src/collective/easyform/browser/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,20 @@
       />
   <browser:page
       name="folder_contents"
       for="collective.easyform.interfaces.IEasyForm"
       permission="zope2.View"
       class=".view.FolderContentsView"
       />
+  <browser:page
+      name="folder_contents"
+      for="collective.easyform.browser.actions.EasyFormActionsView"
+      permission="zope2.View"
+      class=".view.FolderContentsView"
+      />
   <configure zcml:condition="installed plone.dexterity.exportimport">
     <browser:page
         name="export-easyform"
         for="collective.easyform.interfaces.IEasyForm"
         permission="cmf.ManagePortal"
         class=".exportimport.EasyFormExportView"
         layer="..interfaces.IEasyFormLayer"
```

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/controlpanel.py` & `collective.easyform-4.1.4/src/collective/easyform/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/easyform.css` & `collective.easyform-4.1.4/src/collective/easyform/browser/easyform.css`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/easyform_form.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/easyform_form.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/easyform_form_embedded.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/easyform_form_embedded.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/easyform_layout.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/easyform_layout.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/exportimport.py` & `collective.easyform-4.1.4/src/collective/easyform/browser/exportimport.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/fields.py` & `collective.easyform-4.1.4/src/collective/easyform/browser/fields.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/fields.zcml` & `collective.easyform-4.1.4/src/collective/easyform/browser/fields.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/fields_listing.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/fields_listing.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/label.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/label.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/likert.py` & `collective.easyform-4.1.4/src/collective/easyform/browser/likert.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/likert.zcml` & `collective.easyform-4.1.4/src/collective/easyform/browser/likert.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/likert_display.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/likert_display.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/likert_input.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/likert_input.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/model_listing.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/model_listing.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/modeleditor.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/modeleditor.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/rich_label.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/rich_label.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/saveddata.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/saveddata.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/saveddata_form.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/saveddata_form.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/thank_you.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/thank_you.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/view.py` & `collective.easyform-4.1.4/src/collective/easyform/browser/view.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/widget.pt` & `collective.easyform-4.1.4/src/collective/easyform/browser/widget.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/widgets.py` & `collective.easyform-4.1.4/src/collective/easyform/browser/widgets.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/browser/widgets.zcml` & `collective.easyform-4.1.4/src/collective/easyform/browser/widgets.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/config.py` & `collective.easyform-4.1.4/src/collective/easyform/config.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/configure.zcml` & `collective.easyform-4.1.4/src/collective/easyform/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/default_schemata/fields_default.xml` & `collective.easyform-4.1.4/src/collective/easyform/default_schemata/fields_default.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/default_schemata/mail_body_default.pt` & `collective.easyform-4.1.4/src/collective/easyform/default_schemata/mail_body_default.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/exportimport.py` & `collective.easyform-4.1.4/src/collective/easyform/exportimport.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/exportimport.zcml` & `collective.easyform-4.1.4/src/collective/easyform/exportimport.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/fields.py` & `collective.easyform-4.1.4/src/collective/easyform/fields.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/fields.zcml` & `collective.easyform-4.1.4/src/collective/easyform/fields.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/interfaces/__init__.py` & `collective.easyform-4.1.4/src/collective/easyform/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/interfaces/actions.py` & `collective.easyform-4.1.4/src/collective/easyform/interfaces/actions.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/interfaces/customscript.py` & `collective.easyform-4.1.4/src/collective/easyform/interfaces/customscript.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/interfaces/easyform.py` & `collective.easyform-4.1.4/src/collective/easyform/interfaces/easyform.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/interfaces/fields.py` & `collective.easyform-4.1.4/src/collective/easyform/interfaces/fields.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/interfaces/mailer.py` & `collective.easyform-4.1.4/src/collective/easyform/interfaces/mailer.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/interfaces/savedata.py` & `collective.easyform-4.1.4/src/collective/easyform/interfaces/savedata.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/interfaces/validators.py` & `collective.easyform-4.1.4/src/collective/easyform/interfaces/validators.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/collective.easyform.pot` & `collective.easyform-4.1.4/src/collective/easyform/locales/collective.easyform.pot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/de/LC_MESSAGES/plone.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/de/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/en/LC_MESSAGES/plone.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/es/LC_MESSAGES/plone.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/eu/LC_MESSAGES/plone.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/eu/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/fr/LC_MESSAGES/plone.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/it/LC_MESSAGES/plone.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/it/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/ja/LC_MESSAGES/plone.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/ja/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/nl/LC_MESSAGES/plone.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/plone.pot` & `collective.easyform-4.1.4/src/collective/easyform/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/locales/uk/LC_MESSAGES/plone.po` & `collective.easyform-4.1.4/src/collective/easyform/locales/uk/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/migration/actions.py` & `collective.easyform-4.1.4/src/collective/easyform/migration/actions.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/migration/data.py` & `collective.easyform-4.1.4/src/collective/easyform/migration/data.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/migration/fields.py` & `collective.easyform-4.1.4/src/collective/easyform/migration/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     "FormMultiSelectionField": Type("zope.schema.Set", append_field),
     "FormTextField": Type("zope.schema.Text", append_field),
     "FormRichTextField": Type("plone.app.textfield.RichText", append_field),
     "FormRichLabelField": Type(
         "collective.easyform.fields.RichLabel", append_label_field
     ),
     "FormFileField": Type("plone.namedfile.field.NamedBlobFile", append_field),
-    "FormCaptchaField": Type("collective.easyform.fields.ReCaptcha", append_field),
+    "FormCaptchaField": Type("collective.easyform.fields.ReCaptcha", append_label_field),
     "FormLikertField": Type("collective.easyform.fields.Likert", append_field),
     "FieldsetStart": Type("", append_fieldset),
     "FieldsetEnd": Type("", None),
 }
 
 PROPERTIES_MAPPING = {
     "description": Property("description", append_node),
```

### Comparing `collective.easyform-4.1.3/src/collective/easyform/migration/pfg.py` & `collective.easyform-4.1.4/src/collective/easyform/migration/pfg.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/permissions.zcml` & `collective.easyform-4.1.4/src/collective/easyform/permissions.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/profiles/default/actions.xml` & `collective.easyform-4.1.4/src/collective/easyform/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/profiles/default/registry.xml` & `collective.easyform-4.1.4/src/collective/easyform/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/profiles/default/rolemap.xml` & `collective.easyform-4.1.4/src/collective/easyform/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/profiles/default/types/EasyForm.xml` & `collective.easyform-4.1.4/src/collective/easyform/profiles/default/types/EasyForm.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/profiles/uninstall/actions.xml` & `collective.easyform-4.1.4/src/collective/easyform/profiles/uninstall/actions.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/serializer.py` & `collective.easyform-4.1.4/src/collective/easyform/serializer.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/setuphandlers.py` & `collective.easyform-4.1.4/src/collective/easyform/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/PloneLogo.png` & `collective.easyform-4.1.4/src/collective/easyform/tests/PloneLogo.png`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/action_errors.rst` & `collective.easyform-4.1.4/src/collective/easyform/tests/action_errors.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/attachment.rst` & `collective.easyform-4.1.4/src/collective/easyform/tests/attachment.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/base.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/base.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/basic.rst` & `collective.easyform-4.1.4/src/collective/easyform/tests/basic.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/browser.rst` & `collective.easyform-4.1.4/src/collective/easyform/tests/browser.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_file.xml` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/fieldset_file.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_form.xml` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/fieldset_form.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_multiple_choice.xml` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/fieldset_multiple_choice.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_recaptcha.xml` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/fieldset_recaptcha.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/fieldset_with_single_field.xml` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/fieldset_with_single_field.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/hcaptcha.xml` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/hcaptcha.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/hidden_form.xml` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/hidden_form.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/radio_form.xml` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/radio_form.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/recaptcha.xml` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/recaptcha.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/single_field.xml` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/single_field.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/fixtures/wrapper_template.pt` & `collective.easyform-4.1.4/src/collective/easyform/tests/fixtures/wrapper_template.pt`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/robot/keywords.robot` & `collective.easyform-4.1.4/src/collective/easyform/tests/robot/keywords.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_addform.robot` & `collective.easyform-4.1.4/src/collective/easyform/tests/robot/test_addform.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_editxmlmodel.robot` & `collective.easyform-4.1.4/src/collective/easyform/tests/robot/test_editxmlmodel.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/robot/test_headerinjection.robot` & `collective.easyform-4.1.4/src/collective/easyform/tests/robot/test_headerinjection.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addaction.robot` & `collective.easyform-4.1.4/src/collective/easyform/tests/robot/todo_test_addaction.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addfield.robot` & `collective.easyform-4.1.4/src/collective/easyform/tests/robot/todo_test_addfield.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_addfieldset.robot` & `collective.easyform-4.1.4/src/collective/easyform/tests/robot/todo_test_addfieldset.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/robot/todo_test_submit.robot` & `collective.easyform-4.1.4/src/collective/easyform/tests/robot/todo_test_submit.robot`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/serverside_field.rst` & `collective.easyform-4.1.4/src/collective/easyform/tests/serverside_field.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/ssl.rst` & `collective.easyform-4.1.4/src/collective/easyform/tests/ssl.rst`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testApi.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testApi.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testControlpanel.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testControlpanel.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testCustomScript.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testCustomScript.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testDocTests.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testDocTests.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testEmbedding.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testEmbedding.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testEvents.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testEvents.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testLikert.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testLikert.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testMailer.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testMailer.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testMisc.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testMisc.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testSavedDataSerializer.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testSavedDataSerializer.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testSaver.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testSaver.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testSetup.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testThanksPage.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testThanksPage.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/testValidators.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/testValidators.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,23 +489,23 @@
         proxy.private_key = u"bar"
 
     def test_no_answer(self):
         data = {"verification": ""}
         request = self.LoadRequestForm(**data)
         request.method = "POST"
         form = EasyFormForm(self.ff1, request)()
-        self.assertIn("<div class=\"invalid-feedback\">", form)
+        self.assertIn("class=\"invalid-feedback\"", form)
         self.assertNotIn("Thanks for your input.", form)
 
     def test_wrong(self):
         data = {"verification": "123"}
         request = self.LoadRequestForm(**data)
         request.method = "POST"
         form = EasyFormForm(self.ff1, request)()
-        self.assertIn("<div class=\"invalid-feedback\">", form)
+        self.assertIn("class=\"invalid-feedback\"", form)
         self.assertNotIn("Thanks for your input.", form)
 
 
 class DummyUpload(FileUpload):
     def __init__(self, size, filename):
         self.file = StringIO("x" * size)
         self.file.filename = filename
```

### Comparing `collective.easyform-4.1.3/src/collective/easyform/tests/test_robot.py` & `collective.easyform-4.1.4/src/collective/easyform/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/upgrades/1002.zcml` & `collective.easyform-4.1.4/src/collective/easyform/upgrades/1002.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/upgrades/1007.zcml` & `collective.easyform-4.1.4/src/collective/easyform/upgrades/1007.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/upgrades/1016.zcml` & `collective.easyform-4.1.4/src/collective/easyform/upgrades/1016.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/upgrades/__init__.py` & `collective.easyform-4.1.4/src/collective/easyform/upgrades/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/upgrades/configure.zcml` & `collective.easyform-4.1.4/src/collective/easyform/upgrades/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/upgrades/profiles/1016/actions.xml` & `collective.easyform-4.1.4/src/collective/easyform/upgrades/profiles/1016/actions.xml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/validators.py` & `collective.easyform-4.1.4/src/collective/easyform/validators.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/validators.zcml` & `collective.easyform-4.1.4/src/collective/easyform/validators.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/vocabularies.py` & `collective.easyform-4.1.4/src/collective/easyform/vocabularies.py`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective/easyform/vocabularies.zcml` & `collective.easyform-4.1.4/src/collective/easyform/vocabularies.zcml`

 * *Files identical despite different names*

### Comparing `collective.easyform-4.1.3/src/collective.easyform.egg-info/PKG-INFO` & `collective.easyform-4.1.4/src/collective.easyform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.easyform
-Version: 4.1.3
+Version: 4.1.4
 Summary: Forms for Plone
 Home-page: https://github.com/collective/collective.easyform
 Author: Roman Kozlovskyi
 Author-email: krzroman@gmail.com
 Maintainer: Plone Release Team
 Maintainer-email: releaseteam@plone.org
 License: GPLv2
@@ -33,16 +33,16 @@
 EasyForm - Form Builder for Plone
 =================================
 
 .. image:: https://badge.fury.io/py/collective.easyform.svg
     :target: https://badge.fury.io/py/collective.easyform
     :alt: latest release version badge by Badge Fury
 
-.. image:: https://travis-ci.org/collective/collective.easyform.png?branch=master
-    :target: https://travis-ci.org/collective/collective.easyform
+.. image:: https://github.com/collective/collective.easyform/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/collective/collective.easyform/actions
     :alt: Travis CI status
 
 .. image:: https://coveralls.io/repos/github/collective/collective.easyform/badge.svg?branch=master
     :target: https://coveralls.io/github/collective/collective.easyform?branch=master
     :alt: Coveralls status
 
 
@@ -342,14 +342,22 @@
 - 3.x targets Plone 5.2
 - 4.x targets Plone 6, on Python 3
 
 Changelog
 =========
 
 
+4.1.4 (2023-07-27)
+------------------
+
+- fix folder_contents accessibility from @@saveddata. [ThibautBorn]
+
+- make ReCaptcha fields not required during PloneFormGen migration [ThibautBorn]
+
+
 4.1.3 (2023-05-16)
 ------------------
 
 
 Bug fixes:
 
 - Add upgrade step and profile to update contenttype icon in registry.
```

### Comparing `collective.easyform-4.1.3/src/collective.easyform.egg-info/SOURCES.txt` & `collective.easyform-4.1.4/src/collective.easyform.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -119,33 +119,53 @@
 src/collective/easyform/interfaces/fields.py
 src/collective/easyform/interfaces/layer.py
 src/collective/easyform/interfaces/mailer.py
 src/collective/easyform/interfaces/savedata.py
 src/collective/easyform/interfaces/validators.py
 src/collective/easyform/locales/collective.easyform.pot
 src/collective/easyform/locales/plone.pot
+src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.mo
 src/collective/easyform/locales/de/LC_MESSAGES/collective.easyform.po
+src/collective/easyform/locales/de/LC_MESSAGES/plone.mo
 src/collective/easyform/locales/de/LC_MESSAGES/plone.po
+src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.mo
 src/collective/easyform/locales/en/LC_MESSAGES/collective.easyform.po
+src/collective/easyform/locales/en/LC_MESSAGES/plone.mo
 src/collective/easyform/locales/en/LC_MESSAGES/plone.po
+src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.mo
 src/collective/easyform/locales/es/LC_MESSAGES/collective.easyform.po
+src/collective/easyform/locales/es/LC_MESSAGES/plone.mo
 src/collective/easyform/locales/es/LC_MESSAGES/plone.po
+src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.mo
 src/collective/easyform/locales/eu/LC_MESSAGES/collective.easyform.po
+src/collective/easyform/locales/eu/LC_MESSAGES/plone.mo
 src/collective/easyform/locales/eu/LC_MESSAGES/plone.po
+src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.mo
 src/collective/easyform/locales/fr/LC_MESSAGES/collective.easyform.po
+src/collective/easyform/locales/fr/LC_MESSAGES/plone.mo
 src/collective/easyform/locales/fr/LC_MESSAGES/plone.po
+src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.mo
 src/collective/easyform/locales/it/LC_MESSAGES/collective.easyform.po
+src/collective/easyform/locales/it/LC_MESSAGES/plone.mo
 src/collective/easyform/locales/it/LC_MESSAGES/plone.po
+src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.mo
 src/collective/easyform/locales/ja/LC_MESSAGES/collective.easyform.po
+src/collective/easyform/locales/ja/LC_MESSAGES/plone.mo
 src/collective/easyform/locales/ja/LC_MESSAGES/plone.po
+src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.mo
 src/collective/easyform/locales/nl/LC_MESSAGES/collective.easyform.po
+src/collective/easyform/locales/nl/LC_MESSAGES/plone.mo
 src/collective/easyform/locales/nl/LC_MESSAGES/plone.po
+src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.mo
 src/collective/easyform/locales/pt_BR/LC_MESSAGES/collective.easyform.po
+src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.mo
 src/collective/easyform/locales/pt_BR/LC_MESSAGES/plone.po
+src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.mo
 src/collective/easyform/locales/uk/LC_MESSAGES/collective.easyform.po
+src/collective/easyform/locales/uk/LC_MESSAGES/plone.mo
 src/collective/easyform/locales/uk/LC_MESSAGES/plone.po
 src/collective/easyform/migration/__init__.py
 src/collective/easyform/migration/actions.py
 src/collective/easyform/migration/configure.zcml
 src/collective/easyform/migration/data.py
 src/collective/easyform/migration/fields.py
 src/collective/easyform/migration/pfg.py
```

### Comparing `collective.easyform-4.1.3/src/collective.easyform.egg-info/requires.txt` & `collective.easyform-4.1.4/src/collective.easyform.egg-info/requires.txt`

 * *Files identical despite different names*

