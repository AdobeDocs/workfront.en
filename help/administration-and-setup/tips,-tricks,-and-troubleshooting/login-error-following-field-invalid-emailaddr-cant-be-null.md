---
filename: login-error-following-field-invalid-emailaddr-cant-be-null
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
---




# Login Error: The following fields are invalid: emailAddr cannot be null {#login-error-the-following-fields-are-invalid-emailaddr-cannot-be-null}



## Problem&nbsp; {#problem}

When I try to log into `Workfront` with my URL (https://customerdomain.my.workfront.com), I am redirected to the SAML login portal and then redirected back to `Workfront` with the following error:


"Let's try that again. The following fields are invalid:&nbsp;emailAddr cannot be null."


## Cause {#cause}

This error is caused by an incorrect item in the Map User Attributes&nbsp;area of the SAML 2.0 configuration. For more information about mapping user attributes for SAML 2.0, see [Configure Workfront with SAML 2.0](configure-workfront-saml-2.md).


## Solution {#solution}

Update the Attribute Mapping for the email address, and click **Save**.
