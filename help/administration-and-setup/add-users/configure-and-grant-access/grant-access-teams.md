


# Grant access to teams {#grant-access-to-teams}

The information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment.


As an *`Adobe Workfront administrator`*, you can use an access level to define a user’s access to teams in *`Workfront`*, as explained in [Access levels overview](access-levels-overview.md).


>[!NOTE]
>
>This functionality, releasing with 2022.1, does not change your users' existing access to teams. For more information, see [How users' existing access to teams remains unchanged in the 2022.1 Teams access level setting](#the) in this article.




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



## Configure users’ access to edit users using a custom access level {#configure-users-access-to-edit-users-using-a-custom-access-level}




1. Begin creating or editing the access level, as explained in [Create or modify custom access levels](create-modify-access-levels.md).
1. Click the gear icon ![](assets/gear-icon-settings.png) on the `View` or `Edit` button to the right of *`Teams`*, then select the abilities you want to grant under **Fine-tune your settings**.
    
    
    1. **View**: If you are configuring how users with any license can view teams, change any of the following options:
    
    
    <table style="width: 100%;margin-left: 0;margin-right: auto;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" style="width: 807px;">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">View teams associated with my groups</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">
    <ul>
     <li><p>Enabled: When users look for teams in a Team type-ahead field, the users can see the teams associated with their groups whether or not they are team members. </p></li>
     <li><p>Disabled: When users look for teams in a Team type-ahead field, the users can see the teams associated with their groups only where they are team members</p><p>This option is enabled by default.</p></li>
    </ul></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader"><b>View all teams</b></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"><p>When this option is enabled and users look for teams in a Team type-ahead field, the users can see and select any team.</p><p>This option is enabled by default. </p></td>
  </tr>
 </tbody>
</table>    
    
    
    1. **Edit**: If you are configuring how users with a *`Plan`* license and *`Work`* license can manage teams, change any of the following options:
    
    
    <table style="width: 100%;mc-table-style: url('../../../Resources/TableStyles/TableStyle-List-options-in-steps.css');margin-left: 0;margin-right: auto;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
 <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
 <tbody>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Create</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Allows users with a <span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> license or <span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> license to create teams.</p><p>This option is enabled by default.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Delete</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p> Allows users with a <span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> license to delete the teams that they have access to edit (unavailable for users with a <span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> license).</p><p>This option is enabled by default.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader"><span class="bold">Edit teams in groups I manage (Group Admins only)</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray"><p>Allows <span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> license users who are designated as <span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> to edit teams associated with the groups they manage.</p><p>This option is enabled by default.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader"><span class="bold">Edit teams I'm on</span></td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray"><p>Allows users <span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> license or <span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> license to edit teams where they are a member.</p><p>This option is disabled by default.</p></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">View teams associated with my groups</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">
    <ul>
     <li><p>Enabled: When users<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
         with a 
        <span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> license or 
        <span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> license
       </MadCap:conditionalText> look for teams in a Team type-ahead field, the users can see the teams associated with their groups whether or not they are team members. </p></li>
     <li><p>Disabled: When users<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
         with a 
        <span class="mc-variable WFVariables.WFLicense-Plan variable varname">Plan</span> license or 
        <span class="mc-variable WFVariables.WFLicense-Work variable varname">Work</span> license
       </MadCap:conditionalText> look for teams in a Team type-ahead field, the users can see the teams associated with their groups only where they are team members</p><p data-mc-conditions="SnippetConditions.HIDE">Also, when this option is disabled, <b>View all teams</b> is automatically disabled along with it.</p><p>This option is enabled by default.</p></li>
    </ul></td>
  </tr>
  <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">View all teams</td>
   <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray"><p>When this option is enabled and users look for teams in a Team type-ahead field, the users can see and select any team.</p><p data-mc-conditions="SnippetConditions.HIDE">Also, when it is enabled, <b>View teams associated with my groups</b> is automatically enabled along with it. </p><p>This option is enabled by default. </p></td>
  </tr>
 </tbody>
</table>    
    
    
    
    

1.  Click the X to close the `Fine-tune your settings` box.
1.  (Optional) To configure access settings for other objects and areas in the access level you are working on, continue with one of the articles listed in [Configure access to Adobe Workfront](_configure-access.md), such as [Grant access to tasks](grant-access-tasks.md) and [Grant access to financial data](grant-access-financial.md).
1. When you are finished, click **Save**.




>[!NOTE]
>
>
>
>
>*  The following are true, regardless of access level settings:
>
>    
>    
>    *  Team owners can always view and edit their teams
>    *  Users always have access to view the teams they’re on
>    
>    
>
>*  The configuration of any option available for both View and Edit (such as "View teams associated with my groups") is retained if you decide to select View instead of Edit or Edit instead of View in an access level.
>
>





## Access to teams by license type {#access-to-teams-by-license-type}

This table lists what a *`Workfront administrator`* can allow users with each license type to do with *`teams`*. For information about the *`Workfront`* license types, see [Adobe Workfront licenses overview](wf-licenses.md).


External users don't have access to teams.

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
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">Edit teams associated with groups they manage (<span class="mc-variable WFVariables.AdminGroup-plur variable varname">group administrators</span> only)</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray"> <p>Edit teams they're on</p> </td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray">&nbsp;</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">&nbsp;</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">View teams associated with their groups</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">✓</td> 
  </tr> 
  <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray"> 
   <td scope="row" class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">View all teams</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray">✓</td> 
   <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">✓</td> 
  </tr> 
 </tbody> 
</table>



## How users' existing access to teams remains unchanged in the 2022.1 Teams access level setting {#how-users-existing-access-to-teams-remains-unchanged-in-the-teams-access-level-setting}

In an access level, when you click the gear icon ![](assets/gear-icon-in-access-levels.png) on the View or Edit button for the new Teams setting, the options "View all teams" and "View teams associated with my groups," are:



*  Disabled if "View only companies, groups & teams they belong to" was enabled previously under "Set additional restrictions." 
*  Enabled if "View only companies, groups & teams they belong to" was *not* enabled previously under "Set additional restrictions." 



` `**Tip: **`` To view the restriction "View only companies, groups & teams they belong to," click **Set additional restrictions** at the bottom of the Edit Access Level box.


With the addition of the Teams feature in access levels, this restriction is renamed "View only companies & groups they belong to."
