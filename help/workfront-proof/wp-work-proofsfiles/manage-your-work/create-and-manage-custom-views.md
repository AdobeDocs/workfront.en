---
filename: create-and-manage-custom-views
product: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Create and Manage Custom Views in Workfront Proof Proof
description: You can create custom views of your files and proofs to list the items you want in the ways you want them displayed. You can also export the information in your Custom view as a report (in CSV, comma separated value, file format).
---

# Create and Manage Custom Views in Workfront Proof Proof

>[!IMPORTANT]
>
>This article refers to functionality in the standalone product Workfront Proof. For information on proofing inside Adobe Workfront, see [Proofing](../../../review-and-approve-work/proofing/proofing.md).

You can create custom views of your files and proofs to list the items you want in the ways you want them displayed. You can also export the information in your Custom view as a report (in CSV, comma separated value, file format).

>[!NOTE]
>
>Custom views are available only on Select and Premium plans. Please contact our Sales team for a quote.x

## Creating a Custom View

When you create a custom view, you can choose:

* Whether to include proofs, files, or both
* Which columns are displayed
* Which column&nbsp;to sort by
* The sort order for the&nbsp;column (ascending or descending)
* Which types of filters to use for determining what information is included in the view

After the custom view is&nbsp;created, it is&nbsp;available to use immediately. The name of the new view is&nbsp;also included in the drop-down menu under the heading My custom views (below the Standard views).

To create a custom view:

<ol start="1"> 
 <li value="1">Go to the <span class="bold">Views</span> page.</li> 
 <p>For more information about views, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md" class="MCXref xref">Manage Items on the Views Page in Workfront Proof</a>.</p> 
 <li value="2">Do either of the following, depending on whether you want to create a new custom view from scratch, or create a new custom view based on an existing standard view: 
  <ul> 
   <li>To create a new custom view based on an existing standard view: From the drop-down menu, select the existing standard view you want to use as the basis for your new custom view. Click the <span class="bold">View Settings</span> icon, then click <span class="bold">Copy</span> to new custom view.</li> 
   <p><img src="assets/proof-custom-view-icon.png"></p> 
   <li><p>To create a new custom view from scratch: Click the <span class="bold">New View</span> icon.</p></li> 
   <p><img src="assets/proof-newview.png"></p> 
  </ul></li> 
 <li value="3"> <p>In the <span class="bold">Details</span> section, specify the following information:</p> 
  <ul> 
   <li><span class="bold">Name</span> (required): The name for the new view. Use a unique name so users can easily find the custom view in the drop-down menu on the Views.</li> 
   <li><span class="bold">Items</span>: Select whether you want both proofs and file, proofs only, or files only included in the view. By default, both proofs and files are included.</li> 
  </ul> </li> 
 <li value="4">In the <span class="bold">Columns</span> section, determine which columns you want to include in the custom view. 
  <ol style="list-style-type: lower-alpha;"> 
   <li value="1">Click the Right arrow icon. </li> 
   <p><img src="assets/proof-view-rightarrow.png"></p> 
  </ol> 
  <ol style="list-style-type: lower-alpha;" data-mc-continue="true"> 
   <li value="2">Double-click the name of the selected column.</li> 
   <p>You must select at least one column, and a column can be added only once.</p> 
   <li value="3">Select a column from the <span class="bold">Available columns</span> area that you want to include in the new view.</li> 
   <p>The columns are moved from the <span class="bold">Available columns</span> list to the <span class="bold">Selected columns</span> list.</p> 
   <p>You can select from the standard columns, or you can choose Custom fields and Decision Reasons to be columns in your custom view. (If you have these configured in your account, they appear under the standard list of Available columns area.)</p> 
   <p>Standard columns you can include</p> 
   <table cellspacing="15"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th><span class="bold">Column</span></th> 
      <th><span class="bold">Function</span></th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td><span class="bold">Active stage name</span></td> 
      <td>Name of the active stage in the&nbsp;automated workflow.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Comments</span></td> 
      <td>The number of comments received.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Counter</span></td> 
      <td>Shows a number of the proof that has been uploaded on your account (you have to have a proof counter option enabled in Account Settings).</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Created</span></td> 
      <td>The date and time the item was created.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Creator</span></td> 
      <td>The user who created the item.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Date added to proof</span></td> 
      <td>The date you were&nbsp;added to the proof.&nbsp;</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Deadline</span></td> 
      <td>The deadline for the whole proof.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Decisions</span></td> 
      <td>The number of decisions given out of the expected number (e.g. 0 of 1, 1 of 1, etc.)</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Downloads</span></td> 
      <td>The number of times the original file has been downloaded.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Filename</span></td> 
      <td>The name of the file or proof.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Folder</span></td> 
      <td>The folder containing the item.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Last activity</span></td> 
      <td>The date and time of the last activity on the item.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Latest decision on</span></td> 
      <td>The date and time of the last decision made.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">My deadline</span></td> 
      <td>Your own deadline on the proofs where you are explicitly added as a Reviewer/Approver (if applied).</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Owner</span></td> 
      <td>The owner of the item.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Owner country</span></td> 
      <td>The country registered in the system for the owner of the proof.&nbsp;</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Parent proof</span></td> 
      <td>The name of the parent proof.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Progress</span></td> 
      <td><p>Progress bar.&nbsp;Displays proofs that are not yet Started, Opened, Commented on, or Decided on.</p><p>This information is not sorted on.</p></td> 
     </tr> 
     <tr> 
      <td><span class="bold">Proof name</span></td> 
      <td>The name of the proof.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Proof type</span></td> 
      <td><p>The type of proof: Static file, Static web page, Interactive web (.zip upload), Interactive web page (https), Video, Audio, and Other. </p><p>Combined proofs are identified as "Combined proof type." File type of the proof.</p></td> 
     </tr> 
     <tr> 
      <td><span class="bold">Size on disk</span></td> 
      <td><p>File size of the proof as it relates to the disk usage quota.</p><p>This information provided for the current version of the proof. If there is no current version, it is for the most recent version.</p></td> 
     </tr> 
     <tr> 
      <td><span class="bold">Stage deadlines</span></td> 
      <td>Deadline of stages in&nbsp;the automated workflow.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Stage name</span></td> 
      <td>Name of each&nbsp;stage in the automated workflow. This includes past stages, active stages, and future stages.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">State</span></td> 
      <td>Active, Locked, Draft, or Submitted.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Status</span></td> 
      <td>Pending, Changes required, Approved with changes, Approved, or Not relevant.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Tags</span></td> 
      <td>Any tags attached to the item.</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Upcoming stage names</span></td> 
      <td> Name of each stage that has not yet started&nbsp;in the automated workflow. </td> 
     </tr> 
     <tr> 
      <td><span class="bold">Version counter</span></td> 
      <td> The number of versions of the item.&nbsp;</td> 
     </tr> 
     <tr> 
      <td><span class="bold">Proof version number</span></td> 
      <td><font size="2">The version number of the proof.</font></td> 
     </tr> 
    </tbody> 
   </table> 
   <li value="4">(Optional) Do either of the following to move the column to the <span class="bold">Selected columns</span> area so that it is included in the new view: 
    <ul data-mc-continue="true"> 
     <li>Reorder any columns in the <span class="bold">Selected columns</span> list.</li> 
     <p>The order in which columns are shown in the <span class="bold">Selected columns</span> list determines the order in which the columns are displayed in the custom view.</p> 
     <p>The columns are visible in the <span class="bold">Selected columns</span> list in the order that you added them from the <span class="bold">Available columns</span> list.</p> 
     <p>To reorder a column in the <span class="bold">Selected columns</span> list, select the name of the column and drag it either up or down in the list.</p> 
    </ul> 
    <ul data-mc-continue="true"> 
     <li>Remove a column from the <span class="bold">Selected columns</span> list, by clicking the name of the selected&nbsp;column, then clicking the <span class="bold">Left</span> arrow. Alternatively, you can double-click the name of the selected column (the column is&nbsp;moved back to the <span class="bold">Available columns</span> list).</li> <note type="note">
      A&nbsp;column can be added only once. For example, if you move Comments column from Available to Selected columns list, the name of this column will disappear from Available columns list.
     </note> 
    </ul></li> 
  </ol></li> 
 <li value="5">In the <span class="bold">Sorting</span> section, specify the following information: 
  <ul> 
   <li><span class="bold">Sort by:</span>&nbsp;Use the Sorting tab if you want to set a particular order in which items are listed in your custom view. If you do not select a column for sorting, the default is No column - that is, no special sort column or order.</li> 
   <p>Only the columns you selected on the Columns tab are included in the Sort by column drop down list.</p> 
   <li><span class="bold">Ascending or Descending:</span> Select whether you want to sort the column either ascending or descending by default.</li> 
  </ul></li> 
 <li value="6">Use the <span class="bold">Filters</span> section to define one or more criteria for selecting items to include in your Custom view. Filters are especially helpful if you want to use your custom view as a report.</li> <note type="note">
  To include all&nbsp;items in your custom view, skip the 
  <span class="bold">Filters</span> section.
 </note> 
 <p>Available filters</p> 
 <p> 
  <ul> 
   <li><span class="bold">Field:</span>&nbsp;Select the Field for this filter (Comments is the default field.) The Field list contains all the Standard fields (as in the Columns tab). The list is not limited to the columns you selected for display.</li> 
   <li><span class="bold">Operator:</span>&nbsp;The Operators available for the filter depend on the type of Field you selected. Select an Operator that shows the relationship between the Field and the value field. You will fill in this information later.</li> 
   <li><span class="bold">Value:</span>&nbsp;Select or enter your chosen value in this Field, according to the field and the Operator you selected. Depending on the Operator you chose, there might be one Value field or two or none. &nbsp;See the examples below.</li> 
   <li> <p><span class="bold">Filters are applied using the following logic:</span>&nbsp;Filter criteria between different fields will use the AND operator. Multiple filter criteria using the same field will use the OR operator for the same field.</p> <p>If you want to see only proofs with zero comments,select the following values:</p> 
    <ul> 
     <li>Field: Comments</li> 
     <li>Operator: Equals</li> 
     <li>Value field: 0</li> 
    </ul> <p> If you want to see only proofs with two or more comments, select the following values:</p> 
    <ul> 
     <li>Field: Comments</li> 
     <li>&nbsp;Operator: Greater or equal to</li> 
     <li>Value field: 2</li> 
    </ul> <p> If you want to see only proofs with between 1 and 4 comments, select the following values: </p> 
    <ul> 
     <li>Field: Comments</li> 
     <li>Operator: Between</li> 
     <li>Value field (first field): 1</li> 
     <li> <p>Value field (second field): 4</p> <p>You can change a filter that you have added to your Custom view without any problems or remove it by clicking the cross icon next to the setup filter if needed.</p> <p>Because the Field list is not limited to the columns you selected on the Columns tab, take care when you create a filter that includes a column you did not select for display in your custom view. For example, the following filter for the view will select all proofs with a Version counter value of 2 or more: 
       <ul> 
        <li>Field = Version counter</li> 
        <li>Operator = Greater or equal to</li> 
        <li><p>Value field = 2</p><note type="note">
          You can change a filter that you have added to your Custom view without any problems or remove it by clicking the cross icon next to the setup filter if needed.
         </note></li> 
       </ul></p> </li> 
    </ul> </li> 
  </ul> </p> 
 <li value="7">In the <span class="bold">Sharing</span> section, select which users in your account will be able to see your Custom view.</li> 
 <p>Custom views are specific to the user who creates them. By default the new Custom view is visible only for its creator; however, you can choose to share your custom view by choosing one of the following options:</p> 
 <ul> 
  <li><span class="bold">Only you can see this custom view</span> (default): Select this option if you want the custom view to be available only to you.</li> 
  <li><span class="bold">All users can see this custom view</span>: Select this option to make the custom view available to all users on your account.</li> 
  <li><span class="bold">Select users that can see this custom view</span>: Select this option to make the custom view available only to specific users.</li> 
  <p>Begin typing the name or the email address of the user who you want to have access to the custom view, then click the name when it appears in the drop-down list.</p> 
  <p>If you choose to not share your view with other users at this point, you can do so later by editing the custom view.</p> 
 </ul> 
 <li value="8"> <p>Click <span class="bold">Create</span>.</p> </li> 
 <p>The&nbsp;Custom view is displayed&nbsp;and is&nbsp;available on the Views page. For more information about views, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md" class="MCXref xref">Manage Items on the Views Page in Workfront Proof</a>.</p> 
</ol>

## Editing Custom Views

You can edit a custom view easily. To edit a custom view:

<ol> 
 <li value="1">Go to the <span class="bold">Views</span> page.<br>For more information about views, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md" class="MCXref xref">Manage Items on the Views Page in Workfront Proof</a>.</li> 
 <li value="2">Click on the Views button (1)</li> 
 <li value="3">Select the view you want to edit from the drop-down menu.<br><img src="assets/proof-view-edit.png"></li> 
 <li value="4">Click the&nbsp;<span class="bold">View Options</span> button, then click <span class="bold">Edit view</span>.<br><img src="assets/proof-view-options.png"><br>The Edit Custom View page is displayed.</li> 
 <li value="5">Click on the Actions menu. (3)<br>This button is available only if you include the Proof name column in your view.</li> 
 <li value="6">Select Edit view from the menu.&nbsp;(4)&nbsp;<br><img src="assets/editing-custom-view-2-350x258.png" alt="editing_custom_view_2.png" style="width: 350;height: 258;"></li> 
 <li value="7">The Edit custom view page&nbsp;is displayed.</li> 
</ol>

![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)

`NOTE`If you edit your Custom view, the&nbsp;columns in Selected columns list will arrange in an alphabetical order automatically. You will need to rearrange them if needed before updating the view.

## Copying Custom Views

The Copy view function lets you easily make a copy of an existing custom view. This is really useful, for example, if you want to set up separate views for all your designers, with each view being the same except for the proof owner (designer).

To copy a custom view:

<ol> 
 <li value="1">Go to the <span class="bold">Views</span> page.<br>For more information about views, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md" class="MCXref xref">Manage Items on the Views Page in Workfront Proof</a>.</li> 
 <li value="2">Click on the <span class="bold">Views</span> button. (1)</li> 
 <li value="3">Select your Custom view from the list. (2)</li> 
 <li value="4">Click the <span class="bold">Actions</span> menu. (3)<br>This button is available only if you include the Proof name column in your view.</li> 
 <li value="5">Select Copy from the menu. (4)<br><img src="assets/copying-custom-view-350x258.png" alt="copying_custom_view.png" style="width: 350;height: 258;"></li> 
 <li value="6">In the Copy custom view page, all the original settings are populated.&nbsp;Modify the Custom view as per your choice and click the <span class="bold">Copy view</span> button. You will be taken to your new view immediately.<br><img src="assets/copy-custom-view-page-350x542.png" style="width: 350;height: 542;"></li> 
</ol>

## Sharing Custom Views

The Share view function lets you share a view with other users in your account if you did not already select them on the Sharing section&nbsp;for the view. When you share a custom view with other users, the view appears in their My custom views section of the Views drop down menu.

To share a custom view with other users:

1. Go to the `Views` page.  
   For more information about views, see [Manage Items on the Views Page in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Click on the `Views` button (1)
1. Select your Custom View from the list (2)
1. Click the `Actions` menu. (3)  
   This button is available only if you include the Proof name column in your view.

1. Select Share view from the menu (4)
1. The Edit custom view page will come up.
1. In the Sharing section elect the users you want to share the view with and click  `Update view`.

&nbsp; ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)

## Exporting Custom Views to CSV Files

To export the data from a custom view to a CSV file:

<ol> 
 <li value="1">Go to the <span class="bold">Views</span> page.<br>For more information about views, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md" class="MCXref xref">Manage Items on the Views Page in Workfront Proof</a>.</li> 
 <li value="2">Click on the <span class="bold">Views</span> button. (1)</li> 
 <li value="3">Select your Custom View from the list. (2)</li> 
 <li value="4">Click the <span class="bold">Actions</span> menu. (3)<br>This button is available only if you include the Proof name column in your view.</li> 
 <li value="5">Select Export to CSV from the menu. (4)<br><img src="assets/exporting-custom-view-350x258.png" alt="exporting_custom_view.png" style="width: 350;height: 258;"><br>In a separate browser window, 'Generating report: 100%' appears plus the number of records (the number of items included in the report from your custom view)</li> 
 <li value="6">(Conditional) If a security message appears indicating that the report download is currently blocked, click&nbsp;to allow the download to proceed.</li> 
 <li value="7">Click <span class="bold">Save</span> when the File Download window appears asking if you want to open or save the file.</li> 
 <li value="8">Select a location on your computer and save the file.</li> 
</ol>

## Deleting Custom Views

You can delete a Custom view easily. To do this:

<ol> 
 <li value="1">Go to the <span class="bold">Views</span> page.<br>For more information about views, see <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md" class="MCXref xref">Manage Items on the Views Page in Workfront Proof</a>.</li> 
 <li value="2">Click on the <span class="bold">Views</span> button.</li> 
 <li value="3">Select your Custom view from the list</li> 
 <li value="4">Click the <span class="bold">Actions</span> menu. (3)<br>This button is available only if you include the Proof name column in your view.</li> 
 <li value="5">Select Delete from the menu. (4)<br><img src="assets/deleting-custom-view-350x258.png" alt="deleting_custom_view.png" style="width: 350;height: 258;"></li> 
 <li value="6">Click <span class="bold">Delete</span>&nbsp;(5) to confirm that you want to delete the current Custom view<br><img src="assets/delete--1--350x187.png" alt="delete__1_.png" style="width: 350;height: 187;"></li> 
 <li value="7">The default All items view is displayed and your deleted custom view no longer appears in the <span class="bold">Views</span> drop-down menu.</li> 
</ol>

