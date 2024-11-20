---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filter: Create Multiple Filter Rules That Reference the Same Field ('AND' Statements)"
description: In the standard mode interface, when attempting to create multiple filters that reference the same field (using the AND qualifier), one of the filters is deleted when you save the report and exit the report builder.
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
---
# Filter: create multiple filter rules that reference the same field ("AND" statements)

<!--Audited: 10/2024-->

In the standard mode interface, when attempting to create multiple filters that reference the same field (using the AND qualifier), one of the filters is deleted when you save the report and exit the report builder.

**Example:** You might want to view only tasks that contain the word "green" but do not contain the word "red" in the name. Adobe Workfront does not allow you to save the following filter rules using the standard mode interface because it references the same field (Task Name) but uses different modifiers and refers to different values:

* Task Name > Contains > Green
* Task Name > Does Not Contain > Red

However, you can create this filter using text mode.

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
    <p>New:</p>
   <ul><li><p>Contributor to modify a filter </p></li>
   <li><p>Standard to modify a report</p></li> </ul>

   <p>Current:</p>
   <ul><li><p>Request to modify a filter </p></li>
   <li><p>Plan to modify a report</p></li> </ul></td> 
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

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Create multiple filter rules that reference the same field

1. Go to a list of tasks.
1. From the **Filter** drop-down menu, select **New Filter**.
1. Click **Text Mode**.
1. In the box displayed, add the following code:

   ``` 
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >To build similar filters, build the first statement first. For example: 
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Copy and paste the statement as many times as needed. You can then add as many statements as you need to reference the same field (in our case "name") and make the following modifications to the additional statements: 
   >
   >1. Precede the two copied lines with "AND:1:", "AND:2:", "AND:3:", etc for each new field possible value. 
   >1. Replace the field line with the new field value (after the "=" sign). 
   >1. Replace the modifier line (_Mod) with the new modifier. 
   >   
   >These statements are case-sensitive.

1. Click **Apply**, then **Save as new**.
