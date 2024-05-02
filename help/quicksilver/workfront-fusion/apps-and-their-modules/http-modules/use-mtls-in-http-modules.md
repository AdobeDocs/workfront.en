---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: http-modules
title: Use Mutual TLS in HTTP modules in Adobe Workfront Fusion
description: You can use Mutual TLS in your Adobe Workfront Fusion HTTP modules, allowing both sides of the information transaction to verify the other's identity.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
---
# Use Mutual TLS in HTTP modules in [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>Adobe Workfront Fusion requires an [!DNL Adobe Workfront Fusion] license in addition to an Adobe Workfront license.

## Mutual TLS overview

When you send data over the internet, it's important to ensure that it goes to or comes from the correct location and that only the intended recipient can read it. With TLS enabled, the client (computer requesting information) uses certificates to verify the identity of the server (computer providing information). This makes secure HTTP connections.

Mutual TLS allows this identity confirmation to go both ways. When the server sends its certificate to verify its identity to the client, it also requests the client's certificate. This ensures that the server does not send information to a site or user that would misuse it.

>[!INFO]
>
>**Example:**
>
>* **TLS**: When a person types "MyGreatBank.com" into a browser, they want to be sure that they are going to My Great Bank, not a website that might misuse or sell their banking information. They also want to be sure their bank account information is encrypted.
>
>   When the browser (the client) connects to MyGreatBank.com (the server), TLS requires a certificate from MyGreatBank.com to verify its identity. The certificate is provided by a certificate authority such as [!DNL DigiCert] or [!DNL Thawte]. Because the browser trusts the certificate authority, it allows the connection.
>
>* **Mutual TLS**: MySoftware.com is a software client that needs information from the MyGreatBank.com API. MyGreatBank allows only trusted clients to connect to their servers. So, in addition to the regular TLS verifying the identity of MyGreatBank.com, the TLS/certificate authority process also verifies the request from MySoftware.com.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

&#42;&#42;For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Providing your [!DNL Workfront Fusion] public certificate


When you connect to a web service with an HTTP request, the web service usually requires a [!DNL Workfront Fusion] public certificate for verification. This allows the web service to compare the certificate presented in the HTTP request to the one on file, as a way to ensure that the certificate is on the web service's allowlist.

For instructions on uploading the [!DNL Adobe Workfront Fusion] public certificate to a web service, see the web service's documentation.

>[!NOTE]
>
>You may need to provide other information in addition to the certificate. For information on what a web service requires, see the web service's API documentation.

You can use the following links to download the Workfront Fusion public certificates:

### Certificates for April 23, 2023-May 7, 2024

>[!IMPORTANT]
>
>* These [!DNL Workfront Fusion] public certificates expire on May 7, 2025. After yours expires you will need to upload a new certificate to the web service. We recommend that you:
>
>   * Make note of the expiration date and set a reminder for yourself to upload the certificate to your web service.
>   * Bookmark this page to easily find the new certificates.
>
>* These are non-wildcard mTLS certificates.

* [Download [!DNL Workfront Fusion] Certificate 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-us-mtls-certificate.pem)
* [Download [!DNL Workfront Fusion] EU Certificate 2023](/help/quicksilver/workfront-fusion/apps-and-their-modules/http-modules/assets/fusion-prod-eu-mtls-certificate.pem)

   For use in the EU 

<!--

### Certificates for November 14, 2022 - July 15, 2023

>[!IMPORTANT]
>
>* These [!DNL Workfront Fusion] public certificates expire on July 15, 2023.
>* These are wildcard mTLS certificates.

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Download [!DNL Workfront Fusion] EU Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   For use in the EU 

   -->

## Enabling Mutual TLS&nbsp;in [!DNL Workfront Fusion] HTTP modules

All [!DNL Workfront Fusion] [!UICONTROL HTTP] request modules have the option to enable Mutual TLS.

To enable Mutual TLS in an [!UICONTROL HTTP] request module:

1. Add an [!UICONTROL HTTP] request module to your scenario.
1. Begin configuring the module.

   For instructions on configuring an [!UICONTROL HTTP] request module, see the appropriate article under [[!UICONTROL HTTP] modules](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Enable **[!UICONTROL Show advanced settings]** near the bottom of the module.
1. Enable **[!UICONTROL Use Mutual TLS]**.
