---
filename: audit-logs
title: Audit logs
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
---



# Audit logs {#audit-logs}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


As an *`Adobe Workfront administrator`*, you can track user-triggered changes in the system using the audit logs described below.


For instructions on viewing and filtering what you want to see in these audit logs, see [View and export audit logs](view-and-export-audit-logs.md).


>[!NOTE]
>
>This is not available if your organization’s *`Workfront`* instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.




## Information you can find in an audit log {#information-you-can-find-in-an-audit-log}

The following fields are recorded in every audit log entry:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Date &amp; Time</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">When the action occurred.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Log Type</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Type of the audit log, such as Access Level or Custom Form.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">User Name</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Name of the user who performed the action.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Action</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> Action performed by the user, such as Change, Create, and Delete. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Object</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> Name of the object affected as a result of the action. </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Details</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Additional details about the action. Mouse over the text to read the full message.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">IP Address</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>IP address of the user who performed the action at the time of the action.</p> <p>The IP address is not available for some system actions.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Audit log types and the actions that trigger them {#audit-log-types-and-the-actions-that-trigger-them}


<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Access Level</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The system generates an Access Level log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates an access level</li> 
     <li>Deletes an access level</li> 
     <li>Changes an access level:
      <ul>
       <li>Modifies the license type</li>
       <li><p>Changes permissions to Projects, Tasks, Issues, Portfolios, Programs, Reports, Documents, Users, or Templates</p><p>Note: <p>The system does not record any permission changes to&nbsp;Financial Data or within the following access types: View and Edit.<br></p><p>For example, if a user changes the Planner access type from View to Edit, the system will not display information contained in the Fine-tune your settings drop-down menu.</p></p></li>
      </ul></li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="preview">Company</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <div class="preview"> 
     <p>The system generates a Company audit log entry when a user does one of the following:</p> 
     <ul> 
      <li> <p>Creates a company</p> </li> 
      <li> <p>Changes a company:</p> 
       <ul> 
        <li>Renames it</li> 
        <li>Adds or removes members</li> 
        <li>Adds, edits, or deletes the value in its Group field </li> 
        <li>Adds or edits a company billing rate for a job role</li> 
        <li>Removes a company billing rate for a job role</li> 
        <li> Sets it as the primary company for the organization</li> 
        <li>Attaches or removes a custom form</li> 
       </ul> </li> 
      <li>Deletes a company</li> 
     </ul> 
     <p>For more information about statuses, see <a href="statuses-overview.md" class="MCXref xref">Statuses overview</a>.</p> 
    </div> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Condition</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The system generates a Condition audit log entry when a user does one of the following actions:</p> 
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
    </ul> <p>For more information about configuring job roles, see <a href="create-edit-custom-conditions.md" class="MCXref xref">Create or edit a custom condition</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Custom Field</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>The system generates a Custom Field audit audit log entry when a user does one of the following actions:</p> 
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
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Custom Forms</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The system generates a Custom Forms audit log entry when a user does one of the following actions:</p> 
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
       <li class="preview"><p>Hides or displays the formula associated with a calculated field in the Instructions hover text</p></li>
       <li><p>Enables or disables Update previous calculations</p></li>
       <li><p>Adds or changes skip logic or display logic</p></li>
      </ul></li> 
     <li>Deletes a custom form</li> 
     <li>Shares a custom form</li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Custom Section</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>The system generates a Custom Section audit log entry when a user does one of the following actions in a custom form:</p> 
    <ul> 
     <li>Creates a custom section</li> 
     <li>Changes the name or description of a custom section</li> 
     <li>Deletes a custom section</li> 
    </ul> <p>For information about custom sections in custom forms, see <a href="create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Exchange Rate</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The system generates an Exchange Rate audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates an exchange rate</li> 
     <li>Changes an exchange rate:
      <ul>
       <li>Adds a currency</li>
       <li>Changes the rate for the currency</li>
       <li>Sets the currency as the base (default) currency for all projects and reports throughout the system</li>
      </ul></li> 
     <li>Deletes an exchange rate</li> 
    </ul> <p>For more information about configuring exchange rates, see <a href="set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Group</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>The system generates a Group audit log entry when a user does one of the following actions:</p> 
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
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Job Roles</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The system generates a Job Roles audit log entry when a user does one of the following actions:</p> 
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
    </ul> <p>For more information about configuring job roles, see <a href="create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Login Attempt</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>The system generates a Login Attempt audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Logs in, logs out, or fails a login attempt in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> (in a browser and in the mobile app)</li> 
     <li>Logs in, logs out, or fails a login attempt in any <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> integration (such as <span class="mc-variable WFVariables.Integration-SL variable varname">Workfront for Slack</span> and <span class="mc-variable WFVariables.Integration-SF variable varname">Workfront for Salesforce</span>)</li> 
     <li> <p>Logs in or logs out of the Workfront API</p> </li> 
    </ul> <p>Login Attempt Logs do not record when a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> uses the Log In As feature.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Priority</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The system generates a Priority audit log entry when a user does one of the following actions:</p> 
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
    </ul> <p>For more information about configuring priorities, see <a href="create-customize-priorities .md" class="MCXref xref">Create and customize priorities</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Project Preferences</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>The system generates a Project Preferences audit log entry when a user does one of the following actions:</p> 
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
    </ul> <p>For more information about project preferences, see <a href="set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Severity</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The system generates a Severity audit log entry when a user does one of the following actions:</p> 
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
    </ul> <p>For more information about configuring job roles, see <a href="create-customize-issue-severities.md" class="MCXref xref">Create and customize issue severities</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="preview">Status</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <div class="preview"> 
     <p>The system generates a Status audit log entry when a user does one of the following actions:</p> 
     <ul> 
      <li>Creates a status on the system or group level</li> 
      <li>Changes a status on the system or group level:
       <ul>
        <li>Renames it</li>
        <li>Makes it a default status</li>
        <li>Locks or unlocks it</li>
        <li>Hides or unhides it</li>
        <li>Changes the color or description </li>
       </ul></li> 
      <li>Deletes a status on the system or group level</li> 
     </ul> 
     <p>For more information about statuses, see <a href="statuses-overview.md" class="MCXref xref">Statuses overview</a>.</p> 
    </div> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Tasks &amp; Issues Preferences</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>The system generates a Tasks &amp; Issues Preferences audit log entry when a user changes a Tasks &amp; Issues preference in one of the following ways:</p> 
    <ul> 
     <li>Locks or unlocks a preference</li> 
     <li>Changes the setting for a preference</li> 
     <li>Changes an Access setting for tasks, issues, or requests</li> 
    </ul> <p>For more information about task and issue preferences, see <a href="set-task-issue-preferences.md" class="MCXref xref">Configure system-wide task and issue preferences</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">User</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>The system generates a User audit log entry when a user does one of the following actions:</p> 
    <ul> 
     <li>Creates a user</li> 
     <li>Deletes a user</li> 
     <li>Changes a user's access level, company, team, or group</li> 
     <li>Activates a user</li> 
     <li>Deactivates a user</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

