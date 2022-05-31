---
title: Encryptor
description: Encryptor
draft: Probably
---
# Encryptor

Adobe Workfront Fusion Encryptor modules allow you to encrypt any text data. They currently support message encryption via AES256 and PGP (OpenPGP).

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
   <td> <p>Workfront Fusion for Work Automation and Integration </p>   <p>Workfront Fusion for Work Automation</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Message encryption and decryption using PGP

When encrypting and decrypting via PGP, it is necessary to use a keychain and to create a private or public key (or both).

For more information on public and private keys, see [Basic terms in Adobe Workfront Fusion](../../workfront-fusion/get-started/basic-terms.md). For more information on keychains, see [Keys in Adobe Workfront Fusion](../../workfront-fusion/connections/keys.md).

## Encryptor modules and their fields

When you are configuring Encryptor modules, the following fields display. A bolded title in a module indicates a required field.

### Encrypt a PGP message

This module allows you to encrypt a message using public and private keys.

<table style="table-layout:auto">
    <tr>
        <td>Private key</td>
        <td>Enter the sender's private key. This can authenticate the sender's identity.</td>
    </tr>
    <tr>
        <td>Public key</td>
        <td>Enter the recipient's public key.</td>
    </tr>
    <tr>
        <td>Message</td>
        <td>Enter the message that you want to encrypt.</td>
    </tr>

### Decrypt a PGP message

This module allows you to decrypt a message using public and private keys.

<table style="table-layout:auto">
    <tr>
        <td>Private key</td>
        <td>Enter the recipient's private key.</td>
    </tr>
    <tr>
        <td>Public key</td>
        <td>Enter the recipient's public key. This can authenticate the sender's identity.</td>
    </tr>
    <tr>
        <td>Message</td>
        <td>Map the message that you want to decrypt.</td>
    </tr>
</table>

&nbsp;
