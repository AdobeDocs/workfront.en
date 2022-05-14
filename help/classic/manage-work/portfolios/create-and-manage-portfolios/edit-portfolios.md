---
filename: edit-portfolios
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Edit portfolios
description: You can edit information on portfolios that you have created, or that other users have created if they shared them with you.
---

# Edit portfolios

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can edit information on portfolios that you have created, or that other users have created if they shared them with you.

You can edit a portfolio in the portfolio page or you can edit portfolios in a list.

## Access requirements

You must have the following access to perform the steps in this article: 

<table> 
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

1. Go to the **Projects** area in the Global Navigation Bar. 
1. Select the **Portfolios** tab, then  do one of the following:

   * Click the name of a portfolio to open it, then click **Portfolio Details**.

     ![](assets/portfolio-with-is-active-350x307.png)

   * Select one or more portfolios in the list, then click **Edit** to open the Edit Portfolio box.

     ![](assets/edit-portfolio-box-classic-350x224.png)

1. Consider updating the following fields in the Portfolio Details tab or the Edit Portfolio box: 

   <table> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>Update the name of the portfolio.</p> <p>Tip: This is not available in the Edit Portfolio box when you select more than one portfolio. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td> <p>Type a description for the Portfolio to indicate what is unique about it. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Portfolio Manager</td> 
      <td> <p>Start typing the name of a user that you want to indicate as the portfolio manager, then select it when it appears in the list. This is the same as the Portfolio Owner. This is the person who can oversee the work defined in the projects of the portfolio and can approve the Business Case.</p> <p>Important: When you designate someone as the Portfolio Manager, they automatically gain&nbsp;Manage permissions to the portfolio, the programs and the projects in the portfolio. </p> <p>&nbsp;</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Group</td> 
      <td> <p>Add the name of a single group if the group is associated with the portfolio or has responsibility for completing it. </p> </td> 
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

1. Click **Custom Forms**.
1. Select the custom form or forms that you want to associate with the portfolio. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. For more information about building custom forms, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). You can add up to ten custom forms to a portfolio. 
1. (Conditional)&nbsp;In the Portfolio&nbsp;Details box, click **Edit Custom Form** to update the fields on a custom form.

   >[!NOTE]
   >
   >Depending on how your Workfront administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the portfolio itself. For information about setting permissions on sections of a custom form, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. (Conditional) In the Edit Portfolio box, click **Comment**.

   ![](assets/comment-box-edit-portfolio-classic-350x227.png)

   Do the following:

   1. Add a comment in the **Post an update to the portfolio** field.
   1. (Optional) Click the **People** icon to add a user or a team to the comment. 
   1. (Optional)&nbsp;Click the **Lock** icon to lock the comment and make it private to only users in your company.

      After you save your changes, the comment you add displays in the portfolio's Updates tab and sends an email to the users included in it.

   >[!TIP]
   >
   >You cannot add a comment in the Portfolio&nbsp;Details tab.

1. (Conditional) Click&nbsp;**Save** in the Portfolio Details tab

   Or

   Click **Save Changes** in the Edit Portfolio box. 

1. (Optional) From the portfolio page, click the **Programs** tab to add programs to the portfolio.

   For information about creating programs, see [Create a program](../../../manage-work/portfolios/create-and-manage-programs/create-program.md). 

1. (Optional)&nbsp;From the portfolio page, click the **Projects** tab to add projects to the portfolio.

   For more information, see [Add projects to a portfolio](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Classic,QuicksilverOrClassic.Draft mode">
<h2>Edit portfolios in a list</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is drafted for right now, but it might change (especially for NWE) - keeping it to easily copy it to NWE if needed.)</p>
-->
<!--
<ol>
<li value="1"> <p>Go to a list of portfolios and select one or more portfolios that you want to edit, then click the <strong>Edit</strong> icon <img src="assets/edit-icon.png"> at the top of the list. </p> <p>The <strong>Edit Portfolio</strong> dialog box displays.</p> <p> <img src="assets/edit-portfolio-box-classic-350x224.png" style="width: 350;height: 224;"> </p> <p>All portfolio fields are available in the Edit Portfolio box and are grouped by the areas listed in the left panel. </p> </li>
<li value="2">Consider specifying information in any of the following sections:
<ul>
<li><a href="#overview" class="MCXref xref">Overview</a></li>
<li><a href="#Custom%C2%A0F" class="MCXref xref">Custom&nbsp;Forms</a></li>
<li><a href="#comment" class="MCXref xref">Comment</a></li>
</ul></li>
</ol>
<p><strong>Overview</strong></p>
<ol>
<li value="1">Begin editing a portfolio as described above.</li>
<li value="2"> <p>Click <strong>Overview</strong> and specify the following fields: </p>
<table>
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Name</td>
<td> <p>Update the name of the portfolio. </p> <note type="tip">
This is not available when you selected more than one portfolio.
</note> </td>
</tr>
<tr>
<td role="rowheader">Description</td>
<td> <p>Type a description for the Portfolio to indicate what is unique about it. </p> </td>
</tr>
<tr>
<td role="rowheader">Portfolio Manager</td>
<td> <p>Start typing the name of a user that you want to indicate as the portfolio manager, then select it when it appears in the list. This is the same as the Portfolio Owner. This is the person who can oversee the work defined in the projects of the portfolio and can approve the Business Case.</p> <note type="important">
When you designate someone as the Portfolio Manager, they automatically gain&nbsp;Manage permissions to the portfolio, the programs and the projects in the portfolio.
</note> </td>
</tr>
<tr>
<td role="rowheader">Group</td>
<td> <p>Add the name of a single group if the group is associated with the portfolio or has responsibility for completing it. </p> </td>
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
</table> </li>
<li value="3"> <p>Click <strong>Save Changes</strong> or continue editing the following sections.</p> </li>
</ol>
<h3><a name="Custom&nbsp;F"></a>Custom&nbsp;Forms</h3>
<ol>
<li value="1"> <p>Begin editing the portfolio as described above. </p> </li>
<li value="2"> <p>Click the <strong>Add Forms</strong> drop-down menu to select a custom forms and add it to the portfolio. </p> <p>You must create portfolio custom forms before they are available to add. </p> <note type="note">
Depending on how your Workfront administrator set the permissions for the sections in your custom form, not everyone can view or edit the same fields on a given custom form. The permissions to edit fields within a section of a custom form depend on the permissions you have on the portfolio itself. For information about setting permissions on sections of a custom form, see
<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.
</note> </li>
<li value="3"> <p>Update any fields in the custom forms, then click <strong>Save Changes</strong> or continue with the following section. </p> </li>
</ol>
<p><strong>Comment</strong></p>
<ol>
<li value="1"> <p>Begin editing a portfolio as described above.</p> </li>
<li value="2"> <p>Click&nbsp;<strong>Comment</strong>. </p> <p> <img src="assets/comment-box-edit-portfolio-classic-350x227.png" style="width: 350;height: 227;"> </p> </li>
<li value="3"> <p>Add a comment in the <strong>Post an update to the portfolio</strong> field.</p> </li>
<li value="4"> <p>(Optional) Click the <strong>People</strong> icon to add a user or a team to the comment. </p> </li>
<li value="5"> <p>(Optional)&nbsp;Click the <strong>Lock</strong> icon to lock the comment and make it private to only users in your company. </p> </li>
</ol>
</div>
-->

