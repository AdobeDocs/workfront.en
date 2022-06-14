---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: Use Mutual TLS in HTTP modules in Adobe Workfront Fusion
description: You can use Mutual TLS in your Adobe Workfront Fusion HTTP modules, allowing both sides of the information transaction to verify the other's identity. 
feature: Workfront Fusion
---

# Use Mutual TLS in HTTP modules in Adobe Workfront Fusion

>[!AVAILABILITY]
>
>Adobe Workfront Fusion requires an Adobe Workfront Fusion license in addition to an Adobe Workfront license.

## Mutual TLS overview

When you send data over the internet, it's important to ensure that it goes to or comes from the correct location and that only the intended recipient can read it. With TLS enabled, the client (computer requesting information) uses certificates to verify the identity of the server (computer providing information). This makes secure HTTP connections.

Mutual TLS allows this identity confirmation to go both ways. When the server sends its certificate to verify its identity to the client, it also requests the client's certificate. This ensures that the server does not send information to a site or user that would misuse it.

>[!INFO]
>
>**Example:**
>
>* **TLS**: When a person types "MyGreatBank.com" into a browser, they want to be sure that they are going to My Great Bank, not a website that might misuse or sell their banking information. They also want to be sure their bank account information is encrypted.
>
>   When the browser (the client) connects to MyGreatBank.com (the server), TLS requires a certificate from MyGreatBank.com to verify its identity. The certificate is provided by a certificate authority such as DigiCert or Thawte. Because the browser trusts the certificate authority, it allows the connection.
>
>* **Mutual TLS**: MySoftware.com is a software client that needs information from the MyGreatBank.com API. MyGreatBank allows only trusted clients to connect to their servers. So, in addition to the regular TLS verifying the identity of MyGreatBank.com, the TLS/certificate authority process also verifies the request from MySoftware.com.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Providing your Workfront Fusion public certificate


When you connect to a web service with an HTTP request, the web service usually requires a Workfront Fusion public certificate for verification. This allows the web service to compare the certificate presented in the HTTP request to the one on file, as a way to ensure that the certificate is on the web service's allowlist.

For instructions on uploading the Adobe Workfront Fusion public certificate to a web service, see the web service's documentation.

You can use the following links to download the Workfront Fusion public certificates:

### Certificates for the year November 17, 2021 - November 17, 2022

* [Download Workfront Fusion Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com_certificate-chain-2022.crt) 
* [Download Workfront Fusion EU Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app-eu_workfrontfusion_com_certificate-chain-2022.crt)

  For use in the EU

>[!IMPORTANT]
>
>Workfront Fusion public certificates expire annually. After yours expires you will need to upload a new certificate to the web service. We recommend that you:
>
>* Make note of the expiration date and set a reminder for yourself to upload the certificate to your web service.
>* Bookmark this page to easily find the new certificates.
>

>[!NOTE]
>
>You may need to provide other information in addition to the certificate. For information on what a web service requires, see the web service's API documentation.

## Enabling Mutual TLS&nbsp;in Workfront Fusion HTTP modules

All Workfront Fusion HTTP request modules have the option to enable Mutual TLS.

To enable Mutual TLS in an HTTP request module:

1. Add an HTTP request module to your scenario.
1. Begin configuring the module.

   For instructions on configuring an HTTP request module, see the appropriate article under [HTTP modules](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Enable **Show advanced settings** near the bottom of the module.
1. Enable **Use Mutual TLS**.

