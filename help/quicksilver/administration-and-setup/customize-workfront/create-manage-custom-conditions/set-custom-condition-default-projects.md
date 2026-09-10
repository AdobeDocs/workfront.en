---
title: Set a Custom Condition as the Default for Projects
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: If the Condition Type of a project is set to Progress Status instead of Manual, Adobe Workfront automatically displays one of three built-in default conditions on the project (On Target, At Risk, or In Trouble) as it progresses, as explained in Overview of Project Condition and Condition Type.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
TQID: https://experienceleague.adobe.com/4DNiEZ7cIWavM-3anuC3IU3fQ93y9hsokS31ZL-FSaQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Set a custom condition as the default for projects

If the Condition Type of a project is set to Progress Status instead of Manual, Adobe Workfront automatically displays one of three built-in default conditions on the project (On Target, At Risk, or In Trouble) as it progresses, as explained in [Overview of Project Condition and Condition Type](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![Condition in project header and details](assets/condition-of-project-0825.png)

You can set your custom conditions as default conditions instead of using these three built-in default conditions. For example, you could change the On Target default condition to display as Tracking Well in all projects.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>System Administrator</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Set a custom condition as a default condition for all projects:

{{step-1-to-setup}}

1. Click **Project Preferences** > **Conditions**.  

1. Click the **Projects** tab. 
1. Click **Set default conditions**.
1. In the drop-down menu for the default condition you want to change, click the custom condition you want to use instead. 
1. Repeat the previous step for any other default condition you want to change.
1. Click **Save**.

For information about setting a custom condition as a default condition for tasks and issues, see [Set a custom condition as the default for tasks and issues](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

For information about setting up a project so that users can update its condition manually, see [Update Condition for tasks and issues](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
