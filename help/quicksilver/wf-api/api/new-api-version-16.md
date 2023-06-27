---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 16
description: Adobe Workfront released API version 16 on April 6, 2022. API version 16 features the following changes from version 15.
author: Becky
feature: Workfront API
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
---
# What's new in API version 16

Adobe Workfront released API version 16 on April 6, 2022. API version 16 features the following changes from version 15.

## Added resources

No resources were added for API version 16.

## Removed resources

No resources were removed for API version 16

## Modified resources

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Approval (APPROVAL)](#approval-approval)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [ExternalSection (EXTSEC)](#externalsection-extsec)
* [Hour (HOUR)](#hour-hour)
* [LayoutTemplate (UITMPL)](#layouttemplate-uitmpl)
* [Note (NOTE)](#note-note)
* [OpTask / Issue (OPTASK)](#note-note)
* [Project (PROJ)](#project-proj)
* [Rate (RATE)](#rate-rate)
* [RichTextNote (RHNOTE)](#richtextnote-rhnote)
* [Role / Job Role (ROLE)](#role--job-role-role)
* [Task (TASK)](#task-task)
* [Timesheet (TSHET)](#timesheet-tshet)
* [UIFilter / Filter (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Grouping (UIGB)](#uigroupby--grouping-uigb)
* [UIView / View (UIVW)](#uiview--view-uivw)
* [User (USER)](#user-user)
* [UserNote (USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

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
            <p><b>workPerDate</b>
            </p>
            <p>This field has been added, and shows the number of minutes of work per day that you need to do. It has the format <code>YYYY-MM-DD: (number of minutes)</code>, and takes timezone into account.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Assignment (ASSGN)

An assignment object represents the connection between a work item and the user, team, or group that is assigned to work on it.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>This field has been added, and shows the number of minutes of work per day that you need to do. It has the format <code>YYYY-MM-DD: (number of minutes)</code>, and takes timezone into account.</p>
          </li>
          <li>
            <p><b>isContoured</b>
            </p>
            <p>This field has been added, and is a boolean that reflects whether the assignment is contoured. If the assignment's minutes per day has been edited in the Workload Balancer, then the assignment has been contoured.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

The CustomEnum object aids with converting status codes into human-readable text.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
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
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>This action returns a boolean that describes whether the customer has disabled the option to auto-upgrade Contributor license holders.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTSEC)

An ExternalSection object is an external web page that is embedded in a Workfront report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>This was added, and calculates the URL of an iFrame embedded in a report.</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>This was added, and calculates the URLs of  iFrames embedded in a report.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Hour (HOUR)

An Hour object represents an hour logged by a user on a timesheet.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>timesheetHourIdentifier</b>
            </p>
            <p>Added. This parameter is used to identify the hours created with <code>batchSave</code>. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### Note (NOTE)

A Note object is a comment or update made on a Workfront object.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>attachedDocuments</b>
            </p>
            <p>This field was added, and represents a list of documents attached to the comment.</p>
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
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>This field has been added, and shows the number of minutes of work per day that you need to do. It has the format <code>YYYY-MM-DD: (number of minutes)</code>, and takes timezone into account.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>This action added the field <code>teamIDs</code> to support the functionality of assigning multiple teams to a task or issue.</p>
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
            <p>This field was added, and represents the sum of all Budgeted Hours on the project.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Rate (RATE)

A Rate object represents a billing rate in Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>These parameters have been moved to the Rate object from the Role object, so that Role and User objects can have multiple values (for separate date ranges).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>These parameters represent the ID and the object code of the object that the Rate is attached to.
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>This action has been added, and attaches Rate objects to the given Object. This endpoint works for all Rate Attachable objects.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHNOTE)

A RichTextNote object is a comment or update made on a Workfront object, that includes rich text such as bold or italicized text.

The RichTextNote object removed the flag `REPORTABLE`.

### Role / Job Role (ROLE)

A Role object (job role) represents a functional capacity or a skill set a user might fill, such as Designer or Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
           <li>
            <p><b>rates</b>
            </p>
            <p>This has been added, and represents the Rate objects attached to this role.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Task (TASK)

A Task object represents a work item that must be performed as a step toward achieving a final goal (completing a Project).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>This field has been added, and shows the number of minutes of work per day that you need to do. It has the format <code>YYYY-MM-DD: (number of minutes)</code>, and takes timezone into account.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>This action added the field <code>teamIDs</code> to support the functionality of assigning multiple teams to a task or issue.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### Timesheet (TSHET)

A Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct Fields</td>
      <td>
        <ul>
           <li>
            <p><b>availableActions</b>
            </p>
            <p>This parameter removed the flag <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>This parameter removed the flag <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>This parameter was added, and stores the timesheets duration in days regardless of changes to "Equivalent Hours for Full Workday."  For example, if Equivalent Hours is set to 6, and one day is logged, then Equivalent Hours is changed to 8 hours, <code>totalDays</code> still has a value of 1.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / Filter (UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>This action was added, and takes a filter query map and adds the <code>allowingnull</code> join for nullable fields.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>These actions support the ability to share filters, views, and groupings system-wide.</p><p>For more information, see <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Make filters, views, or groupings available to all users</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Grouping (UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>These actions support the ability to share filters, views, and groupings system-wide.</p><p>For more information, see <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Make filters, views, or groupings available to all users</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView / View (UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>Added the following possible value:</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">actions</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>These actions support the ability to share filters, views, and groupings system-wide.</p><p>For more information, see <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Make filters, views, or groupings available to all users</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### User (USER)

A User object represents a person with an account in Workfront that can log in and interact with the system.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
           <li>
            <p><b>rates</b>
            </p>
            <p>This has been added, and represents the Rate objects attached to this user.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

A UserNote object is a notification.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Queries</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>Added the following possible value:
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Work (WORK)

A Work object is a common interface that both Task and OpTask inherit, and shares common code between the two.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>This field has been added, and shows the number of minutes of work per day that you need to do. It has the format <code>YYYY-MM-DD: (number of minutes)</code>, and takes timezone into account.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
