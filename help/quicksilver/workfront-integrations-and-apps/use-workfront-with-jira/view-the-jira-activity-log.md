---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: View the Jira Activity Log
description: As a Jira administrator, you can view the exceptions and errors that occur during the synchronization or creation of the tickets between Adobe Workfront and Jira in an Activity Log.
author: Becky
feature: Workfront Integrations and Apps
---

# View the Jira Activity Log

As a Jira administrator, you can view the exceptions and errors that occur during the synchronization or creation of the tickets between Adobe Workfront and Jira in an Activity Log.&nbsp;

You can see up to 500 items in the Activity Log, and they are listed starting with the most recent ones.

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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

## Prerequisites

Before you can link items between Workfront and Jira, you must

* Install Workfront for Jira

  For instructions on installing Workfront for Jira, see [Install Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Access the Jira Activity Log:&nbsp;

1. Log into Jira as a system administrator.
1. Click **Settings** in the main Jira menu.
1. Click **Add-ons**, then **Manage add-ons**.

1. Expand the **Workfront** add-on.
1. Click **Configure**.
1. Log in to Workfront as a system administrator.
1. Select the **Activity Log**&nbsp;tab.

   View information about exceptions and errors that occurred during the creation of items or&nbsp;synchronization of fields between the two applications.

   The log includes the following fields:

   * Date of the occurrence
   * The name of the user in Jira
   * Jira issue number
   * A brief description of the error that occurred.

