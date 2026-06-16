---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configure Basic Information for Your System
description: As part of configuring your Adobe Workfront system, you can manage details about your organization in the Basic Info section of your Customer Info page.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
last-update: 2026-04-29T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/4536sfZCe8ugbGGuFUQeyFXnNNifG0e5MZ4npIlH1iI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Configure basic information for your system

{{highlighted-preview}}

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

As part of configuring your Adobe Workfront system, you can manage details about your organization in the Basic Info section of your Customer Info page.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>You must be a Workfront administrator. </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Access Customer Info

The customer represents the Workfront instance for your organization. The options in this area are unique to you, as a customer of Workfront.

To access the Customer Info page:

{{step-1-to-setup}}

1. In the left panel, click **System** > **Customer Info**.

   Depending on the Workfront package that you have purchased, some sections might be missing from the Customer Info page. Contact your Account Representative if you need to find out which Workfront package your organization uses.

   The sections available in the Customer Info area are:

   | Section | More information |
   |---------|-----------------|
   | **Basic Info** | For information about configuring basic information in Workfront, see [Configure Basic Info](#configure-basic-info). |
   | <span class="preview">**Storage Overview**</span> | <span class="preview">For information about checking document storage usage and quota, see [Check document storage limits](../../documents/managing-documents/check-document-storage.md).</span> |
   | **API Key Settings** | For information about API key settings, see [Manage API keys](../../administration-and-setup/manage-workfront/security/manage-api-keys.md). |
   | **IP Allowlist** | For information about adding the IP addresses to your allowlist for where your users can access Workfront, see [Configure your firewall's allowlist](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md). |
   | **Email Allowlist** | For information about adding emails to your allowlist, see [Configure your email allowlist](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md). |

   <!--
   * **License**

     For information about licenses, see [Manage available licenses in your system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).
     -->

## Configure Basic Info {#configure-basic-info}

Inside the Basic Info area of your Customer Info page, some details about your customer are configured by Workfront and they display in a read-only mode. Other details can be configured by you. Any options you can edit in this area have a global effect on all users in Workfront.

To configure your Basic Info section in your Customer Info area:

{{step-1-to-setup}}

1. In the left panel, click **System** > **Customer Info**. 

1. In the **Basic Info** section at the top of the **Customer Info** page, find the following information about your instance with Workfront:

   <table style="table-layout:auto"> 
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
      <td> <p>The email address of your Workfront administrator. You can edit this field to match the email address of one of your Workfront administrators. The user associated with this email address is considered the main Workfront administrator of your Workfront system. Any site-wide communication from Workfront is directed to this email address, so it is important to keep it updated.</p> <p><b>NOTE</b>:  You cannot deactivate, delete, or change the Access Level of the user associated with the Admin Email.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domain</td> 
      <td> <p>The domain is set by Workfront when your account is created.</p> <p>The domain identifies your unique sub-domain of the URL you use to access Workfront.<p>For example, if your organization has been assigned the domain "mycompany," the URL you use to access Workfront is <i>https://mycompany.my.workfront.com.</i></p><p>You cannot edit the domain yourself. If you want to change your domain, you can contact Workfront Customer Support. For more information about contacting Workfront Customer Support, see <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Time Zone</td> 
      <td> <p>This is the default time zone of your Workfront instance. You can edit this field to match the time zone of your primary Workfront location. The time zone you select determines the following: </p> 
       <ul> 
        <li>The date and time displayed in outgoing emails</li> 
        <li>The default time zone for new users when they are created</li> 
       </ul> <p>Users can modify the time zone for their Workfront instance under their profile. When users modify their time zone, the date and time in their emails from Workfront match their profile preferences. For more information about modifying user profile preferences, see <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>. It is selected as the default time zone when you create a new schedule. For more information about creating schedules, see <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p>For information about using schedules to help users collaborate in Workfront across time zones, see <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Working across time zones</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Default Email Locale</td> 
      <td>Controls the language, date, and number format used in outgoing email messages. The locale selected here is the default when new users are created. Users can modify their locale, in their user profile. When users modify their locale, the language, date and number format in their emails from Workfront match their profile preferences. For more information about modifying your profile preferences, see <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save**.
