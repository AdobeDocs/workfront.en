---
product-area: requests
navigation-topic: create-requests
title: Create and manage views in the Requests area
description: If you are using the new requesting experience, you can create and save views for the Requests area.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
---

# Create and manage views in the Requests area

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>





If you are using the new requesting experience in Adobe Workfront, you can create and save views for the Requests area. These views include filters, and column arrangements. 

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* This functionality is available only in the new requesting experience in the Requests area. 
>* View settings are also available in the My Requests widget in Home. However, the views from the Requests area are separate from those from the My Requests widget.
>* The requests list in the Requests area uses the enhanced list in Workfront. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Contributor or higher</p>
   <p>Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p>  <p>You must be a Workfront administrator to add views to layout templates</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create a view for requests

You can create a view in the Requests area of Workfront when you use the new requests experience. 

1. To access the Requests list:

   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.

1. In the **Requests** list, click the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png) and click **New view**.

   ![New view](assets/create-new-view.png)

1. Enter a name for the new view, and click **Create**.
1. Continue to [Edit a view in the Requests area](#edit-a-view-in-the-requests-area).

## Edit a view for requests

You can edit existing views, including views you have just created in the Requests area of Workfront.

By editing a view in the Requests area, you can change the following elements of the view:

* Name
* Filters
* Columns

The changes you make on a view are visible to all those you share the view with. 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to edit from the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png).

1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and click the three-dot menu next to the view, select **Rename**, then type in the new name for the view.
1. Press Enter to save the new name. 
1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and select the view you want to edit.
1. To add a field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list. 

   The **Column manager** opens.
1. Click the plus icon next to the field that you want to add as a column to the view, then click **Save**.

   Fields associated with the objects in the list are available to add as columns. <!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >Fields you add to the columns must exist before they are available in the **Column manager**.


1. (Optional) Click **Columns** to open the F**ields visibility and order** box. 
1. Turn on the setting for each field  you want to show in the list, turn it off to hide it, or drag and drop the fields in a different order.

1. (Optional) Click **Filters** and start adding conditions for what requests you want to view. 

    You can filter by the following request fields:  

    * **Workspace**: The workspace the request form is associated with.
    * **Object type**: The record type the request form is associated with.
    * **Entry date**: The date when the request was submitted.
    * **Request form**: The name of the request form used to submit the request.
    * **Status**: The status of the request.
    * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

    You can also filter by any fields that have been added to the view for any object visible in the view.

    You can have multiple filters joined by either **And** or **Or**.
    The request list is filtered automatically, as you add the filter conditions. 
 

<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Changes to views are saved automatically.
> * Changes to views are visible to anyone that uses the view.
> * Use the **Me (logged-in user)** filter wildcard in any field that has users as the value.

## Add the requests view to a layout template.

A Workfront administrator can add the new view to layout templates.

For instructions, see [Customize Filters, Views, and Groupings using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Share a view

You can share views that you create with other users, teams, or groups.

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to share.
1. Hover over the view that you want to share, then click on the three-dot menu to the right of the view name, then click  **Share**.
1. In the **Share** box, enter the people, teams, roles, groups, or companies that you want to share the view with, then select them from the list when they appear.
1. Click **Save**.

   The view is shared with the entities you indicate. They can view the updated view elements you edited for the view before sharing it. <span class="preview">If they update the view, their changes will not visible to others, unless they make a copy of the same view and preserve their changes before they share the copy. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
