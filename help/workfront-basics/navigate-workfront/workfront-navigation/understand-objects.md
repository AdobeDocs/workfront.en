---
filename: understand-objects
content-type: overview;reference
navigation-topic: workfront-navigation
title: Understand objects in Adobe Workfront
description: The information you display in Adobe Workfront is represented by objects which are stored in the Workfront database. The objects are what drives the information in Workfront.
---

# Understand objects in *Adobe Workfront*

The information you display in *Adobe Workfront* is represented by objects which are stored in the *Workfront* database. The objects are what drives the information in *Workfront*.

Understanding how the objects are defined in *Workfront* is important so you can use the correct object for the needs necessary in your organization.

For example, when you plan a large amount of work, you need to use the Project object to define that work. To divide this work into smaller planned increments, you can use the Task object. For a smaller amount of work that is not planned, and can occur unexpectedly, you can use the Issue object. If you want to track the progress and the adherence to budget and timeline of a group of projects, you can organize them in Portfolios and Programs. To define other elements that help you resolve your work, you want to use other objects that are stored under Projects, Tasks, Issues, or Portfolios, like Documents, Notes, Hours, Users, or Job Roles.

Reports and Dashboards are another example of objects that can help you organize the amount of data you have in *Workfront* visually, to make it easily accessible for all users.

For a complete list of objects in *Workfront*, see the [API Explorer](../../../wf-api/general/api-explorer.md).

## Interdependency and hierarchy of objects

Objects are linked to one another in *Workfront*. For example, a task or an issue can never exist independently outside of a project. Tasks and issues are examples of objects that are stored in the project object. Tasks and issues are considered child objects to projects.

The following are some of the most commonly used objects in *Workfront* and their respective parent and children objects:

| `Object`  | `Parent objects`  | `Child objects`  |
|---|---|---|
| Portfolios |  |Programs, Projects, Documents, Notes, Users |
| Programs |Portfolios |Projects, Documents, Notes, Users |
| Projects |Portfolios, Programs |Tasks, Issues, Documents, Notes, Hours, Users |
| Tasks |Projects |Issues, Children Tasks, Documents, Notes, Hours, Users |
| Issues |Tasks, Projects |Documents, Notes, Hours, Users |
| Dashboards |  |Reports, External Pages |
| Reports |Dashboards |  |
| Groups |  |Users |
| Teams |  |Users |
| Users |Groups, Teams, Companies |Job Roles |
| Companies |  |Users |
| Documents |Tasks, Issues, Projects, Portfolios, Programs, Users |  |
| Plans&#42;  |&nbsp; |Initiatives |
| Plans&#42;  |&nbsp; |Initiatives |
| Goals&#42; |&nbsp; |Results,&nbsp;Activities |
| Goals&#42; |&nbsp; |Results,&nbsp;Activities |

For a complete list of objects in *Workfront*, see the [API Explorer](../../../wf-api/general/api-explorer.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">* Plans are the objects of the <em>Workfront Scenario Planner</em>. For information about the <em>Scenario Planner</em>, see <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">The Adobe Workfront Scenario Planner overview</a>.</p>
-->

&#42; Plans are the objects of the *Workfront Scenario Planner*. For information about the *Scenario Planner*, see [The Adobe Workfront Scenario Planner overview](../../../scenario-planner/scenario-planner-overview.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">*&nbsp;Goals are the objects of <em>Workfront Goals</em>.&nbsp;For information about <em>Workfront Goals</em>, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront Goals overview</a>. </p>
-->

&#42;&nbsp;Goals are the objects of *Workfront Goals*.&nbsp;For information about *Workfront Goals*, see [Adobe Workfront Goals overview](../../../workfront-goals/goal-management/wf-goals-overview.md).

## Customize object names

As a *Workfront administrator*, you can customize object names in *Workfront* by using a Layout Template.

For more information about how to customize object names using a Layout Template, see [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

After you customize a layout template and you assign it to users, those users see the customized names for the objects. The users that have been assigned to the layout template no longer see the default names for the objects anywhere in the web application.

>[!NOTE]
>
>For the new names of the objects to be visible for your users, they must log out and log back in to *Workfront* after you have saved the Layout Template.

>[!IMPORTANT]
>
>The *Workfront* documentation always refers to the default names of the objects. As a *Workfront administrator*, ensure that you notify users of the changes in object names, so they can understand how to use the *Workfront* documentation, as well as the areas of the applications which do not reflect the changes in the names of the objects.

* [Object names that can be customized using a Layout Template](#objects-that-can-have-customized-names) 
* [Areas of Workfront that reflect the customized object names](#areas-with-cutomized-object-names) 
* [Areas of Workfront that do not reflect the customized object names](#areas-without-customized-names)

### Object names that can be customized using a Layout Template

As a *Workfront administrator*, you can customize the names of the following objects to match the terminology in your organization:

* Portfolio
* Program
* Project
* Task
* Issue

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Goal*</li>
  -->

* Goal&#42;

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver">Result*</li>
  -->

* Result&#42;

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Activity*</p> <p>*Goals, results, and activities are only available if your company purchased <em>Workfront Goals</em>.&nbsp;For information about <em>Workfront Goals</em>, see <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront Goals overview</a>.</p> </li>
  -->

* Activity&#42;

  &#42;Goals, results, and activities are only available if your company purchased *Workfront Goals*.&nbsp;For information about *Workfront Goals*, see [Adobe Workfront Goals overview](../../../workfront-goals/goal-management/wf-goals-overview.md).

For example, if the larger amount of work in your organization is known as a 'Campaign', you can replace the name 'Project' with 'Campaign'. Your *Workfront* interface shows 'Campaign' instead of 'Project' everywhere where the name 'Project' would appear.

For more information about how you can customize object names using Layout Templates, see [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

You cannot customize the names of any other object in *Workfront*. For a complete list of objects in *Workfront*, see the [API Explorer](../../../wf-api/general/api-explorer.md).

When you customize the name of an object, the new name for that object appears in most areas of the *Workfront* application where that object name would appear.

### Areas of *Workfront* that reflect the customized object names

The following areas show the updated name of the objects:

* 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  Top Navigation
  </MadCap:conditionalText>
  -->

  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Top Navigation</MadCap:conditionalText>` 

* All 

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  sections in the left panel navigation
  </MadCap:conditionalText>
  -->

  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> sections in the left panel navigation</MadCap:conditionalText>`

* All menus
* In-app notifications
* Report builder and reporting elements (views, filters and groupings)
* Save buttons
* Exported files
* Emails
* Mobile Apps

### Areas of *Workfront* that do not reflect the customized object names

The following areas do not show the updated name of the objects:

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Legacy Gantt</li>
  -->

* Legacy Gantt

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates</li>
  -->

* Resource Estimates

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Budget Manager</li>
  -->

* Resource Budget Manager

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Capacity Planner</li>
  -->

* Capacity Planner

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Grid</li>
  -->

* Resource Grid

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Team Builder</li>
  -->

* Team Builder

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Portfolio Optimizer</li>
  -->

* Portfolio Optimizer
* Referenced Object Type selection for a Typeahead field in a Custom Form
* Outlook Add-in

## Implications of customizing object names

You should be aware of the following when customizing object names in *Workfront*:

<ul> 
 <li>You may encounter stylistic or grammatical errors in system displays. For example, if you rename 'Issue' to 'Request' and you see anywhere in the system the phrase 'An request', this is functioning as intended and should not be considered a bug.</li> 
 <li>Your custom names for the objects are not translatable. Only the <em>Workfront</em> default names can be translated in the supported languages. For more information about languages that are supported in <em>Workfront</em>, see <a href="../../../workfront-basics/supported-languages-in-workfront.md" class="MCXref xref">Supported languages in Adobe Workfront</a>. The custom object name fields support foreign characters so you can input terminology in any language.</li> 
 <li>When you customize object names using a Layout Template, we recommend that you assign your Layout Templates around your business units (Teams or Groups).<br>We recommend that you use names that are clearly understood by the users of these business units, to avoid confusion.</li> 
 <li> <p>Email notifications and delivered reports always contain object names as defined by the Layout Template of the user who generates the email. Your users should be prepared to see object names in their emails that are not related to their group or team, if they receive email notifications from users in other teams and groups.<br>As a <em>Workfront administrator</em>, advise users to notice the icons associated with each object. The icons remain consistent between various object names and consistent with the default object, as it appears in the database. For a list of all <em>Workfront</em> icons associated with objects, see <a href="#understanding-object-icons" class="MCXref xref">Object icons</a>.</p> <note type="tip">
    For common tasks in your organization, consider creating custom documentation to reflect your terminology.
  </note> </li> 
</ul>

## Object icons

The *Workfront* documentation always refers to the default names of objects. If your objects have had their names customized, you can rely on the icon associated with them to understand which customized object corresponds to which *Workfront* default object.

For more information about which objects can have customized names in *Workfront*, see * [Object names that can be customized using a Layout Template](#objects-that-can-have-customized-names).*

The following is a list of objects and their corresponding icons in *Workfront*.

| `Object`  | `Icon`  | `Customizable object ame`  |
|---|---|---|
| Company | 

<!--
<img src="assets/company-icon-nwe.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/company-icon-nwe.png) 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
,
<img src="assets/nwe-company-icon-54x54.png" style="width: 54;height: 54;">
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ,  <img src="assets/nwe-company-icon-54x54.png" style="width: 54;height: 54;"></MadCap:conditionalText>`  |  |
| Dashboard | 

<!--
<img src="assets/dashboard-icon-nwe.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/dashboard-icon-nwe.png) 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
,
<img src="assets/nwe-dashboards-icon.png">
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ,  <img src="assets/nwe-dashboards-icon.png"></MadCap:conditionalText>`  |  |
| Goal | ![](assets/nwe-goal-icon.png)

|✔ |
| Goal | ![](assets/nwe-goal-icon.png)

|✔ |
| Group | 

<!--
<img src="assets/groups-icon-nwe.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/groups-icon-nwe.png) 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
,
<img src="assets/nwe-group-icon.png">
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ,  <img src="assets/nwe-group-icon.png"></MadCap:conditionalText>`  |  |
| Issue | 

<!--
<img src="assets/issue-icon-nwe.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/issue-icon-nwe.png) 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
,
<img src="assets/nwe-issues-icon.png">
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ,  <img src="assets/nwe-issues-icon.png"></MadCap:conditionalText>`  |✔ |
| Job Role | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png)

|  |
| Plan | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png)

|&nbsp; |
| Plan | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png)

|&nbsp; |
| Portfolio | 

<!--
<img src="assets/portfolio-icon-nwe.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/portfolio-icon-nwe.png) 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
,
<img src="assets/nwe-portfolios-icon.png">
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ,  <img src="assets/nwe-portfolios-icon.png"></MadCap:conditionalText>`  |✔ |
| Program | 

<!--
<img src="assets/program-icon-nwe.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/program-icon-nwe.png) 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
,
<img src="assets/nwe-programs-icon.png">
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ,  <img src="assets/nwe-programs-icon.png"></MadCap:conditionalText>`  |✔ |
| Project | 

<!--
<img src="assets/project-icon-nwe.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/project-icon-nwe.png) 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
,
<img src="assets/nwe-projects-icon.png">
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ,  <img src="assets/nwe-projects-icon.png"></MadCap:conditionalText>`  |✔ |
| Report | 

<!--
<img src="assets/report-icon-nwe.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/report-icon-nwe.png)

<!--
<span data-mc-conditions="QuicksilverOrClassic.Quicksilver">, <img src="assets/nwe-reports-icon.png"></span>
-->

`, ![](assets/nwe-reports-icon.png)

`  |  |
| Task | 

<!--
<img src="assets/task-icon-new.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/task-icon-new.png) 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
,
<img src="assets/nwe-tasks-icon.png">
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ,  <img src="assets/nwe-tasks-icon.png"></MadCap:conditionalText>`  |✔ |
| Team | 

<!--
<img src="assets/team-icon-nwe.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
,
<img src="assets/nwe-teams-icon.png">
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ,  <img src="assets/nwe-teams-icon.png"></MadCap:conditionalText>` |  |
| Template | 

<!--
<img src="assets/template-icon-nwe.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/template-icon-nwe.png) 

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
,
<img src="assets/nwe-templates-icon.png">
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ,  <img src="assets/nwe-templates-icon.png"></MadCap:conditionalText>`  |  |

## Reference Numbers of objects

Each object created in *Workfront* is assigned a unique reference number. Reference numbers are useful in distinguishing between two otherwise similar objects (such as tasks with the same name). You can search for objects using their reference numbers and you can include reference numbers in reports.

For information about how to search for objects by reference number, see [Use the reference number of objects](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Object-specific searches

You can search across all the objects that are searchable in *Workfront*, or you can select a specific object to search for in your basic and advanced searches.

Not all objects are searchable in *Workfront*. You can run basic and advanced searches for the following objects in *Workfront*:

| `Object`  | `Basic Search`  | `Advanced Search`  |
|---|---|---|
| Projects |✓ | ✓ |
| Tasks |✓ | ✓ |
| Issues |✓ | ✓ |
| Reports |✓ | ✓ |
|  

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
Users
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Users</MadCap:conditionalText>`  |✓ | ✓ |
| Templates |✓ | ✓ |
| Documents |✓ | ✓ |
| Portfolios |✓ | ✓ |
| Programs | ✓ | ✓ |
| Dashboards | ✓ | ✓ |
| Companies | ✓ | ✓ |
| Notes | ✓ |  |

For more information about running basic and advanced searches in *Workfront*, see [Search Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## Report on objects

Understanding the hierarchy and interdependency of objects is extremely important before you start building reports in *Workfront*. Reports are object-specific. You must select the correct object for your report before you can display the data that you want.

Depending on what object you selected for your report, you can access only those objects that are directly linked to the object of the report.

>[!IMPORTANT]
>
>You can report only on the object you select and the parent objects in the same report. You cannot have information about the children objects in a parent object report. For example, you can display project information in a task report, but not task information in a project report.

You can report on all objects in the database using our open API. For a complete list of all objects in the database, see [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>If you have customized the names of your objects using a layout template, the names for the object in the report builder have also been customized. Ensure you know what objects have been customized and look for the customized name in the report builder. For more information about which objects can have customized names in *Workfront*, see * [Object names that can be customized using a Layout Template](#objects-that-can-have-customized-names).* 
>When using text mode in your reports, the names of the objects in text mode expressions are the standard names in *Workfront*, and not the customized object names. For more information about using text mode in reports, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

For more information about building a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).  
For more information about our API, see [API Explorer](../../../wf-api/general/api-explorer.md).

You can report on the following objects when using the report builder in the *Workfront* web application:

<ul> 
 <li>Project</li> 
 <li>Task</li> 
 <li>Hour</li> 
 <li>Issue</li> 
 <li>User</li> 
 <li>Access Level</li> 
 <li>Approval</li> 
 <li>Approval Process</li> 
 <li>Assignment</li> 
 <li>Backlog Work Item<br>Displays tasks or issues on the agile backlog. For more information about the agile backlog, see <a href="../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md" class="MCXref xref">Manage the agile backlog</a>.</li> 
 <li>Baseline</li> 
 <li>Baseline Task</li> 
 <li>Billing Record</li> 
 <li> <p>Budgeted Hour</p> <p>This is the Budgeted Hours, as they appear in the Resource Planner.</p> </li> 
 <li>Calendar Event</li> 
 <li>Category (or Custom Form)</li> 
 <li>Company</li> 
 <li>Dashboard</li> 
 <li>Document</li> 
 <li>Document Approval</li> 
 <li>Document Version<br>Enables you to view various information about the version of the document, the document the version is associated with, who created the version, and the user who created the <em>proof</em> on the document version if one exists (Proof Creator).</li> 
 <li>Email Template</li> 
 <li>Expense</li> 
 <li>Expense Type</li> 
 <li>External Page</li> 
 <li>Favorite</li> 
 <li>Filter</li> 
 <li> <p>Goal </p> <p>You can build a report for strategic goals or you can display goal-related information in a project report when projects are associated with goals as goal activities. You can create strategic goals and connect projects them only if your organization has purchased a <em>Workfront Goals</em> license. For information about <em>Workfront Goals</em>, see <a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&topicId=Content%2FWorkfront_Goals%2FGoal_management%2Fwf-goals-overview.htm&_LANG=en" target="_blank"><em>Workfront Goals</em> overview</a>. For information about connecting projects to strategic goals, see <a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&topicId=Content%2FWorkfront_Goals%2FResults_and_activities%2Fconnect-projects-to-goals-overview.htm&_LANG=en" target="_blank">Overview of connecting projects to goals</a>. </p> <note type="tip">
   You cannot report on project goals that are associated with a Business Case. For information about project goals vs strategic goals, see 
   <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossary of Adobe Workfront terminology</a>. 
  </note> </li> 
 <li>Group</li> 
 <li>Grouping</li> 
 <li>Hour Type</li> 
 <li> <p><span>Initiative</span> </p> <p><span>You can build a report for initiatives which are the children objects of a plan only if your company has purchased a <em>Workfront Scenario Planner</em> license. For information about initiatives, see</span> <a href="https://one.workfront.com/s/csh?context=2066&pubname=the-new-workfront-experience">Initiatives overview in the <em>Workfront Scenario Planner</em></a>.</p> </li> 
 <li> <p><span>Initiative Job Role</span> </p> <p><span>You can build a report for the job roles associated with the initiatives in a plan only if your company has purchased a <em>Workfront Scenario Planner</em> license. For information about creating initiatives and associating them with job roles, see</span> <a href="https://one.workfront.com/s/csh?context=2061&pubname=the-new-workfront-experience">Create and edit initiatives in the <em>Workfront Scenario Planner</em></a>.</p> </li> 
 <li>Iteration</li> 
 <li>Job Role</li> 
 <li> <p>Journal Entry</p> <p>You can report on tracked system updates in the Updates area of objects like tasks, projects, issues, etc. To learn more, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md" class="MCXref xref">Report on the Updates area</a>.</p> </li> 
 <li>Layout Template</li> <draft-comment>
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Legacy Resource Pool</p> <note type="note">
    This report captures information about an area in&nbsp;
    <em>Workfront</em> that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about the current resource pools, see 
    <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview in Adobe Workfront</a>.
   </note> </li>
 </draft-comment>
 <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Legacy Resource Pool</p> <note type="note">
   This report captures information about an area in&nbsp;
   <em>Workfront</em> that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about the current resource pools, see 
   <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview in Adobe Workfront</a>.
  </note> </li> 
 <li>Milestone</li> 
 <li>Milestone Path</li> 
 <li>Note<br><note type="note">
    You can report on comments added by individual users.
  </note></li> 
 <li>Parameter (or Custom Field)</li> 
 <li>Parameter Group (or Section Break)</li> 
 <li>Portal Profile</li> 
 <li>Portfolio</li> 
 <li>Program</li> 
 <li> <p>Project (Financial Data)</p> <note type="note">
   Financial information populates in Project (Financial&nbsp;Data) reports only when the data associated with it is less than 5 years old. For example, if a job role was allocated to a task in January 2015 and today is September 2021, a financial filed like the Allocation Date for the job role does not populate in the Project (Financial&nbsp;Data) report. 
  </note> </li> 
 <li>Proof Approval<br>Enables you to view various information about the <em>proof</em> approval, including: the <em>proof</em> that was submitted for approval, information about the Approver, information about the Requester (if the Requester is a licensed <em>Workfront</em> user), version information, the <em>proof</em> ID, and the <em>proof</em> creation date.<br>Proof Approval reports include only <em>proofs</em> that are available in users' My Work areas where decisions have not yet been made.<br>Proof approvals are assigned in <em>Workfront</em> as described <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add" class="MCXref xref">Add users to a proof</a> in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md" class="MCXref xref">Share a proof within Adobe Workfront</a>.</li> 
 <li>Queue</li> 
 <li>Queue Topic</li> 
 <li>Rate</li> 
 <li>Reminder Notification</li> 
 <li>Report</li> <draft-comment>
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Resource Estimate</p> <note type="note">
    This report captures information about an area in&nbsp;
    <em>Workfront</em> that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see 
    <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.
   </note> </li>
 </draft-comment>
 <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Resource Estimate</p> <note type="note">
   This report captures information about an area in&nbsp;
   <em>Workfront</em> that has been removed. The report might display legacy information but it does not update with current data. Although not recommended, you may update the information in this report using the API. For information about how you estimate resources for projects, see 
   <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Resource Planner overview</a>.
  </note> </li> 
 <li>Resource Pool</li> 
 <li>Risk</li> 
 <li>Risk Type</li> 
 <li>Schedule</li> 
 <li>Scorecard</li> 
 <li>Team</li> 
 <li>Template</li> 
 <li>Template Task</li> 
 <li> <p>Time Off</p> <p>You can report on a user's time off as indicated by the user in their profile.</p> </li> 
 <li>Timesheet</li> 
 <li>Timesheet Profile</li> 
 <li>Topic Group</li> 
 <li>User Delegation<br>You can report on users who have been delegated to perform others' tasks and issues while they are out of the office. This report displays the user who is out of the office as well as the user who fulfills their duties while they are out. </li> 
 <li>View</li> 
 <li>Work Item</li> 
</ul>

