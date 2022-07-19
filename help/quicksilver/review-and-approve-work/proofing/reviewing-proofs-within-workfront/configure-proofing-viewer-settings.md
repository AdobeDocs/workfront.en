---
product-area: documents;setup
navigation-topic: review-a-proof
title: Configure proofing viewer settings
description: You can configure the following settings for both the Web Proofing Viewer and the Desktop Proofing Viewer - EDIT ME.
author: Courtney
feature: Digital Content and Documents
---

# Configure proofing viewer settings

You can configure the following settings for both the Web Proofing Viewer and the Desktop Proofing Viewer:

* Whether comment markups and pins display on proofs.
* Whether the markup tools display across the top of the proofing viewer or in a drop-down menu.
* Which email notifications you receive as a reviewer on the proof you have open.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

You can configure the following settings for the Desktop Proofing Viewer:

* How you want links within website content to open in the Viewer.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* What happens when you click a link that is set to open in a new browser tab or window.
* Clear the cache data that might be saved with the proof you are viewing in order to enable content such as pop-ups (that can be blocked by browser cache data) to display in the Viewer.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current plan: Work or Plan</p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof Permission Profile </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or Proof Permission Profile you have, contact your Workfront or Workfront Proof administrator.

## Configure proofing viewer settings

To configure proofing viewer settings:

1. Open the Web Proofing Viewer or the Desktop Proofing Viewer in one of the following ways:

   * If you proof within Adobe Workfront, go to a document list containing a proof you want to view, hover over the document, then click&nbsp;**Open proof**.
   * If you use Workfront Proof, click the **Go to Proof** icon for the proof in the Dashboard or a Views list ![](assets/go-to-proof-blue-icon.png).

1. If the left toolbar is not showing, click the&nbsp;**Menu**&nbsp;icon, located in the upper-left corner of the Web Proofing Viewer.

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. In the left toolbar, click the **Settings** icon ![](assets/settings-icon-in-pv.png).   

1. Configure any of the following **Settings** that display.

   The settings available might vary depending on the type of proof you have open.

   * **Show markups**&nbsp;(always available in the Web Proofing Viewer and the Desktop Proofing Viewer): These are the comment marks that reviewers add to proofs when they use the markup tools. If you disable them, you can still see them when you click a comment in the comment list.

     This setting affects all proofs you open.
   
   * **Show pins**&nbsp;(always available in the Web Proofing Viewer and the Desktop Proofing Viewer): These are the numbered pins that reviewers add to proofs when they use the markup tools. They indicate where and in what order the reviewer added comments. If you disable them, you can still see them when you click a comment in the comment list.

     This setting affects all proofs you open.
   
   * **Use expanded markup tools**&nbsp;(always available in the Web Proofing Viewer and the Desktop Proofing Viewer): By default, the markup tool options display across the top of the proofing viewer.&nbsp;You can configure them to display in a vertical menu that opens only when you click it.

     This setting is in effect for all proofs you open.
   
   * **Send me email notifications about** (always available in the Web Proofing Viewer and the Desktop Proofing Viewer): Click one of the options below. This setting affects only the proof you have open. For more information, see [Notifications for proof comments and decisions overview](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">All activity</td> 
        <td>Workfront sends an email to the reviewer every time there is any activity on the proof, such as&nbsp;a new&nbsp;comment, reply, or&nbsp;decision. <p>This is a great option for the person who is managing the proofing process because&nbsp;it allows them to see the activity as it happens. </p><p>Users do not receive an email alert about their own activity.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Replies to my comments</td> 
        <td>An email is sent to the reviewer only if someone replies explicitly to their&nbsp;comment&nbsp;(this excludes their own replies on their own comments). This means that if somebody on the proof makes a new comment, the reviewer is not notified.<p>This&nbsp;setting is recommended for your clients on the proof so that they are not&nbsp;notified of any other comments&nbsp;on the proof, and are&nbsp;notified only&nbsp;of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new&nbsp;comments, they can still view&nbsp;all&nbsp;comments&nbsp;on the proof in&nbsp;the proofing viewer.</p><p>For information about comments, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">View and reply to proof comments</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisions</td> 
        <td>Workfront sends an email to the reviewer only when someone makes a&nbsp;decision.<p>This can be useful for the person who is managing the approval process&nbsp;(such as a project manager) and&nbsp;needs to monitor progress on the proof and see which users have&nbsp;made their&nbsp;decision.</p><p>You are not notified of your own decision unless you select an email confirmation option when submitting your decision.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Final decision</td> 
        <td>Workfront sends an email when the last approver on the proof has made their&nbsp;decision.<p>This alert is often used by the designer, who does not usually need to take part in the actual review discussion. When the final decision is made, the designer is&nbsp;notified and&nbsp;can then take&nbsp;action on any necessary changes.</p><p>This alert can also be useful&nbsp;for a department leader&nbsp;who needs to be notified only when the review process is finished.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Hourly Summary</td> 
        <td>Workfront sends an email to the reviewer every hour with a summary of all the&nbsp;comments, replies, and&nbsp;decisions&nbsp;that have occurred in the hour.<p>The email is sent only when&nbsp;activity besides your own&nbsp;occurs within the past&nbsp;hour. </p><p>This alert is a good way of seeing an overview of the project.</p><p>An example use case for this summary is a&nbsp;senior reviewer&nbsp;who needs an overview of the project but does not need to be notified immediately of all activity on the proof.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Daily Summary</td> 
        <td>Workfront sends one email with all&nbsp;comments, replies, and decisions listed only on days when there is activity besides your own.<p>This alert is a good way of seeing a summary of the project&nbsp;without being overwhelmed with multiple&nbsp;updates throughout the day.</p><p>An example use case for this summary is a department leader&nbsp;who wants to monitor the overall progress of the project.</p><p>For more information, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Manage notifications for proof comments and decisions</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">No email</td> 
        <td>Workfront does not send any email alerts.<br>This is useful&nbsp;for a person who is added to a proof only for reference purposes and does not need to be notified of any changes.<p>The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your proofs have this setting.</p></td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->   
   
   * **When clicking hyperlinks in a proof** (available only in the Desktop Proofing Viewer): Select an option to specify what happens in the Desktop Proofing Viewer when you click a link that is set to open in a new browser tab or window.

     This setting is in effect for all interactive proofs you open.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Open within the proofing viewer</td> 
        <td>Links always open within the Desktop Proofing Viewer and you can proof the linked content. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Open in the browser</td> 
        <td>Links always open within the browser, not in a proofing viewer. You are not able to proof the linked content.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Ask me every time</td> 
        <td> <p>You are prompted each time whether you want to open the link within the Desktop Proofing Viewer or in the browser. If you open the link within the Desktop Proofing Viewer, you can proof the linked content. If you open the link in the browser, you are not able to proof the linked content.</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>This setting affects only the proof you have open.</p> </td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->   
   
   * **Clear cache**: Clears the browser cache data that might be saved with an interactive proof you are viewing. This enables content such as pop-ups (that can be blocked by browser cache data) to display in the Desktop Proofing Viewer.

     The data that is cleared includes the HTTP cache (such as images to be reused after the next page refresh) and the web storage data cache (such as cookies and data that identifies users).

     This setting affects only the proof you have open.

