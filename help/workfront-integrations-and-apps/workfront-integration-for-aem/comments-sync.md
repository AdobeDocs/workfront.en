

# `Workfront Tools for AEM User Guide : Comments Sync`

Creates a comment under an asset representing the `Adobe Workfront` Note object.

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
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> <!--
   Adobe Workfront license* Review or higher
  --> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>You must have a license to Adobe Experience Manager</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the object the note is attached to</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

* You must install Workfront Tools for Adobe Experience Manager before you can use it to auto publish assets.

  For instructions, see [Workfront Tools for AEM User Guide: Installation Guide 1.x.x](../../workfront-integrations-and-apps/workfront-integration-for-aem/installation-guide.md)

## Create Event Subscriptions for Note Objects

<ol> 
 <li value="1"> <p>Navigate to <span class="uitext">Tools → Cloud Services → Workfront Tools Configuration</span>. Select the configuration and click <span class="uitext">Properties</span>.<br><img src="assets/properties-config-350x280.png" style="width: 350;height: 280;"></p> <p> <img src="assets/wf-tools-350x286.png" style="width: 350;height: 286;"> </p> </li> 
 <li value="2"> <p>Select the <span class="uitext">Event Subscriptions</span> tab. Under the <span class="uitext">Create a new event subscription</span> menu, select <span class="uitext">create </span>from the Event dropdown and under the Object dropdown select <span class="uitext">note</span>. This we create a workflow step that listens for comments added to <span>Workfront</span> linked documents and add the comment in AEM. </p> <p> <img src="assets/event-subs-350x238.png" style="width: 350;height: 238;"> </p> <p> <img src="assets/create-note-event-350x225.png" style="width: 350;height: 225;"> <br> </p> </li> 
 <li value="3"> <p>Test the Create Note Event</p> 
  <ol> 
   <li value="1"> <p>Navigate to a linked document in <span>Workfront</span> and leave a comment in the Updates tab.</p> </li> 
   <li value="2"> <p>Navigate to the same linked document in AEM. Once the document is selected, navigate to the Timeline menu in the left navigation and select <span class="uitext">Comments</span>. Here you should see you synced comments from <span>Workfront</span>.</p> <p> <img src="assets/update-stream-comment-350x225.png" style="width: 350;height: 225;"> </p> <p> <img src="assets/699826215-350x225.png" style="width: 350;height: 225;"> </p> </li> 
  </ol> </li> 
</ol>

