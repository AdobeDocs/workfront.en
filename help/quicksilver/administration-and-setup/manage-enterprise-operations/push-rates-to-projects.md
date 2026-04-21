---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Push Rate Changes to Projects
description: A rate card represents the contractual agreement with your client in which hourly rates are defined for the job roles that will complete the work. In a rate card, you can define multiple billing rates per job role, based on attributes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c38e60dd-7fb2-4afc-976a-b0966398c162
---
# Push rate changes to projects

When a rate card is attached to a project <!--or a staffing plan-->, the rates on the rate card can still be adjusted. Then, you can optionally push those rates to the projects that the rate card is attached to. If you do not push the new rates, then the original rates remain on the project.
<!-- and staffing plans -->
<!-- or staffing plan -->

For information about attaching a rate card to a project, see [Attach a rate card to a project](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>Edit access to [!UICONTROL Rate Cards]</td> 
  </tr> 
  <tr> 
   <td>Object permissions</td> 
   <td>To edit a rate card shared with you, you must have Manage permissions to the rate card.</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Push rate changes to projects

{{step-1-to-setup}}

1. In the left panel, click [!UICONTROL **Rate cards**].
1. Click the rate card name in the Rate Cards list.
1. On the Rate Card > Job Roles and Rates screen, verify that the rates are correct and edit any rates as needed.
1. Click [!UICONTROL **Push changes**].
1. On the [!UICONTROL **Apply to all projects**] dialog, all of the projects that use this rate card are selected by default. If you do not want a project to apply the rate changes, you must deselect it.

   <!--/staffing plans-->
   <!--and staffing plans -->
   <!--or staffing plan -->

1. Click [!UICONTROL **Save**].

   The new rates are now reflected on the projects <!--and staffing plans -->that use the rate card.
