---
content-type: api
navigation-topic: api-navigation-topic
title: What's new in API version 19
description: Adobe Workfront released API version 19 on April 6, 2022. API version 19 features the following changes from version 18.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
---
# What's new in API version 19

Adobe Workfront released API version 19 on April 8, 2024. API version 19 features the following changes from version 18.

## Added resources

No resources were added for API version 19.

## Removed resources

No resources were removed for API version 19

## Modified resources

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestrictions</b><p>Added the following possible values:
            </p>
            <ul>
              <li>
                <p>Disable the Workfront AI Assistant (AIOFF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Assignment (ASSGN)

An Assignment object represents the connection between a work item and the user, team, or group that is assigned to work on it.

The Assignment object added the flag **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>Added the following direct fields:
        <ul>
          <li>
            <p><b>categoryID</b><p>A category is a custom form.
            </p>
          </li>
          <li>
            <p><b>priority</b><p>This field allows the following values:
            <ul>
              <li>0 (None)</li>
              <li>1 (Low)</li>
              <li>2 (Normal)</li>
              <li>3 (High)</li>
              <li>4 (Urgent)</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>Added the following reference fields:
        <ul>
          <li>
            <p><b>category</b><p>A category is a custom form.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>Added the following collection fields:
        <ul>
          <li>
            <p><b>objectCategories</b><p>A category is a custom form.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### Category (CTGY)

A Category object is a custom form.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b><p>Added the following possible values:
            </p>
            <ul>
              <li>
                <p>Assignment (ASSGN)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objTypes</b><p>Added the following possible values:
            </p>
            <ul>
              <li>
                <p>Assignment (ASSGN)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Classifier (CLSF)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Actions</td>
      <td>Added the following actions
        <ul>
          <li>
            <p><b>activateClassifiers</b><p</p>
          </li>
          <li>
            <p><b>deactivateClassifiers</b><p></p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### Customer

A Customer object represents an organization that uses an instance of Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumTypes</b><p>Added the following possible values:
            </p>
            <ul>
              <li>
                <p>Assignment Priorities (PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>The CustomEnum object aids with converting status codes into human-readable text.</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### CustomerPreferences (CUSTPR)

A CustomerPreferences object represents the set of preferences that a customer has set for their instance of Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>name</b><p>removed the following possible values:
            </p>
            <ul>
              <li>
                <p>Enable Zoom integration in the updates stream (password:zoomIntegrationEnabled)
                </p>
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



### ExchangeRate (EXRATE)

An ExchangeRate object represents a currency exchange rate set up in Workfront. ExchangeRate objects are not dynamic.



### Hour (HOUR)

An Hour object represents an hour logged by a user on a timesheet.



### JournalEntry (JRNLE)

The JournalEntry object can be set up to log information about specific object fields any time those fields are modified. When a field is set up to be logged as a part of the Journal Entry object, a corresponding Journal Entry will be created every time that field is modified.



### Parameter

A Parameter object is a custom field.



### Role (ROLE)

A Role object (job role) represents a functional capacity or a skill set a user might fill, such as Designer or Product Manager.



### TemplateAssignment (TASSGN)

A TemplateAssignment object represents the connection between a template task and the user, team, or group that is assigned to work on it. When the template is used for a project, that user, team, or group is assigned to the task.

### Timesheet (TSHET)

A Timesheet object represents a virtual timecard that allows Users to enter actual hours worked for Tasks, Projects, and overhead Hour Types.




