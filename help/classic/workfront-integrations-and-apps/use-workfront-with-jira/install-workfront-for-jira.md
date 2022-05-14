---
filename: install-workfront-for-jira
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Install Adobe Workfront for Jira
description: You can use Adobe Workfront for Jira to integrate your Jira and Workfront systems.
---

# Install Adobe Workfront for Jira

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can use Adobe Workfront for Jira to integrate your Jira and Workfront systems.

After installing the add-on, you can define workflows that create Jira issues automatically when Workfront work items are created. The items in both applications become linked, and some of their information can be automatically updated in both systems.&nbsp;

All users in Workfront and Jira can benefit from this integration. They only need a license for the system in which they work the most, and not for both systems.&nbsp;

This add-on is available for the Server, Data Center, and OnDemand (or Cloud) versions of Jira Software.

For a list of Jira versions that Workfront for Jira currently supports, see [Workfront for Jira](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) at the Atlassian Marketplace.

## Access requirements

You must have the following:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront plan</a>*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira access</td> 
   <td> <p>System administrator access</p> <p>Important:  We recommend that you create separate system administrator accounts in Jira and Workfront to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Install Workfront for Jira

Installing Workfront for Jira OnDemand is identical to installing it on a Jira Server instance.

You must be a Jira administrator to install the Workfront add-on.

If you are not a Jira administrator, you can browse for the Workfront add-on and request it to be installed. Your request is sent to the Jira administrator for approval and installation.

For more information about requesting an add-on to be installed on your Jira application, see [Managing user requests for add-ons.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

To install Workfront for Jira:

1. Log in to Jira as a Jira administrator.
1. Find the **Workfront for Jira**&nbsp;add-on in the [Atlassian Marketplace](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1. Click **Get it now** to install it.

   After the installation completes, you can log in to Workfront from Jira and configure your integration.

   For more information, see [Configure Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Considerations for a Jira Server or Jira Data Center installation

>[!NOTE]
>
>These requirements do not apply to the OnDemand (Cloud) version of Jira Software.

Although installing the Workfront add-on in the two Jira environments is similar, you must consider the following when working with a Jira Server installation:

* When configuring the add-on in Jira, the address specified in the&nbsp;**JIRA Base URL**&nbsp;field may not be the same URL you use to access Jira on your private server. The **JIRA Base URL** must be a publicly-accessible address connected to your private server using NAT or reverse proxy protocols, so Workfront can access it to make requests to your server.&nbsp;&nbsp;

* You must use SSL encryption to secure the communication between JIRA and Workfront. When you enable SSL, you must have a full SSL certificate stack from a certificate authority. We do not support self-signed certificates.&nbsp; 
* You must ensure that the jira.workfront.com domain is accessible from your corporate servers. It serves as a middleware environment between Workfront and Jira and is required for the add-on to operate.

  You must also add the following static IP addresses to the allowlist on your firewall for outbound and inbound connections.
   
     ```   
     35.162.128.73
     ```
   
     ```   
     34.213.36.118
     ```

   
     ```   
     35.160.0.242
     ```

   
     ```   
     3.209.27.146
     ```
   
     ```   
     18.205.251.4
     ```

  For more information about configuring your firewall for optimal functionality with Workfront, see [Configuring Your Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

