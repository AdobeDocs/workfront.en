---
filename: manage-company-memberships
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
---



# Manage company memberships {#manage-company-memberships}

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


In the Companies area in Setup, you can add and remove a company's members. You can also edit their user profiles, remind them to register in Workfront, deactivate them in *`Workfront`*, and remove them from the *`Workfront`* system. 


## Access requirements {#access-requirements}

You must have the following in order to manage companies in *`Workfront`*:

<table class="TableStyle-TableStyle-List-options-in-steps" style="margin-left: 0;margin-right: auto;caption-side: bottom;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" data-mc-conditions=""> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" data-mc-conditions=""> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"> <p>Workfront plan*</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><span class="mc-variable WFVariables.WFPlan-Team variable varname">Team</span> or higher</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"> <p><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</p> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader"><span class="bold">Access level*</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>In order to manage companies, you must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level, which allows you to edit any company in the system. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p>Administrative access to manage companies, which allows you to edit any company in the system. For more information, see <a href="grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </li> 
    </ul> <p>Note: You can also manage companies associated with any group where you are assigned as a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span>.</p> 
    <div data-mc-conditions="SnippetConditions.HIDE"> 
     <p>In order to add to and remove users from the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> system, you must have one of the following:</p> 
     <ul> 
      <li> <p>The System Administrator access level. For information about this access level, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
      <li> <p>In your access level, Edit must be selected for the Users setting. And, for the Users setting, under Fine-tune your settings <img src="assets/gear-icon-in-access-levels.png"> , the Create option and at least one of the two User Admin options must be enabled. </p> <p>If you are using the User Admin (Group Users) option, you must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of a group where the user is a member.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>For information about the Users setting in an access level, see <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
     </ul> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your *`Workfront administrator`*.


## Manage company memberships {#manage-company-memberships-1}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1.  Click `Companies`.
1.  Click the name of the company.
1.  With the **Company Members** section selected in the left panel, do any of the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" style="width: 135px;"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Add a member</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Do one of the following:</p> 
    <ul> 
     <li> <p>If you are using the Production environment, add a person who has not yet been added to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> by clicking <b>New Person</b>, then entering information about the user.</p> <p>For information about adding users to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, see <a href="add-users.md" class="MCXref xref">Add users</a> and <a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
     <li class="preview"> <p>If you are using the Preview environment, click <b>Add member</b>, then select one of these options in the drop-down menu that displays:</p> 
      <ul> 
       <li> <p><b>New user</b>: Add a user who has not yet been added to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>. </p> <p>For information about adding users to <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, see <a href="add-users.md" class="MCXref xref">Add users</a> and <a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
       <li> <p><b>Existing user</b>: Add a user already, existing in the system, that you have access to edit.</p> <p>Important: If the user is already a member of another company, the new assignment overrides the old one. The user loses access to items shared with the previous company and gains access to items shared with this company.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Edit members</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> 
    <ol> 
     <li value="1"> <p>Select at least one user, then do one of the following.</p> 
      <ul> 
       <li> <p>If you are using the Production environment, click <b>Edit</b> in the toolbar.</p> </li> 
       <li> <p><span class="preview">If you are using the Preview environment, click the Edit icon <img src="assets/edit-icon.png"> in the toolbar.</span> </p> </li> 
      </ul> </li> 
     <li value="2"> <p>Configure the options in the <b>Edit Person</b> box that displays. For information about these options, see <a href="edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Remove users</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> 
    <div> 
     <p>Select at least one user, then do one of the following:</p> 
     <ul> 
      <li>If you are using the Production environment, click the More menu icon<img src="assets/more-icon.png">, then click <b>Delete</b>.</li> 
      <li> <p class="preview">If you are using the Preview environment, click <b>Remove users</b>, then select one of the following options in the drop-down menu that displays:
        <ul>
         <li><b>Remove from company</b>: Removes the user or users from the company.</li>
         <li><b>Delete</b>: Deletes the user or users from the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> system.</li>
        </ul></p> </li> 
     </ul> 
    </div> <p>Important: Deleting a user from the system also deletes information associated with the user that you might want to retain. We recommend deactivating users instead of deleting them. For more information, see <a href="deactivate-a-user.md" class="MCXref xref">Deactivate a user</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Send a comment to users and to their Updates areas</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select at least one user, then do one of the following:</p> 
    <ul> 
     <li> <p>If you are using the Production environment, click <b>Update</b> in the toolbar. </p> </li> 
     <li> <p><span class="preview">If you are using the Preview environment, click the Comment icon <img src="assets/comment-icon.png"> in the toolbar.</span> </p> </li> 
    </ul> <p>Type the comment you want to send to the users and to the Updates area of their user profiles.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Export the list of company members</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>If you are using the Production environment, click <b>Export</b> in the toolbar, then select the format you want for the exported file.</p> <p><span class="preview">Or, if you are using the Preview environment, click the Export icon <img src="assets/export.png"> in the toolbar, then select the format you want for the exported file.</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Deactivate members in the system</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Select at least one user, then do one of the following:</p> 
    <ul> 
     <li> <p>If you are using the Production environment, click <b>More</b> in the toolbar, then select <b>Deactivate</b>. </p> </li> 
    </ul> 
    <ul> 
     <li class="preview"> <p>If you're using the Preview environment, click the More icon <img src="assets/more-icon.png"> in the toolbar, then select <b>Deactivate</b>. </p> </li> 
    </ul> <p>For more information, see <a href="deactivate-a-user.md" class="MCXref xref">Deactivate a user</a>.</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray" data-mc-conditions=""> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Remind a user to register in the system</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p> In the <b>Name</b> column, <b>Unregistered</b> displays next to the name of each unregistered user. To remind these users to register in the system, select them, click <b>More</b> in the toolbar, then select <b>Send&nbsp;Invitations</b>. and do one of the following:</p> 
    <ul> 
     <li> <p>If you are using the Production environment, click <b>More</b> in the toolbar, then select <b>Send Invitations</b>. </p> </li> 
     <li> <p><span class="preview">If you're using the Preview environment, click the More icon <img src="assets/more-icon.png"> in the toolbar, then select </span><b class="preview">Remind user to register</b><span class="preview">.</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>




