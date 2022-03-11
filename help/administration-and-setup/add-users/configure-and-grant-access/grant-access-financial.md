---
filename: grant-access-financial
title: Grant access to financial data
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
title: Grant access to financial data
description: As an Adobe Workfront administrator, you can define a user’s access to the following through the user's access level, as explained in Access levels overview:
---

# Grant access to financial data

As an `Adobe Workfront administrator`, you can define a user’s access to the following through the user's access level, as explained in [Access levels overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md):

* Financial information on projects in `Workfront`
* Resource budgeting information in the Resource Planning tools

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Considerations for granting access to financial data

Consider the following when granting users access to financial data in `Workfront`:

* A user whose access level doesn't allow access to financial data cannot create a risk for a project. For more information, see [Create and edit risks on projects](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* You can also use an access level to determine which Resource Management activities a user can employ to budget or view resource allocation. For information, see [Grant access to Resource Management](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Configure user access to financial data using a custom access level

<ol> 
 <li value="1"> <p>Begin creating or editing the access level, as explained in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </li> 
 <li value="2"> <p>Click the gear icon <img src="assets/gear-icon-settings.png"> on the <span class="bold">View</span> or <span class="bold">Edit</span> button to the right of <span>Financial Data</span>, then select the abilities you want to grant under <b>Fine-tune your settings</b>.</p>  </li> 
 <li value="3"> <p>(Optional) In the <span class="bold">Allow administrative access for</span> area, select the following options:<![CDATA[
]]></p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Exchange rates</td> 
     <td> <p>Add new currency in <span>Workfront</span>.</p> <p>Without this access, the user can only add an existing currency to a project they create.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Expenses</td> 
     <td> <p>View all expenses on objects in <span>Workfront</span>.<br></p> <p>This does not allow the user to create new Expense Types.<br></p> <p>Without this access, the user can only view the following:</p> 
      <ul> 
       <li>Expenses on projects, tasks or issues they manage</li> 
       <li>Their own expenses</li> 
       <li>The expenses of their subordinates</li> 
      </ul> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4"> <p>(Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref" data-mc-variable-override="">Configure access to Adobe Workfront</a>, such as <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref" data-mc-variable-override="">Grant access to tasks</a> and <a href="#" class="MCXref xref selected" data-mc-variable-override="">Grant access to financial data</a>.</p> </li> 
 <li value="5"> <p>When you are finished, click Save.</p> <p>After the access level is created, you can assign it to a user. For more information, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Edit a user's profile</a>.<br></p> </li> 
</ol>

## Access to shared financial information

You can share financial information on a project, task, or issue with other users by granting them permissions to it, as explained in [Share financial permissions on an object in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

When you share any object with another user, the recipient’s rights on it are determined by a combination of two things:

* The permissions that you grant to your recipient for the object
* The recipient’s access level settings for the object's type

## Access to financial information by license type

For information about what users in each access level can do with financial information, see the section [Financial data](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) in the article [Functionality available for each object type](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Access to financial information by setting

The following information can help you understand how to use the Access level settings to control users' access to financial data.

### No access

A user with no access to financial data does not have access to the following:

<ul> 
 <li>Finance section under Project and Task objects</li> 
 <li>Business case</li> 
 <li>Billing rates and Billing records</li> 
 <li> <p>Cost per hour and billing per hour on User preferences </p> <p>You can configure this using the gear icon <img src="assets/gear-icon-settings.png"> on the View button in step 4 above.</p> </li> 
 <li> <p>Cost per hour and billing per hour on Job Roles</p> <p>You can configure this using the gear icon <img src="assets/gear-icon-settings.png"> on the View button in step 4 above.</p> </li> 
</ul>

### View access

A user with View access to financial data can view (not edit) the following:

<ul> 
 <li>Finance section under Project and Task objects</li> 
 <li>Business case</li> 
 <li>Billing rates and Billing records</li> 
 <li> <p>Cost per hour and billing per hour on User preferences </p> <p>You can configure this using the gear icon <img src="assets/gear-icon-settings.png"> on the View button in step 4 above.</p> </li> 
 <li> <p>Cost per hour and billing per hour on Job Roles</p> <p>You can configure this using the gear icon <img src="assets/gear-icon-settings.png"> on the View button in step 4 above.</p> </li> 
</ul>

### Edit access

A user with Edit access to financial data can view and edit the following:

<ul> 
 <li>Finance section under Project and Task objects</li> 
 <li>Business case</li> 
 <li>Billing rates and Billing records</li> 
 <li> <p>Cost per hour and billing per hour on User preferences</p> <p>You can configure this using the gear icon <img src="assets/gear-icon-settings.png"> on the Edit button in step 4 above.</p> </li> 
 <li> <p>Cost per hour and billing per hour on Job Roles</p> <p>You can configure this using the gear icon <img src="assets/gear-icon-settings.png"> on the Edit button in step 4 above.</p> </li> 
</ul>

