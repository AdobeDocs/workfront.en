---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configure system updates
description: Workfront generates automatic system updates in an object's [!UICONTROL Updates] area to record the changes that users perform on the object. As a [!DNL Workfront] administrator, you can configure which object fields and actions [!DNL Workfront] tracks to record system updates.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
---
# Configure system updates

[!DNL Adobe Workfront] generates automatic system updates in an object's [!UICONTROL Updates] area to record the following events:

* Changes users make in an object field
* Actions users perform on an object

These system updates include the change that was made, the name of the user who made the change, and the time and date of the change.

For more information about system updates, see [System-tracked updates](../system-tracked-update-feeds/system-tracked-update-feeds.md).

As a [!DNL Workfront] administrator, you can configure which object fields and actions [!DNL Workfront] tracks to record system updates.

For example, you could have [!DNL Workfront] track all changes users make to the names of issues throughout the system. Any issue name change then appears as a system update on the issue's [!UICONTROL Updates] area.

## Access requirements

You must have the following access to perform the steps in this article:

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a [!DNL Workfront] administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Determine which fields [!DNL Workfront] tracks for an object type

You can determine what information [!DNL Workfront] tracks when users change information associated with a certain object type throughout the entire [!DNL Workfront] interface. You do this by adding or removing the fields you want [!DNL Workfront] to track for that object type.

>[!NOTE]
>
>* [!DNL Workfront] cannot track and record updates about calculated custom fields.
>* You can customize the system update for projects, tasks, issues, portfolios, programs, and users. You cannot customize the system update for templates, documents or timesheets, but [!DNL Workfront] does record system updates for these objects.
>



* [Add fields you want [!DNL Workfront] to track](#add-fields-you-want-workfront-to-track)
* [Remove fields that you don't want tracked](#remove-fields-that-you-don-t-want-tracked)

### Add fields you want [!DNL Workfront] to track {#add-fields-you-want-workfront-to-track}

You can add fields you want [!DNL Workfront] to track for a particular type of object throughout the [!DNL Workfront] interface. When users change information in that field, [!DNL Workfront] records information about the change as a system update in the [!UICONTROL Updates] area for the object.

>[!NOTE]
>
>You can track up to 300 built-in and custom fields in the update feeds. If you are tracking the maximum number of fields and want to track additional fields that are not displayed in the [!UICONTROL All Fields] Sub-tab, you must first remove some of the tracked fields in order to track new fields. For more information about removing fields from the update fields, see see [Remove fields that you don't want tracked](#remove-fields-that-you-don-t-want-tracked).

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront], then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. In the panel on the left, click **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. &#x200B;Click **[!UICONTROL Add Fields]**, then click the object that you want to be tracked.

1. In the&#x200B; **[!UICONTROL Update Feeds]** box that appears, start typing either a built-in (standard) field or a custom field for the object, then click to select it when it appears in the list.

   If [!DNL Workfront] is already tracking the field, you cannot add it a second time from the list.

1. After adding all the fields you want [!DNL Workfront] to track, click **[!UICONTROL Add Fields]**.

   The built-in fields that you added show under the **[!UICONTROL Built-in Fields]** sub-tab.

   The custom fields you added show under the **[!UICONTROL Custom Fields]** sub-tab.

   The **[!UICONTROL All Fields]** sub-tab shows both the built-in and the custom fields that are being tracked.

### Remove fields that you don't want tracked {#remove-fields-that-you-don-t-want-tracked}

You can remove fields you do not want the system to track for a particular type of object throughout the [!DNL Workfront] interface.

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront], then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Click **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. On the **[!UICONTROL Tracked Fields]** tab, select the **[!UICONTROL All Fields]** sub-tab.

   This shows both the built-in and the custom fields that are currently being tracked.

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

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront], then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Click **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. Click the **[!UICONTROL Actions]** tab.

1. Select an action to enable it, or deselect an action to disable it.
1. Click **[!UICONTROL Save]**.

When you disable an action, any previously-recorded update about that action is preserved in the [!UICONTROL Updates] area where it was recorded.
