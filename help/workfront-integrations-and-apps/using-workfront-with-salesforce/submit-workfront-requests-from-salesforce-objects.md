---
filename: submit-workfront-requests-from-salesforce-objects
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Submit Adobe Workfront requests from Salesforce objects
description: After installing Adobe Workfront for Salesforce, you can submit Workfront requests from Salesforce Opportunities and Accounts. This functionality exists in both the Classic and Lightning Experience frameworks.
---

# Submit *Adobe Workfront* requests from Salesforce objects

After installing *Adobe Workfront* for Salesforce, you can submit *Workfront* requests from Salesforce Opportunities and Accounts. This functionality exists in both the Classic and Lightning Experience frameworks.

## Access requirements

You must have the following access to use the functionality described in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <p>[Insert any access level configurations needed] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: Edit access to Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: Edit access to Documents
      </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[Insert any access level configurations needed] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: Edit access to Documents
     </MadCap:conditionalText></p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront administrator</em>. For information on <em>Workfront administrators</em>, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>group administrator</em>. For more information on <em>group administrators</em>, see <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Group administrators</a>.</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>[Insert permissions needed and specify the object] <draft-comment>
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        Example: View access or higher on Documents
       </MadCap:conditionalText>
      </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       Example: View access or higher on Documents
      </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[Insert permissions needed and specify the object] <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
      Example: View access or higher on Documents
     </MadCap:conditionalText></p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

To submit a *Workfront* request from a Salesforce Opportunity or Account ensure that you have the following in your environment:

<ul> 
 <li> Your <em>Workfront administrator</em> has installed <em>Workfront</em> for Salesforce.<br>For more information about installing <em>Workfront</em> for Salesforce, see <a href="../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md" class="MCXref xref">Install Adobe Workfront for Salesforce</a></li> 
 <li> Your <em>Workfront administrator</em> has added the <em>Workfront</em> section to your Opportunity and Account page layouts.<br>For more information about adding the <em>Workfront</em> section to a page layout, see <a href="../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md" class="MCXref xref">Configure the Adobe Workfront section for Salesforce users</a>.</li> 
 <li> <p>You have a <em>Workfront</em> account and you can log in to it from the <em>Workfront</em> section inside your Opportunity or Account. <br>Once you log in, you can see the New Requests tab where you can start entering requests.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;<img style="font-size: small;width: 350;height: 327;" src="assets/salesforce-new-requests-tab-350x327.png" alt="salesforce_new_requests_tab.png"></p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">&nbsp;<img style="font-size: small;width: 350;height: 327;" src="assets/salesforce-new-requests-tab-350x327.png" alt="salesforce_new_requests_tab.png"></p> </li> 
</ul>

## Submit *Workfront* requests from Salesforce

1. Go to an Opportunity or Account in Salesforce. 
1. Go to the *Workfront* section.
1. In the `New Requests` tab, select a request type in the `Select a Request Type` drop-down menu.

   You can see the same request queues that you have access to see in *Workfront*.&nbsp;

1. Start filling out the available fields for your request.

   Submitting a request from Salesforce is identical to submitting a request in the *Workfront* web application.

   Continue to follow the steps described in [Create and submit Adobe Workfront requests](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Click `Submit`.

## View *Workfront* requests

<ol> 
 <li value="1">Go to an Opportunity or Account in Salesforce.</li> 
 <li value="2"> <p>Go to the <span class="bold"><em>Workfront</em></span> section.</p> <note type="note">
   Depending on how your 
   <em>Workfront administrator</em> configured this section, it might have a different name.
  </note> </li> 
 <li value="3"> <p>Select the <span class="bold">Submitted Requests</span> tab.<br></p> <p>You can view all the requests that you or others have submitted from this Opportunity or Account in this tab.Requests that are submitted to this request queue in the web application do not display in this list in Salesforce.</p> <note type="note">
   Requests that are submitted to this request queue in the web application do not display in this list in Salesforce.
  </note> <p> <img src="assets/salesforce-submitted-requests-350x58.png" alt="salesforce_submitted_requests.png" style="width: 350;height: 58;"> </p> <p>You can view the following information about the submitted requests:</p> 
  <ul> 
   <li>Requests Name (in the Subject&nbsp;column)</li> 
   <li>Reference Number</li> 
   <li>Request&nbsp;Type</li> 
   <li>Status</li> 
   <li>Submitted on&nbsp;Date</li> 
   <li>Requested by Name</li> 
   <li>Assigned to Name<br>When this information is updated in <em>Workfront</em>, it is also updated in this list.&nbsp;</li> 
  </ul> </li> 
 <li value="4"> <p>(Optional) Click the name of the request to open it in <em>Workfront</em>.&nbsp;</p> <p>On the Summary panel <img src="assets/summary-panel-icon.png">, notice the <span class="bold">Integrations</span> indicator that signifies that this issue originated in Salesforce and is currently linked to an item there.&nbsp;</p> </li> 
 <li value="5"> <p>(Optional) Click <span class="bold">Go to Salesforce</span> to access the Opportunity or Account where the issue originated.</p> <note type="note">
   The Go to Salesforce link is visible to all 
   <em>Workfront</em> users who can view the issue. You must have a Salesforce account to be able to go to the Salesforce Opportunity or Account where the issue was logged.&nbsp;
  </note> </li> 
</ol>

