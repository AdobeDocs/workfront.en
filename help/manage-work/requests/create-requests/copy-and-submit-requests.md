

# Copy and submit requests

When you submit similar requests frequently you can copy an existing submitted request. In this case, you can copy an existing request, make minimal changes to it, and resubmit it as a new request.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Request</em> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

You must have a request that you or someone in your organization previously submitted to be able to copy it and resubmit it. If the request belongs to someone else, you must have at least access to View it to be able to copy and submit it as new.

## Considerations about copying and submitting requests as new

<ul> 
 <li> <p>You can only copy and submit submitted requests. You cannot copy drafted requests.</p> </li> 
 <li> <p>You can copy and submit requests you originally submitted, or requests that others submitted and you have access to at least&nbsp;View.</p> </li> 
 <li> <p>You always have access to copy and submit a copy of your own requests, unless someone removed your permissions to them.</p> </li> 
 <li> <p>The access to copy and submit requests originally submitted by others might be granted automatically to people in the same company when the creator of the request queue enables the <b>People from the same company will inherit the same permissions for all requests</b> in the Queue Details or Edit Project areas. Disabling this setting allows only the original requestor to view their own requests.</p> <p>For more information, see the following articles:</p> 
  <ul> 
   <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a> </p> </li> 
   <li> <p><a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a> </p> </li> 
  </ul> </li> 
 <li> <p>You can update the copy of the original request before resubmitting it as a new request.</p> </li> 
 <li> <p>If the following changes occur after the original request is submitted, you can no longer copy it and resubmit it:</p> 
  <ul> 
   <li> <p>The request queue was deleted.</p> </li> 
   <li> <p>The queue topic was deleted.</p> <note type="tip">
     If the queue topic was the only one in the request queue, you can still copy and submit the request and it will be saved under the request queue itself.
    </note> </li> 
   <li> <p>The request queue is no longer published as a Help Request Queue. For information, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>.</p> </li> 
   <li> <p>The Status of the project associated with the request queue is no longer Current.</p> </li> 
  </ul> </li> 
 <li> <p>You can copy and submit a copy of a converted request if the request was preserved in the conversion process. For more information, see <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Overview of converting issues in Adobe Workfront</a>.</p> <note type="tip">
   The copied request is not linked to a resolving object.
  </note> </li> 
</ul>

## Copy and submit requests

<ol> 
 <li value="1"> <p>Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <em>Adobe Workfront</em>, then click <span class="bold">Requests</span>.</p> </li> 
 <li value="2"> <p>(Conditional) If the Submitted section does not display by default, click <span class="bold">Submitted</span> in the left panel.</p> </li> 
 <li value="3"> <p>Locate the request that you want to copy and submit as new, and do one of the following:</p> 
  <ul> 
   <li> <p>Select it, then click the <span class="bold">Copy and submit as new</span> icon <img src="assets/copy-and-submit-as-new-requests-area-nwe.png"> in the upper-left corner of the Submitted requests list.</p> </li> 
   <li> <p>Click the <span class="bold">More</span> menu<img src="assets/more-icon.png"> to the right of the request name, then click&nbsp;<span class="bold">Copy and submit as new</span></p> <p>Or</p> <p>Right-click on the selected request, then click <span class="bold">Copy and submit as new</span>.</p> <p> <img src="assets/request-selected-more-menu-options-nwe-350x191.png" style="width: 350;height: 191;"> </p> <note type="tip">
     <span class="preview">When you do not have access to create issues, you receive a warning that your administrator restricted you from creating requests.</span> 
    </note> </li> 
  </ul> </li> 
 <li value="4"> <p>(Optional) Update the following information, if needed:</p> 
  <ul> 
   <li> <p><b>Request Type</b>: the request queue where the copied request is saved. By default, the copied request is saved to the request queue of the original request.</p> </li> 
   <li> <p><b>Topic Groups</b> and <b>Queue&nbsp;Topics</b>, if they are selected. The names or topic groups and queue topics are customized for your environment. By default, the copied request is saved to the topic groups and the queue topics of the original request.</p> <note type="tip">
     If the path changes from the path of the original request, then the creator of the request queue modified the queue.
    </note> </li> 
  </ul> </li> 
 <li value="5"> <p>(Optional) Update any information from the copied request. Depending on what fields the request queue creator enabled in the <span class="bold">New Issue Fields</span> section of the <span class="bold">Queue Details</span>&nbsp;subtab on the project, you might find&nbsp;any of the following fields:</p> 
  <div> 
   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><span class="bold">Subject</span> </td> 
      <td>Displays the name of the original request. Update it, if necessary.&nbsp;Otherwise, <em>Workfront</em> names the copied request <b>Copy of <Name of original request></b>. This is a mandatory field.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Description</span> </td> 
      <td>Displays the description of the original request. Update it, if necessary.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">URL</span> </td> 
      <td> <p>Displays the URL of the original request. Update it, if necessary.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Priority</span> </td> 
      <td> <p>Specify the priority of your request. The priority should define how fast you think this request should be resolved. The default&nbsp;options are:</p> 
       <ul> 
        <li>None</li> 
        <li>Low</li> 
        <li>Normal</li> 
        <li>High</li> 
        <li>Urgent</li> 
       </ul> <p>Your <em>Workfront administrator</em> can modify the names of priorities.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Severity</span> </td> 
      <td> <p>Specify the severity for your request. The severity should define the impact this request has on your work should it not be resolved in time. The default&nbsp;options are:</p> 
       <ul> 
        <li>Cosmetic</li> 
        <li>Causes Confusion</li> 
        <li>Bug with workaround</li> 
        <li>Bug with no workaround</li> 
        <li>Fatal error</li> 
       </ul> <p>Your <em>Workfront administrator</em> can modify the names of severities.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Primary Contact</span> </td> 
      <td>The Primary Contact of a request defaults to you, as you are the point person to address any questions pertaining to the request. However, you can change this to any other <em>Workfront</em> user.</td> 
     </tr> <draft-comment>
      <tr data-mc-conditions=""> 
       <td role="rowheader"><span>Assignments*</span> </td> 
       <td> <p>Indicate the name of an active user, job role, or a team that the request should be assigned to. </p> <note type="tip">
         You can specify only one team. 
        </note> <p>Depending on how the request queue was set up, you might be able to only assign the request to one or two types of resources, instead of all three. </p> <p>We recommend using Routing Rules for your Request Queues so that they can be automatically routed to the appropriate resources. </p> </td> 
      </tr>
     </draft-comment>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Assignments*</span> </td> 
      <td> <p>Indicate the name of an active user, job role, or a team that the request should be assigned to. </p> <note type="tip">
        You can specify only one team. 
       </note> <p>Depending on how the request queue was set up, you might be able to only assign the request to one or two types of resources, instead of all three. </p> <p>We recommend using Routing Rules for your Request Queues so that they can be automatically routed to the appropriate resources. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <note type="note"> 
        <p style="font-weight: normal;">* Depending on how the request queue was set up, you might be able to only assign one type of resource to the request (for example, users). If a routing rule is also associated to the request queue and it automatically routes the request to a different type of resource (for example, a team), your request is assigned to both the entity that you manually specify when submitting the request (users) and the resource specified in the routing rule (the team.)</p> 
        <p style="font-weight: normal;">For more information, see the following articles:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Create Routing Rules</a> <br> </p> </li> 
        </ul> 
       </note> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Planned Hours</span> </td> 
      <td> <p>Estimate how many hours it would take for this request to complete.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Planned Start Date</span> </td> 
      <td> <p>The date when work on this request should start.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Planned Completion Date</span> </td> 
      <td>The date when you would like for this request to be resolved.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Status</span> </td> 
      <td>The default status of a new request is "New." Your <em>Workfront administrator</em> might have changed the name of this&nbsp;status. You can also change the status to something else from this drop-down menu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span class="bold">Documents</span> </td> 
      <td> <p>Add documents to your request. The documents attached to the original request do not transfer to the copied request.</p> <note type="tip">
        Depending on how the request queue was set up, the Documents section might display before or after the custom fields.
       </note> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table> 
  </div> </li> 
 <li value="6"> <p>(Optional) Update any information in the custom forms attached, if needed.</p> 
  <div class="tips" data-mc-autonum="<b>Tips: </b>">
   <span class="autonumber"><span><b>Tips: </b></span></span> 
   <ul> 
    <li> <p>All custom forms attached to the original request and the values included in the custom fields transfer to the copied request. This includes fields that contain logic.</p> </li> 
    <li> <p>You cannot remove custom forms from the copied request.</p> </li> 
   </ul> 
  </div> </li> 
 <li value="7"> <p>Click&nbsp;<span class="bold">Submit</span>.</p> <p>The copied request is submitted as a new request in the request queue you specified.</p> </li> 
</ol>

