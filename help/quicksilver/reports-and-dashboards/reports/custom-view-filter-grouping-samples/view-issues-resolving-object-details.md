---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Issues with Resolving Object Details'
description: This issue view displays the name and percentage complete of the resolving object of the Issue, allowing the issue originator to have insight into the progress of the issue even without access to the resolving task or project.
author: Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
---
# View: issues with resolving object details

<!--Audited: 11/2024-->

This issue view displays the name and percentage complete of the resolving object of the Issue, allowing the issue originator to have insight into the progress of the issue even without access to the resolving task or project.

This view uses the `sharecol=true` tag to combine multiple fields under the same column header. For more information on the `sharecol` tag, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

![issue_custom_view_with_resolving_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or Request to modify a view </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## View issues with resolving object details

1. Go to a list of issues.
1. From the **View** drop-down menu, select **New View**.

1. In the**Column Preview** area, eliminate all columns except for one.
1. Click the header of the remaining column, click **Switch to Text Mode**, then click **Edit Text Mode**.
1. Remove the text you find in the **Edit Text Mode** box, and replace it with the following code:

    ```
    column.0.querysort=name
    column.0.stretch=0
    column.0.valuefield=name
    column.0.valueformat=HTML
    column.0.width=150
    column.1.descriptionkey=sourceobject
    column.1.linkedname=direct
    column.1.listsort=nested(referenceObject).HTML(name)
    column.1.namekey=sourceobject.abbr
    column.1.shortview=false
    column.1.stretch=0
    column.1.valuefield=referenceObject:name
    column.1.valueformat=HTML
    column.1.viewalias=source
    column.1.width=100
    column.2.descriptionkey=assignedto
    column.2.link.linkproperty.0.name=ID
    column.2.link.linkproperty.0.valuefield=assignedTo:ID
    column.2.link.linkproperty.0.valueformat=int
    column.2.link.lookup=link.view
    column.2.link.valuefield=assignedTo:objCode
    column.2.link.valueformat=val
    column.2.linkedname=assignedTo
    column.2.listsort=nested(assignedTo).string(name)
    column.2.namekey=assignedto
    column.2.querysort=assignedTo:name
    column.2.shortview=false
    column.2.stretch=25
    column.2.valuefield=assignedTo:name
    column.2.valueformat=HTML
    column.2.width=150
    column.3.descriptionkey=entrydate
    column.3.linkedname=direct
    column.3.listsort=atDateAsAtDate(entryDate)
    column.3.namekey=entrydate.abbr
    column.3.querysort=entryDate
    column.3.shortview=false
    column.3.stretch=0
    column.3.valuefield=entryDate
    column.3.valueformat=atDate
    column.3.width=150
    column.4.descriptionkey=description
    column.4.linkedname=direct
    column.4.listsort=string(description)
    column.4.namekey=description.abbr
    column.4.querysort=description
    column.4.shortview=false
    column.4.stretch=75
    column.4.valuefield=description
    column.4.valueformat=HTML
    column.4.width=150
    column.5.descriptionkey=status
    column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum
    column.5.linkedname=direct
    column.5.listsort=string(status)
    column.5.namekey=status.abbr
    column.5.querysort=status
    column.5.shortview=false
    column.5.stretch=0
    column.5.type=enum
    column.5.valuefield=status
    column.5.valueformat=val
    column.5.width=150
    column.6.displayname=Resolving Object Name
    column.6.linkedname=resolveTask
    column.6.namekey=view.relatedcolumn
    column.6.namekeyargkey.0=resolveTask
    column.6.namekeyargkey.1=name
    column.6.querysort=resolveTask:name
    column.6.sharecol=true
    column.6.textmode=true
    column.6.valuefield=resolveTask:name
    column.6.valueformat=HTML
    column.7.displayname=
    column.7.linkedname=resolveOpTask
    column.7.namekey=view.relatedcolumn
    column.7.namekeyargkey.0=resolveOpTask
    column.7.namekeyargkey.1=name
    column.7.querysort=resolveOpTask:name
    column.7.sharecol=true
    column.7.textmode=true
    column.7.valuefield=resolveOpTask:name
    column.7.valueformat=HTML
    column.8.displayname=
    column.8.linkedname=resolveProject
    column.8.namekey=view.relatedcolumn
    column.8.namekeyargkey.0=resolveProject
    column.8.namekeyargkey.1=name
    column.8.querysort=resolveProject:name
    column.8.textmode=true
    column.8.valuefield=resolveProject:name
    column.8.valueformat=HTML
    column.9.displayname=Resolving Object Percent Complete
    column.9.textmode=true
    column.9.valueexpression=IF(ISBLANK({resolveTask}.{ID}),{resolveProject}.{percentComplete},IF(ISBLANK({resolveProject}.{ID}),{resolveTask}.{percentComplete},''))
    column.9.valueformat=doubleAsPercentRounded
    ```

1. Click **Done** > **Save View**.
1. (Optional) Update the view name, then click **Save View**.
