---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Manage rate cards
description: Rate cards allow you to define multiple billing rates per role, based on location.
author: Lisa
feature: System Setup and Administration
role: Admin
---
# Manage rate cards

{{highlighted-preview-article-level}}

Rate cards allow you to define multiple billing rates per role, based on location. You could have a job role of Designer based in Paris and a second Designer based in New York, each with different billing rates. However, a location is not required for job roles on a rate card. A billing rate for a job role (and possibly location) on a rate card can also include effective dates.

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
   <td><p>Legacy plan: [!UICONTROL Plan]</p>
       <p>Current plan: [!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to [!UICONTROL Financial Data]</p> <p><b>NOTE</b>: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>To edit a rate card shared with you, you must have Manage permissions to the rate card.</td> 
  </tr> 
 </tbody> 
</table>

## Add a rate card

{{step-1-to-setup}}

1. In the left panel, click [!UICONTROL **Rate cards**].
1. Click [!UICONTROL **New rate card**], then enter the rate card name and description in the list.
1. To add billing rates, click the rate card name in the list.
1. On the card screen, click [!UICONTROL **New billing rate**].
1. In the New Billing Rate dialog, select a [!UICONTROL **Job Role**] to define billing rates for.

   The Default Billing Rate displays the system-level rate for this job role.

   ![New Billing Rate dialog](assets/location-rate-for-rate-card.png)

1. Select a [!UICONTROL **Currency**] for the job role.
1. (Optional) Select a [!UICONTROL **Location**] for the job role.
1. In the [!UICONTROL **Billing Rate 1**] field, enter the billing rate for this location. Then, click [!UICONTROL **Save**] to override the billing rate one time.
   
   Or
   
   Click [!UICONTROL **Add Rate**] to add more location-specific billing rates with effective dates.

1. (Conditional) If you are adding more than one billing rate for this location, enter the following information:

   * **[!UICONTROL Billing Rate 1], 2, etc.:** The value of the billing rate for the time period.
   * **[!UICONTROL Start Date]:** The date when the rate override begins.
   * **[!UICONTROL End Date]:** The date when the rate override ends.

     Billing Rate 1 will not have a start date and the last billing rate will not have an end date. Some dates are added automatically. For example, if Billing Rate 1 does not have an end date, and you add Billing Rate 2 with a start date of May 1, 2023, an end date of April 30, 2023 is added to Billing Rate 1 so that no gaps exist.

1. Click [!UICONTROL **Save**].
1. (Optional) To add another billing rate, either for the same job role in another location or for a separate job role, click [!UICONTROL **New billing rate**].

## Copy a rate card

{{step-1-to-setup}}

1. In the left panel, click [!UICONTROL **Rate cards**].
1. Select the check box next to rate card in the list and click the **Copy** icon ![Copy icon](assets/copy-icon.png).

   A duplicate rate card is added. Click the rate card name in the list to change its name.

## Delete a rate card

{{step-1-to-setup}}

1. In the left panel, click [!UICONTROL **Rate cards**].
1. Select the check box next to rate card in the list click the **Delete** icon ![Delete icon](assets/delete.png).

   >[!NOTE]
   >
   >A rate card attached to a project will be deleted from the project.
