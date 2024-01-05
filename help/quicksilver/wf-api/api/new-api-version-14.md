---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 14
description: Adobe Workfront released API version 14 on September 9, 2021. API version 14 features the following changes from version 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
---
# What's new in API version 14

Adobe Workfront released API version 14 on September 9, 2021. API version 14 features the following changes from version 14.

## Added resources

No resources were added for API version 14.

## Removed resources

No resources were removed for API verson 14.

## Modified resources

The following resources were modified for API version 14.

* [BillingRecord (BILL)](#billingrecord-bill) 
* [Category (CTGY)](#category-ctgy) 
* [CustomEnum (CSTEM)](#customenum-cstem) 
* [Customer (CUST)](#customer-cust) 
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr) 
* [DocumentVersion (DOCV)](#documentversion-docv) 
* [Group (GROUP)](#group-group) 
* [NoteTag (NTAG)](#notetag-ntag) 
* [Project (PROJ)](#project-proj) 
* [QueueDef (QUED)](#queuedef-qued) 
* [Resource Allocation (RSALLO)](#resource-allocation-rsallo) 
* [Role (ROLE)](#role-role) 
* [Template (TMPL)](#template-tmpl) 
* [Timesheet (TSHET)](#timesheet-tshet)

### BillingRecord (BILL) {#billingrecord-bill}

A BillingRecord object records the revenue, hours, or expenses that can be billed. This information can be used to create invoices in an external accounting system.

For more information on billing records, see [Create billing records](../../manage-work/projects/project-finances/create-billing-records.md).

The BillingRecord object added the flag **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Direct Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>Added. A Category is a Custom Form. This parameter was added to support the ability to add Custom Forms to BillingRecord objects.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reference Fields</td> 
   <td> 
    <ul> 
     <li> <p><b>category</b> </p> <p>Added. A Category is a custom form. This parameter was added to support the ability to add custom forms to BillingRecord objects.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Collection Fields</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Added. This represents a collection of Categories (custom forms) associated with the BillingRecord object.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Added. This action recalculates the expressions in custom form fields.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Category (CTGY) {#category-ctgy}

A Category object is a custom form.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>Added possible value:</p> 
      <ul> 
       <li> <p> BILL (BillingRecord)</p> </li> 
      </ul> <p>This value was added to support the ability to add custom forms to BillingRecord objects.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>This action takes the parameters objID and objCode, and returns a boolean.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

The CustomEnum object aids with converting status codes into human-readable text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Queries</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>Added. This query supports the ability to create and manage statuses for groups and subgroups. </p> <p>For more information, see <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Manage group statuses</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Customer (CUST) {#customer-cust}

A Customer object represents an organization that uses an instance of Workfront.

This is an internal object.

### CustomerPreferences (CUSTPR) {#customerpreferences-custpr}

A CustomerPreferences object represents the set of preferences that a customer has set for their instance of Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>Added possible value:</p> 
      <ul> 
       <li> <p>Allow users to add images in updates (updates:images.toggle)</p> </li> 
      </ul> <p>This parameter supports the ability to add images into work item updates. </p> <p>For more information, see <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update work</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

A DocumentVersion object represents a specific version of a file (such as written material, images, or other forms of information).

For more information about document versions, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Added. This field records the date and time of the last callback from Workfront Proof, if the version is associated to a proof.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Group (GROUP) {#group-group}

A Group object represents a set of users and teams. Groups often represent departmental structure.

For more information on groups, see [Groups vs. teams in Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>Added. This action takes an array of groupIDs and adds those groups as subgroups to the specified group.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag (NTAG) {#notetag-ntag}

A NoteTag object represents the act of tagging a user or team in an update to a work item.

For more information on tagging in updates, see [Tag others on updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Operations</td> 
   <td> <p>The following operations were added to the NoteTag object:</p> 
    <ul> 
     <li> <p><b>COUNT</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>REPORT</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Project (PROJ) {#project-proj}

Projects are work items within Workfront, and are a main building block in the way Workfront helps people to do work. A Project object represents a group of tasks with a common, specific goal.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Added.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

For more information on Request Queues, see [Create a Request Queue](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>Added. This action supports the ability to find requests by using the path through the request queue and topic groups.</p> <p>For more information on searching request queues by path, see <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Create requests and generate drafts in the Workfront web app</a> in <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>.</p> </li> 
    </ul> <p>&nbsp;</p> </td> 
  </tr> 
 </tbody> 
</table>

### Resource Allocation (RSALLO) {#resource-allocation-rsallo}

A Resource Allocation object represents the estimate of resources needed for a given project. This object is used only in the legacy Resource Planner. For the corresponding field in the new Resource Planner, use Budgeted Hour (BGHR).

The Resource Allocation object removed the flag **REPORTABLE**.

### Role (ROLE) {#role-role}

A Role object (job role) represents a functional capacity or a skill set a user might fill, such as Designer or Product Manager.

For information on job roles, see [Job role overview](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Added. This is a boolean parameter that has a value of true if an object is Active and false if it is not. Objects that are set to Active appear in drop-down menus and type-ahead fields and can be attached to other objects.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Default Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Template (TMPL) {#template-tmpl}

A Template object represents a pattern for a project. Projects can be created from templates to save time. A template contains a team and tasks, which will be copied to any project created from the template.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Added. This field was added to support the ability to associate groups with templates.</p> <p style="font-weight: normal;">For more information, see <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Edit project templates</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>group</p> <p style="font-weight: normal;">Added. This field was added to support the ability to associate groups with templates.</p> <p style="font-weight: normal;">For more information, see <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Edit project templates</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->
