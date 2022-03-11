---
filename: add-results-to-goals
product: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Add results to goals in Adobe Workfront Goals
description: Results measure the progress of a goal. Without associating results, activities, or aligned goals to a goal, you cannot activate the goal and you cannot record progress on it.
---

# Add results to goals in `Adobe Workfront Goals`

Results measure the progress of a goal. Without associating results, activities, or aligned goals to a goal, you cannot activate the goal and you cannot record progress on it.

## Access requirements

You must have the following:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Request</span> or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td> <p>You must purchase an additional license for the <span>Adobe Workfront Goals</span> to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Adobe Workfront Goals</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Goals or higher</p> <p>Note:  <p>If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> Object permissions Manage permissions to the goal For information about sharing goals, see Share a goal in Adobe Workfront Goals. 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

You must have the following before you can start:

* A Layout Template that includes the Goals area in the Main&nbsp;Menu.
* An existing goal.

  For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>A goal cannot have more than a total of 50 activities, results, or aligned goals.

## Add a result to a goal

<ol> 
 <li value="1">Go to the goal for which you want to add a result and click the name to open the <span class="bold">Goal&nbsp;Details</span> panel.</li> 
 <li value="2"> <p>Click <span class="bold">Add results</span>.</p> <p> <img src="assets/add-result-inside-goal-details-highlighted-350x145.png" style="width: 350;height: 145;"> </p> </li> 
 <li value="3">Start typing the result you want to achieve in the <span class="bold">Result</span> field. This is the name of the result and it displays wherever the goal displays. </li> 
 <li value="4"> <p>(Optional) If you want to set the Result Owner as someone other than yourself, click your name in the <span class="bold">Owner</span> field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.</p> <note type="note">
   You cannot assign a team or group as a result owner.
  </note> </li> 
 <li value="5"> <p>In the <span style="font-weight: bold;">Value</span> drop-down menu, select the type of value that you want to measure your success by. </p> <p> <img src="assets/results-value-initial-target-boxes-350x49.png" style="width: 350;height: 49;"> </p> <p>Select from the following options:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">#</td> 
     <td>Number value</td> 
    </tr> 
    <tr> 
     <td role="rowheader">%</td> 
     <td>Percentage value</td> 
    </tr> 
    <tr> 
     <td role="rowheader">$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , € , ₹, ฿, MYR, ₪ </td> 
     <td>Currency values</td> 
    </tr> 
   </tbody> 
  </table> <p> <p>For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value. </p> <note type="tip">
    The result Type is always Metric and cannot be edited. 
   </note> </p> </li> 
 <li value="6"> <p>In the <span style="font-weight: bold;">Initial</span> field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. </p> </li> 
 <li value="7">In the <span style="font-weight: bold;">Target</span> field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.</li> 
 <li value="8"> <p>Click <span class="bold">Save</span>.</p> <p>The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result. </p> </li> 
</ol>

