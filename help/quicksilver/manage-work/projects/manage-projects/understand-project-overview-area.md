---
content-type: overview
product-area: projects
navigation-topic: manage-projects
title: Manage information in the project Overview area
description: Manage information in the project Overview area
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6113bc62-18f2-4558-bc2f-986b1e7d1a83
---
# Manage information in the project Overview area

<!--
<p>(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

You can view or edit the information of a project by accessing the Overview area of the Project Details section. There is a limited number of fields that you can view or edit in this area. For information about editing all information for a project see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Projects or higher</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Access the Overview section

1. Go to the project whose Overview section you want to view.
1. Click **Project Details** in the left panel. 
1. The **Overview** section should display first as part of the Project&nbsp;Details and should be expanded by default

   Or

   Click the **Edit** icon ![](assets/edit-icon.png) in the upper-right corner of the Details section,  then click **Overview**. This opens the Overview area for editing.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator configured your Layout Template, the Overview section might not be listed first, in which case it is collapsed. For information, see [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. (Conditional) If there is a specific field that needs to be updated on a project but is not displayed in this section, click &nbsp;the **More menu** ![](assets/more-icon.png) next to the project name, then **Edit** to view more project fields.

   For more information about editing projects, see [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Edit or review the fields in the table below that display in the **Overview** section.   
   To edit any field that is available for editing, click the field or click **+Add** to add information to an empty field.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator configured your Layout Template, all fields might not display. For information, see [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader"><b>Field</b></td> 
      <td><b>Description</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Describe the purpose of this project. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td>Insert any URL in this field. It can be a Workfront URL or any other. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priority</td> 
      <td>Serves as the designated&nbsp;priority or importance of the project.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>The project&nbsp;Status. </p> <p>Tip: You cannot complete a project unless all tasks and issues have also completed. If the Completion&nbsp;Mode of the Project is set to Automatic, you cannot manually complete a project. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Condition&nbsp;Type</td> 
      <td>Determines if the manager sets the Condition&nbsp;of the project or if Workfront does.&nbsp;For information about Project&nbsp;Condition, see the article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Overview of Project Condition and Condition Type</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schedule Mode</td> 
      <td>Sets how the project is scheduled.&nbsp;For example, whether the project is scheduled from Start Date or from the Completion Date.&nbsp;</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Start Date and Time</td> 
      <td> When the project is planned to start. This is manually set by the project manager when the project is scheduled from Start&nbsp;Date. Workfront automatically sets this date when the project is scheduled from&nbsp;Completion&nbsp;Date, based on the duration of the tasks in the project.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planned Completion Date and Time</td> 
      <td> When the project is planned to complete. This is manually set by the project manager when the project is scheduled from Completion Date. Workfront automatically sets this date when the project is scheduled from&nbsp;Start Date, based on the duration of the tasks in the project. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Portfolio</td> 
      <td>The portfolio associated with the project. You must create the portfolio before you can add it to a project. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Program</td> 
      <td>The program associated with the portfolio of the project. You must create the program before you can add it to a project. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group</td> 
      <td> <p>The Group associated with the project.</p> <p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
      By default, one of the following groups is automatically associated with a project when it is created, unless you specify a different group:
        <ul> 
         <li> <p><span>When the project is created from the Projects area, project creator's Home Group is associated with the project.</span> </p> </li> 
         <li> <p><span>When the project is created from a group's main page in the Setup area, that group is automatically associated with the project.</span> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Company</td> 
      <td>The Company associated with the project. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Project Owner </td> 
      <td>This is the owner of the project. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Project Sponsor</td> 
      <td> <p>This is the primary stakeholder for the project. This is usually an executive overseeing and championing the project, or it is the person with budgetary responsibility.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Manager</td> 
      <td> <p>This is the person who can manage user resources in the project. </p> <p>For information about Resource Managers, see the article <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md" class="MCXref xref">Designate Resource Managers for a project or template </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >When updating the Project Owner, Project Sponsor, and Resource Manager fields, notice the avatar, the user's Primary Role, or their email address to distinguish between users with identical names. 
   >
   >Users must be associated with at least one job role to view it as you add them.
   > 
   >You must have the View Contact Info setting enabled in your access level for Users to view users' emails. For information, see [Grant access to users](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md). 


1. Review the following fields in the Overview section. You cannot edit the following fields: 

   | Field |Description  |
   |---|---|
   | Reference Number |This is an automatically generated field and it always has a unique value for each project.  |
   | Projected Start Date |This is a 'real time' date of when work is going to start based on completed work and remaining work. |
   | Projected Completion Date |This is a 'real time' date of when the project is going to be completed based on the progress of completed tasks and based on the progress updates on the tasks that are either New or In Progress status. |
   | Planned Hours |Hours planned on the project. These hours are a total of Planned Hours for each task.  |
   | Actual Hours |Hours logged on the project. These hours are a total of the logged hours on the project, the tasks, or the issues of the project.  |
   | Planned Duration |Amount of time the project will span, based on the time frame between the earliest Planned Start Date of a task and the latest Planned Completion Date of a task on the project.  |
   | Actual Duration |Amount of time the project will actually span, based on the timeframe between the earliest Actual Start Date of a task and the latest Actual Completion Date of a task on the project.  |
   | Entry Date |The date and time when the project is created.  |
   | Entered By |The name of the user who created the project.  |
   | Last Update Date |The date and time when the project was last updated.  |
   | Last Updated By |The name of the user who last updated the project.  |
   | Template |&nbsp; |

  
1. If your company has purchased an additional license for the Adobe Workfront Scenario Planner, and the project has information published from a linked initiative, review the following initiative information in the Scenario Planner area:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><b>Field</b></td> 
      <td><b>Description</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader"><span>Initiative Duration</span> </td> 
      <td><span>The duration of the corresponding initiative when the project is linked to an initiative. This field is not editable.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Last Published Date</span> </td> 
      <td><span>The date when the project was last published from a corresponding initiative.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Initiative Start Date</span> </td> 
      <td><span>The first day of the start month of the initiative, when the project is linked to an initiative.</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Initiative End Date</span> </td> 
      <td><span>The last day of the end month of the initiative, when the project is linked to an initiative.&nbsp;</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Initiative Job&nbsp;Roles in FTEs and Hours</span> </td> 
      <td> <p>Information about the associated job roles and their time allocations for the initiative.&nbsp;This includes:</p> 
       <ul> 
        <li>Job&nbsp;Role name</li> 
        <li>Number of FTEs</li> 
        <li> <p>Number of Hours for all&nbsp;FTEs</p> <p>You can estimate the amount of job roles needed for your plan or initiative using hours or FTEs.&nbsp;</p> <p>For more information, see <a href="../../../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>. </p> </li> 
       </ul> <p>Tip: <span>If the number of job role is different for each month in the initiative, this field displays the maximum amount of roles needed for the initiative. For example, if you need 1 Consultant for January and 2 for February, the column displays 2FTE and the corresponding amount of hours for 2 FTEs for all months.</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   For information about linking projects with initiatives, see [Update or create projects by publishing initiatives in the Scenario Planner](../../../scenario-planner/publish-scenarios-update-projects.md).

1. Click **Save Changes**.
