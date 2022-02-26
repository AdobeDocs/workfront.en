---
filename: set-up-azure-active-directory-enhanced-authentication
user-type: administrator
product-area: system-administration;setup
navigation-topic: security
title: Set up Azure Active Directory with Enhanced Authentication
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Set up Azure Active Directory with Enhanced Authentication

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

When *Adobe Workfront* expects a different signature method for the SAML response, you need to change which parts of the SAML token are digitally signed by Azure Active Directory (AD).

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
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Set up Azure Active Directory with Enhanced Authentication

<ol> 
 <li value="1">Open the Azure portal and sign in as a global administrator or co-administrator.</li> 
 <li value="2">Select <span class="bold">All services</span> at the top-left side of the <span class="bold">navigation pane</span> to open the <span class="bold">Azure AD extension</span>.</li> 
 <li value="3">Type <code>Azure Active Directory</code> in the filter search box, and then select <span class="bold">Azure Active Directory</span>.</li> 
 <li value="4"> In the <span class="bold">Azure AD navigation pane</span> select <span class="bold">Enterprise Applications</span>.</li> 
 <li value="5">Click <span class="bold">All Applications</span> to view a list of your apps.</li> <note type="note">
  If you don't see 
  <em>Workfront</em>, use the 
  <span class="bold">Filter control</span> at the top of the 
  <span class="bold">All Applications List</span>, set the 
  <span class="bold">Show option</span> to 
  <span class="bold">All Applications</span>.
 </note> 
 <li value="6">Select <span class="bold">Workfront</span> to configure <em>Workfront</em> for single sign-on.</li> 
 <li value="7">After <em>Workfront</em> loads, select <span class="bold">Single sign-on</span> in the <span class="bold">Azure AD navigation pane</span>.</li> 
 <li value="8">Under <span class="bold">SAML Signing Certificate</span>, click <span class="bold">Show advanced certificate signing settings</span>.</li> 
 <li value="9">In the <span class="bold">Signing Option list</span> select <span class="bold">Sign SAML response</span>.</li> <note type="note">
  <em>Workfront</em> requires Sign SAML response.
 </note> 
</ol>

The next time that you sign in to *Workfront*, Azure AD will sign the part of the SAML response that you selected.
