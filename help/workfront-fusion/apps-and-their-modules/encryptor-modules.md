

# Encryptor

Encryptor modules allow you to encrypt any text data. They currently support message encryption via AES256 and PGP (OpenPGP).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Message encryption and decryption using PGP

When encrypting and decrypting via PGP, it is necessary to use a keychain and to create a private or public key (or both).

For more information on public and private keys, see [Basic terms](../../workfront-fusion/get-started/basic-terms.md). For more information on keychains, see [Keys in Adobe Workfront Fusion](../../workfront-fusion/connections/keys.md).

## Encryptor modules and their fields

When you are configuring Encryptor modules, the following fields display. A bolded title in a module indicates a required field.

### Encrypt a PGP message

This module allows you to encrypt a message using public and private keys.

| Private key |Enter the sender's private key. This can authenticate the sender's identity. |
|---|---|
| Public key |Enter the recipient's public key.  |
| Message |Enter the message that you want to encrypt. |

### Decrypt a PGP message

This module allows you to decrypt a message using public and private keys.

| Private key |Enter the recipient's private key.  |
|---|---|
| Public key |Enter the recipient's public key. This can authenticate the sender's identity. |
| Message |Map the message that you want to decrypt.  |

&nbsp;
