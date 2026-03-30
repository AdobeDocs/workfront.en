---
product-area: requests
navigation-topic: create-requests
title: Delete a Submitted Request or Request Draft
description: You can delete submitted requests or request drafts in Adobe Workfront. 
author: Alina
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
---
# Delete a submitted request or request draft

You can delete Adobe Workfront or Adobe Workfront Planning submitted requests or request drafts that you created or have Manage permissions to.

Workfront administrators and Workfront Planning workspace managers can also delete requests and request drafts they didn't create. 

You cannot view Planning requests in the legacy request experience. 

This article describes how you can delete request drafts in the new request experience. Deleting Workfront and Planning requests or their drafts is identical.

For more information, see:

* [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md) 
* [Create requests from drafts](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)
* [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md)

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any Workfront or Workflow package</p>
   
   <p>Any Workfront Planning package to manage Planning requests </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Contributor or higher</p>
   <p>Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator or Planning workspace manager to delete requests that you did not create.</p><p>You must have Edit access to Issues.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You must have created the request or draft to delete it in the new requesting experience, or be a Workfront administrator or Planning workspace manager to delete drafts of requests you didn't submit.
   </p><p>You must have Edit permissions to the issues you are deleting.</p>  </td> 
  </tr> 
 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Delete  requests or request drafts in the new requesting experience

You can delete requests and drafts in the following areas: 

* In the Requests area of Workfront
* In the My Requests widget in Home
* From a request page

The following users can delete request drafts: 

* Workfront administrators can delete requests and drafts that they or others submitted. 
* Workfront Planning workspace managers can delete requests and drafts in the Planning workspace that they administer.
* Users can delete requests and drafts that they submitted.

### Delete a request or a draft from the Requests area or My Requests widget in Home

{{step1-to-requests}}

1. To access the **My Requests** widget in **Home**:
   
   {{step1-to-home}}

   1. Locate the **My Requests** widget. 

      For more information on the **My Requests** widget, see [Use the My Requests widget](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. In the **Requests** list or the **My Requests** widget in **Home**, hover over the request or draft that you want to delete, then click the **More** menu ![More menu](assets/more-menu.png) 

1. Click **Delete** 

     Or

     Right-click on the selected request, then click **Delete**.

     >[!TIP]
     >
     >When you do not have access to create issues, you receive a warning that your administrator restricted you from creating requests.

1. In the dialog that opens, click **Delete**.

   The request or draft is deleted.

   Deleted requests are saved in the Recycle Bin and a Workfront administrator can recover them for up to 30 days. Drafts cannot be recovered.

### Bulk delete requests from a list

{{step1-to-requests}}

1. To access the **My Requests** widget in **Home**:
   
   {{step1-to-home}}
   
   1. Locate the **My Requests** widget. 

      For more information on the My Requests widget, see [Use the My Requests widget](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. In the **Requests** list or the **My Requests** widget, click the box to the left of each request that you want to delete.
1. In the blue bar at the bottom of the page, click **Delete**.

   >[!NOTE]
   >
   >If the **Delete** option is not visible in the blue bar, you do not have permission to delete one or more of the selected requests.

### Prerequisites for deleting request drafts

You must do the following before you can delete a request draft:

* Start creating a request. This saves the request as a draft automatically in the Drafts section.

  For information about creating requests, see [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Delete request drafts in the legacy requesting experience

You can delete drafted requests after they are saved as drafts if you no longer find them relevant. You cannot recover deleted draft requests.

You cannot access Planning requests or their drafts from the legacy requesting experience. 

{{step1-to-requests}}

1. Click **Drafts** in the left panel.

   All drafts for all request queues display in this list. 

1. Select a draft in the list, then click **Delete** at the top of the list.
1. Click **Yes, Delete it**.

   The draft is deleted and cannot be recovered.






