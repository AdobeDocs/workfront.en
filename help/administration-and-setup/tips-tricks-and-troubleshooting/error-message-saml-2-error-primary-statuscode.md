---
filename: error-message-saml-2-error-primary-statuscode
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Error message: SAML 2.0 error: Primary StatusCode
description: You are unable to establish a successful connection to ADFS.
---

# Error message: SAML 2.0 error: Primary StatusCode

## Problem

You are unable to establish a successful connection to ADFS.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>If you establish a successful test connection and you are still experiencing issues, you might have incorrect attribute mappings or issues with the federation IDs. Contact customer support with questions.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cause 1: Secure hash algorithm is set to SHA-256

### Solution

<ol> 
 <li value="1">In Windows, click <span class="bold">Start</span> > <span class="bold">Administration</span> > <span class="bold">ADFS&nbsp;2.0 Management</span>.<br>The ADFS 2.0 Management dialog box is displayed.</li> 
 <li value="2">Select <span class="bold">Trust Relationship</span> > <span class="bold">Relying Party Trusts</span> in the left-hand pane.</li> 
 <li value="3">Right-click on the relying party trust related to <em>Adobe Workfront</em>, then select <span class="bold">Properties</span>.</li> 
 <li value="4">Click on the <span class="bold">Advanced</span>&nbsp;tab, then select <span class="bold">SHA-1</span> from&nbsp;the <span class="bold">Secure hash algorithm</span> drop-down menu.<br><img src="assets/1-350x287.png" style="width: 350;height: 287;"></li> 
</ol>

## Cause 2: ADFS Signing Certificate is about to expire and has been replaced by a new Certificate with overlapping dates

### Solution

The *Workfront* SSO Setup Page lists the certificate expiration date. If the certificate is about to expire, you need to manually pull the New Signing Certificate from the ADFS Server:

1. In Windows, click `Start` > `Administration` > `ADFS 2.0 Management`.  
   The ADFS 2.0 Management dialog box is displayed.

1. Select `Trust Relationship` > `Relying Party Trusts` in the left-hand pane.

1. Right-click on the relying party trust related to *Workfront*, and select `Properties`.

1. Click on the `Signature` tab.
1. Click on the name of the Signing Certificate, and click `View`.
1. Click Copy to `File`..., and select `Next`.

1. Select `Base-64 encoded x.509 (CER)`, and click `Next`.

1. Specify the file name, and click `Next`.
1. Click `Finish`.
1. In *Workfront*, navigate to `Setup` > `System` > `Single Sign-On (SSO)` and manually upload the Signing Certificate.

## Cause 3: Certificate revocation check is failing

### Solution

Run the following PowerShell Commands replacing domain with their Domain:

1. In Windows, click `Start` > `Administrative Tools` > `Windows Powershell Modules`.

1. In the Powershell window, type:   
   *Set-ADFSRelyingPartyTrust -TargetIdentifier "DOMAIN.my.workfront.com/SAML2" -SigningCertificateRevocationCheck None&nbsp;*

1. `<li value="1">The "DOMAIN.my.workfront.com/SAML2" will be the identifier name of your relying party trust as displayed int he ADFS Management console.</li>` 
1. Then run  
   *Set-ADFSRelyingPartyTrust -TargetIdentifier "DOMAIN.my.workfront.com/SAML2" -EncryptionCertificateRevocationCheck None&nbsp;*

