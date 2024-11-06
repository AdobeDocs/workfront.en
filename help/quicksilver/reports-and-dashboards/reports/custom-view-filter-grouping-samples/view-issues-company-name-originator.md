---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Issues with the Company Name of the Originator'
description: This issue view displays the company name associated with the user who submitted the issue.
author: Nolan
feature: Reports and Dashboards
exl-id: e628f7cf-4a7b-4125-bea6-348c72477bd7
---
# View: issues with the company name of the originator

<!--Audit: 11/2024-->

This issue view displays the company name associated with the user who submitted the issue.

![custom_view_for_issues_with_originator_company_name.png](assets/custom-view-for-issues-350x33.png)

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

## View issues with the company name of the originator

1. Go to a list of issues.
1. From the **View** drop-down menu, select **New View**.
1. In the **Column Preview** area, eliminate all columns except for one.
1. Click the header of the remaining column, and click **Switch to Text Mode**, then click **Edit Text Mode**.
1. Remove the text you find in the **Edit Text Mode** box, and replace it with the following code:  


      ```
      column.0.descriptionkey=name
      column.0.link.linkproperty.0.name=ID
      column.0.link.linkproperty.0.valuefield=ID
      column.0.link.linkproperty.0.valueformat=val
      column.0.link.lookup=link.view
      column.0.link.value=val(objCode)
      column.0.listsort=string(name)
      column.0.namekey=name
      column.0.querysort=name
      column.0.valuefield=name
      column.0.valueformat=HTML
      column.0.width=140
      column.1.descriptionkey=originator
      column.1.link.linkproperty.0.name=ID
      column.1.link.linkproperty.0.valuefield=ownerID
      column.1.link.linkproperty.0.valueformat=int
      column.1.link.lookup=link.view
      column.1.link.valuefield=owner:objCode
      column.1.link.valueformat=val
      column.1.listsort=nested(owner).string(name)
      column.1.namekey=originator.abbr
      column.1.querysort=owner:name
      column.1.valuefield=owner:name
      column.1.valueformat=HTML
      column.1.width=151
      column.2.descriptionkey=entrydate
      column.2.listsort=atDateAsAtDate(entryDate)
      column.2.namekey=entrydate.abbr
      column.2.querysort=entryDate
      column.2.valuefield=entryDate
      column.2.valueformat=atDate
      column.2.width=75
      column.3.descriptionkey=age
      column.3.listsort=doubleAsDouble(age)
      column.3.namekey=age
      column.3.querysort=age
      column.3.valuefield=howOld
      column.3.valueformat=val
      column.3.width=80
      column.4.viewalias=statusicons
      column.4.displayname=Flags
      column.4.linkedname=direct
      column.4.namekey=statusicons
      column.4.valuefield=
      column.4.valueformat=HTML
      column.4.querysort=
      column.4.tile.name=component.issuestatusicons
      column.4.tile.pdfcomponent=issueStatusIcons
      column.4.delimiter=
      column.4.tile.template=/WEB-INF/jsp/lists/components/issueStatusIcons.jsp
      column.5.description=Originator's Company Name
      column.5.link.linkproperty.0.name=ID
      column.5.link.linkproperty.0.valuefield=owner:companyID
      column.5.link.linkproperty.0.valueformat=int
      column.5.link.lookup=link.view
      column.5.link.valuefield=owner:company:objCode
      column.5.link.valueformat=val
      column.5.listsort=nested(owner:company).string(name)
      column.5.name=Originator Company
      column.5.querysort=owner:company:name
      column.5.valuefield=owner:company:name
      column.5.valueformat=HTML
      column.5.width=151
      ```

1. Click **Done** > **Save View**.
1. (Optional) Update the view name, then click **Save View**.
