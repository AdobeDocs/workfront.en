---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Deactivate or Delete a Team
description: You can deactivate teams you no longer use while retaining the associated historical data. Adobe Workfront administrators can reactivate a team at any time from the Teams area in Setup.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
---
# Deactivate or delete a team

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

Deactivated teams don't appear when you search for a team, but will still display in [!UICONTROL Home Team] and Other Teams if the user was assigned to the team prior to deactivation.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront package</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr>
   <td>Access level configurations</td>
   <td><p>To deactivate a team, no configurations are required.</p>
   <p>To delete a team, you must be a System administrator.</p></td>
  </tr>
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Deactivate a team

Any work assigned to the team prior to deactivation remains assigned. We recommend reassigning work before you deactivate the team.

>[!TIP]
>
>You can create a report to filter for any tasks or issues where the deactivated team is still assigned.

When using request queues, if you deactivate a team assigned as the default team in a routing rule, the team remains and requests are still routed to the deactivated team. We recommend updating routing rules with active teams before you deactivate the team.

{{step1-to-team}}

1. Click the **[!DNL Switch team]** icon, then either select a new team from the drop-down menu or search for a team in the search bar.
1. Click the **[!UICONTROL More]** menu, then select **[!UICONTROL Edit]**.

   ![](assets/edit-team-settings.png)

1. Clear the **[!UICONTROL Is Active]** check box in the team settings.
1. Click **[!UICONTROL Save changes]**.

## Known limitations of deactivating a team

Deactivated teams display in the following areas:

* The Owner field in [!DNL Workfront Goals]. This requires an additional license for [!DNL Adobe Workfront Goals]. For more information, see [Get started with [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Delete a team

Only a system administrator can delete a team. If you are a team owner (but not an administrator) and you try to delete a team, you will see an error message.

To delete a team:

{{step1-to-team}}

1. Click the **[!DNL Switch team]** icon, then either select a new team from the drop-down menu or search for a team in the search bar.
1. Click the **[!UICONTROL More]** menu, then select **[!UICONTROL Delete]**.

   ![](assets/edit-team-settings.png)

1. Click [!UICONTROL **Confirm**] on the confirmation message to permanently delete the team. Deleted teams cannot be recovered.
