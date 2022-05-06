---
filename: create-program
product-area: programs
navigation-topic: create and manage programs
title: Create a program
description: A program represents a collection of projects that share a common strategy, objective, or goal that transcends project boundaries. Programs cannot exist outside of a portfolio.
---

# Create a program

A program represents a collection of projects that share a common strategy, objective, or goal that transcends project boundaries. Programs cannot exist outside of a portfolio.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Business or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Portfolios and Programs </p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the portfolio</p> <p>After you create a program, you have Manage permissions to it, by default</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Create a program

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Do one of the following.

   * Create a program from the Programs area:

      1. Click **Programs** in the Main Menu.
      1. Click **New Program**.
      1. In the box that displays, type the name of an existing Portfolio in the **Select Portfolio** field.
      1. Type the name of the new program in the **Name** field.
      1. Click **Save**.

   * Create a program from the Portfolios area:

      1. Click **Portfolios** in the Main Menu, then click a portfolio.
      1. In the left panel, click **Programs**.
      1. Click the **New Program** drop-down menu, then **New Program**.

1. Specify the name for the Program in the **Untitled Program** field.

   The name can contain up to 255 characters.

1. (Optional) Click **Program Manager** in the header of the program to update it.

   >[!TIP]
   >
   >As the creator of the program, you are set as the Program Manager by default.

1. Click **Program Details** in the left panel. 
1. Double-click any field to update the information in the **Overview** area. 
1. Specify the following information:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Field</th> 
      <th>Description</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>Specify a description for the program.</p> <p>The description is displayed on the landing page of the program.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Program Manager</td> 
      <td> <p>Begin typing the name of the user who you want to act as the Program Manager, then click the user's name when it appears in the drop-down list. This is the same as the Program Owner. </p> <p>Tip: You can also update the Program Manager in the program header. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Group </td> 
      <td> <p>Add the name of a single group if the group owns the program or has responsibility for completing it. </p> <p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional and conditional) Click inside the **Add custom form** box to select a custom form for the portfolio and update the custom fields.

   >[!TIP]
   >
   >You must have program custom forms already created before you can attach them to programs.

1. (Optional) Double-click any field to update information on the custom form. 
1. Click **Projects** in the left panel, then **Add Projects** to add projects to the program.

   For information about adding projects to programs, see [Add a project to a program](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. Click **Save Changes**. 
1. (Optional) Click the **More menu** ![](assets/more-icon.png) next to the program name and click **Deactivate Program**.

   When you deactivate a program, the program no longer displays in a list of program when users try to add it to a project. You can still access the program from the Programs area.

## Program header overview

You can find limited information about the program in its header.

The following information displays in the header of a program:

##

<table cellspacing="0" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Header Information</td> 
   <td> <p><strong>Notes</strong> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Breadcrumb with the name of the portfolio</td> 
   <td>You can access the portfolio that the program belongs to from the header of the program. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name of the program</td> 
   <td>You can edit the program name in the header.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name of the object type and activation status</td> 
   <td>The word "Program" displays in a green outline when you view a program. The word "Deactivated" displays next to it and the outline is gray if the program is not marked as Active. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">The actions area of the program </td> 
   <td> <p>Click any of the following to access more information or editing options for the program:</p> 
    <ul> 
     <li>The star icon to add the program to your list of Favorites</li> 
     <li> <p>The More menu <img src="assets/qs-more-menu.png"> to do one of the following: </p> 
      <ul> 
       <li>Edit the program</li> 
       <li>Deactivate it. When a program is deactivated, you can no longer associate it with projects at the project level. </li> 
       <li> <p>Delete it. Deleting the program does not delete the projects in the program. It removes the association of the projects with the program. </p> </li> 
       <li>Share it with others</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Percent Complete</td> 
   <td> <p>You cannot edit the Percent Complete of the program in the header. This information is updated from the projects in the program. By default, the percent complete of the program is an average of the percent complete values of the projects in a Current and Approved status that belong to the program.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Program Manager</td> 
   <td> <p>You can edit the Program Manager in the header. This is the same as the Program Owner. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Planned Completion Date</td> 
   <td>You cannot edit the percent complete of the program in the header. The percent complete of the program is an average of the percent complete of the projects in the header. The projects represented here are projects with a status of Current and Approved. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Active Projects Condition</td> 
   <td>This is a calculation of what percentage of projects in the program have the Condition set as On Target, At Risk, or In Trouble. The projects represented here are projects with a status of Current and Approved. </td> 
  </tr> 
 </tbody> 
</table>

## Move a program

You can add existing programs to a portfolio. Because programs cannot exist in two different portfolios, adding an existing program permanently moves it from one portfolio to another.

For more information, see [Add an existing program to a portfolio](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
