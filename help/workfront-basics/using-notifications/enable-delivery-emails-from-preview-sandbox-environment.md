---
filename: enable-delivery-emails-from-preview-sandbox-environment
navigation-topic: notifications
---



# Enable delivery of emails from the Preview Sandbox environment {#enable-delivery-of-emails-from-the-preview-sandbox-environment}

*`Adobe Workfront`* disables all email communication from both the Preview and the Custom Refresh Sandbox environments. For information about the Preview Sandbox environment, see [The Adobe Workfront Preview Sandbox Environment](wf-preview-sandbox-environment.md). For information about the Custom Refresh Sandbox environment, see [The Adobe Workfront Custom Refresh Sandbox environment](wf-custom-refresh-sandbox-environment.md).


If you want to receive the following email notifications from the Preview Sandbox environment, you must enable this functionality in your user settings while you are logged into Preview:



* Email notifications triggered by event notifications
* Reminder notifications
* Automatic late or early reminder notifications
* Email invitations


You can do this for yourself or for any user that you have access to edit. For more information about the access needed to edit users, see [Grant access to users](grant-access-other-users.md).


>[!NOTE]
>
>Report delivery and push notifications on the mobile app are always disabled for the Preview Sandbox environment. Neither you nor the *`Workfront administrator`* can enable report delivery or push notifications for the mobile app when you access the Preview Sandbox environment.
>
>
>For information about report deliveries, see [Report delivery overview](set-up-report-deliveries.md).





## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 </col> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 </col> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Request variable varname">Request</span> or higher to change your own setting</p> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> to edit the setting for other users</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must have one of the following:</p> 
    <ul> 
     <li> <p>The System Administrator access level.</p> <p> For information about this access level, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>. </p> </li> 
     <li> <p>In your access level, Edit must be selected for the Users setting. And, for the Users setting, under Fine-tune your settings <img src="assets/gear-icon-in-access-levels.png"> , the Create option and at least one of the two User Admin options must be enabled. </p> <p>If you are using the User Admin (Group Users) option, you must be a <span class="mc-variable WFVariables.AdminGroup variable varname">group administrator</span> of a group where the user is a member.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>For information about the Users setting in an access level, see <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
    </ul> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Enable the delivery of emails from the Preview Sandbox environment {#enable-the-delivery-of-emails-from-the-preview-sandbox-environment}




1. Log in to your Preview Sandbox environment.
1.  Click your profile picture in the upper-right corner of *`Workfront`*. `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Then, click the  <span class="bold">More</span> menu and select  <span class="bold">Edit</span>. </MadCap:conditionalText>`


   Or


   Search for a user in *`Workfront`* and click their name. `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Then, click the  <span class="bold">More</span> menu and select  <span class="bold">Edit</span>. </MadCap:conditionalText>`


   Or


   For multiple users, `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> and select  <span class="bold">Users</span> <img src="assets/users-icon-in-main-menu.png">,</MadCap:conditionalText>` select multiple users, then click `Edit`.

1. Click `Preferences`.
1.  Select `Receive emails from this test environment`.


   >[!NOTE]
   >
   >This option is not available if you are in a production environment.



1. Click `Save Changes`.


