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

{{highlighted-preview-article-level}}

You can configure the default locations available to assign as attributes to job roles in rate cards. This ensures that the rate cards accurately reflect the market rates in each location.

Rate cards allow your organization to easily manage billing rates for projects. For more information, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

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
1. Click [!UICONTROL **Add more Locations**] at the bottom of the list.
1. Enter the location name and description.
1. Click outside of the entry area to save the location.
1. To delete a location, select it in the list and click the **Delete** icon ![Delete icon](assets/delete.png).

>[!NOTE]
>
>Locations associated with job roles on a rate card can't be deleted.

## Add a sub-location

You can add a sub-location to an existing location. For example, if you already have a location of United Kingdom, then London could be a sub-location.

Three levels of sub-locations are permitted. Country, state or province, and city are common uses of sub-locations.

Each sub-location can be added as an attribute on a rate card in the same way as a top level location, to define the rate for a specific job role at that location.

{{step-1-to-setup}}

1. In the left panel, click [!UICONTROL **Locations**].
1. Select an existing location in the list and click **Add sub location**.
1. Enter the location name and description.
1. Click outside of the entry area to save the location.

   The sub-location is indented under the top level location.

   ![Locations and sub-locations](assets/locations-sublocations.png)


