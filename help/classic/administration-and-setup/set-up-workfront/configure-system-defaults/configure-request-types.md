---
filename: configure-request-types
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configure request types
description: While working on a project, you might discover that unexpected events arise. You can log those unexpected events as issues for a particular project or task. You can also submit requests, which are recorded as issues on a project that is designated as a Request Queue. Issues and requests are used considered to be interchangeable in Adobe Workfront.
---

# Configure request types

While working on a project, you might discover that unexpected events arise. You can log those unexpected events as issues for a particular project or task. You can also submit requests, which are recorded as issues on a project that is designated as a Request Queue. Issues and requests are used considered to be interchangeable in Adobe Workfront.

For information about creating issues in Workfront, see [Create issues](../../../manage-work/issues/manage-issues/create-issues.md). For information about creating requests in Workfront, see [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md). For information about associating Request&nbsp;Types with projects, see [Define Request Types for a project in Adobe Workfront](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
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
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2><a name="understanding-request-types"></a>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind&nbsp;of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind&nbsp;of unexpected work&nbsp;might occur during the lifetime of a project.</p>
<p>You can specify the&nbsp;type of requests that can be logged on a project when you configure the <strong>Queue Details</strong>&nbsp;area on the <strong>Queue Setup</strong> tab for the project.&nbsp;</p>
<ol>
<li value="1"> <p> Go to the <strong>Projects</strong> area in the Global Navigation Bar. </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> Click <strong>More</strong> > <strong>Queue Setup</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, on the <strong>Queue Details</strong> sub-tab, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified&nbsp;will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## Customize the names of the request types

As a Workfront administrator, you can configure&nbsp;the names of the request types in your system. The new names are visible&nbsp;in any area of Workfront where the **Issue Type** or **Request Type** fields display:

* In the **Queue Details** area of the **Queue Setup** tab of&nbsp;a project that will receive the issues or requests.&nbsp;

* If more than one request type is selected for a Request Queue, in the **New Issue Form** in the **Issue Type** field, when you create a new issue or submit a new request.

  For more information about creating issues in Workfront, see&nbsp; [Create issues](../../../manage-work/issues/manage-issues/create-issues.md)

  For more information about creating requests in Workfront, see&nbsp; [Create and submit Adobe Workfront requests](../../../manage-work/requests/create-requests/create-submit-requests.md).

* On the **Queue Topic Detail** form, when you configure the Queue Topic.  
  For more information about creating Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

To customize the names of the request types:

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.
1. Click **Project Preferences** > **Statuses**.

1. Click the **Issues** tab.
1. At the top of the **Issues** tab, hover over the name of a request type, then click the **Edit** icon that appears.

   ![edit_request_type_name.png](assets/edit-request-type-name-350x76.png)

1. In the box that appears, type a new name, then press **Enter**.

## Configure issue statuses within different request types

You can associate each request type with different issue statuses. You can also change&nbsp;the order in which the statuses display on an issue, depending on what type of issue it is.&nbsp;

For more information about changing the default order of issue statuses and configuring issue statuses, see the [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) section in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
