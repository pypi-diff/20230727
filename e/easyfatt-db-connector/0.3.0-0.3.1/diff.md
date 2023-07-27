# Comparing `tmp/easyfatt_db_connector-0.3.0.tar.gz` & `tmp/easyfatt_db_connector-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfatt_db_connector-0.3.0.tar", max compression
+gzip compressed data, was "easyfatt_db_connector-0.3.1.tar", max compression
```

## Comparing `easyfatt_db_connector-0.3.0.tar` & `easyfatt_db_connector-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1092 2023-04-26 12:59:14.893885 easyfatt_db_connector-0.3.0/LICENSE
--rw-r--r--   0        0        0      858 2023-07-19 11:09:34.997601 easyfatt_db_connector-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7472 2023-07-19 11:09:14.187602 easyfatt_db_connector-0.3.0/README.md
--rw-r--r--   0        0        0      159 2023-07-14 08:17:32.167009 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/__init__.py
--rw-r--r--   0        0        0      227 2023-06-26 18:40:35.254373 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/constants.py
--rw-r--r--   0        0        0       52 2023-07-11 18:37:02.948252 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/__init__.py
--rw-r--r--   0        0        0      109 2023-06-26 18:40:35.471873 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/__init__.py
--rw-r--r--   0        0        0     6880 2023-06-27 15:57:18.413422 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_base.py
--rw-r--r--   0        0        0     4320 2023-06-28 23:13:06.501806 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_fdb.py
--rw-r--r--   0        0        0     5088 2023-06-26 18:40:35.478873 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_sqlalchemy.py
--rw-r--r--   0        0        0      674 2023-07-18 15:14:49.864785 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/exceptions.py
--rw-r--r--   0        0        0       55 2023-05-06 15:37:53.636002 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/__init__.py
--rw-r--r--   0        0        0       22 2023-05-07 22:06:24.536129 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/dynamic/__init__.py
--rw-r--r--   0        0        0     1429 2023-05-08 13:00:10.987069 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/dynamic/factory.py
--rw-r--r--   0        0        0      410 2023-05-08 13:05:49.414570 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/static/__init__.py
--rw-r--r--   0        0        0    66243 2023-05-08 13:03:58.168072 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/static/models.py
--rw-r--r--   0        0        0        0 2023-06-26 18:40:35.330373 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/utils/__init__.py
--rw-r--r--   0        0        0      206 2023-06-26 18:40:35.412373 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/utils/decorators.py
--rw-r--r--   0        0        0     4397 2023-06-26 18:40:35.336373 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/utils/downloader.py
--rw-r--r--   0        0        0     1388 2023-07-18 15:39:01.437958 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/__init__.py
--rw-r--r--   0        0        0       68 2023-07-17 14:07:01.710189 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/__init__.py
--rw-r--r--   0        0        0      982 2023-07-17 14:08:21.793688 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/fields.py
--rw-r--r--   0        0        0    12307 2023-07-19 10:55:41.045602 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/mapper.py
--rw-r--r--   0        0        0     2302 2023-07-19 09:25:29.675103 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/README.md
--rw-r--r--   0        0        0     3852 2023-07-19 10:29:25.313603 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/company.py
--rw-r--r--   0        0        0    32696 2023-07-19 10:26:28.461603 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/document.py
--rw-r--r--   0        0        0     5855 2023-07-19 10:37:16.667602 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/product.py
--rw-r--r--   0        0        0     2926 2023-07-15 12:18:32.404214 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/README.md
--rw-r--r--   0        0        0     2908 2023-07-14 10:02:05.284009 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/root.py
--rw-r--r--   0        0        0     1449 2023-07-19 10:37:40.096102 easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/vat_code.py
--rw-r--r--   0        0        0     8224 1970-01-01 00:00:00.000000 easyfatt_db_connector-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-26 12:59:14.893885 easyfatt_db_connector-0.3.1/LICENSE
+-rw-r--r--   0        0        0      858 2023-07-27 15:10:11.700415 easyfatt_db_connector-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     7472 2023-07-19 11:09:14.187602 easyfatt_db_connector-0.3.1/README.md
+-rw-r--r--   0        0        0      159 2023-07-14 08:17:32.167009 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/__init__.py
+-rw-r--r--   0        0        0      227 2023-06-26 18:40:35.254373 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/constants.py
+-rw-r--r--   0        0        0       52 2023-07-11 18:37:02.948252 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/core/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-26 18:40:35.471873 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/core/connection/__init__.py
+-rw-r--r--   0        0        0     6880 2023-06-27 15:57:18.413422 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/core/connection/_base.py
+-rw-r--r--   0        0        0     4320 2023-06-28 23:13:06.501806 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/core/connection/_fdb.py
+-rw-r--r--   0        0        0     5088 2023-06-26 18:40:35.478873 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/core/connection/_sqlalchemy.py
+-rw-r--r--   0        0        0      674 2023-07-18 15:14:49.864785 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/core/exceptions.py
+-rw-r--r--   0        0        0       55 2023-05-06 15:37:53.636002 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/orm/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-07 22:06:24.536129 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/orm/dynamic/__init__.py
+-rw-r--r--   0        0        0     1429 2023-05-08 13:00:10.987069 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/orm/dynamic/factory.py
+-rw-r--r--   0        0        0      410 2023-05-08 13:05:49.414570 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/orm/static/__init__.py
+-rw-r--r--   0        0        0    66243 2023-05-08 13:03:58.168072 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/orm/static/models.py
+-rw-r--r--   0        0        0        0 2023-06-26 18:40:35.330373 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/utils/__init__.py
+-rw-r--r--   0        0        0      206 2023-06-26 18:40:35.412373 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/utils/decorators.py
+-rw-r--r--   0        0        0     4397 2023-06-26 18:40:35.336373 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/utils/downloader.py
+-rw-r--r--   0        0        0     1388 2023-07-18 15:39:01.437958 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-17 14:07:01.710189 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/common/__init__.py
+-rw-r--r--   0        0        0      982 2023-07-17 14:08:21.793688 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/common/fields.py
+-rw-r--r--   0        0        0    12546 2023-07-25 13:05:32.858047 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/common/mapper.py
+-rw-r--r--   0        0        0     2302 2023-07-19 09:25:29.675103 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/common/README.md
+-rw-r--r--   0        0        0     3862 2023-07-24 13:24:05.411648 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/company.py
+-rw-r--r--   0        0        0    33413 2023-07-26 15:05:18.657711 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/document.py
+-rw-r--r--   0        0        0     5865 2023-07-24 13:24:05.412148 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/product.py
+-rw-r--r--   0        0        0     3106 2023-07-26 22:04:57.315223 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/README.md
+-rw-r--r--   0        0        0     2908 2023-07-14 10:02:05.284009 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/root.py
+-rw-r--r--   0        0        0     1459 2023-07-24 13:24:05.412148 easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/vat_code.py
+-rw-r--r--   0        0        0     8224 1970-01-01 00:00:00.000000 easyfatt_db_connector-0.3.1/PKG-INFO
```

### Comparing `easyfatt_db_connector-0.3.0/LICENSE` & `easyfatt_db_connector-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/pyproject.toml` & `easyfatt_db_connector-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easyfatt-db-connector"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Luca Salvarani <lucasalvarani99@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "easyfatt_db_connector", from = "./src/"}]
 repository = "https://github.com/LukeSavefrogs/easyfatt-db-connector/"
 homepage = "https://github.com/LukeSavefrogs/easyfatt-db-connector/"
```

### Comparing `easyfatt_db_connector-0.3.0/README.md` & `easyfatt_db_connector-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_base.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/core/connection/_base.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_fdb.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/core/connection/_fdb.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/connection/_sqlalchemy.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/core/connection/_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/core/exceptions.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/dynamic/factory.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/orm/dynamic/factory.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/orm/static/models.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/orm/static/models.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/utils/downloader.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/__init__.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/fields.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/common/fields.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/mapper.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/common/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,20 @@
             (f"{attr}='{value}'" if type(value) == str else f"{attr}={value}")
             for attr, value in self.__dict__.items()
         ]
         return f"{self.__class__.__name__}({', '.join(attributes)})"
 
     def __repr__(self) -> str:
         return self.__str__()
+    
+    def __hash__(self) -> int:
+        """ Returns a hash of the object. """
+        return hash((type(self),) + tuple(
+            [tuple(value) if type(value) == list else value for value in self.__dict__.values()]
+        ))
 
     @classmethod
     def _get_xml_tag(cls) -> str:
         return cls.__xml_name__ if getattr(cls, "__xml_name__", None) else cls.__name__
 
     @classmethod
     def from_xml_string(cls, string: str, convert_types=True, *, _warn_untracked=True):
```

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/common/README.md` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/common/README.md`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/company.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/company.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 from easyfatt_db_connector.xml.common import XMLMapper
 
-@dataclass(init=False)
+@dataclass(eq=False, init=False)
 class Company(XMLMapper):
     """ Dati dell'azienda che ha originato il file. 
     
     Fonte: https://www.danea.it/software/easyfatt/xml/documenti/#section-126
     """
     __xml_mapping__ = {
         "name": "Name",
```

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/document.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/document.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "P",
     "Q",
     "R",
     "S",
 ]
 
 
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class Payment(XMLMapper):
     """Campi nelle righe di pagamento (elementi `<Payment>`)."""
     __xml_name__ = "Payment"
 
     __xml_mapping__ = {
         "advance": "Advance",
         "amount": "Amount",
@@ -85,15 +85,15 @@
         ```xml
         <Payment>
             <Paid>false</Paid>
         </Payment>
         ```
     """
     
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class DeliveryInfo(XMLMapper):
 	""" Campi nelle righe di consegna (elementi `<Delivery*>`).
     
     I campi "Delivery" si riferiscono all'indirizzo di consegna o spedizione e
 	vanno specificati se tale indirizzo differisce da quello nei precedenti campi "Customer".
 	"""
     
@@ -170,15 +170,15 @@
 		```xml
         <Document>
 		    <DeliveryCountry>...</DeliveryCountry>
         </Document>
 		```
 	"""
 
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class TransportInfo(XMLMapper):
     """ Campi nelle righe di trasporto (elementi `<Transport*>`, `<Shipment>`, ecc). """
 
     __xml_mapping__ = {
         "carrier": "Carrier",
         "reason": "TransportReason",
         "goods_appearance": "GoodsAppearance",
@@ -273,15 +273,15 @@
         ```xml
         <Document>
             <TrackingNumber>...</TrackingNumber>
         </Document>
         ```
     """
 
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class CustomerInfo(XMLMapper):
     """ Campi del'intestatario del documento. 
     
     Va notato che i campi "Customer" (ovvero ... "Cliente") conterranno invece i dati del fornitore per i documenti di fornitura (ordine cliente, arrivo merce, etc.).
     """
 
     __xml_mapping__ = {
@@ -493,15 +493,15 @@
         ```xml
         <Document>
             <CustomerReference>...</CustomerReference>
         </Document>
         ```
     """
 
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class DocumentNotes(XMLMapper):
     """ Campi note/commenti del documento. """
 
     __xml_mapping__ = {
         "internal_comment": "InternalComment",
         "custom1": "CustomField1",
         "custom2": "CustomField2",
@@ -572,15 +572,15 @@
         ```xml
         <Document>
             <FootNotes>...</CustomerCode>
         </Document>
         ```
     """
 
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class WithholdingTax(XMLMapper):
     """ Campi ritenute d'acconto. """
 
     __xml_mapping__ = {
         "rate1": "WithholdingTaxPerc",
         "rate2": "WithholdingTaxPerc2",
         "amount": "WithholdingTaxAmount",
@@ -640,15 +640,15 @@
         <Document>
             <WithholdingTaxNameB>...</WithholdingTaxNameB>
         </Document>
         ```
     """
 
 
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class Contributions(XMLMapper):
     """ Campi contributi previdenziali. """
 
     __xml_mapping__ = {
         "description": "ContribDescription",
         "percentage": "ContribPerc",
         "is_subject_to_withholding_tax": "ContribSubjectToWithholdingTax",
@@ -708,15 +708,15 @@
         <Document>
             <ContribVatCode>...</ContribVatCode>
         </Document>
         ```
     """
 
 
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class DocumentPDFFile(XMLMapper):
     """ Campo `<Pdf>`. """
 
     __xml_name__ = "Pdf"
     __xml_mapping__ = {
         "filename": "@FileName",
         "content": "#TEXT",
@@ -741,15 +741,15 @@
         <Document>
             <Pdf>...</Pdf>
         </Document>
         ```
     """
     
 
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class Document(XMLMapper):
     """ Dati del documento corrente (elementi `<Document>`).
 
     Fonte: https://www.danea.it/software/easyfatt/xml/documenti/#section-124
     """
 
     __xml_mapping__ = {
@@ -859,15 +859,15 @@
         ```xml
         <Document>
             <DocumentType>C</DocumentType>
         </Document>
         ```
     """
 
-    delivery: Optional[DeliveryInfo] = None
+    delivery: DeliveryInfo = field(default_factory=DeliveryInfo)
     """ Informazioni aggiuntive sulla consegna o spedizione.
 
     Example:
         ```xml
         <Document>
             <DeliveryName>...</DeliveryName>
             <DeliveryAddress>...</DeliveryAddress>
@@ -875,15 +875,15 @@
             <DeliveryCity>...</DeliveryCity>
             <DeliveryProvince>...</DeliveryProvince>
             <DeliveryCountry>...</DeliveryCountry>
         </Document>
         ```
     """
 
-    transport: Optional[TransportInfo] = None
+    transport: TransportInfo = field(default_factory=TransportInfo)
     """ Informazioni aggiuntive sul trasporto.
 
     Example:
         ```xml
         <Document>
             <Carrier>...</Carrier>
             <TransportReason>...</TransportReason>
@@ -893,15 +893,15 @@
             <ShipmentTerms>...</ShipmentTerms>
             <TransportedWeight>...</TransportedWeight>
             <TrackingNumber>...</TrackingNumber>
         </Document>
         ```
     """
 
-    customer: Optional[CustomerInfo] = None
+    customer: CustomerInfo = field(default_factory=CustomerInfo)
     """ Informazioni aggiuntive sull'intestatario del documento.
     
     Questo può essere cliente o fornitore a seconda del tipo di documento.
 
     Example:
         ```xml
         <Document>
@@ -911,15 +911,15 @@
             <CustomerAddress>...</CustomerAddress>
             <CustomerVatCode>...</CustomerVatCode>
             <CustomerEmail>...</CustomerEmail>
         </Document>
         ```
     """
 
-    notes: Optional[DocumentNotes] = None
+    notes: DocumentNotes = field(default_factory=DocumentNotes)
     """ Note aggiuntive sul documento.
 
     Example:
         ```xml
         <Document>
             <InternalComment>...</InternalComment>
             <CustomField1>...</CustomField1>
@@ -938,15 +938,15 @@
         ```xml
         <Document>
             <CostDescription>...</CostDescription>
         </Document>
         ```
     """
 
-    cost_vat_code: Optional[VatCode] = None
+    cost_vat_code: VatCode = field(default_factory=VatCode)
     """ Codice IVA spese aggiuntive (deve essere già presente nella tabella "Categorie Iva" dell'applicazione).
     
     Il codice è accompagnato dalle seguenti proprietà, il cui uso è facoltativo:
     - `Perc` (percentuale di tassazione applicata)
     - `Class` (classe: imponibile, non imponibile, intra-ue, extra-ue, esente, escluso, fuori campo, iva non esposta, rev. charge)
     - `Description`: descrizione libera del codice Iva
 
@@ -1031,18 +1031,18 @@
         ```xml
         <Document>
             <TotalSubjectToWithholdingTax>...</TotalSubjectToWithholdingTax>
         </Document>
         ```
     """
 
-    withholding_tax: Optional[WithholdingTax] = None
+    withholding_tax: WithholdingTax = field(default_factory=WithholdingTax)
     """ Informazioni sulla ritenuta d'acconto. """
 
-    contributions: Optional[Contributions] = None
+    contributions: Contributions = field(default_factory=Contributions)
     """ Informazioni sui contributi previdenziali. """
 
     # ----------------------------------
 
     delayed_vat: Optional[bool] = None
     """ Iva ad esigibilità differita [true|false].
 
@@ -1151,15 +1151,15 @@
         ```xml
         <Document>
             <DocReference>...</DocReference>
         </Document>
         ```
     """
 
-    pdf: Optional[DocumentPDFFile] = None
+    pdf: DocumentPDFFile = field(default_factory=DocumentPDFFile)
     """ Documento in formato Pdf condificato Base64.
 
     Example:
         ```xml
         <Document>
             <Pdf>...</Pdf>
         </Document>
@@ -1308,7 +1308,18 @@
     document = Document.from_xml_string(xml)
     print(f"Example of <Document> as object: {document}\n")
     print(f"Document number is             : {document.number}\n")
     print(f"Document VatCode is            : {document.date}")
     print(f"Document VatCode percentage is : {document.type}")
     print(f"Document first product is      : {document.rows[0].description}")
     print(f"Document first payment is      : {document.payments[0].amount}\n")
+
+    print(f"Same object              : {document == document}")
+    unique_documents = set([document, document])
+    print(f"Count of unique documents: {len(unique_documents)}")
+
+    document2 = Document.from_xml_string(xml)
+    document.number = "TEST2"
+
+    print(f"Same object              : {document == document2}")
+    unique_documents = set([document, document, document2])
+    print(f"Count of unique documents: {len(unique_documents)}")
```

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/product.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 import lxml.etree as ET
 
 from easyfatt_db_connector.xml.common import Field, XMLMapper
 from easyfatt_db_connector.xml.vat_code import VatCode
 
 
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class Product(XMLMapper):
     """ Campi nelle righe del documento (elementi <Row>). """
     __xml_name__ = "Row"
 
     __xml_mapping__ = {
         "code": "Code",
         "supplier_code": "SupplierCode",
```

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/README.md` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 # Lettura file `.DefXml`
 
 Questo modulo permette di leggere il tracciato XML dei **documenti esportati da Easyfatt** e trasformarlo in una serie di **oggetti Python**.
 
+> Dalla documentazione ufficiale:
+>
+> "_Questa funzione si applica ai seguenti tipi di documenti:_
+>
+> - _Fattura_
+> - _Fattura pro-forma_
+> - _Parcella_
+> - _Avviso di parcella_
+> - _Vendita al banco_
+> - _Ordine cliente_
+> - _Documento di trasporto_
+> - _Ordine fornitore_
+> - _Rapporto d'intervento_
+> - _Nota di credito_
+> - _Nota di debito_
+> - _Preventivo_
+> - _Ricevuta fiscale_
+> - _Preventivo fornitore_
+> - _Arrivi merce fornitore_"
+
 Ad esempio, il seguente codice leggerà il file `fatture.DefXml` e restituirà i dati desiderati riguardo i documenti definiti all'interno:
 
 ```python
 from easyfatt_db_connector import read_xml
 
 xml_file = read_xml("fatture.DefXml")
 
@@ -31,8 +51,7 @@
 > - In **esportazione da Easyfatt**, se un campo ha un valore nullo (stringa vuota, oppure numero uguale a zero), il relativo tag viene omesso dal tracciato.
 > - In **importazione**, se Easyfatt riscontra un tag con contenuto nullo (stringa vuota, oppure numero uguale a zero), imposterà tale valore nel relativo campo; se, invece, il tag viene omesso del tutto, Easyfatt imposterà il valore di default per quel contesto (ad esempio, se in un tracciato è assente il tag <Date>, il documento importato avrà la data del giorno e non la data nulla, se invece è assente il tag <Number> Easyfatt imposterà l'incremento automatico del numero del documento).
 > - Il file XML deve essere codificato in **UNICODE UTF-8** che prevede importanti regole nella codifica delle stringhe racchiuse tra tag
 
 ## Limitazioni
 
 - Al momento della scrittura di questo documento, è possibile solamente **leggere** i file XML esportati da Easyfatt, non è possibile crearli o modificarli.
-- Non sono stati implementati tutti i tag presenti nel tracciato XML, quindi si potrebbero verificare dei `WARNING` durante la lettura del file. Questi `WARNING` non influiscono sul corretto funzionamento del programma, ma è consigliato controllare che i dati letti siano corretti.
```

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/root.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/root.py`

 * *Files identical despite different names*

### Comparing `easyfatt_db_connector-0.3.0/src/easyfatt_db_connector/xml/vat_code.py` & `easyfatt_db_connector-0.3.1/src/easyfatt_db_connector/xml/vat_code.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 
 import lxml.etree as ET
 from easyfatt_db_connector.xml.common import XMLMapper
 
 
-@dataclass(init=False, repr=False)
+@dataclass(eq=False, init=False, repr=False)
 class VatCode(XMLMapper):
     """ Informazioni sull'IVA applicata al prodotto. """
     __xml_mapping__ = {
         "code": "#TEXT",
         "description": "@Description",
         "percentage": "@Perc",
         "vat_class": "@Class",
```

### Comparing `easyfatt_db_connector-0.3.0/PKG-INFO` & `easyfatt_db_connector-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyfatt-db-connector
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Home-page: https://github.com/LukeSavefrogs/easyfatt-db-connector/
 License: MIT
 Author: Luca Salvarani
 Author-email: lucasalvarani99@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

