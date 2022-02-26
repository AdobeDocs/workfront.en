---
filename: configure-basic-info
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configure basic information for your system
description: As part of configuring your Adobe Workfront system, you can manage details about your organization in the Basic Info section of your Customer Info page.
---

# Configure basic information for your system

As part of configuring your *Adobe Workfront* system, you can manage details about your organization in the Basic Info section of your Customer Info page.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a <em>Workfront administrator</em>. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Access Customer Info

The customer represents the *Workfront* instance for your organization. The options in this area are unique to you, as a customer of *Workfront*.

To access the Customer Info page:

<ol> 
 <li value="1"><![CDATA[
]]>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.<br></li> 
 <li value="2"> <p>In the left panel, click <span class="bold">System</span> > <span class="bold">Customer Info</span>. </p> <p>Depending on the <em>Workfront</em> plan that you have purchased, some sections might be missing from the Customer Info page. Contact your Account Representative if you need to find out which <em>Workfront</em> plan your organization uses.</p> <p>The sections available in the Customer Info area are:</p> 
  <ul> 
   <li> <p><span class="bold">Basic Info</span> </p> <p>For information&nbsp;about configuring basic information in <em>Workfront</em>, see <a href="#configuring-basic-info" class="MCXref xref">Configure Basic Info</a>.</p> </li> 
   <li> <p><span class="bold">API Key Settings</span> </p> <p>For information about API key settings, see <a href="../../administration-and-setup/manage-workfront/security/manage-api-keys.md" class="MCXref xref">Manage API keys </a>.</p> </li> 
   <li> <p><span class="bold">IP Allowlist</span> </p> <p>For information about adding the IP addresses to your allowlist for where your users can access <em>Workfront</em>, see <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Configure your firewall's allowlist</a>.</p> </li> 
   <li> <p><span class="bold">License</span> </p> <p>For information about licenses, see <a href="../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md" class="MCXref xref">Manage available licenses in your system</a>.</p> </li> 
  </ul> </li> 
</ol>

## Configure Basic Info

Inside the Basic Info area of your Customer Info page, some details about your customer are configured by *Workfront* and they display in a read-only mode. Other details can be configured by you. Any options you can edit in this area have a global effect on all users in *Workfront*.

To&nbsp;configure your Basic Info section in your Customer Info area:

<ol> 
 <li value="1">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Setup</span> <img src="assets/gear-icon-settings.png">.</li> 
 <li value="2">In the left panel, click <span class="bold">System</span> > <span class="bold">Customer Info</span>. </li> 
 <li value="3"> <p>In the <span class="bold">Basic Info</span> section at the top of the <span class="bold">Customer Info</span> page, find the following information about your instance with <em>Workfront</em>:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Name</td> 
     <td>The name of your organization, which also matches the name of your company. This is added by <em>Workfront</em> and it cannot be edited.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Cluster Setup </td> 
     <td>The cluster number for your instance.</td> 
    </tr> 
    <tr> 
     <td role="rowheader"><a name="Admin_Email"></a>Admin Email</td> 
     <td> <p>The email address of your <em>Workfront administrator</em>. You can edit this field to match the email address of one of your <em>Workfront administrators</em>. The user associated with this email address is considered the main <em>Workfront administrator</em> of your <em>Workfront</em> system. Any site-wide communication from <em>Workfront</em> is directed&nbsp;to this email address, so it is important to keep it updated.</p> <note type="note">
        You cannot deactivate, delete, or change the Access Level of the user associated with the Admin Email.
      </note> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Domain</td> 
     <td> <p>The domain is set by <em>Workfront</em> when your account is created.</p> <p>The domain identifies your&nbsp;unique sub-domain of the URL you use to access <em>Workfront</em>.<br>For example, if your organization has been assigned the domain "mycompany," the URL you use to access <em>Workfront</em> is <i>https://mycompany.my.workfront.com</i>.<br>You cannot edit the domain yourself. If you want to change your domain, you can contact <em>Workfront</em> Customer Support. For more information about&nbsp;contacting <em>Workfront</em>&nbsp;Customer Support, see <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Time Zone</td> 
     <td> <p>This is the default time zone of your <em>Workfront</em> instance. You can edit this field to match the time zone of your primary <em>Workfront</em> location. The time zone you select affects the following: </p> 
      <ul> 
       <li>Controls the date and time displayed in outgoing emails. </li> 
       <li>It is selected as the default time zone for new users when they are created.</li> 
      </ul> <p>Users can modify the time zone for their <em>Workfront</em>&nbsp;instance under their profile. When&nbsp;users modify their time zone, the date and time in their emails from <em>Workfront</em> match their profile preferences. For more information about modifying user profile&nbsp;preferences, see <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>. It is selected as&nbsp;the default time zone when you create a new schedule. For more information about creating schedules, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Locale</td> 
     <td>Controls the language, date, and number format used in outgoing email messages. The locale selected here&nbsp;is&nbsp;the default when new users are created. Users can modify their locale, in their user profile. When users modify their locale, the language, date and number format in their emails from <em>Workfront</em> match their profile preferences. For more information about modifying your profile preferences, see <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Storage Quota</td> 
     <td> <p>This is the amount of document storage space available in&nbsp;your <em>Workfront</em> instance.<br>The quota contains documents that you upload directly to <em>Workfront</em>.<br>It does not include:</p> 
      <ul> 
       <li>Documents you link to&nbsp;<em>Workfront</em> from any other third-party service provider (SharePoint, Google Drive, Webdam, Box, Dropbox, any other Document Asset Management provider).</li> 
       <li>Your <em>Workfront</em> data (projects, tasks, issues, users, and so forth).</li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Product Version</td> 
     <td>This is the type of <em>Workfront</em> instance that is assigned to you. The product version for most <em>Workfront</em> customers is <span class="bold">Enterprise</span>.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="4">Click <span class="bold">Save</span>.</li> 
</ol>

