# Comparing `tmp/openworld-sdk-python-fraudprevention-0.7.0.tar.gz` & `tmp/openworld-sdk-python-fraudprevention-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openworld-sdk-python-fraudprevention-0.7.0.tar", last modified: Tue May 23 17:19:46 2023, max compression
+gzip compressed data, was "openworld-sdk-python-fraudprevention-0.8.0.tar", last modified: Tue May 30 14:40:27 2023, max compression
```

## Comparing `openworld-sdk-python-fraudprevention-0.7.0.tar` & `openworld-sdk-python-fraudprevention-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:19:46.015706 openworld-sdk-python-fraudprevention-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-23 17:19:46.015706 openworld-sdk-python-fraudprevention-0.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:19:46.015706 openworld-sdk-python-fraudprevention-0.7.0/openworld/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:19:46.015706 openworld-sdk-python-fraudprevention-0.7.0/openworld/sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:19:46.015706 openworld-sdk-python-fraudprevention-0.7.0/openworld/sdk/fraudprevention/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-23 17:19:39.000000 openworld-sdk-python-fraudprevention-0.7.0/openworld/sdk/fraudprevention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-23 17:19:39.000000 openworld-sdk-python-fraudprevention-0.7.0/openworld/sdk/fraudprevention/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    70872 2023-05-23 17:19:39.000000 openworld-sdk-python-fraudprevention-0.7.0/openworld/sdk/fraudprevention/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:19:46.015706 openworld-sdk-python-fraudprevention-0.7.0/openworld_sdk_python_fraudprevention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-23 17:19:46.000000 openworld-sdk-python-fraudprevention-0.7.0/openworld_sdk_python_fraudprevention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-23 17:19:46.000000 openworld-sdk-python-fraudprevention-0.7.0/openworld_sdk_python_fraudprevention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:19:46.000000 openworld-sdk-python-fraudprevention-0.7.0/openworld_sdk_python_fraudprevention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-23 17:19:46.000000 openworld-sdk-python-fraudprevention-0.7.0/openworld_sdk_python_fraudprevention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 17:19:46.000000 openworld-sdk-python-fraudprevention-0.7.0/openworld_sdk_python_fraudprevention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:19:46.015706 openworld-sdk-python-fraudprevention-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-23 17:19:31.000000 openworld-sdk-python-fraudprevention-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/openworld/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-30 14:40:21.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-30 14:40:21.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68115 2023-05-30 14:40:21.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-30 14:40:27.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-30 14:40:27.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:40:27.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-30 14:40:27.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 14:40:27.000000 openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:40:27.644522 openworld-sdk-python-fraudprevention-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-30 14:40:05.000000 openworld-sdk-python-fraudprevention-0.8.0/setup.py
```

### Comparing `openworld-sdk-python-fraudprevention-0.7.0/PKG-INFO` & `openworld-sdk-python-fraudprevention-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudprevention
-Version: 0.7.0
+Version: 0.8.0
 Summary: Open World Fraud Prevention SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-fraudprevention-0.7.0/openworld/sdk/fraudprevention/__init__.py` & `openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-fraudprevention-0.7.0/openworld/sdk/fraudprevention/client.py` & `openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         r"""Fraud Prevention API Client.
 
         Args:
             client_config(ClientConfig): SDK Client Configurations Holder.
         """
         python_version = platform.python_version()
         os_name, os_version, *_ = platform.platform().split('-')
-        sdk_metadata = f'open-world-sdk-python-fraudprevention/0.7.0'
+        sdk_metadata = f'open-world-sdk-python-fraudprevention/0.8.0'
 
         self.__api_client = ApiClient(client_config, _OpenWorldAuthClient)
 
         self.__user_agent = f'{sdk_metadata} (Python {python_version}; {os_name} {os_version})'
 
     def screen(self, transaction_id: UUID = uuid4(), body: OrderPurchaseScreenRequest = None) -> Union[OrderPurchaseScreenResponse, ExtendedError, Error]:
         r"""The Order Purchase API gives a Fraud recommendation for a transaction. A recommendation can be Accept, Reject, or Review. A transaction is marked as Review whenever there are insufficient signals to recommend Accept or Reject. These incidents are manually reviewed, and a corrected recommendation is made asynchronously.
```

### Comparing `openworld-sdk-python-fraudprevention-0.7.0/openworld/sdk/fraudprevention/model.py` & `openworld-sdk-python-fraudprevention-0.8.0/openworld/sdk/fraudprevention/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,15 +36,19 @@
     ORDER_UPDATE: Any = 'ORDER_UPDATE'
     CHARGEBACK_FEEDBACK: Any = 'CHARGEBACK_FEEDBACK'
     INSULT_FEEDBACK: Any = 'INSULT_FEEDBACK'
     REFUND_UPDATE: Any = 'REFUND_UPDATE'
     PAYMENT_UPDATE: Any = 'PAYMENT_UPDATE'
 
 
-class CancellationReason(BaseModel, smart_union=True, extra=Extra.forbid):
+class CancellationReason(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model CancellationReason: Reason of order update cancellation.
     Attributes:
         primary_reason_code(Optional[constr(max_length=200)], optional): Primary cancellation reason code.
         sub_reason_code(Optional[constr(max_length=200)], optional): Substitute cancellation reason code.
         primary_reason_description(constr(max_length=200)): Primary cancellation reason code. Required if `order_status = CANCELLED`.
         sub_reason_description(Optional[constr(max_length=200)], optional): Substitute cancellation reason description.
 
@@ -76,15 +80,19 @@
         NON_FRAUD(Any): --
 
     """
     FRAUD: Any = 'FRAUD'
     NON_FRAUD: Any = 'NON_FRAUD'
 
 
-class ChargebackDetail(BaseModel, smart_union=True, extra=Extra.forbid):
+class ChargebackDetail(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model ChargebackDetail: Details related to the chargeback.
     Attributes:
         chargeback_reason(ChargebackReason): Reason for chargeback which can be `Fraud` or `Non Fraud`.
         chargeback_amount(float): Chargeback amount received by the partner.
         currency_code(constr(regex=r'^[A-Z]{3}$', max_length=200)): The 3-letter currency code defined in ISO 4217. https://www.currency-iso.org/dam/downloads/lists/list_one.xml.
         bank_reason_code(Optional[constr(max_length=200)], optional): Unique code provided by the acquiring bank for the category of fraud.
         chargeback_reported_timestamp(Optional[datetime], optional): Date and time when the chargeback was reported to the partner, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
@@ -108,15 +116,19 @@
     """
     chargeback_reported_timestamp: Optional[datetime] = None
     """
     Date and time when the chargeback was reported to the partner, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
     """
 
 
-class InsultDetail(BaseModel, smart_union=True, extra=Extra.forbid):
+class InsultDetail(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model InsultDetail: Details related to the insult.
     Attributes:
         insult_reported_timestamp(Optional[datetime], optional): Date and time when the insult was reported to the partner, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
 
     """
     insult_reported_timestamp: Optional[datetime] = None
     """
@@ -154,15 +166,19 @@
 
     """
     ACCEPT: Any = 'ACCEPT'
     REVIEW: Any = 'REVIEW'
     REJECT: Any = 'REJECT'
 
 
-class ErrorDetail(BaseModel, smart_union=True, extra=Extra.forbid):
+class ErrorDetail(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model ErrorDetail: Error details in case of any errors.
     Attributes:
         code(Optional[int], optional): --
         message(Optional[constr(max_length=200)], optional): Description of the error. Clients may choose to use the description field to display to end clients.
         detailed_message(Optional[constr(max_length=500)], optional): Detailed description of the error.
 
     """
@@ -173,15 +189,19 @@
     """
     detailed_message: Optional[constr(max_length=500)] = None
     """
     Detailed description of the error.
     """
 
 
-class Error(BaseModel, smart_union=True, extra=Extra.forbid):
+class Error(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Error: The object used the describe an error, containing both human-readable and in a machine-readable information.
     Attributes:
         type(AnyUrl): A URI reference, compliant with the standard EG error type format, which identifies the error type. It provides a machine-readable identifier for the error type. The error type will be aligned with the HTTP status code of the response. The URI can either be absolute or relative to the API's base URI. When dereferenced, it can also provide human-readable documentation for the error type.
         detail(str): A human-readable explanation of the error, specific to this error occurrence.
 
     """
     type: AnyUrl = Field(..., example='https://apis.expediagroup.com/errors/common/invalid-argument')
@@ -213,15 +233,19 @@
     """
     HEADER: Any = 'HEADER'
     PATH: Any = 'PATH'
     QUERY: Any = 'QUERY'
     BODY: Any = 'BODY'
 
 
-class ErrorCause(BaseModel, smart_union=True, extra=Extra.forbid):
+class ErrorCause(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model ErrorCause: The object used to describe a cause for an error, containing both human-readable and in a machine-readable information.
     Attributes:
         type(AnyUrl): A URI reference, compliant with the standard EG error type format, which identifies the cause type. It provides a machine-readable identifier for the cause type. The cause type will be aligned with the error type. The URI can either be absolute or relative to the API's base URI. When dereferenced, it provides human-readable documentation for the cause type.
         detail(str): A human-readable explanation of the cause, specific to this cause occurrence.
         location(Optional[Location], optional): The location of the element in the request that identifies this specific cause. When specified, the `name` will be specified and when applicable, the `value` as well. Can be one of: * `HEADER` - When an error has been identified in one of the request headers. * `PATH` - When an error has been identified in one of the path parameters. * `QUERY` - When an error has been identified in one of the query parameters. * `BODY` - When an error has been identified in the request body.
         name(Optional[str], optional): The name of the element for this cause. When specified, the `location` will be specified and when applicable, the `value` as well. This name is a function of the value of the `location` property:   * When the `location` is set to `HEADER`, this will be the name of the request header (e.g. `Content-Type`).   * When the `location` is set to `PATH`, this will be the name of the path parameter (e.g. in a path defined as `/users/{user_id}`, the value would be `user_id`).   * When the `location` is set to `QUERY`, this will be the name of the query string parameter (e.g. `offset`).   * When the `location` is set to `BODY`, this will one of the field names specified in the body of the request.     * For a top level field, it should only be set to the field name (e.g. `firstName`).     * For a field in a nested object, it may contain the path to reach the field (e.g. `address.city`).     * For a field in an object part of collection, it may contain the index in the collection (e.g. `permissions[0].name`).
         value(Optional[str], optional): A string representation of the erroneous value of the element identified in `name`, perceived to be the cause of the error. When specified, the `location` and `name` should be specified as well. This value may be omitted in cases where it cannot be provided (e.g. missing require field), or the erroneous value cannot be represented as a string.
@@ -262,15 +286,19 @@
     value: Optional[str] = Field(None, example='NotANumber')
     """
     A string representation of the erroneous value of the element identified in `name`, perceived to be the cause of the error. When specified, the `location` and `name` should be specified as well. This value may be omitted in cases where it cannot be provided (e.g. missing require field), or the erroneous value cannot be represented as a string.
 
     """
 
 
-class SiteInfo(BaseModel, smart_union=True, extra=Extra.forbid):
+class SiteInfo(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model SiteInfo
     Attributes:
         country_code(constr(regex=r'^[A-Z]{3}$')): The alpha-3 ISO code that represents a country name.
         agent_assisted(bool): Identifies if an agent assisted in booking travel for the customer. `False` if the order was directly booked by customer.
 
     """
     country_code: constr(regex=r'^[A-Z]{3}$') = Field(..., example='USA')
@@ -279,15 +307,19 @@
     """
     agent_assisted: bool = None
     """
     Identifies if an agent assisted in booking travel for the customer. `False` if the order was directly booked by customer.
     """
 
 
-class DeviceDetails(BaseModel, smart_union=True, extra=Extra.forbid):
+class DeviceDetails(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model DeviceDetails
     Attributes:
         source(Optional[constr(max_length=50)], optional): Source of the device_box. Default value is `TrustWidget`.
         device_box(constr(max_length=16000)): Device related information retrieved from TrustWidget.
         ip_address(Optional[constr(regex=r'^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$|^(?:[A-F0-9]{1,4}:){7}[A-F0-9]{1,4}$')], optional): IP address of the device used for booking.
 
     """
@@ -365,15 +397,19 @@
         WORK(Any): --
 
     """
     HOME: Any = 'HOME'
     WORK: Any = 'WORK'
 
 
-class Address(BaseModel, smart_union=True, extra=Extra.forbid):
+class Address(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Address
     Attributes:
         address_type(Optional[AddressType], optional): --
         address_line1(constr(max_length=200)): Address line 1 of the address provided.
         address_line2(Optional[constr(max_length=200)], optional): Address line 2 of the address provided.
         city(constr(max_length=200)): City of the address provided.
         state(constr(regex=r'^[A-Z]{2}$')): The two-characters ISO code for the state or province of the address.
@@ -417,15 +453,19 @@
         AGENCY(Any): --
 
     """
     MERCHANT: Any = 'MERCHANT'
     AGENCY: Any = 'AGENCY'
 
 
-class TravelersReference(BaseModel, smart_union=True, extra=Extra.forbid):
+class TravelersReference(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model TravelersReference
     Attributes:
         __root__(constr(max_length=50)): --
 
     """
     __root__: constr(max_length=50) = None
 
@@ -441,15 +481,19 @@
 
     """
     ROUNDTRIP: Any = 'ROUNDTRIP'
     ONEWAY: Any = 'ONEWAY'
     MULTIPLE_DESTINATION: Any = 'MULTIPLE_DESTINATION'
 
 
-class AirSegment(BaseModel, smart_union=True, extra=Extra.forbid):
+class AirSegment(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model AirSegment
     Attributes:
         airline_code(constr(max_length=10)): Airline code of the trip segment
         departure_airport_code(constr(max_length=10)): Departure airport of the trip segment
         arrival_airport_code(constr(max_length=10)): Arrival airport of the trip segment
         departure_time(Optional[datetime], optional): Local date and time of departure from departure location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
         arrival_time(Optional[datetime], optional): Local date and time of arrival to destination location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
@@ -473,15 +517,19 @@
     """
     arrival_time: Optional[datetime] = None
     """
     Local date and time of arrival to destination location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
     """
 
 
-class PaymentThreeDSCriteria(BaseModel, smart_union=True, extra=Extra.forbid):
+class PaymentThreeDSCriteria(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model PaymentThreeDSCriteria: Payment 3DS criteria attributes.
     Attributes:
         probable_flag(Optional[bool], optional): This is a flag passed that indicates that this transaction could potentially go through 3DS.
         transaction_model(Optional[constr(max_length=200)], optional): Model used to process payment transaction.
 
     """
     probable_flag: Optional[bool] = None
@@ -556,15 +604,19 @@
 
     """
     CREDIT_CARD: Any = 'CREDIT_CARD'
     PAYPAL: Any = 'PAYPAL'
     POINTS: Any = 'POINTS'
 
 
-class Name(BaseModel, smart_union=True, extra=Extra.forbid):
+class Name(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Name: Group of attributes intended to hold information about a customer or traveler's name for the order.
     Attributes:
         last_name(constr(max_length=200)): Surname, or last name, of the person.
         first_name(constr(max_length=200)): Given, or first name, of the person.
         middle_name(Optional[constr(max_length=200)], optional): Middle name of the person.
         title(Optional[constr(max_length=200)], optional): Title of the person for name (e.g. Mr., Ms. etc).
         suffix(Optional[constr(max_length=50)], optional): Generational designations (e.g. Sr, Jr, III) or values that indicate the individual holds a position, educational degree, accreditation, office, or honor (e.g. PhD, CCNA, OBE).
@@ -627,27 +679,35 @@
 
     """
     MOBILE: Any = 'MOBILE'
     LANDLINE: Any = 'LANDLINE'
     VOIP: Any = 'VOIP'
 
 
-class Email(BaseModel, smart_union=True, extra=Extra.forbid):
+class Email(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Email: Group of attributes intended to hold information about email address associated with the transaction.
     Attributes:
         email_address(Optional[EmailStr], optional): Full email address including the alias, @ symbol, domain, and root domain.
 
     """
     email_address: Optional[EmailStr] = None
     """
     Full email address including the alias, @ symbol, domain, and root domain.
     """
 
 
-class Amount(BaseModel, smart_union=True, extra=Extra.forbid):
+class Amount(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Amount
     Attributes:
         value(float): The amount required in payment for the product/order in local currency.
         currency_code(constr(regex=r'^[A-Z]{3}$', max_length=3)): The ISO  alpha-3 country code for the amount currency.
 
     """
     value: float = None
@@ -667,28 +727,154 @@
     Attributes:
         application_json(Any): --
 
     """
     application_json: Any = 'application/json'
 
 
-class OrderPurchaseScreenResponse(BaseModel, smart_union=True, extra=Extra.forbid):
+class OrderPurchaseUpdateRequestGeneric(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model OrderPurchaseUpdateRequest
+    Attributes:
+        type(UpdateType): --
+        risk_id(constr(max_length=200)): The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
+
+    """
+    type: UpdateType = None
+    risk_id: constr(max_length=200) = Field(..., example='123456789')
+    """
+    The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
+    """
+
+
+class OrderUpdate(
+    OrderPurchaseUpdateRequestGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model OrderUpdate
+    Attributes:
+        order_status(Status): --
+        cancellation_reason(Optional[CancellationReason], optional): --
+        type(Literal['ORDER_UPDATE']): --
+
+    """
+    order_status: Status = None
+    cancellation_reason: Optional[CancellationReason] = None
+    type: Literal['ORDER_UPDATE'] = 'ORDER_UPDATE'
+
+
+class ChargebackFeedback(
+    OrderPurchaseUpdateRequestGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model ChargebackFeedback
+    Attributes:
+        chargeback_detail(Optional[ChargebackDetail], optional): --
+        type(Literal['CHARGEBACK_FEEDBACK']): --
+
+    """
+    chargeback_detail: Optional[ChargebackDetail] = None
+    type: Literal['CHARGEBACK_FEEDBACK'] = 'CHARGEBACK_FEEDBACK'
+
+
+class InsultFeedback(
+    OrderPurchaseUpdateRequestGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model InsultFeedback
+    Attributes:
+        insult_detail(Optional[InsultDetail], optional): --
+        type(Literal['INSULT_FEEDBACK']): --
+
+    """
+    insult_detail: Optional[InsultDetail] = None
+    type: Literal['INSULT_FEEDBACK'] = 'INSULT_FEEDBACK'
+
+
+class RefundUpdate(
+    OrderPurchaseUpdateRequestGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model RefundUpdate
+    Attributes:
+        acquirer_reference_number(constr(max_length=200)): A unique number that tags a credit or debit card transaction when it goes from the merchant's bank through to the cardholder's bank.
+        refund_deposit_timestamp(datetime): Date and time when the refund was deposited to the original form of payment.
+        refund_settlement_timestamp(datetime): Date and time when the 3rd party payment processor confirmed that a previously submitted payment refund has settled at the participating financial institutions.
+        settlement_id(constr(max_length=200)): Unique settlement identifier generated for a previously submitted payment refund.
+        refund_amount(Amount): --
+        type(Literal['REFUND_UPDATE']): --
+
+    """
+    acquirer_reference_number: constr(max_length=200) = None
+    """
+    A unique number that tags a credit or debit card transaction when it goes from the merchant's bank through to the cardholder's bank.
+    """
+    refund_deposit_timestamp: datetime = None
+    """
+    Date and time when the refund was deposited to the original form of payment.
+    """
+    refund_settlement_timestamp: datetime = None
+    """
+    Date and time when the 3rd party payment processor confirmed that a previously submitted payment refund has settled at the participating financial institutions.
+    """
+    settlement_id: constr(max_length=200) = None
+    """
+    Unique settlement identifier generated for a previously submitted payment refund.
+    """
+    refund_amount: Amount = None
+    type: Literal['REFUND_UPDATE'] = 'REFUND_UPDATE'
+
+
+class PaymentUpdate(
+    OrderPurchaseUpdateRequestGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model PaymentUpdate
+    Attributes:
+        merchant_order_code(constr(max_length=200)): Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
+        type(Literal['PAYMENT_UPDATE']): --
+
+    """
+    merchant_order_code: constr(max_length=200) = None
+    """
+    Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
+    """
+    type: Literal['PAYMENT_UPDATE'] = 'PAYMENT_UPDATE'
+
+
+class OrderPurchaseScreenResponse(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model OrderPurchaseScreenResponse
     Attributes:
         risk_id(Optional[constr(max_length=200)], optional): --
         decision(Optional[FraudDecision], optional): --
         error_detail(Optional[ErrorDetail], optional): --
 
     """
     risk_id: Optional[constr(max_length=200)] = Field(None, example='1234567')
     decision: Optional[FraudDecision] = None
     error_detail: Optional[ErrorDetail] = None
 
 
-class ExtendedError(BaseModel, smart_union=True, extra=Extra.forbid):
+class ExtendedError(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model ExtendedError: The object used the describe an error, containing both human-readable and in a machine-readable information.
     Attributes:
         type(AnyUrl): A URI reference, compliant with the standard EG error type format, which identifies the error type. It provides a machine-readable identifier for the error type. The error type will be aligned with the HTTP status code of the response. The URI can either be absolute or relative to the API's base URI. When dereferenced, it can also provide human-readable documentation for the error type.
         detail(str): A human-readable explanation of the error, specific to this error occurrence.
         causes(Optional[List[ErrorCause]], optional): An array of cause objects, that identify the specific causes of the error.
 
     """
@@ -703,15 +889,223 @@
     """
     causes: Optional[List[ErrorCause]] = None
     """
     An array of cause objects, that identify the specific causes of the error.
     """
 
 
-class PaymentOutcome(BaseModel, smart_union=True, extra=Extra.forbid):
+class TravelProductGeneric(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model TravelProduct
+    Attributes:
+        price(Amount): --
+        type(constr(max_length=40)): Type of product advertised on the website.
+        inventory_type(constr(max_length=30)): Type of inventory.
+        inventory_source(InventorySource): Identifies the business model through which the supply is being sold. Merchant/Agency.
+        travelers_references(List[constr(max_length=50)]): List of travelerGuids who are part of the traveling party on the order for the product.
+
+    """
+    price: Amount = None
+    type: constr(max_length=40) = None
+    """
+    Type of product advertised on the website.
+    """
+    inventory_type: constr(max_length=30) = None
+    """
+    Type of inventory.
+    """
+    inventory_source: InventorySource = None
+    """
+    Identifies the business model through which the supply is being sold. Merchant/Agency.
+    """
+    travelers_references: List[constr(max_length=50)] = Field(..., maxItems=40, minItems=1)
+    """
+    List of travelerGuids who are part of the traveling party on the order for the product.
+    """
+
+
+class Air(
+    TravelProductGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Air
+    Attributes:
+        departure_time(datetime): Local date and time of departure from original departure location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        arrival_time(datetime): Local date and time of arrival to final destination location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        air_segments(List[AirSegment]): Additional airline and flight details for each of the trip segments.
+        flight_type(Optional[FlightType], optional): Identifies the type of air trip based on the air destinations.
+        passenger_name_record(Optional[constr(max_length=100)], optional): Airline booking confirmation code for the trip.
+        global_distribution_system_type(Optional[constr(max_length=100)], optional): Associated with Passenger Name Record (PNR).
+        type(Literal['Air']): Type of product advertised on the website.
+
+    """
+    departure_time: datetime = None
+    """
+    Local date and time of departure from original departure location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+    """
+    arrival_time: datetime = None
+    """
+    Local date and time of arrival to final destination location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+    """
+    air_segments: List[AirSegment] = Field(..., maxItems=30, minItems=1)
+    """
+    Additional airline and flight details for each of the trip segments.
+    """
+    flight_type: Optional[FlightType] = None
+    """
+    Identifies the type of air trip based on the air destinations.
+    """
+    passenger_name_record: Optional[constr(max_length=100)] = None
+    """
+    Airline booking confirmation code for the trip.
+    """
+    global_distribution_system_type: Optional[constr(max_length=100)] = None
+    """
+    Associated with Passenger Name Record (PNR).
+    """
+    type: Literal['Air'] = 'Air'
+    """
+    Type of product advertised on the website.
+    """
+
+
+class Cruise(
+    TravelProductGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Cruise
+    Attributes:
+        departure_time(datetime): Local date and time of departure from original departure location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        arrival_time(datetime): Local date and time of arrival from original arrival location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        embarkation_port(constr(max_length=200)): Location from where cruise will depart.
+        disembarkation_port(constr(max_length=200)): The cruise's final destination.
+        ship_name(constr(max_length=200)): Name of the cruise ship.
+        type(Literal['Cruise']): Type of product advertised on the website.
+
+    """
+    departure_time: datetime = None
+    """
+    Local date and time of departure from original departure location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+    """
+    arrival_time: datetime = None
+    """
+    Local date and time of arrival from original arrival location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+    """
+    embarkation_port: constr(max_length=200) = None
+    """
+    Location from where cruise will depart.
+    """
+    disembarkation_port: constr(max_length=200) = None
+    """
+    The cruise's final destination.
+    """
+    ship_name: constr(max_length=200) = None
+    """
+    Name of the cruise ship.
+    """
+    type: Literal['Cruise'] = 'Cruise'
+    """
+    Type of product advertised on the website.
+    """
+
+
+class Car(
+    TravelProductGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Car
+    Attributes:
+        pick_up_location(constr(max_length=200)): Location where the automobile will be picked up.
+        drop_off_location(constr(max_length=200)): Location at which the automobile will be returned.
+        pickup_time(datetime): Local date and time the automobile will be picked-up, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        return_time(datetime): Local date and time the automobile will be returned, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        type(Literal['Car']): Type of product advertised on the website.
+
+    """
+    pick_up_location: constr(max_length=200) = None
+    """
+    Location where the automobile will be picked up.
+    """
+    drop_off_location: constr(max_length=200) = None
+    """
+    Location at which the automobile will be returned.
+    """
+    pickup_time: datetime = None
+    """
+    Local date and time the automobile will be picked-up, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+    """
+    return_time: datetime = None
+    """
+    Local date and time the automobile will be returned, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+    """
+    type: Literal['Car'] = 'Car'
+    """
+    Type of product advertised on the website.
+    """
+
+
+class Hotel(
+    TravelProductGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Hotel
+    Attributes:
+        hotel_id(constr(max_length=200)): Unique hotel identifier assigned by the partner.
+        price_withheld(Optional[bool], optional): Identifies if the product price was withheld from the customer during the booking process.
+        hotel_name(constr(max_length=200)): Name of the hotel.
+        room_count(Optional[int], optional): Total number of rooms booked within the hotel product collection.
+        address(Address): --
+        checkin_time(datetime): Local date and time of the hotel check-in, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        checkout_time(datetime): Local date and time of the hotel check-out, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        type(Literal['Hotel']): Type of product advertised on the website.
+
+    """
+    hotel_id: constr(max_length=200) = Field(..., example='8883333999221')
+    """
+    Unique hotel identifier assigned by the partner.
+    """
+    price_withheld: Optional[bool] = None
+    """
+    Identifies if the product price was withheld from the customer during the booking process.
+    """
+    hotel_name: constr(max_length=200) = Field(..., example='Hotel Expedia')
+    """
+    Name of the hotel.
+    """
+    room_count: Optional[int] = None
+    """
+    Total number of rooms booked within the hotel product collection.
+    """
+    address: Address = None
+    checkin_time: datetime = None
+    """
+    Local date and time of the hotel check-in, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+    """
+    checkout_time: datetime = None
+    """
+    Local date and time of the hotel check-out, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+    """
+    type: Literal['Hotel'] = 'Hotel'
+    """
+    Type of product advertised on the website.
+    """
+
+
+class PaymentOutcome(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model PaymentOutcome
     Attributes:
         status(Optional[PaymentStatus], optional): --
         code(Optional[constr(max_length=200)], optional): A mnemonic code for the payment processing.
         description(Optional[constr(max_length=200)], optional): A short description providing additional explanation regarding the mnemonic code.
 
     """
@@ -722,15 +1116,35 @@
     """
     description: Optional[constr(max_length=200)] = None
     """
     A short description providing additional explanation regarding the mnemonic code.
     """
 
 
-class Telephone(BaseModel, smart_union=True, extra=Extra.forbid):
+class Insurance(
+    TravelProductGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Insurance
+    Attributes:
+        type(Literal['Insurance']): Type of product advertised on the website.
+
+    """
+    type: Literal['Insurance'] = 'Insurance'
+    """
+    Type of product advertised on the website.
+    """
+
+
+class Telephone(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Telephone: Group of attributes intended to hold information about phone number associated with the transaction.  A user can have one to many phone numbers (home, work, mobile, etc.).
     Attributes:
         type(Optional[TelephoneType], optional): --
         platform_type(Optional[TelephonePlatformType], optional): --
         country_access_code(constr(regex=r'^[0-9]{1,3}$', max_length=3)): Numeric digit between 1 to 3 characters used to represent the country code for international dialing.  Does not include symbols, spaces, or leading zeros.
         area_code(constr(regex=r'^[0-9]{1,20}$', max_length=20)): A number prefixed to an individual telephone number: used in making long-distance calls.  Does not include symbols, spaces, or leading zeros.
         phone_number(constr(regex=r'^[0-9]{1,50}$', max_length=50)): A number that is dialed on a telephone, without the country or area codes, to reach a particular person, business, etc.  Does not include symbols, spaces, or leading zeros.
@@ -773,15 +1187,19 @@
     """
     verified_flag: Optional[bool] = None
     """
     Flag indicating whether user passed validation of possession of their phone number via a text or voice multi factor authentication challenge.
     """
 
 
-class CustomerAccount(BaseModel, smart_union=True, extra=Extra.forbid):
+class CustomerAccount(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model CustomerAccount
     Attributes:
         user_id(Optional[str], optional): Unique identifier assigned to the account owner by the partner. `user_id` is specific to the partner namespace
         account_type(AccountType): Identifies if the customer account is known to the client. Possible values are:  -`GUEST` - Applicable if the partner maintains record to distinguish whether the transaction was booked via a guest account.  -`STANDARD` - Default account type.
         name(Name): --
         email_address(EmailStr): Email address for the account owner.
         telephones(Optional[List[Telephone]], optional): --
@@ -811,15 +1229,19 @@
     address: Optional[Address] = None
     registered_time: Optional[datetime] = None
     """
     The local date and time that the customer first registered on the client site, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
     """
 
 
-class Traveler(BaseModel, smart_union=True, extra=Extra.forbid):
+class Traveler(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Traveler
     Attributes:
         traveler_name(Name): --
         email_address(Optional[EmailStr], optional): Email address associated with the traveler as supplied by the partner system.
         telephones(Optional[List[Telephone]], optional): --
         primary(bool): Indicator for one of the travelers who is the primary traveler. One traveler in each itinerary item must be listed as primary. By default, for a single traveler this should be set to `true`.
         age(Optional[float], optional): Age of the traveler.
@@ -852,57 +1274,85 @@
     """
     traveler_id: Optional[constr(max_length=100)] = None
     """
     A unique identifier for travelers in the transaction.
     """
 
 
-class PaymentOperation(BaseModel, smart_union=True, extra=Extra.forbid):
+class PaymentOperation(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model PaymentOperation
     Attributes:
         id(Optional[constr(max_length=200)], optional): --
         amount(Optional[Amount], optional): --
         outcome(Optional[PaymentOutcome], optional): --
 
     """
     id: Optional[constr(max_length=200)] = None
     amount: Optional[Amount] = None
     outcome: Optional[PaymentOutcome] = None
 
 
-class Verify(PaymentOperation, smart_union=True, extra=Extra.forbid):
+class Verify(
+    PaymentOperation,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Verify: A verify operation represents the intent to verify the payment associated with this transaction.
     Attributes:
         type(Optional[VerificationType], optional): --
 
     """
     type: Optional[VerificationType] = None
 
 
-class Authorize(PaymentOperation, smart_union=True, extra=Extra.forbid):
+class Authorize(
+    PaymentOperation,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Authorize: Authorize operation on the payment. An authorize operation represents placing the funds on hold with the specified form of payment."""
     pass
 
 
-class AuthorizeReversal(PaymentOperation, smart_union=True, extra=Extra.forbid):
+class AuthorizeReversal(
+    PaymentOperation,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model AuthorizeReversal: Authorize Reversal operation on the payment. An authorize reversal operation represents a notification received usually from a 3rd party payment processor to indicate that an authorization hold should be released as a result of a sale being partially or completely cancelled."""
     pass
 
 
-class Capture(PaymentOperation, smart_union=True, extra=Extra.forbid):
+class Capture(
+    PaymentOperation,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Capture: Capture operation on the payment. A capture operation represents a notification received usually from a 3rd party payment processor to indicate that the funds placed on hold will be captured and the funds transfer process will occur from the customer's funds to the merchant's funds."""
     pass
 
 
-class Refund(PaymentOperation, smart_union=True, extra=Extra.forbid):
+class Refund(
+    PaymentOperation,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Refund: Refund operation on the payment. A refund operation represents the intent to refund a previous charge."""
     pass
 
 
-class Operations(BaseModel, smart_union=True, extra=Extra.forbid):
+class Operations(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Operations: All operations related to a payment throughout its lifespan. An operation represents an event external to Fraud Prevention Service that specifies to perform a payment operation. Possible operation types include:
 
     - `Verify`
 
     - `Authorize`
 
     - `AuthorizeReversal`
@@ -922,15 +1372,19 @@
     verify: Optional[Verify] = None
     authorize: Optional[Authorize] = None
     authorize_reversal: Optional[AuthorizeReversal] = None
     capture: Optional[Capture] = None
     refunds: Optional[List[Refund]] = Field(None, maxItems=20)
 
 
-class Payment(BaseModel, smart_union=True, extra=Extra.forbid):
+class PaymentGeneric(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model Payment
     Attributes:
         brand(constr(max_length=200)): Payment brand used for payment on this transaction.
         method(PaymentMethod): --
         reason(Optional[PaymentReason], optional): --
         billing_name(Name): --
         billing_address(Optional[Address], optional): --
@@ -960,27 +1414,32 @@
     operations: Optional[Operations] = None
     total_refund_amount: Optional[float] = None
     """
     Total amount refunded towards the transaction.
     """
 
 
-class CreditCard(Payment, smart_union=True, extra=Extra.forbid):
+class CreditCard(
+    PaymentGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model CreditCard
     Attributes:
         card_type(constr(max_length=200)): Type of card used for payment, (eg. `CREDIT`, `DEBIT`).
         card_number(constr(max_length=200)): All the digits (unencrypted) of the credit card number associated with the payment.
         expiry_date(Optional[datetime], optional): Expiration date of the credit card used for payment.
         electronic_commerce_indicator(Optional[constr(max_length=200)], optional): Electronic Commerce Indicator, a two or three digit number usually returned by a 3rd party payment processor in regards to the authentication used when gathering the cardholder's payment credentials.
         virtual_credit_card_flag(Optional[bool], optional): A flag to indicate that the bank card being used for the charge is a virtual credit card.
         wallet_type(Optional[constr(max_length=200)], optional): If a virtual/digital form of payment was used, the type of digital wallet should be specified here. Possible `wallet_type`'s include: `Google` or `ApplePay`.
         card_avs_response(constr(max_length=50)): A field used to confirm if the address provided at the time of purchase matches what the bank has on file for the Credit Card.
         card_cvv_response(constr(max_length=20)): A field used to confirm the Card Verification Value on the Credit Card matches the Credit Card used at the time of purchase.
         telephones(List[Telephone]): Telephone(s) associated with card holder and credit card.
         merchant_order_code(Optional[constr(max_length=200)], optional): Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
+        method(Literal['CREDIT_CARD']): --
 
     """
     card_type: constr(max_length=200) = None
     """
     Type of card used for payment, (eg. `CREDIT`, `DEBIT`).
     """
     card_number: constr(max_length=200) = None
@@ -1015,73 +1474,63 @@
     """
     Telephone(s) associated with card holder and credit card.
     """
     merchant_order_code: Optional[constr(max_length=200)] = None
     """
     Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
     """
+    method: Literal['CREDIT_CARD'] = 'CREDIT_CARD'
 
 
-class PayPal(Payment, smart_union=True, extra=Extra.forbid):
+class PayPal(
+    PaymentGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model PayPal
     Attributes:
         payer_id(constr(max_length=200)): Unique PayPal Customer Account identification number.
         transaction_id(constr(max_length=200)): Unique transaction number to identify Auth calls at PayPal.
         merchant_order_code(Optional[constr(max_length=200)], optional): Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
+        method(Literal['PAYPAL']): --
 
     """
     payer_id: constr(max_length=200) = None
     """
     Unique PayPal Customer Account identification number.
     """
     transaction_id: constr(max_length=200) = None
     """
     Unique transaction number to identify Auth calls at PayPal.
     """
     merchant_order_code: Optional[constr(max_length=200)] = None
     """
     Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
     """
+    method: Literal['PAYPAL'] = 'PAYPAL'
 
 
-class Points(Payment, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model Points"""
-    pass
-
-
-class OrderPurchaseScreenRequest(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model OrderPurchaseScreenRequest
+class Points(
+    PaymentGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Points
     Attributes:
-        transaction(Optional[OrderPurchaseTransaction], optional): --
+        method(Literal['POINTS']): --
 
     """
-    transaction: Optional[OrderPurchaseTransaction] = None
+    method: Literal['POINTS'] = 'POINTS'
 
 
-class OrderPurchaseTransaction(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model OrderPurchaseTransaction
-    Attributes:
-        site_info(SiteInfo): --
-        device_details(DeviceDetails): --
-        customer_account(CustomerAccount): --
-        transaction_details(TransactionDetails): --
-        bypass_risk_flag(Optional[bool], optional): A flag to indicate whether the client is ignoring the decision by Trust validation and proceeds to process the even in-case the outcome is ‘Reject’ or ‘Review’.
-
-    """
-    site_info: SiteInfo = None
-    device_details: DeviceDetails = None
-    customer_account: CustomerAccount = None
-    transaction_details: TransactionDetails = None
-    bypass_risk_flag: Optional[bool] = None
-    """
-    A flag to indicate whether the client is ignoring the decision by Trust validation and proceeds to process the even in-case the outcome is ‘Reject’ or ‘Review’.
-    """
-
-
-class TransactionDetails(BaseModel, smart_union=True, extra=Extra.forbid):
+class TransactionDetails(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
     r"""pydantic model TransactionDetails
     Attributes:
         order_id(constr(max_length=50)): Unique identifier assigned to the order by the partner. `order_id` is specific to the partner namespace.
         current_order_status(CurrentOrderStatus): Status of the order.
         order_type(OrderType): Type of order. Possible `order_types`.  `CREATE` - Initial type of a brand new order.  `CHANGE` - If a `OrderPurchaseScreenRequest` has already been submitted for the initial booking with `order_type = CREATE`, but has now been modified and partner wishes to resubmit for Fraud screening then the `order_type = CHANGE`. Examples of changes that are supported are changes made to `check-in/checkout dates` or `price of a TravelProduct`.
         travel_products(List[TravelProduct]): --
         travelers(List[Traveler]): Individuals who are part of the travel party for the order. At minimum there must be at least `1` traveler.
@@ -1117,374 +1566,56 @@
     """
     credit_card_authentication_failure_count: Optional[int] = None
     """
     Total authentication failure count for given credit card. Authentication failures happen when a cardholder enters their card information incorrectly.
     """
 
 
-class OrderUpdate(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model OrderUpdate
-    Attributes:
-        risk_id(constr(max_length=200)): The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
-        order_status(Status): --
-        cancellation_reason(Optional[CancellationReason], optional): --
-        type(Literal["OrderUpdate"]): --
-
-    """
-    risk_id: constr(max_length=200) = Field(..., example='123456789')
-    """
-    The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
-    """
-    order_status: Status = None
-    cancellation_reason: Optional[CancellationReason] = None
-    type: Literal["OrderUpdate"] = None
-
-
-class ChargebackFeedback(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model ChargebackFeedback
-    Attributes:
-        risk_id(constr(max_length=200)): The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
-        chargeback_detail(Optional[ChargebackDetail], optional): --
-        type(Literal["ChargebackFeedback"]): --
-
-    """
-    risk_id: constr(max_length=200) = Field(..., example='123456789')
-    """
-    The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
-    """
-    chargeback_detail: Optional[ChargebackDetail] = None
-    type: Literal["ChargebackFeedback"] = None
-
-
-class InsultFeedback(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model InsultFeedback
-    Attributes:
-        risk_id(constr(max_length=200)): The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
-        insult_detail(Optional[InsultDetail], optional): --
-        type(Literal["InsultFeedback"]): --
-
-    """
-    risk_id: constr(max_length=200) = Field(..., example='123456789')
-    """
-    The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
-    """
-    insult_detail: Optional[InsultDetail] = None
-    type: Literal["InsultFeedback"] = None
-
-
-class RefundUpdate(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model RefundUpdate
-    Attributes:
-        risk_id(constr(max_length=200)): The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
-        acquirer_reference_number(constr(max_length=200)): A unique number that tags a credit or debit card transaction when it goes from the merchant's bank through to the cardholder's bank.
-        refund_deposit_timestamp(datetime): Date and time when the refund was deposited to the original form of payment.
-        refund_settlement_timestamp(datetime): Date and time when the 3rd party payment processor confirmed that a previously submitted payment refund has settled at the participating financial institutions.
-        settlement_id(constr(max_length=200)): Unique settlement identifier generated for a previously submitted payment refund.
-        refund_amount(Amount): --
-        type(Literal["RefundUpdate"]): --
-
-    """
-    risk_id: constr(max_length=200) = Field(..., example='123456789')
-    """
-    The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
-    """
-    acquirer_reference_number: constr(max_length=200) = None
-    """
-    A unique number that tags a credit or debit card transaction when it goes from the merchant's bank through to the cardholder's bank.
-    """
-    refund_deposit_timestamp: datetime = None
-    """
-    Date and time when the refund was deposited to the original form of payment.
-    """
-    refund_settlement_timestamp: datetime = None
-    """
-    Date and time when the 3rd party payment processor confirmed that a previously submitted payment refund has settled at the participating financial institutions.
-    """
-    settlement_id: constr(max_length=200) = None
-    """
-    Unique settlement identifier generated for a previously submitted payment refund.
-    """
-    refund_amount: Amount = None
-    type: Literal["RefundUpdate"] = None
-
-
-class PaymentUpdate(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model PaymentUpdate
-    Attributes:
-        risk_id(constr(max_length=200)): The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
-        merchant_order_code(constr(max_length=200)): Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
-        type(Literal["PaymentUpdate"]): --
-
-    """
-    risk_id: constr(max_length=200) = Field(..., example='123456789')
-    """
-    The `risk_id` provided by Expedia's Fraud Prevention Service in the `OrderPurchaseScreenResponse`.
-    """
-    merchant_order_code: constr(max_length=200) = None
-    """
-    Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
-    """
-    type: Literal["PaymentUpdate"] = None
-
-
-class Air(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model Air
-    Attributes:
-        price(Amount): --
-        inventory_type(constr(max_length=30)): Type of inventory.
-        inventory_source(InventorySource): Identifies the business model through which the supply is being sold. Merchant/Agency.
-        travelers_references(List[constr(max_length=50)]): List of travelerGuids who are part of the traveling party on the order for the product.
-        departure_time(datetime): Local date and time of departure from original departure location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-        arrival_time(datetime): Local date and time of arrival to final destination location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-        air_segments(List[AirSegment]): Additional airline and flight details for each of the trip segments.
-        flight_type(Optional[FlightType], optional): Identifies the type of air trip based on the air destinations.
-        passenger_name_record(Optional[constr(max_length=100)], optional): Airline booking confirmation code for the trip.
-        global_distribution_system_type(Optional[constr(max_length=100)], optional): Associated with Passenger Name Record (PNR).
-        type(Literal["Air"]): Type of product advertised on the website.
-
-    """
-    price: Amount = None
-    inventory_type: constr(max_length=30) = None
-    """
-    Type of inventory.
-    """
-    inventory_source: InventorySource = None
-    """
-    Identifies the business model through which the supply is being sold. Merchant/Agency.
-    """
-    travelers_references: List[constr(max_length=50)] = Field(..., maxItems=40, minItems=1)
-    """
-    List of travelerGuids who are part of the traveling party on the order for the product.
-    """
-    departure_time: datetime = None
-    """
-    Local date and time of departure from original departure location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-    """
-    arrival_time: datetime = None
-    """
-    Local date and time of arrival to final destination location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-    """
-    air_segments: List[AirSegment] = Field(..., maxItems=30, minItems=1)
-    """
-    Additional airline and flight details for each of the trip segments.
-    """
-    flight_type: Optional[FlightType] = None
-    """
-    Identifies the type of air trip based on the air destinations.
-    """
-    passenger_name_record: Optional[constr(max_length=100)] = None
-    """
-    Airline booking confirmation code for the trip.
-    """
-    global_distribution_system_type: Optional[constr(max_length=100)] = None
-    """
-    Associated with Passenger Name Record (PNR).
-    """
-    type: Literal["Air"] = None
-    """
-    Type of product advertised on the website.
-    """
-
-
-class Cruise(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model Cruise
-    Attributes:
-        price(Amount): --
-        inventory_type(constr(max_length=30)): Type of inventory.
-        inventory_source(InventorySource): Identifies the business model through which the supply is being sold. Merchant/Agency.
-        travelers_references(List[constr(max_length=50)]): List of travelerGuids who are part of the traveling party on the order for the product.
-        departure_time(datetime): Local date and time of departure from original departure location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-        arrival_time(datetime): Local date and time of arrival from original arrival location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-        embarkation_port(constr(max_length=200)): Location from where cruise will depart.
-        disembarkation_port(constr(max_length=200)): The cruise's final destination.
-        ship_name(constr(max_length=200)): Name of the cruise ship.
-        type(Literal["Cruise"]): Type of product advertised on the website.
-
-    """
-    price: Amount = None
-    inventory_type: constr(max_length=30) = None
-    """
-    Type of inventory.
-    """
-    inventory_source: InventorySource = None
-    """
-    Identifies the business model through which the supply is being sold. Merchant/Agency.
-    """
-    travelers_references: List[constr(max_length=50)] = Field(..., maxItems=40, minItems=1)
-    """
-    List of travelerGuids who are part of the traveling party on the order for the product.
-    """
-    departure_time: datetime = None
-    """
-    Local date and time of departure from original departure location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-    """
-    arrival_time: datetime = None
-    """
-    Local date and time of arrival from original arrival location, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-    """
-    embarkation_port: constr(max_length=200) = None
-    """
-    Location from where cruise will depart.
-    """
-    disembarkation_port: constr(max_length=200) = None
-    """
-    The cruise's final destination.
-    """
-    ship_name: constr(max_length=200) = None
-    """
-    Name of the cruise ship.
-    """
-    type: Literal["Cruise"] = None
-    """
-    Type of product advertised on the website.
-    """
-
-
-class Car(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model Car
+class OrderPurchaseTransaction(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model OrderPurchaseTransaction
     Attributes:
-        price(Amount): --
-        inventory_type(constr(max_length=30)): Type of inventory.
-        inventory_source(InventorySource): Identifies the business model through which the supply is being sold. Merchant/Agency.
-        travelers_references(List[constr(max_length=50)]): List of travelerGuids who are part of the traveling party on the order for the product.
-        pick_up_location(constr(max_length=200)): Location where the automobile will be picked up.
-        drop_off_location(constr(max_length=200)): Location at which the automobile will be returned.
-        pickup_time(datetime): Local date and time the automobile will be picked-up, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-        return_time(datetime): Local date and time the automobile will be returned, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-        type(Literal["Car"]): Type of product advertised on the website.
+        site_info(SiteInfo): --
+        device_details(DeviceDetails): --
+        customer_account(CustomerAccount): --
+        transaction_details(TransactionDetails): --
+        bypass_risk_flag(Optional[bool], optional): A flag to indicate whether the client is ignoring the decision by Trust validation and proceeds to process the even in-case the outcome is ‘Reject’ or ‘Review’.
 
     """
-    price: Amount = None
-    inventory_type: constr(max_length=30) = None
-    """
-    Type of inventory.
-    """
-    inventory_source: InventorySource = None
-    """
-    Identifies the business model through which the supply is being sold. Merchant/Agency.
-    """
-    travelers_references: List[constr(max_length=50)] = Field(..., maxItems=40, minItems=1)
-    """
-    List of travelerGuids who are part of the traveling party on the order for the product.
-    """
-    pick_up_location: constr(max_length=200) = None
-    """
-    Location where the automobile will be picked up.
-    """
-    drop_off_location: constr(max_length=200) = None
-    """
-    Location at which the automobile will be returned.
-    """
-    pickup_time: datetime = None
-    """
-    Local date and time the automobile will be picked-up, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-    """
-    return_time: datetime = None
-    """
-    Local date and time the automobile will be returned, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-    """
-    type: Literal["Car"] = None
+    site_info: SiteInfo = None
+    device_details: DeviceDetails = None
+    customer_account: CustomerAccount = None
+    transaction_details: TransactionDetails = None
+    bypass_risk_flag: Optional[bool] = None
     """
-    Type of product advertised on the website.
+    A flag to indicate whether the client is ignoring the decision by Trust validation and proceeds to process the even in-case the outcome is ‘Reject’ or ‘Review’.
     """
 
 
-class Hotel(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model Hotel
+class OrderPurchaseScreenRequest(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model OrderPurchaseScreenRequest
     Attributes:
-        price(Amount): --
-        inventory_type(constr(max_length=30)): Type of inventory.
-        inventory_source(InventorySource): Identifies the business model through which the supply is being sold. Merchant/Agency.
-        travelers_references(List[constr(max_length=50)]): List of travelerGuids who are part of the traveling party on the order for the product.
-        hotel_id(constr(max_length=200)): Unique hotel identifier assigned by the partner.
-        price_withheld(Optional[bool], optional): Identifies if the product price was withheld from the customer during the booking process.
-        hotel_name(constr(max_length=200)): Name of the hotel.
-        room_count(Optional[int], optional): Total number of rooms booked within the hotel product collection.
-        address(Address): --
-        checkin_time(datetime): Local date and time of the hotel check-in, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-        checkout_time(datetime): Local date and time of the hotel check-out, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-        type(Literal["Hotel"]): Type of product advertised on the website.
+        transaction(Optional[OrderPurchaseTransaction], optional): --
 
     """
-    price: Amount = None
-    inventory_type: constr(max_length=30) = None
-    """
-    Type of inventory.
-    """
-    inventory_source: InventorySource = None
-    """
-    Identifies the business model through which the supply is being sold. Merchant/Agency.
-    """
-    travelers_references: List[constr(max_length=50)] = Field(..., maxItems=40, minItems=1)
-    """
-    List of travelerGuids who are part of the traveling party on the order for the product.
-    """
-    hotel_id: constr(max_length=200) = Field(..., example='8883333999221')
-    """
-    Unique hotel identifier assigned by the partner.
-    """
-    price_withheld: Optional[bool] = None
-    """
-    Identifies if the product price was withheld from the customer during the booking process.
-    """
-    hotel_name: constr(max_length=200) = Field(..., example='Hotel Expedia')
-    """
-    Name of the hotel.
-    """
-    room_count: Optional[int] = None
-    """
-    Total number of rooms booked within the hotel product collection.
-    """
-    address: Address = None
-    checkin_time: datetime = None
-    """
-    Local date and time of the hotel check-in, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-    """
-    checkout_time: datetime = None
-    """
-    Local date and time of the hotel check-out, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
-    """
-    type: Literal["Hotel"] = None
-    """
-    Type of product advertised on the website.
-    """
+    transaction: Optional[OrderPurchaseTransaction] = None
 
 
-class Insurance(BaseModel, smart_union=True, extra=Extra.forbid):
-    r"""pydantic model Insurance
-    Attributes:
-        price(Amount): --
-        inventory_type(constr(max_length=30)): Type of inventory.
-        inventory_source(InventorySource): Identifies the business model through which the supply is being sold. Merchant/Agency.
-        travelers_references(List[constr(max_length=50)]): List of travelerGuids who are part of the traveling party on the order for the product.
-        type(Literal["Insurance"]): Type of product advertised on the website.
+OrderPurchaseUpdateRequest = Union[OrderUpdate, ChargebackFeedback, InsultFeedback, RefundUpdate, PaymentUpdate, OrderPurchaseUpdateRequestGeneric]
 
-    """
-    price: Amount = None
-    inventory_type: constr(max_length=30) = None
-    """
-    Type of inventory.
-    """
-    inventory_source: InventorySource = None
-    """
-    Identifies the business model through which the supply is being sold. Merchant/Agency.
-    """
-    travelers_references: List[constr(max_length=50)] = Field(..., maxItems=40, minItems=1)
-    """
-    List of travelerGuids who are part of the traveling party on the order for the product.
-    """
-    type: Literal["Insurance"] = None
-    """
-    Type of product advertised on the website.
-    """
-
-
-OrderPurchaseUpdateRequest = Union[OrderUpdate, ChargebackFeedback, InsultFeedback, RefundUpdate, PaymentUpdate]
+TravelProduct = Union[Air, Cruise, Car, Hotel, Insurance, TravelProductGeneric]
 
-TravelProduct = Union[Air, Cruise, Car, Hotel, Insurance]
+Payment = Union[CreditCard, PayPal, Points, PaymentGeneric]
 
 
 CancellationReason.update_forward_refs()
 
 
 ChargebackDetail.update_forward_refs()
 
@@ -1524,95 +1655,92 @@
 
 Email.update_forward_refs()
 
 
 Amount.update_forward_refs()
 
 
-OrderPurchaseScreenResponse.update_forward_refs()
-
-
-ExtendedError.update_forward_refs()
+OrderUpdate.update_forward_refs()
 
 
-PaymentOutcome.update_forward_refs()
+ChargebackFeedback.update_forward_refs()
 
 
-Telephone.update_forward_refs()
+InsultFeedback.update_forward_refs()
 
 
-CustomerAccount.update_forward_refs()
+RefundUpdate.update_forward_refs()
 
 
-Traveler.update_forward_refs()
+PaymentUpdate.update_forward_refs()
 
 
-PaymentOperation.update_forward_refs()
+OrderPurchaseScreenResponse.update_forward_refs()
 
 
-Verify.update_forward_refs()
+ExtendedError.update_forward_refs()
 
 
-Authorize.update_forward_refs()
+Air.update_forward_refs()
 
 
-AuthorizeReversal.update_forward_refs()
+Cruise.update_forward_refs()
 
 
-Capture.update_forward_refs()
+Car.update_forward_refs()
 
 
-Refund.update_forward_refs()
+Hotel.update_forward_refs()
 
 
-Operations.update_forward_refs()
+PaymentOutcome.update_forward_refs()
 
 
-Payment.update_forward_refs()
+Insurance.update_forward_refs()
 
 
-CreditCard.update_forward_refs()
+Telephone.update_forward_refs()
 
 
-PayPal.update_forward_refs()
+CustomerAccount.update_forward_refs()
 
 
-Points.update_forward_refs()
+Traveler.update_forward_refs()
 
 
-OrderPurchaseScreenRequest.update_forward_refs()
+PaymentOperation.update_forward_refs()
 
 
-OrderPurchaseTransaction.update_forward_refs()
+Verify.update_forward_refs()
 
 
-TransactionDetails.update_forward_refs()
+Authorize.update_forward_refs()
 
 
-OrderUpdate.update_forward_refs()
+AuthorizeReversal.update_forward_refs()
 
 
-ChargebackFeedback.update_forward_refs()
+Capture.update_forward_refs()
 
 
-InsultFeedback.update_forward_refs()
+Refund.update_forward_refs()
 
 
-RefundUpdate.update_forward_refs()
+Operations.update_forward_refs()
 
 
-PaymentUpdate.update_forward_refs()
+CreditCard.update_forward_refs()
 
 
-Air.update_forward_refs()
+PayPal.update_forward_refs()
 
 
-Cruise.update_forward_refs()
+Points.update_forward_refs()
 
 
-Car.update_forward_refs()
+TransactionDetails.update_forward_refs()
 
 
-Hotel.update_forward_refs()
+OrderPurchaseTransaction.update_forward_refs()
 
 
-Insurance.update_forward_refs()
+OrderPurchaseScreenRequest.update_forward_refs()
```

### Comparing `openworld-sdk-python-fraudprevention-0.7.0/openworld_sdk_python_fraudprevention.egg-info/PKG-INFO` & `openworld-sdk-python-fraudprevention-0.8.0/openworld_sdk_python_fraudprevention.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudprevention
-Version: 0.7.0
+Version: 0.8.0
 Summary: Open World Fraud Prevention SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-fraudprevention-0.7.0/setup.py` & `openworld-sdk-python-fraudprevention-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 from setuptools import setup
 
 setup(
     name='openworld-sdk-python-fraudprevention',
-    version='0.7.0',
+    version='0.8.0',
     packages=['openworld.sdk.fraudprevention'],
     package_dir={'openworld-sdk-python-fraudprevention': '.'},
     license='Apache License, Version 2.0',
     author='Expedia Group',
     author_email='oss@expediagroup.com',
     url='https://github.com/ExpediaGroup/openworld-sdk-python',
     classifiers=[
```

