---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Map User Attributes
description: Using single sign-on (SSO), you can pass attributes from your identity provider's Active Directory to your Adobe Workfront users.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
TQID: https://experienceleague.adobe.com/nuU1cn2BDPN7k-gr7a3t5JFR54zD9gHaxBeESEL53p0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Map user attributes

<!--Audited 2/2024-->

Using single sign-on (SSO), you can pass attributes from your identity provider's Active Directory to your Adobe Workfront users. 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>You must be a Workfront administrator</p></td>
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tips for mapping attributes

Keep the following in mind when mapping attributes:

* Always test in a Preview sandbox or a Customer Refresh (CR) sandbox.
* Test with both administrator and non-administrator accounts to confirm that you are mapping attributes correctly.
* Attributes that are mapped are applied each time a user signs in via single-sign on.

   Example: if you are mapping "last name" and update their name in Workfront without updating the value in their Identity Provider, then the last name will get overwritten to match the value of whatever is in the Identity Provider the next time the user signs in.

## Map user attributes for your organization

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-left.png) in the upper-left corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).

1. Click **System** > **Single Sign-On (SSO)**.

1. Select the **Adobe** tab.

1. (Optional and conditional) If your organization had attribute mapping configured in the classic experience and you want to copy that attribute mapping to the Adobe unified experience, click **Migrate Mappings**. You can then discard, delete, or edit these mappings.

   >[!NOTE]
   >
   >We recommend migrating mappings the first time you configure mappings in the Adobe unified experience. There is no harm in migrating them again later, but migrating them more than once is unnecessary.
 
1. To create a new attribute mapping, click **Add Mapping**.

1. Click the arrow next to the Workfront field name and select the [!DNL Workfront] field that you want to map to. 

1. (Optional) If you want to create more than one rule for a given field, click the arrow next to **Always** and select the operator that you want the rule to use. 

1. (Conditional) If you have selected an operator besides Always, select the Workfront field and value that the operator applies to.

   >[!NOTE]
   >
   >The operators `Is Truthy` and `Is Falsy` do not require values.

1. Select whether you want to apply the value of an attribute in your identity manager to the Workfront field, or if you want to apply a specific constant value.

1. Enter the name of the identity manager field that you want to apply, or enter the text of the constant value you want to apply.

1. (Optional) To add more rules for the same Workfront field, click **Add New Rule**, and follow steps 4-9.
   
   >[!IMPORTANT]
   >
   > * Any rule below an Always rule will be ignored. If you have an Always rule, you must move it to the bottom of the list of rules. You can move rules in the list by clicking the three-dot menu to the right of the rule and move the rule up or down.
   > * To create a rule in the middle of the list, click the three-dot menu next to the rule that you want to be above or below the new rule, and select **Add Rule Above** or **Add Rule Below**.

1. To delete a rule, click the three-dot menu next to the rule you want to delete, and select **Delete**.
1. To delete a mapping, click the **Delete** icon that is on the card for that mapping.

1. To save, scroll to the top of the page and click **Save**.


