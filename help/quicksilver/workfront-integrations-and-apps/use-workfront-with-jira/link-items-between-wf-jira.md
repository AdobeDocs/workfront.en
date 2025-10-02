---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Link items between [!DNL Adobe Workfront] and [!DNL Jira]
description: You can link [!DNL Jira] issues to [!DNL Adobe Workfront] tasks or issues either automatically or manually.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
---
# Link items between [!DNL Adobe Workfront] and [!DNL Jira]

 <!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

You can link [!DNL Jira] issues to [!DNL Adobe Workfront] tasks or issues either automatically or manually.

Only one item in [!DNL Workfront] can be linked to one item in [!DNL Jira]. You can never link one [!DNL Workfront] item to multiple [!DNL Jira] issues, nor one [!DNL Jira] issue to multiple [!DNL Workfront] items.

## Access requirements

You must have the following:

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a></td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] licenses overview</a></td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira access</td> 
   <td> <p>System administrator access</p> <p><b>IMPORTANT</b>  
   
   We recommend that you create separate system administrator accounts in [!DNL Jira] and [!DNL Workfront] to dedicate to this integration, rather than using existing ones that might be attached to users.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a [!DNL Workfront] administrator. For information on [!DNL Workfront] administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

 +++

## Prerequisites

Before you can link items between [!DNL Workfront] and [!DNL Jira], you must do the following:

* Install [!DNL Workfront] for [!DNL Jira].

   For instructions, see [Install Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configure [!DNL Workfront] for Jira.

   For instructions, see [Configure Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Automatically link [!DNL Workfront] items to [!DNL Jira] issues 

As a [!DNL Workfront] administrator, you can define triggers that will automatically create an issue in [!DNL Jira] every time certain conditions are met on a task or an issue in [!DNL Workfront]. The Workfront and [!DNL Jira] items become linked.

After you have completed the configuration of [!DNL Workfront] for Jira, when an item is either created or updated in [!DNL Workfront] to match your triggers, a new item is automatically created in [!DNL Jira].

Workfront users that create and update Workfront items do not need a [!DNL Jira] license to trigger the creation of items in [!DNL Jira].

For more information, see  [Configure [!DNL Adobe Workfront] for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>You can create [!DNL Jira] items automatically by attaching a template to a project. If the template contains tasks with assignments that meet the [!DNL Jira] triggers, the new tasks generate new [!DNL Jira] issues.

Automatically linking a [!DNL Workfront] issue to a [!DNL Jira] issue is identical to automatically linking a [!DNL Workfront] task to a [!DNL Jira] issue.

To automatically link a [!DNL Workfront] task to a [!DNL Jira] issue:

1. Ensure that your [!DNL Jira] system administrator has configured triggers for automatically creating [!DNL Jira] issues when [!DNL Workfront] items are assigned, then log in to [!DNL Workfront] with an access level that allows you to create a task.

   For more information about access to tasks, see [Grant access to tasks](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

{{step1-to-projects}}

1. On the **Projects** page, select a project.

1. In the project left panel, select **[!UICONTROL Tasks]**.

1. Click **+ New Task**.

   >[!NOTE]
   >
   >To link an existing Workfront item to a Jira issue, select **Edit** from the item's **More** ![More icon](assets/more-icon.png) menu.

1. Specify or update any of the fields available for the task.
1. In the **[!UICONTROL Assignments]** field, search for and select the user, role, or team that is specified as a trigger in the [!DNL Jira] integration.

1. Click **Create Task**. The task is created in Workfront, and a new comment appears in the task's **Updates** tab to indicate that a new issue has also been created in [!DNL Jira].

1. (Optional) In the **[!UICONTROL Integrations]** area of the **[!UICONTROL Details]** section of the task or issue header, click the **[!UICONTROL Go to Jira]** link to open the issue in Jira.

   Your system or group administrator must add the [!UICONTROL Integrations] field to your layout template to display it in the task or issue header. For information, see [Customize object headers using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Any [!DNL Jira] user can immediately start working on items automatically created from [!DNL Workfront] and their updates will transfer to [!DNL Workfront] without needing a license for [!DNL Workfront] to do so.

   Only the fields that you as a [!DNL Workfront] administrator configured during the setup of the [!DNL Workfront] add-on are updated.

   For more information about synchronizing fields between Workfront and Jira, see the Configure Workfront for Jira section in  [Configure Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >The [!DNL Jira] issue isn't assigned to anyone in [!DNL Jira] when it's automatically created from Workfront.

## Manually link [!DNL Jira] issues to [!DNL Workfront] items

After items have been created in [!DNL Jira] and [!DNL Workfront] independent of each other, you can manually link a [!DNL Jira] issue to an existing [!DNL Workfront] task or issue.

You cannot manually link a [!DNL Workfront] item from [!DNL Workfront] to an existing [!DNL Jira] item.

>[!NOTE]
>
>If the [!DNL Jira] issue is not on a project which is not identified as a trigger in the [!DNL Workfront] Integration you cannot manually link it to a Workfront item when using the integration with [!DNL Jira] On-Premise.\
>For more information about setting up triggers for the Workfront to Jira workflow, see [Automatically link Workfront items to Jira issues](#automatically-link-workfront-items-to-jira-issues).

When [!DNL Workfront] and [!DNL Jira] items are linked, certain fields from one item can be automatically updated on the other.\
For more information about updating linked items, see [Update linked items between Jira and Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

To manually link [!DNL Jira] issues to [!DNL Workfront] items:

1. (Conditional) Log in to [!DNL Workfront] and find an issue or a task that you want to link to a [!DNL Jira] issue.
1. (Conditional) In the **Basic information** section in the **Task Details** or **Issue Details** tab, copy the **[!UICONTROL Reference Number]** of the item in Workfront.
   
   Or

   From the address bar of the item, copy the **URL** of the item in Workfront.

   >[!IMPORTANT]
   >
   >If your organization has been onboarded to the Adobe Unified Experience, you must use the **Reference Number** for linking Workfront items to Jira. (The URL option is available, but it will return an error if you use it.) For information about the Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >For organizations not on the Adobe Unified Experience, it's not recommended to use the URL option because URLs can change.

   >[!NOTE]
   >
   >You must have a [!DNL Workfront] license to log in to [!DNL Workfront]. Otherwise, a [!DNL Workfront] user must supply this information to you.

1. In [!DNL Jira], navigate to an issue that you want to manually link to the [!DNL Workfront] item.
1. In the [!DNL Workfront] right panel, paste the **[!UICONTROL Reference Number]** or the **URL** of the [!DNL Workfront] item that you want to link it to.

1. Click **[!UICONTROL Link]**. The two items become linked and the [!DNL Workfront] right panel is populated with information from the [!DNL Workfront] item.

   By default, the following [!DNL Workfront] fields are visible in [!DNL Jira] in the [!DNL Workfront] right panel:

   * The **[!UICONTROL Name]** of the item. You can access the [!DNL Workfront] item by clicking the name in the panel. 
   * The **[!UICONTROL Project Name]**.
   * The **[!UICONTROL Status]** of the item.
   * The **[!UICONTROL Priority]** of the item.
   * The date that it was created in [!DNL Workfront].
   * The **[!UICONTROL Planned Hours]** of the item.
   * The **[!UICONTROL Reference Number]**. You can access the [!DNL Workfront] item by clicking the **Reference Number** in the panel.

   For more information about enabling additional fields to display in the right panel, see the Configure field synchronization between [!DNL Jira] and [!DNL Workfront] Items section in [Configure [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). A comment from the [!DNL Workfront] administrator associated with the integration is posted in the **[!DNL Workfront]** tab of the [!DNL Jira] issue to confirm that a new [!DNL Jira] item has been created. The comment contains a link to the [!DNL Jira] issue.

## Unlink items between [!DNL Jira] and [!DNL Workfront]

Linked items between [!DNL Jira] and [!DNL Workfront] can be manually unlinked in [!DNL Jira]. You cannot unlink a [!DNL Workfront] item from their [!DNL Jira] counterpart in [!DNL Workfront]. 

You need the following access to unlink manually linked item:

* You are the user who manually linked the items.
* You are the [!DNL Jira] system administrator.

>[!NOTE]
>
>Only a [!DNL Workfront] administrator can unlink items that were automatically linked. 

To unlink a [!DNL Jira] issue from a [!DNL Workfront] item:

1. Log in to Jira.
1. Navigate to the issue that is linked to a [!DNL Workfront] task or issue.
1. Go to the **Workfront** right panel.
1. Click the **[!UICONTROL Unlink]** icon, then click **[!UICONTROL Unlink]**. The previously linked [!DNL Jira] and [!DNL Workfront] items unlink. 

   Any of their fields, comments, or documents that are updated in the future are not updated on their previous counterpart in the other application. 
