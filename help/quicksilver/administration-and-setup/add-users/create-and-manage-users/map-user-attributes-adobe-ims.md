---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Map user attributes and auto-provision new users
description: Using single sign-on (SSO), you can pass attributes from your identity provider's Active Directory to your Adobe Workfront users. You can also add new users to Workfront using the Auto-Provision option (also called Just In Time Provisioning or JIT).
author: Becky
feature: System Setup and Administration
role: Admin
---
# Map user attributes (Adobe IMS)

Using single sign-on (SSO), you can pass attributes from your identity provider's Active Directory to your Adobe Workfront users.

### Map user attributes (Adobe organizations)

1. Click the **Main Menu** icon ![](assets/main-menu-left.png) in the upper-left corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **System** > **Single Sign-On (SSO)**.

1. Select the **Adobe** tab.

1. To create a new attribute mapping, click **Add Mapping**.

1. Click the arrow next to the field and select the [!DNL Workfront] field that you want to map to. 

1. (Optional) If you want to create more than one rule for a given field, click the arrow next to **Always** and select the operator that you want the rule to use. 

1. (Conditional) If you have selected operator besides Always, select the Workfront field and value that the operator applies to.

   >[!NOTE]
   >
   >The operators `Is Truthy` and `Is Falsy` do not require values.












