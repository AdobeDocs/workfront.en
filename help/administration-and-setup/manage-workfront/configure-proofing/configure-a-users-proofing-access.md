---
filename: configure-a-users-proofing-access
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
---



# Configure a user's *`proofing`* access {#configure-a-users-proofing-access}

As a *`Adobe Workfront administrator`* or *`Workfront Proof administrator`*, you can configure a user's access to create and view *`proofs`* in *`Workfront`* and *`Workfront Proof`*.


For information about *`proofing`* functionality available for basic and integrated *`proofing`*, see [Access to proofing functionality in Workfront](access-to-proofing-functionality.md).


## Access requirements {#access-requirements}

You must have the following access to perform the steps in this article:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> license*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Plan</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must be a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> or <span class="mc-variable WFVariables.FullProdNameAdminWFP variable varname">Workfront Proof administrator</span>. For information on <span class="mc-variable WFVariables.AdminWF-plur variable varname">Workfront administrators</span>, see <a href="grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Enable and disable *`proofing`* for&nbsp;a user (legacy plans only) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

If your organization is using a legacy Select or Premium Workfront Plan, as a *`Workfront administrator`*, you can enable and disable *`proofing`* functionality for the user.


When you enable *`proofing`* for a user, *`Workfront`* enables the option for the user's *`proofs`* to generate automatically. For more information about this option and how to disable it, see [Configure a user's proofing access](#).&nbsp;


Though you can enable a user as a *`proofing`* user, he or she must have Administrator permissions in order to navigate directly to the *`Workfront Proof`* interface from the *`Workfront`* `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>`. For information about how you can enable this option for all *`proofing`* users in your *`Workfront`* system, see [Configure Workfront Proof access via Workfront Main Menu for all users](#configuring-whether-all-users-can-access-proofhq-directly-from-the-workfront-global-nav).



1. In the `Main Menu`, select `Users`.

1. Select a user, then click the `Edit`icon.
1. In the `Access` section, select or deselect `User can generate proofs`.





## Configure a user's *`proof`* permission profile {#configure-a-users-proof-permission-profile}

The permission profile you select is granted to the users for each *`proof`* that exists within your organization.



1.  Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Users` ![](assets/users-icon-in-main-menu.png). 
1.  Select one or more users, then click `Edit`.  

1.  In the `Access`section, click one of the following *`Workfront Proof`* permission options in the `Proof Permission Profile`&nbsp;drop-down menu:


   >[!NOTE]
   >
   >If you are on a legacy Workfront plan, make sure the `User can generate proofs` option is enabled, as explained above in the section [Enable and disable proofing for a user (legacy plans only)](#enabling-and-disabling-proofing-for-a-user).&nbsp;



<table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Supervisor</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Users can manage and view all <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> created on your organization's account. They can also edit reviewers added to these <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span>. Users with this permission profile can't manage users or edit <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span> settings.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Manager</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p> Users can manage and view <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> created or owned on your organization's account. They can view other users' <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> only when added as a reviewer. This is a default setting. </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Administrator</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> Users are given Administrator permissions in <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span> and can edit account settings. Users can manage and view all <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> created on your organization's account. This includes adding and removing reviewers, <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span>, and comments.</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">Custom</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Available only if you have configured a custom permission profile within <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span>.</p> <p>Note:  <p>Ensure that the permission profile you grant here does not provide higher access than the user's&nbsp;Access Level&nbsp;setting in <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> (see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>). If it does provide higher&nbsp;access, the user can access <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> within <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span> that he or she cannot access within <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>.</p> <p>This is especially important if you plan to allow all <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> users to access <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span> directly from the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> as described in&nbsp;<a href="access-wf-proof-in-workfront.md" class="MCXref xref">Access Workfront Proof from Adobe Workfront</a>.</p> <p>By default, only <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> administrators have access to a direct link to the <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span> site from the <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span> Global Navigation Bar.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

   The permission profile you select is granted to the users for each *`proof`* that exists within your organization.

1.  Click `Save Changes`&nbsp;to complete the update to the user settings.


   >[!NOTE]
   >
   >When you create or update a user in *`Workfront`* and the user's *`Workfront`* email address matches that of a licensed *`Workfront Proof`* user, the system enables *`proofing`* for the user within *`Workfront`*.&nbsp;For more information, see [User synchronization between Adobe Workfront and Workfront Proof](user-sync-proofing.md).







### Considerations {#considerations}

Consider the following information when setting permissions:



*  If you change a user's permission profile to a profile with fewer permissions, the user might lose visibility to existing *`proofs`* within *`Workfront`*. This can occur when someone shares a task with a user within *`Workfront`*, but doesn't share the *`proof`* attached to the task (see&nbsp; [Share a proof within Adobe Workfront](share-a-proof-in-workfront.md)&nbsp;in [Share a proof within Adobe Workfront](share-a-proof-in-workfront.md)).
*  You can set *`Workfront Proof`* permissions from *`Workfront`* only if your *`Workfront`* environment is integrated with a *`Workfront Proof`* Premium account. If you cannot use *`proofing`* as discussed in this section, contact your *`Workfront administrator`*.
*  At least one user in your *`Workfront`* environment must have Administrator permissions for  *`proofing`*. An error message appears if you try to attempt to remove Administrator permissions for *`proofing`* from all users.
*  When you change a user's *`Workfront`* Access level to any level other than System Administrator, the user's *`Workfront Proof`* permission profile defaults to Manager.   

*  When you change the *`Workfront`* Access level to System Administrator, the Proof Permission profile changes to Administrator.




## Configure *`Workfront Proof`* access via *`Workfront`* `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>` for all users {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

By default, only users with administrative rights within *`Workfront`* can access *`Workfront Proof`* as described&nbsp; [Access Workfront Proof from Adobe Workfront](access-wf-proof-in-workfront.md).


You can grant all users access to the *`Workfront Proof`* button within the *`Workfront`* `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Main Menu</MadCap:conditionalText>` by contacting *`Workfront`* Support and submitting a request.


>[!IMPORTANT] {type="important"}
>
>If you plan to allow all *`Workfront`* users to access *`Workfront Proof`* directly from the *`Workfront`* Global Navigation Bar, ensure that the permission profile for each user does not provide more access than the user's access level within *`Workfront`*. This prevents users from accessing *`proofs`* within *`Workfront Proof`* that they cannot access within *`Workfront`*. For more information, see [Enable and disable proofing for a user (legacy plans only)](#enabling-and-disabling-proofing-for-a-user).




## Configure user access to the *`Desktop Proofing Viewer`* {#configure-user-access-to-the-desktop-proofing-viewer}

If the users in your organization would prefer to use the *`Desktop Proofing Viewer`* instead of the *`Web Proofing Viewer`* to review interactive content, you can configure the *`Desktop Proofing Viewer`* to launch automatically when users open interactive content proofs. For information about this the *`Desktop Proofing Viewer`* and how it differs from the *`Web Proofing Viewer`*, see [Understand the Desktop Proofing Viewer](destop-proofing-viewer.md) and [Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview](understand-differences-between-web-viewer.md).



1.  From *`Workfront`*, click the *`Workfront Proof`* icon in the Global Navigation Bar to access *`Workfront`* Proof.


   ![](assets/proof-access-proofhq-350x39.png)








1. Click `Account settings` near the upper-right corner of *`Workfront Proof`*, then click the `Settings` tab.

1. Under `Proof Defaults`, at the end of the ` *`Desktop Proofing Viewer`* for Interactive *`proofing`*` row, click `Setup`.

1. Modify the *`Desktop Proofing Viewer`* settings, as described in [Desktop Proofing Viewer](configure-proofing-organization.md#desktop-proofing-viewer) in the article [Configure proof settings for your organization](configure-proofing-organization.md).

1. Click `Save`.




## Configure custom devices for interactive proofs {#configure-custom-devices-for-interactive-proofs}

You can add any custom devices to your system, allowing users to review interactive content and simulate how the content appears on a specific device when they are using the *`Desktop Proofing Viewer`*. (This functionality is not available in the *`Web Proofing Viewer`*, where users can review&nbsp;interactive content, but only as it appears in various resolutions, not on various devices.) 


For more information, see [Change interactive proof resolution in the proofing viewer](view-interactive-content-as-it-appears-in-device.md).



1. From *`Workfront`*, access the *`Workfront Proof`* interface, as described in [Access Workfront Proof from Adobe Workfront](access-wf-proof-in-workfront.md).

1. Modify the *`Desktop Proofing Viewer`* settings, as described in [Configure custom devices for proofs](configure-proofing-organization.md#custom-devices-for-proofs) in the article [Configure proof settings for your organization](configure-proofing-organization.md). `  
   `



