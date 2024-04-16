---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JWT modules
description: The [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] app provides a module that creates JWT tokens based on the provided algorithm.
author: Becky
feature: Workfront Fusion
exl-id: 1c09967e-a236-404f-bf3e-9de66118e77b
---
# [!UICONTROL JWT] module

The [!DNL Adobe Workfront Fusion] [!UICONTROL JWT] app provides a module that creates JWT tokens based on the provided algorithm.

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
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## JWT module and its fields

### Generate JWT

This module generates a JWT based on the selected algorithm. 

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Algorithm]</td> 
   <td> <p>Select algorithm with which you want to generate the JWT.</p> <ul>
   <li><b>HS256</b>: HMAC using SHA-256 hash algorithm</li>
   <li><b>HS384</b>: HMAC using SHA-384 hash algorithm</li>
   <li><b>HS512</b>: HMAC using SHA-512 hash algorithm</li>
   <li><b>RS256</b>: RSASSA-PKCS1-v1_5 using SHA-256 hash algorithm</li>
   <li><b>RS384</b>: RSASSA-PKCS1-v1_5 using SHA-384 hash algorithm</li>
   <li><b>RS512</b>: RSASSA-PKCS1-v1_5 using SHA-512 hash algorithm</li>
   <li><b>PS256</b>: RSASSA-PSS using SHA-256 hash algorithm (only Node ^6.12.0 OR >=8.0.0)</li>
   <li><b>PS384</b>: RSASSA-PSS using SHA-384 hash algorithm (only Node ^6.12.0 OR >=8.0.0)</li>
   <li><b>PS512</b>: RSASSA-PSS using SHA-512 hash algorithm (only Node ^6.12.0 OR >=8.0.0)</li>
   <li><b>ES256</b>: ECDSA using P-256 curve and SHA-256 hash algorithm</li>
   <li><b>ES384</b>: ECDSA using P-384 curve and SHA-384 hash algorithm</li>
   <li><b>ES512</b>: ECDSA using P-521 curve and SHA-512 hash algorithm</li>
   </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Payload] </td> 
   <td> <p>For each payload item you want to add, click <b>Add item</b> and enter the item's key and value.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Options] </td> 
   <td> <p>For each option item you want to add, click <b>Add item</b> and enter the item's key and value.</p> <p>The following keys are available:
   <ul>
   <li><b>algorithm</b>: (default: RS256)</li>
   <li><b>expiresIn</b>: Expressed in seconds or a string describing a time span (e.g., 2 days, 10h, 7d). A numeric value is interpreted as a seconds count. If you use a string, be sure to provide the time units (days, hours, etc.), otherwise milliseconds unit is used by default (120 is equal to 120ms).</li>
   <li><b>notBefore</b>: Expressed in seconds or a string describing a time span (e.g., 2 days, 10h, 7d). A numeric value is interpreted as a seconds count. If you use a string, be sure to provide the time units (days, hours, etc.), otherwise milliseconds unit is used by default (120 is equal to 120ms).
</li>
   <li><b>audience</b></li>
   <li><b>issuer</b></li>
   <li><b>jwtid</b></li>
   <li><b>subject</b></li>
   <li><b>noTimestamp</b></li>
   <li><b>header</b></li>
   <li><b>keyid</b></li>
   <li><b>mutatePayload</b>: If <code>true</code>, the sign function will modify the payload object directly. This is useful if you need a raw reference to the payload after claims have been applied to it but before it has been encoded into a token.</li>
   <li><b>allowInsecureKeySizes</b>: If <code>true</code>, allows private keys with a modulus below 2048 to be used for RSA.</li>
   <li><b>allowInvalidAsymmetricKeyTypes</b>: If <code>true</code>, allows asymmetric keys which do not match the specified algorithm. This option is intended only for backward compatibility and should be avoided.</li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>
