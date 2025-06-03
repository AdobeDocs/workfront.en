---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configure System Updates
description: Workfront generates automatic system updates in an object's [!UICONTROL Updates] area to record the changes that users perform on the object. As a [!DNL Workfront] administrator, you can configure which object fields and actions [!DNL Workfront] tracks to record system updates.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
---
# Configure system updates

<!-- Audited: 5/2025 -->

[!DNL Adobe Workfront] generates automatic system updates in an object's [!UICONTROL Updates] area to record the following events:

* Changes users make in an object field
* Actions users perform on an object

These system updates include the following type of information:

* The change that was made
* The name of the user who made the change
* The time and date of the change

For more information about system updates, see [System-tracked updates](../system-tracked-update-feeds/system-tracked-update-feeds.md).

As a [!DNL Workfront] administrator, you can configure which object fields and actions [!DNL Workfront] tracks to record system updates.

For example, you could have [!DNL Workfront] track all changes users make to the names of issues throughout the system. Any issue name change then appears as a system update on the issue's [!UICONTROL Updates] area.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Determine which fields [!DNL Workfront] tracks for an object type

You can determine what information [!DNL Workfront] tracks when users change information associated with a certain object type throughout the entire [!DNL Workfront] interface. You do this by adding or removing the fields you want [!DNL Workfront] to track for that object type.

>[!NOTE]
>
>* [!DNL Workfront] can't track and record updates about calculated custom fields.
>* You can customize the system update for projects, tasks, issues, portfolios, programs, and users. You can't customize the system update for templates, documents or timesheets, but [!DNL Workfront] does record system updates for these objects.
>



* [Add fields you want [!DNL Workfront] to track](#add-fields-you-want-workfront-to-track)
* [Remove fields you don't want tracked](#remove-fields-you-don-t-want-tracked)

### Add fields you want [!DNL Workfront] to track {#add-fields-you-want-workfront-to-track}

You can add fields you want [!DNL Workfront] to track for a particular type of object throughout the [!DNL Workfront] interface. When users change information in that field, [!DNL Workfront] records information about the change as a system update in the [!UICONTROL Updates] area for the object.

>[!NOTE]
>
>You can track up to 300 built-in and custom fields in the update feeds. If you are tracking the maximum number of fields and want to track additional fields that are not displayed in the [!UICONTROL All Fields] subtab, you must first remove some of the tracked fields in order to track new fields. For more information about removing fields from the update fields, see [Remove fields you don't want tracked](#remove-fields-you-don-t-want-tracked).

{{step1-to-setup}}

1. In the panel on the left, click **[!UICONTROL Interface]**, then **[!UICONTROL Update Feeds]**.

1. &#x200B;Click **[!UICONTROL Add Fields]**, then select the object that you want to be tracked from the drop-down.

1. In the box that appears, start typing either a built-in (standard) field or a custom field for the object, then select it when it appears in the list.

   >[!NOTE]
   >
   >If [!DNL Workfront] is already tracking the field, you can't add it a second time from the list.

1. After adding all the fields you want [!DNL Workfront] to track, click **[!UICONTROL Add Fields]**. The built-in fields that you added show under the **[!UICONTROL Built-in Fields]** subtab, and the custom fields show under the **[!UICONTROL Custom Fields]** subtab.

   The **[!UICONTROL All Fields]** subtab shows both the built-in and the custom fields that are being tracked.

### Remove fields you don't want tracked {#remove-fields-you-don-t-want-tracked}

You can remove fields you don't want the system to track for a particular type of object throughout the [!DNL Workfront] interface.

{{step1-to-setup}}

1. Click **[!UICONTROL Interface]**, then **[!UICONTROL Update Feeds]**.

1. On the **[!UICONTROL Tracked Fields]** tab, select the **[!UICONTROL All Fields]** subtab. Both the built-in and custom fields that are currently being tracked display.

1. Select the field you want to stop tracking, then click **[!UICONTROL Remove]**.

1. In the **[!UICONTROL Remove Field]** box that appears, click **[!UICONTROL Yes, Remove It]** to confirm.

Any updates about the previously-tracked fields are preserved in the [!UICONTROL Updates] area where they were recorded.

## Determine which actions [!DNL Workfront] tracks for an object type

You can have [!DNL Workfront] track the following actions that users can perform on objects throughout the [!DNL Workfront] interface.

For example, you can have [!DNL Workfront] record an update every time a user changes an assignment to a task or issue. The change then appears as a system update in the [!UICONTROL Updates] area for the task or issue.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Action</strong> </th> 
   <th><strong>Objects</strong> </th> 
   <th><strong>Default Status</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Assignment is changed</td> 
   <td>Tasks, Issues</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Baseline is deleted</td> 
   <td>Projects</td> 
   <td> <p>Disabled</p> </td> 
  </tr> 
  <tr> 
   <td>Billing record is created or deleted</td> 
   <td>Projects</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Document is created or deleted</td> 
   <td>Projects, Tasks, Issues, Portfolios, Programs</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Expense is created or deleted</td> 
   <td>Projects, Tasks</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Hour is logged or deleted</td> 
   <td>Projects, Tasks, Issues</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Issue is deleted</td> 
   <td>Projects</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Task is deleted</td> 
   <td>Projects</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Someone's Access is changed</td> 
   <td>Projects, Tasks, Issues, Documents, Portfolios, Programs</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
  <tr> 
   <td>Subscribe comment object</td> 
   <td>Projects, Tasks, Issues</td> 
   <td> <p>Enabled</p> </td> 
  </tr> 
 </tbody> 
</table>

To configure which actions you want [!DNL Workfront] to track:

{{step1-to-setup}}

1. Click **[!UICONTROL Interface]**, then **[!UICONTROL Update Feeds]**.

1. Click the **[!UICONTROL Actions]** tab.

1. Select an action's checkbox to enable it, or deselect it to disable it.
1. Click **[!UICONTROL Save]**.

When you disable an action, any previously-recorded update about that action is preserved in the [!UICONTROL Updates] area where it was recorded.
