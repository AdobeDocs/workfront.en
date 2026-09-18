---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configure Effect on Hours When an Object Is Deleted and Restored
description: You can configure what happens to hours when someone deletes a project, task, or issue that the hours are logged against. The option you choose also determines what happens to the hours if the project, task, or issue is restored at a later time. (For more information about restoring items in Workfront, see Restore deleted items.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
TQID: https://experienceleague.adobe.com/-qjytcjOGAEltoclAl6xXJ-EuvW9hD0CrwMy8T3c-5g
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Configure effect on hours when an object is deleted and restored

You can configure what happens to hours when someone deletes a project, task, or issue that the hours are logged against. The option you choose also determines what happens to the hours if the project, task, or issue is restored at a later time. (For more information about restoring items in Workfront, see [Restore deleted items](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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

## Configure how hours are managed when an item is deleted and restored

{{step-1-to-setup}} 

1. Expand **Timesheets & Hours**, then click**Preferences**.

1. Locate the **Project, Task or Issue Deletion Preferences** section.
1. (Conditional) To configure how hours are managed when a project is deleted, select one of the following options in the **When deleting projects** section:

   * Keep logged hours already added to timesheets as general hours (If this project is restored at a later time, the hours remain on the timesheet)  
     This option is selected by default.
   * Delete any logged hours (If this project is restored at a later time, logged hours are restored to the project)

1. (Conditional) To configure how hours are managed when a task or issue is deleted, select one of the following options in the **When deleting tasks or issues** section:

   * Move any logged hours to the project where the task or issue resides (If this task or issue is restored at a later time, the hours remain on the project)  
     This option is selected by default.
   * Delete any logged hours (If this task or issue is restored at a later time, logged hours are restored to the task or issue)

1. Click **Save**.
