---
filename: share-financial-permissions-object
title: Share financial permissions on an object
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Share financial permissions on an object in Adobe Workfront
description: Your Adobe Workfront administrator can grant you access to view or edit financial data when assigning your access level. For more information, see Grant access to financial data.
---

# Share financial permissions on an object in Adobe Workfront

Your Adobe Workfront administrator can grant you access to view or edit financial data when assigning your access level. For more information, see [Grant access to financial data](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Along with the access level that users are granted, you can also grant them permissions to View or Manage finances for specific projects, tasks, or issues that you have access to share.

For information about what users in each access level can do with financial data, see the section [Financial data](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) in the article [Functionality available for each object type](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Access requirements

You must have the following to share financial data information on objects:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial&nbsp;Data</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Share an object and grant financial permissions

Consider the following when granting financial permissions to objects:

* You can grant financial permissions to projects, tasks, and issues. 
* Permissions can be inherited: if you have View Finance permissions to a project, you automatically inherit View Finance permissions to the tasks and issues on the project.

To grant financial permissions to an object:

<ol> 
 <li value="1">Go to a task, project, or issue that you want to share with others.</li> 
 <li value="2"> Near the name of the object, click the More menu , then click Sharing. </li> 
 <li value="3"> <p>In the <span class="bold">Give <Object name>&nbsp;access to</span> field start typing the name of a user, team, role, group or a company that you want to share the object with.</p> <note type="tip">
   You can share an object only with active users, teams, 
   <span>roles,</span> or companies.
  </note> </li> 
 <li value="4">If a drop-down menu appears to the right of the name you selected, click one of the following options that is available: 
  <ul>
   <li><span class="bold">View it</span></li>
   <li><span class="bold">Contribute to it</span></li>
   <li><p><span class="bold">Manage it&nbsp;</span></p><p><img src="assets/12.png" alt="">&nbsp; &nbsp; &nbsp;<img src="assets/13.png" alt=""><img src="assets/14.png" alt=""></p></li>
  </ul></li> 
 <li value="5">In the same drop-down menu, click <span class="bold">Advanced Settings</span>, then do one of the following: 
  <ul>
   <li>If you selected one of the three options in the previous step, make sure <span class="bold">View Finance</span> is selected.</li>
   <li>If you selected <span class="bold">Manage Finance</span> in the previous step, make sure <span class="bold">Manage Finance</span> is selected.</li>
  </ul></li> 
 <li value="6">Click <span class="bold">Save</span>.<br></li> 
</ol>

## Financial permission for all sharing levels

The following table displays what financial permissions users gain when you grant them View, Contribute, or Manage permissions on objects:&nbsp;

<table cellspacing="15"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><span class="bold">Actions</span> </th> 
   <th><span class="bold">Manage</span> </th> 
   <th><span class="bold">Contribute</span> </th> 
   <th><span class="bold">View</span> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Manage Billing Records</td> 
   <td>✓</td> 
   <td> <p>&nbsp;</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Manage/ View Role Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Manage/ View User Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>View Finance</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>&nbsp;✓</td> 
  </tr> 
  <tr> 
   <td>View information by Cost in the Resource Planning tools</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Budget resources in the Resource Planning tools*</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>View resources in the Resource Planning tools*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Requires additional Resource Management access.

For information about Resource Management access, see [Grant access to Resource Management](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
