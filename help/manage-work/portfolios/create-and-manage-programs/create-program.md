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
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Business</span> or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Portfolios and Programs </p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the portfolio</p> <p>After you create a program, you have Manage permissions to it, by default</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Create a program

<ol> Click the Main Menu icon in the upper-right corner of Adobe Workfront. Do one of the following. Create a program from the Programs area: Click Programs in the Main Menu. Click New Program. In the box that displays, type the name of an existing Portfolio in the Select Portfolio field. Type the name of the new program in the Name field. Click Save. Create a program from the Portfolios area: Click Portfolios in the Main Menu, then click a portfolio. In the left panel, click Programs. Click the New Program drop-down menu, then New Program. 
 <li value="3"> <p>Specify the name for the Program in the <span class="bold">Untitled Program</span> field.</p> <p>The name can contain up to 255 characters.</p> </li> (Optional) Click Program Manager in the header of the program to update it. Tip: As the creator of the program, you are set as the Program Manager by default. 
 <li value="5"> Click Program Details in the left panel. </li> 
 <li value="6"> Double-click any field to update the information in the Overview area. </li> 
 <li value="7"> <p>Specify the following information:</p> 
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
     <td> <p>Begin typing the name of the user who you want to act as the Program Manager, then click the user's name when it appears in the drop-down list. This is the same as the Program Owner. </p> Tip: You can also update the Program Manager in the program header. </td> 
    </tr> Group Add the name of a single group if the group owns the program or has responsibility for completing it. You can make sure you are selecting the right group by hovering over it and clicking the information icon that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators. 
   </tbody> 
  </table> </li> (Optional and conditional) Click inside the Add custom form box to select a custom form for the portfolio and update the custom fields. Tip: You must have program custom forms already created before you can attach them to programs. 
 <li value="9">(Optional) Double-click any field to update information on the custom form. </li> 
 <li value="10"> <p> Click Projects in the left panel, then Add Projects to add projects to the program. </p> <p>For information about adding projects to programs, see <a href="../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md" class="MCXref xref">Add a project to a program </a>.</p> </li> Click Save Changes. (Optional) Click the More menu next to the program name and click Deactivate Program. When you deactivate a program, the program no longer displays in a list of program when users try to add it to a project. You can still access the program from the Programs area. 
</ol>

## Program header overview

You can find limited information about the program in its header.

The following information displays in the header of a program:

##  

Header Information Notes Breadcrumb with the name of the portfolio You can access the portfolio that the program belongs to from the header of the program. Name of the program You can edit the program name in the header. Name of the object type and activation status The word "Program" displays in a green outline when you view a program. The word "Deactivated" displays next to it and the outline is gray if the program is not marked as Active. The actions area of the program Click any of the following to access more information or editing options for the program: The star icon to add the program to your list of Favorites The More menu to do one of the following: Edit the program Deactivate it. When a program is deactivated, you can no longer associate it with projects at the project level. Delete it. Deleting the program does not delete the projects in the program. It removes the association of the projects with the program. Share it with others Percent Complete You cannot edit the Percent Complete of the program in the header. This information is updated from the projects in the program. By default, the percent complete of the program is an average of the percent complete values of the projects in a Current and Approved status that belong to the program. Program Manager You can edit the Program Manager in the header. This is the same as the Program Owner. Planned Completion Date You cannot edit the percent complete of the program in the header. The percent complete of the program is an average of the percent complete of the projects in the header. The projects represented here are projects with a status of Current and Approved. Active Projects Condition This is a calculation of what percentage of projects in the program have the Condition set as On Target, At Risk, or In Trouble. The projects represented here are projects with a status of Current and Approved. 

## Move a program

You can add existing programs to a portfolio. Because programs cannot exist in two different portfolios, adding an existing program permanently moves it from one portfolio to another.

For more information, see [Add an existing program to a portfolio](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
