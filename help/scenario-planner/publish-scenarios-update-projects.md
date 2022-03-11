---
filename: publish-scenarios-update-projects
product-area: enterprise-scenario-planner-product-area
keywords: publish,plans,projects,scenario,scenarios
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Update or create projects by publishing initiatives in the Adobe Workfront Scenario Planner
description: Publishing a scenario from the Adobe Workfront Scenario Planner accomplishes the following:
---

# Update or create projects by publishing initiatives in the `Adobe Workfront Scenario Planner`

Publishing a scenario from the `Adobe Workfront Scenario Planner` accomplishes the following:

* Creates projects from the initiatives on the scenario and links them together.
* Updates projects already linked to initiatives on the scenario with information from the linked initiative. Projects can also be linked to initiatives when you import them in to a plan. For information, see [Import projects to plans in the Adobe Workfront Scenario Planner](../scenario-planner/import-projects-to-plans.md)

## Access requirements

You must have the following:

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><span>Adobe Workfront</span> plan*</p> </td> 
   <td><span>Business</span> or higher</td> 
  </tr> 
  <tr> 
   <td> <p><span>Adobe Workfront</span> license*</p> </td> 
   <td> <p><span>Review</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Product</span> </td> 
   <td> <p>You must purchase an additional license for the <span>Adobe Workfront Scenario Planner</span> to access functionality described in this article.</p> <p>For information about obtaining the <span>Workfront Scenario Planner</span>, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the Adobe Workfront Scenario Planner</a>. </p> </td> 
  </tr> Access level* Edit for Scenario Planner and Projects Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see Create or modify custom access levels. Object permissions Manage permissions for the plan Manage permissions for published projects For information on requesting additional access to projects, see Request access to objects in Adobe Workfront. For information on requesting additional access to a plan, see Request access to a plan in the Adobe Workfront Scenario Planner. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

For additional information about access to the `Workfront Scenario Planner`, see [Access needed to use the Adobe Workfront Scenario Planner](../scenario-planner/access-needed-to-use-sp.md).

## Prerequisites

Before you begin:

* You must use `the new Adobe Workfront experience` to be able to access the `Scenario Planner`. 

* You must create and save a plan before you can publish initiatives from it.

## Considerations about publishing initiatives to projects

<ul> 
 <li>You can publish only one scenario from a plan. </li> 
 <li>One initiative can be linked to only one project.</li> 
 <li> <p>One project can be linked to more than one initiative when the initiatives belong to different plans. </p> <note type="tip">
   <span>When a project exists on multiple plans and you publish information to the project from all plans, the latest publish overwrites the existing <span>Scenario Planner</span> information on the project. </span> 
  </note> </li> 
 <li> <p>If initiatives were created on the plan by importing projects to the plan, publishing the initiative also updates the linked projects with initiative information. </p> <note type="tip">
   You can import the same project into multiple plans. Publishing might overwrite initiative information on a project that is linked to multiple initiatives. 
  </note> <p>For information about creating initiatives by importing projects, see <a href="../scenario-planner/import-projects-to-plans.md" class="MCXref xref">Import projects to plans in the Adobe Workfront Scenario Planner</a>. </p> </li> 
 <li> <p>Any changes made to the project do not transfer to the linked initiative. </p> </li> 
</ul>

&nbsp;

## Publish initiatives

>[!IMPORTANT]
>
>If you make any changes to initiatives on the plan, including resolve conflicts, you must republish the initiative in order for the new information to be visible on the project. This information displays on the projects linked to initiatives only when you publish the corresponding the initiative. For information about resolving conflicts between initiatives, see [Resolve initiative conflicts in the Adobe Workfront Scenario Planner](../scenario-planner/resolve-conflicts-in-sp.md)

<ol> 
 <li value="1"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Workfront</span>, then click <span class="bold">Scenarios</span></p> </li> 
 <li value="2"> <p>(Optional and conditional) If you want to publish from an existing plan, click the <span class="bold">Filter</span> icon <img src="assets/filter-nwepng.png"> in the upper-right corner of the plan and select one of the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">All</td> 
     <td>Displays all plans that you own or are shared with you. This is the default. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">My plans</td> 
     <td>Displays plans that you created.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Shared with me</td> 
     <td> <p>Displays plans you did not create but are shared with you.</p> <note type="important">
       You must have Manage permissions to plans shared with you to be able to publish them. 
      </note> </td> 
    </tr> 
   </tbody> 
  </table> <p> <img src="assets/plans-filters-dropdown-options-scenario-planer.png"> </p> </li> 
 <li value="3"> <p>(Optional)&nbsp;Click the <span class="bold">Search</span> icon <img src="assets/search-icon.png"> and start typing the name of a plan to quickly find it in the list.</p> </li> 
 <li value="4"> <p>(Conditional)&nbsp;To publish from a new plan, create a plan.</p> <p> For information about creating plans, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Adobe Workfront Scenario Planner</a> . </p> </li> 
 <li value="5"> <p>(Optional) Click the name of an existing plan and create new scenarios for the plan.</p> <p>For information about creating scenarios for a plan, see <a href="../scenario-planner/create-and-compare-scenarios-for-a-plan.md" class="MCXref xref">Create and compare plan scenarios in the Adobe Workfront Scenario Planner</a>. </p> </li> 
 <li value="6"> <p>(Optional) Update the initiatives of an existing or a new plan or create new ones.</p> <p>For information about creating initiatives, see <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Create and edit initiatives in the Adobe Workfront Scenario Planner</a>.</p> </li> 
 <li value="7">Click <span class="bold">Save plan</span>. </li> 
 <li value="8"> <p>Select the scenario you want to publish from the <span class="bold">Initial scenario</span> drop-down menu, then click <span class="bold">Go to Publish</span> <img src="assets/go-to-publish-button-icon.png"> in the upper-right corner.</p> <p>Or</p> <p>Click <span class="bold">Compare scenarios</span>, hover over the scenario card that you want to publish from, then click <span class="bold">Go to Publish</span> <img src="assets/go-to-publish-button-icon.png">. </p> <p>The Publish initiatives page displays, showing a list of all initiatives in the scenario. If any of the initiatives was previously published, the project icon <img src="assets/project-icon-sp.png"> displays after their name and the <span class="bold">Last published</span> date is populated in the list. </p> <note type="tip">
   Initiatives that have been created by importing projects also display the project icon 
   <img src="assets/project-icon-sp.png"> to the right of their name
  </note> <p> <img src="assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png" style="width: 350;height: 63;"> </p> </li> 
 <li value="9"> <p>(Optional and conditional) If you want to publish from an existing plan, click the <span class="bold">Filter</span> icon <img src="assets/filter-nwepng.png"> in the upper-right corner of the plan and select one of the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">All</td> 
     <td>Displays all initiatives of the selected scenario. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Published</td> 
     <td>Displays initiatives that you or another user published before. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Unpublished</td> 
     <td> <p>Displays unpublished initiatives. </p> </td> 
    </tr> 
   </tbody> 
  </table> <p> <img src="assets/initiatives-fitler-in-publishing-screen-scenario-planner.png"> </p> </li> 
 <li value="10"> <p>(Optional)&nbsp;Click the <span class="bold">Search</span> icon <img src="assets/search-icon.png"> and start typing the name of an initiative to quickly find it in the list.</p> </li> 
 <li value="11"> <p>Select one or multiple initiatives to publish and create or update projects from them, then click <span class="bold">Publish initiatives</span>. </p> <p>This creates a new project from each selected initiatives or updates the existing connected projects, if the published initiatives were already linked to a project. </p> <note type="tip">
   New projects have the same name as the published initiatives. 
  </note> </li> 
 <li value="12"> <p>(Conditional) Do one of the following: </p> 
  <ul> 
   <li> <p>If you published one initiative, click <span class="bold">See associated project</span> to open the project created or updated from the initiative. </p> </li> 
   <li> <p>If you published more than one initiative, click&nbsp;<span class="bold">See associated projects</span> to open a list of projects published from initiatives. <span>Workfront</span> applies the Scenario Planner Projects filter to the list of projects by default. The projects published most recently display at the top of the list. </p> <p> <img src="assets/scenario-planner-filter-after-publishing-initiatives-350x81.png" style="width: 350;height: 81;"> </p> </li> 
  </ul> </li> 
 <li value="13"> <p>Go to the following areas to view initiative information on the project:</p> 
  <div> 
   <ul> 
    <li> <p><b>The Updates section</b>: An update publishes to indicate that the project was created or updated from the initiative. The update contains the name of the initiative that created or updated the project and the linked name of the plan that contains the initiative. You can click the name of the plan in the update to open the plan in the <span>Scenario Planner</span>. </p> <p> <img src="assets/update-stream-confirmation-of-publish-on-project-350x65.png" style="width: 350;height: 65;"> </p> </li> 
    <li> <p><b>The Overview area of the Project Details section</b>: A new Scenario Planner section is created in this area that contains information from the linked initiative. </p> <note type="tip">
      This information is visible only when viewing Project&nbsp;Details in 
      <span>the new Adobe Workfront experience</span>. 
     </note> <p> <img src="assets/scenario-planner-on-project-details-350x135.png" style="width: 350;height: 135;"> </p> <p>The following initiative information is published in the Scenario Planner area of the Project&nbsp;Details section:</p> <p> 
      <table cellspacing="0"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader"><span>Initiative Duration*</span> </td> 
         <td><span>The duration of the corresponding initiative when the project is linked to an initiative. This field is not editable.</span> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"><span>Last Published Date*</span> </td> 
         <td><span>The date when the project was last published from a corresponding initiative.</span> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"><span>Initiative Start Date*</span> </td> 
         <td><span>The first day of the start month of the initiative, when the project is linked to an initiative.</span> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"><span>Initiative End Date*</span> </td> 
         <td><span>The last day of the end month of the initiative, when the project is linked to an initiative.&nbsp;</span> </td> 
        </tr> 
        <tr> 
         <td role="rowheader"><span>Initiative Job&nbsp;Roles in FTEs and Hours*</span> </td> 
         <td> <p>Information about the associated job roles and their time allocations for the initiative.&nbsp;This includes:</p> 
          <ul> 
           <li>Job&nbsp;Role name</li> 
           <li>Number of FTEs</li> 
           <li> <p>Number of Hours for all&nbsp;FTEs</p> <p>You can estimate the amount of job roles needed for your plan or initiative using hours or FTEs.&nbsp;</p> <p>For more information, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Adobe Workfront Scenario Planner</a>. </p> </li> 
          </ul> <note type="tip">
           <span>If the number of job role is different for each month in the initiative, this field displays the maximum amount of roles needed for the initiative. For example, if you need 1 Consultant for January and 2 for February, the column displays 2FTE and the corresponding amount of hours for 2 FTEs for all months.</span> 
          </note> </td> 
        </tr> 
       </tbody> 
      </table> </p> <note type="note"> 
      <p>All users with View access to the project can see the <span>Scenario Planner</span> section in the Overview area. You can control whether this area displays in the Details section by using a layout template. If users do not have a layout template associated with them, this area displays by default. </p> 
      <ul> 
       <li> <p>For information about adding or removing areas in the Details section using a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md" class="MCXref xref">Customize the Details view using a layout template</a>. </p> </li> 
       <li> <p>For more information about viewing information in the Overview area of the Project&nbsp;Details, see <a href="../manage-work/projects/manage-projects/understand-project-overview-area.md" class="MCXref xref">Manage information in the project Overview area</a>.</p> </li> 
      </ul> 
     </note> </li> 
    <li> <p><b>The Role Allocation panel in the</b><span>Workload Balancer</span><b> or the task list of the project</b>: Information about role allocation on the initiative populates in this area, in addition to role allocations on the project. </p> <p> For more information, see <a href="../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md" class="MCXref xref">Overview of reconciling resource allocations between projects and initiatives </a>. </p> <p> <img src="assets/role-allocation-panel-350x174.png" style="width: 350;height: 174;"> </p> <p>Any changes to the dates or resources of the project do not affect the corresponding initiative or any of the areas on the project that contain initiative information. </p> </li> 
    <li> <p><b>The Resource Budgeting area of the Business Case of the project</b>: A new option for managing project resources using <span>Scenario Planner</span> information is added in the Resource Budgeting area of the Business Case of the project. </p> <p>For more information, see <a href="../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md" class="MCXref xref">Budget resources in the Business Case using the Adobe Workfront Scenario Planner</a>. </p> <p> <img src="assets/sp-in-business-case-selected-350x110.png" style="width: 350;height: 110;"> </p> </li> 
   </ul> 
  </div> </li> 
 <li value="14"> <p>(Optional) Review the following information in the <span>Scenario Planner</span> after you published a scenario: </p> 
  <ul> 
   <li>The published scenario becomes the first scenario after you publish initiatives from it. </li> 
   <li>You cannot publish from any other scenario after you have published a scenario at least once. </li> 
   <li>The Go to Publish option is removed from all other scenarios after at least one initiative has been published from a scenario. </li> 
   <li> <p>A green indicator displays next to the published initiatives' project icons in the plan. </p> <p> <img src="assets/indicator-for-published-initiative-icon-350x119.png" style="width: 350;height: 119;"> </p> </li> 
   <li> <p>A green "Published"&nbsp;indicator displays at the top of the scenario and on the scenario card and the Published field is populated on the scenario card indicating the number of initiatives in the scenario that have been published. </p> <p> <img src="assets/published-scenario-highlighted-350x632.png" style="width: 350;height: 632;"> </p> <note type="tip">
     If all the projects published from the scenario's initiatives are deleted, the indication that the scenario has been published is removed. For information, see 
     <a href="../manage-work/projects/manage-projects/delete-projects.md" class="MCXref xref">Delete projects </a>. 
    </note> </li> 
  </ul> </li> 
 <li value="15"> <p>(Optional) Update information on the initiative and repeat the process described above to republish the initiative and update initiative information on the linked project. </p> <p>For information about editing initiatives, see <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Create and edit initiatives in the Adobe Workfront Scenario Planner</a>. </p> </li> 
</ol>

&nbsp;
