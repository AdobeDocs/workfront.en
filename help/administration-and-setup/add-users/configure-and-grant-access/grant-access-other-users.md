


# Grant access to users {#grant-access-to-users}

As an *`Adobe Workfront administrator`*, you can use an access level to define a user’s access to other users in *`Workfront`*, as explained in [Access levels overview](access-levels-overview.md).


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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



## Configuring access to users {#configuring-access-to-users}

You can manage what information users can view and edit for other users using a default access level or a custom access level that you create. Users with the default *`Plan`* and *`Work`* licenses can view the contact information of other users. Any of the following users can create and edit other users:



*  A *`Workfront administrator`*.


  For more information, see [Grant a user full administrative access](grant-a-user-full-administrative-access.md).

*  A user with a default *`Plan`* license who also has access to users, as explained in this article.


  Users that are restricted to see only users from their company or the primary company have access to edit only the users they can see. For more information, see [Create or modify custom access levels](create-modify-access-levels.md).

*  A user with a default *`Plan`* license who is also specified as the manager of another user.


  Users who are granted Edit access to users in their access level can manage users who report to them. For information about managing a user, see [View the organizational chart](view-the-org-chart.md).

*  A user with a default *`Plan`* license who created a user can deactivate, delete, or edit the user they created. For information about creating new users, see [Add users](add-users.md).




## Configure users’ access to edit users using a custom access level {#configure-users-access-to-edit-users-using-a-custom-access-level}




1. Begin creating or editing the access level, as explained in [Create or modify custom access levels](create-modify-access-levels.md).
1. To change the ability of users with a *`Plan`* or *`Work`* license to view the profiles of other users:
    
    
    1. Click the gear icon ![](assets/gear-icon-settings.png) on the `View` button to the right of `Users`.
    
    1. Disable `View Contact info`, then click the X to close the `Fine-tune your settings` box.
    
    
    

1.  To modify the ability of users with a *`Plan`* license access to edit other users, click the gear icon ![](assets/gear-icon-settings.png) on the `Edit` button to the right of `Users`, then select the abilities you want to grant:

<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Create</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Allows users to create users.<br>This option is enabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Delete</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> Allows users to delete the users they have created themselves.<br>This option is enabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">User Admin (All Users)</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Allows users to do the following for any user in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>:</p> 
    <ul> 
     <li>Edit, delete, or deactivate the user</li> 
     <li>Log in as the user</li> 
     <li>Reset the user's password</li> 
    </ul> <p>This option is disabled by default.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">User Admin (Group Users)</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Allows users to do the following for any user in a group they administer: 
     <ul>
      <li><p>Edit, delete, or deactivate the user</p></li>
      <li>Log in as the user</li>
      <li><p>Reset the user's password</p><p>Note:  A <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> cannot log in as or reset the password of a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>.<br></p></li>
     </ul><p>This option is disabled by default.</p></p> </td> 
  </tr> 
 </tbody> 
</table>


   ` `**Tip: **`` If you don’t want to grant *`group administrators`* access to all members of the groups they administer, disable both of the User Admin options above. *`Group administrators`* will still be able to access group members whom they add to *`Workfront`*, or who report to them in *`Workfront`*.

1.  (Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in [Configure access to Adobe Workfront](_configure-access.md), such as [Grant access to tasks](grant-access-tasks.md) and [Grant access to financial data](grant-access-financial.md).
1. When you are finished, click **Save**.




## Access to users by license type {#access-to-users-by-license-type}

This table lists what a *`Workfront administrator`* can allow users with each license type to do with *`users`*. For information about the *`Workfront`* license types, see [Adobe Workfront licenses overview](wf-licenses.md).


External users are not included here because they can only search for users.

<table style="mc-table-style: url('../../../Resources/TableStyles/TableStyle-HeaderRow.css');margin-left: 0;margin-right: auto;width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <col class="TableStyle-TableStyle-HeaderRow-Column-Column1"> 
 <thead> 
  <tr class="TableStyle-TableStyle-HeaderRow-Head-Header1"> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p>Action</p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p>Plan</p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1">Work</th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadE-Column1-Header1"> <p>Review</p> </th> 
   <th class="TableStyle-TableStyle-HeaderRow-HeadD-Column1-Header1"> <p>Request</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Create</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Delete</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>Edit</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>User Admin<br>(All Users)</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray"> <p>User Admin<br>(Group Users)</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>View User</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">View Contact Info</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray"> ✓&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray">&nbsp;✓ </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray"> ✓&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

