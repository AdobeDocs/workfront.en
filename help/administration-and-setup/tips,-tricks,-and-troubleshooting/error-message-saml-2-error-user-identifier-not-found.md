---
filename: error-message-saml-2-error-user-identifier-not-found
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
---




# Error Message: SAML 2.0 Error: User Identifier Not Found {#error-message-saml-error-user-identifier-not-found}



## Problem {#problem}

You are unable to establish a successful connection to ADFS.


![identifier_not_found.png](assets/identifier-not-found.png)




>[!NOTE]
>
>If you establish a successful test connection and you are still experiencing issues, you might have incorrect attribute mappings or issues with the federation IDs. Contact customer support with questions.




## Cause: {#cause}

Claims on the ADFS server are incorrect


## Solution {#solution}

On the ADFS server, make sure&nbsp;there is a claim for name ID:



1. In Windows, click **Start** > **Administration** > **ADFS&nbsp;2.0 Management**.  
   The ADFS 2.0 Management dialog box is displayed.

1. Select **Trust Relationship** > **Relying Party Trusts** in the left-hand pane.

1. Right-click on the relying party trust related to `Workfront`, and select **Edit Claim Rules**.

1. Verify the claim has an **Outgoing Claim Type** of **Name ID**.



![1.png](assets/1-600x491.png)

