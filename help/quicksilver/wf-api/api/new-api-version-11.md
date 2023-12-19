---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 11
description: ReportableBudgedHour has been added to the Adobe Workfront API as a resource for Reporting. It features reference fields, core fields, and default fields that are absent in BudgetedHour.
author: Becky
feature: Workfront API
role: Developer
exl-id: b8826dc6-9791-49f6-923d-5a0c5392a8b0
---
# What's new in API version 11

* [Added Resources](#added-resources) 
* [Removed Resources](#removed-resources) 
* [Modified Resources](#modified-resources)

## Added Resources {#added-resources}

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasaccessrule" class="MCXref xref">LoginAsAccessRule</a> </li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginasadditionalrule" class="MCXref xref">LoginAsAdditionalRule</a> </li>
  -->

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#loginassettings" class="MCXref xref">LoginAsSettings</a> </li>
  -->

* [ReportableBudgetedHour](#reportablebudgetedhour)

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasaccessrule">LoginAsAccessRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessExpirationDate</li> 
     <li style="font-weight: bold;">accessorID</li> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">userID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">accessor</li> 
     <li style="font-weight: bold;">customer</li> 
     <li style="font-weight: bold;">user &nbsp;</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Core Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginasadditionalrule">LoginAsAdditionalRule</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">loginAsSettingsID</li> 
     <li style="font-weight: bold;">objID</li> 
     <li style="font-weight: bold;">objObjCode &nbsp;</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customer &nbsp;</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Core Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="loginassettings">LoginAsSettings</h3>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customerID</li> 
     <li style="font-weight: bold;">licenseTypes</li> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">restrictedLoginAs &nbsp;</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">customer &nbsp;</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collection Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">additionalRules</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Core Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ReportableBudgetedHour {#reportablebudgetedhour}

ReportableBudgedHour has been added to the Adobe Workfront API as a resource for Reporting. It features reference fields, core fields, and default fields that are absent in BudgetedHour. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">allocationDate </p> <p>The Allocation Date is the first day (a Sunday) of the week for which you budgeted the hours in the Resource Planner.</p> </li> 
     <li> <p style="font-weight: bold;">budgetedHours </p> <p>Budgeted Hours are hours that the resource manager budgets for the work that resources need to complete on projects</p> </li> 
     <li> <p style="font-weight: bold;">ID </p> <p>The unique Workfront ID assigned to a specific Reportable Budgeted Hour object.</p> </li> 
     <li style="font-weight: bold;">plannedBudgetedHours </li> 
     <li> <p style="font-weight: bold;">projectID </p> <p>The unique Workfront ID assigned to a specific Project.</p> </li> 
     <li> <p style="font-weight: bold;">roleID</p> <p>The unique Workfront ID assigned to a specific Job Role.</p> </li> 
     <li> <p style="font-weight: bold;">userID</p> <p>The unique Workfront ID assigned to a specific User.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">project</p> <p>The Project that a ReportableBudgetedHour is associated with.</p> </li> 
     <li> <p style="font-weight: bold;">role</p> <p>The Job Role that a ReportableBudgetedHour is associated with.</p> </li> 
     <li> <p style="font-weight: bold;">user</p> <p>The User that a ReportableBudgetedHour is associated with.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Core Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">ID</li> 
     <li style="font-weight: bold;">name</li> 
     <li style="font-weight: bold;">objCode</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Default Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">name</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Operations</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">COUNT</li> 
     <li style="font-weight: bold;">GET</li> 
     <li style="font-weight: bold;">REPORT </li> 
     <li style="font-weight: bold;">SEARCH</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Removed Resources {#removed-resources}

No resources were removed for API v11.

## Modified Resources {#modified-resources}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </li> 
     <li><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </li> 
     <li><a href="#accessrule" class="MCXref xref">AccessRule</a> </li> 
     <li><a href="#approval" class="MCXref xref">Approval</a> </li> 
     <li><a href="#approvalpath" class="MCXref xref">ApprovalPath</a> </li> 
     <li><a href="#approvalprocess" class="MCXref xref">ApprovalProcess</a> </li> 
     <li><a href="#assignment" class="MCXref xref">Assignment</a> </li> 
     <li><a href="#baselinetask" class="MCXref xref">BaselineTask</a> </li> 
     <li><a href="#category" class="MCXref xref">Category</a> </li> 
     <li><a href="#company" class="MCXref xref">Company</a> </li> 
     <li><a href="#customenum" class="MCXref xref">CustomEnum</a> </li> 
     <li><a href="#customer" class="MCXref xref">Customer</a> </li> 
     <li><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#docmetadatalinkgroup" class="MCXref xref">DocMetadataLinkGroup</a> </li> 
     <li><a href="#document" class="MCXref xref">Document</a> </li> 
     <li><a href="#iteration" class="MCXref xref">Iteration</a> </li> 
     <li><a href="#layout-template" class="MCXref xref">Layout Template</a> </li> 
     <li><a href="#milestonepath" class="MCXref xref">MilestonePath</a> </li> 
     <li><a href="#note" class="MCXref xref">Note</a> </li> 
     <li><a href="#optask" class="MCXref xref">OpTask</a> </li> 
     <li><a href="#parameter" class="MCXref xref">Parameter</a> </li> 
     <li><a href="#portfolio" class="MCXref xref">Portfolio</a> </li> 
     <li><a href="#program" class="MCXref xref">Program</a> </li> 
     <li><a href="#project" class="MCXref xref">Project</a> </li> 
     <li><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </li> 
     <li><a href="#queuedef" class="MCXref xref">QueueDef</a> </li> 
     <li><a href="#reservedtime" class="MCXref xref">ReservedTime</a> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li><a href="#resourceplannerfilter" class="MCXref xref">ResourcePlannerFilter</a> </li> 
     <li><a href="#risk" class="MCXref xref">Risk</a> </li> 
     <li><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </li> 
     <li><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </li> 
     <li><a href="#task" class="MCXref xref">Task</a> </li> 
     <li><a href="#team" class="MCXref xref">Team</a> </li> 
     <li><a href="#template" class="MCXref xref">Template</a> </li> 
     <li><a href="#templateassignment" class="MCXref xref">TemplateAssignment</a> </li> 
     <li><a href="#templatetask" class="MCXref xref">TemplateTask</a> </li> 
     <li><a href="#timesheet" class="MCXref xref">Timesheet</a> </li> 
     <li><a href="#update" class="MCXref xref">Update</a> </li> <!--
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#user" class="MCXref xref">User</a> </li>
     --> 
     <li><a href="#usernote" class="MCXref xref">UserNote</a> </li> 
     <li><a href="#work" class="MCXref xref">Work </a> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

### AccessLevelPermissions {#accesslevelpermissions}

An AccessLevelPermissions object represents a set of permissions. This set of permissions can then be associated with an Access Level.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> <p>The following fields added the possible value BUDGETING_INFORMATION. This allows users with permission to edit priorities and budget hours in the planner.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions &nbsp;</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRequest {#accessrequest}

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: bold;">action</p> <p>Added the possible value BUDGETING_INFORMATION. This allows users with permission to edit priorities and budget hours in the planner. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessRule {#accessrule}

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> <p>The following fields added the possible value BUDGETING_INFORMATION. This allows users with permission to edit priorities and budget hours in the planner.</p> 
    <ul> 
     <li style="font-weight: bold;">coreAction</li> 
     <li style="font-weight: bold;">forbiddenActions</li> 
     <li style="font-weight: bold;">secondaryActions &nbsp;</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Approval {#approval}

A given work item, such as a task, document, or timesheet, may require that a supervisor or other user sign off on the work item. An Approval object represents the action of signing off on a work item.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direct Fields<p style="font-weight: normal;">The following fields added the validators AT_DATE_BEFORE_YEAR and AT_DATE_AFTER_YEAR. These validators specify that dates on associated objects can't be set before the year 1900 or after 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">The following fields were added to the public API for transparency in calculating EAC (Estimate at Completion).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Also known as the Earned Value, the Budgeted Cost of Work Performed (BCWP) is a project performance metric that represents the budgeted cost of the amount of the task that has actually completed at the time when this metric is calculated. For tasks, BCWP = Actual Percent Complete x Task Budget. For Projects, BCWP = SUM(BCWP values of all parent and individual tasks).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Also known as the Planned Value, the Budgeted Cost of Work Scheduled (BCWS) is a project performance metric that represents the budgeted cost of the amount of the task that should have completed at the time when this metric is calculated. For tasks, BCWS = Planned Percent Complete x Task Budget. For projects, BCWS = SUM(BCWS values of all parent and individual tasks).</p></li>
    </ul><p style="font-weight: normal;">The following fields added the possible value ET. This value represents the unit of time Elapsed Months, which refers to months without regard to weekends or holidays.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">The following fields added the flag CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">The following fields were removed from the Approval object.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul><p style="font-weight: normal;">The following field was added to the Approval object.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Removed from the Approval object &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collection Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Added to the Approval object.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalPath {#approvalpath}

An ApprovalPath object is a branch within an Approval Process. Approval Paths are based on the status of the object that the Approval Process is associated with.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Added the possible value ET. This value represents the unit of time Elapsed Months, which refers to months without regard to weekends or holidays. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ApprovalProcess {#approvalprocess}

An ApprovalProcess object is a multi-step Approval that can be associated with a Project, Task, or Issue.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">This field was added, and is a boolean parameter that has a value of true if an object is active and false if it is not. Objects that are set to Active appear in drop-down menus and type-ahead fields and can be attached to other objects. Objects not set to Active are not visible in drop-down menus and type-ahead fields to attach to other objects. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Default Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Assignment {#assignment}

An assignment object represents the connection between a work item and the user, team, or group that is assigned to work on it.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit </p> <p style="font-weight: normal;">Added the possible value ET. This value represents the unit of time Elapsed Months, which refers to months without regard to weekends or holidays. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BaselineTask {#baselinetask}

Baselines are snapshots of what the performance of a project looked like at a given moment in time. They store key pieces of information about the project, like key dates, progress, cost and revenue values. When you create a baseline, the task information is also captured on the baseline tasks of that baseline.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>durationUnit </p> <p style="font-weight: normal;">Added the possible value ET. This value represents the unit of time Elapsed Months, which refers to months without regard to weekends or holidays. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Category {#category}

A Category object is a custom form. You can build reports for this object and you can show it in other object reports, as well.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">This field was added, and is a boolean parameter that has a value of true if an object is active and false if it is not. Objects that are set to Active appear in drop-down menus and type-ahead fields and can be attached to other objects. Objects not set to Active are not visible in drop-down menus and type-ahead fields to attach to other objects. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Default Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Company {#company}

A Company object represents an organization consisting of a collection of people. Companies are associated with a user or a project.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">This field was added, and is a boolean parameter that has a value of true if an object is active and false if it is not. Objects that are set to Active appear in drop-down menus and type-ahead fields and can be attached to other objects. Objects not set to Active are not visible in drop-down menus and type-ahead fields to attach to other objects. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Default Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum {#customenum}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A CustomEnum object is an enumeration that is created in Workfront to be used in objects and fields throughout Workfront.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Actions</td> 
   <td> <p style="font-weight: normal;">The following actions were added to the CustomEnum object</p> 
    <ul> 
     <li style="font-weight: bold;">getDefaultOpTaskConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultProjectConditionEnum</li> 
     <li style="font-weight: bold;">getDefaultTaskConditionEnum</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Queries</td> 
   <td> <p>The following queries were added to the CustomEnum object</p> 
    <ul> 
     <li style="font-weight: bold;">opTaskConditions</li> 
     <li style="font-weight: bold;">projectConditions</li> 
     <li style="font-weight: bold;">taskConditions</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Customer {#customer}

A Customer object represents an organization that uses an instance of Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>customEnumTypes</p> <p style="font-weight: normal;">Added possible values: </p> 
      <ul> 
       <li style="font-weight: normal;">CONDITION_PROJ (Project Conditions)</li> 
       <li style="font-weight: normal;">CONDITION_TASK (Task Conditions)</li> 
       <li style="font-weight: normal;">CONDITION_OPTASK (Issue Conditions) &nbsp;</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Reference Fields</td> 
    <td> 
     <ul> 
      <li style="font-weight: bold;"> <p>loginAsSettings</p> <p style="font-weight: normal;">Added. &nbsp;</p> </li> 
     </ul> </td> 
   </tr>
  --> 
  <tr> 
   <td>Actions</td> 
   <td> <p style="font-weight: normal;">The following actions were added to the Customer object</p> 
    <ul> 
     <li style="font-weight: bold;">goalsEnabled</li> 
     <li style="font-weight: bold;">updateLoginAsSettings</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

A CustomerPreferences object represents the set of preferences that a customer has set for their instance of Workfront.

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Added possible values:</p> 
      <ul> 
       <li style="font-weight: normal;">password:password.eauthPolicy (Password Complexity Requirements)</li> 
       <li style="font-weight: normal;"> password:password.minimumLength (Minimum Password Length)</li> 
       <li style="font-weight: normal;">password:mobileSessionTimeout (Mobile Session Time Out)</li> 
       <li style="font-weight: normal;"> project.mgmt:default.project.usertimeoff (User Time Off)</li> 
       <li style="font-weight: normal;">timesheet:default.timesheet.manualrole (Manual control role)</li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientRole (config.proofhq.defaultnonrecipientrole) </li> 
       <li style="font-weight: normal;">proof:defaultNonRecipientGuestRole (config.proofhq.defaultnonrecipientguestrole) &nbsp;</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocMetadataLinkGroup {#docmetadatalinkgroup}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Actions</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>getMetadataDetailsForDocument</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Document {#document}

A Document object represents a file (such as written material, images, or other forms of information).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Actions</td> 
   <td> <p>The following actions were added to the Document object.</p> 
    <ul> 
     <li style="font-weight: bold;">completeLargeDocument</li> 
     <li style="font-weight: bold;">createLargeDocument</li> 
     <li style="font-weight: bold;">createProofRest</li> 
     <li style="font-weight: bold;">getDocumentProofTemplate</li> 
     <li style="font-weight: bold;">getProofRecipients</li> 
     <li style="font-weight: bold;">getProofStages</li> 
     <li style="font-weight: bold;">getProofTemplate</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Iteration {#iteration}

An Iteration object represents a single Agile Iteration. Iterations are discrete periods of time used to plan and complete Agile stories.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> <p>The following fields were added to the Iteration object.</p> 
    <ul> 
     <li style="font-weight: bold;">originalTotalPoints</li> 
     <li style="font-weight: bold;">points Completed</li> 
     <li style="font-weight: bold;">totalPoints &nbsp;</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Layout Template {#layout-template}

A Layout Template object represents a particular arrangement of layout elements, such as the main menu, navigation panel, or the Home area. Layout templates can be assigned to users, teams, groups, or job roles.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps </p> <p style="font-weight: normal;">This field was added, and is a boolean parameter that has a value of true if a Layout Template is set to show timestamps for due dates in the Work List and Calendar, and false if it is set to hide timestamps. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Default Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>showHomeTimestamps</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### MilestonePath {#milestonepath}

A milestone is a marker on a task indication that it is a key point in the Project. Generally used to denote a significant event such as the completion of a phase of the project or a set of critical activities. A MilestonePath object is a collection of milestones.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">This field was added, and is a boolean parameter that has a value of true if an object is active and false if it is not. Objects that are set to Active appear in drop-down menus and type-ahead fields and can be attached to other objects. Objects not set to Active are not visible in drop-down menus and type-ahead fields to attach to other objects. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Default Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Note {#note}

A Note object is a comment or update made on a Workfront object.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> <p>The following fields were added to the Note object.</p> 
    <ul> 
     <li style="font-weight: bold;">proofID &nbsp;</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collection Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>likes</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

An OpTask object is commonly known as an Issue. An issue is a work item that usually indicates that there is a problem preventing the completion of a task or project. An Issue can also be a Help Desk request. Change Orders, Requests, and Bugs are also Issues.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direct Fields<p style="font-weight: normal;">The following fields added the validators AT_DATE_BEFORE_YEAR and AT_DATE_AFTER_YEAR. These valdators specify that dates on associated objects can't be set before the year 1900 or after 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">The following fields were added to OpTask.</p>
    <ul>
     <li style="font-weight: bold;"><p>kanbanBoardID </p><p style="font-weight: normal;">The unique Workfront ID of a Kanban Board object.</p></li>
     <li style="font-weight: bold;"><p>percentComplete</p><p style="font-weight: normal;">Percent Complete is a parameter that will return the completed amount of an issue, as a percentage.</p></li>
     <li style="font-weight: bold;">storyPoints</li>
     <li style="font-weight: bold;">work &nbsp;</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Collection Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Search Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>work</p> <p style="font-weight: normal;">Removed</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Default Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>percentComplete</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actions</td> 
   <td> <p>The following actions were added to the OpTask object</p> 
    <ul> 
     <li style="font-weight: bold;">bulkMove</li> 
     <li style="font-weight: bold;">copyIssue</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parameter {#parameter}

A Parameter object is a custom field.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Added possible value TYAH (Typeahead).</p> </li> 
     <li style="font-weight: bold;"> <p>refObjCode </p> <p style="font-weight: normal;">This field was added and refers to the object code of a referenced object. Object codes for all objects can be found in the <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

A Portfolio object is a collection of projects that compete for the same resources, typically money or people to complete them.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>description</p> <p style="font-weight: normal;">Added the validator MAX_LENGTH, which specifies that the length of the description is no more than 4000 characters.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Program {#program}

A Program object is a subset within a portfolio, where similar projects can be grouped together.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>description</p> <p style="font-weight: normal;">Added the validator MAX_LENGTH, which specifies that the length of the description is no more than 4000 characters.</p> </li> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">This field was added, and is a boolean parameter that has a value of true if an object is active and false if it is not. Objects that are set to Active appear in drop-down menus and type-ahead fields and can be attached to other objects. Objects not set to Active are not visible in drop-down menus and type-ahead fields to attach to other objects. &nbsp;</p> </li> 
     <li style="font-weight: bold;"> <p>name </p> <p style="font-weight: normal;">Added the validator MAX_LENGTH, which specifies that the length of the name is no more than 255 characters. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Default Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Project {#project}

Projects are work items within Workfront, and are a main building block in the way Workfront helps people to do work. A Project object represents a group of tasks with a common, specific goal.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direct Fields<p style="font-weight: normal;">The following fields added the validators AT_DATE_BEFORE_YEAR and AT_DATE_AFTER_YEAR. These valdators specify that dates on associated objects can't be set before the year 1900 or after 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">The following fields were added to the public API for transparency in calculating EAC (Estimate at Completion).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Also known as the Earned Value, the Budgeted Cost of Work Performed (BCWP) is a project performance metric that represents the budgeted cost of the amount of the task that has actually completed at the time when this metric is calculated. For tasks, BCWP = Actual Percent Complete x Task Budget. For Projects, BCWP = SUM(BCWP values of all parent and individual tasks).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Also known as the Planned Value, the Budgeted Cost of Work Scheduled (BCWS) is a project performance metric that represents the budgeted cost of the amount of the task that should have completed at the time when this metric is calculated. For tasks, BCWS = Planned Percent Complete x Task Budget. For projects, BCWS = SUM(BCWS values of all parent and individual tasks).</p></li>
    </ul><p style="font-weight: normal;">The following fields added the flag CURRENCY</p>
    <ul>
     <li style="font-weight: bold;">projectBudgetedCost</li>
     <li style="font-weight: bold;">projectNetValue</li>
    </ul><p style="font-weight: normal;">The following field was removed from the Project object.</p>
    <ul>
     <li style="font-weight: bold;">timelineExceptionInfo</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Collection Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ProofApproval {#proofapproval}

A ProofApproval object represents an approval that is directly connected to a proof.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isAwaitingDecision</p> <p style="font-weight: normal;">This field was added, and is a boolean parameter that has a value of true if a proof is awaiting a decision and false if it is not. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

A QueueDef object represents a Queue, which is a Project that has been published to the Help Desk area to allow users to submit Issues to it.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> <p>The following fields added the possible value BUDGETING_INFORMATION. This allows users with permission to edit priorities and budget hours in the planner.</p> 
    <ul> 
     <li style="font-weight: bold;">requestorCoreAction</li> 
     <li style="font-weight: bold;">requestorForbiddenActions</li> 
    </ul> &nbsp;</td> 
  </tr> 
 </tbody> 
</table>

### ReservedTime {#reservedtime}

A ReservedTime object represents days specified on a User's Personal Time, indicating that the User will not be available for work.

The ReservedTime resource added the flag REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> <p>The following fields removed the flag NOT_GROUPABLE.</p> 
    <ul> 
     <li style="font-weight: bold;">endDate</li> 
     <li style="font-weight: bold;">extRefID</li> 
     <li style="font-weight: bold;">startDate </li> 
    </ul> <p>The following field was removed from the ReservedTime object.</p> 
    <ul> 
     <li style="font-weight: bold;">taskID</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>task</p> <p style="font-weight: normal;">Removed &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Operations</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>EDIT</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ResourcePlannerFilter {#resourceplannerfilter}

A ResourcePlannerFilter object is a set of rules that determine which items will display in the Resource Planner.

The ResourcePlannerFilter resource added the flag SHARABLE. There were no other changes to the object.

### Risk {#risk}

A Risk object represents a possible event that may prevent a project from finishing on time or within budget. Risks are added to projects in the planning phase to identify potential obstacles prior to the approval of any work.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> <p>The following fields were added to the Risk object:</p> 
    <ul> 
     <li style="font-weight: bold;"> <p>enteredByID</p> <p style="font-weight: normal;">The ID of the user that originally created the object.</p> </li> 
     <li> <p style="font-weight: bold;">entryDate</p> <p>The date an object was submitted by a user in Workfront.</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdateDate</p> <p>The Last Update Date parameter will return that Date that the Last Update was made to an object,</p> </li> 
     <li> <p style="font-weight: bold;">lastUpdatedByID </p> <p>Last Updated By ID is a parameter that will return the User ID of the last User that updated the object. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> <p style="font-weight: normal;">The following Reference Fields were added to the RIsk object.</p> 
    <ul> 
     <li style="font-weight: bold;">enteredBy</li> 
     <li style="font-weight: bold;">lastUpdatedBy &nbsp;</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

A ScheduledReport object represents a report that has been configured to be scheduled for delivery.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>pageSize</p> <p style="font-weight: normal;">Added the following possible values:</p> 
      <ul> 
       <li style="font-weight: normal;">A2</li> 
       <li style="font-weight: normal;">A1</li> 
       <li style="font-weight: normal;">A0 &nbsp;</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

A ScoreCardQuestion object represents a question that has been added to a Scorecard. These questions are usually determined by the Portfolio manager, and their answers allow the manager to understand how well a project aligns with the goals of the portfolio.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Added possible value TYAH (Typeahead) &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Task {#task}

A Task object represents a work item that must be performed as a step toward achieving a final goal (completing a Project).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direct Fields<p style="font-weight: normal;">The following fields added the validators AT_DATE_BEFORE_YEAR and AT_DATE_AFTER_YEAR. These valdators specify that dates on associated objects can't be set before the year 1900 or after 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">The following fields were added to the public API for transparency in calculating EAC (Estimate at Completion).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Also known as the Earned Value, the Budgeted Cost of Work Performed (BCWP) is a project performance metric that represents the budgeted cost of the amount of the task that has actually completed at the time when this metric is calculated. For tasks, BCWP = Actual Percent Complete x Task Budget. For Projects, BCWP = SUM(BCWP values of all parent and individual tasks).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Also known as the Planned Value, the Budgeted Cost of Work Scheduled (BCWS) is a project performance metric that represents the budgeted cost of the amount of the task that should have completed at the time when this metric is calculated. For tasks, BCWS = Planned Percent Complete x Task Budget. For projects, BCWS = SUM(BCWS values of all parent and individual tasks).</p></li>
    </ul><p style="font-weight: normal;">The following fields added the possible value ET. This value represents the unit of time Elapsed Months, which refers to months without regard to weekends or holidays.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">The following field was removed from the Task object.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">The following field was added to the Task object.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Removed &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collection Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Team {#team}

A Team object is a collection of Users that can be assigned to a work item.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>agileEstimateType </p> <p style="font-weight: normal;">This field was added to the Team object. Agile Estimate Type determines how the work load of a story is estimated. If estimated in hours, then this is the number of Planned Hours that are added to the story. If estimated in points, each point will add a number of Planned Hours to the story based on how the points are set (default is 8 hours). Possible values for Agile Estimate Type are:</p> 
      <ul> 
       <li style="font-weight: normal;"> STORY_POINTS (Story Points)</li> 
       <li style="font-weight: normal;">HOURS (Hours)</li> 
       <li style="font-weight: normal;">LEGACY_POINTS (Hours as Points) &nbsp;</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Template {#template}

A Template object represents a pattern for a Project. Projects can be created from Templates to save time. A Template contains a Team and Tasks, which will be copied to a Project when the Template is used.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">This field was added, and is a boolean parameter that has a value of true if an object is active and false if it is not. Objects that are set to Active appear in drop-down menus and type-ahead fields and can be attached to other objects. Objects not set to Active are not visible in drop-down menus and type-ahead fields to attach to other objects. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collection Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorities</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Default Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateAssignment {#templateassignment}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A TemplateAssignment object represents the connection between a Template and the User, Team, or Group it is assigned to.</p>
-->

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>workUnit</p> <p style="font-weight: normal;">Added the possible value ET. This value represents the unit of time Elapsed Months, which refers to months without regard to weekends or holidays. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

A TemplateTask object represents a Task that is part of a Template. Template Tasks become Tasks in the Project where the Template is used.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> <p style="font-weight: normal;">The following fields added the possible value ET. This value represents the unit of time Elapsed Months, which refers to months without regard to weekends or holidays.</p> 
    <ul> 
     <li style="font-weight: bold;">durationUnit</li> 
     <li style="font-weight: bold;">workUnit</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collection Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allPriorities</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Timesheet {#timesheet}

A&nbsp;Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Core Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>objCode</p> <p style="font-weight: normal;">Removed</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Update {#update}

Work Items in Workfront can be updated to keep users informed of the current status. An Update object represents one of these updates. Updates can be entered by users or created by the Workfront system.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>updateType</p> <p style="font-weight: normal;">Added possible value referenceObjectCustomData (enum.updatetypeenum.referenceobjectcustomdata) &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Queries</td> 
   <td> <p style="font-weight: normal;">The following queries were added to the Update object.</p> 
    <ul> 
     <li style="font-weight: bold;">objectUpdatesMobile</li> 
     <li style="font-weight: bold;">updateThreadMobile</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="user">User</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">A User object represents a person with an account in Workfront that can log in and interact with the system.</p>
-->

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Collection Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>loginAsAccessRules</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actions</td> 
   <td> <p style="font-weight: normal;">The following actions were added to the User object.</p> 
    <ul> 
     <li style="font-weight: bold;">hasGrantLoginAsAccess</li> 
     <li style="font-weight: bold;">isUserAdmin</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Queries</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>userAdmins</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserNote {#usernote}

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Actions</td> 
   <td> <p style="font-weight: normal;">The following actions were added to the User object.</p> 
    <ul> 
     <li style="font-weight: bold;">acknowledgeMyNotifications</li> 
     <li style="font-weight: bold;">unacknowledgedAllObjectsTypeCount &nbsp;</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Queries</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>myAllObjectTypesUnreadNotifications</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Work  {#work}

A Work object is a common interface that both Task and OpTask inherit, and shares common code between the two.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td colspan="2">Direct Fields<p style="font-weight: normal;">The following fields added the validators AT_DATE_BEFORE_YEAR and AT_DATE_AFTER_YEAR. These valdators specify that dates on associated objects can't be set before the year 1900 or after 2200.</p>
    <ul>
     <li style="font-weight: bold;">actualCompletionDate</li>
     <li style="font-weight: bold;">actualStartDate</li>
     <li style="font-weight: bold;">constraintDate</li>
     <li style="font-weight: bold;">plannedCompletionDate</li>
     <li style="font-weight: bold;">plannedStartDate</li>
    </ul><p style="font-weight: normal;">The following fields were added to the public API for transparency in calculating EAC (Estimate at Completion).</p>
    <ul>
     <li><p style="font-weight: bold;">bcwp</p><p style="font-weight: normal;">Also known as the Earned Value, the Budgeted Cost of Work Performed (BCWP) is a project performance metric that represents the budgeted cost of the amount of the task that has actually completed at the time when this metric is calculated. For tasks, BCWP = Actual Percent Complete x Task Budget. For Projects, BCWP = SUM(BCWP values of all parent and individual tasks).</p></li>
     <li><p style="font-weight: bold;">bcws</p><p style="font-weight: normal;">Also known as the Planned Value, the Budgeted Cost of Work Scheduled (BCWS) is a project performance metric that represents the budgeted cost of the amount of the task that should have completed at the time when this metric is calculated. For tasks, BCWS = Planned Percent Complete x Task Budget. For projects, BCWS = SUM(BCWS values of all parent and individual tasks).</p></li>
    </ul><p style="font-weight: normal;">The following fields added the possible value ET. This value represents the unit of time Elapsed Months, which refers to months without regard to weekends or holidays.</p>
    <ul>
     <li style="font-weight: bold;">durationUnit</li>
     <li style="font-weight: bold;">workUnit</li>
    </ul><p style="font-weight: normal;">The following field was removed from the Work object.</p>
    <ul>
     <li style="font-weight: bold;">reservedTimeID</li>
    </ul><p style="font-weight: normal;">The following field was added to the Work object.</p>
    <ul>
     <li style="font-weight: bold;">storyPoints</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>reservedTime</p> <p style="font-weight: normal;">Removed &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Collection Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>allConditions</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
