---
filename: import-projects-to-plans
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Import projects to plans in the Scenario Planner
description: You can import existing projects into a plan. The imported projects are converted to initiatives and you can manage them within the plan as you would manage a new initiative. The original project remains linked to the new initiative.
---

# Import projects to plans in the Scenario Planner

You can import existing projects into a plan. The imported projects are converted to initiatives and you can manage them within the plan as you would manage a new initiative. The original project remains linked to the new initiative.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Access requirements

You must have the following:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront<b> plan*</b> </p> </td> 
   <td>Business or higher</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront<b> license*</b> </p> </td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Product</b> </td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Scenario Planner to access functionality described in this article.</p> <p>For information about obtaining the Workfront Scenario Planner, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Scenario Planner</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access or higher to the Scenario Planner</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Manage permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the Scenario Planner</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations about importing projects into plans as new initiatives

* You must create projects before you can import them into a plan as new initiatives.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* You must have at least View permissions to the projects to be able to import them into a plan as new initiative. 
* You can import the same project into multiple plans. 
* The projects you want to import must have dates included in the time frame of your plan. You cannot import projects with a Planned Completion Date earlier than the start of the plan or a Planned Start Date later than the end of the plan. 
* You cannot import more than 100 projects at a time. 
* Some project information is also imported into the plan and becomes initiative information. For information about what project information is imported into the plan and becomes initiative information, see the [Project information imported into the plan](#project-information-imported-into-the-plan) section in this article. 
* Changes that occur on the linked projects do not affect the initiatives on the plan. 
* Changes that occur on the initiatives on the plan do not automatically affect the linked projects Initiative changes affect the linked projects only when you publish the initiative from the plan. For information about how publishing initiatives affects the linked projects, see [Update or create projects by publishing initiatives in the Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md). 
* Deleting an initiative that has been created by importing a project does not delete the project. 
* Deleting a project linked to an initiative does not delete the initiative.

## Project information imported into the plan {#project-information-imported-into-the-plan}

When you import a project into a plan some project information is also imported into the plan and it becomes initiative information. The following table shows what project information becomes initiative information when you import a project into a plan:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Project information</td> 
   <td>Initiative information </td> 
  </tr> 
  <tr> 
   <td>Project&nbsp;Name</td> 
   <td>Initiative name</td> 
  </tr> 
  <tr> 
   <td>Project Planned Dates</td> 
   <td> <p>Initiative start and end months.</p> <p>If a project starts or ends in the middle of a month, the imported dates are extended to cover a full month in the plan.&nbsp;For example, if the Project Planned Dates are March 20 - May 5, 2020, then the dates of the imported initiative are March - May, 2020.</p> <p>If the Planned Start or Completion Date is beyond the duration of the plan, there is a visual indication that the imported initiative starts before or ends after the plan. </p> </td> 
  </tr> 
  <tr> 
   <td>Job roles assigned to tasks and issues</td> 
   <td> <p>Initiative Job&nbsp;Roles. </p> <p>Note:   <p>If a user changes roles during the life of the project, the roles that are imported depend on the status of the assignment when you import the project. The following scenarios exist:</p> 
     <ul> 
      <li> <p>If a user assigned to a task or an issue changed their role after they marked their assignment as Done, Workfront imports to the initiative the role the user fulfilled before they marked the assignment as Done.</p> </li> 
      <li> <p>If a user assigned to a task or issue changed the role during the life of the project but their assignment on the task or issue is not marked as Done when you import the project, Workfront imports only the current role of the assigned user. </p> </li> 
     </ul> <p>For information about the status of an assignment, see "Assignment Status" in <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossary of Adobe Workfront terminology</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Project Planned Hours associated with job roles assigned to tasks or issues</td> 
   <td> <p><span>Depending on whether the plan is set up to use FTEs or hours, the Planned Hours from the tasks on the project become either</span> Required FTEs <span>or Required hours on the plan</span>. </p> <p>For information about setting up a plan to use&nbsp;FTEs or hours, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>. </p> <p>Consider the following:</p> 
    <ul> 
     <li> <p>Workfront uses the job roles assigned to tasks and issues or the job roles that the users assigned to tasks or issues are associated with on the project and transfers them to the new initiative as Required Job&nbsp;Roles. </p> </li> 
     <li> <p>When the plan is set up to use FTEs, the Planned Hours associated with the job roles on the tasks and issues of the project are first converted to FTE.&nbsp;This FTE is then assigned to the initiative's job role. <span>Planned Hours are equally distributed in Workfront. If a task or an issue spans multiple months, the amount of Planned Hours for each month in the duration of the initiative is converted in monthly FTE and transferred to each month of the initiative.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span>For example, if a task is assigned to a job role for 80 Planned Hours in September, then the imported job role displays 0.5 FTE for the initiative in September.</span> </p> </li> 
     <li> <p>Workfront calculates the FTE of the Required Job&nbsp;roles associated with the initiative using the following formula:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Tip: The Scenario Planner assumes that there are 160 working hours in a month.</p> <p>For example, if a project has a Duration of 1200 minutes and a job role on the project is associated with 600 minutes of Planned Hours, their FTE is 0.5. When importing the project, the Required Job Role FTE on the newly created initiative is 0.5 for each month of the initiative. </p> </li> 
     <li>When a job role is assigned to a task on the project with zero Planned Hours, the Required FTE for the job role of the initiative is zero by default. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>When a job role is assigned to a task on the project with a zero Duration, the Required FTE&nbsp;<span>or hours</span> for the job role of the initiative is zero by default, even if the task has Planned Hours. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

## Import projects into a plan

>[!IMPORTANT]
>
>After importing projects into a plan, they become initiatives on the plan. Although the two items are linked, they exist as independent entities and do not automatically affect each other when they are updated. 
>
>The following occur:
>
>* Changes to the project never affect the initiative after you import the project into the plan.These changes include changes to the job role allocations. 
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>* Changes to the initiative affect the information in the Scenario Planner area on the project only when you publish the initiative to the corresponding project. Otherwise, they do not affect the Planned Hours information for the tasks and issues of the project. 
>
>  ```For information about how publishing initiatives affects the linked projects, see``` ``` [Update or create projects by publishing initiatives in the Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md)```. 
>

1. Click the **Main Menu** ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click&nbsp;Scenarios to access the Scenario Planner.

1. Click the name of a plan where you want to import projects.
1. Click **New Initiative**, then click **Import Projects**.

   The Import Projects box displays. Projects that have dates included in the time frame of your plan display in a list.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >Projects in any status display in the list.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Optional)&nbsp;Click the **Filter icon** ![](assets/filter-nwepng.png)and select an available filter from the list to reduce the amount of projects on your list. By default, the list of projects is filtered by the user's currently selected project filter in a list of projects. 

1. (Optional) Click the **Search icon** ![](assets/search-icon.png) and add a keyword displayed on any field on the screen. The items containing the search word display in the list automatically and all items are hidden. 

1. (Conditional)&nbsp;Click the **X icon** to remove the search and display all projects. 
1. Select up to 100 projects and click **Import**.

   The projects are imported as new initiatives.

   Notice the following:

   * A project icon ![](assets/project-icon-sp.png) displays to the right of the initiative name.
   * If the project timeline exceeds the duration of the plan, the bar of the initiative ends with a pointed margin to the left (when the Start Date is earlier than the plan's date) or to the right (when the End Date is later than the plan's date).

     ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * The number of months and job roles have been updated to match those of the project.

   >[!TIP]
   >
   >The costs associated with the job roles update at the initiative level and are not imported from the project.

1. Click the bar representing the new initiative to open the initiative details panel to the right.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   In the **Initiative Duration** area review the following information: 

   <table> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Initiative Duration</td> 
      <td>This is the duration of the initiative in months. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Initiative</td> 
      <td>The Start and End dates of the initiative. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Project</td> 
      <td> <p>The Planned Start and Completion dates of the linked project.</p> <p>Tip: If the Project information is missing, the project was deleted.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Edit the name of the initiative. By default, it matches the name of the project. 
1. (Optional) Do one of the following:

   * Update job roles in the **Required Job Roles** section
   * Update the **Fixed Costs** in the **Costs** section
   
   * Click **Update available job roles** or **Update available budget** to resolve conflicts between the new initiative and other initiatives on the plan.

1. (Conditional) Click **Apply** to save changes to your initiative. 
1. Click&nbsp;**Save Plan** to save the changes to your plan. 
1. (Optional) To update the changes you make to the initiative back to the project it was imported from, publish the project from the plan.&nbsp;For information about publishing plans, see [Update or create projects by publishing initiatives in the Scenario Planner](../scenario-planner/publish-scenarios-update-projects.md). 
1. (Optional) Click the project icon to access the linked project.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)

