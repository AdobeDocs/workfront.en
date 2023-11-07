---
title: Overview
description: Overview
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
---
# Overview

**Welcome to the Workfront Proof API**

The Workfront Proof API is a simple HTTP service that is secured using SSL. The API aims to provide you with all the functionality that used in our own application.

## Supported formats

The public interface is SOAP 1.1 compliant with WSDL support.&nbsp;All requests are therefore&nbsp;executed&nbsp;using XML over HTTPS.

## API versioning

In order to preserve compatibility with existing client&nbsp;integration's&nbsp;we have introduced API versioning as from our 12.1 release. Please see the&nbsp; [API updates](http://api.proofhq.com/new-updates) page for more information. If a method or parameter has no version information it means that you'll find this as part of our standard API, please see the "Getting started with the API" section below.

## Getting started with the API

The API entry point:

`https://soap.proofhq.com/soap` (please note the use of HTTPS)

The&nbsp;WSDL can be found here:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**This WSDL contains all the changes up until the 12.1 release, after which we introduced API versioning. Please see the API Updates page for more information about the various WSDL versions and upcoming changes**

Every API request requires a session key. This session key identifies the Workfront Proof user performing the action(s) and is obtained by calling the doLogin() method and passing in the user's email address and password. The doLogin() method only needs to be called once before a sequence of API requests. The session key remains active for a short period of time and is renewed on every method call.&nbsp;*We will be adding support for token based authentication very soon.*

All requests use the following envelope, header and body format:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

## FAQ's

For a collection of frequently asked questions, please visit [this](http://api.proofhq.com/faqs) page.
