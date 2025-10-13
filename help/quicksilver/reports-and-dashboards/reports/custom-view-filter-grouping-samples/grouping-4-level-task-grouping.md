---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Grouping: 4-level Task Grouping for Portfolio Owner, Program Owner, Project Owner, and Project Status'
description: This task Grouping provides 4 levels of Grouping. In this case, tasks are grouped by Portfolio Owner, Program Owner, Project Owner, and Project Status. You can only have up to 3 levels of Grouping using the standard interface. To add a fourth level, you must use Text Mode. You cannot group reports by more than 4 criteria at the same time.
author:  Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
---
# Grouping: 4-level task grouping for Portfolio Owner, Program Owner, Project Owner, and Project Status

<!--Audited: 10/2024-->

This task Grouping provides 4 levels of Grouping. In this case, tasks are grouped by Portfolio Owner, Program Owner, Project Owner, and Project Status. You can only have up to 3 levels of Grouping using the standard interface. To add a fourth level, you must use Text Mode. You cannot group reports by more than 4 criteria at the same time.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

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
   <p>Contributor or Request to modify a filter </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create a 4-level task Grouping for Portfolio Owner, Program Owner, Project Owner, and Project Status

To apply this grouping:

1. Go to a list of tasks.
1. From the **Grouping** drop-down menu, select **New Grouping**.

1. Click **Switch to Text Mode**.
1. Remove the text in the **Group your Report** area.
1. Replace the text in the box displayed with the following code:  
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Owner<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Owner<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valuefield=projectOwnerMM:name<br>group.2.valueformat=string<br>group.3.enumclass=com.attask.common.constants.ProjectStatusEnum<br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val</pre>

1. Click **Done**, then **Save Grouping**.
1. (Optional) Update the name for the grouping, then click **Save Grouping**.
