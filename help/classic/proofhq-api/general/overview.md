

# Overview

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

**Welcome to the Workfront Proof API**

The Workfront Proof API is a simple HTTP service that is secured using SSL. The API aims to provide you with all the functionality that used in our own application.

## Supported formats

The public interface is SOAP 1.1 compliant with WSDL support.&nbsp;All requests are therefore&nbsp;executed&nbsp;using XML over HTTPS.

## API versioning

In order to preserve compatibility with existing client&nbsp;integration's&nbsp;we have introduced API versioning as from our 12.1 release. Please see the&nbsp; [API updates](http://api.proofhq.com/new-updates) page for more information. If a method or parameter has no version information it means that you'll find this as part of our standard API, please see the "Getting started with the API" section below.

## Getting started with the API

The API entry point:
<pre><code>https://soap.proofhq.com/soap</code></pre> (please note the use of HTTPS)

The&nbsp;WSDL can be found here:

[

```
https://soap.proofhq.com/soap?wsdl
```

](https://soap.proofhq.com/soap?wsdl)

>[!NOTE]
>
>**This WSDL contains all the changes up until the 12.1 release, after which we introduced API versioning. Please see the API Updates page for more information about the various WSDL versions and upcoming changes**

Every API request requires a session key. This session key identifies the Workfront Proof user performing the action(s) and is obtained by calling the doLogin() method and passing in the user's email address and password. The doLogin() method only needs to be called once before a sequence of API requests. The session key remains active for a short period of time and is renewed on every method call.&nbsp;*We will be adding support for token based authentication very soon.*

All requests use the following envelope, header and body format:
<pre><code><soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi"></code><br><code>&nbsp;&nbsp; &nbsp;<soapenv:Header/></code><br><code>&nbsp;&nbsp; &nbsp;<soapenv:Body></code><br><code>&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;... API function and data inserted here ...</code><br><code>&nbsp;&nbsp; &nbsp;</soapenv:Body></code><br><code></soapenv:Envelope></code></pre>

## FAQ's

For a collection of frequently asked questions, please visit [this](http://api.proofhq.com/faqs) page.
