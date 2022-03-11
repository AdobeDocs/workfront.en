---
filename: update-users-SSO
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Update users for single sign-on
description: The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
---

# Update users for single sign-on

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that are not yet onboarded to the Adobe Admin Console.
>
>If your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

When single sign-on (SSO) is enabled in your `Adobe Workfront` instance, you can log into `Workfront` with your SSO credentials.

If you have an existing system that is already populated with users associated with SSO credentials, you can import the users' IDs into `Workfront` by importing a comma-separated values (CSV) file into `Workfront`.

For more information about integrating `Workfront` with an SSO system, see [Overview of single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>This is not available if your organization’s `Workfront` instance is enabled with Adobe IMS. See your network or IT administrator if you need more information.

##  

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <span>Workfront administrator</span>. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## SSO usernames

Depending on what SSO solution you use, the username in your SSO environment can be called any of the following:

* SSO Username
* Federation ID 
* Federation Username
* LDAP Username
* AD Username
* Active Directory Username

In `Workfront`, all these names are stored in the SSO Username field, on the user object.

In order for your users to be able to use their SSO credentials to log in to `Workfront`, you must update their profile to include their SSO Username, in addition to their `Workfront` username.

As a `Workfront administrator`, you can bulk update the SSO Username field for your `Workfront` users by using a list of usernames and importing it in `Workfront`. This list must contain the `Workfront` User ID (GUID) as well as the corresponding SSO Username for each user and it must be saved as a CSV or a TSV file. This process either updates existing SSO Usernames in `Workfront`, or adds a new SSO Username, if one is missing for users.

## Prepare the import file

You can start preparing your import file by building a report of all users in `Workfront` that must have their SSO Username fields updated.

<ol> 
 <li value="1"> <p>Build a user report in <span>Workfront</span>.</p> <p>For instructions on building user reports in <span>Workfront</span>, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. </p> </li> 
 <li value="2"> <p>Select the following fields in your report:</p> <p> <img src="assets/users-with-sso-username-and-no-sso-access-only-field-350x47.png" style="width: 350;height: 47;"> </p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Name</td> 
     <td>The full name of the <span>Workfront</span> user.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">ID</td> 
     <td>The ID is the <span>Workfront</span> alphanumeric GUID.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">SSO Username</td> 
     <td>Select the SSO Username field to ensure there are no usernames you are overwriting with your import. This field should be blank for all users, if your users have not yet been updated for SSO.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="3">Save the report. </li> 
 <li value="4">Click <span class="bold">Export</span> at the top of the report and export the report to Excel. </li> 
 <li value="5"> <p>Open the exported Excel file, and start adding your SSO Usernames for each user in the report in the SSO Username column.</p> <note type="important">
   SSO usernames are case-sensitive. 
  </note> </li> 
 <li value="6">Eliminate all columns in the Excel file, except for the <span class="bold">ID</span> and the <span class="bold">SSO Username</span> columns. </li> 
 <li value="7"> <p>Eliminate the column headers and ensure there are no blank rows at the top of the report. </p> <p>The file you are using for updating your <span>Workfront</span> users with the SSO usernames must contain just 2 columns, in this order:</p> 
  <ul> 
   <li>The first column should display the <span>Workfront</span> user ID (the user GUID as found in <span>Workfront</span>).</li> 
   <li>The second column should contain the SSO Username, as it displays in your SSO system.</li> 
   <li> <p>The columns should have no headers, and there should not be any empty rows at the top of the list of names.</p> <p> <img src="assets/update-users-for-sso-csv-file-for-import-350x47.png" alt="" style="width: 350;height: 47;"> </p> </li> 
  </ul> </li> 
 <li value="8">Save the report as a CSV or TSV file on your computer.</li> 
</ol>

## Update your users for SSO

The process of updating users for SSO either adds the SSO Username field to your `Workfront` users if one is not present, or updates the value in that field if there is a value already associated with the users.

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span>Adobe Workfront</span>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">Click <span class="bold">System</span> then <span class="bold">Update Users For SSO</span>.</li> 
 <li value="3"> <p>Click <span class="bold">Choose File</span> to browse for the file you prepared.</p> <p>For more information about how to prepare this file, see <a href="#preparing-the-import-file" class="MCXref xref">Prepare the import file</a>.</p> </li> 
 <li value="4"> <p>Select the file where it is saved on your computer, then click <b>Open</b>.</p> <p>This enables all users to log in to <span>Workfront</span> using their SSO credentials. </p> <p>The <span class="bold">Only Allow <SSO Configuration> Authentication</span> setting is enabled for all users included in the CSV. For more information about user settings, see <a href="#" class="MCXref xref selected">Update users for single sign-on</a>.</p> </li> 
</ol>

## Verify SSO your users' `Workfront` usernames

For instructions on building a user report containing SSO Username information, see [Prepare the import file](#preparing-the-import-file).

<ol> 
 <li value="1"> <p>Run a user report containing SSO Username information.</p> <p>Notice that the SSO Username column is populated for each user.</p> </li> 
 <li value="2">Ensure that the values for the SSO Username column match the SSO Username on your SSO server.</li> 
 <li value="3"> <p>If the SSO Username column is blank, update your users' SSO Usernames. </p> <p> <img src="assets/users-with-sso-field-updated-350x45.png" alt="" style="width: 350;height: 45;"> </p> <p>For instructions on updating your users for SSO, see <a href="#updating-users-for-sso" class="MCXref xref">Update your users for SSO</a>.</p> </li> 
</ol>

