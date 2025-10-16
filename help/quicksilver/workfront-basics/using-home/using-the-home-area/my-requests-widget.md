---
product-area: projects
navigation-topic: use-the-home-area
title: Use the My Requests widget
description: You can submit requests in the My Requests widget. You can also customize the widget with filters and columns.
author: Becky
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
---
# Use the My Requests widget

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

>[!IMPORTANT]
>
>This article describes the new My Requests widget. You must have the new requesting experience enabled to see the new widget.
>You can enable the new requesting experience in your Requests area.

The My Requests widget displays requests that have been submitted to your organization. You can filter the requests, search for specific requests, or adjust column order and visibility. You can also create a new request from the My Requests widget.

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
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license</strong></td> 
   <td> <p>Contributor or higher</p>
   <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
    <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
  </tr> 
   <td role="rowheader"><strong>Access level configuration</strong></td> 
   <td> <p>View access or higher to any objects for which you are tagged in a conversation or need to resolve an approval (Projects, Tasks, Issues, Documents)</p> </td> 
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

For instructions, see [Create a request](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) in the article Create work items and projects from the Home area.

## Filter requests

The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR.

To configure the filter in the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**. 
1. In the My Requests widget, click **Filter**.
1. In the leftmost field, select what you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.

The filter is saved automatically.

>[!TIP]
>
>If your organization has purchased Workfront Planning, the My Requests widget will include both Workfront and Workfront Planning requests.
> 
>* To filter for only Workfront requests, set the filter to **Object type** > **Has any of** > **Issues**.
>* To filter for only Workfront Planning requests, et the filter to **Object type** > **Has none of** > **Issues**.

## Adjust columns

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
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**. 
1. In the My Requests widget, click **Columns**.
1. (Optional)To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the leftmost column.
1. (Optional) Use the toggle to control whether a column is displayed in the My Requests widget.

Column preferences are saved automatically.

## Search requests

To search for specific requests in the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**. 
1. In the search bar near the upper-right of the My Requests widget, enter the term that you want to search for.

   Requests that contain the term are highlighted in orange.

1. (Optional) To jump to the highlighted requests, click the up or down arrows in the search bar.
