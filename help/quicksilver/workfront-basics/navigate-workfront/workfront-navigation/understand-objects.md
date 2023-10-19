---
content-type: overview;reference
navigation-topic: workfront-navigation
title: Understand objects in [!DNL Adobe Workfront]
description: Understand objects in [!DNL Adobe Workfront]
feature: Get Started with Workfront
exl-id: f324f198-5472-4cf2-a46e-7fc24605ca90
---
# Understand objects in [!DNL Adobe Workfront]

<!--
<***Linked to several articles, do not remove/ change. 
-->

The information you display in [!DNL Adobe Workfront] is represented by objects which are stored in the [!DNL Workfront] database. The objects are what drives the information in [!DNL Workfront].

Understanding how the objects are defined in [!DNL Workfront] is important so you can use the correct object for the needs necessary in your organization.

For example, when you plan a large amount of work, you need to use the [!UICONTROL Project] object to define that work. To divide this work into smaller planned increments, you can use the [!UICONTROL Task] object. For a smaller amount of work that is not planned, and can occur unexpectedly, you can use the Issue object. If you want to track the progress and the adherence to budget and timeline of a group of projects, you can organize them in [!UICONTROL Portfolios] and [!UICONTROL Programs]. To define other elements that help you resolve your work, you want to use other objects that are stored under [!UICONTROL Projects], [!UICONTROL Tasks], [!UICONTROL Issues], or [!UICONTROL Portfolios], like [!UICONTROL Documents], [!UICONTROL Updates], [!UICONTROL Hours], [!UICONTROL Users], or [!UICONTROL Job Roles].

[!UICONTROL Reports] and [!UICONTROL Dashboards] are another example of objects that can help you organize the amount of data you have in [!DNL Workfront] visually, to make it easily accessible for all users.

For a complete list of objects in [!DNL Workfront], see the [API Explorer](../../../wf-api/general/api-explorer.md).

## Interdependency and hierarchy of objects

Objects are linked to one another in [!UICONTROL Workfront]. For example, a task or an issue can never exist independently outside of a project. [!UICONTROL Tasks] and [!UICONTROL issues] are examples of objects that are stored in the [!UICONTROL project] object. [!UICONTROL Tasks] and [!UICONTROL issues] are considered child objects to projects.

The following are some of the most commonly used objects in [!DNL Workfront] and their respective parent and children objects:

| **Object** | **Parent objects** | **Child objects** |
|---|---|---|
| [!UICONTROL Portfolios] |  | [!UICONTROL Programs], [!UICONTROL Projects], [!UICONTROL Documents], [!DNL Notes], [!UICONTROL Users] |
| [!UICONTROL Programs] | [!UICONTROL Portfolios] | [!UICONTROL Projects], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Users] |
| [!UICONTROL Projects] | [!UICONTROL Portfolios], [!UICONTROL Programs] | [!UICONTROL Tasks], [!UICONTROL Issues], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Hours], [!UICONTROL Users] |
| [!UICONTROL Tasks] | [!UICONTROL Projects] | [!UICONTROL Issues], [!UICONTROL Children Tasks], [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Hours], [!UICONTROL Users] |
| [!UICONTROL Issues] | [!UICONTROL Tasks], [!UICONTROL Projects] | [!UICONTROL Documents], [!UICONTROL Notes], [!UICONTROL Hours], [!UICONTROL Users] |
| [!UICONTROL Dashboards] |  | [!UICONTROL Reports], External Pages |
| [!UICONTROL Reports] | [!UICONTROL Dashboards] |  |
| [!UICONTROL Groups] |  | [!UICONTROL Users] |
| [!UICONTROL Teams] |  | [!UICONTROL Users] |
| [!UICONTROL Users] | [!UICONTROL Groups], [!UICONTROL Teams], [!UICONTROL Companies] | [!UICONTROL Job Roles] |
| [!UICONTROL Companies] |  | [!UICONTROL Users] |
| [!UICONTROL Documents] | [!UICONTROL Tasks], [!UICONTROL Issues], [!UICONTROL Projects], [!UICONTROL Portfolios], [!UICONTROL Programs], [!UICONTROL Users] |  |
| [!UICONTROL Plans]* |  | [!UICONTROL Initiatives] |
| [!DNL Goals]* |  | [!UICONTROL Results], [!UICONTROL Activities] |

For a complete list of objects in [!DNL Workfront], see the [API Explorer](../../../wf-api/general/api-explorer.md).

*Plans are the objects of the [!DNL Adobe Workfront Scenario Planner]. For information about the [!DNL Scenario Planner], see [The [!UICONTROL Scenario Planner] overview](../../../scenario-planner/scenario-planner-overview.md).

*[!UICONTROL Goals] are the objects of [!DNL Adobe Workfront Goals]. For information about [!DNL Workfront Goals], see [[!DNL Adobe Workfront Goals] overview](../../../workfront-goals/goal-management/wf-goals-overview.md).


## Customize object names

As a [!DNL Workfront] administrator, you can customize object names in [!DNL Workfront] by using a  [!UICONTROL Layout Template].

For more information about how to customize object names using a  [!UICONTROL Layout Template], see [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

After you customize a layout template and you assign it to users, those users see the customized names for the objects. The users that have been assigned to the layout template no longer see the default names for the objects anywhere in the web application.

>[!NOTE]
>
>For the new names of the objects to be visible for your users, they must log out and log back in to [!DNL Workfront] after you have saved the  [!UICONTROL Layout Template].

>[!IMPORTANT]
>
>The [!DNL Workfront] documentation always refers to the default names of the objects. As a [!DNL Workfront] administrator, ensure that you notify users of the changes in object names, so they can understand how to use the [!DNL Workfront] documentation, as well as the areas of the applications which do not reflect the changes in the names of the objects.

* [Object names that can be customized using a  [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template)
* [Areas of [!DNL Workfront] that reflect the customized object names](#areas-of-workfront-that-reflect-the-customized-object-names)
* [Areas of [!DNL Workfront] that do not reflect the customized object names](#areas-of-workfront-that-do-not-reflect-the-customized-object-names)

### Object names that can be customized using a [!UICONTROL Layout Template]

As a [!DNL Workfront] administrator, you can customize the names of the following objects to match the terminology in your organization:

* [!UICONTROL Portfolio]
* [!UICONTROL Program]
* [!UICONTROL Project]
* [!UICONTROL Task]
* [!UICONTROL Issue]
* [!UICONTROL Goal]*
* [!UICONTROL Result]*
* [!UICONTROL Activity]*

   *[!UICONTROL Goals], [!UICONTROL results], and [!UICONTROL activities] are only available if your company purchased [!DNL Workfront Goals]. For information about [!DNL Workfront Goals], see [[!DNL Adobe Workfront Goals] overview](../../../workfront-goals/goal-management/wf-goals-overview.md).

* [!UICONTROL Initiative]**
* [!UICONTROL Scenario]**
* [!UICONTROL Plan]**

   **[!UICONTROL Initiatives], [!UICONTROL scenarios], and [!UICONTROL plans] are available only if your company purchased the [!DNL Workfront Scenario Planner]. For information about the [!DNL Scenario Planner], see [Get started with the [!DNL Scenario Planner]](../../../scenario-planner/get-started-with-scenario-planning.md).


For example, if the larger amount of work in your organization is known as a 'Engagement', you can replace the name '[!UICONTROL Project]' with 'Engagement'. Your [!DNL Workfront] interface shows 'Engagement' instead of '[!UICONTROL Project]' everywhere where the name '[!UICONTROL Project]' would appear.

For more information about how you can customize object names using  [!UICONTROL Layout Templates], see [Create and manage layout templates](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

You cannot customize the names of any other object in Workfront. For a complete list of objects in [!DNL Workfront], see the [API Explorer](../../../wf-api/general/api-explorer.md).

When you customize the name of an object, the new name for that object appears in most areas of the [!DNL Workfront] application where that object name would appear.

### Areas of [!DNL Workfront] that reflect the customized object names 

The following areas show the updated name of the objects:

* Top Navigation
* All  sections in the left panel navigation
* All menus
* In-app notifications
* Report builder and reporting elements (views, filters, and groupings)
* [!UICONTROL Save] buttons
* Exported files
* Emails
* Mobile Apps

### Areas of [!DNL Workfront] that do not reflect the customized object names 

The following areas do not show the updated name of the objects:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Referenced Object Type selection for a Typeahead field in a Custom Form </p> <p>(NOTE: drafting this because I don't think this is true)</p> </li>
  -->

* [!DNL Outlook] Add-in

### Implications of customizing object names

You should be aware of the following when customizing object names in [!DNL Workfront]:

* You may encounter stylistic or grammatical errors in system displays. For example, if you rename '[!UICONTROL Issue]' to 'Request' and you see anywhere in the system the phrase 'An request', this is functioning as intended and should not be considered a bug.
* Your custom names for the objects are not translatable. Only the [!DNL Workfront] default names can be translated in the supported languages. For more information about languages that are supported in [!DNL Workfront], see [Supported languages in [!DNL Adobe Workfront]](../../../workfront-basics/supported-languages-in-workfront.md). The custom object name fields support foreign characters so you can input terminology in any language.
* When you customize object names using a  [!UICONTROL Layout Template], we recommend that you assign your  [!UICONTROL Layout Templates] around your business units (Teams or Groups).\
   We recommend that you use names that are clearly understood by the users of these business units, to avoid confusion.
* Email notifications and delivered reports always contain object names as defined by the  [!UICONTROL Layout Template] of the user who generates the email. Your users should be prepared to see object names in their emails that are not related to their group or team, if they receive email notifications from users in other teams and groups.\
   As a [!DNL Workfront] administrator, advise users to notice the icons associated with each object. The icons remain consistent between various object names and consistent with the default object, as it appears in the database. For a list of all [!DNL Workfront] icons associated with objects, see [Object icons](#object-icons).

   >[!TIP]
   >
   >For common tasks in your organization, consider creating custom documentation to reflect your terminology.

## Object icons 

The [!DNL Workfront] documentation always refers to the default names of objects. If your objects have had their names customized, you can rely on the icon associated with them to understand which customized object corresponds to which [!DNL Workfront] default object.

For more information about which objects can have customized names in [!DNL Workfront], see [Object names that can be customized using a  [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template).

The following is a list of objects and their corresponding icons in Workfront.

| **Object** | **Icon** | **Customizable object name** |
|---|---|---|
| [!UICONTROL Company] | ![](assets/company-icon-nwe.png)  , ![](assets/nwe-company-icon-54x54.png) |  |
| [!UICONTROL Dashboard] | ![](assets/dashboard-icon-nwe.png)  , ![](assets/nwe-dashboards-icon.png) |  |
| [!UICONTROL Goal] | ![](assets/nwe-goal-icon.png) | ✔ |
| [!UICONTROL Group] | ![](assets/groups-icon-nwe.png)  , ![](assets/nwe-group-icon.png) |  |
| [!UICONTROL Issue] | ![](assets/issue-icon-nwe.png)  , ![](assets/nwe-issues-icon.png) | ✔ |
| [!UICONTROL Job Role] | ![job_role_icon.png](assets/job-role-icon-52x50.png), ![job_role_icon__1_.png](assets/job-role-icon--1--53x44.png), ![](assets/job-role-nwe-no-color.png), ![](assets/job-role-icon-nwe-color.png) |  |
| [!UICONTROL Plan] | ![](assets/plan-icon.png), ![](assets/nwe-plan-icon-60x57.png) |  |
| [!UICONTROL Portfolio] | ![](assets/portfolio-icon-nwe.png)  , ![](assets/nwe-portfolios-icon.png) | ✔ |
| [!UICONTROL Program] | ![](assets/program-icon-nwe.png)  , ![](assets/nwe-programs-icon.png) | ✔ |
| [!UICONTROL Project] | ![](assets/project-icon-nwe.png)  , ![](assets/nwe-projects-icon.png) | ✔ |
| [!UICONTROL Report] | ![](assets/report-icon-nwe.png) , ![](assets/nwe-reports-icon.png) |  |
| [!UICONTROL Task] | ![](assets/task-icon-new.png)  , ![](assets/nwe-tasks-icon.png) | ✔ |
| [!UICONTROL Team] | ![](assets/team-icon-nwe.png), ![](assets/team-icon-nwe-color.png) , ![](assets/nwe-teams-icon.png) |  |
| [!UICONTROL Template] | ![](assets/template-icon-nwe.png)  , ![](assets/nwe-templates-icon.png) |  |

## Reference Numbers of objects

Each object created in [!DNL Workfront] is assigned a unique reference number. Reference numbers are useful in distinguishing between two otherwise similar objects (such as tasks with the same name). You can search for objects using their reference numbers and you can include reference numbers in reports.

For information about how to search for objects by reference number, see [Use the reference number of objects](../../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md).

## Object-specific searches

You can search across all the objects that are searchable in [!DNL Workfront], or you can select a specific object to search for in your basic and advanced searches.

Not all objects are searchable in [!DNL Workfront]. You can run basic and advanced searches for the following objects in [!DNL Workfront]:

| **Object** | **Basic Search** | **Advanced Search** |
|---|---|---|
| [!UICONTROL Projects] | ✓ | ✓ |
| [!UICONTROL Tasks] | ✓ | ✓ |
| [!UICONTROL Issues] | ✓ | ✓ |
| [!UICONTROL Reports] | ✓ | ✓ |
| [!UICONTROL Users] | ✓ | ✓ |
| [!UICONTROL Templates] | ✓ | ✓ |
| [!UICONTROL Documents] | ✓ | ✓ |
| [!UICONTROL Portfolios] | ✓ | ✓ |
| [!UICONTROL Programs] | ✓ | ✓ |
| [!UICONTROL Dashboards] | ✓ | ✓ |
| [!UICONTROL Companies] | ✓ | ✓ |
| [!UICONTROL Notes] (or [!UICONTROL Updates]) | ✓ |  |

For more information about running basic and advanced searches in [!DNL Workfront], see [Search [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

## Report on objects

Understanding the hierarchy and interdependency of objects is extremely important before you start building reports in [!DNL Workfront]. Reports are object-specific. You must select the correct object for your report before you can display the data that you want.

Depending on what object you selected for your report, you can access only those objects that are directly linked to the object of the report.

>[!IMPORTANT]
>
>You can report only on the object you select and the parent objects in the same report. You cannot have information about the children objects in a parent object report. For example, you can display project information in a task report, but not task information in a project report.

You can report on all objects in the database using our open API. For a complete list of all objects in the database, see [API Explorer](../../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>If you have customized the names of your objects using a layout template, the names for the object in the report builder have also been customized. Ensure you know what objects have been customized and look for the customized name in the report builder. For more information about which objects can have customized names in [!DNL Workfront], see *[Object names that can be customized using a  [!UICONTROL Layout Template]](#object-names-that-can-be-customized-using-a-layout-template).*
>When using text mode in your reports, the names of the objects in text mode expressions are the standard names in [!DNL Workfront], and not the customized object names. For more information about using text mode in reports, see [Text Mode overview](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

For more information about building a report, see [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).\
For more information about our API, see [API Explorer](../../../wf-api/general/api-explorer.md).

You can report on the following objects when using the report builder in the [!DNL Workfront] web application:

* [!UICONTROL Project]
* [!UICONTROL Task]
* [!UICONTROL Hour]
* [!UICONTROL Issue]
* [!UICONTROL User]
* [!UICONTROL Access] Level
* [!UICONTROL Approval]
* [!UICONTROL Approval Process]
* [!UICONTROL Assignment]
<!--this is no longer available: * [!UICONTROL Backlog Work Item]\
   Displays tasks or issues on the agile backlog. For more information about the agile backlog, see [Manage the agile backlog](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).-->

* [!UICONTROL Baseline]
* [!UICONTROL Baseline Task]
* [!UICONTROL Billing Record]
* [!UICONTROL Budgeted Hour]

   This is the [!UICONTROL Budgeted Hours], as they appear in the in older, deprecated resource management tools.

   The "Bud. Hours" field in the [!UICONTROL Budgeted Hour] report refers to the hours budgeted for job roles in the [!UICONTROL Resource Planner]. For more information, see [Understand [!UICONTROL Budgeted Labor Cost] and [!UICONTROL Budgeted Hours] for projects](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* [!UICONTROL Calendar Event]
* [!UICONTROL Company]
* [!UICONTROL Custom Form]
* [!UICONTROL Dashboard]
* [!UICONTROL Document]
* [!UICONTROL Document Approval]
* [!UICONTROL Document Version]\
   You can view information about the version of the document, the document the version is associated with, who created the version, and the user who created the proof on the document version if one exists (Proof Creator).
* [!UICONTROL Email Template]
* [!UICONTROL Expense]
* [!UICONTROL Expense Type]
* [!UICONTROL External Page]
* [!UICONTROL Favorite]
* [!UICONTROL Filter]
* [!UICONTROL Goal]

   You can build a report for strategic goals or you can display goal-related information in a project report when projects are associated with goals as goal activities. You can create strategic goals and connect projects them only if your organization has purchased a [!DNL Workfront Goals] license. For information about [!DNL Workfront Goals], see [[!DNL Workfront Goals] overview](../../../workfront-goals/goal-management/wf-goals-overview.md). For information about connecting projects to strategic goals, see [Add projects to goals in Adobe Workfront Goals](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).
   
   >[!TIP]
   >
   >You cannot report on project goals that are associated with a [!UICONTROL Business Case]. For information about project goals vs strategic goals, see [Glossary of [!DNL Adobe Workfront] terminology](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* [!UICONTROL Group]
* [!UICONTROL Grouping]
* [!UICONTROL Hour Type]
* [!UICONTROL Initiative]

   You can build a report for initiatives which are the children objects of a plan only if your company has purchased a [!DNL Workfront Scenario Planner] license. For information about initiatives, see [Initiatives overview in the [!DNL Workfront Scenario Planner]](../../../scenario-planner/initiatives-overview.md).
   
 
* Initiative Job Role

   You can build a report for the job roles associated with the initiatives in a plan only if your company has purchased a [!DNL Workfront Scenario Planner] license. For information about creating initiatives and associating them with job roles, see [Create and edit initiatives in the [!DNL Workfront Scenario Planner]](../../../scenario-planner/create-and-edit-initiatives.md).


* [!UICONTROL Iteration]
* [!UICONTROL Job Role]
* [!UICONTROL Journal Entry]

   You can report on tracked system updates in the [!UICONTROL Updates] area of objects like tasks, projects, issues, etc. To learn more, see [Report on the [!UICONTROL Updates] area](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

* [!UICONTROL Layout Template]
* [!UICONTROL Milestone]
* [!UICONTROL Milestone Path]
* [!UICONTROL Note] or [!UICONTROL Updates]

   >[!NOTE]
   >
   >You can report on comments added by individual users.

* [!UICONTROL Parameter] (or [!UICONTROL Custom Field])
* [!UICONTROL Parameter Group] (or [!UICONTROL Section Break])
<!--this is no longer in the UI: * [!UICONTROL Portal Profile] (this displays information that has been deprecated)-->
* [!UICONTROL Portfolio]
* [!UICONTROL Program]
* [!UICONTROL Project] ([!UICONTROL Financial Data])

   >[!NOTE]
   >
   >Financial information populates in [!UICONTROL Project] ([!UICONTROL Financial Data]) reports only when the data associated with it is less than 5 years old. For example, if a job role was allocated to a task in January 2015 and today is September 2021, a financial filed like the [!UICONTROL Allocation Date] for the job role does not populate in the [!UICONTROL Project (Financial Data)] report.

* [!UICONTROL Proof Approval]\
   Enables you to view various information about the proof approval, including: the proof that was submitted for approval, information about the [!UICONTROL Approver], information about the Requester (if the Requester is a licensed [!DNL Workfront] user), version information, the proof ID, and the proof creation date.\
   [!UICONTROL Proof Approval] reports include only proofs that are available in users' My Work areas where decisions have not yet been made.\
   Proof approvals are assigned in [!DNL Workfront] as described [Add users to a proof](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Share a proof within [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* [!UICONTROL Queue]
* [!UICONTROL Queue Topic]
* [!UICONTROL Rate] (this displays job role [!UICONTROL Billing Rate] information)
* [!UICONTROL Reminder Notification]
* [!UICONTROL Report]
* [!UICONTROL Resource Pool]
* [!UICONTROL Risk]
* [!UICONTROL Risk Type]
* [!UICONTROL Schedule]
* [!UICONTROL Scorecard]
* [!UICONTROL Team]
* [!UICONTROL Template]
* [!UICONTROL Template Task]
* [!UICONTROL Time Off]

   You can report on a user's time off as indicated by the user in their profile.

* [!UICONTROL Timesheet]
* [!UICONTROL Timesheet Profile]
* [!UICONTROL Topic Group]
* [!UICONTROL User Approval]
* [!UICONTROL User Delegation]

   You can report on users who have been delegated to perform others' tasks and issues while they are out of the office. This report displays the user who is out of the office as well as the user who fulfills their duties while they are out.
* [!UICONTROL Users Decisions]
* [!UICONTROL View]
* [!UICONTROL Work Item] (this produces a report for tasks and issues)
