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



### Category (CTGY)

A Category object is a custom form.



### Company (CMPY)

A Company object represents an organization consisting of a collection of people.



### Customer (CUST)

A Customer object represents an organization that uses an instance of Workfront.



### CustomerPreferences (CUSTPR)

A CustomerPreferences object represents the set of preferences that a customer has set for their instance of Workfront.



### DocumentFolder (DOCFDR)

Documents can be organized into folders. You can create personal folders in your personal Documents area. The DocumentFolder object represents one of these folders.



### DocumentVersion (DOCV)

A DocumentVersion object represents a specific version of a file (such as written material, images, or other forms of information).



### ExchangeRate (EXRATE)

An ExchangeRate object represents a currency exchange rate set up in Workfront. ExchangeRate objects are not dynamic.



### JournalEntry (JRNLE)

The JournalEntry object can be set up to log information about specific object fields any time those fields are modified. When a field is set up to be logged as a part of the Journal Entry object, a corresponding Journal Entry will be created every time that field is modified.



### JournalField



### OriginalRequest



### Parameter (PARAM)

A Parameter object is a custom field.



### ParameterGroup



### PortalSection



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







