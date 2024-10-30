---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect data dictionary
description: This page contains information about the structure and content of the data in Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
---
# Workfront Data Connect data dictionary

This page contains information about the structure and content of the data in Workfront Data Connect. 

>[!NOTE]
>
>The data in Data Connect refreshes every four hours, so recent changes may not be immediately reflected.

## Table types

There are a number of table types you can utilize in Data Connect to view your Workfront data in a way that provides the most insight.

* **Current table**

  The Current table reflects data similarly to how it exists in Workfront, every object and its current state. However, it can be navigated with much lower latency than within Workfront.

* **Event table**

  The Event table tracks every change record in Workfront: that is, every time an object changes state, a record is created that shows when the change happened, who made the change, and what was changed. Therefore, this table is useful for point-in-time comparisons. This table only includes records from the past three years. 

* **Daily History table**

  The Daily History table offers an abbreviated version of the Event table, in that it shows the state of each object on a daily basis rather than when each individual event occurred. As such, this table is useful for trend analysis.

<!-- Custom table -->

## Entity relationship diagram

Objects in Workfront (and, therefore, in your Data Connect data lake) are defined not only by their individual values, but by their relationships with other objects. The entity relationship diagram below provides a high-level mapping of object relationships in Data Connect. The diagram can be viewed and downloaded using the following link:

[Data Connect entity relationship diagram](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>The entity relationship diagram is a work in progress—as such, it is for reference purposes only and is subject to change.

## Date types

There are a number of date objects that provide information about when specific events occur. 

* `DL_LOAD_TIMESTAMP`: This date is used for internal reference, and reflects when the data was loaded into the Current, Event, or Daily History table. This date should not be used for data analysis, and planned to be removed during the beta phase of Workfront data lake.
* `CALENDAR_DATE`: This date is present only in the Daily History table. This table provides a record of what the data looked like at 11:59 UTC for each date specified in `CALENDAR_DATE`.
* `BEGIN_EFFECTIVE_TIMESTAMP`: This date is present in both Event and Daily History tables, and records exactly when a record changed _to_ the value it has in the current row.
* `END_EFFECTIVE_TIMESTAMP`: This date is present in both Event and Daily History tables, and records exactly when a record changed _from_ the value in the current row to a value in a different row. To allow for between queries on `BEGIN_EFFECTIVE_TIMESTAMP` and `END_EFFECTIVE_TIMESTAMP` this is value is never null, even if there is no new value. In the event a record is still valid (i.e., the value has not changed), `END_EFFECTIVE_TIMESTAMP` will have a value of 2300-01-01.

## Terminology table

The following table correlates object names in Workfront (as well as their names in the interface and API) with their equivalent names in Data Connect.

<table>
  <thead>
    <tr>
        <th>Workfront Entity Name</th>
        <th>Interface References</th>
        <th>API Reference | Label</th>
        <th>Data Lake Tables</th>
        <th>Relationships Field</th>
        <th>Relationship Table &amp; Field</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>Access Level</td>
        <td>Access Level</td>
        <td>ACSLVL | Access Level</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td>ACCESSLEVELID (self)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>Self<br>Not a relationship; used for internal application purposes<br>USER_CURRENT | USERID<br>Not a relationship; used for internal application purposes<br>The ID of the object identified in the OBJCODE field<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Access Rule</td>
        <td>Share</td>
        <td>ACSRUL | Share</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td>ACCESSORID <br>ACCESSRULEID (self)  <br>ANCESTORID  <br>LASTUPDATEDBYID  <br>SECURITYOBJID <br>SYSID</td>
        <td>The ID of the object identified in ACCESSOROBJCODE field<br>Self<br>The ID of the object identified in the ANCESTOROBJCODE field<br>USERS_CURRENT | USERID<br>The ID of the object identified in the SECURITYOBJCODE field<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Approval Path</td>
        <td>Approval Path</td>
        <td>ARVPTH | Approval</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td>APPROVALPATHID (self) <br>APPROVALPROCESSID  <br>ENTEREDBYID  <br>GLOBALPATHID  <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>Not a relationship; used for internal application purposes<br>USERS_CURRENT | USERID<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Approval Process</td>
        <td>Approval Process</td>
        <td>ARVPRC | Approval Process</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td>APPROVALPROCESSID (self) <br>ENTEREDBYID  <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Approval Step</td>
        <td>Approval Step</td>
        <td>ARVSTP | Approval Stage</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td>APPROVALPATHID <br>APPROVALSTEPID (self)  <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>Self<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>ApproverStatus</td>
        <td>Approver Status</td>
        <td>ARVSTS | ApproverStatus</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        <td>APPROVERSTATUSID (self)<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID  <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br>SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>Self<br>The ID of the object identified in the APPROVABLEOBJCODE field<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | USERID  <br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>OPTASKS_CURRENT | OPTASKID<br>USERS_CURRENT | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>Not a relationship; used for internal application purposes<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Assignment</td>
        <td>Assignment</td>
        <td>ASSGN | Assignment</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID (self)<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>Classifier table not supported currently<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Awaiting Approvals</td>
        <td>Awaiting Approvals</td>
        <td>AWAPVL | Awaiting Approval</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td>ACCESSREQUESTID<br>APPROVABLEID  <br>APPROVERID  <br>AWAITINGAPPROVALID (self)  <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID  <br>PROJECTID  <br>ROLEID  <br>SUBMITTEDBYID <br>SYSID<br>TASKID  <br>TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>Access Request table not supported currently<br>Not a relationship; used for internal application purposes<br>USERS_CURRENT | USERID<br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>PROJECTS_CURRENT | PROJECTID<br>ROLES_CURRENT | ROLEID<br>USERS_CURRENT | USERID<br>Not a relationship; used for internal application purposes<br>TASKS_CURRENT | TASKID<br>TEAMS_CURRENT | TEAMID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Baseline</td>
        <td>Baseline</td>
        <td>BLIN | Baseline</td>
        <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        <td>BASELINEID (self)<br>EXCHANGERATEID  <br>PROJECTID  <br>SYSID</td>
        <td>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Baseline Task</td>
        <td>Baseline Task</td>
        <td>BSTSK | Baseline Task</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td>BASELINEID<br>BASELINETASKID (self)  <br>EXCHANGERATEID  <br>PROJECTID  <br>SYSID<br>TASKID</td>
        <td>BASELINES_CURRENT | BASELINEID<br>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Not a relationship; used for internal application purposes<br>TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>Billing Rate</td>
        <td>Rate or Override Rate</td>
        <td>RATE | Billing Rate</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID  (self)<br>ROLEID  <br>SOURCERATECARDID  <br>SYSID  <br>TEMPLATEID<br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>Classifier table not supported currently<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Non-Labor Resource Category  table not supported currently<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>The ID of the object identified in the OBJCODE field<br>PROJECTS_CURRENT | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>Self<br>ROLES_CURRENT | ROLEID  <br>RATECARD_CURRENT | RATECARDID  <br>Not a relationship; used for internal application purposes  <br>TEMPLATES_CURRNT | TEMPLATEID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Billing Record</td>
        <td>Billing Record</td>
        <td>BILL | Billing Record</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td>BILLINGRECORDID (self)<br>CATEGORYID<br>EXCHANGERATEID  <br>INVOICEID  <br>LASTUPDATEDBYID  <br>PROJECTID  <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID  <br>Invoice  table not supported currently  <br>USERS_CURRENT | USERID  <br>PROJECTS_CURRENT | PROJECTID   <br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Booking</td>
        <td>Booking</td>
        <td>BOOKNG | Booking</td>
        <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        <td>BOOKINGID (self)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Non-labor Resource Category table not supported currently<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>The ID of the object identified in the OBJOBJCODE field<br>PROJECTS_CURRENT | PROJECTID <br>Not a relationship; used for internal application purposes<br>TASKS_CURRENT | TASKID     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>The ID of the object identified in the TOPOBJCODE field</td>
    </tr>
    <tr>
        <td>Category</td>
        <td>Custom Form</td>
        <td>CTGY | Category</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td>CATEGORYID (self)<br>ENTEREDBYID<br>GROUPID  <br>LASTUPDATEDBYID  <br>SYSID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID  <br>USERS_CURRENT | USERID  <br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Category Parameter</td>
        <td>Custom Form Fields</td>
        <td>CTGYPA | Category Parameter</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td>CATEGORIESPARAMETERID (self)<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID    <br>SYSID</td>
        <td>Self<br>CATEGORIES_CURRENT | CATEGORYID<br>Parameter Group table not supported currently<br>PARAMETERS_CURRENT | PARAMETERID    <br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Company</td>
        <td>Company</td>
        <td>CMPY | Company</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td>CATEGORYID<br>COMPANYID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID  <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID  <br>RATECARD_CURRENT | RATECARDID<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Custom Quarter</td>
        <td>Custom Quarter</td>
        <td>CSTQRT | Custom Quarter</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td>CUSTOMQUARTERID (self)  <br>SYSID</td>
        <td>Self<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>Condition, Priority, Severity, Status</td>
        <td>CSTEM | Custom Enum</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT<br>* The type of record is identified through the `enumClass` property. The following are the expected types:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID</td>
    </tr>
    <tr>
        <td>Document</td>
        <td>Document</td>
        <td>DOCU | Document</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASEVERSIONID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID<br>USERID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>Self<br>Document Request table not supported currently<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>Varibale depending on DOCOBJCODE value<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Release Version table not supported currently<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Varibale depending on TOPOBJCODE value<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Document Approval</td>
        <td>Document Approval</td>
        <td>DOCAPL | Document Approval</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td>APPROVERID<br>DOCAPPROVALID (self)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | USERID  <br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID  <br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Document Folder</td>
        <td>Document Folder</td>
        <td>DOCFLD | DocsFolders</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td>DOCFOLDERID (self)<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID  <br>PROGRAMID    <br>PROJECTID<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>Self<br>USERS_CURRENT | USERID<br>OPTASKS_CURRENT | OPTASKID<br>ITERATIONS_CURRENT | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_CURRENT | PORTFOLIOID  <br>PROGRAM_CURRENT | PROGRAMID    <br>PROJECTS_CURRENT | PROJECTID <br>Not a relationship; used for internal application purposes<br>TASKS_CURRENT | TASKID     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>DocumentProvideMetadata</td>
        <td>Document Provide Metadata</td>
        <td>DOCMET | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td>DOCPROVIDERMETAID (self)  <br>SYSID</td>
        <td>Self<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>Document Provider</td>
        <td>DOCPRO | Document Provider</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID (self)<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>Self<br>USERS_CURRENT | USERID    <br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>Document Provider Config</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td>DOCPROVIDERCONFIGID (self)<br>SYSID</td>
        <td>Self<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>DocumentVersion</td>
        <td>Document Version</td>
        <td>DOCV | Document Version</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>Self<br>USER_CURRENT | USERID<br>External ID<br>Proof Approval Status table not supported currently<br>USER_CURRENT | USERID<br>Proof table not supported currently<br>USER_CURRENT | USERID<br>Proof Stage table not supported currently</td>
    </tr>
    <tr>
        <td>Exchange Rate</td>
        <td>Exchange Rate</td>
        <td>EXRATE | Exchange Rate</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td>EXCHANGERATEID (self)<br>PROJECTID<br>SYSID  <br>TEMPLATEID  </td>
        <td>Self<br>PROJECTS_CURRENT | PROJECTID <br>Not a relationship; used for internal application purposes  <br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>Expense</td>
        <td>Expense</td>
        <td>EXPNS | Expense</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID  <br>EXPENSEID (self)  <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID  <br>Self  <br>EXPENSETYPES_CURRENT | EXPENSETYPEID <br>USERS_CURRENT | USERID <br>The ID of the object identified in the OBJCODE field <br>PROJECTS_CURRENT | PROJECTID <br>Not a relationship; used for internal application purposes<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>The ID of the object identified in the TOPOBJCODE field</td>
    </tr>
    <tr>
        <td>Expense Type</td>
        <td>Expense Type</td>
        <td>EXPTYP | Expense Type</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td>APPGLOBALID<br>EXPENSETYPEID (self)<br>OBJID  <br>SYSID  </td>
        <td>Not a relationship; used for internal application purposes<br>Self<br>The ID of the object identified in the OBJCODE field  <br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Group</td>
        <td>Group</td>
        <td>GROUP | Group</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>Self<br>Layout Template table will not be supported<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Hour</td>
        <td>Hour</td>
        <td>HOUR | Hour</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>ROLEID<br>TASKID<br>TIMESHEETID</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>Classifier table not supported currently<br>Not a relationship; used for internal application purposes<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Not a Workfront relationship; used for integration to external systems<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Not a relationship; used for internal application purposes<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TIMESHEET_CURRENT | TIMESHEETID</td>
    </tr>
    <tr>
        <td>Hour Type</td>
        <td>Hour Type</td>
        <td>HOURT | Hour Type</td>
        <td>HOURTYPES_CURRENT</td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>Not a relationship; used for internal application purposes<br>Self<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Iteration</td>
        <td>Iteration</td>
        <td>ITRN | Iteration</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID (self)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID <br>Self<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Not a relationship; used for internal application purposes<br>TEAMS_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Journal Entry</td>
        <td>Journal Entry</td>
        <td>JRNLE | Journal Entry</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID  <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID<br>INITIATIVEID<br>JOURNALENTRIEID (self)<br>OBJID<br>OPTASKID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>SUBOBJID<br>SUBSCRIBEID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TIMESHEETID<br>TOPOBJID<br>USERID</td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>Audit record  table not supported currently<br>BASELINES_CURRENT | BASELINEID  <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTS_CURRENT | DOCUMENTID <br>Document Share table not supported currently <br>USERS_CURRENT | USERID<br>EXPENSES_CURRENT | EXPENSEID<br>HOURS_CURRENT | HOURID<br>Initiative table not supported currently<br>Self<br>The ID of the object identified in the OBJCODE field<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>The ID of the object identified in the SUBOBJCODE field<br>Subscribe table not supported currently<br>Not a relationship; used for internal application purposes<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>The ID of the object identified in the TOPOBJCODE field<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LNKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID (self)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>External ID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID  <br>Self<br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Milestone</td>
        <td>Milestone</td>
        <td>MILE | Milestone</td>
        <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>Self<br>MILESTONEPATH_CURRENT | MILESTONEID</td>
    </tr>
    <tr>
        <td>MilestonePath</td>
        <td>Milestone Path</td>
        <td>MPATH | Milestone Path</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>NonLaborResource</td>
        <td>Non-labor resource</td>
        <td>NLBR | Non-labor resource</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td>CATEGORYID<br>NONLABORRESOURCEID (self)<br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID  <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>USERS_CURRENT | USERID  <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID  <br>Non-labor Resource Category table not supported currently  <br>Not a relationship; used for internal application purposes    </td>
    </tr>
    <tr>
        <td>Non-Work Day</td>
        <td>Schedule Exception</td>
        <td>NONWKD | Non Work Day</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td>NONWORKDAYID (self)<br>OBJID  <br>SCHEDULEID  <br>SYSID  <br>USERID  </td>
        <td>Self<br>The ID of the object identified in the OBJCODE field  <br>SCHEDULES_CURRENT | SCHEDULEID  <br>Not a relationship; used for internal application purposes  <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Note</td>
        <td>Note</td>
        <td>NOTE | Note</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td>ATTACHDOCUMENTID<br>ATTACHOBJID<br>ATTACHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PARENTENDORSEMENTID<br>PARENTJOURNALENTRYID<br>PARENTNOTEID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>PROOFACTIONID<br>PROOFID<br>RICHTEXTNOTEID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>THREADID<br>TIMESHEETID<br>TOPOBJID<br>USERID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>Variable depending on ATTACHOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | USERID<br>Audit Record table not supportd currently<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENT_CURRENT | DOCUMENTID<br>Not a Workfront relationship; used for integration to external systems<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>Variable depending on the NOTEOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>Endorsement table not supported currently<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTE_CURRENT | NOTEID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Proof Action table not supported currently<br>Proof table not supported currently<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTE_CURRENT | NOTEID<br>TIMESHEET_CURRENT | TIMESHEETID<br>Variable depending on TOPOBJCODE<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Object Integration</td>
        <td>Object Integration</td>
        <td>OBJINT | ObjectIntegration</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   (self)<br>OBJID  <br>SYSID  </td>
        <td>The ID of the object identified in the LINKEDOBJECTCODE field  <br>Self<br>The ID of the object identified in the OBJCODE field  <br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Objects Category</td>
        <td>Object Categories</td>
        <td>OBJCAT | Object Category</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID (self)<br>OBJID  <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>The ID of the object identified in the OBJCODE field  <br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>OpTask</td>
        <td>Issue, Request</td>
        <td>OPTASK | Issue</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>QUEUEDEFID<br>QUEUETOPICID<br>RESOLVEOPTASKID<br>RESOLVEPROJECTID<br>RESOLVETASKID<br>RESOLVINGOBJID<br>ROLEID<br>SOURCEOBJID<br>SOURCETASKID<br>SUBMITTEDBYID<br>TEAMID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>Kanban Board table not supported currently<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Queue Definition table not supported currently<br>Queue Topic table not supported currently<br>OPTASK_CURRENT | OPTASKID<br>PROJECT_CURRENT | PROJECTID<br>TASK_CURRENT | TASKID<br>Variable depending on RESOLVINGOBJCODE<br>ROLE_CURRENT | ROLEID<br>Variable depending on SOURCEOBJCODE<br>TASK_CURRENT | TASKID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>Parameter</td>
        <td>Custom Field</td>
        <td>PARAM | Parameter</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID  (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br>Parameter Filter table not supported currently<br>Self<br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Parameter Option</td>
        <td>Parameter Option</td>
        <td>POPT | Parameter Option</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td>PARAMETERID<br>PARAMETEROPTIONID (self)  <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>Self  <br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Portal Section</td>
        <td>Report</td>
        <td>PTLSEC | Report</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID (self)<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VIEWID</td>
        <td>Not a relationship; used for internal application purposes  <br>USERS_CURRENT | USERID  <br>UIFILTERS_CURRENT | FILTERID<br>UIGROUPBYS_CURRENT | GROUPBYID<br>USERS_CURRENT | USERID  <br>USERS_CURRENT | USERID  <br>The ID of the object identified in the OBJOBJCODE field<br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | USERID  <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | USERID  <br>Scheduled Report table not supported currently<br>Not a relationship; used for internal application purposes  <br>UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>Portal Tab</td>
        <td>Dashboard</td>
        <td>PTLTAB | Dashboard</td>
        <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID (self)<br>SYSID<br>USERID</td>
        <td>Not a relationship; used for internal application purposes  <br>USERS_CURRENT | USERID  <br>Portal Profile table will not be supported <br>Self<br>Not a relationship; used for internal application purposes  <br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Portal Tab Section</td>
        <td>Dashboard Section</td>
        <td>PRTBSC | Portal Tab Section</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID  <br>PORTALSECTIONOBJID  <br>PORTALTABID<br>PORTALTABSECTIONID (self)<br>SYSID</td>
        <td>Calendar Portal Section not supported currently<br>External Sections table not supported currently<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID  <br>The ID of the object identified in the PORTALSECTIONOBJCODE field<br>PORTALTABS_CURRENT | PORTALTABID<br>Self<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>Report Last Viewers</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td>REPORTID<br>REPORTLASTVIEWERID (self)<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID  <br>REPORTLASTVIEWERID (self)<br>Not a relationship; used for internal application purposes<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Portfolio</td>
        <td>Portfolio</td>
        <td>PORT | Portfolio</td>
        <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT<br>PORTFOLIOS_CUSTOM_VALUE_CURRENT<br>PORTFOLIOS_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIOS_CUSTOM_VALUE_EVENT</td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>Scorecard table not supported currently<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>Preference</td>
        <td>View, Filter, Grouping, Report Definition</td>
        <td>PROSET | Preference</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        <td>APPGLOBALID<br>PREFERENCEID (self)  <br>SYSID  </td>
        <td>Not a relationship; used for internal application purposes<br>Self  <br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Program</td>
        <td>Program</td>
        <td>PRGM | Program</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>Self</td>
    </tr>
    <tr>
        <td>Project</td>
        <td>Project</td>
        <td>PROJ | Project</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID<br>OWNERID<br>POPACCOUNTID<br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFID<br>REJECTIONISSUEID<br>RESOURCEPOOLID<br>SCHEDULEID<br>SPONSORID<br>SUBMITTEDBYID<br>TEAMID<br>TEMPLATEID</td>
        <td>Not a Workfront relationship; used for integration to external systems<br>Scorecard table not supported currently<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>Scorecard table not supported currently<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>USER_CURRENT | USERID<br>Pop Account table not supported currently<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Self<br>Queue Definition  table not supported currently<br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>RateCard</td>
        <td>Rate Card</td>
        <td>RTCRD |Rate Card</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID  <br>RATECARDID (self) <br>SECURITYROOTID  <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>USERS_CURRENT | USERID  <br>USERS_CURRENT | USERID    <br>Self<br>The ID of the object identified in the SECURITYOBJCODE field  <br>The ID of the object identified in the SOURCEOBJCODE field<br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Report Folder</td>
        <td>Report Folder</td>
        <td>RPTFDR | Report Folder</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td>REPORTFOLDERID (self)  <br>SYSID  </td>
        <td>Self  <br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Reserved Time</td>
        <td>(Personal) Time Off</td>
        <td>RESVT | Time Off</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td>RESERVEDTIMEID (self)  <br>SYSID<br>TASKID<br>USERID  </td>
        <td>Self<br>Not a relationship; used for internal application purposes<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | USERID  </td>
    </tr>
    <tr>
        <td>Resource Pool</td>
        <td>Resource Pool</td>
        <td>RSPL | Resource Pool</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID  (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Self<br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Rich Text Note</td>
        <td>Rich Text Note</td>
        <td>RHNOTE | Rich Text Note</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td>RICHTEXTNOTEID (self)  <br>SYSID  </td>
        <td>Self  <br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Rich Text Parameter Value</td>
        <td>Rich Text Parameter Value</td>
        <td>RCHVAL | RichTextParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID (self)  <br>SYSID  </td>
        <td>Paramter Value table not supported currently<br>Self  <br>Not a relationship; used for internal application purposes  </td>
    </tr>
    <tr>
        <td>Risk</td>
        <td>Risk</td>
        <td>RISK | Risk</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td>ENTEREDBYID<br>EXCHANGERATEID<br>LASTUPDATEDBYID  <br>PROJECTID  <br>RISKID (self)<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | USERID  <br>PROJECTS_CURRENT | PROJECTID   <br>Self<br>RISKTYPES_CURRENT | RISKTYPEID<br>Not a relationship; used for internal application purposes<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Risk Type</td>
        <td>Risk Type</td>
        <td>RSKTYP | Risk Type</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>Self<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Role</td>
        <td>Job Role</td>
        <td>ROLE | Job Role</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>Layout Template table will not be supported<br>RATECARD_CURRENT | RATECARDID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Schedule</td>
        <td>Schedule</td>
        <td>SCHED | Schedule</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>Self</td>
    </tr>
    <tr>
        <td>Step Approver</td>
        <td>Step Approver</td>
        <td>SPAPVR | Stage Approver</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID (self)<br>SYSID  <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>ROLES_CURRENT | ROLEID<br>Self<br>Not a relationship; used for internal application purposes  <br>TEAMS_CURRENT | TEAMID<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Task</td>
        <td>Task</td>
        <td>TASK | Task</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>PROJECTID<br>RECURRENCERULEID<br>REJECTIONISSUEID<br>RESERVEDTIMEID<br>ROLEID<br>SUBMITTEDBYID<br>TASKID<br>TEAMID<br>TEMPLATETASKID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | ITERATIONID<br>Kanban Board table not supported currently<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | PROJECTID<br>Recurrence Rule table not supported currently<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>USER_CURRENT | USERID<br>Self<br>TEAM_CURRENT | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Task Predecessor</td>
        <td>Predecessor</td>
        <td>PRED | Predecessor</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td>ID (self)<br>PREDECESSORID<br>SUCCESSORID  <br>SYSID</td>
        <td>Self<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID  <br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Team</td>
        <td>Team</td>
        <td>TEAMOB | Team</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>Layout Template table will not be supported<br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | USERID<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Team Member</td>
        <td>Other Teams, Team Member</td>
        <td>TEAMMB | Team Member</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID  (self)<br>USERID</td>
        <td>Not a relationship; used for internal application purposes <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>TeamMemberRole</td>
        <td>Team Member Role</td>
        <td>TEAMMR | Team Member Role</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID  (self)<br>USERID</td>
        <td>ROLES_CURRENT | ROLEID <br>TEAMS_CURRENT | TEAMID<br>Self<br>USERS_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Template</td>
        <td>Template</td>
        <td>TMPL | Template</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID  <br>DELIVERABLESCORECARDID  <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID  <br>OWNERID  <br>PRIVATERATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID  <br>SYSID  <br>TEAMID<br>TEMPLATEID (self)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID  <br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID  <br>USERS_CURRENT | USERID  <br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | PROGRAMID<br>Queue Definition table not supported currently<br>SCHEDULES_CURRENT | SCHEDULEID  <br>Not a relationship; used for internal application purposes  <br>TEAMS_CURRENT | TEAMID<br>Self</td>
    </tr>
    <tr>
        <td>Template Assignment</td>
        <td>Template Assignment</td>
        <td>TASSGN | Template Assignment</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID (self)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>The ID of the object identified in the OBJCODE field<br>ROLES_CURRENT | ROLEID<br>Not a relationship; used for internal application purposes<br>TEAMS_CURRENT | TEAMID<br>Team Timelineable table not supported currently<br>Self<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Template Task</td>
        <td>Template Task</td>
        <td>TTSK | Template Task</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENCERULEID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEID<br>TEMPLATETASKID  (self)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>Recurrence Rule table not supported currently<br>ROLES_CURRENT | ROLEID<br>Not a relationship; used for internal application purposes<br>TEAMS_CURRENT | TEAMID<br>Team Timelineable table not supported currently<br>TEMPLATES_CURRENT | TEMPLATEID<br>Self</td>
    </tr>
    <tr>
        <td>Template Task Predecessor</td>
        <td>Template Predecessor</td>
        <td>TPRED | Predecessor</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td>PREDECESSORID<br>SUCCESSORID  <br>TEMPLATEPREDECESSORID (self)<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID  <br>Self<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>Timesheet</td>
        <td>Timesheet</td>
        <td>TSHET | Timesheet</td>
        <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | USERID</td>
    </tr>
    <tr>
        <td>Timesheet Profile</td>
        <td>Timesheet Profile</td>
        <td>TSPRO | Timesheet Profile</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td>APPROVERID<br>ENTEREDBYID  <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID (self)</td>
        <td>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID  <br>GROUPS_CURRENT | GROUPID<br>Not a relationship; used for internal application purposes<br>Self</td>
    </tr>
    <tr>
        <td>UI Filter</td>
        <td>Filter</td>
        <td>UIFT | Filter</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID  <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID  <br>UIFILTERID  (self)</td>
        <td>Not a relationship; used for internal application purposes<br>USERS_CURRENT | USERID  <br>USERS_CURRENT | USERID <br>The ID of the object identified in the OBJCODE field<br>PREFERENCES_CURRENT | PREFERENCEID<br>Not a relationship; used for internal application purposes  <br>Self</td>
    </tr>
    <tr>
        <td>UI Group By</td>
        <td>Grouping</td>
        <td>UIGB | Grouping</td>
        <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID  <br>LASTUPDATEDBYID <br>SYSID  <br>UITEMPLATEID  (self)</td>
        <td>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID  <br>USERS_CURRENT | USERID <br>Not a relationship; used for internal application purposes  <br>Self</td>
    </tr>
    <tr>
        <td>UI Template</td>
        <td>Layout Template</td>
        <td>UITMPL | Layout Template</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID  <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID  <br>UIGROUPBYID  (self)</td>
        <td>Not a relationship; used for internal application purposes<br>USERS_CURRENT | USERID  <br>USERS_CURRENT | USERID <br>The ID of the object identified in the OBJCODE field<br>PREFERENCES_CURRENT | PREFERENCEID<br>Not a relationship; used for internal application purposes  <br>Self</td>
    </tr>
    <tr>
        <td>UI View</td>
        <td>View</td>
        <td>UIVIEW | View</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID  <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID  <br>UIVIEWID  (self)</td>
        <td>Not a relationship; used for internal application purposes<br>USERS_CURRENT | USERID  <br>USERS_CURRENT | USERID <br>The ID of the object identified in the OBJCODE field<br>PREFERENCES_CURRENT | PREFERENCEID<br>Not a relationship; used for internal application purposes  <br>Self</td>
    </tr>
    <tr>
        <td>User</td>
        <td>User</td>
        <td>USER | User</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUPDATEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANAGERID<br>PORTALPROFILEID<br>PREFUIID<br>PRIVATERATECARDID<br>RESOURCEPOOLID<br>ROLEID<br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UITEMPLATEID<br>USERID<br>UUMUSERID</td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>Not a relationship; used for internal application purposes<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>TEAM_CURRENT | TEAMID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>Layout Template table will not be supported<br>USER_CURRENT | USERID<br>Portal Profile table will not be supported<br>Not a relationship; used for internal application purposes<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ROLEID<br>SCHEDULE_CURRENT | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Self<br>Not a relationship; used for internal application purposes</td>
    </tr>
    <tr>
        <td>User Delegation</td>
        <td>User Delegation</td>
        <td>USRDEL | User Delegation</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td>FROMUSERID<br>SYSID  <br>TOUSERID <br>USERDELEGATIONID  (self)</td>
        <td>USERS_CURRENT | USERID<br>Not a relationship; used for internal application purposes  <br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>User Group</td>
        <td>Other Groups</td>
        <td>USRGPS | User Group</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td>GROUPID <br>SYSID<br>USERID  <br>USERSGROUPID (self)</td>
        <td>GROUPS_CURRENT | GROUPID <br>Not a relationship; used for internal application purposes<br>USERS_CURRENT | USERID  <br>Self</td>
    </tr>
    <tr>
        <td>User Role</td>
        <td>Other Roles</td>
        <td>USRROL | User Role</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td>ROLEID <br>SYSID<br>USERID    <br>USERROLESETID<br>USERSROLEID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Not a relationship; used for internal application purposes<br>USERS_CURRENT | USERID    <br>USERROLESET_CURRENT | USERROLESETID<br>Self</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | User Preference</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID (self)</td>
        <td>Not a relationship; used for internal application purposes<br>USERS_CURRENT | USERID    <br>Self</td>
    </tr>
    <tr>
        <td>UserRoleSet</td>
        <td>UserRoleSet</td>
        <td>URSET | UserRoleSet</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td>PRIMARYROLEID <br>SYSID<br>USERID    <br>USERROLESETID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Not a relationship; used for internal application purposes<br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>UsersDecisions</td>
        <td>Users Decisions</td>
        <td>USRDEC | Users Decisions</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td>USERDECISIONID (self)<br>SYSID  <br>USERID  </td>
        <td>Self<br>Not a relationship; used for internal application purposes <br>USERS_CURRENT | USERID </td>
    </tr>
    <tr>
        <td>WorkItem</td>
        <td>Work Item</td>
        <td>WRKITM | WorkItem</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>PROJECTID <br>SYSID<br>TASKID    <br>USERID  <br>WORKITEMID (self)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br>The ID of the object identified in the OBJOBJCODE field<br>OPTASK_CURRENT | OPTASKID    <br>PROJECTS_CURRENT | PROJECTID <br>Not a relationship; used for internal application purposes<br>TASKS_CURRENT | TASKID    <br>USERS_CURRENT | USERID    <br>Self </td>
    </tr>
  </tbody>
</table>
