---
filename: error-message-couldnt-validate-xml-digital-signature
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
---




# Error message: Couldn't validate XML digital signature {#error-message-couldnt-validate-xml-digital-signature}



## Problem {#problem}

You are unable to establish a successful connection to ADFS.


![error_message.png](assets/error-message.png)




>[!NOTE]
>
>If you establish a successful test connection and you are still experiencing issues, you might have incorrect attribute mappings or issues with the federation IDs. Contact customer support with questions.





* [Cause](#cause-1) 
* [Cause 2: The certificate is signed using DSA when Workfront is expecting an RSA signature](#cause-2dsa/rsa) 
* [Cause 3: XML Data is incorrect](#cause-3-incorrect-xml) 
* [Cause 4: The request could not be performed due to an error on the SAML side](#cause-4-issue-with-saml) 




## Cause {#cause}

1: The certificate is incorrect


### Solution {#solution}

Manually retrieve the Signing Certificate from the ADFS Server:



1. In Windows, click **Start** > **Administration** > **ADFS&nbsp;2.0 Management**.  
   The ADFS 2.0 Management dialog box is displayed.

1. Select **Trust Relationship** > **Relying Party Trusts** in the left-hand pane.

1. Right-click on **Relying Party Trust**, and select **Properties**.

1. Click on the **Signature** tab.
1. Click on the name of the Signing Certificate, and click **View**.
1. Click Copy to **File**..., and select **Next**.

1. Select **Base-64 encoded x.509 (CER)**, and click **Next**.

1. Specify the file name, and click **Next**.
1. Click **Finish**.
1. In `Workfront`, navigate to **Setup** > **System** > **Single Sign-On (SSO)** and manually upload the Signing Certificate.





## Cause 2: The certificate is signed using DSA when `Workfront` is expecting an RSA signature {#cause-the-certificate-is-signed-using-dsa-when-workfront-is-expecting-an-rsa-signature}



### Solution {#solution-1}

Recreate the certificate and use the RSA signature instead of the DSA.


## Cause 3: XML Data is incorrect {#cause-xml-data-is-incorrect}



### Solution {#solution-2}

Re-export and re-import the XML metadata from the ADFS management system.


## Cause 4: The request could not be performed due to an error on the SAML side {#cause-the-request-could-not-be-performed-due-to-an-error-on-the-saml-side}



### Solution {#solution-3}

Contact your SAML provider.
