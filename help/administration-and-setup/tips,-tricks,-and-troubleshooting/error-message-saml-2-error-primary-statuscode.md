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




## Cause {#cause}

1: Secure hash algorithm is set to SHA-256


### Solution {#solution}




1. In Windows, click **Start** > **Administration** > **ADFS&nbsp;2.0 Management**.  
   The ADFS 2.0 Management dialog box is displayed.

1. Select **Trust Relationship** > **Relying Party Trusts** in the left-hand pane.

1. Right-click on the relying party trust related to `Workfront`, then select **Properties**.

1. Click on the **Advanced**&nbsp;tab, then select **SHA-1 **from&nbsp;the **Secure hash algorithm** drop-down menu.  
   ![](assets/1-600x491.png)






## Cause 2: ADFS Signing Certificate is about to expire and has been replaced by a new Certificate with overlapping dates {#cause-adfs-signing-certificate-is-about-to-expire-and-has-been-replaced-by-a-new-certificate-with-overlapping-dates}



### Solution {#solution-1}

The `Workfront` SSO Setup Page lists the certificate expiration date. If the certificate is about to expire, you need to manually pull the New Signing Certificate from the ADFS Server:



1. In Windows, click **Start** > **Administration** > **ADFS&nbsp;2.0 Management**.  
   The ADFS 2.0 Management dialog box is displayed.

1. Select **Trust Relationship** > **Relying Party Trusts** in the left-hand pane.

1. Right-click on the relying party trust related to `Workfront`, and select **Properties**.

1. Click on the **Signature** tab.
1. Click on the name of the Signing Certificate, and click **View**.
1. Click Copy to **File**..., and select **Next**.

1. Select **Base-64 encoded x.509 (CER)**, and click **Next**.

1. Specify the file name, and click **Next**.
1. Click **Finish**.
1. In `Workfront`, navigate to **Setup** > **System** > **Single Sign-On (SSO)** and manually upload the Signing Certificate.





## Cause 3: Certificate revocation check is failing {#cause-certificate-revocation-check-is-failing}



### Solution {#solution-2}

Run the following PowerShell Commands replacing domain with their Domain:



1. In Windows, click **Start** > **Administrative Tools** > **Windows Powershell Modules**.

1. In the Powershell window, type:   
   *Set-ADFSRelyingPartyTrust -TargetIdentifier "DOMAIN.my.workfront.com/SAML2" -SigningCertificateRevocationCheck None&nbsp;*

1.  `<li value="1">The "DOMAIN.my.workfront.com/SAML2" will be the identifier name of your relying party trust as displayed int he ADFS Management console.</li>` 
1. Then run  
   *Set-ADFSRelyingPartyTrust -TargetIdentifier "DOMAIN.my.workfront.com/SAML2" -EncryptionCertificateRevocationCheck None&nbsp;*



