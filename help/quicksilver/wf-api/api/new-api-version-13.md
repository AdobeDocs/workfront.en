---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 13
description: Adobe Workfront released API version 13 on April 22, 2021. API version 13 features the following changes from version 12.
author: Becky
feature: Workfront API
role: Developer
exl-id: afbc986e-8b5c-40bc-9120-e8d34e0f7004
---
# What's new in API version 13

Adobe Workfront released API version 13 on April 22, 2021. API version 13 features the following changes from version 12.

## Added resources

No resources were added for API version 13.

## Removed resources

No resources were removed for API verson 13.

## Modified resources

The following resources were modified for API version 13.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#breadcrumb" class="MCXref xref">BreadCrumb</a> </p> </li> 
     <li> <p><a href="#burndownevent" class="MCXref xref">BurndownEvent</a> </p> </li> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Group </a> </p> </li> 
     <li> <p><a href="#journalentry" class="MCXref xref">JournalEntry</a> </p> </li> 
     <li> <p><a href="#layouttemplate" class="MCXref xref">LayoutTemplate</a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#project" class="MCXref xref">Project</a> </p> </li> 
     <li> <p><a href="#proofapproval" class="MCXref xref">ProofApproval</a> </p> </li> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Task</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Timesheet</a> </p> </li> 
     <li> <p><a href="#timesheetprofile" class="MCXref xref">TimesheetProfile</a> </p> </li> 
     <li> <p><a href="#uitemplate" class="MCXref xref">UITemplate</a> </p> </li> 
     <li> <p><a href="#userdelegation" class="MCXref xref">UserDelegation</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Work </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevel {#accesslevel}

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

For more information on access levels, see [How access levels work](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direct Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Description</b> </p> <p>Added the validator MAX_LENGTH, which specifies that the length of the description is no more than 4000 characters.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BreadCrumb {#breadcrumb}

A BreadCrumb object represents an element in the parent/child hierarchy of a Workfront work item. Breadcrumbs indicate how a work item fits into the greater structure of Portfolios, Projects, Projects, and Tasks.

For more information on breadcrumbs, see [Breadcrumbs overview in the new Adobe Workfront experience](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direct Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Object codes can be found in the <a href="../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### BurndownEvent {#burndownevent}

A BurndownEvent object represents an object that changes the bundown of an iteration.

For more information on burndown, see [Burndown](../../agile/use-scrum-in-an-agile-team/burndown/burndown.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direct Fields</p> </td> 
   <td> <p>The following fields removed the flag NOT_GROUPABLE </p> 
    <ul> 
     <li> <p>applyDate</p> </li> 
     <li> <p>entryDate</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomerPreferences {#customerpreferences}

A CustomerPreferences object represents the set of preferences that a customer has set for their instance of Workfront.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>name</p> <p style="font-weight: normal;">Added possible values:</p> 
      <ul> 
       <li style="font-weight: normal;">password:aemAPIKey (config.general.aem.apikey)</li> 
       <li style="font-weight: normal;"> password:aemAADomain (config.general.aem.aadomain) </li> 
       <li style="font-weight: normal;">password:aemIntegrationEnabled (config.general.aem.enabled)</li> 
       <li style="font-weight: normal;">password:aemHost (config.general.aem.host)</li> 
       <li style="font-weight: normal;">timesheet:default.timesheet.restrict.timesheet.edit.owners.admins (config.timesheet.restrict.timesheet.edit.owners.admins)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actions</td> 
   <td> <p>The following actions were added to the CustomerPreferences resource.</p> 
    <ul> 
     <li> <p><b>getTimesheetPreferences</b> </p> </li> 
     <li> <p><b>setTimesheetPreferences</b> </p> <p>Takes the argument:</p> 
      <ul> 
       <li> <p>preferences (map)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion {#documentversion}

A DocumentVersion object represents a specific version of a file (such as written material, images, or other forms of information).

For more information about document versions, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direct Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Added possible value:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><b>proofID</b> </p> <p>Added flag NOT_FILTERABLE</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Group  {#group}

A Group object represents a set of users and teams. Groups often represent departmental structure.

For more information on groups, see [Groups vs. teams in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Actions</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>getParents</b> </p> <p>This action returns an array of the group's parent groups (groups that the given group is a subgroup of).</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### JournalEntry {#journalentry}

The JournalEntry object can be set up to log information about specific object fields any time those fields are modified. When a field is set up to be logged as a part of the Journal Entry object, a corresponding Journal Entry will be created every time that field is modified.

The JournalEntry resource added the flag REPORTABLE.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direct Fields</p> </td> 
   <td> <p>The following fields removed the flag NOT_GROUPABLE:</p> 
    <ul> 
     <li> <p><b>changeType</b> </p> </li> 
     <li> <p><b>entryDate</b> </p> </li> 
     <li> <p><b>fieldName</b> </p> </li> 
     <li> <p><b>objObjCode</b> </p> </li> 
    </ul> <p>The following fields added the flag NOT_FILTERABLE:</p> 
    <ul> 
     <li> <p><b>subObjCode</b> </p> </li> 
     <li> <p><b>subObjID</b> </p> </li> 
     <li> <p><b>topObjCode</b> </p> </li> 
     <li> <p><b>topObjID</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LayoutTemplate {#layouttemplate}

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. The LayoutTemplate object is specific to Adobe Workfront Classic.

For the object that represents layout templates in the new Adobe Workfront experience, see [UITemplate](#uitemplate)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direct Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>Description</b> </p> <p>Added the validator MAX_LENGTH, which specifies that the length of the description is no more than 4000 characters.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### LinkedFolder {#linkedfolder}

A LinkedFolder object represents a folder linked from an external document provider, such as Google Drive or Dropbox.

For more information on Linked Folders, see [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direct Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>externalIntegrationType</b> </p> <p>Added possible value:</p> 
      <ul> 
       <li> <p>AEM (Adobe Experience Manager)</p> </li> 
      </ul> </li> 
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
   <td> <p>Search Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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
   <td> <p>Direct Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>convertedOpTaskOriginatorID</b> </p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Removed flag NOT&nbsp;FILTERABLE</p>
      --> </li> 
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
   <td> <p>Direct Fields</p> </td> 
   <td> <p>The following fields were added to the ProofApproval resource.</p> 
    <ul> 
     <li> <p><b>approverStage</b> </p> </li> 
     <li> <p><b>DecisionDate</b> </p> </li> 
     <li> <p><b>workflowTemplate</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef {#queuedef}

A QueueDef object represents a Queue, which is a Project that has been published to the Help Desk area to allow users to submit Issues to it.

For more information on Request Queues, see [Create a Request Queue](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><b>documentPosition</b> </p> <p>Added. Possible values are:</p> 
      <ul> 
       <li> <p>0 (After custom forms)</p> </li> 
       <li> <p>1 (Before custom forms)</p> </li> 
      </ul> </li> 
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
   <td> <p>Search Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
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

### Timesheet {#timesheet}

A&nbsp;Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Added</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Core Fields</td> 
   <td> 
    <ul> 
     <li> <p><b>objCode</b> </p> <p>Removed</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TimesheetProfile {#timesheetprofile}

A&nbsp;Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Added</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Default Fields</td> 
   <td> 
    <ul> 
     <li> <p><b>isOvertimeDisabled</b> </p> <p>Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UITemplate {#uitemplate}

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. The UITemplate object is specific to the new Adobe Workfront experience.

For the object that represents layout templates in Adobe Workfront Classic, see [LayoutTemplate](#layouttemplate).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> <p>The following actions were added to the UITemplate resource.</p> 
    <ul> 
     <li> <p><b>migrateCustomersAllLayoutTemplates</b> </p> <p>Takes the argument:</p> 
      <ul> 
       <li> <p>overrideIfExists (boolean)</p> </li> 
      </ul> </li> 
     <li> <p><b>migrateLayoutTemplates</b> </p> <p>Takes the arguments:</p> 
      <ul> 
       <li> <p>layoutTemplateIDs (string[])</p> </li> 
       <li> <p>overrideIfExists (boolean)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### UserDelegation {#userdelegation}

A UserDelegation object represents the act of delegating work from one user to another for a specific period of time.

The UserDelegation object added the flag REPORTABLE.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> <p>The following fields removed the flag NOT_GROUPABLE</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Default Fields</td> 
   <td> <p>The following fields were added:</p> 
    <ul> 
     <li> <p><b>endDate</b> </p> </li> 
     <li> <p><b>startDate</b> </p> </li> 
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
   <td> <p>Search Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>favoritedByUsersMM</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
