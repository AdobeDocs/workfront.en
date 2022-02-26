---
filename: view-remove-link-to-object
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: View: remove link to an object in a column
description: Some objects that you display in a view link to the Details page of the object, by default. For example, the column that displays the Name of a project is a link to the project; the column that displays the Name of a user is a link to the user's profile page.
---

# View: remove link to an object in a column

Some objects that you display in a view link to the Details page of the object, by default. For example, the column that displays the Name of a project is a link to the project; the column that displays the Name of a user is a link to the user's profile page.

You can remove this link using text mode in columns that display in all views.

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

## Example: Remove the link to a task from the Task Name column in a task view:

<ol> 
 <li value="1">Go to a list of tasks.</li> 
 <li value="2"> <p>From the <span class="bold">View</span> drop-down menu, click <span class="bold">New View</span> to create a new view.</p> <p>Or</p> <p>Click <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
      the 
     <span class="bold">Edit icon</span> 
     <img src="assets/edit-icon.png"> 
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     the 
    <span class="bold">Edit icon</span> 
    <img src="assets/edit-icon.png"> 
   </MadCap:conditionalText> to edit an existing view, then select the view.</p> </li> 
 <li value="3"> <p>Click <span class="bold">Add Column</span> to add a new column.</p> <p>Or</p> <p>Click an existing column with a link to an object.</p> </li> 
 <li value="4">Click <span class="bold">Switch to Text Mode</span>.</li> 
 <li value="5">Hover over the text mode area, and click <span class="bold">Click to edit text</span>.</li> 
 <li value="6"> <p>Remove the text you find in the <span class="bold">Text Mode</span> box, and replace it with the following code:</p><pre>displayname=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><span class="bold">valueexpression={name}</span><br>valueformat=Compound</pre> 
  <div class="tips" data-mc-autonum="<b>Tips: </b>"> <span class="autonumber"><span><b>Tips: </b></span></span> 
   <p> You can use similar code for other objects by doing adjusting the following:</p> 
   <ul> 
    <li> <p>Replace the <span class="bold">valuefield</span> line of the code with <span class="bold">valueexpression</span> and keep the same name included in curly brackets after the equal sign.</p> </li> 
   </ul> 
   <ul> 
    <li> <p>Eliminate all the lines that start with <code>link.</code> from the original text of the column. For example, eliminate all the following lines:</p><pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre> </li> 
   </ul> 
  </div> </li> 
 <li value="7">Click <span class="bold">Save</span>, then <span class="bold">Save View</span>.</li> 
</ol>

