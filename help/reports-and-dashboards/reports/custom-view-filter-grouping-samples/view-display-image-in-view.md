---
filename: view-display-image-in-view
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: View: display an image instead of a string in a column
description: You can replace the name of an object in a view with an image using text mode. You can also add a link to the image that can open the object it replaces.
---

# View: display an image instead of a string in a column

You can replace the name of an object in a view with an image using text mode. You can also add a link to the image that can open the object it replaces.

>[!NOTE]
>
>Images appear in their actual resolution so try to use small images.

![](assets/replace-project-name-with-image-and-link-350x125.png)

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
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Example: Replace the name of a project in a project view with an image:

<ol> 
 <li value="1"> <p>Upload an image to a web site or server external of <em>Adobe Workfront</em>. You must be able to access the image using your web browser.</p> 
  <div class="tips" data-mc-autonum="<b>Tips: </b>">
   <span class="autonumber"><span><b>Tips: </b></span></span> 
   <ul> 
    <li> <p>Every browser type is different but all are capable of displaying URLs.</p> </li> 
    <li> <p>Avoid using images that are uploaded to <em>Workfront</em>. Because images stored in <em>Workfront</em> are not publicly available and have an access key that expires after a period of time, these images stop displaying in the view over time.</p> </li> 
    <li> <p>An image saved on your computer does not have an inherent URL. Find a site that provides image hosting and host your image there. Your organization might already have such a site.</p> </li> 
   </ul> 
  </div> </li> 
 <li value="2"> <p>Using your web browser, go to the image that you saved.</p> </li> 
 <li value="3"> <p>Obtain the image's URL by doing the following:</p> 
  <ol> 
   <li value="1"> <p>Right-click and select <span class="bold">Copy image location</span>, or <span class="bold">Get link</span>, depending on your browser. You now have the URL for that specific image and can paste it from your clipboard.</p> </li> 
   <li value="2"> <p>Ensure that everyone with that link has permissions to view the image by just going to the link and they don't need a login to access it.</p> </li> 
  </ol> </li> 
 <li value="4"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Go to a project, click the 
    <span class="bold">More</span> menu 
    <img src="assets/more-icon-45x33.png" style="width: 45;height: 33;"> next to the name of the project, then click 
    <span class="bold">Edit</span>.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Go to a project, click the 
   <span class="bold">More</span> menu 
   <img src="assets/more-icon-45x33.png" style="width: 45;height: 33;"> next to the name of the project, then click 
   <span class="bold">Edit</span>.
  </MadCap:conditionalText> </li> 
 <li value="5">In the <span class="bold">URL</span> field, add the link to the image.</li> 
 <li value="6">Navigate to a project view in a list or report and customize the view.</li> 
 <li value="7">Click the header of the column for the <span class="bold">Project Name</span>, then click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="8"> <p>Add the following code to the column to the existing code:</p> <p><code>displayname=Link Project</code> </p> <p><code>image.name=Link Project</code> </p> <p><code>image.valuefield=URL</code> </p> <p><code>link.linkproperty.0.name=projectID</code> </p> <p><code>link.linkproperty.0.value=ID</code> </p> <p><code>link.lookup=link.edit</code> </p> <p><code>link.page=/view</code> </p> <p><code>link.valuefield=objCode</code> </p> <p><code>link.valueformat=val</code> </p> <p><code>textmode=true</code> </p> <p><code>type=image</code> </p> <p><code>valueformat=</code> </p> <p>The image you selected replaces the Project Name in the project view and the image is a link to the project.</p> </li> 
 <li value="9">Click <span class="bold">Save View</span>.</li> 
</ol>

