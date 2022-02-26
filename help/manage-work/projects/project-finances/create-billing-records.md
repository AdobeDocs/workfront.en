---
filename: create-billing-records
navigation-topic: financials
title: Create billing records
description: In addition to setting up revenue and tracking expenses, you can create billing records on a project for information that needs to be billed.
---

# Create billing records

In addition to setting up revenue and tracking expenses, you can create billing records on a project for information that needs to be billed.

You cannot create billing records for tasks. You can only create billing records for projects.

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
   <td> <p>Edit access to Projects and Financial&nbsp;Data</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Billing records overview

Billing records are created as attachments to a project and contain financial data from the project as well as some financial information for the tasks in a project.

Consider the following when planning to use billing records:

<ul> 
 <li>You create a billing record when you want to bill an amount of money related to the project to an external vendor or partner. In addition to billing a fixed amount to an external source, there are times when you need to bill out the amount of work on the project (from logged hours) to an external contractor, as well as the expenses incurred or the amount of fixed revenues. You can include all this information in the same billing record.</li> 
 <li> <p>Once a billing record is set to Billed it can not be edited. </p> <note type="important">
   This is important when your rates vary and you want to lock the revenue and expense information on your project. Adding it to a billing record and marking it as Billed prevents it from being updated when the rates update in your system. 
  </note> </li> 
 <li>A project with billing records that have been marked as Billed cannot be deleted.</li> 
</ul>

## Create a billing record

<ol> 
 <li value="1">Navigate to a project.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billing Records</span> in the left panel. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billing Records</span> in the left panel. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">This section might be located under <span class="bold">Show More</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">This section might be located under <span class="bold">Show More</span>.</p> </li> 
 <li value="3"> <p>With <span class="bold">Billing Record Details</span> selected in the left panel, click <span class="bold">New Billing Record</span>.</p> </li> 
 <li value="4"> <p>In the <span class="bold">New Billing Record</span> box that displays, specify the following information:</p> 
  <table cellspacing="0"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Description</td> 
     <td>This is a required field. Specify a description for the billing record, to reflect the purpose or the intent for this record.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Billing Status</td> 
     <td> <p>Select <span class="bold">Not Billed</span>, if this record has not been billed yet.</p> <p>Select <span class="bold">Billed</span> when the billing record is billed.</p> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Billing Date</td> 
     <td>Select the date for when this billing record is billed, by clicking the calendar icon.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">PO Number</td> 
     <td>If there is a PO Number associated with this billing record, specify this information in this field.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Invoice ID</td> 
     <td>If there is an Invoice associated with this billing record, specify this information in this field.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Additional Amount</td> 
     <td>Enter the fixed amount of your billing record. This is the amount you intend to bill an external customer, contractor or partner for this project. This amount cannot be modified after the status of the billing record is changed to Billed.</td> 
    </tr> 
   </tbody> 
  </table> </li> 
 <li value="5"> <p>(Optional) Under <span class="bold">Custom Forms</span>, select a billing records custom form that you want to add to the billing record.</p> <p>You (or another user with access to custom forms) must create a billing records custom form before you can select it here. Only active custom forms display in the list. For information about creating custom forms, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</p> <p>You can repeat this step to add other custom forms that you need for the billing record.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Save.</span></p> <p>The billing record is created. To include Billable Hours, Expenses and Fixed Revenues in the billing record, follow the steps outlined in the following sub-section.</p> </li> 
</ol>

## Include Billable Hours, Expenses and Fixed Revenues in a billing record

* [Include Billable Hours in a billing record](#including-billable-hours-in-a-billing-record) 
* [Include Billable Expenses in a billing record](#including-billable-expenses-in-a-billing-record) 
* [Include Fixed Revenues in a billing record](#including-fixed-revenue-in-a-billing-record)

### Include Billable Hours in a billing record

You can include hours that have been logged on tasks, issues, or the project in your billing records.  
If the user who logs the hours or their Primary Job Role is associated with a Billing per Hour Rate, the revenue from these hours is added to the billing record.

* [What hours can be added to a billing record](#understanding-what-hours-can-be-added) 
* [Add Hours to a billing record](#adding-hours-to-a-billing-record)

#### `What hours can be added to a billing record`

You can add hours to a billing record when the following conditions are met:

<ul> 
 <li>Tasks, issues, or the project have hours logged. </li> 
 <li> <p>The Hour Type of the hours logged is marked as Count as Revenue.</p> <p>For more information about Hour Types, see the article <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md" class="MCXref xref">Manage hour types</a>.</p> </li> 
 <li>All hours logged for issues or for the project can be added to a billing record if the user who logs the time has a Billing per Hour rate associated with them or their Primary Job Role. </li> 
 <li>If the hours are logged on a task, the task must have the following Revenue Type: 
  <ul>
   <li>The Revenue Type cannot be set to Not Billable.</li>
   <li>If the Revenue Type is set to User Hourly, the user who logs the time must have a Billing per Hour rate set in their profile. </li>
   <li>If the Revenue Type is set to Role Hourly, the Primary Role of the user who logs the time must have a Billing per Hour rate.<br><note type="note">
      You can override billing rates for job roles at the project level.
     <br>For more information about overriding job role billing rates, see the section "Overriding Job Role Billing Rates at the Project Level" in the article 
     <a href="../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md" class="MCXref xref">Overview of overriding Job Role Billing Rates and calculating Revenue on a project</a>.
    </note></li>
  </ul></li> 
 <li>If <span class="bold">Require time to be approved for this project</span> is checked under Project Settings, then the Project Owner must approve the hours logged.<br>For more information about requiring approval on project hours, see the article <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Require time to be approved for a project</a>. </li> 
</ul>

#### `Add Hours to a billing record`

To add billable hours to a billing record:

<ol> 
 <li value="1">Go to the project with the billing records.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billing Records</span> in the left panel. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billing Records</span> in the left panel. </p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">This section might be located under <span class="bold">Show More</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">This section might be located under <span class="bold">Show More</span>.</p> </li> 
 <li value="3">Click the <span class="bold">Description</span> of a billing record to open the <span class="bold">Billing Record Details</span> tab.</li> 
 <li value="4"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billable Hours</span> in the left panel.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billable Hours</span> in the left panel.</p> </li> 
 <li value="5">If there are hours that could be included in a billing record, click <span class="bold">Add Hours</span>.<br>The <span class="bold">Add Billable Hours</span> box opens. <br><note type="note">
    If there are no hours logged or if the hours logged do not meet the conditions required to be added to a billing record, the 
   <span class="bold">Add Hours</span> button does not display. For more information about what hours can be logged to a billing record, see the section 
   <a href="#understanding-what-hours-can-be-added" class="MCXref xref">What hours can be added to a billing record</a> in this article.
  </note></li> 
 <li value="6">Select the hour entries you want to include in the billing record, and click <span class="bold">Add Hours</span>. <br>The Actual Cost of the hours is added as the <span class="bold">Billable Hours</span> amount to the <span class="bold">Billing Record Total</span>. </li> 
 <li value="7">(Optional) Click <span class="bold">Billing Records Details</span> to review the <span class="bold">Billable Hours</span> and <span class="bold">Billing Record Total</span> amounts. <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    You can also see the billing record total in the header of the billing record. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   You can also see the billing record total in the header of the billing record. 
  </MadCap:conditionalText></li> 
</ol>

### Include Billable Expenses in a billing record

If you are adding Billable Expenses to the billing record, ensure the expenses on the tasks and the project are marked as Billable. Expenses that are not marked as Billable are not available to add in a billing record. For more information about adding expenses, see the article [Manage project expenses](../../../manage-work/projects/project-finances/manage-project-expenses.md).

To add billable expenses to a billing record:

<ol> 
 <li value="1">Go to the project with the billing records.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billing Records</span> in the left panel.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billing Records</span> in the left panel.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You might have to click <span class="bold">Show More</span>, then <span class="bold">Billing Records</span>. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You might have to click <span class="bold">Show More</span>, then <span class="bold">Billing Records</span>. </p> </li> 
 <li value="3">Click the <span class="bold">Description</span> of a billing record to open the <span class="bold">Billing Record Details</span> tab.</li> 
 <li value="4"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billable Expenses</span> in the left panel. </p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billable Expenses</span> in the left panel. </p> </li> 
 <li value="5">(Conditional) If you have added expenses to your tasks or the project and have marked them as Billable, click <span class="bold">Add Expenses</span>.<br><note type="note">
    If you have expenses but they are not marked as Billable, the 
   <span class="bold">Add Expenses</span> button does not display. Only billable expenses with an Actual Amount greater than zero are eligible to be included in a billing record.
  </note></li> 
 <li value="6">Select the billable expenses that are available to be added to the billing record, then click <span class="bold">Add Expenses</span>.<br>The Actual Amount of the expenses is added as the <span class="bold">Billable Expenses</span> amount to the <span class="bold">Billing Record Total</span>.</li> 
 <li value="7">(Optional) Click <span class="bold">Billing Records Details</span> to review the <span class="bold">Billable Expenses</span> and <span class="bold">Billing Record Total</span> amounts. <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    You can also see the billing record total in the header of the billing record. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   You can also see the billing record total in the header of the billing record. 
  </MadCap:conditionalText></li> 
</ol>

### Include Fixed Revenues in a billing record

You can add Fixed Revenues to your billing records if you have tasks that have Fixed Revenue available. No other types of task or project revenue is available to be added in a billing record. For more information about revenue types, see the [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md) section in [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

To add fixed revenues to a billing record:

<ol> 
 <li value="1">Go to the project with the billing records.</li> 
 <li value="2"> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billing Records</span> in the left panel.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <span class="bold">Billing Records</span> in the left panel.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You might have to click <span class="bold">Show More</span>, then <span class="bold">Billing Records</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You might have to click <span class="bold">Show More</span>, then <span class="bold">Billing Records</span>.</p> </li> 
 <li value="3">Click the <span class="bold">Description</span> of a billing record to open the <span class="bold">Billing Record Details</span> tab.</li> 
 <li value="4">Select the <span class="bold">Fixed Revenues</span> tab.</li> 
 <li value="5">If you have added fixed revenues to your tasks, click <span class="bold">Add Fixed Revenues</span>.<br><note type="note">
    If you have revenue amounts on tasks but they are not marked as "Fixed', the 
   <span class="bold">Add Fixed Revenue</span> button does not display.
  </note></li> 
 <li value="6">Select the tasks whose fixed revenues you want to include in the billing record, then click <span class="bold">Add Tasks</span>.<br>The <span class="bold">Fixed Revenue</span> amount of the tasks is added as the <span class="bold">Billable Revenues</span> amount to the <span class="bold">Billing Record Total</span>.</li> 
 <li value="7">(Optional) Click <span class="bold">Billing Records Details</span> to review the <span class="bold">Billable Revenues</span> and <span class="bold">Billing Record Total</span> amounts. <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    You can also see the billing record total in the header of the billing record. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   You can also see the billing record total in the header of the billing record. 
  </MadCap:conditionalText></li> 
</ol>

## Edit a billing record

After creating a billing record and including hours, expenses and revenues in the billing record, you can edit some information on the existing record, before it is marked as Billed.

<ol> 
 <li value="1"> <p>Go to the billing record.</p> </li> 
 <li value="2"> <p> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     With 
     <span class="bold">Billing Record Details</span> selected in the left panel
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    With 
    <span class="bold">Billing Record Details</span> selected in the left panel
   </MadCap:conditionalText><draft-comment>
    <span data-mc-conditions="QuicksilverOrClassic.Draft mode">
     <draft-comment>
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
       <span class="preview">and the <span class="bold">Overview</span> section expanded</span>
      </MadCap:conditionalText>
     </draft-comment>
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <span class="preview">and the <span class="bold">Overview</span> section expanded</span>
     </MadCap:conditionalText></span>
   </draft-comment><span data-mc-conditions="QuicksilverOrClassic.Draft mode">
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
     <span class="preview">and the <span class="bold">Overview</span> section expanded</span>
    </MadCap:conditionalText></span> <draft-comment>
    <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     , edit information in any available fields
    </MadCap:conditionalText>
   </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    , edit information in any available fields
   </MadCap:conditionalText>.</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Or</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Edit icon</span> <img src="assets/edit-icon.png"> in the upper-right corner, then edit information in any available fields.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Edit icon</span> <img src="assets/edit-icon.png"> in the upper-right corner, then edit information in any available fields.</p> <p>These fields are available for editing:</p> 
  <ul> 
   <li><span class="bold">Description</span> </li> 
   <li> <p><span class="bold">Billing Status</span> </p> <note type="tip">
      If you select 
     <span class="bold">Billed</span> for the Billing Status, the billing record cannot be edited, after you save your changes.
    </note> </li> 
   <li><span class="bold">Billing Date</span> </li> 
   <li><span class="bold">PO Number</span> </li> 
   <li><span class="bold">Invoice ID</span> </li> 
   <li><span class="bold">Additional Amount</span> </li> 
  </ul> <p>These fields are not available for editing:</p> 
  <ul> 
   <li><span class="bold">Billable Hours:</span> The total of the Actual Revenue of the hours included in the billing record. For more information about including hours in a billing record, see the section <a href="#including-billable-hours-in-a-billing-record" class="MCXref xref">Include Billable Hours in a billing record</a> in this article.</li> 
   <li><span class="bold">Billable Expenses</span>: The total of the Actual Amount of the billable expenses included in the billing record. For more information about including billable expenses in a billing record, see the section <a href="#including-billable-expenses-in-a-billing-record" class="MCXref xref">Include Billable Expenses in a billing record</a> in this article.</li> 
   <li><span class="bold">Billable Revenues</span>: The total of the Fixed Revenue of the tasks included in the billing record. For more information about including fixed revenues in a billing record, see the section <a href="#including-fixed-revenue-in-a-billing-record" class="MCXref xref">Include Fixed Revenues in a billing record</a> in this article.</li> 
   <li> <p><span class="bold">Billing Record Total</span>: The total of all billable amounts. This is calculated by the following formula:</p> <p><code>Included Hourly Revenue (Billable Hours) + Included Expenses (Billable Expenses) + Included Fixed Revenue (Billable Revenues) + Fixed Amount for Other Billable Items (Additional Amount)</code> </p> </li> 
  </ul> </li> 
 <li value="3">Click <span class="bold">Save</span><draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    <span class="bold"> Changes</span>
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <span class="bold"> Changes</span>
  </MadCap:conditionalText>.</li> 
</ol>

