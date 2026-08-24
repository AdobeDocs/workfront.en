---
user-type: administrator
product-area: system-administration;setup
title: Configure Fields to Track in Change History
description: As a Workfront administrator, you can configure which object fields and actions Workfront tracks.
author: Lisa
feature: System Setup and Administration
role: Admin
---
# Configure fields to track in change history

{{highlighted-preview-article-level}}

Adobe Workfront generates automatic system updates to record the following events:

* Changes users make in an object field
* Actions users perform on an object

These system updates include the following type of information:

* The change that was made
* The name of the user who made the change
* The time and date of the change

As a Workfront administrator, you can configure which object fields and actions Workfront tracks.

For example, you could have Workfront track all changes users make to the names of issues throughout the system. Any issue name change then appears as an entry on the change history log. For more information, see [View and manage change history](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>System administrator</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limits to field tracking

The limits for the number of fields you can track are defined by your Workfront package.

|Workfront package | Maximum number of tracked fields |
|---------|----------|
| Select | 700 |
| Prime | 3000 |
| Ultimate | 5000 |
| Workflow Select | 1000 |
| Workflow Prime | 5000 |
| Workflow Ultimate | Unlimited |

## Add fields you want to track

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Configuration**.
1. On the Configuration screen, click **Add field**.
1. In the **Add fields** box, select an object. You can begin typing the object name, then select it when it appears in the list.
1. Next, select the field names that you want to track for that object. You can begin typing the field name, then select it when it appears in the list.

   Both custom fields and native fields are available for the object.
   Fields already being tracked are shown as selected in the list.
   
   ![Add fields for change tracking](assets/change-history-config-add-fields.png)

1. After selecting all of the fields you want to track, click **Add**.
   
   The fields are added to the Tracked Fields list.

## Remove fields you no longer want tracked

You can remove fields you don't want the system to track for a particular type of object throughout the Workfront interface.

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Configuration**.
1. On the Configuration screen, select the field or fields you want to stop tracking.

   You might see the same field name more than once. The fields are grouped by object so you can locate the correct field. You can also use the search box at the top of the screen.

1. Select **Delete** in the action bar at the bottom of the screen.
1. Click **Remove** on the confirmation message.

   The fields are removed from the Tracked Fields list.


