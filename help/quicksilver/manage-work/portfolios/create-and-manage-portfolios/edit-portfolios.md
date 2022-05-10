---
filename: edit-portfolios
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Edit portfolios
description: You can edit information on portfolios that you have created, or that other users have created if they shared them with you.
---

# Edit portfolios

You can edit information on portfolios that you have created, or that other users have created if they shared them with you.

You can edit a portfolio in the portfolio page or you can edit portfolios in a list.

## Access requirements

You must have the following access to perform the steps in this article: 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses overview*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Portfolios</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to portfolios in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md" class="MCXref xref">Grant access to portfolios</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a portfolio</p> <p> For information about granting permissions to portfolios, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md" class="MCXref xref">Share a portfolio </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Edit portfolios

1. Go to the **Main Menu**.
1. Click **Portfolios**, then click the name of a portfolio to open it. 
1. (Optional) To edit limited information about the portfolio, click **Portfolio Details** in the left panel.

   ![](assets/portfolio-details-tab-nwe-350x163.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the note below will also be true for Edit Portfolio box)</p>
   -->

   >[!NOTE]
   >
   >Depending on how your Workfront administrator or Group administrator modified your Layout Template, the fields in the Portfolio Details area might be rearranged or not display. For information, see [Customize the Details view using a layout template](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   To edit information in the Details section, do the following:

   1. (Optional) Click the **Collapse All** icon in the upper-right corner to collapse all areas. 
   1. (Optional and conditional) When an area is collapsed, click the **right-pointing arrow** ![](assets/right-pointing-arrow.png) next to each area to expand the area you want to edit. 
   1. For information about the fields visible in the Portfolio Details section, continue with editing the portfolio in the Edit Portfolio box as described below. 
   1. (Optional) If there are no custom forms attached to the portfolio, start typing the name of a form in the **Add custom form** field, select it when it displays in the list, then click&nbsp;**Save Changes**. 
   1. (Optional) Click the **Export** icon ![](assets/export.png) to export the Overview and custom forms information to a PDF file, then click **Export**. Select from the following:

      * Select all (displays only when there is at least one custom form attached)
      * Overview
      * The name of one or multiple custom forms

      The PDF file downloads to your computer.

      ![](assets/export-portfolio-details-box-with-export-button-350x368.png)

      For more information, see [Export custom forms and object details](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

1. To edit all information about one or more portfolios do one of the following:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this might have to be split in two sections if the single edit and the bulk edit won't come at the same time for portfolios)</p>
   -->

   * Click the **More** menu next to the portfolio name, then **Edit.**

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will change in NWE with a new Edit Portfolio UI)</p>   
     -->

   * Go to a list of portfolios and select one or more portfolio that you want to edit, then click the **Edit** icon ![](assets/edit-icon.png) at the top of the list.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to split into another section when they release the new Edit Portfolio UI)</p>   
     -->

   The **Edit Portfolio** dialog box displays.

   ![](assets/edit-portfolio-box-classic-350x224.png)

   All portfolio fields are available in the Edit Portfolio box and are grouped by the areas listed in the left panel. 

1. Consider specifying information in any of the following sections:

   * [Overview](#overview)
   * [Custom Forms](#Custom%C2%A0F)
   * [Comment](#comment)

### Overview {#overview}

1. Begin editing a portfolio as described above.
1. Click **Overview** and specify the following fields:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;note below is drafted: drafted till they release new Edit Portfolio boxes)</p>
   -->

   <!--
   <note type="note">
   Depending on how your Workfront administrator or Group administrator sets up our Layout Template, the fields in the Edit Portfolio box might be rearranged or not display. For information, see
   <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md" class="MCXref xref">Customize the Details view using a layout template</a>.
   </note>
   -->

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>Update the name of the portfolio. </p> <p>Tip: This is not available when you selected more than one portfolio. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>Type a description for the Portfolio to indicate what is unique about it. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Portfolio Manager</td> 
      <td> <p>Start typing the name of a user that you want to indicate as the portfolio manager, then select it when it appears in the list. This is the same as the Portfolio Owner. This is the person who can oversee the work defined in the projects of the portfolio and can approve the Business Case.</p> <p>Important: When you designate someone as the Portfolio Manager, they automatically gain&nbsp;Manage permissions to the portfolio, the programs and the projects in the portfolio. </p> <p>Tip: You can quickly update the portfolio manager in the portfolio header. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group</td> 
      <td> <p>Add the name of a single group if the group is associated with the portfolio or has responsibility for completing it. </p> <p>Tip:  <p>When accessing the Group field from the Portfolio Details page, do the following: </p> <p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> <p>This option is not available in the Edit Portfolio box. </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Alignment Scorecard</p> </td> 
      <td> <p>Select the alignment scorecard that you want to use from the drop-down list. A scorecard is used to measure how well a project aligns with the established criteria of a Portfolio often reflecting an organization’s mission, values, and strategic goals. For more information, see <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Apply a scorecard to a project and generate an Alignment Score</a> and <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Create a scorecard</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is Active</td> 
      <td> <p> Select this checkbox if you want the portfolio to be active. Other users can find active portfolios and attach them to projects when creating or editing projects. Inactive portfolios cannot be attached to projects. This is enabled by default.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Save Changes** or continue editing the following sections.

### Custom&nbsp;Forms

1. Begin editing the portfolio as described above. 
1. Click the **Add Forms** drop-down menu to select a custom forms and add it to the portfolio.

   You must create portfolio custom forms before they are available to add.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the portfolio itself. For information about setting permissions on sections of a custom form, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Update any fields in the custom forms, then click **Save Changes** or continue with the following section.

### Comment {#comment}

1. Begin editing a portfolio as described above.
1. Click&nbsp;**Comment**.

   ![](assets/comment-box-edit-portfolio-classic-350x227.png)

1. Add a comment in the **Post an update to the portfolio** field.
1. (Optional) Click the **People** icon to add a user or a team to the comment. 
1. (Optional)&nbsp;Click the **Lock** icon to lock the comment and make it private to only users in your company. 
1. Click&nbsp;**Save Changes**.

#### 

