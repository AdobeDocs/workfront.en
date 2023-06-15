---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Create custom sections
description: The information you see in the [!DNL Workfront] web application is often displayed in the sections in the left panel by default. Each section contains different information about a [!DNL Workfront] area or object.
author: Nolan
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
---
# Create custom sections

## [!DNL Adobe Workfront] sections

The information you see in the [!DNL Workfront] web application is often displayed in the left panel sections by default. Each section contains different information about a [!DNL Workfront] area or object.\
For more information about the default areas of [!DNL Workfront], see the article [About the default [!DNL Adobe Workfront] layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

In addition to the sections that come with [!DNL Workfront] by default, you can add a dashboard on which you can display information relevant to your workflow. You cannot add a dashboard to all areas and objects.

The following table lists all the [!DNL Workfront] areas and objects that contain sections in the left panel and which of them can be customized:

| **[!DNL Workfront] area or object** | **Default system sections** | **Custom sections** |
|---|---|---|
| [!UICONTROL Projects] area | ✓ | ✓ |
| [!UICONTROL Team] | ✓ | &nbsp; |
| [!UICONTROL Requests] area | ✓ | &nbsp; |
| [!UICONTROL Timesheets] area | ✓ | &nbsp; |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Program] | ✓ | ✓ |
| [!UICONTROL Project] | ✓ | ✓ |
| [!UICONTROL Task] | ✓ | &nbsp;✓ |
| [!UICONTROL Issue] | &nbsp;✓ | &nbsp;✓ |
| [!UICONTROL User] | &nbsp;✓ | &nbsp;✓ |
| [!UICONTROL Document] | &nbsp;✓ | &nbsp;✓ |

{style="table-layout:auto"}

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td>[!UICONTROL Reviewer] or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td>View access to the object type</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your [!DNL Workfront] administrator.

## Add a dashboard in the left panel of a [!DNL Workfront] object or area 

Before you can add a dashboard, you must build the dashboard with all the information you want to display on it. You may also build an external page.\
For more information about building dashboards, see the article [Create a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
For more information about building external pages, see the article [Embed an external web page in a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

After you build the dashboard or the external page, you can add them to the left panel.

1. Go to one of the [!DNL Workfront] areas or objects where you can add a custom section in the left panel.\
   Or
1. Go to an object where you can add a [!UICONTROL dashboard] in the left panel.\
   For more information about what areas and objects you can add custom sections to, see [[!DNL Adobe Workfront] sections](#adobe-workfront-sections).
1. Click **[!UICONTROL Add dashboard]** in the left panel.
1. Type a name for the dashboard in the **[!UICONTROL Quick link name]** field. This is visible only to you.
1. Start typing the name of an existing dashboard or external page in the **[!UICONTROL Choose a dashboard]** field, then select the dashboard when it displays in the list.
1. Click **[!UICONTROL Add]**.
1. (Optional) Drag and drop the sections in the order in which you would like to display them.

   The top section is the default section for the page.

   The sections you created for individual objects display when you access all objects of the same type and are available only to you.

## Display dashboards in the left panel of objects

For more information about adding a dashboard under an object, see the section [[!UICONTROL Add a dashboard] in the left panel of a Workfront object or area](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) in this article.

When you add a dashboard to a custom section under an object, the object acts as a filter for the dashboard. For example, if you add a task report on a dashboard and you add the dashboard to a project, the custom section that contains the dashboard on the project displays only tasks on the project you are viewing.

The following objects are filtered for the object under which they display, if that object is higher in hierarchy than them:

* Project
* Task
* Issue
* Approval Process
* Note
* Document

For more information about the hierarchy and interdependency of objects, see the section [Interdependency and hierarchy of objects](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in the article [Understand objects in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Customize the left panel in a layout template

When you add dashboards to your [!DNL Workfront] instance, they are only visible to you.

You can customize the sections in [!DNL Workfront] and share the new layout with several users in a layout template. Only a system or a group administrator can share them with other users in a layout template. For more information about customizing the left panel with a layout template, see [Customize the left panel using a layout template](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
