---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 22
description: Adobe Workfront released API version 22 on May 11, 2026. API version 22 features the following changes from version 21.
author: Becky
feature: Workfront API
role: Developer
---
# What's new in API version 22

Adobe Workfront released API version 22 on May 8, 2026. API version 22 features the following changes from version 21.

## Added resources

The following resources were added for API version 22.

### ReportShareableFolder (RPSHFD)

You can use shareable report folders to organize reports and share those folders with other users. This feature is designed for teams that manage large volumes of reports and need scalable, consistent access control.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>name</li>
        </ul>
      </td>
    </tr>
   <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>DELETE</li>
          <li>EDIT</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## Removed resources

The following resources were removed from API version 22.

### UserLocation (USRLOC)

This object has been removed.

## Modified resources

The following resources were modified for API version 22.

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following field has been modified with changes to possible values. For details, see the developer documentation.
        <ul>
          <li><b>fieldAccessPrivileges</b></li>
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
      <td>The following fields have been modified with changes to possible values. For details, see the developer documentation.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>The following field has been modified with changes to possible values. For details, see the developer documentation.
        <ul>
          <li><b>action</b></li>
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
      <td>The following fields have been modified with changes to possible values. For details, see the developer documentation.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>The following fields were added to support Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>The following field has been added.
        <ul>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### Company (CMPY)

A Company object represents an organization consisting of a collection of people.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following fields were added to support Enterprise Storage Management.
        <ul>
          <li><b>esmProjectID</b></li>
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
      <td>Added
        <ul>
          <li><p><b>getDefaultAssignmentStatusEnum</b></p></li>
          <li><p><b>getDefaultBookingStatusEnum</b></p></li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Queries</td>
      <td>Added
        <ul>
          <li><p><b>assignmentStatuses</b></p></li>
          <li><p><b>bookingStatuses</b></p></li>
        </ul>
      </td>
    </tr>
</tbody>
</table>

### Customer (CUST)

A Customer object represents an organization that uses an instance of Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following field has been modified.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Added the following possible values.</p>
             <ul>
              <li>
                <p><code>STATUS_BOOKING</code> (Booking Statuses)</p>
              </li>
              <li>
                <p><code>STATUS_ASSIGNMENT</code> (Assignment Statuses)</p>
              </li>
            </ul>
         </li>
         </ul>
         <p>The following fields were added to support Enterprise Storage Management.
         <ul>
         <li><b>isLegacyCustomerEsmStorageEnabled</b></li>
         <li><b>isLegacyCustomerSystemFileMigrationEnabled</b></li>
         <li><b>legacyCustomerEsmStorageMigrationDate</b></li>
         <li><b>legacyCustomerSystemFileMigrationDate</b></li>
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
      <td>The following field has been modified.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Added the following possible values to support Enterprise Storage Management:</p>
             <ul>
              <li>
                <p><code>customer:config.defaultStorageModeAllowOverride</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageMode</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageGroupRollout</code> </p>
              </li>
               <li>
                <p><code>customer:config.defaultStorageGroupOptions</code> </p>
              </li>
             </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>


### Document (DOCU)

A Document object represents a file (such as written material, images, or other forms of information).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following fields were added to support Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmAsset</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>The following action has been modified.
        <ul>
          <li><p><b>createLargeDocument
          </b></p><p>The following fields were added to support Enterprise Storage Management.
         <ul>
         <li><b>docObjCode</b></li>
         <li><b>objID</b></li>
         </ul>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### DocumentFolder (DOCFDR)

Documents can be organized into folders. You can create personal folders in your personal Documents area. The DocumentFolder object represents one of these folders.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following fields were added to support Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmFolder</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

A DocumentVersion object represents a specific version of a file (such as written material, images, or other forms of information).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following field was added to support Enterprise Storage Management.
        <ul>
          <li><b>esmVersionID</b></li>
        </ul>
      The following field has been modified.
        <ul>
          <li><b>version</b><p>Removed the validator "REQUIRED".</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Actions</td>
      <td>The following action has been added.
        <ul>
          <li><p><b>sendToAEMDetails</b></p>
         </li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Operations</td>
      <td>The following operation has been added.
        <ul>
          <li><p><b>EDIT</b></p>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### ExchangeRate (EXRATE)

An ExchangeRate object represents a currency exchange rate set up in Workfront. ExchangeRate objects are not dynamic.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following fields were added.
        <ul>
          <li><b>portfolioID</b></li>
          <li><b>programID
          </b></li>
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
      <td>The following fields have been modified.
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Added the following possible values.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Move folder)</p>
              </li>
              </ul>
         </li>
          <li>
            <p><b>flags</b>
            </p>
            <p>Added the following possible values.</p>
             <ul>
              <li>
                <p><code>CI</code>(enum.journalentryflagenum.iscontactinfoentry)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalField (JRNLF)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following fields have been modified.
        <ul>
          <li>
            <p><b>action</b>
            </p>
            <p>Added the following possible values.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Move folder)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask (OPTASK)

An OpTask object is commonly known as an Issue. An issue is a work item that usually indicates that there is a problem preventing the completion of a task or project. An Issue can also be a Help Desk request. Change Orders, Requests, and Bugs are also Issues.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>actualWorkRequired</b><p>Added the following flags:
           <ul>
           <li><code>AUTO_LOAD</code></li>
           <li><code>DYNAMIC</code></li>
           </ul>
           </p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Search fields</td>
      <td>
        <ul>
          <li><b>actualWork</b><p>Type changed from <code>null</code> to <code>double</code>.</p></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OriginalRequest(ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Operations</td>
      <td>The following operations have been added.
        <ul>
          <li><p><b>COUNT</b></p>
          <li><p><b>GET</b></p>
          <li><p><b>REPORT</b></p>
          <li><p><b>SEARCH</b></p>
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
      <td>The following fields were added.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### ParameterGroup (PGRP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following fields were added.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### PortalSection (PTLSEC)

A PortalSection object is a Report.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following field was added.
        <ul>
          <li><b>reportShareableFolderID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>The following field was added.
        <ul>
          <li><b>reportShareableFolder</b></li>
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
      <td role="rowheader">Direct fields</td>
      <td>The following fields were added to support Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
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
      <td role="rowheader">Direct fields</td>
      <td>The following fields were added to support Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      The following field has been modified.
        <ul>
          <li><b>portfolioID</b><p>Added the validator "REQUIRED".</li>
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
      <td>The following fields were added to support Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### QueueDef (QUED)

A QueueDef object represents a request queue definition in Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following fields have been modified with changes to possible values. For details, see the developer documentation.
        <ul>
          <li><b>requestorCoreAction</b></li>
          <li><b>requestorForbiddenActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScheduledReport (SCHREP)

A ScheduledReport object represents a report that has been configured to be scheduled for delivery.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>The following field has been modified with extensive changes to possible values. For details, see the developer documentation.
        <ul>
          <li><b>format</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Task (TASK)

A Task object represents a work item that must be completed as part of achieving a final goal (completing a project).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><p><b>convertedOpTaskID</b><p>
              <p>Added</p></li>
          <li><p><b>actualWorkRequired</b></p><p>Added flags <code>AUTO_LOAD</code> and <code>DYNAMIC</code>.</p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li>
            <p><b>convertedOpTask</b>
            </p>
            <p>Added</p>
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
      <td role="rowheader">Direct fields</td>
      <td>The following fields were added to support Enterprise Storage Management.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>The following field has been modified.
        <ul>
          <li>
            <p><b>action</b>
            </p>
            <p>Added the following possible value.</p>
             <ul>
              <li>
                <p><code>primaryFolderMoved</code></p>
              </li>
              </ul>
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
      <td role="rowheader">Direct fields</td>
      <td>The following field was added.
        <ul>
          <li><b>eauthUserID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>The following field was removed.
        <ul>
          <li><b>userLocations</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>





