---
filename: audit-logs
title: Audit logs
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Audit logs
description: As an Adobe Workfront administrator, you can track user-changes triggered in the system during the past 90 days using the audit logs described below.
---

# Audit logs

As an `Adobe Workfront administrator`, you can track user-changes triggered in the system during the past 90 days using the audit logs described below.

For instructions on viewing and filtering what you want to see in these audit logs, see [View and export audit logs](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Information you can find in an audit log

The following fields are recorded in every audit log entry:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Date &amp; Time</td> 
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
   <td> Action performed by the user, such as Change, Create, and Delete. </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span class="bold">Object</span> </td> 
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

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Access Level</td> 
   <td> <p>The system generates an Access Level log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates an access level</li> 
     <li>Deletes an access level</li> 
     <li>Changes an access level:
      <ul>
       <li>Modifies the license type</li>
       <li><p>Changes permissions to Projects, Tasks, Issues, Portfolios, Programs, Reports, Documents, Users, or Templates</p><p>Note: <p>The system does not record any permission changes to&nbsp;Financial Data or within the following access types: View and Edit.<br></p><p>For example, if a user changes the Planner access type from View to Edit, the system will not display information contained in the Fine-tune your settings drop-down menu.</p></p></li>
      </ul></li> 
    </ul> </td> 
  </tr> Company The system generates a Company audit log entry when a user does one of the following: Creates a company Changes a company: Renames it Adds or removes members Adds, edits, or deletes the value in its Group field Adds or edits a company billing rate for a job role Removes a company billing rate for a job role Sets it as the primary company for the organization Attaches or removes a custom form Deletes a company For more information about statuses, see Statuses overview. 
  <tr> 
   <td role="rowheader">Condition</td> 
   <td> <p>The system generates a Condition audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates a condition</li> 
     <li>Changes a condition:
      <ul>
       <li>Changes the name</li>
       <li>Changes the color</li>
       <li>Sets it as the default</li>
       <li>Changes or removes the description of the condition</li>
       <li>Hides or shows the condition</li>
      </ul></li> 
     <li>Deletes a condition</li> 
    </ul> <p>For more information about configuring job roles, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md" class="MCXref xref">Create or edit a custom condition</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Custom Field</td> 
   <td> <p>The system generates a Custom Field audit audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates a custom field</li> 
     <li>Changes a custom field:
      <ul>
       <li>Changes the name, label, instructions, or format</li>
       <li><p>Changes the display type</p><p>This is available only if the field is a one of the following types: single line, paragraph, drop-down, checkbox, radio button</p></li>
       <li><p>Changes the field size</p><p>This is available only if the field is a one of the following types: single line, paragraph, text with formatting</p></li>
       <li>Adds, removes, or hides a field choice</li>
       <li>Edits a field choice label or value</li>
       <li>Configures the field choice to be selected or not selected by default</li>
       <li>Configures a drop-down field to allow multiple selections or a single selection</li>
       <li>Configures a date field to display or not display the time of day</li>
       <li>Edits the hyperlink or changes the value in a descriptive text field</li>
      </ul></li> 
     <li>Deletes a custom field</li> 
     <li>Shares a custom field</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Custom Forms</td> 
   <td> <p>The system generates a Custom Forms audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates a custom form</li> 
     <li>Changes a custom form:
      <ul>
       <li>Changes the name or description</li>
       <li>Enables or disables Is Active </li>
       <li>Adds or removes a field or section</li>
       <li><p>For a custom section, changes a setting under Additional settings</p></li>
       <li><p>Changes a field to required or not required</p></li>
       <li><p>Changes a calculation in a custom field</p></li>
       <li><p>Hides or displays the formula associated with a calculated field in the Instructions hover text</p></li>
       <li><p>Enables or disables Update previous calculations</p></li>
       <li><p>Adds or changes skip logic or display logic</p></li><!--
        Adds or changes a filter for a typeahead field
       -->
      </ul></li> 
     <li>Deletes a custom form</li> 
     <li>Shares a custom form</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Custom Section</td> 
   <td> <p>The system generates a Custom Section audit log entry when a user does one of the following actions in a custom form:</p> 
    <ul> 
     <li>Creates a custom section</li> 
     <li>Changes the name or description of a custom section</li> 
     <li>Deletes a custom section</li> 
    </ul> <p>For information about custom sections in custom forms, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Exchange Rate</td> 
   <td> <p>The system generates an Exchange Rate audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates an exchange rate</li> 
     <li>Changes an exchange rate:
      <ul>
       <li>Adds a currency</li>
       <li>Changes the rate for the currency</li>
       <li>Sets the currency as the base (default) currency for all projects and reports throughout the system</li>
      </ul></li> 
     <li>Deletes an exchange rate</li> 
    </ul> <p>For more information about configuring exchange rates, see <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Group</td> 
   <td> <p>The system generates a Group audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates a group</li> 
     <li>Deletes a group</li> 
     <li>Changes a group:
      <ul>
       <li>Adds or removes users</li>
       <li>Adds or removes subgroups</li>
      </ul></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Job Roles</td> 
   <td> <p>The system generates a Job Roles audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates a job role</li> 
     <li>Changes a job role:
      <ul>
       <li>Changes the name</li>
       <li>Adds, changes, or removes the description</li>
       <li>Adds, changes, or removes the cost per hour (Cost/Hr.)</li>
       <li>Adds, changes, or removes the billing rate (Bill/Hr.)</li>
      </ul></li> 
     <li>Deletes a job role</li> 
    </ul> <p>For more information about configuring job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Login Attempt</td> 
   <td> <p>The system generates a Login Attempt audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Logs in, logs out, or fails a login attempt in <span>Workfront</span> (in a browser and in the mobile app)</li> 
     <li>Logs in, logs out, or fails a login attempt in any <span>Workfront</span> integration (such as <span>Workfront for Slack</span> and <span>Workfront for Salesforce</span>)</li> 
     <li> <p>Logs in or logs out of the Workfront API</p> </li> 
    </ul> <p>Login Attempt Logs do not record when a <span>Workfront administrator</span> uses the Log In As feature.</p> <p>Note: This is not available if your organization’s <span>Workfront</span> instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Priority</td> 
   <td> <p>The system generates a Priority audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates a priority</li> 
     <li>Changes a priority:
      <ul>
       <li>Changes the name</li>
       <li>Changes the color</li>
       <li>Sets it as the default</li>
       <li>Adds, changes, or removes the description of the priority</li>
       <li>Hides or shows the priority</li>
      </ul></li> 
     <li>Deletes a priority</li> 
    </ul> <p>For more information about configuring priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities-.md" class="MCXref xref">Create and customize priorities</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project Preferences</td> 
   <td> <p>The system generates a Project Preferences audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates a custom quarter</li> 
     <li>Changes a project preference:
      <ul>
       <li>Locks or unlocks it</li>
       <li>Changes one of its settings</li>
       <li>Enables, disables, or edits it</li>
       <li>Edits a timeline calculation</li>
      </ul></li> 
     <li>Deletes a custom quarter</li> 
    </ul> <p>For more information about project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Severity</td> 
   <td> <p>The system generates a Severity audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates an issue severity</li> 
     <li>Changes an issue severity:
      <ul>
       <li>Changes the name</li>
       <li>Changes the color</li>
       <li>Sets it as the default</li>
       <li>Changes or removes the description of the severity</li>
       <li>Hides or shows the severity</li>
      </ul></li> 
     <li>Deletes an issue severity</li> 
    </ul> <p>For more information about configuring job roles, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">Create and customize issue severities</a>.</p> </td> 
  </tr> Status The system generates a Status audit log entry when a user does one of the following actions: Creates a status on the system or group level Changes a status on the system or group level: Renames it Makes it a default status Locks or unlocks it Hides or unhides it Changes the color or description Deletes a status on the system or group level For more information about statuses, see Statuses overview. 
  <tr> 
   <td role="rowheader">Tasks &amp; Issues Preferences</td> 
   <td> <p>The system generates a Tasks &amp; Issues Preferences audit log entry when a user changes a Tasks &amp; Issues preference in one of the following ways:</p> 
    <ul> 
     <li>Locks or unlocks a preference</li> 
     <li>Changes the setting for a preference</li> 
     <li>Changes an Access setting for tasks, issues, or requests</li> 
    </ul> <p>For more information about task and issue preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">User</td> 
   <td> <p>The system generates a User audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li> <p>Creates a user<!--
        Gevorg checking with Jonah on whether this note should be here:
       --></p> <p>Note: This is not available if your organization’s <span>Workfront</span> instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.</p> </li> 
     <li>Deletes a user</li> 
     <li>Changes a user's access level, company, team, or group</li> 
     <li>Activates a user</li> 
     <li>Deactivates a user</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

