---
filename: filter-information-wf-goals
product: workfront-goals
navigation-topic: goal-management
title: Filter information in Adobe Workfront Goals
description: You can view goals that you or anyone else added in Adobe Workfront Goals. For information about creating goals, see Create goals in Adobe Workfront Goals. When viewing goals, you can filter information in Workfront Goals to view only goals that are important to you.
---

# Filter information in Adobe Workfront Goals

You can view goals that you or anyone else added in&nbsp;Adobe Workfront Goals. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md). When viewing goals, you can filter information in Workfront Goals to view only goals that are important to you.

## Access requirements

You must have the following access to perform the actions described in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Adobe Workfront Goals</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>View or higher access to&nbsp;Goals</p> <p>Note:  <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> Object permissions View or higher permissions on goals For information about sharing goals, see Share a goal in Adobe Workfront Goals. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

You must have the following before you can start:

* A Layout Template that includes the Goals area in the Main&nbsp;Menu.

## Overview of filters in&nbsp;Workfront Goals

>[!NOTE]
>
>To efficiently find and focus on the right goals, we recommend that you use filters in Workfront Goals. This allows you to display the correct information before you start managing goals that are important to you. By default, Workfront Goals displays all goals in the system.

You can locate and filter for goals in several sections of the&nbsp;Goals area in&nbsp;Workfront:

* Goal List 
* Graphs
* Goal Alignment
* Pulse

>[!TIP]
>
>You cannot filter information in the Check-in section. Only active goals for whose progress you are responsible display in this section.

For information about sections of the Goals area, see [Overview of the Adobe Workfront Goals sections](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>You can configure filters for one section and they remain persistent when moving to another section of Workfront Goals.

Consider the following when working with filters in Workfront Goals:

* You can create and apply a filter without saving it, or you can save a filter to reuse at a later time.

  The following scenarios exist:

  * When you save a filter, it becomes the default filter for you every time you log in to Workfront Goals. 
  * When you apply a filter without saving it, you can revert to the original lists by refreshing your page.

* You can only view and apply filters you created. Filters created by other users display only for those users. 
* You cannot share filters you created with other users.

## Create and apply a filter in Workfront Goals

The process for creating filters is the same for any section of Workfront Goals.

You can create a filter from scratch or edit one of the built-in filters.

<ol> 
 <li value="1"> <p>Go to the Workfront Goals. </p> <p>For information about accessing Workfront Goals, see <a href="../../workfront-goals/goal-management/access-goals-in-wf-goals.md" class="MCXref xref">Access and open goals in Adobe Workfront Goals </a></p> <p>By default, the Goal List section displays. </p> </li> 
 <li value="2"> <p>Click <span class="bold">Filter </span>in the upper-right corner of the list. </p> <p> <img src="assets/filter-icon-and-label.png"> </p> <p>By default, Workfront applies the <span class="bold">All</span> filter which displays all goals in your system. </p> <note type="tip">
   You cannot edit or delete the All filter.
  </note> </li> 
 <li value="3"> <p>Do one of the following:</p> 
  <ul> 
   <li> <p>Click any of the following predefined filters to display goals only for the following owners:</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">All</td> 
       <td>All goals in your system, regardless of who created them, what the time period for them is, or who the owner is. This is the default filter and you cannot edit it. </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Personal</td> 
       <td>The goals for which you are the owner.</td> 
      </tr> 
      <tr> 
       <td role="rowheader">My teams</td> 
       <td> <p>The goals for which any of your teams is selected as the owner. </p> <note type="tip">
         No goals display when you are not assigned to any teams. 
        </note> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">My groups</td> 
       <td>The goals for which any of your groups is selected as the owner. </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Company</td> 
       <td> <p>The goals associated with your organization. </p> 
        <div class="tip_one-tip-with_bullets" data-mc-autonum="<b>Tip: </b>">
         <span class="autonumber"><span><b>Tip: </b></span></span> 
         <p>In Adobe Workfront Goals, the Company filter displays the goals for which your organization is selected as the owner. </p> 
         <p>You cannot search for companies using this field. Only your organization who is the owner of your Workfront instance is selected by default. </p> 
        </div> </td> 
      </tr> 
     </tbody> 
    </table> </li> 
  </ul> 
  <ul> 
   <li> <p>Hover over the name of a filter, then click the <span class="bold">Edit</span> icon <img src="assets/edit-icon.png"> next to its name to customize it and add specific names of users, teams, groups, or the name of your organization, then select it when they appear on the list. </p> </li> 
  </ul> 
  <ul> 
   <li> <p>Click <span class="bold">New Filter</span> to create a new filter, then select from the following options to customize the new filter:</p> 
    <table cellspacing="0"> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td role="rowheader">Period</td> 
       <td>Select a time period in the drop-down menu. You can select multiple time periods. </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Status</td> 
       <td> <p>Select a status in the drop-down menu from the following options:</p> 
        <ul> 
         <li> <p>Active</p> </li> 
         <li> <p>Draft</p> </li> 
         <li> <p>Inactive</p> </li> 
         <li> <p>Closed</p> </li> 
        </ul> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Progress</td> 
       <td> <p>Select a progress in the drop-down menu from the following options: </p> 
        <ul> 
         <li> <p>In Trouble</p> </li> 
         <li> <p>At Risk</p> </li> 
         <li> <p>On Target</p> </li> 
        </ul> </td> 
      </tr> 
      <tr> 
       <td role="rowheader">Owner</td> 
       <td> <p>Start typing the name of an owner, then select it when it appears in the list. </p> <p>You can type the names of users, teams, groups, or the name of your organization or you can select from predefined options. </p> <p>The following predefined filter options always refer to the user who is currently logged in: </p> 
        <ul> 
         <li> <p><span class="bold">Me</span>: Displays goals where you are the owner.</p> </li> 
         <li> <p><span class="bold">My Home Team</span> and <span class="bold">All My Teams</span>: Displays goals where either your Home Team or any of your teams are designated as the owner. </p> <note type="tip">
           No goals display when you are not assigned to any teams. 
          </note> </li> 
         <li> <p><span class="bold">My Home Group</span> and <span class="bold">All&nbsp;My&nbsp;Groups</span>: Displays goals where either your Home Group or any of your groups are designated as the owner.</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </li> 
  </ul> </li> 
 <li value="4">(Optional) Click <span class="bold">Reset</span> to clear out all the fields you have selected and start building the filter from scratch. </li> 
 <li value="5"> <p>(Optional) Click <span class="bold">Apply</span> to apply the filter without saving. </p> <p>The filter displays in the <span class="bold">Unsaved</span> area of the filter builder as <span class="bold">New Filter</span>. </p> <p>You cannot rename an unsaved filter. </p> <p>Unsaved filters are removed from the Goals area next time you log out of Workfront and log back in.</p> <note type="tip">
   You can have only one unsaved New Filter at one time. 
  </note> </li> 
 <li value="6"> <p>Click <span class="bold">Save</span> to save the filter to use it later, then add a name for the filter in the <span class="bold">Add filter name </span>field and click <span class="bold">Done</span>. </p> <p>This saves the filter in the <span class="bold">Saved</span> section of the filter builder. You can use this filter in the future. </p> <p>The last saved and applied filter displays by default next time you log back in to Workfront</p> </li> 
 <li value="7"> <p>(Optional) Click the <span class="bold">left-pointing arrow</span> next to <span class="bold">New Filter</span> to exit the filter builder and return to the list of filters. </p> </li> 
 <li value="8"> <p>(Optional) Hover over the name of a filter, click the <span class="bold">More</span> menu, then click&nbsp;<span class="bold">Delete</span>, then&nbsp;<span class="bold">Delete</span>. This deletes the filter and you cannot recover it. </p> <note type="tip">
   You cannot delete any of the predefined filters.
  </note> </li> 
 <li value="9"> <p>Click the <span class="bold">X icon</span> in the upper-right corner of the filter builder to close the filter builder.</p> <p>The name of the filter currently applied displays to the right of the Filter icon, in the upper-right corner of the goals list. </p> <p>The list of goals is filtered by your filter criteria. </p> </li> 
 <li value="10"> <p>(Optional) If you want to view the filtered out results, click&nbsp;<span class="bold">Show them</span> in the list of goals in the Goal List or the Goal Alignment section. </p> <p> <img src="assets/show-them-link-on-filtered-items-goal-list-350x109.png" style="width: 350;height: 109;"> </p> <p>The filter name is outlined in yellow to indicate that it is being ignored.</p> <p> <img src="assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png" style="width: 350;height: 118;"> </p> <note type="tip">
   Displaying items that are hidden by filters is not possible in the Graphs and Pulse sections. 
  </note> </li> 
 <li value="11"> <p>Click&nbsp;<span class="bold">Reapply filter</span> to apply the filter and omit the items you displayed in the previous step. </p> </li> 
</ol>

&nbsp;

###  

