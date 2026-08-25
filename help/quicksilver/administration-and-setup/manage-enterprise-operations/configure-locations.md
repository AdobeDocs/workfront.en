---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Configure Locations
description: You can configure the default locations available to assign as attributes to job roles in rate cards.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 69233499-fbcb-44a4-a247-d5051f9bc8b9
---
# Configure locations

{{preview-fast-release-general}}

You can configure the default locations available to assign as attributes to job roles in rate cards. This ensures that the rate cards accurately reflect the market rates in each location.

Rate cards allow your organization to easily manage billing rates for projects. For more information, see [Manage rate cards](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md) and [Define rate attributes](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

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
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Add a location

{{step-1-to-setup}}

1. In the left panel, click [!UICONTROL **Locations**].
1. In the Production environment, click [!UICONTROL **Add more Locations**] at the bottom of the list.
   <span class="preview">In the Preview environment, click [!UICONTROL **New row**] at the bottom of the list.</span>

1. Enter the location name and description.
1. Click outside of the row to save the location.
1. To delete a location in the Production environment, select it in the list and click the **Delete** icon ![Delete icon](assets/delete.png).
   <span class="preview">To delete a location in the Preview environment, select it in the list and click [!UICONTROL **Delete**] in the action bar at the bottom of the screen.</span>

>[!NOTE]
>
>Locations associated with job roles on a rate card can't be deleted.

## Add a sub-location

You can add a sub-location to an existing location. For example, if you already have a location of United Kingdom, then London could be a sub-location.

Three levels of sub-locations are permitted. Country, state or province, and city are common uses of sub-locations.

Each sub-location can be added as an attribute on a rate card in the same way as a top level location, to define the rate for a specific job role at that location.

{{step-1-to-setup}}

1. In the left panel, click [!UICONTROL **Locations**].
1. In the Production environment, select an existing location in the list and click [!UICONTROL **Add sub location**].
   <span class="preview">In the Preview environment, select an existing location in the list and click [!UICONTROL **Add sub location**] in the action bar at the bottom of the screen.</span>

1. Enter the location name and description.
1. Click outside of the entry area to save the location.

   The sub-location is indented under the top level location.

   Sample image in the Production environment:
   ![Locations and sub-locations](assets/locations-sublocations.png)

   <span class="preview">Sample image in the Preview environment:</span>
   ![Locations and sub-locations](assets/locations-sublocations-082526.png)


