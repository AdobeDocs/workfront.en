---
filename: change-pw-auto-provisioned-user
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
---



# Change the password for an auto-provisioned user {#change-the-password-for-an-auto-provisioned-user}

When you create users through auto provisioning, *`Adobe Workfront`* assigns them a GUID (Globally Unique Identifier) for a user name. A GUID is a unique string of random numbers and letters, for example, *5489cb430012526e1ea635e8c29f377f*. 


Often, when a new user attempts to change their temporary password, they enter their email address for their user name and receive an error for an incorrect user name. In order for the user to change their password, they must enter their system-assigned user name, which is a GUID. 


Because GUID user names can be difficult to use, we recommend you first change a user's user name to their Workfront mail address, then allow them to change their password.


>[!NOTE]
>
>The only way to find a user's GUID is through a query of the Workfront API.




##  

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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span>. For more information, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

{#access-requirements-you-must-have-the-following-to-perform-the-steps-in-this-article-adobe-workfront-plan-any-adobe-workfront-license-plan-access-level-configurations-you-must-be-a-workfront-administrator-for-more-information-see-grant-a-user-full-administrative-access-note-if-you-still-dont-have-access-ask-your-workfront-administrator-if-they-set-additional-restrictions-in-your-access-level-for-information-on-how-a-workfront-administrator-can-modify-your-access-level-see-create-or-modify-custom-access-levels}



## Change the password for an auto-provisioned user {#change-the-password-for-an-auto-provisioned-user-1}




1.  Determine a user's GUID user name by passing an API request, as shown in the following example:
   `<pre><a href="https://domain.my.workfront.com/attask/api/v10/USER/search?fields=Username&ID=">https://<domain>.my.workfront.com/attask/api/v14.0/USER/search?fields=username&ID=<ID of User></a></pre>` Where *<domain>* is your company's domain and *<ID of User>* is the user's *`Workfront`* ID. 


   You receive a response similar to the following:


   ![](assets/getguid-350x105.png)




   The return for "username" is the user's GUID.

1.  Using their GUID as their user name, change the user's password.


   For more information on changing your password, see [Reset your password](reset-your-password.md).


   If your organization uses a SSO system, only a Workfront system administrator can change a user's password. For more information, see [Overview of single sign-on in Adobe Workfront](sso-in-workfront.md)

1.  With the user logged in to Workfront, navigate to:


   https://<your domain>.my.workfront.com/login/convertUsername

1.  In the `Your login email address` box, verify that user's email address is correct, then click `Update Account`.


   ![](assets/guidusername-350x272.png)




   The user's user name is changed to their Workfront email address.




` `**Tip: **`` To find a user's ID:



1.  `<li value="1" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <span class="bold">Main Menu</span> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span>, then click <span class="bold">Users</span> <img src="assets/users-icon-in-main-menu.png">. </li>` `<li value="2"> <p>Select the user.</p> <p>The user's profile page opens and their user ID displays in the URL.</p> </li>` 



