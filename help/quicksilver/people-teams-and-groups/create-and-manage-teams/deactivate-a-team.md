---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Deactivate a team
description: You can deactivate teams you no longer use while retaining the associated historical data. Adobe Workfront administrators can reactivate a team at any time from the Teams area in Setup.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
---
# Deactivate a team

You can deactivate teams you no longer use while retaining the associated historical data. [!DNL Adobe Workfront] administrators can reactivate a team at any time from the Teams area in Setup. If you deactivate a team, the team no longer displays in the following areas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Typeahead fields in custom forms</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Sharing dialog for objects</p> </li> 
     <li> <p>[!UICONTROL User Profile]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Main selection drop-down menu in the [!UICONTROL Teams] area</p> </li> 
     <li> <p>[!UICONTROL Assignments] typeahead</p> </li> 
     <li> <p>[!UICONTROL Add to Kanban] board dialog in a project</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Deactivated teams don't appear when you search for a team, but will still display in [!UICONTROL Home Team] and Other Teams if the user was assigned to the team prior to deactivation.[!UICONTROL ]

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your [!DNL Workfront] administrator.

## Deactivate a team

Any work assigned to the team prior to deactivation remains assigned. We recommend reassigning work before you deactivate the team.

>[!TIP]
>
>You can create a report to filter for any tasks or issues where the deactivated team is still assigned.

When using request queues, if you deactivate a team assigned as the default team in a routing rule, the team remains and requests are still routed to the deactivated team. We recommend updating routing rules with active teams before you deactivate the team.

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Teams]**.
1. Click the **[!DNL Switch team]** icon, then either select a new team from the drop-down menu or search for a team in the search bar.
1. Click the **[!UICONTROL More]** menu, then select **[!UICONTROL Edit]**.

   ![](assets/edit-team-settings-350x205.png)

1. Clear the **[!UICONTROL Is Active]** check box.
1. Click **[!UICONTROL Save changes]**.

## Known limitations

Deactivated teams display in the following areas:

* The Owner field in [!DNL Workfront Goals]. This requires an additional license for [!DNL Adobe Workfront Goals]. For more information, see [Get started with [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
