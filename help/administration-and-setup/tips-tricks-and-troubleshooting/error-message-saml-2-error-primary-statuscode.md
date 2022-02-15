---
filename: error-message-saml-2-error-primary-statuscode
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
---



# Error message: SAML 2.0 error: Primary StatusCode {#error-message-saml-error-primary-statuscode}



## Problem {#problem}

You are unable to establish a successful connection to ADFS.


![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)




>[!NOTE]
>
>If you establish a successful test connection and you are still experiencing issues, you might have incorrect attribute mappings or issues with the federation IDs. Contact customer support with questions.




## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Cause 1: Secure hash algorithm is set to SHA-256 {#cause-secure-hash-algorithm-is-set-to-sha}



### Solution {#solution}




1. In Windows, click `Start` > `Administration` > `ADFS 2.0 Management`.  
   The ADFS 2.0 Management dialog box is displayed.

1. Select `Trust Relationship` > `Relying Party Trusts` in the left-hand pane.

1. Right-click on the relying party trust related to *`Adobe Workfront`*, then select `Properties`.

1. Click on the `Advanced` tab, then select `SHA-1`from the `Secure hash algorithm` drop-down menu.  
   ![](assets/1-350x287.png)






## Cause 2: ADFS Signing Certificate is about to expire and has been replaced by a new Certificate with overlapping dates {#cause-adfs-signing-certificate-is-about-to-expire-and-has-been-replaced-by-a-new-certificate-with-overlapping-dates}



### Solution {#solution-1}

The *`Workfront`* SSO Setup Page lists the certificate expiration date. If the certificate is about to expire, you need to manually pull the New Signing Certificate from the ADFS Server:



1. In Windows, click `Start` > `Administration` > `ADFS 2.0 Management`.  
   The ADFS 2.0 Management dialog box is displayed.

1. Select `Trust Relationship` > `Relying Party Trusts` in the left-hand pane.

1. Right-click on the relying party trust related to *`Workfront`*, and select `Properties`.

1. Click on the `Signature` tab.
1. Click on the name of the Signing Certificate, and click `View`.
1. Click Copy to `File`..., and select `Next`.

1. Select `Base-64 encoded x.509 (CER)`, and click `Next`.

1. Specify the file name, and click `Next`.
1. Click `Finish`.
1. In *`Workfront`*, navigate to `Setup` > `System` > `Single Sign-On (SSO)` and manually upload the Signing Certificate.





## Cause 3: Certificate revocation check is failing {#cause-certificate-revocation-check-is-failing}



### Solution {#solution-2}

Run the following PowerShell Commands replacing domain with their Domain:



1. In Windows, click `Start` > `Administrative Tools` > `Windows Powershell Modules`.

1. In the Powershell window, type:   
   *Set-ADFSRelyingPartyTrust -TargetIdentifier "DOMAIN.my.workfront.com/SAML2" -SigningCertificateRevocationCheck None&nbsp;*

1.  `<li value="1">The "DOMAIN.my.workfront.com/SAML2" will be the identifier name of your relying party trust as displayed int he ADFS Management console.</li>` 
1. Then run  
   *Set-ADFSRelyingPartyTrust -TargetIdentifier "DOMAIN.my.workfront.com/SAML2" -EncryptionCertificateRevocationCheck None&nbsp;*



