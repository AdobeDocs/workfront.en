---
filename: combined-pages-object-details
content-type: overview
navigation-topic: the-new-workfront-experience
title: Edit object details in the new Adobe Workfront experience
description: We have merged all the subtabs located under the Details tab of an object into a single page in the new Adobe Workfront experience.
---

# Edit object details in the new Adobe Workfront experience

We have merged all the subtabs located under the Details tab of an object into a single page in the new Adobe Workfront experience.

>[!NOTE]
>
>This is currently available for projects, tasks, issues, programs, portfolios, templates, template tasks, users, documents.

## Benefits of displaying all object details on one page

* You can access all information about the object in one place with fewer clicks.
* Your Adobe Workfront administrator can modify the sequence of the areas displayed in the Details page or remove fields according to your needs using a Layout Template.
* You can update all fields that you have permissions to edit in one place without navigating between multiple subtabs.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the object whose details you want to update</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the object whose details you want to update</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Edit the Details page on an object

Accessing the Details page for an object is similar to all objects where this functionality is supported.

>[!NOTE]
>
>Currently, you can access the combined Details page on projects, tasks, issues, programs, portfolios, templates, and template tasks.

1. Go to the object whose **Details** page you want to access.
1. In the left panel, click **<Object> Details**.&nbsp;For example, for a project, click&nbsp;**Project Details**.

   ![](assets/one-page-project-details-page-350x279.png)

   Notice the following in the new Details page:

  * The page displays to the right of the left panel and it is organized in several areas.

    Your Workfront administrator determines what areas and what fields display on the Details page when configuring and assigning you a Layout Template. For information about Layout Templates in the new Adobe Workfront experience, see the article [Layout templates](../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).
  
  * Each area contains multiple cards that group similar information together.

    ![](assets/project-details-with-cards-and-titles-350x148.png)

  * The following areas display on the Details page by default:

    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">Overview</td> 
       <td> <p>Displays general information about the object. The fields in this area are Workfront system fields.</p> <p>This area is expanded by default.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Names of custom forms</td> 
       <td> <p>If they are attached, the names of the custom forms display here. </p> <p>They are collapsed by default. The fields in this area are fields created by your organization. </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Finance</td> 
       <td> <p>This is available only for projects and tasks. </p> <p>Displays financial information related to the object. </p> <p>This area is collapsed by default. </p> </td> 
      </tr> 
     </tbody> 
    </table>

1. (Optional) Click the **Collapse All** icon ![](assets/collapse-all-icon-for-custom-forms-on-details-page.png) in the upper-right corner to collapse all the areas. 
1. 
   To add or edit information for fields in the Details section,

  1. Click the **Edit** icon ![](assets/edit-icon.png) in the upper-right corner of the Details section, then do one of the following:

    * Click **Edit all** to open all areas and custom forms for editing.
    * Click **Edit sections**, then click a section or custom form to open it for editing.

     If you use Edit sections to open one area or custom form for editing, you can repeat this step to open others.
  
  1. Edit any field that is available for editing, or click **+Add** to add information to an empty field.

     You can double-click ```or hover over and single-click``` an editable field to edit its contents.

     Fields are not available for editing if they are automatically generated by Workfront or if you don't have editing permissions on them.
  
  1. Click **Save changes** when you ares finished editing information in fields.

1. (Optional) Click the **Export** icon ![](assets/export.png) to export the Overview and custom forms information to a PDF file, then click **Export**. Select from the following:Select all (displays only when there is at least one custom form attached)OverviewThe name of one or multiple custom formsThe PDF file downloads to your computer.

   This is available for the following objects:

  * Projects
  * Tasks
  * Issues
  * Portfolios
  * Programs

   For more information, see [Export custom forms and object details in Adobe Workfront](../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md). 

1. (Conditional) If you have made edits, click **Save Changes**.

   ``` ```**Tips: **``````

  * You can click the Edit icon again if you made no changes and want to close the edit-mode Details page. &nbsp;
  * ```When the Details page is editable, you cannot edit information in the header of the object at the same time. You can only subscribe to the object or add it to your list of favorites before you save your changes.```

