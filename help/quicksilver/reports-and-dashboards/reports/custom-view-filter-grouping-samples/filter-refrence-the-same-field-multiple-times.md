---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filter: create multiple filter rules that reference the same field ('AND' statements)"
description: In the standard mode interface, when attempting to create multiple filters that reference the same field (using the AND qualifier), one of the filters is deleted when you save the report and exit the report builder.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
---
# Filter: create multiple filter rules that reference the same field ("AND" statements)

In the standard mode interface, when attempting to create multiple filters that reference the same field (using the AND qualifier), one of the filters is deleted when you save the report and exit the report builder.

**Example:** You might want to view only tasks that contain the word "green" but do not contain the word "red" in the name. Adobe Workfront does not allow you to save the following filter rules using the standard mode interface because it references the same field (Task Name) but uses different modifiers and refers to different values:

* Task Name > Contains > Green
* Task Name > Does Not Contain > Red

However, you can create this filter using text mode.

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
   <td> <p>Request to modify a filter </p>
   <p>Plan to modify a report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create multiple filter rules that reference the same field

1. Go to a list of tasks.
1. From the **Filter** drop-down menu, select **New Filter**.
1. Click **Switch to Text Mode**.
1. Hover over the text mode area, and click **Click to edit text**.
1. In the Set Filter Rules for your Report area, add the following code:

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

1. Click **Done**, then **Save Filter**.
