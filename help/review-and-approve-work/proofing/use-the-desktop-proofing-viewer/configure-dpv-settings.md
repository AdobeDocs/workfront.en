

# Configure `Desktop Proofing Viewer` settings

You can configure the following settings for the `Desktop Proofing Viewer`:

* Whether comment markups and pins display on `proofs`.
* Whether the markup tools display across the top of the `proofing viewer` or in a drop-down menu.
* Which email notifications you receive as a reviewer on the `proof` you have open.

  <!--
  Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).
  -->

You can configure the following settings for the `Desktop Proofing Viewer`:

* How you want links within website content to open in the Viewer.

  <!--
  Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.
  -->

* What happens when you click a link that is set to open in a new browser tab or window.
* Clear the cache data that might be saved with the `proof` you are viewing in order to enable content such as pop-ups (that can be blocked by browser cache data) to display in the Viewer.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Current plan: Pro or Higher</p> <p>or</p> <p>Legacy plan: Select or Premium</p> <p>For more information about proofing access with the different plans, see <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Access to proofing functionality in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p>Current plan: <span>Work</span> or <span>Plan</span></p> <p>Legacy plan: Any (You must have proofing enabled for the user)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Proof Permission Profile</span> </td> 
   <td>Manager or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Documents</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, role, or `Proof Permission Profile` you have, contact your `Workfront` or `Workfront Proof administrator`.

## Configure `proofing viewer` settings

To configure `proofing viewer` settings:

<ol> 
 <li value="1">Open the <span>Web Proofing Viewer</span> or the <span>Desktop Proofing Viewer</span> in one of the following ways: 
  <ul>
   <li>If you <span>proof</span> within <span>Adobe Workfront</span>, go to a document list containing a <span>proof</span> you want to view, hover over the document, then click&nbsp;<span class="bold">Open <span>proof</span></span>.</li>
   <li>If you use <span>Workfront Proof</span>, click the <span class="bold">Go to Proof</span> icon for the <span>proof</span> in the Dashboard or a Views list. <img src="assets/go-to-proof-blue-icon.png"><br></li>
  </ul></li> 
 <li value="2"> <p>If the left toolbar is not showing, click the&nbsp;<span class="bold">Menu</span>&nbsp;icon, located in the upper-left corner of the <span>Web Proofing Viewer</span>.</p> <p> <img src="assets/menu-icon-in-proofing-viewer-350x228.png" style="width: 350;height: 228;"> </img> </p> </li> 
 <li value="3"> In the left toolbar, click the <span class="bold">Settings</span> icon <img src="assets/settings-icon-in-pv.png">. <br></li> 
 <li value="4"> <p> Configure any of the following <span class="bold">Settings</span> that display.</p> <p>The settings available might vary depending on the type of <span>proof</span> you have open.</p> 
  <ul> 
   <li> <p><span class="bold">Show markups</span>&nbsp;(always available in the <span>Web Proofing Viewer</span> and the <span>Desktop Proofing Viewer</span>): These are the comment marks that reviewers add to <span>proofs</span> when they use the markup tools. If you disable them, you can still see them when you click a comment in the comment list.</p> <p>This setting affects all <span>proofs</span> you open.</p> </li> 
   <li> <p><span class="bold">Show pins</span>&nbsp;(always available in the <span>Web Proofing Viewer</span> and the <span>Desktop Proofing Viewer</span>): These are the numbered pins that reviewers add to <span>proofs</span> when they use the markup tools. They indicate where and in what order the reviewer added comments. If you disable them, you can still see them when you click a comment in the comment list.</p> <p>This setting affects all <span>proofs</span> you open.</p> </li> 
   <li> <p><span class="bold">Use expanded markup tools</span>&nbsp;(always available in the <span>Web Proofing Viewer</span> and the <span>Desktop Proofing Viewer</span>): By default, the markup tool options display across the top of the <span>proofing</span> viewer.&nbsp;You can configure them to display in a vertical menu that opens only when you click it.</p> <p>This setting is in effect for all <span>proofs</span> you open.</p> </li> 
   <li> <p><span class="bold">Send me email notifications about</span> (always available in the <span>Web Proofing Viewer</span> and the <span>Desktop Proofing Viewer</span>): Click one of the options below. This setting affects only the <span>proof</span> you have open. For more information, see <a href="../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md" class="MCXref xref">Notifications for proof comments and decisions overview</a>.</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">All activity</td> 
       <td><span>Workfront</span> sends an email to the reviewer every time there is any activity on the <span>proof</span>, such as&nbsp;a new&nbsp;comment, reply, or&nbsp;decision. <p>This is a great option for the person who is managing the <span>proofing</span> process because&nbsp;it allows them to see the activity as it happens. </p><p>Users do not receive an email alert about their own activity.</p></td> 
      </tr> 
      <tr> 
       <td role="rowheader">Replies to my comments</td> 
       <td>An email is sent to the reviewer only if someone replies explicitly to their&nbsp;comment&nbsp;(this excludes their own replies on their own comments). This means that if somebody on the <span>proof</span> makes a new comment, the reviewer is not notified.<p>This&nbsp;setting is recommended for your clients on the <span>proof</span> so that they are not&nbsp;notified of any other comments&nbsp;on the <span>proof</span>, and are&nbsp;notified only&nbsp;of replies to their own comments.</p><p>Although reviewers with this email alert setting are not notified of other new&nbsp;comments, they can still view&nbsp;all&nbsp;comments&nbsp;on the <span>proof</span> in&nbsp;the <span>proofing viewer</span>.</p><p>For information about comments, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">View and reply to proof comments</a>.</p></td> 
      </tr> 
      <tr> 
       <td role="rowheader">Decisions</td> 
       <td><span>Workfront</span> sends an email to the reviewer only when someone makes a&nbsp;decision.<p>This can be useful for the person who is managing the approval process&nbsp;(such as a project manager) and&nbsp;needs to monitor progress on the <span>proof</span> and see which users have&nbsp;made their&nbsp;decision.</p><p>You are not notified of your own decision unless you select an email confirmation option when submitting your decision.</p></td> 
      </tr> 
      <tr> 
       <td role="rowheader">Final decision</td> 
       <td><span>Workfront</span> sends an email when the last approver on the <span>proof</span> has made their&nbsp;decision.<p>This alert is often used by the designer, who does not usually need to take part in the actual review discussion. When the final decision is made, the designer is&nbsp;notified and&nbsp;can then take&nbsp;action on any necessary changes.</p><p>This alert can also be useful&nbsp;for a department leader&nbsp;who needs to be notified only when the review process is finished.</p></td> 
      </tr> 
      <tr> 
       <td role="rowheader">Hourly Summary</td> 
       <td><span>Workfront</span> sends an email to the reviewer every hour with a summary of all the&nbsp;comments, replies, and&nbsp;decisions&nbsp;that have occurred in the hour.<p>The email is sent only when&nbsp;activity besides your own&nbsp;occurs within the past&nbsp;hour. </p><p>This alert is a good way of seeing an overview of the project.</p><p>An example use case for this summary is a&nbsp;senior reviewer&nbsp;who needs an overview of the project but does not need to be notified immediately of all activity on the <span>proof</span>.</p></td> 
      </tr> 
      <tr> 
       <td role="rowheader">Daily Summary</td> 
       <td><span>Workfront</span> sends one email with all&nbsp;comments, replies, and decisions listed only on days when there is activity besides your own.<p>This alert is a good way of seeing a summary of the project&nbsp;without being overwhelmed with multiple&nbsp;updates throughout the day.</p><p>An example use case for this summary is a department leader&nbsp;who wants to monitor the overall progress of the project.</p><p>For more information, see <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Manage notifications for proof comments and decisions</a>.</p></td> 
      </tr> No email Workfront does not send any email alerts. This is useful for a person who is added to a proof only for reference purposes and does not need to be notified of any changes. The system default is Daily summary (also seen as Not Set). If you or your reviewers do not make any other changes, all your proofs have this setting. <!--
       Set a deadline Select the day and time when users must take action on the proof. If you are adding users to a proof for a document that already exists in Workfront, you should have already set a deadline.
      --> <!--
       Notify people by email Select this option to send an email to the users, notifying them of the proof. Click Add a custom message to specify a message to include in the email notification.
      --> 
     </tbody> 
    </table> </li> <!--
    Use desktop app as default: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see Desktop Proofing Viewer in the article Configure proof settings for your organization. For comparative information about the two viewers, see Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview.
   --> 
   <li> <p><span class="bold">When clicking hyperlinks in a <span>proof</span></span> (available only in the <span>Desktop Proofing Viewer</span>): Select an option to specify what happens in the <span>Desktop Proofing Viewer</span> when you click a link that is set to open in a new browser tab or window.</p> <p>This setting is in effect for all interactive <span>proofs</span> you open.</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">Open within the <span>proofing viewer</span></td> 
       <td>Links always open within the <span>Desktop Proofing Viewer</span> and you can <span>proof</span> the linked content. </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Open in the browser</td> 
       <td>Links always open within the browser, not in a <span>proofing viewer</span>. You are not able to <span>proof</span> the linked content.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">Ask me every time</td> 
       <td> <p>You are prompted each time whether you want to open the link within the <span>Desktop Proofing Viewer</span> or in the browser. If you open the link within the <span>Desktop Proofing Viewer</span>, you can <span>proof</span> the linked content. If you open the link in the browser, you are not able to <span>proof</span> the linked content.</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>This setting affects only the <span>proof</span> you have open.</p> </td> 
      </tr> 
     </tbody> 
    </table> </li> <!--
    Background color (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.
   --> 
   <li> <p><span class="bold">Clear cache</span>: Clears the browser cache data that might be saved with an interactive <span>proof</span> you are viewing. This enables content such as pop-ups (that can be blocked by browser cache data) to display in the <span>Desktop Proofing Viewer</span>.</p> <p>The data that is cleared includes the HTTP cache (such as images to be reused after the next page refresh) and the web storage data cache (such as cookies and data that identifies users).</p> <p>This setting affects only the <span>proof</span> you have open.</p> </li> 
  </ul> </li> 
</ol>

