---
filename: list-access-levels-and-licenses-for-your-users
title: How access levels and permissions work together
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,level,license
navigation-topic: access-levels
---



# List your users’ access levels and licenses {#list-your-users-access-levels-and-licenses}

You can see which access level and license is assigned to each user in a user list or report. 


>[!TIP] {type="tip"}
>
>You can also group the list by license types, or filter it by a specific license.




## Access requirements {#access-requirements}

You must have the following:

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
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"> <p><span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> </p> </td> 
  </tr> 
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray"> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">Access level configurations*</td> 
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray"> <p>View access to users. For more information about access to viewing users, see <a href="grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> <p>Note: If you still don't have access, ask your <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span class="mc-variable WFVariables.AdminWF variable varname">Workfront administrator</span> can modify your access level, see <a href="create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *`Workfront administrator`*.


## List your users’ access levels and licenses {#list-your-users-access-levels-and-licenses-1}




1.   `<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Click the  <span class="bold">Main Menu</span> icon  <img src="assets/main-menu-icon.png"> in the upper-right corner of  <span class="mc-variable WFVariables.FullProdNameWF variable varname">Adobe Workfront</span>, then click <span class="bold"> Users</span>.</MadCap:conditionalText>` 


   By default, all users who are set as Active display in the list.

1.   In the `View` drop-down menu, select `Licenses`.


   The `License` column displays the name of the license assigned to each user.

1.  In the `Grouping` drop-down menu, click `License Type`.


   This view groups together the users who have the same license types.

1. (Optional) To filter the list by a specific license:
    
    
    1. Click the `Filter` drop-down menu, then click `New Filter`.
    
    1. Click `Add a Filter Rule`.
    1. Start typing `License` and select it when it appears in the list.
    1. With the `Equal` modifier selected, start typing the name of the license you want to filter the list by.
    
    
       You can specify more than one license type.
    
    1. Click `Save Filter`.
    
    
       The list displays only the users associated with the license types that you specified in the filter.
    
    
    


