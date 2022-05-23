---
filename: configure-basic-info
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configure basic information for your system
description: As part of configuring your Adobe Workfront system, you can manage details about your organization in the Basic Info section of your Customer Info page.
---

# Configure basic information for your system

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **&nbsp;</p>
-->

As part of configuring your Adobe Workfront system, you can manage details about your organization in the Basic Info section of your Customer Info page.

## Access requirements

You must have the following access to perform the steps in this article: 

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>Note<>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Access Customer Info

The customer represents the Workfront instance for your organization. The options in this area are unique to you, as a customer of Workfront.

To access the Customer Info page:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  

1. In the left panel, click **System** > **Customer Info**.

   Depending on the Workfront plan that you have purchased, some sections might be missing from the Customer Info page. Contact your Account Representative if you need to find out which Workfront plan your organization uses.

   The sections available in the Customer Info area are:

   * **Basic Info**

     For information&nbsp;about configuring basic information in Workfront, see [Configure Basic Info](#configure-basic-info).
   
   * **API Key Settings**

     For information about API key settings, see [Manage API keys](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).
   
   * **IP Allowlist**

     For information about adding the IP addresses to your allowlist for where your users can access Workfront, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
   
   * **License**

     For information about licenses, see [Manage available licenses in your system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## Configure Basic Info {#configure-basic-info}

Inside the Basic Info area of your Customer Info page, some details about your customer are configured by Workfront and they display in a read-only mode. Other details can be configured by you. Any options you can edit in this area have a global effect on all users in Workfront.

To&nbsp;configure your Basic Info section in your Customer Info area:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **System** > **Customer Info**. 

1. In the **Basic Info** section at the top of the **Customer Info** page, find the following information about your instance with Workfront:

   <table> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>The name of your organization, which also matches the name of your company. This is added by Workfront and it cannot be edited.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cluster Setup </td> 
      <td>The cluster number for your instance.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Admin Email</td> 
      <td> <p>The email address of your Workfront administrator. You can edit this field to match the email address of one of your Workfront administrators. The user associated with this email address is considered the main Workfront administrator of your Workfront system. Any site-wide communication from Workfront is directed&nbsp;to this email address, so it is important to keep it updated.</p> <p>Note:  You cannot deactivate, delete, or change the Access Level of the user associated with the Admin Email.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domain</td> 
      <td> <p>The domain is set by Workfront when your account is created.</p> <p>The domain identifies your&nbsp;unique sub-domain of the URL you use to access Workfront.<br>For example, if your organization has been assigned the domain "mycompany," the URL you use to access Workfront is <i>https://mycompany.my.workfront.com</i>.<br>You cannot edit the domain yourself. If you want to change your domain, you can contact Workfront Customer Support. For more information about&nbsp;contacting Workfront&nbsp;Customer Support, see <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Time Zone</td> 
      <td> <p>This is the default time zone of your Workfront instance. You can edit this field to match the time zone of your primary Workfront location. The time zone you select determines the following: </p> 
       <ul> 
        <li>The date and time displayed in outgoing emails</li> 
        <li>The default time zone for new users when they are created</li> 
       </ul> <p>Users can modify the time zone for their Workfront&nbsp;instance under their profile. When&nbsp;users modify their time zone, the date and time in their emails from Workfront match their profile preferences. For more information about modifying user profile&nbsp;preferences, see <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>. It is selected as&nbsp;the default time zone when you create a new schedule. For more information about creating schedules, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p>For information about using schedules to help users collaborate in Workfront across time zones, see <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Working across time zones</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Locale</td> 
      <td>Controls the language, date, and number format used in outgoing email messages. The locale selected here&nbsp;is&nbsp;the default when new users are created. Users can modify their locale, in their user profile. When users modify their locale, the language, date and number format in their emails from Workfront match their profile preferences. For more information about modifying your profile preferences, see <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Storage Quota</td> 
      <td> <p>This is the amount of document storage space available in&nbsp;your Workfront instance.<br>The quota contains documents that you upload directly to Workfront.<br>It does not include:</p> 
       <ul> 
        <li>Documents you link to&nbsp;Workfront from any other third-party service provider (SharePoint, Google Drive, Webdam, Box, Dropbox, any other Document Asset Management provider).</li> 
        <li>Your Workfront data (projects, tasks, issues, users, and so forth).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Product Version</td> 
      <td>This is the type of Workfront instance that is assigned to you. The product version for most Workfront customers is <strong>Enterprise</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.

