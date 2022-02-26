---
filename: add-user-to-an-organization
product: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Add a user to an organization
description: You must have the following access to use the functionality in this article:
---

# Add a user to an organization

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p>Plan, Work</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront Fusion</em> license**</td> 
   <td> <p><em>Workfront Fusion for Work Automation and Integration</em>,</p> <draft-comment>
     <p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p>
    </draft-comment><p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <em>Adobe Workfront Fusion</em> as well as <em>Adobe Workfront</em> to use functionality described in this article.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

&#42;&#42;For information on *Adobe Workfront Fusion* licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Add users to an organization

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add2" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<h3><a name="Add"></a>Add a user to an organization that has been onboarded to the Adobe Business Platform</h3>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<h3><a name="Add2"></a>Add a user to an organization that has not been onboarded to the Adobe Business Console</h3>
</div>
-->

The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform.

* [Add a user to an organization that has been onboarded to the Adobe Business Platform](#add) 
* [Add a user to an organization that has not been onboarded to the Adobe Business Console](#add2)

### Add a user to an organization that has been onboarded to the Adobe Business Platform

If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.

For instructions on adding a user in the Adobe Admin Console:

* See [Create users in Workfront with the Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create)
* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
* Contact your Adobe Admin Console Administrator.

For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

### Add a user to an organization that has not been onboarded to the Adobe Business Console

To add users to the organization, you must be an administrator at the organization you want to add users to. For information about roles, see [Organization roles](../../workfront-fusion/organizations/organization-roles.md).

To add a user to the organization:

1. Navigate to `Organizations` in the menu and select the organization you want to add a user to.
1. Open the `Users` tab in your Dashboard.
1. Click `Invite a new user`, fill the form (Email, Message, Role), and send the invitation by clicking `Send`.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>If you do not see the Invite a new user button, your organization has been onboarded to the Adobe Business Platform. </p>
   <p>For instructions on adding a user to an organization that has been onboarded to the Adobe Business Platform, see <a href="#add" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a></p>
   </div>
   -->

   If you do not see the Invite a new user button, your organization has been onboarded to the Adobe Business Platform.

   For instructions on adding a user to an organization that has been onboarded to the Adobe Business Platform, see [Add a user to an organization that has been onboarded to the Adobe Business Platform](#add)
   The user receives an invitation email where they can accept the invitation by clicking an Accept the Role button.

