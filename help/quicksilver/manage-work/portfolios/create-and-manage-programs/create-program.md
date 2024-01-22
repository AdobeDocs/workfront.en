---
product-area: programs
navigation-topic: create and manage programs
title: Create a program
description: A program represents a collection of projects that share a common strategy, objective, or goal that transcends project boundaries. Programs cannot exist outside of a portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6ec353c2-2241-47c2-8c59-1d8ddc43781e
---
# Create a program

<!-- Audited: 1/2024 -->

A program represents a collection of projects that share a common strategy, objective, or goal that transcends project boundaries. Programs cannot exist outside of a portfolio.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>New: Any</p><p>Or</p><p>Current: [!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard] </p><p>Or </p><p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>After you create a program, you have [!UICONTROL Manage] permissions to it, by default.</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Create a program

1. Click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, or (if available), click the **[!UICONTROL Main Menu]** icon ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png) in the upper-left corner.

1. Do one of the following.

   * Create a program from the [!UICONTROL Programs] area:

      1. Click **[!UICONTROL Programs]** in the Main Menu.
      1. Click **[!UICONTROL New Program]**.
      1. In the box that displays, type the name of an existing Portfolio in the **[!UICONTROL Select Portfolio]** field.
      1. Type the name of the new program in the **[!UICONTROL Name]** field.
      1. Click **[!UICONTROL Save]**.
   * Create a program from the [!UICONTROL Portfolios] area:

      1. Click **[!UICONTROL Portfolios]** in the [!UICONTROL Main Menu], then open a portfolio.
      1. In the left panel, click **[!UICONTROL Programs]**.
      1. Click the **[!UICONTROL New Program]** drop-down menu, then **[!UICONTROL New Program]**.


1. (Conditional) If you have created the program from a portfolio, specify the name for the Program in the **[!UICONTROL Untitled Program]** field.

   The name can contain up to 255 characters.

1. (Optional) Click **[!UICONTROL Program Manager]** in the header of the program to update it.

   >[!TIP]
   >
   >As the creator of the program, you are set as the Program Manager by default.

1. Click **[!UICONTROL Program Details]** in the left panel.
1. Double-click any field to update the information in the **[!UICONTROL Overview]** area.

You can specify the following information:

   <table style="table-layout:auto"> 
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
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td> <p>Specify a description for the program.</p> <p>The description is displayed on the landing page of the program.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Program Manager]</td> 
      <td> <p>Begin typing the name of the user who you want to act as the Program Manager, then click the user's name when it appears in the drop-down list. This is the same as the [!UICONTROL Program Owner]. </p> <p>Tip: You can also update the Program Manager in the program header. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Group] </td> 
      <td> <p>Add the name of a single group if the group owns the program or has responsibility for completing it. </p> <p>You can make sure you are selecting the right group by hovering over it and clicking the [!UICONTROL information] icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> 
       <div data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
        <img src="assets/group-details-widget-programs-350x268.png" style="width: 350;height: 268;"> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional and conditional) Click inside the **[!UICONTROL Add custom form]** box to select a custom form for the portfolio and update the custom fields.

   >[!TIP]
   >
   >You must have program custom forms already created before you can attach them to programs.

1. (Optional and conditional) If you are adding a custom form, click any field on the custom form to update information in that field.
1. Click **[!UICONTROL Save Changes]**.
1. Click **[!UICONTROL Projects]** in the left panel, then **[!UICONTROL Add Projects]** to add projects to the program.

   For information about adding projects to programs, see [Add a project to a program](../../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

1. Click **[!UICONTROL Save Changes]**.
1. (Optional) Click the **[!UICONTROL More menu]** ![](assets/more-icon.png) next to the program name and click **[!UICONTROL Deactivate Program]**.

   When you deactivate a program, the program no longer displays in a list of program when users try to add it to a project. You can still access the program from the [!UICONTROL Programs] area.

## Program header overview

You can find some information about the program in its header.

The following information displays in the header of a program:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Header Information</td> 
   <td> <strong>Notes</strong> </td> 
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
   <td>The word "Program" displays with an orange icon when you view a program. The word "[!UICONTROL Deactivated]" displays next to it and the outline is gray if the program is not marked as [!UICONTROL Active]. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">The actions area of the program </td> 
   <td> <p>Click any of the following to access more information or editing options for the program:</p> 
    <ul> 
     <li>The star icon to add the program to your list of Favorites</li> 
     <li> <p>The [!UICONTROL More] menu <img src="assets/qs-more-menu.png"> to do one of the following: </p> 
      <ul> 
       <li>Edit the program</li> 
       <li>Deactivate it. When a program is deactivated, you can no longer associate it with projects at the project level. </li> 
       <li> <p>Delete it. Deleting the program does not delete the projects in the program. It removes the association of the projects with the program. </p> </li> 
       <li>Share it with others</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Percent Complete]</td> 
   <td> <p>You cannot edit the [!UICONTROL Percent Complete] of the program in the header. This information is updated from the projects in the program. By default, the percent complete of the program is an average of the percent complete values of the projects in a [!UICONTROL Current] or [!UICONTROL Approved] status that belong to the program.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Program Manager]</td> 
   <td> <p>You can edit the Program Manager in the header. This is the same as the [!UICONTROL Program Owner]. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Completion Date]</td> 
   <td>You cannot edit the Planned Completion Date of the program in the header.  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Active Projects Condition]</td> 
   <td>This is a calculation of what percentage of projects in the program have the [!UICONTROL Condition] set as [!UICONTROL On Target], [!UICONTROL At Risk], or [!UICONTROL In Trouble]. The projects represented here are projects with a status of [!UICONTROL Current] and [!UICONTROL Approved]. </td> 
  </tr> 
 </tbody> 
</table>

## Move a program

You can add existing programs to a portfolio. Because programs cannot exist in two different portfolios, adding an existing program permanently moves it from one portfolio to another.

For more information, see [Add an existing program to a portfolio](../../../manage-work/portfolios/create-and-manage-programs/move-program.md).
