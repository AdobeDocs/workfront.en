---
filename: delete-a-user
title: Delete a user
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
---



# Delete users {#delete-users}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


>[!IMPORTANT] {type="important"}
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Adobe Business Platform. If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.
>
>
>For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](actions-in-admin-console.md).



When a user leaves your organization, can remove that user from *`Adobe Workfront`*.


>[!IMPORTANT] {type="important"}
>
>Deleting a user from the system also deletes information associated with the user that you might want to retain. We recommend deactivating users instead of deleting them. For more information, see [Deactivate a user](deactivate-a-user.md).




## Access requirements {#access-requirements}

You must have the following to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level. For information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p><b>Users</b> setting in your access level configured to <b>Edit</b> access, with <b>Create</b> and at least one of the two <b>User Admin</b> options enabled under <b>Fine-tune your settings </b><img src="assets/gear-icon-in-access-levels.png">. </p> <p>Of these two options, if User <b>Admin (Group Users)</b> is enabled, you must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of a group where the user is a member.</p> <p>For more information about the <b>Users</b> setting in an access level, see <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Deleting vs. deactivating a user {#deleting-vs-deactivating-a-user}

Deactivating a user causes the following things to happen:



* Removes the user's licenses to both *`Workfront`* and *`Workfront Proof`* if the *`Workfront Proof`* component is associated with your *`Workfront`* account. For more information about *`Workfront Proof`*, see [Workfront Proof](_workfront-proof.md).&nbsp;

* The user can no longer be assigned work.
* The user can no longer be added to updates.
* The user can no longer be added to teams or groups.
* Objects can no longer be shared with the user.
* Their association with the following objects remains intact:
*  `<li>Tasks, issues, projects, portfolios</li>` `<li> <p>Dashboards</p> <note type="note">  If you deactivate a user and can no longer view the reports or dashboards associated with a user, you may need to update the   <span class="bold">Run this report with the Access Rights of:</span> field.  <br>To learn more, see the   <a href="reports-faq.md#why" class="MCXref xref">Why can't I access a report owned by a deactivated user?</a> section of the   <a href="reports-faq.md" class="MCXref xref">Reports FAQs</a> article. </note> </li>` `<li>Documents</li>` `<li>Updates</li>` `<li>Hours</li>` 

* If the user has checked-out documents, the documents remain checked out when you deactivate them. Only a *`Workfront administrator`* can check them back in.For more information about checking out documents, see [Check out documents](check-out-documents.md).



Deleting a user causes the following things to happen:



* Removes the user's licenses to both *`Workfront`* and *`Workfront Proof`*, if the *`Workfront Proof`* component is associated with your *`Workfront`* account. For more information about *`Workfront Proof`*, see [Workfront Proof](_workfront-proof.md)

* The user can no longer be assigned work.
* The user can no longer be added to updates.
* The user can no longer be added to teams or groups.
* Objects can no longer be shared with the user.
* Deletes the association of that user with the following objects:
*  `<li>Tasks, issues, projects, portfolio</li>` `<li> <p>Dashboards</p> <note type="note">  You also lose access to custom   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">   sections  </MadCap:conditionalText> that contained dashboards associated to the deleted user.  <br>To learn more, see the   <a href="reports-faq.md#how" class="MCXref xref">How do I access a dashboard that contains a report owned by a deleted user?</a> section of the   <a href="reports-faq.md" class="MCXref xref">Reports FAQs</a> article. </note> </li>` `<li>Updates</li>` `<li> <p>Hours</p> <note type="note">   These objects remain in   <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> but the owner of the object is now blank. </note> </li>` 

* If the user uploaded any documents under the Documents area in the Global Navigation Bar, the documents are&nbsp; also deleted.
* If the user has checked out documents that they own and the documents are uploaded in the main Documents area (accessed from the `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>`), the documents are deleted with the user. For more information about checking out documents, see [Check out documents](check-out-documents.md).



For more information about deactivating users, see [Deactivate a user](deactivate-a-user.md).


You can permanently delete users one at a time, or you can permanently delete multiple users simultaneously. When you delete individual users, you must wait for the deletion process to complete prior to moving on to other activities in *`Workfront`*. The process of deleting multiple users simultaneously runs as a background process, so you can continue using *`Workfront`* as the users are deleted.


## Delete one or more users {#delete-one-or-more-users}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*.

1. Click `Users`.
1.  If you are using the Production environment, select the user you want to delete, click **More**, then click **Delete**.


   Or


   If you are using the Preview environment, select the user you want to delete, click the More `menu icon ![](assets/more-icon.png)

   `, then click **Delete**.

1.  In the box that appears, click `Delete Anyway` to confirm the deletion.


   The process of deleting users runs as a background process, so you can continue using *`Workfront`* as the user or users are deleted. 


   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.


   After receiving the confirmation in *`Workfront`* that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.


   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.



