---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 22
description: Adobe Workfront released API version 22 on October 23, 2025. API version 22 features the following changes from version 21.
author: Becky
feature: Workfront API
role: Developer
---
# What's new in API version 22

Adobe Workfront released API version 22 on May 1, 2026. API version 22 features the following changes from version 21.

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
      <td>Added
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
      <td role="rowheader">actions</td>
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
            <p>Added the following possible values:</p>
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
      <td role="rowheader">actions</td>
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
      <td>The following field has been modified.
        <ul>
          <li><b>version</b><p>Removed the validator "REQUIRED".</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### ExchangeRate (EXRATE)

An ExchangeRate object represents a currency exchange rate set up in Workfront. ExchangeRate objects are not dynamic.



### JournalEntry (JRNLE)

The JournalEntry object can be set up to log information about specific object fields any time those fields are modified. When a field is set up to be logged as a part of the Journal Entry object, a corresponding Journal Entry will be created every time that field is modified.



### JournalField (JRNLF)



### OriginalRequest(ORGREQ)



### Parameter (PARAM)

A Parameter object is a custom field.



### ParameterGroup (PGRP)



### PortalSection (PTLSEC)

A PortalSection object is a Report.



### Portfolio (PORT)

A Portfolio object is a collection of projects that compete for the same resources, typically money or people to complete them.



### Program (PRGM)

A Program object is a subset of projects within a portfolio, where similar projects can be grouped together.



### Project (PROJ)

Projects are work items within Workfront, and are a main building block in the way Workfront helps people to do work. A Project object represents a group of tasks with a common, specific goal.



### ScheduledReport (SCHREP)

A ScheduledReport object represents a report that has been configured to be scheduled for delivery.



### Template (TMPL)

A Template object represents a pattern for a project. Projects can be created from templates to save time. A template contains a team and tasks, which will be copied to any project created from the template.



### Update (UPDATE)

Work Items in Workfront can be updated to keep users informed of the current status. An Update object represents one of these updates. Updates can be entered by users or created by the Workfront system.



### User (USER)

A User object represents a person with an account in Workfront that can log in and interact with the system.







