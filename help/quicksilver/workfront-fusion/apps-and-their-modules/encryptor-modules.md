---
title: Encryptor
description: Adobe Workfront Fusion Encryptor modules allow you to encrypt any text data. They currently support message encryption via AES256 and PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
---
# Encryptor

[!DNL Adobe Workfront Fusion] [!UICONTROL Encryptor] modules allow you to encrypt any text data. They currently support message encryption via AES256 and PGP ([!UICONTROL OpenPGP]).

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

## Message encryption and decryption using PGP

When encrypting and decrypting via PGP, it is necessary to use a keychain and to create a private or public key (or both).

For more information on public and private keys, see [Basic terms in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). For more information on keychains, see [Keys in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Encryptor] modules and their fields

When you are configuring [!UICONTROL Encryptor] modules, the following fields display. A bolded title in a module indicates a required field.

### Encrypt a PGP message

This module allows you to encrypt a message using public and private keys.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>Enter the sender's private key. This can authenticate the sender's identity.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Enter the recipient's public key.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Enter the message that you want to encrypt.</td>
    </tr>

### Decrypt a PGP message

This module allows you to decrypt a message using public and private keys.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Private key]</td>
        <td>Enter the recipient's private key.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Public key]</td>
        <td>Enter the recipient's public key. This can authenticate the sender's identity.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Message]</td>
        <td>Map the message that you want to decrypt.</td>
    </tr>
</table>
