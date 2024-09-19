---
product-area: projects
navigation-topic: manage-projects
title: Require time to be approved for a project
description: Require time to be approved for a project
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
---
# Require time to be approved for a project

<!--audited: 08/2024-->

You can configure the project to require that the hours logged against the project are approved by the Project Owner. When configured in this way, hours must be first approved by the Project Owner before they can be eligible to be used on a billing record.   
For more information about billing records, see the article [Create billing records](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Enabling this option does not remove a timesheet approver's ability to approve time on the timesheet. If the Project Owner doesn't approve or reject time, a timesheet approver can still approve the time on a timesheet. 

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>To require time to be approved on the project:</p>
   <ul><li>New: Standard</li>
   <li>Current: Plan</li></ul>
   
   <p>To approve hours logged on a project:</p>
   <ul><li>New: Light or higher</li>
   <li>Review or higher</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects or higher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher</p>
  </tr> 
  <tr> 
   <td role="rowheader">Additional access</td> 
   <td> <p>You must meet at least one of the following conditions to approve time on a project:</p> 
    <ul> 
     <li>You are the Project Owner with the access and permissions specified above. In this case, you can do the following if one of the conditions below exists: 
      <ul>
       <li>If you have Manage permissions on the project, you can approve or reject hours logged on the project by any other user.</li>
       <li> If you have Contribute or View access to the project you will be able to approve or reject only the hours logged by you or any other user that reports you.<br></li>
      </ul></li> 
     <li>You have a Plan license with administrative access to Timesheets &amp; Hours. In this case:
      <ul>
       <li>You can approve or reject any hours on the projects you have at least permissions to View. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Require time to be approved for a project

To require project manager approval for hours on the project:

1. Go to the project where you want to require approval for hours.
1. Click the **More** icon ![](assets/more-icon.png) to the right of the project name, then click **Edit**.  
   The Edit Project dialog box displays.

1. In the **Project Settings** section, select **Require time to be approved for this project**. 
1. Click **Save**.  
   Now when time is logged and approved, those hours become locked and cannot be altered by the user who entered them on the project or the timesheet. Only a Workfront administrator can adjust the time recorded.

## Approve and reject time on a project

As a project manager, you can approve or reject hours that are logged for tasks, issues, or the project.

Approving the hours at the project level does not have any impact on the timesheet of any of the users who logged the hours. For example, the hours in the project may be approved by the project manager, but the timesheet is still yet to be approved by the manager of the user or the timesheet approver. 

If you set up a project to require approval on the hours logged, the project manager must approve the hours in order for them to be available to be included in a billing record for the project. For more information about creating billing records, see the article [Create billing records](../../../manage-work/projects/project-finances/create-billing-records.md).

To approve or reject hours on a project:

1. Go to the project.
1. Click the **Hours** area in the left panel. This might be located under the **Show More** area.   

1. The hours logged for issues, tasks, and the project display and should have a status of **Submitted**.  
   Click the box to the left of the hour entries to select the hours you want to approve.

1. Click the **Approve** icon ![](assets/approve-hours-icon.png) at the top of the hour list.  
   The status of the hours changes to **Approved**.  
   If you later reject the approved hours, the status of the hours changes to **Not Approved**.  
   When you include the approved hours in a billing record, the status of the hours changes to **Billed and Approved**. Hours added to a billing record cannot be deleted. For more information about creating billing records, see the article [Create billing records](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Optional) Click **Reject** icon ![](assets/reject-hours-icon.png) to reject the time entries on the project.  
   The status of the hours changes to **Rejected**.

   >[!NOTE]
   >
   >   If the hours you select are included in a Billing Record that has been marked as Billed or Billed and Approved, the Approve and Reject icons do not display. You can only approve hours that are not already billed in a Billing Record.

