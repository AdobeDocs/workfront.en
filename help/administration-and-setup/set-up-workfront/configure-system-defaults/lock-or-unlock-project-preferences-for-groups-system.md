---
filename: lock-or-unlock-project-preferences-for-groups-system
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
---



# Lock or unlock project preferences for all groups in the system {#lock-or-unlock-project-preferences-for-all-groups-in-the-system}

Groups in your organization might need a project preference configured differently for their unique workf lows. You can unlock the preference for all groups throughout the organization so that they can configure it on their own.


When a preference is unlocked and the *`group administrator`* modifies it, the projects associated with the group acquire the configuration for that preference from the group-level setting instead of from the system-level setting.


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



## About locked and unlocked preferences {#about-locked-and-unlocked-preferences}

Locking a project, task, or issue preference that you have configured at the`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level">  system</MadCap:conditionalText>` level ensures that everyone`<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level">  throughout the system</MadCap:conditionalText>` is using the same setting for that preference. Though you can still reconfigure a preference that you lock, *`group administrators`* can’t reconfigure it for `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level"> their</MadCap:conditionalText>` groups.


Conversely, unlocking a project, task, or issue preference allows *`group administrators`* more flexibility to manage the way their groups work with those items. When a preference is unlocked, *`group administrators`* can reconfigure it for `<MadCap:conditionalText data-mc-conditions="SnippetConditions-wf-groups.system-level"> their groups</MadCap:conditionalText>`.


For instructions on locking or unlocking a system-level project, task, or issue preference, see [Lock or unlock project preferences for all groups in the system](#) or this one needs to be broken out on it's own also: [Configure system-wide task and issue preferences](set-task-issue-preferences.md).


>[!NOTE]
>
>After a *`Workfront administrator`* unlocks a preference at the system level, any *`group administrator`* can configure it and then lock it to ensure that everyone in their group and the subgroups below is using the same configuration. This is parallel to the ability that a *`Workfront administrator`* has to configure and lock a preference for everyone in the system. For more information, see [Configure project preferences for a group](configure-project-preferences-group.md) and [Lock or unlock a project, task, or issue preference for subgroups](lock-or-unlock-a-group-preference.md).




## Unlock a project preference so that groups can configure it {#unlock-a-project-preference-so-that-groups-can-configure-it}




1. Click the `Main Menu` icon ![](assets/main-menu-icon.png) in the upper-right corner of *`Adobe Workfront`*, then click `Setup` ![](assets/gear-icon-settings.png).

1. Click `Project Preferences`, then click `Projects`.

1.  Do any of the following:

    
    
    * If you want *`group administrators`* to be able to configure a preference for their groups, unlock it ![](assets/unlock-toggle-button.png).
    
    * If you want all groups to use your configuration for a preference, make sure that it is locked (this is the default).    
    
      >[!IMPORTANT] {type="important"}
      >
      >We recommend that you communicate with the administrators and users in groups throughout the system to ensure that all needs are accounted for in the way you configure a locked preference. When you lock it, your configuration for it is inherited by all groups in the system. And if the preference has been unlocked for any period of time, your configuration replaces those that *`group administrators`* might have made.
    
    
    
    

1. Click `Save`.


