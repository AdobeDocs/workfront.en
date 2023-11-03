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

1. Click the arrow next to the Workfront field name and select the [!DNL Workfront] field that you want to map to. 

1. (Optional) If you want to create more than one rule for a given field, click the arrow next to **Always** and select the operator that you want the rule to use. 

1. (Conditional) If you have selected an operator besides Always, select the Workfront field and value that the operator applies to.

   >[!NOTE]
   >
   >The operators `Is Truthy` and `Is Falsy` do not require values.

1. Select whether you want to apply the value of a field in your identity manager to the Workfront field, or if you want to apply a specific constant value.

1. Enter the name of the identity manager field that you want to apply, or enter the text of the constant value you want to apply.

1. (Optional) To add more rules for the same Workfront field, click **Add New Rule**, and follow steps 4-9.
   
   >[!IMPORTANT]
   >
   > * Any rule below an Always rule will be ignored. If you have an Always rule, you must move it to the bottom of the list of rules. You can move rules in the list by clicking the three-dot menu to the right of the rule and move the rule up or down.
   > * To create a rule in the middle of the list, click the three-dot menu next to the rule that you want to be above or below the new rule, and select **Add Rule Above** or **Add Rule Below**.

1. To delete a rule, click the three-dot menu next to the rule you want to delete, and select **Delete**.

1. To save, scroll to the top of the page and click **Save**.










