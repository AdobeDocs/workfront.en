---
product-area: projects;templates
navigation-topic: create-projects
title: Create a project using a template
description: You can use templates as a framework to create projects in Adobe Workfront. If you have projects that repeat often, using templates for the general timeline of the new project saves you from having to build the same projects repeatedly.
author: Alina
feature: Work Management
exl-id: 622cbfe0-b8c0-4045-bef2-9e21d45bfda0
---
# Create a project using a template

<!-- Audited: 01/2024 -->

You can use templates as a framework to create projects in Adobe Workfront. If you have projects that repeat often, using templates for the general timeline of the new project saves you from having to build the same projects repeatedly.

Templates provide you with a way to capture repeatable processes, information, and settings associated with your projects. The information associated with a template is transferred to the project. This includes tasks, assignments, durations, documents, financial details, risks, and custom forms.

>[!TIP]
>
>Workfront defines the Group and Status of the new project as follows:
>
>* The default status of a new project created from a template corresponds with the status defined by your Workfront administrator in the main Project Preferences area, or by a group administrator (or Workfront administrator) in the Project Preferences area for a group. For information about configuring project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) or [Configure project preferences for a group](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md). 
>
>* The Group of the new project is the Group of the template. If the template is not associated with a Group, then the Group of the project is the Home Group of the user who creates the project.
>
>* The statuses available for a new project match the statuses of the Group of the project, which is either the Group of the template, or the Home Group of the user who creates the project. 

You have the following options for creating a project from a template:

* Create a project from a template in the Projects area
* Create a project from a template at the template level
* Attach a template to an existing project

  For information, see [Attach a template to a project](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Create a project from a template in the Groups area

## Access requirements

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and to Templates</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects and to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a template</p> <p>When you create a project, you automatically receive Manage permissions to the project.</p></td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Create a project from a template in the Projects area

You can create a project from the Projects area in the Main Menu , or from the Projects area of a portfolio or a program.

1. Do one of the following:

   * Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner. Click **Projects**, then expand **New Project**. 
   * Go to a portfolio, then expand **New Project**.

     >[!TIP]
     >
     >When you create a project using a template from a portfolio, the Portfolio field of the new project updates to display the portfolio you chose to create the project from. This overwrites the Portfolio field on the template, if it is specified.

   * Go to a program, then expand **New Project**.

     >[!TIP]
     >
     >When you create a project using a template from a program, the Program field of the new projects updates to display the Program you chose to create the project from. The Portfolio field of the template updates to display the portfolio of the program you chose to create the project from. This overwrites the Program and Portfolio fields on the template, if they are specified.

   * If you are a group administrator, you can also create a project in the Projects section of a group you manage. For more information, see [Create and modify a group's projects](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

     >[!TIP]
     >
     >When you create a project using a template from a group, the group you create the project from displays in the Group field of the new project only when the Group field of the template is not specified. If the template Group field is specified, the Group field of the new project is that of the template.

   <!--
   <p>(this, above, is hyperlinked to the classic version of this article; the Milestone View steps are similar to creating a project in Classic than to the way you do it in NWE)</p>
   -->

   ![New Project options](assets/new-project-dropdown.png)

1. Click the name of a template in the **Favorite templates** list.

   ![Select a favorite template](assets/new-project-from-template-dropdown-with-template-favorites.png)

   Or

   Do the following:

   1. Select **New Project from Template**.
   1. In the **Search Templates** field, start typing the name of a template and click it when it displays in the list.
   1. Review the template details on the right.
   
      The template details include the following:

      * Template duration
      * Template owner
      * The number of top-level tasks, which includes the names of the top three tasks
      * The number of all tasks in the template
      * The names of the template custom forms

   1. (Optional) Hover over the name of a template name in the left pane and click the **Favorites** **icon** ![](assets/favorites-icon-small.png) to mark it as a favorite for future use.

      Or

      Expand the **Favorite templates** list and select a template from the drop-down list.

      >[!TIP]
      >
      >You can have up to 40 Workfront items marked as favorites. This includes templates and other items.

   1. Click **Use template** when you have selected a template.

      ![Template details](assets/new-project-from-template-small-box-with-template-details-panel.png)

      >[!NOTE]
      >
      >If you have the Milestone View applied to the list of projects, click the name of a template in the **New from Template section**.
      >
      >
      >![Milestone view of creating a project from a template](assets/create-project-from-template-box-from-milestone-view-nwe-350x275.png)
      >

   The **New Project** box opens.

   ![New Project box](assets/new-project-from-template-box.png)

1. If a field is already populated in the template, the field is pre-populated in the **New Project** box. You can edit the pre-populated values to better match your project. For more information, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).
1. Click **Create Project**.

   All details defined in the template associate automatically with the newly created project if you didn't change them in the previous step.

## Create a project from a template in the Templates area

Instead of starting in the Projects area, you can create a project from a template by starting with the template.

{{step1-to-templates}}

1. Click the name of a template you want to use.
1. Click the **More** menu ![](assets/more-icon.png), then click **Create Project**.

   ![Create project from template](assets/project-sharing-on-template.png)

   The **New Project** box opens.

1. Enter a name for the project, then review each section and make any necessary changes.

   ![New Project box](assets/new-project-from-template-box.png)

   If a field is already populated in the template, the field is pre-populated in the **New Project** box. You can edit the pre-populated values to better match your project. For more information, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Click **Create Project**.

   All details defined in the template associate automatically with the newly created project if you didn't change them in the previous step.
