---
filename: submit-workfront-requests-from-ms-teams
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Submit Adobe Workfront requests from Microsoft Teams
description: After your team owner installs Adobe Workfront for Microsoft Teams, you can submit Workfront requests from your Microsoft Teams account. To do so, you must have a Workfront account with access to submit requests. For information about installing Workfront for Microsoft Teams, see Installing Workfront for Microsoft Teams.
---

# Submit Adobe Workfront requests from Microsoft Teams

After your team owner installs Adobe Workfront for Microsoft Teams, you can submit Workfront requests from your Microsoft Teams account. To do so, you must have a Workfront account with access to submit requests. For information about installing Workfront for Microsoft Teams, see [Installing Workfront for Microsoft Teams](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

>[!NOTE]
>
>Microsoft Teams no longer supports Internet Explorer. To use the Adobe Workfront for Microsoft Teams integration, you must use a web browser other than Internet Explorer.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work, Plan, Review, Request</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>[Insert any access level configurations needed]
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: Edit access to Documents
       </MadCap:conditionalText>
      </p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You must be a Workfront administrator. For information on Workfront administrators, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a group administrator. For more information on group administrators, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
     </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed and specify the object]
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: View access or higher on Documents
       </MadCap:conditionalText>
      </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Your Microsoft Teams team owner must install Workfront for Microsoft Teams before you can use it.

## Submit Workfront requests from Microsoft Teams

1. Click the **More added apps** icon on the left navigation bar in Microsoft Teams.

   ![](assets/ms-teams-more-added-apps-icon.png)

1. Click **Workfront** in the list that appears.
1. Click the **Requests** tab.
1. Click **New Request**.
1. In the **Select a Request Type** box, select the request queue where you want to submit the request.
1. (Optional) Select a Topic Group or a Queue Topic, if they are available on the request queue.
1. Specify the following information:

   (Depending on how the request queue was set up, the options and boxes you see might vary. For a complete list and description of possible fields, see [Create and submit Adobe Workfront requests](../../manage-work/requests/create-requests/create-submit-requests.md).)

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Subject</td> 
      <td>Type a subject name for the request.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Type a description for the request.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">&nbsp;</td> 
      <td> <p>Attach any documents that you want to include in the request. You can attach documents via drag and drop, or by clicking Select file and browsing to and selecting the document in your file system.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) If the Workfront administrator attached custom forms to the request queue, provide the information in the fields available on the custom forms.
1. The custom forms display at the bottom of the new request.
1. Click **Submit**.

   The Request appears in Workfront, in the specified request queue. You receive a confirmation that the request was submitted successfully.

## View Workfront requests you submitted in Microsoft Teams

1. Click the **More added apps** icon on the left navigation bar in Microsoft Teams.

   ![](assets/ms-teams-more-added-apps-icon.png)

1. Click **Workfront** in the list that appears.
1. Click the **Requests** tab.

   ![](assets/ms-teams-requests-page-with-count-350x198.png)

   Requests you submitted are listed in the My submitted requests area of the Requests tab. You cannot configure the information displayed in this tab about the requests you submitted.

   You can view the following information about your submitted requests in the My submitted requests area of the Requests tab:

   | Subject |The name of the request |
   |---|---|
   | Reference number |&nbsp; |
   | Request type |The name of the request queue where you submitted the request |
   | Status |&nbsp; |
   | Submitted on |The date when you submitted the request |
   | Assigned to |&nbsp; |

1. (Optional) Click the header of any of the columns in the list to sort the list by that column. By default, Workfront sorts the list by the Submitted on date, starting with the most recently submitted request.

