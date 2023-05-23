---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: display Program and Portfolio information in a task view'
description: This task view displays the Program and Portfolio that are associated with the project of the task. This information is not available in the report builder when building a task view. This is information is available only in text mode.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
---
# View: display Program and Portfolio information in a task view

This task view displays the Program and Portfolio that are associated with the project of the task. This information is not available in the report builder when building a task view. This is information is available only in text mode.

The view also provides links to the Project, Program, and Portfolio from a task list.

![](assets/view--program-and-portfolio-350x116.png)

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request to modify a view </p>
   <p>Plan to modify a report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Display Program and Portfolio information in a task View

To apply this view to a task list:

1. Go to a list of tasks.
1. From the&nbsp;**View**&nbsp;drop-down menu, select&nbsp;**New View**.

1. In the**Column Preview**&nbsp;area, eliminate all columns except for one.
1. Click the header of the remaining column, then click **Switch to Text Mode**.
1. Mouse over the text mode area, and click&nbsp;**Click to edit text**.
1. Remove the text you find in the&nbsp;**Text Mode**&nbsp;box, and replace it with the following code:  
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=project<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=project:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=project:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=project<br>column.1.listsort=nested(project).string(name)<br>column.1.namekey=project<br>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=project:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=program<br>column.2.displayname=Program<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=project:program:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=project:program:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=project<br>column.2.listsort=nested(project:program).string(name)<br>column.2.namekey=project<br>column.2.querysort=project:program:name<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=project:program:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.descriptionkey=portfolio<br>column.3.displayname=Portfolio<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=project:portfolio:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=project:portfolio:objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=project<br>column.3.listsort=nested(project:portfolio).string(name)<br>column.3.namekey=project<br>column.3.querysort=project:portfolio:name<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=project:portfolio:name<br>column.3.valueformat=HTML<br>column.3.width=150&nbsp;</pre>

1. Click&nbsp;**Save View**.
