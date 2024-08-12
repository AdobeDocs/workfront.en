---
title: Audit Logs
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: As an Adobe Workfront administrator, you can track user-changes triggered in the system during the past 90 days using audit logs.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
---
# Audit logs

<!--Audited: 01/2024-->

As an Adobe Workfront administrator, you can track user-changes triggered in the system during the past 90 days using the audit logs described below.

For instructions on viewing and filtering what you want to see in these audit logs, see [View and export audit logs](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Information you can find in an audit log

The following fields are recorded in every audit log entry:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Date and Time</td> 
   <td>When the action occurred.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Log Type</td> 
   <td>Type of the audit log, such as Access Level or Custom Form.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">User Name</td> 
   <td> <p>Name of the user who performed the action.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Action</td> 
   <td> Actions performed by the user, such as Change, Create, and Delete. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object</td> 
   <td> Name of the object affected as a result of the action. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Details</td> 
   <td>Additional details about the action. Mouse over the text to read the full message.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">IP Address</td> 
   <td> <p>IP address of the user who performed the action at the time of the action.</p> <p>The IP address is not available for some system actions.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Audit log types and the actions that trigger them

* [Access Level](#access-level) 
* [Company](#company) 
* [Condition](#condition) 
* [Custom Field](#custom-field) 
* [Custom Forms](#custom-forms) 
* [Custom Section](#custom-section) 
* [Exchange Rate](#exchange-rate) 
* [Group](#group) 
* [Job Roles](#job-roles) 
* [Login Attempt](#login-attempt) 
* [Priority](#priority) 
* [Project Preference](#project-preference) 
* [Severity](#severity) 
* [Status](#status) 
* [Tasks & Issues Preferences](#tasks-issues-preferences) 
* [User](#user)

### Access Level {#access-level}

The system generates an Access Level log entry when a user does one of the following actions:

* Creates an access level
* Deletes an access level
* Changes an access level:

   * Modifies the license type
   * Changes permissions to Projects, Tasks, Issues, Portfolios, Programs, Reports, Documents, Users, or Templates

     >[!NOTE]
     >
     >The system does not record any permission changes to Financial Data or within the following access types: View and Edit.
     >
     >For example, if a user changes the Planner access type from View to Edit, the system does not display information contained in the Fine-tune your settings drop-down menu.

### Company {#company}

The system generates a Company audit log entry when a user does one of the following:

* Creates a company
* Changes a company:

   * Renames it
   * Adds or removes members
   * Adds, edits, or deletes the value in its Group field
   * Adds or edits a company billing rate for a job role
   * Removes a company billing rate for a job role
   * Sets it as the primary company for the organization
   * Attaches or removes a custom form

* Deletes a company

For more information about statuses, see [Statuses overview](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Condition {#condition}

The system generates a Condition audit log entry when a user does one of the following actions:

* Creates a condition
* Changes a condition:

   * Changes the name
   * Changes the color
   * Sets it as the default
   * Changes or removes the description of the condition
   * Hides or shows the condition

* Deletes a condition

For more information about configuring job roles, see [Create or edit a custom condition](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Custom Field {#custom-field}

The system generates a Custom Field audit log entry when a user does one of the following actions:

* Creates a custom field
* Changes a custom field:

   * Changes the name, label, instructions, or format
   * Changes the display type

     This is available only if the field is a one of the following types: single line, paragraph, drop-down, checkbox, radio button
   
   * Changes the field size

     This is available only if the field is a one of the following types: single line, paragraph, text with formatting
   
   * Adds, removes, or hides a field choice
   * Edits a field choice label or value
   * Configures the field choice to be selected or not selected by default
   * Configures a drop-down field to allow multiple selections or a single selection
   * Configures a date field to display or not display the time of day
   * Edits the hyperlink or changes the value in a descriptive text field

* Deletes a custom field
* Shares a custom field

### Custom Forms {#custom-forms}

The system generates a Custom Forms audit log entry when a user does one of the following actions:

* Creates a custom form
* Changes a custom form:

   * Changes the name or description
   * Enables or disables Is Active 
   * Adds or removes a field or section
   * For a custom section, changes a setting under Additional settings
   * Changes a field to required or not required
   * Changes a calculation in a custom field
   * Hides or displays the formula associated with a calculated field in the Instructions hover text
   * Enables or disables Update previous calculations
   * Adds or changes skip logic or display logic

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Deletes a custom form
* Shares a custom form

### Custom Section {#custom-section}

The system generates a Custom Section audit log entry when a user does one of the following actions in a custom form:

* Creates a custom section
* Changes the name or description of a custom section
* Deletes a custom section

For information about custom sections in custom forms, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Exchange Rate {#exchange-rate}

The system generates an Exchange Rate audit log entry when a user does one of the following actions:

* Creates an exchange rate
* Changes an exchange rate:

   * Adds a currency
   * Changes the rate for the currency
   * Sets the currency as the base (default) currency for all projects and reports throughout the system

* Deletes an exchange rate

For more information about configuring exchange rates, see [Set up exchange rates](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Group {#group}

The system generates a Group audit log entry when a user does one of the following actions:

* Creates a group
* Deletes a group
* Changes a group:

   * Adds or removes users
   * Adds or removes subgroups

### Job Roles {#job-roles}

The system generates a Job Roles audit log entry when a user does one of the following actions:

* Creates a job role
* Changes a job role:

   * Changes the name
   * Adds, changes, or removes the description
   * Adds, changes, or removes the cost per hour (Cost/Hr.)
   * Adds, changes, or removes the billing rate (Bill/Hr.)

* Deletes a job role

For more information about configuring job roles, see [Create and manage job roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Login Attempt {#login-attempt}

The system generates a Login Attempt audit log entry when a user does one of the following actions:

* Logs in, logs out, or fails a login attempt in Workfront (in a browser and in the mobile app)
* Logs in, logs out, or fails a login attempt in any Workfront integration (such as Workfront for Slack and Workfront for Salesforce)
* Logs in or logs out of the Workfront API

Login Attempt Logs do not record when a Workfront administrator uses the Log In As feature.

>[!NOTE]
>
>This is not available if your organization has been onboarded to the Adobe Admin Console. See your network or IT administrator if you need more information.

### Priority {#priority}

The system generates a Priority audit log entry when a user does one of the following actions:

* Creates a priority
* Changes a priority:

   * Changes the name
   * Changes the color
   * Sets it as the default
   * Adds, changes, or removes the description of the priority
   * Hides or shows the priority

* Deletes a priority

For more information about configuring priorities, see [Create and customize priorities](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Project Preference {#project-preference}

The system generates a Project Preferences audit log entry when a user does one of the following actions:

* Creates a custom quarter
* Changes a project preference:

   * Locks or unlocks it
   * Changes one of its settings
   * Enables, disables, or edits it
   * Edits a timeline calculation

* Deletes a custom quarter

For more information about project preferences, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Severity {#severity}

The system generates a Severity audit log entry when a user does one of the following actions:

* Creates an issue severity
* Changes an issue severity:

   * Changes the name
   * Changes the color
   * Sets it as the default
   * Changes or removes the description of the severity
   * Hides or shows the severity

* Deletes an issue severity

For more information about configuring job roles, see [Create or customize issue severities](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Status {#status}

The system generates a Status audit log entry when a user does one of the following actions:

* Creates a status on the system or group level
* Changes a status on the system or group level:

   * Renames it
   * Makes it a default status
   * Locks or unlocks it
   * Hides or unhides it
   * Changes the color or description

* Deletes a status on the system or group level

For more information about statuses, see [Statuses overview](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Tasks & Issues Preferences {#tasks-issues-preferences}

The system generates a Tasks & Issues Preferences audit log entry when a user changes a Tasks & Issues preference in one of the following ways:

* Locks or unlocks a preference
* Changes the setting for a preference
* Changes an Access setting for tasks, issues, or requests

For more information about task and issue preferences, see [Configure system-wide task and issue preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### User {#user}

The system generates a User audit log entry when a user does one of the following actions:

* Creates a user

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >This is not available if your organization has been onboarded to the Adobe Admin Console. See your network or IT administrator if you need more information.

* Deletes a user
* Changes a user's access level, company, team, or group
* Activates a user
* Deactivates a user
