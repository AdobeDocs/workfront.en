---
filename: view-assigned-users-company-home-group
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: View: assigned user's Company and Home Group
description: This task view displays the Company and Home Group of the Primary Owner of the task. These are values that are not available in the standard interface, but they are accessible through text mode.
---

# View: assigned user's Company and Home Group

This task view displays the Company and Home Group of the Primary Owner of the task. These are values that are not available in the standard interface, but they are accessible through&nbsp;text mode.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## View assigned user's Company and Home Group

1. Go to a list of tasks.
1. From the `View` drop-down menu, select `New View`.

1. In the `Column Preview` area, eliminate all columns except for one.
1. Click the header of the remaining column, then click `Switch to Text Mode`.
1. Mouse over the text mode area, and click `Click to edit text`.
1. Remove the text you find in the `Text Mode` box, and replace it with the following code:
   <pre><em>column.0.descriptionkey=name</em><br><em> column.0.link.linkproperty.0.name=ID</em><br><em> column.0.link.linkproperty.0.valuefield=ID</em><br><em> column.0.link.linkproperty.0.valueformat=int</em><br><em> column.0.link.lookup=link.view</em><br><em> column.0.link.valuefield=objCode</em><br><em> column.0.link.valueformat=val</em><br><em> column.0.linkedname=direct</em><br><em> column.0.listsort=string(name)</em><br><em> column.0.namekey=name.abbr</em><br><em> column.0.querysort=name</em><br><em> column.0.shortview=false</em><br><em> column.0.stretch=100</em><br><em> column.0.valuefield=name</em><br><em> column.0.valueformat=HTML</em><br><em> column.0.width=150</em><br><em> column.1.descriptionkey=assignedto</em><br><em> column.1.link.linkproperty.0.name=ID</em><br><em> column.1.link.linkproperty.0.valuefield=assignedTo:ID</em><br><em> column.1.link.linkproperty.0.valueformat=int</em><br><em> column.1.link.lookup=link.view</em><br><em> column.1.link.valuefield=assignedTo:objCode</em><br><em> column.1.link.valueformat=val</em><br><em> column.1.linkedname=assignedTo</em><br><em> column.1.listsort=nested(assignedTo).string(name)</em><br><em> column.1.namekey=assignedto</em><br><em> column.1.querysort=assignedTo:name</em><br><em> column.1.shortview=false</em><br><em> column.1.stretch=0</em><br><em> column.1.valuefield=assignedTo:name</em><br><em> column.1.valueformat=HTML</em><br><em> column.1.width=150</em><br><em> column.2.description=Assigned To Company</em><br><em> column.2.displayname=Assigned To Company</em><br><em> column.2.linkedname=assignedTo:company</em><br><em> column.2.listsort=nested(assignedTo:company).string(name)</em><br><em> column.2.namekey=assignedto</em><br><em> column.2.querysort=assignedTo:company:name</em><br><em> column.2.shortview=false</em><br><em> column.2.stretch=0</em><br><em> column.2.valuefield=assignedTo:company:name</em><br><em> column.2.valueformat=HTML</em><br><em> column.2.width=150</em><br><em> column.3.description=Assigned To Home Group</em><br><em> column.3.displayname=Assigned To Home Group</em><br><em> column.3.linkedname=assignedTo:homeGroup</em><br><em> column.3.listsort=nested(assignedTo:homeGroup).string(name)</em><br><em> column.3.namekey=assignedto</em><br><em> column.3.querysort=assignedTo:homeGroup:name</em><br><em> column.3.shortview=false</em><br><em> column.3.stretch=0</em><br><em> column.3.valuefield=assignedTo:homeGroup:name</em><br><em> column.3.valueformat=HTML</em><br><em> column.3.width=150</em></pre>

1. Click `Save Changes`.

