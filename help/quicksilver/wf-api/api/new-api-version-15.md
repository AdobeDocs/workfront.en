---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 15
description: Adobe Workfront released API version 14 on June 14, 2022. API version 15 features the following changes from version 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
---
# What's new in API version 15

Adobe Workfront released API version 15 on June 14, 2022. API version 15 features the following changes from version 14.

## Added resources 

* [Initiative (INITIV)](#Initiati)
    
* [IssueDef (ISSDEF)](#IssueDef)
    
* [ObjectIntegration (OBJINT)](#ObjectIn)
    
* [RichTextGroupParameterValue (GRCVAL)](#RichText)
    
* [TaskDef (TSKDEF)](#TaskDef)
    
* [UserApproval (USRAPV)](#UserAppr)
    
### Initiative (INITIV)

The Initiative object creates estimates in the Workfront Scenario Planner for the kind and number of job roles, the Fixed Costs, and the Planned Benefit.

For more information on Initiatives, see [Initiatives overview in the Scenario Planner](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>This is an internal object.</p>
          </li>
          <li>
            <p><b>duration</b>
            </p>
            <p>The amount of time between endDate and startDate.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>The Planned Completion Date for the Initiative.</p>
          </li>
          <li>
            <p><b>enteredByID</b>
            </p>
            <p>The ID&#160;associated with the user that submitted the request.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>The ID associated with the action</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>The ID associated with the Initiative.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>The date the Initiative was last published in the Workfront Scenario Planner.</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>The name of the Initiative</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>The ID of the Plan associated with the Initiative.</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>The name of the Plan associated with the Initiative.</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>The ID&#160;of the project associated with the initiative.</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>The ID&#160;of the scenario in Workfront Scenario Planner associated with the initiative.</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>The Planned Start Date of the Initiative.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td >
        <ul>
          <li>
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>enteredBy</b>
            </p>
          </li>
          <li>
            <p><b>project</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>name</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>REPORT </b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef (ISSDEF)

The IssueDef object represents a set of data regarding the format of issues. This object can be attached to Projects or Templates, and affects the issues added to that Project or Template.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration (OBJINT)

In some cases, it is possible to link Workfront work items directly to objects in an external software product. The ObjectIntegration object represents this link.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>This is an internal object.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>The date and time that the ObjectIntegration was entered in to the Workfront System.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>The unique Workfront ID of the specific ObjectIntegration object.</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>The external software that the ObjectIntegration object creates a link with. Possible values are:</p>
            <ul>
              <li>
                <p>JIRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>objID</b>
            </p>
            <p>The object in Workfront that the ObjectIntegration is associated with.</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>The object code of the object in Workfront that the ObjectIntegration is associated with.</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td >
        <ul>
          <li>
            <p><b>customer</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef (TSKDEF)

The TaskDef object represents a set of data regarding the format of tasks. This object can be attached to Projects or Templates, and affects the tasks added to that Project or Template.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours </b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td >
        <ul>
          <li>
            <p><b>defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories
</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserApproval (USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields </td>
      <td>
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>requestedDate</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td >
        <ul>
          <li>
            <p><b>approver</b>
            </p>
          </li>
          <li>
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Default fields</td>
      <td >
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>approve</b>
            </p>
          </li>
          <li>
            <p><b>reject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>
            <p><b>ADD</b>
            </p>
          </li>
          <li>
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>REPORT</b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Removed resources

No resources were removed for API version 15.

## Modified resources

* [AccessLevel (ACSLVL)](#AccessLe)
    
* [AccessLevelPermissions (ALVPER)](#AccessLe2)
    
* [AccessRequest (ACSREQ)](#AccessRe)
    
* [AccessRule (ACSRUL)](#AccessRu)
    
* [Approval (APPROVAL)](#Approval)
    
* [Category (CTGY)](#Category)
    
* [CategoryParameter (CTGYPA)](#Category2)
    
* [CustomerPreferences (CUSTPR)](#Customer)
    
* [DocumentFolder (DOCFDR)](#Document)
    
* [DocumentVersion (DOCV)](#Document2)
    
* [Group (GROUP)](#Group)
    
* [JournalEntry (JRNLE)](#JournalE)
    
* [LinkedFolder (LNKFDR)](#LinkedFo)
    
* [OpTask / Issue (OPTASK)](#OpTask)
    
* [Parameter (PARAM)](#Paramete)
    
* [Portfolio (PORT)](#Portfoli)
    
* [Program (PRGM)](#Program)
    
* [Project (PROJ)](#Project)
    
* [QueueDef (QUED)](#QueueDef)
    
* [ScoreCardQuestion (SCOREQ)](#ScoreCar)
    
* [Task (TASK)](#Task)
    
* [Template (TMPL)](#Template)
    
* [Timesheet (TSHET)](#Timeshee)
    
* [View (UIVIEW)](#View)
    
* [Update (UPDATE)](#Update)
    
* [User (USER)](#User)
    
* [UserNote (USRNOT)](#UserNote)
    
* [Work (WORK)](#Work)

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

For more information on access levels, see [Access levels](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (string[])</p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p>VTMAWMG (View teams associated with my groups)</p>
              </li>
              <li>
                <p>VALLTM (View all teams)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions (ALVPER)

An AccessLevelPermissions object represents a specific permission to access, create, or modify a Workfront object. These permissions can then be associated with an Access Level.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Edit teams I am on)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Edit teams in groups I manage (Group Admins only))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Edit teams I am on)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Edit teams in groups I manage (Group Admins only))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Edit teams I am on)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Edit teams in groups I manage (Group Admins only))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>action</b> (string)</p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Edit teams I am on)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Edit teams in groups I manage (Group Admins only))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> (string)</p>
            <p>Added the following possible value:</p>
            <ul>
              <li>
                <p>WDL</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Edit teams I am on)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Edit teams in groups I manage (Group Admins only))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Edit teams I am on)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Edit teams in groups I manage (Group Admins only))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Edit teams I am on)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Edit teams in groups I manage (Group Admins only))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Approval (APPROVAL)

A given work item, such as a task, document, or timesheet, may require that a supervisor or other user sign off on the work item. An Approval object represents the action of signing off on a work item.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td >
        <ul>
          <li>
            <p><b>initiative</b>
            </p>
            <p>Added.</p>
            <p>The Initiative object creates estimates in the Workfront Scenario Planner for the kind and number of job roles, the Fixed Costs, and the Planned Benefit. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>Added.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">Added.</p>
            <p>In some cases, it is possible to link Workfront work items directly to objects in an external software product. The ObjectIntegration object represents this link.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b> (string)</p>
            <p>Added the following possible value:</p>
            <ul>
              <li>
                <p>GROUP (Group)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Added.</p>
            <p style="font-weight: normal;">This parameter is an array of possible objects to which the custom form can be attached. It was added to support the ability to attach a custom form to multiple types of objects.</p>
            <p>Possible values: </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Added.</p>
            <p style="font-weight: normal;">This parameter is an array of possible objects to which the custom form can be attached. It was added to support the ability to attach a custom form to multiple types of objects.</p>
            <p>Possible values: </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormulaFromDescription</b>
            </p>
            <p>Added.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>Added.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>Added.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CustomerPreferences (CUSTPR)

A CustomerPreferences object represents the set of preferences that a customer has set for their instance of Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>name</b>
            </p>
            <p>Added the following values:</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (SharePoint (Graph API) Integration Enabled)</p>
                <p>This value supports the updated Sharepoint integration.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (Allow users to create projects without using a template)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

Documents can be organized into folders. You can create personal folders in your personal Documents area. The DocumentFolder object represents one of these folders.

The DocumentFolder object added the flag `SHARABLE`.

### DocumentVersion (DOCV)

A DocumentVersion object represents a specific version of a file (such as written material, images, or other forms of information).

For more information about document versions, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Added the following value: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>This value supports the updated Sharepoint integration.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Group (GROUP)

A Group object represents a set of users and teams. Groups often represent departmental structure.

For more information on groups, see Groups vs. teams.

The Group object added the flag `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <p>The following fields were added:</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>A Category is a Custom Form. This parameter was added to support the ability to add Custom Forms to Group objects. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>This is a boolean parameter that has a value of true if an object is Active and false if it is not. Objects that are set to Active appear in drop-down menus and type-ahead fields and can be attached to other objects.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td >
        <p>The following fields were added:</p>
        <ul>
          <li>
            <p><b>approver</b>
            </p>
          </li>
          <li>
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <p>The following fields were added:</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In some cases, it is possible to link Workfront work items directly to objects in an external software product. The ObjectIntegration object represents this link.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Default fields</td>
      <td >
        <p>The following field was added:</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>This is a boolean parameter that has a value of true if an object is Active and false if it is not. Objects that are set to Active appear in drop-down menus and type-ahead fields and can be attached to other objects.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <p>The following fields were added:</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>This action recalculates the expressions in custom form fields.</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

The JournalEntry object can be set up to log information about specific object fields any time those fields are modified. When a field is set up to be logged as a part of the Journal Entry object, a corresponding Journal Entry will be created every time that field is modified.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>Added the following value: </p>
        <ul>
          <li>
            <p>DW (Download)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

A LinkedFolder object represents a folder linked from an external document provider, such as Google Drive or Dropbox.

For more information on Linked Folders, see Link documents from external applications.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Added the following value: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>This value supports the updated Sharepoint integration.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask / Issue (OPTASK)

An OpTask object is commonly known as an Issue. An issue is a work item that usually indicates that there is a problem preventing the completion of a task or project. An Issue can also be a Help Desk request. Change Orders, Requests, and Bugs are also Issues.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <p>The following actions were added:</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>The following action was modified:</p>
        <ul>
          <li>
            <p><b>copyIssue</b>
            </p>
            <p>Added field <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Parameter (PARAM)

A Parameter object is a custom field.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <p>The following field was added:</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>The following fields were modified:</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Added the possible value <code>WIDGET </code>(Widget) </p>
            <p>This value supports the use of images in custom forms.</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Added the possible value <code>WIDGET </code>(Widget)</p>
            <p>This value supports the use of images in custom forms.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio (PORT)

A Portfolio object is a collection of projects that compete for the same resources, typically money or people to complete them.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Program (PRGM)

A Program object is a subset of projects within a portfolio, where similar projects can be grouped together.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Project (PROJ)

Projects are work items within Workfront, and are a main building block in the way Workfront helps people to do work. A Project object represents a group of tasks with a common, specific goal.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td >
        <ul>
          <li>
            <p><b>initiative</b>
            </p>
            <p>The Initiative object creates estimates in the Workfront Scenario Planner for the kind and number of job roles, the Fixed Costs, and the Planned Benefit. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In some cases, it is possible to link Workfront work items directly to objects in an external software product. The ObjectIntegration object represents this link.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

For more information on Request Queues, see [Create a Request Queue](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Edit teams I am on)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Edit teams in groups I manage (Group Admins only))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Edit teams I am on)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Edit teams in groups I manage (Group Admins only))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

A ScoreCardQuestion object represents a question that has been added to a Scorecard. These questions are usually determined by the Portfolio manager, and their answers allow the manager to understand how well a project aligns with the goals of the portfolio.

For more information on Scorecard Questions, see [Create a scorecard](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Added the possible value <code>WIDGET </code>(Widget)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Task (TASK)

A Task object represents a work item that must be performed as a step toward achieving a final goal (completing a Project).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In some cases, it is possible to link Workfront work items directly to objects in an external software product. The ObjectIntegration object represents this link.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Template (TMPL)

A Template object represents a pattern for a project. Projects can be created from templates to save time. A template contains a team and tasks, which will be copied to any project created from the template.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Timesheet (TSHET)

A Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <p>The following field was removed:</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### View (UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>The following possible values were removed:</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (Four Column Layout)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (Updates)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (Updates)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (Working On)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (Custom Data)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (Update Custom Data)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (Status Update)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (Status Update)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (Status Update)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (Status Update)</p>
              </li>
              <li>
                <p><code>DLIST</code> (Detail List)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (Detail List Section)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Update (UPDATE)

Work Items in Workfront can be updated to keep users informed of the current status. An Update object represents one of these updates. Updates can be entered by users or created by the Workfront system.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
            <p>Added the possible value <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### User (USER)

A User object represents a person with an account in Workfront that can log in and interact with the system.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserNote (USRNOT)

A UserNote object is a notification.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>eventType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>DUP </code>(Requested that you proof a document)</p>
              </li>
              <li>
                <p><code>DUV </code>(Allow you to view a document)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Work (WORK)

A Work object is a common interface that both Task and OpTask inherit, and shares common code between the two.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In some cases, it is possible to link Workfront work items directly to objects in an external software product. The ObjectIntegration object represents this link.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
