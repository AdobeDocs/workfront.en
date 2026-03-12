---
product-area: projects
navigation-topic: use-the-home-area
title: Use the My Requests widget
description: You can submit requests in the My Requests widget. You can also customize the widget with filters and columns.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
---
# Use the My Requests widget

>[!IMPORTANT]
>
>This article describes the new My Requests widget. You must have the new requesting experience enabled to see the new widget.
>You can enable the new requesting experience in your Requests area.

The My Requests widget displays requests that you have submitted. You can filter the requests, search for specific requests, or adjust column order and visibility. You can also create a new request from the My Requests widget.

>[!NOTE]
>
>* When the My Requests widget loads, it displays up to 50 requests. To display more requests, scroll down the list.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Any Workfront or Workflow package</p>
   <p>Any Workfront Planning package to access Workfront Planning requests and their created objects</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license</strong></td> 
   <td> <p>Contributor or higher</p>
   <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>Access level configuration</strong></td> 
   <td> <p>View or higher access to any objects for which you are tagged in a conversation or need to resolve an approval (Projects, Tasks, Issues, Documents)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>[!UICONTROL View] permissions or higher to projects, tasks, issues, documents where you are tagged in a conversation or need to resolve an approval</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create a request

You can create a request directly from the My Requests widget.

For instructions, see the section [Create a request](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request) in the article [Create work items and projects from the Home area](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Copy a request

You can copy a request in the My Requests widget, edit it, and submit it as a new request.

For instructions, see [Copy and submit requests](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Filter requests

The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Filter**.
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.

The filter is saved automatically.

>[!TIP]
>
>If your organization has purchased Workfront Planning in addition to Adobe Workfront, the My Requests widget will include both Workfront and Workfront Planning requests.
> 
>* To filter for only Workfront requests, set the filter to **Object type** > **Has any of** > **Issues**.
>* To filter for only Workfront Planning requests, et the filter to **Object type** > **Has none of** > **Issues**.

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

## Search requests

To search for specific requests in the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**.  
1. In the search bar near the upper-right of the My Requests widget, enter the term that you want to search for.

   Requests that contain the term are highlighted in orange.

1. (Optional) To jump to the highlighted requests, click the up or down arrows in the search bar.

## Go to an object created by a request

You can find objects created by a request in the My Requests widget.

>[!NOTE]
>
>Links to created objects are available in the new requesting experience only for Planning requests, in cases where the request itself created an object. If a Workfront request is converted to a project or other object, a link to that converted object is not available in the request list in the new requesting experience.

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. Locate the request that created the object. 
1. Click the object name in the **Created object** column for that request. 

   The object's page opens.

