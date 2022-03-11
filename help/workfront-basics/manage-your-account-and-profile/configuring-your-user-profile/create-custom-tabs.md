---
filename: create-custom-tabs
product-area: user-management
navigation-topic: configure-your-user-profile
title: Create custom tabs or sections
description: The information you see in the Workfront web application is often displayed in the sections in the left panel by default. Each section contains different information about a Workfront area or object. For more information about the default areas of Workfront, see the article About the default Adobe Workfront layout.
---

# Create custom tabs or sections

Adobe Workfront sections The information you see in the Workfront web application is often displayed in the sections in the left panel by default. Each sectioncontains different information about a Workfront area or object.  
For more information about the default areasof Workfront, see the article [About the default Adobe Workfront layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

In addition to the sectionsthat come with Workfront by default, you can create custom sectionson which you can display information relevant to your workflow. You cannot add custom sectionsto all areas and objects.

The following table lists all the Workfront areas and objects that contain sections in the left panel and which of them can be customized:

&nbsp;
Workfront area or object Default system sections Custom sections Projects area ✓ ✓ Team ✓ Requests area ✓ Timesheets area ✓ Portfolio ✓ ✓ Program ✓ ✓ Project ✓ ✓ Task ✓ ✓ Issue ✓ ✓ User ✓ ✓ Document ✓ ✓ 

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td>Reviewer or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>View access to the object type</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your Workfront administrator.
Add a custom section in the left panel of a Workfront object or area 

Before you can create a custom section, you must build a dashboard with all the information you want to display on the tab. You may also build an external page.  
For more information about building dashboards, see the article [Create a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).  
For more information about building external pages, see the article [Embed an external web page in a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

After you build the dashboard or the external page, you can add them to the custom section.

To add a custom tab:

1. Go to one of the Workfront areas or objects where you can add a custom section in the left panel.  
   Or
1. Go to an object where you can add a custom section in the left panel.  
   For more information about what areas and objects you can add custom sections to, see Adobe Workfront sections.
1. Click Add custom section in the left panel. 
1. Specify the name of the section in the Custom section title field. This is visible only to you.&nbsp;
1. In the `Add a Dashboard` field, start typing the name of the dashboard or external page you want to add and click it when it appears in the list.&nbsp;
1. Click Add new section. 
1. (Optional) Drag and drop the sectionsin the order in which you would like to display them.
   The top section is the default section for the page. The sections you created for individual objects display when you access all objects of the same type and are available only to you.

Display custom sections in the left panel of objects For more information about adding a custom section under an object, see the section Add a custom section in the left panel of a Workfront object or area in this article.

When you add a dashboard to a custom sectionunder an object, the object acts as a filter for the dashboard. For example, if you add a task report on a dashboard and you add the dashboard to a project, the custom sectionthat contains the dashboard on the project displays only tasks on the project you are viewing.&nbsp;

The following objects are filtered for the object under which they display, if that object is higher in hierarchy than them:

* Project
* Task
* Issue
* Approval Process
* Note
* Document

For more information about the hierarchy and interdependency of objects, see the section [Interdependency and hierarchy of objects](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) in the article [Understand objects in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
Customize sections in a Layout Template 

When you add custom sectionsto your Workfront instance, they are only visible to you.&nbsp;

You can customize the sectionsin Workfront and share the new layout with several users by using Layout Templates. Only a system or a group administrator can share them with other users by using Layout Templates.&nbsp;
