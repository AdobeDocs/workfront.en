---
filename: view-username
content-type: reference
product-area: reporting;user-management;resource-management
navigation-topic: custom-view-filter-and-grouping-samples
title: View: username
description: As an administrator, people may ask you to remind them of their username and password. While the password cannot be displayed in any report, you may find it useful to create a view that displays the username for quick access to this information.
hidefromtoc: true
---

# View: username

As an administrator, people may ask you to remind them of their username and password. While the password cannot be displayed in any report, you may find it useful to create a view that displays the username for quick access to this information.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## View username

To apply this view to a user list:

1. Navigate to a list of users.
1. Expand the View drop-down menu, then click **New View**.
1. In the **Column Preview** area, eliminate all the columns in the view, except for one.
1. On the remaining column, click **Switch to Text Mode**.
1. Mouse over the text of the column and click **Click to edit text**.
1. Select all text in the&nbsp;**Text Mode** editor, and paste the text below:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=emailaddr<br>column.1.linkedname=direct<br>column.1.listsort=string(emailAddr)<br>column.1.namekey=emailaddr.abbr<br>column.1.querysort=emailAddr<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=emailAddr<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=Username<br>column.2.linkedname=direct<br>column.2.listsort=string(username)<br>column.2.name=Username<br>column.2.querysort=username<br>column.2.shortview=false<br>column.2.stretch=100<br>column.2.valuefield=username<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. (Optional) To view the SSO Username, replace the code in the lines that start with **column.2.valuefield**&nbsp;to the following code:
   <pre>column.2.description=ssoUsername<br>column.2.linkedname=direct<br>column.2.listsort=string(ssoUsername)<br>column.2.name=ssoUsername<br>column.2.querysort=ssoUsername<br>column.2.shortview=false<br>column.2.stretch=100<br>column.2.valuefield=ssoUsername<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. Click **Save View**.

   The view displays the name, email address and username of the users.

   ![username_custom_view.png](assets/username-custom-view-350x55.png)

