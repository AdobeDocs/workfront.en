---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 12
description: Workfront released API version 12 on November 12, 2020. API version 12 features the following changes from version 11
author: Becky
feature: Workfront API
role: Developer
exl-id: 1ffba3b5-ab24-4ca2-a1ef-f7e5b77e776c
---
# What's new in API version 12

Workfront released API version 12 on November 12, 2020. API version 12 features the following changes from version 11

## Added Resources

The following resources are new in Workfront API version 12.

* [BreadCrumb](#breadcrumb) 
* [RichTextParameterValue](#richtextparametervalue)

### BreadCrumb {#breadcrumb}

A BreadCrumb object represents an element in the parent/child hierarchy of an Adobe Workfront work item. Breadcrumbs indicate how a work item fits into the greater structure of Portfolios, Projects, Projects, and Tasks.

For more information on Breadcrumbs in Workfront, see [Breadcrumbs overview in the new Adobe Workfront experience](../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md)

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> 
   <td>Action</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;">getObjectHierarchy</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### RichTextParameterValue {#richtextparametervalue}

Rich text fields are now available on more objects. The RichTextParameterValue object was added to Workfront to support this availability.

For more information, see [Rich text fields in the Adobe Workfront API](../../wf-api/general/rich-text-field-api.md).

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
     <li style="font-weight: bold;">ID</li> 
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

## Removed Resources

No resources were removed for API version 12.

## Modified Resources

The following resources were modified for Workfront API version 12.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
    <ul> 
     <li> <p><a href="#accesslevel" class="MCXref xref">AccessLevel</a> </p> </li> 
     <li> <p><a href="#accesslevelpermissions" class="MCXref xref">AccessLevelPermissions</a> </p> </li> 
     <li> <p><a href="#accessrequest" class="MCXref xref">AccessRequest</a> </p> </li> 
     <li> <p><a href="#accessrule" class="MCXref xref">AccessRule</a> </p> </li> 
     <li> <p><a href="#activitylog" class="MCXref xref">ActivityLog</a> </p> </li> 
     <li> <p><a href="#announcementattachment" class="MCXref xref">AnnouncementAttachment</a> </p> </li> 
     <li> <p><a href="#approval" class="MCXref xref">Approval</a> </p> </li> 
     <li> <p><a href="#calendarsection" class="MCXref xref">CalendarSection</a> </p> </li> 
     <li> <p><a href="#company" class="MCXref xref">Company</a> </p> </li> 
     <li> <p><a href="#customer" class="MCXref xref">Customer</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#customerpreferences" class="MCXref xref">CustomerPreferences</a> </p> </li> 
     <li> <p><a href="#document" class="MCXref xref">Document</a> </p> </li> 
     <li> <p><a href="#documentversion" class="MCXref xref">DocumentVersion</a> </p> </li> 
     <li> <p><a href="#group" class="MCXref xref">Group </a> </p> </li> 
     <li> <p><a href="#linkedfolder" class="MCXref xref">LinkedFolder</a> </p> </li> 
     <li> <p><a href="#optask" class="MCXref xref">OpTask</a> </p> </li> 
     <li> <p><a href="#parameter" class="MCXref xref">Parameter</a> </p> </li> 
     <li> <p><a href="#portfolio" class="MCXref xref">Portfolio</a> </p> </li> 
     <li> <p><a href="#program" class="MCXref xref">Program</a> </p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p><a href="#queuedef" class="MCXref xref">QueueDef</a> </p> </li> 
     <li> <p><a href="#scheduledreport" class="MCXref xref">ScheduledReport</a> </p> </li> 
     <li> <p><a href="#scorecardquestion" class="MCXref xref">ScoreCardQuestion</a> </p> </li> 
     <li> <p><a href="#task" class="MCXref xref">Task</a> </p> </li> 
     <li> <p><a href="#team" class="MCXref xref">Team</a> </p> </li> 
     <li> <p><a href="#templatetask" class="MCXref xref">TemplateTask</a> </p> </li> 
     <li> <p><a href="#timesheet" class="MCXref xref">Timesheet</a> </p> </li> 
     <li> <p><a href="#user" class="MCXref xref">User</a> </p> </li> 
     <li> <p><a href="#work" class="MCXref xref">Work </a> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&nbsp;

### AccessLevel {#accesslevel}

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

For more information on access levels, see [How access levels work](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table style="table-layout:auto"> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> <!--
  <col data-mc-conditions="QuicksilverOrClassic.Draft mode">
 --> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Direct Fields</td>
   --> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">fieldAccessPrivileges</p>
      --> <!--
       <p style="font-weight: normal;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Added the possible value CPJ (Copy). This allows Users with Planner Access Level to copy Projects.</p>
      --> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AccessLevelPermissions {#accesslevelpermissions}

An AccessLevelPermissions object represents a specific permission to access, create, or modify a Workfront object. These permissions can then be associated with an Access Level.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><strong>coreAction</strong> </p> <p>Added the following possibleValues:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>A user with an access level that includes this permission can update planned hours in the Workload Balancer.</p> <p>For more information, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Update task Planned Hours when managing user allocations</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>A user with an access level that includes this permission can add fields to custom forms.</p> <p>For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>A user with an access level that includes this permission can share a custom field system-wide with Delete access.</p> <p>For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>Added the following possibleValues:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>Added the following possibleValues:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">OR</p>
    --> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value PLANNED_HOURS_CONTOURING, which allows a user to update planned hours in the Workload Balancer</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value ADD_TO_CUSTOM_FORMS, which allows a user to add fields to custom forms.</p>
    --> 
    <ul> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">coreAction</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">forbiddenActions</p>
      --> </li> 
     <li> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">secondaryActions</p>
      --> </li> 
    </ul> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The following fields added the possible value EDIT_SYSTEMWIDE, which allows a user to share a custom field system-wide with Delete access. </p>
    --> <!--
     <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
      <li> <p>coreAction</p> </li> 
      <li> <p>forbiddenActions</p> </li> 
      <li> <p>secondaryActions</p> </li> 
     </ul>
    --> </td> 
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
     <li> <p style="font-weight: bold;">action</p> <p>Added the following possibleValues:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>A user with an access level that includes this permission can update planned hours in the Workload Balancer.</p> <p>For more information, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Update task Planned Hours when managing user allocations</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>A user with an access level that includes this permission can add fields to custom forms.</p> <p>For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>A user with an access level that includes this permission can share a custom field system-wide with Delete access.</p> <p>For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</p> </li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li><strong>coreAction</strong> <p>Added the following possibleValues:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>A user with an access level that includes this permission can update planned hours in the Workload Balancer.</p> <p>For more information, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Update task Planned Hours when managing user allocations</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>A user with an access level that includes this permission can add fields to custom forms.</p> <p>For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>A user with an access level that includes this permission can share a custom field system-wide with Delete access.</p> <p>For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>forbiddenActions</strong> </p> <p>Added the following possibleValues:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
     <li> <p><strong>secondaryActions</strong> </p> <p>Added the following possibleValues:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ActivityLog {#activitylog}

An ActivityLog object is a complete list of all activity that has taken place in a given Workfront Proof account.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Operations</p> </td> 
   <td> <p>The following operation was removed from the ActivityLog object:</p> 
    <ul> 
     <li> <p><strong>ADD</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### AnnouncementAttachment {#announcementattachment}

An AnnouncementAttachment object represents a file that has been attached to a Workfront announcement.

For more about announcement attachments, see [Send announcements](../../administration-and-setup/get-started-wf-administration/view-send-announcements.md)

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td> <p>Direct Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>fileExtension</strong> </p> <p>Added possible values:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
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
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Removed the following flags:</p> 
      <ul> 
       <li> <p>DYNAMIC,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>Added the following flags</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMIC,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>This field was added, and represents whether it takes a user a small, medium, or large amount of daily effort to complete a task. Possible values are:</p> 
      <ul> 
       <li> <p>1 (Small)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Large)</p> </li> 
      </ul> <p>For more information on Work Effort in Workfront, see <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort overview</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CalendarSection {#calendarsection}

A Calendar Section is a calendar report.

For more information on calendar reports, see [Calendar reports overview](../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> <p style="font-weight: normal;">The following fields were added to the CalendarSection object to support the new functionality of using custom dates in calendar reports. </p> <p style="font-weight: normal;">For more information, see <a href="../../reports-and-dashboards/reports/calendars/use-custom-dates.md" class="MCXref xref">Use custom date fields in a calendar report</a>.</p> 
    <ul> 
     <li> <p style="font-weight: normal;">customDate</p> </li> 
     <li> <p style="font-weight: normal;">customEndDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">customStartDateParameterID</p> </li> 
     <li> <p style="font-weight: normal;">ignoreActualDates</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Company {#company}

A Company object represents an organization consisting of a collection of people.

For more information on companies, see [Create and edit companies](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">The ID&nbsp;of the group that the company is associated with.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>group</p> <p style="font-weight: normal;">The group that the company is associated with. Associating a company with a group allows the group administrator to extend group access and permissions to the company.</p> </li> 
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
  <tr> 
   <td>Actions</td> 
   <td> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>productEnabled</strong> </p> <p style="font-weight: normal;">This action takes a CustomerProductTypeEnum argument and returns a boolean that says whether that customer has an account for that product. </p> </li> 
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
       <li style="font-weight: normal;">password:zoomIntegrationEnabled (Enable Zoom integration in the updates stream)</li> 
       <li style="font-weight: normal;"> password:quipIntegrationEnabled (config.general.quip.enabled) &nbsp;</li> 
      </ul> </li> 
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
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>createLinkedProofVersion</p> <p style="font-weight: normal;">Added</p> </li> 
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
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Removed possible value:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p style="font-weight: normal;"><strong>proofDecision</strong> </p> <p>Added</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actions</td> 
   <td> <p>The following actions were added to the Document object.</p> 
    <ul> 
     <li> <p style="font-weight: bold;">getDocumentReviewerDecision</p> <p style="font-weight: normal;">This action takes the documentVersonID argument (string) and returns a map that indicates the reviewer's decision.</p> </li> 
     <li style="font-weight: bold;"> <p>setDocumentReviewerDecision</p> <p style="font-weight: normal;">This action takes the following arguments:</p> 
      <ul style="font-weight: normal;"> 
       <li> <p>documentVersionID (string)</p> </li> 
       <li> <p>reviewerDecision (string)</p> </li> 
       <li> <p>comment (string)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Group  {#group}

A Group object represents a set of users and teams. Groups often represent departmental structure. 

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeaderID</p> <p style="font-weight: normal;">The ID&nbsp;of the Business Leader assigned to the group.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>businessLeader</p> <p style="font-weight: normal;">The Business Leader assigned to the group. A Business Leader is someone who makes business decisions for the group.</p> <p style="font-weight: normal;">For more information on business leaders, see <a href="../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader overview</a>.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Actions</td> 
   <td> 
    <ul> 
     <li> <p><strong>assignMultiple</strong> </p> <p>This action takes the following arguments:</p> 
      <ul> 
       <li> <p>userIDs (string[])</p> </li> 
       <li> <p>roleIDs (string[])</p> </li> 
       <li> <p>teamID (string)</p> </li> 
      </ul> </li> 
     <li> <p><strong>getGroupMembers</strong> </p> </li> 
     <li> <p><strong>updateMembersList</strong> </p> <p>This action takes the following arguments:</p> 
      <ul> 
       <li> <p>newMemberIDs (string[])</p> </li> 
       <li> <p>removedMemberDs (string[])</p> </li> 
      </ul> </li> 
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
     <li style="font-weight: bold;"> <p>externalIntegrationType</p> <p style="font-weight: normal;">Removed possible value:</p> 
      <ul> 
       <li style="font-weight: normal;">QUIP (Quip)</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### OpTask {#optask}

An OpTask object is commonly known as an Issue. An issue is a work item that usually indicates that there is a problem preventing the completion of a task or project. An Issue can also be a Help Desk request. Change Orders, Requests, and Bugs are also Issues.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Direct Fields</p> </td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Order indicates a task or story's position on the Agile backlog.</p> <p>This field removed the following flags:
       <ul>
        <li>DYNAMIC,</li>
        <li>LAZY_READ,</li>
        <li>NOT_GROUPABLE:</li>
       </ul></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> <p>These actions added the argument status to support the new Start button functionality, which changes the status of a work item when a user clicks the button to indicate that they have begun work on the item.</p> <p>For more information, see <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Parameter {#parameter}

A Parameter object is a custom field.

The Parameter resource added the flag SHARABLE.

For more information on custom fields, see [Create or edit a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) in [Create or edit a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><strong>dataType</strong> </p> <p>Added possible value:</p> 
      <ul> 
       <li> <p>RICH (Rich Text)</p> <p>For more information, see <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rich text fields in the Adobe Workfront API</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>displayType</strong> </p> <p>Added possible value:</p> 
      <ul> 
       <li> <p>RICH (Text Field with Formatting)</p> <p>For more information, see <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rich text fields in the Adobe Workfront API</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>label</strong> </p> <p>Added</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Collection Fields</td> 
   <td> 
    <ul> 
     <li> <p><strong>accessRules</strong> </p> <p>Added</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Default Fields</td> 
   <td> 
    <ul> 
     <li> <p class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"><strong>label</strong> </p> <p>Added</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Portfolio {#portfolio}

A Portfolio object is a collection of projects that compete for the same resources, typically money or people to complete them.

For more information on portfolios, see [Portfolio overview in Adobe Workfront](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">The ID&nbsp;of the group that the portfolio is associated with.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>group</p> <p style="font-weight: normal;">The group that the portfolio is associated with. </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Program {#program}

A Program object is a subset of projects within a portfolio, where similar projects can be grouped together.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">The ID&nbsp;of the group that the program is associated with.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Reference Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>group</p> <p style="font-weight: normal;">The group that the program is associated with. </p> </li> 
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
     <li><strong>requestorCoreAction</strong> <p>Added the following possibleValues:</p> 
      <ul> 
       <li> <p>PLANNED_HOURS_CONTOURING </p> <p>A user with an access level that includes this permission can update planned hours in the Workload Balancer.</p> <p>For more information, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md#update" class="MCXref xref">Update task Planned Hours when managing user allocations</a> in <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li> 
       <li> <p>ADD_TO_CUSTOM_FORMS </p> <p>A user with an access level that includes this permission can add fields to custom forms.</p> <p>For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#add2" class="MCXref xref"></a> in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</p> </li> 
       <li> <p>EDIT_SYSTEMWIDE </p> <p>A user with an access level that includes this permission can share a custom field system-wide with Delete access.</p> <p>For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configure sharing for custom fields and widgets</a></p> </li> 
      </ul> <li> <p><strong>requestorForbiddenActions</strong> </p> <p>Added the following possibleValues:</p> 
       <ul> 
        <li> <p>PLANNED_HOURS_CONTOURING </p> </li> 
        <li> <p>ADD_TO_CUSTOM_FORMS </p> </li> 
        <li> <p>EDIT_SYSTEMWIDE </p> </li> 
       </ul> </li> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScheduledReport {#scheduledreport}

A ScheduledReport object represents a report that has been configured to be scheduled for delivery.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><strong>format</strong> </p> <p>Added possible values:</p> 
      <ul> 
       <li> <p>qdoc (enum.fileextension.qdoc)</p> </li> 
       <li> <p>qslides (enum.fileextension.qslides)</p> </li> 
       <li> <p>qsheet (enum.fileextension.qsheet)</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### ScoreCardQuestion {#scorecardquestion}

A ScoreCardQuestion object represents a question that has been added to a Scorecard. These questions are usually determined by the Portfolio manager, and their answers allow the manager to understand how well a project aligns with the goals of the portfolio.

For more information on Scorecard Questions, see [Create a scorecard](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>displayType</p> <p style="font-weight: normal;">Added possible value RICH (Text Field with Formatting) </p> <p style="font-weight: normal;">For more information, see <a href="../../wf-api/general/rich-text-field-api.md" class="MCXref xref">Rich text fields in the Adobe Workfront API</a>. &nbsp;</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Task {#task}

A Task object represents a work item that must be performed as a step toward achieving a final goal (completing a Project).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>This field was added, and represents whether it takes a user a small, medium, or large amount of daily effort to complete a task. Possible values are:</p> 
      <ul> 
       <li> <p>1 (Small)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Large)</p> </li> 
      </ul> <p>For more information on Work Effort in Workfront, see <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort overview</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> <p>These actions added the argument status to support the new Start button functionality, which changes the status of a work item when a user clicks the button to indicate that they have begun work on the item.</p> <p>For more information, see <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a>.</p> 
    <ul> 
     <li> <p><strong>acceptWork</strong> </p> </li> 
     <li> <p><strong>unacceptWork</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Team {#team}

A Team object is a collection of Users that can be assigned to a work item.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> <p>The following fields were added to the Team resource:</p> 
    <ul> 
     <li> <p><strong>completeDaysOnKanbanBoard</strong> </p> <p>This field represents the number of days that a completed card remains on the Kanban board.</p> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../agile/get-started-with-agile-in-workfront/configure-kanban.md" class="MCXref xref">Configure Kanban</a>.</p>
      --> </li> 
     <li> <p><strong>groupID</strong> </p> <p>This field associates a team with a group. This identifies the team as part of the group and allows the Group Administrator to manage the teams.</p> </li> 
     <li> <p><strong>workOnItStatusChange</strong> </p> <p>This is a boolean parameter that indicates whether the team's Work on It button has been configured as a Start button. When a member of the team clicks a Start button to begin work on a work item, the item's status changes from New to a status configured in the team settings.</p> </li> 
     <li> <p>The following fields allow you to specify custom statuses for the Start button on the individual work items.</p> 
      <ul> 
       <li> <p><strong>workOnItOpTaskBugReportStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskChangeOrderStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskIssueStatuses</strong> </p> </li> 
       <li> <p><strong>workOnItOpTaskRequestStatuses</strong> </p> <p><strong>workOnItTaskStatuses</strong> </p> </li> 
      </ul> <p>For more information on the Start button, see <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Replace the Work On It button with a Start button</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Reference Fields</td> 
   <td> <p>The following field was added to the Team resource:</p> 
    <ul> 
     <li> <p><strong>group</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### TemplateTask {#templatetask}

A TemplateTask object represents a Task that is part of a Template. Template Tasks become Tasks in the Project where the Template is used.

For more information on Template Tasks, see [Edit a template task](../../manage-work/projects/create-and-manage-templates/edit-template-task.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><strong>workEffort</strong> </p> <p>This field was added, and represents whether it takes a user a small, medium, or large amount of daily effort to complete a task. Possible values are:</p> 
      <ul> 
       <li> <p>1 (Small)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Large)</p> </li> 
      </ul> <p>For more information on Work Effort in Workfront, see <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort overview</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Timesheet {#timesheet}

A&nbsp;Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.

For more information on Timesheets, see [Timesheets overview](../../timesheets/timesheets/timesheets-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Core Fields</td> 
   <td> <p>The following field was removed from the Timesheet resource:</p> 
    <ul> 
     <li> <p><strong>objcode</strong> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Update

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><strong>updateType</strong> </p> <p>Added the following possible values:</p> 
      <ul> 
       <li> <p>initiativeAdd (enum.updatetypeenum.initiativeadd)</p> </li> 
       <li> <p>initiativeEdit (enum.updatetypeenum.initiativeedit)</p> </li> 
      </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">For more information on initiatives, see <a href="../../scenario-planner/initiatives-overview.md" class="MCXref xref">Initiatives overview in the Scenario Planner</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### User {#user}

A User object represents a person with an account in Workfront that can log in and interact with the system.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direct Fields</td> 
   <td> <p>The following fields were added to the User resource:</p> 
    <ul> 
     <li> <p><strong>actualDeactivationDate</strong> </p> <p>This represents the date and time that a user was deactivated.</p> <p>For more information on deactivated Users, see <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </li> 
     <li> <p><strong>alignAccessType</strong> </p> <p>This field shows the user's access to Workfront Goals. Possible values are:</p> 
      <ul> 
       <li> <p>No access</p> </li> 
       <li> <p>View</p> </li> 
       <li> <p>Edit</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Actions</td> 
   <td> <p>The following action was added to the User resource:</p> 
    <ul> 
     <li> <p><strong>getUserAccessPermissionsByObjCode</strong> </p> <p>This action takes the following arguments</p> 
      <ul> 
       <li> <p>ids (string)</p> </li> 
       <li> <p>objCode (string)</p> </li> 
      </ul> </li> 
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
   <td>Direct Fields</td> 
   <td> 
    <ul> 
     <li> <p><strong>backlogOrder</strong> </p> <p>Order indicates a task or story's position on the Agile backlog.</p> <p>This field removed the following flags:</p> 
      <ul> 
       <li> <p>DYNAMIC,</p> </li> 
       <li> <p>LAZY_READ,</p> </li> 
       <li> <p>NOT_GROUPABLE</p> </li> 
      </ul> </li> 
     <li> <p><strong>groupID</strong> </p> <p>This field added the following flags:</p> 
      <ul> 
       <li> <p>AUTO_LOAD,</p> </li> 
       <li> <p>DYNAMIC,</p> </li> 
       <li> <p>READ_ONLY</p> </li> 
      </ul> </li> 
     <li> <p><strong>workEffort</strong> </p> <p>This field was added, and represents whether it takes a user a small, medium, or large amount of daily effort to complete a task. Possible values are:</p> 
      <ul> 
       <li> <p>1 (Small)</p> </li> 
       <li> <p>2 (Medium)</p> </li> 
       <li> <p>3 (Large)</p> </li> 
      </ul> <p>For more information on Work Effort in Workfront, see <a href="../../manage-work/tasks/task-information/work-effort.md" class="MCXref xref">Work Effort overview</a>.</p> </li> 
    </ul> <p style="font-weight: normal;"> &nbsp;</p> </td> 
  </tr> 
 </tbody> 
</table>
