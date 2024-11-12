---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Reporting Elements Used in Reports'
description: This view displays the View, Filter, and Grouping used to build each report in Adobe Workfront when you use it in a list of reports.
author: Nolan
feature: Reports and Dashboards
exl-id: 67f86523-e136-4768-af93-586a107b106f
---
# View: reporting elements used in reports

<!--Audited: 11/2024-->

This view displays the View, Filter, and Grouping used to build each report in Adobe Workfront when you use it in a list of reports.

You can see the `valuefields` or `valueexpressions` used in every element of the report.

![report_with_elements_definitions.png](assets/report-with-elements-definitions-350x130.png)

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
   <td> <p> Current: 
   <ul>
   <li>Request to modify a view</li> 
   <li>Plan to modify a report</li>
   </ul>
     </p>
     <p> New: 
   <ul>
   <li>Contributor to modify a view</li> 
   <li>Standard to modify a report</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
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

## View reporting elements used in reports

1. Go to a list of reports.
1. From the **View** drop-down menu, select **New View**.
1. In the **Column Preview** area, eliminate all columns except for one.
1. Click the header of the remaining column, then click **Switch to Text Mode** > **Edit Text Mode**.
1. Remove the text you find in the **Edit Text Mode** box, and replace it with the following code:


      ```
      column.0.descriptionkey=name
      column.0.link.linkproperty.0.name=ID
      column.0.link.linkproperty.0.valuefield=ID
      column.0.link.linkproperty.0.valueformat=string
      column.0.link.lookup=link.run
      column.0.link.value=val(objCode)
      column.0.listsort=string(name)
      column.0.namekey=name.abbr
      column.0.querysort=name
      column.0.valuefield=name
      column.0.valueformat=HTML
      column.0.width=200
      column.1.descriptionkey=objecttype
      column.1.listsort=nested(view).string(uiObjCode)
      column.1.namekey=objecttype.abbr
      column.1.querysort=uiObjCode
      column.1.valuefield=uiObjCode
      column.1.valueformat=objCodeMessage
      column.1.width=80
      column.2.descriptionkey=enteredby
      column.2.listsort=nested(enteredBy).string(lastName)
      column.2.namekey=enteredby.abbr
      column.2.querysort=enteredBy:lastName
      column.2.valuefield=enteredBy:name
      column.2.valueformat=HTML
      column.2.width=130
      column.3.displayname=Filter definition
      column.3.textmode=true
      column.3.valuefield=filter:definition
      column.3.valueformat=HTML
      column.4.displayname=View definition
      column.4.textmode=true
      column.4.valuefield=view:definition
      column.4.valueformat=HTML
      column.5.displayname=Grouping definition
      column.5.textmode=true
      column.5.valuefield=groupBy:definition
      column.5.valueformat=HTML
      ```

1. Click **Done** > **Save View**.
