---
user-type: administrator
product-area: system-administration;setup
navigation-topic: security
title: Set up Azure Active Directory with Enhanced Authentication
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
---

# Set up Azure Active Directory with Enhanced Authentication

{{important-admin-console-onboard}}

When Adobe Workfront expects a different signature method for the SAML response, you need to change which parts of the SAML token are digitally signed by Azure Active Directory (AD).

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Set up Azure Active Directory with Enhanced Authentication

1. Open the Azure portal and sign in as a global administrator or co-administrator.
1. Select **All services** at the top-left side of the **navigation pane** to open the **Azure AD extension**.

1. Type 

   ```
   Azure Active Directory
   ```

   in the filter search box, and then select **Azure Active Directory**.

1. In the **Azure AD navigation pane** select **Enterprise Applications**.

1. Click **All Applications** to view a list of your apps.
1. If you don't see Workfront, use the **Filter control** at the top of the **All Applications List**, set the **Show option** to **All Applications**.

1. Select **Workfront** to configure Workfront for single sign-on.
1. After Workfront loads, select **Single sign-on** in the **Azure AD navigation pane**.

1. Under **SAML Signing Certificate**, click **Show advanced certificate signing settings**.

1. In the **Signing Option list** select **Sign SAML response**.

1. Workfront requires Sign SAML response.

The next time that you sign in to Workfront, Azure AD will sign the part of the SAML response that you selected.
