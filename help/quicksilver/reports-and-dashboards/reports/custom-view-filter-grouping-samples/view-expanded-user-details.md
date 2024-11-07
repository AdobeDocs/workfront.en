---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Expanded User Details'
description: This User view displays information about your users. In addition to their name, access levels, and Company, it also shows lists of their Groups, Teams, and Job Roles.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
---
# View: expanded user details

<!--Audited: 11/2024-->

This User view displays information about your users. In addition to their name, access levels, and Company, it also shows lists of their Groups, Teams, and Job Roles.

![expanded_user_view.png](assets/expanded-user-view-350x75.png)

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

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
   <td> <p>New:<ul><li>Contributor to modify a view</li><li>Standard to modify a report</li></ul></p><p>Or</p>Current:<ul><li>Request to modify a view</li><li>Plan to modify a report</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## View expanded user details

To apply this view:

1. Go to a list of users.
1. From the **View** drop-down menu, select **New View**.

1. In the**Column Preview** area, eliminate all columns except for one.
1. Click the header of the remaining column, then click **Switch to Text Mode** > **Edit Text Mode**.
1. Remove the text you find in the **dit Text Mode** box, and replace it with the following code: 

   ```
   column.0.descriptionkey=name 
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=0
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=accesslevel
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=accessLevel:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=accessLevel:objCode
   column.1.link.valueformat=val
   column.1.linkedname=accessLevel
   column.1.listsort=string(displayName)
   column.1.namekey=accesslevel
   column.1.querysort=name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=accessLevel:displayName
   column.1.valueformat=HTML
   column.1.viewalias=accessLevel:displayName
   column.1.width=100
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.value=val(objCode)
   column.2.listdelimiter=
   column.2.listmethod=nested(userGroups).lists
   column.2.namekey=group.plural
   column.2.stretch=50
   column.2.type=iterate
   column.2.valuefield=group:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.displayname=Teams
   column.3.listdelimiter=
   column.3.listmethod=nested(teams).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={name}
   column.3.valueformat=HTML
   column.4.link.linkproperty.0.name=ID
   column.4.link.linkproperty.0.valuefield=ID
   column.4.link.linkproperty.0.valueformat=int
   column.4.link.lookup=link.view
   column.4.link.value=val(objCode)
   column.4.listdelimiter=
   column.4.listmethod=nested(userRoles).lists
   column.4.namekey=jobrole.plural
   column.4.stretch=50
   column.4.type=iterate
   column.4.valuefield=role:name
   column.4.valueformat=HTML
   column.4.width=150
   column.5.descriptionkey=company
   column.5.link.linkproperty.0.name=ID
   column.5.link.linkproperty.0.valuefield=company:ID
   column.5.link.linkproperty.0.valueformat=int
   column.5.link.lookup=link.view
   column.5.link.valuefield=company:objCode
   column.5.link.valueformat=val
   column.5.linkedname=company
   column.5.listsort=nested(company).string(name)
   column.5.namekey=company
   column.5.querysort=company:name
   column.5.shortview=false
   column.5.stretch=0
   column.5.valuefield=company:name
   column.5.valueformat=HTML
   column.5.width=150
   ```

1. Click **Done** > **Save View**.
