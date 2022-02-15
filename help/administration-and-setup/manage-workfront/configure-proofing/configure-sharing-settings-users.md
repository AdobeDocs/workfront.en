---
filename: configure-sharing-settings-users
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
---



# Configure sharing settings for your users {#configure-sharing-settings-for-your-users}

As an *`Adobe Workfront administrator`* or *`Workfront Proof administrator`*, you can configure the user accounts with which *`proofs`* can be shared, whether users can see all versions of a *`proof`*, and the timing when users gain&nbsp;access to shared items.&nbsp;


## Access requirements {#access-requirements}

You must have the following:

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><a href="https://www.workfront.com/plans" target="_blank"><span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span> plan</a> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"> <p>Any</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><a href="wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p>Work or higher</p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access configurations</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>You must have Administrator selected in your <span class="mc-variable WFVariables.Proof-UC-n variable varname">Proof</span> Permission Profile. For more information, see <a href="configure-a-users-proofing-access.md" class="MCXref xref">Configure a user's proofing access</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## Configure sharing with other accounts&nbsp; {#configure-sharing-with-other-accounts}




1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> From  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click the Main Menu  <img src="assets/main-menu-icon.png">, then click Proofing  <img src="assets/proofing-in-main-menu.png"> to access  <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span>.</MadCap:conditionalText>`   

1. Click `Settings` > `Account settings`, then click the `Settings` tab.

1. In the `Sharing` section, to the right of `Allow sharing with`, click `Setup`.

1. In the drop-down list that appears, select an option to specify whether you want to make *`proofs`* available to anyone, restrict the sharing of your *`proofs`* to your own account only, or restrict it to your own account and any partner accounts you're collaborating with.

1. Click `Save.`




## Configure visibility to all versions of a shared *`proof`* {#configure-visibility-to-all-versions-of-a-shared-proof}




1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> From  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click the Main Menu  <img src="assets/main-menu-icon.png">, then click Proofing  <img src="assets/proofing-in-main-menu.png"> to access  <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span>.</MadCap:conditionalText>`   

1. Click `Settings` > `Account settings`, then click the `Settings` tab.

1. In the `Sharing` section, to the right of `Recipients can view all versions`, select `Enable` or `Disable` to indicate whether you want to allow recipients to view all versions of a *`proof`* within the *`proofing viewer`* when the Proof URL is enabled.





## Configure *`proof`* visibility based on workflow stage activity {#configure-proof-visibility-based-on-workflow-stage-activity}

You can specify when *`proofs`* with an automated workflow are visible to users who are associated with a given stage.


>[!NOTE]
>
>
>
>
>*  This option is available only when using the standalone *`Workfront Proof`* application; it is not available when using a *`Workfront Proof`* instance that is integrated with *`Workfront`* or when *`proofing`* within *`Workfront`*.
>
>* Users receive an email notification about the *`proof`* only after it enters the stage the user is associated with, regardless of this setting.
>
>



To configure when *`proofs`* with an automated workflow are visible to users:



1.  `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> From  <span class="mc-variable WFVariables.ProdNameWF variable varname">Workfront</span>, click the Main Menu  <img src="assets/main-menu-icon.png">, then click Proofing  <img src="assets/proofing-in-main-menu.png"> to access  <span class="mc-variable WFVariables.ProdNameWFP variable varname">Workfront Proof</span>.</MadCap:conditionalText>`   

1. Click `Settings` > `Account settings`, then click the `Settings` tab.

1.  In the  `Sharing` section, enable or disable  `Proof visibility based on stage activation`.

<table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1"> 
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2"> 
 <tbody> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Disabled</span> (default)</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Proofs are visible to users at the time&nbsp;the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> is created.<br><p>Any user associated with a stage in the workflow for the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> can see the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> in search results immediately after the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> is created.</p></td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><span class="bold">Enabled</span> </td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"> <p>Proofs are visible to users only&nbsp;after the stage they are associated with becomes <span class="bold">active.</span></p> <p>Note:  
     <ul> 
      <li><em style="font-style: normal;">After you enable this option, existing <span class="mc-variable WFVariables.proof-plur-n variable varname">proofs</span> are still visible to users who could view it when it was created.</em> </li> 
      <li><em style="font-style: normal;">After a user gains access to a version of a <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span> (because the stage the user is associated with becomes active), the user can see only the version where the stage is activated. If a previous version never reached the stage the user is associated with, the user cannot see that version of the <span class="mc-variable WFVariables.proof-sing-n variable varname">proof</span>.&nbsp;</em> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>




