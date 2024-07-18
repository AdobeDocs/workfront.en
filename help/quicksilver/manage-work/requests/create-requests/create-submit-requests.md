---
product-area: requests
navigation-topic: create-requests
title: Create and submit Adobe Workfront requests
description: Planned work is represented in Adobe Workfront by projects and tasks. However, you might work in an environment where unplanned work—in the form of random requests—can come in at any time. Workfront provides a workflow to accommodate this type of environment through the use of Request Queues.
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
---
# Create and submit Adobe Workfront requests

<!--Audited: 12/2023-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE: If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

Planned work is represented in Adobe Workfront by projects and tasks. However, you might work in an environment where unplanned work, in the form of requests, can come in at any time. Workfront provides a workflow to accommodate this type of environment through the use of Request Queues. 

After you create a request in a Request Queue, you can either assign it to be completed or you can convert it to a task or a project.   
For more information about converting issues to a task or project, see the article [Overview of converting issues in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

You can create a request in the following ways:

* From scratch as described in this article. 
* From drafts. For information, see [Create requests from drafts](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* From an existing request, by copying and submitting a copy. For information, see [Copy and submit requests](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Contributor or higher</p>
   Or
   <p>Current: Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites for using Request Queues

A Workfront administrator must create Request Queues and make them available to users before they can use this functionality. A user with a Planner license and with Edit access to Projects and Manage permissions to a specific project can also create Request Queues. 

For information about how to create Requests Queues, see the article [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

A Workfront administrator must create the following components of a Request Queue:

* A project in Current status, published as a Help Request Queue.
* Queue Topics.  
  For more information, see the article [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* Routing Rules.  
  For more information, see the article [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (Optional) Topic Groups.  
  For more information, see the article [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (Optional) Request custom form.  
  For more information, see the article [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* (Optional) Request approval process.  
  For more information, see the article [Create an approval process for work items](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Create requests and generate drafts in the Workfront web app

When you create a request in the Workfront web app, Workfront saves the request as a draft before you submit it. Workfront creates a draft as soon as you select your request queue and start entering information for it.

You can continue submitting the request, or you can complete as much information as you have available and navigate away from it to finish it later. Workfront saves the drafted request that you started in the Drafts folder.

>[!IMPORTANT]
>
>Consider the following when working with drafts:
>
>* Workfront does not create draft requests when you submit them from a third-party application, like emailing them into Workfront, or creating them using any another application. When you submit a request from outside the Workfront web app the request is saved in  the Submitted section.  
>* If the structure of a request queue changes, you can no longer access existing drafts. For example, if a queue topic is removed, or a topic group is added, the saved drafts are no longer accessible. 
>

For information about creating requests from existing drafts, see [Create requests from drafts](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). For information about deleting request drafts, see also [Delete a request draft](../../../manage-work/requests/create-requests/delete-request-draft.md).

To create a request in the Workfront web app: 

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. Click  **Requests**, then click **New Request** in the upper-right corner of the page.

   >[!TIP]
   >
   >* You can access the New Request option from any section in the Requests area.
   >* The New Request option is dimmed when you do not have access to create issues. 

1. (Conditional) Click inside the **Request Type** field and do one of the following:

   * From the **Recent Paths** section, select a path you used recently to open a request queue. A path includes the request queue, the topic groups, and the queue topic that you submitted to recently. The last three paths display by default.

     >[!NOTE]
     >
     >Workfront saves a path only when you have actually submitted a request to it. It does not create paths for drafted requests.

     ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * From the **Request Queues** section, select a request queue. 
   * Enter a keyword that belongs to a previously accessed path to search for a request queue.

     For example, if you have a request queue named "Help Desk" with a Topic Group named "Location" and a Queue Topic named "Remote", you can type "remote" and all the request queues that contain "remote" in any element of their path display.

     >[!TIP]
     >
     >When you type a name that contains a special character, the request queue, queue topic, or topic group display even when you omit typing the character.

     ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

     The list of available request queues and recent paths dynamically updates to include only paths that contain the keyword which is highlighted in the results.

     The results of the search display under the following areas:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Request Queues</td> 
        <td>Request queues that contain the keyword in their name</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Request Paths</td> 
        <td> <p>Paths (which include request queues, topic groups, queue topics) that contain the keyword in any of the names of their elements</p> </td> 
       </tr> 
      </tbody> 
     </table>

   >[!TIP]
   >
   >* The first 200 request queues display by default, in alphabetical order. 
   >* The name of the request queue is the name of the project which has been published as a Help Request Queue. 
   >* The description of the project configured as the selected request queue displays to the right of the request queue name. 
   >   
   >For more information about how to publish a project as a Help Request Queue, see the article [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. In the **New request** form, do one of the following:

   * (Conditional) Select an available draft from the notification message displayed under the Request Type field.

     This area displays only if you have saved drafts before without submitting them.

     The three most recent drafts from three different queue topics display by default.

     ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * Start entering a new request in the selected queue.

     A new draft automatically saves for you in the Drafts  section  after you start entering information for the new request and you give the request a name in the Subject field.

1. (Optional) If your Request Queue includes Topic Groups, select the name of the Topic Group in the first drop-down field. Otherwise, select a Queue Topic.

   >[!TIP]
   >
   >When you hover over a Topic Group or a Queue Topic the Description field displays to the right. This contains additional information about the topic group or queue topic. 
   >
   >
   >![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >
   >

   You can have up to 10 tiers of Topic Groups built into your Request Queue.   
   For more information about how to create Topic Groups, see the article [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). For more information about creating Queue Topics, see the article [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   >
   >If you selected a draft or a previous path, the topic groups and queue topics are already selected. You can select a different one, if needed.

1. Depending on what fields the Workfront administrator enabled in the **New Issue Fields** section of the **Queue Details** subtab on the project, you might find any of the following fields when you submit a new request:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Subject</strong> </td> 
      <td>Specify a name for your request. This is a mandatory field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Specify a description for your request.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Specify a URL that might relate to your request.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong> </td> 
      <td> <p>Specify a priority for your request. The priority should define how fast you think this request should be resolved. The default options are: </p> 
       <ul> 
        <li>None</li> 
        <li>Low </li> 
        <li>Normal</li> 
        <li>High</li> 
        <li>Urgent</li> 
       </ul> <p>Your system administrator can modify the names of priorities.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Severity</strong> </td> 
      <td> <p>Specify a severity for your request. The severity should define the impact this request has on your work should it not be resolved in time. The default options are:</p> 
       <ul> 
        <li>Cosmetic</li> 
        <li>Causes Confusion</li> 
        <li>Bug with workaround</li> 
        <li>Bug with no workaround</li> 
        <li>Fatal error</li> 
       </ul> <p>Your system administrator can modify the names of severities.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Primary Contact</strong> </td> 
      <td>The Primary Contact of a request defaults to you, as you are the point person to address any questions pertaining to the request. However, you can change this to any other Workfront user.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Assignments</strong> </td> 
      <td> <p><span>Specify the name of an active user, job role, or a team that the request should be assigned to.</span> </p> <p>You can specify only one team.</p> 
           
      <p> Depending on how the request queue was set up, you might be able to only assign one or two types of resource to the request, instead of all three (for example, you might only be able to assign the request to users).</p> 
      
      <p>If a routing rule is also associated to the request queue and it automatically routes the request to a different type of resource (for example, a team), your request is assigned to both the entity that you manually specify when submitting the request (users) and the resource specified in the routing rule (the team.) </p>
      
      <p> For more information, see the following articles:</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Create Routing Rules</a> <br> </p> </li> 
      </ul> </p>
      
      <p><span>We recommend using Routing Rules for your Request Queues so that they can be automatically routed to the appropriate resources.</span> </p> </td> 
     </tr> 
     
     <tr> 
      <td role="rowheader"><strong>Planned Hours</strong> </td> 
      <td> <p>Estimate how many hours it would take for this request to complete.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Start Date</strong> </td> 
      <td> <p>Specify the date when work on this request should start.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Completion Date</strong> </td> 
      <td>Specify the date when you would like for this request to be resolved.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>The default status of a new request is "New." Your system administrator might have changed the name of this status. You can also change the status to something else from this drop-down menu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documents</strong> </td> 
      <td> <p>Add documents to your request. </p> <p> Depending on how the request queue was set up, the Documents section might display before or after the custom fields. </p> <p>Documents that you upload to Workfront are stored for 24 hours in a drafted request. After that, you must reattach them when you return to edit and submit the draft. Documents that are linked from other drives are saved on the draft permanently. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) If your Workfront administrator associated a custom form with the Request Queue or with the Queue Topic, specify the fields inside the custom form.   
   Custom forms are different for every Workfront instance. 
1. (Optional and conditional) At any point during entering the request, click [!UICONTROL **Discard draft**] if you want to delete the draft that is automatically created. This deletes the draft which cannot be recovered. A confirmation message displays to acknowledge that you are deleting the draft. 

1. (Optional) Click [!UICONTROL **Undo**] on the confirmation message if you want to revert your action and keep the draft.

1. Do one of the following:

   * Click **Submit** if you are ready to submit the request. The request is saved in the  Submitted section  . Depending on the Routing Rule of the Request Queue, this request might be routed to a different project than the one designated as a Request Queue. For information about routing rules, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     Or

     Click **Close** if you are not quite ready to submit it and you might come back and finish it later. Your request is saved in the Drafts  section and it will be available to you next time you submit a request for this request queue.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

   When you submit the request, the draft automatically deletes and cannot be restored.

   For information about addressing incoming requests, see the article [Manage work and team requests](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   For information about locating submitted or drafted requests, also see [Locate submitted requests](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Create requests from outside of Workfront

You can share a direct link to a request queue when you submit a new request, and embed it in other applications. Users who access this link from the web or from other applications must also be logged in with an active Workfront account to be able to access this queue and submit requests to it. For information, see [Share a link to a request queue](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Create requests by emailing into Workfront

If your Request Queue is enabled to receive requests through email, you can email your requests directly to the email address associated with the Request Queue.

The body text of the email is added as the request description.

>[!NOTE]
>
>HTML formatting is stripped when the request enters Workfront, but signatures and existing Reply-to thread contents are not stripped and appear in the request description.

For information about how to enable a Request Queue to receive requests through email, see [Enable users to email an issue into a Request Queue project](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Create requests using the Outlook client

You can submit requests using the Outlook client. You can create a new request or you can convert an email into a request. 

For information about submitting requests using the Outlook client, see the article [Create an Adobe Workfront request from an Outlook email](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## Create requests by using the Workfront mobile app

You can submit requests using the mobile app on your smartphone. You can create a new request and submit it to the Request Queues you have access to see in the web application. 

For information about submitting requests through the mobile app, see the Requests section in the articles:

* [Adobe Workfront for Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests) 
* [Adobe Workfront for iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md#requests)

## Create requests from other applications

You can submit requests using any applications that have been integrated with Workfront: 

* You can build a custom integration between Workfront and another application that allows you to submit requests to Workfront from the other application.  
  For more information about custom Workfront integrations, see the article [Adobe Workfront integrations](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* You can submit requests from Salesforce if you have installed the Workfront app for Salesforce.  
  For information about submitting requests from Salesforce using our Workfront app for Salesforce, see the article [Submit Adobe Workfront requests from Salesforce objects](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## Locate submitted requests

For information about locating submitted or drafted requests, see [Locate submitted requests](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
