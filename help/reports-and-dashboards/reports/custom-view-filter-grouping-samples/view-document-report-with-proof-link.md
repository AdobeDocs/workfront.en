---
filename: view-document-report-with-proof-link
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: View: document report with link to a proof
description: In this document view, you can insert a link to a proof of the current version of the document.
---

# View: document report with link to a proof

In this document view, you can insert a link to a proof of the current version of the document.

![](assets/view-document-with-proof-link-350x92.png)

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## View a document report with link to a proof

To apply this view:

<ol> 
 <li value="1">Go to a list of documents.</li> 
 <li value="2">From the <span class="bold">View</span> drop-down menu, select <span class="bold">New View</span>.</li> 
 <li value="3">Click <span class="bold">Add Column</span>. </li> 
 <li value="4">Click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="5">Hover over the text mode area, and click <span class="bold">Click to edit text</span>.</li> 
 <li value="6"> <p>Remove the text you find in the <span class="bold">Text Mode</span> box, and replace it with the following code:</p> 
  <div> 
   <p><code>displayname=Proof Link</code> </p> 
   <p><code>shortview=true</code> </p> 
   <p><code>textmode=true</code> </p> 
   <p><code>valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")</code> </p> 
   <p><code>valueformat=HTML</code> </p> 
  </div> <note type="tip">
   Replace "Your domain" with your actual 
   <span>Workfront</span> domain. For example, if your company's 
   <span>Workfront</span> url is 
   <i>Company.my.workfront.com</i>, your domain is "Company."
  </note> </li> 
 <li value="7"> <p>Click&nbsp;<span class="bold">Save</span>, then&nbsp;<span class="bold">Save View</span>.</p> </li> 
 <li value="8"> <p>Type a name for the view, then click <span class="bold">Save View</span>.</p> </li> 
 <li value="9"> <p>(Optional) To ensure you display only documents with proofs, add a filter by doing the following:</p> 
  <ol> 
   <li value="1"> <p>Click the <span class="bold">Filter</span> drop-down menu, then click <span class="bold">New Filter</span>.</p> </li> 
   <li value="2"> <p>Click <span class="bold">Add a Filter Rule</span> and start typing Current Version, then select <span class="bold">Current Version Proof ID</span> when it displays in the list.</p> </li> 
   <li value="3"> <p>Select <span class="bold">Is Not Blank</span> for the filter modifier.</p> <p> <img src="assets/filter-current-version-proof-id-not-blank-350x67.png" style="width: 350;height: 67;"> </p> </li> 
   <li value="4"> <p>Click <span class="bold">Save Filter</span>, type the name of the filter, then click&nbsp;<span class="bold">Save Filter</span>.</p> </li> 
  </ol> </li> 
 <li value="10"> <p>Click the link in the Proof Link column to access the proof of the last version of the document.</p> </li> 
</ol>

