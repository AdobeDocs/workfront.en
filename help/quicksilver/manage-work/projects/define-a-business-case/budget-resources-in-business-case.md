---
filename: budget-resources-in-business-case
navigation-topic: business-case-and-scorecards
title: Budget resources in the Business Case
description: As part of resource planning, you can budget the job roles necessary for completing the work in a project when you build the business case. For more information about creating a Business Case, see Create a Business Case for a project .
---

# Budget resources in the Business Case

As part of resource planning, you can budget the job roles necessary for completing the work in a project when you build the business case. For more information about creating a Business Case, see [Create a Business Case for a project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!NOTE]
>
>Budgeting resources is not the same as scheduling resources for a project. When you budget resources you estimate the roles that might be necessary to complete the work on a project. For actually scheduling or assigning users to the work on a project, see [Get started with Resource Scheduling](../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md). For information about resource planning in Adobe Workfront, see [Get started with Resource Planning](../../../resource-mgmt/resource-planning/get-started-resource-planning.md).

You must associate job roles with the project before you can budget the resources for it. The following are ways of allocating job roles to a project:

* Use the Resource Planner to apply Resource Pools to the project and budget job roles.

  For more information, see [Budget resources in the Business Case using the Resource Planner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md). 

* Use the Scenario Planner to create initiatives with required job roles and link them to the project. For more information, see [Budget resources in the Business Case using the Scenario Planner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md) .

  >[!NOTE]
  >
  >The Scenario Planner is available only in the new Adobe Workfront experience and requires an additional license. For information about the Workfront Scenario Planner, see [The Scenario Planner overview](../../../scenario-planner/scenario-planner-overview.md).

##

##

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:ALL content below has been moved to another article - we now have two "how to" budget in the business case: one for the resource planner and one of the scenario planner)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can associate Resource Pools with a project as part of completing the Resource Budgeting section of the Business Case of the project. The information you update here is also reflected in the Resource Planner.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> For more information about creating a Business Case, see <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Create a Business Case for a project </a>. For more information about planning in the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p>
-->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="prerequisites"></a>Prerequisites for budgeting resources on a project</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To successfully budget your resources in the Business case, you must have the following information available in Adobe Workfront:</p>
-->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have Edit access to projects in your access level.</li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have Manage permissions on the project to be able to edit the Business Case of the project. </li>
  -->

* 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have Edit access to Resource Management and Financial Data, as well as Manage Finance permissions on the project.</p>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the access needed to budget resources, see <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p>
  -->

* 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have Resource Pools attached to the project.</p>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools)</p>
  -->

  <!--
  <note type="note">
  You cannot budget resources assigned to issues in the Business Case. You can budget them in the Resource Planner. For more information about the Resource Planner, see
  <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.
  </note>
  -->

* 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must understand user and job role availability according to the Resource Management Preferences in your system.</p>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Obtaining information about user availability depends on how your Workfront administrator configures your Resource Management Preferences.</p>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about calculating user availability and setting Resource Management Preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p>
  -->

* 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In order to calculate the Budgeted Labor Cost of the project, you must associate users and job roles with Cost per Hour rates. </p>
  -->

  <!--
  <note type="note">
  Cost displays in the Business Case in the currency of the project.
  </note>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about associating Cost per Hour rates with job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p>
  -->

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about associating Cost per Hour rates with users, see <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Although this is not a prerequisite, we also recommend that you might also have Planned Hours associated with your tasks, to understand the amount of work a task might need to complete. </li>
  -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode"><a name="applying-resource-pools-to-the-business-case"></a>Apply Resource Pools to a project and budget resources in the Business Case</h2>
-->

<!--
<note type="important">
You can budget your resources for a period of 15 years. If you budget resources for a project with a duration longer than 15 years the budgeting information might not be accurate.
</note>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To apply Resource Pools and budget project resources in the Business Case for a project with no Resource Pool:</p>
-->

   <!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to the project which you want to associate with the Resource Pools. </li>
   -->

   <!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the <strong>Project Details</strong> tab. </li>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the <strong>Business Case</strong> sub-tab. </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Business Case</strong> in the left panel. </p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Resource Budgeting</strong> section, click <strong>Edit Resource Budgeting</strong>. </p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Select Resource Pool</strong> field, specify one or several <strong>Resource Pools</strong>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You must specify only Resource Pools that are populated with active users.</p>
   -->

   <!--
   <note type="tip">
   If the project is already associated with Resource Pools, the Resource Planner displays by default. To add more Resource Pools to the project, edit the project. For information about editing a project, see
   <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.
   <br>
   </note>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Apply</strong>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Resource Planner is displayed, for the selected project.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about the Resource Planner, see <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/bc-resource-budgeting-area-350x276.png" alt="BC_resource_budgeting_area.png" style="width: 350;height: 276;"> </p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Click <strong>Week</strong>, <strong>Month</strong> or <strong>Quarter</strong> to display information for the project in different time frames.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Today</strong> to return to today's time frame.</p>
   -->

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Click the <strong>Hours</strong> drop-down menu, and select <strong>Hours</strong>, <strong>FTE</strong>, or <strong>Cost</strong> to change how information displays in the Resource Planner. Hours display by default.</li>
   -->

   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Click <strong>Export</strong> to export the Resource Planner to an Excel file.<br><!--
   <note type="note">
   You can export data for up to 12 time periods at a time.
   </note>
   --></li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Click the <strong>Full Screen</strong> icon <img src="assets/full-screen-rp-in-bc.png" alt="full_screen_RP_in_BC.png"> to display the Resource Planner in full screen mode.<br></li>
   -->

   <!--
   <li value="11" data-mc-conditions="QuicksilverOrClassic.Draft mode">Update the <strong>BDG</strong> (Budgeted Hours) field with Hour, FTE, or Cost values for the the users, roles, or the project by doing one of the following: <p>
   <ul>
   <li>
   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Manually estimate the amount of Hours, FTE, or Cost values for roles, users, or the project.</p>
   --><!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or</p>
   --></li><!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>Options</strong> icon for the project or the job roles and select an option to automatically budget the hours for roles, users, or the project.</li>
   -->
   </ul><!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about budgeting in the Project View of the Resource Planner, see the <a href="../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md">Using the Project and Role Views to Budget Resources</a>.</p>
   --><!--
   <note type="note">
   You can budget hours, FTEs, or costs for your resources for any time frame displayed in the Resource Budgeting area, independent of the timeline of the project. For example, if you want to indicate that your resources might not be available during the timeline of the project (where they are associated with Planned Hours), but they might be available during another time, you can do so by budgeting them for time frames where the Planned Hours are zero, if that is when they become available to work.
   </note>
   --></p></li>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) To understand whether you can move the budgeted Hours, FTEs, or Costs to another time frame, click the <strong>Options</strong> icon, then <strong>Adjust Budgeting Dates</strong>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about adjusting budgeted dates, see <a href="../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Adjust budgeting dates in the Resource Planner</a>.</p>
   -->

1. 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save</strong>.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If you have Cost per Hour rates associated with your job roles, budgeting the resources in the Resource Budgeting area calculates the <strong>Budgeted Labor Cost</strong> of the project. The Budgeted Labor Cost is displayed in the Resource Budgeting area of the Business Case and in the Business Case Summary. <br></p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The budgeting information specified in the Business Case is also displayed in the Resource Planner. </p>
   -->

